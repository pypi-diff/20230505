# Comparing `tmp/action-react-0.0.2.tar.gz` & `tmp/action-react-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/action-react-0.0.2.tar", last modified: Sun Mar 26 23:54:34 2023, max compression
+gzip compressed data, was "dist/action-react-0.0.3.tar", last modified: Fri May  5 00:55:50 2023, max compression
```

## Comparing `action-react-0.0.2.tar` & `action-react-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,37 @@
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-03-26 23:54:34.000000 action-react-0.0.2/
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-03-26 23:54:34.000000 action-react-0.0.2/.github/
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-03-26 23:54:34.000000 action-react-0.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 wyu        (501) staff       (20)      834 2023-03-26 23:10:55.000000 action-react-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 wyu        (501) staff       (20)      595 2023-03-26 23:10:55.000000 action-react-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 wyu        (501) staff       (20)      118 2023-03-26 23:10:55.000000 action-react-0.0.2/.github/dependabot.yml
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-03-26 23:54:34.000000 action-react-0.0.2/.github/workflows/
--rw-r--r--   0 wyu        (501) staff       (20)     1097 2023-03-26 23:10:55.000000 action-react-0.0.2/.github/workflows/build.yml
--rw-r--r--   0 wyu        (501) staff       (20)     1818 2023-03-26 23:43:05.000000 action-react-0.0.2/.gitignore
--rw-r--r--   0 wyu        (501) staff       (20)     1022 2023-03-26 23:30:54.000000 action-react-0.0.2/CONTRIBUTING.md
--rw-r--r--   0 wyu        (501) staff       (20)    11357 2023-03-26 23:10:55.000000 action-react-0.0.2/LICENSE
--rw-r--r--   0 wyu        (501) staff       (20)     2280 2023-03-26 23:10:55.000000 action-react-0.0.2/Makefile
--rw-r--r--   0 wyu        (501) staff       (20)    14929 2023-03-26 23:54:34.000000 action-react-0.0.2/PKG-INFO
--rw-r--r--   0 wyu        (501) staff       (20)     1162 2023-03-26 23:43:18.000000 action-react-0.0.2/README.md
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-03-26 23:54:34.000000 action-react-0.0.2/action_react/
--rw-r--r--   0 wyu        (501) staff       (20)     2514 2023-03-26 23:41:18.000000 action-react-0.0.2/action_react/main.py
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-03-26 23:54:34.000000 action-react-0.0.2/action_react/tests/
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-03-26 23:54:34.000000 action-react-0.0.2/action_react/tests/fixtures/
--rw-r--r--   0 wyu        (501) staff       (20)      159 2023-03-26 23:10:55.000000 action-react-0.0.2/action_react/tests/fixtures/config.ini
--rw-r--r--   0 wyu        (501) staff       (20)     2054 2023-03-26 23:10:55.000000 action-react-0.0.2/action_react/tests/test_all.py
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-03-26 23:54:34.000000 action-react-0.0.2/action_react.egg-info/
--rw-r--r--   0 wyu        (501) staff       (20)    14929 2023-03-26 23:54:34.000000 action-react-0.0.2/action_react.egg-info/PKG-INFO
--rw-r--r--   0 wyu        (501) staff       (20)      488 2023-03-26 23:54:34.000000 action-react-0.0.2/action_react.egg-info/SOURCES.txt
--rw-r--r--   0 wyu        (501) staff       (20)        1 2023-03-26 23:54:34.000000 action-react-0.0.2/action_react.egg-info/dependency_links.txt
--rw-r--r--   0 wyu        (501) staff       (20)      173 2023-03-26 23:54:34.000000 action-react-0.0.2/action_react.egg-info/requires.txt
--rw-r--r--   0 wyu        (501) staff       (20)       13 2023-03-26 23:54:34.000000 action-react-0.0.2/action_react.egg-info/top_level.txt
--rw-r--r--   0 wyu        (501) staff       (20)      198 2023-03-26 23:10:55.000000 action-react-0.0.2/config.ini
--rw-r--r--   0 wyu        (501) staff       (20)     2174 2023-03-26 23:42:47.000000 action-react-0.0.2/pyproject.toml
--rw-r--r--   0 wyu        (501) staff       (20)       38 2023-03-26 23:54:34.000000 action-react-0.0.2/setup.cfg
--rw-r--r--   0 wyu        (501) staff       (20)       39 2023-03-26 23:10:55.000000 action-react-0.0.2/setup.py
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/.github/
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 wyu        (501) staff       (20)      834 2023-03-26 23:10:55.000000 action-react-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 wyu        (501) staff       (20)      595 2023-03-26 23:10:55.000000 action-react-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 wyu        (501) staff       (20)      118 2023-03-26 23:10:55.000000 action-react-0.0.3/.github/dependabot.yml
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/.github/workflows/
+-rw-r--r--   0 wyu        (501) staff       (20)     1097 2023-03-26 23:10:55.000000 action-react-0.0.3/.github/workflows/build.yml
+-rw-r--r--   0 wyu        (501) staff       (20)     1848 2023-04-05 01:58:18.000000 action-react-0.0.3/.gitignore
+-rw-r--r--   0 wyu        (501) staff       (20)     1022 2023-03-26 23:30:54.000000 action-react-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0 wyu        (501) staff       (20)    11357 2023-03-26 23:10:55.000000 action-react-0.0.3/LICENSE
+-rw-r--r--   0 wyu        (501) staff       (20)     2622 2023-04-05 14:52:29.000000 action-react-0.0.3/Makefile
+-rw-r--r--   0 wyu        (501) staff       (20)    15688 2023-05-05 00:55:50.000000 action-react-0.0.3/PKG-INFO
+-rw-r--r--   0 wyu        (501) staff       (20)     1921 2023-04-05 14:52:29.000000 action-react-0.0.3/README.md
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react/
+-rw-r--r--   0 wyu        (501) staff       (20)     4217 2023-05-05 00:08:49.000000 action-react-0.0.3/action_react/main.py
+-rw-r--r--   0 wyu        (501) staff       (20)     2426 2023-05-05 00:47:23.000000 action-react-0.0.3/action_react/react.py
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react/tests/
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react/tests/fixtures/
+-rw-r--r--   0 wyu        (501) staff       (20)      159 2023-03-26 23:10:55.000000 action-react-0.0.3/action_react/tests/fixtures/config.ini
+-rw-r--r--   0 wyu        (501) staff       (20)     2054 2023-03-26 23:10:55.000000 action-react-0.0.3/action_react/tests/test_all.py
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react.egg-info/
+-rw-r--r--   0 wyu        (501) staff       (20)    15688 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react.egg-info/PKG-INFO
+-rw-r--r--   0 wyu        (501) staff       (20)      582 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react.egg-info/SOURCES.txt
+-rw-r--r--   0 wyu        (501) staff       (20)        1 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react.egg-info/dependency_links.txt
+-rw-r--r--   0 wyu        (501) staff       (20)      204 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react.egg-info/requires.txt
+-rw-r--r--   0 wyu        (501) staff       (20)       13 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react.egg-info/top_level.txt
+-rw-r--r--   0 wyu        (501) staff       (20)      198 2023-03-26 23:10:55.000000 action-react-0.0.3/config.ini
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/docs/
+-rw-r--r--   0 wyu        (501) staff       (20)      634 2023-04-05 01:53:42.000000 action-react-0.0.3/docs/Makefile
+-rw-r--r--   0 wyu        (501) staff       (20)     2252 2023-04-05 15:48:54.000000 action-react-0.0.3/docs/conf.py
+-rw-r--r--   0 wyu        (501) staff       (20)     2201 2023-04-05 14:52:29.000000 action-react-0.0.3/docs/index.md
+-rw-r--r--   0 wyu        (501) staff       (20)      800 2023-04-05 01:53:42.000000 action-react-0.0.3/docs/make.bat
+-rw-r--r--   0 wyu        (501) staff       (20)     2235 2023-05-05 00:11:22.000000 action-react-0.0.3/pyproject.toml
+-rw-r--r--   0 wyu        (501) staff       (20)       48 2023-05-04 23:55:50.000000 action-react-0.0.3/requirements.txt
+-rw-r--r--   0 wyu        (501) staff       (20)       38 2023-05-05 00:55:50.000000 action-react-0.0.3/setup.cfg
+-rw-r--r--   0 wyu        (501) staff       (20)       39 2023-03-26 23:10:55.000000 action-react-0.0.3/setup.py
```

### Comparing `action-react-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md` & `action-react-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `action-react-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md` & `action-react-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `action-react-0.0.2/.github/workflows/build.yml` & `action-react-0.0.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `action-react-0.0.2/.gitignore` & `action-react-0.0.3/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
+docs/_static/
+docs/_templates
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `action-react-0.0.2/CONTRIBUTING.md` & `action-react-0.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `action-react-0.0.2/LICENSE` & `action-react-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `action-react-0.0.2/Makefile` & `action-react-0.0.3/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+TMPREPO=/tmp/docs/action-react
+
 #########
 # BUILD #
 #########
 develop:  ## install dependencies and build library
 	python -m pip install -e .[develop]
 
 build:  ## build the python library
@@ -91,8 +93,22 @@
 .DEFAULT_GOAL := help
 help:
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
 print-%:
 	@echo '$*=$($*)'
 
-.PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help
+docs:
+	$(MAKE) -C docs/ clean
+	$(MAKE) -C docs/ html
+
+pages:
+	rm -rf $(TMPREPO)
+	git clone -b gh-pages https://github.com/yd-wu/action-react.git $(TMPREPO)
+	rm -rf $(TMPREPO)/*
+	cp -r docs/_build/html/* $(TMPREPO)
+	cd $(TMPREPO);\
+	git add -A ;\
+	git commit -a -m 'auto-updating docs' ;\
+	git push
+
+.PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help docs pages
```

### Comparing `action-react-0.0.2/PKG-INFO` & `action-react-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action-react
-Version: 0.0.2
+Version: 0.0.3
 Summary: telegram listener tool
 Author-email: yd-wu <yw3960@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -225,14 +225,34 @@
 
 `action-react` is a tool that reacts to Telegram chat messages.
 
 ![GitHub](https://img.shields.io/github/license/yd-wu/action-react)
 ![GitHub](https://img.shields.io/github/issues/yd-wu/action-react)
 [![Build Status](https://github.com/yd-wu/action-react/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/yd-wu/action-react/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/yd-wu/action-react/branch/main/graph/badge.svg)](https://codecov.io/gh/yd-wu/action-react)
+[![PyPI](https://img.shields.io/pypi/v/action-react)](https://pypi.org/project/action-react/)
+[![Docs](https://img.shields.io/readthedocs/action-react.svg)](https://action-react.readthedocs.io)
 
 [Project Board](https://github.com/users/yd-wu/projects/1/views/1)
 
 ## Overview
 `action-react` specifically listens to an account in a Telegram chat and makes corresponding http calls given the content of the message. This is inspired by [tuixue.online-visa](https://github.com/Trinkle23897/tuixue.online-visa), a tool that periodically checks and publishes US consulate visa appointment availabilities across the world.
 
 A possible application of this tool is to use it to listen to a Telegram bot publishing messages about new visa appointments, and makes http calls to the consulate appointment service to grab the desired spot.
+
+## Installation
+Install the library's dependencies and build the library using:
+
+`pip install action-react`
+
+## Usage
+In your code, begin by importing the package:
+
+`from action-react import main`
+
+You can connect it to a telegram chat using:
+
+`main(api_id, api_hash, phone, username, target_date, cities)`
+
+For example, you can use `main("123", "hash123", "+12345678901", "username", datetime.date(2022,2,2), ["boston", "houston"])` to start the function.
+
+Alternatively, you can directly run `python main.py` after setting up the configurations in `config.ini`.
```

### Comparing `action-react-0.0.2/README.md` & `action-react-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,34 @@
 
 `action-react` is a tool that reacts to Telegram chat messages.
 
 ![GitHub](https://img.shields.io/github/license/yd-wu/action-react)
 ![GitHub](https://img.shields.io/github/issues/yd-wu/action-react)
 [![Build Status](https://github.com/yd-wu/action-react/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/yd-wu/action-react/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/yd-wu/action-react/branch/main/graph/badge.svg)](https://codecov.io/gh/yd-wu/action-react)
+[![PyPI](https://img.shields.io/pypi/v/action-react)](https://pypi.org/project/action-react/)
+[![Docs](https://img.shields.io/readthedocs/action-react.svg)](https://action-react.readthedocs.io)
 
 [Project Board](https://github.com/users/yd-wu/projects/1/views/1)
 
 ## Overview
 `action-react` specifically listens to an account in a Telegram chat and makes corresponding http calls given the content of the message. This is inspired by [tuixue.online-visa](https://github.com/Trinkle23897/tuixue.online-visa), a tool that periodically checks and publishes US consulate visa appointment availabilities across the world.
 
 A possible application of this tool is to use it to listen to a Telegram bot publishing messages about new visa appointments, and makes http calls to the consulate appointment service to grab the desired spot.
+
+## Installation
+Install the library's dependencies and build the library using:
+
+`pip install action-react`
+
+## Usage
+In your code, begin by importing the package:
+
+`from action-react import main`
+
+You can connect it to a telegram chat using:
+
+`main(api_id, api_hash, phone, username, target_date, cities)`
+
+For example, you can use `main("123", "hash123", "+12345678901", "username", datetime.date(2022,2,2), ["boston", "houston"])` to start the function.
+
+Alternatively, you can directly run `python main.py` after setting up the configurations in `config.ini`.
```

### Comparing `action-react-0.0.2/action_react/tests/test_all.py` & `action-react-0.0.3/action_react/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `action-react-0.0.2/action_react.egg-info/PKG-INFO` & `action-react-0.0.3/action_react.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action-react
-Version: 0.0.2
+Version: 0.0.3
 Summary: telegram listener tool
 Author-email: yd-wu <yw3960@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -225,14 +225,34 @@
 
 `action-react` is a tool that reacts to Telegram chat messages.
 
 ![GitHub](https://img.shields.io/github/license/yd-wu/action-react)
 ![GitHub](https://img.shields.io/github/issues/yd-wu/action-react)
 [![Build Status](https://github.com/yd-wu/action-react/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/yd-wu/action-react/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/yd-wu/action-react/branch/main/graph/badge.svg)](https://codecov.io/gh/yd-wu/action-react)
+[![PyPI](https://img.shields.io/pypi/v/action-react)](https://pypi.org/project/action-react/)
+[![Docs](https://img.shields.io/readthedocs/action-react.svg)](https://action-react.readthedocs.io)
 
 [Project Board](https://github.com/users/yd-wu/projects/1/views/1)
 
 ## Overview
 `action-react` specifically listens to an account in a Telegram chat and makes corresponding http calls given the content of the message. This is inspired by [tuixue.online-visa](https://github.com/Trinkle23897/tuixue.online-visa), a tool that periodically checks and publishes US consulate visa appointment availabilities across the world.
 
 A possible application of this tool is to use it to listen to a Telegram bot publishing messages about new visa appointments, and makes http calls to the consulate appointment service to grab the desired spot.
+
+## Installation
+Install the library's dependencies and build the library using:
+
+`pip install action-react`
+
+## Usage
+In your code, begin by importing the package:
+
+`from action-react import main`
+
+You can connect it to a telegram chat using:
+
+`main(api_id, api_hash, phone, username, target_date, cities)`
+
+For example, you can use `main("123", "hash123", "+12345678901", "username", datetime.date(2022,2,2), ["boston", "houston"])` to start the function.
+
+Alternatively, you can directly run `python main.py` after setting up the configurations in `config.ini`.
```

### Comparing `action-react-0.0.2/pyproject.toml` & `action-react-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "action-react"
 authors = [{name = "yd-wu", email = "yw3960@columbia.edu"}]
 description="telegram listener tool"
 readme = "README.md"
-version = "0.0.2"
+version = "0.0.3"
 requires-python = ">=3.7"
 
-dependencies = ["Telethon >= 1.21.1"]
+dynamic = ["dependencies"]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
@@ -94,7 +94,10 @@
 # disallow_incomplete_defs = true
 # disallow_untyped_decorators = true
 # disallow_untyped_calls = true
 
 [tool.pytest.ini_options]
 asyncio_mode = 'strict'
 testpaths = 'action_react/tests'
+
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
```

