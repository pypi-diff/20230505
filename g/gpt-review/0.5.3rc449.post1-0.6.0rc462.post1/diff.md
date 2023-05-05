# Comparing `tmp/gpt-review-0.5.3rc449.post1.tar.gz` & `tmp/gpt-review-0.6.0rc462.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.5.3rc449.post1.tar", last modified: Fri May  5 15:55:20 2023, max compression
+gzip compressed data, was "gpt-review-0.6.0rc462.post1.tar", last modified: Fri May  5 18:16:59 2023, max compression
```

## Comparing `gpt-review-0.5.3rc449.post1.tar` & `gpt-review-0.6.0rc462.post1.tar`

### file list

```diff
@@ -1,40 +1,43 @@
--rw-r--r--   0        0        0      336 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     2229 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4172 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1952 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/.pypirc
--rw-r--r--   0        0        0     1125 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/LICENSE
--rw-r--r--   0        0        0     3251 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/README.md
--rw-r--r--   0        0        0     4920 2023-05-05 15:55:14.633004 gpt-review-0.5.3rc449.post1/action.yml
--rw-r--r--   0        0        0     8346 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-05 15:55:20.536979 gpt-review-0.5.3rc449.post1/src/gpt/__init__.py
--rw-r--r--   0        0        0      171 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/src/gpt/__main__.py
--rw-r--r--   0        0        0      366 2023-05-05 15:55:20.540979 gpt-review-0.5.3rc449.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      171 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/src/gpt_review/__main__.py
--rw-r--r--   0        0        0    10048 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1924 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5738 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1402 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     3221 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0      788 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     6730 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      464 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      488 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0     2566 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/tests/mock.diff
--rw-r--r--   0        0        0      462 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/tests/test_git.py
--rw-r--r--   0        0        0     1363 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/tests/test_github.py
--rw-r--r--   0        0        0     6511 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      590 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0      420 2023-05-05 15:55:14.637004 gpt-review-0.5.3rc449.post1/tests/test_review.py
--rw-r--r--   0        0        0     5425 1970-01-01 00:00:00.000000 gpt-review-0.5.3rc449.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     2229 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4172 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1761 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/LICENSE
+-rw-r--r--   0        0        0     3251 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/README.md
+-rw-r--r--   0        0        0     3571 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/action.yml
+-rw-r--r--   0        0        0      218 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/config.summary.template.yml
+-rw-r--r--   0        0        0     8346 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-05-05 18:16:59.612726 gpt-review-0.6.0rc462.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-05-05 18:16:59.612726 gpt-review-0.6.0rc462.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0    10048 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1924 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5738 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1441 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     3221 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0      788 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     8870 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      464 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      568 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0      218 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     3124 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/mock.diff
+-rw-r--r--   0        0        0      462 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1363 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/test_github.py
+-rw-r--r--   0        0        0     6707 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      590 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1015 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/test_report.py
+-rw-r--r--   0        0        0      420 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5425 1970-01-01 00:00:00.000000 gpt-review-0.6.0rc462.post1/PKG-INFO
```

### Comparing `gpt-review-0.5.3rc449.post1/.devcontainer/devcontainer.json` & `gpt-review-0.6.0rc462.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.6.0rc462.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/.github/dependabot.yml` & `gpt-review-0.6.0rc462.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/.github/pull_request_template.md` & `gpt-review-0.6.0rc462.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/.github/workflows/codeql.yml` & `gpt-review-0.6.0rc462.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.6.0rc462.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.6.0rc462.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/.github/workflows/python.yml` & `gpt-review-0.6.0rc462.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/.github/workflows/test-action.yml` & `gpt-review-0.6.0rc462.post1/.github/workflows/test-action.yml`

 * *Files 12% similar despite different names*

```diff
@@ -47,14 +47,8 @@
           AZURE_OPENAI_API: ${{ secrets.AZURE_OPENAI_API }}
           AZURE_OPENAI_API_KEY: ${{ secrets.AZURE_OPENAI_API_KEY }}
           LINK: "https://github.com/${{ github.repository }}/pull/${{ github.event.pull_request.number }}"
           FILE_SUMMARY: false
           TEST_SUMMARY: false
           BUG_SUMMARY: false
           RISK_SUMMARY: false
-          RISK_ROLLBACK: false
           RSIK_BREAKING: false
-          RISK_FLAGGED: false
-          SUMMARY_CONFIG: false
-          SUMMARY_SCHEMA: false
-          SUMMARY_FLAGS: false
-          SUMMARY_INCIDENTS: false
```

### Comparing `gpt-review-0.5.3rc449.post1/.gitignore` & `gpt-review-0.6.0rc462.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/.vscode/settings.json` & `gpt-review-0.6.0rc462.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/LICENSE` & `gpt-review-0.6.0rc462.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/README.md` & `gpt-review-0.6.0rc462.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/pyproject.toml` & `gpt-review-0.6.0rc462.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/src/gpt_review/_ask.py` & `gpt-review-0.6.0rc462.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/src/gpt_review/_git.py` & `gpt-review-0.6.0rc462.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/src/gpt_review/_github.py` & `gpt-review-0.6.0rc462.post1/src/gpt_review/_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.6.0rc462.post1/src/gpt_review/_gpt_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,33 +5,30 @@
 
 from knack import CLI, CLICommandsLoader
 
 from gpt_review import __version__
 from gpt_review._ask import AskCommandGroup
 from gpt_review._git import GitCommandGroup
 from gpt_review._github import GitHubCommandGroup
+from gpt_review._review import ReviewCommandGroup
 
 CLI_NAME = "gpt"
 
 
 class GPTCLI(CLI):
     """Custom CLI implemntation to set version for the GPT CLI."""
 
     def get_cli_version(self) -> str:
         return __version__
 
 
 class GPTCommandsLoader(CLICommandsLoader):
     """The GPT CLI Commands Loader."""
 
-    _CommandGroups = [
-        AskCommandGroup,
-        GitHubCommandGroup,
-        GitCommandGroup,
-    ]
+    _CommandGroups = [AskCommandGroup, GitHubCommandGroup, GitCommandGroup, ReviewCommandGroup]
 
     def load_command_table(self, args) -> OrderedDict:
         for command_group in self._CommandGroups:
             command_group.load_command_table(self)
         return OrderedDict(self.command_table)
 
     def load_arguments(self, command) -> None:
```

### Comparing `gpt-review-0.5.3rc449.post1/src/gpt_review/_llama_index.py` & `gpt-review-0.6.0rc462.post1/src/gpt_review/_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/src/gpt_review/_repository.py` & `gpt-review-0.6.0rc462.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/tests/conftest.py` & `gpt-review-0.6.0rc462.post1/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+import yaml
 from collections import namedtuple
 
 
 @pytest.fixture
 def mock_openai(monkeypatch) -> None:
     """
     Mock OpenAI Functions with monkeypatch
@@ -88,7 +89,32 @@
         def diff(self, message, cached) -> str:
             return "test diff response"
 
     def mock_init(cls):
         return MockGit()
 
     monkeypatch.setattr("git.repo.Repo.init", mock_init)
+
+
+@pytest.fixture
+def report_config():
+    """Load sample.report.yaml file"""
+    return load_report_config("config.summary.template.yml")
+
+
+def load_report_config(file_name):
+    with open(file_name, "r") as yaml_file:
+        config = yaml.safe_load(yaml_file)
+        return config["report"]
+
+
+@pytest.fixture
+def config_yaml():
+    return "tests/config.summary.test.yml"
+
+
+@pytest.fixture
+def git_diff() -> str:
+    """Load test.diff file"""
+    with open("tests/mock.diff", "r") as diff_file:
+        diff = diff_file.read()
+    return diff
```

### Comparing `gpt-review-0.5.3rc449.post1/tests/mock.diff` & `gpt-review-0.6.0rc462.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/tests/test_github.py` & `gpt-review-0.6.0rc462.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/tests/test_gpt_cli.py` & `gpt-review-0.6.0rc462.post1/tests/test_gpt_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,15 +111,21 @@
     CLICase("github review"),
     CLICase(
         "ask --files src/gpt_review/__init__.py --files src/gpt_review/__init__.py what programming language is this code written in?"
     ),
     CLICase("ask --fast -f src/gpt_review/__init__.py what programming language is this code written in?"),
 ]
 
-ARGS = ROOT_COMMANDS + ASK_COMMANDS
+REVIEW_COMMANDS = [
+    CLICase("review --help"),
+    CLICase("review diff --help"),
+    CLICase("review diff --diff tests/mock.diff --config tests/config.summary.test.yml"),
+]
+
+ARGS = ROOT_COMMANDS + ASK_COMMANDS + REVIEW_COMMANDS
 
 
 def gpt_cli_test(command: CLICase) -> None:
     os.environ["GPT_ASK_COMMANDS"] = "1"
 
     sys.argv[1:] = command.command.split(" ")
```

### Comparing `gpt-review-0.5.3rc449.post1/tests/test_llama_index.py` & `gpt-review-0.6.0rc462.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.3rc449.post1/PKG-INFO` & `gpt-review-0.6.0rc462.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.5.3rc449.post1
+Version: 0.6.0rc462.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.5.3rc449.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.6.0rc462.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

