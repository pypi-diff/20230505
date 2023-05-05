# Comparing `tmp/django-dragndrop-related-0.1.0.tar.gz` & `tmp/django-dragndrop-related-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-dragndrop-related-0.1.0.tar", last modified: Tue Jun 14 14:56:37 2022, max compression
+gzip compressed data, was "django-dragndrop-related-0.2.0.tar", last modified: Fri May  5 09:25:23 2023, max compression
```

## Comparing `django-dragndrop-related-0.1.0.tar` & `django-dragndrop-related-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-06-14 14:56:37.470118 django-dragndrop-related-0.1.0/
--rw-r--r--   0 james      (501) staff       (20)     1070 2022-06-14 13:19:32.000000 django-dragndrop-related-0.1.0/LICENSE
--rw-r--r--   0 james      (501) staff       (20)      107 2022-06-14 13:32:35.000000 django-dragndrop-related-0.1.0/MANIFEST.in
--rw-r--r--   0 james      (501) staff       (20)     6796 2022-06-14 14:56:37.470379 django-dragndrop-related-0.1.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     5795 2022-06-14 14:54:30.000000 django-dragndrop-related-0.1.0/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-06-14 14:56:37.461258 django-dragndrop-related-0.1.0/django_dragndrop_related.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     6796 2022-06-14 14:56:36.000000 django-dragndrop-related-0.1.0/django_dragndrop_related.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      823 2022-06-14 14:56:37.000000 django-dragndrop-related-0.1.0/django_dragndrop_related.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2022-06-14 14:56:37.000000 django-dragndrop-related-0.1.0/django_dragndrop_related.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2022-06-14 13:36:24.000000 django-dragndrop-related-0.1.0/django_dragndrop_related.egg-info/not-zip-safe
--rw-r--r--   0 james      (501) staff       (20)      159 2022-06-14 14:56:37.000000 django-dragndrop-related-0.1.0/django_dragndrop_related.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       34 2022-06-14 14:56:37.000000 django-dragndrop-related-0.1.0/django_dragndrop_related.egg-info/top_level.txt
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-06-14 14:56:37.462508 django-dragndrop-related-0.1.0/dragndrop_related/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:56:04.000000 django-dragndrop-related-0.1.0/dragndrop_related/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-06-14 14:56:37.463009 django-dragndrop-related-0.1.0/dragndrop_related/templates/
--rw-r--r--   0 james      (501) staff       (20)     2609 2022-06-14 13:32:04.000000 django-dragndrop-related-0.1.0/dragndrop_related/templates/change_form.html
--rw-r--r--   0 james      (501) staff       (20)     7133 2022-06-14 14:19:54.000000 django-dragndrop-related-0.1.0/dragndrop_related/views.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-06-14 14:56:37.466472 django-dragndrop-related-0.1.0/example_project/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:34:34.000000 django-dragndrop-related-0.1.0/example_project/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      407 2022-06-14 13:34:34.000000 django-dragndrop-related-0.1.0/example_project/asgi.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-06-14 14:56:37.468628 django-dragndrop-related-0.1.0/example_project/gallery/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:34:34.000000 django-dragndrop-related-0.1.0/example_project/gallery/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      387 2022-06-14 14:19:59.000000 django-dragndrop-related-0.1.0/example_project/gallery/admin.py
--rw-r--r--   0 james      (501) staff       (20)      146 2022-06-14 13:49:16.000000 django-dragndrop-related-0.1.0/example_project/gallery/apps.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2022-06-14 14:56:37.469782 django-dragndrop-related-0.1.0/example_project/gallery/migrations/
--rw-r--r--   0 james      (501) staff       (20)     1005 2022-06-14 14:22:18.000000 django-dragndrop-related-0.1.0/example_project/gallery/migrations/0001_initial.py
--rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:34:34.000000 django-dragndrop-related-0.1.0/example_project/gallery/migrations/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      423 2022-06-14 14:00:13.000000 django-dragndrop-related-0.1.0/example_project/gallery/models.py
--rwxr-xr-x   0 james      (501) staff       (20)      671 2022-06-14 13:34:34.000000 django-dragndrop-related-0.1.0/example_project/manage.py
--rw-r--r--   0 james      (501) staff       (20)     3533 2022-06-14 14:05:30.000000 django-dragndrop-related-0.1.0/example_project/settings.py
--rw-r--r--   0 james      (501) staff       (20)      960 2022-06-14 14:06:49.000000 django-dragndrop-related-0.1.0/example_project/urls.py
--rw-r--r--   0 james      (501) staff       (20)      407 2022-06-14 13:34:34.000000 django-dragndrop-related-0.1.0/example_project/wsgi.py
--rw-r--r--   0 james      (501) staff       (20)      115 2022-06-14 14:56:37.471299 django-dragndrop-related-0.1.0/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     2003 2022-06-14 14:00:57.000000 django-dragndrop-related-0.1.0/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.954630 django-dragndrop-related-0.2.0/
+-rw-r--r--   0 james      (501) staff       (20)     1070 2022-06-14 13:19:32.000000 django-dragndrop-related-0.2.0/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)      107 2022-06-14 13:32:35.000000 django-dragndrop-related-0.2.0/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)     7431 2023-05-05 09:25:23.955267 django-dragndrop-related-0.2.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     6430 2023-05-05 09:20:18.000000 django-dragndrop-related-0.2.0/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.942214 django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     7431 2023-05-05 09:25:23.000000 django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      847 2023-05-05 09:25:23.000000 django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-05-05 09:25:23.000000 django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2022-06-14 13:36:24.000000 django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/not-zip-safe
+-rw-r--r--   0 james      (501) staff       (20)      159 2023-05-05 09:25:23.000000 django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       34 2023-05-05 09:25:23.000000 django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.942880 django-dragndrop-related-0.2.0/dragndrop_related/
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:56:04.000000 django-dragndrop-related-0.2.0/dragndrop_related/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.935554 django-dragndrop-related-0.2.0/dragndrop_related/templates/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.935682 django-dragndrop-related-0.2.0/dragndrop_related/templates/admin/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.943671 django-dragndrop-related-0.2.0/dragndrop_related/templates/admin/dragndrop_related/
+-rw-r--r--   0 james      (501) staff       (20)     2612 2023-05-05 09:14:23.000000 django-dragndrop-related-0.2.0/dragndrop_related/templates/admin/dragndrop_related/change_form.html
+-rw-r--r--   0 james      (501) staff       (20)     7915 2023-05-05 09:15:48.000000 django-dragndrop-related-0.2.0/dragndrop_related/views.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.948601 django-dragndrop-related-0.2.0/example_project/
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:34:34.000000 django-dragndrop-related-0.2.0/example_project/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      407 2022-06-14 13:34:34.000000 django-dragndrop-related-0.2.0/example_project/asgi.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.951617 django-dragndrop-related-0.2.0/example_project/gallery/
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:34:34.000000 django-dragndrop-related-0.2.0/example_project/gallery/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      387 2022-06-14 14:19:59.000000 django-dragndrop-related-0.2.0/example_project/gallery/admin.py
+-rw-r--r--   0 james      (501) staff       (20)      146 2022-06-14 13:49:16.000000 django-dragndrop-related-0.2.0/example_project/gallery/apps.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.954321 django-dragndrop-related-0.2.0/example_project/gallery/migrations/
+-rw-r--r--   0 james      (501) staff       (20)     1005 2022-06-14 14:22:18.000000 django-dragndrop-related-0.2.0/example_project/gallery/migrations/0001_initial.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:34:34.000000 django-dragndrop-related-0.2.0/example_project/gallery/migrations/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      423 2022-06-14 14:00:13.000000 django-dragndrop-related-0.2.0/example_project/gallery/models.py
+-rwxr-xr-x   0 james      (501) staff       (20)      671 2022-06-14 13:34:34.000000 django-dragndrop-related-0.2.0/example_project/manage.py
+-rw-r--r--   0 james      (501) staff       (20)     3533 2022-06-14 14:05:30.000000 django-dragndrop-related-0.2.0/example_project/settings.py
+-rw-r--r--   0 james      (501) staff       (20)      960 2022-06-14 14:06:49.000000 django-dragndrop-related-0.2.0/example_project/urls.py
+-rw-r--r--   0 james      (501) staff       (20)      407 2022-06-14 13:34:34.000000 django-dragndrop-related-0.2.0/example_project/wsgi.py
+-rw-r--r--   0 james      (501) staff       (20)      115 2023-05-05 09:25:23.956952 django-dragndrop-related-0.2.0/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     2002 2023-05-05 09:23:58.000000 django-dragndrop-related-0.2.0/setup.py
```

### Comparing `django-dragndrop-related-0.1.0/LICENSE` & `django-dragndrop-related-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dragndrop-related-0.1.0/PKG-INFO` & `django-dragndrop-related-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dragndrop-related
-Version: 0.1.0
+Version: 0.2.0
 Summary: Drag-and-drop multiple uploading of related images/files for
 Home-page: http://github.com/BigglesZX/django-dragndrop-related
 Author: James Tiplady
 Maintainer: James Tiplady
 License: MIT
 Keywords: django
 Platform: OS Independent
@@ -37,15 +37,15 @@
 
 ## Rationale
 
 One of the most common requests I get from clients when working on Django projects is to support some kind of drag-and-drop upload to save them the tedium of working with multiple file upload fields. I finally put some effort into solving this problem and came up with this library, which essentially provides for the creation of related models via AJAX POST request.
 
 It assumes some simplicity on the part of the related model – e.g. that only an `ImageField` is required to be populated – and uses [Dropzone.js](https://www.dropzone.dev/js/) to accept uploads and fire off POST requests to an endpoint which creates new child models using the related manager of the parent model.
 
-I decided not to try to support drag-and-drop uploads when *creating* parent model instances, since the uploads would need to be stashed somewhere temporarily then associated with the new model when it was saved. Instead this library operates only on existing model instances and requires the user to reload the page once they're done dropping files, so that Django's admin/inline UI can display the newly created child models for editing. This is acceptable in my use-cases but may not be in yours.
+I decided not to try to support drag-and-drop uploads when _creating_ parent model instances, since the uploads would need to be stashed somewhere temporarily then associated with the new model when it was saved. Instead this library operates only on existing model instances and requires the user to reload the page once they're done dropping files, so that Django's admin/inline UI can display the newly created child models for editing. This is acceptable in my use-cases but may not be in yours.
 
 ## Compatibility
 
 This library has been tested on Django 3.2 and 4.0 on Python 3.8, though I expect it to be fairly compatible with other versions. For now, the package is marked as requiring Python 3.6 or higher.
 
 **Please note that this library is an early beta release, mostly published so that I can share code between my own projects. It works well for my specific use-case but your mileage may vary. If you have issues with the library please open a ticket, but be aware it's not being developed intensively at this stage.**
 
@@ -86,14 +86,27 @@
 
 
 @admin.register(Album)
 class AlbumAdmin(DragAndDropRelatedImageMixin, admin.ModelAdmin):
     inlines = [ImageInline]
 ```
 
+## Usage in combination with [`django-solo`](https://github.com/lazybird/django-solo)
+
+The `django-solo` library provides its own admin `change_form` template with some minimal UI changes to assist with singleton models. When using `django-dragndrop-related` with a `django-solo` singleton model, there is a different mixin which will preserve the proper template inheritance:
+
+```python
+from dragndrop_related.views import DragAndDropSingletonRelatedImageMixin
+from solo.admin import SingletonModelAdmin
+
+@admin.register(models.Homepage)
+class HomepageAdmin(DragAndDropSingletonRelatedImageMixin, SingletonModelAdmin):
+    # ...
+```
+
 ## Configuration
 
 The library makes a few assumptions about your models and their relationship. Consider the following example models:
 
 ```python
 class Album(models.Model):
     # ...
```

### Comparing `django-dragndrop-related-0.1.0/README.md` & `django-dragndrop-related-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ## Rationale
 
 One of the most common requests I get from clients when working on Django projects is to support some kind of drag-and-drop upload to save them the tedium of working with multiple file upload fields. I finally put some effort into solving this problem and came up with this library, which essentially provides for the creation of related models via AJAX POST request.
 
 It assumes some simplicity on the part of the related model – e.g. that only an `ImageField` is required to be populated – and uses [Dropzone.js](https://www.dropzone.dev/js/) to accept uploads and fire off POST requests to an endpoint which creates new child models using the related manager of the parent model.
 
-I decided not to try to support drag-and-drop uploads when *creating* parent model instances, since the uploads would need to be stashed somewhere temporarily then associated with the new model when it was saved. Instead this library operates only on existing model instances and requires the user to reload the page once they're done dropping files, so that Django's admin/inline UI can display the newly created child models for editing. This is acceptable in my use-cases but may not be in yours.
+I decided not to try to support drag-and-drop uploads when _creating_ parent model instances, since the uploads would need to be stashed somewhere temporarily then associated with the new model when it was saved. Instead this library operates only on existing model instances and requires the user to reload the page once they're done dropping files, so that Django's admin/inline UI can display the newly created child models for editing. This is acceptable in my use-cases but may not be in yours.
 
 ## Compatibility
 
 This library has been tested on Django 3.2 and 4.0 on Python 3.8, though I expect it to be fairly compatible with other versions. For now, the package is marked as requiring Python 3.6 or higher.
 
 **Please note that this library is an early beta release, mostly published so that I can share code between my own projects. It works well for my specific use-case but your mileage may vary. If you have issues with the library please open a ticket, but be aware it's not being developed intensively at this stage.**
 
@@ -59,14 +59,27 @@
 
 
 @admin.register(Album)
 class AlbumAdmin(DragAndDropRelatedImageMixin, admin.ModelAdmin):
     inlines = [ImageInline]
 ```
 
+## Usage in combination with [`django-solo`](https://github.com/lazybird/django-solo)
+
+The `django-solo` library provides its own admin `change_form` template with some minimal UI changes to assist with singleton models. When using `django-dragndrop-related` with a `django-solo` singleton model, there is a different mixin which will preserve the proper template inheritance:
+
+```python
+from dragndrop_related.views import DragAndDropSingletonRelatedImageMixin
+from solo.admin import SingletonModelAdmin
+
+@admin.register(models.Homepage)
+class HomepageAdmin(DragAndDropSingletonRelatedImageMixin, SingletonModelAdmin):
+    # ...
+```
+
 ## Configuration
 
 The library makes a few assumptions about your models and their relationship. Consider the following example models:
 
 ```python
 class Album(models.Model):
     # ...
```

### Comparing `django-dragndrop-related-0.1.0/django_dragndrop_related.egg-info/PKG-INFO` & `django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dragndrop-related
-Version: 0.1.0
+Version: 0.2.0
 Summary: Drag-and-drop multiple uploading of related images/files for
 Home-page: http://github.com/BigglesZX/django-dragndrop-related
 Author: James Tiplady
 Maintainer: James Tiplady
 License: MIT
 Keywords: django
 Platform: OS Independent
@@ -37,15 +37,15 @@
 
 ## Rationale
 
 One of the most common requests I get from clients when working on Django projects is to support some kind of drag-and-drop upload to save them the tedium of working with multiple file upload fields. I finally put some effort into solving this problem and came up with this library, which essentially provides for the creation of related models via AJAX POST request.
 
 It assumes some simplicity on the part of the related model – e.g. that only an `ImageField` is required to be populated – and uses [Dropzone.js](https://www.dropzone.dev/js/) to accept uploads and fire off POST requests to an endpoint which creates new child models using the related manager of the parent model.
 
-I decided not to try to support drag-and-drop uploads when *creating* parent model instances, since the uploads would need to be stashed somewhere temporarily then associated with the new model when it was saved. Instead this library operates only on existing model instances and requires the user to reload the page once they're done dropping files, so that Django's admin/inline UI can display the newly created child models for editing. This is acceptable in my use-cases but may not be in yours.
+I decided not to try to support drag-and-drop uploads when _creating_ parent model instances, since the uploads would need to be stashed somewhere temporarily then associated with the new model when it was saved. Instead this library operates only on existing model instances and requires the user to reload the page once they're done dropping files, so that Django's admin/inline UI can display the newly created child models for editing. This is acceptable in my use-cases but may not be in yours.
 
 ## Compatibility
 
 This library has been tested on Django 3.2 and 4.0 on Python 3.8, though I expect it to be fairly compatible with other versions. For now, the package is marked as requiring Python 3.6 or higher.
 
 **Please note that this library is an early beta release, mostly published so that I can share code between my own projects. It works well for my specific use-case but your mileage may vary. If you have issues with the library please open a ticket, but be aware it's not being developed intensively at this stage.**
 
@@ -86,14 +86,27 @@
 
 
 @admin.register(Album)
 class AlbumAdmin(DragAndDropRelatedImageMixin, admin.ModelAdmin):
     inlines = [ImageInline]
 ```
 
+## Usage in combination with [`django-solo`](https://github.com/lazybird/django-solo)
+
+The `django-solo` library provides its own admin `change_form` template with some minimal UI changes to assist with singleton models. When using `django-dragndrop-related` with a `django-solo` singleton model, there is a different mixin which will preserve the proper template inheritance:
+
+```python
+from dragndrop_related.views import DragAndDropSingletonRelatedImageMixin
+from solo.admin import SingletonModelAdmin
+
+@admin.register(models.Homepage)
+class HomepageAdmin(DragAndDropSingletonRelatedImageMixin, SingletonModelAdmin):
+    # ...
+```
+
 ## Configuration
 
 The library makes a few assumptions about your models and their relationship. Consider the following example models:
 
 ```python
 class Album(models.Model):
     # ...
```

### Comparing `django-dragndrop-related-0.1.0/django_dragndrop_related.egg-info/SOURCES.txt` & `django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 django_dragndrop_related.egg-info/SOURCES.txt
 django_dragndrop_related.egg-info/dependency_links.txt
 django_dragndrop_related.egg-info/not-zip-safe
 django_dragndrop_related.egg-info/requires.txt
 django_dragndrop_related.egg-info/top_level.txt
 dragndrop_related/__init__.py
 dragndrop_related/views.py
-dragndrop_related/templates/change_form.html
+dragndrop_related/templates/admin/dragndrop_related/change_form.html
 example_project/__init__.py
 example_project/asgi.py
 example_project/manage.py
 example_project/settings.py
 example_project/urls.py
 example_project/wsgi.py
 example_project/gallery/__init__.py
```

### Comparing `django-dragndrop-related-0.1.0/dragndrop_related/templates/change_form.html` & `django-dragndrop-related-0.2.0/dragndrop_related/templates/admin/dragndrop_related/change_form.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'admin/change_form.html' %}
+{% extends change_form_template_parent %}
 {% load admin_urls %}
 
 {% block extrahead %}
     {{ block.super}}
     <script src="https://unpkg.com/dropzone@5/dist/min/dropzone.min.js"></script>
     <script>
         Dropzone.autoDiscover = false;
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% extends 'admin/change_form.html' %} {% load admin_urls %} {% block extrahead
-%} {{ block.super}}
+{% extends change_form_template_parent %} {% load admin_urls %} {% block
+extrahead %} {{ block.super}}
  {% endblock %} {% block extrastyle %} {{ block.super }}
  {% endblock %} {% block after_related_objects %} {{ block.super }}
 ***** Drag-and-drop upload for {{ related_model_name_plural }} *****
 {% if add %} [Save] the {{ opts.verbose_name }} to enable drag-and-drop {
 { related_model_name }} uploading here. {% else %}
     * Your {{ related_model_name }} was uploaded successfully. When you're
       finished uploading, reload the page or [save and continue editing] to see
```

### Comparing `django-dragndrop-related-0.1.0/dragndrop_related/views.py` & `django-dragndrop-related-0.2.0/dragndrop_related/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,15 +101,20 @@
     ''' Define some helpful properties and methods to add our drag-and-drop UI
         to the `change` template of the associated model. Add a bunch of
         helpful info to the context of `add` or `change` views and define a
         custom route for receiving POSTed uploads.
     '''
 
     ''' Path to the custom admin `change_form` template '''
-    change_form_template = 'change_form.html'
+    change_form_template = 'admin/dragndrop_related/change_form.html'
+
+    ''' Path to template from which the custom admin `change_form` template
+        should inherit
+    '''
+    change_form_template_parent = 'admin/change_form.html'
 
     ''' Name of the reverse relation on the associated model to which images
         will be added
     '''
     related_manager_field_name = 'images'
 
     ''' Name of the field on the *related* model where images will be saved '''
@@ -139,14 +144,16 @@
                 related_model._meta.verbose_name_plural,
             'related_manager_field_name':
                 self.related_manager_field_name,
             'related_model_field_name':
                 self.related_model_field_name,
             'related_model_order_field_name':
                 self.related_model_order_field_name,
+            'change_form_template_parent':
+                self.change_form_template_parent,
         }
 
     def add_view(self, request, form_url='', extra_context=None):
         ''' Add our helpful related model info to the `add` view context '''
 
         extra_context = extra_context or {}
         extra_context = {**extra_context, **self.get_related_model_info()}
@@ -171,7 +178,20 @@
         return [
             re_path(r'^(?P<pk>\d+)/drag-and-drop/$',
                     self.admin_site.admin_view(DragAndDropView.as_view(
                         model=self.model)),
                     self.get_related_model_info(),
                     name='{0}_{1}_drag_and_drop'.format(*info)),
         ] + super().get_urls()
+
+
+class DragAndDropSingletonRelatedImageMixin(DragAndDropRelatedImageMixin):
+    ''' A variation of the mixin designed for use with singleton models
+        provided by `django-solo`. Ensures our `change_form` template inherits
+        from django-solo's, to preserve the minor differences in the singleton
+        UI.
+    '''
+
+    ''' Path to template that the custom admin `change_form` template should
+        inherit from
+    '''
+    change_form_template_parent = 'admin/solo/change_form.html'
```

### Comparing `django-dragndrop-related-0.1.0/example_project/gallery/migrations/0001_initial.py` & `django-dragndrop-related-0.2.0/example_project/gallery/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dragndrop-related-0.1.0/example_project/manage.py` & `django-dragndrop-related-0.2.0/example_project/manage.py`

 * *Files identical despite different names*

### Comparing `django-dragndrop-related-0.1.0/example_project/settings.py` & `django-dragndrop-related-0.2.0/example_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-dragndrop-related-0.1.0/example_project/urls.py` & `django-dragndrop-related-0.2.0/example_project/urls.py`

 * *Files identical despite different names*

### Comparing `django-dragndrop-related-0.1.0/setup.py` & `django-dragndrop-related-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 
 ''' To make a new release:
     1. Bump version number in setup.py
     2. Update CHANGELOG
     3. $ git commit ...
-    4. $ git tag -a x.x.x  # see `git tags` for latest
+    4. $ git tag -a x.x.x  # see `git tag` for latest
     5. $ git push origin main
     6. $ git push --tags
     7. $ python setup.py register sdist
     8. $ twine upload dist/*
 '''
 
 from setuptools import setup, find_packages  # noqa: E402
 
 
-VERSION = '.'.join(('0', '1', '0'))
+VERSION = '.'.join(('0', '2', '0'))
 
 DESCRIPTION = '''Drag-and-drop multiple uploading of related images/files for
               Django admin, using Dropzone.js'''
 
 CLASSIFIERS = [
     'Development Status :: 4 - Beta',
     'Environment :: Web Environment',
```

