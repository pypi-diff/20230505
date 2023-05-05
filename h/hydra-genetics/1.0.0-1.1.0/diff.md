# Comparing `tmp/hydra-genetics-1.0.0.tar.gz` & `tmp/hydra-genetics-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra-genetics-1.0.0.tar", last modified: Mon Feb 20 12:33:20 2023, max compression
+gzip compressed data, was "hydra-genetics-1.1.0.tar", last modified: Fri May  5 06:56:22 2023, max compression
```

## Comparing `hydra-genetics-1.0.0.tar` & `hydra-genetics-1.1.0.tar`

### file list

```diff
@@ -1,115 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.972874 hydra-genetics-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-02-20 12:33:20.972874 hydra-genetics-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.972874 hydra-genetics-1.0.0/hydra_genetics/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-20 12:33:20.972874 hydra-genetics-1.0.0/hydra_genetics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.964874 hydra-genetics-1.0.0/hydra_genetics/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/linters/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/linters/.snakefmt.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/linters/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/linters/report/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/conventional-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/release-please.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.964874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.tests/integration/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.tests/integration/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.tests/integration/samples.tsv
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.tests/integration/units.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/config/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/config/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/config/samples.tsv
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/config/units.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/images/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/images/generate_dag.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/Snakefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/envs/dummy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/notebooks/describe_jupyter_notebook.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/report/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/report/describe_workflow.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/rules/common.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/schemas/samples.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/scripts/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/scripts/test_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/rule-template/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/rule-template/skeleton_env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/rule-template/skeleton_rule.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.968874 hydra-genetics-1.0.0/hydra_genetics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.972874 hydra-genetics-1.0.0/hydra_genetics/utils/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/utils/io/chr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/utils/io/hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/utils/io/hotspot_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/utils/io/multibp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/utils/io/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/utils/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.972874 hydra-genetics-1.0.0/hydra_genetics/utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/utils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/utils/models/hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/utils/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/hydra_genetics/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.964874 hydra-genetics-1.0.0/hydra_genetics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-02-20 12:33:20.000000 hydra-genetics-1.0.0/hydra_genetics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-02-20 12:33:20.000000 hydra-genetics-1.0.0/hydra_genetics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 12:33:20.000000 hydra-genetics-1.0.0/hydra_genetics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-20 12:33:20.000000 hydra-genetics-1.0.0/hydra_genetics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 12:33:20.000000 hydra-genetics-1.0.0/hydra_genetics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-20 12:33:20.000000 hydra-genetics-1.0.0/hydra_genetics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-20 12:33:20.000000 hydra-genetics-1.0.0/hydra_genetics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-20 12:33:20.972874 hydra-genetics-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.972874 hydra-genetics-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.972874 hydra-genetics-1.0.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.972874 hydra-genetics-1.0.0/tests/utils/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/tests/utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/tests/utils/io/test_hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)    67196 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/tests/utils/io/test_mutations_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:20.972874 hydra-genetics-1.0.0/tests/utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/tests/utils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/tests/utils/models/test_hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/tests/utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/tests/utils/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/tests/utils/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    27613 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/tests/utils/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-02-20 12:33:13.000000 hydra-genetics-1.0.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/hydra_genetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/hydra_genetics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33225 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/commands/prep_pipeline_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/linters/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/linters/.snakefmt.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/linters/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/linters/report/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/conventional-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/release-please.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.587232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.tests/integration/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.tests/integration/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.tests/integration/samples.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.tests/integration/units.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/config/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/config/samples.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/config/units.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/includes/abbreviations.md
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/softwares.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    61275 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/images/hydragenetics.png
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/Snakefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/notebooks/describe_jupyter_notebook.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/report/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/report/describe_workflow.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/rules/common.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/rules/dummy.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/schemas/rules.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/schemas/samples.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/scripts/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/scripts/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/hydra_genetics/rule-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/rule-template/config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/rule-template/resources.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/rule-template/rules.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/rule-template/skeleton_rule.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/rule-template/softwares.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/hydra_genetics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/hydra_genetics/utils/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/io/chr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/io/hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/io/hotspot_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/io/multibp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/io/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/hydra_genetics/utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/models/hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-05 06:56:22.000000 hydra-genetics-1.1.0/hydra_genetics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-05 06:56:22.000000 hydra-genetics-1.1.0/hydra_genetics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 06:56:22.000000 hydra-genetics-1.1.0/hydra_genetics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 06:56:22.000000 hydra-genetics-1.1.0/hydra_genetics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 06:56:22.000000 hydra-genetics-1.1.0/hydra_genetics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-05 06:56:22.000000 hydra-genetics-1.1.0/hydra_genetics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 06:56:22.000000 hydra-genetics-1.1.0/hydra_genetics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/tests/utils/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/io/test_hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67196 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/io/test_mutations_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/tests/utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/models/test_hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/versioneer.py
```

### Comparing `hydra-genetics-1.0.0/LICENSE.md` & `hydra-genetics-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/PKG-INFO` & `hydra-genetics-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: hydra-genetics
-Version: 1.0.0
+Version: 1.1.0
 Summary: Helper tools for use with hydra-genetics pipelines.
 Home-page: https://github.com/hydra-genetics/tools
 Author: Patrik Smeds
 Author-email: patrik.smeds@scilifelab.uu.se
 License: GPL-3
 Keywords: hydra-genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next generation sequencing
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 
-# Hydra-genetics
+# <img src="images/hydragenetics.png" width=40 /> Hydra-genetics
 
 Command line interface to create new modules/pipelines or adding a new rule to an existing project. Provides libraries used to make it easier for people not used to pandas to extract information from samples and units dataframes. These dataframes are generated from [units.tsv](https://github.com/hydra-genetics/tools/blob/develop/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml) and [samples.tsv](https://github.com/hydra-genetics/prealignment/blob/develop/workflow/schemas/samples.schema.yaml) files which are used as input.
 
 [![Lint and Test](https://github.com/hydra-genetics/tools/actions/workflows/main.yaml/badge.svg?branch=develop)](https://github.com/hydra-genetics/tools/actions/workflows/main.yaml)
 
 ![python](https://img.shields.io/badge/python-3.8-blue)
 
@@ -39,8 +39,12 @@
  # -t/--tool can be skipped for a single command tool, ex a script
  # this will create a smk file named "super_script.smk" with a rule "super_script"
  hydra-genetics create-rule -c rule3 -t samtools -m snv -a test2 -e "test@test"
 
  # Create input files
  hydra-genetics create-input-files -d path/dir1 -d path/dir2
 
+ # Create singularity cache
+ # all container specified in config.yaml will be fetched
+ hydra-genetics singularity create-singularity-files  -o singularity_cache -c config.yaml
+
 ```
```

### Comparing `hydra-genetics-1.0.0/README.md` & `hydra-genetics-1.1.0/hydra_genetics.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,21 @@
+Metadata-Version: 2.1
+Name: hydra-genetics
+Version: 1.1.0
+Summary: Helper tools for use with hydra-genetics pipelines.
+Home-page: https://github.com/hydra-genetics/tools
+Author: Patrik Smeds
+Author-email: patrik.smeds@scilifelab.uu.se
+License: GPL-3
+Keywords: hydra-genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next generation sequencing
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
-# Hydra-genetics
+
+# <img src="images/hydragenetics.png" width=40 /> Hydra-genetics
 
 Command line interface to create new modules/pipelines or adding a new rule to an existing project. Provides libraries used to make it easier for people not used to pandas to extract information from samples and units dataframes. These dataframes are generated from [units.tsv](https://github.com/hydra-genetics/tools/blob/develop/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml) and [samples.tsv](https://github.com/hydra-genetics/prealignment/blob/develop/workflow/schemas/samples.schema.yaml) files which are used as input.
 
 [![Lint and Test](https://github.com/hydra-genetics/tools/actions/workflows/main.yaml/badge.svg?branch=develop)](https://github.com/hydra-genetics/tools/actions/workflows/main.yaml)
 
 ![python](https://img.shields.io/badge/python-3.8-blue)
 
@@ -27,8 +39,12 @@
  # -t/--tool can be skipped for a single command tool, ex a script
  # this will create a smk file named "super_script.smk" with a rule "super_script"
  hydra-genetics create-rule -c rule3 -t samtools -m snv -a test2 -e "test@test"
 
  # Create input files
  hydra-genetics create-input-files -d path/dir1 -d path/dir2
 
+ # Create singularity cache
+ # all container specified in config.yaml will be fetched
+ hydra-genetics singularity create-singularity-files  -o singularity_cache -c config.yaml
+
 ```
```

### Comparing `hydra-genetics-1.0.0/hydra_genetics/__init__.py` & `hydra-genetics-1.1.0/hydra_genetics/__init__.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/__main__.py` & `hydra-genetics-1.1.0/hydra_genetics/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import click
 import logging
 import os
 import re
 import sys
 
 import hydra_genetics.utils
+from hydra_genetics.commands.prep_pipeline_env import environment
 from hydra_genetics.commands.create import PipelineCreate, RuleCreate, CreateInputFiles
 import rich.console
 import rich.logging
 import rich.traceback
 
 # Set up logging as the root logger
 # Submodules should all traverse back to this
@@ -74,22 +75,22 @@
         value = click.prompt(opts.prompt)
         return validate_wf_name_prompt(ctx, opts, value)
     return value
 
 
 def validate_rule_name_prompt(ctx, opts, value):
     """Force the rule name to meet the hydra-core requirements"""
-    if not re.match(r"^[a-z0-9_]+$", value):
+    if value is not None and not re.match(r"^[a-z0-9_]+$", value):
         click.echo("Invalid command/tool formatting: only lowercase and '_' is allowed.")
         value = click.prompt(opts.prompt)
         return validate_rule_name_prompt(ctx, opts, value)
     return value
 
 
-@cli.command(short_help="create bare bone project")
+@cli.command(short_help="create bare bone project, pipeline or module")
 @click.option(
     "-n",
     "--name",
     prompt="Workflow Name",
     required=True,
     callback=validate_wf_name_prompt,
     type=str,
@@ -100,15 +101,15 @@
 @click.option("-e", "--email", prompt=True, required=True, type=str, help="E-mail(s) of the main author(s)")
 @click.option("--version", type=str, default="0.0.1", help="The initial version number to use")
 @click.option("--min-snakemake-version", type=str, default="6.8.0", help="Min snakemake version")
 @click.option("-g", "--git-user", prompt=True, required=True, help="User name of main git user(s)")
 @click.option("--no-git", is_flag=True, default=False, help="Do not create git repo")
 @click.option("-f", "--force", is_flag=True, default=False, help="Overwrite output directory if it already exists")
 @click.option("-o", "--outdir", type=str, help="Output directory for new pipeline (default: pipeline name)")
-def create_module(name, description, author, email, version, min_snakemake_version, git_user, no_git, force, outdir):
+def create_pipeline(name, description, author, email, version, min_snakemake_version, git_user, no_git, force, outdir):
     pipeline = PipelineCreate(name, description, author, email, version, min_snakemake_version, git_user, no_git, force, outdir)
     pipeline.init_pipeline()
 
 
 @cli.command(short_help="add rule to project")
 @click.option(
     "-c",
@@ -118,29 +119,29 @@
     callback=validate_rule_name_prompt,
     type=str,
     help="command that will be run, will be used to name the rule",
 )
 @click.option(
     "-t",
     "--tool",
-    prompt="tool used run command (optional)",
     required=False,
     callback=validate_rule_name_prompt,
     type=str,
     default=None,
-    help="tool that will be used to run the command, if provided it will be used during the naming of the rule, ex samtools",
+    help="tool that will be used to run the command, if provided it will be used during the naming of the "
+         "rule, ex samtools, optional",
 )
 @click.option(
     "-m",
     "--module",
     prompt="name of module/workflow",
     required=True,
     callback=validate_wf_name_prompt,
     type=str,
-    help="name module/workflow where rule will be added. Expected folder structure is module_name/workflow/, "
+    help="name module/pipeline where rule will be added. Expected folder structure is module_name_or_pipeline/workflow/, "
          " the rule will be added to a subfolder named rules, env.yaml to a subfolder named envs.")
 @click.option(
         "-a",
         "--author",
         prompt=True,
         required=True,
         type=str,
@@ -154,15 +155,14 @@
         help="E-mail(s) of the main author(s)")
 @click.option(
         "-o",
         "--outdir",
         type=str,
         help="Output directory for where module is located (default: current dir)")
 def create_rule(command, tool, module, author, email, outdir):
-    print(": ".join([command, tool, module, author, email, str(outdir)]))
     rule = RuleCreate(command, module, author, email, tool, outdir)
     rule.init_rule()
 
 
 @cli.command(short_help="create input-files, samples.tsv and units.tsv")
 @click.option(
     "-d",
@@ -262,9 +262,11 @@
 
 
 @cli.command(short_help="download reference data")
 def referece_data():
     pass
 
 
+cli.add_command(environment)
+
 if __name__ == "__main__":
     run()
```

### Comparing `hydra-genetics-1.0.0/hydra_genetics/commands/create.py` & `hydra-genetics-1.1.0/hydra_genetics/commands/create.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import glob
 import gzip
 import logging
 import jinja2
 import pathlib
 import os
 import re
+import shutil
 import sys
 import hydra_genetics
 
 log = logging.getLogger(__name__)
 
 
 class PipelineCreate(object):
@@ -91,21 +92,26 @@
                         log.info("Use -f / --force to overwrite existing files")
                         sys.exit(1)
                 else:
                     os.makedirs(output_path)
                 continue
 
             log.debug(f"Rendering template file: '{template_fn}'")
-            j_template = env.get_template(template_fn)
-            rendered_output = j_template.render(object_attrs)
 
-            # Write to the pipeline output file
-            with open(output_path, "w") as fh:
-                log.debug(f"Writing to output file: '{output_path}'")
-                fh.write(rendered_output)
+            if template_fn.endswith(".png"):
+                print(template_fn)
+                shutil.copy(template_fn, output_path)
+            else:
+                j_template = env.get_template(template_fn)
+                rendered_output = j_template.render(object_attrs)
+
+                # Write to the pipeline output file
+                with open(output_path, "w") as fh:
+                    log.debug(f"Writing to output file: '{output_path}'")
+                    fh.write(rendered_output)
 
         if not self.no_git:
             self.git_init_pipeline()
 
     def git_init_pipeline(self):
         """Initialises the new pipeline as a Git repository and submits first commit."""
         log.info("Initialising pipeline git repository")
@@ -152,53 +158,92 @@
         outdir = os.path.normpath(os.path.join(self.outdir, self.module_name))
         if not os.path.exists(outdir):
             outdir_temp = outdir
             outdir = os.path.join(os.path.dirname(self.outdir), self.module_name)
             if not os.path.exists(outdir):
                 log.error(f"Can not find module directory, tried with:\n'{outdir_temp}'\n'{outdir}'")
                 exit(1)
-        outdir = os.path.join(outdir, "workflow")
-        output_rules = os.path.join(outdir, "rules")
-        output_envs = os.path.join(outdir, "envs")
+        outdir_workflow = os.path.join(outdir, "workflow")
+        # Rule path
+        output_rules = os.path.join(outdir_workflow, "rules")
+
+        # Schema path
+        output_schemas = os.path.join(outdir_workflow, "schemas")
+        output_schemas_config = os.path.join(output_schemas, "config.schema.yaml")
+        output_schemas_resources = os.path.join(output_schemas, "resources.schema.yaml")
+        output_schemas_rule = os.path.join(output_schemas, "rules.schema.yaml")
+
+        # Docs software path
+        output_docs_software = os.path.join(outdir, "docs", "softwares.md")
+
         if not os.path.exists(output_rules):
             log.error(f"Can not find output directory '{output_rules}'")
             sys.exit(2)
-        if not os.path.exists(output_envs):
-            log.error(f"Can not find output directory '{output_envs}' exists!")
-            sys.exit(3)
         self.append_rule = False
         self.name = self.command
         if self.tool is None:
-            log.info(f"Creating rule: '{output_rules}/{self.command}.smk'")
+            self.filename_rulename = f"{self.name}__{self.name}"
+            log.info(f"Creating rule: '{output_rules}/{self.name}.smk'")
+            output_rule = os.path.join(output_rules, f"{self.name}.smk")
         else:
             self.name = f"{self.tool}_{self.name}"
+            self.filename_rulename = f"{self.tool}__{self.name}"
             if os.path.exists(os.path.join(output_rules, f"{self.tool}.smk")):
                 log.info(f"Adding entry {self.name} to smk '{outdir}/{self.tool}.smk'")
                 output_rule = os.path.join(output_rules, f"{self.tool}.smk")
-                output_env = os.path.join(output_envs, f"{self.tool}.yaml")
                 self.append_rule = True
             else:
                 log.info(f"Creating smk file: '{output_rules}/{self.tool}.smk' with rule {self.name}")
                 output_rule = os.path.join(output_rules, f"{self.tool}.smk")
-                output_env = os.path.join(output_envs, f"{self.tool}.yaml")
         if os.path.exists(output_rule) and self.tool is None:
             log.error(f"Rule already exists '{output_rule}'")
             sys.exit(4)
-        if os.path.exists(output_env) and self.tool is None:
-            log.error(f"env file already exists '{output_env}'")
-            sys.exit(5)
+
+        if not os.path.exists(output_schemas):
+            log.info(f"Creating schema folder {output_schemas}")
+            os.mkdir(output_schemas)
+
+        if not os.path.exists(output_schemas_config):
+            log.info(f"Creating config schema file {output_schemas_config}")
+            self.append_schema_config = False
+        else:
+            log.info(f"Appending to config schema file {output_schemas_config}")
+            self.append_schema_config = True
+
+        if not os.path.exists(output_schemas_resources):
+            log.info(f"Creating resources schema file {output_schemas_resources}")
+            self.append_schema_resources = False
+        else:
+            log.info(f"Appending to resources schema file {output_schemas_resources}")
+            self.append_schema_resources = True
+
+        if not os.path.exists(output_schemas_rule):
+            log.info(f"Creating rule schema file {output_schemas_rule}")
+            self.append_schema_rule = False
+        else:
+            log.info(f"Appending to rule schema file {output_schemas_rule}")
+            self.append_schema_rule = True
+
+        if not os.path.exists(output_docs_software):
+            log.info(f"Creating docs file {output_docs_software}")
+            self.append_docs_software = False
+            parent_dir = os.path.dirname(output_docs_software)
+            if not os.path.exists(parent_dir):
+                os.mkdir(parent_dir)
+        else:
+            log.info(f"Appending to docs file {output_docs_software}")
+            self.append_docs_software = True
+
         env = jinja2.Environment(
             loader=jinja2.PackageLoader("hydra_genetics", "rule-template"), keep_trailing_newline=True
         )
         template_dir = os.path.join(os.path.dirname(__file__), "../rule-template")
         rename_files = {
             "skeleton_rule.smk": output_rule,
         }
-        if self.tool is None or not self.append_rule:
-            rename_files["skeleton_env.yaml"] = os.path.join("envs", f"{self.tool}.yaml")
         object_attrs = vars(self)
         template_files = list(pathlib.Path(template_dir).glob("**/*"))
         ignore_strs = [".pyc", "__pycache__", ".pyo", ".pyd", ".DS_Store", ".egg", ".snakemake"]
         if self.append_rule:
             with open(output_rule, 'r') as lines:
                 for line in lines:
                     if self.name in line:
@@ -208,28 +253,56 @@
         for template_fn_path_obj in template_files:
             template_fn_path = str(template_fn_path_obj)
             if any([s in template_fn_path for s in ignore_strs]):
                 log.debug(f"Ignoring '{template_fn_path}' in jinja2 template creation")
                 continue
 
             template_fn = os.path.relpath(template_fn_path, template_dir)
-            output_path = os.path.join(outdir, template_fn)
+            if template_fn.endswith(".smk"):
+                output_path = output_rules
+                self.append = self.append_rule
+            elif template_fn.endswith("config.schema.yaml"):
+                output_path = output_schemas_config
+                self.append = self.append_schema_config
+            elif template_fn.endswith("rules.schema.yaml"):
+                output_path = output_schemas_rule
+                self.append = self.append_schema_rule
+            elif template_fn.endswith("resources.schema.yaml"):
+                output_path = output_schemas_resources
+                self.append = self.append_schema_resources
+            elif template_fn.endswith(".md"):
+                output_path = output_docs_software
+                self.append = self.append_docs_software
+
             if template_fn in rename_files:
                 output_path = os.path.join(outdir, rename_files[template_fn])
 
-            log.debug(f"Rendering template file: '{template_fn}'")
+            log.info(f"Rendering template file: '{template_fn}' at {output_path}")
             j_template = env.get_template(template_fn)
-            rendered_output = j_template.render(object_attrs)
+            rendered_output = j_template.render(object_attrs, trim_blocks=False)
 
-            # Write to the pipeline output file
-            with open(output_path, "w" if not self.append_rule else "a") as fh:
-                log.debug(f"Writing to output file: '{output_path}'")
-                fh.write(rendered_output)
-
-        snakefile = os.path.join(outdir, "Snakefile")
+            if os.path.exists(output_path):
+                with open(output_path, "r+") as fh:
+                    lines = fh.readlines()
+                    line_number = 0
+                    for line in lines:
+                        if line.startswith('required:'):
+                            break
+                        else:
+                            line_number += 1
+                    fh.seek(0)
+                    lines.insert(line_number, rendered_output)
+                    log.info(f"Appending to output file: '{output_path}'")
+                    fh.writelines(lines)
+            else:
+                # Write to the content to a new file
+                with open(output_path, "w") as fh:
+                    log.info(f"Writing to new output file: '{output_path}'")
+                    fh.write(rendered_output)
+        snakefile = os.path.join(outdir_workflow, "Snakefile")
         with open(snakefile, 'r+') as fh:
             lines = fh.readlines()
             line_number = 0
             for line in lines:
                 line_number += 1
                 if line.startswith('include: "rules/common.smk"'):
                     break
```

### Comparing `hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md` & `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md` & `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md` & `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml` & `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -8,44 +8,14 @@
      - develop
      - master
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 jobs:
-  integration-small-conda:
-    name: integration small data set conda
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-      - name: Set up Python 3.8
-        uses: actions/setup-python@v3
-        with:
-          python-version: 3.8
-      - name: Setup Mambaforge
-        uses: conda-incubator/setup-miniconda@v2
-        with:
-            miniforge-variant: Mambaforge
-            miniforge-version: latest
-            activate-environment: my-env
-            use-mamba: true
-      - name: Set strict channels
-        run: |
-          conda config --set channel_priority strict
-      - name: Install requirements.txt
-        run: |
-          pip install -r requirements.txt
-      - name: Install requirements.test.txt
-        run: |
-          pip install -r requirements.test.txt
-      - name: Integration test - small dataset
-        working-directory: .tests/integration
-        run: |
-          mamba install -c conda-forge -c bioconda snakemake
-          snakemake -s ../../workflow/Snakefile -j 1 --use-conda --configfile config.yaml
   integration-small-singularity:
     name: integration small data set singularity
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python 3.8
         uses: actions/setup-python@v3
@@ -66,11 +36,14 @@
           pip install -r requirements.txt
       - name: Install requirements.test.txt
         run: |
           pip install -r requirements.test.txt
       - name: Install singularity
         run: |
           mamba install -c conda-forge -c bioconda singularity=3.8.6
+      - name: Add conda to system path
+        run: |
+          echo $CONDA/bin >> $GITHUB_PATH
       - name: Integration test - small dataset
         working-directory: .tests/integration
         run: |
           snakemake -s ../../workflow/Snakefile -j 1 --show-failed-logs --configfile config.yaml  --use-singularity --singularity-args  " --cleanenv --bind /home/runner "
```

### Comparing `hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml` & `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml` & `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml` & `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml` & `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml` & `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/pipeline-template/LICENSE.md` & `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/pipeline-template/README.md` & `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# :snake: hydra-genetics/{{ short_name }}
+# <img src="images/hydragenetics.png" width=40 /> hydra-genetics/{{ short_name }}
 
 #### {{ description }}
 
 ![Lint](https://github.com/hydra-genetics/{{ short_name }}/actions/workflows/lint.yaml/badge.svg?branch=develop)
 ![Snakefmt](https://github.com/hydra-genetics/{{ short_name }}/actions/workflows/snakefmt.yaml/badge.svg?branch=develop)
 ![snakemake dry run](https://github.com/hydra-genetics/{{ short_name }}/actions/workflows/snakemake-dry-run.yaml/badge.svg?branch=develop)
 ![integration test](https://github.com/hydra-genetics/{{ short_name }}/actions/workflows/integration1.yaml/badge.svg?branch=develop)
```

### Comparing `hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/Snakefile` & `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/rules/dummy.smk`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 __author__ = "{{ author }}"
 __copyright__ = "Copyright {{ year }}, {{ author }}"
 __email__ = "{{ email }}"
 __license__ = "GPL-3"
 
-include: "rules/common.smk"
-
-report: "report/workflow.rst"
 
 rule dummy:
     output:
-        "{{ short_name }}/dummy/{sample}_{type}.dummy.txt"
+        OUTPUT1="{{ short_name }}/dummy/{sample}_{type}.dummy.txt"
     params:
         extra=config.get("dummy", {}).get("extra", ""),
     log:
         "{{ short_name }}/dummy/{sample}_{type}.output.log"
     benchmark:
        repeat("module/dummy/{sample}_{type}.output.benchmark.tsv", config.get("dummy", {}).get("benchmark_repeats", 1),)
     threads: # optional
        threads=config.get("dummy", {}).get("threads", config["default_resources"]["threads"]),
     resources:
         threads=config.get("dummy", {}).get("threads", config["default_resources"]["threads"]),
         time=config.get("dummy", {}).get("time", config["default_resources"]["time"]),
     container:
        config.get("dummy", {}).get("container", config["default_container"])
-    conda:
-       "../envs/dummy.yaml"
     message:
        "{rule}: Do stuff on module/{rule}/{wildcards.sample}_{wildcards.type}.input"
     shell:
         """
         touch {output}
         """
-
-rule all:
-    input:
-        unpack(compile_output_list),
```

### Comparing `hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/rules/common.smk` & `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/rules/common.smk`

 * *Files 14% similar despite different names*

```diff
@@ -12,30 +12,37 @@
 from hydra_genetics.utils.units import *
 
 min_version("{{ min_snakemake_version }}")
 
 ### Set and validate config file
 
 if not workflow.overwrite_configfiles:
-    sys.exit("At least one config file must be passed using --configfile/--configfiles, by command line or a profile!")
+    sys.exit(
+        "At least one config file must be passed using --configfile/--configfiles, by command line or a profile!"
+    )
 
 
 validate(config, schema="../schemas/config.schema.yaml")
 config = load_resources(config, config["resources"])
 validate(config, schema="../schemas/resources.schema.yaml")
 
 
 ### Read and validate samples file
 
 samples = pd.read_table(config["samples"], dtype=str).set_index("sample", drop=False)
 validate(samples, schema="../schemas/samples.schema.yaml")
 
 ### Read and validate units file
 
-units = pandas.read_table(config["units"], dtype=str).set_index(["sample", "type", "flowcell", "lane", "barcode"], drop=False).sort_index()
+units = (
+    pandas.read_table(config["units"], dtype=str)
+    .set_index(["sample", "type", "flowcell", "lane", "barcode"], drop=False)
+    .sort_index()
+)
+
 validate(units, schema="../schemas/units.schema.yaml")
 
 ### Set wildcard constraints
 
 
 wildcard_constraints:
     sample="|".join(samples.index),
```

### Comparing `hydra-genetics-1.0.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml` & `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/rule-template/skeleton_rule.smk` & `hydra-genetics-1.1.0/hydra_genetics/rule-template/skeleton_rule.smk`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 
 {% else %}
 
 {% endif -%}
 rule {{ name }}:
     input:
-        "...",
+        input1="...",
     output:
-        "{{ module_name }}/{{ name }}/{sample}_{type}.output.txt",
+        output1="{{ module_name }}/{{ name }}/{sample}_{type}.output.txt",
     params:
         extra=config.get("{{ name }}", {}).get("extra", ""),
     log:
         "{{ module_name }}/{{ name }}/{sample}_{type}.output.log",
     benchmark:
         repeat(
             "{{ module_name }}/{{ name }}/{sample}_{type}.output.benchmark.tsv",
@@ -27,13 +27,11 @@
         mem_mb=config.get("{{ name }}", {}).get("mem_mb", config["default_resources"]["mem_mb"]),
         mem_per_cpu=config.get("{{ name }}", {}).get("mem_per_cpu", config["default_resources"]["mem_per_cpu"]),
         partition=config.get("{{ name }}", {}).get("partition", config["default_resources"]["partition"]),
         threads=config.get("{{ name }}", {}).get("threads", config["default_resources"]["threads"]),
         time=config.get("{{ name }}", {}).get("time", config["default_resources"]["time"]),
     container:
         config.get("{{ name }}", {}).get("container", config["default_container"])
-    conda:
-        "../envs/{{ name }}.yaml"
     message:
         "{rule}: Do stuff on {{ module_name }}/{rule}/{wildcards.sample}_{wildcards.type}.input"
     wrapper:
         "..."
```

### Comparing `hydra-genetics-1.0.0/hydra_genetics/utils/io/chr.py` & `hydra-genetics-1.1.0/hydra_genetics/utils/io/chr.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/utils/io/hotspot.py` & `hydra-genetics-1.1.0/hydra_genetics/utils/io/hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/utils/io/hotspot_report.py` & `hydra-genetics-1.1.0/hydra_genetics/utils/io/hotspot_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
                     break
             if added:
                 break
         if not added:
             other.append(variant)
     log.info("Open genomic vcf")
     g_variants = VariantFile(gvcf_file)
-    sample_format_index_mapper = {sample: index + 1 for index, sample in enumerate(g_variants.header.samples)}
 
     columns = {'columns': []}
     if column_yaml_file is not None:
         log.info("Process yaml for: {}".format(column_yaml_file))
         with open(column_yaml_file) as file:
             columns = yaml.load(file, Loader=yaml.FullLoader)
```

### Comparing `hydra-genetics-1.0.0/hydra_genetics/utils/io/multibp.py` & `hydra-genetics-1.1.0/hydra_genetics/utils/io/multibp.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/utils/io/utils.py` & `hydra-genetics-1.1.0/hydra_genetics/utils/io/utils.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/utils/misc.py` & `hydra-genetics-1.1.0/hydra_genetics/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/utils/models/hotspot.py` & `hydra-genetics-1.1.0/hydra_genetics/utils/models/hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/utils/samples.py` & `hydra-genetics-1.1.0/hydra_genetics/utils/samples.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/hydra_genetics/utils/units.py` & `hydra-genetics-1.1.0/hydra_genetics/utils/units.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     """
     if type is None:
         files = units.loc[(wildcards.sample, wildcards.type)].dropna()
     else:
         files = units.loc[(wildcards.sample, type)].dropna()
     if isinstance(files, pandas.Series):
         files = pandas.DataFrame(
-            [[f[1] for f in files.iteritems()], ], columns=[f[0] for f in files.iteritems()]
+            [[f[1] for f in files.items()], ], columns=[f[0] for f in files.items()]
         ).set_index(units.index.names)
     return [file for file in files.itertuples()]
 
 
 def get_fastq_files(units: pandas.DataFrame, wildcards: snakemake.io.Wildcards, type: str = None):
     """
     function used to extract all fastq files for a sample with a sepecific type
```

### Comparing `hydra-genetics-1.0.0/hydra_genetics.egg-info/PKG-INFO` & `hydra-genetics-1.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,9 @@
-Metadata-Version: 2.1
-Name: hydra-genetics
-Version: 1.0.0
-Summary: Helper tools for use with hydra-genetics pipelines.
-Home-page: https://github.com/hydra-genetics/tools
-Author: Patrik Smeds
-Author-email: patrik.smeds@scilifelab.uu.se
-License: GPL-3
-Keywords: hydra-genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next generation sequencing
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
 
-
-# Hydra-genetics
+# <img src="images/hydragenetics.png" width=40 /> Hydra-genetics
 
 Command line interface to create new modules/pipelines or adding a new rule to an existing project. Provides libraries used to make it easier for people not used to pandas to extract information from samples and units dataframes. These dataframes are generated from [units.tsv](https://github.com/hydra-genetics/tools/blob/develop/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml) and [samples.tsv](https://github.com/hydra-genetics/prealignment/blob/develop/workflow/schemas/samples.schema.yaml) files which are used as input.
 
 [![Lint and Test](https://github.com/hydra-genetics/tools/actions/workflows/main.yaml/badge.svg?branch=develop)](https://github.com/hydra-genetics/tools/actions/workflows/main.yaml)
 
 ![python](https://img.shields.io/badge/python-3.8-blue)
 
@@ -39,8 +27,12 @@
  # -t/--tool can be skipped for a single command tool, ex a script
  # this will create a smk file named "super_script.smk" with a rule "super_script"
  hydra-genetics create-rule -c rule3 -t samtools -m snv -a test2 -e "test@test"
 
  # Create input files
  hydra-genetics create-input-files -d path/dir1 -d path/dir2
 
+ # Create singularity cache
+ # all container specified in config.yaml will be fetched
+ hydra-genetics singularity create-singularity-files  -o singularity_cache -c config.yaml
+
 ```
```

### Comparing `hydra-genetics-1.0.0/hydra_genetics.egg-info/SOURCES.txt` & `hydra-genetics-1.1.0/hydra_genetics.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 hydra_genetics.egg-info/dependency_links.txt
 hydra_genetics.egg-info/entry_points.txt
 hydra_genetics.egg-info/not-zip-safe
 hydra_genetics.egg-info/requires.txt
 hydra_genetics.egg-info/top_level.txt
 hydra_genetics/commands/__init__.py
 hydra_genetics/commands/create.py
+hydra_genetics/commands/prep_pipeline_env.py
 hydra_genetics/pipeline-template/.gitignore
 hydra_genetics/pipeline-template/LICENSE.md
 hydra_genetics/pipeline-template/README.md
+hydra_genetics/pipeline-template/mkdocs.yaml
 hydra_genetics/pipeline-template/requirements.test.txt
 hydra_genetics/pipeline-template/requirements.txt
 hydra_genetics/pipeline-template/.github/CODEOWNERS
 hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
 hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md
 hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md
 hydra_genetics/pipeline-template/.github/linters/.snakefmt.toml
@@ -40,28 +42,38 @@
 hydra_genetics/pipeline-template/.tests/integration/resources.yaml
 hydra_genetics/pipeline-template/.tests/integration/samples.tsv
 hydra_genetics/pipeline-template/.tests/integration/units.tsv
 hydra_genetics/pipeline-template/config/config.yaml
 hydra_genetics/pipeline-template/config/resources.yaml
 hydra_genetics/pipeline-template/config/samples.tsv
 hydra_genetics/pipeline-template/config/units.tsv
-hydra_genetics/pipeline-template/images/generate_dag.txt
+hydra_genetics/pipeline-template/docs/extra.css
+hydra_genetics/pipeline-template/docs/index.md
+hydra_genetics/pipeline-template/docs/intro.md
+hydra_genetics/pipeline-template/docs/requirements.txt
+hydra_genetics/pipeline-template/docs/softwares.md
+hydra_genetics/pipeline-template/docs/includes/abbreviations.md
+hydra_genetics/pipeline-template/images/hydragenetics.png
 hydra_genetics/pipeline-template/workflow/Snakefile
-hydra_genetics/pipeline-template/workflow/envs/dummy.yaml
 hydra_genetics/pipeline-template/workflow/notebooks/describe_jupyter_notebook.txt
 hydra_genetics/pipeline-template/workflow/report/describe_workflow.rst
 hydra_genetics/pipeline-template/workflow/rules/common.smk
+hydra_genetics/pipeline-template/workflow/rules/dummy.smk
 hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml
 hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml
+hydra_genetics/pipeline-template/workflow/schemas/rules.schema.yaml
 hydra_genetics/pipeline-template/workflow/schemas/samples.schema.yaml
 hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml
 hydra_genetics/pipeline-template/workflow/scripts/dummy.py
 hydra_genetics/pipeline-template/workflow/scripts/test_dummy.py
-hydra_genetics/rule-template/skeleton_env.yaml
+hydra_genetics/rule-template/config.schema.yaml
+hydra_genetics/rule-template/resources.schema.yaml
+hydra_genetics/rule-template/rules.schema.yaml
 hydra_genetics/rule-template/skeleton_rule.smk
+hydra_genetics/rule-template/softwares.md
 hydra_genetics/utils/__init__.py
 hydra_genetics/utils/misc.py
 hydra_genetics/utils/resources.py
 hydra_genetics/utils/samples.py
 hydra_genetics/utils/units.py
 hydra_genetics/utils/io/__init__.py
 hydra_genetics/utils/io/chr.py
```

### Comparing `hydra-genetics-1.0.0/setup.py` & `hydra-genetics-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     author="Patrik Smeds",
     author_email="patrik.smeds@scilifelab.uu.se",
     url="https://github.com/hydra-genetics/tools",
     license='GPL-3',
     entry_points={"console_scripts": ["hydra-genetics=hydra_genetics.__main__:run"]},
     install_requires=[
         'pandas>=1.3.1',
-        'click==7.1.2',
+        'click>=8,<9',
         'jinja2==3.0.1',
         'rich==10.9.0',
         'snakemake',
         'pysam',
         'gitpython',
         'pyaml'
     ],
```

### Comparing `hydra-genetics-1.0.0/tests/utils/io/test_hotspot.py` & `hydra-genetics-1.1.0/tests/utils/io/test_hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/tests/utils/io/test_mutations_report.py` & `hydra-genetics-1.1.0/tests/utils/io/test_mutations_report.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/tests/utils/models/test_hotspot.py` & `hydra-genetics-1.1.0/tests/utils/models/test_hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/tests/utils/test_misc.py` & `hydra-genetics-1.1.0/tests/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/tests/utils/test_resources.py` & `hydra-genetics-1.1.0/tests/utils/test_resources.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/tests/utils/test_samples.py` & `hydra-genetics-1.1.0/tests/utils/test_samples.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.0.0/tests/utils/test_units.py` & `hydra-genetics-1.1.0/tests/utils/test_units.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,23 @@
             1
         )
         self.assertEqual(
             len(get_units(self.units_2, Wildcards(fromdict={'sample': 'NA12878', "type": "N"}))),
             2
         )
 
+        # small dataframe that produces a pandas.Series in get_units
+        units3 = pandas.DataFrame(
+            dict(
+                sample=["NA12878", "NA12878", "NA13878"],
+                type=["N", "T", "N"],
+            )
+        ).set_index(["sample", "type"], drop=False)
+        self.assertEqual(len(get_units(units3, Wildcards(fromdict={"sample": "NA12878", "type": "N"}))), 1)
+
     def test_get_unit_barcodes(self):
         from hydra_genetics.utils.units import get_unit_barcodes
         self.assertEqual(
             get_unit_barcodes(self.units, Wildcards(fromdict={'sample': 'NA12878',
                                                               'flowcell': 'HKTG2BGXG',
                                                               'type': "N"})),
             {'ACGGAACA+ACGAGAAC', 'CCGGAACA+ACGAGAAC'}
```

### Comparing `hydra-genetics-1.0.0/versioneer.py` & `hydra-genetics-1.1.0/versioneer.py`

 * *Files identical despite different names*

