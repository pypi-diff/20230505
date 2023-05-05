# Comparing `tmp/invenio-notifications-0.1.0.tar.gz` & `tmp/invenio-notifications-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-notifications-0.1.0.tar", last modified: Thu May  4 14:58:30 2023, max compression
+gzip compressed data, was "dist/invenio-notifications-0.1.1.tar", last modified: Fri May  5 11:31:57 2023, max compression
```

## Comparing `invenio-notifications-0.1.0.tar` & `invenio-notifications-0.1.1.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/backends/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications/backends/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/backends/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/backends/utils/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications/services/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/services/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/services/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/services/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/services/uow.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/invenio_notifications/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.accepted.html
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.accepted.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.created.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.created.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.declined.html
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.declined.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.created.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.created.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.deleted.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.deleted.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.submitted.html
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.submitted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/invenio_notifications/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/invenio_notifications.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:58:30.000000 invenio-notifications-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-04 14:58:22.000000 invenio-notifications-0.1.0/tests/test_invenio_notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/backends/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/backends/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/backends/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/backends/utils/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/services/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/services/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/services/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/services/uow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.accepted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.accepted.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.created.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.created.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.declined.html
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.declined.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.created.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.created.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.deleted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.deleted.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.submitted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.submitted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/translations/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-05 11:31:56.000000 invenio-notifications-0.1.1/invenio_notifications/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/invenio_notifications/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/invenio_notifications.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:31:57.000000 invenio-notifications-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-05 11:31:47.000000 invenio-notifications-0.1.1/tests/test_invenio_notifications.py
```

### Comparing `invenio-notifications-0.1.0/.editorconfig` & `invenio-notifications-0.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/.github/workflows/pypi-publish.yml` & `invenio-notifications-0.1.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/.github/workflows/tests.yml` & `invenio-notifications-0.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/.tx/config` & `invenio-notifications-0.1.1/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/CONTRIBUTING.rst` & `invenio-notifications-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/MANIFEST.in` & `invenio-notifications-0.1.1/MANIFEST.in`

 * *Files 10% similar despite different names*

```diff
@@ -18,7 +18,8 @@
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
 recursive-include docs Makefile
 recursive-include invenio_notifications *.html *.txt
 recursive-include invenio_notifications/translations *.po *.pot *.mo
 recursive-include tests *.py
+recursive-include invenio_notifications *.gitkeep
```

### Comparing `invenio-notifications-0.1.0/PKG-INFO` & `invenio-notifications-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-notifications
-Version: 0.1.0
+Version: 0.1.1
 Summary: "Invenio module for notifications support."
 Home-page: https://github.com/inveniosoftware/invenio-notifications
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2023 CERN.
@@ -40,15 +40,19 @@
             Invenio-Notifications is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
-        Version 0.1.0
+        Version 0.1.1 (released 2023-05-05)
+        
+        - remove type hints
+        
+        Version 0.1.0 (released 2023-05-04)
         
         - Initial public release.
         
 Keywords: invenio TODO
 Platform: any
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `invenio-notifications-0.1.0/README.rst` & `invenio-notifications-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/babel.ini` & `invenio-notifications-0.1.1/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/docs/Makefile` & `invenio-notifications-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/docs/conf.py` & `invenio-notifications-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/docs/index.rst` & `invenio-notifications-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/docs/make.bat` & `invenio-notifications-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications/__init__.py` & `invenio-notifications-0.1.1/invenio_notifications/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # details.
 
 """Invenio module for notifications support."""
 
 from .ext import InvenioNotifications
 from .proxies import current_notifications, current_notifications_manager
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 __all__ = (
     "__version__",
     "current_notifications",
     "current_notifications_manager",
     "InvenioNotifications",
 )
```

### Comparing `invenio-notifications-0.1.0/invenio_notifications/backends/base.py` & `invenio-notifications-0.1.1/invenio_notifications/backends/base.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications/backends/email.py` & `invenio-notifications-0.1.1/invenio_notifications/backends/email.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications/backends/utils/loaders.py` & `invenio-notifications-0.1.1/invenio_notifications/backends/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications/config.py` & `invenio-notifications-0.1.1/invenio_notifications/config.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications/errors.py` & `invenio-notifications-0.1.1/invenio_notifications/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications/ext.py` & `invenio-notifications-0.1.1/invenio_notifications/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications/manager.py` & `invenio-notifications-0.1.1/invenio_notifications/manager.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications/models.py` & `invenio-notifications-0.1.1/invenio_notifications/models.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications/proxies.py` & `invenio-notifications-0.1.1/invenio_notifications/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications/registry.py` & `invenio-notifications-0.1.1/invenio_notifications/registry.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications/services/builders.py` & `invenio-notifications-0.1.1/invenio_notifications/services/generators.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2023 CERN.
 # Copyright (C) 2023 Graz University of Technology.
 #
 # Invenio-Notifications is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
-"""Builderes for notifications."""
+"""Generators for notification context."""
 
 from abc import ABC, abstractmethod
 
-from invenio_notifications.services.filters import RecipientFilter
-from invenio_notifications.services.generators import (
-    ContextGenerator,
-    RecipientBackendGenerator,
-    RecipientGenerator,
-)
+from invenio_records.dictutils import dict_lookup, dict_set
 
+from invenio_notifications.backends.email import EmailNotificationBackend
+from invenio_notifications.registry import EntityResolverRegistry
 
-class NotificationBuilder(ABC):
-    """Base notification builder."""
 
-    context: list[ContextGenerator]
-    recipients: list[RecipientGenerator]
-    recipient_filters: list[RecipientFilter]
-    recipient_backends: list[RecipientBackendGenerator]
+class ContextGenerator(ABC):
+    """Payload generator for a notification."""
 
-    type = "Notification"
+    @abstractmethod
+    def __call__(self, notification):
+        """Update notification context."""
+        raise NotImplementedError()
+
+
+class RecipientGenerator(ABC):
+    """Recipient generator for a notification."""
 
-    @classmethod
     @abstractmethod
-    def build(cls, **kwargs):
-        """Build notification based on type and additional context."""
+    def __call__(self, notification, recipients):
+        """Add recipients."""
         raise NotImplementedError()
 
-    @classmethod
-    def resolve_context(cls, notification):
-        """Resolve all references in the notification context."""
-        for ctx_func in cls.context:
-            # NOTE: We assume that the notification is mutable and modified in-place
-            ctx_func(notification)
+
+class RecipientBackendGenerator(ABC):
+    """Backend generator for a notification."""
+
+    @abstractmethod
+    def __call__(self, notification, recipient, backends):
+        """Update required recipient information and add backend id."""
+        raise NotImplementedError()
+
+
+class EntityResolve(ContextGenerator):
+    """Payload generator for a notification using the entity resolvers."""
+
+    def __init__(self, key):
+        """Ctor."""
+        self.key = key
+
+    def __call__(self, notification):
+        """Update required recipient information and add backend id."""
+        entity_ref = dict_lookup(notification.context, self.key)
+        entity = EntityResolverRegistry.resolve_entity(entity_ref)
+        dict_set(notification.context, self.key, entity)
         return notification
 
-    @classmethod
-    def build_recipients(cls, notification):
-        """Return a dictionary of unique recipients for the notification."""
-        recipients = {}
-        for recipient_func in cls.recipients:
-            recipient_func(notification, recipients)
-        return recipients
-
-    @classmethod
-    def filter_recipients(cls, notification, recipients):
-        """Apply filters to the recipients."""
-        for recipient_filter_func in cls.recipient_filters:
-            recipient_filter_func(notification, recipients)
-        return recipients
-
-    @classmethod
-    def build_recipient_backends(cls, notification, recipient):
-        """Return the backends for recipient."""
-        backends = []
-        for recipient_backend_func in cls.recipient_backends:
-            recipient_backend_func(notification, recipient, backends)
-        return backends
+
+class UserEmailBackend(RecipientBackendGenerator):
+    """User related email backend generator for a notification."""
+
+    def __call__(self, notification, recipient, backends):
+        """Add backend id to backends."""
+        backend_id = EmailNotificationBackend.id
+        backends.append(backend_id)
+        return backend_id
```

### Comparing `invenio-notifications-0.1.0/invenio_notifications/services/filters.py` & `invenio-notifications-0.1.1/invenio_notifications/services/filters.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications/services/uow.py` & `invenio-notifications-0.1.1/invenio_notifications/services/uow.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications/tasks.py` & `invenio-notifications-0.1.1/invenio_notifications/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications/views.py` & `invenio-notifications-0.1.1/invenio_notifications/views.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/invenio_notifications.egg-info/PKG-INFO` & `invenio-notifications-0.1.1/invenio_notifications.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-notifications
-Version: 0.1.0
+Version: 0.1.1
 Summary: "Invenio module for notifications support."
 Home-page: https://github.com/inveniosoftware/invenio-notifications
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2023 CERN.
@@ -40,15 +40,19 @@
             Invenio-Notifications is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
-        Version 0.1.0
+        Version 0.1.1 (released 2023-05-05)
+        
+        - remove type hints
+        
+        Version 0.1.0 (released 2023-05-04)
         
         - Initial public release.
         
 Keywords: invenio TODO
 Platform: any
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `invenio-notifications-0.1.0/invenio_notifications.egg-info/SOURCES.txt` & `invenio-notifications-0.1.1/invenio_notifications.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -61,11 +61,12 @@
 invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-invitation.declined.txt
 invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.created.html
 invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.created.txt
 invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.deleted.html
 invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.deleted.txt
 invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.submitted.html
 invenio_notifications/templates/semantic-ui/invenio_notifications/email/community-submission.submitted.txt
+invenio_notifications/translations/.gitkeep
 invenio_notifications/translations/en/LC_MESSAGES/messages.mo
 invenio_notifications/translations/en/LC_MESSAGES/messages.po
 tests/conftest.py
 tests/test_invenio_notifications.py
```

### Comparing `invenio-notifications-0.1.0/run-tests.sh` & `invenio-notifications-0.1.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/setup.cfg` & `invenio-notifications-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/tests/conftest.py` & `invenio-notifications-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-notifications-0.1.0/tests/test_invenio_notifications.py` & `invenio-notifications-0.1.1/tests/test_invenio_notifications.py`

 * *Files identical despite different names*

