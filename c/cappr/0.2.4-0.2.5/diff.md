# Comparing `tmp/cappr-0.2.4.tar.gz` & `tmp/cappr-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cappr-0.2.4.tar", last modified: Fri Apr 28 23:56:05 2023, max compression
+gzip compressed data, was "cappr-0.2.5.tar", last modified: Fri May  5 10:33:42 2023, max compression
```

## Comparing `cappr-0.2.4.tar` & `cappr-0.2.5.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.020650 cappr-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.024650 cappr-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-28 23:55:54.000000 cappr-0.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-28 23:55:54.000000 cappr-0.2.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 23:55:54.000000 cappr-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-28 23:55:54.000000 cappr-0.2.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 23:55:54.000000 cappr-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-04-28 23:56:05.032650 cappr-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-04-28 23:55:54.000000 cappr-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.024650 cappr-0.2.4/demos/
--rw-r--r--   0 runner    (1001) docker     (123)  2760040 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/computational_analysis.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.028650 cappr-0.2.4/demos/raft/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/ade.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/b77.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/nis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/ose.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/over.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/sot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/sri.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15611 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/tai.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/tc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/teh.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/raft/tos.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.028650 cappr-0.2.4/demos/superglue/
--rw-r--r--   0 runner    (1001) docker     (123)    64027 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/superglue/copa.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    42865 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/superglue/wsc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-28 23:55:54.000000 cappr-0.2.4/demos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.028650 cappr-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.028650 cappr-0.2.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/1_is_for_me.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/2_motivation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/3_installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/4_user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/5_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/6_computational_performance.rst
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/7_future_research.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.028650 cappr-0.2.4/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/_static/github-mark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/docs/source/_static/scaling_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    53692 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/_static/scaling_classes/batch_size_32.png
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.huggingface.classify.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.huggingface.classify_no_cache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.huggingface.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.openai.api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.openai.classify.rst
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.openai.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.rst
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.utils.classify.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/cappr.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/related_work.rst
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/research.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-28 23:55:54.000000 cappr-0.2.4/docs/source/walkthrough.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-28 23:55:54.000000 cappr-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:56:05.032650 cappr-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-28 23:55:54.000000 cappr-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.020650 cappr-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/src/cappr/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/src/cappr/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/huggingface/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34123 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/huggingface/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    27937 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/huggingface/classify_no_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/src/cappr/openai/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25351 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/openai/classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/src/cappr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/utils/_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/utils/_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-04-28 23:55:54.000000 cappr-0.2.4/src/cappr/utils/classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/src/cappr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-04-28 23:56:04.000000 cappr-0.2.4/src/cappr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-28 23:56:05.000000 cappr-0.2.4/src/cappr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:56:04.000000 cappr-0.2.4/src/cappr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-28 23:56:04.000000 cappr-0.2.4/src/cappr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 23:56:04.000000 cappr-0.2.4/src/cappr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-28 23:55:54.000000 cappr-0.2.4/tests/_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/tests/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-04-28 23:55:54.000000 cappr-0.2.4/tests/huggingface/test_huggingface_classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-28 23:55:54.000000 cappr-0.2.4/tests/openai/test_openai_classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:56:05.032650 cappr-0.2.4/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-28 23:55:54.000000 cappr-0.2.4/tests/utils/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-28 23:55:54.000000 cappr-0.2.4/tests/utils/test_utils_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.997619 cappr-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.985619 cappr-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.985619 cappr-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-05 10:33:31.000000 cappr-0.2.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-05 10:33:31.000000 cappr-0.2.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 10:33:31.000000 cappr-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-05 10:33:31.000000 cappr-0.2.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 10:33:31.000000 cappr-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-05 10:33:41.997619 cappr-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-05-05 10:33:31.000000 cappr-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.989619 cappr-0.2.5/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)  2760040 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/computational_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/politeness.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.989619 cappr-0.2.5/demos/raft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/ade.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/b77.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/nis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/ose.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/over.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/sot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/sri.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15611 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/tai.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/tc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/teh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/tos.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.989619 cappr-0.2.5/demos/superglue/
+-rw-r--r--   0 runner    (1001) docker     (123)    64027 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/superglue/copa.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42865 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/superglue/wsc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.989619 cappr-0.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/1_is_for_me.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/2_motivation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/3_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/4_user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/5_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/6_computational_performance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/7_future_research.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/_static/github-mark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/docs/source/_static/scaling_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    53692 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/_static/scaling_classes/batch_size_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.huggingface.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.huggingface.classify_no_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.huggingface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.openai.api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.openai.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.openai.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.utils.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/related_work.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/research.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/walkthrough.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 10:33:31.000000 cappr-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:33:41.997619 cappr-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-05 10:33:31.000000 cappr-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.985619 cappr-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/src/cappr/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/src/cappr/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/huggingface/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34123 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/huggingface/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27982 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/huggingface/classify_no_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/src/cappr/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25351 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/openai/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.997619 cappr-0.2.5/src/cappr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/utils/_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/utils/_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/utils/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/src/cappr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-05 10:33:41.000000 cappr-0.2.5/src/cappr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-05 10:33:41.000000 cappr-0.2.5/src/cappr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:33:41.000000 cappr-0.2.5/src/cappr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-05 10:33:41.000000 cappr-0.2.5/src/cappr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 10:33:41.000000 cappr-0.2.5/src/cappr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.997619 cappr-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-05 10:33:31.000000 cappr-0.2.5/tests/_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.997619 cappr-0.2.5/tests/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-05-05 10:33:31.000000 cappr-0.2.5/tests/huggingface/test_huggingface_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.997619 cappr-0.2.5/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-05 10:33:31.000000 cappr-0.2.5/tests/openai/test_openai_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.997619 cappr-0.2.5/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-05 10:33:31.000000 cappr-0.2.5/tests/utils/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-05 10:33:31.000000 cappr-0.2.5/tests/utils/test_utils_classify.py
```

### Comparing `cappr-0.2.4/.github/workflows/python-publish.yml` & `cappr-0.2.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/.github/workflows/test.yml` & `cappr-0.2.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/LICENSE` & `cappr-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/PKG-INFO` & `cappr-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cappr
-Version: 0.2.4
+Version: 0.2.5
 Summary: Zero-shot text classification using autoregressive language models.
 Home-page: https://github.com/kddubey/cappr/
 Author-email: kushdubey63@gmail.com
 License: Apache License 2.0
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: hf
```

### Comparing `cappr-0.2.4/README.md` & `cappr-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/computational_analysis.ipynb` & `cappr-0.2.5/demos/computational_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/raft/README.md` & `cappr-0.2.5/demos/raft/README.md`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/raft/ade.ipynb` & `cappr-0.2.5/demos/raft/ade.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/raft/b77.ipynb` & `cappr-0.2.5/demos/raft/b77.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/raft/nis.ipynb` & `cappr-0.2.5/demos/raft/nis.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/raft/ose.ipynb` & `cappr-0.2.5/demos/raft/ose.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/raft/over.ipynb` & `cappr-0.2.5/demos/raft/over.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/raft/sot.ipynb` & `cappr-0.2.5/demos/raft/sot.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/raft/sri.ipynb` & `cappr-0.2.5/demos/raft/sri.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/raft/tai.ipynb` & `cappr-0.2.5/demos/raft/tai.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/raft/tc.ipynb` & `cappr-0.2.5/demos/raft/tc.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/raft/teh.ipynb` & `cappr-0.2.5/demos/raft/teh.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/raft/tos.ipynb` & `cappr-0.2.5/demos/raft/tos.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/superglue/copa.ipynb` & `cappr-0.2.5/demos/superglue/copa.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/superglue/wsc.ipynb` & `cappr-0.2.5/demos/superglue/wsc.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/demos/utils.py` & `cappr-0.2.5/demos/utils.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/docs/Makefile` & `cappr-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/docs/make.bat` & `cappr-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/docs/source/1_is_for_me.rst` & `cappr-0.2.5/docs/source/1_is_for_me.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/docs/source/2_motivation.rst` & `cappr-0.2.5/docs/source/2_motivation.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/docs/source/3_installation.rst` & `cappr-0.2.5/docs/source/3_installation.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/docs/source/4_user_guide.rst` & `cappr-0.2.5/docs/source/4_user_guide.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/docs/source/6_computational_performance.rst` & `cappr-0.2.5/docs/source/6_computational_performance.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/docs/source/7_future_research.rst` & `cappr-0.2.5/docs/source/7_future_research.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/docs/source/_static/github-mark.png` & `cappr-0.2.5/docs/source/_static/github-mark.png`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/docs/source/_static/scaling_classes/batch_size_32.png` & `cappr-0.2.5/docs/source/_static/scaling_classes/batch_size_32.png`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/docs/source/conf.py` & `cappr-0.2.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/docs/source/index.rst` & `cappr-0.2.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/docs/source/related_work.rst` & `cappr-0.2.5/docs/source/related_work.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/setup.py` & `cappr-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/src/cappr/_example.py` & `cappr-0.2.5/src/cappr/_example.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/src/cappr/huggingface/_utils.py` & `cappr-0.2.5/src/cappr/huggingface/_utils.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/src/cappr/huggingface/classify.py` & `cappr-0.2.5/src/cappr/huggingface/classify.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/src/cappr/huggingface/classify_no_cache.py` & `cappr-0.2.5/src/cappr/huggingface/classify_no_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,14 +412,15 @@
 
 @classify._predict_proba
 def predict_proba(
     prompts: Sequence[str],
     completions: Sequence[str],
     model: str = None,
     model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    prior: Optional[Sequence[float]] = None,
     end_of_prompt: str = " ",
     batch_size: int = 32,
 ) -> npt.NDArray[np.floating]:
     """
     Predict probabilities of each completion coming after each prompt.
 
     Note
```

### Comparing `cappr-0.2.4/src/cappr/openai/api.py` & `cappr-0.2.5/src/cappr/openai/api.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/src/cappr/openai/classify.py` & `cappr-0.2.5/src/cappr/openai/classify.py`

 * *Files 0% similar despite different names*

```diff
@@ -470,15 +470,15 @@
         # alternative implied by the 1st premise: 'The man broke his toe'
         pred_probs[0,1]
         # 0.53
 
         # predicted probability that 'the liquid in the bottle poured out' is the
         # alternative implied by the 2nd premise: 'I tipped the bottle'
         pred_probs[1,1]
-        # 0.66
+        # 0.75
     """
     return log_probs_conditional_examples(examples, model, ask_if_ok=ask_if_ok)
 
 
 @classify._predict
 def predict(
     prompts: Sequence[str],
```

### Comparing `cappr-0.2.4/src/cappr/utils/_batch.py` & `cappr-0.2.5/src/cappr/utils/_batch.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/src/cappr/utils/_check.py` & `cappr-0.2.5/src/cappr/utils/_check.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/src/cappr/utils/classify.py` & `cappr-0.2.5/src/cappr/utils/classify.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     num_completions_per_prompt = [
         len(log_probs_completions) for log_probs_completions in log_probs
     ]
     num_completions_per_prompt_set = set(num_completions_per_prompt)
     if not len(num_completions_per_prompt_set) == 1:
         raise ValueError(
             "log_probs does not have a constant number of completions, i.e., there are "
-            "indices i, j such that len(log_probs[i]) != len(log_probs[j]). Please use "
-            "the slower function, agg_log_probs, instead."
+            "indices i, j such that len(log_probs[i]) != len(log_probs[j])."
         )
     ## Say, e.g., we have 2 completions, ['a b', 'c d e'], and 2 prompts.
     ## Then log_probs looks like:
     ## [ [ [a1, b1],      (token log-probs for completion 1 | prompt 1)
     #      [c1, d1, e1]], (token log-probs for completion 2 | prompt 1)
     ##   [ [a2, b2],      (token log-probs for completion 1 | prompt 2)
     ##     [c2, d2, e2]]  (token log-probs for completion 2 | prompt 2)
@@ -172,53 +171,60 @@
     else:
         posteriors_unnorm = likelihoods * prior
     marginals = posteriors_unnorm.sum(axis=axis, keepdims=True)
     marginals[~normalize] = 1  ## denominator of 1 <=> no normalization
     return posteriors_unnorm / marginals
 
 
-def _predict_proba(conditional_func):
+def _predict_proba(log_probs_conditional):
     """
-    TODO: docstring
+    Decorator which converts a `log_probs_condtional` function call into a
+    `predict_proba` call. The decorated `predict_proba` function should take a `prior`
+    keyword argument.
     """
 
-    @wraps(conditional_func)
+    @wraps(log_probs_conditional)
     def wrapper(
         prompts: Sequence[str], completions: Sequence[str], *args, **kwargs
     ) -> npt.NDArray[np.floating]:
         ## Before hitting any APIs ($$), let's check the prior
         prior = kwargs.get("prior", None)
         _check.prior(prior)
         if prior is not None and len(completions) != len(prior):
             raise ValueError(
                 "completions and prior are different lengths: "
                 f"{len(completions)}, {len(prior)}."
             )
 
-        log_probs_completions = conditional_func(prompts, completions, *args, **kwargs)
+        log_probs_completions = log_probs_conditional(
+            prompts, completions, *args, **kwargs
+        )
         likelihoods = agg_log_probs(log_probs_completions)
         ## If there's only 1 completion, normalizing will cause the probability to
         ## trivially be 1! So let's not normalize in that case, and hope the user knows
         ## what they're doing
         normalize = len(completions) > 1
         return posterior_prob(likelihoods, axis=1, prior=prior, normalize=normalize)
 
     return wrapper
 
 
-def _predict_proba_examples(conditional_examples_func):
+def _predict_proba_examples(log_probs_conditional_examples):
     """
-    TODO: docstring
+    Decorator which converts a `log_probs_conditional_examples` function call into a
+    `predict_proba_examples` call.
     """
 
-    @wraps(conditional_examples_func)
+    @wraps(log_probs_conditional_examples)
     def wrapper(
         examples, *args, **kwargs
     ) -> Union[list[list[float]], npt.NDArray[np.floating]]:
-        log_probs_completions = conditional_examples_func(examples, *args, **kwargs)
+        log_probs_completions = log_probs_conditional_examples(
+            examples, *args, **kwargs
+        )
         likelihoods = agg_log_probs(log_probs_completions)
         ## If an example has just 1 completion, normalizing will cause the probability
         ## to trivially be 1! So let's not normalize in that case, and hope the user
         ## knows what they're doing
         num_completions_per_prompt = [len(example.completions) for example in examples]
         normalize = [num > 1 for num in num_completions_per_prompt]
         num_completions_per_prompt_set = set(num_completions_per_prompt)
@@ -259,15 +265,15 @@
         )
 
     return wrapper
 
 
 def _predict(predict_proba_func):
     """
-    TODO: docstring
+    Decorator which converts a `predict_proba` function call into a `predict` call.
     """
 
     @wraps(predict_proba_func)
     def wrapper(
         prompts: Sequence[str], completions: Sequence[str], *args, **kwargs
     ) -> list[str]:
         pred_probs: npt.NDArray = predict_proba_func(
@@ -277,15 +283,16 @@
         return [completions[pred_class_idx] for pred_class_idx in pred_class_idxs]
 
     return wrapper
 
 
 def _predict_examples(predict_proba_examples_func):
     """
-    TODO: docstring
+    Decorator which converts a `predict_proba_examples` function call into a
+    `predict_examples` call.
     """
 
     @wraps(predict_proba_examples_func)
     def wrapper(examples, *args, **kwargs) -> list[str]:
         pred_probs: Union[
             list[list[float]], npt.NDArray[np.floating]
         ] = predict_proba_examples_func(examples, *args, **kwargs)
```

### Comparing `cappr-0.2.4/src/cappr.egg-info/PKG-INFO` & `cappr-0.2.5/src/cappr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cappr
-Version: 0.2.4
+Version: 0.2.5
 Summary: Zero-shot text classification using autoregressive language models.
 Home-page: https://github.com/kddubey/cappr/
 Author-email: kushdubey63@gmail.com
 License: Apache License 2.0
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: hf
```

### Comparing `cappr-0.2.4/src/cappr.egg-info/SOURCES.txt` & `cappr-0.2.5/src/cappr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 .github/workflows/python-publish.yml
 .github/workflows/test.yml
 demos/computational_analysis.ipynb
+demos/politeness.ipynb
 demos/utils.py
 demos/raft/README.md
 demos/raft/ade.ipynb
 demos/raft/b77.ipynb
 demos/raft/nis.ipynb
 demos/raft/ose.ipynb
 demos/raft/over.ipynb
```

### Comparing `cappr-0.2.4/tests/_test.py` & `cappr-0.2.5/tests/_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Helper functions to test that predict_proba and predict function outputs have the
-correct form, but not necessarily the correct content.
+Helper functions to test that `predict_proba` and `predict` function outputs have the
+correct form.
 """
 from __future__ import annotations
 from typing import Any, Callable, Sequence, Union
 
 import numpy as np
 import numpy.typing as npt
 
@@ -23,15 +23,20 @@
     """
     Tests that `predict_proba_func(prompts, completions, *args, **kwargs)` returns a
     numpy array with the correct shape, and that each row is a probability distribution.
     """
     pred_probs = predict_proba_func(prompts, completions, *args, **kwargs)
     assert isinstance(pred_probs, np.ndarray)
     assert pred_probs.shape == (len(prompts), len(completions))
-    if pred_probs.shape[1] > 1:  ## we don't normalize if there's one completion
+    assert np.all(pred_probs >= 0)
+    if pred_probs.shape[1] == 1:
+        ## We don't normalize if there's one completion. It's almost definitely the case
+        ## that the predicted probability is < 1 by a decent amount.
+        assert not any(np.isclose(pred_probs[:, 0], 1))
+    else:
         assert np.allclose(pred_probs.sum(axis=1), 1)
 
 
 def predict_proba_examples(
     predict_proba_examples_func: Callable[
         [Sequence[Example], Any], Union[list[list[float]], npt.NDArray[np.floating]]
     ],
@@ -43,15 +48,20 @@
     Tests that `predict_proba_examples_func(examples, *args, **kwargs)` returns a
     list with the correct shape, and that each element is a probability distribution.
     """
     pred_probs = predict_proba_examples_func(examples, *args, **kwargs)
     assert len(pred_probs) == len(examples)
     for pred_prob_example, example in zip(pred_probs, examples):
         assert len(pred_prob_example) == len(example.completions)
-        if len(pred_prob_example) > 1:  ## we don't normalize if there's one completion
+        assert np.all(np.array(pred_prob_example) >= 0)
+        if len(pred_prob_example) == 1:
+            ## We don't normalize if there's one completion. It's almost definitely the
+            ## case that the predicted probability is < 1 by a decent amount.
+            assert not any(np.isclose(pred_prob_example, 1))
+        else:
             assert np.isclose(sum(pred_prob_example), 1)
 
 
 def predict(
     predict_func: Callable[[Sequence[str], Sequence[str], Any], list[str]],
     prompts: Sequence[str],
     completions: Sequence[str],
```

### Comparing `cappr-0.2.4/tests/huggingface/test_huggingface_classify.py` & `cappr-0.2.5/tests/huggingface/test_huggingface_classify.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-Unit tests `cappr.huggingface.classify` by comparing its functions' outputs to those
-from `cappr.huggingface.classify_no_cache`, which is assumed to be correct (TODO: yeah I
-really should test that).
+Unit tests `cappr.huggingface.classify` by checking that its functions' outputs are
+numerically close to those from `cappr.huggingface.classify_no_cache`, which is assumed
+to be correct (TODO: yeah I really should test that).
 """
 from __future__ import annotations
 import os
 import sys
 from typing import Mapping
 
 import pytest
@@ -57,14 +57,18 @@
 
 
 @pytest.mark.parametrize("prompts", (["a b c", "c"],))
 @pytest.mark.parametrize("num_completions_per_prompt", (2, (2, 3)))
 def test__keys_values_prompts(
     model, tokenizer, prompts, num_completions_per_prompt, atol
 ):
+    """
+    Tests that the model's attention keys and values for the prompt are identical. If
+    this test fails, all tests which call `_test_logits` will also fail.
+    """
     _outputs_slow = slow._keys_values_prompts(
         model, tokenizer, prompts, num_completions_per_prompt
     )
     _outputs_fast = fast._keys_values_prompts(
         model, tokenizer, prompts, num_completions_per_prompt
     )
     keys_vals_slow, encodings_slow, offsets_slow, logits_last_slow = _outputs_slow
@@ -86,18 +90,22 @@
 
 def _test_encodings(
     logits_slow: torch.Tensor,
     encodings_slow: Mapping[str, torch.Tensor],
     logits_fast: torch.Tensor,
     encodings_fast: Mapping[str, torch.Tensor],
 ):
-    ## Test shapes
+    """
+    Tests that all objects have the expected shape, and that the encodings `offsets` are
+    identical.
+    """
+
     def _test_shapes(logits, encodings):
-        assert encodings["input_ids"].shape[:2] == logits.shape[:2]
-        assert encodings["input_ids"].shape[:2] == encodings["attention_mask"].shape[:2]
+        assert encodings["input_ids"].shape == logits.shape[:2]  ## 3rd dim is vocab
+        assert encodings["input_ids"].shape == encodings["attention_mask"].shape
         assert encodings["input_ids"].shape[0] == encodings["offsets"].shape[0]
 
     _test_shapes(logits_slow, encodings_slow)
     _test_shapes(logits_fast, encodings_fast)
 
     ## Test offsets. These should be exactly the same b/c they're the number of
     ## of non-pad tokens in each prompt
@@ -107,22 +115,25 @@
 def _test_logits(
     logits_slow: torch.Tensor,
     encodings_slow: Mapping[str, torch.Tensor],
     logits_fast: torch.Tensor,
     encodings_fast: Mapping[str, torch.Tensor],
     atol,
 ):
+    """
+    Tests that logits have identical shape, and that their non-pad token logits are
+    numerically close.
+    """
     ## Test shapes
     assert logits_slow.shape[0] == logits_fast.shape[0]  ## batch size
-    ## Middle dimension for the # of tokens is different (by design) b/c
-    ## logits_slow includes prompt and completion tokens, while logits_fast only
-    ## includes completion tokens.
+    ## Middle dimension (for the # of tokens) is different b/c logits_slow includes
+    ## prompt and completion tokens, while logits_fast only includes completion tokens.
     assert logits_slow.shape[2] == logits_fast.shape[2]  ## vocab size
 
-    ## Test logits at every *non-pad* token (automatic version)
+    ## Test logits at every *non-pad* token
     completion_token_idxs = [
         list(range(num_completion_tokens))
         for num_completion_tokens in encodings_fast["attention_mask"].sum(dim=1)
     ]
     for text_idx in range(logits_slow.shape[0]):
         offset = encodings_fast["offsets"][text_idx].item() - 1
         ## number of non-pad prompt tokens - 1 (!) b/c in the fast version we
@@ -132,53 +143,70 @@
                 logits_fast[text_idx, completion_token_idx],
                 logits_slow[text_idx, offset + completion_token_idx],
                 atol=atol,
             )
 
 
 def _test_log_probs(
-    log_probs_completions_slow,
-    log_probs_completions_fast,
-    expected_len,
-    num_completions_per_prompt,
+    log_probs_completions_slow: list[list[list[float]]],
+    log_probs_completions_fast: list[list[list[float]]],
+    expected_len: int,
+    num_completions_per_prompt: list[int],
     atol,
 ):
+    """
+    Tests that the conditional token log-probabilities are the right shape and are
+    numerically close.
+    """
+    ## Test lengths before zipping. Note transitivity
     assert len(log_probs_completions_slow) == len(log_probs_completions_fast)
     assert len(log_probs_completions_fast) == expected_len
+    assert len(log_probs_completions_slow) == len(num_completions_per_prompt)
     zipped_outer = zip(
         log_probs_completions_slow,
         log_probs_completions_fast,
         num_completions_per_prompt,
     )
     for log_probs_slow, log_probs_fast, num_completions in zipped_outer:
         assert len(log_probs_fast) == num_completions
-        assert len(log_probs_slow) == len(log_probs_fast)
+        assert len(log_probs_slow) == num_completions
         zipped_inner = zip(log_probs_slow, log_probs_fast)
         for log_probs_tokens_slow, log_probs_tokens_fast in zipped_inner:
+            ## cast to tensor so that we are consistent w/ the way "numerical closeness"
+            ## is defined for model-dependent outputs
             assert torch.allclose(
                 torch.tensor(log_probs_tokens_slow),
                 torch.tensor(log_probs_tokens_fast),
                 atol=atol,
             )
 
 
 @pytest.mark.parametrize("prompts", (["a b c", "c"],))
 @pytest.mark.parametrize(
     "completions",
     (
         ["d", "e f g h i"],
-        ####### Next set of completions #######
+        ####### Next set of completions to test #######
         ["d", "d e f"],
     ),
 )
 @pytest.mark.parametrize("end_of_prompt", (" ",))  ## TODO: expand
 class TestPromptsCompletions:
+    """
+    Tests all model-dependent, non-`_examples` functions, sharing the same set of
+    prompts and completions.
+    """
+
     def test__logits_completions_given_prompts(
         self, model, tokenizer, prompts, completions, end_of_prompt, atol
     ):
+        """
+        Tests that encodings have the right shape and that logits are numerically close.
+        If this test fails, all of the tests below will fail.
+        """
         slow_out = slow._logits_completions_given_prompts(
             model, tokenizer, prompts, completions, end_of_prompt=end_of_prompt
         )
         fast_out = fast._logits_completions_given_prompts(
             model, tokenizer, prompts, completions, end_of_prompt=end_of_prompt
         )
         _test_encodings(*slow_out, *fast_out)
@@ -209,32 +237,76 @@
             log_probs_completions_fast,
             expected_len,
             num_completions_per_prompt,
             atol,
         )
 
     def test_predict_proba(
-        self, prompts, completions, model_and_tokenizer, end_of_prompt
+        self, prompts, completions, model_and_tokenizer, end_of_prompt, atol
     ):
         _test.predict_proba(
             fast.predict_proba,
             prompts,
             completions,
             model_and_tokenizer=model_and_tokenizer,
             end_of_prompt=end_of_prompt,
         )
+        _test.predict_proba(
+            slow.predict_proba,
+            prompts,
+            completions,
+            model_and_tokenizer=model_and_tokenizer,
+            end_of_prompt=end_of_prompt,
+        )
+        pred_probs_fast = fast.predict_proba(
+            prompts,
+            completions,
+            model_and_tokenizer=model_and_tokenizer,
+            end_of_prompt=end_of_prompt,
+        )
+        pred_probs_slow = slow.predict_proba(
+            prompts,
+            completions,
+            model_and_tokenizer=model_and_tokenizer,
+            end_of_prompt=end_of_prompt,
+        )
+        ## cast to tensor so that we are consistent w/ the way "numerical closeness"
+        ## is defined for model-dependent outputs
+        assert torch.allclose(
+            torch.tensor(pred_probs_fast), torch.tensor(pred_probs_slow), atol=atol
+        )
 
     def test_predict(self, prompts, completions, model_and_tokenizer, end_of_prompt):
         _test.predict(
             fast.predict,
             prompts,
             completions,
             model_and_tokenizer=model_and_tokenizer,
             end_of_prompt=end_of_prompt,
         )
+        _test.predict(
+            slow.predict,
+            prompts,
+            completions,
+            model_and_tokenizer=model_and_tokenizer,
+            end_of_prompt=end_of_prompt,
+        )
+        preds_fast = fast.predict(
+            prompts,
+            completions,
+            model_and_tokenizer=model_and_tokenizer,
+            end_of_prompt=end_of_prompt,
+        )
+        preds_slow = slow.predict(
+            prompts,
+            completions,
+            model_and_tokenizer=model_and_tokenizer,
+            end_of_prompt=end_of_prompt,
+        )
+        assert preds_fast == preds_slow
 
 
 @pytest.mark.parametrize(
     "examples",
     (
         [
             Ex("a b c", ["d", "e f g"]),
@@ -245,17 +317,25 @@
             Ex("chi", ["can", "ery"]),
             Ex("koyaa", ["nisqatsi"]),
             Ex("hi hi", ["bye bye", "yo yo"]),
         ],
     ),
 )
 class TestExamples:
+    """
+    Tests all model-dependent, `_examples` functions, sharing the same set of examples.
+    """
+
     def test__logits_completions_given_prompts_examples(
         self, model, tokenizer, examples, atol
     ):
+        """
+        Tests that encodings have the right shape and that logits are numerically close.
+        If this test fails, all of the tests below will fail.
+        """
         slow_out = slow._logits_completions_given_prompts_examples(
             model, tokenizer, examples
         )
         fast_out = fast._logits_completions_given_prompts_examples(
             model, tokenizer, examples
         )
         _test_encodings(*slow_out, *fast_out)
@@ -277,18 +357,49 @@
             log_probs_completions_slow,
             log_probs_completions_fast,
             expected_len,
             num_completions_per_prompt,
             atol,
         )
 
-    def test_predict_proba_examples(self, examples, model_and_tokenizer):
+    def test_predict_proba_examples(self, examples, model_and_tokenizer, atol):
         _test.predict_proba_examples(
             fast.predict_proba_examples,
             examples,
             model_and_tokenizer=model_and_tokenizer,
         )
+        _test.predict_proba_examples(
+            slow.predict_proba_examples,
+            examples,
+            model_and_tokenizer=model_and_tokenizer,
+        )
+        pred_probs_fast = fast.predict_proba_examples(
+            examples, model_and_tokenizer=model_and_tokenizer
+        )
+        pred_probs_slow = slow.predict_proba_examples(
+            examples, model_and_tokenizer=model_and_tokenizer
+        )
+        for pred_probs_fast_ex, pred_probs_slow_ex in zip(
+            pred_probs_fast, pred_probs_slow
+        ):
+            ## cast to tensor so that we are consistent w/ the way "numerical closeness"
+            ## is defined for model-dependent outputs
+            assert torch.allclose(
+                torch.tensor(pred_probs_fast_ex),
+                torch.tensor(pred_probs_slow_ex),
+                atol=atol,
+            )
 
     def test_predict_examples(self, examples, model_and_tokenizer):
         _test.predict_examples(
             fast.predict_examples, examples, model_and_tokenizer=model_and_tokenizer
         )
+        _test.predict_examples(
+            slow.predict_examples, examples, model_and_tokenizer=model_and_tokenizer
+        )
+        preds_fast = fast.predict_examples(
+            examples, model_and_tokenizer=model_and_tokenizer
+        )
+        preds_slow = slow.predict_examples(
+            examples, model_and_tokenizer=model_and_tokenizer
+        )
+        assert preds_fast == preds_slow
```

### Comparing `cappr-0.2.4/tests/openai/test_openai_classify.py` & `cappr-0.2.5/tests/openai/test_openai_classify.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 @pytest.fixture(autouse=True)
 def patch_openai_method_retry(monkeypatch):
     ## During testing, there's never going to be a case where we want to actually hit
     ## an OpenAI endpoint!
     def _log_probs(texts: list[str]) -> list[list[float]]:
         """
-        Returns a list `log_probs` where `log_probs[i]` is `list(range(size))` where `size`
-        is the number of tokens in `texts[i]`.
+        Returns a list `log_probs` where `log_probs[i]` is `list(range(size))` where
+        `size` is the number of tokens in `texts[i]`.
         """
         tokenizer = tiktoken.get_encoding("gpt2")
         return [list(range(len(tokens))) for tokens in tokenizer.encode_batch(texts)]
 
     ## Note that the the text completion endpoint uses a kwarg named prompt, but that's
     ## actually set to prompt + completion in the CAPPr scheme. We input that to get
     ## log-probs of completion tokens given prompt
```

### Comparing `cappr-0.2.4/tests/utils/test_batch.py` & `cappr-0.2.5/tests/utils/test_batch.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.4/tests/utils/test_utils_classify.py` & `cappr-0.2.5/tests/utils/test_utils_classify.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,18 +28,19 @@
     assert np.allclose(log_probs_agg, np.exp([[4, 1], [1, 4]]))
 
 
 @pytest.mark.parametrize("likelihoods", ([[4, 1], [1, 4]],))
 @pytest.mark.parametrize("prior", (None, [1 / 2, 1 / 2], [1 / 3, 2 / 3]))
 @pytest.mark.parametrize("normalize", (True, False))
 def test_posterior_prob_2d(likelihoods, prior, normalize):
+    ## TODO: clean this up
     posteriors = classify.posterior_prob(
         likelihoods, axis=1, prior=prior, normalize=normalize
     )
-    if prior == [1 / 2, 1 / 2]:  ## hard-coded b/c idk how to engineer tests
+    if prior == [1 / 2, 1 / 2]:
         if normalize:
             assert np.all(np.isclose(posteriors, [[4 / 5, 1 / 5], [1 / 5, 4 / 5]]))
         else:
             assert np.all(posteriors == np.array(likelihoods) / 2)
     elif prior is None:
         if normalize:
             assert np.all(np.isclose(posteriors, [[4 / 5, 1 / 5], [1 / 5, 4 / 5]]))
```

