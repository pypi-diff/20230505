# Comparing `tmp/forged-client-0.0.1.tar.gz` & `tmp/forged-client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\rsummers\Documents\repositories\forged-org\forged-clients\forged-py\dist\.tmp-fqi_rg2c\forged-client-0.0.1.tar", last modified: Wed Jan 25 17:48:17 2023, max compression
+gzip compressed data, was "forged-client-0.1.0.tar", last modified: Fri May  5 11:55:57 2023, max compression
```

## Comparing `forged-client-0.0.1.tar` & `forged-client-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-01-25 17:48:17.000000 forged-client-0.0.1/
--rw-rw-rw-   0        0        0      934 2023-01-25 17:48:17.000000 forged-client-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-01-25 17:42:27.000000 forged-client-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-25 17:48:17.000000 forged-client-0.0.1/forged/
--rw-rw-rw-   0        0        0       54 2023-01-24 08:59:47.000000 forged-client-0.0.1/forged/__init__.py
--rw-rw-rw-   0        0        0     5162 2023-01-24 08:59:47.000000 forged-client-0.0.1/forged/client.py
-drwxrwxrwx   0        0        0        0 2023-01-25 17:48:17.000000 forged-client-0.0.1/forged_client.egg-info/
--rw-rw-rw-   0        0        0      934 2023-01-25 17:48:17.000000 forged-client-0.0.1/forged_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-01-25 17:48:17.000000 forged-client-0.0.1/forged_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-25 17:48:17.000000 forged-client-0.0.1/forged_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-01-25 17:48:17.000000 forged-client-0.0.1/forged_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-25 17:48:17.000000 forged-client-0.0.1/forged_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      774 2023-01-25 17:42:27.000000 forged-client-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-25 17:48:17.000000 forged-client-0.0.1/setup.cfg
+drwxr-xr-x   0 yatekii    (501) staff       (20)        0 2023-05-05 11:55:57.511327 forged-client-0.1.0/
+-rw-r--r--   0 yatekii    (501) staff       (20)      980 2023-05-05 11:55:57.511175 forged-client-0.1.0/PKG-INFO
+-rw-r--r--   0 yatekii    (501) staff       (20)      401 2023-05-05 11:38:05.000000 forged-client-0.1.0/README.md
+drwxr-xr-x   0 yatekii    (501) staff       (20)        0 2023-05-05 11:55:57.510216 forged-client-0.1.0/forged/
+-rw-r--r--   0 yatekii    (501) staff       (20)       52 2023-02-24 00:15:36.000000 forged-client-0.1.0/forged/__init__.py
+-rw-r--r--   0 yatekii    (501) staff       (20)     6104 2023-05-05 11:38:05.000000 forged-client-0.1.0/forged/client.py
+drwxr-xr-x   0 yatekii    (501) staff       (20)        0 2023-05-05 11:55:57.511011 forged-client-0.1.0/forged_client.egg-info/
+-rw-r--r--   0 yatekii    (501) staff       (20)      980 2023-05-05 11:55:57.000000 forged-client-0.1.0/forged_client.egg-info/PKG-INFO
+-rw-r--r--   0 yatekii    (501) staff       (20)      244 2023-05-05 11:55:57.000000 forged-client-0.1.0/forged_client.egg-info/SOURCES.txt
+-rw-r--r--   0 yatekii    (501) staff       (20)        1 2023-05-05 11:55:57.000000 forged-client-0.1.0/forged_client.egg-info/dependency_links.txt
+-rw-r--r--   0 yatekii    (501) staff       (20)        9 2023-05-05 11:55:57.000000 forged-client-0.1.0/forged_client.egg-info/requires.txt
+-rw-r--r--   0 yatekii    (501) staff       (20)        7 2023-05-05 11:55:57.000000 forged-client-0.1.0/forged_client.egg-info/top_level.txt
+-rw-r--r--   0 yatekii    (501) staff       (20)      740 2023-05-05 11:40:56.000000 forged-client-0.1.0/pyproject.toml
+-rw-r--r--   0 yatekii    (501) staff       (20)       38 2023-05-05 11:55:57.511365 forged-client-0.1.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `forged-client-0.0.1/PKG-INFO` & `forged-client-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-Metadata-Version: 2.1
-Name: forged-client
-Version: 0.0.1
-Summary: Forged.dev Client library
-Author-email: Ryan Summers <ryan.summers@vertigo-designs.com>, Noah Hüsser <noah@huesser.dev>
-Project-URL: Homepage, https://forged.dev
-Keywords: api,client,database,embedded
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Manufacturing
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: System :: Hardware
-Description-Content-Type: text/markdown
-
-# Forged Python Client
-
-This package is a client to interface with the forged.dev manufacturing/provisioning service.
-
-When used in the automated Forged provisioner UI, uploading data blocks can be accomplished as
-simply as:
-```py
-from forged import Forged
-
-async def main():
-    await Forged.upload_value("my_block", 10.0)
-```
+Metadata-Version: 2.1
+Name: forged-client
+Version: 0.1.0
+Summary: Forged.dev Client library
+Author-email: Ryan Summers <ryan.summers@vertigo-designs.com>, Noah Hüsser <noah@huesser.dev>
+Project-URL: Homepage, https://forged.dev
+Keywords: api,client,database,embedded
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Manufacturing
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: System :: Hardware
+Description-Content-Type: text/markdown
+
+# Forged Python Client
+
+This package is a client to interface with the forged.dev manufacturing/provisioning service.
+
+When used in the automated Forged provisioner UI, uploading data blocks can be accomplished as
+simply as:
+```py
+from forged import Forged
+
+async def main():
+    await Forged.upload_value("my_block", 10.0)
+    blocks = await Forged.blocks()
+    assert blocks["my_block"] == 10.0
+```
```

### Comparing `forged-client-0.0.1/forged/client.py` & `forged-client-0.1.0/forged/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,146 +1,181 @@
-#!/usr/bin/python3
-"""
-Forged client module
-
-Author: Forged.dev
-
-Description: Utilities for uploading data to forged.dev test runs from custom tests.
-"""
-import logging
-import os
-from typing import Union, Dict
-
-import gql
-from gql.transport.aiohttp import AIOHTTPTransport
-
-# The default endpoint to use when connecting to the cloud-based forged.dev service.
-DEFAULT_FORGED_API_ENDPOINT = 'https://api.forged.dev'
-
-class Forged:
-    """ The main method for creating a connection to forged.dev.
-
-    Example:
-    ```
-    # Use a token automatically injected via the environment
-    # Note: You can also pass the token here directly.
-    with Forged() as client:
-        # Assign the value of 3.5 to the block `test_data`
-        client.upload_block("test_data", 3.5)
-    ```
-    """
-
-    def __init__(self, token=None, url=DEFAULT_FORGED_API_ENDPOINT):
-        """ Configure the connection parameters.
-
-        Args:
-            * `token` - The token to use for authentication. If unspecified, the environment
-              variable `FORGED_API_TOKEN` will be used instead.
-            * `url` - The URL to connect to. The default value connects to forged.dev's cloud
-              service.
-        """
-        if not token:
-            token = os.environ.get('FORGED_API_TOKEN')
-
-        # If there's a URL injected by the provisioner into the environment, use that URL instead of
-        # the default.
-        environment_url = os.environ.get('FORGED_API_URL')
-        if environment_url:
-            logging.info('Overriding provided URL to %s', environment_url)
-            url = environment_url
-
-        assert token is not None, 'Please provide a forged API token'
-
-        transport = AIOHTTPTransport(url=url, headers={'Authorization': f'Bearer {token}'})
-        self.client = gql.Client(transport=transport, fetch_schema_from_transport=True)
-        self.session = None
-
-
-    async def __aenter__(self):
-        return await ForgedSession._create(await self.client.__aenter__())
-
-
-    async def __aexit__(self, *args, **kwargs):
-        await self.client.__aexit__(*args, **kwargs)
-
-
-    @classmethod
-    async def upload_value(cls, name: str, value: Union[float, int, str], token=None,
-                           url=DEFAULT_FORGED_API_ENDPOINT):
-        """ Upload a singular value data block to the current run.
-
-        Note:
-            If no token is provided and one is not found in the environment, the block upload is
-            silently ignored.
-
-        Args:
-            * `name` - The name of the block being uploaded.
-            * `value` - The value to upload to the block.
-            * `token` - The token to use for authentication. If unspecified, the environment
-              variable `FORGED_API_TOKEN` will be used instead.
-            * `url` - The URL to connect to. The default value connects to forged.dev's cloud
-              service.
-        """
-        if token is None:
-            token = os.environ.get('FORGED_API_TOKEN')
-
-        if not token:
-            logging.warning('No forged API token was found. Ignoring block upload')
-            return
-
-        async with cls(token, url) as client:
-            await client.upload_value(name, value)
-
-
-class ForgedSession:
-    """ An asynchronous connection with the forged.dev run. """
-
-    @classmethod
-    async def _create(cls, session):
-        """ Create the session from a graphQL connection. """
-        provisioner_query = gql.gql("""
-        query getRunData {
-            currentProvisioner {
-                projectId
-            }
-        }""")
-        provisioner = await session.execute(provisioner_query)
-        project_id = provisioner['currentProvisioner']['projectId']
-        return cls(session, project_id)
-
-
-    def __init__(self, session, project_id: str):
-        """ Constructor """
-        self.session = session
-        self.project_id = project_id
-
-
-    async def upload_value(self, name: str, value: Union[float, int, str]):
-        """ Upload a block that contains a single value. """
-        return await self.upload_block(name, {'value': value})
-
-
-    async def upload_block(self, name: str, data: Dict):
-        """ Upload a block of data to the current run.
-
-        Note:
-            This uploads raw data to the block in an unformatted manner. The user is responsible for
-            constructing the proper data format for the given schema. Use other upload methods if
-            you would like to have the data structured for you.
-
-        Args:
-            * `name` - The name of the block being uploaded.
-            * `data` - The data associated with the block.
-        """
-        block_mutation = gql.gql("""
-        mutation CreateBlock($schemaName: String!, $data: JSON!) {
-            blockCreate(schemaName: $schemaName, data: $data) {
-                id
-            }
-        }""")
-
-        result = await self.session.execute(block_mutation, variable_values={
-            'schemaName': name,
-            'data': data
-        })
-
-        return result['blockCreate']['id']
+#!/usr/bin/python3
+"""
+Forged client module
+
+Author: Forged.dev
+
+Description: Utilities for uploading data to forged.dev test runs from custom tests.
+"""
+import logging
+import os
+from typing import Union, Dict
+
+import gql
+from gql.transport.aiohttp import AIOHTTPTransport
+
+# The default endpoint to use when connecting to the cloud-based forged.dev service.
+DEFAULT_FORGED_API_ENDPOINT = 'https://api.forged.dev'
+
+class Forged:
+    """ The main method for creating a connection to forged.dev.
+
+    Example:
+    ```
+    # Use a token automatically injected via the environment
+    # Note: You can also pass the token here directly.
+    with Forged() as client:
+        # Assign the value of 3.5 to the block `test_data`
+        client.upload_block("test_data", 3.5)
+    ```
+    """
+
+    def __init__(self, token=None, url=DEFAULT_FORGED_API_ENDPOINT):
+        """ Configure the connection parameters.
+
+        Args:
+            * `token` - The token to use for authentication. If unspecified, the environment
+              variable `FORGED_API_TOKEN` will be used instead.
+            * `url` - The URL to connect to. The default value connects to forged.dev's cloud
+              service.
+        """
+        if not token:
+            token = os.environ.get('FORGED_API_TOKEN')
+
+        # If there's a URL injected by the provisioner into the environment, use that URL instead of
+        # the default.
+        environment_url = os.environ.get('FORGED_API_URL')
+        if environment_url:
+            logging.info('Overriding provided URL to %s', environment_url)
+            url = environment_url
+
+        assert token is not None, 'Please provide a forged API token'
+
+        transport = AIOHTTPTransport(url=url, headers={'Authorization': f'Bearer {token}'})
+        self.client = gql.Client(transport=transport, fetch_schema_from_transport=True)
+        self.session = None
+
+
+    async def __aenter__(self):
+        return await ForgedSession._create(await self.client.__aenter__())
+
+
+    async def __aexit__(self, *args, **kwargs):
+        await self.client.__aexit__(*args, **kwargs)
+
+
+    @classmethod
+    async def upload_value(cls, name: str, value: Union[float, int, str], token=None,
+                           url=DEFAULT_FORGED_API_ENDPOINT):
+        """ Upload a singular value data block to the current run.
+
+        Note:
+            If no token is provided and one is not found in the environment, the block upload is
+            silently ignored.
+
+        Args:
+            * `name` - The name of the block being uploaded.
+            * `value` - The value to upload to the block.
+            * `token` - The token to use for authentication. If unspecified, the environment
+              variable `FORGED_API_TOKEN` will be used instead.
+            * `url` - The URL to connect to. The default value connects to forged.dev's cloud
+              service.
+        """
+        if token is None:
+            token = os.environ.get('FORGED_API_TOKEN')
+
+        if not token:
+            logging.warning('No forged API token was found. Ignoring block upload')
+            return
+
+        async with cls(token, url) as client:
+            await client.upload_value(name, value)
+
+    @classmethod
+    async def blocks(cls, token=None, url=DEFAULT_FORGED_API_ENDPOINT):
+        """ Get all of the blocks for the current device. """
+        async with cls(token, url) as client:
+            return await client.blocks()
+
+
+class ForgedSession:
+    """ An asynchronous connection with the forged.dev run. """
+
+    @classmethod
+    async def _create(cls, session):
+        """ Create the session from a graphQL connection. """
+        provisioner_query = gql.gql("""
+        query getRunData {
+            currentProvisioner {
+                projectId
+            }
+        }""")
+        provisioner = await session.execute(provisioner_query)
+        project_id = provisioner['currentProvisioner']['projectId']
+        return cls(session, project_id)
+
+
+    def __init__(self, session, project_id: str):
+        """ Constructor """
+        self.session = session
+        self.project_id = project_id
+
+
+    async def blocks(self):
+        blocks_query = gql.gql("""
+        query getBlocks {
+            currentProvisioner {
+                currentRun {
+                    blocks {
+                        dataDecoded
+                        schema {
+                            name
+                        }
+                    }
+                }
+            }
+        }
+        """)
+
+        query = await self.session.execute(blocks_query)
+
+        blocks = {}
+        for block in query['currentProvisioner']['currentRun']['blocks']:
+            data = block['dataDecoded']
+            blocks[block['schema']['name']] = block['dataDecoded'][list(data.keys())[0]]
+
+        return blocks
+
+
+    async def upload_value(self, name: str, value: Union[float, int, str]):
+        """ Upload a block that contains a single value. """
+        try:
+            upload = await self.upload_block(name, {'value': value})
+        except gql.transport.exceptions.TransportQueryError as error:
+            logging.warning('Failed to upload %s: %s', name, error)
+
+
+    async def upload_block(self, name: str, data: Dict):
+        """ Upload a block of data to the current run.
+
+        Note:
+            This uploads raw data to the block in an unformatted manner. The user is responsible for
+            constructing the proper data format for the given schema. Use other upload methods if
+            you would like to have the data structured for you.
+
+        Args:
+            * `name` - The name of the block being uploaded.
+            * `data` - The data associated with the block.
+        """
+        block_mutation = gql.gql("""
+        mutation CreateBlock($schemaName: String!, $data: JSON!) {
+            blockCreate(schemaName: $schemaName, data: $data) {
+                id
+            }
+        }""")
+
+        result = await self.session.execute(block_mutation, variable_values={
+            'schemaName': name,
+            'data': data
+        })
+
+        return result['blockCreate']['id']
```

### Comparing `forged-client-0.0.1/forged_client.egg-info/PKG-INFO` & `forged-client-0.1.0/forged_client.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-Metadata-Version: 2.1
-Name: forged-client
-Version: 0.0.1
-Summary: Forged.dev Client library
-Author-email: Ryan Summers <ryan.summers@vertigo-designs.com>, Noah Hüsser <noah@huesser.dev>
-Project-URL: Homepage, https://forged.dev
-Keywords: api,client,database,embedded
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Manufacturing
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: System :: Hardware
-Description-Content-Type: text/markdown
-
-# Forged Python Client
-
-This package is a client to interface with the forged.dev manufacturing/provisioning service.
-
-When used in the automated Forged provisioner UI, uploading data blocks can be accomplished as
-simply as:
-```py
-from forged import Forged
-
-async def main():
-    await Forged.upload_value("my_block", 10.0)
-```
+Metadata-Version: 2.1
+Name: forged-client
+Version: 0.1.0
+Summary: Forged.dev Client library
+Author-email: Ryan Summers <ryan.summers@vertigo-designs.com>, Noah Hüsser <noah@huesser.dev>
+Project-URL: Homepage, https://forged.dev
+Keywords: api,client,database,embedded
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Manufacturing
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: System :: Hardware
+Description-Content-Type: text/markdown
+
+# Forged Python Client
+
+This package is a client to interface with the forged.dev manufacturing/provisioning service.
+
+When used in the automated Forged provisioner UI, uploading data blocks can be accomplished as
+simply as:
+```py
+from forged import Forged
+
+async def main():
+    await Forged.upload_value("my_block", 10.0)
+    blocks = await Forged.blocks()
+    assert blocks["my_block"] == 10.0
+```
```

### Comparing `forged-client-0.0.1/pyproject.toml` & `forged-client-0.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-[build-system]
-requires = ["setuptools", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "forged-client"
-description = "Forged.dev Client library"
-version = "0.0.1"
-readme = "README.md"
-authors = [
-    { name = "Ryan Summers", email = "ryan.summers@vertigo-designs.com" },
-    { name = "Noah Hüsser", email = "noah@huesser.dev" },
-]
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Intended Audience :: Developers",
-    "Intended Audience :: Manufacturing",
-    "License :: OSI Approved :: MIT License",
-    "Topic :: Scientific/Engineering",
-    "Topic :: System :: Hardware",
-]
-keywords = ["api", "client", "database", "embedded"]
-dependencies = [
-    "gql[all]"
-]
-
-[project.urls]
-Homepage = "https://forged.dev"
+[build-system]
+requires = ["setuptools", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "forged-client"
+description = "Forged.dev Client library"
+version = "0.1.0"
+readme = "README.md"
+authors = [
+    { name = "Ryan Summers", email = "ryan.summers@vertigo-designs.com" },
+    { name = "Noah Hüsser", email = "noah@huesser.dev" },
+]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Manufacturing",
+    "License :: OSI Approved :: MIT License",
+    "Topic :: Scientific/Engineering",
+    "Topic :: System :: Hardware",
+]
+keywords = ["api", "client", "database", "embedded"]
+dependencies = ["gql[all]"]
+
+[project.urls]
+Homepage = "https://forged.dev"
```

