# Comparing `tmp/geniac-2.6.3.tar.gz` & `tmp/geniac-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geniac-2.6.3.tar", last modified: Fri Jan  6 16:10:48 2023, max compression
+gzip compressed data, was "geniac-3.0.0.tar", last modified: Fri May  5 12:26:16 2023, max compression
```

## Comparing `geniac-2.6.3.tar` & `geniac-3.0.0.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.256656 geniac-2.6.3/
--rw-rw-rw-   0 root         (0) root         (0)      589 2023-01-06 16:04:00.000000 geniac-2.6.3/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-01-06 16:04:00.000000 geniac-2.6.3/.gitattributes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.168657 geniac-2.6.3/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.188657 geniac-2.6.3/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0 root         (0) root         (0)      511 2023-01-06 16:04:00.000000 geniac-2.6.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-01-06 16:04:00.000000 geniac-2.6.3/.github/ISSUE_TEMPLATE/new_feature.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.188657 geniac-2.6.3/.github/PULL_REQUEST_TEMPLATE/
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-01-06 16:04:00.000000 geniac-2.6.3/.github/PULL_REQUEST_TEMPLATE/merge_request_template.md
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-01-06 16:04:00.000000 geniac-2.6.3/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.168657 geniac-2.6.3/.gitlab/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.192657 geniac-2.6.3/.gitlab/issue_templates/
--rw-rw-rw-   0 root         (0) root         (0)      511 2023-01-06 16:04:00.000000 geniac-2.6.3/.gitlab/issue_templates/bug_report.md
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-01-06 16:04:00.000000 geniac-2.6.3/.gitlab/issue_templates/new_feature.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.192657 geniac-2.6.3/.gitlab/merge_request_templates/
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-01-06 16:04:00.000000 geniac-2.6.3/.gitlab/merge_request_templates/merge_request_template.md
--rw-rw-rw-   0 root         (0) root         (0)      765 2023-01-06 16:04:00.000000 geniac-2.6.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-01-06 16:04:00.000000 geniac-2.6.3/.isort.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1355 2023-01-06 16:04:00.000000 geniac-2.6.3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-01-06 16:04:00.000000 geniac-2.6.3/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     9933 2023-01-06 16:04:00.000000 geniac-2.6.3/CHANGELOG
--rw-rw-rw-   0 root         (0) root         (0)     4555 2023-01-06 16:04:00.000000 geniac-2.6.3/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)     2567 2023-01-06 16:04:00.000000 geniac-2.6.3/INSTALL.md
--rw-rw-rw-   0 root         (0) root         (0)    21778 2023-01-06 16:04:00.000000 geniac-2.6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    33969 2023-01-06 16:10:48.256656 geniac-2.6.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1532 2023-01-06 16:04:00.000000 geniac-2.6.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.200657 geniac-2.6.3/cmake/
--rw-rw-rw-   0 root         (0) root         (0)     2824 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)     2780 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/FindApptainer.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2683 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/FindDocker.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2834 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/FindNextflow.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2683 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/FindPodman.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2994 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/FindSingularity.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2082 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/checkConfigFiles.cmake
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/createPathDirectories.cmake
--rw-rw-rw-   0 root         (0) root         (0)     1987 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/createWorkDir.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2086 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/functionColorMessage.cmake
--rw-rw-rw-   0 root         (0) root         (0)     1293 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/initCmakePreload.sh
--rw-rw-rw-   0 root         (0) root         (0)     2124 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/stepAddTestTargets.cmake
--rw-rw-rw-   0 root         (0) root         (0)     5530 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/stepCheckOptions.cmake
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/stepFindPackages.cmake
--rw-rw-rw-   0 root         (0) root         (0)     4031 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/stepGitInfo.cmake
--rw-rw-rw-   0 root         (0) root         (0)    16664 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/stepMainCoreScript.cmake
--rw-rw-rw-   0 root         (0) root         (0)     5864 2023-01-06 16:04:00.000000 geniac-2.6.3/cmake/stepSetVariables.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.200657 geniac-2.6.3/data/
--rw-rw-rw-   0 root         (0) root         (0)     4052 2023-01-06 16:04:00.000000 geniac-2.6.3/data/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.204657 geniac-2.6.3/data/conf/
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-01-06 16:04:00.000000 geniac-2.6.3/data/conf/cluster.config
--rw-rw-rw-   0 root         (0) root         (0)      593 2023-01-06 16:04:00.000000 geniac-2.6.3/data/conf/conda.config
--rw-rw-rw-   0 root         (0) root         (0)      590 2023-01-06 16:04:00.000000 geniac-2.6.3/data/conf/docker.config
--rw-rw-rw-   0 root         (0) root         (0)     2497 2023-01-06 16:04:00.000000 geniac-2.6.3/data/conf/geniac.config
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-01-06 16:04:00.000000 geniac-2.6.3/data/conf/genomes.config
--rw-rw-rw-   0 root         (0) root         (0)      606 2023-01-06 16:04:00.000000 geniac-2.6.3/data/conf/multiconda.config
--rw-rw-rw-   0 root         (0) root         (0)     1468 2023-01-06 16:04:00.000000 geniac-2.6.3/data/conf/multipath.config
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-01-06 16:04:00.000000 geniac-2.6.3/data/conf/path.config
--rw-rw-rw-   0 root         (0) root         (0)      590 2023-01-06 16:04:00.000000 geniac-2.6.3/data/conf/podman.config
--rw-rw-rw-   0 root         (0) root         (0)     7830 2023-01-06 16:04:00.000000 geniac-2.6.3/data/conf/singularity.config
--rw-rw-rw-   0 root         (0) root         (0)     2639 2023-01-06 16:04:00.000000 geniac-2.6.3/data/createSubmodule.bash
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.168657 geniac-2.6.3/data/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.208657 geniac-2.6.3/data/modules/fromSource/
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-01-06 16:04:00.000000 geniac-2.6.3/data/modules/fromSource/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.172657 geniac-2.6.3/data/recipes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.172657 geniac-2.6.3/data/recipes/dependencies/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.208657 geniac-2.6.3/data/recipes/dependencies/renvGlad/
--rw-rw-rw-   0 root         (0) root         (0)     1269 2023-01-06 16:04:00.000000 geniac-2.6.3/data/recipes/dependencies/renvGlad/renv.lock
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.208657 geniac-2.6.3/data/recipes/docker/
--rw-rw-rw-   0 root         (0) root         (0)     1261 2023-01-06 16:04:00.000000 geniac-2.6.3/data/recipes/docker/r.Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.208657 geniac-2.6.3/data/recipes/singularity/
--rw-rw-rw-   0 root         (0) root         (0)     1241 2023-01-06 16:04:00.000000 geniac-2.6.3/data/recipes/singularity/r.def
--rw-rw-rw-   0 root         (0) root         (0)     3818 2023-01-06 16:04:00.000000 geniac-2.6.3/data/useCases.bash
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.220656 geniac-2.6.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1180 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.220656 geniac-2.6.3/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/_static/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     4148 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/admin.rst
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/check.rst
--rw-rw-rw-   0 root         (0) root         (0)     3977 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/cli.rst
--rw-rw-rw-   0 root         (0) root         (0)    14555 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/conda.rst
--rw-rw-rw-   0 root         (0) root         (0)     5327 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     4532 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/customcmd.rst
--rw-rw-rw-   0 root         (0) root         (0)     6257 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/devcycle.rst
--rw-rw-rw-   0 root         (0) root         (0)     1678 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/environment.yml
--rw-rw-rw-   0 root         (0) root         (0)    19262 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/faq.rst
--rw-rw-rw-   0 root         (0) root         (0)     7936 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/from-source-examples.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.228656 geniac-2.6.3/docs/images/
--rw-rw-rw-   0 root         (0) root         (0)   102057 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/images/bash-startup.png
--rw-rw-rw-   0 root         (0) root         (0)   184337 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/images/geniac-cli-uml.png
--rw-rw-rw-   0 root         (0) root         (0)    10972 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/images/geniac-logo.png
--rw-rw-rw-   0 root         (0) root         (0)     7514 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/images/geniac-logo.svg
--rw-rw-rw-   0 root         (0) root         (0)    12102 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/images/geniac.uml
--rw-rw-rw-   0 root         (0) root         (0)    50235 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/images/git-workflow.png
--rw-rw-rw-   0 root         (0) root         (0)    24741 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/images/git-workflow.svg
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/images/image-source.txt
--rw-rw-rw-   0 root         (0) root         (0)    22607 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/images/install.png
--rw-rw-rw-   0 root         (0) root         (0)     9413 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/images/installed.png
--rw-rw-rw-   0 root         (0) root         (0)     7719 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/images/path.png
--rw-rw-rw-   0 root         (0) root         (0)      536 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    17204 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/install.rst
--rw-rw-rw-   0 root         (0) root         (0)     4002 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/intro.rst
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/linux.rst
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/misc.rst
--rw-rw-rw-   0 root         (0) root         (0)     3365 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/overview.rst
--rw-rw-rw-   0 root         (0) root         (0)    24746 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/process.rst
--rw-rw-rw-   0 root         (0) root         (0)     1381 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/profiles.rst
--rw-rw-rw-   0 root         (0) root         (0)     6430 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/renv.rst
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)    16503 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/run.rst
--rw-rw-rw-   0 root         (0) root         (0)     2849 2023-01-06 16:04:00.000000 geniac-2.6.3/docs/substitutions.rst
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-01-06 16:04:00.000000 geniac-2.6.3/environment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.228656 geniac-2.6.3/install/
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-01-06 16:04:00.000000 geniac-2.6.3/install/cmake-init-default.cmake
--rw-rw-rw-   0 root         (0) root         (0)    16045 2023-01-06 16:04:00.000000 geniac-2.6.3/install/docker.nf
--rw-rw-rw-   0 root         (0) root         (0)     2126 2023-01-06 16:04:00.000000 geniac-2.6.3/install/nextflow.config.in
--rw-rw-rw-   0 root         (0) root         (0)    38772 2023-01-06 16:04:00.000000 geniac-2.6.3/install/singularity.nf
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-01-06 16:04:00.000000 geniac-2.6.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2032 2023-01-06 16:10:48.260655 geniac-2.6.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-01-06 16:04:00.000000 geniac-2.6.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.176657 geniac-2.6.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.228656 geniac-2.6.3/src/geniac/
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.236656 geniac-2.6.3/src/geniac/cli/
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15278 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.240656 geniac-2.6.3/src/geniac/cli/commands/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2668 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/commands/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/commands/clean.py
--rw-rw-rw-   0 root         (0) root         (0)     2209 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/commands/configs.py
--rw-rw-rw-   0 root         (0) root         (0)     2436 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/commands/init.py
--rw-rw-rw-   0 root         (0) root         (0)    10068 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/commands/install.py
--rw-rw-rw-   0 root         (0) root         (0)    59890 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/commands/lint.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/commands/options.py
--rw-rw-rw-   0 root         (0) root         (0)     2723 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/commands/recipes.py
--rw-rw-rw-   0 root         (0) root         (0)     1454 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/commands/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.176657 geniac-2.6.3/src/geniac/cli/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.240656 geniac-2.6.3/src/geniac/cli/data/conf/
--rw-rw-rw-   0 root         (0) root         (0)    16758 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/data/conf/geniac.ini
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/data/conf/logging.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.240656 geniac-2.6.3/src/geniac/cli/data/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     7387 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/data/scripts/geniac.bash
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.244656 geniac-2.6.3/src/geniac/cli/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5747 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/parsers/base.py
--rw-rw-rw-   0 root         (0) root         (0)    16641 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/parsers/config.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/parsers/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.244656 geniac-2.6.3/src/geniac/cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25101 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/utils/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1919 2023-01-06 16:04:00.000000 geniac-2.6.3/src/geniac/cli/utils/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.236656 geniac-2.6.3/src/geniac.egg-info/
--rw-r--r--   0 root         (0) root         (0)    33969 2023-01-06 16:10:48.000000 geniac-2.6.3/src/geniac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3951 2023-01-06 16:10:48.000000 geniac-2.6.3/src/geniac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-06 16:10:48.000000 geniac-2.6.3/src/geniac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-01-06 16:10:48.000000 geniac-2.6.3/src/geniac.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-06 16:10:47.000000 geniac-2.6.3/src/geniac.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      188 2023-01-06 16:10:48.000000 geniac-2.6.3/src/geniac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-01-06 16:10:48.000000 geniac-2.6.3/src/geniac.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.248656 geniac-2.6.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.248656 geniac-2.6.3/tests/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.256656 geniac-2.6.3/tests/data/conf/
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/conf/README.md
--rw-rw-rw-   0 root         (0) root         (0)      394 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/conf/base.config
--rwxrwxrwx   0 root         (0) root         (0)      226 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/conf/cluster.config
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/conf/conda.config
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/conf/docker.config
--rw-rw-rw-   0 root         (0) root         (0)     1155 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/conf/geniac.config
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/conf/genomes.config
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/conf/multiconda.config
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/conf/multipath.config
--rw-rw-rw-   0 root         (0) root         (0)      808 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/conf/path.config
--rw-rw-rw-   0 root         (0) root         (0)     3692 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/conf/process.config
--rw-rw-rw-   0 root         (0) root         (0)     1259 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/conf/singularity.config
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/conf/test.config
--rw-rw-rw-   0 root         (0) root         (0)    15327 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/main.nf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.180657 geniac-2.6.3/tests/data/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.256656 geniac-2.6.3/tests/data/modules/fromSource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/modules/fromSource/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.256656 geniac-2.6.3/tests/data/modules/fromSource/dolorSit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/modules/fromSource/dolorSit/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 16:10:48.256656 geniac-2.6.3/tests/data/modules/fromSource/helloWorld/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/modules/fromSource/helloWorld/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)     1689 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/data/nextflow.config
--rw-rw-rw-   0 root         (0) root         (0)     1646 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/test_commands_lint.py
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-01-06 16:04:00.000000 geniac-2.6.3/tests/test_main.py
--rw-rw-rw-   0 root         (0) root         (0)     1921 2023-01-06 16:04:00.000000 geniac-2.6.3/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.990733 geniac-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      589 2023-05-05 12:18:07.000000 geniac-3.0.0/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-05 12:18:07.000000 geniac-3.0.0/.gitattributes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.918735 geniac-3.0.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.938735 geniac-3.0.0/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-05-05 12:18:07.000000 geniac-3.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-05 12:18:07.000000 geniac-3.0.0/.github/ISSUE_TEMPLATE/new_feature.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.938735 geniac-3.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-05-05 12:18:07.000000 geniac-3.0.0/.github/PULL_REQUEST_TEMPLATE/merge_request_template.md
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-05-05 12:18:07.000000 geniac-3.0.0/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.918735 geniac-3.0.0/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.938735 geniac-3.0.0/.gitlab/issue_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-05-05 12:18:07.000000 geniac-3.0.0/.gitlab/issue_templates/bug_report.md
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-05 12:18:07.000000 geniac-3.0.0/.gitlab/issue_templates/new_feature.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.938735 geniac-3.0.0/.gitlab/merge_request_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-05-05 12:18:07.000000 geniac-3.0.0/.gitlab/merge_request_templates/merge_request_template.md
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-05-05 12:18:07.000000 geniac-3.0.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-05 12:18:07.000000 geniac-3.0.0/.isort.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2023-05-05 12:18:07.000000 geniac-3.0.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-05 12:18:07.000000 geniac-3.0.0/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    10723 2023-05-05 12:18:07.000000 geniac-3.0.0/CHANGELOG
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2023-05-05 12:18:07.000000 geniac-3.0.0/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2567 2023-05-05 12:18:07.000000 geniac-3.0.0/INSTALL.md
+-rw-rw-rw-   0 root         (0) root         (0)    21778 2023-05-05 12:18:07.000000 geniac-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    34759 2023-05-05 12:26:16.990733 geniac-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1532 2023-05-05 12:18:07.000000 geniac-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.946735 geniac-3.0.0/cmake/
+-rw-rw-rw-   0 root         (0) root         (0)     2824 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2780 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/FindApptainer.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2683 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/FindDocker.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2834 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/FindNextflow.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2683 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/FindPodman.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2994 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/FindSingularity.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/checkConfigFiles.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/createPathDirectories.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/createWorkDir.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/functionColorMessage.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/initCmakePreload.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2124 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/stepAddTestTargets.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     5530 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/stepCheckOptions.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/stepFindPackages.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     4031 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/stepGitInfo.cmake
+-rw-rw-rw-   0 root         (0) root         (0)    16624 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/stepMainCoreScript.cmake
+-rw-rw-rw-   0 root         (0) root         (0)     5643 2023-05-05 12:18:07.000000 geniac-3.0.0/cmake/stepSetVariables.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.950734 geniac-3.0.0/data/
+-rw-rw-rw-   0 root         (0) root         (0)     4052 2023-05-05 12:18:07.000000 geniac-3.0.0/data/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.954734 geniac-3.0.0/data/conf/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-05 12:18:07.000000 geniac-3.0.0/data/conf/cluster.config
+-rw-rw-rw-   0 root         (0) root         (0)      593 2023-05-05 12:18:07.000000 geniac-3.0.0/data/conf/conda.config
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-05-05 12:18:07.000000 geniac-3.0.0/data/conf/docker.config
+-rw-rw-rw-   0 root         (0) root         (0)     2497 2023-05-05 12:18:07.000000 geniac-3.0.0/data/conf/geniac.config
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-05-05 12:18:07.000000 geniac-3.0.0/data/conf/genomes.config
+-rw-rw-rw-   0 root         (0) root         (0)      606 2023-05-05 12:18:07.000000 geniac-3.0.0/data/conf/multiconda.config
+-rw-rw-rw-   0 root         (0) root         (0)     1468 2023-05-05 12:18:07.000000 geniac-3.0.0/data/conf/multipath.config
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-05-05 12:18:07.000000 geniac-3.0.0/data/conf/path.config
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-05-05 12:18:07.000000 geniac-3.0.0/data/conf/podman.config
+-rw-rw-rw-   0 root         (0) root         (0)     1676 2023-05-05 12:18:07.000000 geniac-3.0.0/data/conf/singularity.config
+-rw-rw-rw-   0 root         (0) root         (0)     2639 2023-05-05 12:18:07.000000 geniac-3.0.0/data/createSubmodule.bash
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.922735 geniac-3.0.0/data/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.954734 geniac-3.0.0/data/modules/fromSource/
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2023-05-05 12:18:07.000000 geniac-3.0.0/data/modules/fromSource/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.922735 geniac-3.0.0/data/recipes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.922735 geniac-3.0.0/data/recipes/dependencies/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.954734 geniac-3.0.0/data/recipes/dependencies/renvGlad/
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2023-05-05 12:18:07.000000 geniac-3.0.0/data/recipes/dependencies/renvGlad/renv.lock
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.954734 geniac-3.0.0/data/recipes/docker/
+-rw-rw-rw-   0 root         (0) root         (0)     1261 2023-05-05 12:18:07.000000 geniac-3.0.0/data/recipes/docker/r.Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.954734 geniac-3.0.0/data/recipes/singularity/
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2023-05-05 12:18:07.000000 geniac-3.0.0/data/recipes/singularity/r.def
+-rw-rw-rw-   0 root         (0) root         (0)     3818 2023-05-05 12:18:07.000000 geniac-3.0.0/data/useCases.bash
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.962734 geniac-3.0.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.962734 geniac-3.0.0/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/_static/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     4148 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/admin.rst
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/check.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3977 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/cli.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14555 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/conda.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4532 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/customcmd.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6257 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/devcycle.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1678 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/environment.yml
+-rw-rw-rw-   0 root         (0) root         (0)    18295 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/faq.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7936 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/from-source-examples.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.970734 geniac-3.0.0/docs/images/
+-rw-rw-rw-   0 root         (0) root         (0)   102057 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/images/bash-startup.png
+-rw-rw-rw-   0 root         (0) root         (0)   184337 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/images/geniac-cli-uml.png
+-rw-rw-rw-   0 root         (0) root         (0)    10972 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/images/geniac-logo.png
+-rw-rw-rw-   0 root         (0) root         (0)     7514 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/images/geniac-logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12102 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/images/geniac.uml
+-rw-rw-rw-   0 root         (0) root         (0)    50235 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/images/git-workflow.png
+-rw-rw-rw-   0 root         (0) root         (0)    24741 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/images/git-workflow.svg
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/images/image-source.txt
+-rw-rw-rw-   0 root         (0) root         (0)    22607 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/images/install.png
+-rw-rw-rw-   0 root         (0) root         (0)     9413 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/images/installed.png
+-rw-rw-rw-   0 root         (0) root         (0)     7719 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/images/path.png
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16972 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4000 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/intro.rst
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/linux.rst
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/misc.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3365 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/overview.rst
+-rw-rw-rw-   0 root         (0) root         (0)    24882 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/process.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/profiles.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6430 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/renv.rst
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)    15909 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/run.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2849 2023-05-05 12:18:07.000000 geniac-3.0.0/docs/substitutions.rst
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-05-05 12:18:07.000000 geniac-3.0.0/environment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.970734 geniac-3.0.0/install/
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-05-05 12:18:07.000000 geniac-3.0.0/install/cmake-init-default.cmake
+-rw-rw-rw-   0 root         (0) root         (0)    16045 2023-05-05 12:18:07.000000 geniac-3.0.0/install/docker.nf
+-rw-rw-rw-   0 root         (0) root         (0)     2057 2023-05-05 12:18:07.000000 geniac-3.0.0/install/nextflow.config.in
+-rw-rw-rw-   0 root         (0) root         (0)    31501 2023-05-05 12:18:07.000000 geniac-3.0.0/install/singularity.nf
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-05-05 12:18:07.000000 geniac-3.0.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2032 2023-05-05 12:26:16.990733 geniac-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-05-05 12:18:07.000000 geniac-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.922735 geniac-3.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.970734 geniac-3.0.0/src/geniac/
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.974734 geniac-3.0.0/src/geniac/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15278 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.978734 geniac-3.0.0/src/geniac/cli/commands/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2668 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/commands/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/commands/clean.py
+-rw-rw-rw-   0 root         (0) root         (0)     2209 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/commands/configs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2436 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/commands/init.py
+-rw-rw-rw-   0 root         (0) root         (0)    10068 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/commands/install.py
+-rw-rw-rw-   0 root         (0) root         (0)    63886 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/commands/lint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/commands/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     2723 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/commands/recipes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/commands/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.926735 geniac-3.0.0/src/geniac/cli/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.978734 geniac-3.0.0/src/geniac/cli/data/conf/
+-rw-rw-rw-   0 root         (0) root         (0)    16447 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/data/conf/geniac.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/data/conf/logging.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.978734 geniac-3.0.0/src/geniac/cli/data/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     7387 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/data/scripts/geniac.bash
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.982734 geniac-3.0.0/src/geniac/cli/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5747 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/parsers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    15057 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/parsers/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     5098 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/parsers/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.982734 geniac-3.0.0/src/geniac/cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25101 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/utils/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1919 2023-05-05 12:18:07.000000 geniac-3.0.0/src/geniac/cli/utils/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.974734 geniac-3.0.0/src/geniac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    34759 2023-05-05 12:26:16.000000 geniac-3.0.0/src/geniac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3951 2023-05-05 12:26:16.000000 geniac-3.0.0/src/geniac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 12:26:16.000000 geniac-3.0.0/src/geniac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-05 12:26:16.000000 geniac-3.0.0/src/geniac.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 12:26:16.000000 geniac-3.0.0/src/geniac.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-05 12:26:16.000000 geniac-3.0.0/src/geniac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-05 12:26:16.000000 geniac-3.0.0/src/geniac.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.982734 geniac-3.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.986734 geniac-3.0.0/tests/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.990733 geniac-3.0.0/tests/data/conf/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/conf/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      394 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/conf/base.config
+-rwxrwxrwx   0 root         (0) root         (0)      226 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/conf/cluster.config
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/conf/conda.config
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/conf/docker.config
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/conf/geniac.config
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/conf/genomes.config
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/conf/multiconda.config
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/conf/multipath.config
+-rw-rw-rw-   0 root         (0) root         (0)      808 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/conf/path.config
+-rw-rw-rw-   0 root         (0) root         (0)     3692 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/conf/process.config
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/conf/singularity.config
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/conf/test.config
+-rw-rw-rw-   0 root         (0) root         (0)    15327 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/main.nf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.926735 geniac-3.0.0/tests/data/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.990733 geniac-3.0.0/tests/data/modules/fromSource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/modules/fromSource/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.990733 geniac-3.0.0/tests/data/modules/fromSource/dolorSit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/modules/fromSource/dolorSit/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:26:16.990733 geniac-3.0.0/tests/data/modules/fromSource/helloWorld/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/modules/fromSource/helloWorld/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1689 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/data/nextflow.config
+-rw-rw-rw-   0 root         (0) root         (0)     1646 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/test_commands_lint.py
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-05-05 12:18:07.000000 geniac-3.0.0/tests/test_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1921 2023-05-05 12:18:07.000000 geniac-3.0.0/tox.ini
```

### Comparing `geniac-2.6.3/.coveragerc` & `geniac-3.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/.gitignore` & `geniac-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/.gitlab-ci.yml` & `geniac-3.0.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/.pre-commit-config.yaml` & `geniac-3.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/.readthedocs.yml` & `geniac-3.0.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/CHANGELOG` & `geniac-3.0.0/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+version-3.0.0
+05/05/2023
+
+NEW FEATURES
+   - singularity profile:
+      * the profile has been simplified since the option '--containall' has been removed and the profile now sets 'autoMounts = true'
+	  * functionalities introduced in version 2.6.* to manage singularity bindings are not needed anymore
+      * option 'params.containers.specificBinds' (used in the geniac-template) introduced in version-2.1.0 is not needed anymore 
+      * cmake option 'ap_mount_dir' introduced in version-2.0.0 to bind folders inside containers is now deprecated since it is not needed anymore
+   - Possibility to define label with variable: label (params.someValue ?: 'toolPrefix')
+   - Geniac CLI:
+      * 'geniac lint': improve error message when name of a conda recipe is not coherent with the label
+
 version-2.6.3
 01/06/2023
 
 NEW FEATURES
    - singularity profile:
       * Allow the binding of relative (to launchDir) paths
       * Order the bindings according to the natural ordering
```

### Comparing `geniac-2.6.3/CMakeLists.txt` & `geniac-3.0.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/INSTALL.md` & `geniac-3.0.0/INSTALL.md`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/LICENSE` & `geniac-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/PKG-INFO` & `geniac-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geniac
-Version: 2.6.3
+Version: 3.0.0
 Summary: Automatic Configuration GENerator and Installer for nextflow pipeline
 Home-page: https://gitlab.curie.fr/bioinfo-guidelines/geniac
 Author: Philippe Hupé, Julien Romejon, Fabrice Allain
 Author-email: philippe.hupe@curie.fr
 License: CeCILL
 Project-URL: Documentation, https://geniac.readthedocs.io/en/latest/
 Project-URL: Demonstration, https://github.com/bioinfo-pf-curie/geniac-demo.git
@@ -40,14 +40,27 @@
 * [Centre national de la recherche scientifique](http://www.cnrs.fr)
 * This project has received funding from the European Union’s Horizon 2020 research and innovation programme and the Canadian Institutes of Health Research under the grant agreement No 825835 in the framework on the [European-Canadian Cancer Network](https://eucancan.com/)
 
 ## Citation
 
 [Allain F, Roméjon J, La Rosa P et al. Geniac: Automatic Configuration GENerator and Installer for nextflow pipelines. Open Research Europe 2021, 1:76](https://open-research-europe.ec.europa.eu/articles/1-76)
 
+version-3.0.0
+05/05/2023
+
+NEW FEATURES
+   - singularity profile:
+      * the profile has been simplified since the option '--containall' has been removed and the profile now sets 'autoMounts = true'
+	  * functionalities introduced in version 2.6.* to manage singularity bindings are not needed anymore
+      * option 'params.containers.specificBinds' (used in the geniac-template) introduced in version-2.1.0 is not needed anymore 
+      * cmake option 'ap_mount_dir' introduced in version-2.0.0 to bind folders inside containers is now deprecated since it is not needed anymore
+   - Possibility to define label with variable: label (params.someValue ?: 'toolPrefix')
+   - Geniac CLI:
+      * 'geniac lint': improve error message when name of a conda recipe is not coherent with the label
+
 version-2.6.3
 01/06/2023
 
 NEW FEATURES
    - singularity profile:
       * Allow the binding of relative (to launchDir) paths
       * Order the bindings according to the natural ordering
```

### Comparing `geniac-2.6.3/README.md` & `geniac-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/CMakeLists.txt` & `geniac-3.0.0/cmake/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/FindApptainer.cmake` & `geniac-3.0.0/cmake/FindApptainer.cmake`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/FindDocker.cmake` & `geniac-3.0.0/cmake/FindDocker.cmake`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/FindNextflow.cmake` & `geniac-3.0.0/cmake/FindNextflow.cmake`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/FindPodman.cmake` & `geniac-3.0.0/cmake/FindPodman.cmake`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/FindSingularity.cmake` & `geniac-3.0.0/cmake/FindSingularity.cmake`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/checkConfigFiles.cmake` & `geniac-3.0.0/cmake/checkConfigFiles.cmake`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/createPathDirectories.cmake` & `geniac-3.0.0/cmake/createPathDirectories.cmake`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/createWorkDir.cmake` & `geniac-3.0.0/cmake/createWorkDir.cmake`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/functionColorMessage.cmake` & `geniac-3.0.0/cmake/functionColorMessage.cmake`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/initCmakePreload.sh` & `geniac-3.0.0/cmake/initCmakePreload.sh`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/stepAddTestTargets.cmake` & `geniac-3.0.0/cmake/stepAddTestTargets.cmake`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/stepCheckOptions.cmake` & `geniac-3.0.0/cmake/stepCheckOptions.cmake`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/stepFindPackages.cmake` & `geniac-3.0.0/cmake/stepFindPackages.cmake`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/stepGitInfo.cmake` & `geniac-3.0.0/cmake/stepGitInfo.cmake`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/cmake/stepMainCoreScript.cmake` & `geniac-3.0.0/cmake/stepMainCoreScript.cmake`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,14 @@
             -Dpipeline_source_dir=${pipeline_source_dir}
             -Dgeniac_source_dir=${CMAKE_SOURCE_DIR}
             -Dgeniac_binary_dir=${CMAKE_BINARY_DIR}
             -Ddocker_registry=${ap_docker_registry}
             -Dlinux_distro=${ap_linux_distro}
             -Dconda_release=${ap_conda_release}
             -Dsingularity_build_options=${ap_singularity_build_options}
-            -Dmount_dir=${ap_mount_dir}
             -P ${CMAKE_SOURCE_DIR}/cmake/createWorkDir.cmake
     COMMAND ${CMAKE_COMMAND} -E echo "workDir/ has been created"
     COMMAND ${CMAKE_COMMAND} -E touch "${CMAKE_BINARY_DIR}/workDir.done"
     COMMENT "Creation of the workDir for cmake"
     DEPENDS ${workdir_depends_files})
 
 # ##############################################################################
```

### Comparing `geniac-2.6.3/cmake/stepSetVariables.cmake` & `geniac-3.0.0/cmake/stepSetVariables.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         "When building the docker/singularity images, geniac bootstraps from docker containers available on the docker hub registry https://hub.docker.com/u/4geniac. When a tool is installed with Conda, the container obviously needs Conda. Therefore, this variable defines which Conda release to use from https://hub.docker.com/u/4geniac. For details, about the docker containers see https://github.com/bioinfo-pf-curie/4geniac. Default is py39_4.12.0."
 )
 
 set(ap_mount_dir
     ""
     CACHE
         STRING
-        "When using the docker/singularity profiles, the list of directories passed with this option will be made available inside the containers. The directories must be provided as a comma separated list (e.g. '/folder1,/folder2'). Default is empty."
+        "Option is deprecated."
 )
 
 set(ap_singularity_build_options
     ""
     CACHE
         STRING
         "Allow to pass specific options when building singularity images. (e.g. --fakeroot). Default is empty."
```

### Comparing `geniac-2.6.3/data/CMakeLists.txt` & `geniac-3.0.0/data/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/data/conf/conda.config` & `geniac-3.0.0/data/conf/conda.config`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/data/conf/docker.config` & `geniac-3.0.0/data/conf/docker.config`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/data/conf/geniac.config` & `geniac-3.0.0/data/conf/geniac.config`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/data/conf/multiconda.config` & `geniac-3.0.0/data/conf/multiconda.config`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/data/conf/multipath.config` & `geniac-3.0.0/data/conf/multipath.config`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/data/conf/path.config` & `geniac-3.0.0/data/conf/path.config`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/data/conf/podman.config` & `geniac-3.0.0/data/conf/podman.config`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/data/createSubmodule.bash` & `geniac-3.0.0/data/createSubmodule.bash`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/data/modules/fromSource/CMakeLists.txt` & `geniac-3.0.0/data/modules/fromSource/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/data/recipes/dependencies/renvGlad/renv.lock` & `geniac-3.0.0/data/recipes/dependencies/renvGlad/renv.lock`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/data/recipes/docker/r.Dockerfile` & `geniac-3.0.0/data/recipes/docker/r.Dockerfile`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/data/recipes/singularity/r.def` & `geniac-3.0.0/data/recipes/singularity/r.def`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/data/useCases.bash` & `geniac-3.0.0/data/useCases.bash`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/Makefile` & `geniac-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/admin.rst` & `geniac-3.0.0/docs/admin.rst`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/cli.rst` & `geniac-3.0.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/conda.rst` & `geniac-3.0.0/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/conf.py` & `geniac-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/customcmd.rst` & `geniac-3.0.0/docs/customcmd.rst`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/devcycle.rst` & `geniac-3.0.0/docs/devcycle.rst`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/environment.yml` & `geniac-3.0.0/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/faq.rst` & `geniac-3.0.0/docs/faq.rst`

 * *Files 9% similar despite different names*

```diff
@@ -246,14 +246,59 @@
    make
    make install
    
    cd ${INSTALL_DIR}/pipeline
    
    nextflow -c conf/test.config run main.nf -profile multiconda
 
+How can a process have a label which is defined by a variable?
+==============================================================
+
+With nextflow, it is possible to define a label using a variable instead of a fixed string. In this case, the label value must be given in parenthesis. `geniac` also support such label. However, the label must be defined according to the following format: ``label (params.someValue ?: 'toolPrefix')``. In any case, the content of the ``params.someValue`` must start by the ``toolPrefix`` value. The `geniac` linter will check that there is a tool with a name starting with such a prefix, if it is not the case, it will throw an error. 
+
+A typical use case is the possibility to launch a pipeline with a version of a tool given as an option on the nextflow command line. Let's consider that you have declare three versions the ``mySoft`` tool in the ``geniac.config`` file as follows:
+
+::
+
+   params {
+      geniac{
+         tools {
+            mySoft = "conda-forge::mySoft=v0=r351h96ca727_1003`
+            mySoft_v1 = "conda-forge::mySoft=v1=r351h96ca727_1003`
+            mySoft_v2 = "conda-forge::mySoft=v1=r351h96ca727_1003`
+         }
+      }
+   }
+
+
+Then, in the netxflow process, define the label as follows:
+
+::
+
+   process mySoft {
+     label (params.mySoftVersion ?: 'mySoft')
+     label 'minMem'
+     label 'minCpu'
+
+
+     script:
+     """
+     mySoft --version
+     """
+   }
+
+
+When you launch nextflow, pass the option ``--mySoftversion`` to set which version of ``mySoft`` you want to use. 
+
+::
+   
+   nextflow run main.nf --mySoftversion v2 -profile test,singularity
+
+You may also write your nextflow code to use the default version (i.e. ``v0`` with the ``mySoft`` label) if no version is specified.
+
 What are the @git_*@ variables?
 ===============================
 
 You will find in both the ``main.nf`` and ``nextflow.config`` some variables surrounded by ``@`` such ``as @git_repo_name@``. These variables are used during the ``cmake`` step to extract the information from the git repository and replace them by their value. These variables are used in the nextflow manifest for example. If needed, you can remove these variables and set the value to whatever you want.
 
 Why does the conda profile fail to build its environment or take to much time?
 ==============================================================================
@@ -302,50 +347,12 @@
 * Using standard `cmake` options:
 
   * if you have the `sudo` privileges, pass the option ``-Dap_install_singularity_images=ON`` to `cmake`, and then run ``sudo make`` (see :ref:`install-run-singularity`),
   * if your are allowed to use the fakeroot option, pass both options ``-Dap_install_singularity_images=ON`` and ``-Dap_singularity_build_options=--fakeroot`` to `cmake`, and then run ``make``.
 
 .. _faq-singularity-invalid-binding:
 
-Why does the singularity profile complain of folder which does not exist or invalid binding?
-============================================================================================
-
-To ensure reproducibility, the singularity profile does the following:
-
-* it launches singularity with the ``--containall`` option
-* it sets ``autoMounts = false`` in nextflow
-* it mounts only few directoryies are mounted by default:
-
-   * ``work`` (i.e. the workDir)
-   * ``/tmp`` (binding in the workDir)
-   * ``/var/tmp`` (binding in the workDir)
-   * ``${projectDir}``
-   * ``${params.genomeAnnotationPath}``
-   * ``${params.outDir}``
-   * if a samplePlan is used by the pipeline to analyse the data (see :ref:`run-options-sampleplan` option), bindings are automatically added:
-
-       * for a samplePlan with 4 columns: the third and fourth columns are used for the bindings
-       * for a samplePlan with 3 columns: the third column is used for the bindings
-       * for a samplePlan with 1 column: the second column is used for the bindings
-       * bindings are not considered for of samplePlan format
-
-This means that if the pipeline needs any file located in a folder which is not mounted by singularity, it will not be available unless you explicitly tells singularity to mount the folder you need. This can be done using :ref:`install-ap_mount_dir` option during the configure step to set the folder which need to be mounted.
-
-
-Moreover, we avoid the interaction between the singularity images and the HOME directory which can drive to unpredictible reproducibility issues. Indeed, if the HOME directory would be available, some libraries installed in the user’s $HOME could be loaded by some programming languages (such as python). If the pipeline throws a message error  containing ``invalid binding``, move your data from your HOME directory into a subfolder.
-
-
-Why does the pipeline complain of data not available when using the singularity profile?
-========================================================================================
-
-As explained in the section :ref:`faq-singularity-invalid-binding`, the :ref:`run-profile-singularity` profile restricts the binding inside the container since it sets ``autoMounts = false`` in nextflow.
-
-If you data is located in a folder which is not in the binding list available in the :ref:`run-profile-singularity` profile, the pipeline will fail. To solve this issue, you have two solutions:
-
-* either you deploy the pipeline setting the correct value in the :ref:`install-ap_mount_dir` option during the configure step to set the folder which need to be mounted
-* or you launch the pipeline setting the correct value in the :ref:`run-specificbinds-option`
-
 
 What is the difference between singularity and apptainer?
 =========================================================
 
 In may 2021, the commercial entity `sylabs <https://sylabs.io/>`_ behind Singularity forked the project. The original Singularity repository has been moved to https://github.com/apptainer/singularity which will persist as an archive and be set to read-only after the first release of `Apptainer <https://apptainer.org/>`_ (https://github.com/apptainer/apptainer). Apptainer will provide singularity as a command line link and will maintain as much of the CLI and environment functionality as possible. From the user's perspective, very little, if anything, will change.
```

### Comparing `geniac-2.6.3/docs/from-source-examples.rst` & `geniac-3.0.0/docs/from-source-examples.rst`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/images/bash-startup.png` & `geniac-3.0.0/docs/images/bash-startup.png`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/images/geniac-cli-uml.png` & `geniac-3.0.0/docs/images/geniac-cli-uml.png`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/images/geniac-logo.png` & `geniac-3.0.0/docs/images/geniac-logo.png`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/images/geniac-logo.svg` & `geniac-3.0.0/docs/images/geniac-logo.svg`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/images/geniac.uml` & `geniac-3.0.0/docs/images/geniac.uml`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/images/git-workflow.png` & `geniac-3.0.0/docs/images/git-workflow.png`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/images/git-workflow.svg` & `geniac-3.0.0/docs/images/git-workflow.svg`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/images/install.png` & `geniac-3.0.0/docs/images/install.png`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/images/installed.png` & `geniac-3.0.0/docs/images/installed.png`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/images/path.png` & `geniac-3.0.0/docs/images/path.png`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/index.rst` & `geniac-3.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/install.rst` & `geniac-3.0.0/docs/install.rst`

 * *Files 2% similar despite different names*

```diff
@@ -158,17 +158,15 @@
 | Default is ``almalinux:8.7``. See also options :ref:`install-ap_conda_release` and :ref:`install-ap_docker_registry`.
 
 .. _install-ap_mount_dir:
 
 ap_mount_dir
 ++++++++++++
 
-| STRING
-| When using the docker/singularity profiles, the list of directories passed with this option will be made available inside the containers. The directories must be provided as a comma separated list (e.g. '/folder1,/folder2').
-| Default is empty.
+| Option is deprecated.
 
 ap_nf_executor
 ++++++++++++++
 
 | STRING
 | `executor <https://www.nextflow.io/docs/latest/executor.html>`_ used by nextflow (e.g. pbs, slurm, etc.).
 | Default is pbs.
```

### Comparing `geniac-2.6.3/docs/intro.rst` & `geniac-3.0.0/docs/intro.rst`

 * *Files 2% similar despite different names*

```diff
@@ -62,11 +62,11 @@
 Acknowledgements
 ================
 
 * `Institut Curie <https://www.curie.fr>`_
 * `Centre national de la recherche scientifique <https://www.cnrs.fr>`_
 * This project has received funding from the European Union’s Horizon 2020 research and innovation programme and the Canadian Institutes of Health Research under the grant agreement No 825835 in the framework on the `European-Canadian Cancer Network <https://eucancan.com/>`_.
 
-Citation
-========
+Cite us
+=======
 
 |geniacref|_
```

### Comparing `geniac-2.6.3/docs/linux.rst` & `geniac-3.0.0/docs/linux.rst`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/overview.rst` & `geniac-3.0.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/process.rst` & `geniac-3.0.0/docs/process.rst`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,16 @@
         - pip:
             - numpy==1.19.2
 
 .. warning::
 
    The ``yml`` file with the conda recipe must follow the following guidelines:
 
-   * Choose a unique name for your conda envirnoment.
+   * Name the file using the name of the label (e.g. if the label is ``trickySoftware``, the file must be named ``trickySoftware.yml``)
+   * Choose a unique name for your conda environment.
    * Each conda package has the naming pattern ``softName = "condaChannelName::softName=version=buildString"``.
    * If you need ``pip`` to install some packages, add ``pip`` in your dependencies and use the pattern ``softName==version`` for each package to be installed with ``pip``.
 
 Edit the file ``conf/geniac.config`` and add for example ``trickySoftware = "${projectDir}/recipes/conda/trickySoftware.yml`` in the section ``params.geniac.tools`` as follows:
 
 ::
```

### Comparing `geniac-2.6.3/docs/profiles.rst` & `geniac-3.0.0/docs/profiles.rst`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/renv.rst` & `geniac-3.0.0/docs/renv.rst`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/docs/run.rst` & `geniac-3.0.0/docs/run.rst`

 * *Files 3% similar despite different names*

```diff
@@ -239,25 +239,14 @@
 Whenever you use the :ref:`run-profile-conda` or :ref:`run-profile-multiconda` profiles, the |conda|_ environments are created in the ``${HOME}/conda-cache-nextflow`` folder by default. This folder can be changed using the ``--condaCacheDir`` option. For example:
 
 ::
 
    nextflow -c conf/test.config run main.nf -profile multiconda --condaCacheDir "${HOME}/myCondaCacheDir"
 
 
-.. _run-specificbinds-option:
-
-\-\-containers.specificBinds
-++++++++++++++++++++++++++++++
-
-When you use the :ref:`run-profile-singularity` profile, it sets ``autoMounts = false`` in nextflow. This means that only the folders that have been passed to the :ref:`install-ap_mount_dir` option during the installation process will be available inside the container. If your pipeline needs to access other folders, you can specify them when your launch the pipeline. For example:
-
-::
-
-   nextflow -c conf/test.config run main.nf -profile singularity --containers.specificBinds '/path/to/my/folder'
-
 \-\-genomeAnnotationPath
 ++++++++++++++++++++++++++
 
 The genome annotations are expected to be found in the folder ``annotations`` by default, and organized as specified in the ``conf/genomes.config`` file. The ``--genomeAnnotationPath`` option allows the path of the ``annotations`` folder to be changed at runtine. For example:
 
 ::
```

### Comparing `geniac-2.6.3/docs/substitutions.rst` & `geniac-3.0.0/docs/substitutions.rst`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/environment.yml` & `geniac-3.0.0/environment.yml`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/install/cmake-init-default.cmake` & `geniac-3.0.0/install/cmake-init-default.cmake`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/install/docker.nf` & `geniac-3.0.0/install/docker.nf`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/install/nextflow.config.in` & `geniac-3.0.0/install/nextflow.config.in`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,14 @@
 
   // docker registry
   dockerRegistry = '@docker_registry@'
 
   // package manager for the Linux Distro
   yum = 'dnf'
 
-  // mount directories for the containers
-  mountDir = '@mount_dir@'
 }
 
 
 process {
   errorStrategy = 'retry'
   maxRetries = 3
   maxErrors = '-1'
```

### Comparing `geniac-2.6.3/install/singularity.nf` & `geniac-3.0.0/install/singularity.nf`

 * *Files 11% similar despite different names*

```diff
@@ -636,226 +636,38 @@
   output:
     file("singularity.config") into finalSingularityConfigCh
 
   script:
     """
     cat << EOF > "singularity.config"
     import java.io.File;
-    import java.nio.file.Files;
-    import java.nio.file.Path;
-    import java.nio.file.Paths;
-    import java.util.Arrays;
-    import java.util.TreeMap;
-    import java.util.List;
-    import java.util.Map;
-    import java.util.Map.Entry;
-    import java.util.regex.Matcher;
-    import java.util.regex.Pattern;
-
-    START_PATTERN = "__sta__";
-    STOP_PATTERN = "__sto__";
-    p1 = Pattern.compile("\\\"(.*?)\\\"");
-    p2 = Pattern
-            .compile("(" + START_PATTERN + "((?!" + STOP_PATTERN + ").)*?) +(.*?" + STOP_PATTERN + ")");
-    SPECIAL_PATHS = Arrays.asList(new String[] { "\\\\\\\$PWD" });
-
-
-    String sanitizePath(String path) throws Exception {
-        if (path.endsWith("/")) {
-            path = path.substring(0, path.length() - 1);
-        }
-
-        if (!path.startsWith("/") && !SPECIAL_PATHS.contains(path)) {
-            path = "" + launchDir + "/" + path
-        }
-
-        return Paths.get(path).normalize().toString();
-    }
-
-    void checkPath(String source, String target, Map pathMap) {
-        if ("\\\$HOME".contains(source)) {
-            throw new Exception("ERROR reported from conf/singularity.config. \'" + source
-                    + "\' is an invalid binding source. Indeed, as a result of this binding the user HOME directory would be available inside the container which can drive to unpredictible reproducibility issues. You should modify what was passed to the \'-Dap_mount_dir\' option during the cmake configuration step with geniac (see https://geniac.readthedocs.io and the FAQ).");
-        }
-
-        if (!target.startsWith("/")) {
-            throw new Exception("ERROR reported from conf/singularity.config. \'" + target + "\' is an invalid binding target, it must be an absolute path. You should modify what was passed to the \'-Dap_mount_dir\' option during the cmake configuration step with geniac (see https://geniac.readthedocs.io and the FAQ).");
-        }
-
-        if (pathMap.containsKey(target) && !source.equals(pathMap.get(target))) {
-            throw new Exception("Several bindings for to the same target " + target);
-        }
-    }
-
-    void checkSamplePlan() {
-        if (!params.samplePlan) {
-            return;
-        }
-
-        singularity.runOptions += " -B " + params.samplePlan;
-
-        Set set = [];
-        (new File(params.samplePlan)).eachLine{
-            defSamplePlanRow = it.split(",");
-            nbCol = defSamplePlanRow.size();
-            if(nbCol == 4) {
-                r1Dir = defSamplePlanRow[2].substring(0, defSamplePlanRow[2].lastIndexOf("/"));
-                r2Dir = defSamplePlanRow[3].substring(0, defSamplePlanRow[3].lastIndexOf("/"));
-                set.add(r1Dir);
-                set.add(r2Dir);
-            } else if(nbCol == 3) {
-                r1Dir = defSamplePlanRow[2].substring(0, defSamplePlanRow[2].lastIndexOf("/"));
-                set.add(r1Dir);
-            } else if(nbCol == 2) {
-                r1Dir = defSamplePlanRow[1].substring(0, defSamplePlanRow[1].lastIndexOf("/"));
-                set.add(r1Dir);
-            }
-            else {
-                return;
-            }
-        };
-
-        set.each{
-            singularity.runOptions += " -B " + it;
-        }
-    }
-
-    void checkSymlink(pathToCheck, add, map) {
-        if (SPECIAL_PATHS.contains(pathToCheck)) {
-            return;
-        }
-
-        if (add) {
-            singularity.runOptions += " -B " + pathToCheck;
-            map.put(pathToCheck, pathToCheck);
-        }
-
-        List<String> pathSteps = Arrays.asList(pathToCheck.split("/"));
-        List<String> recursivePathsToCheck = new ArrayList<>();
-        for (i = 1 ; i <= pathSteps.size() ; i++) {
-            String currPathToCheck = pathSteps.subList(0, i).join("/");
-            File f = new File(currPathToCheck);
-            Path p = f.toPath();
-            if (Files.isSymbolicLink(p)) {
-                String symlinkPath = p.toRealPath();
-                String nextPathToCheck = symlinkPath + "/" + pathSteps.subList(i, pathSteps.size()).join("/");
-                recursivePathsToCheck.add(nextPathToCheck);
-            }
-        }
-
-        checkSymlinks(recursivePathsToCheck, map);
-    }
-
-    void checkSymlinks(pathsToProcess, map) {
-        for (String pathToProcess: pathsToProcess) {
-            checkSymlink(pathToProcess, true, map);
-        }
-    }
-
-    void checkBindings() throws Exception {
-        singularity.runOptions += " -B \\\$projectDir,\\\$launchDir,\\\\\\\$PWD:/tmp,\\\\\\\$PWD:/var/tmp,\\\${params.genomeAnnotationPath?:''},\\\${params.outDir?:''},${params.mountDir?:''}";
-        checkSamplePlan();
-        String input = singularity.runOptions;
-
-        // replace double quotes by start/stop pattern
-        Matcher m = p1.matcher(input);
-        if (m.find()) {
-            input = m.replaceAll(START_PATTERN + "\\\\\\\$1" + STOP_PATTERN);
-        }
-
-        // replace spaces in start/stop pattern by ##
-        m = p2.matcher(input);
-        while (m.find()) {
-            input = m.replaceAll("\\\\\\\$1##\\\\\\\$3");
-            m = p2.matcher(input);
-        }
-
-        // split on remaining spaces
-        String[] tab = input.split(" ");
-        Map<String, String> pathMap = new TreeMap<>();
-        boolean curr = false;
-        String newRunOptions = '';
-        for (String inputElem : tab) {
-            // binding option key
-            if (inputElem.equals("-B") || inputElem.equals("--bind")) {
-                curr = true;
-            }
-            // binding option value
-            else if (!inputElem.startsWith("-") && curr) {
-                // each path to bind
-                for (String path : inputElem.split(",")) {
-                    if (path.isEmpty()) {
-                        continue;
-                    }
-
-                    // restore original value (revert p1/p2 pattern effects)
-                    path = path.replaceAll("##", " ");
-                    path = path.replaceAll(START_PATTERN, "\"");
-                    path = path.replaceAll(STOP_PATTERN, "\"");
-
-                    // source/target paths
-                    String[] pathTab = path.split(":");
-
-                    String target = null;
-                    String source = sanitizePath(pathTab[0]);
-
-                    if (pathTab.length > 1) {
-                        target = sanitizePath(pathTab[1]);
-                    } else {
-                        target = source;
-                    }
-
-                    checkPath(source, target, pathMap);
-                    pathMap.put(target, source);
-
-                    // is symlink
-                    checkSymlink(source, false, pathMap);
-                }
-            }
-            // not binding option value/key
-            else {
-                newRunOptions += " " + inputElem;
-                curr = false;
-            }
-        }
-
-        newRunOptions += " -B ,";
-        for (Entry<String, String> entry : pathMap.entrySet()) {
-            System.out.println("path " + entry.getValue() + " mounted in " + entry.getKey() + ".");
-            newRunOptions += entry.getValue() + (entry.getValue() == entry.getKey() ? '' : ":" + entry.getKey()) + ",";
-        }
-
-        singularity.runOptions = newRunOptions;
-    }
-
 
     def checkProfileSingularity(path){
       if (new File(path).exists()){
         File directory = new File(path)
         def contents = []
         directory.eachFileRecurse (groovy.io.FileType.FILES){ file -> contents << file }
         if (!path?.trim() || contents == null || contents.size() == 0){
           System.out.println("   ### ERROR ###    The option '-profile singularity' requires the singularity images to be installed on your system. See \\`--singularityImagePath\\` for advanced usage.");
           System.exit(-1)
         }
-      }else{
+      } else {
         System.out.println("   ### ERROR ###    The option '-profile singularity' requires the singularity images to be installed on your system. See \\`--singularityImagePath\\` for advanced usage.");
         System.exit(-1)
       }
     }
 
     singularity {
       enabled = true
-      autoMounts = false
-      runOptions = "--containall " + (params.geniac.containers?.singularityRunOptions ?: '').replace('-C', '').replace('--containall', '')
+      autoMounts = true
+      runOptions = (params.geniac.containers?.singularityRunOptions ?: '')
     }
 
     process {
       checkProfileSingularity("\\\${params.geniac.singularityImagePath}")
-      checkBindings()
     EOF
     for keyFile in ${key}
     do
         cat \${keyFile} >> singularity.config
     done
     echo "}"  >> singularity.config
     """
```

### Comparing `geniac-2.6.3/setup.cfg` & `geniac-3.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/setup.py` & `geniac-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac/cli/__main__.py` & `geniac-3.0.0/src/geniac/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac/cli/commands/base.py` & `geniac-3.0.0/src/geniac/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac/cli/commands/clean.py` & `geniac-3.0.0/src/geniac/cli/commands/clean.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac/cli/commands/configs.py` & `geniac-3.0.0/src/geniac/cli/commands/configs.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac/cli/commands/init.py` & `geniac-3.0.0/src/geniac/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac/cli/commands/install.py` & `geniac-3.0.0/src/geniac/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac/cli/commands/lint.py` & `geniac-3.0.0/src/geniac/cli/commands/lint.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     )
     # REGEX check if a string from a yml recipe with pip is valid
     CONDA_YML_PIP_RECIPES_RE = re.compile(
         r"(?P<recipes>([.\w-]+==?[\d.]))"
     )
     # REGEX to check if a string is a path for yml or yaml file
     CONDA_PATH_RE = re.compile(
-        r"(?P<nxfvar>\${(baseDir|projectDir)})/(?P<basepath>[/\w]+\.(?P<ext>yml|yaml))"
+        #r"(?P<nxfvar>\${(baseDir|projectDir)})/(?P<basepath>[/\w]+\.(?P<ext>yml|yaml))"
+        r"(?P<nxfvar>\${(baseDir|projectDir)})/(?P<basepath>.+\.(?P<ext>yml|yaml))"
     )
     # REGEX to check if a string is a path for renv.lock file
     RENV_LOCKFILE_PATH_RE = re.compile(
         r"(?P<nxfvar>\${(baseDir|projectDir)})/(?P<basepath>[/\w]+\.(?P<ext>lock))"
     )
     # REGEX to check if install cmake directive has been correctly added in the main CMakeLists.txt
     INSTALL_MAIN_CMAKE_RE = re.compile(
@@ -141,14 +142,15 @@
         """Merge geniac labels from Nextflow configs"""
         self._processes_from_workflow |= value
 
     @property
     def labels_from_workflow(self):
         """Workflow labels from Nextflow folders"""
         # Init labels list if empty
+    
         labels = list(
             dict.fromkeys(
                 [
                     label
                     for process, process_scope in self.processes_from_workflow.items()
                     for label in process_scope["label"]
                     if label is not None
@@ -527,14 +529,21 @@
                                                            self.error(
                                                                "In section 'pip' of the file '%s', the value '%s' of '%s' tool does not follow the pattern "
                                                                '"softName==version".',
                                                                conda_path.relative_to(self.src_path),
                                                                pip_tool,
                                                                label
                                                            )
+                                # Test that the name of the conda recipe (yml or yaml file) is consistent with the label
+                                if label != os.path.splitext(os.path.basename(conda_path))[0]:
+                                        self.error(
+                                                "In the file 'conf/geniac.config', the label '%s' uses the custom conda recipe '%s'. Rename the recipe into '%s' to match your label.",
+                                                label,
+                                                recipe,
+                                                os.path.dirname(recipe) + "/" + label + ".yml")
                             else:
                                 self.error(
                                     "Conda file %s related to %s tool does not exist.",
                                     conda_path.relative_to(self.src_path),
                                     label,
                                 )
                     # Elif the tool value is a conda recipe
@@ -1111,74 +1120,131 @@
 
         return self.labels_from_folders
 
     def check_labels(
         self,
     ):
         """Check labels"""
-        # Get the difference with labels from geniac tools and folders and labels used
-        # in the workflow
-        cross_labels = [
-            label
-            for label in self.labels_all
-            if label not in self.labels_from_workflow and label != "onlyLinux"
-        ]
-        if len(cross_labels) >= 1:
-            self.warning(
-                "You have recipes, modules or geniac.tools label(s) that are not used in workflow "
-                "scripts %s.",
-                cross_labels,
-            )
 
         # Check if there is any inconsistencies with labels in other parts of config files (post,
         # envCustom) in global nxf_config scope
         for extra_section in (
             "params.geniac.containers.cmd.post",
             "params.geniac.containers.cmd.envCustom",
         ):
             self.nxf_config_container.check_labels_in_section(
                 extra_section, self.labels_all
             )
 
+        # List of candidate tools defined in a process
+        # using a label defined by a variable
+        listCandidateToolsWitlLabelVariable = []
         for process, process_scope in self.processes_from_workflow.items():
             # Get the diff of process labels not present in process scope in config
             # files and present within geniac tools scope
-            matched_labels = [
-                label
-                for label in process_scope.get("label")
-                if label not in self.labels_from_process_config
-                and label in self.labels_all
-            ]
+            if process_scope.get("label") == None:
+                matched_labels = []
+                unmatched_labels = []
+            else:
+                matched_labels = [
+                    label
+                    for label in process_scope.get("label")
+                    if label not in self.labels_from_process_config
+                    and label in self.labels_all
+                ]
+                unmatched_labels = [
+                    label
+                    for label in process_scope.get("label")
+                    if label not in self.labels_all
+                    and label not in self.labels_from_process_config
+                ]
+
+            if len(matched_labels) == 0:
+                if process_scope.get("labelVariable") != None:
+                    if len(process_scope.get("labelVariable")) > 0:
+                        foundLabelWithPrefix = False
+                        candidateTools = []
+                        for labelVariable in process_scope.get("labelVariable"):
+                            startWithLabel = list(filter(re.compile(r"^"+labelVariable+r".*").match, self.labels_all))
+                            if len(startWithLabel) > 0:
+                                foundLabelWithPrefix = True
+                                candidateTools = startWithLabel
+                                listCandidateToolsWitlLabelVariable = listCandidateToolsWitlLabelVariable + candidateTools
+                        if foundLabelWithPrefix:
+                            self.info(
+                                    "The process '%s' has a label defined by a variable. Candidate tool(s): '%s'.",
+                                    process,
+                                    candidateTools
+                                    )
+                        else:
+                            self.error(
+                                    "The process '%s' has a label defined by the variable '%s' and associated prefix label '%s' but no candidate tool has been found with such a prefix. Check the nextflow process to be sure that the syntax 'label (params.someValue ?: 'toolPrefix')' has been used. 'toolPrefix' must match one of the available labels among the following list:\n'%s'.",
+                                    process,
+                                    process_scope.get("labelVariableParams"),
+                                    process_scope.get("labelVariable"),
+                                    self.labels_all
+                            )
+                    else:
+                        self.error(
+                                "The process '%s' does not have any label which corresponds to a tool. Available labels are:\n'%s'.",
+                                process,
+                                self.labels_all
+                        )
+                else:
+                    self.error(
+                            "The process '%s' does not have any label which corresponds to a tool. Available labels are:\n'%s'.",
+                            process,
+                            self.labels_all
+                    )
+
             if len(matched_labels) > 1:
                 self.error(
                     "Use only one recipes, modules or geniac.tools label for the process %s %s. "
                     "A process should have only one geniac.tools label.",
                     process,
                     matched_labels,
                 )
-            unmatched_labels = [
-                label
-                for label in process_scope.get("label")
-                if label not in self.labels_all
-                and label not in self.labels_from_process_config
-            ]
+
             if len(unmatched_labels) >= 1:
                 process_path = self.get_config_path(
                     GeniacLint.GENIAC_CHECK_CONFIG, "process", single_path=True
                 ).relative_to(self.src_path)
                 self.error(
                     "Label(s) %s from process %s in the file %s not defined in the file %s.",
                     unmatched_labels,
                     process,
                     Path(process_scope.get("NextflowScriptPath")).relative_to(
                         self.src_path
                     ),
                     process_path,
                 )
 
+        # Get the difference with labels from geniac tools and folders and labels used
+        # in the workflow
+        cross_labels = [
+            label
+            for label in self.labels_all
+            if label not in self.labels_from_workflow and label != "onlyLinux"
+        ]
+        if len(cross_labels) >= 1:
+            if len(listCandidateToolsWitlLabelVariable) >=1:
+                notFound = set(cross_labels) - set(listCandidateToolsWitlLabelVariable)
+                if len(notFound) >= 1:
+                    self.warning(
+                        "You have recipes, modules or geniac.tools label(s) that are not used in workflow "
+                        "scripts %s.",
+                        notFound,
+                    )
+            else:
+                self.warning(
+                    "You have recipes, modules or geniac.tools label(s) that are not used in workflow "
+                    "scripts %s.",
+                    cross_labels,
+                )
+
     def check_labels_containers(
         self, container
     ):
         """Check labels for containers"""
         for label_name in ["modules"]:
             if container_diff := sorted(
                 list(
```

### Comparing `geniac-2.6.3/src/geniac/cli/commands/options.py` & `geniac-3.0.0/src/geniac/cli/commands/options.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac/cli/commands/recipes.py` & `geniac-3.0.0/src/geniac/cli/commands/recipes.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac/cli/commands/test.py` & `geniac-3.0.0/src/geniac/cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac/cli/data/conf/geniac.ini` & `geniac-3.0.0/src/geniac/cli/data/conf/geniac.ini`

 * *Files 1% similar despite different names*

```diff
@@ -362,20 +362,18 @@
 patterns
 scopes      =
     yum
     git
     cmd
 
 [scope.params.geniac.containers.values.default]
-singularityRunOptions   = "--bind $${params.containers.specificBinds}"
+singularityRunOptions   = ""
 dockerRunOptions        = ""
 podmanRunOptions        = ""
 
-[scope.params.geniac.containers.values.prohibited]
-singularityRunOptions   = (?P<opt>(?<=-B )|(?<=--bind ))\s*(?P<values>[\w_/,:]*(?P<prohibited>((?P<precomma>,)|(?<= ))(?P<host>[\w/_]+:|)(?P<prohibited_pattern>/tmp)(?P<mnt>:[\w/_]+|)((?(precomma)|,)|\s|$$))[\w_/,:]*)
 
 # params.geniac.containers.yum
 [scope.params.geniac.containers.yum]
 files
 required    = false
 paths
 properties
```

### Comparing `geniac-2.6.3/src/geniac/cli/data/conf/logging.json` & `geniac-3.0.0/src/geniac/cli/data/conf/logging.json`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac/cli/data/scripts/geniac.bash` & `geniac-3.0.0/src/geniac/cli/data/scripts/geniac.bash`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac/cli/parsers/base.py` & `geniac-3.0.0/src/geniac/cli/parsers/base.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac/cli/parsers/config.py` & `geniac-3.0.0/src/geniac/cli/parsers/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,52 +78,23 @@
         ]
         # If there is mandatory properties, we check against default values and/or prohibited
         # patterns
         for config_prop in config_properties:
             default_values = self.get_config_section_items(
                 f"scope.{nxf_config_scope}.values.default"
             ).get(config_prop, [])
-            prohibited_patterns = self.get_config_section_items(
-                f"scope.{nxf_config_scope}.values.prohibited"
-            ).get(config_prop)
             cfg_vals = scope.get(config_prop, [None])
 
             for cfg_val in cfg_vals:
                 # If the values doesn't match default values
                 if (
                     config_prop
                     and default_values
                     and cfg_val not in [_.strip("'\"") for _ in default_values]
                 ):
-                    # Check for prohibited pattern only if the value doesn't match default values
-                    for reg in (
-                        [re.compile(pattern) for pattern in prohibited_patterns]
-                        if prohibited_patterns
-                        else []
-                    ):
-                        if match := reg.search(cfg_val):
-                            matches = match.groupdict()
-                            cfg_val_without_pro = cfg_val.replace(
-                                matches.get("prohibited"), ""
-                            )
-                            warn_flag = cfg_val_without_pro != cfg_val.replace(
-                                matches.get("values"), ""
-                            )
-                            self.error(
-                                'Value "%s" of %s.%s parameter match the following prohibited '
-                                'pattern "%s". %s%s',
-                                cfg_val,
-                                nxf_config_scope,
-                                config_prop,
-                                matches.get("prohibited_pattern"),
-                                "It should normally correspond to the string below:\n\t"
-                                if warn_flag
-                                else "",
-                                cfg_val_without_pro if warn_flag else "",
-                            )
 
                     if cfg_val is not None:
                         self.warning(
                             'Value "%s" of %s.%s parameter'
                             " in file %s doesn't correspond to one of the expected values [%s].",
                             cfg_val,
                             nxf_config_scope,
```

### Comparing `geniac-2.6.3/src/geniac/cli/parsers/scripts.py` & `geniac-3.0.0/src/geniac/cli/parsers/scripts.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 class NextflowScript(GeniacParser):
     """Nextflow script file parser"""
 
     # process flag
     PROCESS_RE = re.compile(r"^ *process +(?P<processName>\w+) *{")
     # process label
     LABEL_RE = re.compile(r"^ *label +['\"](?P<labelName>\w+)['\"] *")
+    # process label defined by a variable
+    LABEL_VARIABLE_RE = re.compile(r"^ *label +[(](?P<labelParamsValue>.*) \?\: ['\"'](?P<labelName>.*)['\"'][)] *")
     # script flag
     SCRIPT_RE = re.compile(
         r"^ *(?P<startScript>[\"']{3})"
         r"((?P<script>.+)(?<=(?P<endScript>[\"']{3})))? *$"
     )
     # output/input flag
     INOUT_RE=re.compile(r"^[ \t]*(?P<inout>input|output|script):[ \t]*")
@@ -62,17 +64,25 @@
                 process = values.get("processName")
                 self.content["process"][process] = defaultdict(list)
                 # Save the path to the nextflow script for future logs
                 self.content["process"][process]["NextflowScriptPath"] = str(in_path)
             if match := self.LABEL_RE.match(line):
                 values = match.groupdict()
                 label = values.get("labelName")
-                self.debug("FOUND label %s in process %s.", label, process)
+                self.debug("FOUND label '%s' in process '%s'.", label, process)
                 self.content["process"][process]["label"].append(label)
                 continue
+            if match := self.LABEL_VARIABLE_RE.match(line):
+                values = match.groupdict()
+                label = values.get("labelName")
+                paramsValue = values.get("labelParamsValue")
+                self.info("FOUND label '%s' in process '%s' defined using the variable '%s'.", label, process, paramsValue)
+                self.content["process"][process]["labelVariable"].append(label)
+                self.content["process"][process]["labelVariableParams"].append(paramsValue)
+                continue
             # For the moment we append everything into the same list even with conditional nextflow
             # script
             if match := self.SCRIPT_RE.match(line):
                 inout = ""
                 input_flag = False
                 output_flag = False
                 values = match.groupdict()
```

### Comparing `geniac-2.6.3/src/geniac/cli/utils/base.py` & `geniac-3.0.0/src/geniac/cli/utils/base.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac/cli/utils/logging.py` & `geniac-3.0.0/src/geniac/cli/utils/logging.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/src/geniac.egg-info/PKG-INFO` & `geniac-3.0.0/src/geniac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geniac
-Version: 2.6.3
+Version: 3.0.0
 Summary: Automatic Configuration GENerator and Installer for nextflow pipeline
 Home-page: https://gitlab.curie.fr/bioinfo-guidelines/geniac
 Author: Philippe Hupé, Julien Romejon, Fabrice Allain
 Author-email: philippe.hupe@curie.fr
 License: CeCILL
 Project-URL: Documentation, https://geniac.readthedocs.io/en/latest/
 Project-URL: Demonstration, https://github.com/bioinfo-pf-curie/geniac-demo.git
@@ -40,14 +40,27 @@
 * [Centre national de la recherche scientifique](http://www.cnrs.fr)
 * This project has received funding from the European Union’s Horizon 2020 research and innovation programme and the Canadian Institutes of Health Research under the grant agreement No 825835 in the framework on the [European-Canadian Cancer Network](https://eucancan.com/)
 
 ## Citation
 
 [Allain F, Roméjon J, La Rosa P et al. Geniac: Automatic Configuration GENerator and Installer for nextflow pipelines. Open Research Europe 2021, 1:76](https://open-research-europe.ec.europa.eu/articles/1-76)
 
+version-3.0.0
+05/05/2023
+
+NEW FEATURES
+   - singularity profile:
+      * the profile has been simplified since the option '--containall' has been removed and the profile now sets 'autoMounts = true'
+	  * functionalities introduced in version 2.6.* to manage singularity bindings are not needed anymore
+      * option 'params.containers.specificBinds' (used in the geniac-template) introduced in version-2.1.0 is not needed anymore 
+      * cmake option 'ap_mount_dir' introduced in version-2.0.0 to bind folders inside containers is now deprecated since it is not needed anymore
+   - Possibility to define label with variable: label (params.someValue ?: 'toolPrefix')
+   - Geniac CLI:
+      * 'geniac lint': improve error message when name of a conda recipe is not coherent with the label
+
 version-2.6.3
 01/06/2023
 
 NEW FEATURES
    - singularity profile:
       * Allow the binding of relative (to launchDir) paths
       * Order the bindings according to the natural ordering
```

### Comparing `geniac-2.6.3/src/geniac.egg-info/SOURCES.txt` & `geniac-3.0.0/src/geniac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/tests/data/conf/geniac.config` & `geniac-3.0.0/tests/data/conf/geniac.config`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/tests/data/conf/multipath.config` & `geniac-3.0.0/tests/data/conf/multipath.config`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/tests/data/conf/path.config` & `geniac-3.0.0/tests/data/conf/path.config`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/tests/data/conf/process.config` & `geniac-3.0.0/tests/data/conf/process.config`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/tests/data/conf/singularity.config` & `geniac-3.0.0/tests/data/conf/singularity.config`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/tests/data/conf/test.config` & `geniac-3.0.0/tests/data/conf/test.config`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/tests/data/main.nf` & `geniac-3.0.0/tests/data/main.nf`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/tests/data/nextflow.config` & `geniac-3.0.0/tests/data/nextflow.config`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/tests/test_base.py` & `geniac-3.0.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/tests/test_commands_lint.py` & `geniac-3.0.0/tests/test_commands_lint.py`

 * *Files identical despite different names*

### Comparing `geniac-2.6.3/tox.ini` & `geniac-3.0.0/tox.ini`

 * *Files identical despite different names*

