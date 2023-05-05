# Comparing `tmp/simulariumio-1.7.1.tar.gz` & `tmp/simulariumio-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulariumio-1.7.1.tar", last modified: Mon Feb 20 18:01:43 2023, max compression
+gzip compressed data, was "simulariumio-1.8.0.tar", last modified: Fri May  5 21:05:48 2023, max compression
```

## Comparing `simulariumio-1.7.1.tar` & `simulariumio-1.8.0.tar`

### file list

```diff
@@ -1,319 +1,327 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.764880 simulariumio-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-02-20 18:01:28.000000 simulariumio-1.7.1/.cookiecutter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-20 18:01:28.000000 simulariumio-1.7.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.688876 simulariumio-1.7.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-20 18:01:28.000000 simulariumio-1.7.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.688876 simulariumio-1.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-02-20 18:01:28.000000 simulariumio-1.7.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-20 18:01:28.000000 simulariumio-1.7.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-20 18:01:28.000000 simulariumio-1.7.1/.github/ISSUE_TEMPLATE/maintenance_task.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-02-20 18:01:28.000000 simulariumio-1.7.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-20 18:01:28.000000 simulariumio-1.7.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.688876 simulariumio-1.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-02-20 18:01:28.000000 simulariumio-1.7.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-20 18:01:28.000000 simulariumio-1.7.1/.github/workflows/create-issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-02-20 18:01:28.000000 simulariumio-1.7.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-02-20 18:01:28.000000 simulariumio-1.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-20 18:01:28.000000 simulariumio-1.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-02-20 18:01:28.000000 simulariumio-1.7.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-02-20 18:01:28.000000 simulariumio-1.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-02-20 18:01:28.000000 simulariumio-1.7.1/Justfile
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-02-20 18:01:28.000000 simulariumio-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-02-20 18:01:43.764880 simulariumio-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-02-20 18:01:28.000000 simulariumio-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.692876 simulariumio-1.7.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-02-20 18:01:28.000000 simulariumio-1.7.1/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-20 18:01:28.000000 simulariumio-1.7.1/benchmarks/TEST_RESOURCES_HASH.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-02-20 18:01:28.000000 simulariumio-1.7.1/benchmarks/benchmark_simulariumio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-02-20 18:01:28.000000 simulariumio-1.7.1/benchmarks/download_benchmark_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-02-20 18:01:28.000000 simulariumio-1.7.1/benchmarks/upload_benchmark_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.692876 simulariumio-1.7.1/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5362 2023-02-20 18:01:28.000000 simulariumio-1.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-20 18:01:28.000000 simulariumio-1.7.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-20 18:01:28.000000 simulariumio-1.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-02-20 18:01:28.000000 simulariumio-1.7.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-20 18:01:28.000000 simulariumio-1.7.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-20 18:01:28.000000 simulariumio-1.7.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.692876 simulariumio-1.7.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-02-20 18:01:28.000000 simulariumio-1.7.1/examples/Tutorial_cellpack.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-02-20 18:01:28.000000 simulariumio-1.7.1/examples/Tutorial_custom.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-02-20 18:01:28.000000 simulariumio-1.7.1/examples/Tutorial_cytosim.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-02-20 18:01:28.000000 simulariumio-1.7.1/examples/Tutorial_filters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-02-20 18:01:28.000000 simulariumio-1.7.1/examples/Tutorial_mcell.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-02-20 18:01:28.000000 simulariumio-1.7.1/examples/Tutorial_md.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-02-20 18:01:28.000000 simulariumio-1.7.1/examples/Tutorial_medyan.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-02-20 18:01:28.000000 simulariumio-1.7.1/examples/Tutorial_physicell.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-02-20 18:01:28.000000 simulariumio-1.7.1/examples/Tutorial_plots.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-02-20 18:01:28.000000 simulariumio-1.7.1/examples/Tutorial_readdy.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-02-20 18:01:28.000000 simulariumio-1.7.1/examples/Tutorial_smoldyn.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-02-20 18:01:28.000000 simulariumio-1.7.1/examples/Tutorial_springsalad.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-20 18:01:28.000000 simulariumio-1.7.1/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.692876 simulariumio-1.7.1/examples/img/
--rw-r--r--   0 runner    (1001) docker     (123)  3109823 2023-02-20 18:01:28.000000 simulariumio-1.7.1/examples/img/drag_drop.gif
--rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-02-20 18:01:28.000000 simulariumio-1.7.1/file_format.md
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-02-20 18:01:28.000000 simulariumio-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 18:01:43.764880 simulariumio-1.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.700877 simulariumio-1.7.1/simulariumio/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.700877 simulariumio-1.7.1/simulariumio/cellpack/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/cellpack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/cellpack/cellpack_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/cellpack/cellpack_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.700877 simulariumio-1.7.1/simulariumio/cytosim/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/cytosim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/cytosim/cytosim_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/cytosim/cytosim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/cytosim/cytosim_object_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.704877 simulariumio-1.7.1/simulariumio/data_objects/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/data_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25272 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/data_objects/agent_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/data_objects/camera_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/data_objects/dimension_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/data_objects/display_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/data_objects/histogram_plot_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/data_objects/input_file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/data_objects/meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/data_objects/model_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/data_objects/scatter_plot_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/data_objects/trajectory_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/data_objects/unit_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/file_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.704877 simulariumio-1.7.1/simulariumio/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/filters/add_agents_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/filters/every_nth_agent_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/filters/every_nth_subpoint_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/filters/every_nth_timestep_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/filters/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/filters/multiply_space_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/filters/multiply_time_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/filters/transform_spatial_axes_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/filters/translate_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.704877 simulariumio-1.7.1/simulariumio/mcell/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/mcell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/mcell/mcell_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/mcell/mcell_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.708877 simulariumio-1.7.1/simulariumio/md/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/md/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/md/md_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/md/md_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.708877 simulariumio-1.7.1/simulariumio/medyan/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/medyan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/medyan/medyan_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/medyan/medyan_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.708877 simulariumio-1.7.1/simulariumio/package_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/package_data/jmolcolors.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.708877 simulariumio-1.7.1/simulariumio/physicell/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/physicell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.708877 simulariumio-1.7.1/simulariumio/physicell/dep/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/physicell/dep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21762 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/physicell/dep/pyMCDS.py
--rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/physicell/physicell_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/physicell/physicell_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.708877 simulariumio-1.7.1/simulariumio/plot_readers/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/plot_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/plot_readers/histogram_plot_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/plot_readers/plot_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/plot_readers/scatter_plot_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.708877 simulariumio-1.7.1/simulariumio/readdy/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/readdy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/readdy/readdy_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/readdy/readdy_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.712877 simulariumio-1.7.1/simulariumio/readers/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/readers/binary_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/readers/simularium_binary_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.712877 simulariumio-1.7.1/simulariumio/smoldyn/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/smoldyn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/smoldyn/smoldyn_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/smoldyn/smoldyn_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.712877 simulariumio-1.7.1/simulariumio/springsalad/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/springsalad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/springsalad/springsalad_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/springsalad/springsalad_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.712877 simulariumio-1.7.1/simulariumio/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.712877 simulariumio-1.7.1/simulariumio/tests/buffer/
--rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/buffer/test_buffer_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/buffer/test_buffer_size.py
--rw-r--r--   0 runner    (1001) docker     (123)    49478 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.716877 simulariumio-1.7.1/simulariumio/tests/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/converters/test_cellpack_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/converters/test_cytosim_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/converters/test_mcell_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/converters/test_md_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13942 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/converters/test_medyan_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20573 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/converters/test_physicell_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/converters/test_readdy_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/converters/test_smoldyn_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11807 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/converters/test_springsalad_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    41761 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/converters/test_trajectory_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.684876 simulariumio-1.7.1/simulariumio/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.716877 simulariumio-1.7.1/simulariumio/tests/data/binary/
--rw-r--r--   0 runner    (1001) docker     (123)  1979356 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/binary/50filaments_motor_linker_binary.binary
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/binary/binary_test.binary
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.720878 simulariumio-1.7.1/simulariumio/tests/data/cellpack/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cellpack/example_2D_recipe.json
--rw-r--r--   0 runner    (1001) docker     (123)    18827 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cellpack/example_2D_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cellpack/mock_recipe.json
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cellpack/mock_results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.684876 simulariumio-1.7.1/simulariumio/tests/data/cytosim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.720878 simulariumio-1.7.1/simulariumio/tests/data/cytosim/3_fibers_3_frames/
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/3_fibers_3_frames/fiber_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/3_fibers_3_frames/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.736878 simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/aster_pull3D_couple_actin_solid.cym
--rw-r--r--   0 runner    (1001) docker     (123)  2076304 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/couples.txt
--rw-r--r--   0 runner    (1001) docker     (123)  8485882 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/fiber_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)  1461550 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/singles.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68842 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/solids.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.736878 simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couple_actin_solid.cym
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames.json
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames_small.json
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/couples.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/fiber_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/singles.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/solids.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.736878 simulariumio-1.7.1/simulariumio/tests/data/cytosim/fiber_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/cytosim/fiber_test/fiber_points.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.736878 simulariumio-1.7.1/simulariumio/tests/data/mcell/
--rw-r--r--   0 runner    (1001) docker     (123)  1033648 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example.blend
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.736878 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.736878 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/data_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.740878 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/
--rw-r--r--   0 runner    (1001) docker     (123)   157373 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.geometry.mdl
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.initialization.mdl
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.instantiation.mdl
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.main.mdl
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.mod_surf_regions.mdl
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.molecules.mdl
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.parameters.mdl
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.reactions.mdl
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.release_patterns.mdl
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.rxn_output.mdl
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.surface_classes.mdl
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.viz_output.mdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.684876 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.740878 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/a.World.dat
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/b.World.dat
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/c.World.dat
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/d.World.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.684876 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.740878 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/Scene.cellbin.0.dat
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/Scene.cellbin.1.dat
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/Scene.cellbin.2.dat
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/start_time.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.744879 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_viz_output/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.cellbin.0.dat
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.cellbin.1.dat
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.cellbin.2.dat
--rw-r--r--   0 runner    (1001) docker     (123)   297563 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.data_model.00.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.744879 simulariumio-1.7.1/simulariumio/tests/data/md/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/md/example.xyz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.744879 simulariumio-1.7.1/simulariumio/tests/data/medyan/
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/medyan/snapshot.traj
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/medyan/test.traj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.684876 simulariumio-1.7.1/simulariumio/tests/data/physicell/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.748879 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/initial.xml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/initial_cells.mat
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/initial_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (123)    80024 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/initial_mesh0.mat
--rw-r--r--   0 runner    (1001) docker     (123)   100047 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/initial_microenvironment0.mat
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000000.xml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000000_cells.mat
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000000_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (123)   100047 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000000_microenvironment0.mat
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000001.xml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000001_cells.mat
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000001_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (123)   100047 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000001_microenvironment0.mat
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000002.xml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000002_cells.mat
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000002_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (123)   100047 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000002_microenvironment0.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.756879 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/initial.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/initial_cells.mat
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/initial_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (123)   776184 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/initial_mesh0.mat
--rw-r--r--   0 runner    (1001) docker     (123)   970247 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/initial_microenvironment0.mat
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000000.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000000_cells.mat
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000000_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (123)   970247 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000000_microenvironment0.mat
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000001_cells.mat
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000001_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (123)   970247 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000001_microenvironment0.mat
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000002.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000002_cells.mat
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000002_cells_physicell.mat
--rw-r--r--   0 runner    (1001) docker     (123)   970247 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000002_microenvironment0.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.756879 simulariumio-1.7.1/simulariumio/tests/data/readdy/
--rw-r--r--   0 runner    (1001) docker     (123)    88121 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/readdy/test.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.756879 simulariumio-1.7.1/simulariumio/tests/data/smoldyn/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/smoldyn/example_2D.txt
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/smoldyn/example_3D.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/smoldyn/example_data.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.756879 simulariumio-1.7.1/simulariumio/tests/data/springsalad/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/springsalad/Simulation0_SIM_VIEW_Run0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/data/springsalad/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.760879 simulariumio-1.7.1/simulariumio/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/filters/test_add_agents_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    26508 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/filters/test_every_nth_agent_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    31715 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/filters/test_every_nth_subpoint_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    25395 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/filters/test_every_nth_timestep_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/filters/test_multiply_space_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/filters/test_multiply_time_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/filters/test_transform_spatial_axes_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/filters/test_translate_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/filters/test_translate_filter_sphere_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.760879 simulariumio-1.7.1/simulariumio/tests/plot_readers/
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/plot_readers/test_histogram_plot_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/plot_readers/test_scatter_plot_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.760879 simulariumio-1.7.1/simulariumio/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/readers/test_binary_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/test_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/test_input_file_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.760879 simulariumio-1.7.1/simulariumio/tests/writers/
--rw-r--r--   0 runner    (1001) docker     (123)    32766 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/tests/writers/test_binary_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/trajectory_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.760879 simulariumio-1.7.1/simulariumio/writers/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/writers/binary_chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/writers/binary_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/writers/binary_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/writers/json_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-02-20 18:01:28.000000 simulariumio-1.7.1/simulariumio/writers/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.700877 simulariumio-1.7.1/simulariumio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-02-20 18:01:43.000000 simulariumio-1.7.1/simulariumio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-02-20 18:01:43.000000 simulariumio-1.7.1/simulariumio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 18:01:43.000000 simulariumio-1.7.1/simulariumio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 18:01:42.000000 simulariumio-1.7.1/simulariumio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-02-20 18:01:43.000000 simulariumio-1.7.1/simulariumio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-20 18:01:43.000000 simulariumio-1.7.1/simulariumio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.764880 simulariumio-1.7.1/ui-templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/base_types.json
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/cellpack_data.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:01:43.764880 simulariumio-1.7.1/ui-templates/custom-types/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/custom-types/camera_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/custom-types/coordinates_xyz.json
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/custom-types/cytosim_object_info.json
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/custom-types/display_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/custom-types/meta_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/custom-types/model_meta_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/custom-types/space_unit_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/custom-types/time_unit_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/cytosim_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/medyan_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/smoldyn_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-02-20 18:01:28.000000 simulariumio-1.7.1/ui-templates/springsalad_data.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.429441 simulariumio-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-05 21:05:36.000000 simulariumio-1.8.0/.cookiecutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 21:05:36.000000 simulariumio-1.8.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.369439 simulariumio-1.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 21:05:36.000000 simulariumio-1.8.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.369439 simulariumio-1.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-05 21:05:36.000000 simulariumio-1.8.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 21:05:36.000000 simulariumio-1.8.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-05 21:05:36.000000 simulariumio-1.8.0/.github/ISSUE_TEMPLATE/maintenance_task.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-05 21:05:36.000000 simulariumio-1.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-05 21:05:36.000000 simulariumio-1.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.369439 simulariumio-1.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-05 21:05:36.000000 simulariumio-1.8.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-05 21:05:36.000000 simulariumio-1.8.0/.github/workflows/create-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-05 21:05:36.000000 simulariumio-1.8.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-05 21:05:36.000000 simulariumio-1.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-05 21:05:36.000000 simulariumio-1.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-05 21:05:36.000000 simulariumio-1.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-05 21:05:36.000000 simulariumio-1.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-05 21:05:36.000000 simulariumio-1.8.0/Justfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-05 21:05:36.000000 simulariumio-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-05-05 21:05:48.429441 simulariumio-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-05-05 21:05:36.000000 simulariumio-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.369439 simulariumio-1.8.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-05 21:05:36.000000 simulariumio-1.8.0/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-05 21:05:36.000000 simulariumio-1.8.0/benchmarks/TEST_RESOURCES_HASH.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-05 21:05:36.000000 simulariumio-1.8.0/benchmarks/benchmark_simulariumio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-05 21:05:36.000000 simulariumio-1.8.0/benchmarks/download_benchmark_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-05 21:05:36.000000 simulariumio-1.8.0/benchmarks/upload_benchmark_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.369439 simulariumio-1.8.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5362 2023-05-05 21:05:36.000000 simulariumio-1.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 21:05:36.000000 simulariumio-1.8.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-05 21:05:36.000000 simulariumio-1.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-05 21:05:36.000000 simulariumio-1.8.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-05 21:05:36.000000 simulariumio-1.8.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 21:05:36.000000 simulariumio-1.8.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.373440 simulariumio-1.8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-05 21:05:36.000000 simulariumio-1.8.0/examples/Tutorial_cellpack.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-05-05 21:05:36.000000 simulariumio-1.8.0/examples/Tutorial_custom.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-05 21:05:36.000000 simulariumio-1.8.0/examples/Tutorial_cytosim.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-05 21:05:36.000000 simulariumio-1.8.0/examples/Tutorial_filters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-05 21:05:36.000000 simulariumio-1.8.0/examples/Tutorial_mcell.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-05-05 21:05:36.000000 simulariumio-1.8.0/examples/Tutorial_md.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-05-05 21:05:36.000000 simulariumio-1.8.0/examples/Tutorial_medyan.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-05 21:05:36.000000 simulariumio-1.8.0/examples/Tutorial_physicell.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-05-05 21:05:36.000000 simulariumio-1.8.0/examples/Tutorial_plots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-05-05 21:05:36.000000 simulariumio-1.8.0/examples/Tutorial_readdy.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-05-05 21:05:36.000000 simulariumio-1.8.0/examples/Tutorial_smoldyn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-05 21:05:36.000000 simulariumio-1.8.0/examples/Tutorial_springsalad.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-05 21:05:36.000000 simulariumio-1.8.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.373440 simulariumio-1.8.0/examples/img/
+-rw-r--r--   0 runner    (1001) docker     (123)  3109823 2023-05-05 21:05:36.000000 simulariumio-1.8.0/examples/img/drag_drop.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-05-05 21:05:36.000000 simulariumio-1.8.0/file_format.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-05 21:05:36.000000 simulariumio-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:05:48.429441 simulariumio-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.377440 simulariumio-1.8.0/simulariumio/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.377440 simulariumio-1.8.0/simulariumio/cellpack/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/cellpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15769 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/cellpack/cellpack_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/cellpack/cellpack_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.377440 simulariumio-1.8.0/simulariumio/cytosim/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/cytosim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12930 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/cytosim/cytosim_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/cytosim/cytosim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/cytosim/cytosim_object_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.381440 simulariumio-1.8.0/simulariumio/data_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/data_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29455 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/data_objects/agent_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/data_objects/camera_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/data_objects/dimension_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/data_objects/display_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/data_objects/histogram_plot_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/data_objects/input_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/data_objects/meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/data_objects/model_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/data_objects/scatter_plot_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/data_objects/trajectory_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/data_objects/unit_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/file_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.381440 simulariumio-1.8.0/simulariumio/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/filters/add_agents_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/filters/every_nth_agent_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/filters/every_nth_subpoint_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/filters/every_nth_timestep_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/filters/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/filters/multiply_space_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/filters/multiply_time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/filters/transform_spatial_axes_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/filters/translate_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.381440 simulariumio-1.8.0/simulariumio/mcell/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/mcell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/mcell/mcell_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/mcell/mcell_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.381440 simulariumio-1.8.0/simulariumio/md/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/md/md_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/md/md_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.381440 simulariumio-1.8.0/simulariumio/medyan/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/medyan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/medyan/medyan_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/medyan/medyan_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.381440 simulariumio-1.8.0/simulariumio/package_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/package_data/jmolcolors.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.381440 simulariumio-1.8.0/simulariumio/physicell/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/physicell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.381440 simulariumio-1.8.0/simulariumio/physicell/dep/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/physicell/dep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21762 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/physicell/dep/pyMCDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15759 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/physicell/physicell_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/physicell/physicell_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.385440 simulariumio-1.8.0/simulariumio/plot_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/plot_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/plot_readers/histogram_plot_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/plot_readers/plot_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/plot_readers/scatter_plot_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.385440 simulariumio-1.8.0/simulariumio/readdy/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/readdy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/readdy/readdy_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/readdy/readdy_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.385440 simulariumio-1.8.0/simulariumio/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/readers/binary_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/readers/simularium_binary_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.385440 simulariumio-1.8.0/simulariumio/smoldyn/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/smoldyn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/smoldyn/smoldyn_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/smoldyn/smoldyn_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.385440 simulariumio-1.8.0/simulariumio/springsalad/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/springsalad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/springsalad/springsalad_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/springsalad/springsalad_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.385440 simulariumio-1.8.0/simulariumio/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.385440 simulariumio-1.8.0/simulariumio/tests/buffer/
+-rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/buffer/test_buffer_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/buffer/test_buffer_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49341 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.389440 simulariumio-1.8.0/simulariumio/tests/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/converters/test_cellpack_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/converters/test_cytosim_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/converters/test_mcell_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/converters/test_md_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/converters/test_medyan_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21824 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/converters/test_physicell_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12765 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/converters/test_readdy_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13977 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/converters/test_smoldyn_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/converters/test_springsalad_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41763 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/converters/test_trajectory_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.365440 simulariumio-1.8.0/simulariumio/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.389440 simulariumio-1.8.0/simulariumio/tests/data/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)  1979356 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/binary/50filaments_motor_linker_binary.binary
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/binary/binary_test.binary
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.389440 simulariumio-1.8.0/simulariumio/tests/data/cellpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cellpack/example_2D_recipe.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18827 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cellpack/example_2D_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cellpack/mock_recipe.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cellpack/mock_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cellpack/two_ingredients_recipe.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15676 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cellpack/two_ingredients_results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.365440 simulariumio-1.8.0/simulariumio/tests/data/cytosim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.389440 simulariumio-1.8.0/simulariumio/tests/data/cytosim/3_fibers_3_frames/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/3_fibers_3_frames/fiber_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/3_fibers_3_frames/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.405440 simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/aster_pull3D_couple_actin_solid.cym
+-rw-r--r--   0 runner    (1001) docker     (123)  2076304 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/couples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  8485882 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/fiber_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1461550 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/singles.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68842 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/solids.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.405440 simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couple_actin_solid.cym
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames_small.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/couples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/fiber_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/singles.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/solids.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.405440 simulariumio-1.8.0/simulariumio/tests/data/cytosim/fiber_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/cytosim/fiber_test/fiber_points.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.405440 simulariumio-1.8.0/simulariumio/tests/data/malformed_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/malformed_data/malformed_cytosim.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/malformed_data/malformed_medyan.traj
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/malformed_data/malformed_smoldyn.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/malformed_data/springsalad_broken_link.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.405440 simulariumio-1.8.0/simulariumio/tests/data/mcell/
+-rw-r--r--   0 runner    (1001) docker     (123)  1033648 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example.blend
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.405440 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.405440 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/data_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.409440 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   157373 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.geometry.mdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.initialization.mdl
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.instantiation.mdl
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.main.mdl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.mod_surf_regions.mdl
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.molecules.mdl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.parameters.mdl
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.reactions.mdl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.release_patterns.mdl
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.rxn_output.mdl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.surface_classes.mdl
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.viz_output.mdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.365440 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.409440 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/a.World.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/b.World.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/c.World.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/react_data/seed_00001/d.World.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.365440 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.409440 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/Scene.cellbin.0.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/Scene.cellbin.1.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/viz_data/seed_00001/Scene.cellbin.2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/start_time.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.409440 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_viz_output/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.cellbin.0.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.cellbin.1.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.cellbin.2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   297563 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.data_model.00.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.409440 simulariumio-1.8.0/simulariumio/tests/data/md/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/md/example.xyz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.413440 simulariumio-1.8.0/simulariumio/tests/data/medyan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/medyan/snapshot.traj
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/medyan/test.traj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.365440 simulariumio-1.8.0/simulariumio/tests/data/physicell/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.413440 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/initial.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/initial_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/initial_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (123)    80024 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/initial_mesh0.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   100047 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/initial_microenvironment0.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000000.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000000_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000000_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   100047 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000000_microenvironment0.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000001_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000001_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   100047 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000001_microenvironment0.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000002.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000002_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000002_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   100047 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000002_microenvironment0.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.421440 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/initial.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/initial_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/initial_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   776184 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/initial_mesh0.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   970247 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/initial_microenvironment0.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000000.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000000_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000000_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   970247 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000000_microenvironment0.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000001_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000001_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   970247 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000001_microenvironment0.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000002.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000002_cells.mat
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000002_cells_physicell.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   970247 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000002_microenvironment0.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.421440 simulariumio-1.8.0/simulariumio/tests/data/readdy/
+-rw-r--r--   0 runner    (1001) docker     (123)    88121 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/readdy/test.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.421440 simulariumio-1.8.0/simulariumio/tests/data/smoldyn/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/smoldyn/example_2D.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/smoldyn/example_3D.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/smoldyn/example_data.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.421440 simulariumio-1.8.0/simulariumio/tests/data/springsalad/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/springsalad/Simulation0_SIM_VIEW_Run0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/data/springsalad/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.425440 simulariumio-1.8.0/simulariumio/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/filters/test_add_agents_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26508 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/filters/test_every_nth_agent_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31715 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/filters/test_every_nth_subpoint_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25395 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/filters/test_every_nth_timestep_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/filters/test_multiply_space_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/filters/test_multiply_time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/filters/test_transform_spatial_axes_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/filters/test_translate_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/filters/test_translate_filter_sphere_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.425440 simulariumio-1.8.0/simulariumio/tests/plot_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/plot_readers/test_histogram_plot_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/plot_readers/test_scatter_plot_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.425440 simulariumio-1.8.0/simulariumio/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/readers/test_binary_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/test_agents_from_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/test_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/test_input_file_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.425440 simulariumio-1.8.0/simulariumio/tests/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)    32766 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/tests/writers/test_binary_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/trajectory_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.425440 simulariumio-1.8.0/simulariumio/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/writers/binary_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/writers/binary_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/writers/binary_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/writers/json_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-05-05 21:05:36.000000 simulariumio-1.8.0/simulariumio/writers/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.377440 simulariumio-1.8.0/simulariumio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-05-05 21:05:48.000000 simulariumio-1.8.0/simulariumio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-05-05 21:05:48.000000 simulariumio-1.8.0/simulariumio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:05:48.000000 simulariumio-1.8.0/simulariumio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:05:47.000000 simulariumio-1.8.0/simulariumio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-05 21:05:48.000000 simulariumio-1.8.0/simulariumio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 21:05:48.000000 simulariumio-1.8.0/simulariumio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.425440 simulariumio-1.8.0/ui-templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/base_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/cellpack_data.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:05:48.429441 simulariumio-1.8.0/ui-templates/custom-types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/custom-types/camera_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/custom-types/coordinates_xyz.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/custom-types/cytosim_object_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/custom-types/display_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/custom-types/meta_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/custom-types/model_meta_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/custom-types/space_unit_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/custom-types/time_unit_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/cytosim_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/medyan_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/smoldyn_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-05 21:05:36.000000 simulariumio-1.8.0/ui-templates/springsalad_data.json
```

### Comparing `simulariumio-1.7.1/.github/PULL_REQUEST_TEMPLATE.md` & `simulariumio-1.8.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/.github/workflows/ci.yml` & `simulariumio-1.8.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/.github/workflows/docs.yml` & `simulariumio-1.8.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/.gitignore` & `simulariumio-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/CODE_OF_CONDUCT.md` & `simulariumio-1.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/CONTRIBUTING.md` & `simulariumio-1.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/Justfile` & `simulariumio-1.8.0/Justfile`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/LICENSE` & `simulariumio-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/PKG-INFO` & `simulariumio-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulariumio
-Version: 1.7.1
+Version: 1.8.0
 Summary: Python package that converts simulation outputs to the format consumed by the Simularium viewer website
 Author-email: Blair Lyons <blairl@alleninstitute.org>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://github.com/Simularium/simulariumio
 Project-URL: Bug Tracker, https://github.com/Simularium/simulariumio/issues
 Project-URL: Documentation, https://Simularium.github.io/simulariumio
 Project-URL: User Support, https://github.com/Simularium/simulariumio/issues
```

### Comparing `simulariumio-1.7.1/README.md` & `simulariumio-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/benchmarks/README.md` & `simulariumio-1.8.0/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/benchmarks/benchmark_simulariumio.py` & `simulariumio-1.8.0/benchmarks/benchmark_simulariumio.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/benchmarks/download_benchmark_resources.py` & `simulariumio-1.8.0/benchmarks/download_benchmark_resources.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/benchmarks/upload_benchmark_resources.py` & `simulariumio-1.8.0/benchmarks/upload_benchmark_resources.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/docs/conf.py` & `simulariumio-1.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/docs/installation.rst` & `simulariumio-1.8.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/examples/Tutorial_cellpack.ipynb` & `simulariumio-1.8.0/examples/Tutorial_cellpack.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/examples/Tutorial_custom.ipynb` & `simulariumio-1.8.0/examples/Tutorial_custom.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/examples/Tutorial_cytosim.ipynb` & `simulariumio-1.8.0/examples/Tutorial_cytosim.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/examples/Tutorial_filters.ipynb` & `simulariumio-1.8.0/examples/Tutorial_filters.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/examples/Tutorial_mcell.ipynb` & `simulariumio-1.8.0/examples/Tutorial_mcell.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/examples/Tutorial_md.ipynb` & `simulariumio-1.8.0/examples/Tutorial_md.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/examples/Tutorial_medyan.ipynb` & `simulariumio-1.8.0/examples/Tutorial_medyan.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/examples/Tutorial_physicell.ipynb` & `simulariumio-1.8.0/examples/Tutorial_physicell.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/examples/Tutorial_plots.ipynb` & `simulariumio-1.8.0/examples/Tutorial_plots.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/examples/Tutorial_readdy.ipynb` & `simulariumio-1.8.0/examples/Tutorial_readdy.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/examples/Tutorial_smoldyn.ipynb` & `simulariumio-1.8.0/examples/Tutorial_smoldyn.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/examples/Tutorial_springsalad.ipynb` & `simulariumio-1.8.0/examples/Tutorial_springsalad.ipynb`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/examples/img/drag_drop.gif` & `simulariumio-1.8.0/examples/img/drag_drop.gif`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/file_format.md` & `simulariumio-1.8.0/file_format.md`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/pyproject.toml` & `simulariumio-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/__init__.py` & `simulariumio-1.8.0/simulariumio/__init__.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/cellpack/cellpack_converter.py` & `simulariumio-1.8.0/simulariumio/cellpack/cellpack_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 # -*- coding: utf-8 -*-
 
 import logging
 import os
 import numpy as np
 import json
 from scipy.spatial.transform import Rotation as R
+from typing import Callable
 
 from cellpack import RecipeLoader
 from ..constants import DISPLAY_TYPE, VIZ_TYPE, VALUES_PER_3D_POINT
 from ..data_objects.camera_data import CameraData
 from ..trajectory_converter import TrajectoryConverter
 from ..data_objects import TrajectoryData, AgentData, DimensionData
 from ..data_objects import MetaData, DisplayData
+from ..exceptions import InputDataError
 from .cellpack_data import HAND_TYPE, CellpackData
 
 ###############################################################################
 
 log = logging.getLogger(__name__)
 
 ###############################################################################
@@ -28,27 +30,42 @@
 )
 
 # NOTE: Default scale is 0.1, so the actual default r will be 1.0
 DEFAULT_RADIUS = 10
 
 
 class CellpackConverter(TrajectoryConverter):
-    def __init__(self, input_data: CellpackData):
+    def __init__(
+        self,
+        input_data: CellpackData,
+        progress_callback: Callable[[float], None] = None,
+        callback_interval: float = 10,
+    ):
         """
         This object reads packing results outputs
         from Cellpack (http://www.cellpack.org)
         and plot data and writes them in the JSON format used
         by the Simularium viewer
 
         Parameters
         ----------
         input_data : CellpackData
             An object containing info for reading
             Cellpack simulation trajectory outputs and plot data
+        progress_callback : Callable[[float], None] (optional)
+            Callback function that accepts 1 float argument and returns None
+            which will be called at a given progress interval, determined by
+            callback_interval requested, providing the current percent progress
+            Default: None
+        callback_interval : float (optional)
+            If a progress_callback was provided, the period between updates
+            to be sent to the callback, in seconds
+            Default: 10
         """
+        super().__init__(input_data, progress_callback, callback_interval)
         self._data = self._read(input_data)
 
     @staticmethod
     def _get_box_center(recipe_data):
         options = recipe_data["options"]
         bb = options["boundingBox"]
         x_pos = (bb[1][0] - bb[0][0]) / 2.0 + bb[0][0]
@@ -251,29 +268,35 @@
                 DISPLAY_TYPE.FIBER
                 if ingredient_data["Type"] == "Grow"
                 else DISPLAY_TYPE.SPHERE
             )
             url = ""
         return {"display_type": display_type, "color": color, "url": url}
 
-    @staticmethod
     def _process_ingredients(
+        self,
         all_ingredients,
         time_step_index: int,
         scale_factor: float,
         box_center: np.array,
         geo_type: DISPLAY_TYPE,
         handedness: HAND_TYPE,
         geometry_url: str,
         display_data,
     ) -> AgentData:
         dimensions = CellpackConverter._parse_dimensions(all_ingredients)
         spatial_data = AgentData.from_dimensions(dimensions)
         display_data = {} if display_data is None else display_data
         agent_id_counter = 0
+
+        total_agents = 0
+        for ingredient in all_ingredients:
+            total_agents += len(ingredient["results"].get("results", []))
+            total_agents += len(ingredient["results"].get("nbCurve", []))
+
         for ingredient in all_ingredients:
             ingredient_data = ingredient["recipe_data"]
             ingredient_key = ingredient_data["name"]
             ingredient_results_data = ingredient["results"]
             agent_display_data = TrajectoryConverter._get_display_data_for_agent(
                 ingredient_key, display_data
             )
@@ -307,59 +330,64 @@
                         agent_id_counter,
                         spatial_data,
                         scale_factor,
                         box_center,
                         handedness,
                     )
                     agent_id_counter += 1
+                    self.check_report_progress(agent_id_counter / total_agents)
             elif ingredient_results_data["nbCurve"] > 0:
                 for i in range(ingredient_results_data["nbCurve"]):
                     CellpackConverter._unpack_curve(
                         ingredient_results_data,
                         time_step_index,
                         ingredient_key,
                         i,
                         agent_id_counter,
                         spatial_data,
                         scale_factor,
                         box_center,
                     )
                     agent_id_counter += 1
+                    self.check_report_progress(agent_id_counter / total_agents)
+
         spatial_data.display_data = display_data
         return spatial_data
 
     @staticmethod
     def _update_meta_data(meta_data: MetaData, box_size: np.array) -> MetaData:
         camera_z_position = box_size[2] if box_size[2] > 10 else 100.0
         meta_data.camera_defaults = CameraData(
             position=np.array([10.0, 0.0, camera_z_position]),
             look_at_position=np.array([10.0, 0.0, 0.0]),
         )
 
-    @staticmethod
-    def _read(input_data: CellpackData) -> TrajectoryData:
+    def _read(self, input_data: CellpackData) -> TrajectoryData:
         """
         Return a TrajectoryData object containing the Cellpack data
         """
         print("Reading Cellpack Data -------------")
         # currently only converts one model, ie one time step
         time_step_index = 0
         # default scale for cellpack => simularium
         # user is supposed to send in the cellPACK scale factor
         # if they send one in at all.
         input_data.meta_data.scale_factor *= 0.1
 
-        # load the data from Cellpack output JSON file
-        recipe_loader = RecipeLoader(input_data.recipe_file_path)
-        recipe_data = recipe_loader.recipe_data
-        results_data = json.loads(input_data.results_file.get_contents())
-        all_ingredients = recipe_loader.get_all_ingredients(results_data)
+        try:
+            # load the data from Cellpack output JSON file
+            recipe_loader = RecipeLoader(input_data.recipe_file_path)
+            recipe_data = recipe_loader.recipe_data
+            results_data = json.loads(input_data.results_file.get_contents())
+            all_ingredients = recipe_loader.get_all_ingredients(results_data)
+        except Exception as e:
+            raise InputDataError(f"Error reading cellpack input file: {e}")
 
         box_center = CellpackConverter._get_box_center(recipe_data)
-        agent_data = CellpackConverter._process_ingredients(
+        agent_data = self._process_ingredients(
             all_ingredients,
             time_step_index,
             input_data.meta_data.scale_factor,
             box_center,
             input_data.geometry_type,
             input_data.handedness,
             input_data.geometry_url,
```

### Comparing `simulariumio-1.7.1/simulariumio/cellpack/cellpack_data.py` & `simulariumio-1.8.0/simulariumio/cellpack/cellpack_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/constants.py` & `simulariumio-1.8.0/simulariumio/constants.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/cytosim/cytosim_converter.py` & `simulariumio-1.8.0/simulariumio/cytosim/cytosim_converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,63 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-from typing import Any, Dict, List, Tuple
-
+from typing import Any, Dict, List, Tuple, Callable
 import numpy as np
 
 from ..trajectory_converter import TrajectoryConverter
 from ..data_objects import (
     TrajectoryData,
     AgentData,
     UnitData,
     DimensionData,
     DisplayData,
 )
 from ..constants import VIZ_TYPE, DISPLAY_TYPE, SUBPOINT_VALUES_PER_ITEM
+from ..exceptions import InputDataError
 from .cytosim_data import CytosimData
 from .cytosim_object_info import CytosimObjectInfo
 
 ###############################################################################
 
 log = logging.getLogger(__name__)
 
 ###############################################################################
 
 
 class CytosimConverter(TrajectoryConverter):
-    def __init__(self, input_data: CytosimData):
+    def __init__(
+        self,
+        input_data: CytosimData,
+        progress_callback: Callable[[float], None] = None,
+        callback_interval: float = 10,
+    ):
         """
         This object reads simulation trajectory outputs
         from CytoSim (https://gitlab.com/f.nedelec/cytosim)
         and plot data and writes them in the JSON format used
         by the Simularium viewer
 
         Parameters
         ----------
         input_data : CytosimData
             An object containing info for reading
             Cytosim simulation trajectory outputs and plot data
+        progress_callback : Callable[[float], None] (optional)
+            Callback function that accepts 1 float argument and returns None
+            which will be called at a given progress interval, determined by
+            callback_interval requested, providing the current percent progress
+            Default: None
+        callback_interval : float (optional)
+            If a progress_callback was provided, the period between updates
+            to be sent to the callback, in seconds
+            Default: 10
         """
+        super().__init__(input_data, progress_callback, callback_interval)
         self._data = self._read(input_data)
 
     @staticmethod
     def _ignore_line(line: str) -> bool:
         """
         if the line doesn't have any data, it can be ignored
         """
@@ -164,31 +179,34 @@
             float(object_info.display_data[raw_tid].radius)
             if raw_tid in object_info.display_data
             and object_info.display_data[raw_tid].radius is not None
             else 1.0
         )
         return (result, uids, used_unique_IDs)
 
-    @staticmethod
     def _parse_objects(
+        self,
         object_type: str,
         data_lines: List[str],
         scale_factor: float,
         object_info: CytosimObjectInfo,
         result: AgentData,
         used_unique_IDs: List[int],
-    ) -> Tuple[Dict[str, Any], List[int]]:
+        overall_line: int,
+        total_lines: int,
+    ) -> Tuple[Dict[str, Any], List[int], int]:
         """
         Parse a Cytosim output file containing objects
         (fibers, solids, singles, or couples) to get agents
         """
         time_index = -1
         uids = {}
         is_fiber = "fiber" in object_type
         for line in data_lines:
+            overall_line += 1
             if CytosimConverter._ignore_line(line):
                 continue
             columns = line.split()
             if line[0] == "%":
                 if "frame" in line:
                     # start of frame
                     time_index += 1
@@ -248,45 +266,60 @@
                             float(columns[object_info.position_indices[0]].strip("+,")),
                             float(columns[object_info.position_indices[1]].strip("+,")),
                             float(columns[object_info.position_indices[2]].strip("+,")),
                         ]
                     )
                 )
                 result.n_agents[time_index] += 1
+            self.check_report_progress(overall_line / total_lines)
+
         result.n_timesteps = time_index + 1
-        return (result, used_unique_IDs)
+        return (result, used_unique_IDs, overall_line)
 
-    @staticmethod
-    def _read(input_data: CytosimData) -> TrajectoryData:
+    def _read(self, input_data: CytosimData) -> TrajectoryData:
         """
         Return a TrajectoryData object containing the CytoSim data
         """
         print("Reading Cytosim Data -------------")
         # load the data from Cytosim output .txt files
         cytosim_data = {}
-        for object_type in input_data.object_info:
-            cytosim_data[object_type] = (
-                input_data.object_info[object_type]
-                .cytosim_file.get_contents()
-                .split("\n")
-            )
+        try:
+            for object_type in input_data.object_info:
+                cytosim_data[object_type] = (
+                    input_data.object_info[object_type]
+                    .cytosim_file.get_contents()
+                    .split("\n")
+                )
+        except Exception as e:
+            raise InputDataError(f"Error reading input cytosim file: {e}")
+
         # parse
         dimensions = CytosimConverter._parse_dimensions(cytosim_data)
         agent_data = AgentData.from_dimensions(dimensions)
         agent_data.draw_fiber_points = input_data.draw_fiber_points
+        overall_line = 0
+        total_lines = sum(
+            len(cytosim_data[object_type]) for object_type in input_data.object_info
+        )
+
         uids = []
         for object_type in input_data.object_info:
-            agent_data, uids = CytosimConverter._parse_objects(
-                object_type,
-                cytosim_data[object_type],
-                input_data.meta_data.scale_factor,
-                input_data.object_info[object_type],
-                agent_data,
-                uids,
-            )
+            try:
+                (agent_data, uids, overall_line) = self._parse_objects(
+                    object_type,
+                    cytosim_data[object_type],
+                    input_data.meta_data.scale_factor,
+                    input_data.object_info[object_type],
+                    agent_data,
+                    uids,
+                    overall_line,
+                    total_lines,
+                )
+            except Exception as e:
+                raise InputDataError(f"Error reading input cytosim data: {e}")
         # get display data (geometry and color)
         for object_type in input_data.object_info:
             for tid in input_data.object_info[object_type].display_data:
                 display_data = input_data.object_info[object_type].display_data[tid]
                 if "fiber" in object_type and (
                     display_data.display_type != DISPLAY_TYPE.NONE
                     and display_data.display_type != DISPLAY_TYPE.FIBER
```

### Comparing `simulariumio-1.7.1/simulariumio/cytosim/cytosim_data.py` & `simulariumio-1.8.0/simulariumio/cytosim/cytosim_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/cytosim/cytosim_object_info.py` & `simulariumio-1.8.0/simulariumio/cytosim/cytosim_object_info.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/data_objects/__init__.py` & `simulariumio-1.8.0/simulariumio/data_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/data_objects/agent_data.py` & `simulariumio-1.8.0/simulariumio/data_objects/agent_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import copy
 import logging
-from typing import List, Tuple, Dict, Any
+from typing import List, Tuple, Dict, Any, Union
 
 import numpy as np
 import pandas as pd
 
 from ..constants import (
     V1_SPATIAL_BUFFER_STRUCT,
     VIZ_TYPE,
@@ -26,113 +26,140 @@
 log = logging.getLogger(__name__)
 
 ###############################################################################
 
 
 class AgentData:
     n_timesteps: int
-    times: np.ndarray
-    n_agents: np.ndarray
-    viz_types: np.ndarray
-    unique_ids: np.ndarray
+    times: Union[np.ndarray, List[float]]
+    n_agents: Union[np.ndarray, List[int]]
+    viz_types: Union[np.ndarray, List[List[float]]]
+    unique_ids: Union[np.ndarray, List[List[int]]]
     types: List[List[str]]
-    positions: np.ndarray
-    radii: np.ndarray
-    rotations: np.ndarray
-    n_subpoints: np.ndarray
-    subpoints: np.ndarray
+    positions: Union[np.ndarray, List[List[List[float]]]]
+    radii: Union[np.ndarray, List[List[float]]]
+    rotations: Union[np.ndarray, List[List[List[float]]]]
+    n_subpoints: Union[np.ndarray, List[List[float]]]
+    subpoints: Union[np.ndarray, List[List[List[float]]]]
     display_data: Dict[str, DisplayData]
     draw_fiber_points: bool
 
     def __init__(
         self,
-        times: np.ndarray,
-        n_agents: np.ndarray,
-        viz_types: np.ndarray,
-        unique_ids: np.ndarray,
+        times: Union[np.ndarray, List[float]],
+        n_agents: Union[np.ndarray, List[int]],
+        viz_types: Union[np.ndarray, List[List[float]]],
+        unique_ids: Union[np.ndarray, List[List[int]]],
         types: List[List[str]],
-        positions: np.ndarray,
-        radii: np.ndarray,
-        rotations: np.ndarray = None,
-        n_subpoints: np.ndarray = None,
-        subpoints: np.ndarray = None,
+        positions: Union[np.ndarray, List[List[List[float]]]],
+        radii: Union[np.ndarray, List[List[float]]],
+        rotations: Union[np.ndarray, List[List[List[float]]]] = None,
+        n_subpoints: Union[np.ndarray, List[List[int]]] = None,
+        subpoints: Union[np.ndarray, List[List[List[float]]]] = None,
         display_data: Dict[str, DisplayData] = None,
         draw_fiber_points: bool = False,
         n_timesteps: int = -1,
     ):
         """
         This object contains spatial simulation data
 
         Parameters
         ----------
-        times : np.ndarray (shape = [timesteps])
-            A numpy ndarray containing the elapsed simulated time
-            at each timestep (in the units specified by
+        times : np.ndarray or List[float] (shape = [timesteps])
+            A numpy ndarray or list containing the elapsed simulated
+            time at each timestep (in the units specified by
             TrajectoryData.time_units)
-        n_agents : np.ndarray (shape = [timesteps])
-            A numpy ndarray containing the number of agents
+        n_agents : np.ndarray or List[int] (shape = [timesteps])
+            A numpy ndarray or list containing the number of agents
             that exist at each timestep
-        viz_types : np.ndarray (shape = [timesteps, agents])
-            A numpy ndarray containing the viz type
+        viz_types : np.ndarray or List[List[float]] (shape = [timesteps, agents])s
+            A numpy ndarray or list containing the viz type
             for each agent at each timestep. Current options:
                 1000 : default,
                 1001 : fiber (which will require subpoints)
-        unique_ids : np.ndarray (shape = [timesteps, agents])
-            A numpy ndarray containing the unique ID
+        unique_ids : np.ndarray or List[List[int]] (shape = [timesteps, agents])
+            A numpy ndarray or list containing the unique ID
             for each agent at each timestep
         types : List[List[str]] (list of shape [timesteps, agents])
             A list containing timesteps, for each a list of
             the string name for the type of each agent
-        positions : np.ndarray (shape = [timesteps, agents, 3])
-            A numpy ndarray containing the XYZ position
+        positions : np.ndarray or List[List[List[float]]]
+        (shape = [timesteps, agents, 3])
+            A numpy ndarray or list containing the XYZ position
             for each agent at each timestep (in the units
             specified by TrajectoryData.spatial_units)
-        radii : np.ndarray (shape = [timesteps, agents])
-            A numpy ndarray containing the radius
+        radii : np.ndarray or List[List[float]] (shape = [timesteps, agents])
+            A numpy ndarray or list containing the radius
             for each agent at each timestep
-        rotations : np.ndarray (shape = [timesteps, agents, 3]) (optional)
-            A numpy ndarray containing the XYZ euler angles representing
+        rotations : np.ndarray or List[List[List[float]]]
+        (shape = [timesteps, agents, 3]) (optional)
+            A numpy ndarray or list containing the XYZ euler angles representing
             the rotation for each agent at each timestep in degrees
             Default: [0, 0, 0] for each agent
-        n_subpoints : np.ndarray (shape = [timesteps, agents]) (optional)
-            A numpy ndarray containing the number of subpoints
+        n_subpoints : np.ndarray or List[List[int]]
+        (shape = [timesteps, agents]) (optional)
+            A numpy ndarray or list containing the number of subpoints
             belonging to each agent at each timestep. Required if
             subpoints are provided
             Default: None
-        subpoints : np.ndarray
+        subpoints : np.ndarray or List[List[List[float]]]
         (shape = [timesteps, agents, subpoints]) (optional)
-            A numpy ndarray containing a list of subpoint data
+            A numpy ndarray or list containing a list of subpoint data
             for each agent at each timestep. These values are
             currently used for fiber and sphere group agents
             Default: None
         display_data: Dict[str,DisplayData] (optional)
             A dictionary mapping agent type name to DisplayData
             to use for that type
             Default: None
         draw_fiber_points: bool (optional)
             Draw spheres at every other fiber point for fibers?
             Default: False
         n_timesteps : int (optional)
             Use the first n_timesteps frames of data
             Default: -1 (use the full length of the buffer)
         """
-        self.times = times
-        self.n_agents = n_agents
-        self.viz_types = viz_types
-        self.unique_ids = unique_ids
+        self.times = np.array(times)
+        self.n_agents = np.array(n_agents)
+        self.viz_types = (
+            AgentData._fill_df(pd.DataFrame(viz_types), 1000.0).to_numpy(dtype=float)
+            if type(viz_types) is list
+            else viz_types
+        )
+        self.unique_ids = (
+            AgentData._fill_df(pd.DataFrame(unique_ids), 0).to_numpy(dtype=int)
+            if type(unique_ids) is list
+            else unique_ids
+        )
         self.types = types
-        self.positions = positions
-        self.radii = radii
+        self.positions = (
+            AgentData._jagged_3d_list_to_numpy_array(positions)
+            if type(positions) is list
+            else positions
+        )
+        self.radii = (
+            AgentData._fill_df(pd.DataFrame(radii), 0.0).to_numpy()
+            if type(radii) is list
+            else radii
+        )
         self.rotations = (
-            rotations if rotations is not None else np.zeros_like(positions)
+            AgentData._jagged_3d_list_to_numpy_array(rotations)
+            if rotations is not None
+            else np.zeros_like(self.positions)
         )
         self.n_subpoints = (
-            n_subpoints if n_subpoints is not None else np.zeros_like(radii)
+            AgentData._fill_df(pd.DataFrame(n_subpoints), 0.0).to_numpy(dtype=int)
+            if n_subpoints is not None
+            else np.zeros_like(self.radii)
+        )
+        self.subpoints = (
+            AgentData._get_subpoints_numpy_array(subpoints)
+            if subpoints is not None
+            else np.zeros_like(n_agents)
         )
-        self.subpoints = subpoints if subpoints is not None else np.zeros_like(n_agents)
         self.display_data = display_data if display_data is not None else {}
         self.draw_fiber_points = draw_fiber_points
         self.n_timesteps = n_timesteps
 
     @staticmethod
     def _get_buffer_data_dimensions(buffer_data: Dict[str, Any]) -> DimensionData:
         """
@@ -326,14 +353,75 @@
             rotations=agent_data.rotations,
             n_subpoints=agent_data.n_subpoints,
             subpoints=agent_data.subpoints,
             display_data=display_data,
             draw_fiber_points=False,
         )
 
+    @staticmethod
+    def _fill_df(df: pd.DataFrame, fill: List[float]) -> pd.DataFrame:
+        """
+        Fill Nones in a DataFrame with a fill value
+        """
+        # Create a dataframe of fill values
+        fill_array = [[fill] * df.shape[1]] * df.shape[0]
+        fill_df = pd.DataFrame(fill_array)
+        # Replace all entries with None with the fill
+        df[df.isna()] = fill_df
+        return df
+
+    @staticmethod
+    def _jagged_3d_list_to_numpy_array(
+        jagged_3d_list: Union[np.ndarray, List]
+    ) -> np.ndarray:
+        """
+        Shape a jagged list with 3 dimensions to a numpy array
+        """
+        if type(jagged_3d_list) is np.ndarray:
+            return jagged_3d_list
+
+        df = AgentData._fill_df(pd.DataFrame(jagged_3d_list), [0, 0, 0])
+        df_t = df.transpose()
+        exploded = [df_t[col].explode() for col in list(df_t.columns)]
+        x = np.array(exploded, dtype=float).reshape((df.shape[0], df.shape[1], 3))
+        print(x)
+        return x
+
+    @staticmethod
+    def _get_subpoints_numpy_array(subpoints: Union[np.ndarray, List]) -> np.ndarray:
+        """
+        Shape a 3 dimensional jagged list for subpoints into a numpy array
+        """
+        if type(subpoints) is np.ndarray:
+            return subpoints
+
+        frame_arrays = []
+        max_agents = 0
+        max_subpoints = 0
+        total_steps = len(subpoints) if subpoints else 0
+        for time_index in range(total_steps):
+            filled_frame = AgentData._fill_df(pd.DataFrame(subpoints[time_index]), 0.0)
+            frame_array = np.array(filled_frame, dtype=float)
+            if frame_array.shape[0] > max_agents:
+                max_agents = frame_array.shape[0]
+            if frame_array.shape[1] > max_subpoints:
+                max_subpoints = frame_array.shape[1]
+            frame_arrays.append(frame_array)
+        values_per_frame = max_agents * max_subpoints
+        result = np.zeros(total_steps * values_per_frame)
+        for time_index, frame_array in enumerate(frame_arrays):
+            if frame_array.shape[1] < max_subpoints:
+                new_frame_array = np.zeros((frame_array.shape[0], max_subpoints, 3))
+                new_frame_array[:, : frame_array.shape[1]] = frame_array
+                frame_array = new_frame_array
+            flat_array = frame_array.flatten()
+            start_index = time_index * values_per_frame
+            result[start_index : start_index + flat_array.shape[0]] = flat_array
+        return result.reshape(total_steps, max_agents, max_subpoints)
+
     @classmethod
     def from_dataframe(cls, traj: pd.DataFrame):
         """
         Create AgentData from a pandas DataFrame with columns:
         time, unique_id, type, positionX, positionY, positionZ, radius
         (only for default agents, no fibers)
         """
@@ -541,28 +629,28 @@
                 display_type=self._default_display_type_for_agent(
                     time_index, agent_index
                 ),
             )
         return self.display_data[type_name].display_type
 
     def _default_display_type_for_agent(
-        self, 
-        time_index: int, 
-        agent_index: int
+        self, time_index: int, agent_index: int
     ) -> DISPLAY_TYPE:
         """
-        Get the default DISPLAY_TYPE to use 
+        Get the default DISPLAY_TYPE to use
         given the number of subpoints for the agent
         at the given time and agent indices
         """
         n_subpoints = self.n_subpoints[time_index][agent_index]
+        if n_subpoints < 1:
+            return DISPLAY_TYPE.SPHERE
         default_display_types = {
-            4 : DISPLAY_TYPE.SPHERE_GROUP, 
-            3 : DISPLAY_TYPE.FIBER, 
-            1 : DISPLAY_TYPE.SPHERE,
+            4: DISPLAY_TYPE.SPHERE_GROUP,
+            3: DISPLAY_TYPE.FIBER,
+            1: DISPLAY_TYPE.SPHERE,
         }
         for values_per_item in default_display_types:
             if n_subpoints % float(values_per_item) == 0:
                 return default_display_types[values_per_item]
         return DISPLAY_TYPE.SPHERE
 
     def _check_subpoints_match_display_type(self):
```

### Comparing `simulariumio-1.7.1/simulariumio/data_objects/camera_data.py` & `simulariumio-1.8.0/simulariumio/data_objects/camera_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/data_objects/dimension_data.py` & `simulariumio-1.8.0/simulariumio/data_objects/dimension_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/data_objects/display_data.py` & `simulariumio-1.8.0/simulariumio/data_objects/display_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/data_objects/histogram_plot_data.py` & `simulariumio-1.8.0/simulariumio/data_objects/histogram_plot_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/data_objects/input_file_data.py` & `simulariumio-1.8.0/simulariumio/data_objects/input_file_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/data_objects/meta_data.py` & `simulariumio-1.8.0/simulariumio/data_objects/meta_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/data_objects/model_meta_data.py` & `simulariumio-1.8.0/simulariumio/data_objects/model_meta_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/data_objects/scatter_plot_data.py` & `simulariumio-1.8.0/simulariumio/data_objects/scatter_plot_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/data_objects/trajectory_data.py` & `simulariumio-1.8.0/simulariumio/data_objects/trajectory_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/data_objects/unit_data.py` & `simulariumio-1.8.0/simulariumio/data_objects/unit_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/exceptions.py` & `simulariumio-1.8.0/simulariumio/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,7 +38,21 @@
 
     def __init__(self, issue, **kwargs):
         super().__init__(**kwargs)
         self.issue = issue
 
     def __str__(self):
         return f"Problem with Data: '{self.issue}'."
+
+
+class InputDataError(Exception):
+    """
+    This exception is intended to communicate that an error occurred
+    while the input files were being read or parsed.
+    """
+
+    def __init__(self, issue, **kwargs):
+        super().__init__(**kwargs)
+        self.issue = issue
+
+    def __str__(self):
+        return f"Problem with input file: {self.issue}."
```

### Comparing `simulariumio-1.7.1/simulariumio/file_converter.py` & `simulariumio-1.8.0/simulariumio/file_converter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/filters/__init__.py` & `simulariumio-1.8.0/simulariumio/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/filters/add_agents_filter.py` & `simulariumio-1.8.0/simulariumio/filters/add_agents_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/filters/every_nth_agent_filter.py` & `simulariumio-1.8.0/simulariumio/filters/every_nth_agent_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/filters/every_nth_subpoint_filter.py` & `simulariumio-1.8.0/simulariumio/filters/every_nth_subpoint_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/filters/every_nth_timestep_filter.py` & `simulariumio-1.8.0/simulariumio/filters/every_nth_timestep_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/filters/filter.py` & `simulariumio-1.8.0/simulariumio/filters/filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/filters/multiply_space_filter.py` & `simulariumio-1.8.0/simulariumio/filters/multiply_space_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/filters/multiply_time_filter.py` & `simulariumio-1.8.0/simulariumio/filters/multiply_time_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/filters/transform_spatial_axes_filter.py` & `simulariumio-1.8.0/simulariumio/filters/transform_spatial_axes_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/filters/translate_filter.py` & `simulariumio-1.8.0/simulariumio/filters/translate_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/mcell/mcell_converter.py` & `simulariumio-1.8.0/simulariumio/mcell/mcell_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,69 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-from typing import Dict, Any
+from typing import Dict, Any, Callable
 import json
 import os
 import array
-
 import numpy as np
 import scipy.linalg as linalg
 from scipy.spatial.transform import Rotation
 
 from ..trajectory_converter import TrajectoryConverter
 from ..data_objects import (
     TrajectoryData,
     AgentData,
     UnitData,
     DimensionData,
 )
 from .mcell_data import McellData
 from ..constants import VALUES_PER_3D_POINT
+from ..exceptions import InputDataError
 
 ###############################################################################
 
 log = logging.getLogger(__name__)
 
 ###############################################################################
 
 
 BLENDER_GEOMETRY_SCALE_FACTOR = 0.005
 
 
 class McellConverter(TrajectoryConverter):
-    def __init__(self, input_data: McellData):
+    def __init__(
+        self,
+        input_data: McellData,
+        progress_callback: Callable[[float], None] = None,
+        callback_interval: float = 10,
+    ):
         """
         This object reads simulation trajectory outputs
         from MCell (https://mcell.org/)
         and plot data and writes them in the JSON format used
         by the Simularium viewer
 
         Parameters
         ----------
         input_data : McellData
             An object containing info for reading
             MCell simulation trajectory outputs and plot data
+        progress_callback : Callable[[float], None] (optional)
+            Callback function that accepts 1 float argument and returns None
+            which will be called at a given progress interval, determined by
+            callback_interval requested, providing the current percent progress
+            Default: None
+        callback_interval : float (optional)
+            If a progress_callback was provided, the period between updates
+            to be sent to the callback, in seconds
+            Default: 10
         """
+        super().__init__(input_data, progress_callback, callback_interval)
         self._data = self._read(input_data)
 
     @staticmethod
     def _normalize(v: np.ndarray) -> np.ndarray:
         """
         normalize a vector
         """
@@ -279,30 +294,36 @@
                     ] = rotations
                     result.n_agents[time_index] += n_mols
                 except EOFError:
                     mol_file.close()
                     break
         return result
 
-    @staticmethod
     def _read_cellblender_data(
+        self,
         timestep: float,
         molecule_list: Dict[str, Any],
         input_data: McellData,
     ) -> AgentData:
         """
         Parse cellblender binary files to get spatial data
         """
-        dimensions = McellConverter._get_dimensions_of_cellblender_data(
-            input_data.path_to_binary_files, input_data.nth_timestep_to_read
-        )
+        try:
+            dimensions = McellConverter._get_dimensions_of_cellblender_data(
+                input_data.path_to_binary_files, input_data.nth_timestep_to_read
+            )
+        except Exception as e:
+            raise InputDataError(f"Error reading Mcell binary files: {e}")
+
         result = AgentData.from_dimensions(dimensions)
         # get metadata for each agent type
         molecule_info = {}
         total_steps = 0
+        step_count = 0
+
         for molecule in molecule_list:
             molecule_info[molecule["mol_name"]] = molecule
         for file_name in os.listdir(input_data.path_to_binary_files):
             if not McellConverter._should_read_cellblender_binary_file(
                 file_name, input_data.nth_timestep_to_read
             ):
                 continue
@@ -314,31 +335,36 @@
             result = McellConverter._read_binary_cellblender_viz_frame(
                 os.path.join(input_data.path_to_binary_files, file_name),
                 time_index,
                 molecule_info,
                 input_data,
                 result,
             )
+            step_count += 1
+            self.check_report_progress(step_count / dimensions.total_steps)
         result.n_timesteps = total_steps + 1
         return result
 
-    @staticmethod
-    def _read(input_data: McellData) -> TrajectoryData:
+    def _read(self, input_data: McellData) -> TrajectoryData:
         """
         Return an object containing the data shaped for Simularium format
         """
         print("Reading MCell Data -------------")
         # read data model json
-        with open(input_data.path_to_data_model_json) as data_model_file:
-            data_model = json.load(data_model_file)
+        try:
+            with open(input_data.path_to_data_model_json) as data_model_file:
+                data_model = json.load(data_model_file)
+        except Exception as e:
+            raise InputDataError(f"Error reading Mcell file: {e}")
+
         # read spatial data
         time_units = UnitData(
             "s", float(data_model["mcell"]["initialization"]["time_step"])
         )
-        agent_data = McellConverter._read_cellblender_data(
+        agent_data = self._read_cellblender_data(
             time_units.magnitude,
             data_model["mcell"]["define_molecules"]["molecule_list"],
             input_data,
         )
         time_units.magnitude = 1
         # get box size
         partitions = data_model["mcell"]["initialization"]["partitions"]
```

### Comparing `simulariumio-1.7.1/simulariumio/mcell/mcell_data.py` & `simulariumio-1.8.0/simulariumio/mcell/mcell_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/md/md_converter.py` & `simulariumio-1.8.0/simulariumio/md/md_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 import copy
-from typing import Set
+from typing import Set, Callable
 
 import numpy as np
 import pandas as pd
 from MDAnalysis.topology.core import guess_atom_element
 from MDAnalysis.topology.tables import vdwradii
 
 from ..trajectory_converter import TrajectoryConverter
@@ -19,33 +19,48 @@
 
 log = logging.getLogger(__name__)
 
 ###############################################################################
 
 
 class MdConverter(TrajectoryConverter):
-    def __init__(self, input_data: MdData):
+    def __init__(
+        self,
+        input_data: MdData,
+        progress_callback: Callable[[float], None] = None,
+        callback_interval: float = 10,
+    ):
         """
         This object reads simulation trajectory outputs
         from molecular dynamics models
         and plot data and writes them in the format used
         by the Simularium viewer
 
         Parameters
         ----------
         input_data : MdData
             An object containing info for reading
             MD simulation trajectory outputs and plot data
+        progress_callback : Callable[[float], None] (optional)
+            Callback function that accepts 1 float argument and returns None
+            which will be called at a given progress interval, determined by
+            callback_interval requested, providing the current percent progress
+            Default: None
+        callback_interval : float (optional)
+            If a progress_callback was provided, the period between updates
+            to be sent to the callback, in seconds
+            Default: 10
         """
+        super().__init__(input_data, progress_callback, callback_interval)
         self._data = self._read(input_data)
 
     @staticmethod
     def _read_universe_dimensions(
         input_data: MdData,
-    ) -> AgentData:
+    ) -> DimensionData:
         """
         Use a MD Universe to get the number of timesteps
         and maximum agents per timestep
         """
         result = DimensionData(
             total_steps=0,
             max_agents=0,
@@ -119,16 +134,15 @@
                 type_name, input_data.display_data
             )
             if element_display_data:
                 display_data = copy.copy(element_display_data)
                 display_data.name = type_name
             else:
                 display_data = DisplayData(
-                    name=type_name,
-                    display_type=DISPLAY_TYPE.SPHERE
+                    name=type_name, display_type=DISPLAY_TYPE.SPHERE
                 )
         if display_data.color:
             return display_data
         display_data.color = color
         return display_data
 
     @staticmethod
@@ -143,26 +157,24 @@
         for raw_type_name in unique_raw_type_names:
             display_data = MdConverter._get_display_data_for_type(
                 raw_type_name, jmol_colors, input_data
             )
             result[display_data.name] = display_data
         return result
 
-    @staticmethod
-    def _read_universe(
-        input_data: MdData,
-    ) -> AgentData:
+    def _read_universe(self, input_data: MdData) -> AgentData:
         """
         Use a MD Universe to get AgentData
         """
         dimensions = MdConverter._read_universe_dimensions(input_data)
         result = AgentData.from_dimensions(dimensions)
         get_type_name_func = np.frompyfunc(MdConverter._get_type_name, 2, 1)
         unique_raw_type_names = set([])
         time_index = 0
+
         for frame in input_data.md_universe.trajectory[
             :: input_data.nth_timestep_to_read
         ]:
             result.times[time_index] = input_data.md_universe.trajectory.time
             atom_positions = input_data.md_universe.atoms.positions
             result.n_agents[time_index] = atom_positions.shape[0]
             result.unique_ids[time_index] = np.arange(atom_positions.shape[0])
@@ -176,28 +188,29 @@
             result.radii[time_index] = input_data.meta_data.scale_factor * np.array(
                 [
                     MdConverter._get_radius(type_name, input_data)
                     for type_name in input_data.md_universe.atoms.names
                 ]
             )
             time_index += 1
+            self.check_report_progress(time_index / dimensions.total_steps)
+
         result.n_timesteps = dimensions.total_steps
         result.display_data = MdConverter._get_display_data_mapping(
             unique_raw_type_names, input_data
         )
         return result
 
-    @staticmethod
-    def _read(input_data: MdData) -> TrajectoryData:
+    def _read(self, input_data: MdData) -> TrajectoryData:
         """
         Return a TrajectoryData object containing the MD data
         """
         print("Reading MD Data -------------")
         # get data from the MD Universe
-        agent_data = MdConverter._read_universe(input_data)
+        agent_data = self._read_universe(input_data)
         # create TrajectoryData
         input_data.spatial_units.multiply(1.0 / input_data.meta_data.scale_factor)
         input_data.meta_data._set_box_size()
         return TrajectoryData(
             meta_data=input_data.meta_data,
             agent_data=agent_data,
             time_units=input_data.time_units,
```

### Comparing `simulariumio-1.7.1/simulariumio/md/md_data.py` & `simulariumio-1.8.0/simulariumio/md/md_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/medyan/medyan_converter.py` & `simulariumio-1.8.0/simulariumio/medyan/medyan_converter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-from typing import List
+from typing import List, Callable
 import math
 
 from ..trajectory_converter import TrajectoryConverter
 from ..data_objects import (
     TrajectoryData,
     AgentData,
     UnitData,
@@ -15,37 +15,53 @@
 )
 from ..constants import (
     VIZ_TYPE,
     DISPLAY_TYPE,
     VALUES_PER_3D_POINT,
     SUBPOINT_VALUES_PER_ITEM,
 )
+from ..exceptions import InputDataError
 from .medyan_data import MedyanData
 
 ###############################################################################
 
 log = logging.getLogger(__name__)
 
 ###############################################################################
 
 
 class MedyanConverter(TrajectoryConverter):
-    def __init__(self, input_data: MedyanData):
+    def __init__(
+        self,
+        input_data: MedyanData,
+        progress_callback: Callable[[float], None] = None,
+        callback_interval: float = 10,
+    ):
         """
         This object reads simulation trajectory outputs
         from MEDYAN (http://medyan.org/)
         and plot data and writes them in the JSON format used
         by the Simularium viewer
 
         Parameters
         ----------
         input_data : MedyanData
             An object containing info for reading
             MEDYAN simulation trajectory outputs and plot data
+        progress_callback : Callable[[float], None] (optional)
+            Callback function that accepts 1 float argument and returns None
+            which will be called at a given progress interval, determined by
+            callback_interval requested, providing the current percent progress
+            Default: None
+        callback_interval : float (optional)
+            If a progress_callback was provided, the period between updates
+            to be sent to the callback, in seconds
+            Default: 10
         """
+        super().__init__(input_data, progress_callback, callback_interval)
         self._data = self._read(input_data)
 
     @staticmethod
     def _draw_endpoints(line: str, object_type: str, input_data: MedyanData) -> bool:
         """
         Parse a line of a MEDYAN snapshot.traj output file
         and determine whether to also draw the endpoints as spheres
@@ -128,21 +144,27 @@
                         result.max_subpoints = 2 * SUBPOINT_VALUES_PER_ITEM(
                             DISPLAY_TYPE.FIBER
                         )
         if agents > result.max_agents:
             result.max_agents = agents
         return result
 
-    @staticmethod
-    def _get_trajectory_data(input_data: MedyanData) -> AgentData:
+    def _get_trajectory_data(
+        self,
+        input_data: MedyanData,
+    ) -> AgentData:
         """
         Parse a MEDYAN snapshot.traj output file to get agents
         """
-        lines = input_data.snapshot_file.get_contents().split("\n")
-        dimensions = MedyanConverter._parse_data_dimensions(lines, input_data)
+        try:
+            lines = input_data.snapshot_file.get_contents().split("\n")
+            dimensions = MedyanConverter._parse_data_dimensions(lines, input_data)
+        except Exception as e:
+            raise InputDataError(f"Error reading input medyan data: {e}")
+
         result = AgentData.from_dimensions(dimensions)
         time_index = -1
         at_frame_start = True
         parsing_object = False
         uids = {
             "filament": {},
             "linker": {},
@@ -153,14 +175,16 @@
             "filament": {},
             "linker": {},
             "motor": {},
         }
         last_tid = 0
         object_type = ""
         draw_endpoints = False
+        line_count = 0
+
         for line in lines:
             if len(line) < 1:
                 at_frame_start = True
                 continue
             cols = line.split()
             if at_frame_start:
                 # start of timestep
@@ -249,24 +273,26 @@
                             dim_index
                         ] = input_data.meta_data.scale_factor * float(cols[i])
                 parsing_object = False
                 agent_index += 1
                 if draw_endpoints:
                     agent_index += 2
                     result.n_agents[time_index] += 2
+            line_count += 1
+            self.check_report_progress(line_count / len(lines))
+
         result.n_timesteps = time_index + 1
         return result
 
-    @staticmethod
-    def _read(input_data: MedyanData) -> TrajectoryData:
+    def _read(self, input_data: MedyanData) -> TrajectoryData:
         """
         Return an object containing the data shaped for Simularium format
         """
         print("Reading MEDYAN Data -------------")
-        agent_data = MedyanConverter._get_trajectory_data(input_data)
+        agent_data = self._get_trajectory_data(input_data)
         # get display data (geometry and color)
         for object_type in input_data.display_data:
             for tid in input_data.display_data[object_type]:
                 display_data = input_data.display_data[object_type][tid]
                 if (
                     display_data.display_type != DISPLAY_TYPE.NONE
                     and display_data.display_type != DISPLAY_TYPE.FIBER
```

### Comparing `simulariumio-1.7.1/simulariumio/medyan/medyan_data.py` & `simulariumio-1.8.0/simulariumio/medyan/medyan_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/package_data/jmolcolors.csv` & `simulariumio-1.8.0/simulariumio/package_data/jmolcolors.csv`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/physicell/dep/pyMCDS.py` & `simulariumio-1.8.0/simulariumio/physicell/dep/pyMCDS.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/physicell/physicell_converter.py` & `simulariumio-1.8.0/simulariumio/physicell/physicell_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 from simulariumio.data_objects.dimension_data import DimensionData
-from typing import Dict, Tuple, List
+from typing import Dict, Tuple, List, Callable
 from pathlib import Path
-
 import numpy as np
 import pandas as pd
 from .dep.pyMCDS import pyMCDS
 
 from ..trajectory_converter import TrajectoryConverter
 from ..data_objects import TrajectoryData, AgentData, UnitData, DisplayData
-from ..exceptions import MissingDataError, DataError
+from ..exceptions import MissingDataError, DataError, InputDataError
 from ..constants import (
     DISPLAY_TYPE,
     SUBPOINT_VALUES_PER_ITEM,
     DEFAULT_COLORS,
     VALUES_PER_3D_POINT,
 )
 from .physicell_data import PhysicellData
@@ -25,27 +24,42 @@
 
 log = logging.getLogger(__name__)
 
 ###############################################################################
 
 
 class PhysicellConverter(TrajectoryConverter):
-    def __init__(self, input_data: PhysicellData):
+    def __init__(
+        self,
+        input_data: PhysicellData,
+        progress_callback: Callable[[float], None] = None,
+        callback_interval: float = 10,
+    ):
         """
         This object reads simulation trajectory outputs
         from PhysiCell (http://physicell.org/)
         and plot data and writes them in the JSON format used
         by the Simularium viewer
 
         Parameters
         ----------
         input_data : PhysicellData
             An object containing info for reading
             PhysiCell simulation trajectory outputs and plot data
+        progress_callback : Callable[[float], None] (optional)
+            Callback function that accepts 1 float argument and returns None
+            which will be called at a given progress interval, determined by
+            callback_interval requested, providing the current percent progress
+            Default: None
+        callback_interval : float (optional)
+            If a progress_callback was provided, the period between updates
+            to be sent to the callback, in seconds
+            Default: 10
         """
+        super().__init__(input_data, progress_callback, callback_interval)
         self._data = self._read(input_data)
 
     @staticmethod
     def _load_data(
         path_to_output_dir: str, nth_timestep_to_read: int
     ) -> Tuple[List[pd.DataFrame], str]:
         """
@@ -144,43 +158,49 @@
     def _display_owner_number(owner_id: int, input_data: PhysicellData) -> bool:
         result = owner_id
         max_owners = input_data.max_owner_cells
         while result - max_owners > 0:
             result -= max_owners
         return result
 
-    @staticmethod
     def _get_trajectory_data(
+        self,
         input_data: PhysicellData,
     ) -> Tuple[AgentData, UnitData, Dict[int, Dict[int, int]]]:
         """
         Get data in Simularium format
         """
         type_ids = {}
         last_id = 0
         type_mapping = {}
-        discrete_cells, units = PhysicellConverter._load_data(
-            input_data.path_to_output_dir, input_data.nth_timestep_to_read
-        )
+        try:
+            discrete_cells, units = PhysicellConverter._load_data(
+                input_data.path_to_output_dir, input_data.nth_timestep_to_read
+            )
+        except Exception as e:
+            raise InputDataError(f"Error reading from Physicell output directory: {e}")
+
         dimensions = PhysicellConverter._get_dimensions(discrete_cells)
         result = AgentData.from_dimensions(dimensions)
         result.times = (
             input_data.nth_timestep_to_read
             * input_data.timestep
             * np.arange(dimensions.total_steps)
         )
         # get data
         max_subpoints = 0
         values_per_subcell = SUBPOINT_VALUES_PER_ITEM(DISPLAY_TYPE.SPHERE_GROUP)
         n_def_agents = []
         subcells = []
+
         for time_index in range(dimensions.total_steps):
             n_cells = int(len(discrete_cells[time_index]["position_x"]))
             n_def_agents.append(0)
             subcells.append({})
+            self.check_report_progress(time_index / (dimensions.total_steps * 2))
             for cell_index in range(n_cells):
                 cell_type_id = int(discrete_cells[time_index]["cell_type"][cell_index])
                 if PhysicellConverter._cell_is_subcell(cell_type_id, input_data):
                     # this is a subcell
                     if cell_type_id not in subcells[time_index]:
                         subcells[time_index][cell_type_id] = []
                     subcells[time_index][cell_type_id].append(cell_index)
@@ -242,14 +262,17 @@
                 max_subpoints,
             )
         )
         owner_cell_color_indices = {}
         next_color_index = 0
         for time_index in range(dimensions.total_steps):
             agent_index = n_def_agents[time_index]
+            self.check_report_progress(
+                (time_index + dimensions.total_steps) / (dimensions.total_steps * 2)
+            )
             for owner_id in subcells[time_index]:
                 if owner_id not in owner_cell_color_indices:
                     owner_cell_color_indices[owner_id] = next_color_index
                     next_color_index += 1
                     if next_color_index >= len(DEFAULT_COLORS):
                         next_color_index = 0
                 result.unique_ids[time_index][agent_index] = owner_id
@@ -304,23 +327,23 @@
         spatial_units = UnitData(
             units,
             1.0 / input_data.meta_data.scale_factor,
         )
         result.n_timesteps = dimensions.total_steps
         return result, spatial_units, type_ids
 
-    @staticmethod
-    def _read(input_data: PhysicellData) -> TrajectoryData:
+    def _read(
+        self,
+        input_data: PhysicellData,
+    ) -> TrajectoryData:
         """
         Return a TrajectoryData object containing the PhysiCell data
         """
         print("Reading PhysiCell Data -------------")
-        agent_data, spatial_units, type_ids = PhysicellConverter._get_trajectory_data(
-            input_data
-        )
+        agent_data, spatial_units, type_ids = self._get_trajectory_data(input_data)
         # get display data (geometry and color)
         for cell_id in input_data.display_data:
             display_data = input_data.display_data[cell_id]
             if cell_id not in type_ids:
                 raise DataError(
                     f"cell type ID {cell_id} provided in display_data "
                     "does not exist in PhysiCell data"
```

### Comparing `simulariumio-1.7.1/simulariumio/physicell/physicell_data.py` & `simulariumio-1.8.0/simulariumio/physicell/physicell_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/plot_readers/histogram_plot_reader.py` & `simulariumio-1.8.0/simulariumio/plot_readers/histogram_plot_reader.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/plot_readers/scatter_plot_reader.py` & `simulariumio-1.8.0/simulariumio/plot_readers/scatter_plot_reader.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/readdy/readdy_converter.py` & `simulariumio-1.8.0/simulariumio/readdy/readdy_converter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,73 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-from typing import Any, Tuple
+from typing import Any, Tuple, Callable
 
 import numpy as np
 import readdy
 
 from ..trajectory_converter import TrajectoryConverter
 from ..data_objects import TrajectoryData, AgentData, DimensionData, DisplayData
 from ..constants import DISPLAY_TYPE, VIZ_TYPE
 from .readdy_data import ReaddyData
+from ..exceptions import InputDataError
 
 ###############################################################################
 
 log = logging.getLogger(__name__)
 
 ###############################################################################
 
 
 class ReaddyConverter(TrajectoryConverter):
-    def __init__(self, input_data: ReaddyData):
+    def __init__(
+        self,
+        input_data: ReaddyData,
+        progress_callback: Callable[[float], None] = None,
+        callback_interval: float = 10,
+    ):
         """
         This object reads simulation trajectory outputs
         from ReaDDy (https://readdy.github.io/)
         and plot data and writes them in the JSON format used
         by the Simularium viewer
 
         Parameters
         ----------
         input_data : ReaddyData
             An object containing info for reading
             ReaDDy simulation trajectory outputs and plot data
+        progress_callback : Callable[[float], None] (optional)
+            Callback function that accepts 1 float argument and returns None
+            which will be called at a given progress interval, determined by
+            callback_interval requested, providing the current percent progress
+            Default: None
+        callback_interval : float (optional)
+            If a progress_callback was provided, the period between updates
+            to be sent to the callback, in seconds
+            Default: 10
         """
+        super().__init__(input_data, progress_callback, callback_interval)
         self._data = self._read(input_data)
 
     @staticmethod
     def _get_raw_trajectory_data(
         input_data: ReaddyData,
     ) -> Tuple[AgentData, Any, np.ndarray]:
         """
         Return agent data populated from a ReaDDy .h5 trajectory file
         """
         # load the trajectory
         traj = readdy.Trajectory(input_data.path_to_readdy_h5)
         n_agents, positions, type_ids, ids = traj.to_numpy(start=0, stop=None)
         return (traj, n_agents, positions, type_ids, ids)
 
-    @staticmethod
-    def _get_agent_data(
-        input_data: ReaddyData,
-    ) -> AgentData:
+    def _get_agent_data(self, input_data: ReaddyData) -> AgentData:
         """
         Pack raw ReaDDy trajectory data into AgentData,
         ignoring particles with type names in ignore_types
         """
         (
             traj,
             n_agents,
@@ -62,14 +75,15 @@
             type_ids,
             ids,
         ) = ReaddyConverter._get_raw_trajectory_data(input_data)
         data_dimensions = DimensionData(
             total_steps=n_agents.shape[0],
             max_agents=int(np.amax(n_agents)),
         )
+
         result = AgentData.from_dimensions(data_dimensions)
         result.times = input_data.timestep * np.arange(data_dimensions.total_steps)
         result.viz_types = VIZ_TYPE.DEFAULT * np.ones(
             shape=(data_dimensions.total_steps, data_dimensions.max_agents)
         )
         for time_index in range(data_dimensions.total_steps):
             new_agent_index = 0
@@ -78,15 +92,16 @@
                 if traj.species_name(tid) in input_data.ignore_types:
                     continue
                 raw_type_name = traj.species_name(tid)
                 input_display_data = TrajectoryConverter._get_display_data_for_agent(
                     raw_type_name, input_data.display_data
                 )
                 display_data = (
-                    input_display_data if input_display_data is not None
+                    input_display_data
+                    if input_display_data is not None
                     else DisplayData(
                         name=raw_type_name, display_type=DISPLAY_TYPE.SPHERE
                     )
                 )
                 result.unique_ids[time_index][new_agent_index] = ids[time_index][
                     agent_index
                 ]
@@ -97,23 +112,30 @@
                     * positions[time_index][agent_index]
                 )
                 result.radii[time_index][new_agent_index] = (
                     display_data.radius if display_data.radius is not None else 1.0
                 )
                 new_agent_index += 1
             result.n_agents[time_index] = new_agent_index
+            self.check_report_progress(time_index / data_dimensions.total_steps)
         return result
 
-    @staticmethod
-    def _read(input_data: ReaddyData) -> TrajectoryData:
+    def _read(
+        self,
+        input_data: ReaddyData,
+    ) -> TrajectoryData:
         """
         Return an object containing the data shaped for Simularium format
         """
         print("Reading ReaDDy Data -------------")
-        agent_data = ReaddyConverter._get_agent_data(input_data)
+        try:
+            agent_data = self._get_agent_data(input_data)
+        except Exception as e:
+            raise InputDataError(f"Error reading input Readdy data: {e}")
+
         # get display data (geometry and color)
         for tid in input_data.display_data:
             display_data = input_data.display_data[tid]
             agent_data.display_data[display_data.name] = display_data
         input_data.spatial_units.multiply(1.0 / input_data.meta_data.scale_factor)
         input_data.meta_data._set_box_size()
         return TrajectoryData(
```

### Comparing `simulariumio-1.7.1/simulariumio/readdy/readdy_data.py` & `simulariumio-1.8.0/simulariumio/readdy/readdy_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/readers/binary_info.py` & `simulariumio-1.8.0/simulariumio/readers/binary_info.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/readers/simularium_binary_reader.py` & `simulariumio-1.8.0/simulariumio/readers/simularium_binary_reader.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/smoldyn/smoldyn_converter.py` & `simulariumio-1.8.0/simulariumio/smoldyn/smoldyn_converter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,55 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-from typing import List
-
+from typing import List, Callable
 import numpy as np
 
 from ..trajectory_converter import TrajectoryConverter
 from ..data_objects import TrajectoryData, AgentData, DimensionData
+from ..exceptions import InputDataError
 from .smoldyn_data import SmoldynData
 
 ###############################################################################
 
 log = logging.getLogger(__name__)
 
 ###############################################################################
 
 
 class SmoldynConverter(TrajectoryConverter):
-    def __init__(self, input_data: SmoldynData):
+    def __init__(
+        self,
+        input_data: SmoldynData,
+        progress_callback: Callable[[float], None] = None,
+        callback_interval: float = 10,
+    ):
         """
         This object reads simulation trajectory outputs
         from Smoldyn (http://www.smoldyn.org)
         and plot data and writes them in the JSON format used
         by the Simularium viewer
 
         Parameters
         ----------
         input_data : SmoldynData
             An object containing info for reading
             Smoldyn simulation trajectory outputs and plot data
+        progress_callback : Callable [[float], None] (optional)
+            Callback function that accepts 1 float argument and returns None
+            which will be called at a given progress interval, determined by
+            callback_interval requested, providing the current percent progress
+            Default: None
+        callback_interval : float (optional)
+            If a progress_callback was provided, the period between updates
+            to be sent to the callback, in seconds
+            Default: 10
         """
+        super().__init__(input_data, progress_callback, callback_interval)
         self._data = self._read(input_data)
 
     @staticmethod
     def _parse_dimensions(smoldyn_data_lines: List[str]) -> DimensionData:
         """
         Parse Smoldyn output files to get the number of timesteps
         and maximum agents per timestep
@@ -50,39 +65,41 @@
                 result.total_steps += 1
             else:
                 agents += 1
         if agents > result.max_agents:
             result.max_agents = agents
         return result
 
-    @staticmethod
     def _parse_objects(
+        self,
         smoldyn_data_lines: List[str],
         input_data: SmoldynData,
     ) -> AgentData:
         """
         Parse a Smoldyn output file to get AgentData
         """
         dimensions = SmoldynConverter._parse_dimensions(smoldyn_data_lines)
         result = AgentData.from_dimensions(dimensions)
         time_index = -1
         agent_index = 0
+        line_count = 0
+
         for line in smoldyn_data_lines:
             if len(line) < 1:
                 continue
             cols = line.split()
             if len(cols) == 2:
                 if time_index >= 0:
                     result.n_agents[time_index] = agent_index
                 agent_index = 0
                 time_index += 1
                 result.times[time_index] = float(cols[0])
             else:
                 if len(cols) < 4:
-                    raise Exception(
+                    raise InputDataError(
                         "Smoldyn data is not formatted as expected, "
                         "please use the Smoldyn `listmols` command for output"
                     )
                 is_3D = len(cols) > 4
                 result.unique_ids[time_index][agent_index] = int(
                     cols[4] if is_3D else cols[3]
                 )
@@ -111,28 +128,33 @@
                     agent_index
                 ] = input_data.meta_data.scale_factor * (
                     input_display_data.radius
                     if input_display_data and input_display_data.radius is not None
                     else 1.0
                 )
                 agent_index += 1
+            line_count += 1
+            self.check_report_progress(line_count / len(smoldyn_data_lines))
+
         result.n_agents[time_index] = agent_index
         result.n_timesteps = time_index + 1
         return result
 
-    @staticmethod
-    def _read(input_data: SmoldynData) -> TrajectoryData:
+    def _read(self, input_data: SmoldynData) -> TrajectoryData:
         """
         Return a TrajectoryData object containing the Smoldyn data
         """
         print("Reading Smoldyn Data -------------")
         # load the data from Smoldyn output .txt file
-        smoldyn_data = input_data.smoldyn_file.get_contents().split("\n")
+        try:
+            smoldyn_data = input_data.smoldyn_file.get_contents().split("\n")
+        except Exception as e:
+            raise InputDataError(f"Error reading input smoldyn data: {e}")
         # parse
-        agent_data = SmoldynConverter._parse_objects(smoldyn_data, input_data)
+        agent_data = self._parse_objects(smoldyn_data, input_data)
         # get display data (geometry and color)
         for tid in input_data.display_data:
             display_data = input_data.display_data[tid]
             agent_data.display_data[display_data.name] = display_data
         # create TrajectoryData
         input_data.spatial_units.multiply(1.0 / input_data.meta_data.scale_factor)
         input_data.meta_data._set_box_size()
```

### Comparing `simulariumio-1.7.1/simulariumio/smoldyn/smoldyn_data.py` & `simulariumio-1.8.0/simulariumio/smoldyn/smoldyn_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/springsalad/springsalad_converter.py` & `simulariumio-1.8.0/simulariumio/springsalad/springsalad_converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-from typing import List, Tuple
-
+from typing import List, Tuple, Callable
 import numpy as np
 
 from ..trajectory_converter import TrajectoryConverter
 from ..data_objects import (
     TrajectoryData,
     AgentData,
     UnitData,
@@ -17,36 +16,52 @@
 from .springsalad_data import SpringsaladData
 from ..constants import (
     VIZ_TYPE,
     DISPLAY_TYPE,
     VALUES_PER_3D_POINT,
     SUBPOINT_VALUES_PER_ITEM,
 )
+from ..exceptions import InputDataError
 
 ###############################################################################
 
 log = logging.getLogger(__name__)
 
 ###############################################################################
 
 
 class SpringsaladConverter(TrajectoryConverter):
-    def __init__(self, input_data: SpringsaladData):
+    def __init__(
+        self,
+        input_data: SpringsaladData,
+        progress_callback: Callable[[float], None] = None,
+        callback_interval: float = 10,
+    ):
         """
         This object reads simulation trajectory outputs
         from SpringSaLaD (https://vcell.org/ssalad)
         and plot data and writes them in the JSON format used
         by the Simularium viewer
 
         Parameters
         ----------
         input_data : SpringsaladData
             An object containing info for reading
             SpringSaLaD simulation trajectory outputs and plot data
+        progress_callback : Callable[[float], None] (optional)
+            Callback function that accepts 1 float argument and returns None
+            which will be called at a given progress interval, determined by
+            callback_interval requested, providing the current percent progress
+            Default: None
+        callback_interval : float (optional)
+            If a progress_callback was provided, the period between updates
+            to be sent to the callback, in seconds
+            Default: 10
         """
+        super().__init__(input_data, progress_callback, callback_interval)
         self._data = self._read(input_data)
 
     @staticmethod
     def _parse_dimensions(
         springsalad_data: List[str], draw_bonds: bool
     ) -> DimensionData:
         """
@@ -67,30 +82,33 @@
                 agents += 1
             if draw_bonds and "Link" in line:  # line has data for a bond
                 agents += 1
         if agents > result.max_agents:
             result.max_agents = agents
         return result
 
-    @staticmethod
     def _parse_springsalad_data(
-        springsalad_data: List[str], input_data: SpringsaladData
+        self,
+        springsalad_data: List[str],
+        input_data: SpringsaladData,
     ) -> Tuple[AgentData, np.ndarray]:
         """
         Parse SpringSaLaD SIM_VIEW txt file to get spatial data
         """
         dimensions = SpringsaladConverter._parse_dimensions(
             springsalad_data, input_data.draw_bonds
         )
         result = AgentData.from_dimensions(dimensions)
         box_size = np.zeros(VALUES_PER_3D_POINT)
         time_index = -1
         agent_index = 0
         max_uid = 0
         scene_agent_positions = {}
+        line_count = 0
+
         for line in springsalad_data:
             cols = line.split()
             if "xsize" in line:
                 box_size[0] = 2 * float(cols[1])
             if "ysize" in line:
                 box_size[1] = 2 * float(cols[1])
             if "z_outside" in line:
@@ -133,15 +151,15 @@
             if input_data.draw_bonds and "Link" in line:  # line has data for a bond
                 particle1_id = int(cols[1])
                 particle2_id = int(cols[3])
                 if (
                     particle1_id not in scene_agent_positions
                     or particle2_id not in scene_agent_positions
                 ):
-                    raise Exception(
+                    raise InputDataError(
                         "Could not find particle ID connected by Link "
                         f"at timepoint {time_index} in SpringSaLaD data, "
                         "try converting without drawing bonds"
                     )
                 result.n_agents[time_index] += 1
                 result.viz_types[time_index][agent_index] = VIZ_TYPE.FIBER
                 result.unique_ids[time_index][agent_index] = max_uid
@@ -153,25 +171,29 @@
                 result.subpoints[time_index][agent_index][
                     0:VALUES_PER_3D_POINT
                 ] = scene_agent_positions[particle1_id]
                 result.subpoints[time_index][agent_index][
                     VALUES_PER_3D_POINT : 2 * VALUES_PER_3D_POINT
                 ] = scene_agent_positions[particle2_id]
                 agent_index += 1
+            line_count += 1
+            self.check_report_progress(line_count / len(springsalad_data))
         result.n_timesteps = time_index + 1
         return result, box_size
 
-    @staticmethod
-    def _read(input_data: SpringsaladData) -> TrajectoryData:
+    def _read(self, input_data: SpringsaladData) -> TrajectoryData:
         """
         Return an object containing the data shaped for Simularium format
         """
         print("Reading SpringSaLaD Data -------------")
-        springsalad_data = input_data.sim_view_txt_file.get_contents().split("\n")
-        agent_data, box_size = SpringsaladConverter._parse_springsalad_data(
+        try:
+            springsalad_data = input_data.sim_view_txt_file.get_contents().split("\n")
+        except Exception as e:
+            raise InputDataError(f"Error reading input SpringSaLaD data: {e}")
+        agent_data, box_size = self._parse_springsalad_data(
             springsalad_data, input_data
         )
         # get display data (geometry and color)
         for tid in input_data.display_data:
             display_data = input_data.display_data[tid]
             agent_data.display_data[display_data.name] = display_data
         if input_data.draw_bonds:
```

### Comparing `simulariumio-1.7.1/simulariumio/springsalad/springsalad_data.py` & `simulariumio-1.8.0/simulariumio/springsalad/springsalad_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/buffer/test_buffer_contents.py` & `simulariumio-1.8.0/simulariumio/tests/buffer/test_buffer_contents.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/buffer/test_buffer_size.py` & `simulariumio-1.8.0/simulariumio/tests/buffer/test_buffer_size.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/conftest.py` & `simulariumio-1.8.0/simulariumio/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,18 +176,14 @@
                         [13.32273796, -44.79360525, -24.91450698],
                         [21.93697483, 43.86451151, 4.10861266],
                         [44.97026158, -13.06491594, -7.16740679],
                     ],
                 ]
             ),
             display_data={
-                "C": DisplayData(
-                    name="C",
-                    display_type=DISPLAY_TYPE.SPHERE,
-                ),
                 "W": DisplayData(
                     name="W",
                     display_type=DISPLAY_TYPE.SPHERE,
                     color="#666",
                 ),
                 "S": DisplayData(
                     name="S",
```

### Comparing `simulariumio-1.7.1/simulariumio/tests/converters/test_cellpack_converter.py` & `simulariumio-1.8.0/simulariumio/tests/converters/test_cellpack_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import pytest
+from unittest.mock import Mock
 
 from simulariumio.cellpack import CellpackConverter, HAND_TYPE, CellpackData
 from simulariumio import InputFileData, UnitData, DisplayData, JsonWriter
 from simulariumio.constants import (
     DEFAULT_CAMERA_SETTINGS,
     DISPLAY_TYPE,
     VIZ_TYPE,
 )
+from simulariumio.exceptions import InputDataError
 
 
 data = CellpackData(
     results_file=InputFileData(
         file_path="simulariumio/tests/data/cellpack/mock_results.json"
     ),
     geometry_type=DISPLAY_TYPE.SPHERE,
@@ -250,7 +252,59 @@
     assert round(from_quat_right[0], 2) == round(from_matrix_right[0], 2)
     assert round(from_quat_right[1], 2) == round(from_matrix_right[1], 2)
     assert round(from_quat_right[2], 2) == round(from_matrix_right[2], 2)
 
     assert round(from_quat_left[0], 2) == round(from_matrix_left[0], 2)
     assert round(from_quat_left[1], 2) == round(from_matrix_left[1], 2)
     assert round(from_quat_left[2], 2) == round(from_matrix_left[2], 2)
+
+
+def test_input_file_error():
+    wrong_recipe_file = CellpackData(
+        results_file=InputFileData(
+            file_path="simulariumio/tests/data/cellpack/mock_results.json"
+        ),
+        geometry_type=DISPLAY_TYPE.SPHERE,
+        recipe_file_path="simulariumio/tests/data/cellpack/mock_results.json",
+    )
+    with pytest.raises(InputDataError):
+        CellpackConverter(wrong_recipe_file)
+
+    bad_file_type = CellpackData(
+        results_file=InputFileData(
+            file_path="simulariumio/tests/data/springsalad/broken_link.txt"
+        ),
+        geometry_type=DISPLAY_TYPE.SPHERE,
+        recipe_file_path="simulariumio/tests/data/cellpack/mock_recipe.json",
+    )
+    with pytest.raises(InputDataError):
+        CellpackConverter(bad_file_type)
+
+
+data = CellpackData(
+    results_file=InputFileData(
+        file_path="simulariumio/tests/data/cellpack/two_ingredients_results.json"
+    ),
+    geometry_type=DISPLAY_TYPE.OBJ,
+    recipe_file_path="simulariumio/tests/data/cellpack/two_ingredients_recipe.json",
+    time_units=UnitData("ns"),
+    spatial_units=UnitData("nm"),
+    handedness=HAND_TYPE.LEFT,
+    geometry_url="https://aics-simularium-data.s3.us-east-2.amazonaws.com/meshes/obj/",
+)
+
+
+def test_callback_fn():
+    callback_fn = Mock()
+    call_interval = 0.000000001
+    CellpackConverter(data, callback_fn, call_interval)
+    assert callback_fn.call_count > 1
+
+    # calls to the callback function should be strictly increasing
+    # and the value should never exceed 1.0 (100%)
+    call_list = callback_fn.call_args_list
+    last_call_val = 0.0
+    for call in call_list:
+        call_value = call.args[0]
+        assert call_value > last_call_val
+        assert call_value <= 1.0
+        last_call_val = call_value
```

### Comparing `simulariumio-1.7.1/simulariumio/tests/converters/test_cytosim_converter.py` & `simulariumio-1.8.0/simulariumio/tests/converters/test_cytosim_converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import pytest
 import numpy as np
+from unittest.mock import Mock
 
 from simulariumio import JsonWriter
 from simulariumio.cytosim import (
     CytosimConverter,
     CytosimData,
     CytosimObjectInfo,
 )
 from simulariumio import MetaData, DisplayData, InputFileData
 from simulariumio.constants import (
     DISPLAY_TYPE,
     DEFAULT_BOX_SIZE,
     VIZ_TYPE,
 )
+from simulariumio.exceptions import InputDataError
 
 data = CytosimData(
     object_info={
         "fibers": CytosimObjectInfo(
             cytosim_file=InputFileData(
                 file_path=(
                     "simulariumio/tests/data/cytosim/3_fibers_3_frames/test.txt"
@@ -334,7 +336,57 @@
 
 
 def test_parse_dimensions():
     dimension_data = CytosimConverter._parse_dimensions(cytosim_data)
     assert dimension_data.total_steps == 3
     assert dimension_data.max_agents == 19
     assert dimension_data.max_subpoints == 18
+
+
+def test_input_file_error():
+    # throws an error when the file is the right type, but is malformed
+    malformed_data = CytosimData(
+        object_info={
+            "fibers": CytosimObjectInfo(
+                cytosim_file=InputFileData(
+                    file_path=(
+                        "simulariumio/tests/data/malformed_data/malformed_cytosim.txt"
+                    ),
+                ),
+            )
+        },
+    )
+    with pytest.raises(InputDataError):
+        CytosimConverter(malformed_data)
+
+    # throws an error for a file type it can't read
+    wrong_file = CytosimData(
+        object_info={
+            "fibers": CytosimObjectInfo(
+                cytosim_file=InputFileData(
+                    file_path=(
+                        "simulariumio/tests/data/physicell/"
+                        "default_output/initial_cells.mat"
+                    ),
+                ),
+            )
+        },
+    )
+    with pytest.raises(InputDataError):
+        CytosimConverter(wrong_file)
+
+
+def test_callback_fn():
+    callback_fn_0 = Mock()
+    call_interval = 0.000000001
+    CytosimConverter(aster_pull3D_objects, callback_fn_0, call_interval)
+    assert callback_fn_0.call_count > 1
+
+    # calls to the callback function should be strictly increasing
+    # and the value should never exceed 1.0 (100%)
+    call_list = callback_fn_0.call_args_list
+    last_call_val = 0.0
+    for call in call_list:
+        call_value = call.args[0]
+        assert call_value > last_call_val
+        assert call_value <= 1.0
+        last_call_val = call_value
```

### Comparing `simulariumio-1.7.1/simulariumio/tests/converters/test_mcell_converter.py` & `simulariumio-1.8.0/simulariumio/tests/converters/test_mcell_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import pytest
-
+from unittest.mock import Mock
 import numpy as np
 
 from simulariumio.mcell import McellConverter, McellData
 from simulariumio import DisplayData, MetaData, JsonWriter
 from simulariumio.constants import (
     DEFAULT_CAMERA_SETTINGS,
     DISPLAY_TYPE,
     VIZ_TYPE,
 )
+from simulariumio.exceptions import InputDataError
 
 data = McellData(
     path_to_data_model_json="simulariumio/tests/data/mcell/"
     "organelle_model_viz_output/Scene.data_model.00.json",
     path_to_binary_files="simulariumio/tests/data/mcell/" "organelle_model_viz_output",
 )
 converter = McellConverter(data)
@@ -267,7 +268,42 @@
             [90.0, 0.0, 90.0],
         )
     ],
 )
 def test_get_euler_angles(v1, expected_result):
     euler_angles = McellConverter._get_euler_angles(v1, 45)
     assert (euler_angles == expected_result).all()
+
+
+def test_input_file_error():
+    invalid_json = McellData(
+        path_to_data_model_json="simulariumio/tests/data/md/example.xyz",
+        path_to_binary_files="simulariumio/tests/data/mcell/organelle_model_viz_output",
+    )
+    with pytest.raises(InputDataError):
+        McellConverter(invalid_json)
+
+    wrong_bin = McellData(
+        path_to_data_model_json="simulariumio/tests/data/mcell/"
+        "organelle_model_viz_output/Scene.data_model.00.json",
+        path_to_binary_files="simulariumio/tests/data/mcell/"
+        "organelle_model_example_files/mcell/output_data/react_data/seed_00001",
+    )
+    with pytest.raises(InputDataError):
+        McellConverter(wrong_bin)
+
+
+def test_callback_fn():
+    callback_fn_0 = Mock()
+    call_interval = 0.000000001
+    McellConverter(data, callback_fn_0, call_interval)
+    assert callback_fn_0.call_count > 1
+
+    # calls to the callback function should be strictly increasing
+    # and the value should never exceed 1.0 (100%)
+    call_list = callback_fn_0.call_args_list
+    last_call_val = 0.0
+    for call in call_list:
+        call_value = call.args[0]
+        assert call_value >= last_call_val
+        assert call_value <= 1.0
+        last_call_val = call_value
```

### Comparing `simulariumio-1.7.1/simulariumio/tests/converters/test_md_converter.py` & `simulariumio-1.8.0/simulariumio/tests/converters/test_md_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import pytest
 import numpy as np
+from unittest.mock import Mock
 from MDAnalysis import Universe
 
 from simulariumio.md import (
     MdConverter,
     MdData,
 )
 from simulariumio import MetaData, UnitData, DisplayData, JsonWriter
 from simulariumio.constants import (
     DEFAULT_CAMERA_SETTINGS,
     DEFAULT_BOX_SIZE,
     VIZ_TYPE,
-    DISPLAY_TYPE
+    DISPLAY_TYPE,
 )
 
 data = MdData(md_universe=Universe("simulariumio/tests/data/md/example.xyz"))
 converter = MdConverter(data)
 results = JsonWriter.format_trajectory_data(converter._data)
 
 
@@ -363,7 +364,24 @@
 def test_bundleData(bundleData, expected_bundleData):
     assert expected_bundleData == bundleData["data"]
 
 
 def test_agent_ids():
     assert JsonWriter._check_agent_ids_are_unique_per_frame(results_display_data)
     assert JsonWriter._check_agent_ids_are_unique_per_frame(results_nth_timestep)
+
+
+def test_callback_fn():
+    callback_fn_0 = Mock()
+    call_interval = 0.000000001
+    MdConverter(data, callback_fn_0, call_interval)
+    assert callback_fn_0.call_count > 1
+
+    # calls to the callback function should be strictly increasing
+    # and the value should never exceed 1.0 (100%)
+    call_list = callback_fn_0.call_args_list
+    last_call_val = 0.0
+    for call in call_list:
+        call_value = call.args[0]
+        assert call_value > last_call_val
+        assert call_value <= 1.0
+        last_call_val = call_value
```

### Comparing `simulariumio-1.7.1/simulariumio/tests/converters/test_medyan_converter.py` & `simulariumio-1.8.0/simulariumio/tests/converters/test_medyan_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pytest
+from unittest.mock import Mock
 
 from simulariumio.medyan import MedyanConverter, MedyanData
 from simulariumio import MetaData, DisplayData, InputFileData, JsonWriter
 from simulariumio.constants import (
     DEFAULT_BOX_SIZE,
     DEFAULT_CAMERA_SETTINGS,
     VIZ_TYPE,
-    DISPLAY_TYPE
+    DISPLAY_TYPE,
 )
+from simulariumio.exceptions import InputDataError
 
 data = MedyanData(
     snapshot_file=InputFileData(file_path="simulariumio/tests/data/medyan/test.traj"),
 )
 converter = MedyanConverter(data)
 results = JsonWriter.format_trajectory_data(converter._data)
 
@@ -476,7 +478,42 @@
 )
 def test_bundleData_drawing_endpoints(bundleData, expected_bundleData):
     assert expected_bundleData == bundleData["data"]
 
 
 def test_agent_ids_drawing_endpoints():
     assert JsonWriter._check_agent_ids_are_unique_per_frame(results_drawing_endpoints)
+
+
+def test_input_file_error():
+    # path to a file of the wrong format
+    wrong_file = MedyanData(
+        snapshot_file=InputFileData(file_path="simulariumio/tests/data/md/example.xyz"),
+    )
+    with pytest.raises(InputDataError):
+        MedyanConverter(wrong_file)
+
+    # file missing first frame start
+    invalid_traj = MedyanData(
+        snapshot_file=InputFileData(
+            file_path="simulariumio/tests/data/malformed_data/malformed_medyan.traj"
+        ),
+    )
+    with pytest.raises(InputDataError):
+        MedyanConverter(invalid_traj)
+
+
+def test_callback_fn():
+    callback_fn_0 = Mock()
+    call_interval = 0.000000001
+    MedyanConverter(data, callback_fn_0, call_interval)
+    assert callback_fn_0.call_count > 1
+
+    # calls to the callback function should be strictly increasing
+    # and the value should never exceed 1.0 (100%)
+    call_list = callback_fn_0.call_args_list
+    last_call_val = 0.0
+    for call in call_list:
+        call_value = call.args[0]
+        assert call_value > last_call_val
+        assert call_value <= 1.0
+        last_call_val = call_value
```

### Comparing `simulariumio-1.7.1/simulariumio/tests/converters/test_physicell_converter.py` & `simulariumio-1.8.0/simulariumio/tests/converters/test_physicell_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pytest
+from unittest.mock import Mock
 
 from simulariumio.physicell import PhysicellConverter, PhysicellData
 from simulariumio import MetaData, DisplayData, JsonWriter, UnitData
 from simulariumio.constants import (
     DEFAULT_BOX_SIZE,
     DEFAULT_COLORS,
     DISPLAY_TYPE,
-    VIZ_TYPE
+    VIZ_TYPE,
 )
+from simulariumio.exceptions import InputDataError
 
 data = PhysicellData(
     timestep=360.0,
     path_to_output_dir="simulariumio/tests/data/physicell/default_output/",
 )
 converter = PhysicellConverter(data)
 results = JsonWriter.format_trajectory_data(converter._data)
@@ -673,16 +675,16 @@
                 0,
                 1.0,
                 4,
                 0,
                 0,
                 0,
                 0,
-            ]
-        )
+            ],
+        ),
     ],
 )
 def test_bundleData(bundleData, expected_bundleData):
     assert False not in np.isclose(
         np.array(expected_bundleData),
         np.array(bundleData["data"]),
     )
@@ -702,15 +704,52 @@
                     box_size=np.array([1000.0, 1000.0, 100.0]),
                     scale_factor=0.01,
                 ),
                 "timestep": 360.0,
                 "path_to_output_dir": "../simulariumio/tests/data/physicell/",
             },
             {},
-            marks=pytest.mark.raises(exception=AttributeError),
+            marks=pytest.mark.raises(exception=InputDataError),
         ),
     ],
 )
 def test_bad_path_to_output_dir(trajectory, expected_data):
     converter = PhysicellConverter(trajectory)
     buffer_data = JsonWriter.format_trajectory_data(converter._data)
     assert expected_data == buffer_data
+
+
+def test_input_file_error():
+    # path to a file, not a directory
+    invalid_data_0 = PhysicellData(
+        timestep=360.0,
+        path_to_output_dir=(
+            "simulariumio/tests/data/physicell/default_output/output00000000.xml",
+        )
+    )
+    with pytest.raises(InputDataError):
+        PhysicellConverter(invalid_data_0)
+
+    # path to directory with no output files
+    invalid_data_1 = PhysicellData(
+        timestep=360.0,
+        path_to_output_dir="simulariumio/tests/data/physicell/",
+    )
+    with pytest.raises(InputDataError):
+        PhysicellConverter(invalid_data_1)
+
+
+def test_callback_fn():
+    callback_fn_0 = Mock()
+    call_interval = 0.000000001
+    PhysicellConverter(data, callback_fn_0, call_interval)
+    assert callback_fn_0.call_count > 1
+
+    # calls to the callback function should be strictly increasing
+    # and the value should never exceed 1.0 (100%)
+    call_list = callback_fn_0.call_args_list
+    last_call_val = -1.0
+    for call in call_list:
+        call_value = call.args[0]
+        assert call_value > last_call_val
+        assert call_value <= 1.0 and call_value >= 0.0
+        last_call_val = call_value
```

### Comparing `simulariumio-1.7.1/simulariumio/tests/converters/test_readdy_converter.py` & `simulariumio-1.8.0/simulariumio/tests/converters/test_readdy_converter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pytest
+from unittest.mock import Mock
 
 from simulariumio.readdy import ReaddyConverter, ReaddyData
 from simulariumio import UnitData, MetaData, DisplayData, JsonWriter
 from simulariumio.constants import (
     DEFAULT_CAMERA_SETTINGS,
     DISPLAY_TYPE,
     DEFAULT_BOX_SIZE,
     VIZ_TYPE,
 )
+from simulariumio.exceptions import InputDataError
 
 
 data = ReaddyData(
     timestep=0.1,
     path_to_readdy_h5="simulariumio/tests/data/readdy/test.h5",
 )
 converter = ReaddyConverter(data)
@@ -420,7 +422,42 @@
 )
 def test_bundleData_ignored_types(bundleData, expected_bundleData):
     assert expected_bundleData == bundleData["data"]
 
 
 def test_agent_ids_ignored_types():
     assert JsonWriter._check_agent_ids_are_unique_per_frame(results_display_data)
+
+
+def test_input_file_error():
+    # a .txt file should trigger an error when trying to read the data
+    txt_file = ReaddyData(
+        timestep=0.1,
+        path_to_readdy_h5="simulariumio/tests/data/smoldyn/example_data.txt",
+    )
+    with pytest.raises(InputDataError):
+        ReaddyConverter(txt_file)
+
+    # also expect an error for a json file
+    json_file = ReaddyData(
+        timestep=0.1,
+        path_to_readdy_h5="simulariumio/tests/data/cellpack/mock_results.json",
+    )
+    with pytest.raises(InputDataError):
+        ReaddyConverter(json_file)
+
+
+def test_callback_fn():
+    callback_fn_0 = Mock()
+    call_interval = 0.000000001
+    ReaddyConverter(data, callback_fn_0, call_interval)
+    assert callback_fn_0.call_count > 1
+
+    # calls to the callback function should be strictly increasing
+    # and the value should never exceed 1.0 (100%)
+    call_list = callback_fn_0.call_args_list
+    last_call_val = -1.0
+    for call in call_list:
+        call_value = call.args[0]
+        assert call_value > last_call_val
+        assert call_value <= 1.0 and call_value >= 0.0
+        last_call_val = call_value
```

### Comparing `simulariumio-1.7.1/simulariumio/tests/converters/test_smoldyn_converter.py` & `simulariumio-1.8.0/simulariumio/tests/converters/test_smoldyn_converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import pytest
 import numpy as np
+from unittest.mock import Mock
 
 from simulariumio.smoldyn import (
     SmoldynConverter,
     SmoldynData,
 )
 from simulariumio import MetaData, UnitData, DisplayData, InputFileData, JsonWriter
 from simulariumio.constants import (
     DEFAULT_BOX_SIZE,
     DEFAULT_CAMERA_SETTINGS,
     DISPLAY_TYPE,
     VIZ_TYPE,
 )
+from simulariumio.exceptions import InputDataError
 
 data = SmoldynData(
     smoldyn_file=InputFileData(
         file_path="simulariumio/tests/data/smoldyn/example_data.txt"
     )
 )
 converter = SmoldynConverter(data)
@@ -457,7 +459,47 @@
                 0.0,
             ],
         )
     ],
 )
 def test_bundleData_3D(bundleData, expected_bundleData):
     assert expected_bundleData == bundleData["data"]
+
+
+def test_input_file_error():
+    # malformed_smoldyn.txt is missing a column for some agents
+    malformed_data = SmoldynData(
+        smoldyn_file=InputFileData(
+            file_path="simulariumio/tests/data/malformed_data/malformed_smoldyn.txt"
+        )
+    )
+    with pytest.raises(InputDataError):
+        SmoldynConverter(malformed_data)
+
+    # also expect an error for a file of the wrong file type
+    wrong_file = SmoldynData(
+        smoldyn_file=InputFileData(file_path="simulariumio/tests/data/readdy/test.h5")
+    )
+    with pytest.raises(InputDataError):
+        SmoldynConverter(wrong_file)
+
+
+def test_callback_fn():
+    data = SmoldynData(
+        smoldyn_file=InputFileData(
+            file_path="simulariumio/tests/data/smoldyn/example_2D.txt"
+        )
+    )
+    callback_fn_0 = Mock()
+    call_interval = 0.000000001
+    SmoldynConverter(data, callback_fn_0, call_interval)
+    assert callback_fn_0.call_count > 1
+
+    # calls to the callback function should be strictly increasing
+    # and the value should never exceed 1.0 (100%)
+    call_list = callback_fn_0.call_args_list
+    last_call_val = 0.0
+    for call in call_list:
+        call_value = call.args[0]
+        assert call_value > last_call_val
+        assert call_value <= 1.0
+        last_call_val = call_value
```

### Comparing `simulariumio-1.7.1/simulariumio/tests/converters/test_springsalad_converter.py` & `simulariumio-1.8.0/simulariumio/tests/converters/test_springsalad_converter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pytest
+from unittest.mock import Mock
 
 from simulariumio.springsalad import SpringsaladConverter, SpringsaladData
 from simulariumio import DisplayData, MetaData, InputFileData, JsonWriter
 from simulariumio.constants import (
     DEFAULT_CAMERA_SETTINGS,
     DISPLAY_TYPE,
     DEFAULT_BOX_SIZE,
     VIZ_TYPE,
 )
+from simulariumio.exceptions import InputDataError
 
 
 data = SpringsaladData(
     sim_view_txt_file=InputFileData(
         file_path=("simulariumio/tests/data/springsalad/test.txt"),
     ),
     draw_bonds=False,
@@ -415,7 +417,48 @@
 )
 def test_bundleData_bonds(bundleData, expected_bundleData):
     assert expected_bundleData == bundleData["data"]
 
 
 def test_agent_ids_bonds():
     assert JsonWriter._check_agent_ids_are_unique_per_frame(results_display_data)
+
+
+def test_input_file_error():
+    # springsalad_broken_link.txt is makes a link with an agent that doesn't exist
+    data = SpringsaladData(
+        sim_view_txt_file=InputFileData(
+            file_path=(
+                "simulariumio/tests/data/malformed_data/springsalad_broken_link.txt"
+            )
+        ),
+        draw_bonds=True,
+    )
+    with pytest.raises(InputDataError):
+        SpringsaladConverter(data)
+
+    # also expect an error for a file of the wrong file type
+    wrong_file = SpringsaladData(
+        sim_view_txt_file=InputFileData(
+            file_path="simulariumio/tests/data/readdy/test.h5"
+        ),
+        draw_bonds=False,
+    )
+    with pytest.raises(InputDataError):
+        SpringsaladConverter(wrong_file)
+
+
+def test_callback_fn():
+    callback_fn_0 = Mock()
+    callback_interval = 0.0000001
+    SpringsaladConverter(data, callback_fn_0, callback_interval)
+    assert callback_fn_0.call_count > 1
+
+    # calls to the callback function should be strictly increasing
+    # and the value should never exceed 1.0 (100%)
+    call_list = callback_fn_0.call_args_list
+    last_call_val = 0.0
+    for call in call_list:
+        call_value = call.args[0]
+        assert call_value > last_call_val
+        assert call_value <= 1.0
+        last_call_val = call_value
```

### Comparing `simulariumio-1.7.1/simulariumio/tests/converters/test_trajectory_converter.py` & `simulariumio-1.8.0/simulariumio/tests/converters/test_trajectory_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         (
             fiber_agents_data["trajectoryInfo"]["version"],
             CURRENT_VERSION.TRAJECTORY_INFO,
         ),
         (
             sphere_group_data["trajectoryInfo"]["version"],
             CURRENT_VERSION.TRAJECTORY_INFO,
-        )
+        ),
     ],
 )
 def test_versions_trajectory(trajectory_version, expected_version):
     assert trajectory_version == expected_version
 
 
 # test time units
@@ -1339,15 +1339,15 @@
                     1.0,
                     8.0,
                     9.0,
                     2.0,
                 ],
             },
         ),
-    ]
+    ],
 )
 def test_bundle_data_sphere_group(data, expected_data):
     assert data == expected_data
 
 
 # test plot data
 @pytest.mark.parametrize(
```

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/binary/50filaments_motor_linker_binary.binary` & `simulariumio-1.8.0/simulariumio/tests/data/binary/50filaments_motor_linker_binary.binary`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/binary/binary_test.binary` & `simulariumio-1.8.0/simulariumio/tests/data/binary/binary_test.binary`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cellpack/example_2D_recipe.json` & `simulariumio-1.8.0/simulariumio/tests/data/cellpack/example_2D_recipe.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cellpack/example_2D_results.json` & `simulariumio-1.8.0/simulariumio/tests/data/cellpack/example_2D_results.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cellpack/mock_recipe.json` & `simulariumio-1.8.0/simulariumio/tests/data/cellpack/mock_recipe.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cellpack/mock_results.json` & `simulariumio-1.8.0/simulariumio/tests/data/cellpack/mock_results.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/3_fibers_3_frames/fiber_points.txt` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/3_fibers_3_frames/fiber_points.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/3_fibers_3_frames/test.txt` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/3_fibers_3_frames/test.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/aster_pull3D_couple_actin_solid.cym` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/aster_pull3D_couple_actin_solid.cym`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/couples.txt` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/couples.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/fiber_points.txt` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/fiber_points.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/singles.txt` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/singles.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/solids.txt` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/solids.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couple_actin_solid.cym` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couple_actin_solid.cym`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames.json` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames_small.json` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames_small.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/couples.txt` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/couples.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/fiber_points.txt` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/fiber_points.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/singles.txt` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/singles.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/solids.txt` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/solids.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/cytosim/fiber_test/fiber_points.txt` & `simulariumio-1.8.0/simulariumio/tests/data/cytosim/fiber_test/fiber_points.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example.blend` & `simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example.blend`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.geometry.mdl` & `simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.geometry.mdl`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.initialization.mdl` & `simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.initialization.mdl`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.instantiation.mdl` & `simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.instantiation.mdl`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.data_model.00.json` & `simulariumio-1.8.0/simulariumio/tests/data/mcell/organelle_model_viz_output/Scene.data_model.00.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/medyan/snapshot.traj` & `simulariumio-1.8.0/simulariumio/tests/data/medyan/snapshot.traj`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/medyan/test.traj` & `simulariumio-1.8.0/simulariumio/tests/data/medyan/test.traj`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/initial.xml` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/initial.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/initial_cells_physicell.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/initial_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/initial_mesh0.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/initial_mesh0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/initial_microenvironment0.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/initial_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000000.xml` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000000.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000000_cells_physicell.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000000_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000000_microenvironment0.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000000_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000001.xml` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000001.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000001_cells_physicell.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000001_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000001_microenvironment0.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000001_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000002.xml` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000002.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000002_cells_physicell.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000002_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/default_output/output00000002_microenvironment0.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/default_output/output00000002_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/initial.xml` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/initial.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/initial_cells.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/initial_cells.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/initial_cells_physicell.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/initial_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/initial_mesh0.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/initial_mesh0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/initial_microenvironment0.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/initial_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000000.xml` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000000.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000000_cells.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000000_cells.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000000_cells_physicell.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000000_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000000_microenvironment0.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000000_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000001.xml` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000001.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000001_cells.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000001_cells.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000001_cells_physicell.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000001_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000001_microenvironment0.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000001_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000002.xml` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000002.xml`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000002_cells.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000002_cells.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000002_cells_physicell.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000002_cells_physicell.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/physicell/subcell_output/output00000002_microenvironment0.mat` & `simulariumio-1.8.0/simulariumio/tests/data/physicell/subcell_output/output00000002_microenvironment0.mat`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/readdy/test.h5` & `simulariumio-1.8.0/simulariumio/tests/data/readdy/test.h5`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/springsalad/Simulation0_SIM_VIEW_Run0.txt` & `simulariumio-1.8.0/simulariumio/tests/data/springsalad/Simulation0_SIM_VIEW_Run0.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/data/springsalad/test.txt` & `simulariumio-1.8.0/simulariumio/tests/data/springsalad/test.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/filters/test_add_agents_filter.py` & `simulariumio-1.8.0/simulariumio/tests/filters/test_add_agents_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/filters/test_every_nth_agent_filter.py` & `simulariumio-1.8.0/simulariumio/tests/filters/test_every_nth_agent_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/filters/test_every_nth_subpoint_filter.py` & `simulariumio-1.8.0/simulariumio/tests/filters/test_every_nth_subpoint_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/filters/test_every_nth_timestep_filter.py` & `simulariumio-1.8.0/simulariumio/tests/filters/test_every_nth_timestep_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/filters/test_multiply_space_filter.py` & `simulariumio-1.8.0/simulariumio/tests/filters/test_multiply_space_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/filters/test_multiply_time_filter.py` & `simulariumio-1.8.0/simulariumio/tests/filters/test_multiply_time_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/filters/test_transform_spatial_axes_filter.py` & `simulariumio-1.8.0/simulariumio/tests/filters/test_transform_spatial_axes_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/filters/test_translate_filter.py` & `simulariumio-1.8.0/simulariumio/tests/filters/test_translate_filter.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/filters/test_translate_filter_sphere_groups.py` & `simulariumio-1.8.0/simulariumio/tests/filters/test_translate_filter_sphere_groups.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/plot_readers/test_histogram_plot_reader.py` & `simulariumio-1.8.0/simulariumio/tests/plot_readers/test_histogram_plot_reader.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/plot_readers/test_scatter_plot_reader.py` & `simulariumio-1.8.0/simulariumio/tests/plot_readers/test_scatter_plot_reader.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/readers/test_binary_reader.py` & `simulariumio-1.8.0/simulariumio/tests/readers/test_binary_reader.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/test_from_dict.py` & `simulariumio-1.8.0/simulariumio/tests/test_from_dict.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/test_input_file_data.py` & `simulariumio-1.8.0/simulariumio/tests/test_input_file_data.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/tests/writers/test_binary_writer.py` & `simulariumio-1.8.0/simulariumio/tests/writers/test_binary_writer.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/utils.py` & `simulariumio-1.8.0/simulariumio/utils.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/writers/binary_chunk.py` & `simulariumio-1.8.0/simulariumio/writers/binary_chunk.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/writers/binary_values.py` & `simulariumio-1.8.0/simulariumio/writers/binary_values.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/writers/binary_writer.py` & `simulariumio-1.8.0/simulariumio/writers/binary_writer.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/writers/json_writer.py` & `simulariumio-1.8.0/simulariumio/writers/json_writer.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio/writers/writer.py` & `simulariumio-1.8.0/simulariumio/writers/writer.py`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/simulariumio.egg-info/PKG-INFO` & `simulariumio-1.8.0/simulariumio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulariumio
-Version: 1.7.1
+Version: 1.8.0
 Summary: Python package that converts simulation outputs to the format consumed by the Simularium viewer website
 Author-email: Blair Lyons <blairl@alleninstitute.org>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://github.com/Simularium/simulariumio
 Project-URL: Bug Tracker, https://github.com/Simularium/simulariumio/issues
 Project-URL: Documentation, https://Simularium.github.io/simulariumio
 Project-URL: User Support, https://github.com/Simularium/simulariumio/issues
```

### Comparing `simulariumio-1.7.1/simulariumio.egg-info/SOURCES.txt` & `simulariumio-1.8.0/simulariumio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 simulariumio/smoldyn/smoldyn_converter.py
 simulariumio/smoldyn/smoldyn_data.py
 simulariumio/springsalad/__init__.py
 simulariumio/springsalad/springsalad_converter.py
 simulariumio/springsalad/springsalad_data.py
 simulariumio/tests/__init__.py
 simulariumio/tests/conftest.py
+simulariumio/tests/test_agents_from_lists.py
 simulariumio/tests/test_from_dict.py
 simulariumio/tests/test_input_file_data.py
 simulariumio/tests/buffer/test_buffer_contents.py
 simulariumio/tests/buffer/test_buffer_size.py
 simulariumio/tests/converters/test_cellpack_converter.py
 simulariumio/tests/converters/test_cytosim_converter.py
 simulariumio/tests/converters/test_mcell_converter.py
@@ -133,14 +134,16 @@
 simulariumio/tests/converters/test_trajectory_converter.py
 simulariumio/tests/data/binary/50filaments_motor_linker_binary.binary
 simulariumio/tests/data/binary/binary_test.binary
 simulariumio/tests/data/cellpack/example_2D_recipe.json
 simulariumio/tests/data/cellpack/example_2D_results.json
 simulariumio/tests/data/cellpack/mock_recipe.json
 simulariumio/tests/data/cellpack/mock_results.json
+simulariumio/tests/data/cellpack/two_ingredients_recipe.json
+simulariumio/tests/data/cellpack/two_ingredients_results.json
 simulariumio/tests/data/cytosim/3_fibers_3_frames/fiber_points.txt
 simulariumio/tests/data/cytosim/3_fibers_3_frames/test.txt
 simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/aster_pull3D_couple_actin_solid.cym
 simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/couples.txt
 simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/fiber_points.txt
 simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/singles.txt
 simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid/solids.txt
@@ -148,14 +151,18 @@
 simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames.json
 simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/aster_pull3D_couples_actin_solid_3_frames_small.json
 simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/couples.txt
 simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/fiber_points.txt
 simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/singles.txt
 simulariumio/tests/data/cytosim/aster_pull3D_couples_actin_solid_3_frames/solids.txt
 simulariumio/tests/data/cytosim/fiber_test/fiber_points.txt
+simulariumio/tests/data/malformed_data/malformed_cytosim.txt
+simulariumio/tests/data/malformed_data/malformed_medyan.traj
+simulariumio/tests/data/malformed_data/malformed_smoldyn.txt
+simulariumio/tests/data/malformed_data/springsalad_broken_link.txt
 simulariumio/tests/data/mcell/organelle_model_example.blend
 simulariumio/tests/data/mcell/organelle_model_example_files/start_time.txt
 simulariumio/tests/data/mcell/organelle_model_example_files/mcell/data_layout.json
 simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.geometry.mdl
 simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.initialization.mdl
 simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.instantiation.mdl
 simulariumio/tests/data/mcell/organelle_model_example_files/mcell/output_data/Scene.main.mdl
```

### Comparing `simulariumio-1.7.1/simulariumio.egg-info/requires.txt` & `simulariumio-1.8.0/simulariumio.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/README.md` & `simulariumio-1.8.0/ui-templates/README.md`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/base_types.json` & `simulariumio-1.8.0/ui-templates/base_types.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/cellpack_data.json` & `simulariumio-1.8.0/ui-templates/cellpack_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/custom-types/camera_data.json` & `simulariumio-1.8.0/ui-templates/custom-types/camera_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/custom-types/coordinates_xyz.json` & `simulariumio-1.8.0/ui-templates/custom-types/coordinates_xyz.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/custom-types/cytosim_object_info.json` & `simulariumio-1.8.0/ui-templates/custom-types/cytosim_object_info.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/custom-types/display_data.json` & `simulariumio-1.8.0/ui-templates/custom-types/display_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/custom-types/meta_data.json` & `simulariumio-1.8.0/ui-templates/custom-types/meta_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/custom-types/model_meta_data.json` & `simulariumio-1.8.0/ui-templates/custom-types/model_meta_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/custom-types/space_unit_data.json` & `simulariumio-1.8.0/ui-templates/custom-types/space_unit_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/custom-types/time_unit_data.json` & `simulariumio-1.8.0/ui-templates/custom-types/time_unit_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/cytosim_data.json` & `simulariumio-1.8.0/ui-templates/cytosim_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/medyan_data.json` & `simulariumio-1.8.0/ui-templates/medyan_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/smoldyn_data.json` & `simulariumio-1.8.0/ui-templates/smoldyn_data.json`

 * *Files identical despite different names*

### Comparing `simulariumio-1.7.1/ui-templates/springsalad_data.json` & `simulariumio-1.8.0/ui-templates/springsalad_data.json`

 * *Files identical despite different names*

