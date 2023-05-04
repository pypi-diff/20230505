# Comparing `tmp/iga-0.0.7.tar.gz` & `tmp/iga-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iga-0.0.7.tar", last modified: Tue Apr 25 22:37:13 2023, max compression
+gzip compressed data, was "iga-0.0.8.tar", last modified: Thu May  4 22:43:34 2023, max compression
```

## Comparing `iga-0.0.7.tar` & `iga-0.0.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-25 22:37:13.961297 iga-0.0.7/
--rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-03-16 00:12:10.000000 iga-0.0.7/LICENSE
--rw-r--r--   0 mhucka     (503) staff       (20)    27009 2023-04-25 22:37:13.961392 iga-0.0.7/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)    26103 2023-04-25 22:30:46.000000 iga-0.0.7/README.md
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-25 22:37:13.957922 iga-0.0.7/iga/
--rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-04-25 22:35:25.000000 iga-0.0.7/iga/__init__.py
--rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-03-16 00:12:36.000000 iga-0.0.7/iga/__main__.py
--rw-r--r--   0 mhucka     (503) staff       (20)    32559 2023-04-25 22:30:46.000000 iga-0.0.7/iga/cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-03-27 20:05:34.000000 iga-0.0.7/iga/data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-04-10 21:11:51.000000 iga-0.0.7/iga/doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1179 2023-04-25 22:30:46.000000 iga-0.0.7/iga/exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1447 2023-03-28 00:40:16.000000 iga-0.0.7/iga/exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)    15031 2023-04-20 00:58:38.000000 iga-0.0.7/iga/github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4887 2023-04-25 22:30:46.000000 iga-0.0.7/iga/id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)    16908 2023-04-25 22:30:46.000000 iga-0.0.7/iga/invenio.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2058 2023-04-20 00:58:38.000000 iga-0.0.7/iga/json_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-03-08 23:12:16.000000 iga-0.0.7/iga/licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)    69392 2023-04-20 00:58:38.000000 iga-0.0.7/iga/metadata.py
--rw-r--r--   0 mhucka     (503) staff       (20)    14559 2023-04-20 00:58:38.000000 iga-0.0.7/iga/name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-04-08 02:44:39.000000 iga-0.0.7/iga/orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-04-08 02:44:39.000000 iga-0.0.7/iga/reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-04-08 02:44:39.000000 iga-0.0.7/iga/ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-04-08 02:44:39.000000 iga-0.0.7/iga/text_utils.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-25 22:37:13.958894 iga-0.0.7/iga.egg-info/
--rw-r--r--   0 mhucka     (503) staff       (20)    27009 2023-04-25 22:37:13.000000 iga-0.0.7/iga.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-04-25 22:37:13.000000 iga-0.0.7/iga.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-25 22:37:13.000000 iga-0.0.7/iga.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-04-25 22:37:13.000000 iga-0.0.7/iga.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-25 22:37:13.000000 iga-0.0.7/iga.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-04-25 22:37:13.000000 iga-0.0.7/iga.egg-info/requires.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-04-25 22:37:13.000000 iga-0.0.7/iga.egg-info/top_level.txt
--rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-04-25 22:37:13.961714 iga-0.0.7/setup.cfg
--rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-04-08 01:05:22.000000 iga-0.0.7/setup.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-25 22:37:13.961186 iga-0.0.7/tests/
--rw-r--r--   0 mhucka     (503) staff       (20)     5734 2023-04-25 22:30:46.000000 iga-0.0.7/tests/test_cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-03-27 19:38:15.000000 iga-0.0.7/tests/test_data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-03-17 23:21:28.000000 iga-0.0.7/tests/test_doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-03-02 15:36:12.000000 iga-0.0.7/tests/test_exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-01-13 03:19:50.000000 iga-0.0.7/tests/test_exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-04-07 01:26:59.000000 iga-0.0.7/tests/test_github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-04-07 01:20:36.000000 iga-0.0.7/tests/test_github_mocks.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2551 2023-04-25 22:30:46.000000 iga-0.0.7/tests/test_id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)      641 2022-12-08 00:11:08.000000 iga-0.0.7/tests/test_init.py
--rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-04-20 00:58:38.000000 iga-0.0.7/tests/test_is_person.py
--rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-03-02 15:16:32.000000 iga-0.0.7/tests/test_licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-04-20 00:58:38.000000 iga-0.0.7/tests/test_name_splitting.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-04-20 00:58:38.000000 iga-0.0.7/tests/test_name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-03-18 00:09:09.000000 iga-0.0.7/tests/test_orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1935 2023-04-08 01:31:14.000000 iga-0.0.7/tests/test_record_from_codemeta.py
--rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-03-02 23:04:18.000000 iga-0.0.7/tests/test_reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-03-18 00:05:51.000000 iga-0.0.7/tests/test_ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-04-06 22:54:59.000000 iga-0.0.7/tests/test_text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-04 22:43:34.066073 iga-0.0.8/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-03-16 00:12:10.000000 iga-0.0.8/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)    27417 2023-05-04 22:43:34.066186 iga-0.0.8/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)    26511 2023-05-04 22:41:49.000000 iga-0.0.8/README.md
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-04 22:43:34.060634 iga-0.0.8/iga/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-05-04 22:42:09.000000 iga-0.0.8/iga/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-03-16 00:12:36.000000 iga-0.0.8/iga/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    32771 2023-05-04 22:41:49.000000 iga-0.0.8/iga/cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-03-27 20:05:34.000000 iga-0.0.8/iga/data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-04-10 21:11:51.000000 iga-0.0.8/iga/doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1179 2023-04-25 22:30:46.000000 iga-0.0.8/iga/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1447 2023-03-28 00:40:16.000000 iga-0.0.8/iga/exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    15031 2023-04-20 00:58:38.000000 iga-0.0.8/iga/github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4901 2023-04-26 04:08:12.000000 iga-0.0.8/iga/id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    16908 2023-04-25 22:30:46.000000 iga-0.0.8/iga/invenio.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2058 2023-04-20 00:58:38.000000 iga-0.0.8/iga/json_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-03-08 23:12:16.000000 iga-0.0.8/iga/licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    69419 2023-05-04 22:41:49.000000 iga-0.0.8/iga/metadata.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    14563 2023-04-26 04:08:12.000000 iga-0.0.8/iga/name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-04-08 02:44:39.000000 iga-0.0.8/iga/orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-04-08 02:44:39.000000 iga-0.0.8/iga/reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-04-08 02:44:39.000000 iga-0.0.8/iga/ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-04-08 02:44:39.000000 iga-0.0.8/iga/text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-04 22:43:34.063622 iga-0.0.8/iga.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)    27417 2023-05-04 22:43:34.000000 iga-0.0.8/iga.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-05-04 22:43:34.000000 iga-0.0.8/iga.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-04 22:43:34.000000 iga-0.0.8/iga.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-05-04 22:43:34.000000 iga-0.0.8/iga.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-04 22:43:34.000000 iga-0.0.8/iga.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-05-04 22:43:34.000000 iga-0.0.8/iga.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-05-04 22:43:34.000000 iga-0.0.8/iga.egg-info/top_level.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-05-04 22:43:34.066542 iga-0.0.8/setup.cfg
+-rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-04-08 01:05:22.000000 iga-0.0.8/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-04 22:43:34.065959 iga-0.0.8/tests/
+-rw-r--r--   0 mhucka     (503) staff       (20)     5734 2023-04-25 22:30:46.000000 iga-0.0.8/tests/test_cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-03-27 19:38:15.000000 iga-0.0.8/tests/test_data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-03-17 23:21:28.000000 iga-0.0.8/tests/test_doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-03-02 15:36:12.000000 iga-0.0.8/tests/test_exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-01-13 03:19:50.000000 iga-0.0.8/tests/test_exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-04-07 01:26:59.000000 iga-0.0.8/tests/test_github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-04-07 01:20:36.000000 iga-0.0.8/tests/test_github_mocks.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3666 2023-04-26 04:08:12.000000 iga-0.0.8/tests/test_id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      641 2022-12-08 00:11:08.000000 iga-0.0.8/tests/test_init.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-04-20 00:58:38.000000 iga-0.0.8/tests/test_is_person.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-03-02 15:16:32.000000 iga-0.0.8/tests/test_licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-04-20 00:58:38.000000 iga-0.0.8/tests/test_name_splitting.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-04-20 00:58:38.000000 iga-0.0.8/tests/test_name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-03-18 00:09:09.000000 iga-0.0.8/tests/test_orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1935 2023-04-08 01:31:14.000000 iga-0.0.8/tests/test_record_from_codemeta.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-03-02 23:04:18.000000 iga-0.0.8/tests/test_reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-03-18 00:05:51.000000 iga-0.0.8/tests/test_ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-04-06 22:54:59.000000 iga-0.0.8/tests/test_text_utils.py
```

### Comparing `iga-0.0.7/LICENSE` & `iga-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/PKG-INFO` & `iga-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 0.0.7
+Version: 0.0.8
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
@@ -22,17 +22,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IGA<img width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
 
 IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a GitHub Action that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
+[![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
 [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
 [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
-[![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?color=b44e88&style=flat-square)](https://github.com/caltechlibrary/iga/releases)
+[![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
 * [Usage](#usage)
@@ -111,21 +112,29 @@
 IGA creates a metadata record in an InvenioRDM server and attaches a GitHub release archive to the record. The GitHub release can be specified using _either_ a full release URL, _or_ a combination of GitHub account + repository + tag. Different command-line options can be used to adjust this behavior.
 
 If the installation process described above is successful, you should end up with a program named `iga` in a location where software is normally installed on your computer.  Running `iga` should be as simple as running any other command-line program. For example, the following command should print a helpful message to your terminal:
 ```shell
 iga --help
 ```
 
-### Specification of the InvenioRDM server and access token
+### Identifying the InvenioRDM server
 
-The server address must be provided either as the value of the option `--invenio-server` or in an environment variable named `INVENIO_SERVER`.  If the server address does not begin with `https://`, IGA will prepended it automatically.
+The server address must be provided either as the value of the option `--invenio-server` or in an environment variable named `INVENIO_SERVER`.  If the server address does not begin with `https://`, IGA will prepend it automatically.
 
-A Personal Access Token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token.
+### Providing an InvenioRDM access token
 
-### Specification of a GitHub release
+A Personal Access Token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
+
+To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
+
+### Providing a GitHub access token
+
+It is possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for many repositories, IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+
+### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
  1. The full URL of the web page on GitHub of a tagged release. In this case,
     the URL must be the final argument on the command line invocation of IGA
     and the options `--account` and `--repo` must be omitted.
  2. A combination of _account name_, _repository name_, and _tag_. In this
     case, the final argument on the command line must be the _tag_, and in
@@ -137,18 +146,14 @@
 ```
 and here's the equivalent using approach #2:
 ```shell
 iga --github-account mhucka --github-repo taupe v1.2.0
 ```
 Note that when using this form of the command, the release tag (`v1.2.0` above) must be the last item given on the command line.
 
-### Use of a GitHub access token
-
-It is possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for many repositories, IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
-
 ### Gathering metadata for an InvenioRDM record
 
 The record created in InvenioRDM is constructed using information obtained using GitHub's API as well as several other APIs as needed. The information includes the following:
  * (if one exists) a `codemeta.json` file in the GitHub repository
  * (if one exists) a `CITATION.cff` file in the GitHub repository
  * data available from GitHub for the release
  * data available from GitHub for the repository
@@ -156,35 +161,35 @@
  * data available from GitHub for the accounts of repository contributors
  * file assets associated with the GitHub release
  * data available from ORCID.org for ORCID identifiers
  * data available from ROR.org for Research Organization Registry identifiers
  * data available from DOI.org, NCBI, Google Books, & others for publications
  * data available from spdx.org for software licenses
 
-IGA tries to use `CodeMeta.json` first and `CITATION.cff` second to fill out the fields of the InvenioRDM record. If neither of those files are present, IGA uses values from the GitHub repository instead. You can make it always use all sources of info with the option `--all-metadata`. Depending on how complete and up-to-date your `CodeMeta.json` and `CITATION.cff` are, this may or may not make the record more comprehensive and may or may not introduce redundancies or unwanted values.
+IGA tries to use [`CodeMeta.json`](https://codemeta.github.io) first and [`CITATION.cff`](https://citation-file-format.github.io) second to fill out the fields of the InvenioRDM record. If neither of those files are present, IGA uses values from the GitHub repository instead. You can make it always use all sources of info with the option `--all-metadata`. Depending on how complete and up-to-date your `CodeMeta.json` and `CITATION.cff` are, this may or may not make the record more comprehensive and may or may not introduce redundancies or unwanted values.
 
 To override the auto-created metadata, use the option `--read-metadata` followed by the path to a JSON file structured according to the InvenioRDM schema used by the destination server. When `--read-metadata` is provided, IGA does _not_ extract the data above, but still obtains the file assets from GitHub.
 
-### Specification of GitHub file assets
+### Specifying GitHub file assets
 
 By default, IGA attaches to the InvenioRDM record _only_ the ZIP file asset created by GitHub for the release. To make IGA attach all assets associated with the GitHub release, use the option `--all-assets`.
 
 To upload specific file assets and override the default selections made by IGA, you can use the option `--file` followed by a path to a file to be uploaded.  You can repeat the option `--file` to upload multiple file assets. Note that if `--file` is provided, then IGA _does not use any file assets from GitHub_; it is the user's responsibility to supply all the files that should be uploaded.
 
 If both `--read-metadata` and `--file` are used, then IGA does not actually contact GitHub for any information.
 
 ### Handling communities
 
 To submit your record to a community, use the `--community` option together with a community name. The option `--list-communities` can be used to get a list of communities supported by the InvenioRDM server. Note that submitting a record to a community means that the record will not be finalized and will not be publicly visible when IGA finishes; instead, the record URL that you receive will be for a draft version, pending review by the community moderators.
 
-### Draft versus published records
+### Indicating draft versus published records
 
 If the `--community` option is not used, then by default, IGA will finalize and publish the record. To make it stop short and leave the record as a draft instead, use the option `--draft`. The draft option also takes precedence over the community option: if you use both `--draft` and `--community`, IGA will stop after creating the draft record and will _not_ submit it to the community.  (You can nevertheless submit the record to a community manually once the draft is created, by visiting the record's web page and using the InvenioRDM interface there.)
 
-### Versioning of records
+### Versioning records
 
 The option `--parent-record` can be used to indicate that the record being constructed is a new version of an existing record. This will make IGA use the InvenioRDM API for [record versioning](https://inveniordm.docs.cern.ch/releases/versions/version-v2.0.0/#versioning-support). The newly-created record will be linked to a parent record identified by the value passed to `--parent-record`. The value must be either an InvenioRDM record identifier (which is a sequence of alphanumeric characters of the form _XXXXX-XXXXX_, such as `bknz4-bch35`, generated by the InvenioRDM server), or a URL to the landing page of the record in the InvenioRDM server. (Note that such URLs end in the record identifier.) Here is an example of using this option:
 ```
 iga --parent-record xbcd4-efgh5 https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
 ### Other options recognized by IGA
@@ -197,15 +202,14 @@
 
 By default, the output of the `verbose` and `debug` run modes is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` to indicate console output, or a file path to send the output to the file.
 
 If given the `--version` option, this program will print its version and other information, and exit without doing anything else.
 
 Running IGA with the option `--help` will make it print help text and exit without doing anything else.
 
-
 ### Summary of command-line options
 
 As explain above, IGA takes one required argument on the command line: either (1) the full URL of a web page on GitHub of a tagged release, or (2) a release tag name which is to be used in combination with options `--github-account` and `--github-repo`. The following table summarizes all the command line options available.
 
 | Long&nbsp;form&nbsp;option&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Short&nbsp;&nbsp; | Meaning | Default |  |
 |------------------------|----------|--------------------------------------|---------|---|
 | `--all-assets`         | `-A`     | Attach all GitHub assets | Attach only the release source ZIP| |
@@ -218,16 +222,16 @@
 | `--github-token` _T_   | `-t` _T_ | Use GitHub acccess token _T_| Use value in env. var. `GITHUB_TOKEN` | |
 | `--help`               | `-h`     | Print help info and exit | | |
 | `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
 | `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
-| `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
 | `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
+| `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
 | `--read-metadata` _R_  | `-R` _R_ | Read metadata record from file _R_; don\'t build one | Build metadata record | |
 | `--save-metadata` _D_  | `-S` _D_ | Save metadata record to file _D_; don\'t upload it | Upload to InvenioRDM server | |
 | `--timeout` _X_        | `-T` _X_ | Wait on network operations a max of _X_ seconds | Auto-adjusted based on file size | |
 | `--version`            | `-V`     | Print program version info and exit | | |
 
 ⚑ &nbsp; Can repeat the option to specify multiple files.<br>
 ⚐ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.<br>
@@ -317,10 +321,10 @@
 * [url-normalize](https://github.com/niksite/url-normalize) &ndash; URI/URL normalization utilities
 * [validators](https://github.com/kvesteri/validators) &ndash; data validation package for Python
 * [wheel](https://pypi.org/project/wheel/) &ndash; setuptools extension for building wheels
 
 <div align="center">
   <br>
   <a href="https://www.caltech.edu">
-    <img width="100" height="100" src="https://github.com/caltechlibrary/iga/blob/main/.graphics/caltech-round.png">
+    <img width="100" height="100" src="https://github.com/caltechlibrary/iga/raw/main/.graphics/caltech-round.png">
   </a>
 </div>
```

### Comparing `iga-0.0.7/README.md` & `iga-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # IGA<img width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
 
 IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a GitHub Action that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
+[![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
 [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
 [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
-[![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?color=b44e88&style=flat-square)](https://github.com/caltechlibrary/iga/releases)
+[![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
 * [Usage](#usage)
@@ -87,21 +88,29 @@
 IGA creates a metadata record in an InvenioRDM server and attaches a GitHub release archive to the record. The GitHub release can be specified using _either_ a full release URL, _or_ a combination of GitHub account + repository + tag. Different command-line options can be used to adjust this behavior.
 
 If the installation process described above is successful, you should end up with a program named `iga` in a location where software is normally installed on your computer.  Running `iga` should be as simple as running any other command-line program. For example, the following command should print a helpful message to your terminal:
 ```shell
 iga --help
 ```
 
-### Specification of the InvenioRDM server and access token
+### Identifying the InvenioRDM server
 
-The server address must be provided either as the value of the option `--invenio-server` or in an environment variable named `INVENIO_SERVER`.  If the server address does not begin with `https://`, IGA will prepended it automatically.
+The server address must be provided either as the value of the option `--invenio-server` or in an environment variable named `INVENIO_SERVER`.  If the server address does not begin with `https://`, IGA will prepend it automatically.
 
-A Personal Access Token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token.
+### Providing an InvenioRDM access token
 
-### Specification of a GitHub release
+A Personal Access Token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
+
+To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
+
+### Providing a GitHub access token
+
+It is possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for many repositories, IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+
+### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
  1. The full URL of the web page on GitHub of a tagged release. In this case,
     the URL must be the final argument on the command line invocation of IGA
     and the options `--account` and `--repo` must be omitted.
  2. A combination of _account name_, _repository name_, and _tag_. In this
     case, the final argument on the command line must be the _tag_, and in
@@ -113,18 +122,14 @@
 ```
 and here's the equivalent using approach #2:
 ```shell
 iga --github-account mhucka --github-repo taupe v1.2.0
 ```
 Note that when using this form of the command, the release tag (`v1.2.0` above) must be the last item given on the command line.
 
-### Use of a GitHub access token
-
-It is possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for many repositories, IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
-
 ### Gathering metadata for an InvenioRDM record
 
 The record created in InvenioRDM is constructed using information obtained using GitHub's API as well as several other APIs as needed. The information includes the following:
  * (if one exists) a `codemeta.json` file in the GitHub repository
  * (if one exists) a `CITATION.cff` file in the GitHub repository
  * data available from GitHub for the release
  * data available from GitHub for the repository
@@ -132,35 +137,35 @@
  * data available from GitHub for the accounts of repository contributors
  * file assets associated with the GitHub release
  * data available from ORCID.org for ORCID identifiers
  * data available from ROR.org for Research Organization Registry identifiers
  * data available from DOI.org, NCBI, Google Books, & others for publications
  * data available from spdx.org for software licenses
 
-IGA tries to use `CodeMeta.json` first and `CITATION.cff` second to fill out the fields of the InvenioRDM record. If neither of those files are present, IGA uses values from the GitHub repository instead. You can make it always use all sources of info with the option `--all-metadata`. Depending on how complete and up-to-date your `CodeMeta.json` and `CITATION.cff` are, this may or may not make the record more comprehensive and may or may not introduce redundancies or unwanted values.
+IGA tries to use [`CodeMeta.json`](https://codemeta.github.io) first and [`CITATION.cff`](https://citation-file-format.github.io) second to fill out the fields of the InvenioRDM record. If neither of those files are present, IGA uses values from the GitHub repository instead. You can make it always use all sources of info with the option `--all-metadata`. Depending on how complete and up-to-date your `CodeMeta.json` and `CITATION.cff` are, this may or may not make the record more comprehensive and may or may not introduce redundancies or unwanted values.
 
 To override the auto-created metadata, use the option `--read-metadata` followed by the path to a JSON file structured according to the InvenioRDM schema used by the destination server. When `--read-metadata` is provided, IGA does _not_ extract the data above, but still obtains the file assets from GitHub.
 
-### Specification of GitHub file assets
+### Specifying GitHub file assets
 
 By default, IGA attaches to the InvenioRDM record _only_ the ZIP file asset created by GitHub for the release. To make IGA attach all assets associated with the GitHub release, use the option `--all-assets`.
 
 To upload specific file assets and override the default selections made by IGA, you can use the option `--file` followed by a path to a file to be uploaded.  You can repeat the option `--file` to upload multiple file assets. Note that if `--file` is provided, then IGA _does not use any file assets from GitHub_; it is the user's responsibility to supply all the files that should be uploaded.
 
 If both `--read-metadata` and `--file` are used, then IGA does not actually contact GitHub for any information.
 
 ### Handling communities
 
 To submit your record to a community, use the `--community` option together with a community name. The option `--list-communities` can be used to get a list of communities supported by the InvenioRDM server. Note that submitting a record to a community means that the record will not be finalized and will not be publicly visible when IGA finishes; instead, the record URL that you receive will be for a draft version, pending review by the community moderators.
 
-### Draft versus published records
+### Indicating draft versus published records
 
 If the `--community` option is not used, then by default, IGA will finalize and publish the record. To make it stop short and leave the record as a draft instead, use the option `--draft`. The draft option also takes precedence over the community option: if you use both `--draft` and `--community`, IGA will stop after creating the draft record and will _not_ submit it to the community.  (You can nevertheless submit the record to a community manually once the draft is created, by visiting the record's web page and using the InvenioRDM interface there.)
 
-### Versioning of records
+### Versioning records
 
 The option `--parent-record` can be used to indicate that the record being constructed is a new version of an existing record. This will make IGA use the InvenioRDM API for [record versioning](https://inveniordm.docs.cern.ch/releases/versions/version-v2.0.0/#versioning-support). The newly-created record will be linked to a parent record identified by the value passed to `--parent-record`. The value must be either an InvenioRDM record identifier (which is a sequence of alphanumeric characters of the form _XXXXX-XXXXX_, such as `bknz4-bch35`, generated by the InvenioRDM server), or a URL to the landing page of the record in the InvenioRDM server. (Note that such URLs end in the record identifier.) Here is an example of using this option:
 ```
 iga --parent-record xbcd4-efgh5 https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
 ### Other options recognized by IGA
@@ -173,15 +178,14 @@
 
 By default, the output of the `verbose` and `debug` run modes is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` to indicate console output, or a file path to send the output to the file.
 
 If given the `--version` option, this program will print its version and other information, and exit without doing anything else.
 
 Running IGA with the option `--help` will make it print help text and exit without doing anything else.
 
-
 ### Summary of command-line options
 
 As explain above, IGA takes one required argument on the command line: either (1) the full URL of a web page on GitHub of a tagged release, or (2) a release tag name which is to be used in combination with options `--github-account` and `--github-repo`. The following table summarizes all the command line options available.
 
 | Long&nbsp;form&nbsp;option&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Short&nbsp;&nbsp; | Meaning | Default |  |
 |------------------------|----------|--------------------------------------|---------|---|
 | `--all-assets`         | `-A`     | Attach all GitHub assets | Attach only the release source ZIP| |
@@ -194,16 +198,16 @@
 | `--github-token` _T_   | `-t` _T_ | Use GitHub acccess token _T_| Use value in env. var. `GITHUB_TOKEN` | |
 | `--help`               | `-h`     | Print help info and exit | | |
 | `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
 | `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
-| `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
 | `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
+| `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
 | `--read-metadata` _R_  | `-R` _R_ | Read metadata record from file _R_; don\'t build one | Build metadata record | |
 | `--save-metadata` _D_  | `-S` _D_ | Save metadata record to file _D_; don\'t upload it | Upload to InvenioRDM server | |
 | `--timeout` _X_        | `-T` _X_ | Wait on network operations a max of _X_ seconds | Auto-adjusted based on file size | |
 | `--version`            | `-V`     | Print program version info and exit | | |
 
 ⚑ &nbsp; Can repeat the option to specify multiple files.<br>
 ⚐ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.<br>
@@ -293,10 +297,10 @@
 * [url-normalize](https://github.com/niksite/url-normalize) &ndash; URI/URL normalization utilities
 * [validators](https://github.com/kvesteri/validators) &ndash; data validation package for Python
 * [wheel](https://pypi.org/project/wheel/) &ndash; setuptools extension for building wheels
 
 <div align="center">
   <br>
   <a href="https://www.caltech.edu">
-    <img width="100" height="100" src="https://github.com/caltechlibrary/iga/blob/main/.graphics/caltech-round.png">
+    <img width="100" height="100" src="https://github.com/caltechlibrary/iga/raw/main/.graphics/caltech-round.png">
   </a>
 </div>
```

### Comparing `iga-0.0.7/iga/__init__.py` & `iga-0.0.8/iga/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # .............................................................................
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '0.0.7'
+__version__     = '0.0.8'
 __description__ = 'InvenioRDM GitHub Archiver'
 __url__         = 'https://github.com/caltechlibrary/iga'
 __author__      = 'Michael Hucka'
 __email__       = 'helpdesk@library.caltech.edu'
 __license__     = 'https://github.com/caltechlibrary/iga/blob/main/LICENSE'
```

### Comparing `iga-0.0.7/iga/__main__.py` & `iga-0.0.8/iga/__main__.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/iga/cli.py` & `iga-0.0.8/iga/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,14 +637,20 @@
             _inform(' done.')
 
         if dest:
             import json
             dest.write(json.dumps(metadata, indent=2))
             dest.write('\n')
             _inform(f'Wrote metadata to {dest.name}.')
+
+            if open_in_browser:
+                from os import path
+                file = path.realpath(dest.name)
+                log(f'opening {file}')
+                click.launch(file)
         else:
             _inform('Sending metadata to InvenioRDM server', end='...')
             record = invenio_create(metadata, parent_id)
             _inform(' done.')
 
             _inform('Attaching assets:')
             for item in files_to_upload or github_assets:
@@ -656,20 +662,21 @@
             elif community:
                 invenio_community_send(record, community)
                 _inform(f'The record has been submitted to community "{community}"'
                         f' and the draft is available at {record.draft_url}')
             else:
                 invenio_publish(record)
                 _inform(f'The published record is available at {record.record_url}')
-        if os.environ.get('IGA_RUN_MODE') == 'quiet':
-            # In quiet mode nothing else will be printed, so we finish with this
-            click.echo(record.record_url or record.draft_url)
-        if open_in_browser:
-            log(f'opening {record.record_url or record.draft_url}')
-            click.launch(record.record_url or record.draft_url)
+
+            if os.environ.get('IGA_RUN_MODE') == 'quiet':
+                # Quiet mode => nothing else is printed, so tell user this much.
+                click.echo(record.record_url or record.draft_url)
+            if open_in_browser:
+                log(f'opening {record.record_url or record.draft_url}')
+                click.launch(record.record_url or record.draft_url)
     except KeyboardInterrupt:
         log('keyboard interrupt received')
         exit_code = ExitCode.user_interrupt
     except bdb.BdbQuit:
         # Exiting the debugger. Not a real exception.
         pass
     except Exception as ex:             # noqa: PIE786
```

### Comparing `iga-0.0.7/iga/data_utils.py` & `iga-0.0.8/iga/data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/iga/doi.py` & `iga-0.0.8/iga/doi.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/iga/exceptions.py` & `iga-0.0.8/iga/exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/iga/exit_codes.py` & `iga-0.0.8/iga/exit_codes.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/iga/github.py` & `iga-0.0.8/iga/github.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/iga/id_utils.py` & `iga-0.0.8/iga/id_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,35 +32,37 @@
 
 rdm_regex = re.compile(r'([abcdefghjkmnpqrstvwxyz0-9]{5}-[abcdefghjkmnpqrstvwxyz0-9]{5})')
 '''Matches an InvenioRDM record id.'''
 
 
 def is_invenio_rdm(val):
     '''Return True if the given string is an InvenioRDM record identifier.'''
-    return normalize_invenio_rdm(val)
+    return bool(normalize_invenio_rdm(val))
 
 
 def normalize_invenio_rdm(val):
     '''Normalize an InvenioRDM record identifier.
 
     This accepts a URL that contains an InvenioRDM record identifier if the
     URL has one of the following forms:
 
        https://servername.domain/records/xxxxx-xxxxx
-       https://servername.domain/records/xxxxx-xxxxx/draft
+       https://servername.domain/uploads/xxxxx-xxxxx
 
     If the value is not actually an InvenioRDM identifier or a URL for a
     record containing the record identifier, this will return an empty string.
     '''
     candidate = val
     if val.startswith('http'):
+        val = val.split('?')[0]         # Remove stuff like &preview=1.
+        val = val.removesuffix('/draft')
         url_parts = val.split('/')
-        if url_parts[-2] != 'records' and url_parts[-3] != 'records':
+        if len(url_parts) < 2 or url_parts[-2] not in ['records', 'uploads']:
             return ''
-        candidate = url_parts[-2] if val.endswith('/draft') else url_parts[-1]
+        candidate = url_parts[-1]
     m = rdm_regex.match(candidate)
     return m.group(1) if m else ''
 
 
 # The idutils regular expression for PMCID doesn't have a capturing expression
 # and also, idutils lacks a "normalize_X()" for pmcid, for some reason.
 PMCID_REGEX = re.compile(r"(PMC\d{6,8})", flags=re.IGNORECASE)
@@ -162,12 +164,10 @@
         return 'rdm'
     for scheme in detect_identifier_schemes(text):
         if scheme in RECOGNIZED_SCHEMES:
             return scheme
     else:
         # Special case not handled well by idutils. PMID's are a particular
         # PITA b/c they're integers & cause false-positives for other things.
-        if contains_pmcid(text):
-            return 'pmcid'
-        elif is_pmid(text):
+        if is_pmid(text):
             return 'pmid'
     return None
```

### Comparing `iga-0.0.7/iga/invenio.py` & `iga-0.0.8/iga/invenio.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/iga/json_utils.py` & `iga-0.0.8/iga/json_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/iga/licenses.py` & `iga-0.0.8/iga/licenses.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/iga/metadata.py` & `iga-0.0.8/iga/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     "locations",
     "publication_date",
     "publisher",
     "references",
     "related_identifiers",
     "resource_type",
     "rights",
-#    "sizes",,            # 2023-03-23 not clear we need this. Skip for now.
+#    "sizes",             # 2023-03-23 not clear we need this. Skip for now.
     "subjects",
     "title",
     "version",
 ]
 
 # Not all of these need to be provided.  Based on the test cases in
 # https://github.com/inveniosoftware/invenio-rdm-records, the minimum set of
@@ -1404,15 +1404,15 @@
                              'type': 'personal'}
 
     else:
         name = account.name.strip() if account.name else ''
         person_or_org = {'name': name,
                          'type': 'organizational'}
     result = {'person_or_org': person_or_org}
-    if account.company:
+    if account.company and account.type == 'User':
         account.company = account.company.strip()
         if account.company.startswith('@'):
             # Some people write @foo to indicate org account "foo" in GitHub.
             # Grab only the first token after the '@'.
             log(f'company for {account.login} account starts with @')
             try:
                 import re
```

### Comparing `iga-0.0.7/iga/name_utils.py` & `iga-0.0.8/iga/name_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,17 +340,18 @@
     return ' '.join(word[0].upper() + word[1:] for word in name.split())
 
 
 def _load_organizations():
     global _ORGANIZATIONS
     from os.path import dirname, abspath, join
     import pickle
-    log(f'loading data/{_ORGANIZATIONS_FILENAME} – this may take some time')
     here = dirname(abspath(__file__))
-    with open(join(here, f'data/{_ORGANIZATIONS_FILENAME}'), 'rb') as f:
+    org_file = join(here, f'data/{_ORGANIZATIONS_FILENAME}')
+    log(f'loading {org_file} – this may take some time')
+    with open(org_file, 'rb') as f:
         _ORGANIZATIONS = pickle.load(f)
 
 
 def _load_spacy(charset):
     global _NLP
     import spacy
     model = 'zh_core_web_trf' if charset == 'cjk' else 'en_core_web_trf'
```

### Comparing `iga-0.0.7/iga/orcid.py` & `iga-0.0.8/iga/orcid.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/iga/reference.py` & `iga-0.0.8/iga/reference.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/iga/ror.py` & `iga-0.0.8/iga/ror.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/iga/text_utils.py` & `iga-0.0.8/iga/text_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/iga.egg-info/PKG-INFO` & `iga-0.0.8/iga.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 0.0.7
+Version: 0.0.8
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
@@ -22,17 +22,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IGA<img width="12%" align="right" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/cloud-upload.png">
 
 IGA is the _InvenioRDM GitHub Archiver_, a standalone program as well as a GitHub Action that lets you automatically archive GitHub software releases in an [InvenioRDM](https://inveniosoftware.org/products/rdm/) repository.
 
+[![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?style=flat-square&color=b44e88&label=Latest%20release)](https://github.com/caltechlibrary/iga/releases)
 [![License](https://img.shields.io/badge/License-BSD--like-lightgrey.svg?style=flat-square)](https://github.com/caltechlibrary/iga/LICENSE)
 [![Python](https://img.shields.io/badge/Python-3.9+-brightgreen.svg?style=flat-square)](https://www.python.org/downloads/release/python-390/)
-[![Latest release](https://img.shields.io/github/v/release/caltechlibrary/iga.svg?color=b44e88&style=flat-square)](https://github.com/caltechlibrary/iga/releases)
+[![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
 * [Usage](#usage)
@@ -111,21 +112,29 @@
 IGA creates a metadata record in an InvenioRDM server and attaches a GitHub release archive to the record. The GitHub release can be specified using _either_ a full release URL, _or_ a combination of GitHub account + repository + tag. Different command-line options can be used to adjust this behavior.
 
 If the installation process described above is successful, you should end up with a program named `iga` in a location where software is normally installed on your computer.  Running `iga` should be as simple as running any other command-line program. For example, the following command should print a helpful message to your terminal:
 ```shell
 iga --help
 ```
 
-### Specification of the InvenioRDM server and access token
+### Identifying the InvenioRDM server
 
-The server address must be provided either as the value of the option `--invenio-server` or in an environment variable named `INVENIO_SERVER`.  If the server address does not begin with `https://`, IGA will prepended it automatically.
+The server address must be provided either as the value of the option `--invenio-server` or in an environment variable named `INVENIO_SERVER`.  If the server address does not begin with `https://`, IGA will prepend it automatically.
 
-A Personal Access Token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token.
+### Providing an InvenioRDM access token
 
-### Specification of a GitHub release
+A Personal Access Token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
+
+To obtain a PAT from an InvenioRDM server, first log in to the server, then visit the page at `/account/settings/applications` and use the interface there to create a token. The token will be a long string of alphanumeric characters such as `OH0KYf4PGYQGnCM4b53ejSGicOC4s4YnonRVzGJbWxY`; set the value of the variable `INVENIO_TOKEN` to this string.
+
+### Providing a GitHub access token
+
+It is possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for many repositories, IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
+
+### Specifying a GitHub release
 
 A GitHub release can be specified to IGA in one of two mutually-exclusive ways:
  1. The full URL of the web page on GitHub of a tagged release. In this case,
     the URL must be the final argument on the command line invocation of IGA
     and the options `--account` and `--repo` must be omitted.
  2. A combination of _account name_, _repository name_, and _tag_. In this
     case, the final argument on the command line must be the _tag_, and in
@@ -137,18 +146,14 @@
 ```
 and here's the equivalent using approach #2:
 ```shell
 iga --github-account mhucka --github-repo taupe v1.2.0
 ```
 Note that when using this form of the command, the release tag (`v1.2.0` above) must be the last item given on the command line.
 
-### Use of a GitHub access token
-
-It is possible to run IGA without providing a GitHub access token. GitHub allows up to 60 API calls per minute when running without credentials, and though IGA makes several API calls to GitHub each time it runs, for many repositories, IGA will not hit the limit. However, if you run IGA multiple times in a row or your repository has many contributors, then you may need to supply a GitHub access token. The preferred way of doing that is to set the value of the environment variable `GITHUB_TOKEN`. Alternatively, you can use the option `--github-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.  To obtain a PAT from GitHub, visit https://docs.github.com/en/authentication and follow the instructions for creating a "classic" personal access token.
-
 ### Gathering metadata for an InvenioRDM record
 
 The record created in InvenioRDM is constructed using information obtained using GitHub's API as well as several other APIs as needed. The information includes the following:
  * (if one exists) a `codemeta.json` file in the GitHub repository
  * (if one exists) a `CITATION.cff` file in the GitHub repository
  * data available from GitHub for the release
  * data available from GitHub for the repository
@@ -156,35 +161,35 @@
  * data available from GitHub for the accounts of repository contributors
  * file assets associated with the GitHub release
  * data available from ORCID.org for ORCID identifiers
  * data available from ROR.org for Research Organization Registry identifiers
  * data available from DOI.org, NCBI, Google Books, & others for publications
  * data available from spdx.org for software licenses
 
-IGA tries to use `CodeMeta.json` first and `CITATION.cff` second to fill out the fields of the InvenioRDM record. If neither of those files are present, IGA uses values from the GitHub repository instead. You can make it always use all sources of info with the option `--all-metadata`. Depending on how complete and up-to-date your `CodeMeta.json` and `CITATION.cff` are, this may or may not make the record more comprehensive and may or may not introduce redundancies or unwanted values.
+IGA tries to use [`CodeMeta.json`](https://codemeta.github.io) first and [`CITATION.cff`](https://citation-file-format.github.io) second to fill out the fields of the InvenioRDM record. If neither of those files are present, IGA uses values from the GitHub repository instead. You can make it always use all sources of info with the option `--all-metadata`. Depending on how complete and up-to-date your `CodeMeta.json` and `CITATION.cff` are, this may or may not make the record more comprehensive and may or may not introduce redundancies or unwanted values.
 
 To override the auto-created metadata, use the option `--read-metadata` followed by the path to a JSON file structured according to the InvenioRDM schema used by the destination server. When `--read-metadata` is provided, IGA does _not_ extract the data above, but still obtains the file assets from GitHub.
 
-### Specification of GitHub file assets
+### Specifying GitHub file assets
 
 By default, IGA attaches to the InvenioRDM record _only_ the ZIP file asset created by GitHub for the release. To make IGA attach all assets associated with the GitHub release, use the option `--all-assets`.
 
 To upload specific file assets and override the default selections made by IGA, you can use the option `--file` followed by a path to a file to be uploaded.  You can repeat the option `--file` to upload multiple file assets. Note that if `--file` is provided, then IGA _does not use any file assets from GitHub_; it is the user's responsibility to supply all the files that should be uploaded.
 
 If both `--read-metadata` and `--file` are used, then IGA does not actually contact GitHub for any information.
 
 ### Handling communities
 
 To submit your record to a community, use the `--community` option together with a community name. The option `--list-communities` can be used to get a list of communities supported by the InvenioRDM server. Note that submitting a record to a community means that the record will not be finalized and will not be publicly visible when IGA finishes; instead, the record URL that you receive will be for a draft version, pending review by the community moderators.
 
-### Draft versus published records
+### Indicating draft versus published records
 
 If the `--community` option is not used, then by default, IGA will finalize and publish the record. To make it stop short and leave the record as a draft instead, use the option `--draft`. The draft option also takes precedence over the community option: if you use both `--draft` and `--community`, IGA will stop after creating the draft record and will _not_ submit it to the community.  (You can nevertheless submit the record to a community manually once the draft is created, by visiting the record's web page and using the InvenioRDM interface there.)
 
-### Versioning of records
+### Versioning records
 
 The option `--parent-record` can be used to indicate that the record being constructed is a new version of an existing record. This will make IGA use the InvenioRDM API for [record versioning](https://inveniordm.docs.cern.ch/releases/versions/version-v2.0.0/#versioning-support). The newly-created record will be linked to a parent record identified by the value passed to `--parent-record`. The value must be either an InvenioRDM record identifier (which is a sequence of alphanumeric characters of the form _XXXXX-XXXXX_, such as `bknz4-bch35`, generated by the InvenioRDM server), or a URL to the landing page of the record in the InvenioRDM server. (Note that such URLs end in the record identifier.) Here is an example of using this option:
 ```
 iga --parent-record xbcd4-efgh5 https://github.com/mhucka/taupe/releases/tag/v1.2.0
 ```
 
 ### Other options recognized by IGA
@@ -197,15 +202,14 @@
 
 By default, the output of the `verbose` and `debug` run modes is sent to the standard output (normally the terminal console). The option `--log-dest` can be used to send the output to the given destination instead. The value can be `-` to indicate console output, or a file path to send the output to the file.
 
 If given the `--version` option, this program will print its version and other information, and exit without doing anything else.
 
 Running IGA with the option `--help` will make it print help text and exit without doing anything else.
 
-
 ### Summary of command-line options
 
 As explain above, IGA takes one required argument on the command line: either (1) the full URL of a web page on GitHub of a tagged release, or (2) a release tag name which is to be used in combination with options `--github-account` and `--github-repo`. The following table summarizes all the command line options available.
 
 | Long&nbsp;form&nbsp;option&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Short&nbsp;&nbsp; | Meaning | Default |  |
 |------------------------|----------|--------------------------------------|---------|---|
 | `--all-assets`         | `-A`     | Attach all GitHub assets | Attach only the release source ZIP| |
@@ -218,16 +222,16 @@
 | `--github-token` _T_   | `-t` _T_ | Use GitHub acccess token _T_| Use value in env. var. `GITHUB_TOKEN` | |
 | `--help`               | `-h`     | Print help info and exit | | |
 | `--invenio-server` _S_ | `-s` _S_ | Send record to InvenioRDM server at address _S_ | Use value in env. var. `INVENIO_SERVER` | | 
 | `--invenio-token` _K_  | `-k` _K_ | Use InvenioRDM access token _K_ | Use value in env. var. `INVENIO_TOKEN` | | 
 | `--list-communities`   | `-L`     | List communities available for use with `--community` | | |
 | `--log-dest` _L_       | `-l` _L_ | Write log output to destination _L_ | Write to terminal | ⚐ |
 | `--mode` _M_           | `-m` _M_ | Run in mode `quiet`, `normal`, `verbose`, or `debug` | `normal` | |
-| `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
 | `--open`               | `-o`     | Open record's web page in a browser when done | Do nothing when done | |
+| `--parent-record` _N_  | `-p` _N_ | Make this a new version of existing record _N_ | New record is unrelated to other records | ❖ |
 | `--read-metadata` _R_  | `-R` _R_ | Read metadata record from file _R_; don\'t build one | Build metadata record | |
 | `--save-metadata` _D_  | `-S` _D_ | Save metadata record to file _D_; don\'t upload it | Upload to InvenioRDM server | |
 | `--timeout` _X_        | `-T` _X_ | Wait on network operations a max of _X_ seconds | Auto-adjusted based on file size | |
 | `--version`            | `-V`     | Print program version info and exit | | |
 
 ⚑ &nbsp; Can repeat the option to specify multiple files.<br>
 ⚐ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.<br>
@@ -317,10 +321,10 @@
 * [url-normalize](https://github.com/niksite/url-normalize) &ndash; URI/URL normalization utilities
 * [validators](https://github.com/kvesteri/validators) &ndash; data validation package for Python
 * [wheel](https://pypi.org/project/wheel/) &ndash; setuptools extension for building wheels
 
 <div align="center">
   <br>
   <a href="https://www.caltech.edu">
-    <img width="100" height="100" src="https://github.com/caltechlibrary/iga/blob/main/.graphics/caltech-round.png">
+    <img width="100" height="100" src="https://github.com/caltechlibrary/iga/raw/main/.graphics/caltech-round.png">
   </a>
 </div>
```

### Comparing `iga-0.0.7/iga.egg-info/SOURCES.txt` & `iga-0.0.8/iga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/iga.egg-info/requires.txt` & `iga-0.0.8/iga.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/setup.cfg` & `iga-0.0.8/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iga
-version = 0.0.7
+version = 0.0.8
 description = InvenioRDM GitHub Archiver
 author = Michael Hucka
 author_email = helpdesk@library.caltech.edu
 license = https://github.com/caltechlibrary/iga/blob/main/LICENSE
 license_files = LICENSE
 url = https://github.com/caltechlibrary/iga
 project_urls =
```

### Comparing `iga-0.0.7/setup.py` & `iga-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_cli.py` & `iga-0.0.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_data_utils.py` & `iga-0.0.8/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_doi.py` & `iga-0.0.8/tests/test_doi.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_exceptions.py` & `iga-0.0.8/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_github.py` & `iga-0.0.8/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_github_mocks.py` & `iga-0.0.8/tests/test_github_mocks.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_id_utils.py` & `iga-0.0.8/tests/test_id_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,33 +7,39 @@
 # =============================================================================
 
 from iga.id_utils import (
     contains_pmcid,
     detected_id,
     normalize_pmcid,
     recognized_scheme,
+    is_invenio_rdm,
 )
 
 sample_ids = [
-    ('arXiv:2012.13117v1'            , 'arxiv'),
-    ('10.48550/arXiv.2012.13117'     , 'doi'),
-    ('PMC4908318'                    , 'pmcid'),
-    ('26861819'                      , 'pmid'),
-    ('10.1093/bioinformatics/btw056' , 'doi'),
-    ('10.1007/978-1-4939-3283-2_19'  , 'doi'),
-    ('10.1103/PhysRevD.90.124021'    , 'doi'),
-    ('26677194'                      , 'pmid'),
-    ('978-0982477373'                , 'isbn'),
-    ('9780898714128'                 , 'isbn'),
-    ('9781979381208'                 , 'isbn'),
-    ('978-65-87773-12-4'             , 'isbn'),
-    ('04dkp9463'                     , 'ror'),
-    ('swh:1:cnt:94a9ed024d3859793618152ea559a168bbcbb5e2', 'swh'),
-    ('bknz4-bch35'                   , 'rdm'),
-    ('ry4vm-wny44'                   , 'rdm'),
+    ('arXiv:2012.13117v1'                                 , 'arxiv'),
+    ('10.48550/arXiv.2012.13117'                          , 'doi'),
+    ('PMC4908318'                                         , 'pmcid'),
+    ('26861819'                                           , 'pmid'),
+    ('18183754'                                           , 'pmid'),
+    ('10.1093/bioinformatics/btw056'                      , 'doi'),
+    ('10.1007/978-1-4939-3283-2_19'                       , 'doi'),
+    ('10.1103/PhysRevD.90.124021'                         , 'doi'),
+    ('26677194'                                           , 'pmid'),
+    ('978-0982477373'                                     , 'isbn'),
+    ('9780898714128'                                      , 'isbn'),
+    ('9781979381208'                                      , 'isbn'),
+    ('978-65-87773-12-4'                                  , 'isbn'),
+    ('04dkp9463'                                          , 'ror'),
+    ('swh:1:cnt:94a9ed024d3859793618152ea559a168bbcbb5e2' , 'swh'),
+    ('bknz4-bch35'                                        , 'rdm'),
+    ('ry4vm-wny44'                                        , 'rdm'),
+    ('https://a.b/records/ry4vm-wny44'                    , 'rdm'),
+    ('https://a.b/records/jx193-a0e45?preview=1'          , 'rdm'),
+    ('https://a.b/uploads/ry4vm-wny44'                    , 'rdm'),
+    ('https://a.b/something/ry4vm-wny44'                  , 'url'),
 ]
 
 
 def test_contains_pmcid():
     for _id, scheme in sample_ids:
         if scheme == 'pmcid':
             assert contains_pmcid(_id)
@@ -45,24 +51,33 @@
 
 def test_recognized_scheme():
     for _id, scheme in sample_ids:
         assert recognized_scheme(_id) == scheme
 
 
 sample_unnormalized_ids = [
-    ('http://orcid.org/0000-0001-9105-5960'    , '0000-0001-9105-5960'),
-    ('https://doi.org/10.5281/zenodo.1095472'  , '10.5281/zenodo.1095472'),
-    ('https://ror.org/027m9bs27'               , '027m9bs27'),
-    ('10.1088/0264-9381/26/22/225003'          , '10.1088/0264-9381/26/22/225003'),
-    ('PMCID; PMC4908318'                       , ''),
-    ('pmc4908318'                              , 'PMC4908318'),
-    ('https://ror.org/04dkp9463'               , '04dkp9463'),
-    ('https://a.b/records/ry4vm-wny44'         , 'ry4vm-wny44'),
-    ('https://a.b/records/ry4vm-wny44/draft'   , 'ry4vm-wny44'),
-    # If it's not detected as an RDM record id, it's considered to be just a URL.
-    ('https://a.b/something/ry4vm-wny44/draft' , 'https://a.b/something/ry4vm-wny44/draft'),
+    ('http://orcid.org/0000-0001-9105-5960'      , '0000-0001-9105-5960'),
+    ('https://doi.org/10.5281/zenodo.1095472'    , '10.5281/zenodo.1095472'),
+    ('https://ror.org/027m9bs27'                 , '027m9bs27'),
+    ('10.1088/0264-9381/26/22/225003'            , '10.1088/0264-9381/26/22/225003'),
+    ('PMCID; PMC4908318'                         , ''),
+    ('22110403'                                  , '22110403'),
+    ('pmc4908318'                                , 'PMC4908318'),
+    ('PMC3217025'                                , 'PMC3217025'),
+    ('https://ror.org/04dkp9463'                 , '04dkp9463'),
+    ('https://a.b/records/ry4vm-wny44'           , 'ry4vm-wny44'),
+    ('https://a.b/records/ry4vm-wny44?preview=1' , 'ry4vm-wny44'),
+    ('https://a.b/records/ry4vm-wny44/draft'     , 'ry4vm-wny44'),
+    ('https://a.b/uploads/ry4vm-wny44'           , 'ry4vm-wny44'),
+    # If it's not detected as an RDM record id   , it's considered to be just a URL.
+    ('https://a.b/something/ry4vm-wny44'         , 'https://a.b/something/ry4vm-wny44'),
 ]
 
 
 def test_detected_id():
     for text, id_ in sample_unnormalized_ids:
         assert detected_id(text) == id_
+
+
+def test_is_invenio_rdm():
+    assert is_invenio_rdm('https://a.b/records/ry4vm-wny44')
+    assert not is_invenio_rdm('https://a.b/something/ry4vm-wny44')
```

### Comparing `iga-0.0.7/tests/test_init.py` & `iga-0.0.8/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_is_person.py` & `iga-0.0.8/tests/test_is_person.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_licenses.py` & `iga-0.0.8/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_name_splitting.py` & `iga-0.0.8/tests/test_name_splitting.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_name_utils.py` & `iga-0.0.8/tests/test_name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_orcid.py` & `iga-0.0.8/tests/test_orcid.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_record_from_codemeta.py` & `iga-0.0.8/tests/test_record_from_codemeta.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_reference.py` & `iga-0.0.8/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_ror.py` & `iga-0.0.8/tests/test_ror.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.7/tests/test_text_utils.py` & `iga-0.0.8/tests/test_text_utils.py`

 * *Files identical despite different names*

