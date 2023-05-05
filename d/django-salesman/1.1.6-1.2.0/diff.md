# Comparing `tmp/django-salesman-1.1.6.tar.gz` & `tmp/django_salesman-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-salesman-1.1.6.tar", max compression
+gzip compressed data, was "django_salesman-1.2.0.tar", max compression
```

## Comparing `django-salesman-1.1.6.tar` & `django_salesman-1.2.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
--rw-r--r--   0        0        0     1520 2023-02-06 13:42:33.152724 django-salesman-1.1.6/LICENSE
--rw-r--r--   0        0        0     2150 2023-02-06 13:42:33.152724 django-salesman-1.1.6/README.md
--rw-r--r--   0        0        0     2623 2023-02-06 13:42:33.156724 django-salesman-1.1.6/pyproject.toml
--rw-r--r--   0        0        0       91 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/__init__.py
--rw-r--r--   0        0        0       60 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/__init__.py
--rw-r--r--   0        0        0     4721 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/admin.py
--rw-r--r--   0        0        0      221 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/apps.py
--rw-r--r--   0        0        0     1604 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/filters.py
--rw-r--r--   0        0        0     1352 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/forms.py
--rw-r--r--   0        0        0     7685 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/mixins.py
--rw-r--r--   0        0        0      348 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/static/salesman/admin/wagtail_form.css
--rw-r--r--   0        0        0      404 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/templates/salesman/admin/change_form.html
--rw-r--r--   0        0        0     1316 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/templates/salesman/admin/includes/refund_content.html
--rw-r--r--   0        0        0      986 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/templates/salesman/admin/includes/refund_js.html
--rw-r--r--   0        0        0      801 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/templates/salesman/admin/refund.html
--rw-r--r--   0        0        0      839 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/templates/salesman/admin/wagtail_edit.html
--rw-r--r--   0        0        0      363 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/templates/salesman/admin/wagtail_refund.html
--rw-r--r--   0        0        0     1745 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/utils.py
--rw-r--r--   0        0        0        0 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/wagtail/__init__.py
--rw-r--r--   0        0        0       30 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/wagtail/edit_handlers.py
--rw-r--r--   0        0        0      169 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/wagtail/forms.py
--rw-r--r--   0        0        0      785 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/wagtail/helpers.py
--rw-r--r--   0        0        0     4985 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/wagtail/mixins.py
--rw-r--r--   0        0        0    12474 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/wagtail/panels.py
--rw-r--r--   0        0        0     2668 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/wagtail/views.py
--rw-r--r--   0        0        0     3262 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/wagtail_hooks.py
--rw-r--r--   0        0        0     1529 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/admin/widgets.py
--rw-r--r--   0        0        0       62 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/basket/__init__.py
--rw-r--r--   0        0        0     1438 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/basket/apps.py
--rw-r--r--   0        0        0     4127 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/basket/migrations/0001_initial.py
--rw-r--r--   0        0        0      603 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/basket/migrations/0002_alter_json_fields.py
--rw-r--r--   0        0        0      366 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/basket/migrations/0003_rename_owner_field.py
--rw-r--r--   0        0        0        0 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/basket/migrations/__init__.py
--rw-r--r--   0        0        0    11633 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/basket/models.py
--rw-r--r--   0        0        0     3983 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/basket/modifiers.py
--rw-r--r--   0        0        0     7784 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/basket/serializers.py
--rw-r--r--   0        0        0     1170 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/basket/utils.py
--rw-r--r--   0        0        0     4644 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/basket/views.py
--rw-r--r--   0        0        0       66 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/checkout/__init__.py
--rw-r--r--   0        0        0      233 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/checkout/apps.py
--rw-r--r--   0        0        0     6914 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/checkout/payment.py
--rw-r--r--   0        0        0     4626 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/checkout/serializers.py
--rw-r--r--   0        0        0      721 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/checkout/utils.py
--rw-r--r--   0        0        0     2179 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/checkout/views.py
--rw-r--r--   0        0        0    12870 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/conf.py
--rw-r--r--   0        0        0       58 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/core/__init__.py
--rw-r--r--   0        0        0      217 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/core/apps.py
--rw-r--r--   0        0        0      341 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/core/serializers.py
--rw-r--r--   0        0        0      604 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/core/typing.py
--rw-r--r--   0        0        0     1212 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/core/utils.py
--rw-r--r--   0        0        0       62 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/orders/__init__.py
--rw-r--r--   0        0        0      218 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/orders/apps.py
--rw-r--r--   0        0        0    10494 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/orders/migrations/0001_initial.py
--rw-r--r--   0        0        0      536 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/orders/migrations/0002_alter_order_ref.py
--rw-r--r--   0        0        0      843 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/orders/migrations/0003_alter_json_fields.py
--rw-r--r--   0        0        0        0 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/orders/migrations/__init__.py
--rw-r--r--   0        0        0    16621 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/orders/models.py
--rw-r--r--   0        0        0     8083 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/orders/serializers.py
--rw-r--r--   0        0        0       66 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/orders/signals.py
--rw-r--r--   0        0        0     3405 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/orders/status.py
--rw-r--r--   0        0        0      794 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/orders/utils.py
--rw-r--r--   0        0        0     6042 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/orders/views.py
--rw-r--r--   0        0        0      554 2023-02-06 13:42:33.156724 django-salesman-1.1.6/salesman/urls.py
--rw-r--r--   0        0        0     3803 2023-02-06 13:43:49.391415 django-salesman-1.1.6/setup.py
--rw-r--r--   0        0        0     4165 2023-02-06 13:43:49.391918 django-salesman-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1520 2023-05-05 13:56:27.987393 django_salesman-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2150 2023-05-05 13:56:27.987393 django_salesman-1.2.0/README.md
+-rw-r--r--   0        0        0     2600 2023-05-05 13:56:27.987393 django_salesman-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-05-05 13:56:27.987393 django_salesman-1.2.0/salesman/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-05 13:56:27.987393 django_salesman-1.2.0/salesman/admin/__init__.py
+-rw-r--r--   0        0        0     4721 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/admin.py
+-rw-r--r--   0        0        0      221 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/apps.py
+-rw-r--r--   0        0        0     1604 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/filters.py
+-rw-r--r--   0        0        0     1352 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/forms.py
+-rw-r--r--   0        0        0     7685 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/mixins.py
+-rw-r--r--   0        0        0      348 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/static/salesman/admin/wagtail_form.css
+-rw-r--r--   0        0        0      404 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/templates/salesman/admin/change_form.html
+-rw-r--r--   0        0        0     1316 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/templates/salesman/admin/includes/refund_content.html
+-rw-r--r--   0        0        0      986 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/templates/salesman/admin/includes/refund_js.html
+-rw-r--r--   0        0        0      801 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/templates/salesman/admin/refund.html
+-rw-r--r--   0        0        0      839 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/templates/salesman/admin/wagtail_edit.html
+-rw-r--r--   0        0        0      363 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/templates/salesman/admin/wagtail_refund.html
+-rw-r--r--   0        0        0     1745 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/utils.py
+-rw-r--r--   0        0        0        0 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/wagtail/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/wagtail/forms.py
+-rw-r--r--   0        0        0      785 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/wagtail/helpers.py
+-rw-r--r--   0        0        0     4978 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/wagtail/mixins.py
+-rw-r--r--   0        0        0    11948 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/wagtail/panels.py
+-rw-r--r--   0        0        0     2648 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/wagtail/views.py
+-rw-r--r--   0        0        0     3196 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/wagtail_hooks.py
+-rw-r--r--   0        0        0     1529 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/admin/widgets.py
+-rw-r--r--   0        0        0       62 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/basket/__init__.py
+-rw-r--r--   0        0        0     1438 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/basket/apps.py
+-rw-r--r--   0        0        0     4127 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/basket/migrations/0001_initial.py
+-rw-r--r--   0        0        0      603 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/basket/migrations/0002_alter_json_fields.py
+-rw-r--r--   0        0        0      366 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/basket/migrations/0003_rename_owner_field.py
+-rw-r--r--   0        0        0        0 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/basket/migrations/__init__.py
+-rw-r--r--   0        0        0    11633 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/basket/models.py
+-rw-r--r--   0        0        0     3983 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/basket/modifiers.py
+-rw-r--r--   0        0        0     7784 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/basket/serializers.py
+-rw-r--r--   0        0        0     1170 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/basket/utils.py
+-rw-r--r--   0        0        0     4673 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/basket/views.py
+-rw-r--r--   0        0        0       66 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/checkout/__init__.py
+-rw-r--r--   0        0        0      233 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/checkout/apps.py
+-rw-r--r--   0        0        0     6914 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/checkout/payment.py
+-rw-r--r--   0        0        0     4606 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/checkout/serializers.py
+-rw-r--r--   0        0        0      721 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/checkout/utils.py
+-rw-r--r--   0        0        0     2663 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/checkout/views.py
+-rw-r--r--   0        0        0    13157 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/conf.py
+-rw-r--r--   0        0        0       58 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/core/__init__.py
+-rw-r--r--   0        0        0      217 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/core/apps.py
+-rw-r--r--   0        0        0      341 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/core/serializers.py
+-rw-r--r--   0        0        0      604 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/core/typing.py
+-rw-r--r--   0        0        0     1212 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/core/utils.py
+-rw-r--r--   0        0        0       62 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/orders/__init__.py
+-rw-r--r--   0        0        0      218 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/orders/apps.py
+-rw-r--r--   0        0        0    10494 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/orders/migrations/0001_initial.py
+-rw-r--r--   0        0        0      536 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/orders/migrations/0002_alter_order_ref.py
+-rw-r--r--   0        0        0      843 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/orders/migrations/0003_alter_json_fields.py
+-rw-r--r--   0        0        0        0 2023-05-05 13:56:27.991393 django_salesman-1.2.0/salesman/orders/migrations/__init__.py
+-rw-r--r--   0        0        0    16621 2023-05-05 13:56:27.995393 django_salesman-1.2.0/salesman/orders/models.py
+-rw-r--r--   0        0        0     8063 2023-05-05 13:56:27.995393 django_salesman-1.2.0/salesman/orders/serializers.py
+-rw-r--r--   0        0        0       66 2023-05-05 13:56:27.995393 django_salesman-1.2.0/salesman/orders/signals.py
+-rw-r--r--   0        0        0     3405 2023-05-05 13:56:27.995393 django_salesman-1.2.0/salesman/orders/status.py
+-rw-r--r--   0        0        0      794 2023-05-05 13:56:27.995393 django_salesman-1.2.0/salesman/orders/utils.py
+-rw-r--r--   0        0        0     6222 2023-05-05 13:56:27.995393 django_salesman-1.2.0/salesman/orders/views.py
+-rw-r--r--   0        0        0        0 2023-05-05 13:56:27.995393 django_salesman-1.2.0/salesman/py.typed
+-rw-r--r--   0        0        0      554 2023-05-05 13:56:27.995393 django_salesman-1.2.0/salesman/urls.py
+-rw-r--r--   0        0        0     4151 1970-01-01 00:00:00.000000 django_salesman-1.2.0/PKG-INFO
```

### Comparing `django-salesman-1.1.6/LICENSE` & `django_salesman-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/README.md` & `django_salesman-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/pyproject.toml` & `django_salesman-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 [tool.poetry]
 name = "django-salesman"
-version = "1.1.6"
+version = "1.2.0"
 description = "Headless e-commerce framework for Django and Wagtail."
 authors = ["Dino Perovic <dino.perovic@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://pypi.org/project/django-salesman/"
 repository = "https://github.com/dinoperovic/django-salesman"
 documentation = "https://django-salesman.readthedocs.io"
 keywords = ["e-commerce", "headless", "rest-api", "shop", "framework"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Django",
-    "Framework :: Django :: 3.1",
-    "Framework :: Django :: 3.2",
-    "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Framework :: Wagtail",
-    "Framework :: Wagtail :: 2",
-    "Framework :: Wagtail :: 3",
     "Framework :: Wagtail :: 4",
+    "Framework :: Wagtail :: 5",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Internet",
 ]
 packages = [
     {include = "salesman"},
 ]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-django = ">=3.1,<4.2"
-djangorestframework = ">=3.11,<3.15"
+django = ">=4.1.3,<4.3"
+djangorestframework = ">=3.11.1,<4.0"
 
 # Optional
 Pygments = {version = "^2.6", optional = true}
-wagtail = {version = ">=2.9,<4.2", optional = true}
+wagtail = {version = ">=4.0,<6.0", optional = true}
 pytest = {version = "~7.0.0", optional = true}
 pytest-django = {version = "~4.5.0", optional = true}
 pytest-cov = {version = "~3.0.0", optional = true}
 sphinx = {version = "~4.4.0", optional = true}
 sphinx-rtd-theme = {version = "~1.0.0", optional = true}
 sphinx-autobuild = {version = "~2021.3.0", optional = true}
 sphinxcontrib-httpdomain = {version = "~1.8.0", optional = true}
@@ -77,10 +75,13 @@
 no_implicit_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = false
 no_implicit_reexport = true
 strict_equality = true
 
+[tool.pyright]
+typeCheckingMode = "off"
+
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `django-salesman-1.1.6/salesman/admin/admin.py` & `django_salesman-1.2.0/salesman/admin/admin.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/admin/filters.py` & `django_salesman-1.2.0/salesman/admin/filters.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/admin/forms.py` & `django_salesman-1.2.0/salesman/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/admin/mixins.py` & `django_salesman-1.2.0/salesman/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/admin/templates/salesman/admin/includes/refund_content.html` & `django_salesman-1.2.0/salesman/admin/templates/salesman/admin/includes/refund_content.html`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/admin/templates/salesman/admin/includes/refund_js.html` & `django_salesman-1.2.0/salesman/admin/templates/salesman/admin/includes/refund_js.html`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/admin/templates/salesman/admin/refund.html` & `django_salesman-1.2.0/salesman/admin/templates/salesman/admin/refund.html`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/admin/templates/salesman/admin/wagtail_edit.html` & `django_salesman-1.2.0/salesman/admin/templates/salesman/admin/wagtail_edit.html`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/admin/utils.py` & `django_salesman-1.2.0/salesman/admin/utils.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/admin/wagtail/helpers.py` & `django_salesman-1.2.0/salesman/admin/wagtail/helpers.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/admin/wagtail/mixins.py` & `django_salesman-1.2.0/salesman/admin/wagtail/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from django import forms
 from django.http import HttpRequest
 from django.urls import re_path, reverse
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
-from wagtail.admin.edit_handlers import (
+from wagtail.admin.panels import (
     FieldPanel,
     InlinePanel,
     MultiFieldPanel,
     ObjectList,
     TabbedInterface,
 )
```

### Comparing `django-salesman-1.1.6/salesman/admin/wagtail/panels.py` & `django_salesman-1.2.0/salesman/admin/wagtail/panels.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,20 @@
 
 from django.core.exceptions import FieldDoesNotExist
 from django.http import HttpRequest
 from django.utils.formats import date_format
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
-from wagtail.admin.edit_handlers import EditHandler as Panel
-from wagtail.utils.version import get_main_version as get_wagtail_version
+from wagtail.admin.panels import Panel
 
 from salesman.conf import app_settings
 
 from ..utils import format_price
 
-if get_wagtail_version() < "3.0.0":  # pragma: no cover
-    # Attach dummy BoundPanel class for older Wagtail versions
-    Panel.BoundPanel = object
-
 
 class ReadOnlyPanel(Panel):
     """
     Read only panel for Wagtail. You can pass in a ``formatter`` function
     to override value format and/or a ``renderer`` function to override how
     the value is rendered in html.
     """
@@ -55,43 +50,43 @@
             except AttributeError:
                 pass
         if heading and not self.heading:
             self.heading: str = heading
         if field and not self.help_text:
             self.help_text: str = getattr(field, "help_text", "")
 
-    def get_value(self) -> Any:  # pragma: no cover
+    def get_value(self) -> Any:
         value = getattr(self.instance, self.attr)
         if callable(value):
             value = value(self.instance)
         return value
 
-    def format_value(self, value: Any) -> Any:  # pragma: no cover
+    def format_value(self, value: Any) -> Any:
         if self.formatter and value is not None:
             value = self.formatter(value, self.instance, self.request)
         return value
 
-    def render(self) -> Any:  # pragma: no cover
+    def render(self) -> Any:
         value = self.get_value()
         return self.format_value(value)
 
-    def render_as_object(self) -> Any:  # pragma: no cover
+    def render_as_object(self) -> Any:
         if self.renderer:
             return self.renderer(self.get_value(), self.instance, self.request)
         return format_html(
             "<fieldset><legend>{}</legend>"
             '<ul class="fields"><li><div class="field">'
             '<div style="padding-top: 1.2em;">{}</div>'
             "</div></li></ul>"
             "</fieldset>",
             self.heading,
             self.render(),
         )
 
-    def render_as_field(self) -> Any:  # pragma: no cover
+    def render_as_field(self) -> Any:
         if self.renderer:
             return self.renderer(self.get_value(), self.instance, self.request)
         help_html = (
             format_html('<p class="help">{}</p>', self.help_text)
             if self.help_text
             else ""
         )
@@ -180,60 +175,60 @@
                 _(":"),
                 self.render(),
                 help_html,
             )
 
 
 class OrderDatePanel(ReadOnlyPanel):
-    def format_value(self, value: Any) -> Any:  # pragma: no cover
+    def format_value(self, value: Any) -> Any:
         if value:
             value = date_format(value, format="DATETIME_FORMAT")
         return value
 
     class BoundPanel(ReadOnlyPanel.BoundPanel):
         def format_value(self, value: Any) -> Any:
             if value:
                 value = date_format(value, format="DATETIME_FORMAT")
             return value
 
 
 class OrderCheckboxPanel(ReadOnlyPanel):
-    def format_value(self, value: Any) -> str:  # pragma: no cover
+    def format_value(self, value: Any) -> str:
         icon, color = ("tick", "#157b57") if value else ("cross", "#cd3238")
         template = '<span class="icon icon-{}" style="color: {};"></span>'
         return format_html(template, icon, color)
 
     class BoundPanel(ReadOnlyPanel.BoundPanel):
         def format_value(self, value: Any) -> str:
             icon, color = ("tick", "#157b57") if value else ("cross", "#cd3238")
             template = '<span class="icon icon-{}" style="color: {};"></span>'
             return format_html(template, icon, color)
 
 
 class OrderItemsPanel(ReadOnlyPanel):
-    def classes(self) -> list[str]:  # pragma: no cover
+    def classes(self) -> list[str]:
         return ["salesman-order-items"]
 
-    def render_as_field(self) -> str:  # pragma: no cover
+    def render_as_field(self) -> str:
         return self.render()
 
-    def render_as_object(self) -> str:  # pragma: no cover
+    def render_as_object(self) -> str:
         return self.render()
 
     def format_json(
         self,
         value: dict[str, Any],
         obj: Any,
         request: HttpRequest,
-    ) -> str:  # pragma: no cover
+    ) -> str:
         return app_settings.SALESMAN_ADMIN_JSON_FORMATTER(
             value, context={"order_item": True}
         )
 
-    def render(self) -> str:  # pragma: no cover
+    def render(self) -> str:
         head = f"""<tr>
             <td>{_('Name')}</td>
             <td>{_('Code')}</td>
             <td>{_('Unit price')}</td>
             <td>{_('Quantity')}</td>
             <td>{_('Subtotal')}</td>
             <td>{_('Extra rows')}</td>
@@ -319,24 +314,24 @@
     """
     Retrieves value from model_admin which is bound to the form in `get_edit_handler`.
     """
 
     def on_model_bound(self) -> None:
         pass
 
-    def on_form_bound(self) -> None:  # pragma: no cover
+    def on_form_bound(self) -> None:
         if not hasattr(self.form, "model_admin"):
             raise AssertionError("OrderAdminPanel can only be used in OrderModelAdmin.")
 
         field = getattr(self.form.model_admin, self.attr)
         heading = getattr(field, "short_description", "")
         if heading and not self.heading:
             self.heading = heading
 
-    def get_value(self) -> Any:  # pragma: no cover
+    def get_value(self) -> Any:
         return getattr(self.form.model_admin, self.attr)(self.instance)
 
     class BoundPanel(ReadOnlyPanel.BoundPanel):
         def __init__(
             self,
             panel: Panel,
             **kwargs: Any,
```

### Comparing `django-salesman-1.1.6/salesman/admin/wagtail/views.py` & `django_salesman-1.2.0/salesman/admin/wagtail/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def get_meta_title(self) -> str:
         return _("Viewing Order")
 
     @cached_property
     def refund_url(self) -> str | None:
         try:
             return str(self.url_helper.get_action_url("refund", self.pk_quoted))
-        except NoReverseMatch:  # pragma: no cover
+        except NoReverseMatch:
             return None
 
 
 class OrderRefundView(DeleteView):
     """
     Wagtail admin view that handles Order refunds.
     """
```

### Comparing `django-salesman-1.1.6/salesman/admin/wagtail_hooks.py` & `django_salesman-1.2.0/salesman/admin/wagtail_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
-from typing import Any, Type
+from typing import Type
 
-from wagtail.admin.edit_handlers import EditHandler, ObjectList
+from wagtail.admin.panels import ObjectList, Panel
 from wagtail.contrib.modeladmin.options import ModelAdmin, modeladmin_register
 
 from salesman.conf import app_settings
 from salesman.core.utils import get_salesman_model
 
 from .filters import OrderIsPaidFilter, OrderStatusFilter
 from .wagtail.forms import WagtailOrderModelForm
@@ -57,15 +57,15 @@
         """
         return type(
             "WagtailOrderModelForm",
             (form_class or WagtailOrderModelForm,),
             {"model_admin": self},
         )
 
-    def get_edit_handler(self, *args: Any, **kwargs: Any) -> EditHandler:
+    def get_edit_handler(self) -> Panel:
         """
         Returns edit handler with custom base form class attached.
 
         Returns:
             EditHandler: Edit handler
         """
         if hasattr(self, "edit_handler"):
@@ -77,15 +77,15 @@
             edit_handler = self.model.edit_handler
         elif hasattr(self.model, "panels"):
             panels = self.model.panels
             edit_handler = ObjectList(panels)
         elif hasattr(self, "default_edit_handler") and self.default_edit_handler:
             edit_handler = self.default_edit_handler
         else:
-            edit_handler = super().get_edit_handler(*args, **kwargs)
+            edit_handler = super().get_edit_handler()
 
         edit_handler.base_form_class = self.get_base_form_class(
             form_class=getattr(edit_handler, "base_form_class", None)
         )
         return edit_handler
```

### Comparing `django-salesman-1.1.6/salesman/admin/widgets.py` & `django_salesman-1.2.0/salesman/admin/widgets.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/basket/apps.py` & `django_salesman-1.2.0/salesman/basket/apps.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/basket/migrations/0001_initial.py` & `django_salesman-1.2.0/salesman/basket/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/basket/migrations/0002_alter_json_fields.py` & `django_salesman-1.2.0/salesman/basket/migrations/0002_alter_json_fields.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/basket/models.py` & `django_salesman-1.2.0/salesman/basket/models.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/basket/modifiers.py` & `django_salesman-1.2.0/salesman/basket/modifiers.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/basket/serializers.py` & `django_salesman-1.2.0/salesman/basket/serializers.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/basket/utils.py` & `django_salesman-1.2.0/salesman/basket/utils.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/basket/views.py` & `django_salesman-1.2.0/salesman/basket/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,48 +106,48 @@
     def delete(self, request: Request, *args: Any, **kwargs: Any) -> Response:
         """
         Delete the basket.
         """
         self.get_basket().delete()
         return Response(status=status.HTTP_204_NO_CONTENT)
 
-    @action(detail=False, methods=["get"])
+    @action(["get"], False)
     def count(self, request: Request) -> Response:
         """
         Show basket item count.
         """
         return Response({"count": self.get_basket().count})
 
-    @action(detail=False, methods=["get"])
+    @action(["get"], False)
     def quantity(self, request: Request) -> Response:
         """
         Show basket total quantity.
         """
         return Response({"quantity": self.get_basket().quantity})
 
-    @action(detail=False, methods=["post"], serializer_class=BasketSerializer)
+    @action(["post"], False, serializer_class=BasketSerializer)
     def clear(self, request: Request) -> Response:
         """
         Clear all items from basket.
         """
         self.get_basket().clear()
         return self.list(request)
 
-    @action(
-        detail=False,
-        methods=["get", "put"],
-        serializer_class=BasketExtraSerializer,
-    )
+    @action(["get"], False, serializer_class=BasketExtraSerializer)
     def extra(self, request: Request) -> Response:
         """
-        Update basket extra data.
+        Show basket extra data.
         """
         basket = self.get_basket()
+        serializer = self.get_serializer(basket)
+        return Response(serializer.data)
 
-        if request.method == "GET":
-            serializer = self.get_serializer(basket)
-            return Response(serializer.data)
-
+    @extra.mapping.put
+    def extra_update(self, request: Request) -> Response:
+        """
+        Update basket extra data.
+        """
+        basket = self.get_basket()
         serializer = self.get_serializer(basket, data=request.data, partial=True)
         serializer.is_valid(raise_exception=True)
         serializer.save()
         return Response(serializer.data)
```

### Comparing `django-salesman-1.1.6/salesman/checkout/payment.py` & `django_salesman-1.2.0/salesman/checkout/payment.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/checkout/serializers.py` & `django_salesman-1.2.0/salesman/checkout/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     def validate_payment_method(self, value: str) -> PaymentMethod | None:
         basket, request = self.context["basket"], self.context["request"]
         payment = payment_methods_pool.get_payment(value)
         if payment:
             payment.validate_basket(basket, request)
             return payment
-        return None  # pragma: no cover
+        return None
 
     def validate_extra(self, value: dict[str, Any]) -> dict[str, Any]:
         # Update basket `extra` instead of replacing it, remove null values.
         extra = self.context["basket"].extra
         if value:
             extra.update(value)
             extra = {k: v for k, v in extra.items() if v is not None}
```

### Comparing `django-salesman-1.1.6/salesman/checkout/utils.py` & `django_salesman-1.2.0/salesman/checkout/utils.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/checkout/views.py` & `django_salesman-1.2.0/salesman/checkout/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 from typing import Any
 
 from django.http import HttpRequest
 from django.http.response import HttpResponseBase
 from django.utils.decorators import method_decorator
+from django.utils.translation import gettext_lazy as _
 from django.views.decorators.cache import never_cache
 from rest_framework import mixins, status, viewsets
+from rest_framework.exceptions import PermissionDenied
 from rest_framework.request import Request
 from rest_framework.response import Response
 
+from salesman.conf import app_settings
 from salesman.core.utils import get_salesman_model
 
 from .payment import PaymentError, payment_methods_pool
 from .serializers import CheckoutSerializer
 
 Basket = get_salesman_model("Basket")
 
@@ -36,14 +39,22 @@
 
     def get_serializer_context(self) -> dict[str, Any]:
         context = super().get_serializer_context()
         context["basket"], _ = Basket.objects.get_or_create_from_request(self.request)
         context["basket"].update(self.request)
         return context
 
+    def check_permissions(self, request: Request) -> None:
+        super().check_permissions(request)
+
+        if not app_settings.SALESMAN_ALLOW_ANONYMOUS_USER_CHECKOUT and not bool(
+            request.user and request.user.is_authenticated
+        ):
+            raise PermissionDenied(detail=_("Anonymous checkout not allowed."))
+
     @method_decorator(never_cache)
     def dispatch(
         self,
         request: HttpRequest,
         *args: Any,
         **kwargs: Any,
     ) -> HttpResponseBase:
```

### Comparing `django-salesman-1.1.6/salesman/conf.py` & `django_salesman-1.2.0/salesman/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,14 +287,22 @@
         value and return an HTML formatted string. Also recieves a ``context``
         dictionary with additional render data.
         """
         default = "salesman.admin.utils.format_json"
         value = self._setting("SALESMAN_ADMIN_JSON_FORMATTER", default)
         return self._function(value)
 
+    @property
+    def SALESMAN_ALLOW_ANONYMOUS_USER_CHECKOUT(self) -> bool:
+        """
+        Set to ``False`` if you want to prevent to order if user not authorized.
+        """
+        value: bool = self._setting("SALESMAN_ALLOW_ANONYMOUS_USER_CHECKOUT", True)
+        return value
+
     def _setting(self, name: str, default: Any = None) -> Any:
         from django.conf import settings
 
         return getattr(settings, name, default)
 
     def _error(self, message: str | Exception) -> None:
         from django.core.exceptions import ImproperlyConfigured
```

### Comparing `django-salesman-1.1.6/salesman/core/typing.py` & `django_salesman-1.2.0/salesman/core/typing.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/core/utils.py` & `django_salesman-1.2.0/salesman/core/utils.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/orders/migrations/0001_initial.py` & `django_salesman-1.2.0/salesman/orders/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/orders/migrations/0002_alter_order_ref.py` & `django_salesman-1.2.0/salesman/orders/migrations/0002_alter_order_ref.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/orders/migrations/0003_alter_json_fields.py` & `django_salesman-1.2.0/salesman/orders/migrations/0003_alter_json_fields.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/orders/models.py` & `django_salesman-1.2.0/salesman/orders/models.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/orders/serializers.py` & `django_salesman-1.2.0/salesman/orders/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 
     def validate_payment_method(self, value: str) -> PaymentMethod | None:
         order, request = self.context["order"], self.context["request"]
         payment = payment_methods_pool.get_payment(value)
         if payment:
             payment.validate_order(order, request)
             return payment
-        return None  # pragma: no cover
+        return None
 
     def save(self, **kwargs: Any) -> None:
         # Process the payment.
         order, request = self.context["order"], self.context["request"]
         payment = self.validated_data["payment_method"]
         data = payment.order_payment(order, request)
         # Returning string in payments converts to a URL data value.
```

### Comparing `django-salesman-1.1.6/salesman/orders/status.py` & `django_salesman-1.2.0/salesman/orders/status.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/orders/utils.py` & `django_salesman-1.2.0/salesman/orders/utils.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/salesman/orders/views.py` & `django_salesman-1.2.0/salesman/orders/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -87,75 +87,83 @@
         self,
         request: HttpRequest,
         *args: Any,
         **kwargs: Any,
     ) -> HttpResponseBase:
         return super().dispatch(request, *args, **kwargs)
 
-    @action(detail=False, methods=["get"])
+    @action(["get"], False)
     def last(self, request: Request) -> Response:
         """
         Show last customer order.
         """
         order = self.get_queryset().order_by("date_created").last()
         if not order:
             raise Http404
         serializer = self.get_serializer(order)
         return Response(serializer.data)
 
-    @action(detail=False, methods=["get"], permission_classes=[IsAdminUser])
+    @action(["get"], False, permission_classes=[IsAdminUser])
     def all(self, request: Request) -> Response:
         """
         Show all orders to the admin user.
         """
         return self.list(request)
 
     @action(
-        detail=True,
-        methods=["get", "put"],
+        ["get"],
+        True,
         serializer_class=OrderStatusSerializer,
         permission_classes=[IsAdminUser],
     )
     def status(self, request: Request, ref: str) -> Response:
         """
-        Change order status. Available only to admin user.
+        View order status. Available only to admin user.
         """
         order = self.get_object()
+        serializer = self.get_serializer(order)
+        return Response(serializer.data)
 
-        if request.method == "GET":
-            serializer = self.get_serializer(order)
-            return Response(serializer.data)
-
+    @status.mapping.put
+    def status_update(self, request: Request, ref: str) -> Response:
+        """
+        Update order status. Available only to admin user.
+        """
+        order = self.get_object()
         serializer = self.get_serializer(order, data=request.data, partial=True)
         serializer.is_valid(raise_exception=True)
         serializer.save()
         return Response(serializer.data)
 
-    @action(detail=True, methods=["get", "post"], serializer_class=OrderPaySerializer)
+    @action(["get"], True, serializer_class=OrderPaySerializer)
     def pay(self, request: Request, ref: str) -> Response:
         """
-        Pay for order.
+        View order payment methods.
         """
-        if request.method == "GET":
-            instance = {"payment_methods": payment_methods_pool.get_payments("order")}
-            serializer = self.get_serializer(instance)
-            return Response(serializer.data)
+        instance = {"payment_methods": payment_methods_pool.get_payments("order")}
+        serializer = self.get_serializer(instance)
+        return Response(serializer.data)
 
+    @pay.mapping.post
+    def pay_create(self, request: Request, ref: str) -> Response:
+        """
+        Create order payment.
+        """
         serializer = self.get_serializer(data=request.data)
         serializer.is_valid(raise_exception=True)
         try:
             serializer.save()
             headers = {"Location": serializer.data["url"]}
             return Response(serializer.data, headers=headers)
         except PaymentError as e:
             return Response({"detail": str(e)}, status=status.HTTP_402_PAYMENT_REQUIRED)
 
     @action(
-        detail=True,
-        methods=["post"],
+        ["post"],
+        True,
         serializer_class=OrderRefundSerializer,
         permission_classes=[IsAdminUser],
     )
     def refund(self, request: Request, ref: str) -> Response:
         """
         Refund all order payments.
         """
```

### Comparing `django-salesman-1.1.6/salesman/urls.py` & `django_salesman-1.2.0/salesman/urls.py`

 * *Files identical despite different names*

### Comparing `django-salesman-1.1.6/PKG-INFO` & `django_salesman-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: django-salesman
-Version: 1.1.6
+Version: 1.2.0
 Summary: Headless e-commerce framework for Django and Wagtail.
 Home-page: https://pypi.org/project/django-salesman/
 License: BSD-3-Clause
 Keywords: e-commerce,headless,rest-api,shop,framework
 Author: Dino Perovic
 Author-email: dino.perovic@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Provides-Extra: docs
 Provides-Extra: example
 Provides-Extra: pygments
 Provides-Extra: tests
-Requires-Dist: Pygments (>=2.6,<3.0); extra == "pygments" or extra == "example" or extra == "tests"
-Requires-Dist: django (>=3.1,<4.2)
-Requires-Dist: djangorestframework (>=3.11,<3.15)
-Requires-Dist: pytest (>=7.0.0,<7.1.0); extra == "tests"
-Requires-Dist: pytest-cov (>=3.0.0,<3.1.0); extra == "tests"
-Requires-Dist: pytest-django (>=4.5.0,<4.6.0); extra == "tests"
-Requires-Dist: sphinx (>=4.4.0,<4.5.0); extra == "docs"
-Requires-Dist: sphinx-autobuild (>=2021.3.0,<2021.4.0); extra == "docs"
-Requires-Dist: sphinx-rtd-theme (>=1.0.0,<1.1.0); extra == "docs"
-Requires-Dist: sphinxcontrib-httpdomain (>=1.8.0,<1.9.0); extra == "docs"
-Requires-Dist: wagtail (>=2.9,<4.2); extra == "example" or extra == "tests" or extra == "docs"
+Requires-Dist: Pygments (>=2.6,<3.0) ; extra == "pygments" or extra == "example" or extra == "tests"
+Requires-Dist: django (>=4.1.3,<4.3)
+Requires-Dist: djangorestframework (>=3.11.1,<4.0)
+Requires-Dist: pytest (>=7.0.0,<7.1.0) ; extra == "tests"
+Requires-Dist: pytest-cov (>=3.0.0,<3.1.0) ; extra == "tests"
+Requires-Dist: pytest-django (>=4.5.0,<4.6.0) ; extra == "tests"
+Requires-Dist: sphinx (>=4.4.0,<4.5.0) ; extra == "docs"
+Requires-Dist: sphinx-autobuild (>=2021.3.0,<2021.4.0) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=1.0.0,<1.1.0) ; extra == "docs"
+Requires-Dist: sphinxcontrib-httpdomain (>=1.8.0,<1.9.0) ; extra == "docs"
+Requires-Dist: wagtail (>=4.0,<6.0) ; extra == "example" or extra == "tests" or extra == "docs"
 Project-URL: Documentation, https://django-salesman.readthedocs.io
 Project-URL: Repository, https://github.com/dinoperovic/django-salesman
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="https://django-salesman.readthedocs.org/">
         <img src="https://cdn.jsdelivr.net/gh/dinoperovic/django-salesman@master/docs/_static/logo.svg" width="250" alt="Salesman logo">
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: django-salesman Version: 1.1.6 Summary: Headless e-
+Metadata-Version: 2.1 Name: django-salesman Version: 1.2.0 Summary: Headless e-
 commerce framework for Django and Wagtail. Home-page: https://pypi.org/project/
 django-salesman/ License: BSD-3-Clause Keywords: e-commerce,headless,rest-
 api,shop,framework Author: Dino Perovic Author-email: dino.perovic@gmail.com
 Requires-Python: >=3.8.1,<4.0 Classifier: Development Status :: 5 - Production/
-Stable Classifier: Framework :: Django Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2 Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Wagtail Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3 Classifier: Framework :: Wagtail :: 4
+Stable Classifier: Framework :: Django Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 4 Classifier: Framework :: Wagtail :: 5
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: BSD License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
-Internet Provides-Extra: docs Provides-Extra: example Provides-Extra: pygments
-Provides-Extra: tests Requires-Dist: Pygments (>=2.6,<3.0); extra == "pygments"
-or extra == "example" or extra == "tests" Requires-Dist: django (>=3.1,<4.2)
-Requires-Dist: djangorestframework (>=3.11,<3.15) Requires-Dist: pytest
-(>=7.0.0,<7.1.0); extra == "tests" Requires-Dist: pytest-cov (>=3.0.0,<3.1.0);
-extra == "tests" Requires-Dist: pytest-django (>=4.5.0,<4.6.0); extra ==
-"tests" Requires-Dist: sphinx (>=4.4.0,<4.5.0); extra == "docs" Requires-Dist:
-sphinx-autobuild (>=2021.3.0,<2021.4.0); extra == "docs" Requires-Dist: sphinx-
-rtd-theme (>=1.0.0,<1.1.0); extra == "docs" Requires-Dist: sphinxcontrib-
-httpdomain (>=1.8.0,<1.9.0); extra == "docs" Requires-Dist: wagtail
-(>=2.9,<4.2); extra == "example" or extra == "tests" or extra == "docs"
-Project-URL: Documentation, https://django-salesman.readthedocs.io Project-URL:
-Repository, https://github.com/dinoperovic/django-salesman Description-Content-
-Type: text/markdown
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Internet Provides-
+Extra: docs Provides-Extra: example Provides-Extra: pygments Provides-Extra:
+tests Requires-Dist: Pygments (>=2.6,<3.0) ; extra == "pygments" or extra ==
+"example" or extra == "tests" Requires-Dist: django (>=4.1.3,<4.3) Requires-
+Dist: djangorestframework (>=3.11.1,<4.0) Requires-Dist: pytest
+(>=7.0.0,<7.1.0) ; extra == "tests" Requires-Dist: pytest-cov (>=3.0.0,<3.1.0)
+; extra == "tests" Requires-Dist: pytest-django (>=4.5.0,<4.6.0) ; extra ==
+"tests" Requires-Dist: sphinx (>=4.4.0,<4.5.0) ; extra == "docs" Requires-Dist:
+sphinx-autobuild (>=2021.3.0,<2021.4.0) ; extra == "docs" Requires-Dist:
+sphinx-rtd-theme (>=1.0.0,<1.1.0) ; extra == "docs" Requires-Dist:
+sphinxcontrib-httpdomain (>=1.8.0,<1.9.0) ; extra == "docs" Requires-Dist:
+wagtail (>=4.0,<6.0) ; extra == "example" or extra == "tests" or extra ==
+"docs" Project-URL: Documentation, https://django-salesman.readthedocs.io
+Project-URL: Repository, https://github.com/dinoperovic/django-salesman
+Description-Content-Type: text/markdown
                                 [Salesman_logo]
         **** Headless e-commerce framework for Django and Wagtail. ****
 [PyPI] [GitHub_-_Test_status] [Codecov_branch] [PyPI_-_Python_Version] [PyPI_-
                       Django_Version] [Code_style:_black]
 **Salesman** provides a configurable system for building an online store. It
 includes a **RESTful** API with endpoints for manipulating the basket,
 processing the checkout and payment operations as well as managing customer
```

