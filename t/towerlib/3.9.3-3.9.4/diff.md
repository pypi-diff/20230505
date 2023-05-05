# Comparing `tmp/towerlib-3.9.3.tar.gz` & `tmp/towerlib-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/towerlib-3.9.3.tar", last modified: Mon Jul 11 09:36:57 2022, max compression
+gzip compressed data, was "dist/towerlib-3.9.4.tar", last modified: Thu Sep  1 12:03:38 2022, max compression
```

## Comparing `towerlib-3.9.3.tar` & `towerlib-3.9.4.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-07-11 09:36:57.000000 towerlib-3.9.3/
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        5 2022-07-11 08:40:26.000000 towerlib-3.9.3/.VERSION
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      578 2022-04-19 14:36:54.000000 towerlib-3.9.3/AUTHORS.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1122 2020-07-09 07:01:14.000000 towerlib-3.9.3/CONTRIBUTING.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     4780 2022-07-11 08:40:35.000000 towerlib-3.9.3/HISTORY.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1063 2020-07-09 07:01:14.000000 towerlib-3.9.3/LICENSE
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      390 2020-07-09 07:01:14.000000 towerlib-3.9.3/MANIFEST.in
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    10878 2022-07-11 09:36:57.000000 towerlib-3.9.3/PKG-INFO
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      644 2021-04-26 11:07:44.000000 towerlib-3.9.3/Pipfile
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    49399 2022-07-11 09:36:56.000000 towerlib-3.9.3/Pipfile.lock
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2539 2020-07-09 07:01:14.000000 towerlib-3.9.3/README.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     3101 2021-04-26 07:04:39.000000 towerlib-3.9.3/USAGE.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      601 2022-07-11 09:36:57.000000 towerlib-3.9.3/dev-requirements.txt
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-07-11 09:36:57.000000 towerlib-3.9.3/docs/
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     6770 2020-07-09 07:01:14.000000 towerlib-3.9.3/docs/Makefile
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       28 2020-07-09 07:01:14.000000 towerlib-3.9.3/docs/authors.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     8894 2020-07-09 07:01:14.000000 towerlib-3.9.3/docs/conf.py
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       33 2020-07-09 07:01:14.000000 towerlib-3.9.3/docs/contributing.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       28 2020-07-09 07:01:14.000000 towerlib-3.9.3/docs/history.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      498 2020-07-09 07:01:14.000000 towerlib-3.9.3/docs/index.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)       33 2020-07-09 07:01:14.000000 towerlib-3.9.3/docs/installation.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)       61 2021-07-01 06:10:42.000000 towerlib-3.9.3/docs/modules.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       27 2020-07-09 07:01:14.000000 towerlib-3.9.3/docs/readme.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3035 2021-07-01 06:10:42.000000 towerlib-3.9.3/docs/towerlib.entities.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      542 2020-07-09 07:01:14.000000 towerlib-3.9.3/docs/towerlib.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       26 2020-07-09 07:01:14.000000 towerlib-3.9.3/docs/usage.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      452 2022-07-11 09:36:57.000000 towerlib-3.9.3/requirements.txt
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      148 2022-07-11 09:36:57.000000 towerlib-3.9.3/setup.cfg
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1973 2020-07-09 07:01:14.000000 towerlib-3.9.3/setup.py
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-07-11 09:36:57.000000 towerlib-3.9.3/tests/
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-07-11 09:36:57.000000 towerlib-3.9.3/tests/integration/
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3295 2020-07-09 07:01:14.000000 towerlib-3.9.3/tests/integration/__init__.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2074 2020-07-09 07:01:14.000000 towerlib-3.9.3/tests/integration/common.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9523 2020-07-09 07:01:14.000000 towerlib-3.9.3/tests/integration/test_credential.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     6697 2020-07-09 07:01:14.000000 towerlib-3.9.3/tests/integration/test_group.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     5884 2020-07-09 07:01:14.000000 towerlib-3.9.3/tests/integration/test_host.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3511 2020-07-09 07:01:14.000000 towerlib-3.9.3/tests/integration/test_instance.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     8930 2020-07-09 07:01:14.000000 towerlib-3.9.3/tests/integration/test_inventory.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9020 2021-03-09 17:23:28.000000 towerlib-3.9.3/tests/integration/test_job.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    11358 2020-07-09 07:01:14.000000 towerlib-3.9.3/tests/integration/test_organization.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9239 2020-07-09 07:01:14.000000 towerlib-3.9.3/tests/integration/test_project.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    10791 2020-07-09 07:01:14.000000 towerlib-3.9.3/tests/integration/test_team.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    45410 2020-07-09 07:01:14.000000 towerlib-3.9.3/tests/integration/test_towerlib.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     6347 2020-07-09 07:01:14.000000 towerlib-3.9.3/tests/integration/test_user.py
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        5 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/.VERSION
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      578 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/AUTHORS.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1122 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/CONTRIBUTING.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     4780 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/HISTORY.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1063 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/LICENSE
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      644 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/Pipfile
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    49399 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/Pipfile.lock
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2539 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/README.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     3101 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/USAGE.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     4488 2020-07-09 07:01:14.000000 towerlib-3.9.3/towerlib/__init__.py
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/__pycache__/
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2270 2020-11-06 08:48:43.000000 towerlib-3.9.3/towerlib/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      983 2020-11-06 08:48:43.000000 towerlib-3.9.3/towerlib/__pycache__/_version.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    66839 2021-07-01 06:09:31.000000 towerlib-3.9.3/towerlib/__pycache__/towerlib.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     5149 2021-07-01 06:09:31.000000 towerlib-3.9.3/towerlib/__pycache__/towerlibexceptions.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2177 2020-07-09 07:01:14.000000 towerlib-3.9.3/towerlib/_version.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      601 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/dev-requirements.txt
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/entities/
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     5212 2021-07-01 06:02:01.000000 towerlib-3.9.3/towerlib/entities/__init__.py
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/entities/__pycache__/
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3094 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    12398 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/core.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    14232 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/credential.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9458 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/group.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    10751 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/host.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     5623 2020-11-06 08:48:43.000000 towerlib-3.9.3/towerlib/entities/__pycache__/instance.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    16116 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/inventory.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3108 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/inventory_script.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     6760 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/inventory_source.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    54635 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/job.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    18802 2020-12-07 12:59:39.000000 towerlib-3.9.3/towerlib/entities/__pycache__/notification.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    19275 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/organization.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    14500 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/project.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3598 2020-11-06 08:48:44.000000 towerlib-3.9.3/towerlib/entities/__pycache__/role.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9050 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/schedule.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    10697 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/settings.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    19756 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/team.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9853 2021-07-01 06:09:32.000000 towerlib-3.9.3/towerlib/entities/__pycache__/user.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    13560 2021-07-01 06:07:54.000000 towerlib-3.9.3/towerlib/entities/core.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    14996 2020-12-17 10:37:45.000000 towerlib-3.9.3/towerlib/entities/credential.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    10051 2020-12-17 10:37:45.000000 towerlib-3.9.3/towerlib/entities/group.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    11183 2021-07-01 06:00:36.000000 towerlib-3.9.3/towerlib/entities/host.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     5798 2020-07-09 07:01:14.000000 towerlib-3.9.3/towerlib/entities/instance.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    19768 2020-12-17 10:37:45.000000 towerlib-3.9.3/towerlib/entities/inventory.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     4012 2020-12-17 10:37:45.000000 towerlib-3.9.3/towerlib/entities/inventory_script.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     6894 2020-12-17 10:37:45.000000 towerlib-3.9.3/towerlib/entities/inventory_source.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    52583 2022-07-11 08:40:14.000000 towerlib-3.9.3/towerlib/entities/job.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    15342 2020-12-07 09:55:58.000000 towerlib-3.9.3/towerlib/entities/notification.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    21672 2021-07-01 06:07:54.000000 towerlib-3.9.3/towerlib/entities/organization.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    15838 2021-07-01 06:05:45.000000 towerlib-3.9.3/towerlib/entities/project.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     4439 2020-07-09 07:01:14.000000 towerlib-3.9.3/towerlib/entities/role.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9128 2021-01-06 13:07:05.000000 towerlib-3.9.3/towerlib/entities/schedule.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    11866 2020-12-17 10:37:45.000000 towerlib-3.9.3/towerlib/entities/settings.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    21066 2021-03-09 17:23:28.000000 towerlib-3.9.3/towerlib/entities/team.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    11666 2020-12-17 10:37:45.000000 towerlib-3.9.3/towerlib/entities/user.py
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      452 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib/requirements.txt
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)    82340 2022-04-19 14:36:54.000000 towerlib-3.9.3/towerlib/towerlib.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3825 2021-06-02 09:16:37.000000 towerlib-3.9.3/towerlib/towerlibexceptions.py
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib.egg-info/
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    10878 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib.egg-info/PKG-INFO
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3029 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib.egg-info/SOURCES.txt
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)        1 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib.egg-info/dependency_links.txt
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)        1 2020-10-16 11:43:58.000000 towerlib-3.9.3/towerlib.egg-info/not-zip-safe
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      121 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib.egg-info/requires.txt
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)       15 2022-07-11 09:36:57.000000 towerlib-3.9.3/towerlib.egg-info/top_level.txt
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-09-01 12:03:38.000000 towerlib-3.9.4/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        5 2022-09-01 12:01:50.000000 towerlib-3.9.4/.VERSION
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      578 2022-04-19 14:36:54.000000 towerlib-3.9.4/AUTHORS.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1122 2020-07-09 07:01:14.000000 towerlib-3.9.4/CONTRIBUTING.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     4866 2022-09-01 12:02:08.000000 towerlib-3.9.4/HISTORY.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1063 2020-07-09 07:01:14.000000 towerlib-3.9.4/LICENSE
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      390 2020-07-09 07:01:14.000000 towerlib-3.9.4/MANIFEST.in
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    11012 2022-09-01 12:03:38.000000 towerlib-3.9.4/PKG-INFO
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      644 2021-04-26 11:07:44.000000 towerlib-3.9.4/Pipfile
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    49351 2022-09-01 12:03:35.000000 towerlib-3.9.4/Pipfile.lock
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2539 2020-07-09 07:01:14.000000 towerlib-3.9.4/README.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     3101 2021-04-26 07:04:39.000000 towerlib-3.9.4/USAGE.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      601 2022-09-01 12:03:35.000000 towerlib-3.9.4/dev-requirements.txt
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-09-01 12:03:37.000000 towerlib-3.9.4/docs/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     6770 2020-07-09 07:01:14.000000 towerlib-3.9.4/docs/Makefile
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       28 2020-07-09 07:01:14.000000 towerlib-3.9.4/docs/authors.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     8894 2020-07-09 07:01:14.000000 towerlib-3.9.4/docs/conf.py
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       33 2020-07-09 07:01:14.000000 towerlib-3.9.4/docs/contributing.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       28 2020-07-09 07:01:14.000000 towerlib-3.9.4/docs/history.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      498 2020-07-09 07:01:14.000000 towerlib-3.9.4/docs/index.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)       33 2020-07-09 07:01:14.000000 towerlib-3.9.4/docs/installation.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)       61 2021-07-01 06:10:42.000000 towerlib-3.9.4/docs/modules.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       27 2020-07-09 07:01:14.000000 towerlib-3.9.4/docs/readme.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3035 2021-07-01 06:10:42.000000 towerlib-3.9.4/docs/towerlib.entities.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      542 2020-07-09 07:01:14.000000 towerlib-3.9.4/docs/towerlib.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       26 2020-07-09 07:01:14.000000 towerlib-3.9.4/docs/usage.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      452 2022-09-01 12:03:35.000000 towerlib-3.9.4/requirements.txt
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      148 2022-09-01 12:03:38.000000 towerlib-3.9.4/setup.cfg
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1973 2020-07-09 07:01:14.000000 towerlib-3.9.4/setup.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-09-01 12:03:37.000000 towerlib-3.9.4/tests/
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-09-01 12:03:37.000000 towerlib-3.9.4/tests/integration/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3295 2020-07-09 07:01:14.000000 towerlib-3.9.4/tests/integration/__init__.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2074 2020-07-09 07:01:14.000000 towerlib-3.9.4/tests/integration/common.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9523 2020-07-09 07:01:14.000000 towerlib-3.9.4/tests/integration/test_credential.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     6697 2020-07-09 07:01:14.000000 towerlib-3.9.4/tests/integration/test_group.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     5884 2020-07-09 07:01:14.000000 towerlib-3.9.4/tests/integration/test_host.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3511 2020-07-09 07:01:14.000000 towerlib-3.9.4/tests/integration/test_instance.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     8930 2020-07-09 07:01:14.000000 towerlib-3.9.4/tests/integration/test_inventory.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9020 2021-03-09 17:23:28.000000 towerlib-3.9.4/tests/integration/test_job.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    11358 2020-07-09 07:01:14.000000 towerlib-3.9.4/tests/integration/test_organization.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9239 2020-07-09 07:01:14.000000 towerlib-3.9.4/tests/integration/test_project.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    10791 2020-07-09 07:01:14.000000 towerlib-3.9.4/tests/integration/test_team.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    45410 2020-07-09 07:01:14.000000 towerlib-3.9.4/tests/integration/test_towerlib.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     6347 2020-07-09 07:01:14.000000 towerlib-3.9.4/tests/integration/test_user.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-09-01 12:03:37.000000 towerlib-3.9.4/towerlib/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        5 2022-09-01 12:03:35.000000 towerlib-3.9.4/towerlib/.VERSION
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      578 2022-09-01 12:03:35.000000 towerlib-3.9.4/towerlib/AUTHORS.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1122 2022-09-01 12:03:35.000000 towerlib-3.9.4/towerlib/CONTRIBUTING.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     4866 2022-09-01 12:03:35.000000 towerlib-3.9.4/towerlib/HISTORY.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1063 2022-09-01 12:03:35.000000 towerlib-3.9.4/towerlib/LICENSE
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      644 2022-09-01 12:03:35.000000 towerlib-3.9.4/towerlib/Pipfile
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    49351 2022-09-01 12:03:35.000000 towerlib-3.9.4/towerlib/Pipfile.lock
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2539 2022-09-01 12:03:35.000000 towerlib-3.9.4/towerlib/README.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     3101 2022-09-01 12:03:35.000000 towerlib-3.9.4/towerlib/USAGE.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     4488 2020-07-09 07:01:14.000000 towerlib-3.9.4/towerlib/__init__.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-09-01 12:03:37.000000 towerlib-3.9.4/towerlib/__pycache__/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2270 2020-11-06 08:48:43.000000 towerlib-3.9.4/towerlib/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      983 2020-11-06 08:48:43.000000 towerlib-3.9.4/towerlib/__pycache__/_version.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    66839 2021-07-01 06:09:31.000000 towerlib-3.9.4/towerlib/__pycache__/towerlib.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     5149 2021-07-01 06:09:31.000000 towerlib-3.9.4/towerlib/__pycache__/towerlibexceptions.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2177 2020-07-09 07:01:14.000000 towerlib-3.9.4/towerlib/_version.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      601 2022-09-01 12:03:35.000000 towerlib-3.9.4/towerlib/dev-requirements.txt
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-09-01 12:03:38.000000 towerlib-3.9.4/towerlib/entities/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     5212 2021-07-01 06:02:01.000000 towerlib-3.9.4/towerlib/entities/__init__.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-09-01 12:03:38.000000 towerlib-3.9.4/towerlib/entities/__pycache__/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3094 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    12398 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/core.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    14232 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/credential.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9458 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/group.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    10751 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/host.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     5623 2020-11-06 08:48:43.000000 towerlib-3.9.4/towerlib/entities/__pycache__/instance.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    16116 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/inventory.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3108 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/inventory_script.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     6760 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/inventory_source.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    54635 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/job.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    18802 2020-12-07 12:59:39.000000 towerlib-3.9.4/towerlib/entities/__pycache__/notification.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    19275 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/organization.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    14500 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/project.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3598 2020-11-06 08:48:44.000000 towerlib-3.9.4/towerlib/entities/__pycache__/role.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9050 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/schedule.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    10697 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/settings.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    19756 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/team.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9853 2021-07-01 06:09:32.000000 towerlib-3.9.4/towerlib/entities/__pycache__/user.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    13560 2021-07-01 06:07:54.000000 towerlib-3.9.4/towerlib/entities/core.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    14996 2020-12-17 10:37:45.000000 towerlib-3.9.4/towerlib/entities/credential.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    10051 2020-12-17 10:37:45.000000 towerlib-3.9.4/towerlib/entities/group.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    11184 2022-08-30 09:45:08.000000 towerlib-3.9.4/towerlib/entities/host.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     5798 2020-07-09 07:01:14.000000 towerlib-3.9.4/towerlib/entities/instance.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    19768 2020-12-17 10:37:45.000000 towerlib-3.9.4/towerlib/entities/inventory.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     4012 2020-12-17 10:37:45.000000 towerlib-3.9.4/towerlib/entities/inventory_script.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     6894 2020-12-17 10:37:45.000000 towerlib-3.9.4/towerlib/entities/inventory_source.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    52585 2022-09-01 08:23:35.000000 towerlib-3.9.4/towerlib/entities/job.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    15342 2020-12-07 09:55:58.000000 towerlib-3.9.4/towerlib/entities/notification.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    21672 2021-07-01 06:07:54.000000 towerlib-3.9.4/towerlib/entities/organization.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    15838 2021-07-01 06:05:45.000000 towerlib-3.9.4/towerlib/entities/project.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     4439 2020-07-09 07:01:14.000000 towerlib-3.9.4/towerlib/entities/role.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     9128 2021-01-06 13:07:05.000000 towerlib-3.9.4/towerlib/entities/schedule.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    11866 2020-12-17 10:37:45.000000 towerlib-3.9.4/towerlib/entities/settings.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    21066 2021-03-09 17:23:28.000000 towerlib-3.9.4/towerlib/entities/team.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    11666 2020-12-17 10:37:45.000000 towerlib-3.9.4/towerlib/entities/user.py
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      452 2022-09-01 12:03:35.000000 towerlib-3.9.4/towerlib/requirements.txt
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)    82550 2022-09-01 08:24:40.000000 towerlib-3.9.4/towerlib/towerlib.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3825 2021-06-02 09:16:37.000000 towerlib-3.9.4/towerlib/towerlibexceptions.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2022-09-01 12:03:37.000000 towerlib-3.9.4/towerlib.egg-info/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    11012 2022-09-01 12:03:36.000000 towerlib-3.9.4/towerlib.egg-info/PKG-INFO
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3029 2022-09-01 12:03:36.000000 towerlib-3.9.4/towerlib.egg-info/SOURCES.txt
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)        1 2022-09-01 12:03:36.000000 towerlib-3.9.4/towerlib.egg-info/dependency_links.txt
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)        1 2020-10-16 11:43:58.000000 towerlib-3.9.4/towerlib.egg-info/not-zip-safe
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      121 2022-09-01 12:03:36.000000 towerlib-3.9.4/towerlib.egg-info/requires.txt
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)       15 2022-09-01 12:03:36.000000 towerlib-3.9.4/towerlib.egg-info/top_level.txt
```

### Comparing `towerlib-3.9.3/AUTHORS.rst` & `towerlib-3.9.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/CONTRIBUTING.rst` & `towerlib-3.9.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/HISTORY.rst` & `towerlib-3.9.4/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -292,7 +292,13 @@
 * Linted.
 
 
 3.9.3 (11-07-2022)
 ------------------
 
 * Fixed bug with job execution.
+
+
+3.9.4 (01-09-2022)
+------------------
+
+* Fixed some redirects, bumped dependencies.
```

### Comparing `towerlib-3.9.3/LICENSE` & `towerlib-3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/PKG-INFO` & `towerlib-3.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: towerlib
-Version: 3.9.3
+Version: 3.9.4
 Summary: A python library to interface with ansible tower's (awx) api.
 Home-page: https://github.com/schubergphilis/towerlib.git
 Author: Costas Tyfoxylos
 Author-email: ctyfoxylos@schubergphilis.com
 License: MIT
 Description: ========
         towerlib
@@ -378,14 +378,20 @@
         
         
         3.9.3 (11-07-2022)
         ------------------
         
         * Fixed bug with job execution.
         
+        
+        3.9.4 (01-09-2022)
+        ------------------
+        
+        * Fixed some redirects, bumped dependencies.
+        
 Keywords: towerlib tower awx api ansible python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `towerlib-3.9.3/Pipfile` & `towerlib-3.9.4/Pipfile`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/Pipfile.lock` & `towerlib-3.9.4/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9883727383727384%*

 * *Differences: {"'default'": "{'charset-normalizer': {'hashes': "*

 * *              "['sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845', "*

 * *              "'sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f'], "*

 * *              "'version': '==2.1.1'}, 'pytz': {'hashes': "*

 * *              "['sha256:220f481bdafa09c3955dfbdddb7b57780e9a94f5127e35456a48589b9e0c0197', "*

 * *              "'sha256:cea221417204f2d1a2aa03ddae3e867921971d0d76f14d87abb4414415bbdcf5'], "*

 * *              "'version': '==2 […]*

```diff
@@ -36,19 +36,19 @@
                 "sha256:fe86415d55e84719d75f8b69414f6438ac3547d2078ab91b67e779ef69378412"
             ],
             "markers": "python_full_version >= '3.6.0'",
             "version": "==2022.6.15"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:5189b6f22b01957427f35b6a08d9a0bc45b46d3788ef5a92e978433c7a35f8a5",
-                "sha256:575e708016ff3a5e3681541cb9d79312c416835686d054a23accb873b254f413"
+                "sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845",
+                "sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f"
             ],
             "markers": "python_full_version >= '3.6.0'",
-            "version": "==2.1.0"
+            "version": "==2.1.1"
         },
         "dataclasses": {
             "hashes": [
                 "sha256:454a69d788c7fda44efd71e259be79577822f5e3f53f029a22d08004e951dc9f",
                 "sha256:6988bd2b895eef432d562370bb707d540f32f7360ab13da45340101bc2307d84"
             ],
             "markers": "python_version == '3.6'",
@@ -76,18 +76,18 @@
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
         },
         "pytz": {
             "hashes": [
-                "sha256:1e760e2fe6a8163bc0b3d9a19c4f84342afa0a2affebfaa84b01b978a02ecaa7",
-                "sha256:e68985985296d9a66a881eb3193b0906246245294a881e7c8afe623866ac6a5c"
+                "sha256:220f481bdafa09c3955dfbdddb7b57780e9a94f5127e35456a48589b9e0c0197",
+                "sha256:cea221417204f2d1a2aa03ddae3e867921971d0d76f14d87abb4414415bbdcf5"
             ],
-            "version": "==2022.1"
+            "version": "==2022.2.1"
         },
         "requests": {
             "hashes": [
                 "sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983",
                 "sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349"
             ],
             "index": "pypi",
@@ -107,19 +107,19 @@
                 "sha256:fc53893b3da2c33de295667a0e19f078c14bf86544af307354de5fcf12a3f30d"
             ],
             "markers": "python_full_version >= '3.6.0'",
             "version": "==2.3.2.post1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8298d6d56d39be0e3bc13c1c97d133f9b45d797169a0e11cdd0e0489d786f7ec",
-                "sha256:879ba4d1e89654d9769ce13121e0f94310ea32e8d2f8cf587b77c08bbcdb30d6"
+                "sha256:3fa96cf423e6987997fc326ae8df396db2a8b7c667747d47ddd8ecba91f4a74e",
+                "sha256:b930dd878d5a8afb066a637fbb35144fe7901e3b209d1cd4f524bd0e9deee997"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5' and python_version < '4'",
-            "version": "==1.26.10"
+            "version": "==1.26.12"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:446438bdcca0e05bd45ea2de1668c1d9b032e1a9154c2c259092d77031ddd359",
                 "sha256:a661d72d58e6ea8a57f7a86e37d86716863ee5e92788398526d58b26a4e4dc02"
@@ -172,19 +172,19 @@
                 "sha256:fe86415d55e84719d75f8b69414f6438ac3547d2078ab91b67e779ef69378412"
             ],
             "markers": "python_full_version >= '3.6.0'",
             "version": "==2022.6.15"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:5189b6f22b01957427f35b6a08d9a0bc45b46d3788ef5a92e978433c7a35f8a5",
-                "sha256:575e708016ff3a5e3681541cb9d79312c416835686d054a23accb873b254f413"
+                "sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845",
+                "sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f"
             ],
             "markers": "python_full_version >= '3.6.0'",
-            "version": "==2.1.0"
+            "version": "==2.1.1"
         },
         "coloredlogs": {
             "hashes": [
                 "sha256:34fad2e342d5a559c31b6c889e8d14f97cb62c47d9a2ae7b5ed14ea10a79eff8",
                 "sha256:b869a2dda3fa88154b9dd850e27828d8755bfab5a838a1c97fbc850c6e377c36"
             ],
             "index": "pypi",
@@ -226,18 +226,18 @@
                 "sha256:ff37757e068ae606659c28c3bd0d923f9d29a85de79bf25b2b34b148473b5025"
             ],
             "index": "pypi",
             "version": "==4.5.4"
         },
         "distlib": {
             "hashes": [
-                "sha256:6564fe0a8f51e734df6333d08b8b94d4ea8ee6b99b5ed50613f731fd4089f34b",
-                "sha256:e4b58818180336dc9c529bfb9a0b58728ffc09ad92027a3f30b7cd91e3458579"
+                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
+                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
-            "version": "==0.3.4"
+            "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
                 "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
                 "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
             ],
             "markers": "python_version >= '3.7'",
@@ -255,19 +255,19 @@
                 "sha256:60652d3a2dcee5b8af8acb097c31776fb6d808027aeb7221830f72cdafefc174"
             ],
             "index": "pypi",
             "version": "==0.5.4"
         },
         "filelock": {
             "hashes": [
-                "sha256:37def7b658813cda163b56fc564cdc75e86d338246458c4c28ae84cabefa2404",
-                "sha256:3a0fd85166ad9dbab54c9aec96737b744106dc5f15c0b09a6744a445299fcf04"
+                "sha256:55447caa666f2198c5b6b13a26d2084d26fa5b115c00d065664b2124680c4edc",
+                "sha256:617eb4e5eedc82fc5f47b6d61e4d11cb837c56cb4544e39081099fa17ad109d4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.7.1"
+            "version": "==3.8.0"
         },
         "flake8": {
             "hashes": [
                 "sha256:bcf5163890bb01f11f04f0f444f01004d0f9ad5fab10c51104f770acf532008f",
                 "sha256:e2f33066fb92ac0a3a30ea509f61e325f2110b2e84644333a3ff8e9e98a2beab"
             ],
             "index": "pypi",
@@ -517,19 +517,19 @@
                 "sha256:35b2d75ee967ea93b55750aa9edbbf72813e06a66ba54438df2cfac9e3c27fc8"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.2.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:5eb116118f9612ff1ee89ac96437bb6b49e8f04d8a13b514ba26f620208e26eb",
-                "sha256:dc9c10fb40944260f6ed4c688ece0cd2048414940f1cea51b8b226318411c519"
+                "sha256:56a8508ae95f98e2b9bdf93a6be5ae3f7d8af858b43e02c5a2ff083726be40c1",
+                "sha256:f643f331ab57ba3c9d89212ee4a2dabc6e94f117cf4eefde99a0574720d14c42"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2.12.0"
+            "version": "==2.13.0"
         },
         "pylint": {
             "hashes": [
                 "sha256:7dd78437f2d8d019717dbf287772d0b2dbdfd13fc016aa7faa08d67bccc46adc",
                 "sha256:d0ece7d223fe422088b0e8f13fa0a1e8eb745ebffcb8ed53d3e95394b6101a1c"
             ],
             "markers": "python_version >= '3.5'",
@@ -568,18 +568,18 @@
                 "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"
             ],
             "markers": "python_full_version >= '3.6.8'",
             "version": "==3.0.9"
         },
         "pytz": {
             "hashes": [
-                "sha256:1e760e2fe6a8163bc0b3d9a19c4f84342afa0a2affebfaa84b01b978a02ecaa7",
-                "sha256:e68985985296d9a66a881eb3193b0906246245294a881e7c8afe623866ac6a5c"
+                "sha256:220f481bdafa09c3955dfbdddb7b57780e9a94f5127e35456a48589b9e0c0197",
+                "sha256:cea221417204f2d1a2aa03ddae3e867921971d0d76f14d87abb4414415bbdcf5"
             ],
-            "version": "==2022.1"
+            "version": "==2022.2.1"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
                 "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
@@ -614,19 +614,19 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:73b84905d091c31f36e50b4ae05ae2acead661f6a09a9abb4df7d2ddcdb6a698",
-                "sha256:a727999acfc222fc21d82a12ed48c957c4989785e5865807c65a487d21677497"
+                "sha256:07b7ea234e03e58f77cc222e206e6abb8f4c0435becce5104794ee591f9301c5",
+                "sha256:9fa416704703e509eeb900696751c908ddeb2011319d93700d8f18baff887a69"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==35.0"
+            "version": "==37.0"
         },
         "requests": {
             "hashes": [
                 "sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983",
                 "sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349"
             ],
             "index": "pypi",
@@ -661,19 +661,19 @@
                 "sha256:d2ecbd27c0c7d0d53990e2df98d9aad6490df8b75b71c621d8c441d6e91e3161"
             ],
             "markers": "python_version >= '3.0'",
             "version": "==0.3.0"
         },
         "setuptools": {
             "hashes": [
-                "sha256:16923d366ced322712c71ccb97164d07472abeecd13f3a6c283f6d5d26722793",
-                "sha256:db3b8e2f922b2a910a29804776c643ea609badb6a32c4bcc226fd4fd902cce65"
+                "sha256:2e24e0bec025f035a2e72cdd1961119f557d78ad331bb00ff82efb2ab8da8e82",
+                "sha256:7732871f4f7fa58fb6bdcaeadb0161b2bd046c85905dbaa066bdcbcc81953b57"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==63.1.0"
+            "version": "==65.3.0"
         },
         "sh": {
             "hashes": [
                 "sha256:ae3258c5249493cebe73cb4e18253a41ed69262484bad36fdb3efcb8ad8870bb",
                 "sha256:b52bf5833ed01c7b5c5fb73a7f71b3d98d48e9b9b8764236237bdc7ecae850fc"
             ],
             "version": "==1.12.14"
@@ -823,27 +823,27 @@
                 "sha256:fb1bbeac803adea29cedd70781399c99138358c26d05fcbd23c13016b7f5ec65"
             ],
             "markers": "python_version < '3.8' and implementation_name == 'cpython'",
             "version": "==1.4.3"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8298d6d56d39be0e3bc13c1c97d133f9b45d797169a0e11cdd0e0489d786f7ec",
-                "sha256:879ba4d1e89654d9769ce13121e0f94310ea32e8d2f8cf587b77c08bbcdb30d6"
+                "sha256:3fa96cf423e6987997fc326ae8df396db2a8b7c667747d47ddd8ecba91f4a74e",
+                "sha256:b930dd878d5a8afb066a637fbb35144fe7901e3b209d1cd4f524bd0e9deee997"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5' and python_version < '4'",
-            "version": "==1.26.10"
+            "version": "==1.26.12"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:288171134a2ff3bfb1a2f54f119e77cd1b81c29fc1265a2356f3e8d14c7d58c4",
-                "sha256:b30aefac647e86af6d82bfc944c556f8f1a9c90427b2fb4e3bfbf338cb82becf"
+                "sha256:0ef5be6d07181946891f5abc8047fda8bc2f0b4b9bf222c64e6e8963baee76db",
+                "sha256:635b272a8e2f77cb051946f46c60a54ace3cb5e25568228bd6b57fc70eca9ff3"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==20.15.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==20.16.2"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
@@ -916,15 +916,15 @@
                 "sha256:ef3f72c9666bba2bab70d2a8b79f2c6d2c1a42a7f7e2b0ec83bb2f9e383950af"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==1.14.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:56bf8aadb83c24db6c4b577e13de374ccfb67da2078beba1d037c17980bf43ad",
-                "sha256:c4f6e5bbf48e74f7a38e7cc5b0480ff42b0ae5178957d564d18932525d5cf099"
+                "sha256:05b45f1ee8f807d0cc928485ca40a07cb491cf092ff587c0df9cb1fd154848d2",
+                "sha256:47c40d7fe183a6f21403a199b3e4192cca5774656965b0a4988ad2f8feb5f009"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.8.0"
+            "version": "==3.8.1"
         }
     }
 }
```

### Comparing `towerlib-3.9.3/README.rst` & `towerlib-3.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/USAGE.rst` & `towerlib-3.9.4/USAGE.rst`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/dev-requirements.txt` & `towerlib-3.9.4/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/docs/Makefile` & `towerlib-3.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/docs/conf.py` & `towerlib-3.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/docs/towerlib.entities.rst` & `towerlib-3.9.4/docs/towerlib.entities.rst`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/docs/towerlib.rst` & `towerlib-3.9.4/docs/towerlib.rst`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/setup.py` & `towerlib-3.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/tests/integration/__init__.py` & `towerlib-3.9.4/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/tests/integration/common.py` & `towerlib-3.9.4/tests/integration/common.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/tests/integration/test_credential.py` & `towerlib-3.9.4/tests/integration/test_credential.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/tests/integration/test_group.py` & `towerlib-3.9.4/tests/integration/test_group.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/tests/integration/test_host.py` & `towerlib-3.9.4/tests/integration/test_host.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/tests/integration/test_instance.py` & `towerlib-3.9.4/tests/integration/test_instance.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/tests/integration/test_inventory.py` & `towerlib-3.9.4/tests/integration/test_inventory.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/tests/integration/test_job.py` & `towerlib-3.9.4/tests/integration/test_job.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/tests/integration/test_organization.py` & `towerlib-3.9.4/tests/integration/test_organization.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/tests/integration/test_project.py` & `towerlib-3.9.4/tests/integration/test_project.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/tests/integration/test_team.py` & `towerlib-3.9.4/tests/integration/test_team.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/tests/integration/test_towerlib.py` & `towerlib-3.9.4/tests/integration/test_towerlib.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/tests/integration/test_user.py` & `towerlib-3.9.4/tests/integration/test_user.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/AUTHORS.rst` & `towerlib-3.9.4/towerlib/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/CONTRIBUTING.rst` & `towerlib-3.9.4/towerlib/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/HISTORY.rst` & `towerlib-3.9.4/towerlib/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -292,7 +292,13 @@
 * Linted.
 
 
 3.9.3 (11-07-2022)
 ------------------
 
 * Fixed bug with job execution.
+
+
+3.9.4 (01-09-2022)
+------------------
+
+* Fixed some redirects, bumped dependencies.
```

### Comparing `towerlib-3.9.3/towerlib/LICENSE` & `towerlib-3.9.4/towerlib/LICENSE`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/Pipfile` & `towerlib-3.9.4/towerlib/Pipfile`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/Pipfile.lock` & `towerlib-3.9.4/towerlib/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9883727383727384%*

 * *Differences: {"'default'": "{'charset-normalizer': {'hashes': "*

 * *              "['sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845', "*

 * *              "'sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f'], "*

 * *              "'version': '==2.1.1'}, 'pytz': {'hashes': "*

 * *              "['sha256:220f481bdafa09c3955dfbdddb7b57780e9a94f5127e35456a48589b9e0c0197', "*

 * *              "'sha256:cea221417204f2d1a2aa03ddae3e867921971d0d76f14d87abb4414415bbdcf5'], "*

 * *              "'version': '==2 […]*

```diff
@@ -36,19 +36,19 @@
                 "sha256:fe86415d55e84719d75f8b69414f6438ac3547d2078ab91b67e779ef69378412"
             ],
             "markers": "python_full_version >= '3.6.0'",
             "version": "==2022.6.15"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:5189b6f22b01957427f35b6a08d9a0bc45b46d3788ef5a92e978433c7a35f8a5",
-                "sha256:575e708016ff3a5e3681541cb9d79312c416835686d054a23accb873b254f413"
+                "sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845",
+                "sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f"
             ],
             "markers": "python_full_version >= '3.6.0'",
-            "version": "==2.1.0"
+            "version": "==2.1.1"
         },
         "dataclasses": {
             "hashes": [
                 "sha256:454a69d788c7fda44efd71e259be79577822f5e3f53f029a22d08004e951dc9f",
                 "sha256:6988bd2b895eef432d562370bb707d540f32f7360ab13da45340101bc2307d84"
             ],
             "markers": "python_version == '3.6'",
@@ -76,18 +76,18 @@
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
         },
         "pytz": {
             "hashes": [
-                "sha256:1e760e2fe6a8163bc0b3d9a19c4f84342afa0a2affebfaa84b01b978a02ecaa7",
-                "sha256:e68985985296d9a66a881eb3193b0906246245294a881e7c8afe623866ac6a5c"
+                "sha256:220f481bdafa09c3955dfbdddb7b57780e9a94f5127e35456a48589b9e0c0197",
+                "sha256:cea221417204f2d1a2aa03ddae3e867921971d0d76f14d87abb4414415bbdcf5"
             ],
-            "version": "==2022.1"
+            "version": "==2022.2.1"
         },
         "requests": {
             "hashes": [
                 "sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983",
                 "sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349"
             ],
             "index": "pypi",
@@ -107,19 +107,19 @@
                 "sha256:fc53893b3da2c33de295667a0e19f078c14bf86544af307354de5fcf12a3f30d"
             ],
             "markers": "python_full_version >= '3.6.0'",
             "version": "==2.3.2.post1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8298d6d56d39be0e3bc13c1c97d133f9b45d797169a0e11cdd0e0489d786f7ec",
-                "sha256:879ba4d1e89654d9769ce13121e0f94310ea32e8d2f8cf587b77c08bbcdb30d6"
+                "sha256:3fa96cf423e6987997fc326ae8df396db2a8b7c667747d47ddd8ecba91f4a74e",
+                "sha256:b930dd878d5a8afb066a637fbb35144fe7901e3b209d1cd4f524bd0e9deee997"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5' and python_version < '4'",
-            "version": "==1.26.10"
+            "version": "==1.26.12"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:446438bdcca0e05bd45ea2de1668c1d9b032e1a9154c2c259092d77031ddd359",
                 "sha256:a661d72d58e6ea8a57f7a86e37d86716863ee5e92788398526d58b26a4e4dc02"
@@ -172,19 +172,19 @@
                 "sha256:fe86415d55e84719d75f8b69414f6438ac3547d2078ab91b67e779ef69378412"
             ],
             "markers": "python_full_version >= '3.6.0'",
             "version": "==2022.6.15"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:5189b6f22b01957427f35b6a08d9a0bc45b46d3788ef5a92e978433c7a35f8a5",
-                "sha256:575e708016ff3a5e3681541cb9d79312c416835686d054a23accb873b254f413"
+                "sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845",
+                "sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f"
             ],
             "markers": "python_full_version >= '3.6.0'",
-            "version": "==2.1.0"
+            "version": "==2.1.1"
         },
         "coloredlogs": {
             "hashes": [
                 "sha256:34fad2e342d5a559c31b6c889e8d14f97cb62c47d9a2ae7b5ed14ea10a79eff8",
                 "sha256:b869a2dda3fa88154b9dd850e27828d8755bfab5a838a1c97fbc850c6e377c36"
             ],
             "index": "pypi",
@@ -226,18 +226,18 @@
                 "sha256:ff37757e068ae606659c28c3bd0d923f9d29a85de79bf25b2b34b148473b5025"
             ],
             "index": "pypi",
             "version": "==4.5.4"
         },
         "distlib": {
             "hashes": [
-                "sha256:6564fe0a8f51e734df6333d08b8b94d4ea8ee6b99b5ed50613f731fd4089f34b",
-                "sha256:e4b58818180336dc9c529bfb9a0b58728ffc09ad92027a3f30b7cd91e3458579"
+                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
+                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
-            "version": "==0.3.4"
+            "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
                 "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
                 "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
             ],
             "markers": "python_version >= '3.7'",
@@ -255,19 +255,19 @@
                 "sha256:60652d3a2dcee5b8af8acb097c31776fb6d808027aeb7221830f72cdafefc174"
             ],
             "index": "pypi",
             "version": "==0.5.4"
         },
         "filelock": {
             "hashes": [
-                "sha256:37def7b658813cda163b56fc564cdc75e86d338246458c4c28ae84cabefa2404",
-                "sha256:3a0fd85166ad9dbab54c9aec96737b744106dc5f15c0b09a6744a445299fcf04"
+                "sha256:55447caa666f2198c5b6b13a26d2084d26fa5b115c00d065664b2124680c4edc",
+                "sha256:617eb4e5eedc82fc5f47b6d61e4d11cb837c56cb4544e39081099fa17ad109d4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.7.1"
+            "version": "==3.8.0"
         },
         "flake8": {
             "hashes": [
                 "sha256:bcf5163890bb01f11f04f0f444f01004d0f9ad5fab10c51104f770acf532008f",
                 "sha256:e2f33066fb92ac0a3a30ea509f61e325f2110b2e84644333a3ff8e9e98a2beab"
             ],
             "index": "pypi",
@@ -517,19 +517,19 @@
                 "sha256:35b2d75ee967ea93b55750aa9edbbf72813e06a66ba54438df2cfac9e3c27fc8"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.2.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:5eb116118f9612ff1ee89ac96437bb6b49e8f04d8a13b514ba26f620208e26eb",
-                "sha256:dc9c10fb40944260f6ed4c688ece0cd2048414940f1cea51b8b226318411c519"
+                "sha256:56a8508ae95f98e2b9bdf93a6be5ae3f7d8af858b43e02c5a2ff083726be40c1",
+                "sha256:f643f331ab57ba3c9d89212ee4a2dabc6e94f117cf4eefde99a0574720d14c42"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2.12.0"
+            "version": "==2.13.0"
         },
         "pylint": {
             "hashes": [
                 "sha256:7dd78437f2d8d019717dbf287772d0b2dbdfd13fc016aa7faa08d67bccc46adc",
                 "sha256:d0ece7d223fe422088b0e8f13fa0a1e8eb745ebffcb8ed53d3e95394b6101a1c"
             ],
             "markers": "python_version >= '3.5'",
@@ -568,18 +568,18 @@
                 "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"
             ],
             "markers": "python_full_version >= '3.6.8'",
             "version": "==3.0.9"
         },
         "pytz": {
             "hashes": [
-                "sha256:1e760e2fe6a8163bc0b3d9a19c4f84342afa0a2affebfaa84b01b978a02ecaa7",
-                "sha256:e68985985296d9a66a881eb3193b0906246245294a881e7c8afe623866ac6a5c"
+                "sha256:220f481bdafa09c3955dfbdddb7b57780e9a94f5127e35456a48589b9e0c0197",
+                "sha256:cea221417204f2d1a2aa03ddae3e867921971d0d76f14d87abb4414415bbdcf5"
             ],
-            "version": "==2022.1"
+            "version": "==2022.2.1"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
                 "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
@@ -614,19 +614,19 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:73b84905d091c31f36e50b4ae05ae2acead661f6a09a9abb4df7d2ddcdb6a698",
-                "sha256:a727999acfc222fc21d82a12ed48c957c4989785e5865807c65a487d21677497"
+                "sha256:07b7ea234e03e58f77cc222e206e6abb8f4c0435becce5104794ee591f9301c5",
+                "sha256:9fa416704703e509eeb900696751c908ddeb2011319d93700d8f18baff887a69"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==35.0"
+            "version": "==37.0"
         },
         "requests": {
             "hashes": [
                 "sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983",
                 "sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349"
             ],
             "index": "pypi",
@@ -661,19 +661,19 @@
                 "sha256:d2ecbd27c0c7d0d53990e2df98d9aad6490df8b75b71c621d8c441d6e91e3161"
             ],
             "markers": "python_version >= '3.0'",
             "version": "==0.3.0"
         },
         "setuptools": {
             "hashes": [
-                "sha256:16923d366ced322712c71ccb97164d07472abeecd13f3a6c283f6d5d26722793",
-                "sha256:db3b8e2f922b2a910a29804776c643ea609badb6a32c4bcc226fd4fd902cce65"
+                "sha256:2e24e0bec025f035a2e72cdd1961119f557d78ad331bb00ff82efb2ab8da8e82",
+                "sha256:7732871f4f7fa58fb6bdcaeadb0161b2bd046c85905dbaa066bdcbcc81953b57"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==63.1.0"
+            "version": "==65.3.0"
         },
         "sh": {
             "hashes": [
                 "sha256:ae3258c5249493cebe73cb4e18253a41ed69262484bad36fdb3efcb8ad8870bb",
                 "sha256:b52bf5833ed01c7b5c5fb73a7f71b3d98d48e9b9b8764236237bdc7ecae850fc"
             ],
             "version": "==1.12.14"
@@ -823,27 +823,27 @@
                 "sha256:fb1bbeac803adea29cedd70781399c99138358c26d05fcbd23c13016b7f5ec65"
             ],
             "markers": "python_version < '3.8' and implementation_name == 'cpython'",
             "version": "==1.4.3"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8298d6d56d39be0e3bc13c1c97d133f9b45d797169a0e11cdd0e0489d786f7ec",
-                "sha256:879ba4d1e89654d9769ce13121e0f94310ea32e8d2f8cf587b77c08bbcdb30d6"
+                "sha256:3fa96cf423e6987997fc326ae8df396db2a8b7c667747d47ddd8ecba91f4a74e",
+                "sha256:b930dd878d5a8afb066a637fbb35144fe7901e3b209d1cd4f524bd0e9deee997"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5' and python_version < '4'",
-            "version": "==1.26.10"
+            "version": "==1.26.12"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:288171134a2ff3bfb1a2f54f119e77cd1b81c29fc1265a2356f3e8d14c7d58c4",
-                "sha256:b30aefac647e86af6d82bfc944c556f8f1a9c90427b2fb4e3bfbf338cb82becf"
+                "sha256:0ef5be6d07181946891f5abc8047fda8bc2f0b4b9bf222c64e6e8963baee76db",
+                "sha256:635b272a8e2f77cb051946f46c60a54ace3cb5e25568228bd6b57fc70eca9ff3"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==20.15.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==20.16.2"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
@@ -916,15 +916,15 @@
                 "sha256:ef3f72c9666bba2bab70d2a8b79f2c6d2c1a42a7f7e2b0ec83bb2f9e383950af"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==1.14.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:56bf8aadb83c24db6c4b577e13de374ccfb67da2078beba1d037c17980bf43ad",
-                "sha256:c4f6e5bbf48e74f7a38e7cc5b0480ff42b0ae5178957d564d18932525d5cf099"
+                "sha256:05b45f1ee8f807d0cc928485ca40a07cb491cf092ff587c0df9cb1fd154848d2",
+                "sha256:47c40d7fe183a6f21403a199b3e4192cca5774656965b0a4988ad2f8feb5f009"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.8.0"
+            "version": "==3.8.1"
         }
     }
 }
```

### Comparing `towerlib-3.9.3/towerlib/README.rst` & `towerlib-3.9.4/towerlib/README.rst`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/USAGE.rst` & `towerlib-3.9.4/towerlib/USAGE.rst`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/__init__.py` & `towerlib-3.9.4/towerlib/__init__.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/__pycache__/__init__.cpython-37.pyc` & `towerlib-3.9.4/towerlib/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/__pycache__/_version.cpython-37.pyc` & `towerlib-3.9.4/towerlib/__pycache__/_version.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/__pycache__/towerlib.cpython-37.pyc` & `towerlib-3.9.4/towerlib/__pycache__/towerlib.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/__pycache__/towerlibexceptions.cpython-37.pyc` & `towerlib-3.9.4/towerlib/__pycache__/towerlibexceptions.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/_version.py` & `towerlib-3.9.4/towerlib/_version.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/dev-requirements.txt` & `towerlib-3.9.4/towerlib/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__init__.py` & `towerlib-3.9.4/towerlib/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/__init__.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/core.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/core.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/credential.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/credential.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/group.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/group.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/host.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/host.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/instance.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/instance.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/inventory.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/inventory.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/inventory_script.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/inventory_script.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/inventory_source.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/inventory_source.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/job.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/job.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/notification.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/notification.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/organization.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/organization.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/project.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/project.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/role.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/role.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/schedule.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/schedule.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/settings.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/settings.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/team.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/team.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/__pycache__/user.cpython-37.pyc` & `towerlib-3.9.4/towerlib/entities/__pycache__/user.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/core.py` & `towerlib-3.9.4/towerlib/entities/core.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/credential.py` & `towerlib-3.9.4/towerlib/entities/credential.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/group.py` & `towerlib-3.9.4/towerlib/entities/group.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/host.py` & `towerlib-3.9.4/towerlib/entities/host.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 
         Returns:
             json: Json representation of ansible facts
 
         Raises: None
 
         """
-        url = f'{self._tower.api}/hosts/{self.id}/ansible_facts'
+        url = f'{self._tower.api}/hosts/{self.id}/ansible_facts/'
         response = self._tower.session.get(url)
         if not response.ok:
             self._logger.error('Error finding ansible facts for %s.', self._data.get('name'))
         return response.json() if response.ok else '{}'
 
     def associate_with_groups(self, groups):
         """Associate the host with the provided groups.
```

### Comparing `towerlib-3.9.3/towerlib/entities/instance.py` & `towerlib-3.9.4/towerlib/entities/instance.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/inventory.py` & `towerlib-3.9.4/towerlib/entities/inventory.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/inventory_script.py` & `towerlib-3.9.4/towerlib/entities/inventory_script.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/inventory_source.py` & `towerlib-3.9.4/towerlib/entities/inventory_source.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/job.py` & `towerlib-3.9.4/towerlib/entities/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,15 +442,15 @@
         """
         url = self._data.get('related', {}).get('created_by')
         return self._tower._get_object_by_url('User', url)  # pylint: disable=protected-access
 
     # TOFIX add labels, model them and implement them here
 
     def _get_dynamic_value(self, variable):
-        url = f'{self._tower.api}/jobs/{self.id}'
+        url = f'{self._tower.api}/jobs/{self.id}/'
         response = self._tower.session.get(url)
         return response.json().get(variable) if response.ok else None
 
     def cancel(self):
         """Cancels the running or pending job.
 
         Returns:
@@ -707,15 +707,15 @@
         return self._data.get('job_type')
 
 
 class WorkflowJobRun(JobRun):
     """Models the Workflow Job Run entity of ansible tower."""
 
     def _get_dynamic_value(self, variable):
-        url = f'{self._tower.api}/workflow_jobs/{self.id}'
+        url = f'{self._tower.api}/workflow_jobs/{self.id}/'
         response = self._tower.session.get(url)
         return response.json().get(variable) if response.ok else None
 
     def cancel(self):
         """Cancels the running or pending job.
 
         Returns:
@@ -946,15 +946,15 @@
                      start_date,
                      start_time,
                      limit='',
                      description='',
                      time_zone='Europe/Berlin',
                      repeat_frequency='DAILY',
                      interval=1,
-                     extar_vars: dict = None):
+                     extra_vars: dict = None):
         """Adds a schedule to a job template.
 
         Args:
             name (str): A name of the schedule.
             start_date (datetime.date): The start date of the schedule
             start_time (datetime.time): Start time of the schedule
             limit (str): Limit of the schedule
```

### Comparing `towerlib-3.9.3/towerlib/entities/notification.py` & `towerlib-3.9.4/towerlib/entities/notification.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/organization.py` & `towerlib-3.9.4/towerlib/entities/organization.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/project.py` & `towerlib-3.9.4/towerlib/entities/project.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/role.py` & `towerlib-3.9.4/towerlib/entities/role.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/schedule.py` & `towerlib-3.9.4/towerlib/entities/schedule.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/settings.py` & `towerlib-3.9.4/towerlib/entities/settings.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/team.py` & `towerlib-3.9.4/towerlib/entities/team.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/entities/user.py` & `towerlib-3.9.4/towerlib/entities/user.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib/towerlib.py` & `towerlib-3.9.4/towerlib/towerlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,19 +96,27 @@
 PAGINATION_LIMIT = 25
 CLUSTER_STATE_CACHING_SECONDS = 10
 CONFIGURATION_STATE_CACHING_SECONDS = 60
 CLUSTER_STATE_CACHE = TTLCache(maxsize=1, ttl=CLUSTER_STATE_CACHING_SECONDS)
 CONFIGURATION_STATE_CACHE = TTLCache(maxsize=1, ttl=CONFIGURATION_STATE_CACHING_SECONDS)
 
 
-class Tower:  # pylint: disable=too-many-public-methods
+class Tower:  # pylint: disable=too-many-public-methods, too-many-instance-attributes
     """Models the api of ansible tower."""
 
     # pylint: disable=too-many-arguments
-    def __init__(self, host, username, password, secure=False, ssl_verify=True, token=None, pool_connections=HTTP_POOL_CONNECTIONS, pool_maxsize=HTTP_POOL_MAX_SIZE):
+    def __init__(self,
+                 host,
+                 username,
+                 password,
+                 secure=False,
+                 ssl_verify=True,
+                 token=None,
+                 pool_connections=HTTP_POOL_CONNECTIONS,
+                 pool_maxsize=HTTP_POOL_MAX_SIZE):
         self._logger = logging.getLogger(f'{LOGGER_BASENAME}.{self.__class__.__name__}')
         self.host = self._generate_host_name(host, secure)
         self.api = f'{self.host}/api/v2'
         self.username = username
         self.password = password
         self.token = token
         self.http_pool_maxsize = pool_maxsize
@@ -117,15 +125,16 @@
 
     @staticmethod
     def _generate_host_name(host, secure):
         return f'{"https" if secure else "http"}://{host}'
 
     def _get_authenticated_session(self, secure, ssl_verify):
         session = Session()
-        http_adapter = adapters.HTTPAdapter(pool_connections=self.http_pool_connections, pool_maxsize=self.http_pool_maxsize)
+        http_adapter = adapters.HTTPAdapter(pool_connections=self.http_pool_connections,
+                                            pool_maxsize=self.http_pool_maxsize)
         session.mount('http://', http_adapter)
         session.mount('https://', http_adapter)
         if secure:
             session.verify = ssl_verify
         return self._authenticate(session, self.host, self.username, self.password, self.api, self.token)
 
     @staticmethod
```

### Comparing `towerlib-3.9.3/towerlib/towerlibexceptions.py` & `towerlib-3.9.4/towerlib/towerlibexceptions.py`

 * *Files identical despite different names*

### Comparing `towerlib-3.9.3/towerlib.egg-info/PKG-INFO` & `towerlib-3.9.4/towerlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: towerlib
-Version: 3.9.3
+Version: 3.9.4
 Summary: A python library to interface with ansible tower's (awx) api.
 Home-page: https://github.com/schubergphilis/towerlib.git
 Author: Costas Tyfoxylos
 Author-email: ctyfoxylos@schubergphilis.com
 License: MIT
 Description: ========
         towerlib
@@ -378,14 +378,20 @@
         
         
         3.9.3 (11-07-2022)
         ------------------
         
         * Fixed bug with job execution.
         
+        
+        3.9.4 (01-09-2022)
+        ------------------
+        
+        * Fixed some redirects, bumped dependencies.
+        
 Keywords: towerlib tower awx api ansible python
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `towerlib-3.9.3/towerlib.egg-info/SOURCES.txt` & `towerlib-3.9.4/towerlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

