# Comparing `tmp/gpt-review-0.4.0rc389.post1.tar.gz` & `tmp/gpt-review-0.5.0rc398.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.4.0rc389.post1.tar", last modified: Thu May  4 01:09:22 2023, max compression
+gzip compressed data, was "gpt-review-0.5.0rc398.post1.tar", last modified: Thu May  4 22:35:09 2023, max compression
```

## Comparing `gpt-review-0.4.0rc389.post1.tar` & `gpt-review-0.5.0rc398.post1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0      336 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     2229 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4361 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1795 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/.pypirc
--rw-r--r--   0        0        0     1125 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/LICENSE
--rw-r--r--   0        0        0     3017 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/README.md
--rw-r--r--   0        0        0     4920 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/action.yml
--rw-r--r--   0        0        0     8252 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/pyproject.toml
--rw-r--r--   0        0        0      366 2023-05-04 01:09:21.664787 gpt-review-0.4.0rc389.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0    11455 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1924 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5738 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1402 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0      788 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     6730 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      464 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      488 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0     2566 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/tests/mock.diff
--rw-r--r--   0        0        0      462 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/tests/test_git.py
--rw-r--r--   0        0        0     1363 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/tests/test_github.py
--rw-r--r--   0        0        0     5987 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      420 2023-05-04 01:09:15.608847 gpt-review-0.4.0rc389.post1/tests/test_review.py
--rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 gpt-review-0.4.0rc389.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-04 22:35:01.084391 gpt-review-0.5.0rc398.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-04 22:35:01.084391 gpt-review-0.5.0rc398.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     2229 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4930 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1795 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/LICENSE
+-rw-r--r--   0        0        0     3017 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/README.md
+-rw-r--r--   0        0        0     4920 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/action.yml
+-rw-r--r--   0        0        0     8252 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/pyproject.toml
+-rw-r--r--   0        0        0      366 2023-05-04 22:35:09.088444 gpt-review-0.5.0rc398.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0    10048 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1924 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5738 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1402 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     3221 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0      788 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     6730 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      464 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      488 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0     2566 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/tests/mock.diff
+-rw-r--r--   0        0        0      462 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1363 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/tests/test_github.py
+-rw-r--r--   0        0        0     5987 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      590 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0      420 2023-05-04 22:35:01.088391 gpt-review-0.5.0rc398.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 gpt-review-0.5.0rc398.post1/PKG-INFO
```

### Comparing `gpt-review-0.4.0rc389.post1/.devcontainer/devcontainer.json` & `gpt-review-0.5.0rc398.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.5.0rc398.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/.github/dependabot.yml` & `gpt-review-0.5.0rc398.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/.github/pull_request_template.md` & `gpt-review-0.5.0rc398.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/.github/workflows/codeql.yml` & `gpt-review-0.5.0rc398.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.5.0rc398.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.5.0rc398.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/.github/workflows/python.yml` & `gpt-review-0.5.0rc398.post1/.github/workflows/python.yml`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,34 @@
           ${{ matrix.tools }}: true
           args: ${{ matrix.args }}
           workdir: '.'
           testdir: 'tests'
           python_version: '3.11.3'
           flags: ${{ matrix.flags }}
 
+  unit-tests:
+    runs-on: ubuntu-latest
+    strategy:
+      fail-fast: true
+      matrix:
+        python: ['3.7', '3.8', '3.9', '3.10', '3.11']
+    steps:
+      - uses: actions/checkout@v2
+        with:
+          ref: ${{ github.event.pull_request.head.sha }}
+      - name: ${{ matrix.tools }}
+        uses: microsoft/action-python@0.6.3
+        with:
+          pytest: true
+          args: -m not integration and not cli
+          workdir: '.'
+          testdir: 'tests'
+          python_version: ${{ matrix.python }}
+          flags: unittests-${{ matrix.python }}
+
   publish:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
         with:
           ref: ${{ github.event.pull_request.head.sha }}
           token: ${{ secrets.PAT }}
```

### Comparing `gpt-review-0.4.0rc389.post1/.github/workflows/test-action.yml` & `gpt-review-0.5.0rc398.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/.gitignore` & `gpt-review-0.5.0rc398.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/.vscode/settings.json` & `gpt-review-0.5.0rc398.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/LICENSE` & `gpt-review-0.5.0rc398.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/README.md` & `gpt-review-0.5.0rc398.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/action.yml` & `gpt-review-0.5.0rc398.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/pyproject.toml` & `gpt-review-0.5.0rc398.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/src/gpt_review/_ask.py` & `gpt-review-0.5.0rc398.post1/src/gpt_review/_ask.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,121 +1,30 @@
 """Ask GPT a question."""
 import logging
 import os
 import time
 from typing import Dict, List, Optional
-from typing_extensions import override
 from knack import CLICommandsLoader
 from knack.arguments import ArgumentsContext
 from knack.commands import CommandGroup
 from knack.util import CLIError
 
 import openai
 from azure.identity import DefaultAzureCredential
 from azure.keyvault.secrets import SecretClient
 from openai.error import RateLimitError
-from langchain.llms import AzureOpenAI
-from langchain.embeddings import OpenAIEmbeddings
-from llama_index import (
-    GPTVectorStoreIndex,
-    LangchainEmbedding,
-    ServiceContext,
-    LLMPredictor,
-    SimpleDirectoryReader,
-)
-from llama_index.indices.base import BaseGPTIndex
 
 from gpt_review._command import GPTCommandGroup
+from gpt_review._llama_index import _ask_doc
 import gpt_review.constants as C
 
 
 DEFAULT_KEY_VAULT = "https://dciborow-openai.vault.azure.net/"
 
 
-def _ask_doc(question: str, files: List[str]) -> str:
-    """
-    Ask GPT a question.
-
-    Args:
-        question (List[str]): The question to ask.
-        files (List[str]): The files to search.
-
-    Returns:
-        Dict[str, str]: The response.
-    """
-    documents = SimpleDirectoryReader(input_files=files).load_data()
-    index = _document_indexer(documents)
-
-    return index.as_query_engine().query(question).response  # type: ignore
-
-
-def _document_indexer(documents) -> BaseGPTIndex:
-    """
-    Create a document indexer.
-
-    Deployment names include: "gpt-35-turbo", "text-davinci-003"
-
-    Args:
-        documents (List[Document]): The documents to index.
-        azure (bool): Whether to use Azure OpenAI.
-
-    Returns:
-        GPTVectorStoreIndex: The document indexer.
-    """
-    _load_azure_openai_context()
-
-    llm = AzureGPT35Turbo(  # type: ignore
-        deployment_name="gpt-35-turbo",
-        model_kwargs={
-            "api_key": openai.api_key,
-            "api_base": openai.api_base,
-            "api_type": "azure",
-            "api_version": "2023-03-15-preview",
-        },
-        max_retries=10,
-    )
-    llm_predictor = LLMPredictor(llm=llm)
-
-    embedding_llm = LangchainEmbedding(
-        OpenAIEmbeddings(
-            model="text-embedding-ada-002",
-        ),  # type: ignore
-        embed_batch_size=1,
-    )
-
-    service_context = ServiceContext.from_defaults(
-        llm_predictor=llm_predictor,
-        embed_model=embedding_llm,
-    )
-    return GPTVectorStoreIndex.from_documents(documents, service_context=service_context)
-
-
-class AzureGPT35Turbo(AzureOpenAI):
-    """Azure OpenAI Chat API."""
-
-    @property
-    @override
-    def _default_params(self):
-        """
-        Get the default parameters for calling OpenAI API.
-        gpt-35-turbo does not support best_of, logprobs, or echo.
-        """
-        normal_params = {
-            "temperature": self.temperature,
-            "max_tokens": self.max_tokens,
-            "top_p": self.top_p,
-            "frequency_penalty": self.frequency_penalty,
-            "presence_penalty": self.presence_penalty,
-            "n": self.n,
-            "request_timeout": self.request_timeout,
-            "logit_bias": self.logit_bias,
-        }
-        return {**normal_params, **self.model_kwargs}
-
-
 def validate_parameter_range(namespace) -> None:
     """
     Validate the following parameters:
     - max_tokens is in [1,4000]
     - temperature is in [0,1]
     - top_p is in [0,1]
     - frequency_penalty is in [0,2]
@@ -157,46 +66,49 @@
     max_tokens: int = C.MAX_TOKENS_DEFAULT,
     temperature: float = C.TEMPERATURE_DEFAULT,
     top_p: float = C.TOP_P_DEFAULT,
     frequency_penalty: float = C.FREQUENCY_PENALTY_DEFAULT,
     presence_penalty: float = C.PRESENCE_PENALTY_DEFAULT,
     files: Optional[List[str]] = None,
     fast: bool = False,
+    large: bool = False,
 ) -> Dict[str, str]:
     """Ask GPT a question."""
+    _load_azure_openai_context()
 
     prompt = " ".join(question)
 
     if files:
-        response = _ask_doc(prompt, files)
+        response = _ask_doc(prompt, files, fast=fast, large=large)
     else:
         response = _call_gpt(
             prompt=prompt,
             max_tokens=max_tokens,
             temperature=temperature,
             top_p=top_p,
             frequency_penalty=frequency_penalty,
             presence_penalty=presence_penalty,
             fast=fast,
+            large=large,
         )
     return {"response": response}
 
 
 def _load_azure_openai_context() -> None:
     """
     Load the Azure OpenAI context.
 
     If the environment variables are not set, retrieve the values from Azure Key Vault.
 
     Set both the environment variables and the openai package variables.
     - Without setting the environment variables, the integration tests fail.
     - Without setting the openai package variables, the cli tests fail.
     """
-    openai.api_type = "azure"
-    openai.api_version = "2023-03-15-preview"
+    openai.api_type = os.environ["OPENAI_API_TYPE"] = "azure"
+    openai.api_version = os.environ["OPENAI_API_VERSION"] = "2023-03-15-preview"
 
     if os.getenv("AZURE_OPENAI_API"):
         openai.api_base = os.environ["OPENAI_API_BASE"] = os.getenv("AZURE_OPENAI_API")  # type: ignore
         openai.api_key = os.environ["OPENAI_API_KEY"] = os.getenv("AZURE_OPENAI_API_KEY")  # type: ignore
     else:
         kv_client = SecretClient(
             vault_url=os.getenv("AZURE_KEY_VAULT_URL", DEFAULT_KEY_VAULT), credential=DefaultAzureCredential()
@@ -211,37 +123,37 @@
     max_tokens=500,
     top_p=1.0,
     frequency_penalty=0.5,
     presence_penalty=0.0,
     retry=0,
     messages=None,
     fast: bool = False,
+    large: bool = False,
 ) -> str:
     """
     Call GPT-4 with the given prompt.
 
     Args:
         prompt (str): The prompt to send to GPT-4.
         temperature (float, optional): The temperature to use. Defaults to 0.10.
         max_tokens (int, optional): The maximum number of tokens to generate. Defaults to 500.
         top_p (float, optional): The top_p to use. Defaults to 1.
         frequency_penalty (float, optional): The frequency penalty to use. Defaults to 0.5.
         presence_penalty (float, optional): The presence penalty to use. Defaults to 0.0.
         retry (int, optional): The number of times to retry the request. Defaults to 0.
         messages (List[Dict[str, str]], optional): The messages to send to GPT-4. Defaults to None.
         fast (bool, optional): Whether to use the fast model. Defaults to False.
+        large (bool, optional): Whether to use the large model. Defaults to False.
 
     Returns:
         str: The response from GPT-4.
     """
-    _load_azure_openai_context()
-
     messages = messages or [{"role": "user", "content": prompt}]
     try:
-        engine = _get_engine(prompt, fast)
+        engine = _get_engine(prompt, max_tokens=max_tokens, fast=fast, large=large)
         logging.info("Model Selected based on prompt size: %s", engine)
 
         logging.info("Prompt sent to GPT: %s\n", prompt)
         completion = openai.ChatCompletion.create(
             engine=engine,
             messages=messages,
             max_tokens=max_tokens,
@@ -255,28 +167,51 @@
         if retry < 5:
             logging.warning("Call to GPT failed due to rate limit, retry attempt: %s", retry)
             time.sleep(retry * 10)
             return _call_gpt(prompt, temperature, max_tokens, top_p, frequency_penalty, presence_penalty, retry + 1)
         raise RateLimitError("Retry limit exceeded") from error
 
 
-def _get_engine(prompt: str, fast: bool = False) -> str:
+def _get_engine(prompt: str, max_tokens: int, fast: bool = False, large: bool = False) -> str:
     """
     Get the Engine based on the prompt length.
     - when greater then 8k use gpt-4-32k
     - otherwise use gpt-4
     - enable fast to use gpt-35-turbo for small prompts
+
+    Args:
+        prompt (str): The prompt to send to GPT-4.
+        max_tokens (int): The maximum number of tokens to generate.
+        fast (bool, optional): Whether to use the fast model. Defaults to False.
+        large (bool, optional): Whether to use the large model. Defaults to False.
+
+    Returns:
+        str: The engine to use.
     """
-    if len(prompt) > 8000:
+    tokens = _count_tokens(prompt)
+    if large or tokens + max_tokens > 8000:
         return "gpt-4-32k"
-    if len(prompt) > 4000:
+    if tokens + max_tokens > 4000:
         return "gpt-4"
     return "gpt-35-turbo" if fast else "gpt-4"
 
 
+def _count_tokens(prompt) -> int:
+    """
+    Determine number of tokens in prompt.
+
+    Args:
+        prompt (str): The prompt to send to GPT-4.
+
+    Returns:
+        int: The number of tokens in the prompt.
+    """
+    return int(len(prompt) / 4 * 3)
+
+
 class AskCommandGroup(GPTCommandGroup):
     """Ask Command Group."""
 
     @staticmethod
     def load_command_table(loader: CLICommandsLoader) -> None:
         with CommandGroup(loader, "", "gpt_review._ask#{}") as group:
             group.command("ask", "_ask", is_preview=True)
@@ -288,14 +223,20 @@
             args.argument(
                 "fast",
                 help="Use gpt-35-turbo for prompts < 4000 tokens.",
                 default=False,
                 action="store_true",
             )
             args.argument(
+                "large",
+                help="Use gpt-4-32k for prompts.",
+                default=False,
+                action="store_true",
+            )
+            args.argument(
                 "temperature",
                 type=float,
                 help="Sets the level of creativity/randomness.",
                 validator=validate_parameter_range,
             )
             args.argument(
                 "max_tokens",
```

### Comparing `gpt-review-0.4.0rc389.post1/src/gpt_review/_git.py` & `gpt-review-0.5.0rc398.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/src/gpt_review/_github.py` & `gpt-review-0.5.0rc398.post1/src/gpt_review/_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.5.0rc398.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/src/gpt_review/_repository.py` & `gpt-review-0.5.0rc398.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/src/gpt_review/_review.py` & `gpt-review-0.5.0rc398.post1/src/gpt_review/_review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/tests/conftest.py` & `gpt-review-0.5.0rc398.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/tests/mock.diff` & `gpt-review-0.5.0rc398.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/tests/test_github.py` & `gpt-review-0.5.0rc398.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/tests/test_gpt_cli.py` & `gpt-review-0.5.0rc398.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc389.post1/PKG-INFO` & `gpt-review-0.5.0rc398.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.4.0rc389.post1
+Version: 0.5.0rc398.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.4.0rc389.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.5.0rc398.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

