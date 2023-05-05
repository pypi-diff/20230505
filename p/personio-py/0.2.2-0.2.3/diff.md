# Comparing `tmp/personio-py-0.2.2.tar.gz` & `tmp/personio-py-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/personio-py-0.2.2.tar", last modified: Mon Jul  4 14:13:34 2022, max compression
+gzip compressed data, was "dist/personio-py-0.2.3.tar", last modified: Fri May  5 14:14:19 2023, max compression
```

## Comparing `personio-py-0.2.2.tar` & `personio-py-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 14:13:34.000000 personio-py-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)    10792 2022-07-04 14:13:34.000000 personio-py-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8612 2022-07-04 14:13:25.000000 personio-py-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-04 14:13:34.000000 personio-py-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3338 2022-07-04 14:13:25.000000 personio-py-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 14:13:34.000000 personio-py-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 14:13:34.000000 personio-py-0.2.2/src/personio_py/
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-07-04 14:13:25.000000 personio-py-0.2.2/src/personio_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24357 2022-07-04 14:13:25.000000 personio-py-0.2.2/src/personio_py/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-07-04 14:13:25.000000 personio-py-0.2.2/src/personio_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     8128 2022-07-04 14:13:25.000000 personio-py-0.2.2/src/personio_py/mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)    31683 2022-07-04 14:13:25.000000 personio-py-0.2.2/src/personio_py/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     7418 2022-07-04 14:13:25.000000 personio-py-0.2.2/src/personio_py/search.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-04 14:13:25.000000 personio-py-0.2.2/src/personio_py/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-04 14:13:34.000000 personio-py-0.2.2/src/personio_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10792 2022-07-04 14:13:34.000000 personio-py-0.2.2/src/personio_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-07-04 14:13:34.000000 personio-py-0.2.2/src/personio_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-04 14:13:34.000000 personio-py-0.2.2/src/personio_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-07-04 14:13:34.000000 personio-py-0.2.2/src/personio_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-04 14:13:34.000000 personio-py-0.2.2/src/personio_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:14:19.000000 personio-py-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-05-05 14:14:19.000000 personio-py-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-05-05 14:14:05.000000 personio-py-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:14:19.000000 personio-py-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-05 14:14:05.000000 personio-py-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:14:19.000000 personio-py-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:14:19.000000 personio-py-0.2.3/src/personio_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-05 14:14:05.000000 personio-py-0.2.3/src/personio_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-05-05 14:14:05.000000 personio-py-0.2.3/src/personio_py/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-05 14:14:05.000000 personio-py-0.2.3/src/personio_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-05 14:14:05.000000 personio-py-0.2.3/src/personio_py/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35025 2023-05-05 14:14:05.000000 personio-py-0.2.3/src/personio_py/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-05 14:14:05.000000 personio-py-0.2.3/src/personio_py/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 14:14:05.000000 personio-py-0.2.3/src/personio_py/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:14:19.000000 personio-py-0.2.3/src/personio_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-05-05 14:14:18.000000 personio-py-0.2.3/src/personio_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-05 14:14:18.000000 personio-py-0.2.3/src/personio_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:14:18.000000 personio-py-0.2.3/src/personio_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 14:14:18.000000 personio-py-0.2.3/src/personio_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 14:14:18.000000 personio-py-0.2.3/src/personio_py.egg-info/top_level.txt
```

### Comparing `personio-py-0.2.2/PKG-INFO` & `personio-py-0.2.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,156 +1,161 @@
-Metadata-Version: 2.1
-Name: personio-py
-Version: 0.2.2
-Summary: a lightweight Personio API client
-Home-page: https://github.com/at-gmbh/personio-py
-Author: Sebastian Straub
-Author-email: sebastian.straub@alexanderthamm.com
-License: Apache 2.0
-Project-URL: Documentation, https://at-gmbh.github.io/personio-py/
-Project-URL: Source, https://github.com/at-gmbh/personio-py
-Project-URL: Tracker, https://github.com/at-gmbh/personio-py/issues
-Description: # personio-py
-        
-        [![build](https://github.com/at-gmbh/personio-py/workflows/build/badge.svg?branch=master&event=push)](https://github.com/at-gmbh/personio-py/actions?query=workflow%3Abuild)
-        [![PyPI](https://img.shields.io/pypi/v/personio-py)](https://pypi.org/project/personio-py/)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/personio-py)](https://pypi.org/project/personio-py/)
-        [![documentation](https://img.shields.io/badge/docs-latest-informational)](https://at-gmbh.github.io/personio-py/)
-        [![Codecov](https://img.shields.io/codecov/c/github/at-gmbh/personio-py)](https://codecov.io/gh/at-gmbh/personio-py)
-        [![#personio-py:matrix.org](https://img.shields.io/matrix/personio-py:matrix.org)](https://matrix.to/#/#personio-py:matrix.org)
-        [![PyPI - License](https://img.shields.io/pypi/l/personio-py)](https://github.com/at-gmbh/personio-py/blob/master/LICENSE)
-        
-        **personio-py** is a lightweight [Personio](https://www.personio.de/) API client library for Python. Also, it's pretty intuitive to use. But don't take my word for it, please have a look:
-        
-        ```python
-        >>> from personio_py import Personio
-        >>> p = Personio(client_id='***', client_secret='***')
-        >>> ada = p.search_first("Ada")
-        >>> ada.last_name
-        'Lovelace'
-        >>> absences = p.get_absences(ada)
-        >>> len(absences)
-        12
-        >>> absences[0].to_dict()
-        {'id': 42, 'status': 'approved', 'start_date': '2020-08-01', 'end_date': '2020-08-16', ...}
-        ```
-        
-        **personio-py** aims to provide Python function wrappers and object mappings for all endpoints of the [Personio REST API](https://developer.personio.de/reference). Because personio-py is a third party library, and the REST API may change from time to time, we cannot guarantee that all functions are covered, but we try our best.
-        
-        If something appears to be broken, please have a look at the [open issues](https://github.com/at-gmbh/personio-py/issues) and vote for an existing issue or create a new one, if you can't find an issue that describes your problem.
-        
-        **📖 Documentation is available at [at-gmbh.github.io/personio-py](https://at-gmbh.github.io/personio-py/)**
-        
-        ## Features
-        
-        * Aims to cover all functions of the Personio API (work in progress)
-        * Python function wrappers for all API endpoints as part of the Personio class
-        * Object mappings for all API resources, e.g. an Employee is an object with properties for all the information that is provided by the REST API.
-        * Completely transparent handling of authentication and key rotation
-        * Support for Type Hints
-        * Only one dependency: [requests](https://pypi.org/project/requests/)
-        
-        ## Getting Started
-        
-        The package is available on [PyPI](https://pypi.org/project/personio-py/) and can be installed with
-        
-            pip install personio-py
-        
-        Now you can `import personio_py` and start coding. Please have a look at the [User Guide](https://at-gmbh.github.io/personio-py/guide.html) and the [Examples](https://at-gmbh.github.io/personio-py/examples.html) section for more details.
-        
-        ## Contributing
-        
-        Contributions are very welcome! For our contribution guidelines, please have a look at [CONTRIBUTING.md](./CONTRIBUTING.md).
-        
-        To set up your local development environment, please use a fresh virtual environment, then run
-        
-            pip install -r requirements.txt -r requirements-dev.txt
-        
-        This project is intended to be used as library, so there is no command line interface or stuff like that.
-        
-        We use `pytest` as test framework. To execute the tests, please run
-        
-            python setup.py test
-        
-        To build a distribution package (wheel), please use
-        
-            python setup.py dist
-        
-        this will clean up the build folder and then run the `bdist_wheel` command.
-        
-        Before contributing code, please set up the pre-commit hooks to reduce errors and ensure consistency
-        
-            pip install -U pre-commit && pre-commit install
-        
-        ### PyPI Release
-        
-        This project is released on [PyPI](https://pypi.org/project/personio-py/). Most of the tedious steps that are required to test & publish your release are automated by [CI pipelines](https://github.com/at-gmbh/personio-py/actions). All you have to do is to write your code and when the time comes to make a release, please follow these steps:
-        
-        * update the program version in [`src/personio_py/version.py`](./src/personio_py/version.py)
-        * write a summary of your changes in [`CHANGELOG.md`](./CHANGELOG.md)
-        * add a tag on the master branch with the new version number preceded by the letter `v`, e.g. for version 1.0.0 the tag would be `v1.0.0`. To tag the head of the current branch, use `git tag v1.0.0`
-        * push your changes to github and don't forget to push the tag with `git push origin v1.0.0`
-        * now have a look at the [release pipeline](https://github.com/at-gmbh/personio-py/actions?query=workflow%3Arelease) on GitHub. If it finishes without errors, you can find your release on [TestPyPI](https://test.pypi.org/project/personio-py). Please verify that your release works as expected.
-        * Now for the live deployment on PyPI. To avoid mistakes, this is only triggered, when a release is published on GitHub first. Please have a look at the [Releases](https://github.com/at-gmbh/personio-py/releases) now; there should be a draft release with your version number (this was created by the CI pipeline which also made the TestPyPI release). Edit the draft release, copy the text you added to [`CHANGELOG.md`](./CHANGELOG.md) into the description field and publish it.
-        * After you publish the release, the [deploy pipeline](https://github.com/at-gmbh/personio-py/actions?query=workflow%3Adeploy) is triggered on GitHub. It will publish the release directly to [PyPI](https://pypi.org/project/personio-py/) where everyone can enjoy your latest features.
-        
-        ## API Functions
-        
-        Available
-        
-        * [`POST /auth`](https://developer.personio.de/reference#auth): fully transparent authentication handling
-        * [`GET /company/employees`](https://developer.personio.de/reference#get_company-employees): list all employees
-        * [`GET /company/employees/{id}`](https://developer.personio.de/reference#get_company-employees-employee-id): get the employee with the specified ID
-        * [`GET /company/employees/{id}/profile-picture/{width}`](https://developer.personio.de/reference#get_company-employees-employee-id-profile-picture-width): get the profile picture of the specified employee
-        * [`GET /company/attendances`](https://developer.personio.de/reference#get_company-attendances): fetch attendance data for the company employees
-        * [`GET /company/time-off-types`](https://developer.personio.de/reference#get_company-time-off-types): get a list of available absences types
-        * [`GET /company/time-offs`](https://developer.personio.de/reference#get_company-time-offs): fetch absence data for the company employees
-        * [`POST /company/time-offs`](https://developer.personio.de/reference#post_company-time-offs): add absence data for the company employees
-        * [`GET /company/time-offs/{id}`](https://developer.personio.de/reference#get_company-time-offs-id): get the absence entry with the specified ID
-        * [`DELETE /company/time-offs/{id}`](https://developer.personio.de/reference#delete_company-time-offs-id): delete the absence entry with the specified ID
-        
-        Work in Progress
-        
-        * [`POST /company/employees`](https://developer.personio.de/reference#post_company-employees): create a new employee
-        * [`PATCH /company/employees/{id}`](https://developer.personio.de/reference#patch_company-employees-employee-id): update an existing employee entry
-        * [`POST /company/attendances`](https://developer.personio.de/reference#post_company-attendances): add attendance data for the company employees
-        * [`DELETE /company/attendances/{id}`](https://developer.personio.de/reference#delete_company-attendances-id): delete the attendance entry with the specified ID
-        * [`PATCH /company/attendances/{id}`](https://developer.personio.de/reference#patch_company-attendances-id): update the attendance entry with the specified ID
-        
-        ## Contact
-        
-        Sebastian Straub (sebastian.straub [at] alexanderthamm.com)
-        
-        Developed with ❤ at [Alexander Thamm GmbH](https://www.alexanderthamm.com/)
-        
-        ## License
-        
-            Copyright 2020 Alexander Thamm GmbH
-        
-            Licensed under the Apache License, Version 2.0 (the "License");
-            you may not use this file except in compliance with the License.
-            You may obtain a copy of the License at
-        
-                http://www.apache.org/licenses/LICENSE-2.0
-        
-            Unless required by applicable law or agreed to in writing, software
-            distributed under the License is distributed on an "AS IS" BASIS,
-            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-            See the License for the specific language governing permissions and
-            limitations under the License.
-        
-Platform: any
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Office/Business
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+# personio-py
+
+[![build](https://github.com/at-gmbh/personio-py/workflows/build/badge.svg?branch=master&event=push)](https://github.com/at-gmbh/personio-py/actions?query=workflow%3Abuild)
+[![PyPI](https://img.shields.io/pypi/v/personio-py)](https://pypi.org/project/personio-py/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/personio-py)](https://pypi.org/project/personio-py/)
+[![documentation](https://img.shields.io/badge/docs-latest-informational)](https://at-gmbh.github.io/personio-py/)
+[![Codecov](https://img.shields.io/codecov/c/github/at-gmbh/personio-py)](https://codecov.io/gh/at-gmbh/personio-py)
+[![#personio-py:matrix.org](https://img.shields.io/matrix/personio-py:matrix.org)](https://matrix.to/#/#personio-py:matrix.org)
+[![PyPI - License](https://img.shields.io/pypi/l/personio-py)](https://github.com/at-gmbh/personio-py/blob/master/LICENSE)
+
+**personio-py** is a lightweight [Personio](https://www.personio.de/) API client library for Python. Also, it's pretty intuitive to use. But don't take my word for it, please have a look:
+
+```python
+>>> from personio_py import Personio
+>>> p = Personio(client_id='***', client_secret='***')
+>>> ada = p.search_first("Ada")
+>>> ada.last_name
+'Lovelace'
+>>> absences = p.get_absences(ada)
+>>> len(absences)
+12
+>>> absences[0].to_dict()
+{'id': 42, 'status': 'approved', 'start_date': '2020-08-01', 'end_date': '2020-08-16', ...}
+```
+
+**personio-py** aims to provide Python function wrappers and object mappings for all endpoints of the [Personio REST API](https://developer.personio.de/reference). Because personio-py is a third party library, and the REST API may change from time to time, we cannot guarantee that all functions are covered, but we try our best.
+
+If something appears to be broken, please have a look at the [open issues](https://github.com/at-gmbh/personio-py/issues) and vote for an existing issue or create a new one, if you can't find an issue that describes your problem.
+
+**📖 Documentation is available at [at-gmbh.github.io/personio-py](https://at-gmbh.github.io/personio-py/)**
+
+## Features
+
+* Aims to cover all functions of the Personio API (work in progress)
+* Python function wrappers for all API endpoints as part of the Personio class
+* Object mappings for all API resources, e.g. an Employee is an object with properties for all the information that is provided by the REST API.
+* Completely transparent handling of authentication and key rotation
+* Support for Type Hints
+* Only one dependency: [requests](https://pypi.org/project/requests/)
+
+## Getting Started
+
+The package is available on [PyPI](https://pypi.org/project/personio-py/) and can be installed with
+
+    pip install personio-py
+
+Now you can `import personio_py` and start coding. Please have a look at the [User Guide](https://at-gmbh.github.io/personio-py/guide.html) and the [Examples](https://at-gmbh.github.io/personio-py/examples.html) section for more details.
+
+## Contributing
+
+Contributions are very welcome! For our contribution guidelines, please have a look at [CONTRIBUTING.md](./CONTRIBUTING.md).
+
+To set up your local development environment, please use a fresh virtual environment, then run
+
+    pip install -r requirements.txt -r requirements-dev.txt
+
+This project is intended to be used as library, so there is no command line interface or stuff like that.
+
+We use `pytest` as test framework. To execute the tests, please run
+
+    python setup.py test
+
+To build a distribution package (wheel), please use
+
+    python setup.py dist
+
+this will clean up the build folder and then run the `bdist_wheel` command.
+
+Before contributing code, please set up the pre-commit hooks to reduce errors and ensure consistency
+
+    pip install -U pre-commit && pre-commit install
+
+### PyPI Release
+
+This project is released on [PyPI](https://pypi.org/project/personio-py/). Most of the tedious steps that are required to test & publish your release are automated by [CI pipelines](https://github.com/at-gmbh/personio-py/actions). All you have to do is to write your code and when the time comes to make a release, please follow these steps:
+
+* update the program version in [`src/personio_py/version.py`](./src/personio_py/version.py)
+* write a summary of your changes in [`CHANGELOG.md`](./CHANGELOG.md)
+* add a tag on the master branch with the new version number preceded by the letter `v`, e.g. for version 1.0.0 the tag would be `v1.0.0`. To tag the head of the current branch, use `git tag v1.0.0`
+* push your changes to github and don't forget to push the tag with `git push origin v1.0.0`
+* now have a look at the [release pipeline](https://github.com/at-gmbh/personio-py/actions?query=workflow%3Arelease) on GitHub. If it finishes without errors, you can find your release on [TestPyPI](https://test.pypi.org/project/personio-py). Please verify that your release works as expected.
+* Now for the live deployment on PyPI. To avoid mistakes, this is only triggered, when a release is published on GitHub first. Please have a look at the [Releases](https://github.com/at-gmbh/personio-py/releases) now; there should be a draft release with your version number (this was created by the CI pipeline which also made the TestPyPI release). Edit the draft release, copy the text you added to [`CHANGELOG.md`](./CHANGELOG.md) into the description field and publish it.
+* After you publish the release, the [deploy pipeline](https://github.com/at-gmbh/personio-py/actions?query=workflow%3Adeploy) is triggered on GitHub. It will publish the release directly to [PyPI](https://pypi.org/project/personio-py/) where everyone can enjoy your latest features.
+
+## API Functions
+
+Since the [Personio API](https://developer.personio.de/reference/introduction) gets extended over time, personio-py usually only implements a subset of all available API features. This section gives an overview, which API functions are accessible through personio-py.
+
+### Available
+
+Authentication
+
+* [`POST /auth`](https://developer.personio.de/reference/post_auth-1): fully transparent authentication handling
+
+Employees
+
+* [`GET /company/employees`](https://developer.personio.de/reference/get_company-employees): list all employees
+* [`POST /company/employees`](https://developer.personio.de/reference/post_company-employees): create a new employee
+* [`GET /company/employees/{id}`](https://developer.personio.de/reference/get_company-employees-employee-id): get the employee with the specified ID
+* [`GET /company/employees/{id}/profile-picture/{width}`](https://developer.personio.de/reference/get_company-employees-employee-id-profile-picture-width): get the profile picture of the specified employee
+
+Attendances
+
+* [`GET /company/attendances`](https://developer.personio.de/reference/get_company-attendances): fetch attendance data for the company employees
+* [`POST /company/attendances`](https://developer.personio.de/reference/post_company-attendances): add attendance data for the company employees
+* [`DELETE /company/attendances/{id}`](https://developer.personio.de/reference/delete_company-attendances-id): delete the attendance entry with the specified ID
+* [`PATCH /company/attendances/{id}`](https://developer.personio.de/reference/patch_company-attendances-id): update the attendance entry with the specified ID
+
+Projects
+
+* [`GET /company/attendances/projects`](https://developer.personio.de/reference/get_company-attendances-projects): provides a list of all company projects
+* [`POST /company/attendances/projects`](https://developer.personio.de/reference/post_company-attendances-projects): creates a project into the company account
+* [`DELETE /company/attendances/projects/{id}`](https://developer.personio.de/reference/delete_company-attendances-projects-id): deletes a project from the company account
+* [`PATCH /company/attendances/projects/{id}`](https://developer.personio.de/reference/patch_company-attendances-projects-id): updates a project with the given data
+
+Absences
+
+* [`GET /company/time-off-types`](https://developer.personio.de/reference/get_company-time-off-types): get a list of available absences types
+* [`GET /company/time-offs`](https://developer.personio.de/reference/get_company-time-offs): fetch absence data for the company employees
+* [`POST /company/time-offs`](https://developer.personio.de/reference/post_company-time-offs): add absence data for the company employees
+* [`GET /company/time-offs/{id}`](https://developer.personio.de/reference/get_company-time-offs-id): get the absence entry with the specified ID
+* [`DELETE /company/time-offs/{id}`](https://developer.personio.de/reference/delete_company-time-offs-id): delete the absence entry with the specified ID
+
+### Not yet implemented
+
+* [`PATCH /company/employees/{id}`](https://developer.personio.de/reference/patch_company-employees-employee-id): update an existing employee entry
+* [`GET /company/employees/{employee_id}/absences/balance`](https://developer.personio.de/reference/get_company-employees-employee-id-absences-balance): retrieve the absence balance for a specific employee
+* [`GET /company/employees/custom-attributes`](https://developer.personio.de/reference/get_company-employees-custom-attributes): this endpoint is an alias for /company/employees/attributes
+* [`GET /company/employees/attributes`](https://developer.personio.de/reference/get_company-employees-attributes): lists all the allowed attributes per API credentials including custom (dynamic) attributes.
+* [`GET /company/absence-periods`](https://developer.personio.de/reference/get_company-absence-periods)
+* [`POST /company/absence-periods`](https://developer.personio.de/reference/post_company-absence-periods)
+* [`DELETE /company/absence-periods/{id}`](https://developer.personio.de/reference/delete_company-absence-periods-id)
+
+* [`GET /company/document-categories`](https://developer.personio.de/reference/get_company-document-categories): this endpoint is responsible for fetching all document categories of the company
+* [`POST /company/documents`](https://developer.personio.de/reference/post_company-documents): this endpoint is responsible for uploading documents for the company employees
+* [`GET /company/custom-reports/reports`](https://developer.personio.de/reference/listreports): this endpoint provides you with metadata about existing custom reports in your Personio account, such as report name, report type, report date / timeframe
+* [`GET /company/custom-reports/reports/{report_id}`](https://developer.personio.de/reference/listreportitems): this endpoint provides you with the data of an existing Custom Report
+* [`GET /company/custom-reports/columns`](https://developer.personio.de/reference/listcolumns): this endpoint provides human-readable labels for report table columns
+* all of the [recruiting API](https://developer.personio.de/reference/introduction-1)
+
+## Contact
+
+Sebastian Straub (sebastian.straub [at] alexanderthamm.com)
+
+Developed with ❤ at [Alexander Thamm GmbH](https://www.alexanderthamm.com/)
+
+## License
+
+    Copyright 2020 Alexander Thamm GmbH
+
+    Licensed under the Apache License, Version 2.0 (the "License");
+    you may not use this file except in compliance with the License.
+    You may obtain a copy of the License at
+
+        http://www.apache.org/licenses/LICENSE-2.0
+
+    Unless required by applicable law or agreed to in writing, software
+    distributed under the License is distributed on an "AS IS" BASIS,
+    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+    See the License for the specific language governing permissions and
+    limitations under the License.
```

### Comparing `personio-py-0.2.2/setup.py` & `personio-py-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # read the program version from version.py (without loading the module)
 __version__ = run_path('src/personio_py/version.py')['__version__']
 
 
 def read(fname):
     """Utility function to read the README file."""
-    return open(os.path.join(os.path.dirname(__file__), fname), 'r', encoding='utf-8').read()
+    return open(os.path.join(os.path.dirname(__file__), fname), encoding='utf-8').read()
 
 
 class DistCommand(Command):
 
     description = "build the distribution packages (in the 'dist' folder)"
     user_options = []
```

### Comparing `personio-py-0.2.2/src/personio_py/__init__.py` & `personio-py-0.2.3/src/personio_py/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,9 +27,10 @@
     DynamicAttr,
     Employee,
     HolidayCalendar,
     Office,
     ShortEmployee,
     Team,
     WorkSchedule,
+    Project
 )
 from personio_py.client import Personio
```

### Comparing `personio-py-0.2.2/src/personio_py/client.py` & `personio-py-0.2.3/src/personio_py/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union
 from urllib.parse import urljoin
 
 import requests
 from requests import Response
 
-from personio_py import Absence, AbsenceType, Attendance, DynamicMapping, Employee
+from personio_py import Absence, AbsenceType, Attendance, DynamicMapping, Employee, Project
 from personio_py.errors import MissingCredentialsError, PersonioApiError, PersonioError
 from personio_py.models import PersonioResource
 from personio_py.search import SearchIndex
 
 logger = logging.getLogger('personio_py')
 
 PersonioResourceType = TypeVar('PersonioResourceType', bound=PersonioResource, covariant=True)
@@ -31,14 +31,17 @@
            (if not provided, defaults to the ``CLIENT_SECRET`` environment variable)
     :param dynamic_fields: definition of expected dynamic fields.
            List of :py:class:`DynamicMapping` tuples.
     """
 
     BASE_URL = "https://api.personio.de/v1/"
     """base URL of the Personio HTTP API"""
+    ATTENDANCE_URL = 'company/attendances'
+    ABSENCE_URL = 'company/time-offs'
+    PROJECT_URL = 'company/attendances/projects'
 
     def __init__(self, base_url: str = None, client_id: str = None, client_secret: str = None,
                  dynamic_fields: List[DynamicMapping] = None):
         self.base_url = base_url or self.BASE_URL
         self.client_id = client_id or os.getenv('CLIENT_ID')
         self.client_secret = client_secret or os.getenv('CLIENT_SECRET')
         self.headers = {'accept': 'application/json'}
@@ -134,17 +137,17 @@
             try:
                 return response.json()
             except ValueError:
                 raise PersonioError(f"Failed to parse response as json: {response.text}")
         else:
             raise PersonioApiError.from_response(response)
 
-    def request_paginated(
-            self, path: str, method='GET', params: Dict[str, Any] = None,
-            data: Dict[str, Any] = None, auth_rotation=True, limit=200) -> Dict[str, Any]:
+    def request_paginated(self, path: str, method='GET', params: Dict[str, Any] = None,
+                          data: Dict[str, Any] = None, auth_rotation=True, limit=200
+                          ) -> Dict[str, Any]:
         """
         Make a request against the Personio API, expecting a json response that may be paginated,
         i.e. not all results might have been returned after the first request. Will continue
         to make requests until no more results are provided by the Personio API.
         Returns the parsed json response as dictionary. Will raise a PersonioApiError if the
         request fails.
 
@@ -155,30 +158,44 @@
         :param auth_rotation: set to True, if authentication keys should be rotated
                during this request (default: True for json requests)
         :param limit: the max. number of items to return in response to a single request.
                A higher limit means fewer requests will be made (though there is an upper bound
                that is enforced on the server side)
         :return: the parsed json response, when the request was successful, or a PersonioApiError
         """
-        # prepare the params dict (need limit and offset as parameters)
+        if self.ABSENCE_URL == path:
+            offset = 1
+            url_type = 'absence'
+        elif self.ATTENDANCE_URL == path:
+            offset = 0
+            url_type = 'attendance'
+        else:
+            raise ValueError(f"Invalid path: {path}")
+
         if params is None:
             params = {}
         params['limit'] = limit
-        params['offset'] = 1
-        # continue making requests until no more data is returned
+        params['offset'] = offset
         data_acc = []
         while True:
             response = self.request_json(path, method, params, data, auth_rotation=auth_rotation)
-            resp_data = response['data']
+            resp_data = response.get('data')
             if resp_data:
-                data_acc.extend(resp_data)
-                if response['metadata']['current_page'] == response['metadata']['total_pages']:
-                    break
-                else:
-                    params['offset'] += 1
+                if url_type == 'absence':
+                    data_acc.extend(resp_data)
+                    if response['metadata']['current_page'] == response['metadata']['total_pages']:
+                        break
+                    else:
+                        params['offset'] += 1
+                elif url_type == 'attendance':
+                    if params['offset'] >= response['metadata']['total_elements']:
+                        break
+                    else:
+                        data_acc.extend(resp_data)
+                        params['offset'] += limit
             else:
                 break
         # return the accumulated data
         response['data'] = data_acc
         return response
 
     def request_image(self, path: str, method='GET', params: Dict[str, Any] = None,
@@ -207,24 +224,26 @@
         else:
             # oh noes, something went terribly wrong!
             raise PersonioApiError.from_response(response)
 
     def get_employees(self) -> List[Employee]:
         """
         Get a list of all employee records in your account.
+        Does not involve pagination.
 
         :return: list of ``Employee`` instances
         """
         response = self.request_json('company/employees')
         employees = [Employee.from_dict(d, self) for d in response['data']]
         return employees
 
     def get_employee(self, employee_id: int) -> Employee:
         """
         Get a single employee with the specified ID.
+        Does not involve pagination.
 
         :param employee_id: the Personio ID of the employee to fetch
         :return: an ``Employee`` instance or a PersonioApiError, if the employee does not exist
         """
         response = self.request_json(f'company/employees/{employee_id}')
         employee = Employee.from_dict(response['data'], self)
         return employee
@@ -271,68 +290,127 @@
 
     def update_employee(self, employee: Employee):
         """
         placeholder; not ready to be used
         """
         raise NotImplementedError()
 
-    def get_attendances(self, employees: Union[int, List[int], Employee, List[Employee]],
-                        start_date: datetime = None, end_date: datetime = None) -> List[Attendance]:
+    def get_attendances(
+            self, employees: Union[int, List[int], Employee, List[Employee]],
+            start_date: datetime = None, end_date: datetime = None) -> List[Attendance]:
         """
         Get a list of all attendance records for the employees with the specified IDs
 
         Note that internally, multiple requests may be made by this function due to limitations
         of the Personio API: Only a limited number of records can be retrieved in a single request
         and only a limited number of employee IDs can be passed as URL parameters. The results
         are still presented as a single list, no matter how many requests are made.
 
         :param employees: a single employee or a list of employee objects or IDs.
                Attendance records for all matching employees will be retrieved.
         :param start_date: only return attendance records from this date (inclusive, optional)
         :param end_date: only return attendance records up to this date (inclusive, optional)
         :return: list of ``Attendance`` records for the specified employees
         """
-        return self._get_employee_metadata(
-            'company/attendances', Attendance, employees, start_date, end_date)
-
-    def create_attendances(self, attendances: List[Attendance]):
-        """
-        placeholder; not ready to be used
-        """
-        # attendances can be created individually, but here you can push a huge bunch of items
-        # in a single request, which can be significantly faster
-        raise NotImplementedError()
+        attendances = self._get_employee_metadata(
+            self.ATTENDANCE_URL, Attendance, employees, start_date, end_date)
+        for attendance in attendances:
+            attendance._client = self
+        return attendances
+
+    def create_attendances(self, attendances: List[Attendance]) -> bool:
+        """
+        Create all given attendance records.
+
+        Note: If one or more attendances can not be created, other attendances will be created but
+        their corresponding objects passed as attendances will not be updated.
+
+        :param attendances: A list of attendance records to be created.
+        """
+        data_to_send = [
+            attendance.to_body_params(patch_existing_attendance=False) for attendance in attendances
+        ]
+        response = self.request_json(
+            path=self.ATTENDANCE_URL,
+            method='POST',
+            data={"attendances": data_to_send}
+        )
+        if response['success']:
+            for attendance, response_id in zip(attendances, response['data']['id']):
+                attendance.id_ = response_id
+                attendance.client = self
+            return True
+        return False
+
+    def update_attendance(self, attendance: Attendance):
+        """
+        Update an existing attendance record
+
+        Either an attendance id or o remote query is required. Remote queries are only executed
+        if required. An Attendance object returned by get_attendances() include the attendance id.
+        DO NOT SET THE ID YOURSELF.
+
+        :param attendance: The Attendance object holding the new data.
+        :raises:
+            ValueError: If a query is required but not allowed or the query does not provide
+            exactly one result.
+        """
+        if attendance.id_ is not None:
+            # remote query not necessary
+            response = self.request_json(
+                path=f'{self.ATTENDANCE_URL}/{attendance.id_}',
+                method='PATCH',
+                data=attendance.to_body_params(patch_existing_attendance=True)
+            )
+            return response
+        else:
+            raise ValueError("You need to provide the attendance id")
 
-    def update_attendance(self, attendance_id: int):
-        """
-        placeholder; not ready to be used
+    def delete_attendance(self, attendance: Attendance or int):
         """
-        raise NotImplementedError()
+        Delete an existing record
 
-    def delete_attendance(self, attendance_id: int):
-        """
-        placeholder; not ready to be used
-        """
-        raise NotImplementedError()
+        Either an attendance id or o remote query is required. Remote queries are only
+        executed if required. An Attendance object returned by get_attendances() include the
+        attendance id. DO NOT SET THE ID YOURSELF.
+
+        :param attendance: The Attendance object holding the new data or an attendance record id to
+            delete.
+        :raises:
+            ValueError: If a query is required but not allowed or the query does not provide
+            exactly one result.
+        """
+        if isinstance(attendance, int):
+            response = self.request_json(path=f'{self.ATTENDANCE_URL}/{attendance}',
+                                         method='DELETE')
+            return response
+        elif isinstance(attendance, Attendance):
+            if attendance.id_ is not None:
+                return self.delete_attendance(attendance.id_)
+            else:
+                raise ValueError("You need to provide the attendance")
+        else:
+            raise ValueError("attendance must be an Attendance object or an integer")
 
     def get_absence_types(self) -> List[AbsenceType]:
         """
         Get a list of all available absence types, e.g. "paid vacation" or "parental leave".
 
         The absence types are used to classify the absences of employees
         (see ``get_absences`` to get a list of all absences for the employees).
         Each ``Absence`` also contains the ``AbsenceType`` for this instance; the purpose
         of this function is to provide you with a list of all possible options that can show up.
         """
         response = self.request_json('company/time-off-types')
         absence_types = [AbsenceType.from_dict(d, self) for d in response['data']]
         return absence_types
 
-    def get_absences(self, employees: Union[int, List[int], Employee, List[Employee]],
-                     start_date: datetime = None, end_date: datetime = None) -> List[Absence]:
+    def get_absences(
+            self, employees: Union[int, List[int], Employee, List[Employee]],
+            start_date: datetime = None, end_date: datetime = None) -> List[Absence]:
         """
         Get a list of all absence records for the employees with the specified IDs.
 
         Note that internally, multiple requests may be made by this function due to limitations
         of the Personio API: Only a limited number of records can be retrieved in a single request
         and only a limited number of employee IDs can be passed as URL parameters. The results
         are still presented as a single list, no matter how many requests are made.
@@ -340,24 +418,24 @@
         :param employees: a single employee or a list of employee objects or IDs.
                Absence records for all matching employees will be retrieved.
         :param start_date: only return absence records from this date (inclusive, optional)
         :param end_date: only return absence records up to this date (inclusive, optional)
         :return: list of ``Absence`` records for the specified employees
         """
         return self._get_employee_metadata(
-            'company/time-offs', Absence, employees, start_date, end_date)
+            self.ABSENCE_URL, Absence, employees, start_date, end_date)
 
     def get_absence(self, absence: Union[Absence, int]) -> Absence:
         """
         Get an absence record from a given id.
 
         :param absence: The absence id to fetch.
         """
         if isinstance(absence, int):
-            response = self.request_json(f'company/time-offs/{absence}')
+            response = self.request_json(f'{self.ABSENCE_URL}/{absence}')
             return Absence.from_dict(response['data'], self)
         else:
             if absence.id_:
                 return self.get_absence(absence.id_)
             else:
                 self.__add_remote_absence_id(absence)
                 return self.get_absence(absence.id_)
@@ -366,33 +444,33 @@
         """
         Creates an absence record on the Personio servers
 
         :param absence: The absence object to be created
         :raises PersonioError: If the absence could not be created on the Personio servers
         """
         data = absence.to_body_params()
-        response = self.request_json('company/time-offs', method='POST', data=data)
+        response = self.request_json(self.ABSENCE_URL, method='POST', data=data)
         if response['success']:
             absence.id_ = response['data']['attributes']['id']
             return absence
         raise PersonioError("Could not create absence")
 
     def delete_absence(self, absence: Union[Absence, int]):
         """
         Delete an existing record
 
         An absence id is required.
 
         :param absence: The Absence object holding
-            the new data or an absence record id to delete.
+               the new data or an absence record id to delete.
         :raises ValueError: If a query is required but not allowed
-            or the query does not provide exactly one result.
+                or the query does not provide exactly one result.
         """
         if isinstance(absence, int):
-            response = self.request_json(path=f'company/time-offs/{absence}', method='DELETE')
+            response = self.request_json(path=f'{self.ABSENCE_URL}/{absence}', method='DELETE')
             return response['success']
         elif isinstance(absence, Absence):
             if absence.id_ is not None:
                 return self.delete_absence(absence.id_)
             else:
                 raise ValueError("Only an absence with an absence id can be deleted.")
         else:
@@ -433,14 +511,70 @@
 
     def invalidate_index(self):
         """
         Invalidates the search index. New data will be requested on the next search.
         """
         self.search_index.invalidate()
 
+    def get_projects(self) -> List[Project]:
+        """
+        Get a list of all company projects.
+
+        :return: list of ``Project`` records
+        """
+        response = self.request_json(self.PROJECT_URL)
+        projects = [Project.from_dict(d, self) for d in response['data']]
+        return projects
+
+    def create_project(self, project: Project) -> Project:
+        """
+        Creates a project record on the Personio servers.
+
+        :param project: The project object to be created
+        :raises PersonioError: If the project could not be created on the Personio servers
+        """
+        data = project.to_body_params()
+        response = self.request_json(self.PROJECT_URL, method='POST', data=data)
+        if response['success']:
+            project.id_ = response['data']['id']
+            return project
+        raise PersonioError("Could not create project")
+
+    def update_project(self, project: Project) -> Project:
+        """
+        Updates a project record on the Personio servers.
+
+        :param project: The project object to be updated
+        :raises PersonioErrror: If the project could not be created on the Personio servers
+        """
+        data = project.to_body_params()
+        response = self.request_json(f'{self.PROJECT_URL}/{project.id_}', method='PATCH', data=data)
+        if response['success']:
+            return project
+        raise PersonioError("Could not update project")
+
+    def delete_project(self, project: Union[Project, int]) -> None:
+        """
+        Deletes a project record on the Personio servers.
+
+        :param project: The project object to be updated
+        :raises ValueError: If a query is required but not allowed
+            or the query does not provide exactly one result.
+        """
+        if isinstance(project, int):
+            response = self.request(f'{self.PROJECT_URL}/{project}', method='DELETE')
+            return response
+        elif isinstance(project, Project):
+            if project.id_ is not None:
+                return self.delete_project(project.id_)
+            else:
+                raise ValueError("Only a project with a project id can be deleted.")
+        else:
+            raise ValueError("project must be a Project object or an integer")
+
     def _get_employee_metadata(
             self, path: str, resource_cls: Type[PersonioResourceType],
             employees: Union[int, List[int], Employee, List[Employee]], start_date: datetime = None,
             end_date: datetime = None) -> List[PersonioResourceType]:
         # resolve params to match API requirements
         employees, start_date, end_date = self._normalize_timeframe_params(
             employees, start_date, end_date)
```

### Comparing `personio-py-0.2.2/src/personio_py/errors.py` & `personio-py-0.2.3/src/personio_py/errors.py`

 * *Files identical despite different names*

### Comparing `personio-py-0.2.2/src/personio_py/mapping.py` & `personio-py-0.2.3/src/personio_py/mapping.py`

 * *Files identical despite different names*

### Comparing `personio-py-0.2.2/src/personio_py/models.py` & `personio-py-0.2.3/src/personio_py/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 import logging
 from collections import namedtuple
 from datetime import datetime, timedelta
 from functools import total_ordering
 from typing import Any, Dict, List, NamedTuple, Optional, TYPE_CHECKING, Tuple, Type, TypeVar
 
 from personio_py import PersonioError, UnsupportedMethodError
-from personio_py.mapping import BooleanFieldMapping, DateFieldMapping, DateTimeFieldMapping, \
-    DurationFieldMapping, DynamicMapping, FieldMapping, ListFieldMapping, NumericFieldMapping, \
+from personio_py.mapping import (
+    BooleanFieldMapping, DateFieldMapping, DateTimeFieldMapping,
+    DurationFieldMapping, DynamicMapping, FieldMapping, ListFieldMapping, NumericFieldMapping,
     ObjectFieldMapping
+)
 
 if TYPE_CHECKING:
     # only type checkers may import Personio, otherwise we get an evil circular import error
     from personio_py import Personio
 
 logger = logging.getLogger('personio_py')
 
@@ -617,14 +619,60 @@
             'half_day_end': self.half_day_end
         }
         if self.comment is not None:
             data['comment'] = self.comment
         return data
 
 
+class Project(WritablePersonioResource):
+
+    _api_type_name = "Project"
+    _field_mapping_list = [
+        # note: the id is actually not in the attributes dict, but one level higher
+        NumericFieldMapping('id', 'id_', int),
+        FieldMapping('name', 'name', str),
+        BooleanFieldMapping('active', 'active'),
+        DateTimeFieldMapping('created_at', 'created_at'),
+        DateTimeFieldMapping('updated_at', 'updated_at')
+    ]
+
+    def __init__(self, client: 'Personio' = None, dynamic: Dict[str, Any] = None,
+                 dynamic_raw: List['DynamicAttr'] = None, id_: int = None, name: str = None,
+                 active: bool = None, created_at: datetime = None, updated_at: datetime = None,
+                 **kwargs):
+        super().__init__(client=client, dynamic=dynamic, dynamic_raw=dynamic_raw, **kwargs)
+        self.id_ = id_
+        self.name = name
+        self.active = active
+        self.created_at = created_at
+        self.updated_at = updated_at
+
+    def _create(self, client: 'Personio' = None):
+        return get_client(self, client).create_project(self)
+
+    def _delete(self, client: 'Personio' = None):
+        return get_client(self, client).delete_project(self)
+
+    def _update(self, client: 'Personio' = None):
+        return get_client(self, client).update_project(self)
+
+    def to_dict(self, nested=False) -> Dict[str, Any]:
+        # yes, this is weird an unnecessary, but that's how the api works
+        d = super().to_dict()
+        d['id'] = self.id_
+        del d['attributes']['id']
+        return d
+
+    def to_body_params(self):
+        data = {
+            'name': self.name,
+            'active': self.active}
+        return data
+
+
 class Attendance(WritablePersonioResource):
 
     _api_type_name = "AttendancePeriod"
     _field_mapping_list = [
         # note: the id is actually not in the attributes dict, but one level higher
         NumericFieldMapping('id', 'id_', int),
         NumericFieldMapping('employee', 'employee_id', int),
@@ -666,21 +714,54 @@
         # yes, this is weird an unnecessary, but that's how the api works
         d = super().to_dict()
         d['id'] = self.id_
         del d['attributes']['id']
         return d
 
     def _create(self, client: 'Personio'):
-        pass
+        get_client(self, client).create_attendances([self])
 
     def _update(self, client: 'Personio'):
-        pass
+        get_client(self, client).update_attendance(self)
 
     def _delete(self, client: 'Personio'):
-        pass
+        get_client(self, client).delete_attendance(self)
+
+    def to_body_params(self, patch_existing_attendance=False):
+        """
+        Return the Attendance object in the representation expected by the Personio API
+
+        For an attendance record to be created all_values_required needs to be True.
+        For patch operations only the attendance id is required, but it is not
+        included into the body params.
+
+        :param patch_existing_attendance Get patch body. If False a create body is returned.
+        """
+        if patch_existing_attendance:
+            if self.id_ is None:
+                raise ValueError("An attendance id is required")
+            body_dict = {}
+            if self.date is not None:
+                body_dict['date'] = self.date.strftime("%Y-%m-%d")
+            if self.start_time is not None:
+                body_dict['start_time'] = str(self.start_time)
+            if self.end_time is not None:
+                body_dict['end_time'] = str(self.end_time)
+            if self.break_duration is not None:
+                body_dict['break'] = self.break_duration
+            if self.comment is not None:
+                body_dict['comment'] = self.comment
+            return body_dict
+        else:
+            return {"employee": self.employee_id,
+                    "date": self.date.strftime("%Y-%m-%d"),
+                    "start_time": self.start_time,
+                    "end_time": self.end_time,
+                    "break": self.break_duration or 0,
+                    "comment": self.comment or ""}
 
 
 class Employee(WritablePersonioResource, LabeledAttributesMixin):
 
     _api_type_name = "Employee"
     _can_delete = False
     _field_mapping_list = [
```

### Comparing `personio-py-0.2.2/src/personio_py/search.py` & `personio-py-0.2.3/src/personio_py/search.py`

 * *Files identical despite different names*

### Comparing `personio-py-0.2.2/src/personio_py.egg-info/PKG-INFO` & `personio-py-0.2.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personio-py
-Version: 0.2.2
+Version: 0.2.3
 Summary: a lightweight Personio API client
 Home-page: https://github.com/at-gmbh/personio-py
 Author: Sebastian Straub
 Author-email: sebastian.straub@alexanderthamm.com
 License: Apache 2.0
 Project-URL: Documentation, https://at-gmbh.github.io/personio-py/
 Project-URL: Source, https://github.com/at-gmbh/personio-py
@@ -91,34 +91,67 @@
         * push your changes to github and don't forget to push the tag with `git push origin v1.0.0`
         * now have a look at the [release pipeline](https://github.com/at-gmbh/personio-py/actions?query=workflow%3Arelease) on GitHub. If it finishes without errors, you can find your release on [TestPyPI](https://test.pypi.org/project/personio-py). Please verify that your release works as expected.
         * Now for the live deployment on PyPI. To avoid mistakes, this is only triggered, when a release is published on GitHub first. Please have a look at the [Releases](https://github.com/at-gmbh/personio-py/releases) now; there should be a draft release with your version number (this was created by the CI pipeline which also made the TestPyPI release). Edit the draft release, copy the text you added to [`CHANGELOG.md`](./CHANGELOG.md) into the description field and publish it.
         * After you publish the release, the [deploy pipeline](https://github.com/at-gmbh/personio-py/actions?query=workflow%3Adeploy) is triggered on GitHub. It will publish the release directly to [PyPI](https://pypi.org/project/personio-py/) where everyone can enjoy your latest features.
         
         ## API Functions
         
-        Available
+        Since the [Personio API](https://developer.personio.de/reference/introduction) gets extended over time, personio-py usually only implements a subset of all available API features. This section gives an overview, which API functions are accessible through personio-py.
         
-        * [`POST /auth`](https://developer.personio.de/reference#auth): fully transparent authentication handling
-        * [`GET /company/employees`](https://developer.personio.de/reference#get_company-employees): list all employees
-        * [`GET /company/employees/{id}`](https://developer.personio.de/reference#get_company-employees-employee-id): get the employee with the specified ID
-        * [`GET /company/employees/{id}/profile-picture/{width}`](https://developer.personio.de/reference#get_company-employees-employee-id-profile-picture-width): get the profile picture of the specified employee
-        * [`GET /company/attendances`](https://developer.personio.de/reference#get_company-attendances): fetch attendance data for the company employees
-        * [`GET /company/time-off-types`](https://developer.personio.de/reference#get_company-time-off-types): get a list of available absences types
-        * [`GET /company/time-offs`](https://developer.personio.de/reference#get_company-time-offs): fetch absence data for the company employees
-        * [`POST /company/time-offs`](https://developer.personio.de/reference#post_company-time-offs): add absence data for the company employees
-        * [`GET /company/time-offs/{id}`](https://developer.personio.de/reference#get_company-time-offs-id): get the absence entry with the specified ID
-        * [`DELETE /company/time-offs/{id}`](https://developer.personio.de/reference#delete_company-time-offs-id): delete the absence entry with the specified ID
-        
-        Work in Progress
-        
-        * [`POST /company/employees`](https://developer.personio.de/reference#post_company-employees): create a new employee
-        * [`PATCH /company/employees/{id}`](https://developer.personio.de/reference#patch_company-employees-employee-id): update an existing employee entry
-        * [`POST /company/attendances`](https://developer.personio.de/reference#post_company-attendances): add attendance data for the company employees
-        * [`DELETE /company/attendances/{id}`](https://developer.personio.de/reference#delete_company-attendances-id): delete the attendance entry with the specified ID
-        * [`PATCH /company/attendances/{id}`](https://developer.personio.de/reference#patch_company-attendances-id): update the attendance entry with the specified ID
+        ### Available
+        
+        Authentication
+        
+        * [`POST /auth`](https://developer.personio.de/reference/post_auth-1): fully transparent authentication handling
+        
+        Employees
+        
+        * [`GET /company/employees`](https://developer.personio.de/reference/get_company-employees): list all employees
+        * [`POST /company/employees`](https://developer.personio.de/reference/post_company-employees): create a new employee
+        * [`GET /company/employees/{id}`](https://developer.personio.de/reference/get_company-employees-employee-id): get the employee with the specified ID
+        * [`GET /company/employees/{id}/profile-picture/{width}`](https://developer.personio.de/reference/get_company-employees-employee-id-profile-picture-width): get the profile picture of the specified employee
+        
+        Attendances
+        
+        * [`GET /company/attendances`](https://developer.personio.de/reference/get_company-attendances): fetch attendance data for the company employees
+        * [`POST /company/attendances`](https://developer.personio.de/reference/post_company-attendances): add attendance data for the company employees
+        * [`DELETE /company/attendances/{id}`](https://developer.personio.de/reference/delete_company-attendances-id): delete the attendance entry with the specified ID
+        * [`PATCH /company/attendances/{id}`](https://developer.personio.de/reference/patch_company-attendances-id): update the attendance entry with the specified ID
+        
+        Projects
+        
+        * [`GET /company/attendances/projects`](https://developer.personio.de/reference/get_company-attendances-projects): provides a list of all company projects
+        * [`POST /company/attendances/projects`](https://developer.personio.de/reference/post_company-attendances-projects): creates a project into the company account
+        * [`DELETE /company/attendances/projects/{id}`](https://developer.personio.de/reference/delete_company-attendances-projects-id): deletes a project from the company account
+        * [`PATCH /company/attendances/projects/{id}`](https://developer.personio.de/reference/patch_company-attendances-projects-id): updates a project with the given data
+        
+        Absences
+        
+        * [`GET /company/time-off-types`](https://developer.personio.de/reference/get_company-time-off-types): get a list of available absences types
+        * [`GET /company/time-offs`](https://developer.personio.de/reference/get_company-time-offs): fetch absence data for the company employees
+        * [`POST /company/time-offs`](https://developer.personio.de/reference/post_company-time-offs): add absence data for the company employees
+        * [`GET /company/time-offs/{id}`](https://developer.personio.de/reference/get_company-time-offs-id): get the absence entry with the specified ID
+        * [`DELETE /company/time-offs/{id}`](https://developer.personio.de/reference/delete_company-time-offs-id): delete the absence entry with the specified ID
+        
+        ### Not yet implemented
+        
+        * [`PATCH /company/employees/{id}`](https://developer.personio.de/reference/patch_company-employees-employee-id): update an existing employee entry
+        * [`GET /company/employees/{employee_id}/absences/balance`](https://developer.personio.de/reference/get_company-employees-employee-id-absences-balance): retrieve the absence balance for a specific employee
+        * [`GET /company/employees/custom-attributes`](https://developer.personio.de/reference/get_company-employees-custom-attributes): this endpoint is an alias for /company/employees/attributes
+        * [`GET /company/employees/attributes`](https://developer.personio.de/reference/get_company-employees-attributes): lists all the allowed attributes per API credentials including custom (dynamic) attributes.
+        * [`GET /company/absence-periods`](https://developer.personio.de/reference/get_company-absence-periods)
+        * [`POST /company/absence-periods`](https://developer.personio.de/reference/post_company-absence-periods)
+        * [`DELETE /company/absence-periods/{id}`](https://developer.personio.de/reference/delete_company-absence-periods-id)
+        
+        * [`GET /company/document-categories`](https://developer.personio.de/reference/get_company-document-categories): this endpoint is responsible for fetching all document categories of the company
+        * [`POST /company/documents`](https://developer.personio.de/reference/post_company-documents): this endpoint is responsible for uploading documents for the company employees
+        * [`GET /company/custom-reports/reports`](https://developer.personio.de/reference/listreports): this endpoint provides you with metadata about existing custom reports in your Personio account, such as report name, report type, report date / timeframe
+        * [`GET /company/custom-reports/reports/{report_id}`](https://developer.personio.de/reference/listreportitems): this endpoint provides you with the data of an existing Custom Report
+        * [`GET /company/custom-reports/columns`](https://developer.personio.de/reference/listcolumns): this endpoint provides human-readable labels for report table columns
+        * all of the [recruiting API](https://developer.personio.de/reference/introduction-1)
         
         ## Contact
         
         Sebastian Straub (sebastian.straub [at] alexanderthamm.com)
         
         Developed with ❤ at [Alexander Thamm GmbH](https://www.alexanderthamm.com/)
```

