# Comparing `tmp/rainbow-imager-readfile-1.0.3.tar.gz` & `tmp/rainbow_imager_readfile-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rainbow-imager-readfile-1.0.3.tar", max compression
+gzip compressed data, was "rainbow_imager_readfile-1.1.0.tar", max compression
```

## Comparing `rainbow-imager-readfile-1.0.3.tar` & `rainbow_imager_readfile-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1078 2021-06-16 15:28:11.005799 rainbow-imager-readfile-1.0.3/LICENSE
--rw-r--r--   0        0        0     2384 2021-11-17 16:45:17.660513 rainbow-imager-readfile-1.0.3/README.md
--rw-r--r--   0        0        0      680 2021-11-17 16:46:52.471895 rainbow-imager-readfile-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       50 2021-11-17 16:45:17.660513 rainbow-imager-readfile-1.0.3/rainbow_imager_readfile/__init__.py
--rw-r--r--   0        0        0     7868 2021-11-17 16:50:19.463339 rainbow-imager-readfile-1.0.3/rainbow_imager_readfile/_rainbow.py
--rw-r--r--   0        0        0     3173 2021-11-17 16:50:52.968576 rainbow-imager-readfile-1.0.3/setup.py
--rw-r--r--   0        0        0     3139 2021-11-17 16:50:52.968814 rainbow-imager-readfile-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2021-06-16 15:28:11.000000 rainbow_imager_readfile-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2384 2023-05-04 21:39:27.812884 rainbow_imager_readfile-1.1.0/README.md
+-rw-r--r--   0        0        0      665 2023-05-04 21:40:51.456457 rainbow_imager_readfile-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-05-04 21:40:51.501458 rainbow_imager_readfile-1.1.0/rainbow_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     7868 2021-11-17 16:50:19.000000 rainbow_imager_readfile-1.1.0/rainbow_imager_readfile/_rainbow.py
+-rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 rainbow_imager_readfile-1.1.0/PKG-INFO
```

### Comparing `rainbow-imager-readfile-1.0.3/LICENSE` & `rainbow_imager_readfile-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rainbow-imager-readfile-1.0.3/README.md` & `rainbow_imager_readfile-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 ```console
 $ python3 -m pip install rainbow-imager-readfile
 ```
 
 ## Supported Python Versions
 
-rainbow-imager-readfile officially supports Python 3.6+.
+rainbow-imager-readfile officially supports Python 3.8+.
 
 ## Examples
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
```

### Comparing `rainbow-imager-readfile-1.0.3/pyproject.toml` & `rainbow_imager_readfile-1.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [tool.poetry]
 name = "rainbow-imager-readfile"
-version = "1.0.3"
+version = "1.1.0"
 description = "Read functions for Rainbow ASI PNM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/rainbow-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/rainbow-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
     { include = "rainbow_imager_readfile" },
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

### Comparing `rainbow-imager-readfile-1.0.3/rainbow_imager_readfile/_rainbow.py` & `rainbow_imager_readfile-1.1.0/rainbow_imager_readfile/_rainbow.py`

 * *Files identical despite different names*

### Comparing `rainbow-imager-readfile-1.0.3/setup.py` & `rainbow_imager_readfile-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,91 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: rainbow-imager-readfile
+Version: 1.1.0
+Summary: Read functions for Rainbow ASI PNM raw files
+Home-page: https://github.com/ucalgary-aurora/rainbow-imager-readfile
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
+Project-URL: Repository, https://github.com/ucalgary-aurora/rainbow-imager-readfile
+Description-Content-Type: text/markdown
 
-packages = \
-['rainbow_imager_readfile']
+# Rainbow All-Sky Imager Raw PGM Data Readfile (GO-Canada AGO/CGSM Rainbow)
 
-package_data = \
-{'': ['*']}
+[![Github Actions - Tests](https://github.com/ucalgary-aurora/rainbow-imager-readfile/workflows/tests/badge.svg)](https://github.com/ucalgary-aurora/rainbow-imager-readfile/actions?query=workflow%3Atests)
+[![PyPI version](https://img.shields.io/pypi/v/rainbow-imager-readfile.svg)](https://pypi.python.org/pypi/rainbow-imager-readfile/)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
+[![PyPI Python versions](https://img.shields.io/pypi/pyversions/rainbow-imager-readfile.svg)](https://pypi.python.org/pypi/rainbow-imager-readfile/)
 
-install_requires = \
-['numpy>=1.19.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'rainbow-imager-readfile',
-    'version': '1.0.3',
-    'description': 'Read functions for Rainbow ASI PNM raw files',
-    'long_description': '# Rainbow All-Sky Imager Raw PGM Data Readfile (GO-Canada AGO/CGSM Rainbow)\n\n[![Github Actions - Tests](https://github.com/ucalgary-aurora/rainbow-imager-readfile/workflows/tests/badge.svg)](https://github.com/ucalgary-aurora/rainbow-imager-readfile/actions?query=workflow%3Atests)\n[![PyPI version](https://img.shields.io/pypi/v/rainbow-imager-readfile.svg)](https://pypi.python.org/pypi/rainbow-imager-readfile/)\n[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)\n[![PyPI Python versions](https://img.shields.io/pypi/pyversions/rainbow-imager-readfile.svg)](https://pypi.python.org/pypi/rainbow-imager-readfile/)\n\nPython library for reading Rainbow All-Sky Imager (GO-Canada AGO/CGSM Rainbow) stream0 raw PGM-file data. The data can be found at https://data.phys.ucalgary.ca.\n\n## Installation\n\nThe rainbow-imager-readfile library is available on PyPI:\n\n```console\n$ python3 -m pip install rainbow-imager-readfile\n```\n\n## Supported Python Versions\n\nrainbow-imager-readfile officially supports Python 3.6+.\n\n## Examples\n\nExample Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.\n\n## Usage\n\nImport the library using `import rainbow_imager_readfile`\n\n### Read a single file\n\n```python\n>>> import rainbow_imager_readfile\n>>> filename = "path/to/data/2015/01/01/fsmi_rainbow-11/ut06/20150101_0600_fsmi_rainbow-11_full.pgm.gz"\n>>> img, meta, problematic_files = rainbow_imager_readfile.read(filename)\n```\n\n### Read multiple files\n\n```python\n>>> import rainbow_imager_readfile, glob\n>>> file_list = glob.glob("path/to/files/2015/01/01/fsmi_rainbow-11/ut06/*full.pgm*")\n>>> img, meta, problematic_files = rainbow_imager_readfile.read(file_list)\n```\n\n### Read using multiple worker processes\n\n```python\n>>> import rainbow_imager_readfile, glob\n>>> file_list = glob.glob("path/to/files/2015/01/01/fsmi_rainbow-11/ut06/*full.pgm*")\n>>> img, meta, problematic_files = rainbow_imager_readfile.read(file_list, workers=4)\n```\n\n## Development\n\nClone the repository and install dependencies using Poetry.\n\n```console\n$ git clone https://github.com/ucalgary-aurora/rainbow-imager-readfile.git\n$ cd rainbow-imager-readfile/python\n$ make install\n```\n\n## Testing\n\n```console\n$ make test\n[ or do each test separately ]\n$ make test-flake8\n$ make test-pylint\n$ make test-pytest\n```\n',
-    'author': 'Darren Chaddock',
-    'author_email': 'dchaddoc@ucalgary.ca',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/ucalgary-aurora/rainbow-imager-readfile',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
+Python library for reading Rainbow All-Sky Imager (GO-Canada AGO/CGSM Rainbow) stream0 raw PGM-file data. The data can be found at https://data.phys.ucalgary.ca.
 
+## Installation
+
+The rainbow-imager-readfile library is available on PyPI:
+
+```console
+$ python3 -m pip install rainbow-imager-readfile
+```
+
+## Supported Python Versions
+
+rainbow-imager-readfile officially supports Python 3.8+.
+
+## Examples
+
+Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
+
+## Usage
+
+Import the library using `import rainbow_imager_readfile`
+
+### Read a single file
+
+```python
+>>> import rainbow_imager_readfile
+>>> filename = "path/to/data/2015/01/01/fsmi_rainbow-11/ut06/20150101_0600_fsmi_rainbow-11_full.pgm.gz"
+>>> img, meta, problematic_files = rainbow_imager_readfile.read(filename)
+```
+
+### Read multiple files
+
+```python
+>>> import rainbow_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2015/01/01/fsmi_rainbow-11/ut06/*full.pgm*")
+>>> img, meta, problematic_files = rainbow_imager_readfile.read(file_list)
+```
+
+### Read using multiple worker processes
+
+```python
+>>> import rainbow_imager_readfile, glob
+>>> file_list = glob.glob("path/to/files/2015/01/01/fsmi_rainbow-11/ut06/*full.pgm*")
+>>> img, meta, problematic_files = rainbow_imager_readfile.read(file_list, workers=4)
+```
+
+## Development
+
+Clone the repository and install dependencies using Poetry.
+
+```console
+$ git clone https://github.com/ucalgary-aurora/rainbow-imager-readfile.git
+$ cd rainbow-imager-readfile/python
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

