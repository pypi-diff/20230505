# Comparing `tmp/snk-0.6.2.tar.gz` & `tmp/snk-0.6.3.tar.gz`

## Comparing `snk-0.6.2.tar` & `snk-0.6.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.2/Dockerfile
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 snk-0.6.2/mkdocs.yml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.2/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.2/docs/CNAME
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.2/docs/index.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 snk-0.6.2/docs/reference/cli.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.2/docs/reference/errors.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.2/docs/reference/main.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.2/docs/reference/nest.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.2/snk/__about__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.6.2/snk/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.6.2/snk/errors.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 snk-0.6.2/snk/main.py
--rw-r--r--   0        0        0    15537 2020-02-02 00:00:00.000000 snk-0.6.2/snk/nest.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.6.2/snk/cli/__init__.py
--rw-r--r--   0        0        0    16338 2020-02-02 00:00:00.000000 snk-0.6.2/snk/cli/cli.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 snk-0.6.2/snk/cli/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.2/snk/cli/options.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 snk-0.6.2/snk/cli/pipeline.py
--rw-r--r--   0        0        0     8630 2020-02-02 00:00:00.000000 snk-0.6.2/snk/cli/utils.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.2/tests/.DS_Store
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.2/tests/__init__.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 snk-0.6.2/tests/conftest.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.2/tests/test_nest.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 snk-0.6.2/tests/test_pipline_cli.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 snk-0.6.2/tests/test_snk.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.2/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/cov.fasta
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/bin/snk-basic-pipeline
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/pipeline/.snk
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/pipeline/cli.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/pipeline/config.yaml
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/pipeline/workflow/Snakefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/pipeline/workflow/envs/base.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.2/tests/data/pipeline/workflow/profiles/base/config.yaml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 snk-0.6.2/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.2/LICENSE.txt
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 snk-0.6.2/README.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 snk-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.3/Dockerfile
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 snk-0.6.3/mkdocs.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.3/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.3/docs/CNAME
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.3/docs/index.md
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snk-0.6.3/docs/reference/cli.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.3/docs/reference/errors.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.3/docs/reference/main.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.3/docs/reference/nest.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.3/snk/__about__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.6.3/snk/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.6.3/snk/errors.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 snk-0.6.3/snk/main.py
+-rw-r--r--   0        0        0    15584 2020-02-02 00:00:00.000000 snk-0.6.3/snk/nest.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 snk-0.6.3/snk/pipeline.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.6.3/snk/cli/__init__.py
+-rw-r--r--   0        0        0    16668 2020-02-02 00:00:00.000000 snk-0.6.3/snk/cli/cli.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 snk-0.6.3/snk/cli/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.3/snk/cli/options.py
+-rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 snk-0.6.3/snk/cli/utils.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.3/tests/.DS_Store
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.3/tests/__init__.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 snk-0.6.3/tests/conftest.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.3/tests/test_nest.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 snk-0.6.3/tests/test_pipline_cli.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.6.3/tests/test_snk.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.3/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/cov.fasta
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/bin/snk-basic-pipeline
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/pipeline/.snk
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/pipeline/cli.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/pipeline/config.yaml
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/pipeline/workflow/Snakefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/pipeline/workflow/envs/base.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.3/tests/data/pipeline/workflow/profiles/base/config.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.6.3/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.3/LICENSE.txt
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 snk-0.6.3/README.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 snk-0.6.3/PKG-INFO
```

### Comparing `snk-0.6.2/mkdocs.yml` & `snk-0.6.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/.github/workflows/publish.yml` & `snk-0.6.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/.github/workflows/tests.yml` & `snk-0.6.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/docs/index.md` & `snk-0.6.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/snk/main.py` & `snk-0.6.3/snk/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from types import SimpleNamespace
 import typer
 from pathlib import Path
 import os
 from typing import Optional, List
 from rich.pretty import pprint
 from .nest import Nest
 from .errors import PipelineExistsError, PipelineNotFoundError
@@ -10,14 +11,15 @@
 
 SNK_HOME = None
 SNK_BIN = None
 
 # fmt: off
 @app.callback(context_settings={"help_option_names": ["-h", "--help"]})
 def callback(
+    ctx: typer.Context,
     home: Optional[Path] = typer.Option(
             None, 
             envvar="SNK_HOME", 
             dir_okay=True, 
             file_okay=False, 
             exists=True, 
             help="Overrides default snk location. Pipelines will be installed in $SNK_HOME/pipelines."
@@ -43,22 +45,21 @@
 /_/\__/ / /  / / /    / / // / /  \ \ \     
 \ \/___/ /  / / /    / / // / /    \ \ \    
  \_____\/   \/_/     \/_/ \/_/      \_\_\   
  \b
  \n
  Snakemake pipeline management system
     """
-    global SNK_BIN, SNK_HOME
-    SNK_BIN = bin
-    SNK_HOME = home
+    ctx.obj = SimpleNamespace(snk_home = home, snk_bin = bin)
 # fmt: on
 
 
 @app.command()
 def install(
+    ctx: typer.Context,
     pipeline: str = typer.Argument(
         ..., help="Path, URL or Github name (user/repo) of the pipeline to install."
     ),
     name: Optional[str] = typer.Option(
         None, help="Rename the pipeline (this name will be used to call the CLI.)"
     ),
     tag: Optional[str] = typer.Option(
@@ -80,16 +81,15 @@
     editable: Optional[bool] = typer.Option(
         False, "--editable", "-e", help="Whether to install the pipeline in editable mode."
     ),
 ):
     """
     Install a pipeline.
     """
-    global SNK_BIN, SNK_HOME
-    nest = Nest(snk_home=SNK_HOME, bin_dir=SNK_BIN)
+    nest = Nest(snk_home=ctx.obj.snk_home, bin_dir=ctx.obj.snk_bin)
     if not nest.bin_dir_in_path():
         bin_dir_yellow = typer.style(nest.bin_dir, fg=typer.colors.YELLOW, bold=False)
         typer.echo(f"Please add SNK_BIN to your $PATH: {bin_dir_yellow}")
     if not Path(pipeline).exists() and not pipeline.startswith("http"):
         pipeline = f"https://github.com/{pipeline}.git"
     try:
         installed_pipeline = nest.install(
@@ -110,24 +110,24 @@
     v = installed_pipeline.version
     v = v if v else "latest"
     typer.secho(f"Successfully installed {installed_pipeline.name} ({v})!", fg="green")
 
 
 @app.command()
 def uninstall(
+    ctx: typer.Context,
     name: str = typer.Argument(..., help="Name of the pipeline to uninstall."),
     force: Optional[bool] = typer.Option(
         False, "--force", "-f", help="Force uninstall without asking."
     ),
 ):
     """
     Uninstall a pipeline.
     """
-    global SNK_BIN, SNK_HOME
-    nest = Nest(snk_home=SNK_HOME, bin_dir=SNK_BIN)
+    nest = Nest(snk_home=ctx.obj.snk_home, bin_dir=ctx.obj.snk_bin)
     try:
         uninstalled = nest.uninstall(name, force=force)
     except PipelineNotFoundError as e:
         typer.secho(e, fg="red")
         raise typer.Exit(1)
     if uninstalled:
         typer.secho(f"Successfully uninstalled {name}!", fg="green")
@@ -138,20 +138,21 @@
 #     """
 #     Update a pipeline.
 #     """
 #     raise NotImplementedError
 
 
 @app.command()
-def list():
+def list(
+    ctx: typer.Context,
+):
     """
     List the installed pipelines.
     """
-    global SNK_BIN, SNK_HOME
-    nest = Nest(snk_home=SNK_HOME, bin_dir=SNK_BIN)
+    nest = Nest(snk_home=ctx.obj.snk_home, bin_dir=ctx.obj.snk_bin)
     try:
         pipelines = nest.pipelines
     except FileNotFoundError:
         pipelines = []
     pipeline_dir_yellow = typer.style(
         nest.pipelines_dir, fg=typer.colors.YELLOW, bold=False
     )
```

### Comparing `snk-0.6.2/snk/nest.py` & `snk-0.6.3/snk/nest.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 from git import InvalidGitRepositoryError, Repo, GitCommandError
 import sys
 import stat
 import inspect
 import os
 from typing import List
 import shutil
-import yaml
 
 from .errors import (
     PipelineExistsError,
     PipelineNotFoundError,
     InvalidPipelineRepositoryError,
 )
 from .cli.config import SnkConfig
-from .cli.pipeline import Pipeline
+from .pipeline import Pipeline
 
 
 class Nest:
     """
     Initializes a Nest object.
     Args:
       snk_home (Path, optional): The path to the SNK home directory. Defaults to None.
@@ -113,51 +112,49 @@
         """
         def handle_force_installation(name: str):
             try:
                 self.uninstall(name=name, force=True)
             except PipelineNotFoundError:
                 pass
 
-        if name in [p.name for p in self.pipelines]:
-            raise ValueError("")
+        self._check_pipeline_name_available(name)
         try:
             self._check_repo_url_format(pipeline)
             if not name:
                 name = self._get_name_from_git_url(pipeline)
             if not force:
                 self._check_pipeline_name_available(name)
             else:
                 handle_force_installation(name)
-            path = self.download(pipeline, name, tag_name=tag)
+            pipeline_path = self.download(pipeline, name, tag_name=tag)
         except InvalidPipelineRepositoryError:
-            pipeline = Path(pipeline)
-            if pipeline.suffix == ".snk":
-                pipeline = pipeline.parent
+            pipeline_local_path = Path(pipeline)
+            if pipeline_local_path.name == ".snk":
+                pipeline_local_path = pipeline_local_path.parent
             if not name:
-                name = pipeline.name
+                name = pipeline_local_path.name
             if not force:
                 self._check_pipeline_name_available(name)
             else:
                 handle_force_installation(name)
-            path = self.local(pipeline, name, editable)
+            pipeline_path = self.local(pipeline_local_path, name, editable)
         try:
-            pipeline = Pipeline(path=path)
-            pipeline_executable = self.create_package(pipeline.path)
+            pipeline_executable = self.create_package(pipeline_path)
             self.link_pipeline_executable_to_bin(pipeline_executable)
             if config:
-                self.copy_nonstandard_config(pipeline.path, config)
+                self.copy_nonstandard_config(pipeline_path, config)
             if resources:
-                self.additional_resources(pipeline.path, resources)
+                self.additional_resources(pipeline_path, resources)
             self._confirm_installation(name)
         except Exception as e:
             # remove any half completed steps
             to_remove = self.get_paths_to_delete(name)
             self.delete_paths(to_remove)
             raise e
-        return pipeline
+        return Pipeline(pipeline_path)
 
     def additional_resources(self, pipeline_dir: Path, resources: List[Path]):
         """
         Modify the .snk file so that resources will be copied at runtime.
         Args:
           pipeline_dir (Path): The path to the pipeline directory.
           resources (List[Path]): A list of additional resources to copy.
@@ -261,14 +258,16 @@
             proceed = ans.lower() in ["y", "yes"]
         if not proceed:
             return False
         self.delete_paths(to_remove)
         return True
 
     def _check_pipeline_name_available(self, name: str):
+        if not name:
+            return None
         if name in os.listdir(self.pipelines_dir):
             raise PipelineExistsError(
                 f"Pipeline '{name}' already exists in {self.pipelines_dir}"
             )
         if name in os.listdir(self.bin_dir):
             raise PipelineExistsError(
                 f"Pipeline '{name}' already exists in {self.bin_dir}"
```

### Comparing `snk-0.6.2/snk/cli/cli.py` & `snk-0.6.3/snk/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import inspect
 import sys
 import typer
 from pathlib import Path
 from typing import Optional, List, Callable
-from datetime import datetime
 import subprocess
 import shutil
 import os
 from contextlib import contextmanager
 
 import snakemake
 from rich.console import Console
@@ -17,15 +16,15 @@
 
 from .config import (
     SnkConfig,
     get_config_from_pipeline_dir,
     load_pipeline_snakemake_config,
 )
 from .utils import add_dynamic_options, build_dynamic_cli_options, parse_config_args
-from .pipeline import Pipeline
+from snk.pipeline import Pipeline
 
 
 class CLI:
     """
     Constructor for the CLI class.
     Args:
       pipeline_dir_path (Path): Path to the pipeline directory.
@@ -46,14 +45,19 @@
         self.pipeline = Pipeline(path=pipeline_dir_path)
         self.app = typer.Typer()
         self.snakemake_config = load_pipeline_snakemake_config(pipeline_dir_path)
         self.snk_config: SnkConfig = SnkConfig.from_path(pipeline_dir_path / ".snk")
         self.options = build_dynamic_cli_options(self.snakemake_config, self.snk_config)
         self.snakefile = self._find_snakefile()
         self.conda_prefix_dir = pipeline_dir_path / ".conda"
+        if " " in str(pipeline_dir_path):
+            # cannot have spaces!
+            self.singularity_prefix_dir = None
+        else:
+            self.singularity_prefix_dir = pipeline_dir_path / ".singularity"
         self.name = self.pipeline.name
         self.verbose = False
 
         def _print_pipline_version(ctx: typer.Context, value: bool):
             if value:
                 typer.echo(self.pipeline.version)
                 raise typer.Exit()
@@ -244,14 +248,15 @@
         self,
         ctx: typer.Context,
         target: str = typer.Argument(
             None, help="File to generate. If None will run the pipeline 'all' rule."
         ),
         configfile: Path = typer.Option(
             None,
+            "--config",
             help="Path to snakemake config file. Overrides existing config and defaults.",
             exists=True,
             dir_okay=False,
         ),
         resource: List[Path] = typer.Option(
             [],
             "--resource",
@@ -330,14 +335,16 @@
         args.extend(
             [
                 "--use-conda",
                 f"--conda-prefix={self.conda_prefix_dir}",
                 f"--cores={cores}",
             ]
         )
+        if self.singularity_prefix_dir:
+            args.append(f"--singularity-prefix={self.singularity_prefix_dir}")
         if not self.snakefile.exists():
             raise ValueError("Could not find Snakefile")  # this should occur at install
         else:
             args.append(f"--snakefile={self.snakefile}")
 
         if not configfile:
             configfile = get_config_from_pipeline_dir(self.pipeline.path)
```

### Comparing `snk-0.6.2/snk/cli/config.py` & `snk-0.6.3/snk/cli/config.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/snk/cli/pipeline.py` & `snk-0.6.3/snk/pipeline.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/snk/cli/utils.py` & `snk-0.6.3/snk/cli/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,18 +84,18 @@
                 *args: Variable length argument list.
                 **kwargs: Arbitrary keyword arguments.
             Returns:
                 Callable: A wrapped function with the dynamic options added.
             Notes:
                 This function is used as an inner function in the `add_dynamic_options` decorator.
             """
-            if kwargs["configfile"]:
-                # need to check if kwargs in options have changed
-                # parse the new configfile and update the defautls
-                raise NotImplementedError
+            # if kwargs["configfile"]:
+            #     # need to check if kwargs in options have changed
+            #     # parse the new configfile and update the defautls
+            #     raise NotImplementedError
             for op in options:
                 kwargs["ctx"].args.extend([f"--{op['name']}", kwargs[op["name"]]])
             kwargs = {
                 k: v for k, v in kwargs.items() if k in func_sig.parameters.keys()
             }
             return func(*args, **kwargs)
```

### Comparing `snk-0.6.2/tests/.DS_Store` & `snk-0.6.3/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/tests/conftest.py` & `snk-0.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/tests/test_nest.py` & `snk-0.6.3/tests/test_nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/tests/test_pipline_cli.py` & `snk-0.6.3/tests/test_pipline_cli.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/tests/test_snk.py` & `snk-0.6.3/tests/test_snk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from pathlib import Path
 from typer.testing import CliRunner
 
 from snk.main import app
-from snk.cli.pipeline import Pipeline
+from snk.pipeline import Pipeline
 
 runner = CliRunner()
 
 def test_snk_help():
     result = runner.invoke(app, ["-h"])
     assert result.exit_code == 0
     assert "snk" in result.stdout
```

### Comparing `snk-0.6.2/tests/utils.py` & `snk-0.6.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/tests/data/artic_v4.1.bed` & `snk-0.6.3/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/tests/data/config.yaml` & `snk-0.6.3/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/tests/data/cov.fasta` & `snk-0.6.3/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/LICENSE.txt` & `snk-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/README.md` & `snk-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/pyproject.toml` & `snk-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snk-0.6.2/PKG-INFO` & `snk-0.6.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snk
-Version: 0.6.2
+Version: 0.6.3
 Project-URL: Documentation, https://github.com/wytamma/snk#readme
 Project-URL: Issues, https://github.com/wytamma/snk/issues
 Project-URL: Source, https://github.com/wytamma/snk
 Author-email: Wytamma Wirth <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

