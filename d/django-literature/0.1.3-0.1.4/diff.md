# Comparing `tmp/django_literature-0.1.3.tar.gz` & `tmp/django_literature-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_literature-0.1.3.tar", max compression
+gzip compressed data, was "django_literature-0.1.4.tar", max compression
```

## Comparing `django_literature-0.1.3.tar` & `django_literature-0.1.4.tar`

### file list

```diff
@@ -1,54 +1,57 @@
--rw-r--r--   0        0        0     1089 2023-05-04 11:45:36.141295 django_literature-0.1.3/LICENSE
--rw-r--r--   0        0        0     2343 2023-05-04 11:45:36.141295 django_literature-0.1.3/README.md
--rw-r--r--   0        0        0       22 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/__init__.py
--rw-r--r--   0        0        0     6237 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/admin.py
--rw-r--r--   0        0        0        0 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/api/__init__.py
--rw-r--r--   0        0        0      398 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/api/serialize.py
--rw-r--r--   0        0        0      249 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/api/urls.py
--rw-r--r--   0        0        0      370 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/api/views.py
--rw-r--r--   0        0        0      250 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/apps.py
--rw-r--r--   0        0        0     2514 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/choices.py
--rw-r--r--   0        0        0      724 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/conf.py
--rw-r--r--   0        0        0    36128 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/csl_map.py
--rw-r--r--   0        0        0      985 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/drf.py
--rw-r--r--   0        0        0      761 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/fields.py
--rw-r--r--   0        0        0     4965 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/forms.py
--rw-r--r--   0        0        0     2576 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/formset.py
--rw-r--r--   0        0        0     1932 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/managers.py
--rw-r--r--   0        0        0    13989 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/migrations/0001_initial.py
--rw-r--r--   0        0        0      655 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/migrations/0002_alter_literature_published.py
--rw-r--r--   0        0        0      478 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/migrations/0003_literature_csl.py
--rw-r--r--   0        0        0     2871 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/migrations/0004_remove_literature_doi_remove_literature_isbn_and_more.py
--rw-r--r--   0        0        0      577 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/migrations/0005_remove_literature_pid_remove_literature_pid_type_and_more.py
--rw-r--r--   0        0        0        0 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/migrations/__init__.py
--rw-r--r--   0        0        0     8578 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/models.py
--rw-r--r--   0        0        0     4667 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/static/literature/icons/icons.svg
--rw-r--r--   0        0        0     1513 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/static/literature/icons/three-dots.svg
--rw-r--r--   0        0        0     3106 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/static/literature/js/admin/change_list.js
--rw-r--r--   0        0        0     3111 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/static/literature/js/datatablesHyperlink.js
--rw-r--r--   0        0        0     1715 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/static/literature/js/main copy.js
--rw-r--r--   0        0        0     2012 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/static/literature/js/main.js
--rw-r--r--   0        0        0     6071 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/base.html
--rw-r--r--   0        0        0     2370 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/admin/change_list.html
--rw-r--r--   0        0        0     2085 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/admin/search.html
--rw-r--r--   0        0        0      615 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/author_detail.html
--rw-r--r--   0        0        0     1349 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/author_list.html
--rw-r--r--   0        0        0       73 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/bibliography.html
--rw-r--r--   0        0        0      665 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/citation/bootstrap.html
--rw-r--r--   0        0        0      465 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/citation/plain_text.html
--rw-r--r--   0        0        0      332 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/literature_detail.html
--rw-r--r--   0        0        0     1591 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/literature_form.html
--rw-r--r--   0        0        0      788 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/literature_form1.html
--rw-r--r--   0        0        0      186 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/literature_list.html
--rw-r--r--   0        0        0      301 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/widgets/identifier.html
--rw-r--r--   0        0        0     1128 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/widgets/pdf_viewer.html
--rw-r--r--   0        0        0     1120 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/widgets/postgres_array_widget.html
--rw-r--r--   0        0        0      348 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templates/literature/widgets/preview.html
--rw-r--r--   0        0        0        0 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templatetags/__init__.py
--rw-r--r--   0        0        0      568 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/templatetags/literature.py
--rw-r--r--   0        0        0      429 2023-05-04 11:45:36.145295 django_literature-0.1.3/literature/urls.py
--rw-r--r--   0        0        0     1241 2023-05-04 11:45:36.149295 django_literature-0.1.3/literature/utils.py
--rw-r--r--   0        0        0     3040 2023-05-04 11:45:36.149295 django_literature-0.1.3/literature/views.py
--rw-r--r--   0        0        0      828 2023-05-04 11:45:36.149295 django_literature-0.1.3/literature/widgets.py
--rw-r--r--   0        0        0     3947 2023-05-04 11:46:06.313609 django_literature-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 django_literature-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-05 10:01:57.641494 django_literature-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2343 2023-05-05 10:01:57.641494 django_literature-0.1.4/README.md
+-rw-r--r--   0        0        0       22 2023-05-05 10:01:57.641494 django_literature-0.1.4/literature/__init__.py
+-rw-r--r--   0        0        0     6237 2023-05-05 10:01:57.641494 django_literature-0.1.4/literature/admin.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:01:57.641494 django_literature-0.1.4/literature/api/__init__.py
+-rw-r--r--   0        0        0      398 2023-05-05 10:01:57.641494 django_literature-0.1.4/literature/api/serialize.py
+-rw-r--r--   0        0        0      249 2023-05-05 10:01:57.641494 django_literature-0.1.4/literature/api/urls.py
+-rw-r--r--   0        0        0      370 2023-05-05 10:01:57.641494 django_literature-0.1.4/literature/api/views.py
+-rw-r--r--   0        0        0      250 2023-05-05 10:01:57.641494 django_literature-0.1.4/literature/apps.py
+-rw-r--r--   0        0        0     2514 2023-05-05 10:01:57.641494 django_literature-0.1.4/literature/choices.py
+-rw-r--r--   0        0        0      724 2023-05-05 10:01:57.641494 django_literature-0.1.4/literature/conf.py
+-rw-r--r--   0        0        0    36128 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/csl_map.py
+-rw-r--r--   0        0        0      985 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/drf.py
+-rw-r--r--   0        0        0      761 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/fields.py
+-rw-r--r--   0        0        0     4965 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/forms.py
+-rw-r--r--   0        0        0     2576 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/formset.py
+-rw-r--r--   0        0        0     1932 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/managers.py
+-rw-r--r--   0        0        0    13989 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/migrations/0001_initial.py
+-rw-r--r--   0        0        0      655 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/migrations/0002_alter_literature_published.py
+-rw-r--r--   0        0        0      478 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/migrations/0003_literature_csl.py
+-rw-r--r--   0        0        0     2871 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/migrations/0004_remove_literature_doi_remove_literature_isbn_and_more.py
+-rw-r--r--   0        0        0      577 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/migrations/0005_remove_literature_pid_remove_literature_pid_type_and_more.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/migrations/__init__.py
+-rw-r--r--   0        0        0     8578 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/models.py
+-rw-r--r--   0        0        0     4667 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/static/literature/icons/icons.svg
+-rw-r--r--   0        0        0     1513 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/static/literature/icons/three-dots.svg
+-rw-r--r--   0        0        0     3106 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/static/literature/js/admin/change_list.js
+-rw-r--r--   0        0        0     3111 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/static/literature/js/datatablesHyperlink.js
+-rw-r--r--   0        0        0     1715 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/static/literature/js/main copy.js
+-rw-r--r--   0        0        0     2012 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/static/literature/js/main.js
+-rw-r--r--   0        0        0    74730 2023-05-05 10:01:57.645494 django_literature-0.1.4/literature/static/vendor/DataTables/datatables.min.css
+-rw-r--r--   0        0        0  2452970 2023-05-05 10:01:57.661494 django_literature-0.1.4/literature/static/vendor/DataTables/datatables.min.js
+-rw-r--r--   0        0        0  2274000 2023-05-05 10:01:57.669494 django_literature-0.1.4/literature/static/vendor/js/citation.js
+-rw-r--r--   0        0        0     6071 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/base.html
+-rw-r--r--   0        0        0     2370 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/admin/change_list.html
+-rw-r--r--   0        0        0     2085 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/admin/search.html
+-rw-r--r--   0        0        0      615 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/author_detail.html
+-rw-r--r--   0        0        0     1349 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/author_list.html
+-rw-r--r--   0        0        0       73 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/bibliography.html
+-rw-r--r--   0        0        0      665 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/citation/bootstrap.html
+-rw-r--r--   0        0        0      465 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/citation/plain_text.html
+-rw-r--r--   0        0        0      332 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/literature_detail.html
+-rw-r--r--   0        0        0     1591 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/literature_form.html
+-rw-r--r--   0        0        0      788 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/literature_form1.html
+-rw-r--r--   0        0        0      186 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/literature_list.html
+-rw-r--r--   0        0        0      301 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/widgets/identifier.html
+-rw-r--r--   0        0        0     1128 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/widgets/pdf_viewer.html
+-rw-r--r--   0        0        0     1120 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/widgets/postgres_array_widget.html
+-rw-r--r--   0        0        0      348 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templates/literature/widgets/preview.html
+-rw-r--r--   0        0        0        0 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templatetags/__init__.py
+-rw-r--r--   0        0        0      568 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/templatetags/literature.py
+-rw-r--r--   0        0        0      429 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/urls.py
+-rw-r--r--   0        0        0     1241 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/utils.py
+-rw-r--r--   0        0        0     3040 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/views.py
+-rw-r--r--   0        0        0      828 2023-05-05 10:01:57.673494 django_literature-0.1.4/literature/widgets.py
+-rw-r--r--   0        0        0     3948 2023-05-05 10:02:18.593469 django_literature-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 django_literature-0.1.4/PKG-INFO
```

### Comparing `django_literature-0.1.3/LICENSE` & `django_literature-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/README.md` & `django_literature-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/admin.py` & `django_literature-0.1.4/literature/admin.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/choices.py` & `django_literature-0.1.4/literature/choices.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/conf.py` & `django_literature-0.1.4/literature/conf.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/csl_map.py` & `django_literature-0.1.4/literature/csl_map.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/drf.py` & `django_literature-0.1.4/literature/drf.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/fields.py` & `django_literature-0.1.4/literature/fields.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/forms.py` & `django_literature-0.1.4/literature/forms.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/formset.py` & `django_literature-0.1.4/literature/formset.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/managers.py` & `django_literature-0.1.4/literature/managers.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/migrations/0001_initial.py` & `django_literature-0.1.4/literature/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/migrations/0002_alter_literature_published.py` & `django_literature-0.1.4/literature/migrations/0002_alter_literature_published.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/migrations/0004_remove_literature_doi_remove_literature_isbn_and_more.py` & `django_literature-0.1.4/literature/migrations/0004_remove_literature_doi_remove_literature_isbn_and_more.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/migrations/0005_remove_literature_pid_remove_literature_pid_type_and_more.py` & `django_literature-0.1.4/literature/migrations/0005_remove_literature_pid_remove_literature_pid_type_and_more.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/models.py` & `django_literature-0.1.4/literature/models.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/static/literature/icons/icons.svg` & `django_literature-0.1.4/literature/static/literature/icons/icons.svg`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/static/literature/icons/three-dots.svg` & `django_literature-0.1.4/literature/static/literature/icons/three-dots.svg`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/static/literature/js/admin/change_list.js` & `django_literature-0.1.4/literature/static/literature/js/admin/change_list.js`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/static/literature/js/datatablesHyperlink.js` & `django_literature-0.1.4/literature/static/literature/js/datatablesHyperlink.js`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/static/literature/js/main copy.js` & `django_literature-0.1.4/literature/static/literature/js/main copy.js`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/static/literature/js/main.js` & `django_literature-0.1.4/literature/static/literature/js/main.js`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/templates/base.html` & `django_literature-0.1.4/literature/templates/base.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/templates/literature/admin/change_list.html` & `django_literature-0.1.4/literature/templates/literature/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/templates/literature/admin/search.html` & `django_literature-0.1.4/literature/templates/literature/admin/search.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/templates/literature/author_detail.html` & `django_literature-0.1.4/literature/templates/literature/author_detail.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/templates/literature/author_list.html` & `django_literature-0.1.4/literature/templates/literature/author_list.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/templates/literature/citation/bootstrap.html` & `django_literature-0.1.4/literature/templates/literature/citation/bootstrap.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/templates/literature/literature_form.html` & `django_literature-0.1.4/literature/templates/literature/literature_form.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/templates/literature/literature_form1.html` & `django_literature-0.1.4/literature/templates/literature/literature_form1.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/templates/literature/widgets/pdf_viewer.html` & `django_literature-0.1.4/literature/templates/literature/widgets/pdf_viewer.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/templates/literature/widgets/postgres_array_widget.html` & `django_literature-0.1.4/literature/templates/literature/widgets/postgres_array_widget.html`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/templatetags/literature.py` & `django_literature-0.1.4/literature/templatetags/literature.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/utils.py` & `django_literature-0.1.4/literature/utils.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/views.py` & `django_literature-0.1.4/literature/views.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/literature/widgets.py` & `django_literature-0.1.4/literature/widgets.py`

 * *Files identical despite different names*

### Comparing `django_literature-0.1.3/pyproject.toml` & `django_literature-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-literature"
-version = "0.1.3"
+version = "v0.1.4"
 description = "A scientific literature management tool for Django"
 authors = ["Sam Jennings <samuel.scott.jennings@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "literature"}]
 homepage = "https://github.com/SSJenny90/django-literature"
 keywords = ["django", "literature", "publications", "scientific", "research"]
```

### Comparing `django_literature-0.1.3/PKG-INFO` & `django_literature-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-literature
-Version: 0.1.3
+Version: 0.1.4
 Summary: A scientific literature management tool for Django
 Home-page: https://github.com/SSJenny90/django-literature
 License: MIT
 Keywords: django,literature,publications,scientific,research
 Author: Sam Jennings
 Author-email: samuel.scott.jennings@gmail.com
 Requires-Python: >=3.8,<4.0
```

