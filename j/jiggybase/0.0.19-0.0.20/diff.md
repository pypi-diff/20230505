# Comparing `tmp/jiggybase-0.0.19.tar.gz` & `tmp/jiggybase-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.19.tar", last modified: Mon May  1 01:50:45 2023, max compression
+gzip compressed data, was "jiggybase-0.0.20.tar", last modified: Thu May  4 23:57:52 2023, max compression
```

## Comparing `jiggybase-0.0.19.tar` & `jiggybase-0.0.20.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-01 01:50:45.747926 jiggybase-0.0.19/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.19/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     4606 2023-05-01 01:50:45.747506 jiggybase-0.0.19/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     4071 2023-05-01 01:37:56.000000 jiggybase-0.0.19/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-01 01:50:45.740284 jiggybase-0.0.19/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.19/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.19/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     8508 2023-04-30 00:50:55.000000 jiggybase-0.0.19/jiggybase/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.19/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.19/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-01 01:50:45.746436 jiggybase-0.0.19/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.19/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.19/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.19/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.19/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.19/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.19/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.19/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.19/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.19/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.19/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3452 2023-04-10 19:09:18.000000 jiggybase-0.0.19/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.19/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.19/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.19/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.19/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-01 01:50:45.741782 jiggybase-0.0.19/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     4606 2023-05-01 01:50:45.000000 jiggybase-0.0.19/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      734 2023-05-01 01:50:45.000000 jiggybase-0.0.19/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-01 01:50:45.000000 jiggybase-0.0.19/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-01 01:50:45.000000 jiggybase-0.0.19/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-01 01:50:45.000000 jiggybase-0.0.19/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      669 2023-05-01 01:38:08.000000 jiggybase-0.0.19/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-01 01:50:45.748054 jiggybase-0.0.19/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-01 01:50:45.746913 jiggybase-0.0.19/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.19/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-04 23:57:52.925708 jiggybase-0.0.20/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.20/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-04 23:57:52.925295 jiggybase-0.0.20/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     5292 2023-05-01 15:45:10.000000 jiggybase-0.0.20/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-04 23:57:52.918666 jiggybase-0.0.20/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.20/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.20/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     8508 2023-04-30 00:50:55.000000 jiggybase-0.0.20/jiggybase/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.20/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.20/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-04 23:57:52.924250 jiggybase-0.0.20/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.20/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.20/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.20/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.20/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.20/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.20/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.20/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.20/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.20/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.20/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.20/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.20/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.20/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.20/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.20/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-04 23:57:52.920036 jiggybase-0.0.20/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-04 23:57:52.000000 jiggybase-0.0.20/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      734 2023-05-04 23:57:52.000000 jiggybase-0.0.20/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-04 23:57:52.000000 jiggybase-0.0.20/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-04 23:57:52.000000 jiggybase-0.0.20/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-04 23:57:52.000000 jiggybase-0.0.20/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      669 2023-05-04 23:56:48.000000 jiggybase-0.0.20/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-04 23:57:52.925817 jiggybase-0.0.20/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-04 23:57:52.924742 jiggybase-0.0.20/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.20/test/test.py
```

### Comparing `jiggybase-0.0.19/LICENSE` & `jiggybase-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/PKG-INFO` & `jiggybase-0.0.20/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.19
+Version: 0.0.20
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -38,61 +38,74 @@
 
 After importing, you need to create a JiggyBase client object:
 
 ```python
 jb = jiggybase.JiggyBase()
 ```
 
+Assuming you already created a collection 'my-collection', you can add files to the collection as follows:
+
+```python
+collection = jb.collection('my-collection')
+
+collection.upsert_file('/path/to/my/doc')
+
+```
+The document is now available in the collection and can be accessed by the collection's ChatGPT plugin, via chat.jiggy.ai, or via the associated chat API endpoint.
 
-### Client methods
 
-Here are the available `JiggyBase` client methods:
+### JiggyBase Client
+
+These are the top level methods of th `JiggyBase` client, primarily used for getting the user's organizations or all collections across all organizations.
 
 - `orgs()` - Returns a list of `Org` objects the user is a member of.
 - `get_org(name_or_id: str)` - Returns the `Org` object matching the given name or ID.
 - `api_keys()` - Returns a list of the user's `ApiKey` objects.
 - `authenticated_user()` - Returns the authenticated user's `User` object.
 - `collections()` - Returns a list of all `Collection` objects in all organizations the user is a member of.
 - `collection(name: str)` - Returns the `Collection` object matching the given name.
 
-### Organization methods
+### Organization
+
+Organizations in JiggyBase are a mechanism for separating different customers within the JiggyBase service.   Users can be a member of mutiple unrelated organizations.  A new user who subscribes to a JiggyBase service tier has their own oganization that they control as administrator of the organization.  Users can also be invited to an organization by existing members of the organization.
 
 For an `Org` object (e.g., `my_org = jb.get_org("<org_name>")`), you have access to the following methods:
 
 - `collections()` - Returns a list of `Collection` objects within the organization.
 - `collection(name: str)` - Returns the `Collection` object matching the given name.
 
 - `update([name: Optional[str] = None, description: Optional[str] = None])` - Updates the organization's name or description.
 
 
-### Collection methods
+### Collection
 
-For a `Collection` object (e.g., `my_collection = jb.collection("<collection_name>")`), you have access to the following methods:
+A collection is a group of documents that can be used to augment ChatGPT language models with your personalized information by using information from your collection to inform ChatGPT responses.   A collection can be exposed as a ChatGPT Plugin, via the JiggyBase ChatCompletion API, or via chat.jiggy.ai.   You have full control over who can access to your collection.  
 
-(adapt the usage code for each method accordingly)
+For a `Collection` object (e.g., `my_collection = jb.collection("<collection_name>")`), you have access to the following methods:
 
-- `set_description(self, description: str)` - Updates the description of the collection.
-- `set_oauth_verification_token(self, openai_verification_token: str)` - Sets the OpenAI verification token for the collection's plugin.
-- `plugin_oauth_config()` - Retrieves the OAuth configuration for the collection's plugin.
-- `delete()` - Deletes the collection permanently.
-- `get_chat_config()` - Retrieves the chat configuration for the collection.
-- `update_chat_config(model: str, prompt_task_id: int)` - Updates the chat configuration for the collection.
 - `upsert_file(file_path: str[, mimetype: str = None])` - Uploads a file to the collection.
 - `upsert(documents: List[Document])` - Adds a list of `Document` objects to the collection.
 - `query(queries: Union[str, List[str], Query][, top_k : int = 10])` - Queries the collection and returns a `QueryResponse` object.
 - `get_doc(id: str)` - Retrieves a document by its ID.
 - `get_chunks([start: int = 0, limit: int = 10, reverse: bool = True])` - Iterates through the chunks in a collection.
 - `delete_docs([ids: Optional[List[str]] = None, document_metadata_filter: Optional[DocumentMetadataFilter] = None, delete_all: Optional[bool] = False])` - Deletes items in the collection by document IDs, metadata filter, or deletes all documents.
+- `set_description(self, description: str)` - Updates the description of the collection.
+- `delete()` - Deletes the collection permanently.
+- `get_chat_config()` - Retrieves the chat configuration for the collection.
 
 ### Organization User Management
 
+An organization supports multiple roles for members, including 'admin', 'member', and 'viewer'.   A viwer role can access the data in the collection for chat purposes.  A member can upload new documents to the collection.  
+
 - `members()` - Returns a list of `OrgMember` objects within the organization.
 - `add_member(email: str, role: OrgRole)` - Adds a new member to the organization with the given email and role.
 - `delete_member(email: str)` - Deletes a member from the organization using the given email.
 
 ### Organization Prompt Management
 
+JiggyBase supports user-customized prompts for the JiggyBase ChatCompletion API.   The following methods are provided to manage the customized prompts.
+
 - `prompt_tasks([name=None, version=None])` - Returns a list of `PromptTask` objects, optionally filtering by name and version.
 - `create_prompt_task(name: str, version: int, prompts: List[PromptMessage][, type: Optional[PromptTaskType] = None, description: Optional[str] = None])` - Creates a new `PromptTask` object with the specified parameters.
 - `update_prompt_task(name: str, prompts: List[PromptMessage])` - Updates the specified prompt task's prompts.
 - `get_prompt_task(prompt_task_id: int)` - Retrieves a `PromptTask` object using the given prompt_task_id.
 - `delete_prompt_task(prompt_task_id: int)` - Deletes a `PromptTask` object using the given prompt_task_id.
```

### Comparing `jiggybase-0.0.19/README.md` & `jiggybase-0.0.20/jiggybase.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: jiggybase
+Version: 0.0.20
+Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
+Author-email: Bill Kish <bk@jiggy.ai>
+Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
+Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # JiggyBase
 
 JiggyBase is a Python library for interacting with the JiggyBase service at https://jiggy.ai.
 
 Use it to manage your JiggyBase organization and collections, including uploading documents into a collection.
 
 ## Requirements
@@ -24,61 +38,74 @@
 
 After importing, you need to create a JiggyBase client object:
 
 ```python
 jb = jiggybase.JiggyBase()
 ```
 
+Assuming you already created a collection 'my-collection', you can add files to the collection as follows:
+
+```python
+collection = jb.collection('my-collection')
 
-### Client methods
+collection.upsert_file('/path/to/my/doc')
+
+```
+The document is now available in the collection and can be accessed by the collection's ChatGPT plugin, via chat.jiggy.ai, or via the associated chat API endpoint.
 
-Here are the available `JiggyBase` client methods:
+
+### JiggyBase Client
+
+These are the top level methods of th `JiggyBase` client, primarily used for getting the user's organizations or all collections across all organizations.
 
 - `orgs()` - Returns a list of `Org` objects the user is a member of.
 - `get_org(name_or_id: str)` - Returns the `Org` object matching the given name or ID.
 - `api_keys()` - Returns a list of the user's `ApiKey` objects.
 - `authenticated_user()` - Returns the authenticated user's `User` object.
 - `collections()` - Returns a list of all `Collection` objects in all organizations the user is a member of.
 - `collection(name: str)` - Returns the `Collection` object matching the given name.
 
-### Organization methods
+### Organization
+
+Organizations in JiggyBase are a mechanism for separating different customers within the JiggyBase service.   Users can be a member of mutiple unrelated organizations.  A new user who subscribes to a JiggyBase service tier has their own oganization that they control as administrator of the organization.  Users can also be invited to an organization by existing members of the organization.
 
 For an `Org` object (e.g., `my_org = jb.get_org("<org_name>")`), you have access to the following methods:
 
 - `collections()` - Returns a list of `Collection` objects within the organization.
 - `collection(name: str)` - Returns the `Collection` object matching the given name.
 
 - `update([name: Optional[str] = None, description: Optional[str] = None])` - Updates the organization's name or description.
 
 
-### Collection methods
+### Collection
 
-For a `Collection` object (e.g., `my_collection = jb.collection("<collection_name>")`), you have access to the following methods:
+A collection is a group of documents that can be used to augment ChatGPT language models with your personalized information by using information from your collection to inform ChatGPT responses.   A collection can be exposed as a ChatGPT Plugin, via the JiggyBase ChatCompletion API, or via chat.jiggy.ai.   You have full control over who can access to your collection.  
 
-(adapt the usage code for each method accordingly)
+For a `Collection` object (e.g., `my_collection = jb.collection("<collection_name>")`), you have access to the following methods:
 
-- `set_description(self, description: str)` - Updates the description of the collection.
-- `set_oauth_verification_token(self, openai_verification_token: str)` - Sets the OpenAI verification token for the collection's plugin.
-- `plugin_oauth_config()` - Retrieves the OAuth configuration for the collection's plugin.
-- `delete()` - Deletes the collection permanently.
-- `get_chat_config()` - Retrieves the chat configuration for the collection.
-- `update_chat_config(model: str, prompt_task_id: int)` - Updates the chat configuration for the collection.
 - `upsert_file(file_path: str[, mimetype: str = None])` - Uploads a file to the collection.
 - `upsert(documents: List[Document])` - Adds a list of `Document` objects to the collection.
 - `query(queries: Union[str, List[str], Query][, top_k : int = 10])` - Queries the collection and returns a `QueryResponse` object.
 - `get_doc(id: str)` - Retrieves a document by its ID.
 - `get_chunks([start: int = 0, limit: int = 10, reverse: bool = True])` - Iterates through the chunks in a collection.
 - `delete_docs([ids: Optional[List[str]] = None, document_metadata_filter: Optional[DocumentMetadataFilter] = None, delete_all: Optional[bool] = False])` - Deletes items in the collection by document IDs, metadata filter, or deletes all documents.
+- `set_description(self, description: str)` - Updates the description of the collection.
+- `delete()` - Deletes the collection permanently.
+- `get_chat_config()` - Retrieves the chat configuration for the collection.
 
 ### Organization User Management
 
+An organization supports multiple roles for members, including 'admin', 'member', and 'viewer'.   A viwer role can access the data in the collection for chat purposes.  A member can upload new documents to the collection.  
+
 - `members()` - Returns a list of `OrgMember` objects within the organization.
 - `add_member(email: str, role: OrgRole)` - Adds a new member to the organization with the given email and role.
 - `delete_member(email: str)` - Deletes a member from the organization using the given email.
 
 ### Organization Prompt Management
 
+JiggyBase supports user-customized prompts for the JiggyBase ChatCompletion API.   The following methods are provided to manage the customized prompts.
+
 - `prompt_tasks([name=None, version=None])` - Returns a list of `PromptTask` objects, optionally filtering by name and version.
 - `create_prompt_task(name: str, version: int, prompts: List[PromptMessage][, type: Optional[PromptTaskType] = None, description: Optional[str] = None])` - Creates a new `PromptTask` object with the specified parameters.
 - `update_prompt_task(name: str, prompts: List[PromptMessage])` - Updates the specified prompt task's prompts.
 - `get_prompt_task(prompt_task_id: int)` - Retrieves a `PromptTask` object using the given prompt_task_id.
-- `delete_prompt_task(prompt_task_id: int)` - Deletes a `PromptTask` object using the given prompt_task_id.
+- `delete_prompt_task(prompt_task_id: int)` - Deletes a `PromptTask` object using the given prompt_task_id.
```

### Comparing `jiggybase-0.0.19/jiggybase/client.py` & `jiggybase-0.0.20/jiggybase/client.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase/collection.py` & `jiggybase-0.0.20/jiggybase/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase/jiggybase_session.py` & `jiggybase-0.0.20/jiggybase/jiggybase_session.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase/login.py` & `jiggybase-0.0.20/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase/models/auth.py` & `jiggybase-0.0.20/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase/models/chat.py` & `jiggybase-0.0.20/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase/models/chunk.py` & `jiggybase-0.0.20/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase/models/collection.py` & `jiggybase-0.0.20/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase/models/metadata.py` & `jiggybase-0.0.20/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase/models/org.py` & `jiggybase-0.0.20/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase/models/plugin.py` & `jiggybase-0.0.20/jiggybase/models/plugin.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase/models/plugin_config.py` & `jiggybase-0.0.20/jiggybase/models/plugin_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 from pydantic import BaseModel, HttpUrl, Field, validator
 from typing import List, Optional
 from enum import Enum
-from sqlmodel import SQLModel, Field
 from .collection import PluginAuthType        
 import re
 
 MODELNAME = re.compile("[a-zA-Z][a-zA-Z0-9_]*")
 
 class PluginConfig(BaseModel): 
     """
```

### Comparing `jiggybase-0.0.19/jiggybase/models/prompt.py` & `jiggybase-0.0.20/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase/models/providers.py` & `jiggybase-0.0.20/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase/models/user.py` & `jiggybase-0.0.20/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase/org.py` & `jiggybase-0.0.20/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.20/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: jiggybase
-Version: 0.0.19
-Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
-Author-email: Bill Kish <bk@jiggy.ai>
-Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
-Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # JiggyBase
 
 JiggyBase is a Python library for interacting with the JiggyBase service at https://jiggy.ai.
 
 Use it to manage your JiggyBase organization and collections, including uploading documents into a collection.
 
 ## Requirements
@@ -38,61 +24,74 @@
 
 After importing, you need to create a JiggyBase client object:
 
 ```python
 jb = jiggybase.JiggyBase()
 ```
 
+Assuming you already created a collection 'my-collection', you can add files to the collection as follows:
+
+```python
+collection = jb.collection('my-collection')
 
-### Client methods
+collection.upsert_file('/path/to/my/doc')
+
+```
+The document is now available in the collection and can be accessed by the collection's ChatGPT plugin, via chat.jiggy.ai, or via the associated chat API endpoint.
 
-Here are the available `JiggyBase` client methods:
+
+### JiggyBase Client
+
+These are the top level methods of th `JiggyBase` client, primarily used for getting the user's organizations or all collections across all organizations.
 
 - `orgs()` - Returns a list of `Org` objects the user is a member of.
 - `get_org(name_or_id: str)` - Returns the `Org` object matching the given name or ID.
 - `api_keys()` - Returns a list of the user's `ApiKey` objects.
 - `authenticated_user()` - Returns the authenticated user's `User` object.
 - `collections()` - Returns a list of all `Collection` objects in all organizations the user is a member of.
 - `collection(name: str)` - Returns the `Collection` object matching the given name.
 
-### Organization methods
+### Organization
+
+Organizations in JiggyBase are a mechanism for separating different customers within the JiggyBase service.   Users can be a member of mutiple unrelated organizations.  A new user who subscribes to a JiggyBase service tier has their own oganization that they control as administrator of the organization.  Users can also be invited to an organization by existing members of the organization.
 
 For an `Org` object (e.g., `my_org = jb.get_org("<org_name>")`), you have access to the following methods:
 
 - `collections()` - Returns a list of `Collection` objects within the organization.
 - `collection(name: str)` - Returns the `Collection` object matching the given name.
 
 - `update([name: Optional[str] = None, description: Optional[str] = None])` - Updates the organization's name or description.
 
 
-### Collection methods
+### Collection
 
-For a `Collection` object (e.g., `my_collection = jb.collection("<collection_name>")`), you have access to the following methods:
+A collection is a group of documents that can be used to augment ChatGPT language models with your personalized information by using information from your collection to inform ChatGPT responses.   A collection can be exposed as a ChatGPT Plugin, via the JiggyBase ChatCompletion API, or via chat.jiggy.ai.   You have full control over who can access to your collection.  
 
-(adapt the usage code for each method accordingly)
+For a `Collection` object (e.g., `my_collection = jb.collection("<collection_name>")`), you have access to the following methods:
 
-- `set_description(self, description: str)` - Updates the description of the collection.
-- `set_oauth_verification_token(self, openai_verification_token: str)` - Sets the OpenAI verification token for the collection's plugin.
-- `plugin_oauth_config()` - Retrieves the OAuth configuration for the collection's plugin.
-- `delete()` - Deletes the collection permanently.
-- `get_chat_config()` - Retrieves the chat configuration for the collection.
-- `update_chat_config(model: str, prompt_task_id: int)` - Updates the chat configuration for the collection.
 - `upsert_file(file_path: str[, mimetype: str = None])` - Uploads a file to the collection.
 - `upsert(documents: List[Document])` - Adds a list of `Document` objects to the collection.
 - `query(queries: Union[str, List[str], Query][, top_k : int = 10])` - Queries the collection and returns a `QueryResponse` object.
 - `get_doc(id: str)` - Retrieves a document by its ID.
 - `get_chunks([start: int = 0, limit: int = 10, reverse: bool = True])` - Iterates through the chunks in a collection.
 - `delete_docs([ids: Optional[List[str]] = None, document_metadata_filter: Optional[DocumentMetadataFilter] = None, delete_all: Optional[bool] = False])` - Deletes items in the collection by document IDs, metadata filter, or deletes all documents.
+- `set_description(self, description: str)` - Updates the description of the collection.
+- `delete()` - Deletes the collection permanently.
+- `get_chat_config()` - Retrieves the chat configuration for the collection.
 
 ### Organization User Management
 
+An organization supports multiple roles for members, including 'admin', 'member', and 'viewer'.   A viwer role can access the data in the collection for chat purposes.  A member can upload new documents to the collection.  
+
 - `members()` - Returns a list of `OrgMember` objects within the organization.
 - `add_member(email: str, role: OrgRole)` - Adds a new member to the organization with the given email and role.
 - `delete_member(email: str)` - Deletes a member from the organization using the given email.
 
 ### Organization Prompt Management
 
+JiggyBase supports user-customized prompts for the JiggyBase ChatCompletion API.   The following methods are provided to manage the customized prompts.
+
 - `prompt_tasks([name=None, version=None])` - Returns a list of `PromptTask` objects, optionally filtering by name and version.
 - `create_prompt_task(name: str, version: int, prompts: List[PromptMessage][, type: Optional[PromptTaskType] = None, description: Optional[str] = None])` - Creates a new `PromptTask` object with the specified parameters.
 - `update_prompt_task(name: str, prompts: List[PromptMessage])` - Updates the specified prompt task's prompts.
 - `get_prompt_task(prompt_task_id: int)` - Retrieves a `PromptTask` object using the given prompt_task_id.
 - `delete_prompt_task(prompt_task_id: int)` - Deletes a `PromptTask` object using the given prompt_task_id.
```

### Comparing `jiggybase-0.0.19/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.20/jiggybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.19/pyproject.toml` & `jiggybase-0.0.20/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.19"
+version = "0.0.20"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pedantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.0.19/test/test.py` & `jiggybase-0.0.20/test/test.py`

 * *Files identical despite different names*

