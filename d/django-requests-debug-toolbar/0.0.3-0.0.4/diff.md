# Comparing `tmp/django-requests-debug-toolbar-0.0.3.tar.gz` & `tmp/django-requests-debug-toolbar-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-requests-debug-toolbar-0.0.3.tar", last modified: Tue Sep 27 19:10:02 2022, max compression
+gzip compressed data, was "django-requests-debug-toolbar-0.0.4.tar", last modified: Fri May  5 09:07:51 2023, max compression
```

## Comparing `django-requests-debug-toolbar-0.0.3.tar` & `django-requests-debug-toolbar-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mts        (501) staff       (20)        0 2022-09-27 19:10:02.452952 django-requests-debug-toolbar-0.0.3/
--rw-r--r--   0 mts        (501) staff       (20)     1059 2022-09-27 18:50:31.000000 django-requests-debug-toolbar-0.0.3/LICENSE
--rw-r--r--   0 mts        (501) staff       (20)       80 2022-09-27 18:50:31.000000 django-requests-debug-toolbar-0.0.3/MANIFEST.in
--rw-r--r--   0 mts        (501) staff       (20)     1396 2022-09-27 19:10:02.453095 django-requests-debug-toolbar-0.0.3/PKG-INFO
--rw-r--r--   0 mts        (501) staff       (20)      591 2022-09-27 18:50:31.000000 django-requests-debug-toolbar-0.0.3/README.rst
-drwxr-xr-x   0 mts        (501) staff       (20)        0 2022-09-27 19:10:02.428442 django-requests-debug-toolbar-0.0.3/django_requests_debug_toolbar.egg-info/
--rw-r--r--   0 mts        (501) staff       (20)     1396 2022-09-27 19:10:02.000000 django-requests-debug-toolbar-0.0.3/django_requests_debug_toolbar.egg-info/PKG-INFO
--rw-r--r--   0 mts        (501) staff       (20)      441 2022-09-27 19:10:02.000000 django-requests-debug-toolbar-0.0.3/django_requests_debug_toolbar.egg-info/SOURCES.txt
--rw-r--r--   0 mts        (501) staff       (20)        1 2022-09-27 19:10:02.000000 django-requests-debug-toolbar-0.0.3/django_requests_debug_toolbar.egg-info/dependency_links.txt
--rw-r--r--   0 mts        (501) staff       (20)       26 2022-09-27 19:10:02.000000 django-requests-debug-toolbar-0.0.3/django_requests_debug_toolbar.egg-info/requires.txt
--rw-r--r--   0 mts        (501) staff       (20)       15 2022-09-27 19:10:02.000000 django-requests-debug-toolbar-0.0.3/django_requests_debug_toolbar.egg-info/top_level.txt
-drwxr-xr-x   0 mts        (501) staff       (20)        0 2022-09-27 19:10:02.451892 django-requests-debug-toolbar-0.0.3/requests_panel/
--rw-r--r--   0 mts        (501) staff       (20)       22 2022-09-27 19:05:17.000000 django-requests-debug-toolbar-0.0.3/requests_panel/__init__.py
--rw-r--r--   0 mts        (501) staff       (20)     3795 2022-09-27 19:03:29.000000 django-requests-debug-toolbar-0.0.3/requests_panel/panel.py
-drwxr-xr-x   0 mts        (501) staff       (20)        0 2022-09-27 19:10:02.424842 django-requests-debug-toolbar-0.0.3/requests_panel/templates/
-drwxr-xr-x   0 mts        (501) staff       (20)        0 2022-09-27 19:10:02.452545 django-requests-debug-toolbar-0.0.3/requests_panel/templates/requests_panel/
--rw-r--r--   0 mts        (501) staff       (20)     1675 2022-09-27 18:50:31.000000 django-requests-debug-toolbar-0.0.3/requests_panel/templates/requests_panel/panel.html
--rw-r--r--   0 mts        (501) staff       (20)     4394 2022-09-27 18:50:31.000000 django-requests-debug-toolbar-0.0.3/requests_panel/tracker.py
--rw-r--r--   0 mts        (501) staff       (20)      233 2022-09-27 19:10:02.453622 django-requests-debug-toolbar-0.0.3/setup.cfg
--rw-r--r--   0 mts        (501) staff       (20)     1326 2022-09-27 18:50:31.000000 django-requests-debug-toolbar-0.0.3/setup.py
+drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:07:51.338771 django-requests-debug-toolbar-0.0.4/
+-rw-r--r--   0 mts        (501) staff       (20)     1059 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.4/LICENSE
+-rw-r--r--   0 mts        (501) staff       (20)       80 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.4/MANIFEST.in
+-rw-r--r--   0 mts        (501) staff       (20)     1773 2023-05-05 09:07:51.339019 django-requests-debug-toolbar-0.0.4/PKG-INFO
+-rw-r--r--   0 mts        (501) staff       (20)      591 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.4/README.rst
+drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:07:51.337104 django-requests-debug-toolbar-0.0.4/django_requests_debug_toolbar.egg-info/
+-rw-r--r--   0 mts        (501) staff       (20)     1773 2023-05-05 09:07:51.000000 django-requests-debug-toolbar-0.0.4/django_requests_debug_toolbar.egg-info/PKG-INFO
+-rw-r--r--   0 mts        (501) staff       (20)      441 2023-05-05 09:07:51.000000 django-requests-debug-toolbar-0.0.4/django_requests_debug_toolbar.egg-info/SOURCES.txt
+-rw-r--r--   0 mts        (501) staff       (20)        1 2023-05-05 09:07:51.000000 django-requests-debug-toolbar-0.0.4/django_requests_debug_toolbar.egg-info/dependency_links.txt
+-rw-r--r--   0 mts        (501) staff       (20)       26 2023-05-05 09:07:51.000000 django-requests-debug-toolbar-0.0.4/django_requests_debug_toolbar.egg-info/requires.txt
+-rw-r--r--   0 mts        (501) staff       (20)       15 2023-05-05 09:07:51.000000 django-requests-debug-toolbar-0.0.4/django_requests_debug_toolbar.egg-info/top_level.txt
+drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:07:51.338065 django-requests-debug-toolbar-0.0.4/requests_panel/
+-rw-r--r--   0 mts        (501) staff       (20)       22 2023-05-05 09:07:17.000000 django-requests-debug-toolbar-0.0.4/requests_panel/__init__.py
+-rw-r--r--   0 mts        (501) staff       (20)     3833 2023-05-05 09:05:48.000000 django-requests-debug-toolbar-0.0.4/requests_panel/panel.py
+drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:07:51.333743 django-requests-debug-toolbar-0.0.4/requests_panel/templates/
+drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:07:51.338491 django-requests-debug-toolbar-0.0.4/requests_panel/templates/requests_panel/
+-rw-r--r--   0 mts        (501) staff       (20)     1675 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.4/requests_panel/templates/requests_panel/panel.html
+-rw-r--r--   0 mts        (501) staff       (20)     4394 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.4/requests_panel/tracker.py
+-rw-r--r--   0 mts        (501) staff       (20)      233 2023-05-05 09:07:51.339867 django-requests-debug-toolbar-0.0.4/setup.cfg
+-rw-r--r--   0 mts        (501) staff       (20)     1475 2023-05-05 09:07:48.000000 django-requests-debug-toolbar-0.0.4/setup.py
```

### Comparing `django-requests-debug-toolbar-0.0.3/LICENSE` & `django-requests-debug-toolbar-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-requests-debug-toolbar-0.0.3/README.rst` & `django-requests-debug-toolbar-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-requests-debug-toolbar-0.0.3/requests_panel/panel.py` & `django-requests-debug-toolbar-0.0.4/requests_panel/panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     nav_title = title
     template = 'requests_panel/panel.html'
     has_content = True
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._local = threading.local()
+        self._local.request_count = 0
 
     @property
     def nav_subtitle(self):
         return ngettext('%(count)s request', '%(count)s requests', self._local.request_count) % {
             'count': self._local.request_count,
         }
```

### Comparing `django-requests-debug-toolbar-0.0.3/requests_panel/templates/requests_panel/panel.html` & `django-requests-debug-toolbar-0.0.4/requests_panel/templates/requests_panel/panel.html`

 * *Files identical despite different names*

### Comparing `django-requests-debug-toolbar-0.0.3/requests_panel/tracker.py` & `django-requests-debug-toolbar-0.0.4/requests_panel/tracker.py`

 * *Files identical despite different names*

### Comparing `django-requests-debug-toolbar-0.0.3/setup.py` & `django-requests-debug-toolbar-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,9 +33,12 @@
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

