# Comparing `tmp/django-sessionprofile-2.0.0.tar.gz` & `tmp/django-sessionprofile-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sessionprofile-2.0.0.tar", last modified: Sun Oct 30 14:42:57 2022, max compression
+gzip compressed data, was "django-sessionprofile-3.0.0.tar", last modified: Fri May  5 19:54:21 2023, max compression
```

## Comparing `django-sessionprofile-2.0.0.tar` & `django-sessionprofile-3.0.0.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 14:42:57.836464 django-sessionprofile-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4108 2022-10-30 14:42:57.836464 django-sessionprofile-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 14:42:57.836464 django-sessionprofile-2.0.0/django_sessionprofile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4108 2022-10-30 14:42:57.000000 django-sessionprofile-2.0.0/django_sessionprofile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-10-30 14:42:57.000000 django-sessionprofile-2.0.0/django_sessionprofile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 14:42:57.000000 django-sessionprofile-2.0.0/django_sessionprofile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 14:42:57.000000 django-sessionprofile-2.0.0/django_sessionprofile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-10-30 14:42:57.000000 django-sessionprofile-2.0.0/django_sessionprofile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-30 14:42:57.000000 django-sessionprofile-2.0.0/django_sessionprofile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 14:42:57.836464 django-sessionprofile-2.0.0/sessionprofile/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 14:42:57.836464 django-sessionprofile-2.0.0/sessionprofile/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/backends/db.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 14:42:57.836464 django-sessionprofile-2.0.0/sessionprofile/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 14:42:57.836464 django-sessionprofile-2.0.0/sessionprofile/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/management/commands/sp_clear_expired.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 14:42:57.836464 django-sessionprofile-2.0.0/sessionprofile/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/models.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/sessionprofile/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2022-10-30 14:42:57.840464 django-sessionprofile-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-30 14:42:54.000000 django-sessionprofile-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:54:21.101105 django-sessionprofile-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-05 19:54:21.101105 django-sessionprofile-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:54:21.097105 django-sessionprofile-3.0.0/django_sessionprofile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-05 19:54:21.000000 django-sessionprofile-3.0.0/django_sessionprofile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-05 19:54:21.000000 django-sessionprofile-3.0.0/django_sessionprofile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:54:21.000000 django-sessionprofile-3.0.0/django_sessionprofile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:54:21.000000 django-sessionprofile-3.0.0/django_sessionprofile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-05 19:54:21.000000 django-sessionprofile-3.0.0/django_sessionprofile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 19:54:21.000000 django-sessionprofile-3.0.0/django_sessionprofile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:54:21.097105 django-sessionprofile-3.0.0/sessionprofile/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:54:21.101105 django-sessionprofile-3.0.0/sessionprofile/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/backends/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:54:21.101105 django-sessionprofile-3.0.0/sessionprofile/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:54:21.101105 django-sessionprofile-3.0.0/sessionprofile/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/management/commands/sp_clear_expired.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:54:21.101105 django-sessionprofile-3.0.0/sessionprofile/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/sessionprofile/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-05 19:54:21.101105 django-sessionprofile-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:54:21.101105 django-sessionprofile-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/tests/test_base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/tests/test_db_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-05 19:54:15.000000 django-sessionprofile-3.0.0/tests/test_management_commands.py
```

### Comparing `django-sessionprofile-2.0.0/CHANGELOG.rst` & `django-sessionprofile-3.0.0/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 =========
 Changelog
 =========
 
+3.0.0 (2023-05-05)
+==================
+
+Periodic version compatibility release.
+
+**Breaking changes 💥**
+
+* Dropped support for Python 3.7
+* Dropped support for Django 4.0
+
+The library likely still works on those versions, but they are no longer tested.
+
+**Other changes**
+
+* Confirmed support for Python 3.11
+* Confirmed support for Django 4.2
+
 2.0.0 (2022-10-30)
 ==================
 
 Maintenance release
 
 While the library has continued working without issues since 1.0 more than 6 years ago,
 it was time for some cleanup. A new major version is released because of the dropped
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-sessionprofile-2.0.0/LICENSE.txt` & `django-sessionprofile-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-sessionprofile-2.0.0/PKG-INFO` & `django-sessionprofile-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: django-sessionprofile
-Version: 2.0.0
+Version: 3.0.0
 Summary: Keep track of Django user sessions
 Home-page: https://github.com/modelbrouwers/django-sessionprofile
 Author: Sergei Maertens
 Author-email: sergei@modelbrouwers.nl
 License: MIT
 Project-URL: Documentation, http://django-sessionprofile.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/modelbrouwers/django-sessionprofile/blob/main/CHANGELOG.rst
 Project-URL: Bug Tracker, https://github.com/modelbrouwers/django-sessionprofile/issues
 Project-URL: Source Code, https://github.com/modelbrouwers/django-sessionprofile
 Keywords: django,session,user
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: tests
 Provides-Extra: pep8
 Provides-Extra: coverage
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE.txt
```

### Comparing `django-sessionprofile-2.0.0/README.rst` & `django-sessionprofile-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-sessionprofile-2.0.0/django_sessionprofile.egg-info/PKG-INFO` & `django-sessionprofile-3.0.0/django_sessionprofile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: django-sessionprofile
-Version: 2.0.0
+Version: 3.0.0
 Summary: Keep track of Django user sessions
 Home-page: https://github.com/modelbrouwers/django-sessionprofile
 Author: Sergei Maertens
 Author-email: sergei@modelbrouwers.nl
 License: MIT
 Project-URL: Documentation, http://django-sessionprofile.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/modelbrouwers/django-sessionprofile/blob/main/CHANGELOG.rst
 Project-URL: Bug Tracker, https://github.com/modelbrouwers/django-sessionprofile/issues
 Project-URL: Source Code, https://github.com/modelbrouwers/django-sessionprofile
 Keywords: django,session,user
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: tests
 Provides-Extra: pep8
 Provides-Extra: coverage
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE.txt
```

### Comparing `django-sessionprofile-2.0.0/sessionprofile/backends/base.py` & `django-sessionprofile-3.0.0/sessionprofile/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-sessionprofile-2.0.0/sessionprofile/backends/db.py` & `django-sessionprofile-3.0.0/sessionprofile/backends/db.py`

 * *Files identical despite different names*

### Comparing `django-sessionprofile-2.0.0/sessionprofile/migrations/0001_initial.py` & `django-sessionprofile-3.0.0/sessionprofile/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.9.4 on 2016-03-23 10:54
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
```

### Comparing `django-sessionprofile-2.0.0/sessionprofile/models.py` & `django-sessionprofile-3.0.0/sessionprofile/models.py`

 * *Files identical despite different names*

### Comparing `django-sessionprofile-2.0.0/setup.cfg` & `django-sessionprofile-3.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-sessionprofile
-version = 2.0.0
+version = 3.0.0
 description = Keep track of Django user sessions
 long_description = file: README.rst
 url = https://github.com/modelbrouwers/django-sessionprofile
 project_urls = 
 	Documentation = http://django-sessionprofile.readthedocs.io/en/latest/
 	Changelog = https://github.com/modelbrouwers/django-sessionprofile/blob/main/CHANGELOG.rst
 	Bug Tracker = https://github.com/modelbrouwers/django-sessionprofile/issues
@@ -13,24 +13,24 @@
 author = Sergei Maertens
 author_email = sergei@modelbrouwers.nl
 keywords = django, session, user
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	Operating System :: Unix
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires =
```

