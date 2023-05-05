# Comparing `tmp/rayvision_houdini-1.4.2.tar.gz` & `tmp/rayvision_houdini-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rayvision_houdini-1.4.2.tar", last modified: Tue Sep  6 06:34:40 2022, max compression
+gzip compressed data, was "dist/rayvision_houdini-1.4.5.tar", last modified: Fri May  5 06:37:06 2023, max compression
```

## Comparing `rayvision_houdini-1.4.2.tar` & `rayvision_houdini-1.4.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/
--rw-rw-rw-   0 root         (0) root         (0)      252 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      187 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1121 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      259 2022-09-06 06:16:59.000000 rayvision_houdini-1.4.2/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      472 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      664 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       44 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/dev_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     5357 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/docs/rayvision_houdini/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/docs/rayvision_houdini/core/
--rw-rw-rw-   0 root         (0) root         (0)      141 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/docs/rayvision_houdini/core/cg.rst
--rw-rw-rw-   0 root         (0) root         (0)      296 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/docs/rayvision_houdini/core/constants.rst
--rw-rw-rw-   0 root         (0) root         (0)     5108 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/docs/rayvision_houdini/first_look.rst
--rw-rw-rw-   0 root         (0) root         (0)      854 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/docs/rayvision_houdini/installation_guide.rst
--rw-rw-rw-   0 root         (0) root         (0)      128 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/docs/rayvision_houdini/modules.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/help/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/help/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/help/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/help/doc/docs/
--rw-rw-rw-   0 root         (0) root         (0)     8755 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/help/doc/docs/Configuration Documentation--Maya.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/help/doc/docs_zh/
--rw-rw-rw-   0 root         (0) root         (0)     8250 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/help/doc/docs_zh/配置文件文档之Maya.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/help/examples/
--rw-rw-rw-   0 root         (0) root         (0)     3338 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/help/examples/houdini_demo.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/help/examples/only_analyze.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/help/scenes/
--rw-rw-rw-   0 root         (0) root         (0)   277555 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/help/scenes/sphere.hip
--rw-rw-rw-   0 root         (0) root         (0)      452 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/init_pycharm_setup.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/rayvision_houdini/
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-09-06 06:16:59.000000 rayvision_houdini-1.4.2/rayvision_houdini/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16325 2022-09-06 06:22:12.000000 rayvision_houdini-1.4.2/rayvision_houdini/analyze_houdini.py
--rw-rw-rw-   0 root         (0) root         (0)       82 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/rayvision_houdini/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/
--rw-rw-rw-   0 root         (0) root         (0)      498 2022-09-06 06:09:27.000000 rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py27/
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py27/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   529920 2022-09-06 03:24:39.000000 rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py27/hanalyse.pyd
--rw-rw-rw-   0 root         (0) root         (0)  3939328 2022-09-06 03:24:39.000000 rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py27/hanalyse.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py37/
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py37/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   540672 2022-09-06 03:24:39.000000 rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py37/hanalyse.pyd
--rw-rw-rw-   0 root         (0) root         (0)  5020992 2022-09-06 03:24:40.000000 rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py37/hanalyse.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py39/
--rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py39/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   542720 2022-09-06 03:24:40.000000 rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py39/hanalyse.pyd
--rw-rw-rw-   0 root         (0) root         (0)  5168064 2022-09-06 03:24:40.000000 rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py39/hanalyse.so
--rw-rw-rw-   0 root         (0) root         (0)      787 2022-09-06 04:23:37.000000 rayvision_houdini-1.4.2/rayvision_houdini/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/rayvision_houdini/tests/
--rw-rw-rw-   0 root         (0) root         (0)       39 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/rayvision_houdini/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2022-09-06 03:45:31.000000 rayvision_houdini-1.4.2/rayvision_houdini/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      949 2022-09-06 06:16:59.000000 rayvision_houdini-1.4.2/rayvision_houdini/tests/test_analyze_houdini.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/rayvision_houdini.egg-info/
--rw-r--r--   0 root         (0) root         (0)      472 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/rayvision_houdini.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1946 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/rayvision_houdini.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/rayvision_houdini.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/rayvision_houdini.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/rayvision_houdini.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       43 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       67 2022-09-06 06:34:40.000000 rayvision_houdini-1.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1057 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     3040 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:06.000000 rayvision_houdini-1.4.5/
+-rw-rw-rw-   0 root         (0) root         (0)      252 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      187 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      259 2022-09-06 06:16:59.000000 rayvision_houdini-1.4.5/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-05 06:37:06.000000 rayvision_houdini-1.4.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      664 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       44 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/dev_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     5357 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/docs/rayvision_houdini/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/docs/rayvision_houdini/core/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/docs/rayvision_houdini/core/cg.rst
+-rw-rw-rw-   0 root         (0) root         (0)      296 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/docs/rayvision_houdini/core/constants.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5108 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/docs/rayvision_houdini/first_look.rst
+-rw-rw-rw-   0 root         (0) root         (0)      854 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/docs/rayvision_houdini/installation_guide.rst
+-rw-rw-rw-   0 root         (0) root         (0)      128 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/docs/rayvision_houdini/modules.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/help/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/help/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/help/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/help/doc/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     8755 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/help/doc/docs/Configuration Documentation--Maya.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/help/doc/docs_zh/
+-rw-rw-rw-   0 root         (0) root         (0)     8250 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/help/doc/docs_zh/配置文件文档之Maya.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/help/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     3338 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/help/examples/houdini_demo.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/help/examples/only_analyze.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/help/scenes/
+-rw-rw-rw-   0 root         (0) root         (0)   277555 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/help/scenes/sphere.hip
+-rw-rw-rw-   0 root         (0) root         (0)      452 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/init_pycharm_setup.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/rayvision_houdini/
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-09-06 06:16:59.000000 rayvision_houdini-1.4.5/rayvision_houdini/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15977 2023-04-23 06:59:02.000000 rayvision_houdini-1.4.5/rayvision_houdini/analyze_houdini.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/rayvision_houdini/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/
+-rw-rw-rw-   0 root         (0) root         (0)      498 2022-09-06 06:09:27.000000 rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py27/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py27/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   529920 2022-09-06 03:24:39.000000 rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py27/hanalyse.pyd
+-rw-rw-rw-   0 root         (0) root         (0)  3939328 2022-09-06 03:24:39.000000 rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py27/hanalyse.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py37/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py37/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   540672 2022-09-06 03:24:39.000000 rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py37/hanalyse.pyd
+-rw-rw-rw-   0 root         (0) root         (0)  5020992 2022-09-06 03:24:40.000000 rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py37/hanalyse.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py39/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2022-09-06 03:41:48.000000 rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py39/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   542720 2022-09-06 03:24:40.000000 rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py39/hanalyse.pyd
+-rw-rw-rw-   0 root         (0) root         (0)  5168064 2022-09-06 03:24:40.000000 rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py39/hanalyse.so
+-rw-rw-rw-   0 root         (0) root         (0)      787 2022-09-06 04:23:37.000000 rayvision_houdini-1.4.5/rayvision_houdini/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/rayvision_houdini/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/rayvision_houdini/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2022-09-06 03:45:31.000000 rayvision_houdini-1.4.5/rayvision_houdini/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      949 2022-09-06 06:16:59.000000 rayvision_houdini-1.4.5/rayvision_houdini/tests/test_analyze_houdini.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/rayvision_houdini.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/rayvision_houdini.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/rayvision_houdini.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/rayvision_houdini.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/rayvision_houdini.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-05 06:37:05.000000 rayvision_houdini-1.4.5/rayvision_houdini.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-28 04:38:46.000000 rayvision_houdini-1.4.5/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-05 06:37:06.000000 rayvision_houdini-1.4.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2021-11-25 02:46:16.000000 rayvision_houdini-1.4.5/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     3073 2023-05-05 06:19:19.000000 rayvision_houdini-1.4.5/tox.ini
```

### Comparing `rayvision_houdini-1.4.2/.pre-commit-config.yaml` & `rayvision_houdini-1.4.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/README.md` & `rayvision_houdini-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/docs/Makefile` & `rayvision_houdini-1.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/docs/conf.py` & `rayvision_houdini-1.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/docs/index.rst` & `rayvision_houdini-1.4.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/docs/make.bat` & `rayvision_houdini-1.4.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/docs/rayvision_houdini/first_look.rst` & `rayvision_houdini-1.4.5/docs/rayvision_houdini/first_look.rst`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/docs/rayvision_houdini/installation_guide.rst` & `rayvision_houdini-1.4.5/docs/rayvision_houdini/installation_guide.rst`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/help/doc/docs/Configuration Documentation--Maya.md` & `rayvision_houdini-1.4.5/help/doc/docs/Configuration Documentation--Maya.md`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/help/doc/docs_zh/配置文件文档之Maya.md` & `rayvision_houdini-1.4.5/help/doc/docs_zh/配置文件文档之Maya.md`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/help/examples/houdini_demo.py` & `rayvision_houdini-1.4.5/help/examples/houdini_demo.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/help/scenes/sphere.hip` & `rayvision_houdini-1.4.5/help/scenes/sphere.hip`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/rayvision_houdini/analyze_houdini.py` & `rayvision_houdini-1.4.5/rayvision_houdini/analyze_houdini.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,16 +220,14 @@
 
                     # The $HIP val with this file saved
                     if "set -g HIP = " in str(line):
                         search_elm_cunt += 1
                     if search_elm_cunt >= search_elm:
                         not_find = False
         else:
-            self.add_tip(tips_code.CGFILE_NOTEXISTS, cg_file)
-            self.save_tips()
             raise CGFileNotExistsError(ERROR_CGFILE_NOTEXIST.format(
                 cg_file))
         self.logger.info("_hfs_save_version---%s", _hfs_save_version)
         return _hfs_save_version
 
     def _get_install_path(self, version):
         location = None
@@ -318,16 +316,14 @@
                         VERSION_NOT_MATCH.format(version))
                 else:
                     return self._get_install_path(version)
             else:
                 error_msg = "Cannot found any houdini version"
                 self.logger.error("%s: %s", error_msg, version)
                 if version != "":
-                    self.add_tip(tips_code.CG_NOTEXISTS, error_msg)
-                    self.save_tips()
                     raise CGExeNotExistError(
                         ERROR9899_CGEXE_NOTEXIST.format(version))
         except Exception as e:
             traceback.format_exc()
             raise e
 
     def find_location(self):
@@ -347,17 +343,14 @@
         else:
             location = self.location_from_reg(self.software_version)
             tmp_exe_path = os.path.join(location, "bin", "hython.exe")
             if os.path.exists(tmp_exe_path):
                 exe_path = tmp_exe_path
 
         if exe_path is None:
-            error_msg = "Software of scene has not been found"
-            self.add_tip(tips_code.CG_NOTEXISTS, error_msg)
-            self.save_tips()
             raise CGExeNotExistError(ERROR9899_CGEXE_NOTEXIST.format(
                 self.render_software))
 
         self.logger.info("exe_path: %s", exe_path)
         return exe_path
 
     def analyse_cg_file(self):
```

### Comparing `rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py27/hanalyse.so` & `rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py27/hanalyse.so`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py37/hanalyse.so` & `rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py37/hanalyse.so`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/rayvision_houdini/hanalyse/py39/hanalyse.so` & `rayvision_houdini-1.4.5/rayvision_houdini/hanalyse/py39/hanalyse.so`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/rayvision_houdini/run.py` & `rayvision_houdini-1.4.5/rayvision_houdini/run.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/rayvision_houdini/tests/conftest.py` & `rayvision_houdini-1.4.5/rayvision_houdini/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/rayvision_houdini/tests/test_analyze_houdini.py` & `rayvision_houdini-1.4.5/rayvision_houdini/tests/test_analyze_houdini.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/rayvision_houdini.egg-info/SOURCES.txt` & `rayvision_houdini-1.4.5/rayvision_houdini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/setup.py` & `rayvision_houdini-1.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `rayvision_houdini-1.4.2/tox.ini` & `rayvision_houdini-1.4.5/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 commands =
   pytest --cov={env:CI_PROJECT_NAME} --cov-append {posargs}
 
 [testenv:deploy]
 deps =
     twine
 commands =
+    pip install requests==2.28.2
     python setup.py bdist_wheel register -r rayvision_pip upload -r rayvision_pip
     python setup.py sdist
     twine upload --repository pypi dist/*
 
 [testenv:pre-commit]
 skip_install = true
 deps =  pre-commit
```

