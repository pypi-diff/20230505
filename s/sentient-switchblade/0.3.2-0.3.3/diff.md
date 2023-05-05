# Comparing `tmp/sentient_switchblade-0.3.2.tar.gz` & `tmp/sentient_switchblade-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentient_switchblade-0.3.2.tar", max compression
+gzip compressed data, was "sentient_switchblade-0.3.3.tar", max compression
```

## Comparing `sentient_switchblade-0.3.2.tar` & `sentient_switchblade-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1077 2023-04-25 19:36:38.976660 sentient_switchblade-0.3.2/LICENSE
--rw-r--r--   0        0        0     8349 2023-05-04 19:24:10.174736 sentient_switchblade-0.3.2/README.md
--rw-r--r--   0        0        0     1781 2023-05-04 22:47:02.503505 sentient_switchblade-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 19:36:27.260808 sentient_switchblade-0.3.2/src/switchbladecli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 19:35:52.447291 sentient_switchblade-0.3.2/src/switchbladecli/cli/__init__.py
--rw-r--r--   0        0        0     1491 2023-05-04 19:17:19.432214 sentient_switchblade-0.3.2/src/switchbladecli/cli/__main__.py
--rw-r--r--   0        0        0    11501 2023-05-04 21:09:34.637478 sentient_switchblade-0.3.2/src/switchbladecli/cli/bundle_cache.py
--rw-r--r--   0        0        0     1725 2023-05-01 18:05:13.432197 sentient_switchblade-0.3.2/src/switchbladecli/cli/config.py
--rw-r--r--   0        0        0      677 2023-05-04 22:29:41.057878 sentient_switchblade-0.3.2/src/switchbladecli/cli/lint.py
--rw-r--r--   0        0        0      683 2023-05-04 20:39:52.194670 sentient_switchblade-0.3.2/src/switchbladecli/cli/test.py
--rw-r--r--   0        0        0      479 2023-05-04 20:41:51.180130 sentient_switchblade-0.3.2/src/switchbladecli/cli/update.py
--rw-r--r--   0        0        0      256 2023-05-04 22:00:04.840133 sentient_switchblade-0.3.2/src/switchbladecli/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-26 17:36:55.033765 sentient_switchblade-0.3.2/src/switchbladecli/modes/__init__.py
--rw-r--r--   0        0        0    11679 2023-05-04 22:46:42.476592 sentient_switchblade-0.3.2/src/switchbladecli/modes/python_poetry.py
--rw-r--r--   0        0        0      415 2023-05-04 22:00:19.685629 sentient_switchblade-0.3.2/src/switchbladecli/modes/tool_runner.py
--rw-r--r--   0        0        0      848 2023-05-04 21:04:15.624544 sentient_switchblade-0.3.2/src/switchbladecli/utils.py
--rw-r--r--   0        0        0     9555 1970-01-01 00:00:00.000000 sentient_switchblade-0.3.2/setup.py
--rw-r--r--   0        0        0     9756 1970-01-01 00:00:00.000000 sentient_switchblade-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-25 19:36:38.976660 sentient_switchblade-0.3.3/LICENSE
+-rw-r--r--   0        0        0     8349 2023-05-04 19:24:10.174736 sentient_switchblade-0.3.3/README.md
+-rw-r--r--   0        0        0     1781 2023-05-05 20:47:47.720318 sentient_switchblade-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 19:36:27.260808 sentient_switchblade-0.3.3/src/switchbladecli/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 19:35:52.447291 sentient_switchblade-0.3.3/src/switchbladecli/cli/__init__.py
+-rw-r--r--   0        0        0     1491 2023-05-04 19:17:19.432214 sentient_switchblade-0.3.3/src/switchbladecli/cli/__main__.py
+-rw-r--r--   0        0        0    11501 2023-05-04 21:09:34.637478 sentient_switchblade-0.3.3/src/switchbladecli/cli/bundle_cache.py
+-rw-r--r--   0        0        0     1725 2023-05-01 18:05:13.432197 sentient_switchblade-0.3.3/src/switchbladecli/cli/config.py
+-rw-r--r--   0        0        0      734 2023-05-05 20:07:43.738620 sentient_switchblade-0.3.3/src/switchbladecli/cli/lint.py
+-rw-r--r--   0        0        0      740 2023-05-05 20:08:11.028589 sentient_switchblade-0.3.3/src/switchbladecli/cli/test.py
+-rw-r--r--   0        0        0      479 2023-05-04 20:41:51.180130 sentient_switchblade-0.3.3/src/switchbladecli/cli/update.py
+-rw-r--r--   0        0        0      256 2023-05-04 22:00:04.840133 sentient_switchblade-0.3.3/src/switchbladecli/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-26 17:36:55.033765 sentient_switchblade-0.3.3/src/switchbladecli/modes/__init__.py
+-rw-r--r--   0        0        0    11861 2023-05-05 20:24:32.708701 sentient_switchblade-0.3.3/src/switchbladecli/modes/python_poetry.py
+-rw-r--r--   0        0        0      415 2023-05-04 22:00:19.685629 sentient_switchblade-0.3.3/src/switchbladecli/modes/tool_runner.py
+-rw-r--r--   0        0        0      848 2023-05-04 21:04:15.624544 sentient_switchblade-0.3.3/src/switchbladecli/utils.py
+-rw-r--r--   0        0        0     9555 1970-01-01 00:00:00.000000 sentient_switchblade-0.3.3/setup.py
+-rw-r--r--   0        0        0     9756 1970-01-01 00:00:00.000000 sentient_switchblade-0.3.3/PKG-INFO
```

### Comparing `sentient_switchblade-0.3.2/LICENSE` & `sentient_switchblade-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.3.2/README.md` & `sentient_switchblade-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.3.2/pyproject.toml` & `sentient_switchblade-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sentient-switchblade"
-version = "0.3.2"
+version = "0.3.3"
 description = "Unleash Dev Tool Mastery with a Flick of Your Wrist"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/sentient-switchblade"
 homepage = "https://jensroland.com/sentient-switchblade"
 readme = "README.md"
 packages = [
```

### Comparing `sentient_switchblade-0.3.2/src/switchbladecli/cli/__main__.py` & `sentient_switchblade-0.3.3/src/switchbladecli/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.3.2/src/switchbladecli/cli/bundle_cache.py` & `sentient_switchblade-0.3.3/src/switchbladecli/cli/bundle_cache.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.3.2/src/switchbladecli/cli/config.py` & `sentient_switchblade-0.3.3/src/switchbladecli/cli/config.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.3.2/src/switchbladecli/cli/lint.py` & `sentient_switchblade-0.3.3/src/switchbladecli/cli/lint.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,13 +9,15 @@
 @click.pass_context
 def lint(ctx, linter: str):
     """Run linter(s) on project.
     
     LINTER: Linter to run. If not specified, all linters will be run.
     """
     project_dir, config, verbose = itemgetter("project_dir", "config", "verbose")(ctx.obj)
-    cmd_lint(verbose, project_dir, config, linter)
+    result = cmd_lint(verbose, project_dir, config, linter)
+    if not result:
+        ctx.exit(1)
 
 
 def cmd_lint(verbose: bool, project_dir: str, config: dict, linter_tool: str = "all"):
     tool_runner = get_tool_runner(config)(config, verbose)
-    tool_runner.lint(linter_tool)
+    return tool_runner.lint(linter_tool)
```

### Comparing `sentient_switchblade-0.3.2/src/switchbladecli/cli/test.py` & `sentient_switchblade-0.3.3/src/switchbladecli/cli/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,13 +9,15 @@
 @click.pass_context
 def test(ctx, test: str):
     """Run testing tool(s) on project.
     
     TEST: Testing tool to run. If not specified, all testing tools will be run.
     """
     project_dir, config, verbose = itemgetter("project_dir", "config", "verbose")(ctx.obj)
-    cmd_test(verbose, project_dir, config, test)
+    result = cmd_test(verbose, project_dir, config, test)
+    if not result:
+        ctx.exit(1)
 
 
 def cmd_test(verbose: bool, project_dir: str, config: dict, test_tool: str = "all"):
     tool_runner = get_tool_runner(config)(config, verbose)
-    tool_runner.test(test_tool)
+    return tool_runner.test(test_tool)
```

### Comparing `sentient_switchblade-0.3.2/src/switchbladecli/modes/python_poetry.py` & `sentient_switchblade-0.3.3/src/switchbladecli/modes/python_poetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,16 +165,17 @@
             # Apply local overrides from .switchblade (merging the linter dicts) if any
             switchblade_linters_config = self._config["linters"] if "linters" in self._config else {}
             merged_linters_config = merge({}, bundle_config["linters"], switchblade_linters_config)
 
             success = True
             linter_names = merged_linters_config["all"] if linter_tool in ["all", None] else [linter_tool]
             for linter_name in linter_names:
-                print(f"⚔️ Switchblade running {linter_name}...")
+                print(f"⚔️ Switchblade running {linter_name}...", end=" ")
                 linter_success = self.run_linter(latest_bundle, merged_linters_config[linter_name])
+                print("✅" if linter_success else "❌")
                 success = success and linter_success
                 self._cache.log(f"RAN {linter_name}")
 
         except Exception as exc:
             self._cache.log(f"LINTING {latest_bundle.version} FAILED_WITH_EXCEPTION")
             raise click.ClickException(f"Exception detected while running linters, aborting... {exc}")
 
@@ -190,14 +191,16 @@
         if success:
             self._cache.log(f"LINTING {latest_bundle.version} FINISHED_SUCCESSFULLY")
             click.echo("⚔️ Linting finished successfully. 😎")
         else:
             self._cache.log(f"LINTING {latest_bundle.version} FINISHED_WITH_ERRORS")
             click.secho("⚔️ Linting finished with errors. 😭", err=True, fg="red", bold=True)
 
+        return success
+
 
     # TODO: Place this in a superclass
     def test(self, test_tool: str):
         # Instantiating a Bundle object will fetch the latest bundle from the source or cache
         latest_bundle = Bundle(self._config)
 
         bundle_config = latest_bundle.bundle_config
@@ -234,16 +237,17 @@
             bundle_tests_config = bundle_config["tests"]
             switchblade_tests_config = self._config["tests"] if "tests" in self._config else {}
             merged_tests_config = merge({}, bundle_tests_config, switchblade_tests_config)
 
             success = True
             test_tool_names = merged_tests_config["all"] if test_tool in ["all", None] else [test_tool]
             for test_tool_name in test_tool_names:
-                print(f"⚔️ Switchblade running {test_tool_name}...")
+                print(f"⚔️ Switchblade running {test_tool_name}...", end = " ")
                 test_success = self.run_test(latest_bundle, merged_tests_config[test_tool_name])
+                print("✅" if test_success else "❌")
                 success = success and test_success
                 self._cache.log(f"RAN {test_tool_name}")
 
         except Exception as exc:
             self._cache.log(f"TESTING {latest_bundle.version} FAILED_WITH_EXCEPTION")
             raise click.ClickException(f"Exception detected while running tests, aborting... {exc}")
 
@@ -258,7 +262,9 @@
 
         if success:
             self._cache.log(f"TESTING {latest_bundle.version} FINISHED_SUCCESSFULLY")
             click.echo("⚔️ Tests finished successfully. 😎")
         else:
             self._cache.log(f"TESTING {latest_bundle.version} FINISHED_WITH_ERRORS")
             click.secho("⚔️ Tests finished with errors. 😭", err=True, fg="red", bold=True)
+
+        return success
```

### Comparing `sentient_switchblade-0.3.2/src/switchbladecli/utils.py` & `sentient_switchblade-0.3.3/src/switchbladecli/utils.py`

 * *Files identical despite different names*

### Comparing `sentient_switchblade-0.3.2/setup.py` & `sentient_switchblade-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'tomlkit>=0.11.7,<0.12.0']
 
 entry_points = \
 {'console_scripts': ['swb = switchbladecli.cli.__main__:switchbladecli']}
 
 setup_kwargs = {
     'name': 'sentient-switchblade',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'Unleash Dev Tool Mastery with a Flick of Your Wrist',
     'long_description': '<!-- markdownlint-disable first-line-h1 line-length no-inline-html -->\n<p align="center">\n  <a href="https://github.com/JensRoland/sentient-switchblade">\n    <img src="https://jensroland.com/switchblade/assets/switchblade-logotype.png" width="415px" alt="Switchblade logo" />\n  </a>\n</p>\n\n<h3 align="center">Unleash Dev Tool Mastery with a Flick of Your Wrist</h3>\n<p align="center">Created by <a href="https://jensroland.com/">Jens Roland</a></p>\n\n<br />\n\n## ⚔️ What is Switchblade?\n\nSwitchblade is a command line tool that lets you install and run dev tools from a central repository, and configure them in a standardised way across all your projects.\n\n## Try it\n\nTo use the included `python-poetry-base` bundle for Python, create a `.switchblade` file in your project root:\n\n```toml\n[switchblade]\nbundle = "gh:jensroland/sentient-switchblade/bundles/python-poetry-base"\nmode = "python-poetry"\n```\n\nThen, install Switchblade in your project and call `swb lint` to run the standard Python linters configured in the base bundle:\n\n```shell\n# Install Switchblade\npoetry add -G dev sentient-switchblade\n\n# Run linters from the bundle\npoetry run swb lint\n```\n\nThat\'s it! :tada: Switchblade will fetch the bundle from Github, install the tools specified in the bundle, and run them with the configurations specified in the bundle. No need to install or configure anything yourself, and no need to commit any dev tooling to your project repo.\n\n**Note**: The base bundle assumes that your source code lives under `src/` and your tests under `tests/`, but it is only meant as an example. To specify your own dev tools and tailor them to your needs and project structure, create your own custom bundle (see below).\n\n## Who is this for?\n\nSwitchblade was born from the question: *"How do I ensure that I\'m using the same linting and testing configurations across all of my project repositories?"* Are all of your Python repos using the same version of `Black`? Maybe you switched to `flake8` on your newer repos but never updated the old ones? Sure, maybe it doesn\'t matter very much if your tooling deviates a little between your personal projects, but how about this: when your company\'s DevSecOps team updated all the templates to include scans for known vulnerabilities and credential leaks, did you remember to update all of your repos? And if not, how would you even know?\n\nTo complicate matters, developer tooling is not simply about choosing a particular linter and firing it up. It\'s also how you configure it -- maximum line lengths, whether to use single or double quotes, what rules to ignore entirely -- as well as which arguments to pass when you invoke it.\n\n<!-- Every software engineering organisation has to deal with these issues, and while many solutions exist, they are hardly perfect:\n\n1. Provide project templates with dev tooling built-in, and use those templates to create new projects. This works well initially, but results in duplicated configuration files and makes all subsequent configuration updates both time consuming and error prone, since they have to be made in all projects at once.\n2. Let configs be duplicated across projects and use [a meta-repo tool](https://github.com/mateodelnorte/meta) to perform cross-repo updates. This requires a non-trivial amount of setup and maintenance, and updating a dev configuration still requires committing changes in every repo.\n3. Combine all dev tooling in a package and install it in every project. This works for some types of tooling, but many tools require their config files to exist in the project root rather than inside a package. It also usually requires committing changes (e.g. the updated lockfile) in every repo to get the latest configurations.\n4. Use a monorepo; have one set of dev tools included in the repo and use it for everything. This can actually be a great solution, but it\'s not always possible or desirable to use a monorepo.\n5. Something custom involving Docker containers and prebaked images with dev tools. This involves a lot of complexity and overhead, plus you get all the limitations of the package solution. -->\n\nIn an ideal world, dev tooling would not be checked into version control (*seriously*) but rather **fetched on demand from a centrally managed dev tooling repository, and configured and invoked in exactly the same way in every repo, every time**. This would allow for a single source of truth for all dev tooling, and would make it easy to update configurations across all projects.\n\nTo achieve this however, you would need some kind of small helper tool to abstract away the fetching, configuring and invoking of your centrally curated \'bundles\' of dev tools.\n\nSwitchblade is that tool.\n\n## Custom bundles\n\nTo create your own custom bundle with the dev tools and configurations you need, simply create a new Github repo and add a `bundle.toml` file to it:\n\n```toml\n[bundle]\nname = "my-dev-tool-bundle"\nmode = "python-poetry"\nschema_version = "1.0.0"\n\n# Linters\n[linters]\nall = ["pylint"]\n\n[linters.pylint]\ncommand = "pylint src"\n\n# Tests\n[tests]\nall = ["pytest"]\n\n[tests.pytest]\ncommand = "pytest -c pyproject.toml tests"\n\n# Extensions to pyproject.toml\n[tool.poetry.group.switchblade]\noptional = true\n\n[tool.poetry.group.switchblade.dependencies]\npylint = "^2.17.2"\npytest = "^7.3.1"\n\n[tool.pytest.ini_options]\npythonpath = "src"\n```\n\nFor each linter you want to add, specify a `[linters.<toolname>]` section with a `command` key. The `command` value will be invoked by Switchblade when you run `swb lint <toolname>`.\n\nThe `[linters]` section specifies which linters should be invoked (and in which order) when you run `swb lint` or `swb lint all`.\n\nThe same goes for tests: specify a `[tests.<toolname>]` section with a `command` key, and add the tool to the `[tests]` section to have it invoked when you run `swb test` or `swb test all`.\n\n### Tool configuration\n\nAnything in the `bundle.toml` file under a `tool.*` section will be temporarily added to the project\'s `pyproject.toml` file under that section. This allows you to add dependencies and configuration options to all your projects without having to manually edit all the individual `pyproject.toml` files.\n\nIf you prefer having separate config files, or for tools which do not support `pyproject.toml` configuration, simply add any config files you need in the same folder as the `bundle.toml` file. E.g. you might define a `.pylintrc` in the bundle repo:\n\n```ini\n[MAIN]\n[MESSAGES CONTROL]\ndisable=\n    C0111,  # missing-docstring\n    C0114,  # missing-module-docstring\n    C0115,  # missing-class-docstring\n    C0116,  # missing-function-docstring\n    W0613,  # unused-argument\n```\n\nNow, when you want to use your custom dev tool bundle in a project, simply point to the repo in the project `.switchblade` file as in the example above. Swichblade will then fetch and install the tools you specified in the bundle and run them with the configurations you specified.\n\n### Per-project overrides\n\nTo override the bundle configuration for a specific dev tool in one of your project repos, simply check in the tool dependencies and configuration files in the project repo as you normally would - Switchblade will still invoke the dev tool, but it will not overwrite any existing config files or `[tool.*]` sections in your `pyproject.toml` file. Be aware that this does not \'extend\' the configuration from the bundle, but replaces that tool configuration entirely, so this feature should be used with caution.\n\nTo override the command or the list of linters to run, add the corresponding sections (e.g. `[linters]` or `[linters.pylint]` in the project `.switchblade` file. Switchblade will automatically merge (in this case it does extend rather than replace) the bundle config and Switchblade config before invoking any of the tools.\n\n## Prerequisites\n\n- [Python 3.7+](https://www.python.org/downloads/)\n\nCurrently, you need Python since you install Switchblade with pip. This may change in the future.\n\n## Features\n\n- CLI command `swb lint` to run linters\n- CLI command `swb test` to run tests\n- Project \'modes\' supported: Currently only `python-poetry` is supported, but more will be added soon.\n\n## Development\n\nInstall dependencies:\n\n```shell\n> poetry install\n```\n\nRun unit tests:\n\n```shell\n> poetry run pytest -c pyproject.toml --cov-report=term --cov=src tests\n```\n',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://jensroland.com/sentient-switchblade',
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
-setup_kwargs = { 'name': 'sentient-switchblade', 'version': '0.3.2',
+setup_kwargs = { 'name': 'sentient-switchblade', 'version': '0.3.3',
 'description': 'Unleash Dev Tool Mastery with a Flick of Your Wrist',
 'long_description': '\n
                          \n \n_[Switchblade_logo]\n\n
 \n\n
          **** Unleash Dev Tool Mastery with a Flick of Your Wrist ****
 \n
                             Created by Jens_Roland
```

### Comparing `sentient_switchblade-0.3.2/PKG-INFO` & `sentient_switchblade-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentient-switchblade
-Version: 0.3.2
+Version: 0.3.3
 Summary: Unleash Dev Tool Mastery with a Flick of Your Wrist
 Home-page: https://jensroland.com/sentient-switchblade
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentient-switchblade Version: 0.3.2 Summary:
+Metadata-Version: 2.1 Name: sentient-switchblade Version: 0.3.3 Summary:
 Unleash Dev Tool Mastery with a Flick of Your Wrist Home-page: https://
 jensroland.com/sentient-switchblade License: MIT Author: JensRoland Author-
 email: mail@jensroland.com Requires-Python: >=3.7,<4.0 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
```

