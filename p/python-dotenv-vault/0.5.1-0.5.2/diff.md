# Comparing `tmp/python-dotenv-vault-0.5.1.tar.gz` & `tmp/python-dotenv-vault-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dotenv-vault-0.5.1.tar", last modified: Thu May  4 06:13:15 2023, max compression
+gzip compressed data, was "python-dotenv-vault-0.5.2.tar", last modified: Fri May  5 05:53:39 2023, max compression
```

## Comparing `python-dotenv-vault-0.5.1.tar` & `python-dotenv-vault-0.5.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:13:15.296907 python-dotenv-vault-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-04 06:13:15.296907 python-dotenv-vault-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 06:13:15.296907 python-dotenv-vault-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:13:15.292907 python-dotenv-vault-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:13:15.296907 python-dotenv-vault-0.5.1/src/dotenv_vault/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/src/dotenv_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/src/dotenv_vault/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/src/dotenv_vault/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-04 06:12:52.000000 python-dotenv-vault-0.5.1/src/dotenv_vault/test_vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:13:15.296907 python-dotenv-vault-0.5.1/src/python_dotenv_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-04 06:13:15.000000 python-dotenv-vault-0.5.1/src/python_dotenv_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-04 06:13:15.000000 python-dotenv-vault-0.5.1/src/python_dotenv_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:13:15.000000 python-dotenv-vault-0.5.1/src/python_dotenv_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-04 06:13:15.000000 python-dotenv-vault-0.5.1/src/python_dotenv_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 06:13:15.000000 python-dotenv-vault-0.5.1/src/python_dotenv_vault.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:39.558388 python-dotenv-vault-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-05 05:53:39.558388 python-dotenv-vault-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:53:39.558388 python-dotenv-vault-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:39.558388 python-dotenv-vault-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:39.558388 python-dotenv-vault-0.5.2/src/dotenv_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/src/dotenv_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/src/dotenv_vault/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/src/dotenv_vault/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-05 05:53:21.000000 python-dotenv-vault-0.5.2/src/dotenv_vault/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:39.558388 python-dotenv-vault-0.5.2/src/python_dotenv_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-05 05:53:39.000000 python-dotenv-vault-0.5.2/src/python_dotenv_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-05 05:53:39.000000 python-dotenv-vault-0.5.2/src/python_dotenv_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:53:39.000000 python-dotenv-vault-0.5.2/src/python_dotenv_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 05:53:39.000000 python-dotenv-vault-0.5.2/src/python_dotenv_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 05:53:39.000000 python-dotenv-vault-0.5.2/src/python_dotenv_vault.egg-info/top_level.txt
```

### Comparing `python-dotenv-vault-0.5.1/PKG-INFO` & `python-dotenv-vault-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: python-dotenv-vault
-Version: 0.5.1
+Version: 0.5.2
 Summary: Decrypt .env.vault file.
 Home-page: https://github.com/dotenv-org/python-dotenv-vault
 Author: dotenv
 Author-email: mot@dotenv.org
 License: MIT
 Keywords: environment,environment variables,deployments,settings,env,dotenv,configurations,python,dotenv-vault
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # python-dotenv-vault [![PyPI version](https://badge.fury.io/py/python-dotenv-vault.svg)](http://badge.fury.io/py/python-dotenv-vault)
 
 <img src="https://raw.githubusercontent.com/motdotla/dotenv/master/dotenv.svg" alt="dotenv-vault" align="right" width="200" />
 
 Extends the proven & trusted foundation of [python-dotenv](https://github.com/theskumar/python-dotenv), with a `.env.vault` file.
 
@@ -167,25 +168,31 @@
 
 MIT
 
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
-## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.0...master)
+## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.1...master)
+
+## 0.5.1
+
+### Changed
+
+- Fix error reference [#10](https://github.com/dotenv-org/python-dotenv-vault/pull/10)
 
 ## 0.5.0
 
 ### Added
 
- - Reorganise and simplify code
- - Make API correspond more closely to `python-dotenv`
- - Improve error handling
- - Add tests and CI
- - Upgrade to `build` for release build
+- Reorganise and simplify code
+- Make API correspond more closely to `python-dotenv`
+- Improve error handling
+- Add tests and CI
+- Upgrade to `build` for release build
  
 ## 0.4.1
 
 ### Added
 
 - expand cryptography library version range for better support
```

### Comparing `python-dotenv-vault-0.5.1/README.md` & `python-dotenv-vault-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.5.1/setup.py` & `python-dotenv-vault-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.5.1/src/dotenv_vault/main.py` & `python-dotenv-vault-0.5.2/src/dotenv_vault/main.py`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.5.1/src/dotenv_vault/test_vault.py` & `python-dotenv-vault-0.5.2/src/dotenv_vault/test_vault.py`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.5.1/src/python_dotenv_vault.egg-info/PKG-INFO` & `python-dotenv-vault-0.5.2/src/python_dotenv_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: python-dotenv-vault
-Version: 0.5.1
+Version: 0.5.2
 Summary: Decrypt .env.vault file.
 Home-page: https://github.com/dotenv-org/python-dotenv-vault
 Author: dotenv
 Author-email: mot@dotenv.org
 License: MIT
 Keywords: environment,environment variables,deployments,settings,env,dotenv,configurations,python,dotenv-vault
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # python-dotenv-vault [![PyPI version](https://badge.fury.io/py/python-dotenv-vault.svg)](http://badge.fury.io/py/python-dotenv-vault)
 
 <img src="https://raw.githubusercontent.com/motdotla/dotenv/master/dotenv.svg" alt="dotenv-vault" align="right" width="200" />
 
 Extends the proven & trusted foundation of [python-dotenv](https://github.com/theskumar/python-dotenv), with a `.env.vault` file.
 
@@ -167,25 +168,31 @@
 
 MIT
 
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
-## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.0...master)
+## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.1...master)
+
+## 0.5.1
+
+### Changed
+
+- Fix error reference [#10](https://github.com/dotenv-org/python-dotenv-vault/pull/10)
 
 ## 0.5.0
 
 ### Added
 
- - Reorganise and simplify code
- - Make API correspond more closely to `python-dotenv`
- - Improve error handling
- - Add tests and CI
- - Upgrade to `build` for release build
+- Reorganise and simplify code
+- Make API correspond more closely to `python-dotenv`
+- Improve error handling
+- Add tests and CI
+- Upgrade to `build` for release build
  
 ## 0.4.1
 
 ### Added
 
 - expand cryptography library version range for better support
```

