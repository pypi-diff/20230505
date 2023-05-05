# Comparing `tmp/gpt-review-0.6.0rc462.post1.tar.gz` & `tmp/gpt-review-0.7.0rc475.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.6.0rc462.post1.tar", last modified: Fri May  5 18:16:59 2023, max compression
+gzip compressed data, was "gpt-review-0.7.0rc475.post1.tar", last modified: Fri May  5 19:29:29 2023, max compression
```

## Comparing `gpt-review-0.6.0rc462.post1.tar` & `gpt-review-0.7.0rc475.post1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      336 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     2229 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4172 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1761 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.pypirc
--rw-r--r--   0        0        0     1125 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/LICENSE
--rw-r--r--   0        0        0     3251 2023-05-05 18:16:53.720584 gpt-review-0.6.0rc462.post1/README.md
--rw-r--r--   0        0        0     3571 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/action.yml
--rw-r--r--   0        0        0      218 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/config.summary.template.yml
--rw-r--r--   0        0        0     8346 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-05 18:16:59.612726 gpt-review-0.6.0rc462.post1/src/gpt/__init__.py
--rw-r--r--   0        0        0      171 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt/__main__.py
--rw-r--r--   0        0        0      366 2023-05-05 18:16:59.612726 gpt-review-0.6.0rc462.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      171 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/__main__.py
--rw-r--r--   0        0        0    10048 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1924 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5738 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1441 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     3221 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0      788 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     8870 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      464 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      568 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0      218 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/config.summary.test.yml
--rw-r--r--   0        0        0     3124 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/mock.diff
--rw-r--r--   0        0        0      462 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/test_git.py
--rw-r--r--   0        0        0     1363 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/test_github.py
--rw-r--r--   0        0        0     6707 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      590 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0     1015 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/test_report.py
--rw-r--r--   0        0        0      420 2023-05-05 18:16:53.724584 gpt-review-0.6.0rc462.post1/tests/test_review.py
--rw-r--r--   0        0        0     5425 1970-01-01 00:00:00.000000 gpt-review-0.6.0rc462.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     2229 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4172 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1761 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/LICENSE
+-rw-r--r--   0        0        0     3251 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/README.md
+-rw-r--r--   0        0        0     3561 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/action.yml
+-rw-r--r--   0        0        0      218 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/config.summary.template.yml
+-rw-r--r--   0        0        0     8346 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-05-05 19:29:29.452516 gpt-review-0.7.0rc475.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-05-05 19:29:29.452516 gpt-review-0.7.0rc475.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0    10048 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1924 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5738 2023-05-05 19:29:23.688429 gpt-review-0.7.0rc475.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1441 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     3221 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0      788 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     9707 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      464 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      568 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0      218 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     3124 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/tests/mock.diff
+-rw-r--r--   0        0        0      462 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1363 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/tests/test_github.py
+-rw-r--r--   0        0        0     6707 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      590 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1015 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/tests/test_report.py
+-rw-r--r--   0        0        0      420 2023-05-05 19:29:23.692429 gpt-review-0.7.0rc475.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5425 1970-01-01 00:00:00.000000 gpt-review-0.7.0rc475.post1/PKG-INFO
```

### Comparing `gpt-review-0.6.0rc462.post1/.devcontainer/devcontainer.json` & `gpt-review-0.7.0rc475.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.7.0rc475.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/.github/dependabot.yml` & `gpt-review-0.7.0rc475.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/.github/pull_request_template.md` & `gpt-review-0.7.0rc475.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/.github/workflows/codeql.yml` & `gpt-review-0.7.0rc475.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.7.0rc475.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.7.0rc475.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/.github/workflows/python.yml` & `gpt-review-0.7.0rc475.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/.github/workflows/test-action.yml` & `gpt-review-0.7.0rc475.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/.gitignore` & `gpt-review-0.7.0rc475.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/.vscode/settings.json` & `gpt-review-0.7.0rc475.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/LICENSE` & `gpt-review-0.7.0rc475.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/README.md` & `gpt-review-0.7.0rc475.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/action.yml` & `gpt-review-0.7.0rc475.post1/action.yml`

 * *Files 0% similar despite different names*

```diff
@@ -107,8 +107,8 @@
           PATCH_REPO: ${{ github.repository }}
           FULL_SUMMARY: ${{ inputs.FULL_SUMMARY }}
           FILE_SUMMARY: ${{ inputs.FILE_SUMMARY }}
           TEST_SUMMARY: ${{ inputs.TEST_SUMMARY }}
           BUG_SUMMARY: ${{ inputs.BUG_SUMMARY }}
           RISK_SUMMARY: ${{ inputs.RISK_SUMMARY }}
           RISK_BREAKING: ${{ inputs.RISK_BREAKING }}
-          
+
```

### Comparing `gpt-review-0.6.0rc462.post1/pyproject.toml` & `gpt-review-0.7.0rc475.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/src/gpt_review/_ask.py` & `gpt-review-0.7.0rc475.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/src/gpt_review/_git.py` & `gpt-review-0.7.0rc475.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/src/gpt_review/_github.py` & `gpt-review-0.7.0rc475.post1/src/gpt_review/_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.7.0rc475.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/src/gpt_review/_llama_index.py` & `gpt-review-0.7.0rc475.post1/src/gpt_review/_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/src/gpt_review/_repository.py` & `gpt-review-0.7.0rc475.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/src/gpt_review/_review.py` & `gpt-review-0.7.0rc475.post1/src/gpt_review/_review.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 """Basic functions for requesting review based goals from GPT-4."""
 import logging
 import os
-import yaml
 from typing import Dict
 
+import yaml
+
 from knack.arguments import ArgumentsContext
 from knack import CLICommandsLoader
 from knack.commands import CommandGroup
 
 from gpt_review._ask import _ask
 from gpt_review._command import GPTCommandGroup
 
+SUMMARIZE_PROMPT = """Summarize the following file changed in a pull request submitted by a developer on GitHub,
+focusing on major modifications, additions, deletions, and any significant updates within the files. Do not include the
+file name in the summary and list the summary with bullet points"""
+TEST_COVERAGE_PROMPT = """You are an experienced software developer. Generate unit test cases for the code submitted in
+the pull request, ensuring comprehensive coverage of all functions, methods, and scenarios to validate the correctness
+and reliability of the implementation."""
+BUGS_PROMPT = """Provide a concise summary of the bug found in the code, describing its characteristics, location, and
+potential effects on the overall functionality and performance of the application. Present the potential issues and
+errors first, following by the most important findings, in your summary"""
+
 _CHECKS = {
     "SUMMARY_CHECKS": [
         {
             "flag": "SUMMARY_SUGGEST",
             "header": "Suggestions",
             "goal": "Any suggestions for improving the changes in this PR?",
         },
@@ -41,34 +52,35 @@
             file_name (str): The name of the file.
             diff (str): The diff contents of the file.
         """
         self.file_name = file_name
         self.diff = diff
 
 
-def _request_goal(git_diff, goal, fast: bool = False, large: bool = False) -> str:
+def _request_goal(git_diff, goal, fast: bool = False, large: bool = False, temperature: float = 0) -> str:
     """
     Request a goal from GPT-4.
 
     Args:
         git_diff (str): The git diff to split.
         goal (str): The goal to request from GPT-4.
         fast (bool, optional): Whether to use the fast model. Defaults to False.
         large (bool, optional): Whether to use the large model. Defaults to False.
+        temperature (float, optional): The temperature to use. Defaults to 0.
 
     Returns:
         response (str): The response from GPT-4.
     """
     prompt = f"""
 {goal}
 
 {git_diff}
 """
 
-    response = _ask([prompt], max_tokens=1500, fast=fast, large=large)
+    response = _ask([prompt], max_tokens=1500, fast=fast, large=large, temperature=temperature)
     logging.info(response["response"])
     return response["response"]
 
 
 def _check_goals(git_diff, checks, indent="###") -> str:
     """
     Check goals.
@@ -118,17 +130,15 @@
         diff (str): The file to summarize.
 
     Returns:
         str: The summary of the file.
     """
     git_file = GitFile(diff.split(" b/")[0], diff)
     prompt = f"""
-Summarize the changes to the file {git_file.file_name}.
-- Do not include the file name in the summary.
-- list the summary with bullet points
+{SUMMARIZE_PROMPT}
 {diff}
 """
     response = _ask([prompt], temperature=0.0)
     return f"""
 ### {git_file.file_name}
 {response}
 """
@@ -164,15 +174,15 @@
 
         files[git_file.file_name] = git_file
 
     prompt = f"""
 ```
 {git_diff}
 ```
-Discuss if tests been included to cover the latest changes?
+{TEST_COVERAGE_PROMPT}
 """
 
     return _ask([prompt], temperature=0.0, max_tokens=1500)["response"]
 
 
 def _summarize_bugs_in_pr(git_diff) -> str:
     """
@@ -181,15 +191,15 @@
     Args:
         git_diff (str): The git diff to split.
 
     Returns:
         response (str): The response from GPT-4.
     """
     gpt4_big_prompot = f"""
-Summarize bugs that may be introduced.
+{BUGS_PROMPT}
 
 {git_diff}
 """
     response = _ask([gpt4_big_prompot])
     logging.info(response["response"])
     return response["response"]
```

### Comparing `gpt-review-0.6.0rc462.post1/src/gpt_review/main.py` & `gpt-review-0.7.0rc475.post1/src/gpt_review/main.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/tests/conftest.py` & `gpt-review-0.7.0rc475.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/tests/mock.diff` & `gpt-review-0.7.0rc475.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/tests/test_github.py` & `gpt-review-0.7.0rc475.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/tests/test_gpt_cli.py` & `gpt-review-0.7.0rc475.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/tests/test_llama_index.py` & `gpt-review-0.7.0rc475.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/tests/test_report.py` & `gpt-review-0.7.0rc475.post1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.6.0rc462.post1/PKG-INFO` & `gpt-review-0.7.0rc475.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.6.0rc462.post1
+Version: 0.7.0rc475.post1
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
-Metadata-Version: 2.1 Name: gpt-review Version: 0.6.0rc462.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.7.0rc475.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

