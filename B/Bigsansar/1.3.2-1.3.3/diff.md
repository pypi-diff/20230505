# Comparing `tmp/Bigsansar-1.3.2.tar.gz` & `tmp/Bigsansar-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-1.3.2.tar", last modified: Fri May  5 00:43:06 2023, max compression
+gzip compressed data, was "Bigsansar-1.3.3.tar", last modified: Fri May  5 01:35:20 2023, max compression
```

## Comparing `Bigsansar-1.3.2.tar` & `Bigsansar-1.3.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.825087 Bigsansar-1.3.2/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.805087 Bigsansar-1.3.2/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3121 2023-05-05 00:43:06.000000 Bigsansar-1.3.2/Bigsansar.egg-info/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2326 2023-05-05 00:43:06.000000 Bigsansar-1.3.2/Bigsansar.egg-info/SOURCES.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-05-05 00:43:06.000000 Bigsansar-1.3.2/Bigsansar.egg-info/dependency_links.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-05-05 00:43:06.000000 Bigsansar-1.3.2/Bigsansar.egg-info/entry_points.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       82 2023-05-05 00:43:06.000000 Bigsansar-1.3.2/Bigsansar.egg-info/requires.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-05-05 00:43:06.000000 Bigsansar-1.3.2/Bigsansar.egg-info/top_level.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3121 2023-05-05 00:43:06.825087 Bigsansar-1.3.2/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2508 2023-04-29 15:26:29.000000 Bigsansar-1.3.2/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.805087 Bigsansar-1.3.2/bigsansar/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.805087 Bigsansar-1.3.2/bigsansar/contrib/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.805087 Bigsansar-1.3.2/bigsansar/contrib/account/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/account/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/account/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/account/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.805087 Bigsansar-1.3.2/bigsansar/contrib/account/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/account/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/account/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/account/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.805087 Bigsansar-1.3.2/bigsansar/contrib/account/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/account/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/account/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/account/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.805087 Bigsansar-1.3.2/bigsansar/contrib/blogs/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/blogs/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      541 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/blogs/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/blogs/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.805087 Bigsansar-1.3.2/bigsansar/contrib/blogs/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2218 2023-05-02 12:46:38.000000 Bigsansar-1.3.2/bigsansar/contrib/blogs/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      514 2023-05-05 00:37:47.000000 Bigsansar-1.3.2/bigsansar/contrib/blogs/migrations/0002_remove_post_thumbnails_alter_post_body.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:45:50.000000 Bigsansar-1.3.2/bigsansar/contrib/blogs/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1386 2023-05-05 00:37:31.000000 Bigsansar-1.3.2/bigsansar/contrib/blogs/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/blogs/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/blogs/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.805087 Bigsansar-1.3.2/bigsansar/contrib/sites/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/sites/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/sites/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/sites/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3033 2023-05-02 11:56:47.000000 Bigsansar-1.3.2/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.805087 Bigsansar-1.3.2/bigsansar/contrib/sites/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1847 2023-05-02 12:46:38.000000 Bigsansar-1.3.2/bigsansar/contrib/sites/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:46:31.000000 Bigsansar-1.3.2/bigsansar/contrib/sites/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1891 2023-04-29 15:17:38.000000 Bigsansar-1.3.2/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.805087 Bigsansar-1.3.2/bigsansar/contrib/sites/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/sites/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/sites/templatetags/pages.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/sites/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/contrib/sites/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.815087 Bigsansar-1.3.2/bigsansar/core/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/core/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/core/host.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     8915 2023-05-05 00:42:07.000000 Bigsansar-1.3.2/bigsansar/core/init.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/main.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.815087 Bigsansar-1.3.2/bigsansar/management/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.815087 Bigsansar-1.3.2/bigsansar/management/commands/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/management/commands/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.3.2/bigsansar/management/commands/createuser.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.815087 Bigsansar-1.3.2/bigsansar/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.815087 Bigsansar-1.3.2/bigsansar/static/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/static/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/static/logo.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 00:43:06.825087 Bigsansar-1.3.2/bigsansar/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/templates/404.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/templates/acc_active_email.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1134 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/templates/base.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/templates/default.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/templates/defaultpage.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2171 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/templates/nav.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/templates/parking.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      821 2023-04-27 12:27:15.000000 Bigsansar-1.3.2/bigsansar/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1908 2023-05-02 11:45:28.000000 Bigsansar-1.3.2/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-05-05 00:43:06.825087 Bigsansar-1.3.2/setup.cfg
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1294 2023-05-05 00:39:49.000000 Bigsansar-1.3.2/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.335107 Bigsansar-1.3.3/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.305107 Bigsansar-1.3.3/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3130 2023-05-05 01:35:20.000000 Bigsansar-1.3.3/Bigsansar.egg-info/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2326 2023-05-05 01:35:20.000000 Bigsansar-1.3.3/Bigsansar.egg-info/SOURCES.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-05-05 01:35:20.000000 Bigsansar-1.3.3/Bigsansar.egg-info/dependency_links.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-05-05 01:35:20.000000 Bigsansar-1.3.3/Bigsansar.egg-info/entry_points.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       82 2023-05-05 01:35:20.000000 Bigsansar-1.3.3/Bigsansar.egg-info/requires.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-05-05 01:35:20.000000 Bigsansar-1.3.3/Bigsansar.egg-info/top_level.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3130 2023-05-05 01:35:20.335107 Bigsansar-1.3.3/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2517 2023-05-05 01:34:40.000000 Bigsansar-1.3.3/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.305107 Bigsansar-1.3.3/bigsansar/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.305107 Bigsansar-1.3.3/bigsansar/contrib/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.315107 Bigsansar-1.3.3/bigsansar/contrib/account/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/account/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/account/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/account/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.315107 Bigsansar-1.3.3/bigsansar/contrib/account/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/account/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/account/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/account/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.315107 Bigsansar-1.3.3/bigsansar/contrib/account/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/account/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/account/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/account/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.315107 Bigsansar-1.3.3/bigsansar/contrib/blogs/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/blogs/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      541 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/blogs/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/blogs/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.315107 Bigsansar-1.3.3/bigsansar/contrib/blogs/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2218 2023-05-02 12:46:38.000000 Bigsansar-1.3.3/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      514 2023-05-05 00:37:47.000000 Bigsansar-1.3.3/bigsansar/contrib/blogs/migrations/0002_remove_post_thumbnails_alter_post_body.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:45:50.000000 Bigsansar-1.3.3/bigsansar/contrib/blogs/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1386 2023-05-05 00:37:31.000000 Bigsansar-1.3.3/bigsansar/contrib/blogs/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/blogs/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.315107 Bigsansar-1.3.3/bigsansar/contrib/sites/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/sites/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/sites/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/sites/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3033 2023-05-02 11:56:47.000000 Bigsansar-1.3.3/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.325107 Bigsansar-1.3.3/bigsansar/contrib/sites/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1847 2023-05-02 12:46:38.000000 Bigsansar-1.3.3/bigsansar/contrib/sites/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:46:31.000000 Bigsansar-1.3.3/bigsansar/contrib/sites/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1891 2023-04-29 15:17:38.000000 Bigsansar-1.3.3/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.325107 Bigsansar-1.3.3/bigsansar/contrib/sites/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/sites/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/sites/templatetags/pages.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/sites/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/contrib/sites/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.325107 Bigsansar-1.3.3/bigsansar/core/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/core/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/core/host.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9536 2023-05-05 01:33:32.000000 Bigsansar-1.3.3/bigsansar/core/init.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/main.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.325107 Bigsansar-1.3.3/bigsansar/management/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.325107 Bigsansar-1.3.3/bigsansar/management/commands/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/management/commands/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.3.3/bigsansar/management/commands/createuser.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.325107 Bigsansar-1.3.3/bigsansar/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.325107 Bigsansar-1.3.3/bigsansar/static/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/static/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/static/logo.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-05 01:35:20.335107 Bigsansar-1.3.3/bigsansar/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/templates/404.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/templates/acc_active_email.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1134 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/templates/base.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/templates/default.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/templates/defaultpage.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2171 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/templates/nav.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/templates/parking.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      821 2023-04-27 12:27:15.000000 Bigsansar-1.3.3/bigsansar/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1908 2023-05-02 11:45:28.000000 Bigsansar-1.3.3/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-05-05 01:35:20.335107 Bigsansar-1.3.3/setup.cfg
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1294 2023-05-05 01:34:48.000000 Bigsansar-1.3.3/setup.py
```

### Comparing `Bigsansar-1.3.2/Bigsansar.egg-info/PKG-INFO` & `Bigsansar-1.3.3/Bigsansar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.3.2
+Version: 1.3.3
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
@@ -16,65 +16,65 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # How to get Bigsansar
 
-Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3. 
+Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3.
 Bigsansar is Fully based on django.
 You can use
 [bigsansar](https://bigsansar.com)
 for install packaged.
 
-view our tutorials in 
+view our tutorials in
 [youtube](https://youtube.com/bigsansar)
 
 for playlist:
 [bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth)
 
 # Get the latest development version
 The latest and greatest Bigsasnar version is the one that’s in our Git repository (our revision-control system).
-This is only for experienced users who want to try incoming changes and help identify bugs before an official release. 
+This is only for experienced users who want to try incoming changes and help identify bugs before an official release.
 Get it using this shell command, which requires [Git](https://git-scm.com/):
 
 `git clone https://github.com/pokhrelb9/bigsansar.git`
 
-You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version. 
+You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version.
 This archive is updated every time we commit code.
 
 # After you install bigsansar
-Type `bigsansar init` command for **automatically** setup server . 
+Type `bigsansar init` command for **automatically** setup server .
 
 # For manually setup
 
 ### After you get it
 
-go to `www` path and open `settings.py` file then add 
+go to `www` path and open `settings.py` file then add
 `'bigsansar.apps.BigsansarConfig'`
 `'bigsansar.contrib.account.apps.AccountConfig'`
-in to 
+in to
 `INSTALLED_APPS = []` .
 
 ### For Virtualhost middleware
-go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of 
+go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of
 `MIDDLEWARE = []` .
 
 ## Some usefull commands:
 
 `python3 manage.py createuser` - get unlimited users.
 
 
 
-## New update 
+## New update
+* added ckeditor_uploader models and settings for blog apps 
 * added Description model in domain site
-* added setting for postgres 
-* added sercure proxy ssl header 
+* added setting for postgres
+* added sercure proxy ssl header
 * fixed domain index and pages views system
-* added virtual host in to admin pannel 
 
 
 ## Load page list in templates
 
 `{% load pages %}
 
 {% get_pages  as listpage %}
```

### Comparing `Bigsansar-1.3.2/Bigsansar.egg-info/SOURCES.txt` & `Bigsansar-1.3.3/Bigsansar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/LICENSE` & `Bigsansar-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/PKG-INFO` & `Bigsansar-1.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.3.2
+Version: 1.3.3
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
@@ -16,65 +16,65 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # How to get Bigsansar
 
-Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3. 
+Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3.
 Bigsansar is Fully based on django.
 You can use
 [bigsansar](https://bigsansar.com)
 for install packaged.
 
-view our tutorials in 
+view our tutorials in
 [youtube](https://youtube.com/bigsansar)
 
 for playlist:
 [bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth)
 
 # Get the latest development version
 The latest and greatest Bigsasnar version is the one that’s in our Git repository (our revision-control system).
-This is only for experienced users who want to try incoming changes and help identify bugs before an official release. 
+This is only for experienced users who want to try incoming changes and help identify bugs before an official release.
 Get it using this shell command, which requires [Git](https://git-scm.com/):
 
 `git clone https://github.com/pokhrelb9/bigsansar.git`
 
-You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version. 
+You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version.
 This archive is updated every time we commit code.
 
 # After you install bigsansar
-Type `bigsansar init` command for **automatically** setup server . 
+Type `bigsansar init` command for **automatically** setup server .
 
 # For manually setup
 
 ### After you get it
 
-go to `www` path and open `settings.py` file then add 
+go to `www` path and open `settings.py` file then add
 `'bigsansar.apps.BigsansarConfig'`
 `'bigsansar.contrib.account.apps.AccountConfig'`
-in to 
+in to
 `INSTALLED_APPS = []` .
 
 ### For Virtualhost middleware
-go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of 
+go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of
 `MIDDLEWARE = []` .
 
 ## Some usefull commands:
 
 `python3 manage.py createuser` - get unlimited users.
 
 
 
-## New update 
+## New update
+* added ckeditor_uploader models and settings for blog apps 
 * added Description model in domain site
-* added setting for postgres 
-* added sercure proxy ssl header 
+* added setting for postgres
+* added sercure proxy ssl header
 * fixed domain index and pages views system
-* added virtual host in to admin pannel 
 
 
 ## Load page list in templates
 
 `{% load pages %}
 
 {% get_pages  as listpage %}
```

### Comparing `Bigsansar-1.3.2/README.md` & `Bigsansar-1.3.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 
 # How to get Bigsansar
 
-Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3. 
+Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3.
 Bigsansar is Fully based on django.
 You can use
 [bigsansar](https://bigsansar.com)
 for install packaged.
 
-view our tutorials in 
+view our tutorials in
 [youtube](https://youtube.com/bigsansar)
 
 for playlist:
 [bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth)
 
 # Get the latest development version
 The latest and greatest Bigsasnar version is the one that’s in our Git repository (our revision-control system).
-This is only for experienced users who want to try incoming changes and help identify bugs before an official release. 
+This is only for experienced users who want to try incoming changes and help identify bugs before an official release.
 Get it using this shell command, which requires [Git](https://git-scm.com/):
 
 `git clone https://github.com/pokhrelb9/bigsansar.git`
 
-You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version. 
+You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version.
 This archive is updated every time we commit code.
 
 # After you install bigsansar
-Type `bigsansar init` command for **automatically** setup server . 
+Type `bigsansar init` command for **automatically** setup server .
 
 # For manually setup
 
 ### After you get it
 
-go to `www` path and open `settings.py` file then add 
+go to `www` path and open `settings.py` file then add
 `'bigsansar.apps.BigsansarConfig'`
 `'bigsansar.contrib.account.apps.AccountConfig'`
-in to 
+in to
 `INSTALLED_APPS = []` .
 
 ### For Virtualhost middleware
-go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of 
+go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of
 `MIDDLEWARE = []` .
 
 ## Some usefull commands:
 
 `python3 manage.py createuser` - get unlimited users.
 
 
 
-## New update 
+## New update
+* added ckeditor_uploader models and settings for blog apps 
 * added Description model in domain site
-* added setting for postgres 
-* added sercure proxy ssl header 
+* added setting for postgres
+* added sercure proxy ssl header
 * fixed domain index and pages views system
-* added virtual host in to admin pannel 
 
 
 ## Load page list in templates
 
 `{% load pages %}
 
 {% get_pages  as listpage %}
```

### Comparing `Bigsansar-1.3.2/bigsansar/contrib/account/forms.py` & `Bigsansar-1.3.3/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/contrib/account/migrations/0001_initial.py` & `Bigsansar-1.3.3/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/contrib/account/models.py` & `Bigsansar-1.3.3/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/contrib/blogs/admin.py` & `Bigsansar-1.3.3/bigsansar/contrib/blogs/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/contrib/blogs/migrations/0001_initial.py` & `Bigsansar-1.3.3/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/contrib/blogs/migrations/0002_remove_post_thumbnails_alter_post_body.py` & `Bigsansar-1.3.3/bigsansar/contrib/blogs/migrations/0002_remove_post_thumbnails_alter_post_body.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/contrib/blogs/models.py` & `Bigsansar-1.3.3/bigsansar/contrib/blogs/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/contrib/sites/admin.py` & `Bigsansar-1.3.3/bigsansar/contrib/sites/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/contrib/sites/forms.py` & `Bigsansar-1.3.3/bigsansar/contrib/sites/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/contrib/sites/migrations/0001_initial.py` & `Bigsansar-1.3.3/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/contrib/sites/models.py` & `Bigsansar-1.3.3/bigsansar/contrib/sites/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/core/__init__.py` & `Bigsansar-1.3.3/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/core/init.py` & `Bigsansar-1.3.3/bigsansar/core/init.py`

 * *Files 13% similar despite different names*

```diff
@@ -117,21 +117,34 @@
                     lines.insert(getlinetemplate, newhomedirs)
 
             contents = "".join(lines)
             f.write(contents)
             f.close()
 
         # Open a file with access mode 'a'
-        with open("www/urls.py", "a") as file_object:
+        with open("www/urls.py", "w") as file_object:
             # Append 'hello' at the end of file
             file_object.write(''
                               'from django.conf import settings'
                               '\n'
                               'from django.conf.urls.static import static'
                               '\n'
+                              'from django.contrib import admin'
+                              '\n'
+                              'from django.urls import include, path'
+                              '\n'
+                              '\n'
+                              'urlpatterns = ['
+                              '\n'
+                              'path("imagelist/", include("ckeditor_uploader.urls")),'
+                              '\n'
+                              'path("", admin.site.urls),'
+                              '\n'
+                              ']'
+                              '\n'
                               '\n'
                               'urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)'
                               '\n'
                               'admin.site.site_header = "BIGSANSAR"'
                               '\n'
                               'admin.site.site_title = "Bigsansar"'
                               '\n'
```

### Comparing `Bigsansar-1.3.2/bigsansar/management/commands/createuser.py` & `Bigsansar-1.3.3/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/static/logo.png` & `Bigsansar-1.3.3/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/static/style.css` & `Bigsansar-1.3.3/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/templates/404.html` & `Bigsansar-1.3.3/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/templates/base.html` & `Bigsansar-1.3.3/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/templates/default.html` & `Bigsansar-1.3.3/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/templates/defaultpage.html` & `Bigsansar-1.3.3/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/templates/nav.html` & `Bigsansar-1.3.3/bigsansar/templates/nav.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/templates/parking.html` & `Bigsansar-1.3.3/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/urls.py` & `Bigsansar-1.3.3/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/bigsansar/views.py` & `Bigsansar-1.3.3/bigsansar/views.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.3.2/setup.py` & `Bigsansar-1.3.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="1.3.2",
+    version="1.3.3",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bigsansar.com",
     project_urls={
```

