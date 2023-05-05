# Comparing `tmp/autoretouch-0.0.2.tar.gz` & `tmp/autoretouch-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/oliverallweyer/data/repos/autoretouch/api-clients/python-client/dist/tmpftmvycjz/autoretouch-0.0.2.tar", last modified: Mon May 23 07:35:04 2022, max compression
+gzip compressed data, was "dist/autoretouch-0.1.0.tar", last modified: Fri May  5 08:29:13 2023, max compression
```

## Comparing `autoretouch-0.0.2.tar` & `autoretouch-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 oliverallweyer   (501) staff       (20)        0 2022-05-23 07:35:04.000000 autoretouch-0.0.2/
--rw-r--r--   0 oliverallweyer   (501) staff       (20)      644 2021-12-17 15:17:06.000000 autoretouch-0.0.2/LICENSE
--rw-r--r--   0 oliverallweyer   (501) staff       (20)     4737 2022-05-23 07:35:04.000000 autoretouch-0.0.2/PKG-INFO
--rw-r--r--   0 oliverallweyer   (501) staff       (20)     4391 2022-05-20 12:50:25.000000 autoretouch-0.0.2/README.md
-drwxr-xr-x   0 oliverallweyer   (501) staff       (20)        0 2022-05-23 07:35:04.000000 autoretouch-0.0.2/autoretouch/
--rw-r--r--   0 oliverallweyer   (501) staff       (20)      695 2022-05-20 12:06:55.000000 autoretouch-0.0.2/autoretouch/.autoretouch-complete.fish
--rw-r--r--   0 oliverallweyer   (501) staff       (20)     1002 2022-05-20 11:11:22.000000 autoretouch-0.0.2/autoretouch/.autoretouch-complete.zsh
--rw-r--r--   0 oliverallweyer   (501) staff       (20)        0 2022-05-20 11:11:22.000000 autoretouch-0.0.2/autoretouch/__init__.py
-drwxr-xr-x   0 oliverallweyer   (501) staff       (20)        0 2022-05-23 07:35:04.000000 autoretouch-0.0.2/autoretouch/api_client/
--rw-r--r--   0 oliverallweyer   (501) staff       (20)        0 2022-05-20 11:11:22.000000 autoretouch-0.0.2/autoretouch/api_client/__init__.py
--rw-r--r--   0 oliverallweyer   (501) staff       (20)     4889 2022-05-20 11:41:44.000000 autoretouch-0.0.2/autoretouch/api_client/authenticator.py
--rw-r--r--   0 oliverallweyer   (501) staff       (20)    25100 2022-05-20 11:55:29.000000 autoretouch-0.0.2/autoretouch/api_client/client.py
--rw-r--r--   0 oliverallweyer   (501) staff       (20)     2615 2022-05-20 11:11:22.000000 autoretouch-0.0.2/autoretouch/api_client/model.py
-drwxr-xr-x   0 oliverallweyer   (501) staff       (20)        0 2022-05-23 07:35:04.000000 autoretouch-0.0.2/autoretouch/cli/
--rw-r--r--   0 oliverallweyer   (501) staff       (20)        0 2022-05-20 11:11:22.000000 autoretouch-0.0.2/autoretouch/cli/__init__.py
--rw-r--r--   0 oliverallweyer   (501) staff       (20)     8530 2022-05-20 11:54:11.000000 autoretouch-0.0.2/autoretouch/cli/commands.py
-drwxr-xr-x   0 oliverallweyer   (501) staff       (20)        0 2022-05-23 07:35:04.000000 autoretouch-0.0.2/autoretouch.egg-info/
--rw-r--r--   0 oliverallweyer   (501) staff       (20)     4737 2022-05-23 07:35:04.000000 autoretouch-0.0.2/autoretouch.egg-info/PKG-INFO
--rw-r--r--   0 oliverallweyer   (501) staff       (20)      597 2022-05-23 07:35:04.000000 autoretouch-0.0.2/autoretouch.egg-info/SOURCES.txt
--rw-r--r--   0 oliverallweyer   (501) staff       (20)        1 2022-05-23 07:35:04.000000 autoretouch-0.0.2/autoretouch.egg-info/dependency_links.txt
--rw-r--r--   0 oliverallweyer   (501) staff       (20)       73 2022-05-23 07:35:04.000000 autoretouch-0.0.2/autoretouch.egg-info/entry_points.txt
--rw-r--r--   0 oliverallweyer   (501) staff       (20)       39 2022-05-23 07:35:04.000000 autoretouch-0.0.2/autoretouch.egg-info/requires.txt
--rw-r--r--   0 oliverallweyer   (501) staff       (20)       12 2022-05-23 07:35:04.000000 autoretouch-0.0.2/autoretouch.egg-info/top_level.txt
--rw-r--r--   0 oliverallweyer   (501) staff       (20)       85 2022-05-20 11:11:22.000000 autoretouch-0.0.2/pyproject.toml
--rw-r--r--   0 oliverallweyer   (501) staff       (20)       38 2022-05-23 07:35:04.000000 autoretouch-0.0.2/setup.cfg
--rw-r--r--   0 oliverallweyer   (501) staff       (20)     3695 2022-05-20 14:55:27.000000 autoretouch-0.0.2/setup.py
-drwxr-xr-x   0 oliverallweyer   (501) staff       (20)        0 2022-05-23 07:35:04.000000 autoretouch-0.0.2/test/
--rw-r--r--   0 oliverallweyer   (501) staff       (20)     3073 2022-05-20 11:11:22.000000 autoretouch-0.0.2/test/test_authenticator.py
--rw-r--r--   0 oliverallweyer   (501) staff       (20)    11118 2022-05-20 11:11:22.000000 autoretouch-0.0.2/test/test_client.py
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-05-05 08:29:13.000000 autoretouch-0.1.0/
+-rw-r--r--   0 antoine    (501) staff       (20)      644 2022-01-19 09:45:07.000000 autoretouch-0.1.0/LICENSE
+-rw-r--r--   0 antoine    (501) staff       (20)     5205 2023-05-05 08:29:13.000000 autoretouch-0.1.0/PKG-INFO
+-rw-r--r--   0 antoine    (501) staff       (20)     4859 2023-05-05 08:12:06.000000 autoretouch-0.1.0/README.md
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch/
+-rw-r--r--   0 antoine    (501) staff       (20)      695 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/.autoretouch-complete.fish
+-rw-r--r--   0 antoine    (501) staff       (20)     1002 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/.autoretouch-complete.zsh
+-rw-r--r--   0 antoine    (501) staff       (20)        0 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/__init__.py
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch/api_client/
+-rw-r--r--   0 antoine    (501) staff       (20)        0 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/api_client/__init__.py
+-rw-r--r--   0 antoine    (501) staff       (20)     4889 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/api_client/authenticator.py
+-rw-r--r--   0 antoine    (501) staff       (20)    25678 2023-05-05 08:12:06.000000 autoretouch-0.1.0/autoretouch/api_client/client.py
+-rw-r--r--   0 antoine    (501) staff       (20)     2615 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/api_client/model.py
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch/cli/
+-rw-r--r--   0 antoine    (501) staff       (20)        0 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/cli/__init__.py
+-rw-r--r--   0 antoine    (501) staff       (20)     8530 2022-05-23 07:09:43.000000 autoretouch-0.1.0/autoretouch/cli/commands.py
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch.egg-info/
+-rw-r--r--   0 antoine    (501) staff       (20)     5205 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch.egg-info/PKG-INFO
+-rw-r--r--   0 antoine    (501) staff       (20)      597 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch.egg-info/SOURCES.txt
+-rw-r--r--   0 antoine    (501) staff       (20)        1 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch.egg-info/dependency_links.txt
+-rw-r--r--   0 antoine    (501) staff       (20)       73 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch.egg-info/entry_points.txt
+-rw-r--r--   0 antoine    (501) staff       (20)       39 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch.egg-info/requires.txt
+-rw-r--r--   0 antoine    (501) staff       (20)       12 2023-05-05 08:29:13.000000 autoretouch-0.1.0/autoretouch.egg-info/top_level.txt
+-rw-r--r--   0 antoine    (501) staff       (20)       85 2022-05-23 07:09:43.000000 autoretouch-0.1.0/pyproject.toml
+-rw-r--r--   0 antoine    (501) staff       (20)       38 2023-05-05 08:29:13.000000 autoretouch-0.1.0/setup.cfg
+-rw-r--r--   0 antoine    (501) staff       (20)     3695 2023-05-05 08:12:06.000000 autoretouch-0.1.0/setup.py
+drwxr-xr-x   0 antoine    (501) staff       (20)        0 2023-05-05 08:29:13.000000 autoretouch-0.1.0/test/
+-rw-r--r--   0 antoine    (501) staff       (20)     3073 2023-05-05 08:12:06.000000 autoretouch-0.1.0/test/test_authenticator.py
+-rw-r--r--   0 antoine    (501) staff       (20)    11658 2023-05-05 08:12:06.000000 autoretouch-0.1.0/test/test_client.py
```

### Comparing `autoretouch-0.0.2/LICENSE` & `autoretouch-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoretouch-0.0.2/PKG-INFO` & `autoretouch-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: autoretouch
-Version: 0.0.2
+Version: 0.1.0
 Summary: cli and python package to communicate with the autoRetouch API
 Author: ['Antoine Daurat <antoine@autoretouch.com>', 'Oliver Allweyer <oliver@autoretouch.com>', 'Till Lorentzen <till@autoretouch.com>']
 License: BSD Zero
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # autoRetouch client
 
 ## Installation
 
 Prerequisites: Sign up for free at https://app.autoretouch.com.
 
 ### from pypi
 
-```python
+```shell
 pip install autoretouch
 ```
 
 ### for development
 
 clone this repo and then
 ```
@@ -74,43 +74,56 @@
 ##### Batch 
 
 In most cases, you would like to process images according to some workflow within the scope of an organization.
 To do so, you can simply
 
 ```python3
 from autoretouch.api_client.client import AutoRetouchAPIClient
+from uuid import UUID
 
 organization_id = "e722e62e-5b2e-48e1-8638-25890e7279e3"
 
 ar_client = AutoRetouchAPIClient(
     organization_id=organization_id,
     # by default the client saves and reloads your credentials here:
     credentials_path="~/.config/autoretouch-credentials.json"
 )
 
 workflow_id = "26740cd0-3a04-4329-8ba2-e0d6de5a4aaf"
 input_dir = "images_to_retouch/"
 output_dir = "retouched_images/"
 
 # starts a thread for each image and download the results to output_dir
-ar_client.process_batch(workflow_id, input_dir, output_dir)
+ar_client.process_folder(input_dir, output_dir, UUID(workflow_id))
 ```
 ---
 **Note**
 
 - Get your `organization_id` from https://app.autoretouch.com/organization > Copy Organization ID.
 - Get your `workflow_id` from https://app.autoretouch.com/workflows > `⋮` > Workflow API Information > id.
 ---
 
 ##### Single Image
 
 If you wish to process a single image with a workflow, you can do
 
 ```python
-ar_client.process_image("my_image.png", workflow_id, output_dir)
+from autoretouch.api_client.client import AutoRetouchAPIClient
+from uuid import UUID
+
+organization_id = "e722e62e-5b2e-48e1-8638-25890e7279e3"
+
+ar_client = AutoRetouchAPIClient(
+    organization_id=organization_id,
+    # by default the client saves and reloads your credentials here:
+    credentials_path="~/.config/autoretouch-credentials.json"
+)
+workflow_id = "26740cd0-3a04-4329-8ba2-e0d6de5a4aaf"
+output_dir = "retouched_images/"
+ar_client.process_image("my_image.png", output_dir, UUID(workflow_id))
 ```
 
 This is the method called internally by `proces_batch`. It will 
 1. upload the image
 2. start an execution
 3. poll every 2 seconds for the status of the execution
 4. download the result to `output_dir` or return `False` if the execution failed
```

### Comparing `autoretouch-0.0.2/README.md` & `autoretouch-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## Installation
 
 Prerequisites: Sign up for free at https://app.autoretouch.com.
 
 ### from pypi
 
-```python
+```shell
 pip install autoretouch
 ```
 
 ### for development
 
 clone this repo and then
 ```
@@ -65,43 +65,56 @@
 ##### Batch 
 
 In most cases, you would like to process images according to some workflow within the scope of an organization.
 To do so, you can simply
 
 ```python3
 from autoretouch.api_client.client import AutoRetouchAPIClient
+from uuid import UUID
 
 organization_id = "e722e62e-5b2e-48e1-8638-25890e7279e3"
 
 ar_client = AutoRetouchAPIClient(
     organization_id=organization_id,
     # by default the client saves and reloads your credentials here:
     credentials_path="~/.config/autoretouch-credentials.json"
 )
 
 workflow_id = "26740cd0-3a04-4329-8ba2-e0d6de5a4aaf"
 input_dir = "images_to_retouch/"
 output_dir = "retouched_images/"
 
 # starts a thread for each image and download the results to output_dir
-ar_client.process_batch(workflow_id, input_dir, output_dir)
+ar_client.process_folder(input_dir, output_dir, UUID(workflow_id))
 ```
 ---
 **Note**
 
 - Get your `organization_id` from https://app.autoretouch.com/organization > Copy Organization ID.
 - Get your `workflow_id` from https://app.autoretouch.com/workflows > `⋮` > Workflow API Information > id.
 ---
 
 ##### Single Image
 
 If you wish to process a single image with a workflow, you can do
 
 ```python
-ar_client.process_image("my_image.png", workflow_id, output_dir)
+from autoretouch.api_client.client import AutoRetouchAPIClient
+from uuid import UUID
+
+organization_id = "e722e62e-5b2e-48e1-8638-25890e7279e3"
+
+ar_client = AutoRetouchAPIClient(
+    organization_id=organization_id,
+    # by default the client saves and reloads your credentials here:
+    credentials_path="~/.config/autoretouch-credentials.json"
+)
+workflow_id = "26740cd0-3a04-4329-8ba2-e0d6de5a4aaf"
+output_dir = "retouched_images/"
+ar_client.process_image("my_image.png", output_dir, UUID(workflow_id))
 ```
 
 This is the method called internally by `proces_batch`. It will 
 1. upload the image
 2. start an execution
 3. poll every 2 seconds for the status of the execution
 4. download the result to `output_dir` or return `False` if the execution failed
```

### Comparing `autoretouch-0.0.2/autoretouch/.autoretouch-complete.fish` & `autoretouch-0.1.0/autoretouch/.autoretouch-complete.fish`

 * *Files identical despite different names*

### Comparing `autoretouch-0.0.2/autoretouch/.autoretouch-complete.zsh` & `autoretouch-0.1.0/autoretouch/.autoretouch-complete.zsh`

 * *Files identical despite different names*

### Comparing `autoretouch-0.0.2/autoretouch/api_client/authenticator.py` & `autoretouch-0.1.0/autoretouch/api_client/authenticator.py`

 * *Files identical despite different names*

### Comparing `autoretouch-0.0.2/autoretouch/api_client/client.py` & `autoretouch-0.1.0/autoretouch/api_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     "AUTORETOUCH_ORGANIZATION_ID",
     USER_CONFIG["organization"]["id"]
 )
 DEFAULT_WORKFLOW_ID = os.environ.get(
     "AUTORETOUCH_WORKFLOW_ID",
     USER_CONFIG["workflow"]["id"]
 )
-DEFAULT_USER_AGENT = "Autoretouch-Python-Api-Client-0.0.2"
+DEFAULT_USER_AGENT = "Autoretouch-Python-Api-Client-0.1.0"
 
 T = TypeVar("T", bound=Callable)
 
 
 class AutoRetouchAPIClient:
     """
     autoRetouch API client
@@ -303,14 +303,26 @@
         with BytesIO(image_content) as file:
             files = [("file", (image_name, file, mimetype))]
             response = requests.post(url=url, headers=self.base_headers, files=files)
             logger.debug(f"{url} answered with status {response.status_code}")
         response.raise_for_status()
         return response.content.decode(response.encoding)
 
+    def upload_image_from_urls(
+            self,
+            public_accessible_urls: Dict[str, str],
+            organization_id: Optional[UUID] = None,
+    ) -> Dict[str, str]:
+        logger.info("uploading image from public urls...")
+        self.authenticated()
+        organization_id = self._get_organization_id(organization_id)
+        url = f"{self.api_config.BASE_API_URL_CURRENT}/upload?organization={organization_id}"
+        response = requests.post(url=url, headers=self.base_headers, json={"urls": public_accessible_urls})
+        return response.json()["urls"]
+
     def create_workflow_execution_for_image_file(
             self,
             workflow_id: UUID,
             image_path: str,
             labels: Optional[Dict[str, str]] = None,
             workflow_version_id: Optional[UUID] = None,
             organization_id: Optional[UUID] = None,
```

### Comparing `autoretouch-0.0.2/autoretouch/api_client/model.py` & `autoretouch-0.1.0/autoretouch/api_client/model.py`

 * *Files identical despite different names*

### Comparing `autoretouch-0.0.2/autoretouch/cli/commands.py` & `autoretouch-0.1.0/autoretouch/cli/commands.py`

 * *Files identical despite different names*

### Comparing `autoretouch-0.0.2/autoretouch.egg-info/PKG-INFO` & `autoretouch-0.1.0/autoretouch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: autoretouch
-Version: 0.0.2
+Version: 0.1.0
 Summary: cli and python package to communicate with the autoRetouch API
 Author: ['Antoine Daurat <antoine@autoretouch.com>', 'Oliver Allweyer <oliver@autoretouch.com>', 'Till Lorentzen <till@autoretouch.com>']
 License: BSD Zero
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # autoRetouch client
 
 ## Installation
 
 Prerequisites: Sign up for free at https://app.autoretouch.com.
 
 ### from pypi
 
-```python
+```shell
 pip install autoretouch
 ```
 
 ### for development
 
 clone this repo and then
 ```
@@ -74,43 +74,56 @@
 ##### Batch 
 
 In most cases, you would like to process images according to some workflow within the scope of an organization.
 To do so, you can simply
 
 ```python3
 from autoretouch.api_client.client import AutoRetouchAPIClient
+from uuid import UUID
 
 organization_id = "e722e62e-5b2e-48e1-8638-25890e7279e3"
 
 ar_client = AutoRetouchAPIClient(
     organization_id=organization_id,
     # by default the client saves and reloads your credentials here:
     credentials_path="~/.config/autoretouch-credentials.json"
 )
 
 workflow_id = "26740cd0-3a04-4329-8ba2-e0d6de5a4aaf"
 input_dir = "images_to_retouch/"
 output_dir = "retouched_images/"
 
 # starts a thread for each image and download the results to output_dir
-ar_client.process_batch(workflow_id, input_dir, output_dir)
+ar_client.process_folder(input_dir, output_dir, UUID(workflow_id))
 ```
 ---
 **Note**
 
 - Get your `organization_id` from https://app.autoretouch.com/organization > Copy Organization ID.
 - Get your `workflow_id` from https://app.autoretouch.com/workflows > `⋮` > Workflow API Information > id.
 ---
 
 ##### Single Image
 
 If you wish to process a single image with a workflow, you can do
 
 ```python
-ar_client.process_image("my_image.png", workflow_id, output_dir)
+from autoretouch.api_client.client import AutoRetouchAPIClient
+from uuid import UUID
+
+organization_id = "e722e62e-5b2e-48e1-8638-25890e7279e3"
+
+ar_client = AutoRetouchAPIClient(
+    organization_id=organization_id,
+    # by default the client saves and reloads your credentials here:
+    credentials_path="~/.config/autoretouch-credentials.json"
+)
+workflow_id = "26740cd0-3a04-4329-8ba2-e0d6de5a4aaf"
+output_dir = "retouched_images/"
+ar_client.process_image("my_image.png", output_dir, UUID(workflow_id))
 ```
 
 This is the method called internally by `proces_batch`. It will 
 1. upload the image
 2. start an execution
 3. poll every 2 seconds for the status of the execution
 4. download the result to `output_dir` or return `False` if the execution failed
```

### Comparing `autoretouch-0.0.2/autoretouch.egg-info/SOURCES.txt` & `autoretouch-0.1.0/autoretouch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoretouch-0.0.2/setup.py` & `autoretouch-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 
 with open("README.md", "r") as f:
     README = f.read()
 
 setup(
     name="autoretouch",
-    version="0.0.2",
+    version="0.1.0",
     author=[
         "Antoine Daurat <antoine@autoretouch.com>",
         "Oliver Allweyer <oliver@autoretouch.com>",
         "Till Lorentzen <till@autoretouch.com>"
     ],
     description="cli and python package to communicate with the autoRetouch API",
     long_description=README,
```

### Comparing `autoretouch-0.0.2/test/test_authenticator.py` & `autoretouch-0.1.0/test/test_authenticator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from assertpy import assert_that
 import os
 import signal
 
 from autoretouch.api_client.client import AutoRetouchAPIClient
 from test.api_config_dev import CONFIG_DEV
 
-USER_AGENT = "Python-Unit-Test-0.0.1"
+USER_AGENT = "Python-Unit-Test-0.1.0"
 
 
 class TestAuthenticator(TestCase):
 
     test_org_id = "d92fe1cd-7166-4f5d-b43f-a100758d42c9"
     refresh_token = ""
     credentials_path = "../tmp/test-credentials.json"
```

### Comparing `autoretouch-0.0.2/test/test_client.py` & `autoretouch-0.1.0/test/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from autoretouch.api_client.client import (
     AutoRetouchAPIClient,
 )
 from autoretouch.api_client.model import Organization, Workflow, WorkflowExecution
 from test.api_config_dev import CONFIG_DEV
 
 CREDENTIALS_PATH = "../tmp/credentials.json"
-USER_AGENT = "Python-Unit-Test-0.0.1"
+USER_AGENT = "Python-Unit-Test-0.1.0"
 
 
 class HealthApiIntegrationTest(TestCase):
     def setUp(self) -> None:
-        self.client = AutoRetouchAPIClient(api_config=CONFIG_DEV, user_agent="Python-Unit-Test-0.0.1")
+        self.client = AutoRetouchAPIClient(api_config=CONFIG_DEV, user_agent=USER_AGENT)
 
     def test_health(self):
         assert_that(self.client.get_api_status()).is_equal_to(200)
 
 
 class APIClientIntegrationTest(TestCase):
     # Warning! This integration test runs real workflow executions
@@ -37,18 +37,21 @@
         self.assertIsNotNone(input_image_content_hash)
         self.assertEqual(
             input_image_content_hash,
             "8bcac2125bd98cd96ba75667b9a8832024970ac05bf4123f864bb63bcfefbcf7",
         )
 
         workflow_execution_id = (
-            self.client.create_workflow_execution_for_image_reference(workflow.id, input_image_content_hash,
-                                                                      "input_image.jpeg", "image/jpeg",
-                                                                      {"myLabel": "myValue"}, workflow.version,
-                                                                      organization.id)
+            self.client.create_workflow_execution_for_image_reference(
+                workflow_id=workflow.id,
+                image_content_hash=input_image_content_hash,
+                image_name="input_image.jpeg",
+                labels={"myLabel": "myValue"},
+                workflow_version_id=workflow.version,
+                organization_id=organization.id)
         )
         self.assertIsNotNone(workflow_execution_id)
 
         self.__assert_execution_has_started(
             organization,
             workflow,
             workflow_execution_id,
@@ -94,14 +97,24 @@
         input_image_content_hash = self.client.upload_image("../assets/input_image.jpeg", organization.id)
         self.assertIsNotNone(input_image_content_hash)
         self.assertEqual(
             input_image_content_hash,
             "8bcac2125bd98cd96ba75667b9a8832024970ac05bf4123f864bb63bcfefbcf7",
         )
 
+    def test_upload_image_from_urls(self):
+        organization, _ = self.__get_organization_and_workflow()
+        given_urls = {"input_image.jpeg": "https://raw.githubusercontent.com/autoretouch/autoretouch-python-client/main/assets/input_image.jpeg"}
+        result_image_content_hashes = self.client.upload_image_from_urls(given_urls, organization.id)
+        self.assertIsNotNone(result_image_content_hashes)
+        self.assertEqual(
+            result_image_content_hashes.get("input_image.jpeg"),
+            "8bcac2125bd98cd96ba75667b9a8832024970ac05bf4123f864bb63bcfefbcf7",
+        )
+
     def test_start_workflow_execution_immediately_and_wait(self):
         organization, workflow = self.__get_organization_and_workflow()
 
         workflow_execution_id = self.client.create_workflow_execution_for_image_file(workflow.id,
                                                                                      "../assets/input_image.jpeg",
                                                                                      {"myLabel": "myValue"},
                                                                                      workflow.version, organization.id)
@@ -178,15 +191,15 @@
         assert_that([entry.id for entry in workflow_executions.entries]).contains(
             workflow_execution_id
         )
 
     def __wait_for_execution_to_complete(
             self, organization: Organization, workflow_execution_id: UUID
     ):
-        timeout = 10
+        timeout = 30
         interval = 1
         seconds_waited = 0
         while seconds_waited < timeout:
             execution_details = self.client.get_workflow_execution_details(workflow_execution_id, organization.id)
             if execution_details.status == "COMPLETED":
                 return
             elif (
```

