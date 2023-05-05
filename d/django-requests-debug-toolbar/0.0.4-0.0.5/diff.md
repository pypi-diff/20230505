# Comparing `tmp/django-requests-debug-toolbar-0.0.4.tar.gz` & `tmp/django-requests-debug-toolbar-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-requests-debug-toolbar-0.0.4.tar", last modified: Fri May  5 09:07:51 2023, max compression
+gzip compressed data, was "django-requests-debug-toolbar-0.0.5.tar", last modified: Fri May  5 09:22:39 2023, max compression
```

## Comparing `django-requests-debug-toolbar-0.0.4.tar` & `django-requests-debug-toolbar-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:07:51.338771 django-requests-debug-toolbar-0.0.4/
--rw-r--r--   0 mts        (501) staff       (20)     1059 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.4/LICENSE
--rw-r--r--   0 mts        (501) staff       (20)       80 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.4/MANIFEST.in
--rw-r--r--   0 mts        (501) staff       (20)     1773 2023-05-05 09:07:51.339019 django-requests-debug-toolbar-0.0.4/PKG-INFO
--rw-r--r--   0 mts        (501) staff       (20)      591 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.4/README.rst
-drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:07:51.337104 django-requests-debug-toolbar-0.0.4/django_requests_debug_toolbar.egg-info/
--rw-r--r--   0 mts        (501) staff       (20)     1773 2023-05-05 09:07:51.000000 django-requests-debug-toolbar-0.0.4/django_requests_debug_toolbar.egg-info/PKG-INFO
--rw-r--r--   0 mts        (501) staff       (20)      441 2023-05-05 09:07:51.000000 django-requests-debug-toolbar-0.0.4/django_requests_debug_toolbar.egg-info/SOURCES.txt
--rw-r--r--   0 mts        (501) staff       (20)        1 2023-05-05 09:07:51.000000 django-requests-debug-toolbar-0.0.4/django_requests_debug_toolbar.egg-info/dependency_links.txt
--rw-r--r--   0 mts        (501) staff       (20)       26 2023-05-05 09:07:51.000000 django-requests-debug-toolbar-0.0.4/django_requests_debug_toolbar.egg-info/requires.txt
--rw-r--r--   0 mts        (501) staff       (20)       15 2023-05-05 09:07:51.000000 django-requests-debug-toolbar-0.0.4/django_requests_debug_toolbar.egg-info/top_level.txt
-drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:07:51.338065 django-requests-debug-toolbar-0.0.4/requests_panel/
--rw-r--r--   0 mts        (501) staff       (20)       22 2023-05-05 09:07:17.000000 django-requests-debug-toolbar-0.0.4/requests_panel/__init__.py
--rw-r--r--   0 mts        (501) staff       (20)     3833 2023-05-05 09:05:48.000000 django-requests-debug-toolbar-0.0.4/requests_panel/panel.py
-drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:07:51.333743 django-requests-debug-toolbar-0.0.4/requests_panel/templates/
-drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:07:51.338491 django-requests-debug-toolbar-0.0.4/requests_panel/templates/requests_panel/
--rw-r--r--   0 mts        (501) staff       (20)     1675 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.4/requests_panel/templates/requests_panel/panel.html
--rw-r--r--   0 mts        (501) staff       (20)     4394 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.4/requests_panel/tracker.py
--rw-r--r--   0 mts        (501) staff       (20)      233 2023-05-05 09:07:51.339867 django-requests-debug-toolbar-0.0.4/setup.cfg
--rw-r--r--   0 mts        (501) staff       (20)     1475 2023-05-05 09:07:48.000000 django-requests-debug-toolbar-0.0.4/setup.py
+drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:22:39.218896 django-requests-debug-toolbar-0.0.5/
+-rw-r--r--   0 mts        (501) staff       (20)     1059 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.5/LICENSE
+-rw-r--r--   0 mts        (501) staff       (20)       80 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.5/MANIFEST.in
+-rw-r--r--   0 mts        (501) staff       (20)     1773 2023-05-05 09:22:39.219155 django-requests-debug-toolbar-0.0.5/PKG-INFO
+-rw-r--r--   0 mts        (501) staff       (20)      591 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.5/README.rst
+drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:22:39.215842 django-requests-debug-toolbar-0.0.5/django_requests_debug_toolbar.egg-info/
+-rw-r--r--   0 mts        (501) staff       (20)     1773 2023-05-05 09:22:39.000000 django-requests-debug-toolbar-0.0.5/django_requests_debug_toolbar.egg-info/PKG-INFO
+-rw-r--r--   0 mts        (501) staff       (20)      441 2023-05-05 09:22:39.000000 django-requests-debug-toolbar-0.0.5/django_requests_debug_toolbar.egg-info/SOURCES.txt
+-rw-r--r--   0 mts        (501) staff       (20)        1 2023-05-05 09:22:39.000000 django-requests-debug-toolbar-0.0.5/django_requests_debug_toolbar.egg-info/dependency_links.txt
+-rw-r--r--   0 mts        (501) staff       (20)       26 2023-05-05 09:22:39.000000 django-requests-debug-toolbar-0.0.5/django_requests_debug_toolbar.egg-info/requires.txt
+-rw-r--r--   0 mts        (501) staff       (20)       15 2023-05-05 09:22:39.000000 django-requests-debug-toolbar-0.0.5/django_requests_debug_toolbar.egg-info/top_level.txt
+drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:22:39.216886 django-requests-debug-toolbar-0.0.5/requests_panel/
+-rw-r--r--   0 mts        (501) staff       (20)       22 2023-05-05 09:22:14.000000 django-requests-debug-toolbar-0.0.5/requests_panel/__init__.py
+-rw-r--r--   0 mts        (501) staff       (20)     3836 2023-05-05 09:20:47.000000 django-requests-debug-toolbar-0.0.5/requests_panel/panel.py
+drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:22:39.212453 django-requests-debug-toolbar-0.0.5/requests_panel/templates/
+drwxr-xr-x   0 mts        (501) staff       (20)        0 2023-05-05 09:22:39.218056 django-requests-debug-toolbar-0.0.5/requests_panel/templates/requests_panel/
+-rw-r--r--   0 mts        (501) staff       (20)     1675 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.5/requests_panel/templates/requests_panel/panel.html
+-rw-r--r--   0 mts        (501) staff       (20)     4394 2023-05-05 09:04:54.000000 django-requests-debug-toolbar-0.0.5/requests_panel/tracker.py
+-rw-r--r--   0 mts        (501) staff       (20)      233 2023-05-05 09:22:39.219943 django-requests-debug-toolbar-0.0.5/setup.cfg
+-rw-r--r--   0 mts        (501) staff       (20)     1475 2023-05-05 09:21:19.000000 django-requests-debug-toolbar-0.0.5/setup.py
```

### Comparing `django-requests-debug-toolbar-0.0.4/LICENSE` & `django-requests-debug-toolbar-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-requests-debug-toolbar-0.0.4/PKG-INFO` & `django-requests-debug-toolbar-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-requests-debug-toolbar
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Django Debug Toolbar panel for Requests
 Home-page: https://github.com/marceltschoppch/django-requests-debug-toolbar
 Author: Marcel Tschopp
 Author-email: info@marceltschopp.ch
 License: MIT
 Description: django-requests-debug-toolbar
         =============================
```

### Comparing `django-requests-debug-toolbar-0.0.4/README.rst` & `django-requests-debug-toolbar-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `django-requests-debug-toolbar-0.0.4/django_requests_debug_toolbar.egg-info/PKG-INFO` & `django-requests-debug-toolbar-0.0.5/django_requests_debug_toolbar.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-requests-debug-toolbar
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Django Debug Toolbar panel for Requests
 Home-page: https://github.com/marceltschoppch/django-requests-debug-toolbar
 Author: Marcel Tschopp
 Author-email: info@marceltschopp.ch
 License: MIT
 Description: django-requests-debug-toolbar
         =============================
```

### Comparing `django-requests-debug-toolbar-0.0.4/requests_panel/panel.py` & `django-requests-debug-toolbar-0.0.5/requests_panel/panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,20 +92,20 @@
     nav_title = title
     template = 'requests_panel/panel.html'
     has_content = True
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._local = threading.local()
-        self._local.request_count = 0
 
     @property
     def nav_subtitle(self):
-        return ngettext('%(count)s request', '%(count)s requests', self._local.request_count) % {
-            'count': self._local.request_count,
+        request_count = getattr(self._local, 'request_count', 0)
+        return ngettext('%(count)s request', '%(count)s requests', request_count) % {
+            'count': request_count,
         }
 
     def process_request(self, request):
         collector.clear_collection()
         return super().process_request(request)
 
     def generate_stats(self, request, response):
```

### Comparing `django-requests-debug-toolbar-0.0.4/requests_panel/templates/requests_panel/panel.html` & `django-requests-debug-toolbar-0.0.5/requests_panel/templates/requests_panel/panel.html`

 * *Files identical despite different names*

### Comparing `django-requests-debug-toolbar-0.0.4/requests_panel/tracker.py` & `django-requests-debug-toolbar-0.0.5/requests_panel/tracker.py`

 * *Files identical despite different names*

### Comparing `django-requests-debug-toolbar-0.0.4/setup.py` & `django-requests-debug-toolbar-0.0.5/setup.py`

 * *Files identical despite different names*

