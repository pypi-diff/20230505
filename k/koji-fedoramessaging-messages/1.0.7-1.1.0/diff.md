# Comparing `tmp/koji-fedoramessaging-messages-1.0.7.tar.gz` & `tmp/koji-fedoramessaging-messages-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koji-fedoramessaging-messages-1.0.7.tar", max compression
+gzip compressed data, was "koji-fedoramessaging-messages-1.1.0.tar", max compression
```

## Comparing `koji-fedoramessaging-messages-1.0.7.tar` & `koji-fedoramessaging-messages-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    18092 2023-01-24 15:38:49.840028 koji-fedoramessaging-messages-1.0.7/LICENSE
--rw-r--r--   0        0        0      257 2023-01-24 15:38:49.840028 koji-fedoramessaging-messages-1.0.7/README.md
--rw-r--r--   0        0        0      676 2023-01-30 14:55:09.035636 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/__init__.py
--rw-r--r--   0        0        0     1779 2023-04-03 08:49:37.133775 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/base.py
--rw-r--r--   0        0        0     4377 2023-04-03 08:49:37.133775 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/build.py
--rw-r--r--   0        0        0     3498 2023-04-03 08:53:46.826498 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/package.py
--rw-r--r--   0        0        0     2470 2023-04-03 09:01:28.592868 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/repo.py
--rw-r--r--   0        0        0     9699 2023-04-03 08:55:29.437796 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/rpm.py
--rw-r--r--   0        0        0     4027 2023-04-03 09:01:28.615868 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tag.py
--rw-r--r--   0        0        0     6121 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/task.py
--rw-r--r--   0        0        0        0 2023-01-24 15:38:49.841028 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/__init__.py
--rw-r--r--   0        0        0      895 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/test_base.py
--rw-r--r--   0        0        0     1310 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/test_build.py
--rw-r--r--   0        0        0     1541 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/test_package.py
--rw-r--r--   0        0        0     1036 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/test_repo.py
--rw-r--r--   0        0        0     3510 2023-04-03 08:49:37.135775 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/test_rpm.py
--rw-r--r--   0        0        0     2014 2023-04-03 08:49:37.135775 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/test_tag.py
--rw-r--r--   0        0        0     4301 2023-04-03 08:49:37.135775 koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/test_task.py
--rw-r--r--   0        0        0     1648 2023-04-03 12:59:35.330072 koji-fedoramessaging-messages-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      746 2023-04-03 08:49:37.135775 koji-fedoramessaging-messages-1.0.7/tox.ini
--rw-r--r--   0        0        0     2204 2023-04-03 13:02:42.246160 koji-fedoramessaging-messages-1.0.7/setup.py
--rw-r--r--   0        0        0      999 2023-04-03 13:02:42.246423 koji-fedoramessaging-messages-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-01-24 15:38:49.840028 koji-fedoramessaging-messages-1.1.0/LICENSE
+-rw-r--r--   0        0        0      257 2023-01-24 15:38:49.840028 koji-fedoramessaging-messages-1.1.0/README.md
+-rw-r--r--   0        0        0      676 2023-01-30 14:55:09.035636 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/__init__.py
+-rw-r--r--   0        0        0     1779 2023-04-03 08:49:37.133775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/base.py
+-rw-r--r--   0        0        0     4377 2023-04-03 08:49:37.133775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/build.py
+-rw-r--r--   0        0        0     3498 2023-04-03 08:53:46.826498 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/package.py
+-rw-r--r--   0        0        0     2470 2023-04-03 09:01:28.592868 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/repo.py
+-rw-r--r--   0        0        0     9699 2023-04-03 08:55:29.437796 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/rpm.py
+-rw-r--r--   0        0        0     4710 2023-05-03 12:32:49.824172 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tag.py
+-rw-r--r--   0        0        0     6121 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/task.py
+-rw-r--r--   0        0        0        0 2023-01-24 15:38:49.841028 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/__init__.py
+-rw-r--r--   0        0        0      895 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_base.py
+-rw-r--r--   0        0        0     1310 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_build.py
+-rw-r--r--   0        0        0     1541 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_package.py
+-rw-r--r--   0        0        0     1036 2023-04-03 08:49:37.134775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_repo.py
+-rw-r--r--   0        0        0     3510 2023-04-03 08:49:37.135775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_rpm.py
+-rw-r--r--   0        0        0     2307 2023-05-03 12:32:49.825172 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_tag.py
+-rw-r--r--   0        0        0     4301 2023-04-03 08:49:37.135775 koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_task.py
+-rw-r--r--   0        0        0     1648 2023-05-05 14:34:41.381139 koji-fedoramessaging-messages-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      746 2023-04-03 08:49:37.135775 koji-fedoramessaging-messages-1.1.0/tox.ini
+-rw-r--r--   0        0        0     2204 2023-05-05 14:37:14.994838 koji-fedoramessaging-messages-1.1.0/setup.py
+-rw-r--r--   0        0        0      999 2023-05-05 14:37:14.995073 koji-fedoramessaging-messages-1.1.0/PKG-INFO
```

### Comparing `koji-fedoramessaging-messages-1.0.7/LICENSE` & `koji-fedoramessaging-messages-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/__init__.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/base.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/base.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/build.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/build.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/package.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/package.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/repo.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/repo.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/rpm.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/rpm.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tag.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tag.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """Define schema for fedora messages sent by koji"""
 
+import re
 from typing import List
 
 from fedora_messaging.message import DEBUG
 
-from .base import KojiFedoraMessagingMessage, SCHEMA_URL
+from .base import SCHEMA_URL, KojiFedoraMessagingMessage
 
 TAG = {
     "type": "object",
     "properties": {
         "build_id": {"type": "integer", "description": "build id"},
         "name": {"type": "string", "description": "package name"},
         "tag_id": {
@@ -51,18 +52,25 @@
         "release": {
             "type": "string",
             "description": "release number of the package",
         },
     },
 }
 
+_MASS_REBUILD_RE = re.compile(r"^f\d+-rebuild$")
+_ELN_RE = re.compile(r"^eln(-.*)?$")
+
 
 class TagMessage(KojiFedoraMessagingMessage):
     severity = DEBUG
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.priority = self._choose_priority()
+
     @property
     def build_id(self) -> int:
         return self.body.get("build_id")
 
     @property
     def name(self) -> str:
         return self.body.get("name")
@@ -111,14 +119,30 @@
         # This looks like it's the action initiator, no? Seems more correct than the owner.
         return self.user
 
     @property
     def usernames(self) -> List[str]:
         return [name for name in (self.agent_name, self.owner) if name is not None]
 
+    @property
+    def is_mass_rebuild(self) -> bool:
+        return self.tag and _MASS_REBUILD_RE.match(self.tag) is not None
+
+    @property
+    def is_eln(self) -> bool:
+        return self.tag and _ELN_RE.match(self.tag) is not None
+
+    def _choose_priority(self) -> int:
+        # https://pagure.io/fedora-infrastructure/issue/10899
+        if self.is_mass_rebuild:
+            return 0
+        if self.is_eln:
+            return 1
+        return 2
+
 
 class TagV1(TagMessage):
     """This message is sent when a package is tagged."""
 
     topic = "buildsys.tag"
     _summary_action = "tagged into"
     body_schema = {
```

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/task.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/task.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/test_base.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/test_build.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/test_package.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/test_repo.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_repo.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/test_rpm.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_rpm.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/test_tag.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_tag.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 from koji_fedoramessaging_messages.tag import TagV1, UntagV1
 
 
 def test_tag_message():
     body = {
         "build_id": 1457909,
         "name": "http-parser",
@@ -64,7 +66,20 @@
     assert msg.release == "2.el8"
     assert (
         msg.summary
         == "python-twisted-19.10.0-2.el8 was untagged from epel8-signing-pending by autopen"
     )
     assert str(msg) == msg.summary
     assert msg.packages == ["python-twisted"]
+
+
+@pytest.mark.parametrize(
+    "tag,prio",
+    [("f42", 2), ("f42-rebuild", 0), ("eln", 1), ("eln-rebuild", 1), (None, 2)],
+)
+def test_tag_priority(tag, prio):
+    body = {
+        "tag": tag,
+    }
+    msg = TagV1(body=body)
+    msg.validate()
+    assert msg.priority == prio
```

### Comparing `koji-fedoramessaging-messages-1.0.7/koji_fedoramessaging_messages/tests/test_task.py` & `koji-fedoramessaging-messages-1.1.0/koji_fedoramessaging_messages/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/pyproject.toml` & `koji-fedoramessaging-messages-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "koji-fedoramessaging-messages"
-version = "1.0.7"
+version = "1.1.0"
 description = "A schema package for messages sent by the koji-fedoramessaging plugin"
 
 license = "GPL-3.0-or-later"
 
 authors = [
   "Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"
 ]
```

### Comparing `koji-fedoramessaging-messages-1.0.7/tox.ini` & `koji-fedoramessaging-messages-1.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `koji-fedoramessaging-messages-1.0.7/setup.py` & `koji-fedoramessaging-messages-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                      'koji_fedoramessaging.tag.UntagV1 = '
                      'koji_fedoramessaging_messages.tag:UntagV1',
                      'koji_fedoramessaging.task.TaskStateChangeV1 = '
                      'koji_fedoramessaging_messages.task:TaskStateChangeV1']}
 
 setup_kwargs = {
     'name': 'koji-fedoramessaging-messages',
-    'version': '1.0.7',
+    'version': '1.1.0',
     'description': 'A schema package for messages sent by the koji-fedoramessaging plugin',
     'long_description': '# koji-fedoramessaging messages\n\nA schema package for [koji-fedoramessaging](http://github.com/fedora-infra/koji-fedoramessaging).\n\nSee the [detailed documentation](https://fedora-messaging.readthedocs.io/en/latest/messages.html) on packaging your schemas.\n',
     'author': 'Fedora Infrastructure Team',
     'author_email': 'infrastructure@lists.fedoraproject.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/fedora-infra/koji-fedoramessaging-messages',
```

### Comparing `koji-fedoramessaging-messages-1.0.7/PKG-INFO` & `koji-fedoramessaging-messages-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koji-fedoramessaging-messages
-Version: 1.0.7
+Version: 1.1.0
 Summary: A schema package for messages sent by the koji-fedoramessaging plugin
 Home-page: https://github.com/fedora-infra/koji-fedoramessaging-messages
 License: GPL-3.0-or-later
 Keywords: fedora
 Author: Fedora Infrastructure Team
 Author-email: infrastructure@lists.fedoraproject.org
 Requires-Python: >=3.10,<4.0
```

