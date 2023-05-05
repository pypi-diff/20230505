# Comparing `tmp/scw_serverless-1.0.1.tar.gz` & `tmp/scw_serverless-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scw_serverless-1.0.1.tar", max compression
+gzip compressed data, was "scw_serverless-1.0.2.tar", max compression
```

## Comparing `scw_serverless-1.0.1.tar` & `scw_serverless-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      499 2023-04-11 11:30:00.787325 scw_serverless-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1065 2023-02-02 17:20:42.069490 scw_serverless-1.0.1/LICENSE
--rw-r--r--   0        0        0     2495 2023-02-02 17:20:42.069490 scw_serverless-1.0.1/README.md
--rw-r--r--   0        0        0     2974 2023-04-12 12:07:11.489147 scw_serverless-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       54 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/__init__.py
--rw-r--r--   0        0        0     4716 2023-04-04 08:42:26.463081 scw_serverless-1.0.1/scw_serverless/app.py
--rw-r--r--   0        0        0     6100 2023-04-04 08:42:26.463081 scw_serverless-1.0.1/scw_serverless/cli.py
--rw-r--r--   0        0        0       31 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/__init__.py
--rw-r--r--   0        0        0     5104 2023-04-04 13:54:31.192478 scw_serverless-1.0.1/scw_serverless/config/function.py
--rw-r--r--   0        0        0      138 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/generators/__init__.py
--rw-r--r--   0        0        0      219 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/generators/generator.py
--rw-r--r--   0        0        0     4169 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/generators/serverless_framework.py
--rw-r--r--   0        0        0     7045 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/generators/terraform.py
--rw-r--r--   0        0        0     1247 2023-04-04 08:42:26.463081 scw_serverless-1.0.1/scw_serverless/config/route.py
--rw-r--r--   0        0        0       14 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/templates/.gitignore
--rw-r--r--   0        0        0      414 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/templates/serverless.yml
--rw-r--r--   0        0        0      426 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/templates/terraform.tf.json
--rw-r--r--   0        0        0      327 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/config/utils.py
--rw-r--r--   0        0        0     3532 2023-04-04 08:42:26.463081 scw_serverless-1.0.1/scw_serverless/dependencies_manager.py
--rw-r--r--   0        0        0        0 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/deploy/__init__.py
--rw-r--r--   0        0        0      172 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/deploy/backends/__init__.py
--rw-r--r--   0        0        0    11072 2023-03-13 13:34:16.012571 scw_serverless-1.0.1/scw_serverless/deploy/backends/scaleway_api_backend.py
--rw-r--r--   0        0        0      524 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/deploy/backends/serverless_backend.py
--rw-r--r--   0        0        0     1700 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/deploy/backends/serverless_framework_backend.py
--rw-r--r--   0        0        0        0 2023-04-04 08:42:26.463081 scw_serverless-1.0.1/scw_serverless/gateway/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-04 08:42:26.463081 scw_serverless-1.0.1/scw_serverless/gateway/gateway_api_client.py
--rw-r--r--   0        0        0     2341 2023-04-11 15:47:24.983578 scw_serverless-1.0.1/scw_serverless/gateway/gateway_manager.py
--rw-r--r--   0        0        0     2262 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/logger.py
--rw-r--r--   0        0        0      137 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/triggers/__init__.py
--rw-r--r--   0        0        0     1405 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/triggers/cron.py
--rw-r--r--   0        0        0        0 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/utils/__init__.py
--rw-r--r--   0        0        0      239 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/utils/commands.py
--rw-r--r--   0        0        0     1864 2023-03-14 08:51:57.235841 scw_serverless-1.0.1/scw_serverless/utils/credentials.py
--rw-r--r--   0        0        0      590 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/utils/files.py
--rw-r--r--   0        0        0     1476 2023-02-27 15:17:33.009496 scw_serverless-1.0.1/scw_serverless/utils/loader.py
--rw-r--r--   0        0        0      761 2023-02-02 17:20:42.073490 scw_serverless-1.0.1/scw_serverless/utils/string.py
--rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 scw_serverless-1.0.1/setup.py
--rw-r--r--   0        0        0     4009 1970-01-01 00:00:00.000000 scw_serverless-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      617 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1065 2023-05-04 12:54:46.772897 scw_serverless-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2673 2023-05-04 12:54:46.772897 scw_serverless-1.0.2/README.md
+-rw-r--r--   0        0        0     2981 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/__init__.py
+-rw-r--r--   0        0        0     5001 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/app.py
+-rw-r--r--   0        0        0     6100 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/cli.py
+-rw-r--r--   0        0        0       31 2023-05-04 12:54:46.776897 scw_serverless-1.0.2/scw_serverless/config/__init__.py
+-rw-r--r--   0        0        0     5109 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/config/function.py
+-rw-r--r--   0        0        0      138 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/config/generators/__init__.py
+-rw-r--r--   0        0        0      219 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/config/generators/generator.py
+-rw-r--r--   0        0        0     4169 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/config/generators/serverless_framework.py
+-rw-r--r--   0        0        0     7045 2023-05-05 15:18:22.598335 scw_serverless-1.0.2/scw_serverless/config/generators/terraform.py
+-rw-r--r--   0        0        0     1247 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/config/route.py
+-rw-r--r--   0        0        0       14 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/config/templates/.gitignore
+-rw-r--r--   0        0        0      414 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/config/templates/serverless.yml
+-rw-r--r--   0        0        0      426 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/config/templates/terraform.tf.json
+-rw-r--r--   0        0        0      327 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/config/utils.py
+-rw-r--r--   0        0        0     3532 2023-05-05 15:21:28.107228 scw_serverless-1.0.2/scw_serverless/dependencies_manager.py
+-rw-r--r--   0        0        0        0 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/deploy/__init__.py
+-rw-r--r--   0        0        0      172 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/deploy/backends/__init__.py
+-rw-r--r--   0        0        0    11072 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/deploy/backends/scaleway_api_backend.py
+-rw-r--r--   0        0        0      524 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/deploy/backends/serverless_backend.py
+-rw-r--r--   0        0        0     1700 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/deploy/backends/serverless_framework_backend.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:54:46.776897 scw_serverless-1.0.2/scw_serverless/gateway/__init__.py
+-rw-r--r--   0        0        0     1359 2023-05-04 12:54:46.776897 scw_serverless-1.0.2/scw_serverless/gateway/gateway_api_client.py
+-rw-r--r--   0        0        0     2341 2023-05-04 12:54:46.776897 scw_serverless-1.0.2/scw_serverless/gateway/gateway_manager.py
+-rw-r--r--   0        0        0     2262 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/logger.py
+-rw-r--r--   0        0        0      137 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/triggers/__init__.py
+-rw-r--r--   0        0        0     1405 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/triggers/cron.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:54:46.776897 scw_serverless-1.0.2/scw_serverless/utils/__init__.py
+-rw-r--r--   0        0        0      239 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/utils/commands.py
+-rw-r--r--   0        0        0     1864 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/utils/credentials.py
+-rw-r--r--   0        0        0      590 2023-05-04 12:54:46.776897 scw_serverless-1.0.2/scw_serverless/utils/files.py
+-rw-r--r--   0        0        0     1476 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/utils/loader.py
+-rw-r--r--   0        0        0      761 2023-05-05 15:18:22.602335 scw_serverless-1.0.2/scw_serverless/utils/string.py
+-rw-r--r--   0        0        0     4086 1970-01-01 00:00:00.000000 scw_serverless-1.0.2/setup.py
+-rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 scw_serverless-1.0.2/PKG-INFO
```

### Comparing `scw_serverless-1.0.1/LICENSE` & `scw_serverless-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/README.md` & `scw_serverless-1.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Serverless API Framework
 
 [![PyPI version](https://badge.fury.io/py/scw-serverless.svg)](https://badge.fury.io/py/scw-serverless)
 [![Documentation Status](https://readthedocs.org/projects/serverless-api-project/badge/?version=latest)](https://serverless-api-project.readthedocs.io/en/latest/?badge=latest)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scaleway/serverless-api-project/main.svg)](https://results.pre-commit.ci/latest/github/scaleway/serverless-api-project/main)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scaleway/serverless-api-framework-python/main.svg)](https://results.pre-commit.ci/latest/github/scaleway/serverless-api-framework-python/main)
 
-Serverless API Framework is a tool that lets you write and deploy serverless functions in python.
+Serverless API Framework is a tool that lets you write and deploy serverless functions in Python.
 It bridges your code with the deployment configuration to make it a breeze to work with serverless functions.
 
 Starts by defining a simple Python function:
 
 ```python
 from scw_serverless import Serverless
 
@@ -37,15 +37,15 @@
 
 ```console
 scw-serverless --help
 ```
 
 ### Writing and configuring functions
 
-You can transform your python functions into serverless functions by using decorators:
+You can transform your Python functions into serverless functions by using decorators:
 
 ```python
 import os
 import requests
 from scw_serverless import Serverless
 
 app = Serverless("hello-namespace")
@@ -53,28 +53,30 @@
 
 @app.func(memory_limit=256, env={"API_URL": API_URL})
 def hello_world(event, context):
     return requests.get(API_URL)
 ```
 
 The configuration is done by passing arguments to the decorator.
-To view which arguments are supported, head over to this [documentation](https://serverless-api-project.readthedocs.io/) page.
+To view which arguments are supported, head over to this [documentation](https://serverless-api-framework-python.readthedocs.io/) page.
 
 When you are ready, you can deploy your function with the `scw-serverless` CLI tool:
 
 ```console
 scw-serverless deploy app.py
 ```
 
 The tool will use your Scaleway credentials from your environment and config file.
 
 ## What’s Next?
 
 To learn more about the framework, have a look at the [documentation](https://serverless-api-project.readthedocs.io/).
-If you want to see it in action, we provide some [examples](https://github.com/scaleway/serverless-api-project/tree/main/examples) to get you started.
+If you want to see it in action, we provide some [examples](https://github.com/scaleway/serverless-api-framework-python-python/tree/main/examples) to get you started.
+
+To run your Python functions locally, check out [Scaleway Functions Python](https://github.com/scaleway/serverless-functions-python).
 
 ## Contributing
 
 We welcome all contributions.
 
 This project uses [pre-commit](https://pre-commit.com/) hooks to run code quality checks locally. We recommended installing them before contributing.
```

### Comparing `scw_serverless-1.0.1/pyproject.toml` & `scw_serverless-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "scw-serverless"
-version = "1.0.1"
+version = "1.0.2"
 description = "Framework for writing serverless APIs in Python, using Scaleway functions and containers."
 authors = ["Scaleway Serverless Team <opensource@scaleway.com>"]
 readme = "README.md"
 license = "MIT"
-repository = "https://github.com/scaleway/serverless-api-project"
+repository = "https://github.com/scaleway/serverless-api-framework-python-python"
 documentation = "https://serverless-api-project.readthedocs.io/en/latest/"
 keywords = ["serverless", "scaleway", "functions", "cloud", "faas"]
 
 # Should be one of:
 # "Development Status :: 3 - Alpha"
 # "Development Status :: 4 - Beta"
 # "Development Status :: 5 - Production/Stable"
@@ -35,15 +35,15 @@
 
 [tool.poetry.scripts]
 scw-serverless = "scw_serverless.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
-scaleway = ">=0.7,<0.11"
+scaleway = ">=0.7,<0.12"
 requests = "^2.28.2"
 typing-extensions = { version = "^4.4.0", python = "<3.11" }
 pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=2.21,<4.0"
 pytest = "^7.2.0"
@@ -53,17 +53,17 @@
 responses = ">=0.22,<0.24"
 boto3 = "^1.26.97"
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
-myst_parser = ">=0.18.1,<1.1.0"
-sphinx = "^5.3.0"
-sphinx_rtd_theme = "^1.1.1"
+myst_parser = "^1.0.0"
+sphinx = "^6.1.0"
+sphinx_rtd_theme = "^1.2.0"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore:.*pkg_resources\\.declare_namespace.*:DeprecationWarning",
     "ignore:::pkg_resources",
 ]
```

### Comparing `scw_serverless-1.0.1/scw_serverless/app.py` & `scw_serverless-1.0.2/scw_serverless/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,18 +55,15 @@
             self.functions.append(
                 Function.from_handler(
                     handler,
                     kwargs,
                 )
             )
 
-            def _inner(*args, **kwargs):
-                return handler(*args, **kwargs)
-
-            return _inner
+            return handler
 
         return _decorator
 
     def schedule(
         self,
         schedule: Union[str, CronTrigger],
         inputs: Optional[dict[str, Any]] = None,
@@ -100,58 +97,67 @@
         """Define a routed handler which will respond to GET requests.
 
         :param url: relative url to trigger the function
 
         .. note::
 
             Requires an API gateway
+
+            For more information, please consult the :doc:`gateway` page.
         """
         kwargs |= {"relative_url": url, "http_methods": [HTTPMethod.GET]}
         return self.func(**kwargs)
 
     def post(self, url: str, **kwargs: Unpack[FunctionKwargs]) -> Callable:
         """Define a routed handler which will respond to POST requests.
 
         :param url: relative url to trigger the function
 
         .. note::
-
             Requires an API gateway
+
+            For more information, please consult the :doc:`gateway` page.
         """
         kwargs |= {"relative_url": url, "http_methods": [HTTPMethod.POST]}
         return self.func(**kwargs)
 
     def put(self, url: str, **kwargs: Unpack[FunctionKwargs]) -> Callable:
         """Define a routed handler which will respond to PUT requests.
 
         :param url: relative url to trigger the function
 
         .. note::
 
             Requires an API gateway
+
+            For more information, please consult the :doc:`gateway` page.
         """
         kwargs |= {"relative_url": url, "http_methods": [HTTPMethod.PUT]}
         return self.func(**kwargs)
 
     def delete(self, url: str, **kwargs: Unpack[FunctionKwargs]) -> Callable:
         """Define a routed handler which will respond to DELETE requests.
 
         :param url: relative url to trigger the function
 
         .. note::
 
             Requires an API gateway
+
+            For more information, please consult the :doc:`gateway` page.
         """
         kwargs |= {"relative_url": url, "http_methods": [HTTPMethod.DELETE]}
         return self.func(**kwargs)
 
     def patch(self, url: str, **kwargs: Unpack[FunctionKwargs]) -> Callable:
         """Define a routed handler which will respond to PATCH requests.
 
         :param url: relative url to trigger the function
 
         .. note::
 
             Requires an API gateway
+
+            For more information, please consult the :doc:`gateway` page.
         """
         kwargs |= {"relative_url": url, "http_methods": [HTTPMethod.PATCH]}
         return self.func(**kwargs)
```

### Comparing `scw_serverless-1.0.1/scw_serverless/cli.py` & `scw_serverless-1.0.2/scw_serverless/cli.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/scw_serverless/config/function.py` & `scw_serverless-1.0.2/scw_serverless/config/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     :param description: Description. Defaults to the function docstring if defined.
     :param http_option: Either "enabled" or "redirected".
                         If "redirected" (default), allow http traffic to your function.
                         Blocked otherwise.
 
     .. seealso::
 
-        Scaleway Developers Documentation
-        https://developers.scaleway.com/en/products/functions/api/#create-a-function
+        `Scaleway Developers Documentation
+        <https://developers.scaleway.com/en/products/functions/api/#create-a-function>`_
     """
 
     env: dict[str, str]
     secret: dict[str, str]
     min_scale: int
     max_scale: int
     memory_limit: MemoryLimit
```

### Comparing `scw_serverless-1.0.1/scw_serverless/config/generators/serverless_framework.py` & `scw_serverless-1.0.2/scw_serverless/config/generators/serverless_framework.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/scw_serverless/config/generators/terraform.py` & `scw_serverless-1.0.2/scw_serverless/config/generators/terraform.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/scw_serverless/config/route.py` & `scw_serverless-1.0.2/scw_serverless/config/route.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/scw_serverless/dependencies_manager.py` & `scw_serverless-1.0.2/scw_serverless/dependencies_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     def _check_for_scw_serverless(self):
         """Checks for scw_serverless after vendoring the dependencies."""
         if (
             not self.pkg_path.exists()
             or not self.pkg_path.joinpath(__package__).exists()
         ):
             # Installs the current version with pip
-            self._run_pip_install(f"{__package__}=={version(__package__)}")
+            self._run_pip_install(f"{__package__}~={version(__package__)}")
 
     def _run_pip_install(self, *args: str):
         python_path = sys.executable
         command = [
             python_path,
             "-m",
             "pip",
```

### Comparing `scw_serverless-1.0.1/scw_serverless/deploy/backends/scaleway_api_backend.py` & `scw_serverless-1.0.2/scw_serverless/deploy/backends/scaleway_api_backend.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/scw_serverless/deploy/backends/serverless_backend.py` & `scw_serverless-1.0.2/scw_serverless/deploy/backends/serverless_backend.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/scw_serverless/deploy/backends/serverless_framework_backend.py` & `scw_serverless-1.0.2/scw_serverless/deploy/backends/serverless_framework_backend.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/scw_serverless/gateway/gateway_api_client.py` & `scw_serverless-1.0.2/scw_serverless/gateway/gateway_api_client.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/scw_serverless/gateway/gateway_manager.py` & `scw_serverless-1.0.2/scw_serverless/gateway/gateway_manager.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/scw_serverless/logger.py` & `scw_serverless-1.0.2/scw_serverless/logger.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/scw_serverless/triggers/cron.py` & `scw_serverless-1.0.2/scw_serverless/triggers/cron.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/scw_serverless/utils/credentials.py` & `scw_serverless-1.0.2/scw_serverless/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/scw_serverless/utils/files.py` & `scw_serverless-1.0.2/scw_serverless/utils/files.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/scw_serverless/utils/loader.py` & `scw_serverless-1.0.2/scw_serverless/utils/loader.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/scw_serverless/utils/string.py` & `scw_serverless-1.0.2/scw_serverless/utils/string.py`

 * *Files identical despite different names*

### Comparing `scw_serverless-1.0.1/setup.py` & `scw_serverless-1.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 package_data = \
 {'': ['*'], 'scw_serverless.config': ['templates/*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.2,<3.0.0',
- 'scaleway>=0.7,<0.11']
+ 'scaleway>=0.7,<0.12']
 
 extras_require = \
 {':python_version < "3.11"': ['typing-extensions>=4.4.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['scw-serverless = scw_serverless.cli:main']}
 
 setup_kwargs = {
     'name': 'scw-serverless',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'Framework for writing serverless APIs in Python, using Scaleway functions and containers.',
-    'long_description': '# Serverless API Framework\n\n[![PyPI version](https://badge.fury.io/py/scw-serverless.svg)](https://badge.fury.io/py/scw-serverless)\n[![Documentation Status](https://readthedocs.org/projects/serverless-api-project/badge/?version=latest)](https://serverless-api-project.readthedocs.io/en/latest/?badge=latest)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scaleway/serverless-api-project/main.svg)](https://results.pre-commit.ci/latest/github/scaleway/serverless-api-project/main)\n\nServerless API Framework is a tool that lets you write and deploy serverless functions in python.\nIt bridges your code with the deployment configuration to make it a breeze to work with serverless functions.\n\nStarts by defining a simple Python function:\n\n```python\nfrom scw_serverless import Serverless\n\napp = Serverless("hello-namespace")\n\n@app.func(memory_limit=256)\ndef hello_world(event, context):\n    return "Hello World!"\n```\n\nDeploy it with `scw-serverless`:\n\n```console\nscw-serverless deploy app.py\n```\n\n## Quickstart\n\n### Install\n\n```console\npip install scw-serverless\n```\n\nThis will install the `scw-serverless` CLI:\n\n```console\nscw-serverless --help\n```\n\n### Writing and configuring functions\n\nYou can transform your python functions into serverless functions by using decorators:\n\n```python\nimport os\nimport requests\nfrom scw_serverless import Serverless\n\napp = Serverless("hello-namespace")\nAPI_URL = os.environ["API_URL"]\n\n@app.func(memory_limit=256, env={"API_URL": API_URL})\ndef hello_world(event, context):\n    return requests.get(API_URL)\n```\n\nThe configuration is done by passing arguments to the decorator.\nTo view which arguments are supported, head over to this [documentation](https://serverless-api-project.readthedocs.io/) page.\n\nWhen you are ready, you can deploy your function with the `scw-serverless` CLI tool:\n\n```console\nscw-serverless deploy app.py\n```\n\nThe tool will use your Scaleway credentials from your environment and config file.\n\n## What’s Next?\n\nTo learn more about the framework, have a look at the [documentation](https://serverless-api-project.readthedocs.io/).\nIf you want to see it in action, we provide some [examples](https://github.com/scaleway/serverless-api-project/tree/main/examples) to get you started.\n\n## Contributing\n\nWe welcome all contributions.\n\nThis project uses [pre-commit](https://pre-commit.com/) hooks to run code quality checks locally. We recommended installing them before contributing.\n\n```console\npre-commit install\n```\n',
+    'long_description': '# Serverless API Framework\n\n[![PyPI version](https://badge.fury.io/py/scw-serverless.svg)](https://badge.fury.io/py/scw-serverless)\n[![Documentation Status](https://readthedocs.org/projects/serverless-api-project/badge/?version=latest)](https://serverless-api-project.readthedocs.io/en/latest/?badge=latest)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scaleway/serverless-api-framework-python/main.svg)](https://results.pre-commit.ci/latest/github/scaleway/serverless-api-framework-python/main)\n\nServerless API Framework is a tool that lets you write and deploy serverless functions in Python.\nIt bridges your code with the deployment configuration to make it a breeze to work with serverless functions.\n\nStarts by defining a simple Python function:\n\n```python\nfrom scw_serverless import Serverless\n\napp = Serverless("hello-namespace")\n\n@app.func(memory_limit=256)\ndef hello_world(event, context):\n    return "Hello World!"\n```\n\nDeploy it with `scw-serverless`:\n\n```console\nscw-serverless deploy app.py\n```\n\n## Quickstart\n\n### Install\n\n```console\npip install scw-serverless\n```\n\nThis will install the `scw-serverless` CLI:\n\n```console\nscw-serverless --help\n```\n\n### Writing and configuring functions\n\nYou can transform your Python functions into serverless functions by using decorators:\n\n```python\nimport os\nimport requests\nfrom scw_serverless import Serverless\n\napp = Serverless("hello-namespace")\nAPI_URL = os.environ["API_URL"]\n\n@app.func(memory_limit=256, env={"API_URL": API_URL})\ndef hello_world(event, context):\n    return requests.get(API_URL)\n```\n\nThe configuration is done by passing arguments to the decorator.\nTo view which arguments are supported, head over to this [documentation](https://serverless-api-framework-python.readthedocs.io/) page.\n\nWhen you are ready, you can deploy your function with the `scw-serverless` CLI tool:\n\n```console\nscw-serverless deploy app.py\n```\n\nThe tool will use your Scaleway credentials from your environment and config file.\n\n## What’s Next?\n\nTo learn more about the framework, have a look at the [documentation](https://serverless-api-project.readthedocs.io/).\nIf you want to see it in action, we provide some [examples](https://github.com/scaleway/serverless-api-framework-python-python/tree/main/examples) to get you started.\n\nTo run your Python functions locally, check out [Scaleway Functions Python](https://github.com/scaleway/serverless-functions-python).\n\n## Contributing\n\nWe welcome all contributions.\n\nThis project uses [pre-commit](https://pre-commit.com/) hooks to run code quality checks locally. We recommended installing them before contributing.\n\n```console\npre-commit install\n```\n',
     'author': 'Scaleway Serverless Team',
     'author_email': 'opensource@scaleway.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/scaleway/serverless-api-project',
+    'url': 'https://github.com/scaleway/serverless-api-framework-python-python',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `scw_serverless-1.0.1/PKG-INFO` & `scw_serverless-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: scw-serverless
-Version: 1.0.1
+Version: 1.0.2
 Summary: Framework for writing serverless APIs in Python, using Scaleway functions and containers.
-Home-page: https://github.com/scaleway/serverless-api-project
+Home-page: https://github.com/scaleway/serverless-api-framework-python-python
 License: MIT
 Keywords: serverless,scaleway,functions,cloud,faas
 Author: Scaleway Serverless Team
 Author-email: opensource@scaleway.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -21,27 +21,27 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: scaleway (>=0.7,<0.11)
+Requires-Dist: scaleway (>=0.7,<0.12)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.11"
 Project-URL: Documentation, https://serverless-api-project.readthedocs.io/en/latest/
-Project-URL: Repository, https://github.com/scaleway/serverless-api-project
+Project-URL: Repository, https://github.com/scaleway/serverless-api-framework-python-python
 Description-Content-Type: text/markdown
 
 # Serverless API Framework
 
 [![PyPI version](https://badge.fury.io/py/scw-serverless.svg)](https://badge.fury.io/py/scw-serverless)
 [![Documentation Status](https://readthedocs.org/projects/serverless-api-project/badge/?version=latest)](https://serverless-api-project.readthedocs.io/en/latest/?badge=latest)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scaleway/serverless-api-project/main.svg)](https://results.pre-commit.ci/latest/github/scaleway/serverless-api-project/main)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scaleway/serverless-api-framework-python/main.svg)](https://results.pre-commit.ci/latest/github/scaleway/serverless-api-framework-python/main)
 
-Serverless API Framework is a tool that lets you write and deploy serverless functions in python.
+Serverless API Framework is a tool that lets you write and deploy serverless functions in Python.
 It bridges your code with the deployment configuration to make it a breeze to work with serverless functions.
 
 Starts by defining a simple Python function:
 
 ```python
 from scw_serverless import Serverless
 
@@ -70,15 +70,15 @@
 
 ```console
 scw-serverless --help
 ```
 
 ### Writing and configuring functions
 
-You can transform your python functions into serverless functions by using decorators:
+You can transform your Python functions into serverless functions by using decorators:
 
 ```python
 import os
 import requests
 from scw_serverless import Serverless
 
 app = Serverless("hello-namespace")
@@ -86,28 +86,30 @@
 
 @app.func(memory_limit=256, env={"API_URL": API_URL})
 def hello_world(event, context):
     return requests.get(API_URL)
 ```
 
 The configuration is done by passing arguments to the decorator.
-To view which arguments are supported, head over to this [documentation](https://serverless-api-project.readthedocs.io/) page.
+To view which arguments are supported, head over to this [documentation](https://serverless-api-framework-python.readthedocs.io/) page.
 
 When you are ready, you can deploy your function with the `scw-serverless` CLI tool:
 
 ```console
 scw-serverless deploy app.py
 ```
 
 The tool will use your Scaleway credentials from your environment and config file.
 
 ## What’s Next?
 
 To learn more about the framework, have a look at the [documentation](https://serverless-api-project.readthedocs.io/).
-If you want to see it in action, we provide some [examples](https://github.com/scaleway/serverless-api-project/tree/main/examples) to get you started.
+If you want to see it in action, we provide some [examples](https://github.com/scaleway/serverless-api-framework-python-python/tree/main/examples) to get you started.
+
+To run your Python functions locally, check out [Scaleway Functions Python](https://github.com/scaleway/serverless-functions-python).
 
 ## Contributing
 
 We welcome all contributions.
 
 This project uses [pre-commit](https://pre-commit.com/) hooks to run code quality checks locally. We recommended installing them before contributing.
```

