# Comparing `tmp/sec-web-scraper-0.1.0.tar.gz` & `tmp/sec-web-scraper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sec-web-scraper-0.1.0.tar", last modified: Mon Mar 27 09:54:01 2023, max compression
+gzip compressed data, was "sec-web-scraper-0.1.1.tar", last modified: Fri May  5 09:54:42 2023, max compression
```

## Comparing `sec-web-scraper-0.1.0.tar` & `sec-web-scraper-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,37 @@
-drwxr-xr-x   0 deji       (501) staff       (20)        0 2023-03-27 09:54:01.017558 sec-web-scraper-0.1.0/
--rw-r--r--   0 deji       (501) staff       (20)      401 2023-03-27 09:43:26.000000 sec-web-scraper-0.1.0/.bumpversion.cfg
--rw-r--r--   0 deji       (501) staff       (20)     2141 2023-03-27 09:06:29.000000 sec-web-scraper-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 deji       (501) staff       (20)     1070 2023-02-12 23:14:18.000000 sec-web-scraper-0.1.0/LICENSE
--rw-r--r--   0 deji       (501) staff       (20)      392 2023-03-04 08:34:29.000000 sec-web-scraper-0.1.0/MANIFEST.in
--rw-r--r--   0 deji       (501) staff       (20)     2312 2023-03-04 08:23:13.000000 sec-web-scraper-0.1.0/Makefile
--rw-r--r--   0 deji       (501) staff       (20)     4139 2023-03-27 09:54:01.016620 sec-web-scraper-0.1.0/PKG-INFO
--rw-r--r--   0 deji       (501) staff       (20)     2062 2023-03-27 09:18:51.000000 sec-web-scraper-0.1.0/README.md
--rw-r--r--   0 deji       (501) staff       (20)     2259 2023-03-27 09:43:26.000000 sec-web-scraper-0.1.0/pyproject.toml
-drwxr-xr-x   0 deji       (501) staff       (20)        0 2023-03-27 09:54:01.007304 sec-web-scraper-0.1.0/sec_web_scraper/
--rw-r--r--   0 deji       (501) staff       (20)     5046 2023-03-27 04:58:50.000000 sec-web-scraper-0.1.0/sec_web_scraper/Downloader.py
--rw-r--r--   0 deji       (501) staff       (20)     3858 2023-03-26 20:26:06.000000 sec-web-scraper-0.1.0/sec_web_scraper/Scraper.py
--rw-r--r--   0 deji       (501) staff       (20)       57 2023-03-04 08:23:13.000000 sec-web-scraper-0.1.0/sec_web_scraper/__init__.py
--rw-r--r--   0 deji       (501) staff       (20)      987 2023-03-26 20:26:06.000000 sec-web-scraper-0.1.0/sec_web_scraper/__main__.py
--rw-r--r--   0 deji       (501) staff       (20)       22 2023-03-27 09:43:26.000000 sec-web-scraper-0.1.0/sec_web_scraper/_version.py
-drwxr-xr-x   0 deji       (501) staff       (20)        0 2023-03-27 09:54:01.014835 sec-web-scraper-0.1.0/sec_web_scraper/tests/
--rw-r--r--   0 deji       (501) staff       (20)        0 2023-03-04 08:23:13.000000 sec-web-scraper-0.1.0/sec_web_scraper/tests/__init__.py
--rw-r--r--   0 deji       (501) staff       (20)     2667 2023-03-26 20:26:06.000000 sec-web-scraper-0.1.0/sec_web_scraper/tests/test_all.py
--rw-r--r--   0 deji       (501) staff       (20)     3546 2023-03-27 04:58:50.000000 sec-web-scraper-0.1.0/sec_web_scraper/tests/test_downloader.py
-drwxr-xr-x   0 deji       (501) staff       (20)        0 2023-03-27 09:54:01.012229 sec-web-scraper-0.1.0/sec_web_scraper.egg-info/
--rw-r--r--   0 deji       (501) staff       (20)     4139 2023-03-27 09:54:00.000000 sec-web-scraper-0.1.0/sec_web_scraper.egg-info/PKG-INFO
--rw-r--r--   0 deji       (501) staff       (20)      539 2023-03-27 09:54:00.000000 sec-web-scraper-0.1.0/sec_web_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 deji       (501) staff       (20)        1 2023-03-27 09:54:00.000000 sec-web-scraper-0.1.0/sec_web_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 deji       (501) staff       (20)      181 2023-03-27 09:54:00.000000 sec-web-scraper-0.1.0/sec_web_scraper.egg-info/requires.txt
--rw-r--r--   0 deji       (501) staff       (20)       16 2023-03-27 09:54:00.000000 sec-web-scraper-0.1.0/sec_web_scraper.egg-info/top_level.txt
--rw-r--r--   0 deji       (501) staff       (20)       38 2023-03-27 09:54:01.017910 sec-web-scraper-0.1.0/setup.cfg
--rw-r--r--   0 deji       (501) staff       (20)       39 2023-03-04 08:23:13.000000 sec-web-scraper-0.1.0/setup.py
+drwxr-xr-x   0 deji       (501) staff       (20)        0 2023-05-05 09:54:42.367201 sec-web-scraper-0.1.1/
+-rw-r--r--   0 deji       (501) staff       (20)      401 2023-05-05 09:43:35.000000 sec-web-scraper-0.1.1/.bumpversion.cfg
+-rw-r--r--   0 deji       (501) staff       (20)     2387 2023-04-05 05:39:15.000000 sec-web-scraper-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 deji       (501) staff       (20)     1070 2023-02-12 23:14:18.000000 sec-web-scraper-0.1.1/LICENSE
+-rw-r--r--   0 deji       (501) staff       (20)      494 2023-04-07 06:55:02.000000 sec-web-scraper-0.1.1/MANIFEST.in
+-rw-r--r--   0 deji       (501) staff       (20)     2433 2023-04-06 06:31:29.000000 sec-web-scraper-0.1.1/Makefile
+-rw-r--r--   0 deji       (501) staff       (20)     4466 2023-05-05 09:54:42.366507 sec-web-scraper-0.1.1/PKG-INFO
+-rw-r--r--   0 deji       (501) staff       (20)     2368 2023-04-18 21:44:03.000000 sec-web-scraper-0.1.1/README.md
+drwxr-xr-x   0 deji       (501) staff       (20)        0 2023-05-05 09:54:42.344709 sec-web-scraper-0.1.1/docs/
+-rw-r--r--   0 deji       (501) staff       (20)       20 2023-04-06 06:37:28.000000 sec-web-scraper-0.1.1/docs/contributing.md
+drwxr-xr-x   0 deji       (501) staff       (20)        0 2023-05-05 09:54:42.350169 sec-web-scraper-0.1.1/docs/examples/
+-rw-r--r--   0 deji       (501) staff       (20)    71121 2023-04-07 06:55:02.000000 sec-web-scraper-0.1.1/docs/examples/example1.ipynb
+-rw-r--r--   0 deji       (501) staff       (20)    56012 2023-04-07 06:55:02.000000 sec-web-scraper-0.1.1/docs/examples/example1.md
+-rw-r--r--   0 deji       (501) staff       (20)      133 2023-04-07 06:55:02.000000 sec-web-scraper-0.1.1/docs/examples/index.md
+-rw-r--r--   0 deji       (501) staff       (20)     1068 2023-04-07 06:55:02.000000 sec-web-scraper-0.1.1/docs/gen_ref_pages.py
+-rw-r--r--   0 deji       (501) staff       (20)       14 2023-04-06 06:31:29.000000 sec-web-scraper-0.1.1/docs/index.md
+-rw-r--r--   0 deji       (501) staff       (20)       12 2023-04-06 06:31:29.000000 sec-web-scraper-0.1.1/docs/license.md
+-rw-r--r--   0 deji       (501) staff       (20)     2086 2023-04-07 06:55:02.000000 sec-web-scraper-0.1.1/mkdocs.yml
+-rw-r--r--   0 deji       (501) staff       (20)     2500 2023-05-05 09:43:35.000000 sec-web-scraper-0.1.1/pyproject.toml
+drwxr-xr-x   0 deji       (501) staff       (20)        0 2023-05-05 09:54:42.355878 sec-web-scraper-0.1.1/sec_web_scraper/
+-rw-r--r--   0 deji       (501) staff       (20)     9445 2023-05-05 07:52:40.000000 sec-web-scraper-0.1.1/sec_web_scraper/Downloader.py
+-rw-r--r--   0 deji       (501) staff       (20)     9774 2023-05-05 07:52:40.000000 sec-web-scraper-0.1.1/sec_web_scraper/Scraper.py
+-rw-r--r--   0 deji       (501) staff       (20)      639 2023-04-07 06:55:02.000000 sec-web-scraper-0.1.1/sec_web_scraper/__init__.py
+-rw-r--r--   0 deji       (501) staff       (20)     1167 2023-05-05 07:52:40.000000 sec-web-scraper-0.1.1/sec_web_scraper/__main__.py
+-rw-r--r--   0 deji       (501) staff       (20)       22 2023-05-05 09:43:35.000000 sec-web-scraper-0.1.1/sec_web_scraper/_version.py
+drwxr-xr-x   0 deji       (501) staff       (20)        0 2023-05-05 09:54:42.364246 sec-web-scraper-0.1.1/sec_web_scraper/tests/
+-rw-r--r--   0 deji       (501) staff       (20)        0 2023-03-04 08:23:13.000000 sec-web-scraper-0.1.1/sec_web_scraper/tests/__init__.py
+-rw-r--r--   0 deji       (501) staff       (20)     3281 2023-05-05 07:52:40.000000 sec-web-scraper-0.1.1/sec_web_scraper/tests/test_all.py
+-rw-r--r--   0 deji       (501) staff       (20)     3961 2023-05-05 07:52:40.000000 sec-web-scraper-0.1.1/sec_web_scraper/tests/test_downloader.py
+drwxr-xr-x   0 deji       (501) staff       (20)        0 2023-05-05 09:54:42.361605 sec-web-scraper-0.1.1/sec_web_scraper.egg-info/
+-rw-r--r--   0 deji       (501) staff       (20)     4466 2023-05-05 09:54:41.000000 sec-web-scraper-0.1.1/sec_web_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 deji       (501) staff       (20)      701 2023-05-05 09:54:42.000000 sec-web-scraper-0.1.1/sec_web_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 deji       (501) staff       (20)        1 2023-05-05 09:54:41.000000 sec-web-scraper-0.1.1/sec_web_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 deji       (501) staff       (20)      363 2023-05-05 09:54:41.000000 sec-web-scraper-0.1.1/sec_web_scraper.egg-info/requires.txt
+-rw-r--r--   0 deji       (501) staff       (20)       16 2023-05-05 09:54:42.000000 sec-web-scraper-0.1.1/sec_web_scraper.egg-info/top_level.txt
+-rw-r--r--   0 deji       (501) staff       (20)       38 2023-05-05 09:54:42.367447 sec-web-scraper-0.1.1/setup.cfg
+-rw-r--r--   0 deji       (501) staff       (20)       39 2023-03-04 08:23:13.000000 sec-web-scraper-0.1.1/setup.py
```

### Comparing `sec-web-scraper-0.1.0/CONTRIBUTING.md` & `sec-web-scraper-0.1.1/CONTRIBUTING.md`

 * *Files 9% similar despite different names*

```diff
@@ -67,7 +67,16 @@
 - `make build`: build the library using `setuptools`
 - `make lint`: perform static analysis of this library with `flake8` and `black`
 - `make format`: autoformat this library using `black`
 - `make annotate`: run type checking using `mypy`
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 - `make dist`: package library for distribution
+
+
+## Commands for generating documentation
+
+* `mkdocs new [dir-name]` - Create a new project.
+* `mkdocs serve` - Start the live-reloading docs server.
+* `mkdocs build` - Build the documentation site.
+* `mkdocs -h` - Print help message and exit.
+
```

### Comparing `sec-web-scraper-0.1.0/LICENSE` & `sec-web-scraper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sec-web-scraper-0.1.0/Makefile` & `sec-web-scraper-0.1.1/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,25 @@
 
 dist: clean build dist-build dist-check  ## Build dists
 
 publish:  # Upload python3 assets
 	echo "would usually run python3 -m twine upload dist/* --skip-existing"
 
 #########
+# DOCS #
+#########
+install-docs:
+	python3 -m pip install -e .[docs]
+
+
+deploy-docs:
+	mkdocs gh-deploy --force
+
+
+#########
 # CLEAN #
 #########
 deep-clean: ## clean everything from the repository
 	git clean -fdx
 
 clean: ## clean the repository
 	rm -rf .coverage coverage cover htmlcov logs build dist *.egg-info .pytest_cache
```

### Comparing `sec-web-scraper-0.1.0/PKG-INFO` & `sec-web-scraper-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sec-web-scraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: SEC Web Scraper for the EDGAR API
 Author-email: Deji  <deji725@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Deji Oyerinde
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,36 +35,45 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
+Provides-Extra: docs
 License-File: LICENSE
 
 # sec-web-scraper
 A Python based web scraper for the SEC EDGAR database
 
 ![Github](https://img.shields.io/github/license/deji725/sec-web-scraper)
 ![Issues](https://img.shields.io/github/issues/deji725/sec-web-scraper)
 [![codecov](https://codecov.io/gh/deji725/sec-web-scraper/branch/main/graph/badge.svg?token=Y3RGEAR6Q2)](https://codecov.io/gh/deji725/sec-web-scraper)
 ![Github](https://github.com/deji725/sec-web-scraper/actions/workflows/makefile.yml/badge.svg)
+[![docs](https://img.shields.io/github/actions/workflow/status/deji725/sec-web-scraper/docs.yml?label=docs)](https://deji725.github.io/sec-web-scraper/)
 [![PyPI](https://img.shields.io/pypi/v/sec-web-scraper)](https://pypi.org/project/sec-web-scraper/)
 
 ## Overview
 
 This library will for scraping certain financial documents from the EDGAR database such as the 10-K (and it's versions such as 10-K405,10-KSB), 20-F and 40-F. 
 
 The two main features of the library will be:
 - A document downloader portion that will fetch documents from the EDGAR database based on parameters such as a text query, time period, company ticker, and file type. 
 - A scraper that will parse sections and information from the retrieved files. 
 
 ## Installation
 
-Run the command below! 
+
+Please make sure you have Python 3.7 or higher.
+
+You can check your python version with
+
+`python --version`
+
+Then run the command below! 
 
 `pip install sec-web-scraper`
 
 ## Usage
 
 ```py
 # Downloader
@@ -87,14 +96,15 @@
 res = d.find_files_by_type('8-K') 
 
 #More features to be added!
 ``` 
 
 ```py
 #Scraper
+from sec_web_scraper.Scraper import *
 
 #With a particular filing
 sample_10k = "https://www.sec.gov/Archives/edgar/data/20/0000893220-96-000500.txt"
 
 #Get the raw text
 raw_txt = get_document_given_link(sample_10k)
```

### Comparing `sec-web-scraper-0.1.0/README.md` & `sec-web-scraper-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 # sec-web-scraper
 A Python based web scraper for the SEC EDGAR database
 
 ![Github](https://img.shields.io/github/license/deji725/sec-web-scraper)
 ![Issues](https://img.shields.io/github/issues/deji725/sec-web-scraper)
 [![codecov](https://codecov.io/gh/deji725/sec-web-scraper/branch/main/graph/badge.svg?token=Y3RGEAR6Q2)](https://codecov.io/gh/deji725/sec-web-scraper)
 ![Github](https://github.com/deji725/sec-web-scraper/actions/workflows/makefile.yml/badge.svg)
+[![docs](https://img.shields.io/github/actions/workflow/status/deji725/sec-web-scraper/docs.yml?label=docs)](https://deji725.github.io/sec-web-scraper/)
 [![PyPI](https://img.shields.io/pypi/v/sec-web-scraper)](https://pypi.org/project/sec-web-scraper/)
 
 ## Overview
 
 This library will for scraping certain financial documents from the EDGAR database such as the 10-K (and it's versions such as 10-K405,10-KSB), 20-F and 40-F. 
 
 The two main features of the library will be:
 - A document downloader portion that will fetch documents from the EDGAR database based on parameters such as a text query, time period, company ticker, and file type. 
 - A scraper that will parse sections and information from the retrieved files. 
 
 ## Installation
 
-Run the command below! 
+
+Please make sure you have Python 3.7 or higher.
+
+You can check your python version with
+
+`python --version`
+
+Then run the command below! 
 
 `pip install sec-web-scraper`
 
 ## Usage
 
 ```py
 # Downloader
@@ -44,14 +52,15 @@
 res = d.find_files_by_type('8-K') 
 
 #More features to be added!
 ``` 
 
 ```py
 #Scraper
+from sec_web_scraper.Scraper import *
 
 #With a particular filing
 sample_10k = "https://www.sec.gov/Archives/edgar/data/20/0000893220-96-000500.txt"
 
 #Get the raw text
 raw_txt = get_document_given_link(sample_10k)
```

### Comparing `sec-web-scraper-0.1.0/pyproject.toml` & `sec-web-scraper-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "sec-web-scraper"
 authors = [{name = "Deji ", email = "deji725@gmail.com"}]
 description="SEC Web Scraper for the EDGAR API"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.7"
 
 dependencies = [
     "pandas",
     "bs4",
     "requests",
     "tqdm",
+    "selenium",
+    "webdriver-manager",
 ]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
@@ -50,14 +52,22 @@
     "flake8-pyproject",
     "mypy",
     "pytest>=4.3.0",
     "pytest-cov>=2.6.1",
     "twine",
     "wheel",
 ]
+docs = [
+    "mkdocs-material>=9.1.5",
+    "mkdocstrings[python]",
+    "markdown-include>=0.8.1",
+    "mkdocs-gen-files>=0.4.0",
+    "mkdocs-literate-nav>=0.6.0",
+    "mkdocs-section-index>=0.3.5",
+]
 
 [tool.black]
 color = true
 line-length = 120
 target-version = ['py310']
 skip-string-normalization = true
```

### Comparing `sec-web-scraper-0.1.0/sec_web_scraper/__main__.py` & `sec-web-scraper-0.1.1/sec_web_scraper/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,18 @@
-from Scraper import get_company_filings_given_cik, iterate_over_filings
+from Scraper import (
+    get_company_filings_given_cik,
+    iterate_over_filings,
+    create_selenium_browser_headless,
+    get_filings_by_query,
+)
 from Downloader import Downloader
 
 
 def main():
-    sample_10k = "https://www.sec.gov/Archives/edgar/data/20/0000893220-96-000500.txt"
+    # sample_10k = "https://www.sec.gov/Archives/edgar/data/20/0000893220-96-000500.txt"
     # create_selenium_browser_headless()
     # build_index_sec(1993, 2000)
     # raw_txt = get_document_given_link(sample_10k)
     # doc_tags = get_document_tags(raw_txt)
 
     # print("These are the doc tags ")
     # print(doc_tags)
@@ -15,17 +20,19 @@
     apple_cik = get_company_filings_given_cik("0000320193")
     print("These are the keys in the official SEC API based on CIK")
     print(apple_cik.keys())
 
     print("Iterating over the filings....")
     n = iterate_over_filings(apple_cik["filings"])
     print(f"This is the file count {n}")
-    print(sample_10k)
+    # print(sample_10k)
 
     d = Downloader()
     d.build_index_sec(2010, 2010)  # Small Sample of Documents
     d.pretty_print_forms()
     d.read_tsv_files()
+    driver = create_selenium_browser_headless()
+    print(get_filings_by_query('cookies', driver))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `sec-web-scraper-0.1.0/sec_web_scraper/tests/test_all.py` & `sec-web-scraper-0.1.1/sec_web_scraper/tests/test_all.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 from unittest.mock import patch, MagicMock
+from selenium import webdriver
+from selenium.webdriver.chrome.service import Service
+from webdriver_manager.chrome import ChromeDriverManager
+from selenium.webdriver.chrome.options import Options
+
 import pandas as pd
 import pytest
 import requests
 import os
 from sec_web_scraper import *
 
 test_link = "https://www.sec.gov/Archives/edgar/data/20/0000893220-96-000500.txt"
@@ -78,7 +83,20 @@
     assert mock_print.call_args.args == ("Good",)
 
 
 def test_create_selenium_browser_headless_con_err():
     with pytest.raises(ConnectionError) as conn_er:
         create_selenium_browser_headless("https://www.sec.gov/edgar/2/2")
         print(f'{conn_er}')
+
+
+def test_get_filings_by_query():
+    service = Service(ChromeDriverManager().install())
+    chrome_options = Options()
+    chrome_options.add_argument("--headless=new")
+    driver = webdriver.Chrome(service=service, options=chrome_options)
+    test_data = get_filings_by_query('cookies', driver)
+    assert test_data is not None
+
+
+# @patch('Scraper.get_filings_by_query')
+# def test_get_filings_by_query_failure():
```

### Comparing `sec-web-scraper-0.1.0/sec_web_scraper/tests/test_downloader.py` & `sec-web-scraper-0.1.1/sec_web_scraper/tests/test_downloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -118,12 +118,25 @@
 
 def test_find_files_by_type_fail():
     with pytest.raises(Exception) as context:
         d.find_files_by_type('XYZ-123')
     assert "does not exist" in str(context.value)
 
 
+def test_find_files_by_company_empty():
+    resp = d.find_files_by_company('0000104169')
+    # We had a valid CIK but company did not exist in this range
+    assert resp.shape[0] == 0
+
+
+def test_find_files_by_company_fail_assert_fail():
+    with pytest.raises(Exception) as context:
+        # the provided CIK is not of length 10
+        d.find_files_by_company('001104169')
+    assert "10" in str(context.value)
+
+
 # Last test
 def test_cleanup_dir():
     shutil.rmtree(indx_sec_path)
     with pytest.raises(FileNotFoundError) as context:
         os.listdir(indx_sec_path)
```

### Comparing `sec-web-scraper-0.1.0/sec_web_scraper.egg-info/PKG-INFO` & `sec-web-scraper-0.1.1/sec_web_scraper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sec-web-scraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: SEC Web Scraper for the EDGAR API
 Author-email: Deji  <deji725@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Deji Oyerinde
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,36 +35,45 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
+Provides-Extra: docs
 License-File: LICENSE
 
 # sec-web-scraper
 A Python based web scraper for the SEC EDGAR database
 
 ![Github](https://img.shields.io/github/license/deji725/sec-web-scraper)
 ![Issues](https://img.shields.io/github/issues/deji725/sec-web-scraper)
 [![codecov](https://codecov.io/gh/deji725/sec-web-scraper/branch/main/graph/badge.svg?token=Y3RGEAR6Q2)](https://codecov.io/gh/deji725/sec-web-scraper)
 ![Github](https://github.com/deji725/sec-web-scraper/actions/workflows/makefile.yml/badge.svg)
+[![docs](https://img.shields.io/github/actions/workflow/status/deji725/sec-web-scraper/docs.yml?label=docs)](https://deji725.github.io/sec-web-scraper/)
 [![PyPI](https://img.shields.io/pypi/v/sec-web-scraper)](https://pypi.org/project/sec-web-scraper/)
 
 ## Overview
 
 This library will for scraping certain financial documents from the EDGAR database such as the 10-K (and it's versions such as 10-K405,10-KSB), 20-F and 40-F. 
 
 The two main features of the library will be:
 - A document downloader portion that will fetch documents from the EDGAR database based on parameters such as a text query, time period, company ticker, and file type. 
 - A scraper that will parse sections and information from the retrieved files. 
 
 ## Installation
 
-Run the command below! 
+
+Please make sure you have Python 3.7 or higher.
+
+You can check your python version with
+
+`python --version`
+
+Then run the command below! 
 
 `pip install sec-web-scraper`
 
 ## Usage
 
 ```py
 # Downloader
@@ -87,14 +96,15 @@
 res = d.find_files_by_type('8-K') 
 
 #More features to be added!
 ``` 
 
 ```py
 #Scraper
+from sec_web_scraper.Scraper import *
 
 #With a particular filing
 sample_10k = "https://www.sec.gov/Archives/edgar/data/20/0000893220-96-000500.txt"
 
 #Get the raw text
 raw_txt = get_document_given_link(sample_10k)
```

### Comparing `sec-web-scraper-0.1.0/sec_web_scraper.egg-info/SOURCES.txt` & `sec-web-scraper-0.1.1/sec_web_scraper.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 .bumpversion.cfg
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
+mkdocs.yml
 pyproject.toml
 setup.py
+docs/contributing.md
+docs/gen_ref_pages.py
+docs/index.md
+docs/license.md
+docs/examples/example1.ipynb
+docs/examples/example1.md
+docs/examples/index.md
 sec_web_scraper/Downloader.py
 sec_web_scraper/Scraper.py
 sec_web_scraper/__init__.py
 sec_web_scraper/__main__.py
 sec_web_scraper/_version.py
 sec_web_scraper.egg-info/PKG-INFO
 sec_web_scraper.egg-info/SOURCES.txt
```

