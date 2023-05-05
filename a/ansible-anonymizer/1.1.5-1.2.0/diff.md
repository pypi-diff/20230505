# Comparing `tmp/ansible-anonymizer-1.1.5.tar.gz` & `tmp/ansible-anonymizer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-anonymizer-1.1.5.tar", last modified: Tue Apr 11 19:09:33 2023, max compression
+gzip compressed data, was "ansible-anonymizer-1.2.0.tar", last modified: Fri May  5 17:29:54 2023, max compression
```

## Comparing `ansible-anonymizer-1.1.5.tar` & `ansible-anonymizer-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-11 19:09:33.825930 ansible-anonymizer-1.1.5/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      292 2023-03-10 14:59:31.000000 ansible-anonymizer-1.1.5/.editorconfig
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-11 19:09:33.823930 ansible-anonymizer-1.1.5/.github/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      321 2023-03-23 15:13:37.000000 ansible-anonymizer-1.1.5/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-11 19:09:33.823930 ansible-anonymizer-1.1.5/.github/workflows/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      551 2023-03-10 14:59:31.000000 ansible-anonymizer-1.1.5/.github/workflows/tox.yml
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1204 2023-03-10 14:59:31.000000 ansible-anonymizer-1.1.5/.gitignore
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1138 2023-04-05 13:57:02.000000 ansible-anonymizer-1.1.5/.pre-commit-config.yaml
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1094 2023-04-11 19:06:03.000000 ansible-anonymizer-1.1.5/CHANGELOG.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2478 2023-03-23 15:13:37.000000 ansible-anonymizer-1.1.5/CONTRIBUTING.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)       63 2023-03-10 14:59:31.000000 ansible-anonymizer-1.1.5/HISTORY.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)      588 2023-03-22 17:41:29.000000 ansible-anonymizer-1.1.5/LICENSE
--rw-r--r--   0 goneri    (1002) goneri    (1002)      168 2023-04-05 18:22:37.000000 ansible-anonymizer-1.1.5/MANIFEST.in
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1554 2023-04-11 19:09:33.825930 ansible-anonymizer-1.1.5/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1110 2023-04-05 13:57:47.000000 ansible-anonymizer-1.1.5/README.rst
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-11 19:09:33.823930 ansible-anonymizer-1.1.5/ansible_anonymizer/
--rw-r--r--   0 goneri    (1002) goneri    (1002)       90 2023-04-11 19:06:13.000000 ansible-anonymizer-1.1.5/ansible_anonymizer/__init__.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)    11527 2023-04-11 17:36:53.000000 ansible-anonymizer-1.1.5/ansible_anonymizer/anonymizer.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      757 2023-04-11 19:05:08.000000 ansible-anonymizer-1.1.5/ansible_anonymizer/cli.py
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-11 19:09:33.824930 ansible-anonymizer-1.1.5/ansible_anonymizer.egg-info/
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1554 2023-04-11 19:09:33.000000 ansible-anonymizer-1.1.5/ansible_anonymizer.egg-info/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)      566 2023-04-11 19:09:33.000000 ansible-anonymizer-1.1.5/ansible_anonymizer.egg-info/SOURCES.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2023-04-11 19:09:33.000000 ansible-anonymizer-1.1.5/ansible_anonymizer.egg-info/dependency_links.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2023-04-11 19:09:33.000000 ansible-anonymizer-1.1.5/ansible_anonymizer.egg-info/entry_points.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       12 2023-04-11 19:09:33.000000 ansible-anonymizer-1.1.5/ansible_anonymizer.egg-info/requires.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       19 2023-04-11 19:09:33.000000 ansible-anonymizer-1.1.5/ansible_anonymizer.egg-info/top_level.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)      910 2023-03-31 17:38:17.000000 ansible-anonymizer-1.1.5/pyproject.toml
--rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2023-04-11 19:09:33.825930 ansible-anonymizer-1.1.5/setup.cfg
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-11 19:09:33.824930 ansible-anonymizer-1.1.5/tests/
--rw-r--r--   0 goneri    (1002) goneri    (1002)    13291 2023-04-11 18:01:34.000000 ansible-anonymizer-1.1.5/tests/test_anonymizer.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1155 2023-04-05 13:57:03.000000 ansible-anonymizer-1.1.5/tox.ini
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:29:54.500297 ansible-anonymizer-1.2.0/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      292 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.0/.editorconfig
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:29:54.499297 ansible-anonymizer-1.2.0/.github/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      321 2023-03-23 15:13:37.000000 ansible-anonymizer-1.2.0/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:29:54.499297 ansible-anonymizer-1.2.0/.github/workflows/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      551 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.0/.github/workflows/tox.yml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1204 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.0/.gitignore
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1138 2023-04-05 13:57:02.000000 ansible-anonymizer-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1346 2023-05-05 17:10:20.000000 ansible-anonymizer-1.2.0/CHANGELOG.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     2478 2023-03-23 15:13:37.000000 ansible-anonymizer-1.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       63 2023-03-10 14:59:31.000000 ansible-anonymizer-1.2.0/HISTORY.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      588 2023-03-22 17:41:29.000000 ansible-anonymizer-1.2.0/LICENSE
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      168 2023-04-05 18:22:37.000000 ansible-anonymizer-1.2.0/MANIFEST.in
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-05 17:29:54.500297 ansible-anonymizer-1.2.0/PKG-INFO
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1227 2023-05-05 17:28:31.000000 ansible-anonymizer-1.2.0/README.rst
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:29:54.499297 ansible-anonymizer-1.2.0/ansible_anonymizer/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       90 2023-05-05 17:08:57.000000 ansible-anonymizer-1.2.0/ansible_anonymizer/__init__.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     9368 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.0/ansible_anonymizer/anonymizer.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      716 2023-05-01 21:51:04.000000 ansible-anonymizer-1.2.0/ansible_anonymizer/cli.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1914 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.0/ansible_anonymizer/field_checks.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      294 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.0/ansible_anonymizer/jinja2.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    11525 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.0/ansible_anonymizer/parser.py
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:29:54.500297 ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1671 2023-05-05 17:29:54.000000 ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/PKG-INFO
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      659 2023-05-05 17:29:54.000000 ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/SOURCES.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2023-05-05 17:29:54.000000 ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/dependency_links.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2023-05-05 17:29:54.000000 ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/entry_points.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       12 2023-05-05 17:29:54.000000 ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/requires.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       19 2023-05-05 17:29:54.000000 ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/top_level.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1551 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.0/pyproject.toml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2023-05-05 17:29:54.501297 ansible-anonymizer-1.2.0/setup.cfg
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-05-05 17:29:54.500297 ansible-anonymizer-1.2.0/tests/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    17496 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.0/tests/test_anonymizer.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1286 2023-05-05 16:59:24.000000 ansible-anonymizer-1.2.0/tox.ini
```

### Comparing `ansible-anonymizer-1.1.5/.github/workflows/tox.yml` & `ansible-anonymizer-1.2.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.1.5/.gitignore` & `ansible-anonymizer-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.1.5/.pre-commit-config.yaml` & `ansible-anonymizer-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.1.5/CONTRIBUTING.rst` & `ansible-anonymizer-1.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.1.5/LICENSE` & `ansible-anonymizer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.1.5/PKG-INFO` & `ansible-anonymizer-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-anonymizer
-Version: 1.1.5
+Version: 1.2.0
 Summary: Ansible Anonymizer
 Author-email: Gonéri Le Bouder <goneri@lebouder.net>
 Project-URL: Homepage, https://github.com/ansible/anonymizer
 Keywords: pii,anonymize
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -51,7 +51,13 @@
    >>> some_text = """
    ... - name: a task
    ...   a_module:
    ...     secret: foobar
    ... """
    >>> anonymizer.anonymize_text_block(some_text)
    '\n- name: a task\n  a_module:\n    secret: {{ }}\n'
+
+You can also use the ``ansible-anonymizer`` command:
+
+.. code-block:: console
+
+   ansible-anonymizer my-secret-file
```

### Comparing `ansible-anonymizer-1.1.5/README.rst` & `ansible-anonymizer-1.2.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -37,7 +37,13 @@
    >>> some_text = """
    ... - name: a task
    ...   a_module:
    ...     secret: foobar
    ... """
    >>> anonymizer.anonymize_text_block(some_text)
    '\n- name: a task\n  a_module:\n    secret: {{ }}\n'
+
+You can also use the ``ansible-anonymizer`` command:
+
+.. code-block:: console
+
+   ansible-anonymizer my-secret-file
```

### Comparing `ansible-anonymizer-1.1.5/ansible_anonymizer/anonymizer.py` & `ansible-anonymizer-1.2.0/ansible_anonymizer/anonymizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,27 @@
 #!/usr/bin/env python3
 # pylint: disable=missing-module-docstring
 # pylint: disable=missing-function-docstring
 # pylint: disable=invalid-name
 import ipaddress
 import re
-from ipaddress import IPv4Address
-from ipaddress import IPv6Address
-from typing import Any
-from typing import Callable
-from typing import Generator
-from typing import Match
-from typing import Union
+from collections.abc import Generator
+from ipaddress import IPv4Address, IPv6Address
+from re import Match
+from typing import Any, Callable, Union
 from zlib import crc32
 
-# Denylist regex to TC of secrets filter
-# From detect_secrets.plugins (Apache v2 License)
-DENYLIST = (
-    "api_?key",
-    "auth_?key",
-    "service_?key",
-    "account_?key",
-    "db_?key",
-    "database_?key",
-    "priv_?key",
-    "private_?key",
-    "client_?key",
-    r"host\w*_key",
-    "db_?pass",
-    "database_?pass",
-    "key_?pass",
-    "key_?data",
-    "key_?name",
-    "password",
-    "passwd",
-    "pass",
-    "pwd",
-    "secret",
-    "contraseña",
-    "contrasena",
-    "access_key",
+from ansible_anonymizer.field_checks import (
+    is_jinja2_expression,
+    is_password_field_name,
+    is_path,
+    is_uuid_string,
 )
-AFFIX_REGEX = r"\w*"
-DENYLIST_REGEX = r"|".join(DENYLIST)
-# Support for suffix after keyword i.e. password_secure = "value"
-DENYLIST_REGEX_WITH_PREFIX = fr"({DENYLIST_REGEX}){AFFIX_REGEX}"
-
-
-def str_jinja2_variable_name(name: str) -> str:
-    """Sanitize a string to make it suitable to become a Jinja2 variable."""
-    name = name.replace("-", "_")
-    name = re.sub(r'[^a-z_]', '', name, flags=re.IGNORECASE)
-    return name
+from ansible_anonymizer.jinja2 import str_jinja2_variable_name
+from ansible_anonymizer.parser import hide_secrets
 
 
 def gen_email_address(original: Match[str]) -> str:
     samples = [
         "liam",
         "olivia",
         "noah",
@@ -72,44 +39,19 @@
         "lucas",
         "mia",
         "henry",
         "evelyn",
         "theodore",
         "harper",
     ]
-    idx = crc32(original.group('email').encode()) % len(samples)
+    idx = crc32(original.group("email").encode()) % len(samples)
     name = samples[idx]
     return f"{name}{idx}@example.com"
 
 
-def is_password_field_name(name: str) -> bool:
-    flags = re.MULTILINE | re.IGNORECASE
-    return re.search(DENYLIST_REGEX_WITH_PREFIX, name, flags=flags) is not None
-
-
-def is_jinja2_expression(value: str) -> bool:
-    """Check if an unquoted string hold a Jinja2 variable"""
-    if re.match(r"^\s*{{\s*.*?\s*}}\s*$", value):
-        return True
-
-    return False
-
-
-def is_uuid_string(value: str) -> bool:
-    """Check if a given value is a UUID string"""
-    if re.match(
-        r"^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$",
-        value,
-        flags=re.IGNORECASE,
-    ):
-        return True
-
-    return False
-
-
 common_ipv4_networks = [
     ipaddress.IPv4Network("1.0.0.1/32"),
     ipaddress.IPv4Network("1.1.1.1/32"),
     ipaddress.IPv4Network("149.112.112.112/32"),
     ipaddress.IPv4Network("208.67.220.220/32"),
     ipaddress.IPv4Network("208.67.222.222/32"),
     ipaddress.IPv4Network("76.223.122.150/32"),
@@ -186,22 +128,14 @@
         if is_jinja2_expression(unquote(v)):
             return unquote(v)
         variable_name = str_jinja2_variable_name(name)
         return f"{{{{ { variable_name } }}}}"
     return anonymize_text_block(value)
 
 
-def is_path(content: str) -> bool:
-    # Rather conservative on purpose to avoid a false
-    # positive
-    if "/" not in content:
-        return False
-    return bool(re.match(r"^(|~)[a-z0-9_/\.-]+$", content, flags=re.IGNORECASE))
-
-
 def anonymize_struct(o: Any, key_name: str = "") -> Any:
     def key_name_str(k: Any) -> str:
         return k if isinstance(k, str) else ""
 
     if key_name and not isinstance(key_name, str):
         key_name = str(key_name)
 
@@ -211,50 +145,32 @@
         return [anonymize_struct(v, key_name=key_name) for v in o]
     if isinstance(o, str):
         return anonymize_field(o, key_name)
     return o
 
 
 def anonymize(o: Any, key_name: str = "") -> Any:
-    """Deprecated: use anonymize_struct() instead"""
+    """Deprecated: use anonymize_struct() instead."""
     return anonymize_struct(o, key_name=key_name)
 
 
-def hide_secrets(block: str) -> str:
-    flags = re.MULTILINE | re.IGNORECASE
-
-    def _rewrite(m: re.Match[str]) -> str:
-        value = m.group('value')
-        if is_path(value):
-            return m.group(0)
-        field = m.group('field')
-        return f"{field}: \"{anonymize_field(value, field)}\""
-
-    return re.sub(
-        fr"(?P<field>(|\S+){DENYLIST_REGEX_WITH_PREFIX}):\s*(?P<value>.*)",
-        _rewrite,
-        block,
-        flags=flags,
-    )
-
-
 def hide_emails(block: str) -> str:
     flags = re.MULTILINE | re.DOTALL | re.IGNORECASE
     email_re = r"\b\S+@[a-z\.]+[a-z]{2,}\b"
     return re.sub(fr"(?P<email>{email_re})", gen_email_address, block, flags=flags)
 
 
 def hide_ip_addresses(block: str) -> str:
     flags = re.MULTILINE | re.DOTALL | re.IGNORECASE
 
     def _rewrite(m: re.Match[str]) -> str:
         try:
-            ip = ipaddress.ip_address(m.group('ip_address'))
+            ip = ipaddress.ip_address(m.group("ip_address"))
         except ValueError:
-            return m.group('ip_address')
+            return m.group("ip_address")
         func: Callable[[Union[IPv4Address | IPv6Address]], Union[IPv4Address | IPv6Address]]
         func = {4: redact_ipv4_address, 6: redact_ipv6_address}[ip.version]  # type: ignore
         return str(func(ip))
 
     return re.sub(
         r"(?P<ip_address>(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})|[a-f\d:]{3,32})",
         _rewrite,
@@ -273,18 +189,18 @@
     return re.sub(us_ssn_regex, _rewrite, block, flags=flags)
 
 
 def hide_mac_addresses(block: str) -> str:
     flags = re.MULTILINE | re.DOTALL | re.IGNORECASE
 
     def _rewrite(m: re.Match[str]) -> str:
-        idx = crc32(m.group('mac').encode())
+        idx = crc32(m.group("mac").encode())
 
         def gen() -> Generator[str, None, None]:
-            for c in m.group('mac'):
+            for c in m.group("mac"):
                 if c in ["-", ":", "."]:
                     yield c
                 else:
                     yield str(hex(int(c, 16) + idx % 0xF)[-1])
 
         return "".join(c for c in gen())
 
@@ -325,18 +241,15 @@
 
     def _rewrite(m: re.Match[str]) -> str:
         def luhn(n: str) -> bool:
             r = [int(ch) for ch in str(n)][::-1]
             return (sum(r[0::2]) + sum(sum(divmod(d * 2, 10)) for d in r[1::2])) % 10 == 0
 
         cc = m.group("cc").replace(" ", "").replace("-", "")
-        if luhn(cc):
-            new_value = "{{ credit_card_number }}"
-        else:
-            new_value = m.group("cc")
+        new_value = "{{ credit_card_number }}" if luhn(cc) else m.group("cc")
         return m.group("before") + new_value + m.group("after")
 
     cc_regex = r"(?P<before>([^\d-]|^))(?P<cc>(?:\d[ -]*?){13,16})(?P<after>([^\d-]|$))"
 
     return re.sub(cc_regex, _rewrite, block, flags=flags)
 
 
@@ -374,18 +287,15 @@
         "fedora",
         "root",
         "ubuntu",
         "user",
     }
 
     def _rewrite(m: re.Match[str]) -> str:
-        if m.group("user_name") in known_users:
-            user = m.group("user_name")
-        else:
-            user = "ano-user"
+        user = m.group("user_name") if m.group("user_name") in known_users else "ano-user"
         return m.group("before") + user
 
     user_regexes = [
         r"(?P<before>[c-z]:\\users\\)(?P<user_name>\w{,255})",
         r"(?P<before>/(home|Users)/)(?P<user_name>[a-z0-9_-]{,255})",
     ]
     for regex in user_regexes:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ansible-anonymizer-1.1.5/ansible_anonymizer/cli.py` & `ansible-anonymizer-1.2.0/ansible_anonymizer/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 # pylint: disable=missing-module-docstring
 # pylint: disable=missing-function-docstring
 import argparse
 import pathlib
 
 import yaml
 
-from ansible_anonymizer.anonymizer import anonymize_struct
-from ansible_anonymizer.anonymizer import anonymize_text_block
+from ansible_anonymizer.anonymizer import anonymize_struct, anonymize_text_block
 
 
 def main() -> None:
     parser = argparse.ArgumentParser()
-    parser.add_argument('file_path', type=pathlib.Path)
-    parser.add_argument('--format', choices=["text", "yaml"], type=str, default="text")
+    parser.add_argument("file_path", type=pathlib.Path)
+    parser.add_argument("--format", choices=["text", "yaml"], type=str, default="text")
     args = parser.parse_args()
 
     if args.format == "text":
         print(anonymize_text_block(args.file_path.read_text()))
     elif args.format == "yaml":
         print(anonymize_struct(yaml.safe_load(args.file_path.read_text())))
```

### Comparing `ansible-anonymizer-1.1.5/ansible_anonymizer.egg-info/PKG-INFO` & `ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-anonymizer
-Version: 1.1.5
+Version: 1.2.0
 Summary: Ansible Anonymizer
 Author-email: Gonéri Le Bouder <goneri@lebouder.net>
 Project-URL: Homepage, https://github.com/ansible/anonymizer
 Keywords: pii,anonymize
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -51,7 +51,13 @@
    >>> some_text = """
    ... - name: a task
    ...   a_module:
    ...     secret: foobar
    ... """
    >>> anonymizer.anonymize_text_block(some_text)
    '\n- name: a task\n  a_module:\n    secret: {{ }}\n'
+
+You can also use the ``ansible-anonymizer`` command:
+
+.. code-block:: console
+
+   ansible-anonymizer my-secret-file
```

### Comparing `ansible-anonymizer-1.1.5/ansible_anonymizer.egg-info/SOURCES.txt` & `ansible-anonymizer-1.2.0/ansible_anonymizer.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 pyproject.toml
 tox.ini
 .github/ISSUE_TEMPLATE.md
 .github/workflows/tox.yml
 ansible_anonymizer/__init__.py
 ansible_anonymizer/anonymizer.py
 ansible_anonymizer/cli.py
+ansible_anonymizer/field_checks.py
+ansible_anonymizer/jinja2.py
+ansible_anonymizer/parser.py
 ansible_anonymizer.egg-info/PKG-INFO
 ansible_anonymizer.egg-info/SOURCES.txt
 ansible_anonymizer.egg-info/dependency_links.txt
 ansible_anonymizer.egg-info/entry_points.txt
 ansible_anonymizer.egg-info/requires.txt
 ansible_anonymizer.egg-info/top_level.txt
 tests/test_anonymizer.py
```

### Comparing `ansible-anonymizer-1.1.5/tox.ini` & `ansible-anonymizer-1.2.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tox]
-envlist = py39, py310, py311, flake8, mypy, black
+envlist = py39, py310, py311, flake8, mypy, black, ruff
 
 [gh-actions]
 python =
     3.9: py39
     3.10: py310
-    3.11: py311, flake8, mypy, black
+    3.11: py311, flake8, mypy, black, ruff
 
 [testenv:flake8]
 basepython = python
 deps = flake8
 commands = flake8 ansible_anonymizer tests
 
 [testenv]
@@ -43,24 +43,32 @@
 commands =
   python -m build
   python -c "print('finish the upload with: twine upload -s dist/*')"
 
 
 [flake8]
 max-line-length = 160
-ignore = C114,C116
+ignore = C114,C116,W503
 
 
 [testenv:mypy]
 basepython = python3.11
+skip_install = true
 deps =
     {[testenv]deps}
     mypy
     types-PyYAML
 commands = mypy --strict ansible_anonymizer
 
 [testenv:black]
 basepython = python3.11
 deps =
     {[testenv]deps}
     black
 commands = black --check --line-length 100 ansible_anonymizer tests
+
+[testenv:ruff]
+basepython = python3.11
+skip_install = true
+deps =
+    ruff
+commands = ruff .
```

