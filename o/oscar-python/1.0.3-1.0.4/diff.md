# Comparing `tmp/oscar_python-1.0.3.tar.gz` & `tmp/oscar_python-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oscar_python-1.0.3.tar", last modified: Wed Nov 23 12:40:07 2022, max compression
+gzip compressed data, was "oscar_python-1.0.4.tar", last modified: Fri May  5 09:48:09 2023, max compression
```

## Comparing `oscar_python-1.0.3.tar` & `oscar_python-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 12:40:07.279852 oscar_python-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)    11356 2022-11-23 12:39:58.000000 oscar_python-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     5348 2022-11-23 12:40:07.279852 oscar_python-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4931 2022-11-23 12:39:58.000000 oscar_python-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 12:40:07.275852 oscar_python-1.0.3/oscar_python/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-23 12:39:58.000000 oscar_python-1.0.3/oscar_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 12:40:07.279852 oscar_python-1.0.3/oscar_python/_providers/
--rw-r--r--   0 runner    (1001) docker     (122)     1269 2022-11-23 12:39:58.000000 oscar_python-1.0.3/oscar_python/_providers/_minio.py
--rw-r--r--   0 runner    (1001) docker     (122)     3462 2022-11-23 12:39:58.000000 oscar_python-1.0.3/oscar_python/_providers/_onedata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1205 2022-11-23 12:39:58.000000 oscar_python-1.0.3/oscar_python/_providers/_providers_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3212 2022-11-23 12:39:58.000000 oscar_python-1.0.3/oscar_python/_providers/_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     2328 2022-11-23 12:39:58.000000 oscar_python-1.0.3/oscar_python/_providers/_webdav.py
--rw-r--r--   0 runner    (1001) docker     (122)     1756 2022-11-23 12:39:58.000000 oscar_python-1.0.3/oscar_python/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2022-11-23 12:39:58.000000 oscar_python-1.0.3/oscar_python/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      250 2022-11-23 12:39:58.000000 oscar_python-1.0.3/oscar_python/local_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3287 2022-11-23 12:39:58.000000 oscar_python-1.0.3/oscar_python/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 12:40:07.275852 oscar_python-1.0.3/oscar_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5348 2022-11-23 12:40:07.000000 oscar_python-1.0.3/oscar_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      541 2022-11-23 12:40:07.000000 oscar_python-1.0.3/oscar_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-23 12:40:07.000000 oscar_python-1.0.3/oscar_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-23 12:40:07.000000 oscar_python-1.0.3/oscar_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       71 2022-11-23 12:40:07.000000 oscar_python-1.0.3/oscar_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       29 2022-11-23 12:40:07.000000 oscar_python-1.0.3/oscar_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-23 12:40:07.279852 oscar_python-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1574 2022-11-23 12:39:58.000000 oscar_python-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:48:09.684764 oscar_python-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-05 09:47:59.000000 oscar_python-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-05 09:48:09.684764 oscar_python-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-05 09:47:59.000000 oscar_python-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:48:09.684764 oscar_python-1.0.4/oscar_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:48:09.684764 oscar_python-1.0.4/oscar_python/_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/_providers/_minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/_providers/_onedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/_providers/_providers_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/_providers/_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/_providers/_webdav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-05 09:47:59.000000 oscar_python-1.0.4/oscar_python/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:48:09.684764 oscar_python-1.0.4/oscar_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-05 09:48:09.000000 oscar_python-1.0.4/oscar_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-05 09:48:09.000000 oscar_python-1.0.4/oscar_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:48:09.000000 oscar_python-1.0.4/oscar_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:48:09.000000 oscar_python-1.0.4/oscar_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 09:48:09.000000 oscar_python-1.0.4/oscar_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 09:48:09.000000 oscar_python-1.0.4/oscar_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:48:09.684764 oscar_python-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-05 09:47:59.000000 oscar_python-1.0.4/setup.py
```

### Comparing `oscar_python-1.0.3/LICENSE` & `oscar_python-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.3/PKG-INFO` & `oscar_python-1.0.4/oscar_python.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
-Name: oscar_python
-Version: 1.0.3
+Name: oscar-python
+Version: 1.0.4
 Summary: OSCAR API for python
 Home-page: https://github.com/grycap/oscar_python
 Author: GRyCAP - Universitat Politecnica de Valencia
 Author-email: calarcon@i3m.upv.es
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## Python OSCAR API
+## Python OSCAR client
 
 [![Build](https://github.com/grycap/oscar_python/actions/workflows/main.yaml/badge.svg)](https://github.com/grycap/oscar_python/actions/workflows/main.yaml)
 ![PyPI](https://img.shields.io/pypi/v/oscar_python)
 
-This package provides an API to interact with OSCAR (https://oscar.grycap.net) clusters and services. It is available on Pypi with the name [oscar-python](https://pypi.org/project/oscar-python/).
+This package provides a client to interact with OSCAR (https://oscar.grycap.net) clusters and services. It is available on Pypi with the name [oscar-python](https://pypi.org/project/oscar-python/).
 
 ### Contents
-- [Python OSCAR API](#python-oscar-api)
+- [Python OSCAR client](#python-oscar-client)
   - [Contents](#contents)
   - [Sample usage](#sample-usage)
-  - [API methods](#api-methods)
+  - [Client methods](#client-methods)
     - [Cluster methods](#cluster-methods)
     - [Service methods](#service-methods)
     - [Logs methods](#logs-methods)
     - [Storage usage](#storage-usage)
 
 ### Sample usage
 
@@ -50,22 +50,22 @@
 ``` python
 from oscar_python.client import Client
 
 client = Client("cluster-id","https://cluster-endpoint", "username", "password", True)
 
 try:
   client.create_service("/absolute_path/cowsay.yaml")
-  res = client.run_service("cowsay", '{"message": "Hi there"}')   
-  if res.status_code == 200:
-      print(res.text)
+  response = client.run_service("cowsay", input = '{"message": "Hi there"}')   
+  if response.status_code == 200:
+      print(response.text)
 except Exception as err:
   print("Failed with: ", err)
 ```
 
-### API methods
+### Client methods
 
 #### Cluster methods
 
 **get_cluster_info**
 ``` python
 # get the cluster information
 info = client.get_cluster_info() # returns an HTTP response or an HTTPError
@@ -109,20 +109,19 @@
 ``` python
 # remove a service 
 response = client.remove_service("service_name") # returns an http response
 ```
 
 **run_service**
 
-The `input` parameter may not be passed if the function doesn't require input.
+ *`input`, `output` and `timeout` are optional parameters.*
 
 ``` python
 # make a synchronous execution 
-response = client.run_service("service_name", input="input") # returns an http response
-
+response = client.run_service("service_name", input="input", output="out.png", timeout=100) # returns an http response
 ```
 
 #### Logs methods
 
 **get_job_logs**
 ``` python
 # get logs of a job
@@ -172,13 +171,7 @@
 ```
 
 **download_file**
 ``` python
 # download a file from a remote path to a local path 
 response = storage_service.download_file("storage_provider", "local_path", "remote_path")
 ```
-
-
-
-
-
-
```

### Comparing `oscar_python-1.0.3/README.md` & `oscar_python-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-## Python OSCAR API
+## Python OSCAR client
 
 [![Build](https://github.com/grycap/oscar_python/actions/workflows/main.yaml/badge.svg)](https://github.com/grycap/oscar_python/actions/workflows/main.yaml)
 ![PyPI](https://img.shields.io/pypi/v/oscar_python)
 
-This package provides an API to interact with OSCAR (https://oscar.grycap.net) clusters and services. It is available on Pypi with the name [oscar-python](https://pypi.org/project/oscar-python/).
+This package provides a client to interact with OSCAR (https://oscar.grycap.net) clusters and services. It is available on Pypi with the name [oscar-python](https://pypi.org/project/oscar-python/).
 
 ### Contents
-- [Python OSCAR API](#python-oscar-api)
+- [Python OSCAR client](#python-oscar-client)
   - [Contents](#contents)
   - [Sample usage](#sample-usage)
-  - [API methods](#api-methods)
+  - [Client methods](#client-methods)
     - [Cluster methods](#cluster-methods)
     - [Service methods](#service-methods)
     - [Logs methods](#logs-methods)
     - [Storage usage](#storage-usage)
 
 ### Sample usage
 
@@ -37,22 +37,22 @@
 ``` python
 from oscar_python.client import Client
 
 client = Client("cluster-id","https://cluster-endpoint", "username", "password", True)
 
 try:
   client.create_service("/absolute_path/cowsay.yaml")
-  res = client.run_service("cowsay", '{"message": "Hi there"}')   
-  if res.status_code == 200:
-      print(res.text)
+  response = client.run_service("cowsay", input = '{"message": "Hi there"}')   
+  if response.status_code == 200:
+      print(response.text)
 except Exception as err:
   print("Failed with: ", err)
 ```
 
-### API methods
+### Client methods
 
 #### Cluster methods
 
 **get_cluster_info**
 ``` python
 # get the cluster information
 info = client.get_cluster_info() # returns an HTTP response or an HTTPError
@@ -96,20 +96,19 @@
 ``` python
 # remove a service 
 response = client.remove_service("service_name") # returns an http response
 ```
 
 **run_service**
 
-The `input` parameter may not be passed if the function doesn't require input.
+ *`input`, `output` and `timeout` are optional parameters.*
 
 ``` python
 # make a synchronous execution 
-response = client.run_service("service_name", input="input") # returns an http response
-
+response = client.run_service("service_name", input="input", output="out.png", timeout=100) # returns an http response
 ```
 
 #### Logs methods
 
 **get_job_logs**
 ``` python
 # get logs of a job
@@ -159,13 +158,7 @@
 ```
 
 **download_file**
 ``` python
 # download a file from a remote path to a local path 
 response = storage_service.download_file("storage_provider", "local_path", "remote_path")
 ```
-
-
-
-
-
-
```

### Comparing `oscar_python-1.0.3/oscar_python/_providers/_minio.py` & `oscar_python-1.0.4/oscar_python/_providers/_minio.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.3/oscar_python/_providers/_onedata.py` & `oscar_python-1.0.4/oscar_python/_providers/_onedata.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.3/oscar_python/_providers/_providers_base.py` & `oscar_python-1.0.4/oscar_python/_providers/_providers_base.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.3/oscar_python/_providers/_s3.py` & `oscar_python-1.0.4/oscar_python/_providers/_s3.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.3/oscar_python/_providers/_webdav.py` & `oscar_python-1.0.4/oscar_python/_providers/_webdav.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.3/oscar_python/_utils.py` & `oscar_python-1.0.4/oscar_python/_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,39 +9,99 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License. 
 
 import base64
+import json
+import os
 import requests
+_DEFAULT_TIMEOUT = 30
 
 """ Generic http request """
 def make_request(c , path, method, **kwargs):
+
+    if "timeout" in kwargs.keys() and kwargs["timeout"]: 
+        timeout = kwargs["timeout"]
+        print("timeout set to: ", timeout)
+    else: 
+        timeout = _DEFAULT_TIMEOUT
+
     url = c.endpoint+path
-    headers = get_headers(c)
+    headers = get_headers(c)  
     if method in ["post", "put"]:
         if "token" in kwargs.keys() and kwargs["token"]: 
             headers = get_headers_with_token(kwargs["token"])
         if "data" in kwargs.keys() and kwargs["data"]:
-            result = requests.request(method, url, headers=headers, verify=c.ssl, data=kwargs["data"])
+            result = requests.request(method, url, headers=headers, verify=c.ssl, data=kwargs["data"], timeout=timeout)
     else:
-        result = requests.request(method, url, headers=headers, verify=c.ssl)
+        result = requests.request(method, url, headers=headers, verify=c.ssl, timeout=timeout)
 
     if "handle" in kwargs.keys() and kwargs["handle"] == False:
         return result
-
+    
     result.raise_for_status()
     return result
 
 """ Function to generate headers with basic authentication """
 def get_headers(c):
     usr_pass_as_bytes = bytes(c.user+":"+c.password,"utf-8")
     usr_pass_base_64 = base64.b64encode(usr_pass_as_bytes).decode("utf-8")
     return {"Authorization": "Basic "+ usr_pass_base_64}
 
 """ Function to generate headers with token auth """
 def get_headers_with_token(token):
     return {"Authorization": "Bearer "+ str(token)}
 
-def raise_http_errors(response):
-    response.raise_for_status()
+def write_text_file(content, file_path):
+    with open(file_path, 'w') as f:
+        f.write(content)
+
+def isBase64(st):
+    try:
+        base64.b64decode(st)
+        return True
+    except:
+        return False
+
+def decode_b64(b64_str, file_out):
+    file_extension = os.path.splitext(file_out)[1]
+    try:
+        decoded_data = base64.b64decode(b64_str)
+
+        if file_extension in [".txt", ".json"]:
+            decode = 'w'
+            decoded_data = decoded_data.decode("utf-8")
+        else:
+            decode = 'wb' 
+
+        with open(file_out, decode) as f:
+            f.write(decoded_data)
+
+    except ValueError:
+        print('Error decoding output: Invalid base64 string.')
+    except OSError:
+        print('Error decoding output: Failed to write decoded data to file.')   
+
+def encode_input(data):
+    if os.path.isfile(data):
+        try:
+            with open(data, 'rb') as file:
+                return base64.b64encode(file.read())
+        except FileNotFoundError:
+            print('Error encoding input: File {0} not found.'.format(data))
+        except OSError:
+            print('Error encoding input: Failed to read file.')
+    else:
+        message_bytes = data.encode('ascii')
+        return base64.b64encode(message_bytes)
+
+def decode_output(output, file_path):
+    if(isBase64(output)):
+        decode_b64(output, file_path)
+        return
+    if(isinstance(output,str)):
+        write_text_file(output,file_path)
+        return
+
+
```

### Comparing `oscar_python-1.0.3/oscar_python/client.py` & `oscar_python-1.0.4/oscar_python/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License. 
 
+import os
 import json
 import yaml
 import oscar_python._utils as utils
 from oscar_python.storage import Storage
 
 _INFO_PATH = "/system/info"
 _CONFIG_PATH = "/system/config"
@@ -30,14 +31,15 @@
 _ONE_DATA = "onedata"
 _WEBDAV = "webdav"
 
 _GET = "get"
 _POST = "post"
 _PUT = "put"
 _DELETE = "delete"
+_DEFAULT_TIMEOUT = 30
 
 class Client:
     #Cluster info 
     def __init__(self, id, endpoint, user, password, ssl) -> None:
         self.id = id
         self.endpoint = endpoint
         self.user = user
@@ -82,15 +84,15 @@
                     svc_exists = utils.make_request(self, _SVC_PATH+"/"+svc["name"], _GET, handle=False)
                     if svc_exists.status_code == 200:
                         raise ValueError("A service with name '{0}' is already present on the cluster".format(svc["name"]))
                 try:
                     with open(svc["script"]) as s:
                         svc["script"] = s.read()
                 except IOError as err:
-                    raise("Bouldn't read script")
+                    raise("Couldn't read script")
 
                 # cpu parameter has to be string on the request
                 if type(svc["cpu"]) is int or type(svc["cpu"]) is float: svc["cpu"]= str(svc["cpu"])
                 utils.make_request(self, _SVC_PATH, method, data=json.dumps(svc))
         else:
             raise ValueError("Bad yaml format: {0}".format(fdl))
 
@@ -106,21 +108,36 @@
             raise ValueError("The service {0} is not present on the cluster".format(name))
         return self._apply_service(fdl_path, _PUT)
 
     """ Remove a specific service """
     def remove_service(self, name):
         return utils.make_request(self, _SVC_PATH+"/"+name, _DELETE)
 
-    """ Run a synchronous execution """
-    def run_service(self, name, input=""):
-        token = self._get_token(name)
-        if input: return utils.make_request(self, _RUN_PATH+"/"+name, _POST, data=input, token=token)
+    """ Run a synchronous execution. 
+        If an output is provided the result is decoded onto the file.
+        In both cases the function returns the HTTP response."""
+    def run_service(self, name, **kwargs):
+        if "input" in kwargs.keys() and kwargs["input"]:
+            exec_input = kwargs["input"]
+            token = self._get_token(name) 
+            
+            send_data = utils.encode_input(exec_input)
+
+            if "timeout" in kwargs.keys() and kwargs["timeout"]:
+                response = utils.make_request(self, _RUN_PATH+"/"+name, _POST, data=send_data, token=token, timeout=kwargs["timeout"])
+            else:
+                response = utils.make_request(self, _RUN_PATH+"/"+name, _POST, data=send_data, token=token)
+            
+            if "output" in kwargs.keys() and kwargs["output"]:
+                utils.decode_output(response.text, kwargs["output"])
+            return response
+        
         return utils.make_request(self, _RUN_PATH+"/"+name, _POST, token=token)
     
-    """ Run an asynchronous execution (not usable at the moment). """
+    """ Run an asynchronous execution (unable at the moment). """
     #TODO
     """ def _run_job(self, name, input_path =""):
             pass 
     """
 
     def _get_token(self, svc):
         service = utils.make_request(self, _SVC_PATH+"/"+svc, _GET)
```

### Comparing `oscar_python-1.0.3/oscar_python/storage.py` & `oscar_python-1.0.4/oscar_python/storage.py`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.3/oscar_python.egg-info/PKG-INFO` & `oscar_python-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
-Name: oscar-python
-Version: 1.0.3
+Name: oscar_python
+Version: 1.0.4
 Summary: OSCAR API for python
 Home-page: https://github.com/grycap/oscar_python
 Author: GRyCAP - Universitat Politecnica de Valencia
 Author-email: calarcon@i3m.upv.es
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## Python OSCAR API
+## Python OSCAR client
 
 [![Build](https://github.com/grycap/oscar_python/actions/workflows/main.yaml/badge.svg)](https://github.com/grycap/oscar_python/actions/workflows/main.yaml)
 ![PyPI](https://img.shields.io/pypi/v/oscar_python)
 
-This package provides an API to interact with OSCAR (https://oscar.grycap.net) clusters and services. It is available on Pypi with the name [oscar-python](https://pypi.org/project/oscar-python/).
+This package provides a client to interact with OSCAR (https://oscar.grycap.net) clusters and services. It is available on Pypi with the name [oscar-python](https://pypi.org/project/oscar-python/).
 
 ### Contents
-- [Python OSCAR API](#python-oscar-api)
+- [Python OSCAR client](#python-oscar-client)
   - [Contents](#contents)
   - [Sample usage](#sample-usage)
-  - [API methods](#api-methods)
+  - [Client methods](#client-methods)
     - [Cluster methods](#cluster-methods)
     - [Service methods](#service-methods)
     - [Logs methods](#logs-methods)
     - [Storage usage](#storage-usage)
 
 ### Sample usage
 
@@ -50,22 +50,22 @@
 ``` python
 from oscar_python.client import Client
 
 client = Client("cluster-id","https://cluster-endpoint", "username", "password", True)
 
 try:
   client.create_service("/absolute_path/cowsay.yaml")
-  res = client.run_service("cowsay", '{"message": "Hi there"}')   
-  if res.status_code == 200:
-      print(res.text)
+  response = client.run_service("cowsay", input = '{"message": "Hi there"}')   
+  if response.status_code == 200:
+      print(response.text)
 except Exception as err:
   print("Failed with: ", err)
 ```
 
-### API methods
+### Client methods
 
 #### Cluster methods
 
 **get_cluster_info**
 ``` python
 # get the cluster information
 info = client.get_cluster_info() # returns an HTTP response or an HTTPError
@@ -109,20 +109,19 @@
 ``` python
 # remove a service 
 response = client.remove_service("service_name") # returns an http response
 ```
 
 **run_service**
 
-The `input` parameter may not be passed if the function doesn't require input.
+ *`input`, `output` and `timeout` are optional parameters.*
 
 ``` python
 # make a synchronous execution 
-response = client.run_service("service_name", input="input") # returns an http response
-
+response = client.run_service("service_name", input="input", output="out.png", timeout=100) # returns an http response
 ```
 
 #### Logs methods
 
 **get_job_logs**
 ``` python
 # get logs of a job
@@ -172,13 +171,7 @@
 ```
 
 **download_file**
 ``` python
 # download a file from a remote path to a local path 
 response = storage_service.download_file("storage_provider", "local_path", "remote_path")
 ```
-
-
-
-
-
-
```

### Comparing `oscar_python-1.0.3/oscar_python.egg-info/SOURCES.txt` & `oscar_python-1.0.4/oscar_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oscar_python-1.0.3/setup.py` & `oscar_python-1.0.4/setup.py`

 * *Files identical despite different names*

