# Comparing `tmp/django-admin-anchors-2.0.1.tar.gz` & `tmp/django_admin_anchors-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-anchors-2.0.1.tar", last modified: Sat Apr 10 19:14:30 2021, max compression
+gzip compressed data, was "django_admin_anchors-2.0.2.tar", max compression
```

## Comparing `django-admin-anchors-2.0.1.tar` & `django_admin_anchors-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,7 @@
-drwxr-xr-x   0 john      (1000) users      (100)        0 2021-04-10 19:14:30.765837 django-admin-anchors-2.0.1/
--rw-r--r--   0 john      (1000) users      (100)     1055 2021-03-31 23:06:48.000000 django-admin-anchors-2.0.1/LICENSE
--rw-r--r--   0 john      (1000) users      (100)       34 2021-03-31 23:09:02.000000 django-admin-anchors-2.0.1/MANIFEST.in
--rw-r--r--   0 john      (1000) users      (100)     4555 2021-04-10 19:14:30.765837 django-admin-anchors-2.0.1/PKG-INFO
--rw-r--r--   0 john      (1000) users      (100)     2608 2021-04-10 19:09:23.000000 django-admin-anchors-2.0.1/README.md
-drwxr-xr-x   0 john      (1000) users      (100)        0 2021-04-10 19:14:30.765837 django-admin-anchors-2.0.1/admin_anchors/
--rw-r--r--   0 john      (1000) users      (100)      100 2021-04-09 01:07:53.000000 django-admin-anchors-2.0.1/admin_anchors/__init__.py
--rw-r--r--   0 john      (1000) users      (100)     1697 2021-04-08 23:44:52.000000 django-admin-anchors-2.0.1/admin_anchors/decorators.py
--rw-r--r--   0 john      (1000) users      (100)     1198 2021-04-08 18:22:51.000000 django-admin-anchors-2.0.1/admin_anchors/utils.py
-drwxr-xr-x   0 john      (1000) users      (100)        0 2021-04-10 19:14:30.765837 django-admin-anchors-2.0.1/django_admin_anchors.egg-info/
--rw-r--r--   0 john      (1000) users      (100)     4555 2021-04-10 19:14:30.000000 django-admin-anchors-2.0.1/django_admin_anchors.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) users      (100)      387 2021-04-10 19:14:30.000000 django-admin-anchors-2.0.1/django_admin_anchors.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) users      (100)        1 2021-04-10 19:14:30.000000 django-admin-anchors-2.0.1/django_admin_anchors.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) users      (100)        1 2021-03-31 23:03:19.000000 django-admin-anchors-2.0.1/django_admin_anchors.egg-info/not-zip-safe
--rw-r--r--   0 john      (1000) users      (100)      145 2021-04-10 19:14:30.000000 django-admin-anchors-2.0.1/django_admin_anchors.egg-info/requires.txt
--rw-r--r--   0 john      (1000) users      (100)       14 2021-04-10 19:14:30.000000 django-admin-anchors-2.0.1/django_admin_anchors.egg-info/top_level.txt
--rw-r--r--   0 john      (1000) users      (100)     1358 2021-04-10 19:14:30.765837 django-admin-anchors-2.0.1/setup.cfg
--rw-r--r--   0 john      (1000) users      (100)       38 2021-03-31 22:51:15.000000 django-admin-anchors-2.0.1/setup.py
+-rw-r--r--   0        0        0     1055 2021-03-31 23:06:48.789207 django_admin_anchors-2.0.2/LICENSE
+-rw-r--r--   0        0        0     2050 2023-05-05 13:35:42.593916 django_admin_anchors-2.0.2/README.md
+-rw-r--r--   0        0        0       78 2023-05-05 13:35:42.593916 django_admin_anchors-2.0.2/admin_anchors/__init__.py
+-rw-r--r--   0        0        0     1698 2023-05-05 13:35:42.593916 django_admin_anchors-2.0.2/admin_anchors/decorators.py
+-rw-r--r--   0        0        0     1199 2023-05-05 13:35:42.593916 django_admin_anchors-2.0.2/admin_anchors/utils.py
+-rw-r--r--   0        0        0     1660 2023-05-05 13:41:56.391537 django_admin_anchors-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3688 1970-01-01 00:00:00.000000 django_admin_anchors-2.0.2/PKG-INFO
```

### Comparing `django-admin-anchors-2.0.1/LICENSE` & `django_admin_anchors-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-anchors-2.0.1/README.md` & `django_admin_anchors-2.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Django Admin Anchors
 
 [![PyPI][pypi-image]][pypi-url]
+![PyPI - Python Version][python-image]
+![PyPI - Django Version][django-image]
 [![License][license-image]][license-url]
 [![Tests][tests-image]][tests-url]
 
 [pypi-image]: https://img.shields.io/pypi/v/django-admin-anchors
 [pypi-url]: https://pypi.org/project/django-admin-anchors/
+[python-image]: https://img.shields.io/pypi/pyversions/django-admin-anchors
+[django-image]: https://img.shields.io/pypi/djversions/django-admin-anchors
 [license-image]: https://img.shields.io/pypi/l/django-admin-anchors
 [license-url]: https://github.com/DoctorJohn/django-admin-anchors/blob/master/LICENSE
 [tests-image]: https://github.com/DoctorJohn/django-admin-anchors/workflows/Tests/badge.svg
 [tests-url]: https://github.com/DoctorJohn/django-admin-anchors/actions
 
 Turn Django admin list display items into clickable links to related objects using
 decorators.
@@ -59,35 +63,7 @@
 class PlayerAdmin(admin.ModelAdmin):
     readonly_fields = ["profile_link"]
 
     @admin_anchor("profile")
     def profile_link(self, instance):
         return "Profile"
 ```
-
-## Contributing
-
-### Setup
-
-1. Clone the repository and enter the cloned folder
-2. (optional) Create and activate a dedicated Python virtual environment
-3. Run `pip install -e ".[dev]"` to install the projects requirements
-4. (optional) Run `pre-commit install` to install the pre-commit hook
-
-### Pre-commit hook
-
-Our pre-commit hook formats and lints the code.
-
-### Formatting and linting
-
-- Run `black admin_anchors tests` to format the code
-- Run `flake8 admin_anchors tests` to lint the code
-
-### Testing
-
-- Run `py.test --cov admin_anchors tests` to run the tests in the current Python env
-- Run `tox` to run the tests in all supported Python and Django environments
-
-### Makefile
-
-All commands listed above have shortcut make recipes.
-Take a look at the `Makefile` to learn more.
```

### Comparing `django-admin-anchors-2.0.1/admin_anchors/decorators.py` & `django_admin_anchors-2.0.2/admin_anchors/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from django.db import models
 from django.core.exceptions import ImproperlyConfigured
+from django.db import models
+
 from admin_anchors.utils import (
-    get_selected_obj,
-    get_selected_field,
     create_admin_anchor,
+    get_selected_field,
+    get_selected_obj,
 )
 
 
 def admin_anchor(selector: str):
     def inner(func):
         def wrapper(self, instance) -> str:
             obj = get_selected_obj(instance, selector)
```

### Comparing `django-admin-anchors-2.0.1/admin_anchors/utils.py` & `django_admin_anchors-2.0.2/admin_anchors/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import Optional, Dict, List
-from django.db.models.fields import Field
+from typing import Dict, List, Optional
+
 from django.db import models
+from django.db.models.fields import Field
 from django.urls import reverse
-from django.utils.http import urlencode
 from django.utils.html import format_html
+from django.utils.http import urlencode
 
 
 def create_admin_anchor(
     page_name: str,
     app_label: str,
     model_name: str,
     label: str,
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-from typing import Optional, Dict, List from django.db.models.fields import
-Field from django.db import models from django.urls import reverse from
-django.utils.http import urlencode from django.utils.html import format_html
+from typing import Dict, List, Optional from django.db import models from
+django.db.models.fields import Field from django.urls import reverse from
+django.utils.html import format_html from django.utils.http import urlencode
 def create_admin_anchor( page_name: str, app_label: str, model_name: str,
 label: str, args: Optional[List] = None, query: Optional[Dict] = None, ) -
 > str: url = reverse(f"admin:{app_label}_{model_name}_{page_name}", args=args)
 if query: url += "?" + urlencode(query) return format_html("{}", url, label)
 def get_selected_obj(instance: models.Model, selector: str) -> Optional
 [models.Model]: current = instance # The last part is the selected field parts
 = selector.split(".")[0:-1] for part in parts: current = getattr(current, part,
```

