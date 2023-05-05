# Comparing `tmp/econpizza-0.5.4.tar.gz` & `tmp/econpizza-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econpizza-0.5.4.tar", last modified: Sat Apr 15 12:47:11 2023, max compression
+gzip compressed data, was "econpizza-0.5.5.tar", last modified: Fri May  5 14:43:28 2023, max compression
```

## Comparing `econpizza-0.5.4.tar` & `econpizza-0.5.5.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.098390 econpizza-0.5.4/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.085056 econpizza-0.5.4/.github/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.085056 econpizza-0.5.4/.github/workflows/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1527 2023-04-15 12:29:25.000000 econpizza-0.5.4/.github/workflows/continuous-integration.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-03-17 19:22:56.000000 econpizza-0.5.4/.gitignore
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-03-19 10:47:42.000000 econpizza-0.5.4/.pre-commit-config.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-03-22 13:14:47.000000 econpizza-0.5.4/.readthedocs.yaml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-03-02 09:28:46.000000 econpizza-0.5.4/LICENSE
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3817 2023-04-15 12:47:11.098390 econpizza-0.5.4/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3339 2023-03-23 23:42:13.000000 econpizza-0.5.4/README.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.088390 econpizza-0.5.4/docs/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-03-02 09:28:46.000000 econpizza-0.5.4/docs/Makefile
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.085056 econpizza-0.5.4/docs/_static/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.088390 econpizza-0.5.4/docs/_static/css/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-03-02 09:28:46.000000 econpizza-0.5.4/docs/_static/css/custom.css
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1539 2023-03-18 08:31:39.000000 econpizza-0.5.4/docs/conf.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      331 2023-03-22 14:25:19.000000 econpizza-0.5.4/docs/content.rst
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.088390 econpizza-0.5.4/docs/guide/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1278 2023-03-22 08:57:54.000000 econpizza-0.5.4/docs/guide/installation.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8245 2023-03-22 11:47:43.000000 econpizza-0.5.4/docs/guide/method.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1624 2023-03-30 06:43:39.000000 econpizza-0.5.4/docs/guide/solution.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2117 2023-03-30 06:41:47.000000 econpizza-0.5.4/docs/guide/steady_state.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    13122 2023-03-24 20:13:36.000000 econpizza-0.5.4/docs/guide/the_yaml.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2372 2023-03-22 12:36:34.000000 econpizza-0.5.4/docs/index.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    58150 2023-03-02 09:28:46.000000 econpizza-0.5.4/docs/lin_and_nlin.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2023-03-02 09:28:46.000000 econpizza-0.5.4/docs/make.bat
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    22585 2023-03-02 09:28:46.000000 econpizza-0.5.4/docs/p_and_n.png
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       80 2023-03-30 19:10:44.000000 econpizza-0.5.4/docs/requirements.txt
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.091723 econpizza-0.5.4/docs/tutorial/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2954 2023-03-10 20:34:11.000000 econpizza-0.5.4/docs/tutorial/boehl_hommes.rst
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   389792 2023-03-23 23:03:36.000000 econpizza-0.5.4/docs/tutorial/hank1.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   234012 2023-03-22 12:13:19.000000 econpizza-0.5.4/docs/tutorial/hank2.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    63713 2023-03-22 11:52:34.000000 econpizza-0.5.4/docs/tutorial/quickstart.ipynb
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)   407267 2023-03-22 12:01:00.000000 econpizza-0.5.4/docs/tutorial/rank.ipynb
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.091723 econpizza-0.5.4/econpizza/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3547 2023-03-28 11:53:45.000000 econpizza-0.5.4/econpizza/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       61 2023-04-15 12:23:21.000000 econpizza-0.5.4/econpizza/__version__.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.095057 econpizza-0.5.4/econpizza/examples/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      446 2023-03-25 22:11:17.000000 econpizza-0.5.4/econpizza/examples/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      770 2023-03-02 09:28:46.000000 econpizza-0.5.4/econpizza/examples/bh.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7079 2023-03-25 09:51:02.000000 econpizza-0.5.4/econpizza/examples/dsge.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4857 2023-03-25 10:04:56.000000 econpizza-0.5.4/econpizza/examples/ghls.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8709 2023-03-24 20:08:58.000000 econpizza-0.5.4/econpizza/examples/hank2.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5559 2023-03-14 23:49:18.000000 econpizza-0.5.4/econpizza/examples/hank2_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6656 2023-03-26 20:12:16.000000 econpizza-0.5.4/econpizza/examples/hank2_no_capital.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1652 2023-03-25 22:20:39.000000 econpizza-0.5.4/econpizza/examples/hank_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3716 2023-03-24 20:09:04.000000 econpizza-0.5.4/econpizza/examples/hank_labor.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3373 2023-03-15 14:58:36.000000 econpizza-0.5.4/econpizza/examples/hank_labor_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6137 2023-03-24 20:09:14.000000 econpizza-0.5.4/econpizza/examples/hank_with_comments.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1550 2023-04-11 07:59:18.000000 econpizza-0.5.4/econpizza/examples/nk.yml
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5512 2023-03-02 09:28:46.000000 econpizza-0.5.4/econpizza/examples/tank.yml
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.095057 econpizza-0.5.4/econpizza/parser/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)    12023 2023-03-31 05:55:10.000000 econpizza-0.5.4/econpizza/parser/__init__.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8145 2023-03-20 23:57:24.000000 econpizza-0.5.4/econpizza/parser/build_functions.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4728 2023-03-31 05:57:33.000000 econpizza-0.5.4/econpizza/parser/checks.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3237 2023-03-18 14:35:53.000000 econpizza-0.5.4/econpizza/parser/het_agent_base_funcs.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-03-30 18:29:58.000000 econpizza-0.5.4/econpizza/parser/write_dynamic_functions.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.095057 econpizza-0.5.4/econpizza/solvers/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6472 2023-03-10 20:34:11.000000 econpizza-0.5.4/econpizza/solvers/shooting.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2789 2023-03-18 09:32:31.000000 econpizza-0.5.4/econpizza/solvers/solve_linear.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4889 2023-03-10 20:34:11.000000 econpizza-0.5.4/econpizza/solvers/solve_linear_state_space.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5933 2023-03-18 08:06:49.000000 econpizza-0.5.4/econpizza/solvers/stacking.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8548 2023-03-28 11:53:45.000000 econpizza-0.5.4/econpizza/solvers/steady_state.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.095057 econpizza-0.5.4/econpizza/testing/
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.098390 econpizza-0.5.4/econpizza/testing/cache/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1760 2023-03-14 23:53:28.000000 econpizza-0.5.4/econpizza/testing/cache/bh.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7064 2023-03-14 23:54:36.000000 econpizza-0.5.4/econpizza/testing/cache/hank_labor.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2984 2023-03-14 23:55:47.000000 econpizza-0.5.4/econpizza/testing/cache/hank_solid.npy
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      416 2023-03-18 09:32:45.000000 econpizza-0.5.4/econpizza/testing/test_nb_hank1.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      416 2023-03-18 09:32:45.000000 econpizza-0.5.4/econpizza/testing/test_nb_hank2.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      421 2023-03-18 09:32:45.000000 econpizza-0.5.4/econpizza/testing/test_nb_quickstart.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      415 2023-03-18 09:32:45.000000 econpizza-0.5.4/econpizza/testing/test_nb_rank.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      414 2023-03-18 09:32:45.000000 econpizza-0.5.4/econpizza/testing/test_nb_under_the_hood.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1877 2023-03-18 09:26:41.000000 econpizza-0.5.4/econpizza/testing/test_rest.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      940 2023-03-10 20:34:11.000000 econpizza-0.5.4/econpizza/tools.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.098390 econpizza-0.5.4/econpizza/utilities/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3391 2023-03-18 14:36:19.000000 econpizza-0.5.4/econpizza/utilities/dists.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-03-30 15:12:39.000000 econpizza-0.5.4/econpizza/utilities/grids.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4688 2023-03-25 22:22:00.000000 econpizza-0.5.4/econpizza/utilities/interp.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4173 2023-03-30 22:34:43.000000 econpizza-0.5.4/econpizza/utilities/jacobian.py
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5575 2023-03-28 17:26:05.000000 econpizza-0.5.4/econpizza/utilities/newton.py
-drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-04-15 12:47:11.091723 econpizza-0.5.4/econpizza.egg-info/
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3817 2023-04-15 12:47:10.000000 econpizza-0.5.4/econpizza.egg-info/PKG-INFO
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2060 2023-04-15 12:47:11.000000 econpizza-0.5.4/econpizza.egg-info/SOURCES.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-04-15 12:47:10.000000 econpizza-0.5.4/econpizza.egg-info/dependency_links.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       77 2023-04-15 12:47:10.000000 econpizza-0.5.4/econpizza.egg-info/requires.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       10 2023-04-15 12:47:10.000000 econpizza-0.5.4/econpizza.egg-info/top_level.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)      113 2023-04-15 12:24:38.000000 econpizza-0.5.4/requirements.txt
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-04-15 12:47:11.098390 econpizza-0.5.4/setup.cfg
--rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1330 2023-04-15 12:24:22.000000 econpizza-0.5.4/setup.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.226970 econpizza-0.5.5/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.063634 econpizza-0.5.5/.github/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.076968 econpizza-0.5.5/.github/workflows/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1527 2023-04-15 12:29:25.000000 econpizza-0.5.5/.github/workflows/continuous-integration.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      173 2023-03-17 19:22:56.000000 econpizza-0.5.5/.gitignore
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      287 2023-03-19 10:47:42.000000 econpizza-0.5.5/.pre-commit-config.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      599 2023-03-22 13:14:47.000000 econpizza-0.5.5/.readthedocs.yaml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1079 2023-03-02 09:28:46.000000 econpizza-0.5.5/LICENSE
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3829 2023-05-05 14:43:28.226970 econpizza-0.5.5/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3351 2023-05-05 14:03:24.000000 econpizza-0.5.5/README.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.096968 econpizza-0.5.5/docs/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      634 2023-03-02 09:28:46.000000 econpizza-0.5.5/docs/Makefile
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.066968 econpizza-0.5.5/docs/_static/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.096968 econpizza-0.5.5/docs/_static/css/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       55 2023-03-02 09:28:46.000000 econpizza-0.5.5/docs/_static/css/custom.css
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1551 2023-05-02 19:15:35.000000 econpizza-0.5.5/docs/conf.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      331 2023-03-22 14:25:19.000000 econpizza-0.5.5/docs/content.rst
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.103635 econpizza-0.5.5/docs/guide/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1507 2023-04-22 17:10:18.000000 econpizza-0.5.5/docs/guide/installation.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8245 2023-03-22 11:47:43.000000 econpizza-0.5.5/docs/guide/method.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2384 2023-04-22 17:32:46.000000 econpizza-0.5.5/docs/guide/solution.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2117 2023-03-30 06:41:47.000000 econpizza-0.5.5/docs/guide/steady_state.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    14328 2023-05-02 15:47:57.000000 econpizza-0.5.5/docs/guide/the_yaml.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2362 2023-05-02 19:11:53.000000 econpizza-0.5.5/docs/index.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    58150 2023-03-02 09:28:46.000000 econpizza-0.5.5/docs/lin_and_nlin.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      800 2023-03-02 09:28:46.000000 econpizza-0.5.5/docs/make.bat
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    22585 2023-03-02 09:28:46.000000 econpizza-0.5.5/docs/p_and_n.png
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       80 2023-03-30 19:10:44.000000 econpizza-0.5.5/docs/requirements.txt
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.176969 econpizza-0.5.5/docs/tutorial/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2954 2023-03-10 20:34:11.000000 econpizza-0.5.5/docs/tutorial/boehl_hommes.rst
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   389792 2023-03-23 23:03:36.000000 econpizza-0.5.5/docs/tutorial/hank1.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   234012 2023-03-22 12:13:19.000000 econpizza-0.5.5/docs/tutorial/hank2.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    63713 2023-03-22 11:52:34.000000 econpizza-0.5.5/docs/tutorial/quickstart.ipynb
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)   407267 2023-03-22 12:01:00.000000 econpizza-0.5.5/docs/tutorial/rank.ipynb
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.206970 econpizza-0.5.5/econpizza/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3547 2023-03-28 11:53:45.000000 econpizza-0.5.5/econpizza/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       47 2023-05-05 14:43:17.000000 econpizza-0.5.5/econpizza/__version__.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.213636 econpizza-0.5.5/econpizza/examples/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      446 2023-03-25 22:11:17.000000 econpizza-0.5.5/econpizza/examples/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      770 2023-03-02 09:28:46.000000 econpizza-0.5.5/econpizza/examples/bh.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7079 2023-03-25 09:51:02.000000 econpizza-0.5.5/econpizza/examples/dsge.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4857 2023-03-25 10:04:56.000000 econpizza-0.5.5/econpizza/examples/ghls.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8709 2023-03-24 20:08:58.000000 econpizza-0.5.5/econpizza/examples/hank2.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5559 2023-03-14 23:49:18.000000 econpizza-0.5.5/econpizza/examples/hank2_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6656 2023-03-26 20:12:16.000000 econpizza-0.5.5/econpizza/examples/hank2_no_capital.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1652 2023-03-25 22:20:39.000000 econpizza-0.5.5/econpizza/examples/hank_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3716 2023-03-24 20:09:04.000000 econpizza-0.5.5/econpizza/examples/hank_labor.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3373 2023-03-15 14:58:36.000000 econpizza-0.5.5/econpizza/examples/hank_labor_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6137 2023-03-24 20:09:14.000000 econpizza-0.5.5/econpizza/examples/hank_with_comments.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1550 2023-04-11 07:59:18.000000 econpizza-0.5.5/econpizza/examples/nk.yml
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     5512 2023-03-02 09:28:46.000000 econpizza-0.5.5/econpizza/examples/tank.yml
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.216970 econpizza-0.5.5/econpizza/parser/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)    12023 2023-03-31 05:55:10.000000 econpizza-0.5.5/econpizza/parser/__init__.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8145 2023-03-20 23:57:24.000000 econpizza-0.5.5/econpizza/parser/build_functions.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4728 2023-04-21 09:07:56.000000 econpizza-0.5.5/econpizza/parser/checks.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3237 2023-03-18 14:35:53.000000 econpizza-0.5.5/econpizza/parser/het_agent_base_funcs.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-03-30 18:29:58.000000 econpizza-0.5.5/econpizza/parser/write_dynamic_functions.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.220303 econpizza-0.5.5/econpizza/solvers/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6472 2023-03-10 20:34:11.000000 econpizza-0.5.5/econpizza/solvers/shooting.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2789 2023-03-18 09:32:31.000000 econpizza-0.5.5/econpizza/solvers/solve_linear.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4889 2023-03-10 20:34:11.000000 econpizza-0.5.5/econpizza/solvers/solve_linear_state_space.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6106 2023-05-05 14:02:18.000000 econpizza-0.5.5/econpizza/solvers/stacking.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     8549 2023-05-05 11:51:37.000000 econpizza-0.5.5/econpizza/solvers/steady_state.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.220303 econpizza-0.5.5/econpizza/testing/
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.223636 econpizza-0.5.5/econpizza/testing/cache/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1760 2023-03-14 23:53:28.000000 econpizza-0.5.5/econpizza/testing/cache/bh.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     7064 2023-03-14 23:54:36.000000 econpizza-0.5.5/econpizza/testing/cache/hank_labor.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2984 2023-03-14 23:55:47.000000 econpizza-0.5.5/econpizza/testing/cache/hank_solid.npy
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:35:27.000000 econpizza-0.5.5/econpizza/testing/test_nb_hank1.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      429 2023-04-20 15:44:49.000000 econpizza-0.5.5/econpizza/testing/test_nb_hank2.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      421 2023-03-18 09:32:45.000000 econpizza-0.5.5/econpizza/testing/test_nb_quickstart.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      415 2023-03-18 09:32:45.000000 econpizza-0.5.5/econpizza/testing/test_nb_rank.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      414 2023-03-18 09:32:45.000000 econpizza-0.5.5/econpizza/testing/test_nb_under_the_hood.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1877 2023-03-18 09:26:41.000000 econpizza-0.5.5/econpizza/testing/test_rest.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      940 2023-03-10 20:34:11.000000 econpizza-0.5.5/econpizza/tools.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.226970 econpizza-0.5.5/econpizza/utilities/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3391 2023-03-18 14:36:19.000000 econpizza-0.5.5/econpizza/utilities/dists.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4185 2023-04-27 11:18:13.000000 econpizza-0.5.5/econpizza/utilities/grids.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4769 2023-05-04 15:35:28.000000 econpizza-0.5.5/econpizza/utilities/interp.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     4173 2023-03-30 22:34:43.000000 econpizza-0.5.5/econpizza/utilities/jacobian.py
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     6363 2023-05-05 14:02:55.000000 econpizza-0.5.5/econpizza/utilities/newton.py
+drwxr-xr-x   0 gboehl    (1000) gboehl    (1000)        0 2023-05-05 14:43:28.206970 econpizza-0.5.5/econpizza.egg-info/
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     3829 2023-05-05 14:43:27.000000 econpizza-0.5.5/econpizza.egg-info/PKG-INFO
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     2060 2023-05-05 14:43:27.000000 econpizza-0.5.5/econpizza.egg-info/SOURCES.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)        1 2023-05-05 14:43:27.000000 econpizza-0.5.5/econpizza.egg-info/dependency_links.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       77 2023-05-05 14:43:27.000000 econpizza-0.5.5/econpizza.egg-info/requires.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       10 2023-05-05 14:43:27.000000 econpizza-0.5.5/econpizza.egg-info/top_level.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)      113 2023-04-15 12:24:38.000000 econpizza-0.5.5/requirements.txt
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)       38 2023-05-05 14:43:28.226970 econpizza-0.5.5/setup.cfg
+-rw-r--r--   0 gboehl    (1000) gboehl    (1000)     1330 2023-04-15 12:24:22.000000 econpizza-0.5.5/setup.py
```

### Comparing `econpizza-0.5.4/.github/workflows/continuous-integration.yml` & `econpizza-0.5.5/.github/workflows/continuous-integration.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/.readthedocs.yaml` & `econpizza-0.5.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/LICENSE` & `econpizza-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/PKG-INFO` & `econpizza-0.5.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econpizza
-Version: 0.5.4
+Version: 0.5.5
 Summary: Solve nonlinear perfect foresight models with heterogeneous agents
 Home-page: https://github.com/gboehl/econpizza
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
     :target: https://github.com/gboehl/econpizza/actions
 .. image:: https://readthedocs.org/projects/econpizza/badge/?version=latest
     :target: http://econpizza.readthedocs.io/en/latest/?badge=latest
 .. image:: https://badge.fury.io/py/econpizza.svg
     :target: https://badge.fury.io/py/econpizza
 
 **Econpizza** is a framework to solve and simulate *fully nonlinear* perfect foresight models, with or without heterogeneous agents.
-The package implements the solution method proposed in `Robust Nonlinear Transition Dynamics in HANK <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023)*.
+The package implements the solution method proposed in `Robust Nonlinear Transition Dynamics in HANK <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023, SSRN No. 4433585)*.
 It allows to specify and solve nonlinear macroeconomic models quickly in a simple, high-level fashion.
 Generic and robust routines for steady state search are provided.
 
 The package can solve nonlinear models with heterogeneous agents, such as HANK models with one or two assets and portfolio choice. Steady state and nonlinear impulse responses (including, e.g., the ELB) can typically be found within a few seconds.
 The method extends the `Sequence-Space Jacobian <https://github.com/shade-econ/sequence-jacobian>`_ method (`Auclert et al., 2022, ECMA <https://doi.org/10.3982/ECTA17434>`_) to fully nonlinear heterogeneous agent models models by iteratively using `Jacobian-vector producs <https://jax.readthedocs.io/en/latest/notebooks/autodiff_cookbook.html#how-it-s-made-two-foundational-autodiff-functions>`_ to approximate the solution to the linear system of equations associated with each Newton iteration. This not only allows to study the dynamics of aggregate variables, but also the complete nonlinear transition dynamics of the cross-sectional distribution of assets and disaggregated objects.
 
 To solve models with representative agents a shooting methods similar to Laffargue (1990), Boucekkine (1995) and Juillard (1996) is implemented. It is faster and more reliable than the extended path method in dynare due to the use of automatic differentiation for the efficient jacobian decompositions during each Newton-step. Nonlinear perfect-foresight transition dynamics can - even for large-scale nonlinear models with several occassionally binding constraints - be computed in less than a second.
@@ -49,13 +49,13 @@
  * `User guide <https://econpizza.readthedocs.io/en/stable/index.html>`_
  * `Quickstart tutorial <https://econpizza.readthedocs.io/en/stable/tutorial/quickstart.html>`_
 
 Citation
 --------
 .. code-block:: bibtex
 
-    @Misc{boehl2022pizza,
-    title         = {Robust Nonlinear Transition Dynamics in HANK},
-    author        = {Boehl, Gregor},
-    howpublished  = {\url{https://gregorboehl.com/live/hank_speed_boehl.pdf}},
-    year = {2023}
+    @article{boehl2023goodpizza,
+        title       = {Robust Nonlinear Transition Dynamics in HANK},
+        author      = {Boehl, Gregor},
+        journal     = {Available at SSRN 4433585},
+        year        = {2023}
     }
```

### Comparing `econpizza-0.5.4/README.rst` & `econpizza-0.5.5/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     :target: https://github.com/gboehl/econpizza/actions
 .. image:: https://readthedocs.org/projects/econpizza/badge/?version=latest
     :target: http://econpizza.readthedocs.io/en/latest/?badge=latest
 .. image:: https://badge.fury.io/py/econpizza.svg
     :target: https://badge.fury.io/py/econpizza
 
 **Econpizza** is a framework to solve and simulate *fully nonlinear* perfect foresight models, with or without heterogeneous agents.
-The package implements the solution method proposed in `Robust Nonlinear Transition Dynamics in HANK <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023)*.
+The package implements the solution method proposed in `Robust Nonlinear Transition Dynamics in HANK <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023, SSRN No. 4433585)*.
 It allows to specify and solve nonlinear macroeconomic models quickly in a simple, high-level fashion.
 Generic and robust routines for steady state search are provided.
 
 The package can solve nonlinear models with heterogeneous agents, such as HANK models with one or two assets and portfolio choice. Steady state and nonlinear impulse responses (including, e.g., the ELB) can typically be found within a few seconds.
 The method extends the `Sequence-Space Jacobian <https://github.com/shade-econ/sequence-jacobian>`_ method (`Auclert et al., 2022, ECMA <https://doi.org/10.3982/ECTA17434>`_) to fully nonlinear heterogeneous agent models models by iteratively using `Jacobian-vector producs <https://jax.readthedocs.io/en/latest/notebooks/autodiff_cookbook.html#how-it-s-made-two-foundational-autodiff-functions>`_ to approximate the solution to the linear system of equations associated with each Newton iteration. This not only allows to study the dynamics of aggregate variables, but also the complete nonlinear transition dynamics of the cross-sectional distribution of assets and disaggregated objects.
 
 To solve models with representative agents a shooting methods similar to Laffargue (1990), Boucekkine (1995) and Juillard (1996) is implemented. It is faster and more reliable than the extended path method in dynare due to the use of automatic differentiation for the efficient jacobian decompositions during each Newton-step. Nonlinear perfect-foresight transition dynamics can - even for large-scale nonlinear models with several occassionally binding constraints - be computed in less than a second.
@@ -34,13 +34,13 @@
  * `User guide <https://econpizza.readthedocs.io/en/stable/index.html>`_
  * `Quickstart tutorial <https://econpizza.readthedocs.io/en/stable/tutorial/quickstart.html>`_
 
 Citation
 --------
 .. code-block:: bibtex
 
-    @Misc{boehl2022pizza,
-    title         = {Robust Nonlinear Transition Dynamics in HANK},
-    author        = {Boehl, Gregor},
-    howpublished  = {\url{https://gregorboehl.com/live/hank_speed_boehl.pdf}},
-    year = {2023}
+    @article{boehl2023goodpizza,
+        title       = {Robust Nonlinear Transition Dynamics in HANK},
+        author      = {Boehl, Gregor},
+        journal     = {Available at SSRN 4433585},
+        year        = {2023}
     }
```

### Comparing `econpizza-0.5.4/docs/Makefile` & `econpizza-0.5.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/docs/conf.py` & `econpizza-0.5.5/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # must be called AFTER the above:
 from econpizza import __version__
 # autopep8: on
 
 
 # -- Project information -----------------------------------------------------
 project = 'econpizza'
-copyright = '2022, Gregor Boehl'
+copyright = '2023, Gregor Boehl'
 author = 'Gregor Boehl'
 version = __version__
 release = version
 
 # -- General configuration ---------------------------------------------------
 extensions = [
     "nbsphinx",
@@ -32,23 +32,24 @@
 html_theme = "sphinx_book_theme"
 html_copy_source = True
 html_show_sourcelink = True
 html_sourcelink_suffix = ""
 html_title = "econpizza"
 html_theme_options = {
     "path_to_docs": "docs",
+    "show_toc_level": 9,
     "repository_url": "https://github.com/gboehl/econpizza",
     "repository_branch": "main",
     "launch_buttons": {
-        "binderhub_url": "https://mybinder.org",
         "notebook_interface": "classic",
     },
     "use_edit_page_button": True,
     "use_issues_button": True,
     "use_repository_button": True,
     "use_download_button": True,
+    "use_fullscreen_button": False,
 }
 
 autoclass_content = "both"
 autodoc_member_order = "bysource"
 master_doc = 'content'
 latex_use_parts = False
```

### Comparing `econpizza-0.5.4/docs/guide/installation.rst` & `econpizza-0.5.5/docs/guide/installation.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Installation
 ============
 
+On Linux & MacOS
+----------------
+
 Installing the `repository version <https://pypi.org/project/econpizza/>`_ from PyPi is as simple as typing
 
 .. code-block:: bash
 
    pip install econpizza
 
 in your terminal or Anaconda Prompt.
 
 On Windows
 ----------
 
-Econpizza needs the Python package `JAX <https://jax.readthedocs.io>`_ to be installed. This is not a problem for MacOS and Linux (the package will be automatically installed when installing Econpizza), but the time for JAX to fully support Windows has not yet come. Fortunately, there is help out there (see `this link <https://github.com/cloudhan/jax-windows-builder>`_ for the somewhat cryptic original reference). To install JAX, run
+Econpizza depends on the Python package `JAX <https://jax.readthedocs.io>`_. This is not a problem for MacOS and Linux (the package will be automatically installed when installing Econpizza), prebuild binaries do not yet exist for Windows. Fortunately, some unofficial binaries exist (see `this link <https://github.com/cloudhan/jax-windows-builder>`_).
+One way to install JAX on Windows is thus to run
 
 .. code-block:: bash
 
     pip install "jax[cpu]===0.3.25" -f https://whls.blob.core.windows.net/unstable/index.html --use-deprecated legacy-resolver
 
-*prior* to installing Econpizza. Econpizza should then run just fine (`proof <https://github.com/gboehl/econpizza/actions/runs/2579662335>`_).
+in your terminal or Anaconda Prompt, *prior* to installing Econpizza. Then continue as for Linux and Mac. Econpizza then just runns fine (`proof <https://github.com/gboehl/econpizza/actions/runs/2579662335>`_). Alternatively to using the unofficial binaries, you can consult the `JAX installation guide <https://github.com/google/jax#installation>`_.
 
-In case you run into an error with `ptxas` (like `in this case <https://github.com/tensorflow/models/issues/7640>`_), a workaround is to disable CUDA by adding the following line **before** importing econpizza or JAX:
+In case you run into an error with `ptxas` (like `in this case <https://github.com/tensorflow/models/issues/7640>`_), a workaround is to disable CUDA by running the following line **before** importing econpizza or JAX in your python code:
 
 .. code-block:: python
 
     import os; os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
```

### Comparing `econpizza-0.5.4/docs/guide/method.ipynb` & `econpizza-0.5.5/docs/guide/method.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/docs/guide/solution.rst` & `econpizza-0.5.5/docs/guide/solution.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 Nonlinear simulations
 =====================
 
-The main functionality of nonlinear simulations is provided by the functions :meth:`econpizza.PizzaModel.find_path`. The main arguments are either ``shock`` or ``init_state``, which allows to specify an economic shock as a tuple of the shock name (as specified in ``shocks`` in the YAML) and the size of the shock, or a vector of initial states, respectively.
+The main functionality of nonlinear simulations is provided by the function :meth:`econpizza.PizzaModel.find_path`
+The main arguments are either ``shock`` or ``init_state``, which allows to specify an economic shock as a tuple of the shock name (as specified in ``shocks`` in the YAML) and the size of the shock, or a vector of initial states, respectively.
+The function :meth:`econpizza.PizzaModel.get_distributions` allows to retrieve the full nonlinear sequence of the distribution.
 
 .. note::
 
    All numerical methods are subject to numerical errors. To reduce these, you can decrease the numerical tolerance ``tol``. However, this should not be below the tolerance level for the steady state search, or below machine precision.
 
 .. hint::
 
    As stated in the paper, a sufficient condition for convergence of the solution routine is that the generalized eigenvalues of the sequence space Jacobian and its steady-state pendant are all positive (which is prohibitory expensive to check). If the method does not converge, the ``use_solid_solver=True`` flag can be used to check if the model solves when using a conventional Newton method with the true Jacobian.
 
 .. autofunction:: econpizza.PizzaModel.find_path
 
 If the model has heterogeneous agents, the routine will automatically compute the steady state sequence space Jacobian. This can be skipped using the ``skip_jacobian`` flag.
 
+Any additional argument will be passed on to the specific Newton method. For models with heterogeneous agents this is :meth:`econpizza.utilities.newton.newton_for_jvp`:
+
+.. autofunction:: econpizza.utilities.newton.newton_for_jvp
+
+For models with representative agents, the Newton method is :meth:`econpizza.utilities.newton.newton_for_banded_jac`:
+
+.. autofunction:: econpizza.utilities.newton.newton_for_banded_jac
+
+If ``use_solid_solver`` is set to `True`, the Newton method `newton_jax_jit <https://grgrjax.readthedocs.io/en/latest/#grgrjax.newton_jax_jit>`_ from the `grgrjax <https://grgrjax.readthedocs.io>`_ package is used.
+
 The function :meth:`econpizza.PizzaModel.get_distributions` allows to retrieve the sequence of distributions and decision variables. To that end it requires the shocks and initial distribution together with the trajectory of aggregated variables as input.
 
 .. autofunction:: econpizza.PizzaModel.get_distributions
```

### Comparing `econpizza-0.5.4/docs/guide/steady_state.rst` & `econpizza-0.5.5/docs/guide/steady_state.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/docs/guide/the_yaml.rst` & `econpizza-0.5.5/docs/guide/the_yaml.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,38 @@
 
-Model parsing and the yaml-file
--------------------------------
+Specifying models
+-----------------
 
-All relevant information is supplied via the YAML file, which uses the YAML markup language.
-For general information about the YAML and its syntax see `Wikipedia <https://en.wikipedia.org/wiki/YAML>`_.
-
-Model parsing
-^^^^^^^^^^^^^
-
-Models specified as a YAML files can be parsed and loaded using :py:meth:`econpizza.parse` and :py:meth:`econpizza.load`.
-
-.. autofunction:: econpizza.parse
-
-This returns a dictionary containing all the informations provided in the YAML file. Parsing before loading allows to change some features of the model manually. The dictionary can then be forwarded to :py:meth:`econpizza.load`:
-
-.. autofunction:: econpizza.load
-
-If desired, :meth:`econpizza.load` can also parse the YAML-file directly. The function then returns an instance of
-:class:`econpizza.PizzaModel`, which holds all the relevant information and functionality of the model:
-
-.. autoclass:: econpizza.PizzaModel
+Models are specified in a YAML file, which uses the YAML markup language.
+The YAML format is widely used due to its intuitive handling,
+for example for configuration files or in applications where data is being stored or transmitted which should be human readable.
+For general information about the format and its syntax see `Wikipedia <https://en.wikipedia.org/wiki/YAML>`_.
+
+The YAML file contains all relevant information from model equations, variable declarations and steady state values.
+Models specified as a YAML files can be parsed into a :class:`econpizza.PizzaModel`
+using :py:meth:`econpizza.parse` or :py:meth:`econpizza.load`.
+An instance of :class:`econpizza.PizzaModel` holds all the relevant information and functionality of the model.
 
 The YAML file
 ^^^^^^^^^^^^^
 
 The YAML files follow a simple structure:
 
 1. list all variables, parameters and shocks
 2. provide the nonlinear equations. Note that each equation starts with a ``~``.
 3. define the values of the parameters and fixed steady state values in the ``steady_state`` section
-4. optionally provide auxilliary equations that are not directly part of the nonlinear system
+4. optionally provide auxiliary equations that are not directly part of the nonlinear system
 5. optionally provide initial guesses for all other steady state values and parameters
 
 I will first briefly discuss the YAML of the small scale *representative* agents NK model `from the quickstart tutorial <../tutorial/quickstart.ipynb>`_ and then turn to a more complex HANK model.
 
 YAML: representative agent models
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-The file for the small scale NK model can be found `here <https://github.com/gboehl/econpizza/blob/master/econpizza/examples/nk.yml>`_. The first block (``variables`` and ``shocks``) is self explanatory:
+The GitHub version of the YAML file for the small scale NK model can be found `here <https://github.com/gboehl/econpizza/blob/master/econpizza/examples/nk.yml>`_. The first block (``variables`` and ``shocks``) is self explanatory:
 
 .. code-block:: yaml
 
     variables: [y, c, pi, r, rn, beta, w, chi]
     shocks: [e_beta]
 
 Note that it is not necessary to define shocks. You can also simply set the initial values of any (exogenous) state.
@@ -98,21 +89,23 @@
 Finally, the ``steady_state`` block allows to fix parameters and, if desired, some steady state values, and provide initial guesses for others. Note that the default initial guess for any variable/parameter not specified here will be ``1.1``.
 
 
 YAML: heterogeneous agent models
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Let us have a look of the YAML of a hank model we will discuss in `the tutorial <../tutorial/hank1.ipynb>`_.
-`The file <https://github.com/gboehl/econpizza/blob/master/econpizza/examples/hank_with_comments.yml>`_ also contains exhaustive additional comments. The first line reads:
+The GitHub version of the file (`link <https://github.com/gboehl/econpizza/blob/master/econpizza/examples/hank_with_comments.yml>`_) also contains exhaustive additional comments. The first line reads:
 
 .. code-block:: yaml
 
     functions_file: 'hank_functions.py'
 
-The relative path to a functions-file, which may provide additional functions. In this example, the file defines the functions ``transfers``, ``wages``, ``hh``, ``labor_supply`` and ``hh_init``.
+The relative path to a functions-file, which may provide additional functions.
+The GitHub version of the functions file for this model `can be found here <https://github.com/gboehl/econpizza/blob/master/econpizza/examples/hank_functions.py>`_.
+In this example, the file defines the functions ``transfers``, ``wages``, ``hh``, ``labor_supply`` and ``hh_init``.
 
 .. code-block:: yaml
 
     definitions: |
         from jax.numpy import log, maximum
         from econpizza.tools import percentile, jax_print
 
@@ -258,7 +251,29 @@
             R: Rstar # steady state nominal rage
             tax: 0.028
             WaPrime: egm_init(a_grid, skills_stationary)
 
 The steady state block. ``fixed_values`` are those steady state values that are fixed ex-ante. ``init_guesses`` are initial guesses for steady state finding. Values are defined from the top to the bottom, so it is possible to use recursive definitions, such as ``n: w**frisch``.
 
 Note that for heterogeneous agents models it is required that the initial value of inputs to the decisions-stage are given (here ``WaPrime``).
+
+.. note::
+
+   `Econpizza` is written in `JAX <https://jax.readthedocs.io>`_, which is a machine learning framework for Python developed by Google. JAX provides automatic differentiation and just-in-time compilation ("jitting"), which makes the package fast and robust.
+   However, running jitted JAX code brings along a few limitations. Check the `common gotchas in JAX <https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html>`_ for details.
+
+
+Model parsing
+^^^^^^^^^^^^^
+
+Models specified as a YAML files can be parsed and loaded using :py:meth:`econpizza.parse` and :py:meth:`econpizza.load`.
+
+.. autofunction:: econpizza.parse
+
+This returns a dictionary containing all the informations provided in the YAML file. Parsing before loading allows to change some features of the model manually. The dictionary can then be forwarded to :py:meth:`econpizza.load`:
+
+.. autofunction:: econpizza.load
+
+If desired, :meth:`econpizza.load` can also parse the YAML-file directly. The function then returns an instance of
+:class:`econpizza.PizzaModel`, which holds all the relevant information and functionality of the model:
+
+.. autoclass:: econpizza.PizzaModel
```

### Comparing `econpizza-0.5.4/docs/index.rst` & `econpizza-0.5.5/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,35 +2,33 @@
 .. only:: latex
 
     This document is automatically created by `sphinx <https://www.sphinx-doc.org/en/master/index.html>`_, the Python documentation generator.
     It is synced with the online package documentation that is hosted at `Read the Docs <https://econpizza.readthedocs.io>`_.
 
 
 Overview: **Econpizza**
-=======================
+-----------------------
 
 **Econpizza** is a framework to solve and simulate *fully nonlinear* perfect foresight models, with or without heterogeneous agents.
-The package implements the solution method proposed in `Robust Nonlinear Transition Dynamics in HANK <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023)*.
+The package implements the solution method proposed in `Robust Nonlinear Transition Dynamics in HANK <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023, SSRN No. 4433585)*.
 It allows to specify and solve nonlinear macroeconomic models quickly in a simple, high-level fashion.
 
 The package builds heavily on `automatic differentiation <https://en.wikipedia.org/wiki/Automatic_differentiation>`_ via `JAX <https://jax.readthedocs.io/en/latest/notebooks/quickstart.html>`_.
 A central philosophy is to consequently separate the low-level routines for *model solution* (which is what happens under the hood) from
 *model specification* (via a ``yaml`` file) and *model analysis* (what the user does with the model).
 
 The package can solve nonlinear models with heterogeneous households or firms with one or two assets and portfolio choice. Steady state and nonlinear impulse responses (including, e.g., the ZLB) can typically be found within a few seconds.
 It not only allows to study the dynamics of aggregate variables, but also the complete nonlinear transition dynamics of the cross-sectional distribution of assets and disaggregated objects. Routines for models with a representative agents are also provided. These are faster and more reliable than the extended path method in dynare due to the use of automatic differentiation for the efficient Jacobian decompositions during each Newton-step. Nonlinear perfect-foresight transition dynamics can - even for large-scale nonlinear models with several occassionally binding constraints - be computed in less than a second.
 
-.. only:: html
-
-    References
-    ----------
+How to cite
+-----------
 
 Please cite with
 
 .. code-block:: bibtex
 
-    @Misc{boehl2022pizza,
-    title         = {Robust Nonlinear Transition Dynamics in HANK},
-    author        = {Boehl, Gregor},
-    howpublished  = {\url{https://gregorboehl.com/live/hank_speed_boehl.pdf}},
-    year = {2023}
+    @article{boehl2023goodpizza,
+        title       = {Robust Nonlinear Transition Dynamics in HANK},
+        author      = {Boehl, Gregor},
+        journal     = {Available at SSRN 4433585},
+        year        = {2023}
     }
```

### Comparing `econpizza-0.5.4/docs/lin_and_nlin.png` & `econpizza-0.5.5/docs/lin_and_nlin.png`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/docs/make.bat` & `econpizza-0.5.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/docs/p_and_n.png` & `econpizza-0.5.5/docs/p_and_n.png`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/docs/tutorial/boehl_hommes.rst` & `econpizza-0.5.5/docs/tutorial/boehl_hommes.rst`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/docs/tutorial/hank1.ipynb` & `econpizza-0.5.5/docs/tutorial/hank1.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/docs/tutorial/hank2.ipynb` & `econpizza-0.5.5/docs/tutorial/hank2.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/docs/tutorial/quickstart.ipynb` & `econpizza-0.5.5/docs/tutorial/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/docs/tutorial/rank.ipynb` & `econpizza-0.5.5/docs/tutorial/rank.ipynb`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/__init__.py` & `econpizza-0.5.5/econpizza/__init__.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/examples/bh.yml` & `econpizza-0.5.5/econpizza/examples/bh.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/examples/dsge.yml` & `econpizza-0.5.5/econpizza/examples/dsge.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/examples/ghls.yml` & `econpizza-0.5.5/econpizza/examples/ghls.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/examples/hank2.yml` & `econpizza-0.5.5/econpizza/examples/hank2.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/examples/hank2_functions.py` & `econpizza-0.5.5/econpizza/examples/hank2_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/examples/hank2_no_capital.yml` & `econpizza-0.5.5/econpizza/examples/hank2_no_capital.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/examples/hank_functions.py` & `econpizza-0.5.5/econpizza/examples/hank_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/examples/hank_labor.yml` & `econpizza-0.5.5/econpizza/examples/hank_labor.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/examples/hank_labor_functions.py` & `econpizza-0.5.5/econpizza/examples/hank_labor_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/examples/hank_with_comments.yml` & `econpizza-0.5.5/econpizza/examples/hank_with_comments.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/examples/nk.yml` & `econpizza-0.5.5/econpizza/examples/nk.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/examples/tank.yml` & `econpizza-0.5.5/econpizza/examples/tank.yml`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/parser/__init__.py` & `econpizza-0.5.5/econpizza/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/parser/build_functions.py` & `econpizza-0.5.5/econpizza/parser/build_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/parser/checks.py` & `econpizza-0.5.5/econpizza/parser/checks.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/parser/het_agent_base_funcs.py` & `econpizza-0.5.5/econpizza/parser/het_agent_base_funcs.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/parser/write_dynamic_functions.py` & `econpizza-0.5.5/econpizza/parser/write_dynamic_functions.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/solvers/shooting.py` & `econpizza-0.5.5/econpizza/solvers/shooting.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/solvers/solve_linear.py` & `econpizza-0.5.5/econpizza/solvers/solve_linear.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/solvers/solve_linear_state_space.py` & `econpizza-0.5.5/econpizza/solvers/solve_linear_state_space.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/solvers/stacking.py` & `econpizza-0.5.5/econpizza/solvers/stacking.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,22 +44,24 @@
         tial state
     init_dist : array, optional
         tial distribution
     pars : dict, optional
         alternative parameters. Warning: do only change those parameters that are invariant to the steady state.
     horizon : int, optional
         number of periods until the system is assumed to be back in the steady state. Defaults to 200
+    use_solid_solver : bool, optional
+        calculate the full jacobian and use a standard Newton method. Defaults to False
     skip_jacobian : bool, optional
         whether to skip the calculation of the steady state sequence space Jacobian. If True, the last cached Jacobian will be used. Defaults to False
     verbose : bool, optional
         degree of verbosity. 0/`False` is silent
     raise_errors : bool, optional
         whether to raise errors as exceptions, or just inform about them. Defaults to `True`
     newton_args : optional
-        any additional arguments to be passed on to the solver
+        any additional arguments to be passed on to the Newton solver (see the documentations of the solvers)
 
     Returns
     -------
     x : array
         array of the trajectory
     flag : bool
         returns False if the solver was successful, else True
```

### Comparing `econpizza-0.5.4/econpizza/solvers/steady_state.py` & `econpizza-0.5.5/econpizza/solvers/steady_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             if rank != nvars - nfixed:
                 mess += f"Jacobian has rank {rank} for {nvars - nfixed} degrees of freedom ({nvars} variables/parameters, {nfixed} fixed). "
 
     # check if any of the fixed variables are neither a parameter nor variable
     if mess:
         not_var_nor_par = list(
             set(model['steady_state']['fixed_values']) - set(evars) - set(par_names))
-        mess += f"Fixed value(s) ``{'``, ``'.join(not_var_nor_par)}`` not defined. " if not_var_nor_par else ''
+        mess += f"Fixed value(s) ``{'``, ``'.join(not_var_nor_par)}`` not declared. " if not_var_nor_par else ''
 
     if err > tol or not res['success']:
         if not res["success"] or raise_errors:
             location = '' if jnp.isnan(
                 err) else f" (max. error is {err:1.2e} in eqn. {errarg})"
             mess = f"Steady state FAILED{location}. {res['message']} {mess}"
         else:
```

### Comparing `econpizza-0.5.4/econpizza/testing/cache/bh.npy` & `econpizza-0.5.5/econpizza/testing/cache/bh.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/testing/cache/hank_labor.npy` & `econpizza-0.5.5/econpizza/testing/cache/hank_labor.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/testing/cache/hank_solid.npy` & `econpizza-0.5.5/econpizza/testing/cache/hank_solid.npy`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/testing/test_rest.py` & `econpizza-0.5.5/econpizza/testing/test_rest.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/tools.py` & `econpizza-0.5.5/econpizza/tools.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/utilities/dists.py` & `econpizza-0.5.5/econpizza/utilities/dists.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/utilities/grids.py` & `econpizza-0.5.5/econpizza/utilities/grids.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/utilities/interp.py` & `econpizza-0.5.5/econpizza/utilities/interp.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 
 import jax
 import jax.numpy as jnp
 from functools import partial
 from jax._src.typing import Array
 
 
+interpolate_numpy = jnp.vectorize(jnp.interp, signature='(nq),(n),(n)->(nq)')
+
+
 @partial(jnp.vectorize, signature='(n),(nq),(n)->(nq)')
 def interpolate(x: Array, xq: Array, y: Array) -> Array:
     """Efficient linear interpolation exploiting monotonicity.
 
     Complexity O(n+nq), so most efficient when x and xq have comparable number of points.
     Extrapolates linearly when xq out of domain of x.
 
     Parameters
     ----------
-    x  : array (n), ascending data points
+    x  : array (n), ascending input points
     xq : array (nq), ascending query points
     y  : array (n), data points
 
     Returns
     ----------
     yq : array (nq), interpolated points
     """
```

### Comparing `econpizza-0.5.4/econpizza/utilities/jacobian.py` & `econpizza-0.5.5/econpizza/utilities/jacobian.py`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/econpizza/utilities/newton.py` & `econpizza-0.5.5/econpizza/utilities/newton.py`

 * *Files 16% similar despite different names*

```diff
@@ -85,15 +85,28 @@
         return True, (False, "Function returns NaNs.")
     elif cnt >= maxit:
         return True, (False, f"Maximum number of {maxit} iterations reached.")
     else:
         return False, (False, "")
 
 
-def newton_for_jvp(jvp_func, jacobian, x_init, verbose, tol=1e-8, maxit=500, nsteps=30, factor=1.5):
+def newton_for_jvp(jvp_func, jacobian, x_init, verbose, tol=1e-8, maxit=20, nsteps=30, factor=1.5):
+    """Newton solver for heterogeneous agents models as described in the paper.
+
+    Parameters
+    ----------
+    tol : float, optional
+        tolerance of the Newton method, defaults to ``1e-8``
+    maxit : int, optional
+        maximum of iterations for the Newton method, defaults to 20
+    nsteps : int, optional
+        number of function evaluations per Newton iteration, defaults to 30
+    factor : float, optional
+        dampening factor (gamma in the paper), Defaults to 1.5
+    """
 
     start_time = time.time()
     x = x_init[1:-1].flatten()
 
     (x, err, dampening, cnt, fev, err_inner), _ = jax.lax.while_loop(jvp_while_cond, jvp_while_body,
                                                                      ((x, 1., 0., 0, 0, 0), (jvp_func, jacobian, maxit, nsteps, tol, factor, verbose)))
     ltime = time.time() - start_time
@@ -104,14 +117,23 @@
     if not success and not jnp.isnan(err):
         mess += f" Max. error is {err:1.2e}."
 
     return x, not success, mess
 
 
 def newton_for_banded_jac(jav_func, nvars, horizon, X, shocks, verbose, maxit=30, tol=1e-8):
+    """Newton solver for representative agents models.
+
+    Parameters
+    ----------
+    tol : float, optional
+        tolerance of the Newton method, defaults to ``1e-8``
+    maxit : int, optional
+        maximum of iterations for the Newton method, defaults to 20
+    """
 
     st = time.time()
     cnt = 0
 
     while True:
 
         _, (fvals, forward_mat) = jax.lax.scan(sweep_banded_down, (jav_func, jnp.zeros(
@@ -130,21 +152,21 @@
             print(info_str)
 
         do_break, (success, mess) = check_status(err, cnt, maxit, tol)
         if do_break:
             break
 
     if not success:
-        mess += f"Max. error is {err:1.2e}."
+        mess += f" Max. error is {err:1.2e}."
 
-    return X, False, ''
+    return X, not success, mess
 
 
 def newton_jax_jit_wrapper(func, init, **args):
-    """Wrapper around grgrjax.newton.newton_jax_jit to return flag and message
+    """Wrapper around grgrjax.newton.newton_jax_jit. Returns correct flags and messages.
     """
 
     if 'tol' not in args:
         args['tol'] = 1e-8
     if 'maxit' not in args:
         args['maxit'] = 30
```

### Comparing `econpizza-0.5.4/econpizza.egg-info/PKG-INFO` & `econpizza-0.5.5/econpizza.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econpizza
-Version: 0.5.4
+Version: 0.5.5
 Summary: Solve nonlinear perfect foresight models with heterogeneous agents
 Home-page: https://github.com/gboehl/econpizza
 Author: Gregor Boehl
 Author-email: admin@gregorboehl.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
     :target: https://github.com/gboehl/econpizza/actions
 .. image:: https://readthedocs.org/projects/econpizza/badge/?version=latest
     :target: http://econpizza.readthedocs.io/en/latest/?badge=latest
 .. image:: https://badge.fury.io/py/econpizza.svg
     :target: https://badge.fury.io/py/econpizza
 
 **Econpizza** is a framework to solve and simulate *fully nonlinear* perfect foresight models, with or without heterogeneous agents.
-The package implements the solution method proposed in `Robust Nonlinear Transition Dynamics in HANK <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023)*.
+The package implements the solution method proposed in `Robust Nonlinear Transition Dynamics in HANK <https://gregorboehl.com/live/hank_speed_boehl.pdf>`_ *(Gregor Boehl, 2023, SSRN No. 4433585)*.
 It allows to specify and solve nonlinear macroeconomic models quickly in a simple, high-level fashion.
 Generic and robust routines for steady state search are provided.
 
 The package can solve nonlinear models with heterogeneous agents, such as HANK models with one or two assets and portfolio choice. Steady state and nonlinear impulse responses (including, e.g., the ELB) can typically be found within a few seconds.
 The method extends the `Sequence-Space Jacobian <https://github.com/shade-econ/sequence-jacobian>`_ method (`Auclert et al., 2022, ECMA <https://doi.org/10.3982/ECTA17434>`_) to fully nonlinear heterogeneous agent models models by iteratively using `Jacobian-vector producs <https://jax.readthedocs.io/en/latest/notebooks/autodiff_cookbook.html#how-it-s-made-two-foundational-autodiff-functions>`_ to approximate the solution to the linear system of equations associated with each Newton iteration. This not only allows to study the dynamics of aggregate variables, but also the complete nonlinear transition dynamics of the cross-sectional distribution of assets and disaggregated objects.
 
 To solve models with representative agents a shooting methods similar to Laffargue (1990), Boucekkine (1995) and Juillard (1996) is implemented. It is faster and more reliable than the extended path method in dynare due to the use of automatic differentiation for the efficient jacobian decompositions during each Newton-step. Nonlinear perfect-foresight transition dynamics can - even for large-scale nonlinear models with several occassionally binding constraints - be computed in less than a second.
@@ -49,13 +49,13 @@
  * `User guide <https://econpizza.readthedocs.io/en/stable/index.html>`_
  * `Quickstart tutorial <https://econpizza.readthedocs.io/en/stable/tutorial/quickstart.html>`_
 
 Citation
 --------
 .. code-block:: bibtex
 
-    @Misc{boehl2022pizza,
-    title         = {Robust Nonlinear Transition Dynamics in HANK},
-    author        = {Boehl, Gregor},
-    howpublished  = {\url{https://gregorboehl.com/live/hank_speed_boehl.pdf}},
-    year = {2023}
+    @article{boehl2023goodpizza,
+        title       = {Robust Nonlinear Transition Dynamics in HANK},
+        author      = {Boehl, Gregor},
+        journal     = {Available at SSRN 4433585},
+        year        = {2023}
     }
```

### Comparing `econpizza-0.5.4/econpizza.egg-info/SOURCES.txt` & `econpizza-0.5.5/econpizza.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `econpizza-0.5.4/setup.py` & `econpizza-0.5.5/setup.py`

 * *Files identical despite different names*

