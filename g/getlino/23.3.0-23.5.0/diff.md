# Comparing `tmp/getlino-23.3.0.tar.gz` & `tmp/getlino-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getlino-23.3.0.tar", last modified: Mon Mar 27 21:30:18 2023, max compression
+gzip compressed data, was "getlino-23.5.0.tar", last modified: Fri May  5 04:53:52 2023, max compression
```

## Comparing `getlino-23.3.0.tar` & `getlino-23.5.0.tar`

### file list

```diff
@@ -1,56 +1,48 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-27 21:30:18.546779 getlino-23.3.0/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-27 21:30:18.542779 getlino-23.3.0/.tox/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-27 21:30:18.542779 getlino-23.3.0/.tox/py37/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-27 21:30:18.542779 getlino-23.3.0/.tox/py37/lib/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-27 21:30:18.542779 getlino-23.3.0/.tox/py37/lib/python3.7/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-27 21:30:18.542779 getlino-23.3.0/.tox/py37/lib/python3.7/site-packages/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-27 21:30:18.542779 getlino-23.3.0/.tox/py37/lib/python3.7/site-packages/atelier/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13580 2023-03-19 11:03:02.000000 getlino-23.3.0/.tox/py37/lib/python3.7/site-packages/atelier/rstgen.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13781 2021-04-24 18:50:02.000000 getlino-23.3.0/.tox/py37/lib/python3.7/site-packages/atelier/utils.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:56:36.000000 getlino-23.3.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)       59 2019-10-25 15:17:06.000000 getlino-23.3.0/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     1434 2023-03-27 21:30:18.546779 getlino-23.3.0/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      692 2021-06-11 08:29:48.000000 getlino-23.3.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-27 21:30:18.542779 getlino-23.3.0/getlino/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      321 2021-04-30 10:59:59.000000 getlino-23.3.0/getlino/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      804 2022-07-31 09:59:40.000000 getlino-23.3.0/getlino/cli.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    19692 2023-02-28 06:10:38.000000 getlino-23.3.0/getlino/configure.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2719 2022-05-23 11:26:52.000000 getlino-23.3.0/getlino/list.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1785 2023-03-27 21:29:51.000000 getlino-23.3.0/getlino/setup_info.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     7258 2023-02-14 19:03:00.000000 getlino-23.3.0/getlino/startproject.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    24115 2023-03-14 08:39:22.000000 getlino-23.3.0/getlino/startsite.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-27 21:30:18.546779 getlino-23.3.0/getlino/templates/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      890 2021-02-12 13:40:30.000000 getlino-23.3.0/getlino/templates/apache.conf
--rw-rw-rw-   0 luc       (1000) www-data    (33)      312 2022-09-21 17:49:59.000000 getlino-23.3.0/getlino/templates/apps_section.rst
--rw-rw-rw-   0 luc       (1000) www-data    (33)      214 2022-09-10 15:27:38.000000 getlino-23.3.0/getlino/templates/asgi.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     2084 2022-10-19 13:51:08.000000 getlino-23.3.0/getlino/templates/daphne_supervisor.conf
--rw-rw-r--   0 luc       (1000) www-data    (33)      852 2023-01-01 07:07:06.000000 getlino-23.3.0/getlino/templates/django_settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      220 2019-12-09 08:22:28.000000 getlino-23.3.0/getlino/templates/healthcheck.sh
--rw-rw-r--   0 luc       (1000) www-data    (33)      308 2023-01-15 18:29:24.000000 getlino-23.3.0/getlino/templates/lino.ini
--rwxrwxr-x   0 luc       (1000) www-data    (33)     2074 2022-09-15 06:25:41.000000 getlino-23.3.0/getlino/templates/make_snapshot.sh
--rw-rw-r--   0 luc       (1000) www-data    (33)      335 2023-01-10 07:35:27.000000 getlino-23.3.0/getlino/templates/manage.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1469 2021-02-10 17:55:45.000000 getlino-23.3.0/getlino/templates/nginx.conf
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1543 2022-09-10 15:27:38.000000 getlino-23.3.0/getlino/templates/nginx_asgi.conf
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1397 2023-01-06 15:12:48.000000 getlino-23.3.0/getlino/templates/pull.sh
--rw-rw-r--   0 luc       (1000) www-data    (33)     1492 2023-02-28 06:48:28.000000 getlino-23.3.0/getlino/templates/settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1361 2021-02-10 17:53:35.000000 getlino-23.3.0/getlino/templates/uwsgi.ini
--rw-rw-rw-   0 luc       (1000) www-data    (33)      664 2019-10-25 14:15:15.000000 getlino-23.3.0/getlino/templates/uwsgi_params
--rw-rw-rw-   0 luc       (1000) www-data    (33)      251 2019-10-25 14:30:31.000000 getlino-23.3.0/getlino/templates/wsgi.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    19432 2023-02-28 06:10:38.000000 getlino-23.3.0/getlino/utils.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-27 21:30:18.542779 getlino-23.3.0/getlino.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1434 2023-03-27 21:30:18.000000 getlino-23.3.0/getlino.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1129 2023-03-27 21:30:18.000000 getlino-23.3.0/getlino.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-03-27 21:30:18.000000 getlino-23.3.0/getlino.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2023-03-27 21:30:18.000000 getlino-23.3.0/getlino.egg-info/entry_points.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-06-20 10:29:13.000000 getlino-23.3.0/getlino.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)       56 2023-03-27 21:30:18.000000 getlino-23.3.0/getlino.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        8 2023-03-27 21:30:18.000000 getlino-23.3.0/getlino.egg-info/top_level.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-03-27 21:30:18.546779 getlino-23.3.0/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      260 2020-07-10 08:02:46.000000 getlino-23.3.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      308 2019-08-05 08:32:15.000000 getlino-23.3.0/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-03-27 21:30:18.546779 getlino-23.3.0/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2021-03-02 11:04:28.000000 getlino-23.3.0/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1939 2019-11-05 07:22:27.000000 getlino-23.3.0/tests/test_case.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10166 2022-09-17 02:45:04.000000 getlino-23.3.0/tests/test_docker.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      188 2021-03-05 19:40:47.000000 getlino-23.3.0/tests/test_docs.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      182 2019-10-30 08:08:12.000000 getlino-23.3.0/tests/test_packages.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-05-05 04:53:52.407739 getlino-23.5.0/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    34523 2023-02-28 05:23:11.000000 getlino-23.5.0/COPYING
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       59 2023-02-28 05:23:11.000000 getlino-23.5.0/MANIFEST.in
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1434 2023-05-05 04:53:52.407739 getlino-23.5.0/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      692 2023-02-28 05:23:11.000000 getlino-23.5.0/README.rst
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-05-05 04:53:52.407739 getlino-23.5.0/getlino/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      321 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      804 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/cli.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    19692 2023-03-01 10:55:34.000000 getlino-23.5.0/getlino/configure.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2719 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/list.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1785 2023-05-05 04:52:36.000000 getlino-23.5.0/getlino/setup_info.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     7258 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/startproject.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    24115 2023-03-17 12:08:13.000000 getlino-23.5.0/getlino/startsite.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-05-05 04:53:52.407739 getlino-23.5.0/getlino/templates/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      890 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/templates/apache.conf
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      312 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/templates/apps_section.rst
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      214 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/templates/asgi.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1706 2023-05-03 06:08:47.000000 getlino-23.5.0/getlino/templates/daphne_supervisor.conf
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      852 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/templates/django_settings.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      220 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/templates/healthcheck.sh
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      308 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/templates/lino.ini
+-rwxrwxr-x   0 blurry    (1000) blurry    (1000)     2074 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/templates/make_snapshot.sh
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      335 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/templates/manage.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1469 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/templates/nginx.conf
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1543 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/templates/nginx_asgi.conf
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1429 2023-03-31 11:58:32.000000 getlino-23.5.0/getlino/templates/pull.sh
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1492 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/templates/settings.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1361 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/templates/uwsgi.ini
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      664 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/templates/uwsgi_params
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      251 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino/templates/wsgi.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    19432 2023-03-01 10:55:34.000000 getlino-23.5.0/getlino/utils.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-05-05 04:53:52.407739 getlino-23.5.0/getlino.egg-info/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1434 2023-05-05 04:53:52.000000 getlino-23.5.0/getlino.egg-info/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1018 2023-05-05 04:53:52.000000 getlino-23.5.0/getlino.egg-info/SOURCES.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-05-05 04:53:52.000000 getlino-23.5.0/getlino.egg-info/dependency_links.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       46 2023-05-05 04:53:52.000000 getlino-23.5.0/getlino.egg-info/entry_points.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-02-28 05:23:11.000000 getlino-23.5.0/getlino.egg-info/not-zip-safe
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       56 2023-05-05 04:53:52.000000 getlino-23.5.0/getlino.egg-info/requires.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        8 2023-05-05 04:53:52.000000 getlino-23.5.0/getlino.egg-info/top_level.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       38 2023-05-05 04:53:52.407739 getlino-23.5.0/setup.cfg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      260 2023-02-28 05:23:11.000000 getlino-23.5.0/setup.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      308 2023-02-28 05:23:11.000000 getlino-23.5.0/tasks.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-05-05 04:53:52.407739 getlino-23.5.0/tests/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:11.000000 getlino-23.5.0/tests/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1939 2023-02-28 05:23:11.000000 getlino-23.5.0/tests/test_case.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    10166 2023-02-28 05:23:11.000000 getlino-23.5.0/tests/test_docker.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      188 2023-02-28 05:23:11.000000 getlino-23.5.0/tests/test_docs.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      182 2023-02-28 05:23:11.000000 getlino-23.5.0/tests/test_packages.py
```

### Comparing `getlino-23.3.0/COPYING` & `getlino-23.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/PKG-INFO` & `getlino-23.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getlino
-Version: 23.3.0
+Version: 23.5.0
 Summary: A command-line tool for installing Lino in different environments.
 Home-page: https://gitlab.com/lino-framework/getlino
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `getlino-23.3.0/README.rst` & `getlino-23.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino/cli.py` & `getlino-23.5.0/getlino/cli.py`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino/configure.py` & `getlino-23.5.0/getlino/configure.py`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino/list.py` & `getlino-23.5.0/getlino/list.py`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino/setup_info.py` & `getlino-23.5.0/getlino/setup_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 SETUP_INFO = dict(
     name='getlino',
-    version='23.3.0',
+    version='23.5.0',
     install_requires=['click', 'virtualenv', 'jinja2', 'distro', 'synodal', 'rstgen', 'GitPython'],
     # tests_require=['docker', 'atelier'],
     # test_suite='tests',
     description="A command-line tool for installing Lino in different environments.",
     long_description="""
 ``getlino`` is a command-line tool for installing Lino in different environments.
```

### Comparing `getlino-23.3.0/getlino/startproject.py` & `getlino-23.5.0/getlino/startproject.py`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino/startsite.py` & `getlino-23.5.0/getlino/startsite.py`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino/templates/apache.conf` & `getlino-23.5.0/getlino/templates/apache.conf`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino/templates/daphne_supervisor.conf` & `getlino-23.5.0/getlino/templates/daphne_supervisor.conf`

 * *Files 10% similar despite different names*

```diff
@@ -34,34 +34,20 @@
 redirect_stderr = true
 environment = DJANGO_SETTINGS_MODULE={{django_settings_module}}
 directory = {{project_dir}}
 username = www-data
 umask = 002
 
 [program:{{prjname}}_runworker]
-command=/bin/bash -c "source {{envdir}}/bin/activate && python manage.py runworker {{channels}}"
+command=/bin/bash -c "source {{envdir}}/bin/activate && python manage.py lino_runworker {{channels}}"
 stopsignal=KILL
 killasgroup=true
 priority=998
 startsecs=5
  
 # same for every program:
 #stdout_logfile = {{project_dir}}/log/lino.log
 redirect_stderr = true
 environment = DJANGO_SETTINGS_MODULE={{django_settings_module}}
 directory = {{project_dir}}
 username = www-data
 umask = 002
- 
- 
-[program:{{prjname}}_initiate_linod]
-command=/bin/bash -c "source {{envdir}}/bin/activate && python manage.py initiate_linod"
-autorestart=false
-priority=999
- 
-# same for every program:
-#stdout_logfile = {{project_dir}}/log/lino.log
-redirect_stderr = true
-environment = DJANGO_SETTINGS_MODULE={{django_settings_module}}
-directory = {{project_dir}}
-username = www-data
-umask = 002
```

### Comparing `getlino-23.3.0/getlino/templates/django_settings.py` & `getlino-23.5.0/getlino/templates/django_settings.py`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino/templates/make_snapshot.sh` & `getlino-23.5.0/getlino/templates/make_snapshot.sh`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino/templates/nginx.conf` & `getlino-23.5.0/getlino/templates/nginx.conf`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino/templates/nginx_asgi.conf` & `getlino-23.5.0/getlino/templates/nginx_asgi.conf`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino/templates/pull.sh` & `getlino-23.5.0/getlino/templates/pull.sh`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/bin/bash
 # generated by getlino
-# Copyright 2015-2022 Rumma & Ko Ltd
-# License: BSD (see file COPYING for details)
+# Copyright 2015-2023 Rumma & Ko Ltd
+# License: GNU Affero General Public License v3 (see file COPYING for details)
 #
-# Update the application source code in this environment.
-# Runs either `pip --update` or `git pull` depending on the options specified during startsite.
+# Update the application source code in this environment. Run either `pip
+# --update` or `git pull` depending on the options specified during startsite.
 # Also remove all `*.pyc` files in these repositories.
 
 set -e
 umask 0007
 
 PRJDIR=`pwd`
 ENVDIR={{envdir}}
```

### Comparing `getlino-23.3.0/getlino/templates/settings.py` & `getlino-23.5.0/getlino/templates/settings.py`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino/templates/uwsgi.ini` & `getlino-23.5.0/getlino/templates/uwsgi.ini`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino/templates/uwsgi_params` & `getlino-23.5.0/getlino/templates/uwsgi_params`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino/utils.py` & `getlino-23.5.0/getlino/utils.py`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/getlino.egg-info/PKG-INFO` & `getlino-23.5.0/getlino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getlino
-Version: 23.3.0
+Version: 23.5.0
 Summary: A command-line tool for installing Lino in different environments.
 Home-page: https://gitlab.com/lino-framework/getlino
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `getlino-23.3.0/getlino.egg-info/SOURCES.txt` & `getlino-23.5.0/getlino.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 COPYING
 MANIFEST.in
 README.rst
 setup.py
 tasks.py
-.tox/py37/lib/python3.7/site-packages/atelier/rstgen.py
-.tox/py37/lib/python3.7/site-packages/atelier/utils.py
 getlino/__init__.py
 getlino/cli.py
 getlino/configure.py
 getlino/list.py
 getlino/setup_info.py
 getlino/startproject.py
 getlino/startsite.py
```

### Comparing `getlino-23.3.0/tests/test_case.py` & `getlino-23.5.0/tests/test_case.py`

 * *Files identical despite different names*

### Comparing `getlino-23.3.0/tests/test_docker.py` & `getlino-23.5.0/tests/test_docker.py`

 * *Files identical despite different names*

