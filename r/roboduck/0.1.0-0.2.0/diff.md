# Comparing `tmp/roboduck-0.1.0.tar.gz` & `tmp/roboduck-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/roboduck-0.1.0.tar", last modified: Fri Feb  3 03:48:15 2023, max compression
+gzip compressed data, was "roboduck-0.2.0.tar", last modified: Fri May  5 05:11:04 2023, max compression
```

## Comparing `roboduck-0.1.0.tar` & `roboduck-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,40 @@
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-02-03 03:48:15.000000 roboduck-0.1.0/
--rw-r--r--   0 hmamin     (501) staff       (20)       76 2023-02-03 03:45:08.000000 roboduck-0.1.0/MANIFEST.in
--rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-02-03 03:48:15.000000 roboduck-0.1.0/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)       65 2023-02-03 03:45:08.000000 roboduck-0.1.0/README.md
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-02-03 03:46:47.000000 roboduck-0.1.0/requirements.txt
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-02-03 03:48:15.000000 roboduck-0.1.0/roboduck/
--rw-r--r--   0 hmamin     (501) staff       (20)       21 2023-02-03 03:45:08.000000 roboduck-0.1.0/roboduck/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-02-03 03:45:08.000000 roboduck-0.1.0/roboduck/utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-02-03 03:48:15.000000 roboduck-0.1.0/roboduck.egg-info/
--rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-02-03 03:48:14.000000 roboduck-0.1.0/roboduck.egg-info/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)      214 2023-02-03 03:48:15.000000 roboduck-0.1.0/roboduck.egg-info/SOURCES.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-02-03 03:48:14.000000 roboduck-0.1.0/roboduck.egg-info/dependency_links.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-02-03 03:48:15.000000 roboduck-0.1.0/roboduck.egg-info/top_level.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-02-03 03:48:15.000000 roboduck-0.1.0/setup.cfg
--rw-r--r--   0 hmamin     (501) staff       (20)      760 2023-02-03 03:45:08.000000 roboduck-0.1.0/setup.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-05 05:11:04.461710 roboduck-0.2.0/
+-rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.2.0/MANIFEST.in
+-rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-05 05:11:04.461268 roboduck-0.2.0/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)     5067 2023-04-24 03:54:00.000000 roboduck-0.2.0/README.md
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.2.0/requirements.txt
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-05 05:11:04.448877 roboduck-0.2.0/roboduck/
+-rw-r--r--   0 hmamin     (501) staff       (20)      142 2023-05-05 05:10:58.000000 roboduck-0.2.0/roboduck/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-05 05:11:04.453055 roboduck-0.2.0/roboduck/cli/
+-rw-r--r--   0 hmamin     (501) staff       (20)     3215 2023-04-24 03:49:53.000000 roboduck-0.2.0/roboduck/cli/cli.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    18834 2023-05-05 05:05:39.000000 roboduck-0.2.0/roboduck/debug.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     9455 2023-05-03 05:16:00.000000 roboduck-0.2.0/roboduck/decorators.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     9434 2023-05-03 05:15:32.000000 roboduck-0.2.0/roboduck/errors.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     4841 2023-05-03 05:16:35.000000 roboduck-0.2.0/roboduck/ipy_utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-05 05:11:04.455187 roboduck-0.2.0/roboduck/langchain/
+-rw-r--r--   0 hmamin     (501) staff       (20)       79 2023-04-17 04:48:07.000000 roboduck-0.2.0/roboduck/langchain/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1441 2023-04-24 03:50:43.000000 roboduck-0.2.0/roboduck/langchain/callbacks.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    12385 2023-05-05 05:09:51.000000 roboduck-0.2.0/roboduck/langchain/chat.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     2363 2023-05-05 04:36:18.000000 roboduck-0.2.0/roboduck/langchain/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5021 2023-05-01 06:25:10.000000 roboduck-0.2.0/roboduck/logging.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5480 2023-05-01 06:27:21.000000 roboduck-0.2.0/roboduck/magic.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-05 05:11:04.456310 roboduck-0.2.0/roboduck/prompts/
+-rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.2.0/roboduck/prompts/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-05 05:11:04.460491 roboduck-0.2.0/roboduck/prompts/chat/
+-rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.2.0/roboduck/prompts/chat/__template__.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2131 2023-04-17 04:48:07.000000 roboduck-0.2.0/roboduck/prompts/chat/debug.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2178 2023-04-17 04:48:07.000000 roboduck-0.2.0/roboduck/prompts/chat/debug_full.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2106 2023-04-17 04:48:07.000000 roboduck-0.2.0/roboduck/prompts/chat/debug_full_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2075 2023-04-17 04:48:07.000000 roboduck-0.2.0/roboduck/prompts/chat/debug_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     3854 2023-04-30 05:33:59.000000 roboduck-0.2.0/roboduck/prompts/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1313 2023-03-17 02:32:03.000000 roboduck-0.2.0/roboduck/shell.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    12814 2023-05-03 05:15:32.000000 roboduck-0.2.0/roboduck/utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-05-05 05:11:04.452186 roboduck-0.2.0/roboduck.egg-info/
+-rw-r--r--   0 hmamin     (501) staff       (20)      196 2023-05-05 05:11:03.000000 roboduck-0.2.0/roboduck.egg-info/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)      817 2023-05-05 05:11:04.000000 roboduck-0.2.0/roboduck.egg-info/SOURCES.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-05-05 05:11:03.000000 roboduck-0.2.0/roboduck.egg-info/dependency_links.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-05-05 05:11:04.000000 roboduck-0.2.0/roboduck.egg-info/entry_points.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-05-05 05:11:04.000000 roboduck-0.2.0/roboduck.egg-info/requires.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-05-05 05:11:04.000000 roboduck-0.2.0/roboduck.egg-info/top_level.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-05-05 05:11:04.461862 roboduck-0.2.0/setup.cfg
+-rw-r--r--   0 hmamin     (501) staff       (20)      848 2023-04-30 05:56:13.000000 roboduck-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `roboduck-0.1.0/setup.py` & `roboduck-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,22 @@
     with open(path, 'r') as f:
         for row in f:
             if not row.startswith('__version__'):
                 continue
             return row.split(' = ')[-1].strip('\n').strip("'")
 
 
-setuptools.setup(name='roboduck',
-                 version=version(),
-                 author='Harrison Mamin',
-                 author_email='harrisonmamin@gmail.com',
-                 description='A natural language debugger.',
-                 install_requires=requirements(),
-                 packages=setuptools.find_packages())
+setuptools.setup(
+    name='roboduck',
+    version=version(),
+    author='Harrison Mamin',
+    author_email='harrisonmamin@gmail.com',
+    description='A natural language debugger.',
+    install_requires=requirements(),
+    packages=setuptools.find_packages(),
+    package_data={
+        'roboduck': ['**/*.yaml']
+    },
+    entry_points={'console_scripts': ['duck=roboduck.cli.cli:run']},
+    include_package_data=True
+)
```

