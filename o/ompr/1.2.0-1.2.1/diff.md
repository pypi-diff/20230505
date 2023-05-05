# Comparing `tmp/ompr-1.2.0.tar.gz` & `tmp/ompr-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ompr-1.2.0.tar", last modified: Sun Mar 26 17:41:02 2023, max compression
+gzip compressed data, was "dist/ompr-1.2.1.tar", last modified: Fri May  5 19:17:54 2023, max compression
```

## Comparing `ompr-1.2.0.tar` & `ompr-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-03-26 17:41:02.000000 ompr-1.2.0/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      215 2023-03-26 17:41:02.000000 ompr-1.2.0/PKG-INFO
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2534 2023-03-05 14:24:41.000000 ompr-1.2.0/README.md
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-03-26 17:41:02.000000 ompr-1.2.0/ompr/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 19:28:36.000000 ompr-1.2.0/ompr/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      275 2023-03-05 12:31:56.000000 ompr-1.2.0/ompr/helpers.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)    24094 2023-03-18 18:24:42.000000 ompr-1.2.0/ompr/runner.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      784 2023-03-05 12:55:32.000000 ompr-1.2.0/ompr/simple.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-03-26 17:41:02.000000 ompr-1.2.0/ompr.egg-info/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      215 2023-03-26 17:41:02.000000 ompr-1.2.0/ompr.egg-info/PKG-INFO
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      220 2023-03-26 17:41:02.000000 ompr-1.2.0/ompr.egg-info/SOURCES.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        1 2023-03-26 17:41:02.000000 ompr-1.2.0/ompr.egg-info/dependency_links.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        6 2023-03-26 17:41:02.000000 ompr-1.2.0/ompr.egg-info/requires.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        5 2023-03-26 17:41:02.000000 ompr-1.2.0/ompr.egg-info/top_level.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       38 2023-03-26 17:41:02.000000 ompr-1.2.0/setup.cfg
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      637 2023-03-26 17:29:18.000000 ompr-1.2.0/setup.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:17:54.000000 ompr-1.2.1/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      215 2023-05-05 19:17:54.000000 ompr-1.2.1/PKG-INFO
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2534 2023-03-05 14:24:41.000000 ompr-1.2.1/README.md
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:17:54.000000 ompr-1.2.1/ompr/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 19:28:36.000000 ompr-1.2.1/ompr/__init__.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      275 2023-03-05 12:31:56.000000 ompr-1.2.1/ompr/helpers.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)    24206 2023-03-27 15:59:25.000000 ompr-1.2.1/ompr/runner.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      784 2023-03-05 12:55:32.000000 ompr-1.2.1/ompr/simple.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:17:54.000000 ompr-1.2.1/ompr.egg-info/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      215 2023-05-05 19:17:54.000000 ompr-1.2.1/ompr.egg-info/PKG-INFO
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      220 2023-05-05 19:17:54.000000 ompr-1.2.1/ompr.egg-info/SOURCES.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        1 2023-05-05 19:17:54.000000 ompr-1.2.1/ompr.egg-info/dependency_links.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        6 2023-05-05 19:17:54.000000 ompr-1.2.1/ompr.egg-info/requires.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        5 2023-05-05 19:17:54.000000 ompr-1.2.1/ompr.egg-info/top_level.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       38 2023-05-05 19:17:54.000000 ompr-1.2.1/setup.cfg
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      637 2023-05-05 19:17:03.000000 ompr-1.2.1/setup.py
```

### Comparing `ompr-1.2.0/README.md` & `ompr-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ompr-1.2.0/ompr/runner.py` & `ompr-1.2.1/ompr/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,21 +74,27 @@
                         task_ix = ompr_msg.data['task_ix']
                         timeout = ompr_msg.data['task_timeout']
                         task = ompr_msg.data['task']
                         result = None
 
                         # try block for timeout exception
                         try:
-                            if timeout is not None: signal.alarm(timeout)
+
+                            if timeout is not None:
+                                signal.alarm(timeout)
 
                             # try block for process exceptions
-                            try:                   result = rwo.process(**task)
-                            except Exception as e: result = OMPRException(f'exception while processing task {task_ix}: {e}', task=task)
+                            try:
+                                result = rwo.process(**task)
+                            except Exception as e:
+                                result = OMPRException(f'exception while processing task {task_ix}: {e}', task=task)
+
+                            if timeout is not None:
+                                signal.alarm(0)
 
-                            if timeout is not None: signal.alarm(0)
                         except Exception as e:
                             result = OMPRException(f'exception while processing task {task_ix}: {e}', task=task)
 
                         finally:
                             self.oque.put(QMessage(
                                 type=   'exception' if type(result) is OMPRException else 'result',
                                 data=   {
```

### Comparing `ompr-1.2.0/ompr/simple.py` & `ompr-1.2.1/ompr/simple.py`

 * *Files identical despite different names*

### Comparing `ompr-1.2.0/setup.py` & `ompr-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('requirements.txt') as file:
         lines = [l[:-1] if l[-1]=='\n' else l for l in file.readlines()]
         return lines
 
 
 setup(
     name=               'ompr',
-    version=            'v1.2.0',
+    version=            'v1.2.1',
     url=                'https://github.com/piteren/ompr.git',
     author=             'Piotr Niewinski',
     author_email=       'pioniewinski@gmail.com',
     description=        'Object based Multi-Processing Runner',
     packages=           find_packages(),
     install_requires=   get_requirements(),
     license=            'MIT')
```

