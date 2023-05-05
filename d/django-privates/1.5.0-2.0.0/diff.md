# Comparing `tmp/django-privates-1.5.0.tar.gz` & `tmp/django-privates-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-privates-1.5.0.tar", last modified: Tue Jan  3 11:22:58 2023, max compression
+gzip compressed data, was "django-privates-2.0.0.tar", last modified: Fri May  5 16:06:04 2023, max compression
```

## Comparing `django-privates-1.5.0.tar` & `django-privates-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 11:22:58.190327 django-privates-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-01-03 11:22:54.000000 django-privates-1.5.0/Changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-01-03 11:22:54.000000 django-privates-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-01-03 11:22:54.000000 django-privates-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-01-03 11:22:58.190327 django-privates-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-01-03 11:22:54.000000 django-privates-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 11:22:58.190327 django-privates-1.5.0/django_privates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-01-03 11:22:58.000000 django-privates-1.5.0/django_privates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-01-03 11:22:58.000000 django-privates-1.5.0/django_privates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 11:22:58.000000 django-privates-1.5.0/django_privates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 11:22:58.000000 django-privates-1.5.0/django_privates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-01-03 11:22:58.000000 django-privates-1.5.0/django_privates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-03 11:22:58.000000 django-privates-1.5.0/django_privates.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 11:22:58.190327 django-privates-1.5.0/privates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 11:22:54.000000 django-privates-1.5.0/privates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-01-03 11:22:54.000000 django-privates-1.5.0/privates/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-03 11:22:54.000000 django-privates-1.5.0/privates/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-03 11:22:54.000000 django-privates-1.5.0/privates/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 11:22:54.000000 django-privates-1.5.0/privates/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-01-03 11:22:54.000000 django-privates-1.5.0/privates/storages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 11:22:58.182327 django-privates-1.5.0/privates/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 11:22:58.182327 django-privates-1.5.0/privates/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 11:22:58.190327 django-privates-1.5.0/privates/templates/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-01-03 11:22:54.000000 django-privates-1.5.0/privates/templates/admin/widgets/clearable_private_file_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-01-03 11:22:54.000000 django-privates-1.5.0/privates/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-01-03 11:22:54.000000 django-privates-1.5.0/privates/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-01-03 11:22:54.000000 django-privates-1.5.0/privates/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-01-03 11:22:58.190327 django-privates-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-03 11:22:54.000000 django-privates-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:06:04.654770 django-privates-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-05 16:05:57.000000 django-privates-2.0.0/Changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 16:05:57.000000 django-privates-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 16:05:57.000000 django-privates-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-05 16:06:04.654770 django-privates-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-05 16:05:57.000000 django-privates-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:06:04.654770 django-privates-2.0.0/django_privates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-05 16:06:04.000000 django-privates-2.0.0/django_privates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-05 16:06:04.000000 django-privates-2.0.0/django_privates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:06:04.000000 django-privates-2.0.0/django_privates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:06:04.000000 django-privates-2.0.0/django_privates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-05 16:06:04.000000 django-privates-2.0.0/django_privates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 16:06:04.000000 django-privates-2.0.0/django_privates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:06:04.654770 django-privates-2.0.0/privates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/storages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:06:04.650770 django-privates-2.0.0/privates/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:06:04.650770 django-privates-2.0.0/privates/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:06:04.654770 django-privates-2.0.0/privates/templates/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/templates/admin/widgets/clearable_private_file_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-05 16:05:57.000000 django-privates-2.0.0/privates/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-05 16:06:04.654770 django-privates-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:05:57.000000 django-privates-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:06:04.654770 django-privates-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-05 16:05:57.000000 django-privates-2.0.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-05 16:05:57.000000 django-privates-2.0.0/tests/test_modelfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-05 16:05:57.000000 django-privates-2.0.0/tests/test_storage.py
```

### Comparing `django-privates-1.5.0/Changelog.rst` & `django-privates-2.0.0/Changelog.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 =========
 Changelog
 =========
 
+2.0.0 (2023-05-05)
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
 1.5.0 (2023-01-03)
 ==================
 
 Feature release
 
 * Added ``privates.admin.PrivateMediaMixin.private_media_no_download_fields`` so admin
   classes can mark fields for which no file download URL/view should be generated
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-privates-1.5.0/LICENSE` & `django-privates-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-privates-1.5.0/PKG-INFO` & `django-privates-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: django-privates
-Version: 1.5.0
+Version: 2.0.0
 Summary: Batteries included private media integration in Django
 Home-page: https://github.com/sergei-maertens/django-privates
 Author: Sergei Maertens
 Author-email: info@regex-it.nl
 Keywords: django,media,private,storage
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
 License-File: LICENSE
@@ -30,15 +30,15 @@
 ============================================
 Django-privates - private media integrration
 ============================================
 
 Django-privates makes it easy to work with login-protected ``FileField``\ s,
 all the way through your application.
 
-:Version: 1.5.0
+:Version: 2.0.0
 :Source: https://github.com/sergei-maertens/django-privates
 :Keywords: django, media, private, storage
 
 |build-status| |linting| |coverage| |docs| |python-versions| |django-versions| |pypi-version|
 
 .. contents::
```

### Comparing `django-privates-1.5.0/README.rst` & `django-privates-2.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ============================================
 Django-privates - private media integrration
 ============================================
 
 Django-privates makes it easy to work with login-protected ``FileField``\ s,
 all the way through your application.
 
-:Version: 1.5.0
+:Version: 2.0.0
 :Source: https://github.com/sergei-maertens/django-privates
 :Keywords: django, media, private, storage
 
 |build-status| |linting| |coverage| |docs| |python-versions| |django-versions| |pypi-version|
 
 .. contents::
```

### Comparing `django-privates-1.5.0/django_privates.egg-info/PKG-INFO` & `django-privates-2.0.0/django_privates.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: django-privates
-Version: 1.5.0
+Version: 2.0.0
 Summary: Batteries included private media integration in Django
 Home-page: https://github.com/sergei-maertens/django-privates
 Author: Sergei Maertens
 Author-email: info@regex-it.nl
 Keywords: django,media,private,storage
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
 License-File: LICENSE
@@ -30,15 +30,15 @@
 ============================================
 Django-privates - private media integrration
 ============================================
 
 Django-privates makes it easy to work with login-protected ``FileField``\ s,
 all the way through your application.
 
-:Version: 1.5.0
+:Version: 2.0.0
 :Source: https://github.com/sergei-maertens/django-privates
 :Keywords: django, media, private, storage
 
 |build-status| |linting| |coverage| |docs| |python-versions| |django-versions| |pypi-version|
 
 .. contents::
```

### Comparing `django-privates-1.5.0/django_privates.egg-info/SOURCES.txt` & `django-privates-2.0.0/django_privates.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,8 +15,11 @@
 privates/apps.py
 privates/fields.py
 privates/py.typed
 privates/storages.py
 privates/test.py
 privates/views.py
 privates/widgets.py
-privates/templates/admin/widgets/clearable_private_file_input.html
+privates/templates/admin/widgets/clearable_private_file_input.html
+tests/test_admin.py
+tests/test_modelfield.py
+tests/test_storage.py
```

### Comparing `django-privates-1.5.0/privates/admin.py` & `django-privates-2.0.0/privates/admin.py`

 * *Files identical despite different names*

### Comparing `django-privates-1.5.0/privates/storages.py` & `django-privates-2.0.0/privates/storages.py`

 * *Files identical despite different names*

### Comparing `django-privates-1.5.0/privates/templates/admin/widgets/clearable_private_file_input.html` & `django-privates-2.0.0/privates/templates/admin/widgets/clearable_private_file_input.html`

 * *Files identical despite different names*

### Comparing `django-privates-1.5.0/privates/views.py` & `django-privates-2.0.0/privates/views.py`

 * *Files identical despite different names*

### Comparing `django-privates-1.5.0/privates/widgets.py` & `django-privates-2.0.0/privates/widgets.py`

 * *Files identical despite different names*

### Comparing `django-privates-1.5.0/setup.cfg` & `django-privates-2.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [metadata]
 name = django-privates
-version = 1.5.0
+version = 2.0.0
 description = Batteries included private media integration in Django
 long_description = file: README.rst
 url = https://github.com/sergei-maertens/django-privates
 license = 
 author = Sergei Maertens
 author_email = info@regex-it.nl
 keywords = django, media, private, storage
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

