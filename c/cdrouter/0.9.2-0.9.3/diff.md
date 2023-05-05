# Comparing `tmp/cdrouter-0.9.2.tar.gz` & `tmp/cdrouter-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cdrouter-0.9.2.tar", last modified: Mon Apr 24 18:48:17 2023, max compression
+gzip compressed data, was "dist/cdrouter-0.9.3.tar", last modified: Fri May  5 14:24:24 2023, max compression
```

## Comparing `cdrouter-0.9.2.tar` & `cdrouter-0.9.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:48:17.000000 cdrouter-0.9.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter/
--rw-r--r--   0 root         (0) root         (0)      162 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13566 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/alerts.py
--rw-r--r--   0 root         (0) root         (0)     4747 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/annotations.py
--rw-r--r--   0 root         (0) root         (0)     7330 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/attachments.py
--rw-r--r--   0 root         (0) root         (0)     4786 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/captures.py
--rw-r--r--   0 root         (0) root         (0)     1393 2022-11-02 12:33:34.000000 cdrouter-0.9.2/cdrouter/cdr_datetime.py
--rw-r--r--   0 root         (0) root         (0)      246 2020-11-05 19:50:12.000000 cdrouter-0.9.2/cdrouter/cdr_error.py
--rw-r--r--   0 root         (0) root         (0)    18456 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/cdrouter.py
--rw-r--r--   0 root         (0) root         (0)    20256 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/configs.py
--rw-r--r--   0 root         (0) root         (0)    16701 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/devices.py
--rw-r--r--   0 root         (0) root         (0)     1755 2022-11-02 12:33:34.000000 cdrouter-0.9.2/cdrouter/exports.py
--rw-r--r--   0 root         (0) root         (0)     7027 2023-02-02 15:33:12.000000 cdrouter-0.9.2/cdrouter/filters.py
--rw-r--r--   0 root         (0) root         (0)     4640 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/highlights.py
--rw-r--r--   0 root         (0) root         (0)     3481 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/history.py
--rw-r--r--   0 root         (0) root         (0)     9626 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/imports.py
--rw-r--r--   0 root         (0) root         (0)    11132 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/jobs.py
--rw-r--r--   0 root         (0) root         (0)    10675 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/metrics.py
--rw-r--r--   0 root         (0) root         (0)    16100 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/packages.py
--rw-r--r--   0 root         (0) root         (0)    39213 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/results.py
--rw-r--r--   0 root         (0) root         (0)    21568 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/system.py
--rw-r--r--   0 root         (0) root         (0)     4588 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/tags.py
--rw-r--r--   0 root         (0) root         (0)    20275 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/testresults.py
--rw-r--r--   0 root         (0) root         (0)    24462 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/testsuites.py
--rw-r--r--   0 root         (0) root         (0)     8901 2023-04-24 18:47:52.000000 cdrouter-0.9.2/cdrouter/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7138 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      728 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-24 18:48:17.000000 cdrouter-0.9.2/cdrouter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1073 2020-11-05 19:50:12.000000 cdrouter-0.9.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       64 2020-11-05 19:50:12.000000 cdrouter-0.9.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4981 2023-03-01 14:31:24.000000 cdrouter-0.9.2/README.rst
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-02 12:33:34.000000 cdrouter-0.9.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-24 18:48:17.000000 cdrouter-0.9.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2022 2022-11-02 12:33:34.000000 cdrouter-0.9.2/setup.py
--rw-r--r--   0 root         (0) root         (0)     7138 2023-04-24 18:48:17.000000 cdrouter-0.9.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:24:24.000000 cdrouter-0.9.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter/
+-rw-r--r--   0 root         (0) root         (0)      162 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13566 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/alerts.py
+-rw-r--r--   0 root         (0) root         (0)     4747 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/annotations.py
+-rw-r--r--   0 root         (0) root         (0)     7330 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/attachments.py
+-rw-r--r--   0 root         (0) root         (0)     4786 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/captures.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2022-11-02 12:33:34.000000 cdrouter-0.9.3/cdrouter/cdr_datetime.py
+-rw-r--r--   0 root         (0) root         (0)      246 2020-11-05 19:50:12.000000 cdrouter-0.9.3/cdrouter/cdr_error.py
+-rw-r--r--   0 root         (0) root         (0)    18456 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/cdrouter.py
+-rw-r--r--   0 root         (0) root         (0)    22555 2023-05-05 14:23:20.000000 cdrouter-0.9.3/cdrouter/configs.py
+-rw-r--r--   0 root         (0) root         (0)    17803 2023-05-05 14:23:20.000000 cdrouter-0.9.3/cdrouter/devices.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2022-11-02 12:33:34.000000 cdrouter-0.9.3/cdrouter/exports.py
+-rw-r--r--   0 root         (0) root         (0)     7027 2023-02-02 15:33:12.000000 cdrouter-0.9.3/cdrouter/filters.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/highlights.py
+-rw-r--r--   0 root         (0) root         (0)     3481 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/history.py
+-rw-r--r--   0 root         (0) root         (0)     9626 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/imports.py
+-rw-r--r--   0 root         (0) root         (0)    11399 2023-05-05 14:23:20.000000 cdrouter-0.9.3/cdrouter/jobs.py
+-rw-r--r--   0 root         (0) root         (0)    10675 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    17223 2023-05-05 14:23:20.000000 cdrouter-0.9.3/cdrouter/packages.py
+-rw-r--r--   0 root         (0) root         (0)    40582 2023-05-05 14:23:20.000000 cdrouter-0.9.3/cdrouter/results.py
+-rw-r--r--   0 root         (0) root         (0)    21568 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/system.py
+-rw-r--r--   0 root         (0) root         (0)     4588 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/tags.py
+-rw-r--r--   0 root         (0) root         (0)    20275 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/testresults.py
+-rw-r--r--   0 root         (0) root         (0)    24462 2023-05-05 13:02:04.000000 cdrouter-0.9.3/cdrouter/testsuites.py
+-rw-r--r--   0 root         (0) root         (0)     9961 2023-05-05 14:23:20.000000 cdrouter-0.9.3/cdrouter/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7138 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      728 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-05 14:24:24.000000 cdrouter-0.9.3/cdrouter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1073 2020-11-05 19:50:12.000000 cdrouter-0.9.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2020-11-05 19:50:12.000000 cdrouter-0.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4981 2023-03-01 14:31:24.000000 cdrouter-0.9.3/README.rst
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-05 13:04:57.000000 cdrouter-0.9.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-05 14:24:24.000000 cdrouter-0.9.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-05-05 13:04:57.000000 cdrouter-0.9.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)     7138 2023-05-05 14:24:24.000000 cdrouter-0.9.3/PKG-INFO
```

### Comparing `cdrouter-0.9.2/cdrouter/alerts.py` & `cdrouter-0.9.3/cdrouter/alerts.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/annotations.py` & `cdrouter-0.9.3/cdrouter/annotations.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/attachments.py` & `cdrouter-0.9.3/cdrouter/attachments.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/captures.py` & `cdrouter-0.9.3/cdrouter/captures.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/cdr_datetime.py` & `cdrouter-0.9.3/cdrouter/cdr_datetime.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/cdrouter.py` & `cdrouter-0.9.3/cdrouter/cdrouter.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/configs.py` & `cdrouter-0.9.3/cdrouter/configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,30 +134,33 @@
 
     :param group: (optional) Testvar group name as string.
     :param name: (optional) Testvar name as string.
     :param value: (optional) Testvar value as string.
     :param default: (optional) Testvar default value as string.
     :param isdefault: (optional) Bool `True` if testvar is set to default value.
     :param line: (optional) Config file line number as int.
+    :param action: (optional) Action to perform on the testvar or group as string.  Must be `set-testvar`, `delete-testvar`, `create-group` or `delete-group`.  If not specified, defaults to `set-testvar`.
     """
     def __init__(self, **kwargs):
         self.group = kwargs.get('group', None)
         self.name = kwargs.get('name', None)
         self.value = kwargs.get('value', None)
         self.default = kwargs.get('default', None)
         self.isdefault = kwargs.get('isdefault', None)
         self.line = kwargs.get('line', None)
+        self.action = kwargs.get('action', None)
 
 class TestvarSchema(Schema):
     group = fields.Str()
     name = fields.Str()
     value = fields.Str()
     default = fields.Str()
     isdefault = fields.Bool()
     line = fields.Int()
+    action = fields.Str(load_default=None)
 
     class Meta:
         unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Testvar(**data)
@@ -166,40 +169,43 @@
     """Model for CDRouter Configs.
 
     :param id: (optional) Config ID as an int.
     :param name: (optional) Config name as string.
     :param description: (optional) Config description as string.
     :param created: (optional) Creation time as `DateTime`.
     :param updated: (optional) Last-updated time as `DateTime`.
+    :param locked: (optional) Bool `True` if config is locked.
     :param contents: (optional) Config contents as string.
     :param user_id: (optional) User ID as an int.
     :param result_id: (optional) Result ID as an int (if a config snapshot).
     :param tags: (optional) Tags as string list.
     :param note: (optional) Note as string.
     :param interfaces: (optional) :class:`configs.Interfaces <configs.Interfaces>` list (if a config snapshot).
     """
     def __init__(self, **kwargs):
         self.id = kwargs.get('id', None)
         self.name = kwargs.get('name', None)
         self.description = kwargs.get('description', None)
         self.created = kwargs.get('created', None)
         self.updated = kwargs.get('updated', None)
+        self.locked = kwargs.get('locked', None)
         self.contents = kwargs.get('contents', None)
         self.user_id = kwargs.get('user_id', None)
         self.result_id = kwargs.get('result_id', None)
         self.tags = kwargs.get('tags', None)
         self.note = kwargs.get('note', None)
         self.interfaces = kwargs.get('interfaces', None)
 
 class ConfigSchema(Schema):
     id = fields.Int(as_string=True)
     name = fields.Str()
     description = fields.Str()
     created = DateTime()
     updated = DateTime()
+    locked = fields.Bool(load_default=False)
     contents = fields.Str()
     user_id = fields.Int(as_string=True)
     result_id = fields.Int(as_string=True, load_default=None)
     tags = fields.List(fields.Str())
     note = fields.Str()
     interfaces = fields.Nested(InterfacesSchema, many=True, unknown=EXCLUDE)
 
@@ -333,14 +339,36 @@
     def delete(self, id): # pylint: disable=invalid-name,redefined-builtin
         """Delete a config.
 
         :param id: Config ID as an int.
         """
         return self.service.delete_id(self.base, id)
 
+    def lock(self, id): # pylint: disable=invalid-name,redefined-builtin
+        """Lock a config.  Locking prevents the config from being modified or deleted until it is unlocked.
+
+        :param id: Config ID as an int.
+        :return: :class:`configs.Config <configs.Config>` object
+        :rtype: configs.Config
+        """
+        schema = self.GET_SCHEMA
+        resp = self.service.post(self.base+str(id)+'/lock/')
+        return self.service.decode(schema, resp)
+
+    def unlock(self, id): # pylint: disable=invalid-name,redefined-builtin
+        """Unlock a config.  Unlocking a locked config allows it to be modified or deleted once again.
+
+        :param id: Config ID as an int.
+        :return: :class:`configs.Config <configs.Config>` object
+        :rtype: configs.Config
+        """
+        schema = self.GET_SCHEMA
+        resp = self.service.post(self.base+str(id)+'/unlock/')
+        return self.service.decode(schema, resp)
+
     def get_shares(self, id): # pylint: disable=invalid-name,redefined-builtin
         """Get shares for a config.
 
         :param id: Config ID as an int.
         :return: :class:`cdrouter.Share <cdrouter.Share>` list
         """
         return self.service.get_shares(self.base, id)
@@ -516,14 +544,34 @@
 
         :param id: Config ID as an int.
         :param name: Testvar name as string.
         :param group: (optional) Testvar group as string.
         """
         return self.service.delete(self.base+str(id)+'/testvars/'+name+'/', params={'group': group})
 
+    def create_testvar_group(self, id, group): # pylint: disable=invalid-name,redefined-builtin
+        """Create a testvar group in a config. Creating a testvar
+        group is equivalent to removing the IGNORE keyword from the
+        group in the config.
+
+        :param id: Config ID as an int.
+        :param group: Testvar group as string.
+        """
+        return self.service.post(self.base+str(id)+'/testvars/', params={'group': group})
+
+    def delete_testvar_group(self, id, group): # pylint: disable=invalid-name,redefined-builtin
+        """Delete a testvar group in a config. Deleting a testvar
+        group is equivalent to adding the IGNORE keyword to the group
+        in the config.
+
+        :param id: Config ID as an int.
+        :param group: Testvar group as string.
+        """
+        return self.service.delete(self.base+str(id)+'/testvars/', params={'group': group})
+
     def bulk_edit_testvars(self, id, testvars): # pylint: disable=invalid-name,redefined-builtin
         """Bulk edit a config's testvars.
 
         :param id: Config ID as an int.
         :param testvars: :class:`configs.Testvar <configs.Testvar>` list
         :return: :class:`configs.Testvar <configs.Testvar>` list
         """
```

### Comparing `cdrouter-0.9.2/cdrouter/devices.py` & `cdrouter-0.9.3/cdrouter/devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 class Device(object):
     """Model for CDRouter Devices.
 
     :param id: (optional) Device ID as an int.
     :param name: (optional) Name as string.
     :param created: (optional) Creation time as `DateTime`.
     :param updated: (optional) Last-updated time as `DateTime`.
+    :param locked: (optional) Bool `True` if device is locked.
     :param user_id: (optional) User ID as an int.
     :param result_id: (optional) Result ID as an int (if a device snapshot).
     :param attachments_dir: (optional) Filepath for attachments as string.
     :param picture_id: (optional) Attachment ID for used for device picture as an int.
     :param tags: (optional) Tags as string list.
     :param default_ip: (optional) Default IP as a string
     :param default_login: (optional) Default login as a string
@@ -93,14 +94,15 @@
 
     """
     def __init__(self, **kwargs):
         self.id = kwargs.get('id', None)
         self.name = kwargs.get('name', None)
         self.created = kwargs.get('created', None)
         self.updated = kwargs.get('updated', None)
+        self.locked = kwargs.get('locked', None)
         self.user_id = kwargs.get('user_id', None)
         self.result_id = kwargs.get('result_id', None)
         self.attachments_dir = kwargs.get('attachments_dir', None)
         self.picture_id = kwargs.get('picture_id', None)
         self.tags = kwargs.get('tags', None)
 
         self.default_ip = kwargs.get('default_ip', None)
@@ -132,14 +134,15 @@
         self.power_off_cmd = kwargs.get('power_off_cmd', None)
 
 class DeviceSchema(Schema):
     id = fields.Int(as_string=True)
     name = fields.Str()
     created = DateTime()
     updated = DateTime()
+    locked = fields.Bool(load_default=False)
     user_id = fields.Int(as_string=True)
     result_id = fields.Int(as_string=True, load_default=None)
     attachments_dir = fields.Str(load_default=None)
     picture_id = fields.Int(as_string=True)
     tags = fields.List(fields.Str())
 
     default_ip = fields.Str()
@@ -285,14 +288,36 @@
     def delete(self, id): # pylint: disable=invalid-name,redefined-builtin
         """Delete a device.
 
         :param id: Device ID as an int.
         """
         return self.service.delete_id(self.base, id)
 
+    def lock(self, id): # pylint: disable=invalid-name,redefined-builtin
+        """Lock a device.  Locking prevents the device from being modified or deleted until it is unlocked.
+
+        :param id: Device ID as an int.
+        :return: :class:`devices.Device <devices.Device>` object
+        :rtype: devices.Device
+        """
+        schema = DeviceSchema()
+        resp = self.service.post(self.base+str(id)+'/lock/')
+        return self.service.decode(schema, resp)
+
+    def unlock(self, id): # pylint: disable=invalid-name,redefined-builtin
+        """Unlock a device.  Unlocking a locked device allows it to be modified or deleted once again.
+
+        :param id: Device ID as an int.
+        :return: :class:`devices.Device <devices.Device>` object
+        :rtype: devices.Device
+        """
+        schema = DeviceSchema()
+        resp = self.service.post(self.base+str(id)+'/unlock/')
+        return self.service.decode(schema, resp)
+
     def get_shares(self, id): # pylint: disable=invalid-name,redefined-builtin
         """Get shares for a device.
 
         :param id: Device ID as an int.
         :return: :class:`cdrouter.Share <cdrouter.Share>` list
         """
         return self.service.get_shares(self.base, id)
```

### Comparing `cdrouter-0.9.2/cdrouter/exports.py` & `cdrouter-0.9.3/cdrouter/exports.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/filters.py` & `cdrouter-0.9.3/cdrouter/filters.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/highlights.py` & `cdrouter-0.9.3/cdrouter/highlights.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/history.py` & `cdrouter-0.9.3/cdrouter/history.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/imports.py` & `cdrouter-0.9.3/cdrouter/imports.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/jobs.py` & `cdrouter-0.9.3/cdrouter/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,37 +5,40 @@
 
 """Module for accessing CDRouter Jobs."""
 
 from collections import namedtuple
 
 from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_datetime import DateTime
-from .configs import InterfacesSchema
+from .configs import InterfacesSchema, TestvarSchema
 
 class Options(object):
     """Model for CDRouter Job Options.
 
     :param tags: (optional) Tags as string list.
     :param skip_tests: (optional) Tests to skip as string list.
     :param begin_at: (optional) Test name to begin testing at as string.
     :param end_at: (optional) Test name to end testing at as string.
+    :param testvars: (optional) Extra testvars to set as a :class:`configs.Testvar <configs.Testvar>` list.
     :param extra_cli_args: (optional) Extra `cdrouter-cli` arguments as string.
     """
     def __init__(self, **kwargs):
         self.tags = kwargs.get('tags', None)
         self.skip_tests = kwargs.get('skip_tests', None)
         self.begin_at = kwargs.get('begin_at', None)
         self.end_at = kwargs.get('end_at', None)
+        self.testvars = kwargs.get('testvars', None)
         self.extra_cli_args = kwargs.get('extra_cli_args', None)
 
 class OptionsSchema(Schema):
     tags = fields.List(fields.Str(), load_default=None)
     skip_tests = fields.List(fields.Str(), load_default=None)
     begin_at = fields.Str()
     end_at = fields.Str()
+    testvars = fields.Nested(TestvarSchema, many=True, load_default=None, unknown=EXCLUDE)
     extra_cli_args = fields.Str()
 
     class Meta:
         unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
```

### Comparing `cdrouter-0.9.2/cdrouter/metrics.py` & `cdrouter-0.9.3/cdrouter/metrics.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/packages.py` & `cdrouter-0.9.3/cdrouter/packages.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,14 +120,15 @@
     """Model for CDRouter Packages.
 
     :param id: (optional) Package ID as an int.
     :param name: (optional) Name as a string.
     :param description: (optional) Description as a string.
     :param created: (optional) Creation time as `DateTime`.
     :param updated: (optional) Last-updated time as `DateTime`.
+    :param locked: (optional) Bool `True` if package is locked.
     :param test_count: (optional) Test count as an int.
     :param testlist: (optional) Testlist as a string list.
     :param extra_cli_args: (optional) Extra CLI args as a string.
     :param user_id: (optional) User ID as an int.
     :param agent_id: (optional) Agent ID as an int.
     :param config_id: (optional) Config ID as an int.
     :param result_id: (optional) Result ID as an int (if a package snapshot).
@@ -141,14 +142,15 @@
     """
     def __init__(self, **kwargs):
         self.id = kwargs.get('id', None)
         self.name = kwargs.get('name', None)
         self.description = kwargs.get('description', None)
         self.created = kwargs.get('created', None)
         self.updated = kwargs.get('updated', None)
+        self.locked = kwargs.get('locked', None)
         self.test_count = kwargs.get('test_count', None)
         self.testlist = kwargs.get('testlist', None)
         self.extra_cli_args = kwargs.get('extra_cli_args', None)
         self.user_id = kwargs.get('user_id', None)
         self.agent_id = kwargs.get('agent_id', None)
         self.config_id = kwargs.get('config_id', None)
         self.result_id = kwargs.get('result_id', None)
@@ -162,14 +164,15 @@
 
 class PackageSchema(Schema):
     id = fields.Int(as_string=True)
     name = fields.Str()
     description = fields.Str()
     created = DateTime()
     updated = DateTime()
+    locked = fields.Bool(load_default=False)
     test_count = fields.Int(as_string=True)
     testlist = fields.List(fields.Str(), load_default=None)
     extra_cli_args = fields.Str()
     user_id = fields.Int(as_string=True)
     agent_id = fields.Int(as_string=True)
     config_id = fields.Int(as_string=True)
     result_id = fields.Int(as_string=True, load_default=None)
@@ -291,14 +294,36 @@
     def delete(self, id): # pylint: disable=invalid-name,redefined-builtin
         """Delete a package.
 
         :param id: Package ID as an int.
         """
         return self.service.delete_id(self.base, id)
 
+    def lock(self, id): # pylint: disable=invalid-name,redefined-builtin
+        """Lock a package.  Locking prevents the package from being modified or deleted until it is unlocked.
+
+        :param id: Package ID as an int.
+        :return: :class:`packages.Package <packages.Package>` object
+        :rtype: packages.Package
+        """
+        schema = PackageSchema()
+        resp = self.service.post(self.base+str(id)+'/lock/')
+        return self.service.decode(schema, resp)
+
+    def unlock(self, id): # pylint: disable=invalid-name,redefined-builtin
+        """Unlock a package.  Unlocking a locked package allows it to be modified or deleted once again.
+
+        :param id: Package ID as an int.
+        :return: :class:`packages.Package <packages.Package>` object
+        :rtype: packages.Package
+        """
+        schema = PackageSchema()
+        resp = self.service.post(self.base+str(id)+'/unlock/')
+        return self.service.decode(schema, resp)
+
     def get_shares(self, id): # pylint: disable=invalid-name,redefined-builtin
         """Get shares for a package.
 
         :param id: Package ID as an int.
         :return: :class:`cdrouter.Share <cdrouter.Share>` list
         """
         return self.service.get_shares(self.base, id)
```

### Comparing `cdrouter-0.9.2/cdrouter/results.py` & `cdrouter-0.9.3/cdrouter/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import io
 
 from requests_toolbelt.downloadutils import stream
 from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_datetime import DateTime
 from .testresults import TestResultSchema
 from .alerts import AlertSchema
-from .configs import InterfacesSchema
+from .configs import InterfacesSchema, TestvarSchema
 from .metrics import GraphMetric, GraphMetricSchema, Page as MetricPage, MetricSchema as MetricsDotMetricSchema
 
 class TestCount(object):
     """Model for CDRouter Test Counts.
 
     :param name: (optional) Name as a string.
     :param count: (optional) Count as an int.
@@ -404,28 +404,31 @@
 class Options(object):
     """Model for CDRouter Result Options.
 
     :param tags: (optional) Tags as string list.
     :param skip_tests: (optional) Tests to skip as string list.
     :param begin_at: (optional) Test name to begin testing at as string.
     :param end_at: (optional) Test name to end testing at as string.
+    :param testvars: (optional) Extra testvars to set as a :class:`configs.Testvar <configs.Testvar>` list.
     :param extra_cli_args: (optional) Extra `cdrouter-cli` arguments as string.
     """
     def __init__(self, **kwargs):
         self.tags = kwargs.get('tags', None)
         self.skip_tests = kwargs.get('skip_tests', None)
         self.begin_at = kwargs.get('begin_at', None)
         self.end_at = kwargs.get('end_at', None)
+        self.testvars = kwargs.get('testvars', None)
         self.extra_cli_args = kwargs.get('extra_cli_args', None)
 
 class OptionsSchema(Schema):
     tags = fields.List(fields.Str(), load_default=None)
     skip_tests = fields.List(fields.Str(), load_default=None)
     begin_at = fields.Str()
     end_at = fields.Str()
+    testvars = fields.Nested(TestvarSchema, many=True, load_default=None, unknown=EXCLUDE)
     extra_cli_args = fields.Str()
 
     class Meta:
         unknown = EXCLUDE
 
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
@@ -498,14 +501,15 @@
 
 class Result(object):
     """Model for CDRouter Results.
 
     :param id: (optional) Result ID as an int.
     :param created: (optional) Creation time as `DateTime`.
     :param updated: (optional) Last-updated time as `DateTime`.
+    :param locked: (optional) Bool `True` if result is locked.
     :param result: (optional) Result as a string.
     :param active: (optional) Bool `True` if status is 'running' or 'paused'.
     :param status: (optional) Status as a string.
     :param loops: (optional) Loop count as an int.
     :param tests: (optional) Test count as an int.
     :param passed: (optional) Passed count as an int.
     :param fail: (optional) Failed count as an int.
@@ -532,14 +536,15 @@
     :param features: (optional) Dict of feature name strings to :class:`results.Feature <results.Feature>` objects.
     :param interfaces: (optional) :class:`configs.Interfaces <configs.Interfaces>` list.
     """
     def __init__(self, **kwargs):
         self.id = kwargs.get('id', None)
         self.created = kwargs.get('created', None)
         self.updated = kwargs.get('updated', None)
+        self.locked = kwargs.get('locked', None)
         self.result = kwargs.get('result', None)
         self.active = kwargs.get('active', None)
         self.status = kwargs.get('status', None)
         self.loops = kwargs.get('loops', None)
         self.tests = kwargs.get('tests', None)
         self.passed = kwargs.get('pass', None)
         self.fail = kwargs.get('fail', None)
@@ -566,14 +571,15 @@
         self.features = kwargs.get('features', None)
         self.interfaces = kwargs.get('interfaces', None)
 
 class ResultSchema(Schema):
     id = fields.Int(as_string=True)
     created = DateTime()
     updated = DateTime()
+    locked = fields.Bool(load_default=False)
     result = fields.Str()
     active = fields.Bool()
     status = fields.Str()
     loops = fields.Int()
     tests = fields.Int()
     passed = fields.Int(attribute='pass', data_key='pass')
     fail = fields.Int()
@@ -762,14 +768,36 @@
     def delete(self, id): # pylint: disable=invalid-name,redefined-builtin
         """Delete a result.
 
         :param id: Result ID as an int.
         """
         return self.service.delete_id(self.base, id)
 
+    def lock(self, id): # pylint: disable=invalid-name,redefined-builtin
+        """Lock a result.  Locking prevents the result from being modified or deleted until it is unlocked.
+
+        :param id: Result ID as an int.
+        :return: :class:`results.Result <results.Result>` object
+        :rtype: results.Result
+        """
+        schema = ResultSchema()
+        resp = self.service.post(self.base+str(id)+'/lock/')
+        return self.service.decode(schema, resp)
+
+    def unlock(self, id): # pylint: disable=invalid-name,redefined-builtin
+        """Unlock a result.  Unlocking a locked result allows it to be modified or deleted once again.
+
+        :param id: Result ID as an int.
+        :return: :class:`results.Result <results.Result>` object
+        :rtype: results.Result
+        """
+        schema = ResultSchema()
+        resp = self.service.post(self.base+str(id)+'/unlock/')
+        return self.service.decode(schema, resp)
+
     def get_shares(self, id): # pylint: disable=invalid-name,redefined-builtin
         """Get shares for a result.
 
         :param id: Result ID as an int.
         :return: :class:`cdrouter.Share <cdrouter.Share>` list
         """
         return self.service.get_shares(self.base, id)
```

### Comparing `cdrouter-0.9.2/cdrouter/system.py` & `cdrouter-0.9.3/cdrouter/system.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/tags.py` & `cdrouter-0.9.3/cdrouter/tags.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/testresults.py` & `cdrouter-0.9.3/cdrouter/testresults.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/testsuites.py` & `cdrouter-0.9.3/cdrouter/testsuites.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/cdrouter/users.py` & `cdrouter-0.9.3/cdrouter/users.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,38 +18,41 @@
     :param id: (optional) User ID as an int.
     :param admin: (optional) Bool `True` if user is an administrator.
     :param disabled: (optional) Bool `True` if user is disabled.
     :param name: (optional) User name as string.
     :param description: (optional) User description as string.
     :param created: (optional) User creation time as `DateTime`.
     :param updated: (optional) User last-updated time as `DateTime`.
+    :param locked: (optional) Bool `True` if user is locked.
     :param token: (optional) User's API token as string.
     """
     def __init__(self, **kwargs):
         self.id = kwargs.get('id', None)
         self.admin = kwargs.get('admin', None)
         self.disabled = kwargs.get('disabled', None)
         self.name = kwargs.get('name', None)
         self.description = kwargs.get('description', None)
         self.created = kwargs.get('created', None)
         self.updated = kwargs.get('updated', None)
+        self.locked = kwargs.get('locked', None)
         self.token = kwargs.get('token', None)
 
         # only needed for create & change_password
         self.password = kwargs.get('password', None)
         self.password_confirm = kwargs.get('password_confirm', None)
 
 class UserSchema(Schema):
     id = fields.Int(as_string=True)
     admin = fields.Bool()
     disabled = fields.Bool()
     name = fields.Str()
     description = fields.Str()
     created = DateTime()
     updated = DateTime()
+    locked = fields.Bool(load_default=False)
     token = fields.Str()
 
     password = fields.Str()
     password_confirm = fields.Str()
 
     class Meta:
         unknown = EXCLUDE
@@ -188,14 +191,36 @@
     def delete(self, id): # pylint: disable=invalid-name,redefined-builtin
         """Delete a user.
 
         :param id: User ID as an int.
         """
         return self.service.delete_id(self.base, id)
 
+    def lock(self, id): # pylint: disable=invalid-name,redefined-builtin
+        """Lock a user.  Locking prevents the user from being modified or deleted until it is unlocked.
+
+        :param id: User ID as an int.
+        :return: :class:`users.User <users.User>` object
+        :rtype: users.User
+        """
+        schema = UserSchema()
+        resp = self.service.post(self.base+str(id)+'/lock/')
+        return self.service.decode(schema, resp)
+
+    def unlock(self, id): # pylint: disable=invalid-name,redefined-builtin
+        """Unlock a user.  Unlocking a locked user allows it to be modified or deleted once again.
+
+        :param id: User ID as an int.
+        :return: :class:`users.User <users.User>` object
+        :rtype: users.User
+        """
+        schema = UserSchema()
+        resp = self.service.post(self.base+str(id)+'/unlock/')
+        return self.service.decode(schema, resp)
+
     def bulk_copy(self, ids):
         """Bulk copy a set of users.
 
         :param ids: Int list of user IDs.
         :return: :class:`users.User <users.User>` list
         """
         schema = UserSchema()
```

### Comparing `cdrouter-0.9.2/cdrouter.egg-info/PKG-INFO` & `cdrouter-0.9.3/cdrouter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cdrouter
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python client for the CDRouter Web API
 Home-page: https://github.com/qacafe/cdrouter.py
 Author: QA Cafe
 Author-email: support@qacafe.com
 License: MIT
 Description: cdrouter
         ========
```

### Comparing `cdrouter-0.9.2/cdrouter.egg-info/SOURCES.txt` & `cdrouter-0.9.3/cdrouter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/LICENSE.txt` & `cdrouter-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/README.rst` & `cdrouter-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.2/setup.py` & `cdrouter-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,9 +57,9 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     keywords="cdrouter json rest api client",
     packages=["cdrouter"],
-    install_requires=["future", "marshmallow>=3.13.0,<4.0.0", "requests", "requests-toolbelt"],
+    install_requires=["future", "marshmallow>=3.13.0,<4.0.0", "requests", "requests-toolbelt", "urllib3<2"],
 )
```

### Comparing `cdrouter-0.9.2/PKG-INFO` & `cdrouter-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cdrouter
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python client for the CDRouter Web API
 Home-page: https://github.com/qacafe/cdrouter.py
 Author: QA Cafe
 Author-email: support@qacafe.com
 License: MIT
 Description: cdrouter
         ========
```

