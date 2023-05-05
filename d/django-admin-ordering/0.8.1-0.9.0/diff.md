# Comparing `tmp/django-admin-ordering-0.8.1.tar.gz` & `tmp/django-admin-ordering-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-admin-ordering-0.8.1.tar", last modified: Thu Mar 15 16:15:43 2018, max compression
+gzip compressed data, was "dist/django-admin-ordering-0.9.0.tar", last modified: Mon Aug 27 11:51:56 2018, max compression
```

## Comparing `django-admin-ordering-0.8.1.tar` & `django-admin-ordering-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2018-03-15 16:15:43.000000 django-admin-ordering-0.8.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2343 2018-03-15 16:06:13.000000 django-admin-ordering-0.8.1/README.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       65 2017-10-23 11:30:35.000000 django-admin-ordering-0.8.1/AUTHORS
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1754 2017-10-23 11:30:35.000000 django-admin-ordering-0.8.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2018-03-15 16:15:43.000000 django-admin-ordering-0.8.1/django_admin_ordering.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      633 2018-03-15 16:15:43.000000 django-admin-ordering-0.8.1/django_admin_ordering.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2018-03-15 16:15:41.000000 django-admin-ordering-0.8.1/django_admin_ordering.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2018-03-15 16:15:41.000000 django-admin-ordering-0.8.1/django_admin_ordering.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3965 2018-03-15 16:15:41.000000 django-admin-ordering-0.8.1/django_admin_ordering.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2017-10-23 11:37:36.000000 django-admin-ordering-0.8.1/django_admin_ordering.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2018-03-15 16:15:41.000000 django-admin-ordering-0.8.1/django_admin_ordering.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      421 2017-10-23 11:30:35.000000 django-admin-ordering-0.8.1/CONTRIBUTING.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3965 2018-03-15 16:15:43.000000 django-admin-ordering-0.8.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2017-10-23 11:30:35.000000 django-admin-ordering-0.8.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      512 2018-03-15 16:15:43.000000 django-admin-ordering-0.8.1/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2018-03-15 16:15:43.000000 django-admin-ordering-0.8.1/admin_ordering/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2018-03-15 16:15:43.000000 django-admin-ordering-0.8.1/admin_ordering/static/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2018-03-15 16:15:43.000000 django-admin-ordering-0.8.1/admin_ordering/static/admin_ordering/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37940 2018-01-25 15:33:13.000000 django-admin-ordering-0.8.1/admin_ordering/static/admin_ordering/jquery-ui-1.11.4.custom.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2018-03-15 14:12:50.000000 django-admin-ordering-0.8.1/admin_ordering/static/admin_ordering/admin_ordering.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5637 2018-03-15 15:45:31.000000 django-admin-ordering-0.8.1/admin_ordering/static/admin_ordering/admin_ordering.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      607 2018-03-15 14:12:50.000000 django-admin-ordering-0.8.1/admin_ordering/static/admin_ordering/admin_ordering-icon.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      121 2018-03-15 16:06:42.000000 django-admin-ordering-0.8.1/admin_ordering/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2371 2018-03-15 16:06:13.000000 django-admin-ordering-0.8.1/admin_ordering/admin.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1550 2017-10-23 11:30:35.000000 django-admin-ordering-0.8.1/LICENSE
+drwxrwxr-x   0 matthias  (1000) matthias  (1004)        0 2018-08-27 11:51:56.000000 django-admin-ordering-0.9.0/
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)       65 2017-10-23 11:30:35.000000 django-admin-ordering-0.9.0/AUTHORS
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)     1550 2017-10-23 11:30:35.000000 django-admin-ordering-0.9.0/LICENSE
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)      421 2017-10-23 11:30:35.000000 django-admin-ordering-0.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)      225 2017-10-23 11:30:35.000000 django-admin-ordering-0.9.0/MANIFEST.in
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)     3965 2018-08-27 11:51:56.000000 django-admin-ordering-0.9.0/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)     2343 2018-05-13 18:19:51.000000 django-admin-ordering-0.9.0/README.rst
+-rwxrwxr-x   0 matthias  (1000) matthias  (1004)     1754 2017-10-23 11:30:35.000000 django-admin-ordering-0.9.0/setup.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1004)        0 2018-08-27 11:51:56.000000 django-admin-ordering-0.9.0/admin_ordering/
+drwxrwxr-x   0 matthias  (1000) matthias  (1004)        0 2018-08-27 11:51:56.000000 django-admin-ordering-0.9.0/admin_ordering/static/
+drwxrwxr-x   0 matthias  (1000) matthias  (1004)        0 2018-08-27 11:51:56.000000 django-admin-ordering-0.9.0/admin_ordering/static/admin_ordering/
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)     5700 2018-08-27 11:35:34.000000 django-admin-ordering-0.9.0/admin_ordering/static/admin_ordering/admin_ordering.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)     1808 2018-08-27 10:02:17.000000 django-admin-ordering-0.9.0/admin_ordering/static/admin_ordering/admin_ordering.css
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)    37940 2018-08-27 10:02:17.000000 django-admin-ordering-0.9.0/admin_ordering/static/admin_ordering/jquery-ui-1.11.4.custom.min.js
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)      607 2018-08-27 10:02:17.000000 django-admin-ordering-0.9.0/admin_ordering/static/admin_ordering/admin_ordering-icon.svg
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)      121 2018-08-27 11:51:08.000000 django-admin-ordering-0.9.0/admin_ordering/__init__.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)     2449 2018-08-27 11:40:10.000000 django-admin-ordering-0.9.0/admin_ordering/admin.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1004)        0 2018-08-27 11:51:56.000000 django-admin-ordering-0.9.0/django_admin_ordering.egg-info/
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)      633 2018-08-27 11:51:56.000000 django-admin-ordering-0.9.0/django_admin_ordering.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)        1 2017-10-23 11:37:36.000000 django-admin-ordering-0.9.0/django_admin_ordering.egg-info/not-zip-safe
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)     3965 2018-08-27 11:51:56.000000 django-admin-ordering-0.9.0/django_admin_ordering.egg-info/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)       16 2018-08-27 11:51:56.000000 django-admin-ordering-0.9.0/django_admin_ordering.egg-info/requires.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)        1 2018-08-27 11:51:56.000000 django-admin-ordering-0.9.0/django_admin_ordering.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)       15 2018-08-27 11:51:56.000000 django-admin-ordering-0.9.0/django_admin_ordering.egg-info/top_level.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1004)      247 2018-08-27 11:51:56.000000 django-admin-ordering-0.9.0/setup.cfg
```

### Comparing `django-admin-ordering-0.8.1/README.rst` & `django-admin-ordering-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-admin-ordering-0.8.1/setup.py` & `django-admin-ordering-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-admin-ordering-0.8.1/django_admin_ordering.egg-info/SOURCES.txt` & `django-admin-ordering-0.9.0/django_admin_ordering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-ordering-0.8.1/django_admin_ordering.egg-info/PKG-INFO` & `django-admin-ordering-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-admin-ordering
-Version: 0.8.1
+Version: 0.9.0
 Summary: Orderable change lists and inlines done right^Wsimple
 Home-page: https://github.com/matthiask/django-admin-ordering/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: BSD License
 Description: ==============================================================================
         django-admin-ordering -- Orderable change lists and inlines done right^Wsimple
```

### Comparing `django-admin-ordering-0.8.1/PKG-INFO` & `django-admin-ordering-0.9.0/django_admin_ordering.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-admin-ordering
-Version: 0.8.1
+Version: 0.9.0
 Summary: Orderable change lists and inlines done right^Wsimple
 Home-page: https://github.com/matthiask/django-admin-ordering/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: BSD License
 Description: ==============================================================================
         django-admin-ordering -- Orderable change lists and inlines done right^Wsimple
```

### Comparing `django-admin-ordering-0.8.1/admin_ordering/static/admin_ordering/jquery-ui-1.11.4.custom.min.js` & `django-admin-ordering-0.9.0/admin_ordering/static/admin_ordering/jquery-ui-1.11.4.custom.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-ordering-0.8.1/admin_ordering/static/admin_ordering/admin_ordering.css` & `django-admin-ordering-0.9.0/admin_ordering/static/admin_ordering/admin_ordering.css`

 * *Files identical despite different names*

### Comparing `django-admin-ordering-0.8.1/admin_ordering/static/admin_ordering/admin_ordering.js` & `django-admin-ordering-0.9.0/admin_ordering/static/admin_ordering/admin_ordering.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -61,15 +61,15 @@
 
             $sortable = $('#' + data.prefix + '-group tbody');
             $sortableHandle = $sortable.find('.field-' + data.field);
             $sortableHandle.addClass('admin-ordering-field');
             if (data.fieldHideInput) {
                 $sortableHandle.addClass('admin-ordering-field-hide-input');
             }
-            $sortableHandle.find('input').wrap($sortableInputWrapper);
+            $sortableHandle.find('input:not([type="hidden"])').wrap($sortableInputWrapper);
             $sortable.sortable({
                 items: '>.has_original',
                 handle: $sortableHandle,
                 start: function(event, ui) {
                     hideHorizontalOverflow();
                     updatePlaceholderHeight(ui);
                     // fix ui item height
@@ -91,15 +91,15 @@
 
             $sortable = $('#' + data.prefix + '-group');
             $sortableHandle = $sortable.find('.field-' + data.field);
             $sortableHandle.addClass('admin-ordering-field');
             if (data.fieldHideInput) {
                 $sortableHandle.addClass('admin-ordering-field-hide-input');
             }
-            $sortableHandle.find('input').wrap($sortableInputWrapper);
+            $sortableHandle.find('input:not([type="hidden"])').wrap($sortableInputWrapper);
             $sortable.sortable({
                 items: '>.has_original,>>.has_original',
                 handle: $sortableHandle,
                 start: function(event, ui) {
                     hideHorizontalOverflow();
                     updatePlaceholderHeight(ui);
                 },
@@ -118,15 +118,15 @@
             $sortableHandle.addClass('admin-ordering-field');
             if (data.fieldHideInput) {
                 $sortableHandle.addClass('admin-ordering-field-hide-input');
             }
             if (!$sortableHandle.find('input').length) {
                 return;
             }
-            $sortableHandle.find('input').wrap($sortableInputWrapper);
+            $sortableHandle.find('input:not([type="hidden"])').wrap($sortableInputWrapper);
             $sortable.sortable({
                 handle: $sortableHandle,
                 start: function(event, ui) {
                     hideHorizontalOverflow();
                     updatePlaceholderHeight(ui);
                 },
                 update: function(event, ui) {
```

### Comparing `django-admin-ordering-0.8.1/admin_ordering/static/admin_ordering/admin_ordering-icon.svg` & `django-admin-ordering-0.9.0/admin_ordering/static/admin_ordering/admin_ordering-icon.svg`

 * *Files identical despite different names*

### Comparing `django-admin-ordering-0.8.1/LICENSE` & `django-admin-ordering-0.9.0/LICENSE`

 * *Files identical despite different names*

