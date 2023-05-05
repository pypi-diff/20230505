# Comparing `tmp/PyVISA-py-0.6.3.tar.gz` & `tmp/PyVISA-py-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyVISA-py-0.6.3.tar", last modified: Fri Feb 17 10:59:38 2023, max compression
+gzip compressed data, was "PyVISA-py-0.7.0.tar", last modified: Fri May  5 07:12:45 2023, max compression
```

## Comparing `PyVISA-py-0.6.3.tar` & `PyVISA-py-0.7.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:38.309381 PyVISA-py-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:38.305381 PyVISA-py-0.6.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:38.305381 PyVISA-py-0.6.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/.github/ISSUE_TEMPLATE/instrument-communication-issue.md
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:38.305381 PyVISA-py-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/CHANGES
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-02-17 10:59:38.309381 PyVISA-py-0.6.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:38.305381 PyVISA-py-0.6.3/PyVISA_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-02-17 10:59:38.000000 PyVISA-py-0.6.3/PyVISA_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-02-17 10:59:38.000000 PyVISA-py-0.6.3/PyVISA_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 10:59:38.000000 PyVISA-py-0.6.3/PyVISA_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-02-17 10:59:38.000000 PyVISA-py-0.6.3/PyVISA_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-17 10:59:38.000000 PyVISA-py-0.6.3/PyVISA_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/azure-pipelines.yml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/bors.toml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:38.305381 PyVISA-py-0.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:38.305381 PyVISA-py-0.6.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:38.305381 PyVISA-py-0.6.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/docs/source/_static/logo-full.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:38.309381 PyVISA-py-0.6.3/pyvisa_py/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    32701 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/gpib.py
--rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/highlevel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:38.309381 PyVISA-py-0.6.3/pyvisa_py/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26990 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/protocols/hislip.py
--rw-r--r--   0 runner    (1001) docker     (123)    33528 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/protocols/rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/protocols/usbraw.py
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/protocols/usbtmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/protocols/usbutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/protocols/vxi11.py
--rw-r--r--   0 runner    (1001) docker     (123)    16236 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    28217 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)    49746 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/tcpip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:38.309381 PyVISA-py-0.6.3/pyvisa_py/testsuite/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/testsuite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:59:38.309381 PyVISA-py-0.6.3/pyvisa_py/testsuite/keysight_assisted_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/testsuite/keysight_assisted_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/testsuite/keysight_assisted_tests/test_resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/testsuite/keysight_assisted_tests/test_tcpip_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/testsuite/test_highlevel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10867 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/pyvisa_py/usb.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-02-17 10:59:38.000000 PyVISA-py-0.6.3/pyvisa_py/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 10:59:38.309381 PyVISA-py-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-17 10:59:21.000000 PyVISA-py-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:12:45.232563 PyVISA-py-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:12:45.228563 PyVISA-py-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:12:45.228563 PyVISA-py-0.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/.github/ISSUE_TEMPLATE/instrument-communication-issue.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:12:45.228563 PyVISA-py-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-05-05 07:12:45.232563 PyVISA-py-0.7.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:12:45.228563 PyVISA-py-0.7.0/PyVISA_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-05-05 07:12:45.000000 PyVISA-py-0.7.0/PyVISA_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-05 07:12:45.000000 PyVISA-py-0.7.0/PyVISA_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:12:45.000000 PyVISA-py-0.7.0/PyVISA_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-05 07:12:45.000000 PyVISA-py-0.7.0/PyVISA_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 07:12:45.000000 PyVISA-py-0.7.0/PyVISA_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/azure-pipelines.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/bors.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:12:45.228563 PyVISA-py-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:12:45.232563 PyVISA-py-0.7.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:12:45.232563 PyVISA-py-0.7.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/docs/source/_static/logo-full.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:12:45.232563 PyVISA-py-0.7.0/pyvisa_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32826 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/gpib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/highlevel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:12:45.232563 PyVISA-py-0.7.0/pyvisa_py/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27092 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/protocols/hislip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33528 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/protocols/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/protocols/usbraw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/protocols/usbtmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/protocols/usbutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/protocols/vxi11.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28293 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50249 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/tcpip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:12:45.232563 PyVISA-py-0.7.0/pyvisa_py/testsuite/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/testsuite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:12:45.232563 PyVISA-py-0.7.0/pyvisa_py/testsuite/keysight_assisted_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/testsuite/keysight_assisted_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/testsuite/keysight_assisted_tests/test_resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/testsuite/keysight_assisted_tests/test_tcpip_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/testsuite/test_highlevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/testsuite/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/pyvisa_py/usb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-05 07:12:45.000000 PyVISA-py-0.7.0/pyvisa_py/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:12:45.232563 PyVISA-py-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-05 07:12:33.000000 PyVISA-py-0.7.0/setup.py
```

### Comparing `PyVISA-py-0.6.3/.github/FUNDING.yml` & `PyVISA-py-0.7.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/.github/ISSUE_TEMPLATE/instrument-communication-issue.md` & `PyVISA-py-0.7.0/.github/ISSUE_TEMPLATE/instrument-communication-issue.md`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/.github/PULL_REQUEST_TEMPLATE.md` & `PyVISA-py-0.7.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/.github/workflows/ci.yml` & `PyVISA-py-0.7.0/.github/workflows/ci.yml`

 * *Files 19% similar despite different names*

```diff
@@ -21,30 +21,33 @@
     name: Check code formatting
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.8
+          python-version: "3.10"
       - name: Install tools
         run: |
           python -m pip install --upgrade pip
           pip install flake8 black isort mypy pytest
           pip install git+https://github.com/pyvisa/pyvisa.git@main
       - name: Isort
         run: |
           isort pyvisa_py -c;
       - name: Black
+        if: always()
         run: |
           black pyvisa_py --check;
       - name: Flake8
+        if: always()
         run: |
           flake8 pyvisa_py;
       - name: Mypy
+        if: always()
         run: |
           mypy pyvisa_py;
   tests:
     name: Unit tests
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
```

### Comparing `PyVISA-py-0.6.3/.github/workflows/docs.yml` & `PyVISA-py-0.7.0/.github/workflows/docs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
       - setup.py
 
 jobs:
   docs:
     name: Docs building
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r docs/requirements.txt
           pip install git+https://github.com/pyvisa/pyvisa.git
       - name: Install project
         run: |
```

### Comparing `PyVISA-py-0.6.3/.github/workflows/release.yml` & `PyVISA-py-0.7.0/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 jobs:
   build_sdist:
     name: Build sdist
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       - name: Get history and tags for SCM versioning to work
         run: |
           git fetch --prune --unshallow
           git fetch --depth=1 origin +refs/tags/*:refs/tags/*
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
       - name: Build sdist
         run: |
           pip install --upgrade pip
           pip install wheel build
           python -m build . -s
       - name: Test sdist
         run: |
@@ -37,21 +37,21 @@
           path: dist/*
 
   build_wheel:
     name: Build wheel
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       - name: Get history and tags for SCM versioning to work
         run: |
           git fetch --prune --unshallow
           git fetch --depth=1 origin +refs/tags/*:refs/tags/*
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
       - name: Build wheels
         run: |
           pip install --upgrade pip
           pip install wheel build
           python -m build . -w
       - name: Test wheel
         run: |
```

### Comparing `PyVISA-py-0.6.3/.readthedocs.yaml` & `PyVISA-py-0.7.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/AUTHORS` & `PyVISA-py-0.7.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/CHANGES` & `PyVISA-py-0.7.0/CHANGES`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 PyVISA-py Changelog
 ===================
 
+0.7.0 (05/05/2023)
+------------------
+
+- add support for the flush operation with TCPIP::SOCKET resources PR #350
+- drop support for Python 3.7 PR #362
+- fix listing of available resources PR #362
+- fix hislip support for custom sub_addresses PR #359
+- fix bad USBRaw resource preventing enumeration of other resources PR #370
+
 0.6.3 (17-02-2023)
 ------------------
 
 - fix bad behavior on PyVISA 1.12 and hence on Python 3.7 PR #357
   0.6.x is the last version that will support Python 3.7
 
 0.6.2 (08-02-2023)
```

### Comparing `PyVISA-py-0.6.3/LICENSE` & `PyVISA-py-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/PKG-INFO` & `PyVISA-py-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVISA-py
-Version: 0.6.3
+Version: 0.7.0
 Summary: Pure Python implementation of a VISA library.
 Author-email: "Hernan E. Grecco" <hernan.grecco@gmail.com>
 Maintainer-email: "Matthieu C. Dartiailh" <m.dartiailh@gmail.com>
 License: The MIT License
         
         Copyright (c) 2014 PyVISA-py Authors and contributors. See AUTHORS
         
@@ -41,15 +41,15 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: gpib-ctypes
 Provides-Extra: serial
 Provides-Extra: usb
 Provides-Extra: psutil
 Provides-Extra: hislip-discovery
 Provides-Extra: vicp
```

### Comparing `PyVISA-py-0.6.3/PyVISA_py.egg-info/PKG-INFO` & `PyVISA-py-0.7.0/PyVISA_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVISA-py
-Version: 0.6.3
+Version: 0.7.0
 Summary: Pure Python implementation of a VISA library.
 Author-email: "Hernan E. Grecco" <hernan.grecco@gmail.com>
 Maintainer-email: "Matthieu C. Dartiailh" <m.dartiailh@gmail.com>
 License: The MIT License
         
         Copyright (c) 2014 PyVISA-py Authors and contributors. See AUTHORS
         
@@ -41,15 +41,15 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: gpib-ctypes
 Provides-Extra: serial
 Provides-Extra: usb
 Provides-Extra: psutil
 Provides-Extra: hislip-discovery
 Provides-Extra: vicp
```

### Comparing `PyVISA-py-0.6.3/PyVISA_py.egg-info/SOURCES.txt` & `PyVISA-py-0.7.0/PyVISA_py.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -50,10 +50,11 @@
 pyvisa_py/protocols/rpc.py
 pyvisa_py/protocols/usbraw.py
 pyvisa_py/protocols/usbtmc.py
 pyvisa_py/protocols/usbutil.py
 pyvisa_py/protocols/vxi11.py
 pyvisa_py/testsuite/__init__.py
 pyvisa_py/testsuite/test_highlevel.py
+pyvisa_py/testsuite/test_sessions.py
 pyvisa_py/testsuite/keysight_assisted_tests/__init__.py
 pyvisa_py/testsuite/keysight_assisted_tests/test_resource_manager.py
 pyvisa_py/testsuite/keysight_assisted_tests/test_tcpip_resources.py
```

### Comparing `PyVISA-py-0.6.3/README.rst` & `PyVISA-py-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/azure-pipelines.yml` & `PyVISA-py-0.7.0/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/docs/Makefile` & `PyVISA-py-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/docs/index.rst` & `PyVISA-py-0.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/docs/make.bat` & `PyVISA-py-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/docs/source/_static/logo-full.jpg` & `PyVISA-py-0.7.0/docs/source/_static/logo-full.jpg`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/docs/source/conf.py` & `PyVISA-py-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/docs/source/faq.rst` & `PyVISA-py-0.7.0/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/docs/source/index.rst` & `PyVISA-py-0.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/docs/source/installation.rst` & `PyVISA-py-0.7.0/docs/source/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -67,23 +67,21 @@
 that you should also install. Please refer to PyUSB_ documentation for more
 details.
 
 On Unix system, one may have to modify udev rules to allow non-root access to
 the device you are trying to connect to. The following tutorial describes how
 to do it http://ask.xmodulo.com/change-usb-device-permission-linux.html.
 
-On Windows, you may have to uninstall the USBTMC specific driver installed by
-Windows and re-install a generic driver.
+On Windows, you may have to uninstall the USBTMC-specific driver installed by
+Windows and re-install a generic driver. Please check `libusb's guide`_ for more
+details, but installing a ``WinUSB`` driver with Zadig_ should be a good start.
 
 Note that on Windows, devices that are already open cannot be detected and will
 not be returned by ``ResourceManager.list_resources``.
 
-Another useful reference for how to configure your system is h
-ttps://github.com/python-ivi/python-usbtmc.
-
 
 How do I know if PyVISA-py is properly installed?
 -------------------------------------------------
 
 Using the pyvisa information tool. Run in your console::
 
   pyvisa-info
@@ -110,7 +108,9 @@
 .. _`issue tracker`: https://github.com/pyvisa/pyvisa-py/issues
 .. _`linux-gpib`: http://linux-gpib.sourceforge.net/
 .. _`gpib-ctypes`: https://pypi.org/project/gpib-ctypes/
 .. _`psutil`: https://pypi.org/project/psutil/
 .. _`mDNS`: https://en.wikipedia.org/wiki/Multicast_DNS
 .. _`zeroconf`: https://pypi.org/project/zeroconf/
 .. _`pyvicp`: https://pypi.org/project/pyvicp/
+.. _`libusb's guide`: https://github.com/libusb/libusb/wiki/Windows#user-content-How_to_use_libusb_on_Windows
+.. _`Zadig`: https://zadig.akeo.ie/
```

### Comparing `PyVISA-py-0.6.3/pyproject.toml` & `PyVISA-py-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "PyVISA-py"
 description = "Pure Python implementation of a VISA library."
 readme = "README.rst"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
   {name = "Hernan E. Grecco", email = "hernan.grecco@gmail.com"},
 ]
 maintainers = [
   {name = "Matthieu C. Dartiailh", email = "m.dartiailh@gmail.com"}
 ]
@@ -32,15 +32,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
-    "pyvisa>=1.12.0",
+    "pyvisa>=1.13.0",
     "typing_extensions",
     "importlib-metadata; python_version<'3.8'",
 ]
 dynamic=["version"]
 
 [project.optional-dependencies]
 gpib-ctypes = ["gpib-ctypes>=0.3.0"]
@@ -98,14 +98,15 @@
 [[tool.mypy.overrides]]
 module = [
     "usb.*",
     "serial.*",
     "gpib.*",
     "Gpib.*",
     "gpib_ctypes.*",
+    "pyvicp.*",
 
 ]
 ignore_missing_imports = true
 
 [tool.isort]
 profile = "black"
 combine_as_imports = true
```

### Comparing `PyVISA-py-0.6.3/pyvisa_py/__init__.py` & `PyVISA-py-0.7.0/pyvisa_py/__init__.py`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/pyvisa_py/attributes.py` & `PyVISA-py-0.7.0/pyvisa_py/attributes.py`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/pyvisa_py/common.py` & `PyVISA-py-0.7.0/pyvisa_py/common.py`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/pyvisa_py/gpib.py` & `PyVISA-py-0.7.0/pyvisa_py/gpib.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,39 +30,37 @@
             ("ibpct", [ctypes.c_int], ctypes.c_int),
         ]
         for name, argtypes, restype in extra_funcs:
             libfunction = gpib_lib[name]
             libfunction.argtypes = argtypes
             libfunction.restype = restype
     except TypeError:
-        Session.register_unavailable(
-            constants.InterfaceType.gpib,
-            "INSTR",
+        msg = (
             "gpib_ctypes is installed but could not locate the gpib library.\n"
             "Please manually load it using:\n"
             "  gpib_ctypes.gpib.gpib._load_lib(filename)\n"
-            "before importing pyvisa.",
+            "before importing pyvisa."
         )
+        Session.register_unavailable(constants.InterfaceType.gpib, "INSTR", msg)
+        Session.register_unavailable(constants.InterfaceType.gpib, "INTFC", msg)
         raise
 
 except ImportError:
     GPIB_CTYPES = False
     try:
         import gpib  # typing: ignore
         from Gpib import Gpib  # typing: ignore
     except ImportError as e:
-        Session.register_unavailable(
-            constants.InterfaceType.gpib,
-            "INSTR",
-            "Please install linux-gpib (Linux) or "
-            "gpib-ctypes (Windows, Linux) to use "
-            "this resource type. Note that installing"
-            " gpib-ctypes will give you access to a "
-            "broader range of funcionality.\n%s" % e,
+        msg = (
+            "Please install linux-gpib (Linux) or gpib-ctypes (Windows, Linux) "
+            "to use this resource type. Note that installing gpib-ctypes will "
+            "give you access to a broader range of functionalities.\n%s" % e
         )
+        Session.register_unavailable(constants.InterfaceType.gpib, "INSTR", msg)
+        Session.register_unavailable(constants.InterfaceType.gpib, "INTFC", msg)
         raise
 
 
 # patch Gpib to avoid double closing of handles
 def _patch_Gpib() -> None:
     if not hasattr(Gpib, "close"):
         _old_del = Gpib.__del__
```

### Comparing `PyVISA-py-0.6.3/pyvisa_py/highlevel.py` & `PyVISA-py-0.7.0/pyvisa_py/highlevel.py`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/pyvisa_py/protocols/hislip.py` & `PyVISA-py-0.7.0/pyvisa_py/protocols/hislip.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,30 +361,34 @@
 class Instrument:
     """
     this is the principal export from this module.  it opens up a HiSLIP
     connection to the instrument at the specified IP address.
     """
 
     def __init__(
-        self, ip_addr: str, timeout: Optional[float] = None, port: int = PORT
+        self,
+        ip_addr: str,
+        timeout: Optional[float] = None,
+        port: int = PORT,
+        sub_address: str = "hislip0",
     ) -> None:
         # init transaction:
         #     C->S: Initialize
         #     S->C: InitializeResponse
         #     C->S: AsyncInitialize
         #     S->C: AsyncInitializeResponse
 
         timeout = timeout or 5.0
 
         # open the synchronous socket and send an initialize packet
         self._sync = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self._sync.connect((ip_addr, port))
         self._sync.settimeout(timeout)
         self._sync.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
-        init = self.initialize()
+        init = self.initialize(sub_address=sub_address.encode("ascii"))
         if init.overlap != 0:
             print("**** prefer overlap = %d" % init.overlap)
 
         # open the asynchronous socket and send an initialize packet
         self._async = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self._async.connect((ip_addr, port))
         self._async.settimeout(timeout)
```

### Comparing `PyVISA-py-0.6.3/pyvisa_py/protocols/rpc.py` & `PyVISA-py-0.7.0/pyvisa_py/protocols/rpc.py`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/pyvisa_py/protocols/usbraw.py` & `PyVISA-py-0.7.0/pyvisa_py/protocols/usbraw.py`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/pyvisa_py/protocols/usbtmc.py` & `PyVISA-py-0.7.0/pyvisa_py/protocols/usbtmc.py`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/pyvisa_py/protocols/usbutil.py` & `PyVISA-py-0.7.0/pyvisa_py/protocols/usbutil.py`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/pyvisa_py/protocols/vxi11.py` & `PyVISA-py-0.7.0/pyvisa_py/protocols/vxi11.py`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/pyvisa_py/serial.py` & `PyVISA-py-0.7.0/pyvisa_py/serial.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,20 +232,15 @@
 
         Returns
         -------
         constants.StatusCode
             Return value of the library call.
 
         """
-        if (
-            mask & BufferOperation.discard_read_buffer
-            or mask & BufferOperation.discard_read_buffer_no_io
-            or mask & BufferOperation.discard_receive_buffer
-            or mask & BufferOperation.discard_receive_buffer2
-        ):
+        if mask & BufferOperation.discard_read_buffer:
             self.interface.reset_input_buffer()
         if (
             mask & BufferOperation.flush_write_buffer
             or mask & BufferOperation.flush_transmit_buffer
         ):
             self.interface.flush()
         if (
```

### Comparing `PyVISA-py-0.6.3/pyvisa_py/sessions.py` & `PyVISA-py-0.7.0/pyvisa_py/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,26 @@
 
 :copyright: 2014-2020 by PyVISA-py Authors, see AUTHORS for more details.
 :license: MIT, see LICENSE for more details.
 
 """
 import abc
 import time
-from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Type, TypeVar
+from typing import (
+    Any,
+    Callable,
+    ClassVar,
+    Dict,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+)
 
 from pyvisa import attributes, constants, logger, rname
 from pyvisa.constants import ResourceAttribute, StatusCode
 from pyvisa.typing import VISARMSession
 
 from .common import int_to_byte
 
@@ -154,27 +165,25 @@
 
     @classmethod
     def iter_valid_session_classes(
         cls,
     ) -> Iterator[Tuple[Tuple[constants.InterfaceType, str], Type["Session"]]]:
         """Iterator over valid sessions classes infos."""
         for key, val in cls._session_classes.items():
-            if issubclass(val, Session):
+            if not issubclass(val, UnavailableSession):
                 yield key, val
 
     @classmethod
     def iter_session_classes_issues(
         cls,
     ) -> Iterator[Tuple[Tuple[constants.InterfaceType, str], str]]:
         """Iterator over invalid sessions classes (i.e. those with import errors)."""
         for key, val in cls._session_classes.items():
-            try:
+            if issubclass(val, UnavailableSession):
                 yield key, getattr(val, "session_issue")
-            except AttributeError:
-                pass
 
     @classmethod
     def get_session_class(
         cls, interface_type: constants.InterfaceType, resource_class: str
     ) -> Type["Session"]:
         """Get the session class for a given interface type and resource class.
 
@@ -254,29 +263,17 @@
         Returns
         -------
         Type[Session]
             Fake session.
 
         """
 
-        class _internal(Session):
+        class _internal(UnavailableSession):
             #: Message detailing why no session is available.
-            session_issue: str = msg
-
-            def __init__(self, *args, **kwargs) -> None:
-                raise ValueError(msg)
-
-            def _get_attribute(self, attr):
-                raise NotImplementedError()
-
-            def _set_attribute(self, attr, value):
-                raise NotImplementedError()
-
-            def close(self):
-                raise NotImplementedError()
+            session_issue = msg
 
         if (interface_type, resource_class) in cls._session_classes:
             logger.warning(
                 "%s is already registered in the ResourceManager. "
                 "Overwriting with unavailable %s",
                 (interface_type, resource_class),
                 msg,
@@ -850,7 +847,23 @@
         if value == constants.VI_TMO_INFINITE:
             self.timeout = None
         elif value == constants.VI_TMO_IMMEDIATE:
             self.timeout = 0
         else:
             self.timeout = value / 1000.0
         return StatusCode.success
+
+
+class UnavailableSession(Session):
+    session_issue: ClassVar[str]
+
+    def __init__(self, *args, **kwargs) -> None:
+        raise ValueError(self.session_issue)
+
+    def _get_attribute(self, attr):
+        raise NotImplementedError()
+
+    def _set_attribute(self, attr, value):
+        raise NotImplementedError()
+
+    def close(self):
+        raise NotImplementedError()
```

### Comparing `PyVISA-py-0.6.3/pyvisa_py/tcpip.py` & `PyVISA-py-0.7.0/pyvisa_py/tcpip.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import select
 import socket
 import time
 import warnings
 from typing import Any, Dict, List, Optional, Tuple, Type
 
 from pyvisa import attributes, constants, errors, rname
-from pyvisa.constants import ResourceAttribute, StatusCode
+from pyvisa.constants import BufferOperation, ResourceAttribute, StatusCode
 
 from . import common
 from .protocols import hislip, rpc, vxi11
 from .sessions import Session, UnknownAttribute, VISARMSession
 
 # Let psutil be optional dependency
 try:
@@ -29,15 +29,15 @@
 
 # Let zeroconf be optional dependency
 try:
     import zeroconf  # type: ignore
 except ImportError:
     zeroconf = None  # type: ignore
 
-# Let pyvicp be optional dependency
+# Let pyvicp be an optional dependency
 try:
     import pyvicp  # type: ignore
 except ImportError:
     pyvicp = None  # type: ignore
 
 
 # Conversion between VXI11 error codes and VISA status
@@ -125,20 +125,24 @@
             )
         return sorted(resources)
 
     def after_parsing(self) -> None:
         # TODO: board_number not handled
 
         if "," in self.parsed.lan_device_name:
-            _, port_str = self.parsed.lan_device_name.split(",")
+            sub_address, port_str = self.parsed.lan_device_name.split(",")
             port = int(port_str)
         else:
+            sub_address = self.parsed.lan_device_name
             port = 4880
         self.interface = hislip.Instrument(
-            self.parsed.host_address, port=port, timeout=self.timeout
+            self.parsed.host_address,
+            timeout=self.timeout,
+            port=port,
+            sub_address=sub_address,
         )
 
         # initialize the constant attributes
         self.attrs[ResourceAttribute.dma_allow_enabled] = constants.VI_FALSE
         self.attrs[ResourceAttribute.file_append_enabled] = constants.VI_FALSE
         self.attrs[ResourceAttribute.interface_instrument_name] = "TCPIP0 (HiSLIP)"
         self.attrs[ResourceAttribute.interface_number] = 0
@@ -794,242 +798,234 @@
             self._io_timeout = 0
         else:
             self.timeout = value / 1000.0
             self._io_timeout = int(self.timeout * 1000)
         return StatusCode.success
 
 
-# Requires Pyvisa >= 1.13
-if hasattr(rname, "VICPInstr"):
+class TCPIPInstrVicp(Session):
+    """VICP Session that uses pyvicp to do the low level communication."""
 
-    class TCPIPInstrVicp(Session):
-        """VICP Session that uses pyvicp to do the low level communication."""
+    # Override parsed to take into account the fact that this class is only used
+    # for a specific kind of resource
+    parsed: rname.VICPInstr
 
-        # Override parsed to take into account the fact that this class is only used
-        # for a specific kind of resource
-        parsed: rname.VICPInstr
-
-        @staticmethod
-        def list_resources(wait_time=1.0) -> List[str]:
-            resources = []
-            try:
-                services = get_services("_lxi._tcp.local.", wait_time=wait_time)
-            except NotImplementedError:
-                warnings.warn(
-                    "VICP resources discovery requires the zeroconf package to be "
-                    "installed... try 'pip install zeroconf'",
-                    UserWarning,
-                )
-                return []
+    @staticmethod
+    def list_resources(wait_time=1.0) -> List[str]:
+        resources = []
+        try:
+            services = get_services("_lxi._tcp.local.", wait_time=wait_time)
+        except NotImplementedError:
+            warnings.warn(
+                "VICP resources discovery requires the zeroconf package to be "
+                "installed... try 'pip install zeroconf'",
+                UserWarning,
+            )
+            return []
 
-            for host, properties in services.items():
-                if properties["Manufacturer"].lower().startswith("lecroy"):
-                    resources.append(f"VICP::{host}::INSTR")
-
-            return sorted(resources)
-
-        def after_parsing(self) -> None:
-            # TODO: board_number not handled
-            if pyvicp is None:
-                raise NotImplementedError(
-                    "VICP requires the pyvicp package to be installed... "
-                    "try 'pip install pyvicp'"
-                )
+        for host, properties in services.items():
+            if properties["Manufacturer"].lower().startswith("lecroy"):
+                resources.append(f"VICP::{host}::INSTR")
 
-            host_address = self.parsed.host_address
-            if "," in host_address:
-                host_address, port_str = host_address.split(",")
-                port = int(port_str)
-            else:
-                port = 1861
+        return sorted(resources)
 
-            self.interface = pyvicp.Client(
-                self.parsed.host_address, port, timeout=self.timeout
+    def after_parsing(self) -> None:
+        # TODO: board_number not handled
+        if pyvicp is None:
+            raise NotImplementedError(
+                "VICP requires the pyvicp package to be installed... "
+                "try 'pip install pyvicp'"
             )
 
-            # initialize the constant attributes
-            for name in ("SEND_END_EN", "TERMCHAR", "TERMCHAR_EN"):
-                attribute = getattr(constants, "VI_ATTR_" + name)
-                self.attrs[attribute] = attributes.AttributesByID[attribute].default
-
-            self.attrs[ResourceAttribute.dma_allow_enabled] = constants.VI_FALSE
-            self.attrs[ResourceAttribute.file_append_enabled] = constants.VI_FALSE
-            self.attrs[ResourceAttribute.interface_instrument_name] = "TCPIP0 (VICP)"
-            self.attrs[ResourceAttribute.interface_number] = 0
-            self.attrs[ResourceAttribute.io_prot] = constants.VI_PROT_NORMAL
-            self.attrs[
-                ResourceAttribute.read_buffer_operation_mode
-            ] = constants.VI_FLUSH_DISABLE
-            self.attrs[ResourceAttribute.resource_lock_state] = constants.VI_NO_LOCK
-            self.attrs[ResourceAttribute.suppress_end_enabled] = constants.VI_FALSE
-            self.attrs[ResourceAttribute.tcpip_address] = self.parsed.host_address
-            self.attrs[ResourceAttribute.tcpip_hostname] = self.parsed.host_address
-            self.attrs[ResourceAttribute.tcpip_is_hislip] = constants.VI_FALSE
-            self.attrs[ResourceAttribute.tcpip_nodelay] = constants.VI_TRUE
-            self.attrs[ResourceAttribute.tcpip_port] = port
-            self.attrs[
-                ResourceAttribute.write_buffer_operation_mode
-            ] = constants.VI_FLUSH_WHEN_FULL
-
-            # configure the variable attributes
-            self.attrs[ResourceAttribute.tcpip_keepalive] = (
-                self.get_keepalive,
-                self.set_keepalive,
-            )
+        host_address = self.parsed.host_address
+        if "," in host_address:
+            host_address, port_str = host_address.split(",")
+            port = int(port_str)
+        else:
+            port = 1861
 
-            # TODO: additional attributes (someday)
-            # self.attrs[ResourceAttribute.manufacturer_id] = 16711
-            # self.attrs[ResourceAttribute.max_queue_length] = 50
-            # self.attrs[ResourceAttribute.read_buffer_size] = 4096
-            # self.attrs[ResourceAttribute.resource_impl_version] = 0x0050_0c01
-            # self.attrs[ResourceAttribute.resource_manufacturer_id] = 4015
-            # self.attrs[ResourceAttribute.resource_manufacturer_name] = 'Rohde & Schwarz GmbH'
-            # self.attrs[ResourceAttribute.resource_spec_version] = 0x0050_0800
-            # self.attrs[ResourceAttribute.user_data] = 0
-            # self.attrs[ResourceAttribute.write_buffer_size] = 4096
-
-        def get_keepalive(
-            self, attribute: ResourceAttribute
-        ) -> Tuple[bool, StatusCode]:
-            """Is TCP keepalive enabled for the resource."""
-            return self.interface.keepalive, StatusCode.success
-
-        def set_keepalive(
-            self, attribute: ResourceAttribute, keepalive: bool
-        ) -> StatusCode:
-            """Turns TCP keepalive on/off for this connection."""
-            self.interface.keepalive = keepalive
-            return StatusCode.success
+        self.interface = pyvicp.Client(
+            self.parsed.host_address, port, timeout=self.timeout
+        )
 
-        def close(self) -> StatusCode:
-            self.interface.close()
-            self.interface = None
-            return StatusCode.success
+        # initialize the constant attributes
+        for name in ("SEND_END_EN", "TERMCHAR", "TERMCHAR_EN"):
+            attribute = getattr(constants, "VI_ATTR_" + name)
+            self.attrs[attribute] = attributes.AttributesByID[attribute].default
 
-        def read(self, count: int) -> Tuple[bytes, StatusCode]:
-            """Reads data from device or interface synchronously.
+        self.attrs[ResourceAttribute.dma_allow_enabled] = constants.VI_FALSE
+        self.attrs[ResourceAttribute.file_append_enabled] = constants.VI_FALSE
+        self.attrs[ResourceAttribute.interface_instrument_name] = "TCPIP0 (VICP)"
+        self.attrs[ResourceAttribute.interface_number] = 0
+        self.attrs[ResourceAttribute.io_prot] = constants.VI_PROT_NORMAL
+        self.attrs[
+            ResourceAttribute.read_buffer_operation_mode
+        ] = constants.VI_FLUSH_DISABLE
+        self.attrs[ResourceAttribute.resource_lock_state] = constants.VI_NO_LOCK
+        self.attrs[ResourceAttribute.suppress_end_enabled] = constants.VI_FALSE
+        self.attrs[ResourceAttribute.tcpip_address] = self.parsed.host_address
+        self.attrs[ResourceAttribute.tcpip_hostname] = self.parsed.host_address
+        self.attrs[ResourceAttribute.tcpip_is_hislip] = constants.VI_FALSE
+        self.attrs[ResourceAttribute.tcpip_nodelay] = constants.VI_TRUE
+        self.attrs[ResourceAttribute.tcpip_port] = port
+        self.attrs[
+            ResourceAttribute.write_buffer_operation_mode
+        ] = constants.VI_FLUSH_WHEN_FULL
 
-            Corresponds to viRead function of the VISA library.
+        # configure the variable attributes
+        self.attrs[ResourceAttribute.tcpip_keepalive] = (
+            self.get_keepalive,
+            self.set_keepalive,
+        )
 
-            Parameters
-            -----------
-            count : int
-                Number of bytes to be read.
-
-            Returns
-            -------
-            bytes
-                Data read from the device
-            StatusCode
-                Return value of the library call.
+        # TODO: additional attributes (someday)
+        # self.attrs[ResourceAttribute.manufacturer_id] = 16711
+        # self.attrs[ResourceAttribute.max_queue_length] = 50
+        # self.attrs[ResourceAttribute.read_buffer_size] = 4096
+        # self.attrs[ResourceAttribute.resource_impl_version] = 0x0050_0c01
+        # self.attrs[ResourceAttribute.resource_manufacturer_id] = 4015
+        # self.attrs[ResourceAttribute.resource_manufacturer_name] = 'Rohde & Schwarz GmbH'
+        # self.attrs[ResourceAttribute.resource_spec_version] = 0x0050_0800
+        # self.attrs[ResourceAttribute.user_data] = 0
+        # self.attrs[ResourceAttribute.write_buffer_size] = 4096
 
-            """
-            try:
-                data = self.interface.receive(count)
-            except socket.timeout:
-                return b"", StatusCode.error_timeout
+    def get_keepalive(self, attribute: ResourceAttribute) -> Tuple[bool, StatusCode]:
+        """Is TCP keepalive enabled for the resource."""
+        return self.interface.keepalive, StatusCode.success
 
-            if len(data) >= count:
-                return data, StatusCode.success_max_count_read
-            else:
-                return data, StatusCode.success_termination_character_read
+    def set_keepalive(
+        self, attribute: ResourceAttribute, keepalive: bool
+    ) -> StatusCode:
+        """Turns TCP keepalive on/off for this connection."""
+        self.interface.keepalive = keepalive
+        return StatusCode.success
 
-        def write(self, data: bytes) -> Tuple[int, StatusCode]:
-            """Writes data to device or interface synchronously.
+    def close(self) -> StatusCode:
+        self.interface.close()
+        self.interface = None
+        return StatusCode.success
 
-            Corresponds to viWrite function of the VISA library.
+    def read(self, count: int) -> Tuple[bytes, StatusCode]:
+        """Reads data from device or interface synchronously.
 
-            Parameters
-            ----------
-            data : bytes
-                Data to be written.
+        Corresponds to viRead function of the VISA library.
 
-            Returns
-            -------
-            int
-                Number of bytes actually transferred
-            StatusCode
-                Return value of the library call.
+        Parameters
+        -----------
+        count : int
+            Number of bytes to be read.
 
-            """
-            self.interface.send(data)
+        Returns
+        -------
+        bytes
+            Data read from the device
+        StatusCode
+            Return value of the library call.
 
-            return len(data), StatusCode.success
+        """
+        try:
+            data = self.interface.receive(count)
+        except socket.timeout:
+            return b"", StatusCode.error_timeout
 
-        def clear(self) -> StatusCode:
-            """Clears a device.
+        if len(data) >= count:
+            return data, StatusCode.success_max_count_read
+        else:
+            return data, StatusCode.success_termination_character_read
 
-            Corresponds to viClear function of the VISA library.
+    def write(self, data: bytes) -> Tuple[int, StatusCode]:
+        """Writes data to device or interface synchronously.
 
-            """
-            self.interface.device_clear()
+        Corresponds to viWrite function of the VISA library.
 
-            return StatusCode.success
+        Parameters
+        ----------
+        data : bytes
+            Data to be written.
 
-        def _set_timeout(self, attribute: ResourceAttribute, value: int) -> StatusCode:
-            status = super()._set_timeout(attribute, value)
-            if hasattr(self.interface, "timeout"):
-                self.interface.timeout = 1e-3 * value
-
-            return status
-
-        def _get_attribute(
-            self, attribute: ResourceAttribute
-        ) -> Tuple[Any, StatusCode]:
-            """Get the value for a given VISA attribute for this session.
-
-            Use to implement custom logic for attributes.
-
-            Parameters
-            ----------
-            attribute : ResourceAttribute
-                Attribute for which the state query is made
-
-            Returns
-            -------
-            Any
-                State of the queried attribute for a specified resource
-            StatusCode
-                Return value of the library call.
-
-            """
-            raise UnknownAttribute(attribute)
-
-        def _set_attribute(
-            self, attribute: ResourceAttribute, attribute_state: Any
-        ) -> StatusCode:
-            """Sets the state of an attribute.
-
-            Corresponds to viSetAttribute function of the VISA library.
-
-            Parameters
-            ----------
-            attribute : constants.ResourceAttribute
-                Attribute for which the state is to be modified. (Attributes.*)
-            attribute_state : Any
-                The state of the attribute to be set for the specified object.
-
-            Returns
-            -------
-            StatusCode
-                Return value of the library call.
-
-            """
-            raise UnknownAttribute(attribute)
-
-
-if hasattr(constants.InterfaceType, "vicp"):
-    if pyvicp is not None:
-        Session.register(constants.InterfaceType.vicp, "INSTR")(TCPIPInstrVicp)
-    else:
-        Session.register_unavailable(
-            constants.InterfaceType.vicp,
-            "INSTR",
-            "Please install PyVICP to use this resource type.",
-        )
+        Returns
+        -------
+        int
+            Number of bytes actually transferred
+        StatusCode
+            Return value of the library call.
+
+        """
+        self.interface.send(data)
+
+        return len(data), StatusCode.success
+
+    def clear(self) -> StatusCode:
+        """Clears a device.
+
+        Corresponds to viClear function of the VISA library.
+
+        """
+        self.interface.device_clear()
+
+        return StatusCode.success
+
+    def _set_timeout(self, attribute: ResourceAttribute, value: int) -> StatusCode:
+        status = super()._set_timeout(attribute, value)
+        if hasattr(self.interface, "timeout"):
+            self.interface.timeout = 1e-3 * value
+
+        return status
+
+    def _get_attribute(self, attribute: ResourceAttribute) -> Tuple[Any, StatusCode]:
+        """Get the value for a given VISA attribute for this session.
+
+        Use to implement custom logic for attributes.
+
+        Parameters
+        ----------
+        attribute : ResourceAttribute
+            Attribute for which the state query is made
+
+        Returns
+        -------
+        Any
+            State of the queried attribute for a specified resource
+        StatusCode
+            Return value of the library call.
+
+        """
+        raise UnknownAttribute(attribute)
+
+    def _set_attribute(
+        self, attribute: ResourceAttribute, attribute_state: Any
+    ) -> StatusCode:
+        """Sets the state of an attribute.
+
+        Corresponds to viSetAttribute function of the VISA library.
+
+        Parameters
+        ----------
+        attribute : constants.ResourceAttribute
+            Attribute for which the state is to be modified. (Attributes.*)
+        attribute_state : Any
+            The state of the attribute to be set for the specified object.
+
+        Returns
+        -------
+        StatusCode
+            Return value of the library call.
+
+        """
+        raise UnknownAttribute(attribute)
+
+
+if pyvicp is not None:
+    Session.register(constants.InterfaceType.vicp, "INSTR")(TCPIPInstrVicp)
+else:
+    Session.register_unavailable(
+        constants.InterfaceType.vicp,
+        "INSTR",
+        "Please install PyVICP to use this resource type.",
+    )
 
 
 @Session.register(constants.InterfaceType.tcpip, "SOCKET")
 class TCPIPSocketSession(Session):
     """A TCPIP Session that uses the network standard library to do the low
     level communication.
 
@@ -1270,14 +1266,46 @@
             r, w, x = select.select([self.interface], [], [], 0.1)
             if not r:
                 break
             r[0].recv(4096)
 
         return StatusCode.success
 
+    def flush(self, mask: BufferOperation) -> StatusCode:
+        """Flush the specified buffers.
+        Corresponds to viFlush function of the VISA library.
+        Parameters
+        ----------
+        mask : constants.BufferOperation
+            Specifies the action to be taken with flushing the buffer.
+            The values can be combined using the | operator. However multiple
+            operations on a single buffer cannot be combined.
+        Returns
+        -------
+        constants.StatusCode
+            Return value of the library call.
+        """
+        if mask & BufferOperation.discard_read_buffer:
+            self.clear()
+        if (
+            mask & BufferOperation.discard_read_buffer_no_io
+            or mask & BufferOperation.discard_receive_buffer
+            or mask & BufferOperation.discard_receive_buffer2
+        ):
+            self._pending_buffer.clear()
+        if (
+            mask & BufferOperation.flush_write_buffer
+            or mask & BufferOperation.flush_transmit_buffer
+            or mask & BufferOperation.discard_write_buffer
+            or mask & BufferOperation.discard_transmit_buffer
+        ):
+            pass
+
+        return StatusCode.success
+
     def _get_tcpip_nodelay(
         self, attribute: ResourceAttribute
     ) -> Tuple[constants.VisaBoolean, StatusCode]:
         if self.interface:
             value = self.interface.getsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY)
             return (
                 constants.VisaBoolean.true
```

### Comparing `PyVISA-py-0.6.3/pyvisa_py/testsuite/__init__.py` & `PyVISA-py-0.7.0/pyvisa_py/testsuite/__init__.py`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/pyvisa_py/testsuite/keysight_assisted_tests/test_resource_manager.py` & `PyVISA-py-0.7.0/pyvisa_py/testsuite/keysight_assisted_tests/test_resource_manager.py`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/pyvisa_py/testsuite/keysight_assisted_tests/test_tcpip_resources.py` & `PyVISA-py-0.7.0/pyvisa_py/testsuite/keysight_assisted_tests/test_tcpip_resources.py`

 * *Files identical despite different names*

### Comparing `PyVISA-py-0.6.3/pyvisa_py/testsuite/test_highlevel.py` & `PyVISA-py-0.7.0/pyvisa_py/testsuite/test_highlevel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# -*- coding: utf-8 -*-
 """Test creating a resource manager using PyVISA-Py as a backend.
 
 
-:copyright: 2014-2020 by PyVISA-py Authors, see AUTHORS for more details.
+:copyright: 2014-2023 by PyVISA-py Authors, see AUTHORS for more details.
 :license: MIT, see LICENSE for more details.
 
 """
 from pyvisa.highlevel import list_backends
 from pyvisa.testsuite import BaseTestCase
 
 from pyvisa_py import highlevel
```

### Comparing `PyVISA-py-0.6.3/pyvisa_py/usb.py` & `PyVISA-py-0.7.0/pyvisa_py/usb.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,15 +311,15 @@
             try:
                 intfc = intfc[0].index
             except (IndexError, AttributeError):
                 intfc = 0
 
             try:
                 serial = dev.serial_number
-            except (NotImplementedError, ValueError):
+            except (NotImplementedError, ValueError, usb.USBError):
                 msg = (
                     "Found a device whose serial number cannot be read."
                     " The partial VISA resource name is: " + fmt
                 )
                 logger.warning(
                     msg,
                     dict(
```

### Comparing `PyVISA-py-0.6.3/pyvisa_py/version.py` & `PyVISA-py-0.7.0/pyvisa_py/version.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # This file is auto-generated by setuptools-scm do NOT edit it.
 
 from collections import namedtuple
 
 #: A namedtuple of the version info for the current release.
 _version_info = namedtuple("_version_info", "major minor micro status")
 
-parts = "0.6.3".split(".", 3)
+parts = "0.7.0".split(".", 3)
 version_info = _version_info(
     int(parts[0]),
     int(parts[1]),
     int(parts[2]),
     parts[3] if len(parts) == 4 else "",
 )
 
 # Remove everything but the 'version_info' from this module.
 del namedtuple, _version_info, parts
 
-__version__ = "0.6.3"
+__version__ = "0.7.0"
```

