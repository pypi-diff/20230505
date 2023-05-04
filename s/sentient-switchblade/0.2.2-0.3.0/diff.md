# Comparing `tmp/sentient_switchblade-0.2.2.tar.gz` & `tmp/sentient_switchblade-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentient_switchblade-0.2.2.tar", max compression
+gzip compressed data, was "sentient_switchblade-0.3.0.tar", max compression
```

## Comparing `sentient_switchblade-0.2.2.tar` & `sentient_switchblade-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1077 2023-04-25 19:36:38.976660 sentient_switchblade-0.2.2/LICENSE
--rw-r--r--   0        0        0     8176 2023-04-28 18:20:25.734064 sentient_switchblade-0.2.2/README.md
--rw-r--r--   0        0        0     1405 2023-04-29 18:34:38.341962 sentient_switchblade-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 19:36:27.260808 sentient_switchblade-0.2.2/src/switchbladecli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 19:35:52.447291 sentient_switchblade-0.2.2/src/switchbladecli/cli/__init__.py
--rw-r--r--   0        0        0     1656 2023-04-28 12:34:10.275655 sentient_switchblade-0.2.2/src/switchbladecli/cli/__main__.py
--rw-r--r--   0        0        0    11308 2023-04-28 19:56:54.609233 sentient_switchblade-0.2.2/src/switchbladecli/cli/bundle_cache.py
--rw-r--r--   0        0        0      472 2023-04-25 19:36:06.675755 sentient_switchblade-0.2.2/src/switchbladecli/cli/config.py
--rw-r--r--   0        0        0     1087 2023-04-28 18:13:37.061787 sentient_switchblade-0.2.2/src/switchbladecli/cli/lint.py
--rw-r--r--   0        0        0     1089 2023-04-28 12:31:21.153690 sentient_switchblade-0.2.2/src/switchbladecli/cli/test.py
--rw-r--r--   0        0        0      634 2023-04-25 19:36:17.409663 sentient_switchblade-0.2.2/src/switchbladecli/cli/update.py
--rw-r--r--   0        0        0        0 2023-04-26 17:36:55.033765 sentient_switchblade-0.2.2/src/switchbladecli/modes/__init__.py
--rw-r--r--   0        0        0    11146 2023-04-29 18:33:51.414203 sentient_switchblade-0.2.2/src/switchbladecli/modes/python_poetry.py
--rw-r--r--   0        0        0      837 2023-04-25 19:36:32.128019 sentient_switchblade-0.2.2/src/switchbladecli/utils.py
--rw-r--r--   0        0        0     9368 1970-01-01 00:00:00.000000 sentient_switchblade-0.2.2/setup.py
--rw-r--r--   0        0        0     9583 1970-01-01 00:00:00.000000 sentient_switchblade-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-25 19:36:38.976660 sentient_switchblade-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8349 2023-05-04 19:24:10.174736 sentient_switchblade-0.3.0/README.md
+-rw-r--r--   0        0        0     1781 2023-05-04 22:15:47.123305 sentient_switchblade-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 19:36:27.260808 sentient_switchblade-0.3.0/src/switchbladecli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 19:35:52.447291 sentient_switchblade-0.3.0/src/switchbladecli/cli/__init__.py
+-rw-r--r--   0        0        0     1491 2023-05-04 19:17:19.432214 sentient_switchblade-0.3.0/src/switchbladecli/cli/__main__.py
+-rw-r--r--   0        0        0    11501 2023-05-04 21:09:34.637478 sentient_switchblade-0.3.0/src/switchbladecli/cli/bundle_cache.py
+-rw-r--r--   0        0        0     1725 2023-05-01 18:05:13.432197 sentient_switchblade-0.3.0/src/switchbladecli/cli/config.py
+-rw-r--r--   0        0        0      677 2023-05-04 20:39:56.373324 sentient_switchblade-0.3.0/src/switchbladecli/cli/lint.py
+-rw-r--r--   0        0        0      683 2023-05-04 20:39:52.194670 sentient_switchblade-0.3.0/src/switchbladecli/cli/test.py
+-rw-r--r--   0        0        0      479 2023-05-04 20:41:51.180130 sentient_switchblade-0.3.0/src/switchbladecli/cli/update.py
+-rw-r--r--   0        0        0      256 2023-05-04 22:00:04.840133 sentient_switchblade-0.3.0/src/switchbladecli/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-26 17:36:55.033765 sentient_switchblade-0.3.0/src/switchbladecli/modes/__init__.py
+-rw-r--r--   0        0        0    11581 2023-05-01 19:58:11.510253 sentient_switchblade-0.3.0/src/switchbladecli/modes/python_poetry.py
+-rw-r--r--   0        0        0      415 2023-05-04 22:00:19.685629 sentient_switchblade-0.3.0/src/switchbladecli/modes/tool_runner.py
+-rw-r--r--   0        0        0      848 2023-05-04 21:04:15.624544 sentient_switchblade-0.3.0/src/switchbladecli/utils.py
+-rw-r--r--   0        0        0     9555 1970-01-01 00:00:00.000000 sentient_switchblade-0.3.0/setup.py
+-rw-r--r--   0        0        0     9756 1970-01-01 00:00:00.000000 sentient_switchblade-0.3.0/PKG-INFO
```

### Comparing `sentient_switchblade-0.2.2/LICENSE` & `sentient_switchblade-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.2.2/README.md` & `sentient_switchblade-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -132,7 +132,21 @@
 Currently, you need Python since you install Switchblade with pip. This may change in the future.
 
 ## Features
 
 - CLI command `swb lint` to run linters
 - CLI command `swb test` to run tests
 - Project 'modes' supported: Currently only `python-poetry` is supported, but more will be added soon.
+
+## Development
+
+Install dependencies:
+
+```shell
+> poetry install
+```
+
+Run unit tests:
+
+```shell
+> poetry run pytest -c pyproject.toml --cov-report=term --cov=src tests
+```
```

#### html2text {}

```diff
@@ -78,8 +78,10 @@
 the project `.switchblade` file. Switchblade will automatically merge (in this
 case it does extend rather than replace) the bundle config and Switchblade
 config before invoking any of the tools. ## Prerequisites - [Python 3.7+]
 (https://www.python.org/downloads/) Currently, you need Python since you
 install Switchblade with pip. This may change in the future. ## Features - CLI
 command `swb lint` to run linters - CLI command `swb test` to run tests -
 Project 'modes' supported: Currently only `python-poetry` is supported, but
-more will be added soon.
+more will be added soon. ## Development Install dependencies: ```shell > poetry
+install ``` Run unit tests: ```shell > poetry run pytest -c pyproject.toml --
+cov-report=term --cov=src tests ```
```

### Comparing `sentient_switchblade-0.2.2/pyproject.toml` & `sentient_switchblade-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sentient-switchblade"
-version = "0.2.2"
+version = "0.3.0"
 description = "Unleash Dev Tool Mastery with a Flick of Your Wrist"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/sentient-switchblade"
 homepage = "https://jensroland.com/sentient-switchblade"
 readme = "README.md"
 packages = [
@@ -35,11 +35,24 @@
 click = "^8.0.3"
 mergedeep = "^1.3.4"
 PyGithub = "^1.58.1"
 python = "^3.7"
 tomlkit = "^0.11.7"
 
 [tool.poetry.group.dev.dependencies]
+pytest = "^7.3.0"
+pytest-cov = "^4.0.0"
+pytest-subprocess = "^1.5.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+# Directories that are not visited by pytest collector:
+norecursedirs =["tests/files", "hooks", "*.egg", ".eggs", "dist", "build", "docs", ".tox", ".git", "__pycache__"]
+pythonpath = "src"
+
+[tool.coverage.report]
+fail_under = 70
+show_missing = true
+skip_empty = true
```

### Comparing `sentient_switchblade-0.2.2/src/switchbladecli/cli/bundle_cache.py` & `sentient_switchblade-0.3.0/src/switchbladecli/cli/bundle_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,42 +31,45 @@
 
         Args:
             switchblade_config (dict): The switchblade config.
             version (str, optional): The version of the bundle to fetch. Defaults to None.
         """
         self._switchblade_config = switchblade_config
         if version is None:
+            click.echo("⚔️ Switchblade initializing bundle...")
             cache = BundleCache(self._switchblade_config)
             bundle = self._fetch_latest(cache)
             self.version = bundle.version
             self.bundle_folder = bundle.bundle_folder
             self.bundle_config = bundle.bundle_config
 
         else:
+            click.echo(f"⚔️ Switchblade initializing bundle with version {version}...")
             self.version = version
             self.bundle_folder = self._bundle_folder_from_version(version)
             self.bundle_config = self._load_bundle_config()
     
 
     def _load_bundle_config(self) -> dict:
         """Get the bundle config from the config file."""
         bundle_config_file = None
         for bundle_config_file_name in BUNDLE_CONFIG_FILES:
             bundle_config_file = self.bundle_folder / bundle_config_file_name
             if bundle_config_file.exists():
                 break
-        if bundle_config_file is None:
+        if bundle_config_file is None or not bundle_config_file.exists():
             raise FileNotFoundError(f"No bundle config file found in bundle {self.version}")
         return loads(bundle_config_file.read_text(encoding="utf-8"))
     
     
     def _bundle_folder_from_version(self, version) -> Path:
         """Get the bundle folder."""
         return Path(CACHE_FOLDERNAME) / version
 
+
     def get_files(self) -> list:
         """Get the list of files (excluding the config) in the bundle.
         
         Returns a list of file paths relative to the bundle folder.
         """
         return [str(file.relative_to(self.bundle_folder)) for file in self.bundle_folder.rglob("*") if file.name not in BUNDLE_CONFIG_FILES]
 
@@ -123,19 +126,20 @@
         bundle_folder = self._bundle_folder_from_version(remote_version)
         if bundle_source_uri.startswith("gh:"):
             # Create the bundle folder
             bundle_folder.mkdir(parents=True)
             # Get the contents of the repo
             org_name, repo_name, *folder = bundle_source_uri[3:].split("/")
             repo = pygithub.get_repo(f"{org_name}/{repo_name}")
-            repo_contents = repo.get_dir_contents("/".join(folder), ref=remote_version)
+            repo_contents = repo.get_contents("/".join(folder), ref=remote_version)
             # Download all the files
             for repo_asset in repo_contents:
                 with open(bundle_folder / repo_asset.name, "wb") as file:
                     file.write(repo_asset.decoded_content)
+
         else:
             # If the source is a local folder, copy it to the cache
             shutil.copytree(bundle_source_uri, bundle_folder)
 
         cache.log(f"UPDATING {remote_version} SUCCEEDED")
 
         new_bundle = Bundle(self._switchblade_config, remote_version)
```

### Comparing `sentient_switchblade-0.2.2/src/switchbladecli/modes/python_poetry.py` & `sentient_switchblade-0.3.0/src/switchbladecli/modes/python_poetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,30 @@
         self._project_folder = Path(config["project_dir"])
         self._verbose = verbose
         self._cache = BundleCache(self._config)
 
 
     # TODO: Make this an override
     def install_dev_tools(self, bundle: Bundle):
+        # Check for a virtualenv and return an error if one is not found
+        check_env = subprocess.run(["poetry", "env", "info", "--path"], cwd=self._project_folder, check=False, capture_output=True)  # nosec
+        if check_env.returncode != 0:
+            raise click.ClickException("No virtualenv found. Please run `poetry install` first.")
+
         # Read pyproject.toml and remove the sections [tool.poetry.group.switchblade]
         # and [tool.poetry.group.switchblade.dependencies], and add the ones from the
         # bundle.toml file in the commit SHA folder
         self._pyproject_file = self._project_folder / "pyproject.toml"
         self._poetry_lockfile = self._project_folder / "poetry.lock"
 
         self._pyproject_file_raw_before = self._pyproject_file.read_text(encoding="utf-8")
-        self._poetry_lockfile_raw_before = self._poetry_lockfile.read_text(encoding="utf-8")  # TODO: handle missing file
+        if self._poetry_lockfile.exists():
+            self._poetry_lockfile_raw_before = self._poetry_lockfile.read_text(encoding="utf-8")
+        else:
+            self._poetry_lockfile_raw_before = None
         pyproject_config = loads(self._pyproject_file_raw_before)
         pyproject_config["tool"]["poetry"]["group"][
             "switchblade"
         ] = bundle.bundle_config["tool"]["poetry"]["group"]["switchblade"]
 
         # Also take all other sections beginning with 'tool.' and add them to the pyproject.toml
         # unless there is already a section with the same name in the pyproject.toml
```

### Comparing `sentient_switchblade-0.2.2/src/switchbladecli/utils.py` & `sentient_switchblade-0.3.0/src/switchbladecli/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import hashlib
 import os
 
+
 def sha1OfFile(filepath, use_sha):
     with open(filepath, 'rb') as f:
         while True:
             block = f.read(2**10) # Magic number: one-megabyte blocks.
             if not block: break
             use_sha.update(block)
         return use_sha.hexdigest()
 
-def hash_dir(dir_path, use_sha=None):
+def hash_dir(dir_path, existing_sha=None):
     for path, dirs, files in os.walk(dir_path):
-        sha = use_sha or hashlib.sha1()
+        sha = existing_sha or hashlib.sha1()
         for file in sorted(files): # we sort to guarantee that files will always go in the same order
             sha1OfFile(os.path.join(path, file), sha)
         for dir in sorted(dirs): # we sort to guarantee that dirs will always go in the same order
             hash_dir(os.path.join(path, dir), sha)
         break # we only need one iteration - to get files and dirs in current directory
     return sha.hexdigest()
```

### Comparing `sentient_switchblade-0.2.2/setup.py` & `sentient_switchblade-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
  'tomlkit>=0.11.7,<0.12.0']
 
 entry_points = \
 {'console_scripts': ['swb = switchbladecli.cli.__main__:switchbladecli']}
 
 setup_kwargs = {
     'name': 'sentient-switchblade',
-    'version': '0.2.2',
+    'version': '0.3.0',
     'description': 'Unleash Dev Tool Mastery with a Flick of Your Wrist',
-    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://github.com/JensRoland/sentient-switchblade">\n    <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png" width="415px" alt="Switchblade logo" />\n  </a>\n</p>\n\n<h3 align="center">Unleash Dev Tool Mastery with a Flick of Your Wrist</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a></p>\n\n<br />\n\n## ⚔️ What is Switchblade?\n\nSwitchblade is a command line tool that lets you install and run dev tools from a central repository, and configure them in a standardised way across all your projects.\n\n## Try it\n\nTo use the included `python-poetry-base` bundle for Python, create a `.switchblade` file in your project root:\n\n```toml\n[switchblade]\nbundle = "gh:jensroland/sentient-switchblade/bundles/python-poetry-base"\nmode = "python-poetry"\n```\n\nThen, install Switchblade in your project and call `swb lint` to run the standard Python linters configured in the base bundle:\n\n```shell\n# Install Switchblade\npoetry add -G dev sentient-switchblade\n\n# Run linters from the bundle\npoetry run swb lint\n```\n\nThat\'s it! :tada: Switchblade will fetch the bundle from Github, install the tools specified in the bundle, and run them with the configurations specified in the bundle. No need to install or configure anything yourself, and no need to commit any dev tooling to your project repo.\n\n**Note**: The base bundle assumes that your source code lives under `src/` and your tests under `tests/`, but it is only meant as an example. To specify your own dev tools and tailor them to your needs and project structure, create your own custom bundle (see below).\n\n## Who is this for?\n\nSwitchblade was born from the question: *"How do I ensure that I\'m using the same linting and testing configurations across all of my project repositories?"* Are all of your Python repos using the same version of `Black`? Maybe you switched to `flake8` on your newer repos but never updated the old ones? Sure, maybe it doesn\'t matter very much if your tooling deviates a little between your personal projects, but how about this: when your company\'s DevSecOps team updated all the templates to include scans for known vulnerabilities and credential leaks, did you remember to update all of your repos? And if not, how would you even know?\n\nTo complicate matters, developer tooling is not simply about choosing a particular linter and firing it up. It\'s also how you configure it -- maximum line lengths, whether to use single or double quotes, what rules to ignore entirely -- as well as which arguments to pass when you invoke it.\n\n<!-- Every software engineering organisation has to deal with these issues, and while many solutions exist, they are hardly perfect:\n\n1. Provide project templates with dev tooling built-in, and use those templates to create new projects. This works well initially, but results in duplicated configuration files and makes all subsequent configuration updates both time consuming and error prone, since they have to be made in all projects at once.\n2. Let configs be duplicated across projects and use [a meta-repo tool](https://github.com/mateodelnorte/meta) to perform cross-repo updates. This requires a non-trivial amount of setup and maintenance, and updating a dev configuration still requires committing changes in every repo.\n3. Combine all dev tooling in a package and install it in every project. This works for some types of tooling, but many tools require their config files to exist in the project root rather than inside a package. It also usually requires committing changes (e.g. the updated lockfile) in every repo to get the latest configurations.\n4. Use a monorepo; have one set of dev tools included in the repo and use it for everything. This can actually be a great solution, but it\'s not always possible or desirable to use a monorepo.\n5. Something custom involving Docker containers and prebaked images with dev tools. This involves a lot of complexity and overhead, plus you get all the limitations of the package solution. -->\n\nIn an ideal world, dev tooling would not be checked into version control (*seriously*) but rather **fetched on demand from a centrally managed dev tooling repository, and configured and invoked in exactly the same way in every repo, every time**. This would allow for a single source of truth for all dev tooling, and would make it easy to update configurations across all projects.\n\nTo achieve this however, you would need some kind of small helper tool to abstract away the fetching, configuring and invoking of your centrally curated \'bundles\' of dev tools.\n\nSwitchblade is that tool.\n\n## Custom bundles\n\nTo create your own custom bundle with the dev tools and configurations you need, simply create a new Github repo and add a `bundle.toml` file to it:\n\n```toml\n[bundle]\nname = "my-dev-tool-bundle"\nmode = "python-poetry"\nschema_version = "1.0.0"\n\n# Linters\n[linters]\nall = ["pylint"]\n\n[linters.pylint]\ncommand = "pylint src"\n\n# Tests\n[tests]\nall = ["pytest"]\n\n[tests.pytest]\ncommand = "pytest -c pyproject.toml tests"\n\n# Extensions to pyproject.toml\n[tool.poetry.group.switchblade]\noptional = true\n\n[tool.poetry.group.switchblade.dependencies]\npylint = "^2.17.2"\npytest = "^7.3.1"\n\n[tool.pytest.ini_options]\npythonpath = "src"\n```\n\nFor each linter you want to add, specify a `[linters.<toolname>]` section with a `command` key. The `command` value will be invoked by Switchblade when you run `swb lint <toolname>`.\n\nThe `[linters]` section specifies which linters should be invoked (and in which order) when you run `swb lint` or `swb lint all`.\n\nThe same goes for tests: specify a `[tests.<toolname>]` section with a `command` key, and add the tool to the `[tests]` section to have it invoked when you run `swb test` or `swb test all`.\n\n### Tool configuration\n\nAnything in the `bundle.toml` file under a `tool.*` section will be temporarily added to the project\'s `pyproject.toml` file under that section. This allows you to add dependencies and configuration options to all your projects without having to manually edit all the individual `pyproject.toml` files.\n\nIf you prefer having separate config files, or for tools which do not support `pyproject.toml` configuration, simply add any config files you need in the same folder as the `bundle.toml` file. E.g. you might define a `.pylintrc` in the bundle repo:\n\n```ini\n[MAIN]\n[MESSAGES CONTROL]\ndisable=\n    C0111,  # missing-docstring\n    C0114,  # missing-module-docstring\n    C0115,  # missing-class-docstring\n    C0116,  # missing-function-docstring\n    W0613,  # unused-argument\n```\n\nNow, when you want to use your custom dev tool bundle in a project, simply point to the repo in the project `.switchblade` file as in the example above. Swichblade will then fetch and install the tools you specified in the bundle and run them with the configurations you specified.\n\n### Per-project overrides\n\nTo override the bundle configuration for a specific dev tool in one of your project repos, simply check in the tool dependencies and configuration files in the project repo as you normally would - Switchblade will still invoke the dev tool, but it will not overwrite any existing config files or `[tool.*]` sections in your `pyproject.toml` file. Be aware that this does not \'extend\' the configuration from the bundle, but replaces that tool configuration entirely, so this feature should be used with caution.\n\nTo override the command or the list of linters to run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]` in the project `.switchblade` file. Switchblade will automatically merge (in this case it does extend rather than replace) the bundle config and Switchblade config before invoking any of the tools.\n\n## Prerequisites\n\n- [Python 3.7+](https://www.python.org/downloads/)\n\nCurrently, you need Python since you install Switchblade with pip. This may change in the future.\n\n## Features\n\n- CLI command `swb lint` to run linters\n- CLI command `swb test` to run tests\n- Project \'modes\' supported: Currently only `python-poetry` is supported, but more will be added soon.\n',
+    'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://github.com/JensRoland/sentient-switchblade">\n    <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png" width="415px" alt="Switchblade logo" />\n  </a>\n</p>\n\n<h3 align="center">Unleash Dev Tool Mastery with a Flick of Your Wrist</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a></p>\n\n<br />\n\n## ⚔️ What is Switchblade?\n\nSwitchblade is a command line tool that lets you install and run dev tools from a central repository, and configure them in a standardised way across all your projects.\n\n## Try it\n\nTo use the included `python-poetry-base` bundle for Python, create a `.switchblade` file in your project root:\n\n```toml\n[switchblade]\nbundle = "gh:jensroland/sentient-switchblade/bundles/python-poetry-base"\nmode = "python-poetry"\n```\n\nThen, install Switchblade in your project and call `swb lint` to run the standard Python linters configured in the base bundle:\n\n```shell\n# Install Switchblade\npoetry add -G dev sentient-switchblade\n\n# Run linters from the bundle\npoetry run swb lint\n```\n\nThat\'s it! :tada: Switchblade will fetch the bundle from Github, install the tools specified in the bundle, and run them with the configurations specified in the bundle. No need to install or configure anything yourself, and no need to commit any dev tooling to your project repo.\n\n**Note**: The base bundle assumes that your source code lives under `src/` and your tests under `tests/`, but it is only meant as an example. To specify your own dev tools and tailor them to your needs and project structure, create your own custom bundle (see below).\n\n## Who is this for?\n\nSwitchblade was born from the question: *"How do I ensure that I\'m using the same linting and testing configurations across all of my project repositories?"* Are all of your Python repos using the same version of `Black`? Maybe you switched to `flake8` on your newer repos but never updated the old ones? Sure, maybe it doesn\'t matter very much if your tooling deviates a little between your personal projects, but how about this: when your company\'s DevSecOps team updated all the templates to include scans for known vulnerabilities and credential leaks, did you remember to update all of your repos? And if not, how would you even know?\n\nTo complicate matters, developer tooling is not simply about choosing a particular linter and firing it up. It\'s also how you configure it -- maximum line lengths, whether to use single or double quotes, what rules to ignore entirely -- as well as which arguments to pass when you invoke it.\n\n<!-- Every software engineering organisation has to deal with these issues, and while many solutions exist, they are hardly perfect:\n\n1. Provide project templates with dev tooling built-in, and use those templates to create new projects. This works well initially, but results in duplicated configuration files and makes all subsequent configuration updates both time consuming and error prone, since they have to be made in all projects at once.\n2. Let configs be duplicated across projects and use [a meta-repo tool](https://github.com/mateodelnorte/meta) to perform cross-repo updates. This requires a non-trivial amount of setup and maintenance, and updating a dev configuration still requires committing changes in every repo.\n3. Combine all dev tooling in a package and install it in every project. This works for some types of tooling, but many tools require their config files to exist in the project root rather than inside a package. It also usually requires committing changes (e.g. the updated lockfile) in every repo to get the latest configurations.\n4. Use a monorepo; have one set of dev tools included in the repo and use it for everything. This can actually be a great solution, but it\'s not always possible or desirable to use a monorepo.\n5. Something custom involving Docker containers and prebaked images with dev tools. This involves a lot of complexity and overhead, plus you get all the limitations of the package solution. -->\n\nIn an ideal world, dev tooling would not be checked into version control (*seriously*) but rather **fetched on demand from a centrally managed dev tooling repository, and configured and invoked in exactly the same way in every repo, every time**. This would allow for a single source of truth for all dev tooling, and would make it easy to update configurations across all projects.\n\nTo achieve this however, you would need some kind of small helper tool to abstract away the fetching, configuring and invoking of your centrally curated \'bundles\' of dev tools.\n\nSwitchblade is that tool.\n\n## Custom bundles\n\nTo create your own custom bundle with the dev tools and configurations you need, simply create a new Github repo and add a `bundle.toml` file to it:\n\n```toml\n[bundle]\nname = "my-dev-tool-bundle"\nmode = "python-poetry"\nschema_version = "1.0.0"\n\n# Linters\n[linters]\nall = ["pylint"]\n\n[linters.pylint]\ncommand = "pylint src"\n\n# Tests\n[tests]\nall = ["pytest"]\n\n[tests.pytest]\ncommand = "pytest -c pyproject.toml tests"\n\n# Extensions to pyproject.toml\n[tool.poetry.group.switchblade]\noptional = true\n\n[tool.poetry.group.switchblade.dependencies]\npylint = "^2.17.2"\npytest = "^7.3.1"\n\n[tool.pytest.ini_options]\npythonpath = "src"\n```\n\nFor each linter you want to add, specify a `[linters.<toolname>]` section with a `command` key. The `command` value will be invoked by Switchblade when you run `swb lint <toolname>`.\n\nThe `[linters]` section specifies which linters should be invoked (and in which order) when you run `swb lint` or `swb lint all`.\n\nThe same goes for tests: specify a `[tests.<toolname>]` section with a `command` key, and add the tool to the `[tests]` section to have it invoked when you run `swb test` or `swb test all`.\n\n### Tool configuration\n\nAnything in the `bundle.toml` file under a `tool.*` section will be temporarily added to the project\'s `pyproject.toml` file under that section. This allows you to add dependencies and configuration options to all your projects without having to manually edit all the individual `pyproject.toml` files.\n\nIf you prefer having separate config files, or for tools which do not support `pyproject.toml` configuration, simply add any config files you need in the same folder as the `bundle.toml` file. E.g. you might define a `.pylintrc` in the bundle repo:\n\n```ini\n[MAIN]\n[MESSAGES CONTROL]\ndisable=\n    C0111,  # missing-docstring\n    C0114,  # missing-module-docstring\n    C0115,  # missing-class-docstring\n    C0116,  # missing-function-docstring\n    W0613,  # unused-argument\n```\n\nNow, when you want to use your custom dev tool bundle in a project, simply point to the repo in the project `.switchblade` file as in the example above. Swichblade will then fetch and install the tools you specified in the bundle and run them with the configurations you specified.\n\n### Per-project overrides\n\nTo override the bundle configuration for a specific dev tool in one of your project repos, simply check in the tool dependencies and configuration files in the project repo as you normally would - Switchblade will still invoke the dev tool, but it will not overwrite any existing config files or `[tool.*]` sections in your `pyproject.toml` file. Be aware that this does not \'extend\' the configuration from the bundle, but replaces that tool configuration entirely, so this feature should be used with caution.\n\nTo override the command or the list of linters to run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]` in the project `.switchblade` file. Switchblade will automatically merge (in this case it does extend rather than replace) the bundle config and Switchblade config before invoking any of the tools.\n\n## Prerequisites\n\n- [Python 3.7+](https://www.python.org/downloads/)\n\nCurrently, you need Python since you install Switchblade with pip. This may change in the future.\n\n## Features\n\n- CLI command `swb lint` to run linters\n- CLI command `swb test` to run tests\n- Project \'modes\' supported: Currently only `python-poetry` is supported, but more will be added soon.\n\n## Development\n\nInstall dependencies:\n\n```shell\n> poetry install\n```\n\nRun unit tests:\n\n```shell\n> poetry run pytest -c pyproject.toml --cov-report=term --cov=src tests\n```\n',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://jensroland.com/sentient-switchblade',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['switchbladecli', 'switchbladecli.cli',
 'switchbladecli.modes'] package_data = \ {'': ['*']} install_requires = \
 ['PyGithub>=1.58.1,<2.0.0', 'checksumdir>=1.2.0,<2.0.0', 'click>=8.0.3,<9.0.0',
 'mergedeep>=1.3.4,<2.0.0', 'tomlkit>=0.11.7,<0.12.0'] entry_points = \
 {'console_scripts': ['swb = switchbladecli.cli.__main__:switchbladecli']}
-setup_kwargs = { 'name': 'sentient-switchblade', 'version': '0.2.2',
+setup_kwargs = { 'name': 'sentient-switchblade', 'version': '0.3.0',
 'description': 'Unleash Dev Tool Mastery with a Flick of Your Wrist',
 'long_description': '\n
                          \n \n_[Switchblade_logo]\n\n
 \n\n
          **** Unleash Dev Tool Mastery with a Flick of Your Wrist ****
 \n
                             Created by Jens_Roland
@@ -92,13 +92,16 @@
 in the project `.switchblade` file. Switchblade will automatically merge (in
 this case it does extend rather than replace) the bundle config and Switchblade
 config before invoking any of the tools.\n\n## Prerequisites\n\n- [Python 3.7+]
 (https://www.python.org/downloads/)\n\nCurrently, you need Python since you
 install Switchblade with pip. This may change in the future.\n\n##
 Features\n\n- CLI command `swb lint` to run linters\n- CLI command `swb test`
 to run tests\n- Project \'modes\' supported: Currently only `python-poetry` is
-supported, but more will be added soon.\n', 'author': 'JensRoland',
-'author_email': 'mail@jensroland.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://jensroland.com/sentient-
-switchblade', 'package_dir': package_dir, 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'entry_points':
-entry_points, 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+supported, but more will be added soon.\n\n## Development\n\nInstall
+dependencies:\n\n```shell\n> poetry install\n```\n\nRun unit tests:
+\n\n```shell\n> poetry run pytest -c pyproject.toml --cov-report=term --cov=src
+tests\n```\n', 'author': 'JensRoland', 'author_email': 'mail@jensroland.com',
+'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://
+jensroland.com/sentient-switchblade', 'package_dir': package_dir, 'packages':
+packages, 'package_data': package_data, 'install_requires': install_requires,
+'entry_points': entry_points, 'python_requires': '>=3.7,<4.0', } setup
+(**setup_kwargs)
```

### Comparing `sentient_switchblade-0.2.2/PKG-INFO` & `sentient_switchblade-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentient-switchblade
-Version: 0.2.2
+Version: 0.3.0
 Summary: Unleash Dev Tool Mastery with a Flick of Your Wrist
 Home-page: https://jensroland.com/sentient-switchblade
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -166,7 +166,21 @@
 
 ## Features
 
 - CLI command `swb lint` to run linters
 - CLI command `swb test` to run tests
 - Project 'modes' supported: Currently only `python-poetry` is supported, but more will be added soon.
 
+## Development
+
+Install dependencies:
+
+```shell
+> poetry install
+```
+
+Run unit tests:
+
+```shell
+> poetry run pytest -c pyproject.toml --cov-report=term --cov=src tests
+```
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentient-switchblade Version: 0.2.2 Summary:
+Metadata-Version: 2.1 Name: sentient-switchblade Version: 0.3.0 Summary:
 Unleash Dev Tool Mastery with a Flick of Your Wrist Home-page: https://
 jensroland.com/sentient-switchblade License: MIT Author: JensRoland Author-
 email: mail@jensroland.com Requires-Python: >=3.7,<4.0 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
@@ -97,8 +97,10 @@
 the project `.switchblade` file. Switchblade will automatically merge (in this
 case it does extend rather than replace) the bundle config and Switchblade
 config before invoking any of the tools. ## Prerequisites - [Python 3.7+]
 (https://www.python.org/downloads/) Currently, you need Python since you
 install Switchblade with pip. This may change in the future. ## Features - CLI
 command `swb lint` to run linters - CLI command `swb test` to run tests -
 Project 'modes' supported: Currently only `python-poetry` is supported, but
-more will be added soon.
+more will be added soon. ## Development Install dependencies: ```shell > poetry
+install ``` Run unit tests: ```shell > poetry run pytest -c pyproject.toml --
+cov-report=term --cov=src tests ```
```

