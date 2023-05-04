# Comparing `tmp/gpt-review-0.5.0rc406.post1.tar.gz` & `tmp/gpt-review-0.5.0rc407.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.5.0rc406.post1.tar", last modified: Thu May  4 23:00:51 2023, max compression
+gzip compressed data, was "gpt-review-0.5.0rc407.post1.tar", last modified: Thu May  4 23:00:55 2023, max compression
```

## Comparing `gpt-review-0.5.0rc406.post1.tar` & `gpt-review-0.5.0rc407.post1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      336 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     2229 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4923 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1795 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/.pypirc
--rw-r--r--   0        0        0     1125 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/LICENSE
--rw-r--r--   0        0        0     3247 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/README.md
--rw-r--r--   0        0        0     4920 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/action.yml
--rw-r--r--   0        0        0     8252 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/pyproject.toml
--rw-r--r--   0        0        0      366 2023-05-04 23:00:51.135035 gpt-review-0.5.0rc406.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0    10048 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1924 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5738 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1402 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     3221 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0      788 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     6730 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      464 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      488 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0     2566 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/tests/mock.diff
--rw-r--r--   0        0        0      462 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/tests/test_git.py
--rw-r--r--   0        0        0     1363 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/tests/test_github.py
--rw-r--r--   0        0        0     5987 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      590 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0      420 2023-05-04 23:00:36.738731 gpt-review-0.5.0rc406.post1/tests/test_review.py
--rw-r--r--   0        0        0     5306 1970-01-01 00:00:00.000000 gpt-review-0.5.0rc406.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     2229 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4923 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1795 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/LICENSE
+-rw-r--r--   0        0        0     3251 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/README.md
+-rw-r--r--   0        0        0     4920 2023-05-04 23:00:43.677124 gpt-review-0.5.0rc407.post1/action.yml
+-rw-r--r--   0        0        0     8252 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/pyproject.toml
+-rw-r--r--   0        0        0      366 2023-05-04 23:00:54.837303 gpt-review-0.5.0rc407.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0    10048 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1924 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5738 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1402 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     3221 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0      788 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     6730 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      464 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      488 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0     2566 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/tests/mock.diff
+-rw-r--r--   0        0        0      462 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1363 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/tests/test_github.py
+-rw-r--r--   0        0        0     5987 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      590 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0      420 2023-05-04 23:00:43.681124 gpt-review-0.5.0rc407.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5310 1970-01-01 00:00:00.000000 gpt-review-0.5.0rc407.post1/PKG-INFO
```

### Comparing `gpt-review-0.5.0rc406.post1/.devcontainer/devcontainer.json` & `gpt-review-0.5.0rc407.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.5.0rc407.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/.github/dependabot.yml` & `gpt-review-0.5.0rc407.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/.github/pull_request_template.md` & `gpt-review-0.5.0rc407.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/.github/workflows/codeql.yml` & `gpt-review-0.5.0rc407.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.5.0rc407.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.5.0rc407.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/.github/workflows/python.yml` & `gpt-review-0.5.0rc407.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/.github/workflows/test-action.yml` & `gpt-review-0.5.0rc407.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/.gitignore` & `gpt-review-0.5.0rc407.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/.vscode/settings.json` & `gpt-review-0.5.0rc407.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/LICENSE` & `gpt-review-0.5.0rc407.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/README.md` & `gpt-review-0.5.0rc407.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 pip install gpt-review
 
 export AZURE_OPENAI_API=<your azure api url>
 export AZURE_OPENAI_API_KEY=<your azure key>
 ```
 
 Or use Azure Key Vault to secure your API Key. Create secrets for the url named `azure-open-ai`, and for the API Key named `azure-openai-key`.
-```
+```bash
 export AZURE_KEY_VAULT_URL=https://<keyvault_name>.vault.azure.net/
 
 az login
 ```
 
 ## Main Commands
```

#### html2text {}

```diff
@@ -5,29 +5,29 @@
 review contents of pull requests. ## How to install CLI: Install the package
 via `pip` and set the environment variables for your OpenAI API Key and
 Organization ID. To use Azure OpenAI, set the environment variable
 `AZURE_OPENAI_API_URL` and `AZURE_OPENAI_API_URL_KEY` to the URL and key for
 your Azure OpenAI API. ```bash pip install gpt-review export AZURE_OPENAI_API=
 export AZURE_OPENAI_API_KEY= ``` Or use Azure Key Vault to secure your API Key.
 Create secrets for the url named `azure-open-ai`, and for the API Key named
-`azure-openai-key`. ``` export AZURE_KEY_VAULT_URL=https://.vault.azure.net/ az
-login ``` ## Main Commands To show help information about available commands
-and their usage, run: ```bash gpt --help ``` To display the current version of
-this CLI tool, run: ```bash gpt --version ``` Here are the main commands for
-using this CLI tool: ### 1. Ask a Question To submit a question to GPT and
-receive an answer, use the following format: ```bash gpt ask "What is the
-capital of France?" ``` You can customize your request using various options
-like maximum tokens (`--max-tokens`), temperature (`--temperature`), top-
-p value (`--top-p`), frequency penalty (`--frequency-penalty`), presence
-penalty (`--presence-penalty`), etc. #### Ask a Question about a File To submit
-a question to GPT with a file and receive an answer, use the following format:
-```bash gpt ask --files WordDocument.docx "Summarize the contents of this
-document." ``` ### 2. Review a PR To review a PR, use the following format:
-```bash gpt github review \ --access-token $GITHUB_ACCESS_TOKEN \ --pull-
-request $PULL_REQUEST_NUMBER \ --repository $REPOSITORY_NAME ``` ### 3.
-Generate a git commit message with GPT To generate a git commit message with
-GPT after having added the files, use the following format: ```bash git add .
-gpt git commit ``` For more detailed information on each command and its
-options, run: ```bash gpt COMMAND --help ``` Replace COMMAND with one of the
-main commands listed above (e.g., 'ask'). ## Developer Setup To install the
-package in development mode, with additional packages for testing, run the
-following command: ```bash pip install -e .[test] ```
+`azure-openai-key`. ```bash export AZURE_KEY_VAULT_URL=https:/
+/.vault.azure.net/ az login ``` ## Main Commands To show help information about
+available commands and their usage, run: ```bash gpt --help ``` To display the
+current version of this CLI tool, run: ```bash gpt --version ``` Here are the
+main commands for using this CLI tool: ### 1. Ask a Question To submit a
+question to GPT and receive an answer, use the following format: ```bash gpt
+ask "What is the capital of France?" ``` You can customize your request using
+various options like maximum tokens (`--max-tokens`), temperature (`--
+temperature`), top-p value (`--top-p`), frequency penalty (`--frequency-
+penalty`), presence penalty (`--presence-penalty`), etc. #### Ask a Question
+about a File To submit a question to GPT with a file and receive an answer, use
+the following format: ```bash gpt ask --files WordDocument.docx "Summarize the
+contents of this document." ``` ### 2. Review a PR To review a PR, use the
+following format: ```bash gpt github review \ --access-token
+$GITHUB_ACCESS_TOKEN \ --pull-request $PULL_REQUEST_NUMBER \ --repository
+$REPOSITORY_NAME ``` ### 3. Generate a git commit message with GPT To generate
+a git commit message with GPT after having added the files, use the following
+format: ```bash git add . gpt git commit ``` For more detailed information on
+each command and its options, run: ```bash gpt COMMAND --help ``` Replace
+COMMAND with one of the main commands listed above (e.g., 'ask'). ## Developer
+Setup To install the package in development mode, with additional packages for
+testing, run the following command: ```bash pip install -e .[test] ```
```

### Comparing `gpt-review-0.5.0rc406.post1/action.yml` & `gpt-review-0.5.0rc407.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/pyproject.toml` & `gpt-review-0.5.0rc407.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/src/gpt_review/_ask.py` & `gpt-review-0.5.0rc407.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/src/gpt_review/_git.py` & `gpt-review-0.5.0rc407.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/src/gpt_review/_github.py` & `gpt-review-0.5.0rc407.post1/src/gpt_review/_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.5.0rc407.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/src/gpt_review/_llama_index.py` & `gpt-review-0.5.0rc407.post1/src/gpt_review/_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/src/gpt_review/_repository.py` & `gpt-review-0.5.0rc407.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/src/gpt_review/_review.py` & `gpt-review-0.5.0rc407.post1/src/gpt_review/_review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/tests/conftest.py` & `gpt-review-0.5.0rc407.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/tests/mock.diff` & `gpt-review-0.5.0rc407.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/tests/test_github.py` & `gpt-review-0.5.0rc407.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/tests/test_gpt_cli.py` & `gpt-review-0.5.0rc407.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/tests/test_llama_index.py` & `gpt-review-0.5.0rc407.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.5.0rc406.post1/PKG-INFO` & `gpt-review-0.5.0rc407.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.5.0rc406.post1
+Version: 0.5.0rc407.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -67,15 +67,15 @@
 pip install gpt-review
 
 export AZURE_OPENAI_API=<your azure api url>
 export AZURE_OPENAI_API_KEY=<your azure key>
 ```
 
 Or use Azure Key Vault to secure your API Key. Create secrets for the url named `azure-open-ai`, and for the API Key named `azure-openai-key`.
-```
+```bash
 export AZURE_KEY_VAULT_URL=https://<keyvault_name>.vault.azure.net/
 
 az login
 ```
 
 ## Main Commands
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.5.0rc406.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.5.0rc407.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -32,29 +32,29 @@
 review contents of pull requests. ## How to install CLI: Install the package
 via `pip` and set the environment variables for your OpenAI API Key and
 Organization ID. To use Azure OpenAI, set the environment variable
 `AZURE_OPENAI_API_URL` and `AZURE_OPENAI_API_URL_KEY` to the URL and key for
 your Azure OpenAI API. ```bash pip install gpt-review export AZURE_OPENAI_API=
 export AZURE_OPENAI_API_KEY= ``` Or use Azure Key Vault to secure your API Key.
 Create secrets for the url named `azure-open-ai`, and for the API Key named
-`azure-openai-key`. ``` export AZURE_KEY_VAULT_URL=https://.vault.azure.net/ az
-login ``` ## Main Commands To show help information about available commands
-and their usage, run: ```bash gpt --help ``` To display the current version of
-this CLI tool, run: ```bash gpt --version ``` Here are the main commands for
-using this CLI tool: ### 1. Ask a Question To submit a question to GPT and
-receive an answer, use the following format: ```bash gpt ask "What is the
-capital of France?" ``` You can customize your request using various options
-like maximum tokens (`--max-tokens`), temperature (`--temperature`), top-
-p value (`--top-p`), frequency penalty (`--frequency-penalty`), presence
-penalty (`--presence-penalty`), etc. #### Ask a Question about a File To submit
-a question to GPT with a file and receive an answer, use the following format:
-```bash gpt ask --files WordDocument.docx "Summarize the contents of this
-document." ``` ### 2. Review a PR To review a PR, use the following format:
-```bash gpt github review \ --access-token $GITHUB_ACCESS_TOKEN \ --pull-
-request $PULL_REQUEST_NUMBER \ --repository $REPOSITORY_NAME ``` ### 3.
-Generate a git commit message with GPT To generate a git commit message with
-GPT after having added the files, use the following format: ```bash git add .
-gpt git commit ``` For more detailed information on each command and its
-options, run: ```bash gpt COMMAND --help ``` Replace COMMAND with one of the
-main commands listed above (e.g., 'ask'). ## Developer Setup To install the
-package in development mode, with additional packages for testing, run the
-following command: ```bash pip install -e .[test] ```
+`azure-openai-key`. ```bash export AZURE_KEY_VAULT_URL=https:/
+/.vault.azure.net/ az login ``` ## Main Commands To show help information about
+available commands and their usage, run: ```bash gpt --help ``` To display the
+current version of this CLI tool, run: ```bash gpt --version ``` Here are the
+main commands for using this CLI tool: ### 1. Ask a Question To submit a
+question to GPT and receive an answer, use the following format: ```bash gpt
+ask "What is the capital of France?" ``` You can customize your request using
+various options like maximum tokens (`--max-tokens`), temperature (`--
+temperature`), top-p value (`--top-p`), frequency penalty (`--frequency-
+penalty`), presence penalty (`--presence-penalty`), etc. #### Ask a Question
+about a File To submit a question to GPT with a file and receive an answer, use
+the following format: ```bash gpt ask --files WordDocument.docx "Summarize the
+contents of this document." ``` ### 2. Review a PR To review a PR, use the
+following format: ```bash gpt github review \ --access-token
+$GITHUB_ACCESS_TOKEN \ --pull-request $PULL_REQUEST_NUMBER \ --repository
+$REPOSITORY_NAME ``` ### 3. Generate a git commit message with GPT To generate
+a git commit message with GPT after having added the files, use the following
+format: ```bash git add . gpt git commit ``` For more detailed information on
+each command and its options, run: ```bash gpt COMMAND --help ``` Replace
+COMMAND with one of the main commands listed above (e.g., 'ask'). ## Developer
+Setup To install the package in development mode, with additional packages for
+testing, run the following command: ```bash pip install -e .[test] ```
```

