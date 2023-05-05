# Comparing `tmp/ansible-anonymizer-1.2.0.tar.gz` & `tmp/ansible-anonymizer-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-anonymizer-1.2.0.tar", last modified: Fri May  5 17:29:54 2023, max compression
+gzip compressed data, was "ansible-anonymizer-1.2.1.tar", last modified: Fri May  5 17:35:31 2023, max compression
```

## Comparing `ansible-anonymizer-1.2.0.tar` & `ansible-anonymizer-1.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:29:54.500297 ansible-anonymizer-1.2.0/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      292 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.0/.editorconfig
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:29:54.499297 ansible-anonymizer-1.2.0/.github/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      321 2023-03-23 15:13:37.000000 ansible-anonymizer-1.2.0/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:29:54.499297 ansible-anonymizer-1.2.0/.github/workflows/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      551 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.0/.github/workflows/tox.yml
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1204 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.0/.gitignore
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1138 2023-04-05 13:57:02.000000 ansible-anonymizer-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1346 2023-05-05 17:10:20.000000 ansible-anonymizer-1.2.0/CHANGELOG.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2478 2023-03-23 15:13:37.000000 ansible-anonymizer-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)       63 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.0/HISTORY.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)      588 2023-03-22 17:41:29.000000 ansible-anonymizer-1.2.0/LICENSE
--rw-r--r--   0 goneri    (1002) goneri    (1002)      168 2023-04-05 18:22:37.000000 ansible-anonymizer-1.2.0/MANIFEST.in
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-05 17:29:54.500297 ansible-anonymizer-1.2.0/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1227 2023-05-05 17:28:31.000000 ansible-anonymizer-1.2.0/README.rst
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:29:54.499297 ansible-anonymizer-1.2.0/ansible_anonymizer/
--rw-r--r--   0 goneri    (1002) goneri    (1002)       90 2023-05-05 17:08:57.000000 ansible-anonymizer-1.2.0/ansible_anonymizer/__init__.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     9368 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.0/ansible_anonymizer/anonymizer.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      716 2023-05-01 21:51:04.000000 ansible-anonymizer-1.2.0/ansible_anonymizer/cli.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1914 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.0/ansible_anonymizer/field_checks.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      294 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.0/ansible_anonymizer/jinja2.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)    11525 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.0/ansible_anonymizer/parser.py
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:29:54.500297 ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-05 17:29:54.000000 ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)      659 2023-05-05 17:29:54.000000 ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/SOURCES.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2023-05-05 17:29:54.000000 ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/dependency_links.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2023-05-05 17:29:54.000000 ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/entry_points.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       12 2023-05-05 17:29:54.000000 ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/requires.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       19 2023-05-05 17:29:54.000000 ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/top_level.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1551 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.0/pyproject.toml
--rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2023-05-05 17:29:54.501297 ansible-anonymizer-1.2.0/setup.cfg
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:29:54.500297 ansible-anonymizer-1.2.0/tests/
--rw-r--r--   0 goneri    (1002) goneri    (1002)    17496 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.0/tests/test_anonymizer.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1286 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.0/tox.ini
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:35:31.017164 ansible-anonymizer-1.2.1/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      292 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.1/.editorconfig
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:35:31.015164 ansible-anonymizer-1.2.1/.github/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      321 2023-03-23 15:13:37.000000 ansible-anonymizer-1.2.1/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:35:31.015164 ansible-anonymizer-1.2.1/.github/workflows/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      551 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.1/.github/workflows/tox.yml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1204 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.1/.gitignore
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1138 2023-04-05 13:57:02.000000 ansible-anonymizer-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1418 2023-05-05 17:33:32.000000 ansible-anonymizer-1.2.1/CHANGELOG.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     2478 2023-03-23 15:13:37.000000 ansible-anonymizer-1.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       63 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.1/HISTORY.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      588 2023-03-22 17:41:29.000000 ansible-anonymizer-1.2.1/LICENSE
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      168 2023-04-05 18:22:37.000000 ansible-anonymizer-1.2.1/MANIFEST.in
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-05 17:35:31.017164 ansible-anonymizer-1.2.1/PKG-INFO
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1227 2023-05-05 17:28:31.000000 ansible-anonymizer-1.2.1/README.rst
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:35:31.016164 ansible-anonymizer-1.2.1/ansible_anonymizer/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       90 2023-05-05 17:33:47.000000 ansible-anonymizer-1.2.1/ansible_anonymizer/__init__.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     9368 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.1/ansible_anonymizer/anonymizer.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      716 2023-05-01 21:51:04.000000 ansible-anonymizer-1.2.1/ansible_anonymizer/cli.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1914 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.1/ansible_anonymizer/field_checks.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      294 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.1/ansible_anonymizer/jinja2.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    11387 2023-05-05 17:32:31.000000 ansible-anonymizer-1.2.1/ansible_anonymizer/parser.py
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:35:31.017164 ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-05 17:35:30.000000 ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/PKG-INFO
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      659 2023-05-05 17:35:31.000000 ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/SOURCES.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2023-05-05 17:35:30.000000 ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/dependency_links.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2023-05-05 17:35:30.000000 ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/entry_points.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       12 2023-05-05 17:35:30.000000 ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/requires.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       19 2023-05-05 17:35:30.000000 ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/top_level.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1551 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.1/pyproject.toml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2023-05-05 17:35:31.017164 ansible-anonymizer-1.2.1/setup.cfg
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:35:31.017164 ansible-anonymizer-1.2.1/tests/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    17496 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.1/tests/test_anonymizer.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1286 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.1/tox.ini
```

### Comparing `ansible-anonymizer-1.2.0/.github/workflows/tox.yml` & `ansible-anonymizer-1.2.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.0/.gitignore` & `ansible-anonymizer-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.0/.pre-commit-config.yaml` & `ansible-anonymizer-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.0/CHANGELOG.rst` & `ansible-anonymizer-1.2.1/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+Version 1.2.1 (2023-05-05)
+-------------
+
+- clean up some debug traces
+
 Version 1.2.0 (2023-05-05)
 -------------
 
 - hide_secrets: better management of the quotes (#41)
 - tox: skip_install=True with mypy
 - tox: test using ruff
 - pyproject: configure ruff and reformat the code base
```

### Comparing `ansible-anonymizer-1.2.0/CONTRIBUTING.rst` & `ansible-anonymizer-1.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.0/LICENSE` & `ansible-anonymizer-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.0/PKG-INFO` & `ansible-anonymizer-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-anonymizer
-Version: 1.2.0
+Version: 1.2.1
 Summary: Ansible Anonymizer
 Author-email: Gonéri Le Bouder <goneri@lebouder.net>
 Project-URL: Homepage, https://github.com/ansible/anonymizer
 Keywords: pii,anonymize
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `ansible-anonymizer-1.2.0/README.rst` & `ansible-anonymizer-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.0/ansible_anonymizer/anonymizer.py` & `ansible-anonymizer-1.2.1/ansible_anonymizer/anonymizer.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.0/ansible_anonymizer/cli.py` & `ansible-anonymizer-1.2.1/ansible_anonymizer/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.0/ansible_anonymizer/field_checks.py` & `ansible-anonymizer-1.2.1/ansible_anonymizer/field_checks.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.0/ansible_anonymizer/parser.py` & `ansible-anonymizer-1.2.1/ansible_anonymizer/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,15 @@
                 break
             holder = holder.previous
 
     def get_secret(self) -> Union["Node", None]:
         """Identify the secret Node associated with the current Node."""
         candidate = self.next
         has_separator = False
-        print(f"FIELD={self.text}")
         while candidate:
-            print(f"CANDIDATE: {candidate.text} ({candidate.type})")
             if candidate.type is NodeType.space:
                 pass
             elif candidate.type is NodeType.quoted_string_closing:
                 if candidate.holder is not self.holder:
                     raise ParserError()
             elif has_separator:
                 if candidate.type is NodeType.securized:
@@ -84,15 +82,14 @@
                     return candidate
                 if candidate.type is NodeType.quoted_string_holder:
                     return candidate
                 else:
                     return None
             elif candidate.type is NodeType.separator:
                 has_separator = True
-                print("HAS SEP")
             else:
                 return None
             candidate = candidate.next
         return None
 
     def is_password_field_name(self) -> bool:
         """Return True if the field name matches the DENYLIST_REGEX regex."""
```

### Comparing `ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/PKG-INFO` & `ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-anonymizer
-Version: 1.2.0
+Version: 1.2.1
 Summary: Ansible Anonymizer
 Author-email: Gonéri Le Bouder <goneri@lebouder.net>
 Project-URL: Homepage, https://github.com/ansible/anonymizer
 Keywords: pii,anonymize
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/SOURCES.txt` & `ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.0/pyproject.toml` & `ansible-anonymizer-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.0/tests/test_anonymizer.py` & `ansible-anonymizer-1.2.1/tests/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.0/tox.ini` & `ansible-anonymizer-1.2.1/tox.ini`

 * *Files identical despite different names*

