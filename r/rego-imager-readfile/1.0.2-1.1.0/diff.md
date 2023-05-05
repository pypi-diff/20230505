# Comparing `tmp/rego-imager-readfile-1.0.2.tar.gz` & `tmp/rego_imager_readfile-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rego-imager-readfile-1.0.2.tar", max compression
+gzip compressed data, was "rego_imager_readfile-1.1.0.tar", max compression
```

## Comparing `rego-imager-readfile-1.0.2.tar` & `rego_imager_readfile-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1078 2021-02-25 19:14:26.512184 rego-imager-readfile-1.0.2/LICENSE
--rw-r--r--   0        0        0     2274 2021-02-25 19:14:26.512184 rego-imager-readfile-1.0.2/README.md
--rw-r--r--   0        0        0      665 2021-03-29 15:26:02.175667 rego-imager-readfile-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       47 2021-03-29 15:26:02.271668 rego-imager-readfile-1.0.2/rego_imager_readfile/__init__.py
--rw-r--r--   0        0        0     7731 2021-03-29 15:25:44.347667 rego-imager-readfile-1.0.2/rego_imager_readfile/_rego.py
--rw-r--r--   0        0        0     3051 2021-03-29 15:26:13.229345 rego-imager-readfile-1.0.2/setup.py
--rw-r--r--   0        0        0     3017 2021-03-29 15:26:13.230074 rego-imager-readfile-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2021-02-25 19:14:26.000000 rego_imager_readfile-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2400 2023-05-05 00:57:47.375894 rego_imager_readfile-1.1.0/README.md
+-rw-r--r--   0        0        0      650 2023-05-05 01:01:21.257426 rego_imager_readfile-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-05-05 01:01:21.301427 rego_imager_readfile-1.1.0/rego_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     7731 2021-03-29 15:25:44.000000 rego_imager_readfile-1.1.0/rego_imager_readfile/_rego.py
+-rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 rego_imager_readfile-1.1.0/PKG-INFO
```

### Comparing `rego-imager-readfile-1.0.2/LICENSE` & `rego_imager_readfile-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rego-imager-readfile-1.0.2/README.md` & `rego_imager_readfile-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,29 @@
 [![Github Actions - Tests](https://github.com/ucalgary-aurora/rego-imager-readfile/workflows/tests/badge.svg)](https://github.com/ucalgary-aurora/rego-imager-readfile/actions?query=workflow%3Atests)
 [![PyPI version](https://img.shields.io/pypi/v/rego-imager-readfile.svg)](https://pypi.python.org/pypi/rego-imager-readfile/)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 [![PyPI Python versions](https://img.shields.io/pypi/pyversions/rego-imager-readfile.svg)](https://pypi.python.org/pypi/rego-imager-readfile/)
 
 Python library for reading REGO All-Sky Imager (ASI) stream0 raw PGM-file data. The data can be found at https://data.phys.ucalgary.ca.
 
+## Supported Datasets
+
+- REGO raw: [stream0](https://data.phys.ucalgary.ca/sort_by_project/GO-Canada/REGO/stream0) PGM files
+
 ## Installation
 
 The rego-imager-readfile library is available on PyPI:
 
 ```console
 $ python3 -m pip install rego-imager-readfile
 ```
 
 ## Supported Python Versions
 
-rego-imager-readfile officially supports Python 3.6+.
+rego-imager-readfile officially supports Python 3.8+.
 
 ## Examples
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
```

### Comparing `rego-imager-readfile-1.0.2/pyproject.toml` & `rego_imager_readfile-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [tool.poetry]
 name = "rego-imager-readfile"
-version = "1.0.2"
+version = "1.1.0"
 description = "Read functions for REGO ASI PGM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/rego-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/rego-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
     { include = "rego_imager_readfile" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-numpy = "^1.19.2"
+python = "^3.8.1"
+numpy = "^1.24.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
-flake8 = "^3.8.4"
-pylint = "^2.6.0"
-autopep8 = "^1.5.6"
+pytest = "^7.0.0"
+flake8 = "^6.0.0"
+pylint = "^2.16.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rego-imager-readfile-1.0.2/rego_imager_readfile/_rego.py` & `rego_imager_readfile-1.1.0/rego_imager_readfile/_rego.py`

 * *Files identical despite different names*

### Comparing `rego-imager-readfile-1.0.2/setup.py` & `rego_imager_readfile-1.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,95 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: rego-imager-readfile
+Version: 1.1.0
+Summary: Read functions for REGO ASI PGM raw files
+Home-page: https://github.com/ucalgary-aurora/rego-imager-readfile
+License: MIT
+Author: Darren Chaddock
+Author-email: dchaddoc@ucalgary.ca
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.24.0,<2.0.0)
+Project-URL: Repository, https://github.com/ucalgary-aurora/rego-imager-readfile
+Description-Content-Type: text/markdown
 
-packages = \
-['rego_imager_readfile']
+# Redline All-Sky Imager Raw PGM Data Readfile (REGO)
 
-package_data = \
-{'': ['*']}
+[![Github Actions - Tests](https://github.com/ucalgary-aurora/rego-imager-readfile/workflows/tests/badge.svg)](https://github.com/ucalgary-aurora/rego-imager-readfile/actions?query=workflow%3Atests)
+[![PyPI version](https://img.shields.io/pypi/v/rego-imager-readfile.svg)](https://pypi.python.org/pypi/rego-imager-readfile/)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
+[![PyPI Python versions](https://img.shields.io/pypi/pyversions/rego-imager-readfile.svg)](https://pypi.python.org/pypi/rego-imager-readfile/)
 
-install_requires = \
-['numpy>=1.19.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'rego-imager-readfile',
-    'version': '1.0.2',
-    'description': 'Read functions for REGO ASI PGM raw files',
-    'long_description': '# Redline All-Sky Imager Raw PGM Data Readfile (REGO)\n\n[![Github Actions - Tests](https://github.com/ucalgary-aurora/rego-imager-readfile/workflows/tests/badge.svg)](https://github.com/ucalgary-aurora/rego-imager-readfile/actions?query=workflow%3Atests)\n[![PyPI version](https://img.shields.io/pypi/v/rego-imager-readfile.svg)](https://pypi.python.org/pypi/rego-imager-readfile/)\n[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)\n[![PyPI Python versions](https://img.shields.io/pypi/pyversions/rego-imager-readfile.svg)](https://pypi.python.org/pypi/rego-imager-readfile/)\n\nPython library for reading REGO All-Sky Imager (ASI) stream0 raw PGM-file data. The data can be found at https://data.phys.ucalgary.ca.\n\n## Installation\n\nThe rego-imager-readfile library is available on PyPI:\n\n```console\n$ python3 -m pip install rego-imager-readfile\n```\n\n## Supported Python Versions\n\nrego-imager-readfile officially supports Python 3.6+.\n\n## Examples\n\nExample Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.\n\n## Usage\n\nImport the library using `import rego_imager_readfile`\n\n### Read a single file\n\n```python\n>>> import rego_imager_readfile\n>>> filename = "path/to/data/2020/01/01/fsmi_rego-654/ut06/20200101_0600_fsmi_rego-654_6300.pgm.gz"\n>>> img, meta, problematic_files = rego_imager_readfile.read(filename)\n```\n\n### Read multiple files\n\n```python\n>>> import rego_imager_readfile, glob\n>>> file_list = glob.glob("path/to/files/2020/01/01/fsmi_rego-654/ut06/*6300.pgm*")\n>>> img, meta, problematic_files = rego_imager_readfile.read(file_list)\n```\n\n### Read using multiple worker processes\n\n```python\n>>> import rego_imager_readfile, glob\n>>> file_list = glob.glob("path/to/files/2020/01/01/fsmi_rego-654/ut06/*6300.pgm*")\n>>> img, meta, problematic_files = rego_imager_readfile.read(file_list, workers=4)\n```\n\n## Development\n\nClone the repository and install dependencies using Poetry.\n\n```console\n$ git clone https://github.com/ucalgary-aurora/rego-imager-readfile.git\n$ cd rego-imager-readfile/python\n$ make install\n```\n\n## Testing\n\n```console\n$ make test\n[ or do each test separately ]\n$ make test-flake8\n$ make test-pylint\n$ make test-pytest\n```\n',
-    'author': 'Darren Chaddock',
-    'author_email': 'dchaddoc@ucalgary.ca',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/ucalgary-aurora/rego-imager-readfile',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
+Python library for reading REGO All-Sky Imager (ASI) stream0 raw PGM-file data. The data can be found at https://data.phys.ucalgary.ca.
 
+## Supported Datasets
+
+- REGO raw: [stream0](https://data.phys.ucalgary.ca/sort_by_project/GO-Canada/REGO/stream0) PGM files
+
+## Installation
+
+The rego-imager-readfile library is available on PyPI:
+
+```console
+$ python3 -m pip install rego-imager-readfile
+```
+
+## Supported Python Versions
+
+rego-imager-readfile officially supports Python 3.8+.
+
+## Examples
+
+Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
+
+## Usage
+
+Import the library using `import rego_imager_readfile`
+
+### Read a single file
+
+```python
+>>> import rego_imager_readfile
+>>> filename = "path/to/data/2020/01/01/fsmi_rego-654/ut06/20200101_0600_fsmi_rego-654_6300.pgm.gz"
+>>> img, meta, problematic_files = rego_imager_readfile.read(filename)
+```
+
+### Read multiple files
+
+```python
+>>> import rego_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2020/01/01/fsmi_rego-654/ut06/*6300.pgm*")
+>>> img, meta, problematic_files = rego_imager_readfile.read(file_list)
+```
+
+### Read using multiple worker processes
+
+```python
+>>> import rego_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2020/01/01/fsmi_rego-654/ut06/*6300.pgm*")
+>>> img, meta, problematic_files = rego_imager_readfile.read(file_list, workers=4)
+```
+
+## Development
+
+Clone the repository and install dependencies using Poetry.
+
+```console
+$ git clone https://github.com/ucalgary-aurora/rego-imager-readfile.git
+$ cd rego-imager-readfile/python
+$ make install
+```
+
+## Testing
+
+```console
+$ make test
+[ or do each test separately ]
+$ make test-flake8
+$ make test-pylint
+$ make test-pytest
+```
 
-setup(**setup_kwargs)
```

