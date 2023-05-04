# Comparing `tmp/converterpro-0.1.1.tar.gz` & `tmp/converterpro-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "converterpro-0.1.1.tar", max compression
+gzip compressed data, was "converterpro-0.1.2.tar", max compression
```

## Comparing `converterpro-0.1.1.tar` & `converterpro-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-03-18 02:04:48.516036 converterpro-0.1.1/LICENSE
--rw-r--r--   0        0        0     1993 2023-03-27 15:30:57.087982 converterpro-0.1.1/README.md
--rw-r--r--   0        0        0       55 2023-03-27 16:02:14.447291 converterpro-0.1.1/converterpro/__init__.py
--rw-r--r--   0        0        0     5244 2023-03-27 15:30:57.090185 converterpro-0.1.1/converterpro/weight_converter.py
--rw-r--r--   0        0        0     1042 2023-03-27 16:02:14.447555 converterpro-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2573 1970-01-01 00:00:00.000000 converterpro-0.1.1/setup.py
--rw-r--r--   0        0        0     2973 1970-01-01 00:00:00.000000 converterpro-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-20 20:31:00.164604 converterpro-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2935 2023-05-04 22:08:53.369783 converterpro-0.1.2/README.md
+-rw-r--r--   0        0        0      369 2023-05-04 22:08:53.370342 converterpro-0.1.2/converterpro/__init__.py
+-rw-r--r--   0        0        0    17396 2023-05-04 22:08:53.370792 converterpro-0.1.2/converterpro/weight_converter.py
+-rw-r--r--   0        0        0     1403 2023-05-04 22:08:53.372464 converterpro-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3581 1970-01-01 00:00:00.000000 converterpro-0.1.2/setup.py
+-rw-r--r--   0        0        0     4081 1970-01-01 00:00:00.000000 converterpro-0.1.2/PKG-INFO
```

### Comparing `converterpro-0.1.1/LICENSE` & `converterpro-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `converterpro-0.1.1/README.md` & `converterpro-0.1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,71 @@
+<!-- BEGIN INCLUDE -->
 # ConverterPro
+
 A python library to convert units and currencies
 
 ![Hex.pm](https://img.shields.io/hexpm/l/apa?style=flat&color=brightgreen)
 ![GitHub issues](https://img.shields.io/github/issues/oforiwaasam/converterpro)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/oforiwaasam/converterpro/build.yml)](https://github.com/oforiwaasam/converterpro/actions/workflows/build.yml)
-[![Coverage Status](https://coveralls.io/repos/github/oforiwaasam/converterpro/badge.svg?branch=main&kill_cache=1)](https://coveralls.io/github/oforiwaasam/converterpro?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/oforiwaasam/converterpro/badge.svg?branch=main)](https://coveralls.io/github/oforiwaasam/converterpro?branch=main)
 [![black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)
 [![poetry](https://img.shields.io/badge/packaging-poetry-008adf)](https://python-poetry.org/)
+[![PyPI](https://img.shields.io/pypi/v/converterpro)](https://pypi.org/project/converterpro/)
+[![Deployment](https://img.shields.io/github/deployments/oforiwaasam/converterpro/github-pages?label=GitHub&nbsp;Pages)](https://oforiwaasam.github.io/converterpro)
+[![Documentation Status](https://readthedocs.org/projects/converterpro/badge/?version=latest)](https://converterpro.readthedocs.io/en/latest/?badge=latest)
 
 ## 🔭 Overview
+
 This python library will allow developers to easily incorporate conversions into their programs without having to write all the logic for it. The library currently has the following functionalities:
-- Converting Metric System, Imperial System and US System Measurements
 
-## Installation
+## 📝 Features
+
++ Weight conversion between Metric, Imperial and US Systems of Measurement
+  + Grams
+  + Milligrams
+  + Kilograms
+  + Metric Tonnes
+  + Imperial Tons
+  + US tons
+  + Pounds
+  + Ounces
 
-Install **converterpro** with `pip`:
+## 🛠️ Installation
+
+**converterpro** can be found on [PyPi](https://pypi.org/project/converterpro/0.1.1/) and hence can be installed with `pip`:
 
 ```bash
 pip install converterpro
 ```
 
+## ⛯ Basic Usage
+
+```python3
+>>> from converterpro import weight_converter
+>>> my_gram = weight_converter.Gram(1.0)
+>>> my_gram.convert_to_kilograms()
+0.001
+```
+
 ## 📝 Details
+
 This library project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
-- `make`: list available commands
-- `make install`: install and build this library and its dependencies using `poetry`
-- `make lint`: perform static analysis of this library with `ruff` and `black`
-- `make format`: autoformat this library using `black` and `ruff`
-- `make test`: run automated tests with `pytest`
-- `make coverage`: run automated tests with `pytest` and collect coverage information
 
-## 👩🏾‍💻👨🏾‍ Contributing
++ `make`: list available commands
++ `make install`: install and build this library and its dependencies using `poetry`
++ `make lint`: perform static analysis of this library with `ruff` and `black`
++ `make format`: autoformat this library using `black` and `ruff`
++ `make test`: run automated tests with `pytest`
++ `make coverage`: run automated tests with `pytest` and collect coverage information
+<!-- END INCLUDE -->
+
+## 👩🏾‍💻👨🏾‍💻 Contributing
 
-Please see [CONTRIBUTING](CONTRIBUTING.md) for more information.
+Please see [CONTRIBUTING](https://converterpro.readthedocs.io/en/latest/contributing/) for more information.
 
-## License
+## 🪪 License
 
-This software is licensed under the Apache 2.0 license. Please see [LICENSE](LICENSE) for more information.
+This software is licensed under the Apache 2.0 license. Please see [LICENSE](https://converterpro.readthedocs.io/en/latest/license/) for more information.
 
 ## 🙎🏾‍ Author
-Main Maintainer: Lily Sam
 
+Main Maintainer: Lily Sam
```

### Comparing `converterpro-0.1.1/pyproject.toml` & `converterpro-0.1.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [tool.poetry]
 name = "converterpro"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python converter library"
 authors = ["Lily Sam <los2119@columbia.edu>"]
 license = "Apache-2.0"
 readme = "README.md"
+homepage = "http://converterpro.readthedocs.io/"
+repository = "https://github.com/oforiwaasam/converterpro"
+keywords = ["weight-conversion", "converter", "oforiwaasam"]
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
@@ -24,20 +27,28 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 black = "^23.1.0"
 ruff = "^0.0.258"
 pytest-cov = "^4.0.0"
 bump2version = "^1.0.1"
 
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.4.2"
+mkdocstrings = {extras = ["python"], version = "^0.21.2"}
+mkdocs-material = "^9.1.6"
+
 [tool.black]
 color = true
 line-length = 130
 
 [tool.ruff]
 line-length = 130
 
 [tool.ruff.per-file-ignores]
-"__init__.py" = ["F403"]
+"__init__.py" = ["F403", "F401"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `converterpro-0.1.1/setup.py` & `converterpro-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 ['converterpro']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'converterpro',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Python converter library',
-    'long_description': '# ConverterPro\nA python library to convert units and currencies\n\n![Hex.pm](https://img.shields.io/hexpm/l/apa?style=flat&color=brightgreen)\n![GitHub issues](https://img.shields.io/github/issues/oforiwaasam/converterpro)\n[![Build Status](https://img.shields.io/github/actions/workflow/status/oforiwaasam/converterpro/build.yml)](https://github.com/oforiwaasam/converterpro/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/oforiwaasam/converterpro/badge.svg?branch=main&kill_cache=1)](https://coveralls.io/github/oforiwaasam/converterpro?branch=main)\n[![black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)\n[![poetry](https://img.shields.io/badge/packaging-poetry-008adf)](https://python-poetry.org/)\n\n## 🔭 Overview\nThis python library will allow developers to easily incorporate conversions into their programs without having to write all the logic for it. The library currently has the following functionalities:\n- Converting Metric System, Imperial System and US System Measurements\n\n## Installation\n\nInstall **converterpro** with `pip`:\n\n```bash\npip install converterpro\n```\n\n## 📝 Details\nThis library project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:\n- `make`: list available commands\n- `make install`: install and build this library and its dependencies using `poetry`\n- `make lint`: perform static analysis of this library with `ruff` and `black`\n- `make format`: autoformat this library using `black` and `ruff`\n- `make test`: run automated tests with `pytest`\n- `make coverage`: run automated tests with `pytest` and collect coverage information\n\n## 👩🏾\u200d💻👨🏾\u200d Contributing\n\nPlease see [CONTRIBUTING](CONTRIBUTING.md) for more information.\n\n## License\n\nThis software is licensed under the Apache 2.0 license. Please see [LICENSE](LICENSE) for more information.\n\n## 🙎🏾\u200d Author\nMain Maintainer: Lily Sam\n\n',
+    'long_description': '<!-- BEGIN INCLUDE -->\n# ConverterPro\n\nA python library to convert units and currencies\n\n![Hex.pm](https://img.shields.io/hexpm/l/apa?style=flat&color=brightgreen)\n![GitHub issues](https://img.shields.io/github/issues/oforiwaasam/converterpro)\n[![Build Status](https://img.shields.io/github/actions/workflow/status/oforiwaasam/converterpro/build.yml)](https://github.com/oforiwaasam/converterpro/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/oforiwaasam/converterpro/badge.svg?branch=main)](https://coveralls.io/github/oforiwaasam/converterpro?branch=main)\n[![black](https://img.shields.io/badge/code%20style-black-000000)](https://github.com/psf/black)\n[![poetry](https://img.shields.io/badge/packaging-poetry-008adf)](https://python-poetry.org/)\n[![PyPI](https://img.shields.io/pypi/v/converterpro)](https://pypi.org/project/converterpro/)\n[![Deployment](https://img.shields.io/github/deployments/oforiwaasam/converterpro/github-pages?label=GitHub&nbsp;Pages)](https://oforiwaasam.github.io/converterpro)\n[![Documentation Status](https://readthedocs.org/projects/converterpro/badge/?version=latest)](https://converterpro.readthedocs.io/en/latest/?badge=latest)\n\n## 🔭 Overview\n\nThis python library will allow developers to easily incorporate conversions into their programs without having to write all the logic for it. The library currently has the following functionalities:\n\n## 📝 Features\n\n+ Weight conversion between Metric, Imperial and US Systems of Measurement\n  + Grams\n  + Milligrams\n  + Kilograms\n  + Metric Tonnes\n  + Imperial Tons\n  + US tons\n  + Pounds\n  + Ounces\n\n## 🛠️ Installation\n\n**converterpro** can be found on [PyPi](https://pypi.org/project/converterpro/0.1.1/) and hence can be installed with `pip`:\n\n```bash\npip install converterpro\n```\n\n## ⛯ Basic Usage\n\n```python3\n>>> from converterpro import weight_converter\n>>> my_gram = weight_converter.Gram(1.0)\n>>> my_gram.convert_to_kilograms()\n0.001\n```\n\n## 📝 Details\n\nThis library project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:\n\n+ `make`: list available commands\n+ `make install`: install and build this library and its dependencies using `poetry`\n+ `make lint`: perform static analysis of this library with `ruff` and `black`\n+ `make format`: autoformat this library using `black` and `ruff`\n+ `make test`: run automated tests with `pytest`\n+ `make coverage`: run automated tests with `pytest` and collect coverage information\n<!-- END INCLUDE -->\n\n## 👩🏾\u200d💻👨🏾\u200d💻 Contributing\n\nPlease see [CONTRIBUTING](https://converterpro.readthedocs.io/en/latest/contributing/) for more information.\n\n## \U0001faaa License\n\nThis software is licensed under the Apache 2.0 license. Please see [LICENSE](https://converterpro.readthedocs.io/en/latest/license/) for more information.\n\n## 🙎🏾\u200d Author\n\nMain Maintainer: Lily Sam\n',
     'author': 'Lily Sam',
     'author_email': 'los2119@columbia.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'http://converterpro.readthedocs.io/',
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

