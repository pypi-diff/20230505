# Comparing `tmp/kegstandcli-0.3.4.tar.gz` & `tmp/kegstandcli-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kegstandcli-0.3.4.tar", max compression
+gzip compressed data, was "kegstandcli-0.3.5.tar", max compression
```

## Comparing `kegstandcli-0.3.4.tar` & `kegstandcli-0.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1077 2023-04-23 18:42:25.686572 kegstandcli-0.3.4/LICENSE
--rw-r--r--   0        0        0     6518 2023-04-29 20:52:25.087043 kegstandcli-0.3.4/README.md
--rw-r--r--   0        0        0     1545 2023-04-29 20:54:05.619630 kegstandcli-0.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-03 20:22:59.696056 kegstandcli-0.3.4/src/kegstandcli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 20:23:08.893322 kegstandcli-0.3.4/src/kegstandcli/cli/__init__.py
--rw-r--r--   0        0        0    16328 2023-04-12 22:03:29.066576 kegstandcli-0.3.4/src/kegstandcli/cli/__main__.py
--rw-r--r--   0        0        0     3158 2023-04-12 22:03:29.067785 kegstandcli-0.3.4/src/kegstandcli/cli/build.py
--rw-r--r--   0        0        0     1995 2023-04-23 18:42:31.185993 kegstandcli-0.3.4/src/kegstandcli/cli/config.py
--rw-r--r--   0        0        0      154 2023-04-12 22:03:29.068379 kegstandcli-0.3.4/src/kegstandcli/cli/default_lambda.py.tmpl
--rw-r--r--   0        0        0     1887 2023-04-12 22:03:29.068881 kegstandcli-0.3.4/src/kegstandcli/cli/deploy.py
--rw-r--r--   0        0        0     1179 2023-04-25 19:33:46.541089 kegstandcli-0.3.4/src/kegstandcli/cli/new.py
--rw-r--r--   0        0        0     1230 2023-04-29 20:41:27.128807 kegstandcli-0.3.4/src/kegstandcli/cli/teardown.py
--rw-r--r--   0        0        0        0 2023-04-03 20:23:36.547617 kegstandcli-0.3.4/src/kegstandcli/infra/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-26 17:37:46.125480 kegstandcli-0.3.4/src/kegstandcli/infra/app.py
--rw-r--r--   0        0        0      275 2023-04-27 20:31:57.718526 kegstandcli-0.3.4/src/kegstandcli/infra/cdk.json
--rw-r--r--   0        0        0        0 2023-04-03 20:23:50.899135 kegstandcli-0.3.4/src/kegstandcli/infra/stacks/__init__.py
--rw-r--r--   0        0        0     4193 2023-04-12 22:03:29.071990 kegstandcli-0.3.4/src/kegstandcli/infra/stacks/lambda_rest_api.py
--rw-r--r--   0        0        0      989 2023-04-29 20:18:46.411400 kegstandcli-0.3.4/src/kegstandcli/utils.py
--rw-r--r--   0        0        0     7835 1970-01-01 00:00:00.000000 kegstandcli-0.3.4/setup.py
--rw-r--r--   0        0        0     7896 1970-01-01 00:00:00.000000 kegstandcli-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-23 18:42:25.686572 kegstandcli-0.3.5/LICENSE
+-rw-r--r--   0        0        0     6518 2023-05-04 22:42:37.058514 kegstandcli-0.3.5/README.md
+-rw-r--r--   0        0        0     1545 2023-05-04 22:49:27.977273 kegstandcli-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-03 20:22:59.696056 kegstandcli-0.3.5/src/kegstandcli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:08.893322 kegstandcli-0.3.5/src/kegstandcli/cli/__init__.py
+-rw-r--r--   0        0        0    16270 2023-05-04 22:42:38.140953 kegstandcli-0.3.5/src/kegstandcli/cli/__main__.py
+-rw-r--r--   0        0        0     3048 2023-05-04 22:42:38.142413 kegstandcli-0.3.5/src/kegstandcli/cli/build.py
+-rw-r--r--   0        0        0     2516 2023-05-04 22:19:56.398580 kegstandcli-0.3.5/src/kegstandcli/cli/config.py
+-rw-r--r--   0        0        0      154 2023-04-12 22:03:29.068379 kegstandcli-0.3.5/src/kegstandcli/cli/default_lambda.py.tmpl
+-rw-r--r--   0        0        0     1959 2023-05-04 22:42:38.145141 kegstandcli-0.3.5/src/kegstandcli/cli/deploy.py
+-rw-r--r--   0        0        0     1179 2023-04-25 19:33:46.541089 kegstandcli-0.3.5/src/kegstandcli/cli/new.py
+-rw-r--r--   0        0        0     1302 2023-05-04 22:42:38.147183 kegstandcli-0.3.5/src/kegstandcli/cli/teardown.py
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:36.547617 kegstandcli-0.3.5/src/kegstandcli/infra/__init__.py
+-rw-r--r--   0        0        0     2482 2023-04-26 17:37:46.125480 kegstandcli-0.3.5/src/kegstandcli/infra/app.py
+-rw-r--r--   0        0        0      275 2023-04-27 20:31:57.718526 kegstandcli-0.3.5/src/kegstandcli/infra/cdk.json
+-rw-r--r--   0        0        0        0 2023-04-03 20:23:50.899135 kegstandcli-0.3.5/src/kegstandcli/infra/stacks/__init__.py
+-rw-r--r--   0        0        0     4193 2023-04-12 22:03:29.071990 kegstandcli-0.3.5/src/kegstandcli/infra/stacks/lambda_rest_api.py
+-rw-r--r--   0        0        0     1082 2023-05-04 22:42:37.412595 kegstandcli-0.3.5/src/kegstandcli/utils.py
+-rw-r--r--   0        0        0     7835 1970-01-01 00:00:00.000000 kegstandcli-0.3.5/setup.py
+-rw-r--r--   0        0        0     7896 1970-01-01 00:00:00.000000 kegstandcli-0.3.5/PKG-INFO
```

### Comparing `kegstandcli-0.3.4/LICENSE` & `kegstandcli-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.4/README.md` & `kegstandcli-0.3.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 Here are some notable changes, fixes and features that are planned for development:
 
 ## 0.4.0
 
 - [ ] More content on [kegstand.dev](https://kegstand.dev)
 - [ ] Custom domain names
-- [X] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`
+- [x] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`
 
 ### Pre-1.0.0
 
 - [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.
 - [ ] Pagination helper
 - [ ] [Record a screencast](https://asciinema.org/) for the README
 - [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)
```

#### html2text {}

```diff
@@ -41,15 +41,15 @@
 ``` Finally, to build and deploy the service to AWS: ```shell > poetry run keg
 deploy ``` You should now be able to access the API endpoint at `https:/
 /.execute-api..amazonaws.com/prod/hello`. ## Documentation For further examples
 and more advanced usage, see the [official documentation](https://github.com/
 JensRoland/kegstand/blob/main/docs/index.md). ## Roadmap Here are some notable
 changes, fixes and features that are planned for development: ## 0.4.0 - [ ]
 More content on [kegstand.dev](https://kegstand.dev) - [ ] Custom domain names
-- [X] Maybe simplify the folder structure from `src/api/resources//.py` to
+- [x] Maybe simplify the folder structure from `src/api/resources//.py` to
 `src/api/.py` ### Pre-1.0.0 - [ ] Specify event triggers for Lambda functions:
 S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc. - [ ] Pagination
 helper - [ ] [Record a screencast](https://asciinema.org/) for the README - [ ]
 Autogenerated docs using [MkDocs](https://www.mkdocs.org/) - [ ] GitHub Actions
 workflow for pushing docs to the website ### 1.0.0 - [ ] Intuitive and mostly
 automated API Versioning - [ ] Simple way to define/override core API/Lambda
 properties such as CPU/MEM, Python runtime version, warm pool (!), and
```

### Comparing `kegstandcli-0.3.4/pyproject.toml` & `kegstandcli-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kegstandcli"
-version = "0.3.4"
+version = "0.3.5"
 description = "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/kegstand"
 homepage = "https://kegstand.dev"
 readme = "README.md"
 packages = [
@@ -39,12 +39,12 @@
 python = "^3.9"
 tomlkit = "^0.11.7"
 xxhash = "^3.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 pytest-subprocess = "^1.5.0"
-sentient-switchblade = "^0.2.2"
+sentient-switchblade = "^0.3.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kegstandcli-0.3.4/src/kegstandcli/cli/__main__.py` & `kegstandcli-0.3.5/src/kegstandcli/cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 
 import click
 
 from kegstandcli.cli.build import build
+from kegstandcli.cli.config import find_config_file, get_kegstand_config
 from kegstandcli.cli.deploy import deploy
 from kegstandcli.cli.new import new
 from kegstandcli.cli.teardown import teardown
 
 ALIASES = {"init": new, "up": deploy, "party": deploy, "down": teardown}
 
 CONFIG_FILE_NAMES = ["kegstand.toml", ".kegstand", "pyproject.toml"]
@@ -21,19 +22,19 @@
         return super().get_command(ctx, cmd_name)
 
 
 # pylint: disable=line-too-long
 # We pass the project directory to all subcommands via the context
 # so they can use it to find the kegstand.toml file
 @click.group(cls=AliasedGroup)
-@click.option("--config", help="Path to Kegstand configuration file.")
+@click.option("--config", "config_file", help="Path to Kegstand configuration file.")
 @click.option("--verbose", is_flag=True, default=False, help="Show verbose output")
 @click.pass_context
 def kegstandcli(
-    ctx, config, verbose
+    ctx, config_file, verbose
 ):  # ANSI art generated with https://dom111.github.io/image-to-ansi/
     """\b
     \033[49m                        \033[38;5;232;48;5;52m▄\033[38;5;234;48;5;52m▄\033[38;5;232;49m▄▄▄\033[38;5;236;48;5;52m▄\033[38;5;245;48;5;233m▄\033[38;5;252;48;5;232m▄\033[38;5;230;48;5;233m▄\033[38;5;230;48;5;234m▄\033[38;5;230;48;5;233m▄\033[38;5;253;48;5;232m▄\033[38;5;248;48;5;232m▄\033[38;5;59;48;5;52m▄\033[38;5;233;49m▄\033[38;5;232;49m▄\033[49m     \033[38;5;52;49m▄\033[49m       \033[m
     \033[49m                        \033[49;38;5;52m▀\033[38;5;52;48;5;236m▄\033[38;5;237;48;5;188m▄\033[38;5;254;48;5;252m▄\033[38;5;230;48;5;253m▄\033[38;5;230;48;5;230m▄\033[38;5;222;48;5;223m▄\033[38;5;222;48;5;222m▄▄▄▄▄▄\033[38;5;222;48;5;229m▄\033[38;5;222;48;5;253m▄\033[38;5;229;48;5;242m▄\033[38;5;249;48;5;232m▄\033[38;5;234;48;5;52m▄\033[38;5;52;49m▄\033[49m  \033[38;5;52;48;5;233m▄\033[38;5;239;48;5;232m▄\033[38;5;234;48;5;52m▄\033[38;5;52;49m▄\033[49m    \033[m
     \033[49m                        \033[38;5;52;49m▄\033[38;5;232;49m▄\033[38;5;240;48;5;52m▄\033[38;5;144;48;5;236m▄\033[38;5;101;48;5;186m▄\033[38;5;180;48;5;222m▄\033[38;5;222;48;5;222m▄▄▄▄▄▄\033[48;5;222m \033[38;5;222;48;5;222m▄▄▄▄\033[38;5;222;48;5;252m▄\033[38;5;187;48;5;235m▄\033[38;5;235;48;5;52m▄\033[38;5;52;49m▄\033[38;5;236;48;5;233m▄\033[38;5;254;48;5;102m▄\033[38;5;221;48;5;143m▄\033[38;5;237;48;5;232m▄\033[38;5;52;49m▄\033[49m   \033[m
     \033[49m                       \033[38;5;233;48;5;52m▄\033[38;5;250;48;5;234m▄\033[38;5;222;48;5;249m▄\033[38;5;185;48;5;229m▄\033[38;5;221;48;5;221m▄\033[38;5;179;48;5;221m▄\033[38;5;179;48;5;137m▄\033[38;5;137;48;5;180m▄\033[38;5;143;48;5;222m▄\033[38;5;222;48;5;222m▄▄▄\033[48;5;222m \033[38;5;222;48;5;222m▄▄▄▄▄▄▄\033[38;5;249;48;5;144m▄\033[38;5;230;48;5;238m▄\033[38;5;222;48;5;253m▄\033[38;5;222;48;5;222m▄\033[38;5;179;48;5;221m▄\033[38;5;137;48;5;95m▄\033[38;5;232;48;5;233m▄\033[49m   \033[m
     \033[49m                      \033[38;5;234;48;5;233m▄\033[38;5;187;48;5;243m▄\033[38;5;221;48;5;222m▄\033[38;5;221;48;5;215m▄\033[38;5;221;48;5;179m▄\033[38;5;222;48;5;179m▄▄\033[38;5;179;48;5;137m▄\033[38;5;101;48;5;143m▄\033[38;5;143;48;5;101m▄\033[38;5;180;48;5;101m▄\033[38;5;101;48;5;222m▄\033[38;5;222;48;5;222m▄▄▄\033[38;5;179;48;5;186m▄\033[38;5;186;48;5;222m▄\033[38;5;222;48;5;222m▄▄▄▄▄▄▄\033[38;5;221;48;5;222m▄\033[38;5;143;48;5;179m▄\033[38;5;101;48;5;137m▄\033[38;5;232;48;5;232m▄\033[49m   \033[m
@@ -59,27 +60,24 @@
     \033[38;5;167m██   ██ ███████  ██████  ███████ ████████  █████  ███    ██ ██████
     ██  ██  ██      ██       ██         ██    ██   ██ ████   ██ ██   ██
     █████   █████   ██   ███ ███████    ██    ███████ ██ ██  ██ ██   ██
     ██  ██  ██      ██    ██      ██    ██    ██   ██ ██  ██ ██ ██   ██
     ██   ██ ███████  ██████  ███████    ██    ██   ██ ██   ████ ██████
     ===================================================================
     The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS\033[m"""  # noqa: E501
-    # Locate the correct Kegstand configuration file
-    if config is None:
-        for name in CONFIG_FILE_NAMES:
-            if os.path.exists(name):
-                config = name
-                break
 
-    if not os.path.exists(config):
-        raise click.ClickException(f"Configuration file not found: {config}")
+    config_file = find_config_file(verbose, config_file)
+
+    project_dir = os.path.abspath(os.path.dirname(config_file))
+
+    config = get_kegstand_config(verbose, project_dir, config_file)
 
-    project_dir = os.path.abspath(os.path.dirname(config))
     ctx.obj = {
-        "config": os.path.abspath(config),
+        "config": config,
+        "config_file": os.path.abspath(config_file),
         "project_dir": project_dir,
         "verbose": verbose,
     }
 
 
 for command in [new, build, deploy, teardown]:
     kegstandcli.add_command(command)
```

### Comparing `kegstandcli-0.3.4/src/kegstandcli/cli/build.py` & `kegstandcli-0.3.5/src/kegstandcli/cli/build.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import os
 import shutil
 import subprocess  # nosec
+from operator import itemgetter
 
 import click
 
-from kegstandcli.cli.config import get_kegstand_config
-
 
 @click.command()
 @click.pass_context
 def build(ctx):
-    project_dir = ctx.obj["project_dir"]
-    config_file = ctx.obj["config"]
-    verbose = ctx.obj["verbose"]
-    build_command(verbose, project_dir, config_file)
-
+    project_dir, config, verbose = itemgetter("project_dir", "config", "verbose")(
+        ctx.obj
+    )
+    build_command(verbose, project_dir, config)
 
-def build_command(verbose: bool, project_dir: str, config_file: str):
-    config = get_kegstand_config(verbose, project_dir, config_file)
 
+def build_command(verbose: bool, project_dir: str, config: dict):
     # Create a directory to hold the build artifacts, and make sure it is empty
     build_dir = create_empty_folder(project_dir, "dist")
 
     # Handle the different types ('modules') of build
     if "api" in config:
         build_api(
             config, verbose, project_dir, create_empty_folder(build_dir, "api_src")
```

### Comparing `kegstandcli-0.3.4/src/kegstandcli/cli/config.py` & `kegstandcli-0.3.5/src/kegstandcli/cli/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 import os
 import re
 from pathlib import Path
 
 import click
 from tomlkit import loads
 
+CONFIG_FILE_NAMES = ["kegstand.toml", ".kegstand", "pyproject.toml"]
+
+
+def find_config_file(verbose: bool, config_file: str) -> str:
+    # If no config file is specified, locate it automatically
+    if config_file is None:
+        for name in CONFIG_FILE_NAMES:
+            if os.path.exists(name):
+                config_file = name
+                break
+
+    if not os.path.exists(config_file):
+        raise click.ClickException(f"Configuration file not found: {config_file}")
+
+    return config_file
+
 
 def get_kegstand_config(verbose, project_dir: str, config_file: str):
     config_file = os.path.join(project_dir, config_file)
     if verbose:
         click.echo(f"Loading configuration from {config_file}")
 
     parsed_toml_config = loads(Path(config_file).read_text(encoding="utf-8"))
```

### Comparing `kegstandcli-0.3.4/src/kegstandcli/cli/deploy.py` & `kegstandcli-0.3.5/src/kegstandcli/cli/deploy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import subprocess  # nosec
+from operator import itemgetter
 
 import click
 
 from kegstandcli.cli.build import build_command
 
 
 @click.command()
@@ -18,29 +19,29 @@
 @click.option(
     "--skip-build",
     is_flag=True,
     default=False,
     help="Skip building the project before deploying",
 )
 def deploy(ctx, region, hotswap, skip_build):
-    project_dir = ctx.obj["project_dir"]
-    config_file = ctx.obj["config"]
-    verbose = ctx.obj["verbose"]
+    project_dir, config_file, verbose = itemgetter(
+        "project_dir", "config_file", "verbose"
+    )(ctx.obj)
     if not skip_build:
         build_command(verbose, project_dir, config_file)
 
     deploy_command(verbose, project_dir, config_file, region, hotswap)
 
 
 def deploy_command(verbose, project_dir, config_file, region, hotswap):
     # Get the dir of the kegstandcli package (one level up from here)
     kegstandcli_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
     click.echo("Deploying...")
-    command = [
+    command = [  # pylint: disable=duplicate-code
         "cdk",
         "deploy",
         "--app",
         "python infra/app.py",
         "--output",
         f"{project_dir}/cdk.out",
         "--all",
```

### Comparing `kegstandcli-0.3.4/src/kegstandcli/cli/new.py` & `kegstandcli-0.3.5/src/kegstandcli/cli/new.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.4/src/kegstandcli/cli/teardown.py` & `kegstandcli-0.3.5/src/kegstandcli/cli/teardown.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import os
 import subprocess  # nosec
+from operator import itemgetter
 
 import click
 
 
 @click.command()
 @click.pass_context
 @click.option(
     "--region", default="eu-west-1", help="AWS region the stack is deployed to"
 )
 def teardown(ctx, region):
-    project_dir = ctx.obj["project_dir"]
-    config_file = ctx.obj["config"]
-    verbose = ctx.obj["verbose"]
+    project_dir, config_file, verbose = itemgetter(
+        "project_dir", "config_file", "verbose"
+    )(ctx.obj)
     teardown_command(verbose, project_dir, config_file, region)
 
 
 def teardown_command(verbose, project_dir, config_file, region):
     # Get the dir of the Kegstand CLI package itself (one level up from here)
     kegstandcli_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
     subprocess.run(
-        [
+        [  # pylint: disable=duplicate-code
             "cdk",
             "destroy",
             "--app",
             "python infra/app.py",
             "--output",
             f"{project_dir}/cdk.out",
             "--all",
```

### Comparing `kegstandcli-0.3.4/src/kegstandcli/infra/app.py` & `kegstandcli-0.3.5/src/kegstandcli/infra/app.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.4/src/kegstandcli/infra/stacks/lambda_rest_api.py` & `kegstandcli-0.3.5/src/kegstandcli/infra/stacks/lambda_rest_api.py`

 * *Files identical despite different names*

### Comparing `kegstandcli-0.3.4/src/kegstandcli/utils.py` & `kegstandcli-0.3.5/src/kegstandcli/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,16 +10,22 @@
 
     # Loop over folders in api_dir and import the resource modules
     for file_descriptor in os.listdir(api_dir):
         # Ignore folders, only look at files
         if os.path.isdir(os.path.join(api_dir, file_descriptor)):
             continue
         # Skip dotfiles and special files
-        if file_descriptor.startswith('.') or file_descriptor.startswith('__') or file_descriptor == 'lambda.py':
+        if (
+            file_descriptor.startswith(".")
+            or file_descriptor.startswith("__")
+            or file_descriptor == "lambda.py"
+        ):
             continue
         resource_name = os.path.splitext(file_descriptor)[0]
-        resources.append({
-            'name': resource_name,
-            'module_path': f'api.{resource_name}',
-            'fromlist': [resource_name]
-        })
+        resources.append(
+            {
+                "name": resource_name,
+                "module_path": f"api.{resource_name}",
+                "fromlist": [resource_name],
+            }
+        )
     return resources
```

### Comparing `kegstandcli-0.3.4/setup.py` & `kegstandcli-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,17 @@
  'xxhash>=3.2.0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['keg = kegstandcli.cli.__main__:kegstandcli']}
 
 setup_kwargs = {
     'name': 'kegstandcli',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
-    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://kegstand.dev/">\n    <img src="https://kegstand.dev/assets/kegstand-logotype.png" width="540px" alt="Kegstand logo" />\n  </a>\n</p>\n\n<h3 align="center">The Developer\'s Toolbelt For Accelerating <em>Mean Time To Party</em> on AWS</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a> and fueled by a non-zero amount of alcohol</p>\n<p align="center"><a href="https://kegstand.dev/demo">Watch a 3-minute demo</a></p><!-- markdown-link-check-disable-line -->\n\n<br />\n\n## 🥂💃🕺 Welcome to the Party! 🥂💃🕺\n\nKegstand is a free and open-source framework for creating Python APIs and services. It allows you to rapidly build and deploy services on AWS. We all have better things to do than `print(json.dumps(event))` all day long, and Kegstand is here to help you get to the party &mdash; _and into Prod_ &mdash; a lot faster.\n\n**It provides:**\n\n- A CLI tool for creating and deploying your services.\n- A decorator based API abstracting away the boilerplate of Lambda, API Gateway, Cognito, and more.\n- The full power of CDK to define and deploy arbitrary AWS resources with your services.\n\n> _"Experience a streamlined cloud development process, enhanced productivity, and hit that "party" button sooner with Kegstand!"_ > **&mdash; GPT-4, official spokesbot for the Kegstand team**\n\nLearn more on the [Kegstand website](https://kegstand.dev/).\n\n## Prerequisites\n\n- [Python 3.8+](https://www.python.org/downloads/)\n- [Poetry](https://python-poetry.org/docs/#installation) (recommended)\n- An [AWS account](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)\n- The [CDK CLI configured on the local machine and initialized on the AWS account](https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html)\n- The AWS CLI [configured with credentials](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)\n- [Copier](https://copier.readthedocs.io/en/stable/#installation) project scaffolding tool (recommended)\n- [npx](https://docs.npmjs.com/cli/v9/commands/npx) for installing CLI tools (recommended)\n- A well-poured [Belgian style brown ale](https://www.grimbergen.com/)\n\n## Quick start\n\nTo create a service with Kegstand, you\'ll need a Python project with a few dependencies and a folder structure following the Kegstand convention.\n\nYou can create this in a few seconds, either with the Kegstand CLI or using [Copier](https://copier.readthedocs.io/en/stable/#installation).\n\n```shell\n# Using the Kegstand CLI\n> pipx install kegstandcli\n> keg new my-service\n\n# Using Copier\n> copier gh:JensRoland/kegstand-project-template my-service\n```\n\nEither method will create a new project folder called `my-service` containing:\n\n```shell\nmy-service\n├── .gitignore                        # Standard .gitignore file\n├── pyproject.toml                    # Project configuration\n└── src\n    └── api\n        └── hello.py                  # Logic for /hello/\n```\n\nKegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a single, empty `__init__.py` gatecrasher, but we can safely ignore that one.\n\nTo install the dependencies for the new project:\n\n```shell\n> cd my-service\n> poetry install\n```\n\nFinally, to build and deploy the service to AWS:\n\n```shell\n> poetry run keg deploy\n```\n\nYou should now be able to access the API endpoint at `https://<api-id>.execute-api.<region>.amazonaws.com/prod/hello`.\n\n## Documentation\n\nFor further examples and more advanced usage, see the [official documentation](https://github.com/JensRoland/kegstand/blob/main/docs/index.md).\n\n## Roadmap\n\nHere are some notable changes, fixes and features that are planned for development:\n\n## 0.4.0\n\n- [ ] More content on [kegstand.dev](https://kegstand.dev)\n- [ ] Custom domain names\n- [X] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`\n\n### Pre-1.0.0\n\n- [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.\n- [ ] Pagination helper\n- [ ] [Record a screencast](https://asciinema.org/) for the README\n- [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)\n- [ ] GitHub Actions workflow for pushing docs to the website\n\n### 1.0.0\n\n- [ ] Intuitive and mostly automated API Versioning\n- [ ] Simple way to define/override core API/Lambda properties such as CPU/MEM, Python runtime version, warm pool (!), and concurrency\n- [ ] Deploy Lambda-only microservices with no API Gateway\n\n### Future\n\n- [ ] Configurable log level\n- [ ] Add AWS tags in the Kegstand config and they will be applied to the generated resources\n- [ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html)\n- [ ] Add support for APIs using [FastAPI](https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Improved output from deploy command; friendly post-deploy instructions for testing your API\n- [ ] Version bumper with [bump2version](https://pypi.org/project/bump2version/)\n- [ ] Include more goodies from [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) - tracing, metrics, etc.\n- [ ] Add support for APIs using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Unit testing helpers (wrap moto and make it all a little more DRY and intuitive)\n- [ ] Secure endpoints which require re-authentication (and/or MFA) so a refreshed token isn’t enough (to, say, delete your account or change your credit card info)\n- [ ] Live Lambda development a la SST\n- [ ] Build and deploy gRPC endpoints (or similar alternative)\n- [ ] Build and deploy GraphQL endpoints\n- [ ] Build and deploy stream processors?\n- [ ] Option to teardown before deploying: `keg deploy --force-redeploy`\n- [ ] Use env vars to populate values in kegstand.toml\n- [ ] Merge Kegstand and Beth into one tool\n- [ ] CDK Pipelines\n- [ ] Support HTTP method-specific files (e.g. `get.py`, `post.py`, etc.)\n- [ ] Upgrade Copier once the [template-deleting bugfix](https://github.com/copier-org/copier/pull/1037) is released\n',
+    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://kegstand.dev/">\n    <img src="https://kegstand.dev/assets/kegstand-logotype.png" width="540px" alt="Kegstand logo" />\n  </a>\n</p>\n\n<h3 align="center">The Developer\'s Toolbelt For Accelerating <em>Mean Time To Party</em> on AWS</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a> and fueled by a non-zero amount of alcohol</p>\n<p align="center"><a href="https://kegstand.dev/demo">Watch a 3-minute demo</a></p><!-- markdown-link-check-disable-line -->\n\n<br />\n\n## 🥂💃🕺 Welcome to the Party! 🥂💃🕺\n\nKegstand is a free and open-source framework for creating Python APIs and services. It allows you to rapidly build and deploy services on AWS. We all have better things to do than `print(json.dumps(event))` all day long, and Kegstand is here to help you get to the party &mdash; _and into Prod_ &mdash; a lot faster.\n\n**It provides:**\n\n- A CLI tool for creating and deploying your services.\n- A decorator based API abstracting away the boilerplate of Lambda, API Gateway, Cognito, and more.\n- The full power of CDK to define and deploy arbitrary AWS resources with your services.\n\n> _"Experience a streamlined cloud development process, enhanced productivity, and hit that "party" button sooner with Kegstand!"_ > **&mdash; GPT-4, official spokesbot for the Kegstand team**\n\nLearn more on the [Kegstand website](https://kegstand.dev/).\n\n## Prerequisites\n\n- [Python 3.8+](https://www.python.org/downloads/)\n- [Poetry](https://python-poetry.org/docs/#installation) (recommended)\n- An [AWS account](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)\n- The [CDK CLI configured on the local machine and initialized on the AWS account](https://docs.aws.amazon.com/cdk/latest/guide/getting_started.html)\n- The AWS CLI [configured with credentials](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)\n- [Copier](https://copier.readthedocs.io/en/stable/#installation) project scaffolding tool (recommended)\n- [npx](https://docs.npmjs.com/cli/v9/commands/npx) for installing CLI tools (recommended)\n- A well-poured [Belgian style brown ale](https://www.grimbergen.com/)\n\n## Quick start\n\nTo create a service with Kegstand, you\'ll need a Python project with a few dependencies and a folder structure following the Kegstand convention.\n\nYou can create this in a few seconds, either with the Kegstand CLI or using [Copier](https://copier.readthedocs.io/en/stable/#installation).\n\n```shell\n# Using the Kegstand CLI\n> pipx install kegstandcli\n> keg new my-service\n\n# Using Copier\n> copier gh:JensRoland/kegstand-project-template my-service\n```\n\nEither method will create a new project folder called `my-service` containing:\n\n```shell\nmy-service\n├── .gitignore                        # Standard .gitignore file\n├── pyproject.toml                    # Project configuration\n└── src\n    └── api\n        └── hello.py                  # Logic for /hello/\n```\n\nKegstand projects are minimal by design, so a fresh project folder contains just those 3 files. Well, apart from a single, empty `__init__.py` gatecrasher, but we can safely ignore that one.\n\nTo install the dependencies for the new project:\n\n```shell\n> cd my-service\n> poetry install\n```\n\nFinally, to build and deploy the service to AWS:\n\n```shell\n> poetry run keg deploy\n```\n\nYou should now be able to access the API endpoint at `https://<api-id>.execute-api.<region>.amazonaws.com/prod/hello`.\n\n## Documentation\n\nFor further examples and more advanced usage, see the [official documentation](https://github.com/JensRoland/kegstand/blob/main/docs/index.md).\n\n## Roadmap\n\nHere are some notable changes, fixes and features that are planned for development:\n\n## 0.4.0\n\n- [ ] More content on [kegstand.dev](https://kegstand.dev)\n- [ ] Custom domain names\n- [x] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`\n\n### Pre-1.0.0\n\n- [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.\n- [ ] Pagination helper\n- [ ] [Record a screencast](https://asciinema.org/) for the README\n- [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)\n- [ ] GitHub Actions workflow for pushing docs to the website\n\n### 1.0.0\n\n- [ ] Intuitive and mostly automated API Versioning\n- [ ] Simple way to define/override core API/Lambda properties such as CPU/MEM, Python runtime version, warm pool (!), and concurrency\n- [ ] Deploy Lambda-only microservices with no API Gateway\n\n### Future\n\n- [ ] Configurable log level\n- [ ] Add AWS tags in the Kegstand config and they will be applied to the generated resources\n- [ ] Easily add [AWS Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html)\n- [ ] Add support for APIs using [FastAPI](https://fastapi.tiangolo.com/) with [Mangum](https://mangum.io/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Improved output from deploy command; friendly post-deploy instructions for testing your API\n- [ ] Version bumper with [bump2version](https://pypi.org/project/bump2version/)\n- [ ] Include more goodies from [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) - tracing, metrics, etc.\n- [ ] Add support for APIs using pure [Lambda Powertools](https://awslabs.github.io/aws-lambda-powertools-python/2.11.0/) instead of the default Kegstand API framework, and just provide deployment helpers for the API Gateway and Lambda\n- [ ] Unit testing helpers (wrap moto and make it all a little more DRY and intuitive)\n- [ ] Secure endpoints which require re-authentication (and/or MFA) so a refreshed token isn’t enough (to, say, delete your account or change your credit card info)\n- [ ] Live Lambda development a la SST\n- [ ] Build and deploy gRPC endpoints (or similar alternative)\n- [ ] Build and deploy GraphQL endpoints\n- [ ] Build and deploy stream processors?\n- [ ] Option to teardown before deploying: `keg deploy --force-redeploy`\n- [ ] Use env vars to populate values in kegstand.toml\n- [ ] Merge Kegstand and Beth into one tool\n- [ ] CDK Pipelines\n- [ ] Support HTTP method-specific files (e.g. `get.py`, `post.py`, etc.)\n- [ ] Upgrade Copier once the [template-deleting bugfix](https://github.com/copier-org/copier/pull/1037) is released\n',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kegstand.dev',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 'src'} packages = \ ['kegstandcli', 'kegstandcli.cli', 'kegstandcli.infra',
 'kegstandcli.infra.stacks'] package_data = \ {'': ['*']} install_requires = \
 ['aws-cdk-lib>=2.67.0,<3.0.0', 'aws-solutions-constructs-aws-apigateway-
 lambda>=2.36.0,<3.0.0', 'boto3>=1.17.113,<2.0.0', 'click>=8.0.3,<9.0.0',
 'constructs>=10.0.0,<11.0.0', 'copier>=6.2.0,<7.0.0', 'pyjwt>=2.1.0,<3.0.0',
 'tomlkit>=0.11.7,<0.12.0', 'xxhash>=3.2.0,<4.0.0'] entry_points = \
 {'console_scripts': ['keg = kegstandcli.cli.__main__:kegstandcli']}
-setup_kwargs = { 'name': 'kegstandcli', 'version': '0.3.4', 'description': "The
+setup_kwargs = { 'name': 'kegstandcli', 'version': '0.3.5', 'description': "The
 Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
 'long_description': '\n
                            \n \n_[Kegstand_logo]\n\n
 \n\n
 **** The Developer\'s Toolbelt For Accelerating Mean Time To Party on AWS ****
 \n
        Created by Jens_Roland and fueled by a non-zero amount of alcohol
@@ -56,15 +56,15 @@
 service\n> poetry install\n```\n\nFinally, to build and deploy the service to
 AWS:\n\n```shell\n> poetry run keg deploy\n```\n\nYou should now be able to
 access the API endpoint at `https://.execute-api..amazonaws.com/prod/
 hello`.\n\n## Documentation\n\nFor further examples and more advanced usage,
 see the [official documentation](https://github.com/JensRoland/kegstand/blob/
 main/docs/index.md).\n\n## Roadmap\n\nHere are some notable changes, fixes and
 features that are planned for development:\n\n## 0.4.0\n\n- [ ] More content on
-[kegstand.dev](https://kegstand.dev)\n- [ ] Custom domain names\n- [X] Maybe
+[kegstand.dev](https://kegstand.dev)\n- [ ] Custom domain names\n- [x] Maybe
 simplify the folder structure from `src/api/resources//.py` to `src/
 api/.py`\n\n### Pre-1.0.0\n\n- [ ] Specify event triggers for Lambda functions:
 S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.\n- [ ]
 Pagination helper\n- [ ] [Record a screencast](https://asciinema.org/) for the
 README\n- [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)\n- [ ]
 GitHub Actions workflow for pushing docs to the website\n\n### 1.0.0\n\n- [ ]
 Intuitive and mostly automated API Versioning\n- [ ] Simple way to define/
```

### Comparing `kegstandcli-0.3.4/PKG-INFO` & `kegstandcli-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kegstandcli
-Version: 0.3.4
+Version: 0.3.5
 Summary: The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS
 Home-page: https://kegstand.dev
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -120,15 +120,15 @@
 
 Here are some notable changes, fixes and features that are planned for development:
 
 ## 0.4.0
 
 - [ ] More content on [kegstand.dev](https://kegstand.dev)
 - [ ] Custom domain names
-- [X] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`
+- [x] Maybe simplify the folder structure from `src/api/resources/<resource-name>/<method>.py` to `src/api/<resource-name>.py`
 
 ### Pre-1.0.0
 
 - [ ] Specify event triggers for Lambda functions: S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc.
 - [ ] Pagination helper
 - [ ] [Record a screencast](https://asciinema.org/) for the README
 - [ ] Autogenerated docs using [MkDocs](https://www.mkdocs.org/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kegstandcli Version: 0.3.4 Summary: The Developer's
+Metadata-Version: 2.1 Name: kegstandcli Version: 0.3.5 Summary: The Developer's
 Toolbelt For Accelerating Mean-Time-To-Party on AWS Home-page: https://
 kegstand.dev License: MIT Author: JensRoland Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -60,15 +60,15 @@
 ``` Finally, to build and deploy the service to AWS: ```shell > poetry run keg
 deploy ``` You should now be able to access the API endpoint at `https:/
 /.execute-api..amazonaws.com/prod/hello`. ## Documentation For further examples
 and more advanced usage, see the [official documentation](https://github.com/
 JensRoland/kegstand/blob/main/docs/index.md). ## Roadmap Here are some notable
 changes, fixes and features that are planned for development: ## 0.4.0 - [ ]
 More content on [kegstand.dev](https://kegstand.dev) - [ ] Custom domain names
-- [X] Maybe simplify the folder structure from `src/api/resources//.py` to
+- [x] Maybe simplify the folder structure from `src/api/resources//.py` to
 `src/api/.py` ### Pre-1.0.0 - [ ] Specify event triggers for Lambda functions:
 S3, SNS, SQS, DynamoDB, Cloudwatch CRON scheduled events, etc. - [ ] Pagination
 helper - [ ] [Record a screencast](https://asciinema.org/) for the README - [ ]
 Autogenerated docs using [MkDocs](https://www.mkdocs.org/) - [ ] GitHub Actions
 workflow for pushing docs to the website ### 1.0.0 - [ ] Intuitive and mostly
 automated API Versioning - [ ] Simple way to define/override core API/Lambda
 properties such as CPU/MEM, Python runtime version, warm pool (!), and
```

