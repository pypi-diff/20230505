# Comparing `tmp/ansible-anonymizer-1.2.1.tar.gz` & `tmp/ansible-anonymizer-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-anonymizer-1.2.1.tar", last modified: Fri May  5 17:35:31 2023, max compression
+gzip compressed data, was "ansible-anonymizer-1.2.2.tar", last modified: Fri May  5 20:19:47 2023, max compression
```

## Comparing `ansible-anonymizer-1.2.1.tar` & `ansible-anonymizer-1.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:35:31.017164 ansible-anonymizer-1.2.1/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      292 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.1/.editorconfig
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:35:31.015164 ansible-anonymizer-1.2.1/.github/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      321 2023-03-23 15:13:37.000000 ansible-anonymizer-1.2.1/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:35:31.015164 ansible-anonymizer-1.2.1/.github/workflows/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      551 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.1/.github/workflows/tox.yml
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1204 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.1/.gitignore
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1138 2023-04-05 13:57:02.000000 ansible-anonymizer-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1418 2023-05-05 17:33:32.000000 ansible-anonymizer-1.2.1/CHANGELOG.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2478 2023-03-23 15:13:37.000000 ansible-anonymizer-1.2.1/CONTRIBUTING.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)       63 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.1/HISTORY.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)      588 2023-03-22 17:41:29.000000 ansible-anonymizer-1.2.1/LICENSE
--rw-r--r--   0 goneri    (1002) goneri    (1002)      168 2023-04-05 18:22:37.000000 ansible-anonymizer-1.2.1/MANIFEST.in
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-05 17:35:31.017164 ansible-anonymizer-1.2.1/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1227 2023-05-05 17:28:31.000000 ansible-anonymizer-1.2.1/README.rst
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:35:31.016164 ansible-anonymizer-1.2.1/ansible_anonymizer/
--rw-r--r--   0 goneri    (1002) goneri    (1002)       90 2023-05-05 17:33:47.000000 ansible-anonymizer-1.2.1/ansible_anonymizer/__init__.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     9368 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.1/ansible_anonymizer/anonymizer.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      716 2023-05-01 21:51:04.000000 ansible-anonymizer-1.2.1/ansible_anonymizer/cli.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1914 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.1/ansible_anonymizer/field_checks.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      294 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.1/ansible_anonymizer/jinja2.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)    11387 2023-05-05 17:32:31.000000 ansible-anonymizer-1.2.1/ansible_anonymizer/parser.py
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:35:31.017164 ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-05 17:35:30.000000 ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)      659 2023-05-05 17:35:31.000000 ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/SOURCES.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2023-05-05 17:35:30.000000 ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/dependency_links.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2023-05-05 17:35:30.000000 ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/entry_points.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       12 2023-05-05 17:35:30.000000 ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/requires.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       19 2023-05-05 17:35:30.000000 ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/top_level.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1551 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.1/pyproject.toml
--rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2023-05-05 17:35:31.017164 ansible-anonymizer-1.2.1/setup.cfg
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:35:31.017164 ansible-anonymizer-1.2.1/tests/
--rw-r--r--   0 goneri    (1002) goneri    (1002)    17496 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.1/tests/test_anonymizer.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1286 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.1/tox.ini
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 20:19:47.128850 ansible-anonymizer-1.2.2/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      292 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.2/.editorconfig
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 20:19:47.126850 ansible-anonymizer-1.2.2/.github/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      321 2023-03-23 15:13:37.000000 ansible-anonymizer-1.2.2/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 20:19:47.126850 ansible-anonymizer-1.2.2/.github/workflows/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      551 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.2/.github/workflows/tox.yml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1204 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.2/.gitignore
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1138 2023-04-05 13:57:02.000000 ansible-anonymizer-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1486 2023-05-05 20:19:19.000000 ansible-anonymizer-1.2.2/CHANGELOG.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     2478 2023-03-23 15:13:37.000000 ansible-anonymizer-1.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       63 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.2/HISTORY.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      588 2023-03-22 17:41:29.000000 ansible-anonymizer-1.2.2/LICENSE
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      168 2023-04-05 18:22:37.000000 ansible-anonymizer-1.2.2/MANIFEST.in
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-05 20:19:47.128850 ansible-anonymizer-1.2.2/PKG-INFO
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1227 2023-05-05 17:28:31.000000 ansible-anonymizer-1.2.2/README.rst
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 20:19:47.127850 ansible-anonymizer-1.2.2/ansible_anonymizer/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       90 2023-05-05 20:19:19.000000 ansible-anonymizer-1.2.2/ansible_anonymizer/__init__.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     9368 2023-05-05 20:11:23.000000 ansible-anonymizer-1.2.2/ansible_anonymizer/anonymizer.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      716 2023-05-05 20:11:23.000000 ansible-anonymizer-1.2.2/ansible_anonymizer/cli.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1914 2023-05-05 20:19:14.000000 ansible-anonymizer-1.2.2/ansible_anonymizer/field_checks.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      294 2023-05-05 20:19:14.000000 ansible-anonymizer-1.2.2/ansible_anonymizer/jinja2.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    11471 2023-05-05 20:19:19.000000 ansible-anonymizer-1.2.2/ansible_anonymizer/parser.py
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 20:19:47.128850 ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-05 20:19:47.000000 ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/PKG-INFO
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      659 2023-05-05 20:19:47.000000 ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/SOURCES.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2023-05-05 20:19:47.000000 ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/dependency_links.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2023-05-05 20:19:47.000000 ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/entry_points.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       12 2023-05-05 20:19:47.000000 ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/requires.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       19 2023-05-05 20:19:47.000000 ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/top_level.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1551 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.2/pyproject.toml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2023-05-05 20:19:47.128850 ansible-anonymizer-1.2.2/setup.cfg
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 20:19:47.128850 ansible-anonymizer-1.2.2/tests/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    17930 2023-05-05 20:19:19.000000 ansible-anonymizer-1.2.2/tests/test_anonymizer.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1286 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.2/tox.ini
```

### Comparing `ansible-anonymizer-1.2.1/.github/workflows/tox.yml` & `ansible-anonymizer-1.2.2/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.1/.gitignore` & `ansible-anonymizer-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.1/.pre-commit-config.yaml` & `ansible-anonymizer-1.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.1/CHANGELOG.rst` & `ansible-anonymizer-1.2.2/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 1.2.2 (2023-05-05)
+
+- adjustment to handle aws/credentials
+
 Version 1.2.1 (2023-05-05)
 -------------
 
 - clean up some debug traces
 
 Version 1.2.0 (2023-05-05)
 -------------
```

### Comparing `ansible-anonymizer-1.2.1/CONTRIBUTING.rst` & `ansible-anonymizer-1.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.1/LICENSE` & `ansible-anonymizer-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.1/PKG-INFO` & `ansible-anonymizer-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-anonymizer
-Version: 1.2.1
+Version: 1.2.2
 Summary: Ansible Anonymizer
 Author-email: Gonéri Le Bouder <goneri@lebouder.net>
 Project-URL: Homepage, https://github.com/ansible/anonymizer
 Keywords: pii,anonymize
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `ansible-anonymizer-1.2.1/README.rst` & `ansible-anonymizer-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.1/ansible_anonymizer/anonymizer.py` & `ansible-anonymizer-1.2.2/ansible_anonymizer/anonymizer.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.1/ansible_anonymizer/cli.py` & `ansible-anonymizer-1.2.2/ansible_anonymizer/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.1/ansible_anonymizer/field_checks.py` & `ansible-anonymizer-1.2.2/ansible_anonymizer/field_checks.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.1/ansible_anonymizer/parser.py` & `ansible-anonymizer-1.2.2/ansible_anonymizer/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 from collections.abc import Generator
 from enum import Enum
 from typing import Literal, Optional, Union
 
-from ansible_anonymizer.field_checks import is_password_field_name, is_path
+from ansible_anonymizer.field_checks import is_password_field_name
 from ansible_anonymizer.jinja2 import str_jinja2_variable_name
 
 """Parser for YAML-like structure that tolerate error."""
 
 quote_t = Literal['"', "'"]
 
 
@@ -242,41 +242,44 @@
         current_node = current_node.next
 
 
 def combinate_value_fields(root_node: Node) -> None:
     """
     Merge the unquoted value fields.
 
-    In YAML, a value can be an unprotected string with spaces. Internally
-    the parser represent such series of spaces and fields as different
-    Node objects. Since all these objects are actually one single value,
-    we merge them together.
+    In YAML or INI, a value can be an unprotected string with spaces.
+    Internally     the parser represent such series of spaces and fields
+    as different Node objects. Since all these objects are actually one
+    single value, we merge them together.
     """
     current_node = root_node
     mergable_types = [NodeType.space, NodeType.field, NodeType.unknown]
     post_sep = False
     while current_node:
         if post_sep:
             # We ignore the first space after the : sign
             if current_node.type is NodeType.space and current_node.next:
                 current_node = current_node.next
 
             while (
                 current_node.type in mergable_types
+                and not current_node.is_password_field_name()
                 and current_node.next
                 and current_node.next.type in mergable_types
                 and not current_node.next.is_password_field_name()
             ):
                 current_node.type = NodeType.unknown
                 current_node.text += current_node.next.text
+                current_node.next.type = NodeType.deleted
+                current_node.next.text = "KILLED"
                 current_node.next = current_node.next.next
                 if current_node.next:
                     current_node.next.previous = current_node
 
-        elif current_node.type is NodeType.separator and current_node.text == ":":
+        elif current_node.type is NodeType.separator:
             post_sep = True
         if current_node.next is None:
             break
         current_node = current_node.next
 
 
 def print_node(root_node: Node) -> None:
@@ -317,14 +320,12 @@
             continue
         if not node.is_password_field_name():
             continue
 
         secret_node = node.get_secret()
         if not secret_node:
             continue
-        if is_path(secret_node.text):
-            continue
 
         if secret_node.type is NodeType.quoted_string_holder:
             return hide_quoted_string(node, secret_node)
         else:
             return hide_regular_field(node, secret_node)
```

### Comparing `ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/PKG-INFO` & `ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-anonymizer
-Version: 1.2.1
+Version: 1.2.2
 Summary: Ansible Anonymizer
 Author-email: Gonéri Le Bouder <goneri@lebouder.net>
 Project-URL: Homepage, https://github.com/ansible/anonymizer
 Keywords: pii,anonymize
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `ansible-anonymizer-1.2.1/ansible_anonymizer.egg-info/SOURCES.txt` & `ansible-anonymizer-1.2.2/ansible_anonymizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.1/pyproject.toml` & `ansible-anonymizer-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.2.1/tests/test_anonymizer.py` & `ansible-anonymizer-1.2.2/tests/test_anonymizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 
         - name: some example
             a-broken-key:
                 my-secret: "{{ my_secret }}"
                 @^my-secret: "{{ my_secret }}"
                 %@iÜ-secret: "{{ secret }}"
                 quoted-secret: '{{ quoted_secret }}'
-                private_key: ~/.ssh/id_rsa
+                private_key: "{{ private_key }}"
 
     """
     assert anonymize_text_block(source) == expectation
     assert hide_secrets(source) == expectation
 
 
 def test_anonymize_text_block_email_addresses():
@@ -620,7 +620,22 @@
     passwd: "{{ passwd }}"
     """
     assert hide_secrets(origin) == expectation
 
 
 def test_str_jinja2_variable_name_leading_underscore():
     assert str_jinja2_variable_name("-foo-BAR") == "foo_bar"
+
+
+def test_hide_secrets_aws_profile():
+    origin = """
+    [my-secret-account]
+    aws_access_key_id = BJIA5UUFYYOOKZQODC3F
+    aws_secret_access_key = NeTL/2vPPnlnb/8RBtsw3EwnNjflDbgZiDmRskhb
+    """
+
+    expectation = """
+    [my-secret-account]
+    aws_access_key_id = "{{ aws_access_key_id }}"
+    aws_secret_access_key = "{{ aws_secret_access_key }}"
+    """
+    assert hide_secrets(dedent(origin)) == dedent(expectation)
```

### Comparing `ansible-anonymizer-1.2.1/tox.ini` & `ansible-anonymizer-1.2.2/tox.ini`

 * *Files identical despite different names*

