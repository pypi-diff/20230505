# Comparing `tmp/fedora_messaging_the_new_hotness_schema-1.1.2.tar.gz` & `tmp/fedora_messaging_the_new_hotness_schema-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedora_messaging_the_new_hotness_schema-1.1.2.tar", last modified: Mon May 30 16:09:20 2022, max compression
+gzip compressed data, was "fedora_messaging_the_new_hotness_schema-1.2.0.tar", max compression
```

## Comparing `fedora_messaging_the_new_hotness_schema-1.1.2.tar` & `fedora_messaging_the_new_hotness_schema-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,12 @@
-drwxr-xr-x   0 zlopez    (1000) zlopez    (1000)        0 2022-05-30 16:09:20.151818 fedora_messaging_the_new_hotness_schema-1.1.2/
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)    18092 2021-01-25 12:20:24.000000 fedora_messaging_the_new_hotness_schema-1.1.2/LICENSE
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)       68 2022-04-27 11:15:22.000000 fedora_messaging_the_new_hotness_schema-1.1.2/MANIFEST.in
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)     1681 2022-05-30 16:09:20.151818 fedora_messaging_the_new_hotness_schema-1.1.2/PKG-INFO
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)      884 2022-05-30 14:56:03.000000 fedora_messaging_the_new_hotness_schema-1.1.2/README.rst
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)      227 2022-05-26 14:33:23.000000 fedora_messaging_the_new_hotness_schema-1.1.2/dev-requirements.txt
-drwxr-xr-x   0 zlopez    (1000) zlopez    (1000)        0 2022-05-30 16:09:20.151818 fedora_messaging_the_new_hotness_schema-1.1.2/fedora_messaging_the_new_hotness_schema.egg-info/
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)     1681 2022-05-30 16:09:20.000000 fedora_messaging_the_new_hotness_schema-1.1.2/fedora_messaging_the_new_hotness_schema.egg-info/PKG-INFO
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)      598 2022-05-30 16:09:20.000000 fedora_messaging_the_new_hotness_schema-1.1.2/fedora_messaging_the_new_hotness_schema.egg-info/SOURCES.txt
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)        1 2022-05-30 16:09:20.000000 fedora_messaging_the_new_hotness_schema-1.1.2/fedora_messaging_the_new_hotness_schema.egg-info/dependency_links.txt
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)      122 2022-05-30 16:09:20.000000 fedora_messaging_the_new_hotness_schema-1.1.2/fedora_messaging_the_new_hotness_schema.egg-info/entry_points.txt
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)        1 2022-04-27 11:49:18.000000 fedora_messaging_the_new_hotness_schema-1.1.2/fedora_messaging_the_new_hotness_schema.egg-info/not-zip-safe
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)       31 2022-05-30 16:09:20.000000 fedora_messaging_the_new_hotness_schema-1.1.2/fedora_messaging_the_new_hotness_schema.egg-info/requires.txt
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)       15 2022-05-30 16:09:20.000000 fedora_messaging_the_new_hotness_schema-1.1.2/fedora_messaging_the_new_hotness_schema.egg-info/top_level.txt
-drwxr-xr-x   0 zlopez    (1000) zlopez    (1000)        0 2022-05-30 16:09:20.151818 fedora_messaging_the_new_hotness_schema-1.1.2/hotness_schema/
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)      829 2022-05-30 14:56:44.000000 fedora_messaging_the_new_hotness_schema-1.1.2/hotness_schema/__init__.py
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)     6782 2022-04-27 11:19:52.000000 fedora_messaging_the_new_hotness_schema-1.1.2/hotness_schema/messages.py
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)     1094 2022-04-27 11:03:44.000000 fedora_messaging_the_new_hotness_schema-1.1.2/pyproject.toml
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)       32 2022-04-27 11:03:17.000000 fedora_messaging_the_new_hotness_schema-1.1.2/requirements.txt
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)       67 2022-05-30 16:09:20.151818 fedora_messaging_the_new_hotness_schema-1.1.2/setup.cfg
--rw-r--r--   0 zlopez    (1000) zlopez    (1000)     3946 2022-05-30 14:52:51.000000 fedora_messaging_the_new_hotness_schema-1.1.2/setup.py
+-rw-r--r--   0        0        0    18092 2021-01-25 12:20:24.217782 fedora_messaging_the_new_hotness_schema-1.2.0/LICENSE
+-rw-r--r--   0        0        0      884 2022-05-30 14:56:03.568131 fedora_messaging_the_new_hotness_schema-1.2.0/README.rst
+-rw-r--r--   0        0        0      911 2022-11-24 13:44:18.377514 fedora_messaging_the_new_hotness_schema-1.2.0/hotness_schema/__init__.py
+-rw-r--r--   0        0        0     7273 2023-05-05 11:00:10.062412 fedora_messaging_the_new_hotness_schema-1.2.0/hotness_schema/messages.py
+-rw-r--r--   0        0        0      839 2022-04-27 10:53:04.642963 fedora_messaging_the_new_hotness_schema-1.2.0/hotness_schema/tests/__init__.py
+-rw-r--r--   0        0        0    46275 2022-04-27 10:53:04.662963 fedora_messaging_the_new_hotness_schema-1.2.0/hotness_schema/tests/fixtures/org.fedoraproject.prod.hotness.update.bug.file.json
+-rw-r--r--   0        0        0    39698 2022-04-27 10:53:04.662963 fedora_messaging_the_new_hotness_schema-1.2.0/hotness_schema/tests/fixtures/org.fedoraproject.prod.hotness.update.drop.json
+-rw-r--r--   0        0        0    10815 2023-05-05 11:00:10.062412 fedora_messaging_the_new_hotness_schema-1.2.0/hotness_schema/tests/test_messages.py
+-rw-r--r--   0        0        0     1678 2022-04-27 10:53:04.662963 fedora_messaging_the_new_hotness_schema-1.2.0/hotness_schema/tests/test_schema.py
+-rw-r--r--   0        0        0     2708 2023-05-05 11:55:12.335460 fedora_messaging_the_new_hotness_schema-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2017 1970-01-01 00:00:00.000000 fedora_messaging_the_new_hotness_schema-1.2.0/setup.py
+-rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 fedora_messaging_the_new_hotness_schema-1.2.0/PKG-INFO
```

### Comparing `fedora_messaging_the_new_hotness_schema-1.1.2/LICENSE` & `fedora_messaging_the_new_hotness_schema-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fedora_messaging_the_new_hotness_schema-1.1.2/PKG-INFO` & `fedora_messaging_the_new_hotness_schema-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
-Name: fedora_messaging_the_new_hotness_schema
-Version: 1.1.2
+Name: fedora-messaging-the-new-hotness-schema
+Version: 1.2.0
 Summary: JSON schema definitions for messages published by the-new-hotness
 Home-page: https://github.com/fedora-infra/the-new-hotness-messages
+License: GPL-2.0-or-later
+Author: Fedora Infrastructure Team
+Author-email: infrastructure@lists.fedoraproject.org
 Maintainer: Fedora Infrastructure Team
 Maintainer-email: infrastructure@lists.fedoraproject.org
-License: GPLv2+
-Keywords: fedora
-Platform: Fedora
-Platform: GNU/Linux
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: fedora-messaging (>=3.1.0,<4.0.0)
+Project-URL: Documentation, https://the-new-hotness-messaging-schema.readthedocs.io/en/latest
+Project-URL: Repository, https://github.com/fedora-infra/anitya-messages
+Description-Content-Type: text/x-rst
 
 .. image:: https://img.shields.io/pypi/v/fedora_messaging_the_new_hotness_schema.svg
   :target: https://pypi.org/project/fedora_messaging_the_new_hotness_schema/
 
 .. image:: https://readthedocs.org/projects/the-new-hotness-messaging-schema/badge/?version=latest
   :alt: Documentation Status
   :target: https://the-new-hotness-messaging-schema.readthedocs.io/en/latest/?badge=latest
@@ -34,8 +39,7 @@
 Documentation for the-new-hotness Message Schema could be found
 `here <https://the-new-hotness-messaging-schema.readthedocs.io/en/latest>`_.
 
 See http://json-schema.org/ for documentation on the schema format. See
 https://fedora-messaging.readthedocs.io/en/latest/messages.html for
 documentation on fedora-messaging.
 
-
```

### Comparing `fedora_messaging_the_new_hotness_schema-1.1.2/README.rst` & `fedora_messaging_the_new_hotness_schema-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `fedora_messaging_the_new_hotness_schema-1.1.2/fedora_messaging_the_new_hotness_schema.egg-info/PKG-INFO` & `fedora_messaging_the_new_hotness_schema-1.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-Metadata-Version: 2.1
-Name: fedora-messaging-the-new-hotness-schema
-Version: 1.1.2
-Summary: JSON schema definitions for messages published by the-new-hotness
-Home-page: https://github.com/fedora-infra/the-new-hotness-messages
-Maintainer: Fedora Infrastructure Team
-Maintainer-email: infrastructure@lists.fedoraproject.org
-License: GPLv2+
-Keywords: fedora
-Platform: Fedora
-Platform: GNU/Linux
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-License-File: LICENSE
-
-.. image:: https://img.shields.io/pypi/v/fedora_messaging_the_new_hotness_schema.svg
-  :target: https://pypi.org/project/fedora_messaging_the_new_hotness_schema/
-
-.. image:: https://readthedocs.org/projects/the-new-hotness-messaging-schema/badge/?version=latest
-  :alt: Documentation Status
-  :target: https://the-new-hotness-messaging-schema.readthedocs.io/en/latest/?badge=latest
-
-the-new-hotness Message Schema
-==============================
-
-JSON schema definitions for messages published by
-`the-new-hotness <https://github.com/fedora-infra/the-new-hotness>`_.
-
-Documentation for the-new-hotness Message Schema could be found
-`here <https://the-new-hotness-messaging-schema.readthedocs.io/en/latest>`_.
-
-See http://json-schema.org/ for documentation on the schema format. See
-https://fedora-messaging.readthedocs.io/en/latest/messages.html for
-documentation on fedora-messaging.
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
+packages = \
+['hotness_schema', 'hotness_schema.tests']
 
+package_data = \
+{'': ['*'], 'hotness_schema.tests': ['fixtures/*']}
+
+install_requires = \
+['fedora-messaging>=3.1.0,<4.0.0']
+
+entry_points = \
+{'fedora.messages': ['hotness.update.bug.file = hotness_schema:UpdateBugFile',
+                     'hotness.update.drop = hotness_schema:UpdateDrop']}
+
+setup_kwargs = {
+    'name': 'fedora-messaging-the-new-hotness-schema',
+    'version': '1.2.0',
+    'description': 'JSON schema definitions for messages published by the-new-hotness',
+    'long_description': '.. image:: https://img.shields.io/pypi/v/fedora_messaging_the_new_hotness_schema.svg\n  :target: https://pypi.org/project/fedora_messaging_the_new_hotness_schema/\n\n.. image:: https://readthedocs.org/projects/the-new-hotness-messaging-schema/badge/?version=latest\n  :alt: Documentation Status\n  :target: https://the-new-hotness-messaging-schema.readthedocs.io/en/latest/?badge=latest\n\nthe-new-hotness Message Schema\n==============================\n\nJSON schema definitions for messages published by\n`the-new-hotness <https://github.com/fedora-infra/the-new-hotness>`_.\n\nDocumentation for the-new-hotness Message Schema could be found\n`here <https://the-new-hotness-messaging-schema.readthedocs.io/en/latest>`_.\n\nSee http://json-schema.org/ for documentation on the schema format. See\nhttps://fedora-messaging.readthedocs.io/en/latest/messages.html for\ndocumentation on fedora-messaging.\n',
+    'author': 'Fedora Infrastructure Team',
+    'author_email': 'infrastructure@lists.fedoraproject.org',
+    'maintainer': 'Fedora Infrastructure Team',
+    'maintainer_email': 'infrastructure@lists.fedoraproject.org',
+    'url': 'https://github.com/fedora-infra/the-new-hotness-messages',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'entry_points': entry_points,
+    'python_requires': '>=3.8.1,<4.0.0',
+}
+
+
+setup(**setup_kwargs)
```

### Comparing `fedora_messaging_the_new_hotness_schema-1.1.2/hotness_schema/__init__.py` & `fedora_messaging_the_new_hotness_schema-1.2.0/hotness_schema/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
-
+from importlib import metadata
 
 from .messages import UpdateDrop, UpdateBugFile  # noqa: F401
 
-__version__ = "1.1.2"
+__version__ = metadata.version("fedora_messaging_the_new_hotness_schema")
```

### Comparing `fedora_messaging_the_new_hotness_schema-1.1.2/hotness_schema/messages.py` & `fedora_messaging_the_new_hotness_schema-1.2.0/hotness_schema/messages.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 """The schema for the-new-hotness messages."""
 
+import warnings
+
 from fedora_messaging import message
 
 
 class UpdateDrop(message.Message):
     """
     Message sent by the-new-hotness to "hotness.update.drop" topic when update
     is dropped.
@@ -128,14 +130,35 @@
         Return a reason for this drop.
 
         Returns:
             (str): Reason for drop.
         """
         return self.body["reason"]
 
+    @property
+    def app_name(self):
+        return "The New Hotness"
+
+    @property
+    def agent(self):
+        warnings.warn(
+            "agent property is deprecated, please use agent_name instead",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.body.get("agent_name")
+
+    @property
+    def agent_name(self):
+        return self.body.get("agent_name")
+
+    @property
+    def usernames(self):
+        return [self.agent_name]
+
 
 class UpdateBugFile(message.Message):
     """
     Message sent by the-new-hotness to "hotness.update.bug.file" topic when
     bugzilla issue is filled.
 
     Attributes:
```

