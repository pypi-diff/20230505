# Comparing `tmp/oca_port-0.13.tar.gz` & `tmp/oca_port-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oca_port-0.13.tar", last modified: Fri May  5 12:50:30 2023, max compression
+gzip compressed data, was "oca_port-0.9.tar", last modified: Sun Sep 18 10:11:31 2022, max compression
```

## Comparing `oca_port-0.13.tar` & `oca_port-0.9.tar`

### file list

```diff
@@ -1,32 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:50:30.146808 oca_port-0.13/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-05 12:50:18.000000 oca_port-0.13/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:50:30.138807 oca_port-0.13/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:50:30.142808 oca_port-0.13/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-05 12:50:18.000000 oca_port-0.13/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-05 12:50:18.000000 oca_port-0.13/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-05 12:50:18.000000 oca_port-0.13/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-05 12:50:18.000000 oca_port-0.13/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-05 12:50:18.000000 oca_port-0.13/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-05 12:50:18.000000 oca_port-0.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-05 12:50:30.146808 oca_port-0.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-05 12:50:18.000000 oca_port-0.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:50:30.142808 oca_port-0.13/oca_port/
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-05-05 12:50:18.000000 oca_port-0.13/oca_port/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-05 12:50:18.000000 oca_port-0.13/oca_port/migrate_addon.py
--rw-r--r--   0 runner    (1001) docker     (123)    26636 2023-05-05 12:50:18.000000 oca_port-0.13/oca_port/port_addon_pr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:50:30.146808 oca_port-0.13/oca_port/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 12:50:18.000000 oca_port-0.13/oca_port/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-05-05 12:50:18.000000 oca_port-0.13/oca_port/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-05-05 12:50:18.000000 oca_port-0.13/oca_port/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-05 12:50:18.000000 oca_port-0.13/oca_port/utils/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-05 12:50:18.000000 oca_port-0.13/oca_port/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-05 12:50:18.000000 oca_port-0.13/oca_port/utils/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:50:30.142808 oca_port-0.13/oca_port.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-05 12:50:30.000000 oca_port-0.13/oca_port.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-05 12:50:30.000000 oca_port-0.13/oca_port.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:50:30.000000 oca_port-0.13/oca_port.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 12:50:30.000000 oca_port-0.13/oca_port.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 12:50:30.000000 oca_port-0.13/oca_port.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 12:50:30.000000 oca_port-0.13/oca_port.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-05 12:50:18.000000 oca_port-0.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:50:30.146808 oca_port-0.13/setup.cfg
+drwxrwxr-x   0 sbi-local  (1000) sbi-local  (1000)        0 2022-09-18 10:11:31.473864 oca_port-0.9/
+drwxrwxr-x   0 sbi-local  (1000) sbi-local  (1000)        0 2022-09-18 10:11:31.465864 oca_port-0.9/.github/
+drwxrwxr-x   0 sbi-local  (1000) sbi-local  (1000)        0 2022-09-18 10:11:31.469864 oca_port-0.9/.github/workflows/
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)      607 2022-09-18 10:09:49.000000 oca_port-0.9/.github/workflows/publish.yml
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)      212 2022-08-31 11:45:14.000000 oca_port-0.9/.gitignore
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)     7652 2022-08-31 11:45:14.000000 oca_port-0.9/LICENSE
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)    11314 2022-09-18 10:11:31.473864 oca_port-0.9/PKG-INFO
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)     1660 2022-08-31 11:45:14.000000 oca_port-0.9/README.md
+drwxrwxr-x   0 sbi-local  (1000) sbi-local  (1000)        0 2022-09-18 10:11:31.469864 oca_port-0.9/oca_port/
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)     7287 2022-08-31 11:45:14.000000 oca_port-0.9/oca_port/__init__.py
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)     7485 2022-08-31 11:45:14.000000 oca_port-0.9/oca_port/migrate_addon.py
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)    11336 2022-08-31 11:45:14.000000 oca_port-0.9/oca_port/misc.py
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)    26227 2022-08-31 11:45:14.000000 oca_port-0.9/oca_port/port_addon_pr.py
+drwxrwxr-x   0 sbi-local  (1000) sbi-local  (1000)        0 2022-09-18 10:11:31.473864 oca_port-0.9/oca_port.egg-info/
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)    11314 2022-09-18 10:11:31.000000 oca_port-0.9/oca_port.egg-info/PKG-INFO
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)      357 2022-09-18 10:11:31.000000 oca_port-0.9/oca_port.egg-info/SOURCES.txt
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)        1 2022-09-18 10:11:31.000000 oca_port-0.9/oca_port.egg-info/dependency_links.txt
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)       43 2022-09-18 10:11:31.000000 oca_port-0.9/oca_port.egg-info/entry_points.txt
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)       25 2022-09-18 10:11:31.000000 oca_port-0.9/oca_port.egg-info/requires.txt
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)       14 2022-09-18 10:11:31.000000 oca_port-0.9/oca_port.egg-info/top_level.txt
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)      995 2022-09-18 10:09:49.000000 oca_port-0.9/pyproject.toml
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)       38 2022-09-18 10:11:31.473864 oca_port-0.9/setup.cfg
```

### Comparing `oca_port-0.13/LICENSE` & `oca_port-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oca_port-0.13/PKG-INFO` & `oca_port-0.9/oca_port.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: oca_port
-Version: 0.13
+Name: oca-port
+Version: 0.9
 Summary: OCA tool to help with modules migration
 Author: Odoo Community Association (OCA)
 Author-email: Sébastien Alix <sebastien.alix@camptocamp.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -177,34 +177,20 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Odoo
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Pre-commit Status](https://github.com/OCA/oca-port/actions/workflows/pre-commit.yml/badge.svg?branch=main)](https://github.com/OCA/oca-port/actions/workflows/pre-commit.yml?query=branch%3Amain)
-
 oca-port
 ========
 
 Tool helping to port an addon or missing commits of an addon from one branch
 to another.
 
-Installing
-----------
-
-    $ pipx install oca-port
-    $ #OR
-    $ git clone git@github.com:oca/oca-port.git
-    $ cd oca-port
-    $ pipx install .
-
-Using
------
-
 If the addon does not exist on the target branch, it will assist the user in
 the migration, following the OCA migration guide.
 
 If the addon already exists on the target branch, it will retrieve missing
 commits to port. If a Pull Request exists for a missing commit, it will be
 ported with all its commits if they were not yet (fully) ported.
 
@@ -234,11 +220,9 @@
 the upstream repository.
 
 If there are several Pull Requests to port, it will ask the user if he wants
 to base the next PR on the previous one, allowing the user to cumulate ported
 PRs in one branch and creating a draft PR against the upstream repository
 with all of them.
 
-More details here : [OCA Days 2022 - Sébastien Alix and Simone Orsi: oca-port:new OCA tool to help with modules migration](https://www.youtube.com/watch?v=idGLkQiJ5N0)
-
 **Output example (with --verbose):**
 ![oca_port_pr_verbose](https://user-images.githubusercontent.com/5315285/129207041-12ac6c4a-ea96-4b8c-bd68-ae661531ad92.png)
```

### Comparing `oca_port-0.13/README.md` & `oca_port-0.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,13 @@
-[![Pre-commit Status](https://github.com/OCA/oca-port/actions/workflows/pre-commit.yml/badge.svg?branch=main)](https://github.com/OCA/oca-port/actions/workflows/pre-commit.yml?query=branch%3Amain)
-
 oca-port
 ========
 
 Tool helping to port an addon or missing commits of an addon from one branch
 to another.
 
-Installing
-----------
-
-    $ pipx install oca-port
-    $ #OR
-    $ git clone git@github.com:oca/oca-port.git
-    $ cd oca-port
-    $ pipx install .
-
-Using
------
-
 If the addon does not exist on the target branch, it will assist the user in
 the migration, following the OCA migration guide.
 
 If the addon already exists on the target branch, it will retrieve missing
 commits to port. If a Pull Request exists for a missing commit, it will be
 ported with all its commits if they were not yet (fully) ported.
 
@@ -51,11 +37,9 @@
 the upstream repository.
 
 If there are several Pull Requests to port, it will ask the user if he wants
 to base the next PR on the previous one, allowing the user to cumulate ported
 PRs in one branch and creating a draft PR against the upstream repository
 with all of them.
 
-More details here : [OCA Days 2022 - Sébastien Alix and Simone Orsi: oca-port:new OCA tool to help with modules migration](https://www.youtube.com/watch?v=idGLkQiJ5N0)
-
 **Output example (with --verbose):**
 ![oca_port_pr_verbose](https://user-images.githubusercontent.com/5315285/129207041-12ac6c4a-ea96-4b8c-bd68-ae661531ad92.png)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `oca_port-0.13/oca_port/__init__.py` & `oca_port-0.9/oca_port/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,79 +39,57 @@
 of them.
 """
 import os
 
 import click
 import git
 
-from . import utils
+from . import misc
+from .misc import bcolors as bc
 from .migrate_addon import MigrateAddon
 from .port_addon_pr import PortAddonPullRequest
-from .utils.misc import bcolors as bc
 
 
 @click.command()
 @click.argument("from_branch", required=True)
 @click.argument("to_branch", required=True)
 @click.argument("addon", required=True)
-@click.option(
-    "--upstream-org",
-    default="OCA",
-    show_default=True,
-    help="Upstream organization name.",
-)
-@click.option(
-    "--upstream",
-    default="origin",
-    show_default=True,
-    required=True,
-    help="Git remote from which source and target branches are fetched by default.",
-)
+@click.option("--upstream-org", default="OCA", show_default=True,
+              help="Upstream organization name.")
+@click.option("--upstream", default="origin", show_default=True, required=True,
+              help="Git remote from which source and target branches are fetched by default.")
 @click.option("--repo-name", help="Repository name, eg. server-tools.")
-@click.option(
-    "--fork", help="Git remote where branches with ported commits are pushed."
-)
+@click.option("--fork",
+              help="Git remote where branches with ported commits are pushed.")
 @click.option("--user-org", show_default="--fork", help="User organization name.")
-@click.option("--verbose", is_flag=True, help="List the commits of Pull Requests.")
-@click.option(
-    "--non-interactive", is_flag=True, help="Disable all interactive prompts."
-)
-@click.option("--no-cache", is_flag=True, help="Disable user's cache.")
-@click.option("--clear-cache", is_flag=True, help="Clear the user's cache.")
+@click.option("--verbose", is_flag=True,
+              help="List the commits of Pull Requests.")
+@click.option("--non-interactive", is_flag=True,
+              help="Disable all interactive prompts.")
 def main(
-    from_branch,
-    to_branch,
-    addon,
-    upstream_org,
-    upstream,
-    repo_name,
-    fork,
-    user_org,
-    verbose,
-    non_interactive,
-    no_cache,
-    clear_cache,
-):
+        from_branch, to_branch, addon, upstream_org, upstream, repo_name,
+        fork, user_org, verbose, non_interactive
+        ):
     """Migrate ADDON from FROM_BRANCH to TO_BRANCH or list Pull Requests to port
-        if ADDON already exists on TO_BRANCH.
+    if ADDON already exists on TO_BRANCH.
 
-        Migration:
+    Migration:
 
-            Assist the user in the migration of the addon, following the OCA guidelines.
+        Assist the user in the migration of the addon, following the OCA guidelines.
 
-        Port of Pull Requests (missing commits):
+    Port of Pull Requests (missing commits):
 
-            The PRs are found from FROM_BRANCH commits that do not exist in TO_BRANCH.
-    The user will be asked if he wants to port them.
+        The PRs are found from FROM_BRANCH commits that do not exist in TO_BRANCH.
+The user will be asked if he wants to port them.
 
-        To start the migration process, the `--fork` option must be provided in
-    order to push the resulting branch on the user's remote.
+    To start the migration process, the `--fork` option must be provided in
+order to push the resulting branch on the user's remote.
     """
     repo = git.Repo()
-    if repo.is_dirty(untracked_files=True):
+    if repo.is_dirty():
         raise click.ClickException("changes not committed detected in this repository.")
     repo_name = repo_name or os.path.basename(os.getcwd())
     if not user_org:
         # Assume that the fork remote has the same name than the user organization
         user_org = fork
     if fork:
         error_msg = _check_remote(repo_name, repo, fork, raise_exc=False)
@@ -119,60 +97,35 @@
             error_msg += (
                 "\n\nYou can change the GitHub organization with the "
                 f"{bc.DIM}--user-org{bc.END} option."
             )
             raise click.ClickException(error_msg)
     try:
         # Parse source and target branches
-        from_branch = utils.git.Branch(repo, from_branch, default_remote=upstream)
-        to_branch = utils.git.Branch(repo, to_branch, default_remote=upstream)
+        from_branch = misc.Branch(repo, from_branch, default_remote=upstream)
+        to_branch = misc.Branch(repo, to_branch, default_remote=upstream)
     except ValueError as exc:
         _check_remote(repo_name, *exc.args)
+    storage = misc.InputStorage(repo.working_dir)
     _fetch_branches(from_branch, to_branch, verbose=verbose)
     _check_branches(from_branch, to_branch)
     _check_addon_exists(addon, from_branch, raise_exc=True)
-    storage = utils.storage.InputStorage(to_branch, addon)
-    cache = utils.cache.UserCacheFactory(
-        upstream_org, repo_name, addon, from_branch, to_branch, no_cache
-    ).build()
     # Check if the addon (folder) exists on the target branch
     #   - if it already exists, check if some PRs could be ported
     if _check_addon_exists(addon, to_branch):
         PortAddonPullRequest(
-            repo,
-            upstream_org,
-            repo_name,
-            from_branch,
-            to_branch,
-            fork,
-            user_org,
-            addon,
-            storage,
-            cache,
-            verbose,
-            non_interactive,
+            repo, upstream_org, repo_name, from_branch, to_branch,
+            fork, user_org, addon, storage, verbose, non_interactive
         ).run()
     #   - if not, migrate it
     else:
         MigrateAddon(
-            repo,
-            upstream_org,
-            repo_name,
-            from_branch,
-            to_branch,
-            fork,
-            user_org,
-            addon,
-            storage,
-            cache,
-            verbose,
-            non_interactive,
+            repo, upstream_org, repo_name, from_branch, to_branch,
+            fork, user_org, addon, storage, verbose, non_interactive
         ).run()
-    if clear_cache:
-        cache.clear()
 
 
 def _check_remote(repo_name, repo, remote, raise_exc=True):
     """Check that `remote` exists in the local repository."""
     if remote not in repo.remotes:
         msg = (
             f"No remote {bc.FAIL}{remote}{bc.END} in the current repository.\n"
@@ -193,24 +146,27 @@
 def _fetch_branches(*branches, verbose=False):
     """Fetch `branches`."""
     for branch in branches:
         if not branch.remote:
             continue
         remote_url = branch.repo.remotes[branch.remote].url
         if verbose:
-            print(f"Fetch {bc.BOLD}{branch.ref()}{bc.END} from {remote_url}")
+            print(
+                f"Fetch {bc.BOLD}{branch.ref()}{bc.END} from {remote_url}"
+            )
         branch.repo.remotes[branch.remote].fetch(branch.name)
 
 
 def _check_branches(from_branch, to_branch):
     """Check that all required branches exist in the current repository."""
     # Check if the source branch exists (required)
     if not from_branch.remote:
         raise click.ClickException(
-            f"No source branch {bc.BOLD}{from_branch.ref()}{bc.END} available."
+            "No source branch "
+            f"{bc.BOLD}{from_branch.ref()}{bc.END} available."
         )
     # Check if the target branch exists (with or w/o remote, allowing to work
     # on a local one)
     if not to_branch.remote and to_branch.name not in to_branch.repo.heads:
         raise click.ClickException(
             f"No target branch {bc.BOLD}{to_branch.name}{bc.END} or "
             f"{bc.BOLD}{to_branch.ref()}{bc.END} available locally."
@@ -226,9 +182,9 @@
             return False
         raise click.ClickException(
             f"{bc.FAIL}{addon}{bc.ENDC} does not exist on {branch.ref()}"
         )
     return True
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     main()
```

### Comparing `oca_port-0.13/oca_port/migrate_addon.py` & `oca_port-0.9/oca_port/migrate_addon.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,153 +1,118 @@
 # Copyright 2022 Camptocamp SA
 # License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl)
 
+import click
 import os
+import subprocess
 import tempfile
 import urllib.parse
 
-import click
-
+from . import misc
+from .misc import bcolors as bc
 from .port_addon_pr import PortAddonPullRequest
-from .utils import git as g
-from .utils.misc import bcolors as bc
 
-MIG_BRANCH_NAME = "{branch}-mig-{addon}"
+MIG_BRANCH_NAME = (
+    "{branch}-mig-{addon}"
+)
 MIG_MERGE_COMMITS_URL = (
     "https://github.com/OCA/maintainer-tools/wiki/Merge-commits-in-pull-requests"
 )
 MIG_TASKS_URL = (
     "https://github.com/OCA/maintainer-tools/wiki/Migration-to-version-{branch}"
     "#tasks-to-do-in-the-migration"
 )
 MIG_NEW_PR_TITLE = "[{to_branch}][MIG] {addon}"
 MIG_NEW_PR_URL = (
     "https://github.com/{upstream_org}/{repo_name}/compare/"
     "{to_branch}...{user_org}:{mig_branch}?expand=1&title={title}"
 )
-MIG_TIPS = "\n".join(
-    [
-        f"\n{bc.BOLD}{bc.OKCYAN}The next steps are:{bc.END}",
-        ("\t1) Reduce the number of commits " f"('{bc.DIM}OCA Transbot...{bc.END}'):"),
-        f"\t\t=> {bc.BOLD}{MIG_MERGE_COMMITS_URL}{bc.END}",
-        "\t2) Adapt the module to the {to_branch} version:",
-        f"\t\t=> {bc.BOLD}" "{mig_tasks_url}" f"{bc.END}",
-        (
-            "\t3) On a shell command, type this for uploading the content to GitHub:\n"
-            f"{bc.DIM}"
-            "\t\t$ git add --all\n"
-            '\t\t$ git commit -m "[MIG] {addon}: Migration to {to_branch}"\n'
-            "\t\t$ git push {fork} {mig_branch} --set-upstream"
-            f"{bc.END}"
-        ),
-        "\t4) Create the PR against {upstream_org}/{repo_name}:",
-        f"\t\t=> {bc.BOLD}" "{new_pr_url}" f"{bc.END}",
-    ]
-)
-BLACKLIST_TIPS = "\n".join(
-    [
-        f"\n{bc.BOLD}{bc.OKCYAN}The next steps are:{bc.END}",
-        (
-            "\t1) On a shell command, type this for uploading the content to GitHub:\n"
-            f"{bc.DIM}"
-            "\t\t$ git push {fork} {mig_branch} --set-upstream"
-            f"{bc.END}"
-        ),
-        "\t2) Create the PR against {upstream_org}/{repo_name}:",
-        f"\t\t=> {bc.BOLD}" "{new_pr_url}" f"{bc.END}",
-    ]
-)
+MIG_TIPS = "\n".join([
+    f"\n{bc.BOLD}{bc.OKCYAN}The next steps are:{bc.END}",
+    (
+        "\t1) Reduce the number of commits "
+        f"('{bc.DIM}OCA Transbot...{bc.END}'):"
+    ),
+    f"\t\t=> {bc.BOLD}{MIG_MERGE_COMMITS_URL}{bc.END}",
+    "\t2) Adapt the module to the {to_branch} version:",
+    f"\t\t=> {bc.BOLD}" "{mig_tasks_url}" f"{bc.END}",
+    (
+        "\t3) On a shell command, type this for uploading the content to GitHub:\n"
+        f"{bc.DIM}"
+        "\t\t$ git add --all\n"
+        "\t\t$ git commit -m \"[MIG] {addon}: Migration to {to_branch}\"\n"
+        "\t\t$ git push {fork} {mig_branch} --set-upstream"
+        f"{bc.END}"
+    ),
+    "\t4) Create the PR against {upstream_org}/{repo_name}:",
+    f"\t\t=> {bc.BOLD}" "{new_pr_url}" f"{bc.END}",
+])
 
 
-class MigrateAddon:
+class MigrateAddon():
     def __init__(
-        self,
-        repo,
-        upstream_org,
-        repo_name,
-        from_branch,
-        to_branch,
-        fork,
-        user_org,
-        addon,
-        storage,
-        cache=None,
-        verbose=False,
-        non_interactive=False,
-    ):
+            self, repo, upstream_org, repo_name, from_branch, to_branch,
+            fork, user_org, addon, storage, verbose=False, non_interactive=False
+            ):
         self.repo = repo
         self.upstream_org = upstream_org
         self.repo_name = repo_name
         self.from_branch = from_branch
         self.to_branch = to_branch
         self.fork = fork
         self.user_org = user_org
         self.addon = addon
         self.storage = storage
-        self.cache = cache
-        self.mig_branch = g.Branch(
+        self.mig_branch = misc.Branch(
             repo, MIG_BRANCH_NAME.format(branch=to_branch.name[:4], addon=addon)
         )
         self.verbose = verbose
         self.non_interactive = non_interactive
 
     def run(self):
-        blacklisted = self.storage.is_addon_blacklisted()
-        if blacklisted:
+        if self.storage.is_addon_blacklisted(
+                self.from_branch.name, self.to_branch.name, self.addon
+                ):
             print(
-                f"{bc.DIM}Migration of {bc.BOLD}{self.addon}{bc.END} "
-                f"{bc.DIM}to {self.to_branch.name} "
-                f"blacklisted ({blacklisted}){bc.ENDD}"
-            )
+                f"{bc.DIM}Migration to {self.to_branch.name} for "
+                f"{bc.BOLD}{self.addon}{bc.END} {bc.DIM}blacklisted{bc.ENDD}")
             return
         if self.non_interactive:
             # Exit with an error code if the addon is eligible for a migration
             raise SystemExit(1)
         confirm = (
             f"Migrate {bc.BOLD}{self.addon}{bc.END} "
             f"from {bc.BOLD}{self.from_branch.name}{bc.END} "
             f"to {bc.BOLD}{self.to_branch.name}{bc.END}?"
         )
         if not click.confirm(confirm):
-            self.storage.blacklist_addon(confirm=True)
-            if not self.storage.dirty:
-                return
+            self.storage.blacklist_addon(
+                self.from_branch.name, self.to_branch.name,
+                self.addon, confirm=True
+            )
+            return
         # Check if a migration PR already exists
         # TODO
         if not self.fork:
             raise click.UsageError("Please set the '--fork' option")
         if self.repo.untracked_files:
             raise click.ClickException("Untracked files detected, abort")
         self._checkout_base_branch()
         if self._create_mig_branch():
-            # Case where the addon shouldn't be ported (blacklisted)
-            if self.storage.dirty:
-                self.storage.commit()
-                self._print_tips(blacklisted=True)
-                return
             with tempfile.TemporaryDirectory() as patches_dir:
                 self._generate_patches(patches_dir)
                 self._apply_patches(patches_dir)
-            g.run_pre_commit(self.repo, self.addon)
+            self._run_pre_commit()
         # Check if the addon has commits that update neighboring addons to
         # make it work properly
         PortAddonPullRequest(
-            self.repo,
-            self.upstream_org,
-            self.repo_name,
-            self.from_branch,
-            self.mig_branch,
-            self.fork,
-            self.user_org,
-            self.addon,
-            self.storage,
-            self.cache,
-            self.verbose,
-            create_branch=False,
-            push_branch=False,
+            self.repo, self.upstream_org, self.repo_name,
+            self.from_branch, self.mig_branch, self.fork, self.user_org,
+            self.addon, self.storage, self.verbose,
+            create_branch=False, push_branch=False
         ).run()
         self._print_tips()
 
     def _checkout_base_branch(self):
         # Ensure to not start to work from a working branch
         if self.to_branch.name in self.repo.heads:
             self.repo.heads[self.to_branch.name].checkout()
@@ -177,61 +142,56 @@
                 "--no-track", "-b", self.mig_branch.name, self.to_branch.ref()
             )
         return create_branch
 
     def _generate_patches(self, patches_dir):
         print("\tGenerate patches...")
         self.repo.git.format_patch(
-            "--keep-subject",
-            "-o",
-            patches_dir,
+            "--keep-subject", "-o", patches_dir,
             f"{self.to_branch.ref()}..{self.from_branch.ref()}",
-            "--",
-            self.addon,
+            "--", self.addon
         )
 
     def _apply_patches(self, patches_dir):
         patches = [
             os.path.join(patches_dir, f) for f in sorted(os.listdir(patches_dir))
         ]
         # Apply patches with git-am
         print(f"\tApply {len(patches)} patches...")
         self.repo.git.am("-3", "--keep", *patches)
         print(
             f"\t\tCommits history of {bc.BOLD}{self.addon}{bc.END} "
             f"has been migrated."
         )
 
-    def _print_tips(self, blacklisted=False):
+    def _run_pre_commit(self):
+        # Run pre-commit
+        print(
+            f"\tRun {bc.BOLD}pre-commit{bc.END} and commit changes if any..."
+        )
+        # First ensure that 'pre-commit' is initialized for the repository,
+        # then run it (without checking the return code on purpose)
+        subprocess.check_call("pre-commit install", shell=True)
+        subprocess.run("pre-commit run -a", shell=True)
+        if self.repo.untracked_files or self.repo.is_dirty():
+            self.repo.git.add("-A")
+            self.repo.git.commit(
+                "-m", f"[IMP] {self.addon}: black, isort, prettier", "--no-verify"
+            )
+
+    def _print_tips(self):
         mig_tasks_url = MIG_TASKS_URL.format(branch=self.to_branch.name)
         pr_title_encoded = urllib.parse.quote(
             MIG_NEW_PR_TITLE.format(to_branch=self.to_branch.name[:4], addon=self.addon)
         )
         new_pr_url = MIG_NEW_PR_URL.format(
-            upstream_org=self.upstream_org,
-            repo_name=self.repo_name,
-            to_branch=self.to_branch.name,
-            user_org=self.user_org,
-            mig_branch=self.mig_branch.name,
-            title=pr_title_encoded,
-        )
-        if blacklisted:
-            tips = BLACKLIST_TIPS.format(
-                upstream_org=self.upstream_org,
-                repo_name=self.repo_name,
-                fork=self.fork,
-                mig_branch=self.mig_branch.name,
-                new_pr_url=new_pr_url,
-            )
-            print(tips)
-            return
+            upstream_org=self.upstream_org, repo_name=self.repo_name,
+            to_branch=self.to_branch.name, user_org=self.user_org,
+            mig_branch=self.mig_branch.name, title=pr_title_encoded
+        )
         tips = MIG_TIPS.format(
-            upstream_org=self.upstream_org,
-            repo_name=self.repo_name,
-            addon=self.addon,
-            to_branch=self.to_branch.name,
-            fork=self.fork,
-            mig_branch=self.mig_branch.name,
-            mig_tasks_url=mig_tasks_url,
-            new_pr_url=new_pr_url,
+            upstream_org=self.upstream_org, repo_name=self.repo_name,
+            addon=self.addon, to_branch=self.to_branch.name, fork=self.fork,
+            mig_branch=self.mig_branch.name, mig_tasks_url=mig_tasks_url,
+            new_pr_url=new_pr_url
         )
         print(tips)
```

### Comparing `oca_port-0.13/oca_port/port_addon_pr.py` & `oca_port-0.9/oca_port/port_addon_pr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,111 +1,91 @@
 # Copyright 2022 Camptocamp SA
 # License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl)
 
-import os
+from collections import defaultdict
 import shutil
 import tempfile
-from collections import defaultdict
+import os
 
 import click
 import git
 
-from .utils import git as g, github, misc
-from .utils.misc import bcolors as bc
+from . import misc
+from .misc import bcolors as bc
 
 AUTHOR_EMAILS_TO_SKIP = [
     "transbot@odoo-community.org",
-    "noreply@weblate.org",
     "oca-git-bot@odoo-community.org",
     "oca+oca-travis@odoo-community.org",
     "oca-ci@odoo-community.org",
     "shopinvader-git-bot@shopinvader.com",
 ]
 
 SUMMARY_TERMS_TO_SKIP = [
     "Translated using Weblate",
     "Added translation using Weblate",
 ]
 
-PR_BRANCH_NAME = "oca-port-pr-{pr_number}-from-{from_branch}-to-{to_branch}"
+PR_BRANCH_NAME = (
+    "oca-port-pr-{pr_number}-from-{from_branch}-to-{to_branch}"
+)
 
 FOLDERS_TO_SKIP = [
     "setup",
     ".github",
 ]
 
 FILES_TO_KEEP = [
     "requirements.txt",
     "test-requirements.txt",
     "oca_dependencies.txt",
 ]
 
-# Fake PR for commits w/o any PR (used as fallback)
-FAKE_PR = g.PullRequest(*[""] * 6)
-
 
 def path_to_skip(commit_path):
     """Return True if the commit path should not be ported."""
     # Allows all folders (addons!) excepted those like 'setup/' generated
     # automatically by pre-commit.
     if commit_path.isdir:
         return commit_path in FOLDERS_TO_SKIP
     # Forbid all files excepted those that developers could update
     return commit_path not in FILES_TO_KEEP
 
 
-class PortAddonPullRequest:
+class PortAddonPullRequest():
     def __init__(
-        self,
-        repo,
-        upstream_org,
-        repo_name,
-        from_branch,
-        to_branch,
-        fork,
-        user_org,
-        addon,
-        storage,
-        cache=None,
-        verbose=False,
-        non_interactive=False,
-        create_branch=True,
-        push_branch=True,
-    ):
+            self, repo, upstream_org, repo_name,
+            from_branch, to_branch, fork, user_org, addon, storage,
+            verbose=False, non_interactive=False,
+            create_branch=True, push_branch=True
+            ):
         """Port pull requests of `addon`."""
         self.repo = repo
         self.upstream_org = upstream_org
         self.repo_name = repo_name
         self.from_branch = from_branch
         self.to_branch = to_branch
         self.fork = fork
         self.user_org = user_org
         self.addon = addon
         self.storage = storage
-        self.cache = cache
         self.verbose = verbose
         self.non_interactive = non_interactive
         self.create_branch = create_branch
         self.push_branch = push_branch
 
     def run(self):
         print(
             f"{bc.BOLD}{self.addon}{bc.END} already exists "
             f"on {bc.BOLD}{self.to_branch.name}{bc.END}, "
             "checking PRs to port..."
         )
         branches_diff = BranchesDiff(
-            self.repo,
-            self.upstream_org,
-            self.repo_name,
-            self.addon,
-            self.from_branch,
-            self.to_branch,
-            self.storage,
-            self.cache,
+            self.repo, self.upstream_org, self.repo_name, self.addon,
+            self.from_branch, self.to_branch, self.storage
         )
         branches_diff.print_diff(self.verbose)
         if self.non_interactive:
             if branches_diff.commits_diff:
                 # Exit with an error code if commits are eligible for (back)porting
                 raise SystemExit(1)
             return
@@ -116,42 +96,32 @@
     def _port_pull_requests(self, branches_diff):
         """Open new Pull Requests (if it doesn't exist) on the GitHub repository."""
         base_ref = branches_diff.to_branch  # e.g. 'origin/14.0'
         previous_pr = previous_pr_branch = None
         processed_prs = []
         last_pr = (
             list(branches_diff.commits_diff.keys())[-1]
-            if branches_diff.commits_diff
-            else None
+            if branches_diff.commits_diff else None
         )
         for pr, commits in branches_diff.commits_diff.items():
             current_commit = self.repo.commit(self.to_branch.ref())
             pr_branch, based_on_previous = self._port_pull_request_commits(
-                pr,
-                commits,
-                base_ref,
-                previous_pr,
-                previous_pr_branch,
+                pr, commits, base_ref, previous_pr, previous_pr_branch,
             )
             if pr_branch:
-                # Check if commits have been ported.
-                # If none has been ported, blacklist automatically the current PR.
+                # Check if commits have been ported
                 if self.repo.commit(pr_branch.ref()) == current_commit:
                     print("\tℹ️  Nothing has been ported, skipping")
                     self.storage.blacklist_pr(
-                        pr.number,
-                        confirm=True,
-                        reason=f"(auto) Nothing to port from PR #{pr.number}",
+                        self.from_branch.name, self.to_branch.name,
+                        self.addon, pr.number
                     )
-                    if self.storage.dirty:
-                        self.storage.commit()
                     msg = (
                         f"\t{bc.DIM}PR #{pr.number} has been"
-                        if pr.number
-                        else "Orphaned commits have been"
+                        if pr.number else "Orphaned commits have been"
                     ) + f" automatically blacklisted{bc.ENDD}"
                     print(msg)
                     continue
                 previous_pr = pr
                 previous_pr_branch = pr_branch
                 if based_on_previous:
                     processed_prs.append(pr)
@@ -168,21 +138,16 @@
                 pr_url = self._search_pull_request(pr_data["base"], pr_data["title"])
                 if pr_url:
                     print(f"\tExisting PR has been refreshed => {pr_url}")
                 else:
                     self._create_pull_request(pr_branch, pr_data, processed_prs)
 
     def _port_pull_request_commits(
-        self,
-        pr,
-        commits,
-        base_ref,
-        previous_pr=None,
-        previous_pr_branch=None,
-    ):
+            self, pr, commits, base_ref, previous_pr=None, previous_pr_branch=None,
+            ):
         """Port commits of a Pull Request in a new branch."""
         if pr.number:
             print(
                 f"- {bc.BOLD}{bc.OKCYAN}Port PR #{pr.number}{bc.END} "
                 f"({pr.url}) {bc.OKCYAN}{pr.title}{bc.ENDC}..."
             )
         else:
@@ -191,57 +156,54 @@
         # Ensure to not start to work from a working branch
         if self.to_branch.name in self.repo.heads:
             self.repo.heads[self.to_branch.name].checkout()
         else:
             self.repo.git.checkout(
                 "--no-track", "-b", self.to_branch.name, self.to_branch.ref()
             )
-        # Ask the user if he wants to port the PR (or orphaned commits)
         if not click.confirm("\tPort it?" if pr.number else "\tPort them?"):
-            self.storage.blacklist_pr(pr.number, confirm=True)
-            if not self.storage.dirty:
-                return None, based_on_previous
+            self.storage.blacklist_pr(
+                self.from_branch.name, self.to_branch.name,
+                self.addon, pr.number, confirm=True
+            )
+            return None, based_on_previous
         # Create a local branch based on upstream
         if self.create_branch:
             branch_name = PR_BRANCH_NAME.format(
                 pr_number=pr.number,
                 from_branch=self.from_branch.name,
                 to_branch=self.to_branch.name,
             )
             if branch_name in self.repo.heads:
                 # If the local branch already exists, ask the user if he wants
                 # to recreate it + check if this existing branch is based on
                 # the previous PR branch
                 if previous_pr_branch:
                     based_on_previous = self.repo.is_ancestor(
-                        previous_pr_branch.name, branch_name
+                        previous_pr_branch, branch_name
                     )
                 confirm = (
                     f"\tBranch {bc.BOLD}{branch_name}{bc.END} already exists, "
                     "recreate it?\n\t(⚠️  you will lose the existing branch)"
                 )
                 if not click.confirm(confirm):
-                    return g.Branch(self.repo, branch_name), based_on_previous
+                    return misc.Branch(self.repo, branch_name), based_on_previous
                 self.repo.delete_head(branch_name, "-f")
             if previous_pr and click.confirm(
-                f"\tUse the previous {bc.BOLD}PR #{previous_pr.number}{bc.END} "
-                "branch as base?"
-            ):
+                    f"\tUse the previous {bc.BOLD}PR #{previous_pr.number}{bc.END} "
+                    "branch as base?"
+                    ):
                 base_ref = previous_pr_branch
                 based_on_previous = True
             print(
                 f"\tCreate branch {bc.BOLD}{branch_name}{bc.END} from {base_ref.ref()}..."
             )
             self.repo.git.checkout("--no-track", "-b", branch_name, base_ref.ref())
         else:
             branch_name = self.to_branch.name
-        # If the PR has been blacklisted we need to commit this information
-        if self.storage.dirty:
-            self.storage.commit()
-            return g.Branch(self.repo, branch_name), based_on_previous
 
         # Cherry-pick commits of the source PR
         for commit in commits:
             print(
                 f"\t\tApply {bc.OKCYAN}{commit.hexsha[:8]}{bc.ENDC} "
                 f"{commit.summary}..."
             )
@@ -254,43 +216,40 @@
                         print(f"\t\t\t{message}")
                     if diff.a_path in paths_to_port:
                         paths_to_port.remove(diff.a_path)
                     if diff.b_path in paths_to_port:
                         paths_to_port.remove(diff.b_path)
                     continue
             if not paths_to_port:
-                print("\t\t\tℹ️  Nothing to port from this commit, skipping")
+                print(
+                    "\t\t\tℹ️  Nothing to port from this commit, skipping"
+                )
                 continue
             try:
                 patches_dir = tempfile.mkdtemp()
                 self.repo.git.format_patch(
-                    "--keep-subject",
-                    "-o",
-                    patches_dir,
-                    "-1",
-                    commit.hexsha,
-                    "--",
-                    *paths_to_port,
+                    "--keep-subject", "-o", patches_dir, "-1", commit.hexsha,
+                    "--", *paths_to_port
                 )
                 patches = [
                     os.path.join(patches_dir, f)
                     for f in sorted(os.listdir(patches_dir))
                 ]
                 self.repo.git.am("-3", "--keep", *patches)
                 shutil.rmtree(patches_dir)
             except git.exc.GitCommandError as exc:
                 print(f"{bc.FAIL}ERROR:{bc.ENDC}\n{exc}\n")
                 # High chance a conflict occurs, ask the user to resolve it
                 if not click.confirm(
-                    "⚠️  A conflict occurs, please resolve it and "
-                    "confirm to continue the process (y) or skip this commit (N)."
-                ):
+                        "⚠️  A conflict occurs, please resolve it and "
+                        "confirm to continue the process (y) or skip this commit (N)."
+                        ):
                     self.repo.git.am("--abort")
                     continue
-        return g.Branch(self.repo, branch_name), based_on_previous
+        return misc.Branch(self.repo, branch_name), based_on_previous
 
     @staticmethod
     def _skip_diff(commit, diff):
         """Check if a commit diff should be skipped or not.
 
         A skipped diff won't have its file path ported through 'git format-path'.
 
@@ -301,35 +260,32 @@
                 return True, ""
         if diff.b_path not in commit.paths_to_port:
             return True, ""
         if diff.renamed:
             return False, ""
         diff_path = diff.b_path.split("/", maxsplit=1)[0]
         # Do not accept diff on unported addons
-        if (
-            not misc.get_manifest_path(diff_path)
-            and diff_path not in commit.addons_created
-        ):
+        if not misc.get_manifest_path(diff_path) and diff_path not in commit.addons_created:
             return (
                 True,
                 (
                     f"{bc.WARNING}SKIP diff "
                     f"{bc.BOLD}{diff.change_type} {diff.b_path}{bc.END}: "
                     "relates to an unported addon"
-                ),
+                )
             )
         if diff.change_type in ("M", "D"):
             # Do not accept update and deletion on non-existing files
             if not os.path.exists(diff.b_path):
                 return (
                     True,
                     (
                         f"SKIP: '{diff.change_type} {diff.b_path}' diff relates "
                         "to a non-existing file"
-                    ),
+                    )
                 )
         return False, ""
 
     def _push_branch_to_remote(self, branch):
         """Force push the local branch to remote fork."""
         confirm = (
             f"\tPush branch '{bc.BOLD}{branch.name}{bc.END}' "
@@ -372,74 +328,65 @@
     def _search_pull_request(self, base_branch, title):
         params = {
             "q": (
                 f"is:pr repo:{self.upstream_org}/{self.repo_name} base:{base_branch} "
                 f"state:open {title} in:title"
             ),
         }
-        response = github.request("search/issues", params=params)
+        response = misc._request_github("search/issues", params=params)
         if response["items"]:
             return response["items"][0]["html_url"]
 
     def _create_pull_request(self, pr_branch, pr_data, processed_prs):
         if len(processed_prs) > 1:
             print(
                 "\tPR(s) ported locally:",
                 ", ".join(
                     [f"{bc.OKCYAN}#{pr.number}{bc.ENDC}" for pr in processed_prs]
-                ),
+                )
             )
         if click.confirm(
-            f"\tCreate a draft PR from '{bc.BOLD}{pr_branch.name}{bc.END}' "
-            f"to '{bc.BOLD}{self.to_branch.name}{bc.END}' "
-            f"against {bc.BOLD}{self.upstream_org}/{self.repo_name}{bc.END}?"
-        ):
-            response = github.request(
+                f"\tCreate a draft PR from '{bc.BOLD}{pr_branch.name}{bc.END}' "
+                f"to '{bc.BOLD}{self.to_branch.name}{bc.END}' "
+                f"against {bc.BOLD}{self.upstream_org}/{self.repo_name}{bc.END}?"
+                ):
+            response = misc._request_github(
                 f"repos/{self.upstream_org}/{self.repo_name}/pulls",
                 method="post",
-                json=pr_data,
+                json=pr_data
             )
             pr_url = response["html_url"]
             print(
-                f"\t\t{bc.BOLD}{bc.OKCYAN}PR created =>" f"{bc.ENDC} {pr_url}{bc.END}"
+                f"\t\t{bc.BOLD}{bc.OKCYAN}PR created =>"
+                f"{bc.ENDC} {pr_url}{bc.END}"
             )
             return pr_url
 
 
-class BranchesDiff:
+class BranchesDiff():
     """Helper to compare easily commits (and related PRs) between two branches."""
-
     def __init__(
-        self,
-        repo,
-        upstream_org,
-        repo_name,
-        path,
-        from_branch,
-        to_branch,
-        storage,
-        cache,
-    ):
+            self, repo, upstream_org, repo_name, path, from_branch, to_branch, storage
+            ):
         self.repo = repo
         self.upstream_org = upstream_org
         self.repo_name = repo_name
         self.path = path
         self.from_branch, self.to_branch = from_branch, to_branch
-        self.storage = storage
-        self.cache = cache
         self.from_branch_path_commits, _ = self._get_branch_commits(
             self.from_branch.ref(), path
         )
         self.from_branch_all_commits, _ = self._get_branch_commits(
             self.from_branch.ref()
         )
         self.to_branch_path_commits, _ = self._get_branch_commits(
             self.to_branch.ref(), self.path
         )
         self.to_branch_all_commits, _ = self._get_branch_commits(self.to_branch.ref())
+        self.storage = storage
         self.commits_diff = self.get_commits_diff()
 
     def _get_branch_commits(self, branch, path="."):
         """Get commits from the local repository for the given `branch`.
 
         An optional `path` parameter can be set to limit commits to a given folder.
         This function also filters out undesirable commits (merge or translation
@@ -449,24 +396,19 @@
             - a list of Commit objects `[Commit, ...]`
             - a dict of Commits objects grouped by SHA `{SHA: Commit, ...}`
         """
         commits = self.repo.iter_commits(branch, paths=path)
         commits_list = []
         commits_by_sha = {}
         for commit in commits:
-            if self.cache.is_commit_ported(commit.hexsha):
-                continue
-            com = g.Commit(commit)
+            com = misc.Commit(commit)
             if self._skip_commit(com):
                 continue
             commits_list.append(com)
             commits_by_sha[commit.hexsha] = com
-        # Put ancestors at the beginning of the list to loop with
-        # the expected order
-        commits_list.reverse()
         return commits_list, commits_by_sha
 
     @staticmethod
     def _skip_commit(commit):
         """Check if a commit should be skipped or not.
 
         Merge or translations commits are skipped for instance, or commits
@@ -489,32 +431,44 @@
             if pr.number:
                 lines_to_print.append(
                     f"{i}) {bc.BOLD}{bc.OKBLUE}PR #{pr.number}{bc.END} "
                     f"({pr.url or 'w/o PR'}) {bc.OKBLUE}{pr.title}{bc.ENDC}:"
                 )
                 lines_to_print.append(f"\tBy {pr.author}, merged at {pr.merged_at}")
             else:
-                lines_to_print.append(f"{i}) {bc.BOLD}{bc.OKBLUE}w/o PR{bc.END}:")
+                lines_to_print.append(
+                    f"{i}) {bc.BOLD}{bc.OKBLUE}w/o PR{bc.END}:"
+                )
                 fake_pr = pr
             if verbose:
-                pr_paths = ", ".join([f"{bc.DIM}{path}{bc.ENDD}" for path in pr.paths])
-                lines_to_print.append(f"\t=> Updates: {pr_paths}")
+                pr_paths = ", ".join(
+                    [f"{bc.DIM}{path}{bc.ENDD}" for path in pr.paths]
+                )
+                lines_to_print.append(
+                    f"\t=> Updates: {pr_paths}"
+                )
             if pr.number:
                 pr_paths_not_ported = ", ".join(
-                    [f"{bc.OKBLUE}{path}{bc.ENDC}" for path in pr.paths_not_ported]
+                    [
+                        f"{bc.OKBLUE}{path}{bc.ENDC}"
+                        for path in pr.paths_not_ported
+                    ]
+                )
+                lines_to_print.append(
+                    f"\t=> Not ported: {pr_paths_not_ported}"
                 )
-                lines_to_print.append(f"\t=> Not ported: {pr_paths_not_ported}")
             lines_to_print.append(
                 f"\t=> {bc.BOLD}{bc.OKBLUE}{len(self.commits_diff[pr])} "
                 f"commit(s){bc.END} not (fully) ported"
             )
             if verbose or not pr.number:
                 for commit in self.commits_diff[pr]:
                     lines_to_print.append(
-                        f"\t\t{bc.DIM}{commit.hexsha[:8]} " f"{commit.summary}{bc.ENDD}"
+                        f"\t\t{bc.DIM}{commit.hexsha[:8]} "
+                        f"{commit.summary}{bc.ENDD}"
                     )
         if fake_pr:
             # We have commits without PR, adapt the message
             i -= 1
             nb_commits = len(self.commits_diff[fake_pr])
             message = (
                 f"{bc.BOLD}{bc.OKBLUE}{i} pull request(s){bc.END} "
@@ -537,128 +491,136 @@
         their related Pull Request.
 
         :return: a dict {PullRequest: {Commit: data, ...}, ...}
         """
         commits_by_pr = defaultdict(list)
         for commit in self.from_branch_path_commits:
             if commit in self.to_branch_all_commits:
-                self.cache.mark_commit_as_ported(commit.hexsha)
                 continue
             # Get related Pull Request if any
-            pr = self._get_original_pr(commit)
-            if pr:
-                for pr_commit_sha in pr.commits:
-                    try:
-                        raw_commit = self.repo.commit(pr_commit_sha)
-                    except ValueError:
-                        # Ignore commits referenced by a PR but not present
-                        # in the stable branches
-                        continue
-                    pr_commit = g.Commit(raw_commit)
-                    if self._skip_commit(pr_commit):
-                        continue
-                    pr_commit_paths = {
-                        path for path in pr_commit.paths if not path_to_skip(path)
-                    }
-                    pr.paths.update(pr_commit_paths)
-                    # Check that this PR commit does not change the current
-                    # addon we are interested in, in such case also check
-                    # for each updated addons that the commit has already
-                    # been ported.
-                    # Indeed a commit could have been ported partially
-                    # in the past (with git-format-patch), and we now want
-                    # to port the remaining chunks.
-                    if pr_commit not in self.to_branch_path_commits:
-                        paths = set(pr_commit_paths)
-                        # A commit could have been ported several times
-                        # if it was impacting several addons and the
-                        # migration has been done with git-format-patch
-                        # on each addon separately
-                        to_branch_all_commits = self.to_branch_all_commits[:]
-                        skip_pr_commit = False
-                        with g.no_strict_commit_equality():
-                            while pr_commit in to_branch_all_commits:
-                                index = to_branch_all_commits.index(pr_commit)
-                                ported_commit = to_branch_all_commits.pop(index)
-                                ported_commit_paths = {
-                                    path
-                                    for path in ported_commit.paths
-                                    if not path_to_skip(path)
-                                }
-                                pr.ported_paths.update(ported_commit_paths)
-                                pr_commit.ported_commits.append(ported_commit)
-                                paths -= ported_commit_paths
-                                if not paths:
-                                    # The ported commits have already updated
-                                    # the same addons than the original one,
-                                    # we can skip it.
-                                    skip_pr_commit = True
-                        if skip_pr_commit:
+            if any("github.com" in remote.url for remote in self.repo.remotes):
+                gh_commit_pulls = misc._request_github(
+                    f"repos/{self.upstream_org}/{self.repo_name}"
+                    f"/commits/{commit.hexsha}/pulls"
+                )
+                full_repo_name = f"{self.upstream_org}/{self.repo_name}"
+                gh_commit_pull = [
+                    data for data in gh_commit_pulls
+                    if data["base"]["repo"]["full_name"] == full_repo_name
+                ]
+                # Fake PR for commits w/o related PR
+                pr = misc.PullRequest(*[""] * 6, tuple(), tuple())
+                if gh_commit_pull:
+                    pr = self._new_pull_request_from_github_data(gh_commit_pull[0])
+                    # Get all commits of the related PR as they could update
+                    # others addons than the one the user is interested in
+                    gh_pr_commits = misc._request_github(
+                        f"repos/{self.upstream_org}/{self.repo_name}"
+                        f"/pulls/{pr.number}/commits"
+                    )
+                    for gh_pr_commit in gh_pr_commits:
+                        try:
+                            raw_commit = self.repo.commit(gh_pr_commit["sha"])
+                        except ValueError:
+                            # Ignore commits referenced by a PR but not present
+                            # in the stable branches
                             continue
-                    # We want to port commits that were still not ported
-                    # for the addon we are interested in.
-                    # If the commit has already been included, skip it.
-                    if (
-                        pr_commit in self.to_branch_path_commits
-                        and pr_commit in self.to_branch_all_commits
-                    ):
-                        continue
-                    existing_pr_commits = commits_by_pr.get(pr, [])
-                    for existing_pr_commit in existing_pr_commits:
+                        pr_commit = misc.Commit(raw_commit)
+                        if self._skip_commit(pr_commit):
+                            continue
+                        pr_commit_paths = set(
+                            path for path in pr_commit.paths
+                            if not path_to_skip(path)
+                        )
+                        pr.paths.update(pr_commit_paths)
+                        # Check that this PR commit does not change the current
+                        # addon we are interested in, in such case also check
+                        # for each updated addons that the commit has already
+                        # been ported.
+                        # Indeed a commit could have been ported partially
+                        # in the past (with git-format-patch), and we now want
+                        # to port the remaining chunks.
+                        if pr_commit not in self.to_branch_path_commits:
+                            paths = set(pr_commit_paths)
+                            # A commit could have been ported several times
+                            # if it was impacting several addons and the
+                            # migration has been done with git-format-patch
+                            # on each addon separately
+                            to_branch_all_commits = self.to_branch_all_commits[:]
+                            skip_pr_commit = False
+                            with misc.no_strict_commit_equality():
+                                while pr_commit in to_branch_all_commits:
+                                    index = to_branch_all_commits.index(pr_commit)
+                                    ported_commit = to_branch_all_commits.pop(index)
+                                    ported_commit_paths = set(
+                                        path for path in ported_commit.paths
+                                        if not path_to_skip(path)
+                                    )
+                                    pr.ported_paths.update(ported_commit_paths)
+                                    pr_commit.ported_commits.append(ported_commit)
+                                    paths -= ported_commit_paths
+                                    if not paths:
+                                        # The ported commits have already updated
+                                        # the same addons than the original one,
+                                        # we can skip it.
+                                        skip_pr_commit = True
+                            if skip_pr_commit:
+                                continue
+                        # We want to port commits that were still not ported
+                        # for the addon we are interested in.
+                        # If the commit has already been included, skip it.
                         if (
-                            existing_pr_commit == pr_commit
-                            and existing_pr_commit.hexsha == pr_commit.hexsha
+                                pr_commit in self.to_branch_path_commits
+                                and pr_commit in self.to_branch_all_commits
                         ):
-                            # This PR commit has already been appended, skip
-                            break
-                    else:
-                        commits_by_pr[pr].append(pr_commit)
-            # No related PR: add the commit to the fake PR
+                            continue
+                        existing_pr_commits = commits_by_pr.get(pr, [])
+                        for existing_pr_commit in existing_pr_commits:
+                            if (
+                                existing_pr_commit == pr_commit and
+                                existing_pr_commit.hexsha == pr_commit.hexsha
+                            ):
+                                # This PR commit has already been appended, skip
+                                break
+                        else:
+                            commits_by_pr[pr].append(pr_commit)
+                # No related PR: add the current commit anyway
+                else:
+                    commits_by_pr[pr].append(commit)
             else:
-                commits_by_pr[FAKE_PR].append(commit)
+                # FIXME log?
+                pass
         # Sort PRs on the merge date (better to port them in the right order).
         # Do not return blacklisted PR.
         sorted_commits_by_pr = {}
         for pr in sorted(commits_by_pr, key=lambda pr: pr.merged_at or ""):
-            blacklisted = self.storage.is_pr_blacklisted(pr.number)
-            if blacklisted:
+            if self.storage.is_pr_blacklisted(
+                    self.from_branch.name, self.to_branch.name, self.path, pr.number
+                    ):
                 msg = (
-                    f"{bc.DIM}PR #{pr.number}" if pr.number else "Orphaned commits"
-                ) + f" blacklisted ({blacklisted}){bc.ENDD}"
+                    f"{bc.DIM}PR #{pr.number}"
+                    if pr.number else "Orphaned commits"
+                ) + f" blacklisted{bc.ENDD}"
                 print(msg)
                 continue
             sorted_commits_by_pr[pr] = commits_by_pr[pr]
         return sorted_commits_by_pr
 
-    def _get_original_pr(self, commit: g.Commit):
-        """Return the original PR of a given commit."""
-        # Try to get the data from the user's cache first
-        data = self.cache.get_pr_from_commit(commit.hexsha)
-        if data:
-            return g.PullRequest(**data)
-        # Request GitHub to get them
-        if not any("github.com" in remote.url for remote in self.repo.remotes):
-            return
-        raw_data = github.get_original_pr(
-            self.upstream_org, self.repo_name, self.from_branch.name, commit.hexsha
+    @staticmethod
+    def _new_pull_request_from_github_data(data, paths=None, ported_paths=None):
+        """Create a new PullRequest instance from GitHub data."""
+        pr_number = data["number"]
+        pr_url = data["html_url"]
+        pr_author = data["user"].get("login", "")
+        pr_title = data["title"]
+        pr_body = data["body"]
+        pr_merge_at = data["merged_at"]
+        return misc.PullRequest(
+            number=pr_number,
+            url=pr_url,
+            author=pr_author,
+            title=pr_title,
+            body=pr_body,
+            merged_at=pr_merge_at,
+            paths=paths,
+            ported_paths=ported_paths,
         )
-        if raw_data:
-            # Get all commits of the PR as they could update others addons
-            # than the one the user is interested in.
-            # NOTE: commits fetched from PR are already in the right order
-            pr_number = raw_data["number"]
-            pr_commits_data = github.request(
-                f"repos/{self.upstream_org}/{self.repo_name}"
-                f"/pulls/{pr_number}/commits?per_page=100"
-            )
-            pr_commits = [pr["sha"] for pr in pr_commits_data]
-            data = {
-                "number": raw_data["number"],
-                "url": raw_data["html_url"],
-                "author": raw_data["user"].get("login", ""),
-                "title": raw_data["title"],
-                "body": raw_data["body"],
-                "merged_at": raw_data["merged_at"],
-                "commits": pr_commits,
-            }
-            self.cache.store_commit_pr(commit.hexsha, data)
-            return g.PullRequest(**data)
```

### Comparing `oca_port-0.13/oca_port.egg-info/PKG-INFO` & `oca_port-0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: oca-port
-Version: 0.13
+Name: oca_port
+Version: 0.9
 Summary: OCA tool to help with modules migration
 Author: Odoo Community Association (OCA)
 Author-email: Sébastien Alix <sebastien.alix@camptocamp.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -177,34 +177,20 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Odoo
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Pre-commit Status](https://github.com/OCA/oca-port/actions/workflows/pre-commit.yml/badge.svg?branch=main)](https://github.com/OCA/oca-port/actions/workflows/pre-commit.yml?query=branch%3Amain)
-
 oca-port
 ========
 
 Tool helping to port an addon or missing commits of an addon from one branch
 to another.
 
-Installing
-----------
-
-    $ pipx install oca-port
-    $ #OR
-    $ git clone git@github.com:oca/oca-port.git
-    $ cd oca-port
-    $ pipx install .
-
-Using
------
-
 If the addon does not exist on the target branch, it will assist the user in
 the migration, following the OCA migration guide.
 
 If the addon already exists on the target branch, it will retrieve missing
 commits to port. If a Pull Request exists for a missing commit, it will be
 ported with all its commits if they were not yet (fully) ported.
 
@@ -234,11 +220,9 @@
 the upstream repository.
 
 If there are several Pull Requests to port, it will ask the user if he wants
 to base the next PR on the previous one, allowing the user to cumulate ported
 PRs in one branch and creating a draft PR against the upstream repository
 with all of them.
 
-More details here : [OCA Days 2022 - Sébastien Alix and Simone Orsi: oca-port:new OCA tool to help with modules migration](https://www.youtube.com/watch?v=idGLkQiJ5N0)
-
 **Output example (with --verbose):**
 ![oca_port_pr_verbose](https://user-images.githubusercontent.com/5315285/129207041-12ac6c4a-ea96-4b8c-bd68-ae661531ad92.png)
```

### Comparing `oca_port-0.13/pyproject.toml` & `oca_port-0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,14 @@
 documentation = "https://github.com/OCA/oca-port"
 repository = "https://github.com/OCA/oca-port"
 
 [project.scripts]
 oca-port = "oca_port:main"
 
 [build-system]
-requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2"]
+requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages]
 find = {}
 
 [tool.setuptools_scm]
```

