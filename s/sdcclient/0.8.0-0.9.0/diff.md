# Comparing `tmp/sdcclient-0.8.0.tar.gz` & `tmp/sdcclient-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sdcclient-0.8.0.tar", last modified: Sun Apr 14 22:23:17 2019, max compression
+gzip compressed data, was "dist/sdcclient-0.9.0.tar", last modified: Wed Sep 25 00:12:13 2019, max compression
```

## Comparing `sdcclient-0.8.0.tar` & `sdcclient-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 davide     (501) staff       (20)        0 2019-04-14 22:23:17.000000 sdcclient-0.8.0/
--rw-r--r--   0 davide     (501) staff       (20)      249 2019-04-14 22:23:17.000000 sdcclient-0.8.0/PKG-INFO
-drwxr-xr-x   0 davide     (501) staff       (20)        0 2019-04-14 22:23:17.000000 sdcclient-0.8.0/sdcclient/
--rw-r--r--   0 davide     (501) staff       (20)    49788 2019-04-14 21:23:38.000000 sdcclient-0.8.0/sdcclient/_monitor.py
--rw-r--r--   0 davide     (501) staff       (20)    44958 2019-04-14 20:49:24.000000 sdcclient-0.8.0/sdcclient/_common.py
--rw-r--r--   0 davide     (501) staff       (20)      234 2019-04-14 20:49:24.000000 sdcclient-0.8.0/sdcclient/__init__.py
--rw-r--r--   0 davide     (501) staff       (20)    28897 2019-02-20 21:51:16.000000 sdcclient-0.8.0/sdcclient/_scanning.py
--rw-r--r--   0 davide     (501) staff       (20)    46312 2019-03-19 20:00:04.000000 sdcclient-0.8.0/sdcclient/_secure.py
--rw-r--r--   0 davide     (501) staff       (20)    13039 2019-04-14 20:49:24.000000 sdcclient-0.8.0/sdcclient/_monitor_v1.py
--rw-r--r--   0 davide     (501) staff       (20)     5559 2018-05-23 21:31:13.000000 sdcclient-0.8.0/README.md
--rw-r--r--   0 davide     (501) staff       (20)      370 2019-04-14 20:50:03.000000 sdcclient-0.8.0/setup.py
--rw-r--r--   0 davide     (501) staff       (20)       79 2019-04-14 22:23:17.000000 sdcclient-0.8.0/setup.cfg
-drwxr-xr-x   0 davide     (501) staff       (20)        0 2019-04-14 22:23:17.000000 sdcclient-0.8.0/sdcclient.egg-info/
--rw-r--r--   0 davide     (501) staff       (20)      249 2019-04-14 22:23:17.000000 sdcclient-0.8.0/sdcclient.egg-info/PKG-INFO
--rw-r--r--   0 davide     (501) staff       (20)        1 2019-04-14 22:21:00.000000 sdcclient-0.8.0/sdcclient.egg-info/not-zip-safe
--rw-r--r--   0 davide     (501) staff       (20)      358 2019-04-14 22:23:17.000000 sdcclient-0.8.0/sdcclient.egg-info/SOURCES.txt
--rw-r--r--   0 davide     (501) staff       (20)       15 2019-04-14 22:23:17.000000 sdcclient-0.8.0/sdcclient.egg-info/requires.txt
--rw-r--r--   0 davide     (501) staff       (20)       10 2019-04-14 22:23:17.000000 sdcclient-0.8.0/sdcclient.egg-info/top_level.txt
--rw-r--r--   0 davide     (501) staff       (20)        1 2019-04-14 22:23:17.000000 sdcclient-0.8.0/sdcclient.egg-info/dependency_links.txt
+drwxr-xr-x   0 davide     (501) staff       (20)        0 2019-09-25 00:12:13.000000 sdcclient-0.9.0/
+-rw-r--r--   0 davide     (501) staff       (20)      249 2019-09-25 00:12:13.000000 sdcclient-0.9.0/PKG-INFO
+drwxr-xr-x   0 davide     (501) staff       (20)        0 2019-09-25 00:12:13.000000 sdcclient-0.9.0/sdcclient/
+-rw-r--r--   0 davide     (501) staff       (20)    51224 2019-09-20 18:04:53.000000 sdcclient-0.9.0/sdcclient/_monitor.py
+-rw-r--r--   0 davide     (501) staff       (20)     1567 2019-09-20 18:04:53.000000 sdcclient-0.9.0/sdcclient/ibm_auth_helper.py
+-rw-r--r--   0 davide     (501) staff       (20)    45331 2019-09-20 18:04:53.000000 sdcclient-0.9.0/sdcclient/_common.py
+-rw-r--r--   0 davide     (501) staff       (20)      286 2019-09-20 18:04:53.000000 sdcclient-0.9.0/sdcclient/__init__.py
+-rw-r--r--   0 davide     (501) staff       (20)    33061 2019-09-20 18:04:53.000000 sdcclient-0.9.0/sdcclient/_scanning.py
+-rw-r--r--   0 davide     (501) staff       (20)    54280 2019-09-20 18:04:53.000000 sdcclient-0.9.0/sdcclient/_secure.py
+-rw-r--r--   0 davide     (501) staff       (20)    13039 2019-04-14 20:49:24.000000 sdcclient-0.9.0/sdcclient/_monitor_v1.py
+-rw-r--r--   0 davide     (501) staff       (20)     5559 2018-05-23 21:31:13.000000 sdcclient-0.9.0/README.md
+-rw-r--r--   0 davide     (501) staff       (20)      370 2019-09-25 00:11:21.000000 sdcclient-0.9.0/setup.py
+-rw-r--r--   0 davide     (501) staff       (20)       79 2019-09-25 00:12:13.000000 sdcclient-0.9.0/setup.cfg
+drwxr-xr-x   0 davide     (501) staff       (20)        0 2019-09-25 00:12:13.000000 sdcclient-0.9.0/sdcclient.egg-info/
+-rw-r--r--   0 davide     (501) staff       (20)      249 2019-09-25 00:12:13.000000 sdcclient-0.9.0/sdcclient.egg-info/PKG-INFO
+-rw-r--r--   0 davide     (501) staff       (20)        1 2019-04-14 22:21:00.000000 sdcclient-0.9.0/sdcclient.egg-info/not-zip-safe
+-rw-r--r--   0 davide     (501) staff       (20)      387 2019-09-25 00:12:13.000000 sdcclient-0.9.0/sdcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 davide     (501) staff       (20)       15 2019-09-25 00:12:13.000000 sdcclient-0.9.0/sdcclient.egg-info/requires.txt
+-rw-r--r--   0 davide     (501) staff       (20)       10 2019-09-25 00:12:13.000000 sdcclient-0.9.0/sdcclient.egg-info/top_level.txt
+-rw-r--r--   0 davide     (501) staff       (20)        1 2019-09-25 00:12:13.000000 sdcclient-0.9.0/sdcclient.egg-info/dependency_links.txt
```

### Comparing `sdcclient-0.8.0/sdcclient/_monitor.py` & `sdcclient-0.9.0/sdcclient/_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     basestring
 except NameError:
     basestring = str
 
 
 class SdMonitorClient(_SdcCommon):
 
-    def __init__(self, token="", sdc_url='https://app.sysdigcloud.com', ssl_verify=True):
-        super(SdMonitorClient, self).__init__(token, sdc_url, ssl_verify)
+    def __init__(self, token="", sdc_url='https://app.sysdigcloud.com', ssl_verify=True, custom_headers=None):
+        super(SdMonitorClient, self).__init__(token, sdc_url, ssl_verify, custom_headers)
         self.product = "SDC"
         self._dashboards_api_version = 'v2'
         self._dashboards_api_endpoint = '/api/{}/dashboards'.format(self._dashboards_api_version)
         self._default_dashboards_api_endpoint = '/api/{}/defaultDashboards'.format(self._dashboards_api_version)
 
     def get_alerts(self):
         '''**Description**
@@ -302,14 +302,40 @@
 
         **Example**
             `examples/list_dashboards.py <https://github.com/draios/python-sdc-client/blob/master/examples/list_dashboards.py>`_
         '''
         res = requests.get(self.url + self._dashboards_api_endpoint, headers=self.hdrs, verify=self.ssl_verify)
         return self._request_result(res)
 
+    def get_dashboard(self, dashboard_id):
+        '''**Description**
+            Return a dashboard with the pased in ID. This includes the dashboards created by the user and the ones shared with them by other users.
+
+        **Success Return Value**
+            A dictionary containing the requested dashboard data.
+
+        **Example**
+            `examples/dashboard_basic_crud.py <https://github.com/draios/python-sdc-client/blob/master/examples/dashboard_basic_crud.py>`_
+        '''
+        res = requests.get(self.url + self._dashboards_api_endpoint + "/" + str(dashboard_id), headers=self.hdrs, verify=self.ssl_verify)
+        return self._request_result(res)
+
+    def update_dashboard(self, dashboard_data):
+        '''**Description**
+            Updates dashboard with provided in data. Please note that the dictionary will require a valid ID and version field to work as expected.
+
+        **Success Return Value**
+            A dictionary containing the updated dashboard data.
+
+        **Example**
+            `examples/dashboard_basic_crud.py <https://github.com/draios/python-sdc-client/blob/master/examples/dashboard_basic_crud.py>`_
+        '''
+        res = requests.put(self.url + self._dashboards_api_endpoint + "/" + str(dashboard_data['id']), headers=self.hdrs, verify=self.ssl_verify, data=json.dumps({'dashboard': dashboard_data}))
+        return self._request_result(res)
+
     def find_dashboard_by(self, name=None):
         '''**Description**
             Finds dashboards with the specified name. You can then delete the dashboard (with :func:`~SdcClient.delete_dashboard`) or edit panels (with :func:`~SdcClient.add_dashboard_panel` and :func:`~SdcClient.remove_dashboard_panel`)
 
         **Arguments**
             - **name**: the name of the dashboards to find.
```

### Comparing `sdcclient-0.8.0/sdcclient/_common.py` & `sdcclient-0.9.0/sdcclient/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,30 +6,40 @@
 class _SdcCommon(object):
     '''Interact with the Sysdig Monitor/Secure API.
 
     **Arguments**
         - **token**: A Sysdig Monitor/Secure API token from the *Sysdig Cloud API* section of the Settings page for `monitor <https://app.sysdigcloud.com/#/settings/user>`_ or .`secure <https://secure.sysdig.com/#/settings/user>`_.
         - **sdc_url**: URL for contacting the Sysdig API server. Set this in `On-Premises installs <https://support.sysdigcloud.com/hc/en-us/articles/206519903-On-Premises-Installation-Guide>`__.
         - **ssl_verify**: Whether to verify certificate. Set to False if using a self-signed certificate in an `On-Premises install <https://support.sysdigcloud.com/hc/en-us/articles/206519903-On-Premises-Installation-Guide>`__.
+        - **custom_headers**: [dict] Pass in custom headers. Useful for authentication and will override the default headers.
 
     **Returns**
         An object for further interactions with the Sysdig Monitor/Secure API. See methods below.
     '''
     lasterr = None
 
-    def __init__(self, token="", sdc_url='https://app.sysdigcloud.com', ssl_verify=True):
+    def __init__(self, token="", sdc_url='https://app.sysdigcloud.com', ssl_verify=True, custom_headers=None):
         self.token = os.environ.get("SDC_TOKEN", token)
-        self.hdrs = {'Authorization': 'Bearer ' + self.token, 'Content-Type': 'application/json'}
+        self.hdrs = self.__get_headers(custom_headers)
         self.url = os.environ.get("SDC_URL", sdc_url)
         self.ssl_verify = os.environ.get("SDC_SSL_VERIFY", None)
         if self.ssl_verify == None:
             self.ssl_verify = ssl_verify
         else:
             self.ssl_verify = self.ssl_verify.lower() == 'true'
 
+    def __get_headers(self, custom_headers):
+        headers = {
+            'Content-Type': 'application/json',
+            'Authorization': 'Bearer ' + self.token
+        }
+        if custom_headers:
+            headers.update(custom_headers)
+        return headers
+
     def _checkResponse(self, res):
         if res.status_code >= 300:
             errorcode = res.status_code
             self.lasterr = None
 
             try:
                 j = res.json()
```

### Comparing `sdcclient-0.8.0/sdcclient/_scanning.py` & `sdcclient-0.9.0/sdcclient/_scanning.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     from urllib import quote_plus, unquote_plus
 
 from sdcclient._common import _SdcCommon
 
 
 class SdScanningClient(_SdcCommon):
 
-    def __init__(self, token="", sdc_url='https://secure.sysdig.com', ssl_verify=True):
-        super(SdScanningClient, self).__init__(token, sdc_url, ssl_verify)
+    def __init__(self, token="", sdc_url='https://secure.sysdig.com', ssl_verify=True, custom_headers=None):
+        super(SdScanningClient, self).__init__(token, sdc_url, ssl_verify, custom_headers)
         self.product = "SDS"
 
     def add_image(self, image, force=False, dockerfile=None, annotations={}, autosubscribe=True):
         '''**Description**
             Add an image to the scanner
 
         **Arguments**
@@ -159,14 +159,66 @@
                 - os: CVE/distro vulnerabilities against operating system packages
 
         **Success Return Value**
             A JSON object representing the image vulnerabilities.
         '''
         return self._query_image(image, query_group='vuln', query_type=vuln_type, vendor_only=vendor_only)
 
+    def query_images_by_vulnerability(self, vulnerability_id, namespace=None, package=None, severity=None, vendor_only=True):
+        '''**Description**
+            Search system for images with the given vulnerability ID present
+
+        **Arguments**
+            - vulnerability_id: Search for images vulnerable to this vulnerability ID (e.g. CVE-1999-0001)
+            - namespace: Filter results to images with vulnerable packages in the given namespace (e.g. debian:9)
+            - package: Filter results to images with the given vulnerable package name (e.g. sed)
+            - severity: Filter results to images with the given vulnerability severity (e.g. Medium)
+            - vendor_only: Only show images with vulnerabilities explicitly deemed applicable by upstream OS vendor, if present
+
+        **Success Return Value**
+            A JSON object representing the images.
+        '''
+        url = "{base_url}/api/scanning/v1/anchore/query/images/by_vulnerability?vulnerability_id={vulnerability_id}{namespace}{package}{severity}&vendor_only={vendor_only}".format(
+            base_url=self.url,
+            vulnerability_id=vulnerability_id,
+            namespace="&namespace={}".format(namespace) if namespace else "",
+            package="&affected_package={}".format(package) if package else "",
+            severity="&severity={}".format(severity) if severity else "",
+            vendor_only=vendor_only)
+
+        res = requests.get(url, headers=self.hdrs, verify=self.ssl_verify)
+        if not self._checkResponse(res):
+            return [False, self.lasterr]
+
+        return [True, res.json()]
+
+    def query_images_by_package(self, name, version=None, package_type=None):
+        '''**Description**
+            Search system for images with the given package installed
+
+        **Arguments**
+            - name: Search for images with this package name (e.g. sed)
+            - version: Filter results to only packages with given version (e.g. 4.4-1)
+            - package-type: Filter results to only packages of given type (e.g. dpkg)
+
+        **Success Return Value**
+            A JSON object representing the images.
+        '''
+        url = "{base_url}/api/scanning/v1/anchore/query/images/by_package?name={name}{version}{package_type}".format(
+            base_url=self.url,
+            name=name,
+            version="&version={}".format(version) if version else "",
+            package_type="&package_type={}".format(package_type) if package_type else "")
+
+        res = requests.get(url, headers=self.hdrs, verify=self.ssl_verify)
+        if not self._checkResponse(res):
+            return [False, self.lasterr]
+
+        return [True, res.json()]
+
     def _query_image(self, image, query_group="", query_type="", vendor_only=True):
         if not query_group:
             raise Exception("need to specify a query group")
 
         _, _, image_digest = self._discover_inputimage(image)
         if not image_digest:
             return [False, "cannot use input image string (no discovered imageDigest)"]
@@ -235,14 +287,46 @@
 
         res = requests.get(url, headers=self.hdrs, verify=self.ssl_verify)
         if not self._checkResponse(res):
             return [False, self.lasterr]
 
         return [True, res.json()]
 
+    def get_pdf_report(self, image, tag=None, date=None):
+        '''**Description**
+            Get a pdf report of one image
+
+        **Arguments**
+            - image: Input image can be in the following formats: registry/repo:tag
+            - tag: Specify which TAG is evaluated for a given image ID or Image Digest
+            - date: date for the report of interest, the format is 'YYYY-MM-DDTHH:MM:SSZ',
+                    if not provided the latest report will be returned
+
+        **Success Return Value**
+            The pdf content
+        '''
+        image_type, _, image_digest = self._discover_inputimage(image)
+        if not image_digest:
+            return [False, "could not get image record from anchore"]
+        if not tag and image_type != 'tag':
+            return [False, "input image name is not a tag"]
+        image_tag = tag if tag else image
+
+        url = "{base_url}/api/scanning/v1/images/{image_digest}/report?tag={tag}{at}".format(
+            base_url=self.url,
+            image_digest=image_digest,
+            tag=image_tag,
+            at=("&at=%s" % date) if date else "")
+
+        res = requests.get(url, headers=self.hdrs, verify=self.ssl_verify)
+        if not self._checkResponse(res):
+            return [False, self.lasterr]
+
+        return [True, res.content]
+
     def add_registry(self, registry, registry_user, registry_pass, insecure=False, registry_type="docker_v2", validate=True):
         '''**Description**
             Add image registry
 
         **Arguments**
             - registry: Full hostname/port of registry. Eg. myrepo.example.com:5000
             - registry_user: Username
@@ -444,17 +528,23 @@
         **Arguments**
             - policyid: Unique identifier associated with this policy.
             - bundleid: Target bundle. If not specified, the currently active bundle will be used.
 
         **Success Return Value**
             A JSON object containing the policy description.
         '''
-        url = self.url + '/api/scanning/v1/policies/' + policyid
-        if bundleid:
-            url += '?bundleId=' + bundleid
+        ok, policies = self.list_policies(bundleid)
+        if not ok:
+            return [ok, policies]
+
+        for policy in policies:
+            if policy["id"] == policyid:
+                return [True, policy]
+
+        return [False, "Policy not found"]
 
     def update_policy(self, policyid, policy_description):
         '''**Description**
             Update the policy with the given id
 
         **Arguments**
             - policyid: Unique identifier associated with this policy.
```

### Comparing `sdcclient-0.8.0/sdcclient/_secure.py` & `sdcclient-0.9.0/sdcclient/_secure.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import datetime
 import json
 import requests
 import shutil
 import time
 import os
+import yaml
 
 from sdcclient._common import _SdcCommon
 
 
 class SdSecureClient(_SdcCommon):
 
-    def __init__(self, token="", sdc_url='https://secure.sysdig.com', ssl_verify=True):
-        super(SdSecureClient, self).__init__(token, sdc_url, ssl_verify)
+    def __init__(self, token="", sdc_url='https://secure.sysdig.com', ssl_verify=True, custom_headers=None):
+        super(SdSecureClient, self).__init__(token, sdc_url, ssl_verify, custom_headers)
 
         self.customer_id = None
         self.product = "SDS"
 
     def _get_falco_rules(self, kind):
         res = requests.get(self.url + '/api/settings/falco/{}RulesFile'.format(kind), headers=self.hdrs, verify=self.ssl_verify)
         if not self._checkResponse(res):
@@ -171,23 +172,28 @@
 
             if "tag" in res_obj:
                 ret["tag"] = res_obj["tag"]
 
             if "files" in res_obj:
                 ret["files"] = res_obj["files"]
 
+            if "defaultPolicies" in res_obj:
+                ret["defaultPolicies"] = res_obj["defaultPolicies"]
+
             return [True, ret]
 
     def save_default_falco_rules_files(self, fsobj, save_dir):
         '''**Description**
             Given a dict returned from get_default_falco_rules_files, save those files to a set of files below save_dir.
-               The first level below save_dir is a directory with the tag name. The second level is a directory per file.
+               The first level below save_dir is a directory with the tag name and an optional default_policies.yaml file,
+               which groups rules into recommended default policies. The second level is a directory per file.
                The third level is a directory per variant. Finally the files are at the lowest level, in a file called "content".
             For example, using the example dict in get_default_falco_rules_files(), the directory layout would look like:
                 save_dir/
+                    default_policies.yaml
                     v1.5.9/
                         falco_rules.yaml/
                             29/
                                 content: a file containing "- required_engine_version: 29\n\n- list: foo\n"
                             1/
                                 content: a file containing "- required_engine_version: 1\n\n- list: foo\n"
                         k8s_audit_rules.yaml/
@@ -214,14 +220,18 @@
 
         prefix = os.path.join(save_dir, fsobj["tag"])
         try:
             os.makedirs(prefix)
         except Exception as e:
             return [False, "Could not create tag directory {}: {}".format(prefix, str(e))]
 
+        if "defaultPolicies" in fsobj:
+            with open(os.path.join(save_dir, "default_policies.yaml"), 'w') as outfile:
+                yaml.safe_dump(fsobj["defaultPolicies"], outfile)
+
         if "files" in fsobj:
             for fobj in fsobj["files"]:
                 fprefix = os.path.join(prefix, fobj["name"])
                 try:
                     os.makedirs(fprefix)
                 except Exception as e:
                     return [False, "Could not create file directory {}: {}".format(fprefix, str(e))]
@@ -248,14 +258,16 @@
         if not payload[0]:
             return payload
 
         obj = payload[1]["{}FalcoRulesFiles".format(kind)]  # pylint: disable=unsubscriptable-object
 
         obj["tag"] = rules_files["tag"]
         obj["files"] = rules_files["files"]
+        if "defaultPolicies" in rules_files:
+            obj["defaultPolicies"] = rules_files["defaultPolicies"]
 
         res = requests.put(self.url + '/api/settings/falco/{}RulesFiles'.format(kind), headers=self.hdrs, data=json.dumps(payload[1]), verify=self.ssl_verify)
         if not self._checkResponse(res):
             return [False, self.lasterr]
         return [True, res.json()]
 
     def set_default_falco_rules_files(self, rules_files):
@@ -290,23 +302,39 @@
             - A dict matching the format described in get_default_falco_rules_files.
 
         **Example**
             `examples/set_default_falco_rules_files.py <https://github.com/draios/python-sdc-client/blob/master/examples/set_default_falco_rules_files.py>`_
         '''
 
         tags = os.listdir(save_dir)
+
+        try:
+            tags.remove("default_policies.yaml")
+        except ValueError as e:
+            # Do nothing, it wasn't in the list of files
+            pass
+
         if len(tags) != 1:
             return [False, "Directory {} did not contain exactly 1 entry".format(save_dir)]
 
         tpath = os.path.join(save_dir, tags[0])
 
         if not os.path.isdir(tpath):
             return [False, "Tag path {} is not a directory".format(tpath)]
 
-        ret = {"tag": os.path.basename(tpath), "files": []}
+        defjson = []
+        defpath = os.path.join(save_dir, "default_policies.yaml")
+        if os.path.exists(defpath):
+            try:
+                with open(defpath, "r") as infile:
+                    defjson = yaml.safe_load(infile)
+            except Exception as e:
+                return [False, "Could not load default_policies.yaml: " + exc]
+
+        ret = {"tag": os.path.basename(tpath), "files": [], "defaultPolicies": defjson}
 
         for fdir in os.listdir(tpath):
             fpath = os.path.join(tpath, fdir)
             if not os.path.isdir(fpath):
                 return [False, "File path {} is not a directory".format(fpath)]
             fobj = {"name": os.path.basename(fpath), "variants": []}
             for vdir in os.listdir(fpath):
@@ -942,7 +970,185 @@
         url = "{url}/api/commands/{id}?from=0&to={to}{metrics}".format(
             url=self.url,
             id=id,
             to=int(time.time() * 10**6),
             metrics="&metrics=" + json.dumps(metrics) if metrics else "")
         res = requests.get(url, headers=self.hdrs, verify=self.ssl_verify)
         return self._request_result(res)
+
+    def list_image_profiles(self):
+        '''**Description**
+            List the current set of image profiles.
+
+        **Arguments**
+            - None
+
+        **Success Return Value**
+            A JSON object containing the details of each profile.
+
+        '''
+        url = "{url}/api/profiling/v1/secure/profileGroups/0/profiles".format(
+            url = self.url
+        )
+
+        res = requests.get(url, headers=self.hdrs, verify=self.ssl_verify)
+        return self._request_result(res)
+
+
+    def get_image_profile(self, profileId):
+        '''**Description**
+            Find the image profile with a (partial) profile ID <profileId> and return its json description.
+
+        **Arguments**
+            - name: the name of the image profile to fetch
+
+        **Success Return Value**
+            A JSON object containing the description of the image profile. If there is no image profile with
+            the given name, returns False. Moreover, it could happen that more than one profile IDs have a collision.
+            It is due to the fact that a partial profile ID can be passed and interpreted; in this case a set of
+            collision profiles is returned, and the full complete ID string is printed. In this case, it returns
+            false.
+
+        '''
+
+        # RETRIEVE ALL THE IMAGE PROFILES
+        ok, image_profiles = self.list_image_profiles()
+
+        if not ok:
+            return [False, self.lasterr]
+
+        
+        '''
+        The content of the json stored in the image_profiles dictionary:
+
+        {
+            "offset": 0,
+            "limit": 99,
+            "canLoadMore": false,
+            "profiles": [
+            ...
+            ]
+        }
+        '''
+        
+        matched_profiles = self.__get_matched_profileIDs(profileId, image_profiles['profiles'])
+        
+        # Profile ID not found
+        if len(matched_profiles) == 0:
+            return [False, "No profile with ID {}".format(profileId)]
+        
+        # Principal workflow. Profile ID found
+        elif len(matched_profiles) == 1:
+            # Matched id. Return information
+            url = "{url}/api/profiling/v1/secure/profiles/{profileId}".format(
+                url = self.url,
+                profileId = matched_profiles[0]['profileId']
+            )
+            
+            res = requests.get(url, headers=self.hdrs, verify=self.ssl_verify)
+            return self._request_result(res)
+
+        # Collision detected. The full profile IDs are returned
+        elif len(matched_profiles) >= 2:
+            return [False, matched_profiles]
+
+
+    def __get_matched_profileIDs(self, requested_profile, profile_list):
+        '''
+        **Description**
+            Helper function for  retrieving the list of matching profile
+        
+        **Arguments**
+            - the requested profile Id (string)
+            - List of dictionary, where each dictionary contains the profile information
+    
+        **Success Return Value**
+            List of dictionary, where each dictionary represents a profile with the ID prefix substring
+            matching the requested one
+        
+        **Content structure of the profile_list parameter**
+        This array of profiles contains all the relevant information. For the purposes of this function, only
+        the profileId field is relevant.
+        
+        [
+            {
+            "profileGroupId": 0,
+            "profileId": "00000000000000000000000000000000000000000000",
+            "profileVersion": 0,
+            "profileName": "AAA/BBB:XYZ@0000000000000000000000",
+            "imageId": "00000000000000000000000000000000000000000000",
+            "imageName": "AAA/BBB:XYZ",
+            "processesProposal": {
+                "subcategories": [
+                                    {
+                                    "name": "process",
+                                    "ruleName": "process - 00000000000000000000000000000000000000000000",
+                                    "ruleType": "PROCESS",
+                                    "score": 000
+                                    }
+                                ],
+                                "score": 000
+            },
+            "fileSystemProposal": {
+                "subcategories": [
+                                    {
+                                    "name": "filesystem",
+                                    "ruleName": "filesystem - 00000000000000000000000000000000000000000000",
+                                    "ruleType": "FILESYSTEM",
+                                    "score": 000
+                                    }
+                                ],
+                                "score": 000
+            },
+            "syscallProposal": {
+                "subcategories": [
+                                    {
+                                    "name": "syscalls",
+                                    "ruleName": "syscalls - 00000000000000000000000000000000000000000000",
+                                    "ruleType": "SYSCALL",
+                                    "score": 000
+                                    }
+                                ],
+                                "score": 000
+            },
+            "networkProposal": {
+                "subcategories": [
+                                    {
+                                    "name": "network",
+                                    "ruleName": "network - 00000000000000000000000000000000000000000000",
+                                    "ruleType": "NETWORK",
+                                    "score": 000
+                                    }
+                                ],
+                                "score": 000
+            },
+            "containerImagesProposal": {
+                "subcategories": [
+                                    {
+                                    "name": "container image",
+                                    "ruleName": "container image - 00000000000000000000000000000000000000000000",
+                                    "ruleType": "CONTAINER",
+                                    "score": 0
+                                    }
+                                ],
+                                "score": 0
+            },
+            "status": "STATUS_VALUE",
+            "score": 000
+            },
+            ...
+        ]
+        '''
+
+        matched_profiles = []
+
+        request_len = len(requested_profile)
+        for profile in profile_list:
+
+            # get the length of the substring to match    
+            str_len_match = min(len(profile), request_len)
+
+            if profile['profileId'][0:str_len_match] == requested_profile[0:str_len_match]:
+                matched_profiles.append(profile)
+
+        return matched_profiles
+
```

### Comparing `sdcclient-0.8.0/sdcclient/_monitor_v1.py` & `sdcclient-0.9.0/sdcclient/_monitor_v1.py`

 * *Files identical despite different names*

### Comparing `sdcclient-0.8.0/README.md` & `sdcclient-0.9.0/README.md`

 * *Files identical despite different names*

