# Comparing `tmp/vsiew-2.0.1.tar.gz` & `tmp/vsiew-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsiew-2.0.1.tar", last modified: Fri Apr 14 16:07:31 2023, max compression
+gzip compressed data, was "vsiew-2.1.0.tar", last modified: Thu May  4 22:00:47 2023, max compression
```

## Comparing `vsiew-2.0.1.tar` & `vsiew-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:31.506685 vsiew-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-14 16:07:06.000000 vsiew-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-14 16:07:31.506685 vsiew-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-14 16:07:06.000000 vsiew-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:07:31.506685 vsiew-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-14 16:07:06.000000 vsiew-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:31.502685 vsiew-2.0.1/vsiew/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 16:07:06.000000 vsiew-2.0.1/vsiew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 16:07:06.000000 vsiew-2.0.1/vsiew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-14 16:07:06.000000 vsiew-2.0.1/vsiew/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-14 16:07:06.000000 vsiew-2.0.1/vsiew/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:07:31.506685 vsiew-2.0.1/vsiew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-14 16:07:31.000000 vsiew-2.0.1/vsiew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 16:07:31.000000 vsiew-2.0.1/vsiew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:07:31.000000 vsiew-2.0.1/vsiew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-14 16:07:31.000000 vsiew-2.0.1/vsiew.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-14 16:07:31.000000 vsiew-2.0.1/vsiew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 16:07:31.000000 vsiew-2.0.1/vsiew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:47.291335 vsiew-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 22:00:18.000000 vsiew-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-04 22:00:47.291335 vsiew-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-04 22:00:18.000000 vsiew-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 22:00:47.291335 vsiew-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-04 22:00:18.000000 vsiew-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:47.291335 vsiew-2.1.0/vsiew/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-04 22:00:18.000000 vsiew-2.1.0/vsiew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-04 22:00:18.000000 vsiew-2.1.0/vsiew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-04 22:00:18.000000 vsiew-2.1.0/vsiew/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-04 22:00:18.000000 vsiew-2.1.0/vsiew/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:00:47.291335 vsiew-2.1.0/vsiew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-04 22:00:47.000000 vsiew-2.1.0/vsiew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-04 22:00:47.000000 vsiew-2.1.0/vsiew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:00:47.000000 vsiew-2.1.0/vsiew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-04 22:00:47.000000 vsiew-2.1.0/vsiew.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-04 22:00:47.000000 vsiew-2.1.0/vsiew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 22:00:47.000000 vsiew-2.1.0/vsiew.egg-info/top_level.txt
```

### Comparing `vsiew-2.0.1/LICENSE` & `vsiew-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsiew-2.0.1/PKG-INFO` & `vsiew-2.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.0.1
+Version: 2.1.0
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

### Comparing `vsiew-2.0.1/setup.py` & `vsiew-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.0.1/vsiew/init.py` & `vsiew-2.1.0/vsiew/init.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,103 @@
 # Shrimply
 
+from typing import Iterator
+
 base_org = 'Irrational-Encoding-Wizardry'
 
 
-def update(latest_git: bool = False) -> None:
+def update(action: str) -> None:
     import sys
-    from subprocess import check_call
-    from http.client import HTTPSConnection
 
-    def _get_call(package: str, do_git: bool) -> int:
+    def _get_install_call(package: str, do_git: bool) -> int:
+        from subprocess import check_call
+
         args = list[str]()
 
         if do_git:
             package = f'git+https://github.com/{base_org}/{package}.git'
             args.extend(['--force', '--no-deps'])
 
         try:
-            return check_call([sys.executable, '-m', 'pip', 'install', package, '-U', '--no-cache-dir', *args])
+            return check_call([
+                sys.executable, '-m', 'pip', 'install',
+                package, '-U', '--no-cache-dir', *args
+            ])
+        except Exception:
+            return 1
+
+    def _get_uninstall_call(package: str) -> int:
+        from subprocess import check_call
+
+        try:
+            return check_call([
+                sys.executable, '-m', 'pip', 'uninstall', package
+            ])
         except Exception:
             return 1
 
-    if latest_git:
-        err = 0
+    def _get_iew_packages() -> Iterator[tuple[str, str]]:
+        from http.client import HTTPSConnection
 
         conn = HTTPSConnection('raw.githubusercontent.com', 443)
-        conn.request('GET', f'https://raw.githubusercontent.com/{base_org}/vs-iew/master/requirements.txt')
+        conn.request(
+            'GET', f'https://raw.githubusercontent.com/{base_org}'
+            '/vs-iew/master/requirements.txt'
+        )
 
         res = conn.getresponse()
 
-        packages = [line.decode('utf-8').strip() for line in res.readlines() if b'#' in line]
-
-        for package in packages:
-            *_, package = package.split('# ')
+        for line in res.readlines():
+            if b'#' in line:
+                line_s = line.decode('utf-8').strip()
+
+                *left, pypi_package = line_s.split('# ')
+                package = left[0].split('=')[0]
+
+                yield (package, pypi_package)
+
+    err = color = 0
+    message = default_message = 'No error message specified'
+
+    def _set_message(
+        message_succ: str = default_message, message_err: str = default_message
+    ) -> None:
+        nonlocal color, message, err
+        color = 31 if err else 32
+        message = (message_err if err else message_succ).format(err=err)
 
-            if _get_call(package, True):
-                err += 1
+    if action == 'update':
+        err = _get_install_call('vs-iew', True)
 
         if err:
-            color, message = 31, f'There was an error updating ({err}) IEW packages to latest git!'
-        else:
-            color, message = 32, 'Successfully updated all IEW packages to latest git!'
-    else:
-        err = _get_call('vs-iew', True)
+            err = _get_install_call('vsiew', False)
 
-        if err:
-            err = _get_call('vsiew')
+        _set_message(
+            'Successfully updated IEW packages!',
+            'There was an error updating IEW packages!'
+        )
+    elif action == 'update-git':
+        for _, name in _get_iew_packages():
+            if _get_install_call(name, True):
+                err += 1
 
-        if err:
-            color, message = 31, 'There was an error updating IEW packages!'
-        else:
-            color, message = 32, 'Successfully updated IEW packages!'
+        _set_message(
+            'Successfully updated all IEW packages to latest git!',
+            'There was an error updating ({err}) IEW packages to latest git!'
+        )
+    elif action == 'uninstall':
+        for name, _ in reversed(list(_get_iew_packages())):
+            if _get_uninstall_call(name):
+                err += 1
+
+        _set_message(
+            'Successfully uninstalled all IEW packages!',
+            'There was an error uninstalling ({err}) IEW packages!'
+        )
+    else:
+        err = 1
+        _set_message(message_err=f'There\'s no action called "{action}"!')
 
     if sys.stdout and sys.stdout.isatty():
         message = f'\033[0;{color};1m{message}\033[0m'
 
     print(f'\n\t{message}\n')
```

### Comparing `vsiew-2.0.1/vsiew.egg-info/PKG-INFO` & `vsiew-2.1.0/vsiew.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.0.1
+Version: 2.1.0
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

