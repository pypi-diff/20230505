# Comparing `tmp/fuzzly-0.0.3.tar.gz` & `tmp/fuzzly-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzly-0.0.3.tar", last modified: Fri Apr 21 02:31:23 2023, max compression
+gzip compressed data, was "fuzzly-0.0.4.tar", last modified: Fri May  5 05:35:16 2023, max compression
```

## Comparing `fuzzly-0.0.3.tar` & `fuzzly-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:31:23.114749 fuzzly-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-21 02:30:53.000000 fuzzly-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-21 02:31:23.114749 fuzzly-0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:31:23.110749 fuzzly-0.0.3/fuzzly/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:31:23.114749 fuzzly-0.0.3/fuzzly/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/api/post.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/api/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:31:23.114749 fuzzly-0.0.3/fuzzly/client/
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:31:23.114749 fuzzly-0.0.3/fuzzly/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17383 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/post.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-21 02:30:53.000000 fuzzly-0.0.3/fuzzly/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:31:23.114749 fuzzly-0.0.3/fuzzly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-21 02:31:23.000000 fuzzly-0.0.3/fuzzly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-21 02:31:23.000000 fuzzly-0.0.3/fuzzly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 02:31:23.000000 fuzzly-0.0.3/fuzzly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 02:31:23.000000 fuzzly-0.0.3/fuzzly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 02:31:23.000000 fuzzly-0.0.3/fuzzly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 02:31:23.114749 fuzzly-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-21 02:30:53.000000 fuzzly-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:35:16.937991 fuzzly-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-05 05:34:43.000000 fuzzly-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-05 05:35:16.937991 fuzzly-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:35:16.937991 fuzzly-0.0.4/fuzzly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:35:16.937991 fuzzly-0.0.4/fuzzly/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/api/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/api/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:35:16.937991 fuzzly-0.0.4/fuzzly/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:35:16.937991 fuzzly-0.0.4/fuzzly/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/models/_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/models/_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/models/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/models/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-05 05:34:43.000000 fuzzly-0.0.4/fuzzly/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:35:16.937991 fuzzly-0.0.4/fuzzly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-05 05:35:16.000000 fuzzly-0.0.4/fuzzly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-05 05:35:16.000000 fuzzly-0.0.4/fuzzly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:35:16.000000 fuzzly-0.0.4/fuzzly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 05:35:16.000000 fuzzly-0.0.4/fuzzly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 05:35:16.000000 fuzzly-0.0.4/fuzzly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:35:16.937991 fuzzly-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-05 05:34:43.000000 fuzzly-0.0.4/setup.py
```

### Comparing `fuzzly-0.0.3/LICENSE` & `fuzzly-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.3/PKG-INFO` & `fuzzly-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: fuzzly
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fuzz.ly client library for Python3
 Home-page: https://github.com/kheina-com/fuzzly
 Author: kheina
 License: Mozilla Public License 2.0
-Requires-Python: >=3.9.*
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 	<img src="https://github.com/kheina-com/fuzzly/raw/main/logo.png" alt="fuzzly Logo">
 	<br>
 	<a href="https://github.com/kheina-com/fuzzly/actions?query=workflow%3Apython-package+event%3Apush+branch%3Amain">
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: fuzzly Version: 0.0.3 Summary: Fuzz.ly client
+Metadata-Version: 2.1 Name: fuzzly Version: 0.0.4 Summary: Fuzz.ly client
 library for Python3 Home-page: https://github.com/kheina-com/fuzzly Author:
-kheina License: Mozilla Public License 2.0 Requires-Python: >=3.9.*
-Description-Content-Type: text/markdown License-File: LICENSE
+kheina License: Mozilla Public License 2.0 Requires-Python: >=3.9 Description-
+Content-Type: text/markdown License-File: LICENSE
                                 [fuzzly Logo]
                [python-package_workflow] [pypi_package_version]
                       A python client library for fuzz.ly
 # Installation ```bash $ pip install fuzzly ``` # Usage ```python from fuzzly
 import FuzzlyClient from fuzzly.models.post import Post # if you have a bot
 token, make sure you initialize the client with your token token: str =
 'aGV5IG1hbi4gaXQncyB3ZWlyZCB0aGF0IHlvdSBsb29rZWQgYXQgdGhpcywgYnV0IHRoaXMgaXNuJ3QgYSByZWFsIHRva2Vu'
```

### Comparing `fuzzly-0.0.3/fuzzly/__init__.py` & `fuzzly-0.0.4/fuzzly/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A python client library for fuzz.ly"""  # this comment should match the package slogan under the logo in the readme
 
 
-__version__: str = '0.0.3'
+__version__: str = '0.0.4'
 
 
 from typing import List
 
 from .api.post import FetchMyPosts, FetchPost
 from .api.tag import FetchPostTags, FetchTag
 from .client import Client
```

### Comparing `fuzzly-0.0.3/fuzzly/client/__init__.py` & `fuzzly-0.0.4/fuzzly/client/__init__.py`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.3/fuzzly/constants.py` & `fuzzly-0.0.4/fuzzly/constants.py`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.3/fuzzly/models/_database.py` & `fuzzly-0.0.4/fuzzly/models/_database.py`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.3/fuzzly/models/_shared.py` & `fuzzly-0.0.4/fuzzly/models/_shared.py`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.3/fuzzly/models/config.py` & `fuzzly-0.0.4/fuzzly/models/config.py`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.3/fuzzly/models/internal.py` & `fuzzly-0.0.4/fuzzly/models/internal.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 class _InternalClient(Client) :
 	"""
 	There's a lot of api calls that needs to occur within internal models to work correctly.
 	Those are set up within this client so that the main client in the root does not break without internal auth/kvs access
 	"""
 
 	_user_config: Gateway = Gateway(ConfigHost + '/i1/user/{user_id}', UserConfig, method='GET')
-	_post_tags: Gateway = Gateway(TagHost + '/v1/post/{post_id}', TagGroups, method='GET')
+	_post_tags: Gateway = Gateway(TagHost + '/i1/tags/{post_id}', TagGroups, method='GET')
 	_user_posts: Gateway  # this will be assigned later
 	_post: Gateway  # this will be assigned later
 	_user: Gateway  # this will be assigned later
 	_tag: Gateway  # this will be assigned later
 
 	following_many: Callable[[KhUser, List[int]], Coroutine[Any, Any, Dict[int, bool]]]
 	users_many: Callable[[List[int]], Coroutine[Any, Any, Dict[int, InternalUser]]]
@@ -381,15 +381,15 @@
 class InternalPosts(BaseModel) :
 	post_list: List[InternalPost] = []
 
 	def append(self: 'InternalPosts', post: InternalPost) :
 		return self.post_list.append(post)
 
 
-	async def uploaders(self: 'InternalPosts', client: _InternalClient, user: KhUser) -> Dict[int, User] :
+	async def uploaders(self: 'InternalPosts', client: _InternalClient, user: KhUser) -> Dict[int, UserPortable] :
 		"""
 		returns populated user objects for every uploader id provided
 
 		:return: dict in the form user id -> populated User object
 		"""
 		uploader_ids: List[int] = list(set(map(lambda x : x.user_id, self.post_list)))
 		users_task: Task[Dict[int, InternalUser]] = ensure_future(client.users_many(uploader_ids))
@@ -400,26 +400,21 @@
 
 		else :
 			following = defaultdict(lambda : None)
 
 		iusers: Dict[int, InternalUser] = await users_task
 
 		return {
-			user_id: User(
+			user_id: UserPortable(
 				name=iuser.name,
 				handle=iuser.handle,
 				privacy=iuser.privacy,
 				icon=iuser.icon,
-				banner=iuser.banner,
-				website=iuser.website,
-				created=iuser.created,
-				description=iuser.description,
 				verified=iuser.verified,
 				following=following[user_id],
-				badges=iuser.badges,
 			)
 			for user_id, iuser in iusers.items()
 		}
 
 
 	async def scores(self: 'InternalPosts', client: _InternalClient, user: KhUser) -> Dict[PostId, Optional[Score]] :
 		"""
@@ -465,19 +460,19 @@
 
 
 	async def posts(self: 'InternalPosts', client: _InternalClient, user: KhUser) -> List[Post] :
 		"""
 		returns a list of external post objects populated with user and other information
 		"""
 
-		uploaders_task: Task[Dict[int, User]] = ensure_future(self.uploaders(client, user))
+		uploaders_task: Task[Dict[int, UserPortable]] = ensure_future(self.uploaders(client, user))
 		scores_task: Task[Dict[PostId, Optional[Score]]] = ensure_future(self.scores(client, user))
 
 		tags: Dict[PostId, List[str]] = await client.tags_many(list(map(lambda x : PostId(x.post_id), self.post_list)))
-		uploaders: Dict[int, User] = await uploaders_task
+		uploaders: Dict[int, UserPortable] = await uploaders_task
 		scores: Dict[PostId, Optional[Score]] = await scores_task
 
 		posts: List[Post] = []
 		for post in self.post_list :
 			post_id: PostId = PostId(post.post_id)
 			posts.append(Post(
 				post_id=post_id,
```

### Comparing `fuzzly-0.0.3/fuzzly/models/post.py` & `fuzzly-0.0.4/fuzzly/models/post.py`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.3/fuzzly/models/tag.py` & `fuzzly-0.0.4/fuzzly/models/tag.py`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.3/fuzzly.egg-info/PKG-INFO` & `fuzzly-0.0.4/fuzzly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: fuzzly
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fuzz.ly client library for Python3
 Home-page: https://github.com/kheina-com/fuzzly
 Author: kheina
 License: Mozilla Public License 2.0
-Requires-Python: >=3.9.*
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 	<img src="https://github.com/kheina-com/fuzzly/raw/main/logo.png" alt="fuzzly Logo">
 	<br>
 	<a href="https://github.com/kheina-com/fuzzly/actions?query=workflow%3Apython-package+event%3Apush+branch%3Amain">
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: fuzzly Version: 0.0.3 Summary: Fuzz.ly client
+Metadata-Version: 2.1 Name: fuzzly Version: 0.0.4 Summary: Fuzz.ly client
 library for Python3 Home-page: https://github.com/kheina-com/fuzzly Author:
-kheina License: Mozilla Public License 2.0 Requires-Python: >=3.9.*
-Description-Content-Type: text/markdown License-File: LICENSE
+kheina License: Mozilla Public License 2.0 Requires-Python: >=3.9 Description-
+Content-Type: text/markdown License-File: LICENSE
                                 [fuzzly Logo]
                [python-package_workflow] [pypi_package_version]
                       A python client library for fuzz.ly
 # Installation ```bash $ pip install fuzzly ``` # Usage ```python from fuzzly
 import FuzzlyClient from fuzzly.models.post import Post # if you have a bot
 token, make sure you initialize the client with your token token: str =
 'aGV5IG1hbi4gaXQncyB3ZWlyZCB0aGF0IHlvdSBsb29rZWQgYXQgdGhpcywgYnV0IHRoaXMgaXNuJ3QgYSByZWFsIHRva2Vu'
```

### Comparing `fuzzly-0.0.3/fuzzly.egg-info/SOURCES.txt` & `fuzzly-0.0.4/fuzzly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuzzly-0.0.3/setup.py` & `fuzzly-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 	description='Fuzz.ly client library for Python3',
 	long_description=open('readme.md').read(),
 	long_description_content_type='text/markdown',
 	author='kheina',
 	url='https://github.com/kheina-com/fuzzly',
 	packages=find_packages(exclude=['tests']),
 	install_requires=list(filter(None, map(str.strip, open('requirements.txt').read().split()))),
-	python_requires='>=3.9.*',
+	python_requires='>=3.9',
 	license='Mozilla Public License 2.0',
 )
```

