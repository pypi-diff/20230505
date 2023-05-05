# Comparing `tmp/proxycurl-py-0.0.20.tar.gz` & `tmp/proxycurl_py-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxycurl-py-0.0.20.tar", last modified: Thu Apr 27 06:07:33 2023, max compression
+gzip compressed data, was "proxycurl_py-0.0.21.tar", max compression
```

## Comparing `proxycurl-py-0.0.20.tar` & `proxycurl_py-0.0.21.tar`

### file list

```diff
@@ -1,29 +1,14 @@
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    12529 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/PKG-INFO
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    12288 2023-04-27 02:41:27.000000 proxycurl-py-0.0.20/README.md
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 06:07:33.848605 proxycurl-py-0.0.20/proxycurl_py/
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/proxycurl_py/asyncio/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2023-04-27 02:41:52.000000 proxycurl-py-0.0.20/proxycurl_py/asyncio/__init__.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4709 2023-04-27 02:41:27.000000 proxycurl-py-0.0.20/proxycurl_py/asyncio/base.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    72492 2023-04-27 02:41:52.000000 proxycurl-py-0.0.20/proxycurl_py/asyncio/library.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      283 2023-04-27 02:41:27.000000 proxycurl-py-0.0.20/proxycurl_py/config.py
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/proxycurl_py/gevent/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2023-04-27 02:41:52.000000 proxycurl-py-0.0.20/proxycurl_py/gevent/__init__.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4171 2023-04-27 02:41:27.000000 proxycurl-py-0.0.20/proxycurl_py/gevent/base.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    70856 2023-04-27 02:41:52.000000 proxycurl-py-0.0.20/proxycurl_py/gevent/library.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    14796 2023-04-27 02:41:52.000000 proxycurl-py-0.0.20/proxycurl_py/models.py
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/proxycurl_py/twisted/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2023-04-27 02:41:52.000000 proxycurl-py-0.0.20/proxycurl_py/twisted/__init__.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4995 2023-04-27 02:41:27.000000 proxycurl-py-0.0.20/proxycurl_py/twisted/base.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    70542 2023-04-27 02:41:52.000000 proxycurl-py-0.0.20/proxycurl_py/twisted/library.py
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/proxycurl_py.egg-info/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    12529 2023-04-27 06:07:33.000000 proxycurl-py-0.0.20/proxycurl_py.egg-info/PKG-INFO
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      583 2023-04-27 06:07:33.000000 proxycurl-py-0.0.20/proxycurl_py.egg-info/SOURCES.txt
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)        1 2023-04-27 06:07:33.000000 proxycurl-py-0.0.20/proxycurl_py.egg-info/dependency_links.txt
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      168 2023-04-27 06:07:33.000000 proxycurl-py-0.0.20/proxycurl_py.egg-info/requires.txt
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       13 2023-04-27 06:07:33.000000 proxycurl-py-0.0.20/proxycurl_py.egg-info/top_level.txt
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      772 2023-04-27 06:06:45.000000 proxycurl-py-0.0.20/pyproject.toml
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       38 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/setup.cfg
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      985 2023-04-27 06:06:52.000000 proxycurl-py-0.0.20/setup.py
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 06:07:33.852604 proxycurl-py-0.0.20/tests/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       80 2023-04-27 02:41:27.000000 proxycurl-py-0.0.20/tests/test_proxycurl.py
+-rw-r--r--   0        0        0    12288 2023-04-28 09:34:40.817506 proxycurl_py-0.0.21/README.md
+-rw-r--r--   0        0        0       56 2023-05-04 05:21:19.908702 proxycurl_py-0.0.21/proxycurl_py/asyncio/__init__.py
+-rw-r--r--   0        0        0     4709 2023-04-28 09:34:40.820420 proxycurl_py-0.0.21/proxycurl_py/asyncio/base.py
+-rw-r--r--   0        0        0    76763 2023-05-04 05:22:51.225402 proxycurl_py-0.0.21/proxycurl_py/asyncio/library.py
+-rw-r--r--   0        0        0      283 2023-04-28 09:34:40.820503 proxycurl_py-0.0.21/proxycurl_py/config.py
+-rw-r--r--   0        0        0       56 2023-05-04 05:21:19.866110 proxycurl_py-0.0.21/proxycurl_py/gevent/__init__.py
+-rw-r--r--   0        0        0     4171 2023-04-28 09:34:40.820623 proxycurl_py-0.0.21/proxycurl_py/gevent/base.py
+-rw-r--r--   0        0        0    71316 2023-05-04 05:21:19.887379 proxycurl_py-0.0.21/proxycurl_py/gevent/library.py
+-rw-r--r--   0        0        0    14796 2023-05-04 05:21:19.865323 proxycurl_py-0.0.21/proxycurl_py/models.py
+-rw-r--r--   0        0        0       56 2023-05-04 05:21:19.888053 proxycurl_py-0.0.21/proxycurl_py/twisted/__init__.py
+-rw-r--r--   0        0        0     4995 2023-04-28 09:34:40.820764 proxycurl_py-0.0.21/proxycurl_py/twisted/base.py
+-rw-r--r--   0        0        0    71002 2023-05-04 05:21:19.908118 proxycurl_py-0.0.21/proxycurl_py/twisted/library.py
+-rw-r--r--   0        0        0      772 2023-05-04 09:36:44.013150 proxycurl_py-0.0.21/pyproject.toml
+-rw-r--r--   0        0        0    13208 1970-01-01 00:00:00.000000 proxycurl_py-0.0.21/PKG-INFO
```

### Comparing `proxycurl-py-0.0.20/PKG-INFO` & `proxycurl_py-0.0.21/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: proxycurl-py
-Version: 0.0.20
-Author: Nubela
-Author-email: tech@nubela.co
-Requires-Python: >=3.7,<4.0
-Description-Content-Type: text/markdown
-Provides-Extra: asyncio
-Provides-Extra: gevent
-Provides-Extra: twisted
-
 # `proxycurl-py` -  The official Python client for Proxycurl API to scrape and enrich LinkedIn profiles
 
 * [What is Proxycurl?](#what-is-proxycurl-)
 * [Before you install](#before-you-install)
 * [Installation and supported Python versions](#installation-and-supported-python-versions)
 * [Initializing `proxycurl-py` with an API Key](#initializing--proxycurl-py--with-an-api-key)
 * [Usage with examples](#usage-with-examples)
```

### Comparing `proxycurl-py-0.0.20/README.md` & `proxycurl_py-0.0.21/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: proxycurl-py
+Version: 0.0.21
+Summary: 
+Author: Nubela
+Author-email: tech@nubela.co
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: asyncio
+Provides-Extra: gevent
+Provides-Extra: twisted
+Requires-Dist: Twisted (>=21.7.0,<22.0.0) ; extra == "twisted"
+Requires-Dist: aiohttp (>=3.7.4,<4.0.0) ; extra == "asyncio"
+Requires-Dist: asyncio (>=3.4.3,<4.0.0) ; extra == "asyncio"
+Requires-Dist: gevent (>=21.1.1,<22.0.0) ; extra == "gevent"
+Requires-Dist: requests (>=2.25.0,<3.0.0) ; extra == "gevent"
+Requires-Dist: treq (>=21.5.0,<22.0.0) ; extra == "twisted"
+Description-Content-Type: text/markdown
+
 # `proxycurl-py` -  The official Python client for Proxycurl API to scrape and enrich LinkedIn profiles
 
 * [What is Proxycurl?](#what-is-proxycurl-)
 * [Before you install](#before-you-install)
 * [Installation and supported Python versions](#installation-and-supported-python-versions)
 * [Initializing `proxycurl-py` with an API Key](#initializing--proxycurl-py--with-an-api-key)
 * [Usage with examples](#usage-with-examples)
@@ -178,7 +202,8 @@
 | `linkedin.job.get(**kwargs)`                 | [Jobs Profile Endpoint](https://nubela.co/proxycurl/docs#jobs-api-job-profile-endpoint)                                         | [Jobs API](https://nubela.co/proxycurl/docs#jobs-api)       |
 | `linkedin.person.resolve(**kwargs)`          | [Person Lookup Endpoint](https://nubela.co/proxycurl/docs#people-api-person-lookup-endpoint)                                    | [People API](https://nubela.co/proxycurl/docs#people-api)   |
 | `linkedin.company.role_lookup(**kwargs)`     | [Role Lookup Endpoint](https://nubela.co/proxycurl/docs#people-api-role-lookup-endpoint)                                        | [People API](https://nubela.co/proxycurl/docs#people-api)   |
 | `linkedin.person.get(**kwargs)`              | [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint)                                  | [People API](https://nubela.co/proxycurl/docs#people-api)   |
 | `linkedin.school.get(**kwargs)`              | [School Profile Endpoint](https://nubela.co/proxycurl/docs#school-api-school-profile-endpoint)                                  | [School API](https://nubela.co/proxycurl/docs#school-api)   |
 | `linkedin.company.reveal`                    | [Reveal Endpoint](https://nubela.co/proxycurl/docs#reveal-api-reveal-endpoint)                                                  | [Reveal API](https://nubela.co/proxycurl/docs#reveal-api)   |
 | `get_balance(**kwargs)`                      | [View Credit Balance Endpoint](https://nubela.co/proxycurl/docs#meta-api-view-credit-balance-endpoint)                          | [Meta API](https://nubela.co/proxycurl/docs#meta-api)       |
+
```

### Comparing `proxycurl-py-0.0.20/proxycurl_py/asyncio/base.py` & `proxycurl_py-0.0.21/proxycurl_py/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.20/proxycurl_py/asyncio/library.py` & `proxycurl_py-0.0.21/proxycurl_py/gevent/library.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-from typing import (
-    Awaitable,
-    Optional
-)
 from proxycurl_py.config import (
     BASE_URL, PROXYCURL_API_KEY, TIMEOUT, MAX_RETRIES, MAX_BACKOFF_SECONDS
 )
-from proxycurl_py.asyncio.base import ProxycurlBase
+from proxycurl_py.gevent.base import ProxycurlBase
 from proxycurl_py.models import (
     PersonEndpointResponse,
     PersonLookupUrlEnrichResult,
     ReverseEmailUrlEnrichResult,
     ExtractionEmailResult,
     PDLPhoneNumberResult,
     PDLEmailResult,
@@ -30,198 +26,196 @@
 )
 
 
 class _LinkedinPerson:
     def __init__(self, linkedin):
         self.linkedin = linkedin
 
-    async def get(
+    def get(
         self,
-        extra: str,
-        github_profile_id: str,
-        facebook_profile_id: str,
-        twitter_profile_id: str,
-        personal_contact_number: str,
-        personal_email: str,
-        inferred_salary: str,
-        skills: str,
-        use_cache: str,
         fallback_to_cache: str,
         url: str,
-    ) -> Awaitable[PersonEndpointResponse]:
+        use_cache: str = '',
+        skills: str = '',
+        inferred_salary: str = '',
+        personal_email: str = '',
+        personal_contact_number: str = '',
+        twitter_profile_id: str = '',
+        facebook_profile_id: str = '',
+        github_profile_id: str = '',
+        extra: str = '',
+    ) -> PersonEndpointResponse:
         """Person Profile Endpoint
         
                 Cost: 1 credit / successful request.
         Get structured data of a Personal Profile
         
-        :param extra: Enriches the Person Profile with extra details from external sources.
-            Extra details include gender, birth date, industry and interests.
+        :param fallback_to_cache: Tweaks the fallback behavior if an error arises from fetching a fresh profile.
 
             This parameter accepts the following values:
-            - `exclude` (default value) - Does not provide extra data field.
-            - `include` - Append extra data to the person profile object.
-            Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
-        :type extra: str
-        :param github_profile_id: Enriches the Person Profile with Github Id from external sources.
+            * `on-error` (default value) - Fallback to reading the profile from cache if an error arises.
+            * `never` - Do not ever read profile from cache.
+        :type fallback_to_cache: str
+        :param url: URL of the LinkedIn Profile to crawl.
+
+            URL should be in the format of `https://www.linkedin.com/in/<public-identifier>`
+        :type url: str
+        :param use_cache: `if-present` The default behavior. Fetches profile from cache regardless of age of profile. If profile is not available in cache, API will attempt to source profile externally.
+
+            `if-recent` API will make a best effort to return a fresh profile no older than 29 days.Costs an extra `1` credit on top of the cost of the base endpoint.
+        :type use_cache: str
+        :param skills: Include skills data from external sources.
 
             This parameter accepts the following values:
-            - `exclude` (default value) - Does not provide Github Id data field.
-            - `include` - Append Github Id data to the person profile object.
+            - `exclude` (default value) - Does not provide skills data field.
+            - `include` - Append skills data to the person profile object.
             Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
-        :type github_profile_id: str
-        :param facebook_profile_id: Enriches the Person Profile with Facebook Id from external sources.
+        :type skills: str
+        :param inferred_salary: Include inferred salary range from external sources.
 
             This parameter accepts the following values:
-            - `exclude` (default value) - Does not provide Facebook Id data field.
-            - `include` - Append Facebook Id data to the person profile object.
+            - `exclude` (default value) - Does not provide inferred salary data field.
+            - `include` - Append inferred salary range data to the person profile object.
             Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
-        :type facebook_profile_id: str
-        :param twitter_profile_id: Enriches the Person Profile with Twitter Id from external sources.
+        :type inferred_salary: str
+        :param personal_email: Enriches the Person Profile with personal emails from external sources.
 
             This parameter accepts the following values:
-            - `exclude` (default value) - Does not provide Twitter Id data field.
-            - `include` - Append Twitter Id data to the person profile object.
-            Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
-        :type twitter_profile_id: str
+            - `exclude` (default value) - Does not provide personal emails data field.
+            - `include` - Append personal emails data to the person profile object.
+            Costs an extra `1` credit per email returned on top of the cost of the base endpoint (if data is available).
+        :type personal_email: str
         :param personal_contact_number: Enriches the Person Profile with personal numbers from external sources.
 
             This parameter accepts the following values:
             - `exclude` (default value) - Does not provide personal numbers data field.
             - `include` - Append personal numbers data to the person profile object.
             Costs an extra `1` credit per email returned on top of the cost of the base endpoint (if data is available).
         :type personal_contact_number: str
-        :param personal_email: Enriches the Person Profile with personal emails from external sources.
+        :param twitter_profile_id: Enriches the Person Profile with Twitter Id from external sources.
 
             This parameter accepts the following values:
-            - `exclude` (default value) - Does not provide personal emails data field.
-            - `include` - Append personal emails data to the person profile object.
-            Costs an extra `1` credit per email returned on top of the cost of the base endpoint (if data is available).
-        :type personal_email: str
-        :param inferred_salary: Include inferred salary range from external sources.
+            - `exclude` (default value) - Does not provide Twitter Id data field.
+            - `include` - Append Twitter Id data to the person profile object.
+            Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
+        :type twitter_profile_id: str
+        :param facebook_profile_id: Enriches the Person Profile with Facebook Id from external sources.
 
             This parameter accepts the following values:
-            - `exclude` (default value) - Does not provide inferred salary data field.
-            - `include` - Append inferred salary range data to the person profile object.
+            - `exclude` (default value) - Does not provide Facebook Id data field.
+            - `include` - Append Facebook Id data to the person profile object.
             Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
-        :type inferred_salary: str
-        :param skills: Include skills data from external sources.
+        :type facebook_profile_id: str
+        :param github_profile_id: Enriches the Person Profile with Github Id from external sources.
 
             This parameter accepts the following values:
-            - `exclude` (default value) - Does not provide skills data field.
-            - `include` - Append skills data to the person profile object.
+            - `exclude` (default value) - Does not provide Github Id data field.
+            - `include` - Append Github Id data to the person profile object.
             Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
-        :type skills: str
-        :param use_cache: `if-present` The default behavior. Fetches profile from cache regardless of age of profile. If profile is not available in cache, API will attempt to source profile externally.
-
-            `if-recent` API will make a best effort to return a fresh profile no older than 29 days.Costs an extra `1` credit on top of the cost of the base endpoint.
-        :type use_cache: str
-        :param fallback_to_cache: Tweaks the fallback behavior if an error arises from fetching a fresh profile.
+        :type github_profile_id: str
+        :param extra: Enriches the Person Profile with extra details from external sources.
+            Extra details include gender, birth date, industry and interests.
 
             This parameter accepts the following values:
-            * `on-error` (default value) - Fallback to reading the profile from cache if an error arises.
-            * `never` - Do not ever read profile from cache.
-        :type fallback_to_cache: str
-        :param url: URL of the LinkedIn Profile to crawl.
-
-            URL should be in the format of `https://www.linkedin.com/in/<public-identifier>`
-        :type url: str
-        :return: An object of Awaitable[:class:`proxycurl.models.PersonEndpointResponse]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.PersonEndpointResponse]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+            - `exclude` (default value) - Does not provide extra data field.
+            - `include` - Append extra data to the person profile object.
+            Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
+        :type extra: str
+        :return: An object of :class:`proxycurl.models.PersonEndpointResponse` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.PersonEndpointResponse`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/v2/linkedin',
             params={
-                'extra': extra,
-                'github_profile_id': github_profile_id,
-                'facebook_profile_id': facebook_profile_id,
-                'twitter_profile_id': twitter_profile_id,
-                'personal_contact_number': personal_contact_number,
-                'personal_email': personal_email,
-                'inferred_salary': inferred_salary,
-                'skills': skills,
-                'use_cache': use_cache,
                 'fallback_to_cache': fallback_to_cache,
                 'url': url,
+                'use_cache': use_cache,
+                'skills': skills,
+                'inferred_salary': inferred_salary,
+                'personal_email': personal_email,
+                'personal_contact_number': personal_contact_number,
+                'twitter_profile_id': twitter_profile_id,
+                'facebook_profile_id': facebook_profile_id,
+                'github_profile_id': github_profile_id,
+                'extra': extra,
             },
             data={
             },
             result_class=PersonEndpointResponse
         )
-        return resp
 
-    async def resolve(
+    def resolve(
         self,
         first_name: str,
-        last_name: str,
-        title: str,
-        location: str,
         company_domain: str,
-        enrich_profile: str,
-    ) -> Awaitable[PersonLookupUrlEnrichResult]:
+        enrich_profile: str = '',
+        location: str = '',
+        title: str = '',
+        last_name: str = '',
+    ) -> PersonLookupUrlEnrichResult:
         """Person Lookup Endpoint
         
                 Cost: 2 credits / successful request.
         Look up a person with a name and company information.
         
         :param first_name: First name of the user
         :type first_name: str
-        :param last_name: Last name of the user
-        :type last_name: str
-        :param title: Title that user is holding at his/her current job
-        :type title: str
-        :param location: The location of this user.
-
-            Name of country, city or state.
-        :type location: str
         :param company_domain: Company name or domain
         :type company_domain: str
         :param enrich_profile: Enrich the result with a cached profile of the lookup result.
 
             The valid values are:
 
             * `skip` (default): do not enrich the results with cached profile data
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
             please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
-        :return: An object of Awaitable[:class:`proxycurl.models.PersonLookupUrlEnrichResult]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.PersonLookupUrlEnrichResult]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :param location: The location of this user.
+
+            Name of country, city or state.
+        :type location: str
+        :param title: Title that user is holding at his/her current job
+        :type title: str
+        :param last_name: Last name of the user
+        :type last_name: str
+        :return: An object of :class:`proxycurl.models.PersonLookupUrlEnrichResult` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.PersonLookupUrlEnrichResult`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/profile/resolve',
             params={
                 'first_name': first_name,
-                'last_name': last_name,
-                'title': title,
-                'location': location,
                 'company_domain': company_domain,
                 'enrich_profile': enrich_profile,
+                'location': location,
+                'title': title,
+                'last_name': last_name,
             },
             data={
             },
             result_class=PersonLookupUrlEnrichResult
         )
-        return resp
 
-    async def resolve_by_email(
+    def resolve_by_email(
         self,
         work_email: str,
-        enrich_profile: str,
-    ) -> Awaitable[ReverseEmailUrlEnrichResult]:
+        enrich_profile: str = '',
+    ) -> ReverseEmailUrlEnrichResult:
         """Reverse Work Email Lookup Endpoint
         
                 Cost: 3 credits / successful request.
         Resolve LinkedIn Profile from a work email address
         
         :param work_email: Work email address of the user
         :type work_email: str
@@ -233,38 +227,37 @@
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
             please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
-        :return: An object of Awaitable[:class:`proxycurl.models.ReverseEmailUrlEnrichResult]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.ReverseEmailUrlEnrichResult]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :return: An object of :class:`proxycurl.models.ReverseEmailUrlEnrichResult` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.ReverseEmailUrlEnrichResult`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/profile/resolve/email',
             params={
                 'work_email': work_email,
                 'enrich_profile': enrich_profile,
             },
             data={
             },
             result_class=ReverseEmailUrlEnrichResult
         )
-        return resp
 
-    async def lookup_email(
+    def lookup_email(
         self,
-        callback_url: str,
         linkedin_profile_url: str,
-    ) -> Awaitable[ExtractionEmailResult]:
+        callback_url: str = '',
+    ) -> ExtractionEmailResult:
         """Work Email Lookup Endpoint
         
                 Cost: 3 credits / request.
         Lookup work email address of a LinkedIn Person Profile.
 
         Email addresses returned are verified to not be role-based or catch-all emails. Email addresses
         returned by our API endpoint come with a 95+% deliverability guarantee
@@ -272,777 +265,766 @@
         **Endpoint behavior**
 
         *This endpoint* **_may not_** *return results immediately.*
 
         If you provided a webhook in your request parameter, our application will call your webhook with
         the result once. See `Webhook request` below.
         
-        :param callback_url: Webhook to notify your application when
-            the request has finished processing.
-        :type callback_url: str
         :param linkedin_profile_url: Linkedin Profile URL of the person you want to
             extract work email address from.
         :type linkedin_profile_url: str
-        :return: An object of Awaitable[:class:`proxycurl.models.ExtractionEmailResult]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.ExtractionEmailResult]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :param callback_url: Webhook to notify your application when
+            the request has finished processing.
+        :type callback_url: str
+        :return: An object of :class:`proxycurl.models.ExtractionEmailResult` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.ExtractionEmailResult`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/profile/email',
             params={
-                'callback_url': callback_url,
                 'linkedin_profile_url': linkedin_profile_url,
+                'callback_url': callback_url,
             },
             data={
             },
             result_class=ExtractionEmailResult
         )
-        return resp
 
-    async def personal_contact(
+    def personal_contact(
         self,
         linkedin_profile_url: str,
-    ) -> Awaitable[PDLPhoneNumberResult]:
+    ) -> PDLPhoneNumberResult:
         """Personal Contact Number Lookup Endpoint
         
                 Cost: 1 credit / contact number returned.
         Given an LinkedIn profile, returns a list of personal contact numbers belonging to this identity.
         
         :param linkedin_profile_url: LinkedIn Profile URL of the person you want to extract personal contact numbers from.
         :type linkedin_profile_url: str
-        :return: An object of Awaitable[:class:`proxycurl.models.PDLPhoneNumberResult]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.PDLPhoneNumberResult]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :return: An object of :class:`proxycurl.models.PDLPhoneNumberResult` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.PDLPhoneNumberResult`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/contact-api/personal-contact',
             params={
                 'linkedin_profile_url': linkedin_profile_url,
             },
             data={
             },
             result_class=PDLPhoneNumberResult
         )
-        return resp
 
-    async def personal_email(
+    def personal_email(
         self,
         linkedin_profile_url: str,
-        email_validation: str,
-    ) -> Awaitable[PDLEmailResult]:
+        email_validation: str = '',
+    ) -> PDLEmailResult:
         """Personal Email Lookup Endpoint
         
                 Cost: 1 credit / email returned.
         Given an LinkedIn profile, returns a list of personal emails belonging to this identity. Emails are verified to be deliverable.
         
         :param linkedin_profile_url: LinkedIn Profile URL of the person you want to extract personal email addresses from.
         :type linkedin_profile_url: str
         :param email_validation: Perform deliverability validation on each email. (Costs 1 extra credit per email found).
 
             Takes the following values:
              * include - Perform email validation.
              * exclude (default) - Do not perform email validation.
         :type email_validation: str
-        :return: An object of Awaitable[:class:`proxycurl.models.PDLEmailResult]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.PDLEmailResult]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :return: An object of :class:`proxycurl.models.PDLEmailResult` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.PDLEmailResult`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/contact-api/personal-email',
             params={
                 'linkedin_profile_url': linkedin_profile_url,
                 'email_validation': email_validation,
             },
             data={
             },
             result_class=PDLEmailResult
         )
-        return resp
 
-    async def profile_picture(
+    def profile_picture(
         self,
         linkedin_person_profile_url: str,
-    ) -> Awaitable[ProfilePicture]:
+    ) -> ProfilePicture:
         """Person Profile Picture Endpoint
         
                 Cost: 0 credit / successful request.
         Get the profile picture of a person.
 
         Profile pictures are served from cached people profiles found within [LinkDB](https://nubela.co/proxycurl/linkdb).
         If the profile does not exist within [LinkDB](https://nubela.co/proxycurl/linkdb), then the API will return a `404` status code.
         
         :param linkedin_person_profile_url: LinkedIn Profile URL of the person that you are trying to get the profile picture of.
         :type linkedin_person_profile_url: str
-        :return: An object of Awaitable[:class:`proxycurl.models.ProfilePicture]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.ProfilePicture]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :return: An object of :class:`proxycurl.models.ProfilePicture` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.ProfilePicture`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/person/profile-picture',
             params={
                 'linkedin_person_profile_url': linkedin_person_profile_url,
             },
             data={
             },
             result_class=ProfilePicture
         )
-        return resp
 
-    async def person_search(
+    def person_search(
         self,
-        first_name: str,
-        last_name: str,
-        follower_count_min: str,
-        follower_count_max: str,
-        occupation: str,
-        headline: str,
-        summary: str,
-        country: str,
-        country_full_name: str,
-        city: str,
-        state: str,
-        connections_min: str,
-        connections_max: str,
-        birth_date_after: str,
-        birth_date_before: str,
-        page_size: str,
-        enrich_profiles: str,
-    ) -> Awaitable[PersonSearchResult]:
+        enrich_profiles: str = '',
+        page_size: str = '',
+        birth_date_before: str = '',
+        birth_date_after: str = '',
+        connections_max: str = '',
+        connections_min: str = '',
+        state: str = '',
+        city: str = '',
+        country_full_name: str = '',
+        country: str = '',
+        summary: str = '',
+        headline: str = '',
+        occupation: str = '',
+        follower_count_max: str = '',
+        follower_count_min: str = '',
+        last_name: str = '',
+        first_name: str = '',
+    ) -> PersonSearchResult:
         """Person Search Endpoint
         
                 Cost: 35 credits / request.
         Search for people that meet a set of criteria within our exhaustive dataset of people profiles.
 
         This API endpoint is powered by [LinkDB](https://nubela.co/proxycurl/linkdb), our exhaustive dataset of people and company profiles.
         
-        :param first_name: Filter people by their first names by matching it against a regular expression.
+        :param enrich_profiles: Get the full profile data of people returned instead of only their LinkedIn profile URLs.
 
-            The default value of this parameter is `null`.
+            Each request respond with a streaming response of profiles.
 
-            The accepted value is a regular expression (regex).
-        :type first_name: str
-        :param last_name: Filter people by their last names by matching it against a regular expression.
+            The valid values are:
+
+            * `skip` (default): lists employee's profile url
+            * `enrich`: lists full profile of employees
+
+            Calling this API endpoint with this parameter would add `1` credit per result returned.
+        :type enrich_profiles: str
+        :param page_size: Tune the maximum results returned per API call.
+
+            The default value of this parameter is `100`.
+
+            Accepted values for this parameter is an integer ranging from `1` to `100`.
+        :type page_size: str
+        :param birth_date_before: Filter people with a birth date *less than* a value given in this parameter.
 
             The default value of this parameter is `null`.
+        :type birth_date_before: str
+        :param birth_date_after: Filter people with a birth date *more than* a value given in this parameter.
 
-            The accepted value is a regular expression (regex).
-        :type last_name: str
-        :param follower_count_min: Filter people with a LinkedIn follower count *more than* a value given in this parameter.
+            The default value of this parameter is `null`.
+        :type birth_date_after: str
+        :param connections_max: Filter people with a LinkedIn connection count *less than* a value given in this parameter.
 
             The default value of this parameter is `null`.
-        :type follower_count_min: str
-        :param follower_count_max: Filter people with a LinkedIn follower count *less than* a value given in this parameter.
+        :type connections_max: str
+        :param connections_min: Filter people with a LinkedIn connection count *more than* a value given in this parameter.
 
             The default value of this parameter is `null`.
-        :type follower_count_max: str
-        :param occupation: Filter people by their occupations by matching it against a regular expression.
+        :type connections_min: str
+        :param state: Filter people by their states by matching it against a regular expression.
 
             The default value of this parameter is `null`.
 
             The accepted value is a regular expression (regex).
-        :type occupation: str
-        :param headline: Filter people by their headlines by matching it against a regular expression.
+        :type state: str
+        :param city: Filter people by their cities by matching it against a regular expression.
 
             The default value of this parameter is `null`.
 
             The accepted value is a regular expression (regex).
-        :type headline: str
-        :param summary: Filter people by their summaries by matching it against a regular expression.
+        :type city: str
+        :param country_full_name: Filter people by their countries (in English words) by matching it against a regular expression.
 
             The default value of this parameter is `null`.
 
             The accepted value is a regular expression (regex).
-        :type summary: str
+        :type country_full_name: str
         :param country: Filter people by their countries (depicted by a 2-letter country code (ISO 3166-1 alpha-2)) by matching it against a regular expression.
 
             The default value of this parameter is `null`.
 
             The accepted value is a regular expression (regex).
         :type country: str
-        :param country_full_name: Filter people by their countries (in English words) by matching it against a regular expression.
+        :param summary: Filter people by their summaries by matching it against a regular expression.
 
             The default value of this parameter is `null`.
 
             The accepted value is a regular expression (regex).
-        :type country_full_name: str
-        :param city: Filter people by their cities by matching it against a regular expression.
+        :type summary: str
+        :param headline: Filter people by their headlines by matching it against a regular expression.
 
             The default value of this parameter is `null`.
 
             The accepted value is a regular expression (regex).
-        :type city: str
-        :param state: Filter people by their states by matching it against a regular expression.
+        :type headline: str
+        :param occupation: Filter people by their occupations by matching it against a regular expression.
 
             The default value of this parameter is `null`.
 
             The accepted value is a regular expression (regex).
-        :type state: str
-        :param connections_min: Filter people with a LinkedIn connection count *more than* a value given in this parameter.
-
-            The default value of this parameter is `null`.
-        :type connections_min: str
-        :param connections_max: Filter people with a LinkedIn connection count *less than* a value given in this parameter.
+        :type occupation: str
+        :param follower_count_max: Filter people with a LinkedIn follower count *less than* a value given in this parameter.
 
             The default value of this parameter is `null`.
-        :type connections_max: str
-        :param birth_date_after: Filter people with a birth date *more than* a value given in this parameter.
+        :type follower_count_max: str
+        :param follower_count_min: Filter people with a LinkedIn follower count *more than* a value given in this parameter.
 
             The default value of this parameter is `null`.
-        :type birth_date_after: str
-        :param birth_date_before: Filter people with a birth date *less than* a value given in this parameter.
+        :type follower_count_min: str
+        :param last_name: Filter people by their last names by matching it against a regular expression.
 
             The default value of this parameter is `null`.
-        :type birth_date_before: str
-        :param page_size: Tune the maximum results returned per API call.
-
-            The default value of this parameter is `100`.
-
-            Accepted values for this parameter is an integer ranging from `1` to `100`.
-        :type page_size: str
-        :param enrich_profiles: Get the full profile data of people returned instead of only their LinkedIn profile URLs.
-
-            Each request respond with a streaming response of profiles.
 
-            The valid values are:
+            The accepted value is a regular expression (regex).
+        :type last_name: str
+        :param first_name: Filter people by their first names by matching it against a regular expression.
 
-            * `skip` (default): lists employee's profile url
-            * `enrich`: lists full profile of employees
+            The default value of this parameter is `null`.
 
-            Calling this API endpoint with this parameter would add `1` credit per result returned.
-        :type enrich_profiles: str
-        :return: An object of Awaitable[:class:`proxycurl.models.PersonSearchResult]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.PersonSearchResult]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+            The accepted value is a regular expression (regex).
+        :type first_name: str
+        :return: An object of :class:`proxycurl.models.PersonSearchResult` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.PersonSearchResult`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/search/person',
             params={
-                'first_name': first_name,
-                'last_name': last_name,
-                'follower_count_min': follower_count_min,
-                'follower_count_max': follower_count_max,
-                'occupation': occupation,
-                'headline': headline,
-                'summary': summary,
-                'country': country,
-                'country_full_name': country_full_name,
-                'city': city,
-                'state': state,
-                'connections_min': connections_min,
-                'connections_max': connections_max,
-                'birth_date_after': birth_date_after,
-                'birth_date_before': birth_date_before,
-                'page_size': page_size,
                 'enrich_profiles': enrich_profiles,
+                'page_size': page_size,
+                'birth_date_before': birth_date_before,
+                'birth_date_after': birth_date_after,
+                'connections_max': connections_max,
+                'connections_min': connections_min,
+                'state': state,
+                'city': city,
+                'country_full_name': country_full_name,
+                'country': country,
+                'summary': summary,
+                'headline': headline,
+                'occupation': occupation,
+                'follower_count_max': follower_count_max,
+                'follower_count_min': follower_count_min,
+                'last_name': last_name,
+                'first_name': first_name,
             },
             data={
             },
             result_class=PersonSearchResult
         )
-        return resp
 
 
 class _LinkedinCompany:
     def __init__(self, linkedin):
         self.linkedin = linkedin
 
-    async def get(
+    def get(
         self,
-        use_cache: str,
         url: str,
-        acquisitions: str,
-        exit_data: str,
-        extra: str,
-        funding_data: str,
-        categories: str,
-        resolve_numeric_id: str,
-    ) -> Awaitable[LinkedinCompany]:
+        resolve_numeric_id: str = '',
+        categories: str = '',
+        funding_data: str = '',
+        extra: str = '',
+        exit_data: str = '',
+        acquisitions: str = '',
+        use_cache: str = '',
+    ) -> LinkedinCompany:
         """Company Profile Endpoint
         
                 Cost: 1 credit / successful request.
         Get structured data of a Company Profile
         
-        :param use_cache: `if-present` The default behavior. Fetches profile from cache regardless of age of profile. If profile is not available in cache, API will attempt to source profile externally.
-
-            `if-recent` API will make a best effort to return a fresh profile no older than 29 days.Costs an extra `1` credit on top of the cost of the base endpoint.
-        :type use_cache: str
         :param url: URL of the LinkedIn Company Profile to crawl.
 
             URL should be in the format of `https://www.linkedin.com/company/<public_identifier>`
         :type url: str
-        :param acquisitions: Provides further enriched data on acquisitions made by this company from external sources.
+        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator.
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb).
+            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
+
+            This parameter accepts the following values:
+            - `false` (default value) - Will not resolve numerical IDs.
+            - `true` - Enable support for Company Profile URLs with numerical IDs.
+            Costs an extra `2` credit on top of the base cost of the endpoint.
+        :type resolve_numeric_id: str
+        :param categories: Appends categories data of this company.
 
             Default value is `"exclude"`.
-            The other acceptable value is `"include"`, which will include these acquisition data (if available) for `1` extra credit.
-        :type acquisitions: str
-        :param exit_data: Returns a list of investment portfolio exits.
+            The other acceptable value is `"include"`, which will include these categories (if available) for `1` extra credit.
+        :type categories: str
+        :param funding_data: Returns a list of funding rounds that this company has received.
 
             Default value is `"exclude"`.
             The other acceptable value is `"include"`, which will include these categories (if available) for `1` extra credit.
-        :type exit_data: str
+        :type funding_data: str
         :param extra: Enriches the Company Profile with extra details from external sources.
             Details include Crunchbase ranking, contact email, phone number, Facebook account, Twitter account, funding rounds and amount, IPO status, investor information, etc.
 
             Default value is `"exclude"`.
             The other acceptable value is `"include"`, which will include these extra details (if available) for `1` extra credit.
         :type extra: str
-        :param funding_data: Returns a list of funding rounds that this company has received.
+        :param exit_data: Returns a list of investment portfolio exits.
 
             Default value is `"exclude"`.
             The other acceptable value is `"include"`, which will include these categories (if available) for `1` extra credit.
-        :type funding_data: str
-        :param categories: Appends categories data of this company.
+        :type exit_data: str
+        :param acquisitions: Provides further enriched data on acquisitions made by this company from external sources.
 
             Default value is `"exclude"`.
-            The other acceptable value is `"include"`, which will include these categories (if available) for `1` extra credit.
-        :type categories: str
-        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator.
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb).
-            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
+            The other acceptable value is `"include"`, which will include these acquisition data (if available) for `1` extra credit.
+        :type acquisitions: str
+        :param use_cache: `if-present` The default behavior. Fetches profile from cache regardless of age of profile. If profile is not available in cache, API will attempt to source profile externally.
 
-            This parameter accepts the following values:
-            - `false` (default value) - Will not resolve numerical IDs.
-            - `true` - Enable support for Company Profile URLs with numerical IDs.
-            Costs an extra `2` credit on top of the base cost of the endpoint.
-        :type resolve_numeric_id: str
-        :return: An object of Awaitable[:class:`proxycurl.models.LinkedinCompany]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.LinkedinCompany]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+            `if-recent` API will make a best effort to return a fresh profile no older than 29 days.Costs an extra `1` credit on top of the cost of the base endpoint.
+        :type use_cache: str
+        :return: An object of :class:`proxycurl.models.LinkedinCompany` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.LinkedinCompany`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/company',
             params={
-                'use_cache': use_cache,
                 'url': url,
-                'acquisitions': acquisitions,
-                'exit_data': exit_data,
-                'extra': extra,
-                'funding_data': funding_data,
-                'categories': categories,
                 'resolve_numeric_id': resolve_numeric_id,
+                'categories': categories,
+                'funding_data': funding_data,
+                'extra': extra,
+                'exit_data': exit_data,
+                'acquisitions': acquisitions,
+                'use_cache': use_cache,
             },
             data={
             },
             result_class=LinkedinCompany
         )
-        return resp
 
-    async def resolve(
+    def resolve(
         self,
-        enrich_profile: str,
-        company_name: str,
-        company_domain: str,
-        company_location: str,
-    ) -> Awaitable[CompanyUrlEnrichResult]:
+        company_location: str = '',
+        company_domain: str = '',
+        company_name: str = '',
+        enrich_profile: str = '',
+    ) -> CompanyUrlEnrichResult:
         """Company Lookup Endpoint
         
                 Cost: 2 credits / successful request.
         Resolve Company LinkedIn Profile from company name,
             domain name and location.
         
+        :param company_location: The location / region of company.
+            ISO 3166-1 alpha-2 codes
+        :type company_location: str
+        :param company_domain: Company website or Company domain
+            Requires either `company_domain` or `company_name`
+        :type company_domain: str
+        :param company_name: Company Name
+            Requires either `company_domain` or `company_name`
+        :type company_name: str
         :param enrich_profile: Enrich the result with a cached profile of the lookup result.
 
             The valid values are:
 
             * `skip` (default): do not enrich the results with cached profile data
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
             please chain this API call with the [Company Profile Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
-        :param company_name: Company Name
-            Requires either `company_domain` or `company_name`
-        :type company_name: str
-        :param company_domain: Company website or Company domain
-            Requires either `company_domain` or `company_name`
-        :type company_domain: str
-        :param company_location: The location / region of company.
-            ISO 3166-1 alpha-2 codes
-        :type company_location: str
-        :return: An object of Awaitable[:class:`proxycurl.models.CompanyUrlEnrichResult]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.CompanyUrlEnrichResult]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :return: An object of :class:`proxycurl.models.CompanyUrlEnrichResult` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.CompanyUrlEnrichResult`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/company/resolve',
             params={
-                'enrich_profile': enrich_profile,
-                'company_name': company_name,
-                'company_domain': company_domain,
                 'company_location': company_location,
+                'company_domain': company_domain,
+                'company_name': company_name,
+                'enrich_profile': enrich_profile,
             },
             data={
             },
             result_class=CompanyUrlEnrichResult
         )
-        return resp
 
-    async def find_job(
+    def find_job(
         self,
-        search_id: str,
-        keyword: str,
-        geo_id: str,
-        flexibility: str,
-        when: str,
-        experience_level: str,
-        job_type: str,
-    ) -> Awaitable[JobListPage]:
+        job_type: str = '',
+        experience_level: str = '',
+        when: str = '',
+        flexibility: str = '',
+        geo_id: str = '',
+        keyword: str = '',
+        search_id: str = '',
+    ) -> JobListPage:
         """Jobs Listing Endpoint
         
                 Cost: 2 credits / successful request.
         List jobs posted by a company on LinkedIn
         
-        :param search_id: The `search_id` of the company on LinkedIn.
-            You can get the `search_id` of a LinkedIn company via
-            [Company Profile API](#company-api-company-profile-endpoint).
-        :type search_id: str
-        :param keyword: The keyword to search for.
-        :type keyword: str
-        :param geo_id: The `geo_id` of the location to search for.
-            For example, `92000000` is the `geo_id` of world wide.
-
-            See [this article](https://nubela.co/blog/how-to-fetch-geo_id-parameter-for-the-job-api/?utm_source=blog&utm_medium=web&utm_campaign=docs-redirect-to-geo_id-article) as to how you may be able to match regions to `geo_id` input values.
-        :type geo_id: str
-        :param flexibility: The flexibility of the job.
-            It accepts the following 3 case insensitive values only:
-            - `remote`
-            - `on-site`
-            - `hybrid`
+        :param job_type: The nature of the job.
+            It accepts the following 7 case-insensitive values only:
+            - `full-time`
+            - `part-time`
+            - `contract`
+            - `internship`
+            - `temporary`
+            - `volunteer`
             - `anything` (default)
-        :type flexibility: str
-        :param when: The time when the job is posted,
-            It accepts the following case-insensitive values only:
-            - `yesterday`
-            - `past-week`
-            - `past-month`
-            - `anytime` (default)
-        :type when: str
+        :type job_type: str
         :param experience_level: The experience level needed for the job.
             It accepts the following 6 case-insensitive values only:
             - `internship`
             - `entry_level`
             - `associate`
             - `mid_senior_level`
             - `director`
             - `anything` (default)
         :type experience_level: str
-        :param job_type: The nature of the job.
-            It accepts the following 7 case-insensitive values only:
-            - `full-time`
-            - `part-time`
-            - `contract`
-            - `internship`
-            - `temporary`
-            - `volunteer`
+        :param when: The time when the job is posted,
+            It accepts the following case-insensitive values only:
+            - `yesterday`
+            - `past-week`
+            - `past-month`
+            - `anytime` (default)
+        :type when: str
+        :param flexibility: The flexibility of the job.
+            It accepts the following 3 case insensitive values only:
+            - `remote`
+            - `on-site`
+            - `hybrid`
             - `anything` (default)
-        :type job_type: str
-        :return: An object of Awaitable[:class:`proxycurl.models.JobListPage]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.JobListPage]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :type flexibility: str
+        :param geo_id: The `geo_id` of the location to search for.
+            For example, `92000000` is the `geo_id` of world wide.
+
+            See [this article](https://nubela.co/blog/how-to-fetch-geo_id-parameter-for-the-job-api/?utm_source=blog&utm_medium=web&utm_campaign=docs-redirect-to-geo_id-article) as to how you may be able to match regions to `geo_id` input values.
+        :type geo_id: str
+        :param keyword: The keyword to search for.
+        :type keyword: str
+        :param search_id: The `search_id` of the company on LinkedIn.
+            You can get the `search_id` of a LinkedIn company via
+            [Company Profile API](#company-api-company-profile-endpoint).
+        :type search_id: str
+        :return: An object of :class:`proxycurl.models.JobListPage` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.JobListPage`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/v2/linkedin/company/job',
             params={
-                'search_id': search_id,
-                'keyword': keyword,
-                'geo_id': geo_id,
-                'flexibility': flexibility,
-                'when': when,
-                'experience_level': experience_level,
                 'job_type': job_type,
+                'experience_level': experience_level,
+                'when': when,
+                'flexibility': flexibility,
+                'geo_id': geo_id,
+                'keyword': keyword,
+                'search_id': search_id,
             },
             data={
             },
             result_class=JobListPage
         )
-        return resp
 
-    async def job_count(
+    def job_count(
         self,
-        search_id: str,
-        keyword: str,
-        geo_id: str,
-        flexibility: str,
-        when: str,
-        experience_level: str,
-        job_type: str,
-    ) -> Awaitable[JobListCount]:
+        job_type: str = '',
+        experience_level: str = '',
+        when: str = '',
+        flexibility: str = '',
+        geo_id: str = '',
+        keyword: str = '',
+        search_id: str = '',
+    ) -> JobListCount:
         """Jobs Listing Count Endpoint
         
                 Cost: 2 credits / successful request.
         Count number of jobs posted by a company on LinkedIn
         
-        :param search_id: The `search_id` of the company on LinkedIn.
-            You can get the `search_id` of a LinkedIn company via
-            [Company Profile API](#company-api-company-profile-endpoint).
-        :type search_id: str
-        :param keyword: The keyword to search for.
-        :type keyword: str
-        :param geo_id: The `geo_id` of the location to search for.
-            For example, `92000000` is the `geo_id` of world wide.
-
-            See [this article](https://nubela.co/blog/how-to-fetch-geo_id-parameter-for-the-job-api/?utm_source=blog&utm_medium=web&utm_campaign=docs-redirect-to-geo_id-article) as to how you may be able to match regions to `geo_id` input values.
-        :type geo_id: str
-        :param flexibility: The flexibility of the job.
-            It accepts the following 3 case insensitive values only:
-            - `remote`
-            - `on-site`
-            - `hybrid`
+        :param job_type: The nature of the job.
+            It accepts the following 7 case-insensitive values only:
+            - `full-time`
+            - `part-time`
+            - `contract`
+            - `internship`
+            - `temporary`
+            - `volunteer`
             - `anything` (default)
-        :type flexibility: str
-        :param when: The time when the job is posted,
-            It accepts the following case-insensitive values only:
-            - `yesterday`
-            - `past-week`
-            - `past-month`
-            - `anytime` (default)
-        :type when: str
+        :type job_type: str
         :param experience_level: The experience level needed for the job.
             It accepts the following 6 case-insensitive values only:
             - `internship`
             - `entry_level`
             - `associate`
             - `mid_senior_level`
             - `director`
             - `anything` (default)
         :type experience_level: str
-        :param job_type: The nature of the job.
-            It accepts the following 7 case-insensitive values only:
-            - `full-time`
-            - `part-time`
-            - `contract`
-            - `internship`
-            - `temporary`
-            - `volunteer`
+        :param when: The time when the job is posted,
+            It accepts the following case-insensitive values only:
+            - `yesterday`
+            - `past-week`
+            - `past-month`
+            - `anytime` (default)
+        :type when: str
+        :param flexibility: The flexibility of the job.
+            It accepts the following 3 case insensitive values only:
+            - `remote`
+            - `on-site`
+            - `hybrid`
             - `anything` (default)
-        :type job_type: str
-        :return: An object of Awaitable[:class:`proxycurl.models.JobListCount]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.JobListCount]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :type flexibility: str
+        :param geo_id: The `geo_id` of the location to search for.
+            For example, `92000000` is the `geo_id` of world wide.
+
+            See [this article](https://nubela.co/blog/how-to-fetch-geo_id-parameter-for-the-job-api/?utm_source=blog&utm_medium=web&utm_campaign=docs-redirect-to-geo_id-article) as to how you may be able to match regions to `geo_id` input values.
+        :type geo_id: str
+        :param keyword: The keyword to search for.
+        :type keyword: str
+        :param search_id: The `search_id` of the company on LinkedIn.
+            You can get the `search_id` of a LinkedIn company via
+            [Company Profile API](#company-api-company-profile-endpoint).
+        :type search_id: str
+        :return: An object of :class:`proxycurl.models.JobListCount` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.JobListCount`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/v2/linkedin/company/job/count',
             params={
-                'search_id': search_id,
-                'keyword': keyword,
-                'geo_id': geo_id,
-                'flexibility': flexibility,
-                'when': when,
-                'experience_level': experience_level,
                 'job_type': job_type,
+                'experience_level': experience_level,
+                'when': when,
+                'flexibility': flexibility,
+                'geo_id': geo_id,
+                'keyword': keyword,
+                'search_id': search_id,
             },
             data={
             },
             result_class=JobListCount
         )
-        return resp
 
-    async def employee_count(
+    def employee_count(
         self,
         url: str,
-        employment_status: str,
-        linkedin_employee_count: str,
-        use_cache: str,
-    ) -> Awaitable[EmployeeCount]:
+        use_cache: str = '',
+        linkedin_employee_count: str = '',
+        employment_status: str = '',
+    ) -> EmployeeCount:
         """Employee Count Endpoint
         
                 Cost: 1 credit / successful request.
         Get a number of total employees of a Company.
 
         Get an employee count of this company from various sources.
         
         :param url: URL of the LinkedIn Company Profile to target.
 
             URL should be in the format of `https://www.linkedin.com/company/<public_identifier>`
         :type url: str
-        :param employment_status: Parameter to tell the API to filter past or current employees.
-
-            Valid values are `current`, `past`, and `all`:
+        :param use_cache: `if-present`: The default behavior. Fetches data from LinkDB cache regardless of age of profile.
 
-            * `current` (default) : count current employees
-            * `past` : count past employees
-            * `all` : count current & past employees
-        :type employment_status: str
+            `if-recent`: API will make a best effort to return a fresh data no older than 29 days. Costs an extra 1 credit on top of the cost of the base endpoint.
+        :type use_cache: str
         :param linkedin_employee_count: Option to include a scraped employee count value from the target company's LinkedIn profile.
 
             Valid values are `include` and `exclude`:
 
             * `exclude` (default) : To exclude the scraped employee count.
             * `include` : To include the scraped employee count.
 
             Costs an extra `1` credit on top of the base cost of the endpoint.
         :type linkedin_employee_count: str
-        :param use_cache: `if-present`: The default behavior. Fetches data from LinkDB cache regardless of age of profile.
+        :param employment_status: Parameter to tell the API to filter past or current employees.
 
-            `if-recent`: API will make a best effort to return a fresh data no older than 29 days. Costs an extra 1 credit on top of the cost of the base endpoint.
-        :type use_cache: str
-        :return: An object of Awaitable[:class:`proxycurl.models.EmployeeCount]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.EmployeeCount]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+            Valid values are `current`, `past`, and `all`:
+
+            * `current` (default) : count current employees
+            * `past` : count past employees
+            * `all` : count current & past employees
+        :type employment_status: str
+        :return: An object of :class:`proxycurl.models.EmployeeCount` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.EmployeeCount`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/company/employees/count',
             params={
                 'url': url,
-                'employment_status': employment_status,
-                'linkedin_employee_count': linkedin_employee_count,
                 'use_cache': use_cache,
+                'linkedin_employee_count': linkedin_employee_count,
+                'employment_status': employment_status,
             },
             data={
             },
             result_class=EmployeeCount
         )
-        return resp
 
-    async def employee_list(
+    def employee_list(
         self,
         url: str,
-        resolve_numeric_id: str,
-        sort_by: str,
-        employment_status: str,
-        page_size: str,
-        role_search: str,
-        enrich_profiles: str,
-        country: str,
-    ) -> Awaitable[EmployeeList]:
+        country: str = '',
+        enrich_profiles: str = '',
+        role_search: str = '',
+        page_size: str = '',
+        employment_status: str = '',
+        sort_by: str = '',
+        resolve_numeric_id: str = '',
+    ) -> EmployeeList:
         """Employee Listing Endpoint
         
                 Cost: 3 credits / employee returned.
         Get a list of employees of a Company.
 
         This API endpoint is limited by LinkDB which is populated with profiles in the US, UK, Canada, Israel, Australia, Ireland, New Zealand and Singapore.
         As such, this endpoint is best used to list employees working in companies based in those locations only.
         
         :param url: URL of the LinkedIn Company Profile to target.
 
             URL should be in the format of `https://www.linkedin.com/company/<public_identifier>`
         :type url: str
-        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
-            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
-
-            This parameter accepts the following values:
-            - `false` (default value) - Will not resolve numerical IDs.
-            - `true` - Enable support for Company Profile URLs with numerical IDs. 
-            Costs an extra `2` credit on top of the base cost of the endpoint.
-        :type resolve_numeric_id: str
-        :param sort_by: Sort employees by recency.
-
-            Valid values are:
-            * `recently-joined` - Sort employees by their join date. The most recent employee is on the top of the list.
-            * `recently-left` - Sort employees by their departure date. The most recent employee who had just left is on the top of this list.
-            * `none` - The default value. Do not sort.
+        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
 
-            If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per employee returned.
-        :type sort_by: str
-        :param employment_status: Parameter to tell the API to return past or current employees.
+            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
 
-            Valid values are `current`, `past`, and `all`:
+            Costs an extra `3` credit per result returned.
+        :type country: str
+        :param enrich_profiles: Get the full profile of employees instead of only their profile urls.
 
-            * `current` (default) : lists current employees
-            * `past` : lists past employees
-            * `all` : lists current & past employees
-        :type employment_status: str
-        :param page_size: Tune the maximum results returned per API call.
+            Each request respond with a streaming response of profiles.
 
-            The default value of this parameter is `200000`.
+            The valid values are:
 
-            Accepted values for this parameter is an integer ranging from `1` to `200000`.
+            * `skip` (default): lists employee's profile url
+            * `enrich`: lists full profile of employees
 
-            When `enrich_profiles=enrich`, this parameter accepts value ranging from `1` to `100`.
-        :type page_size: str
+            Calling this API endpoint with this parameter would add `1` credit per employee returned.
+        :type enrich_profiles: str
         :param role_search: Filter employees by their title by matching the employee's title against a *regular expression*.
 
             The default value of this parameter is `null`.
 
             The accepted value is a *regular expression* (regex).
 
             (The base cost of calling this API endpoint with this parameter would be `10` credits.
             Each employee matched and returned would cost `6` credits per employee returned.)
         :type role_search: str
-        :param enrich_profiles: Get the full profile of employees instead of only their profile urls.
+        :param page_size: Tune the maximum results returned per API call.
 
-            Each request respond with a streaming response of profiles.
+            The default value of this parameter is `200000`.
 
-            The valid values are:
+            Accepted values for this parameter is an integer ranging from `1` to `200000`.
 
-            * `skip` (default): lists employee's profile url
-            * `enrich`: lists full profile of employees
+            When `enrich_profiles=enrich`, this parameter accepts value ranging from `1` to `100`.
+        :type page_size: str
+        :param employment_status: Parameter to tell the API to return past or current employees.
 
-            Calling this API endpoint with this parameter would add `1` credit per employee returned.
-        :type enrich_profiles: str
-        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
+            Valid values are `current`, `past`, and `all`:
 
-            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
+            * `current` (default) : lists current employees
+            * `past` : lists past employees
+            * `all` : lists current & past employees
+        :type employment_status: str
+        :param sort_by: Sort employees by recency.
 
-            Costs an extra `3` credit per result returned.
-        :type country: str
-        :return: An object of Awaitable[:class:`proxycurl.models.EmployeeList]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.EmployeeList]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+            Valid values are:
+            * `recently-joined` - Sort employees by their join date. The most recent employee is on the top of the list.
+            * `recently-left` - Sort employees by their departure date. The most recent employee who had just left is on the top of this list.
+            * `none` - The default value. Do not sort.
+
+            If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per employee returned.
+        :type sort_by: str
+        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
+            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
+
+            This parameter accepts the following values:
+            - `false` (default value) - Will not resolve numerical IDs.
+            - `true` - Enable support for Company Profile URLs with numerical IDs. 
+            Costs an extra `2` credit on top of the base cost of the endpoint.
+        :type resolve_numeric_id: str
+        :return: An object of :class:`proxycurl.models.EmployeeList` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.EmployeeList`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/company/employees',
             params={
                 'url': url,
-                'resolve_numeric_id': resolve_numeric_id,
-                'sort_by': sort_by,
-                'employment_status': employment_status,
-                'page_size': page_size,
-                'role_search': role_search,
-                'enrich_profiles': enrich_profiles,
                 'country': country,
+                'enrich_profiles': enrich_profiles,
+                'role_search': role_search,
+                'page_size': page_size,
+                'employment_status': employment_status,
+                'sort_by': sort_by,
+                'resolve_numeric_id': resolve_numeric_id,
             },
             data={
             },
             result_class=EmployeeList
         )
-        return resp
 
-    async def role_lookup(
+    def role_lookup(
         self,
         company_name: str,
         role: str,
-        enrich_profile: str,
-    ) -> Awaitable[RoleSearchErichedResult]:
+        enrich_profile: str = '',
+    ) -> RoleSearchErichedResult:
         """Role Lookup Endpoint
         
                 Cost: 3 credits / successful request.
         Finds the closest (person) profile with a given role in a Company.
         For example, you can use this endpoint to find the "CTO" of "Apple".
         This API endpoint returns only one result that is the closest match.
 
@@ -1066,298 +1048,293 @@
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
             please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
-        :return: An object of Awaitable[:class:`proxycurl.models.RoleSearchErichedResult]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.RoleSearchErichedResult]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :return: An object of :class:`proxycurl.models.RoleSearchErichedResult` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.RoleSearchErichedResult`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/find/company/role',
             params={
                 'company_name': company_name,
                 'role': role,
                 'enrich_profile': enrich_profile,
             },
             data={
             },
             result_class=RoleSearchErichedResult
         )
-        return resp
 
-    async def reveal(
+    def reveal(
         self,
         ip: str,
-        role: str,
-        role_personal_email: str,
-        role_contact_number: str,
-    ) -> Awaitable[CompanyReveal]:
+        role_contact_number: str = '',
+        role_personal_email: str = '',
+        role: str = '',
+    ) -> CompanyReveal:
         """Reveal Endpoint
         
                 Cost: 2 credits / successful request.
         Deanonymize an IPv4 address and associate the Company behind the IPv4 address.
         
         :param ip: The target IPv4 address.
         :type ip: str
+        :param role_contact_number: Append personal contact numbers to the response if the system finds a relevant person profile.
+        :type role_contact_number: str
+        :param role_personal_email: Append personal email addresses to the response if the system finds a relevant person profile.
+        :type role_personal_email: str
         :param role: Lookup and append an employee of a certain role of the company.
             Within the same API call, You can choose to lookup a person with a given role within this organisation that you might want to reach out to.
         :type role: str
-        :param role_personal_email: Append personal email addresses to the response if the system finds a relevant person profile.
-        :type role_personal_email: str
-        :param role_contact_number: Append personal contact numbers to the response if the system finds a relevant person profile.
-        :type role_contact_number: str
-        :return: An object of Awaitable[:class:`proxycurl.models.CompanyReveal]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.CompanyReveal]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :return: An object of :class:`proxycurl.models.CompanyReveal` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.CompanyReveal`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/reveal/company',
             params={
                 'ip': ip,
-                'role': role,
-                'role_personal_email': role_personal_email,
                 'role_contact_number': role_contact_number,
+                'role_personal_email': role_personal_email,
+                'role': role,
             },
             data={
             },
             result_class=CompanyReveal
         )
-        return resp
 
-    async def employees(
+    def employees(
         self,
         url: str,
-        resolve_numeric_id: str,
-        sort_by: str,
-        employment_status: str,
-        page_size: str,
-        role_search: str,
-        enrich_profiles: str,
-        country: str,
-    ) -> Awaitable[EmployeeList]:
+        country: str = '',
+        enrich_profiles: str = '',
+        role_search: str = '',
+        page_size: str = '',
+        employment_status: str = '',
+        sort_by: str = '',
+        resolve_numeric_id: str = '',
+    ) -> EmployeeList:
         """Employee Listing Endpoint
         
                 Cost: 3 credits / employee returned.
         Get a list of employees of a Company.
 
         This API endpoint is limited by LinkDB which is populated with profiles in the US, UK, Canada, Israel, Australia, Ireland, New Zealand and Singapore.
         As such, this endpoint is best used to list employees working in companies based in those locations only.
         
         :param url: URL of the LinkedIn Company Profile to target.
 
             URL should be in the format of `https://www.linkedin.com/company/<public_identifier>`
         :type url: str
-        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
-            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
-
-            This parameter accepts the following values:
-            - `false` (default value) - Will not resolve numerical IDs.
-            - `true` - Enable support for Company Profile URLs with numerical IDs. 
-            Costs an extra `2` credit on top of the base cost of the endpoint.
-        :type resolve_numeric_id: str
-        :param sort_by: Sort employees by recency.
-
-            Valid values are:
-            * `recently-joined` - Sort employees by their join date. The most recent employee is on the top of the list.
-            * `recently-left` - Sort employees by their departure date. The most recent employee who had just left is on the top of this list.
-            * `none` - The default value. Do not sort.
+        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
 
-            If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per employee returned.
-        :type sort_by: str
-        :param employment_status: Parameter to tell the API to return past or current employees.
+            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
 
-            Valid values are `current`, `past`, and `all`:
+            Costs an extra `3` credit per result returned.
+        :type country: str
+        :param enrich_profiles: Get the full profile of employees instead of only their profile urls.
 
-            * `current` (default) : lists current employees
-            * `past` : lists past employees
-            * `all` : lists current & past employees
-        :type employment_status: str
-        :param page_size: Tune the maximum results returned per API call.
+            Each request respond with a streaming response of profiles.
 
-            The default value of this parameter is `200000`.
+            The valid values are:
 
-            Accepted values for this parameter is an integer ranging from `1` to `200000`.
+            * `skip` (default): lists employee's profile url
+            * `enrich`: lists full profile of employees
 
-            When `enrich_profiles=enrich`, this parameter accepts value ranging from `1` to `100`.
-        :type page_size: str
+            Calling this API endpoint with this parameter would add `1` credit per employee returned.
+        :type enrich_profiles: str
         :param role_search: Filter employees by their title by matching the employee's title against a *regular expression*.
 
             The default value of this parameter is `null`.
 
             The accepted value is a *regular expression* (regex).
 
             (The base cost of calling this API endpoint with this parameter would be `10` credits.
             Each employee matched and returned would cost `6` credits per employee returned.)
         :type role_search: str
-        :param enrich_profiles: Get the full profile of employees instead of only their profile urls.
+        :param page_size: Tune the maximum results returned per API call.
 
-            Each request respond with a streaming response of profiles.
+            The default value of this parameter is `200000`.
 
-            The valid values are:
+            Accepted values for this parameter is an integer ranging from `1` to `200000`.
 
-            * `skip` (default): lists employee's profile url
-            * `enrich`: lists full profile of employees
+            When `enrich_profiles=enrich`, this parameter accepts value ranging from `1` to `100`.
+        :type page_size: str
+        :param employment_status: Parameter to tell the API to return past or current employees.
 
-            Calling this API endpoint with this parameter would add `1` credit per employee returned.
-        :type enrich_profiles: str
-        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
+            Valid values are `current`, `past`, and `all`:
 
-            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
+            * `current` (default) : lists current employees
+            * `past` : lists past employees
+            * `all` : lists current & past employees
+        :type employment_status: str
+        :param sort_by: Sort employees by recency.
 
-            Costs an extra `3` credit per result returned.
-        :type country: str
-        :return: An object of Awaitable[:class:`proxycurl.models.EmployeeList]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.EmployeeList]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+            Valid values are:
+            * `recently-joined` - Sort employees by their join date. The most recent employee is on the top of the list.
+            * `recently-left` - Sort employees by their departure date. The most recent employee who had just left is on the top of this list.
+            * `none` - The default value. Do not sort.
+
+            If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per employee returned.
+        :type sort_by: str
+        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
+            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
+
+            This parameter accepts the following values:
+            - `false` (default value) - Will not resolve numerical IDs.
+            - `true` - Enable support for Company Profile URLs with numerical IDs. 
+            Costs an extra `2` credit on top of the base cost of the endpoint.
+        :type resolve_numeric_id: str
+        :return: An object of :class:`proxycurl.models.EmployeeList` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.EmployeeList`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/company/employees',
             params={
                 'url': url,
-                'resolve_numeric_id': resolve_numeric_id,
-                'sort_by': sort_by,
-                'employment_status': employment_status,
-                'page_size': page_size,
-                'role_search': role_search,
-                'enrich_profiles': enrich_profiles,
                 'country': country,
+                'enrich_profiles': enrich_profiles,
+                'role_search': role_search,
+                'page_size': page_size,
+                'employment_status': employment_status,
+                'sort_by': sort_by,
+                'resolve_numeric_id': resolve_numeric_id,
             },
             data={
             },
             result_class=EmployeeList
         )
-        return resp
 
-    async def employee_search(
+    def employee_search(
         self,
-        resolve_numeric_id: str,
-        enrich_profiles: str,
-        country: str,
         keyword_regex: str,
         linkedin_company_profile_url: str,
-        page_size: str,
-    ) -> Awaitable[EmployeeList]:
+        page_size: str = '',
+        country: str = '',
+        enrich_profiles: str = '',
+        resolve_numeric_id: str = '',
+    ) -> EmployeeList:
         """Employee Search Endpoint
         
                 Cost: 10 credits / successful request.
         Search employees of a target by their job title.
         This API endpoint is syntactic sugar for the role_search parameter under the [Employee Listing Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-listing-endpoint).
 
         Results are limited by data that we have within [LinkDB](https://nubela.co/proxycurl/linkdb).
         Use [Role Lookup API Endpoint](https://nubela.co/proxycurl/docs#people-api-role-lookup-endpoint) if you need to query for profiles without LinkDB constraints.
         The drawbacks of the Role Lookup API Endpoint is that it is less precise and can return at most one result per query.
         
-        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
-            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
+        :param keyword_regex: Job title keyword to search for in regular expression format.
+        :type keyword_regex: str
+        :param linkedin_company_profile_url: LinkedIn Profile URL of the target company.
+        :type linkedin_company_profile_url: str
+        :param page_size: Tune the maximum results returned per API call.
+            The default value of this parameter is `200000`.
+            Accepted values for this parameter is an integer ranging from `1` to `200000`.
+        :type page_size: str
+        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
 
-            This parameter accepts the following values:
-            - `false` (default value) - Will not resolve numerical IDs.
-            - `true` - Enable support for Company Profile URLs with numerical IDs. 
-            Costs an extra `2` credit on top of the base cost of the endpoint.
-        :type resolve_numeric_id: str
+            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
+
+            Costs an extra `3` credit per result returned.
+        :type country: str
         :param enrich_profiles: Get the full profile of employees instead of only their profile urls.
 
             Each request respond with a streaming response of profiles.
 
             The valid values are:
 
             * `skip` (default): lists employee's profile url
             * `enrich`: lists full profile of employees
 
             Calling this API endpoint with this parameter would add `1` credit per employee returned.
         :type enrich_profiles: str
-        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
-
-            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
+        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
+            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
 
-            Costs an extra `3` credit per result returned.
-        :type country: str
-        :param keyword_regex: Job title keyword to search for in regular expression format.
-        :type keyword_regex: str
-        :param linkedin_company_profile_url: LinkedIn Profile URL of the target company.
-        :type linkedin_company_profile_url: str
-        :param page_size: Tune the maximum results returned per API call.
-            The default value of this parameter is `200000`.
-            Accepted values for this parameter is an integer ranging from `1` to `200000`.
-        :type page_size: str
-        :return: An object of Awaitable[:class:`proxycurl.models.EmployeeList]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.EmployeeList]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+            This parameter accepts the following values:
+            - `false` (default value) - Will not resolve numerical IDs.
+            - `true` - Enable support for Company Profile URLs with numerical IDs. 
+            Costs an extra `2` credit on top of the base cost of the endpoint.
+        :type resolve_numeric_id: str
+        :return: An object of :class:`proxycurl.models.EmployeeList` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.EmployeeList`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/company/employee/search',
             params={
-                'resolve_numeric_id': resolve_numeric_id,
-                'enrich_profiles': enrich_profiles,
-                'country': country,
                 'keyword_regex': keyword_regex,
                 'linkedin_company_profile_url': linkedin_company_profile_url,
                 'page_size': page_size,
+                'country': country,
+                'enrich_profiles': enrich_profiles,
+                'resolve_numeric_id': resolve_numeric_id,
             },
             data={
             },
             result_class=EmployeeList
         )
-        return resp
 
-    async def profile_picture(
+    def profile_picture(
         self,
         linkedin_company_profile_url: str,
-    ) -> Awaitable[ProfilePicture]:
+    ) -> ProfilePicture:
         """Company Profile Picture Endpoint
         
                 Cost: 0 credit / successful request.
         Get the profile picture of a company.
 
         Profile pictures are served from cached company profiles found within [LinkDB](https://nubela.co/proxycurl/linkdb).
         If the profile does not exist within [LinkDB](https://nubela.co/proxycurl/linkdb), then the API will return a `404` status code.
         
         :param linkedin_company_profile_url: LinkedIn Profile URL of the company that you are trying to get the profile picture of.
         :type linkedin_company_profile_url: str
-        :return: An object of Awaitable[:class:`proxycurl.models.ProfilePicture]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.ProfilePicture]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :return: An object of :class:`proxycurl.models.ProfilePicture` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.ProfilePicture`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/company/profile-picture',
             params={
                 'linkedin_company_profile_url': linkedin_company_profile_url,
             },
             data={
             },
             result_class=ProfilePicture
         )
-        return resp
 
-    async def find_role(
+    def find_role(
         self,
         company_name: str,
         role: str,
-        enrich_profile: str,
-    ) -> Awaitable[RoleSearchErichedResult]:
+        enrich_profile: str = '',
+    ) -> RoleSearchErichedResult:
         """Role Lookup Endpoint
         
                 Cost: 3 credits / successful request.
         Finds the closest (person) profile with a given role in a Company.
         For example, you can use this endpoint to find the "CTO" of "Apple".
         This API endpoint returns only one result that is the closest match.
 
@@ -1381,219 +1358,215 @@
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
             please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
-        :return: An object of Awaitable[:class:`proxycurl.models.RoleSearchErichedResult]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.RoleSearchErichedResult]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :return: An object of :class:`proxycurl.models.RoleSearchErichedResult` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.RoleSearchErichedResult`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/find/company/role',
             params={
                 'company_name': company_name,
                 'role': role,
                 'enrich_profile': enrich_profile,
             },
             data={
             },
             result_class=RoleSearchErichedResult
         )
-        return resp
 
 
 class _LinkedinSchool:
     def __init__(self, linkedin):
         self.linkedin = linkedin
 
-    async def get(
+    def get(
         self,
-        use_cache: str,
         url: str,
-    ) -> Awaitable[LinkedinSchool]:
+        use_cache: str = '',
+    ) -> LinkedinSchool:
         """School Profile Endpoint
         
                 Cost: 1 credit / successful request.
         Get structured data of a LinkedIn School Profile
         
-        :param use_cache: `if-present` The default behavior. Fetches profile from cache regardless of age of profile. If profile is not available in cache, API will attempt to source profile externally.
-
-            `if-recent` API will make a best effort to return a fresh profile no older than 29 days.Costs an extra `1` credit on top of the cost of the base endpoint.
-        :type use_cache: str
         :param url: URL of the LinkedIn School Profile to crawl.
 
             URL should be in the format of `https://www.linkedin.com/school/<public_identifier>`
         :type url: str
-        :return: An object of Awaitable[:class:`proxycurl.models.LinkedinSchool]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.LinkedinSchool]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :param use_cache: `if-present` The default behavior. Fetches profile from cache regardless of age of profile. If profile is not available in cache, API will attempt to source profile externally.
+
+            `if-recent` API will make a best effort to return a fresh profile no older than 29 days.Costs an extra `1` credit on top of the cost of the base endpoint.
+        :type use_cache: str
+        :return: An object of :class:`proxycurl.models.LinkedinSchool` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.LinkedinSchool`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/school',
             params={
-                'use_cache': use_cache,
                 'url': url,
+                'use_cache': use_cache,
             },
             data={
             },
             result_class=LinkedinSchool
         )
-        return resp
 
-    async def students(
+    def students(
         self,
         linkedin_school_url: str,
-        resolve_numeric_id: str,
-        sort_by: str,
-        student_status: str,
-        page_size: str,
-        search_keyword: str,
-        enrich_profiles: str,
-        country: str,
-    ) -> Awaitable[StudentList]:
+        country: str = '',
+        enrich_profiles: str = '',
+        search_keyword: str = '',
+        page_size: str = '',
+        student_status: str = '',
+        sort_by: str = '',
+        resolve_numeric_id: str = '',
+    ) -> StudentList:
         """Student Listing Endpoint
         
                 Cost: 3 credits / student returned.
         Get a list of students of a school or university.
         
         :param linkedin_school_url: URL of the LinkedIn School Profile to target.
 
             URL should be in the format of `https://www.linkedin.com/school/<public_identifier>`
         :type linkedin_school_url: str
-        :param resolve_numeric_id: Enable support for School Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
-            For example, we will turn `https://www.linkedin.com/school/1234567890` to `https://www.linkedin.com/school/acme-corp` -- for which the API endpoint only supports the latter.
-
-            This parameter accepts the following values:
-            - `false` (default value) - Will not resolve numerical IDs.
-            - `true` - Enable support for School Profile URLs with numerical IDs. 
-            Costs an extra `2` credit on top of the base cost of the endpoint.
-        :type resolve_numeric_id: str
-        :param sort_by: Sort students by matriculation or graduation dates.
-
-            Valid values are:
-            * `recently-matriculated` - Sort students by their matriculation date. Students who had had most recently started school is on the top of the list.
-            * `recently-graduated` - Sort students by their graduation date. The most recently graduated student is on the top of this list.
-            * `none` - The default value. Do not sort.
+        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
 
-            If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per student returned.
-        :type sort_by: str
-        :param student_status: Parameter to tell the API to return past or current students.
+            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
 
-            Valid values are `current`, `past`, and `all`:
+            Costs an extra `3` credit per result returned.
+        :type country: str
+        :param enrich_profiles: Get the full profile of students instead of only their profile urls.
 
-            * `current` (default) : lists current students
-            * `past` : lists past students
-            * `all` : lists current & past students
-        :type student_status: str
-        :param page_size: Tune the maximum results returned per API call.
+            Each request respond with a streaming response of profiles.
 
-            The default value of this parameter is `200000`.
+            The valid values are:
 
-            Accepted values for this parameter is an integer ranging from `1` to `200000`.
+            * `skip` (default): lists student's profile url
+            * `enrich`: lists full profile of students
 
-            When `enrich_profiles=enrich`, this parameter accepts value ranging from `1` to `100`.
-        :type page_size: str
+            *Calling this API endpoint with this parameter would add `1` credit per student returned.*
+        :type enrich_profiles: str
         :param search_keyword: Filter students by their major by matching the student's major against a *regular expression*.
 
             The default value of this parameter is `null`.
 
             The accepted value is a *regular expression* (regex).
 
             (The base cost of calling this API endpoint with this parameter would be `10` credits.
             Each student matched and returned would cost `6` credits per student returned.)
         :type search_keyword: str
-        :param enrich_profiles: Get the full profile of students instead of only their profile urls.
+        :param page_size: Tune the maximum results returned per API call.
 
-            Each request respond with a streaming response of profiles.
+            The default value of this parameter is `200000`.
 
-            The valid values are:
+            Accepted values for this parameter is an integer ranging from `1` to `200000`.
 
-            * `skip` (default): lists student's profile url
-            * `enrich`: lists full profile of students
+            When `enrich_profiles=enrich`, this parameter accepts value ranging from `1` to `100`.
+        :type page_size: str
+        :param student_status: Parameter to tell the API to return past or current students.
 
-            *Calling this API endpoint with this parameter would add `1` credit per student returned.*
-        :type enrich_profiles: str
-        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
+            Valid values are `current`, `past`, and `all`:
 
-            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
+            * `current` (default) : lists current students
+            * `past` : lists past students
+            * `all` : lists current & past students
+        :type student_status: str
+        :param sort_by: Sort students by matriculation or graduation dates.
 
-            Costs an extra `3` credit per result returned.
-        :type country: str
-        :return: An object of Awaitable[:class:`proxycurl.models.StudentList]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.StudentList]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+            Valid values are:
+            * `recently-matriculated` - Sort students by their matriculation date. Students who had had most recently started school is on the top of the list.
+            * `recently-graduated` - Sort students by their graduation date. The most recently graduated student is on the top of this list.
+            * `none` - The default value. Do not sort.
+
+            If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per student returned.
+        :type sort_by: str
+        :param resolve_numeric_id: Enable support for School Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
+            For example, we will turn `https://www.linkedin.com/school/1234567890` to `https://www.linkedin.com/school/acme-corp` -- for which the API endpoint only supports the latter.
+
+            This parameter accepts the following values:
+            - `false` (default value) - Will not resolve numerical IDs.
+            - `true` - Enable support for School Profile URLs with numerical IDs. 
+            Costs an extra `2` credit on top of the base cost of the endpoint.
+        :type resolve_numeric_id: str
+        :return: An object of :class:`proxycurl.models.StudentList` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.StudentList`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/school/students',
             params={
                 'linkedin_school_url': linkedin_school_url,
-                'resolve_numeric_id': resolve_numeric_id,
-                'sort_by': sort_by,
-                'student_status': student_status,
-                'page_size': page_size,
-                'search_keyword': search_keyword,
-                'enrich_profiles': enrich_profiles,
                 'country': country,
+                'enrich_profiles': enrich_profiles,
+                'search_keyword': search_keyword,
+                'page_size': page_size,
+                'student_status': student_status,
+                'sort_by': sort_by,
+                'resolve_numeric_id': resolve_numeric_id,
             },
             data={
             },
             result_class=StudentList
         )
-        return resp
 
 
 class _LinkedinJob:
     def __init__(self, linkedin):
         self.linkedin = linkedin
 
-    async def get(
+    def get(
         self,
         url: str,
-    ) -> Awaitable[JobProfile]:
+    ) -> JobProfile:
         """Job Profile Endpoint
         
                 Cost: 2 credits / successful request.
         Get structured data of a LinkedIn Job Profile
         
         :param url: URL of the LinkedIn Job Profile to target.
 
             URL should be in the format of
             `https://www.linkedin.com/jobs/view/<job_id>`.
             [Jobs Listing Endpoint](#jobs-api-jobs-listing-endpoint)
             can be used to retrieve a job URL.
         :type url: str
-        :return: An object of Awaitable[:class:`proxycurl.models.JobProfile]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.JobProfile]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :return: An object of :class:`proxycurl.models.JobProfile` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.JobProfile`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/job',
             params={
                 'url': url,
             },
             data={
             },
             result_class=JobProfile
         )
-        return resp
 
 
 class _Linkedin:
     person: _LinkedinPerson
     company: _LinkedinCompany
     school: _LinkedinSchool
     job: _LinkedinJob
@@ -1620,31 +1593,30 @@
         self.api_key = api_key
         self.base_url = base_url
         self.timeout = timeout
         self.max_retries = max_retries
         self.max_backoff_seconds = max_backoff_seconds
         self.linkedin = _Linkedin(self)
 
-    async def get_balance(
+    def get_balance(
         self,
-    ) -> Awaitable[CreditBalance]:
+    ) -> CreditBalance:
         """View Credit Balance Endpoint
         
                 Cost: 0 credit / successful request.
         Get your current credit(s) balance
         
-        :return: An object of Awaitable[:class:`proxycurl.models.CreditBalance]` or **None** if there is an error.
-        :rtype: Awaitable[:class:`proxycurl.models.CreditBalance]`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
+        :return: An object of :class:`proxycurl.models.CreditBalance` or **None** if there is an error.
+        :rtype: :class:`proxycurl.models.CreditBalance`
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
 
         """
 
-        resp = await self.linkedin.proxycurl.request(
+        return self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/credit-balance',
             params={
             },
             data={
             },
             result_class=CreditBalance
         )
-        return resp
```

### Comparing `proxycurl-py-0.0.20/proxycurl_py/gevent/base.py` & `proxycurl_py-0.0.21/proxycurl_py/gevent/base.py`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.20/proxycurl_py/gevent/library.py` & `proxycurl_py-0.0.21/proxycurl_py/twisted/library.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from twisted.internet import defer
+from twisted.internet.defer import Deferred, inlineCallbacks
 from proxycurl_py.config import (
     BASE_URL, PROXYCURL_API_KEY, TIMEOUT, MAX_RETRIES, MAX_BACKOFF_SECONDS
 )
-from proxycurl_py.gevent.base import ProxycurlBase
+from proxycurl_py.twisted.base import ProxycurlBase
 from proxycurl_py.models import (
     PersonEndpointResponse,
     PersonLookupUrlEnrichResult,
     ReverseEmailUrlEnrichResult,
     ExtractionEmailResult,
     PDLPhoneNumberResult,
     PDLEmailResult,
@@ -26,196 +28,201 @@
 )
 
 
 class _LinkedinPerson:
     def __init__(self, linkedin):
         self.linkedin = linkedin
 
+    @inlineCallbacks
     def get(
         self,
-        extra: str,
-        github_profile_id: str,
-        facebook_profile_id: str,
-        twitter_profile_id: str,
-        personal_contact_number: str,
-        personal_email: str,
-        inferred_salary: str,
-        skills: str,
-        use_cache: str,
         fallback_to_cache: str,
         url: str,
-    ) -> PersonEndpointResponse:
+        use_cache: str = '',
+        skills: str = '',
+        inferred_salary: str = '',
+        personal_email: str = '',
+        personal_contact_number: str = '',
+        twitter_profile_id: str = '',
+        facebook_profile_id: str = '',
+        github_profile_id: str = '',
+        extra: str = '',
+    ) -> Deferred:
         """Person Profile Endpoint
         
                 Cost: 1 credit / successful request.
         Get structured data of a Personal Profile
         
-        :param extra: Enriches the Person Profile with extra details from external sources.
-            Extra details include gender, birth date, industry and interests.
+        :param fallback_to_cache: Tweaks the fallback behavior if an error arises from fetching a fresh profile.
 
             This parameter accepts the following values:
-            - `exclude` (default value) - Does not provide extra data field.
-            - `include` - Append extra data to the person profile object.
-            Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
-        :type extra: str
-        :param github_profile_id: Enriches the Person Profile with Github Id from external sources.
+            * `on-error` (default value) - Fallback to reading the profile from cache if an error arises.
+            * `never` - Do not ever read profile from cache.
+        :type fallback_to_cache: str
+        :param url: URL of the LinkedIn Profile to crawl.
+
+            URL should be in the format of `https://www.linkedin.com/in/<public-identifier>`
+        :type url: str
+        :param use_cache: `if-present` The default behavior. Fetches profile from cache regardless of age of profile. If profile is not available in cache, API will attempt to source profile externally.
+
+            `if-recent` API will make a best effort to return a fresh profile no older than 29 days.Costs an extra `1` credit on top of the cost of the base endpoint.
+        :type use_cache: str
+        :param skills: Include skills data from external sources.
 
             This parameter accepts the following values:
-            - `exclude` (default value) - Does not provide Github Id data field.
-            - `include` - Append Github Id data to the person profile object.
+            - `exclude` (default value) - Does not provide skills data field.
+            - `include` - Append skills data to the person profile object.
             Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
-        :type github_profile_id: str
-        :param facebook_profile_id: Enriches the Person Profile with Facebook Id from external sources.
+        :type skills: str
+        :param inferred_salary: Include inferred salary range from external sources.
 
             This parameter accepts the following values:
-            - `exclude` (default value) - Does not provide Facebook Id data field.
-            - `include` - Append Facebook Id data to the person profile object.
+            - `exclude` (default value) - Does not provide inferred salary data field.
+            - `include` - Append inferred salary range data to the person profile object.
             Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
-        :type facebook_profile_id: str
-        :param twitter_profile_id: Enriches the Person Profile with Twitter Id from external sources.
+        :type inferred_salary: str
+        :param personal_email: Enriches the Person Profile with personal emails from external sources.
 
             This parameter accepts the following values:
-            - `exclude` (default value) - Does not provide Twitter Id data field.
-            - `include` - Append Twitter Id data to the person profile object.
-            Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
-        :type twitter_profile_id: str
+            - `exclude` (default value) - Does not provide personal emails data field.
+            - `include` - Append personal emails data to the person profile object.
+            Costs an extra `1` credit per email returned on top of the cost of the base endpoint (if data is available).
+        :type personal_email: str
         :param personal_contact_number: Enriches the Person Profile with personal numbers from external sources.
 
             This parameter accepts the following values:
             - `exclude` (default value) - Does not provide personal numbers data field.
             - `include` - Append personal numbers data to the person profile object.
             Costs an extra `1` credit per email returned on top of the cost of the base endpoint (if data is available).
         :type personal_contact_number: str
-        :param personal_email: Enriches the Person Profile with personal emails from external sources.
+        :param twitter_profile_id: Enriches the Person Profile with Twitter Id from external sources.
 
             This parameter accepts the following values:
-            - `exclude` (default value) - Does not provide personal emails data field.
-            - `include` - Append personal emails data to the person profile object.
-            Costs an extra `1` credit per email returned on top of the cost of the base endpoint (if data is available).
-        :type personal_email: str
-        :param inferred_salary: Include inferred salary range from external sources.
+            - `exclude` (default value) - Does not provide Twitter Id data field.
+            - `include` - Append Twitter Id data to the person profile object.
+            Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
+        :type twitter_profile_id: str
+        :param facebook_profile_id: Enriches the Person Profile with Facebook Id from external sources.
 
             This parameter accepts the following values:
-            - `exclude` (default value) - Does not provide inferred salary data field.
-            - `include` - Append inferred salary range data to the person profile object.
+            - `exclude` (default value) - Does not provide Facebook Id data field.
+            - `include` - Append Facebook Id data to the person profile object.
             Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
-        :type inferred_salary: str
-        :param skills: Include skills data from external sources.
+        :type facebook_profile_id: str
+        :param github_profile_id: Enriches the Person Profile with Github Id from external sources.
 
             This parameter accepts the following values:
-            - `exclude` (default value) - Does not provide skills data field.
-            - `include` - Append skills data to the person profile object.
+            - `exclude` (default value) - Does not provide Github Id data field.
+            - `include` - Append Github Id data to the person profile object.
             Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
-        :type skills: str
-        :param use_cache: `if-present` The default behavior. Fetches profile from cache regardless of age of profile. If profile is not available in cache, API will attempt to source profile externally.
-
-            `if-recent` API will make a best effort to return a fresh profile no older than 29 days.Costs an extra `1` credit on top of the cost of the base endpoint.
-        :type use_cache: str
-        :param fallback_to_cache: Tweaks the fallback behavior if an error arises from fetching a fresh profile.
+        :type github_profile_id: str
+        :param extra: Enriches the Person Profile with extra details from external sources.
+            Extra details include gender, birth date, industry and interests.
 
             This parameter accepts the following values:
-            * `on-error` (default value) - Fallback to reading the profile from cache if an error arises.
-            * `never` - Do not ever read profile from cache.
-        :type fallback_to_cache: str
-        :param url: URL of the LinkedIn Profile to crawl.
-
-            URL should be in the format of `https://www.linkedin.com/in/<public-identifier>`
-        :type url: str
-        :return: An object of :class:`proxycurl.models.PersonEndpointResponse` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.PersonEndpointResponse`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+            - `exclude` (default value) - Does not provide extra data field.
+            - `include` - Append extra data to the person profile object.
+            Costs an extra `1` credit on top of the cost of the base endpoint (if data is available).
+        :type extra: str
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/v2/linkedin',
             params={
-                'extra': extra,
-                'github_profile_id': github_profile_id,
-                'facebook_profile_id': facebook_profile_id,
-                'twitter_profile_id': twitter_profile_id,
-                'personal_contact_number': personal_contact_number,
-                'personal_email': personal_email,
-                'inferred_salary': inferred_salary,
-                'skills': skills,
-                'use_cache': use_cache,
                 'fallback_to_cache': fallback_to_cache,
                 'url': url,
+                'use_cache': use_cache,
+                'skills': skills,
+                'inferred_salary': inferred_salary,
+                'personal_email': personal_email,
+                'personal_contact_number': personal_contact_number,
+                'twitter_profile_id': twitter_profile_id,
+                'facebook_profile_id': facebook_profile_id,
+                'github_profile_id': github_profile_id,
+                'extra': extra,
             },
             data={
             },
             result_class=PersonEndpointResponse
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def resolve(
         self,
         first_name: str,
-        last_name: str,
-        title: str,
-        location: str,
         company_domain: str,
-        enrich_profile: str,
-    ) -> PersonLookupUrlEnrichResult:
+        enrich_profile: str = '',
+        location: str = '',
+        title: str = '',
+        last_name: str = '',
+    ) -> Deferred:
         """Person Lookup Endpoint
         
                 Cost: 2 credits / successful request.
         Look up a person with a name and company information.
         
         :param first_name: First name of the user
         :type first_name: str
-        :param last_name: Last name of the user
-        :type last_name: str
-        :param title: Title that user is holding at his/her current job
-        :type title: str
-        :param location: The location of this user.
-
-            Name of country, city or state.
-        :type location: str
         :param company_domain: Company name or domain
         :type company_domain: str
         :param enrich_profile: Enrich the result with a cached profile of the lookup result.
 
             The valid values are:
 
             * `skip` (default): do not enrich the results with cached profile data
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
             please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
-        :return: An object of :class:`proxycurl.models.PersonLookupUrlEnrichResult` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.PersonLookupUrlEnrichResult`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :param location: The location of this user.
+
+            Name of country, city or state.
+        :type location: str
+        :param title: Title that user is holding at his/her current job
+        :type title: str
+        :param last_name: Last name of the user
+        :type last_name: str
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/profile/resolve',
             params={
                 'first_name': first_name,
-                'last_name': last_name,
-                'title': title,
-                'location': location,
                 'company_domain': company_domain,
                 'enrich_profile': enrich_profile,
+                'location': location,
+                'title': title,
+                'last_name': last_name,
             },
             data={
             },
             result_class=PersonLookupUrlEnrichResult
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def resolve_by_email(
         self,
         work_email: str,
-        enrich_profile: str,
-    ) -> ReverseEmailUrlEnrichResult:
+        enrich_profile: str = '',
+    ) -> Deferred:
         """Reverse Work Email Lookup Endpoint
         
                 Cost: 3 credits / successful request.
         Resolve LinkedIn Profile from a work email address
         
         :param work_email: Work email address of the user
         :type work_email: str
@@ -227,37 +234,39 @@
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
             please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
-        :return: An object of :class:`proxycurl.models.ReverseEmailUrlEnrichResult` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.ReverseEmailUrlEnrichResult`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/profile/resolve/email',
             params={
                 'work_email': work_email,
                 'enrich_profile': enrich_profile,
             },
             data={
             },
             result_class=ReverseEmailUrlEnrichResult
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def lookup_email(
         self,
-        callback_url: str,
         linkedin_profile_url: str,
-    ) -> ExtractionEmailResult:
+        callback_url: str = '',
+    ) -> Deferred:
         """Work Email Lookup Endpoint
         
                 Cost: 3 credits / request.
         Lookup work email address of a LinkedIn Person Profile.
 
         Email addresses returned are verified to not be role-based or catch-all emails. Email addresses
         returned by our API endpoint come with a 95+% deliverability guarantee
@@ -265,766 +274,788 @@
         **Endpoint behavior**
 
         *This endpoint* **_may not_** *return results immediately.*
 
         If you provided a webhook in your request parameter, our application will call your webhook with
         the result once. See `Webhook request` below.
         
-        :param callback_url: Webhook to notify your application when
-            the request has finished processing.
-        :type callback_url: str
         :param linkedin_profile_url: Linkedin Profile URL of the person you want to
             extract work email address from.
         :type linkedin_profile_url: str
-        :return: An object of :class:`proxycurl.models.ExtractionEmailResult` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.ExtractionEmailResult`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :param callback_url: Webhook to notify your application when
+            the request has finished processing.
+        :type callback_url: str
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/profile/email',
             params={
-                'callback_url': callback_url,
                 'linkedin_profile_url': linkedin_profile_url,
+                'callback_url': callback_url,
             },
             data={
             },
             result_class=ExtractionEmailResult
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def personal_contact(
         self,
         linkedin_profile_url: str,
-    ) -> PDLPhoneNumberResult:
+    ) -> Deferred:
         """Personal Contact Number Lookup Endpoint
         
                 Cost: 1 credit / contact number returned.
         Given an LinkedIn profile, returns a list of personal contact numbers belonging to this identity.
         
         :param linkedin_profile_url: LinkedIn Profile URL of the person you want to extract personal contact numbers from.
         :type linkedin_profile_url: str
-        :return: An object of :class:`proxycurl.models.PDLPhoneNumberResult` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.PDLPhoneNumberResult`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/contact-api/personal-contact',
             params={
                 'linkedin_profile_url': linkedin_profile_url,
             },
             data={
             },
             result_class=PDLPhoneNumberResult
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def personal_email(
         self,
         linkedin_profile_url: str,
-        email_validation: str,
-    ) -> PDLEmailResult:
+        email_validation: str = '',
+    ) -> Deferred:
         """Personal Email Lookup Endpoint
         
                 Cost: 1 credit / email returned.
         Given an LinkedIn profile, returns a list of personal emails belonging to this identity. Emails are verified to be deliverable.
         
         :param linkedin_profile_url: LinkedIn Profile URL of the person you want to extract personal email addresses from.
         :type linkedin_profile_url: str
         :param email_validation: Perform deliverability validation on each email. (Costs 1 extra credit per email found).
 
             Takes the following values:
              * include - Perform email validation.
              * exclude (default) - Do not perform email validation.
         :type email_validation: str
-        :return: An object of :class:`proxycurl.models.PDLEmailResult` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.PDLEmailResult`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/contact-api/personal-email',
             params={
                 'linkedin_profile_url': linkedin_profile_url,
                 'email_validation': email_validation,
             },
             data={
             },
             result_class=PDLEmailResult
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def profile_picture(
         self,
         linkedin_person_profile_url: str,
-    ) -> ProfilePicture:
+    ) -> Deferred:
         """Person Profile Picture Endpoint
         
                 Cost: 0 credit / successful request.
         Get the profile picture of a person.
 
         Profile pictures are served from cached people profiles found within [LinkDB](https://nubela.co/proxycurl/linkdb).
         If the profile does not exist within [LinkDB](https://nubela.co/proxycurl/linkdb), then the API will return a `404` status code.
         
         :param linkedin_person_profile_url: LinkedIn Profile URL of the person that you are trying to get the profile picture of.
         :type linkedin_person_profile_url: str
-        :return: An object of :class:`proxycurl.models.ProfilePicture` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.ProfilePicture`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/person/profile-picture',
             params={
                 'linkedin_person_profile_url': linkedin_person_profile_url,
             },
             data={
             },
             result_class=ProfilePicture
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def person_search(
         self,
-        first_name: str,
-        last_name: str,
-        follower_count_min: str,
-        follower_count_max: str,
-        occupation: str,
-        headline: str,
-        summary: str,
-        country: str,
-        country_full_name: str,
-        city: str,
-        state: str,
-        connections_min: str,
-        connections_max: str,
-        birth_date_after: str,
-        birth_date_before: str,
-        page_size: str,
-        enrich_profiles: str,
-    ) -> PersonSearchResult:
+        enrich_profiles: str = '',
+        page_size: str = '',
+        birth_date_before: str = '',
+        birth_date_after: str = '',
+        connections_max: str = '',
+        connections_min: str = '',
+        state: str = '',
+        city: str = '',
+        country_full_name: str = '',
+        country: str = '',
+        summary: str = '',
+        headline: str = '',
+        occupation: str = '',
+        follower_count_max: str = '',
+        follower_count_min: str = '',
+        last_name: str = '',
+        first_name: str = '',
+    ) -> Deferred:
         """Person Search Endpoint
         
                 Cost: 35 credits / request.
         Search for people that meet a set of criteria within our exhaustive dataset of people profiles.
 
         This API endpoint is powered by [LinkDB](https://nubela.co/proxycurl/linkdb), our exhaustive dataset of people and company profiles.
         
-        :param first_name: Filter people by their first names by matching it against a regular expression.
+        :param enrich_profiles: Get the full profile data of people returned instead of only their LinkedIn profile URLs.
 
-            The default value of this parameter is `null`.
+            Each request respond with a streaming response of profiles.
 
-            The accepted value is a regular expression (regex).
-        :type first_name: str
-        :param last_name: Filter people by their last names by matching it against a regular expression.
+            The valid values are:
+
+            * `skip` (default): lists employee's profile url
+            * `enrich`: lists full profile of employees
+
+            Calling this API endpoint with this parameter would add `1` credit per result returned.
+        :type enrich_profiles: str
+        :param page_size: Tune the maximum results returned per API call.
+
+            The default value of this parameter is `100`.
+
+            Accepted values for this parameter is an integer ranging from `1` to `100`.
+        :type page_size: str
+        :param birth_date_before: Filter people with a birth date *less than* a value given in this parameter.
 
             The default value of this parameter is `null`.
+        :type birth_date_before: str
+        :param birth_date_after: Filter people with a birth date *more than* a value given in this parameter.
 
-            The accepted value is a regular expression (regex).
-        :type last_name: str
-        :param follower_count_min: Filter people with a LinkedIn follower count *more than* a value given in this parameter.
+            The default value of this parameter is `null`.
+        :type birth_date_after: str
+        :param connections_max: Filter people with a LinkedIn connection count *less than* a value given in this parameter.
 
             The default value of this parameter is `null`.
-        :type follower_count_min: str
-        :param follower_count_max: Filter people with a LinkedIn follower count *less than* a value given in this parameter.
+        :type connections_max: str
+        :param connections_min: Filter people with a LinkedIn connection count *more than* a value given in this parameter.
 
             The default value of this parameter is `null`.
-        :type follower_count_max: str
-        :param occupation: Filter people by their occupations by matching it against a regular expression.
+        :type connections_min: str
+        :param state: Filter people by their states by matching it against a regular expression.
 
             The default value of this parameter is `null`.
 
             The accepted value is a regular expression (regex).
-        :type occupation: str
-        :param headline: Filter people by their headlines by matching it against a regular expression.
+        :type state: str
+        :param city: Filter people by their cities by matching it against a regular expression.
 
             The default value of this parameter is `null`.
 
             The accepted value is a regular expression (regex).
-        :type headline: str
-        :param summary: Filter people by their summaries by matching it against a regular expression.
+        :type city: str
+        :param country_full_name: Filter people by their countries (in English words) by matching it against a regular expression.
 
             The default value of this parameter is `null`.
 
             The accepted value is a regular expression (regex).
-        :type summary: str
+        :type country_full_name: str
         :param country: Filter people by their countries (depicted by a 2-letter country code (ISO 3166-1 alpha-2)) by matching it against a regular expression.
 
             The default value of this parameter is `null`.
 
             The accepted value is a regular expression (regex).
         :type country: str
-        :param country_full_name: Filter people by their countries (in English words) by matching it against a regular expression.
+        :param summary: Filter people by their summaries by matching it against a regular expression.
 
             The default value of this parameter is `null`.
 
             The accepted value is a regular expression (regex).
-        :type country_full_name: str
-        :param city: Filter people by their cities by matching it against a regular expression.
+        :type summary: str
+        :param headline: Filter people by their headlines by matching it against a regular expression.
 
             The default value of this parameter is `null`.
 
             The accepted value is a regular expression (regex).
-        :type city: str
-        :param state: Filter people by their states by matching it against a regular expression.
+        :type headline: str
+        :param occupation: Filter people by their occupations by matching it against a regular expression.
 
             The default value of this parameter is `null`.
 
             The accepted value is a regular expression (regex).
-        :type state: str
-        :param connections_min: Filter people with a LinkedIn connection count *more than* a value given in this parameter.
-
-            The default value of this parameter is `null`.
-        :type connections_min: str
-        :param connections_max: Filter people with a LinkedIn connection count *less than* a value given in this parameter.
+        :type occupation: str
+        :param follower_count_max: Filter people with a LinkedIn follower count *less than* a value given in this parameter.
 
             The default value of this parameter is `null`.
-        :type connections_max: str
-        :param birth_date_after: Filter people with a birth date *more than* a value given in this parameter.
+        :type follower_count_max: str
+        :param follower_count_min: Filter people with a LinkedIn follower count *more than* a value given in this parameter.
 
             The default value of this parameter is `null`.
-        :type birth_date_after: str
-        :param birth_date_before: Filter people with a birth date *less than* a value given in this parameter.
+        :type follower_count_min: str
+        :param last_name: Filter people by their last names by matching it against a regular expression.
 
             The default value of this parameter is `null`.
-        :type birth_date_before: str
-        :param page_size: Tune the maximum results returned per API call.
-
-            The default value of this parameter is `100`.
 
-            Accepted values for this parameter is an integer ranging from `1` to `100`.
-        :type page_size: str
-        :param enrich_profiles: Get the full profile data of people returned instead of only their LinkedIn profile URLs.
-
-            Each request respond with a streaming response of profiles.
-
-            The valid values are:
+            The accepted value is a regular expression (regex).
+        :type last_name: str
+        :param first_name: Filter people by their first names by matching it against a regular expression.
 
-            * `skip` (default): lists employee's profile url
-            * `enrich`: lists full profile of employees
+            The default value of this parameter is `null`.
 
-            Calling this API endpoint with this parameter would add `1` credit per result returned.
-        :type enrich_profiles: str
-        :return: An object of :class:`proxycurl.models.PersonSearchResult` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.PersonSearchResult`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+            The accepted value is a regular expression (regex).
+        :type first_name: str
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/search/person',
             params={
-                'first_name': first_name,
-                'last_name': last_name,
-                'follower_count_min': follower_count_min,
-                'follower_count_max': follower_count_max,
-                'occupation': occupation,
-                'headline': headline,
-                'summary': summary,
-                'country': country,
-                'country_full_name': country_full_name,
-                'city': city,
-                'state': state,
-                'connections_min': connections_min,
-                'connections_max': connections_max,
-                'birth_date_after': birth_date_after,
-                'birth_date_before': birth_date_before,
-                'page_size': page_size,
                 'enrich_profiles': enrich_profiles,
+                'page_size': page_size,
+                'birth_date_before': birth_date_before,
+                'birth_date_after': birth_date_after,
+                'connections_max': connections_max,
+                'connections_min': connections_min,
+                'state': state,
+                'city': city,
+                'country_full_name': country_full_name,
+                'country': country,
+                'summary': summary,
+                'headline': headline,
+                'occupation': occupation,
+                'follower_count_max': follower_count_max,
+                'follower_count_min': follower_count_min,
+                'last_name': last_name,
+                'first_name': first_name,
             },
             data={
             },
             result_class=PersonSearchResult
         )
+        defer.returnValue(resp)
 
 
 class _LinkedinCompany:
     def __init__(self, linkedin):
         self.linkedin = linkedin
 
+    @inlineCallbacks
     def get(
         self,
-        use_cache: str,
         url: str,
-        acquisitions: str,
-        exit_data: str,
-        extra: str,
-        funding_data: str,
-        categories: str,
-        resolve_numeric_id: str,
-    ) -> LinkedinCompany:
+        resolve_numeric_id: str = '',
+        categories: str = '',
+        funding_data: str = '',
+        extra: str = '',
+        exit_data: str = '',
+        acquisitions: str = '',
+        use_cache: str = '',
+    ) -> Deferred:
         """Company Profile Endpoint
         
                 Cost: 1 credit / successful request.
         Get structured data of a Company Profile
         
-        :param use_cache: `if-present` The default behavior. Fetches profile from cache regardless of age of profile. If profile is not available in cache, API will attempt to source profile externally.
-
-            `if-recent` API will make a best effort to return a fresh profile no older than 29 days.Costs an extra `1` credit on top of the cost of the base endpoint.
-        :type use_cache: str
         :param url: URL of the LinkedIn Company Profile to crawl.
 
             URL should be in the format of `https://www.linkedin.com/company/<public_identifier>`
         :type url: str
-        :param acquisitions: Provides further enriched data on acquisitions made by this company from external sources.
+        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator.
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb).
+            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
+
+            This parameter accepts the following values:
+            - `false` (default value) - Will not resolve numerical IDs.
+            - `true` - Enable support for Company Profile URLs with numerical IDs.
+            Costs an extra `2` credit on top of the base cost of the endpoint.
+        :type resolve_numeric_id: str
+        :param categories: Appends categories data of this company.
 
             Default value is `"exclude"`.
-            The other acceptable value is `"include"`, which will include these acquisition data (if available) for `1` extra credit.
-        :type acquisitions: str
-        :param exit_data: Returns a list of investment portfolio exits.
+            The other acceptable value is `"include"`, which will include these categories (if available) for `1` extra credit.
+        :type categories: str
+        :param funding_data: Returns a list of funding rounds that this company has received.
 
             Default value is `"exclude"`.
             The other acceptable value is `"include"`, which will include these categories (if available) for `1` extra credit.
-        :type exit_data: str
+        :type funding_data: str
         :param extra: Enriches the Company Profile with extra details from external sources.
             Details include Crunchbase ranking, contact email, phone number, Facebook account, Twitter account, funding rounds and amount, IPO status, investor information, etc.
 
             Default value is `"exclude"`.
             The other acceptable value is `"include"`, which will include these extra details (if available) for `1` extra credit.
         :type extra: str
-        :param funding_data: Returns a list of funding rounds that this company has received.
+        :param exit_data: Returns a list of investment portfolio exits.
 
             Default value is `"exclude"`.
             The other acceptable value is `"include"`, which will include these categories (if available) for `1` extra credit.
-        :type funding_data: str
-        :param categories: Appends categories data of this company.
+        :type exit_data: str
+        :param acquisitions: Provides further enriched data on acquisitions made by this company from external sources.
 
             Default value is `"exclude"`.
-            The other acceptable value is `"include"`, which will include these categories (if available) for `1` extra credit.
-        :type categories: str
-        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator.
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb).
-            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
+            The other acceptable value is `"include"`, which will include these acquisition data (if available) for `1` extra credit.
+        :type acquisitions: str
+        :param use_cache: `if-present` The default behavior. Fetches profile from cache regardless of age of profile. If profile is not available in cache, API will attempt to source profile externally.
 
-            This parameter accepts the following values:
-            - `false` (default value) - Will not resolve numerical IDs.
-            - `true` - Enable support for Company Profile URLs with numerical IDs.
-            Costs an extra `2` credit on top of the base cost of the endpoint.
-        :type resolve_numeric_id: str
-        :return: An object of :class:`proxycurl.models.LinkedinCompany` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.LinkedinCompany`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+            `if-recent` API will make a best effort to return a fresh profile no older than 29 days.Costs an extra `1` credit on top of the cost of the base endpoint.
+        :type use_cache: str
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/company',
             params={
-                'use_cache': use_cache,
                 'url': url,
-                'acquisitions': acquisitions,
-                'exit_data': exit_data,
-                'extra': extra,
-                'funding_data': funding_data,
-                'categories': categories,
                 'resolve_numeric_id': resolve_numeric_id,
+                'categories': categories,
+                'funding_data': funding_data,
+                'extra': extra,
+                'exit_data': exit_data,
+                'acquisitions': acquisitions,
+                'use_cache': use_cache,
             },
             data={
             },
             result_class=LinkedinCompany
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def resolve(
         self,
-        enrich_profile: str,
-        company_name: str,
-        company_domain: str,
-        company_location: str,
-    ) -> CompanyUrlEnrichResult:
+        company_location: str = '',
+        company_domain: str = '',
+        company_name: str = '',
+        enrich_profile: str = '',
+    ) -> Deferred:
         """Company Lookup Endpoint
         
                 Cost: 2 credits / successful request.
         Resolve Company LinkedIn Profile from company name,
             domain name and location.
         
+        :param company_location: The location / region of company.
+            ISO 3166-1 alpha-2 codes
+        :type company_location: str
+        :param company_domain: Company website or Company domain
+            Requires either `company_domain` or `company_name`
+        :type company_domain: str
+        :param company_name: Company Name
+            Requires either `company_domain` or `company_name`
+        :type company_name: str
         :param enrich_profile: Enrich the result with a cached profile of the lookup result.
 
             The valid values are:
 
             * `skip` (default): do not enrich the results with cached profile data
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
             please chain this API call with the [Company Profile Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
-        :param company_name: Company Name
-            Requires either `company_domain` or `company_name`
-        :type company_name: str
-        :param company_domain: Company website or Company domain
-            Requires either `company_domain` or `company_name`
-        :type company_domain: str
-        :param company_location: The location / region of company.
-            ISO 3166-1 alpha-2 codes
-        :type company_location: str
-        :return: An object of :class:`proxycurl.models.CompanyUrlEnrichResult` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.CompanyUrlEnrichResult`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/company/resolve',
             params={
-                'enrich_profile': enrich_profile,
-                'company_name': company_name,
-                'company_domain': company_domain,
                 'company_location': company_location,
+                'company_domain': company_domain,
+                'company_name': company_name,
+                'enrich_profile': enrich_profile,
             },
             data={
             },
             result_class=CompanyUrlEnrichResult
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def find_job(
         self,
-        search_id: str,
-        keyword: str,
-        geo_id: str,
-        flexibility: str,
-        when: str,
-        experience_level: str,
-        job_type: str,
-    ) -> JobListPage:
+        job_type: str = '',
+        experience_level: str = '',
+        when: str = '',
+        flexibility: str = '',
+        geo_id: str = '',
+        keyword: str = '',
+        search_id: str = '',
+    ) -> Deferred:
         """Jobs Listing Endpoint
         
                 Cost: 2 credits / successful request.
         List jobs posted by a company on LinkedIn
         
-        :param search_id: The `search_id` of the company on LinkedIn.
-            You can get the `search_id` of a LinkedIn company via
-            [Company Profile API](#company-api-company-profile-endpoint).
-        :type search_id: str
-        :param keyword: The keyword to search for.
-        :type keyword: str
-        :param geo_id: The `geo_id` of the location to search for.
-            For example, `92000000` is the `geo_id` of world wide.
-
-            See [this article](https://nubela.co/blog/how-to-fetch-geo_id-parameter-for-the-job-api/?utm_source=blog&utm_medium=web&utm_campaign=docs-redirect-to-geo_id-article) as to how you may be able to match regions to `geo_id` input values.
-        :type geo_id: str
-        :param flexibility: The flexibility of the job.
-            It accepts the following 3 case insensitive values only:
-            - `remote`
-            - `on-site`
-            - `hybrid`
+        :param job_type: The nature of the job.
+            It accepts the following 7 case-insensitive values only:
+            - `full-time`
+            - `part-time`
+            - `contract`
+            - `internship`
+            - `temporary`
+            - `volunteer`
             - `anything` (default)
-        :type flexibility: str
-        :param when: The time when the job is posted,
-            It accepts the following case-insensitive values only:
-            - `yesterday`
-            - `past-week`
-            - `past-month`
-            - `anytime` (default)
-        :type when: str
+        :type job_type: str
         :param experience_level: The experience level needed for the job.
             It accepts the following 6 case-insensitive values only:
             - `internship`
             - `entry_level`
             - `associate`
             - `mid_senior_level`
             - `director`
             - `anything` (default)
         :type experience_level: str
-        :param job_type: The nature of the job.
-            It accepts the following 7 case-insensitive values only:
-            - `full-time`
-            - `part-time`
-            - `contract`
-            - `internship`
-            - `temporary`
-            - `volunteer`
+        :param when: The time when the job is posted,
+            It accepts the following case-insensitive values only:
+            - `yesterday`
+            - `past-week`
+            - `past-month`
+            - `anytime` (default)
+        :type when: str
+        :param flexibility: The flexibility of the job.
+            It accepts the following 3 case insensitive values only:
+            - `remote`
+            - `on-site`
+            - `hybrid`
             - `anything` (default)
-        :type job_type: str
-        :return: An object of :class:`proxycurl.models.JobListPage` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.JobListPage`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :type flexibility: str
+        :param geo_id: The `geo_id` of the location to search for.
+            For example, `92000000` is the `geo_id` of world wide.
+
+            See [this article](https://nubela.co/blog/how-to-fetch-geo_id-parameter-for-the-job-api/?utm_source=blog&utm_medium=web&utm_campaign=docs-redirect-to-geo_id-article) as to how you may be able to match regions to `geo_id` input values.
+        :type geo_id: str
+        :param keyword: The keyword to search for.
+        :type keyword: str
+        :param search_id: The `search_id` of the company on LinkedIn.
+            You can get the `search_id` of a LinkedIn company via
+            [Company Profile API](#company-api-company-profile-endpoint).
+        :type search_id: str
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/v2/linkedin/company/job',
             params={
-                'search_id': search_id,
-                'keyword': keyword,
-                'geo_id': geo_id,
-                'flexibility': flexibility,
-                'when': when,
-                'experience_level': experience_level,
                 'job_type': job_type,
+                'experience_level': experience_level,
+                'when': when,
+                'flexibility': flexibility,
+                'geo_id': geo_id,
+                'keyword': keyword,
+                'search_id': search_id,
             },
             data={
             },
             result_class=JobListPage
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def job_count(
         self,
-        search_id: str,
-        keyword: str,
-        geo_id: str,
-        flexibility: str,
-        when: str,
-        experience_level: str,
-        job_type: str,
-    ) -> JobListCount:
+        job_type: str = '',
+        experience_level: str = '',
+        when: str = '',
+        flexibility: str = '',
+        geo_id: str = '',
+        keyword: str = '',
+        search_id: str = '',
+    ) -> Deferred:
         """Jobs Listing Count Endpoint
         
                 Cost: 2 credits / successful request.
         Count number of jobs posted by a company on LinkedIn
         
-        :param search_id: The `search_id` of the company on LinkedIn.
-            You can get the `search_id` of a LinkedIn company via
-            [Company Profile API](#company-api-company-profile-endpoint).
-        :type search_id: str
-        :param keyword: The keyword to search for.
-        :type keyword: str
-        :param geo_id: The `geo_id` of the location to search for.
-            For example, `92000000` is the `geo_id` of world wide.
-
-            See [this article](https://nubela.co/blog/how-to-fetch-geo_id-parameter-for-the-job-api/?utm_source=blog&utm_medium=web&utm_campaign=docs-redirect-to-geo_id-article) as to how you may be able to match regions to `geo_id` input values.
-        :type geo_id: str
-        :param flexibility: The flexibility of the job.
-            It accepts the following 3 case insensitive values only:
-            - `remote`
-            - `on-site`
-            - `hybrid`
+        :param job_type: The nature of the job.
+            It accepts the following 7 case-insensitive values only:
+            - `full-time`
+            - `part-time`
+            - `contract`
+            - `internship`
+            - `temporary`
+            - `volunteer`
             - `anything` (default)
-        :type flexibility: str
-        :param when: The time when the job is posted,
-            It accepts the following case-insensitive values only:
-            - `yesterday`
-            - `past-week`
-            - `past-month`
-            - `anytime` (default)
-        :type when: str
+        :type job_type: str
         :param experience_level: The experience level needed for the job.
             It accepts the following 6 case-insensitive values only:
             - `internship`
             - `entry_level`
             - `associate`
             - `mid_senior_level`
             - `director`
             - `anything` (default)
         :type experience_level: str
-        :param job_type: The nature of the job.
-            It accepts the following 7 case-insensitive values only:
-            - `full-time`
-            - `part-time`
-            - `contract`
-            - `internship`
-            - `temporary`
-            - `volunteer`
+        :param when: The time when the job is posted,
+            It accepts the following case-insensitive values only:
+            - `yesterday`
+            - `past-week`
+            - `past-month`
+            - `anytime` (default)
+        :type when: str
+        :param flexibility: The flexibility of the job.
+            It accepts the following 3 case insensitive values only:
+            - `remote`
+            - `on-site`
+            - `hybrid`
             - `anything` (default)
-        :type job_type: str
-        :return: An object of :class:`proxycurl.models.JobListCount` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.JobListCount`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :type flexibility: str
+        :param geo_id: The `geo_id` of the location to search for.
+            For example, `92000000` is the `geo_id` of world wide.
+
+            See [this article](https://nubela.co/blog/how-to-fetch-geo_id-parameter-for-the-job-api/?utm_source=blog&utm_medium=web&utm_campaign=docs-redirect-to-geo_id-article) as to how you may be able to match regions to `geo_id` input values.
+        :type geo_id: str
+        :param keyword: The keyword to search for.
+        :type keyword: str
+        :param search_id: The `search_id` of the company on LinkedIn.
+            You can get the `search_id` of a LinkedIn company via
+            [Company Profile API](#company-api-company-profile-endpoint).
+        :type search_id: str
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/v2/linkedin/company/job/count',
             params={
-                'search_id': search_id,
-                'keyword': keyword,
-                'geo_id': geo_id,
-                'flexibility': flexibility,
-                'when': when,
-                'experience_level': experience_level,
                 'job_type': job_type,
+                'experience_level': experience_level,
+                'when': when,
+                'flexibility': flexibility,
+                'geo_id': geo_id,
+                'keyword': keyword,
+                'search_id': search_id,
             },
             data={
             },
             result_class=JobListCount
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def employee_count(
         self,
         url: str,
-        employment_status: str,
-        linkedin_employee_count: str,
-        use_cache: str,
-    ) -> EmployeeCount:
+        use_cache: str = '',
+        linkedin_employee_count: str = '',
+        employment_status: str = '',
+    ) -> Deferred:
         """Employee Count Endpoint
         
                 Cost: 1 credit / successful request.
         Get a number of total employees of a Company.
 
         Get an employee count of this company from various sources.
         
         :param url: URL of the LinkedIn Company Profile to target.
 
             URL should be in the format of `https://www.linkedin.com/company/<public_identifier>`
         :type url: str
-        :param employment_status: Parameter to tell the API to filter past or current employees.
-
-            Valid values are `current`, `past`, and `all`:
+        :param use_cache: `if-present`: The default behavior. Fetches data from LinkDB cache regardless of age of profile.
 
-            * `current` (default) : count current employees
-            * `past` : count past employees
-            * `all` : count current & past employees
-        :type employment_status: str
+            `if-recent`: API will make a best effort to return a fresh data no older than 29 days. Costs an extra 1 credit on top of the cost of the base endpoint.
+        :type use_cache: str
         :param linkedin_employee_count: Option to include a scraped employee count value from the target company's LinkedIn profile.
 
             Valid values are `include` and `exclude`:
 
             * `exclude` (default) : To exclude the scraped employee count.
             * `include` : To include the scraped employee count.
 
             Costs an extra `1` credit on top of the base cost of the endpoint.
         :type linkedin_employee_count: str
-        :param use_cache: `if-present`: The default behavior. Fetches data from LinkDB cache regardless of age of profile.
+        :param employment_status: Parameter to tell the API to filter past or current employees.
 
-            `if-recent`: API will make a best effort to return a fresh data no older than 29 days. Costs an extra 1 credit on top of the cost of the base endpoint.
-        :type use_cache: str
-        :return: An object of :class:`proxycurl.models.EmployeeCount` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.EmployeeCount`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+            Valid values are `current`, `past`, and `all`:
+
+            * `current` (default) : count current employees
+            * `past` : count past employees
+            * `all` : count current & past employees
+        :type employment_status: str
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/company/employees/count',
             params={
                 'url': url,
-                'employment_status': employment_status,
-                'linkedin_employee_count': linkedin_employee_count,
                 'use_cache': use_cache,
+                'linkedin_employee_count': linkedin_employee_count,
+                'employment_status': employment_status,
             },
             data={
             },
             result_class=EmployeeCount
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def employee_list(
         self,
         url: str,
-        resolve_numeric_id: str,
-        sort_by: str,
-        employment_status: str,
-        page_size: str,
-        role_search: str,
-        enrich_profiles: str,
-        country: str,
-    ) -> EmployeeList:
+        country: str = '',
+        enrich_profiles: str = '',
+        role_search: str = '',
+        page_size: str = '',
+        employment_status: str = '',
+        sort_by: str = '',
+        resolve_numeric_id: str = '',
+    ) -> Deferred:
         """Employee Listing Endpoint
         
                 Cost: 3 credits / employee returned.
         Get a list of employees of a Company.
 
         This API endpoint is limited by LinkDB which is populated with profiles in the US, UK, Canada, Israel, Australia, Ireland, New Zealand and Singapore.
         As such, this endpoint is best used to list employees working in companies based in those locations only.
         
         :param url: URL of the LinkedIn Company Profile to target.
 
             URL should be in the format of `https://www.linkedin.com/company/<public_identifier>`
         :type url: str
-        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
-            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
-
-            This parameter accepts the following values:
-            - `false` (default value) - Will not resolve numerical IDs.
-            - `true` - Enable support for Company Profile URLs with numerical IDs. 
-            Costs an extra `2` credit on top of the base cost of the endpoint.
-        :type resolve_numeric_id: str
-        :param sort_by: Sort employees by recency.
-
-            Valid values are:
-            * `recently-joined` - Sort employees by their join date. The most recent employee is on the top of the list.
-            * `recently-left` - Sort employees by their departure date. The most recent employee who had just left is on the top of this list.
-            * `none` - The default value. Do not sort.
+        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
 
-            If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per employee returned.
-        :type sort_by: str
-        :param employment_status: Parameter to tell the API to return past or current employees.
+            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
 
-            Valid values are `current`, `past`, and `all`:
+            Costs an extra `3` credit per result returned.
+        :type country: str
+        :param enrich_profiles: Get the full profile of employees instead of only their profile urls.
 
-            * `current` (default) : lists current employees
-            * `past` : lists past employees
-            * `all` : lists current & past employees
-        :type employment_status: str
-        :param page_size: Tune the maximum results returned per API call.
+            Each request respond with a streaming response of profiles.
 
-            The default value of this parameter is `200000`.
+            The valid values are:
 
-            Accepted values for this parameter is an integer ranging from `1` to `200000`.
+            * `skip` (default): lists employee's profile url
+            * `enrich`: lists full profile of employees
 
-            When `enrich_profiles=enrich`, this parameter accepts value ranging from `1` to `100`.
-        :type page_size: str
+            Calling this API endpoint with this parameter would add `1` credit per employee returned.
+        :type enrich_profiles: str
         :param role_search: Filter employees by their title by matching the employee's title against a *regular expression*.
 
             The default value of this parameter is `null`.
 
             The accepted value is a *regular expression* (regex).
 
             (The base cost of calling this API endpoint with this parameter would be `10` credits.
             Each employee matched and returned would cost `6` credits per employee returned.)
         :type role_search: str
-        :param enrich_profiles: Get the full profile of employees instead of only their profile urls.
+        :param page_size: Tune the maximum results returned per API call.
 
-            Each request respond with a streaming response of profiles.
+            The default value of this parameter is `200000`.
 
-            The valid values are:
+            Accepted values for this parameter is an integer ranging from `1` to `200000`.
 
-            * `skip` (default): lists employee's profile url
-            * `enrich`: lists full profile of employees
+            When `enrich_profiles=enrich`, this parameter accepts value ranging from `1` to `100`.
+        :type page_size: str
+        :param employment_status: Parameter to tell the API to return past or current employees.
 
-            Calling this API endpoint with this parameter would add `1` credit per employee returned.
-        :type enrich_profiles: str
-        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
+            Valid values are `current`, `past`, and `all`:
 
-            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
+            * `current` (default) : lists current employees
+            * `past` : lists past employees
+            * `all` : lists current & past employees
+        :type employment_status: str
+        :param sort_by: Sort employees by recency.
 
-            Costs an extra `3` credit per result returned.
-        :type country: str
-        :return: An object of :class:`proxycurl.models.EmployeeList` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.EmployeeList`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+            Valid values are:
+            * `recently-joined` - Sort employees by their join date. The most recent employee is on the top of the list.
+            * `recently-left` - Sort employees by their departure date. The most recent employee who had just left is on the top of this list.
+            * `none` - The default value. Do not sort.
+
+            If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per employee returned.
+        :type sort_by: str
+        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
+            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
+
+            This parameter accepts the following values:
+            - `false` (default value) - Will not resolve numerical IDs.
+            - `true` - Enable support for Company Profile URLs with numerical IDs. 
+            Costs an extra `2` credit on top of the base cost of the endpoint.
+        :type resolve_numeric_id: str
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/company/employees',
             params={
                 'url': url,
-                'resolve_numeric_id': resolve_numeric_id,
-                'sort_by': sort_by,
-                'employment_status': employment_status,
-                'page_size': page_size,
-                'role_search': role_search,
-                'enrich_profiles': enrich_profiles,
                 'country': country,
+                'enrich_profiles': enrich_profiles,
+                'role_search': role_search,
+                'page_size': page_size,
+                'employment_status': employment_status,
+                'sort_by': sort_by,
+                'resolve_numeric_id': resolve_numeric_id,
             },
             data={
             },
             result_class=EmployeeList
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def role_lookup(
         self,
         company_name: str,
         role: str,
-        enrich_profile: str,
-    ) -> RoleSearchErichedResult:
+        enrich_profile: str = '',
+    ) -> Deferred:
         """Role Lookup Endpoint
         
                 Cost: 3 credits / successful request.
         Finds the closest (person) profile with a given role in a Company.
         For example, you can use this endpoint to find the "CTO" of "Apple".
         This API endpoint returns only one result that is the closest match.
 
@@ -1048,293 +1079,303 @@
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
             please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
-        :return: An object of :class:`proxycurl.models.RoleSearchErichedResult` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.RoleSearchErichedResult`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/find/company/role',
             params={
                 'company_name': company_name,
                 'role': role,
                 'enrich_profile': enrich_profile,
             },
             data={
             },
             result_class=RoleSearchErichedResult
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def reveal(
         self,
         ip: str,
-        role: str,
-        role_personal_email: str,
-        role_contact_number: str,
-    ) -> CompanyReveal:
+        role_contact_number: str = '',
+        role_personal_email: str = '',
+        role: str = '',
+    ) -> Deferred:
         """Reveal Endpoint
         
                 Cost: 2 credits / successful request.
         Deanonymize an IPv4 address and associate the Company behind the IPv4 address.
         
         :param ip: The target IPv4 address.
         :type ip: str
+        :param role_contact_number: Append personal contact numbers to the response if the system finds a relevant person profile.
+        :type role_contact_number: str
+        :param role_personal_email: Append personal email addresses to the response if the system finds a relevant person profile.
+        :type role_personal_email: str
         :param role: Lookup and append an employee of a certain role of the company.
             Within the same API call, You can choose to lookup a person with a given role within this organisation that you might want to reach out to.
         :type role: str
-        :param role_personal_email: Append personal email addresses to the response if the system finds a relevant person profile.
-        :type role_personal_email: str
-        :param role_contact_number: Append personal contact numbers to the response if the system finds a relevant person profile.
-        :type role_contact_number: str
-        :return: An object of :class:`proxycurl.models.CompanyReveal` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.CompanyReveal`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/reveal/company',
             params={
                 'ip': ip,
-                'role': role,
-                'role_personal_email': role_personal_email,
                 'role_contact_number': role_contact_number,
+                'role_personal_email': role_personal_email,
+                'role': role,
             },
             data={
             },
             result_class=CompanyReveal
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def employees(
         self,
         url: str,
-        resolve_numeric_id: str,
-        sort_by: str,
-        employment_status: str,
-        page_size: str,
-        role_search: str,
-        enrich_profiles: str,
-        country: str,
-    ) -> EmployeeList:
+        country: str = '',
+        enrich_profiles: str = '',
+        role_search: str = '',
+        page_size: str = '',
+        employment_status: str = '',
+        sort_by: str = '',
+        resolve_numeric_id: str = '',
+    ) -> Deferred:
         """Employee Listing Endpoint
         
                 Cost: 3 credits / employee returned.
         Get a list of employees of a Company.
 
         This API endpoint is limited by LinkDB which is populated with profiles in the US, UK, Canada, Israel, Australia, Ireland, New Zealand and Singapore.
         As such, this endpoint is best used to list employees working in companies based in those locations only.
         
         :param url: URL of the LinkedIn Company Profile to target.
 
             URL should be in the format of `https://www.linkedin.com/company/<public_identifier>`
         :type url: str
-        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
-            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
-
-            This parameter accepts the following values:
-            - `false` (default value) - Will not resolve numerical IDs.
-            - `true` - Enable support for Company Profile URLs with numerical IDs. 
-            Costs an extra `2` credit on top of the base cost of the endpoint.
-        :type resolve_numeric_id: str
-        :param sort_by: Sort employees by recency.
-
-            Valid values are:
-            * `recently-joined` - Sort employees by their join date. The most recent employee is on the top of the list.
-            * `recently-left` - Sort employees by their departure date. The most recent employee who had just left is on the top of this list.
-            * `none` - The default value. Do not sort.
+        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
 
-            If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per employee returned.
-        :type sort_by: str
-        :param employment_status: Parameter to tell the API to return past or current employees.
+            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
 
-            Valid values are `current`, `past`, and `all`:
+            Costs an extra `3` credit per result returned.
+        :type country: str
+        :param enrich_profiles: Get the full profile of employees instead of only their profile urls.
 
-            * `current` (default) : lists current employees
-            * `past` : lists past employees
-            * `all` : lists current & past employees
-        :type employment_status: str
-        :param page_size: Tune the maximum results returned per API call.
+            Each request respond with a streaming response of profiles.
 
-            The default value of this parameter is `200000`.
+            The valid values are:
 
-            Accepted values for this parameter is an integer ranging from `1` to `200000`.
+            * `skip` (default): lists employee's profile url
+            * `enrich`: lists full profile of employees
 
-            When `enrich_profiles=enrich`, this parameter accepts value ranging from `1` to `100`.
-        :type page_size: str
+            Calling this API endpoint with this parameter would add `1` credit per employee returned.
+        :type enrich_profiles: str
         :param role_search: Filter employees by their title by matching the employee's title against a *regular expression*.
 
             The default value of this parameter is `null`.
 
             The accepted value is a *regular expression* (regex).
 
             (The base cost of calling this API endpoint with this parameter would be `10` credits.
             Each employee matched and returned would cost `6` credits per employee returned.)
         :type role_search: str
-        :param enrich_profiles: Get the full profile of employees instead of only their profile urls.
+        :param page_size: Tune the maximum results returned per API call.
 
-            Each request respond with a streaming response of profiles.
+            The default value of this parameter is `200000`.
 
-            The valid values are:
+            Accepted values for this parameter is an integer ranging from `1` to `200000`.
 
-            * `skip` (default): lists employee's profile url
-            * `enrich`: lists full profile of employees
+            When `enrich_profiles=enrich`, this parameter accepts value ranging from `1` to `100`.
+        :type page_size: str
+        :param employment_status: Parameter to tell the API to return past or current employees.
 
-            Calling this API endpoint with this parameter would add `1` credit per employee returned.
-        :type enrich_profiles: str
-        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
+            Valid values are `current`, `past`, and `all`:
 
-            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
+            * `current` (default) : lists current employees
+            * `past` : lists past employees
+            * `all` : lists current & past employees
+        :type employment_status: str
+        :param sort_by: Sort employees by recency.
 
-            Costs an extra `3` credit per result returned.
-        :type country: str
-        :return: An object of :class:`proxycurl.models.EmployeeList` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.EmployeeList`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+            Valid values are:
+            * `recently-joined` - Sort employees by their join date. The most recent employee is on the top of the list.
+            * `recently-left` - Sort employees by their departure date. The most recent employee who had just left is on the top of this list.
+            * `none` - The default value. Do not sort.
+
+            If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per employee returned.
+        :type sort_by: str
+        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
+            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
+
+            This parameter accepts the following values:
+            - `false` (default value) - Will not resolve numerical IDs.
+            - `true` - Enable support for Company Profile URLs with numerical IDs. 
+            Costs an extra `2` credit on top of the base cost of the endpoint.
+        :type resolve_numeric_id: str
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/company/employees',
             params={
                 'url': url,
-                'resolve_numeric_id': resolve_numeric_id,
-                'sort_by': sort_by,
-                'employment_status': employment_status,
-                'page_size': page_size,
-                'role_search': role_search,
-                'enrich_profiles': enrich_profiles,
                 'country': country,
+                'enrich_profiles': enrich_profiles,
+                'role_search': role_search,
+                'page_size': page_size,
+                'employment_status': employment_status,
+                'sort_by': sort_by,
+                'resolve_numeric_id': resolve_numeric_id,
             },
             data={
             },
             result_class=EmployeeList
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def employee_search(
         self,
-        resolve_numeric_id: str,
-        enrich_profiles: str,
-        country: str,
         keyword_regex: str,
         linkedin_company_profile_url: str,
-        page_size: str,
-    ) -> EmployeeList:
+        page_size: str = '',
+        country: str = '',
+        enrich_profiles: str = '',
+        resolve_numeric_id: str = '',
+    ) -> Deferred:
         """Employee Search Endpoint
         
                 Cost: 10 credits / successful request.
         Search employees of a target by their job title.
         This API endpoint is syntactic sugar for the role_search parameter under the [Employee Listing Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-listing-endpoint).
 
         Results are limited by data that we have within [LinkDB](https://nubela.co/proxycurl/linkdb).
         Use [Role Lookup API Endpoint](https://nubela.co/proxycurl/docs#people-api-role-lookup-endpoint) if you need to query for profiles without LinkDB constraints.
         The drawbacks of the Role Lookup API Endpoint is that it is less precise and can return at most one result per query.
         
-        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
-            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
+        :param keyword_regex: Job title keyword to search for in regular expression format.
+        :type keyword_regex: str
+        :param linkedin_company_profile_url: LinkedIn Profile URL of the target company.
+        :type linkedin_company_profile_url: str
+        :param page_size: Tune the maximum results returned per API call.
+            The default value of this parameter is `200000`.
+            Accepted values for this parameter is an integer ranging from `1` to `200000`.
+        :type page_size: str
+        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
 
-            This parameter accepts the following values:
-            - `false` (default value) - Will not resolve numerical IDs.
-            - `true` - Enable support for Company Profile URLs with numerical IDs. 
-            Costs an extra `2` credit on top of the base cost of the endpoint.
-        :type resolve_numeric_id: str
+            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
+
+            Costs an extra `3` credit per result returned.
+        :type country: str
         :param enrich_profiles: Get the full profile of employees instead of only their profile urls.
 
             Each request respond with a streaming response of profiles.
 
             The valid values are:
 
             * `skip` (default): lists employee's profile url
             * `enrich`: lists full profile of employees
 
             Calling this API endpoint with this parameter would add `1` credit per employee returned.
         :type enrich_profiles: str
-        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
-
-            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
+        :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
+            For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
 
-            Costs an extra `3` credit per result returned.
-        :type country: str
-        :param keyword_regex: Job title keyword to search for in regular expression format.
-        :type keyword_regex: str
-        :param linkedin_company_profile_url: LinkedIn Profile URL of the target company.
-        :type linkedin_company_profile_url: str
-        :param page_size: Tune the maximum results returned per API call.
-            The default value of this parameter is `200000`.
-            Accepted values for this parameter is an integer ranging from `1` to `200000`.
-        :type page_size: str
-        :return: An object of :class:`proxycurl.models.EmployeeList` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.EmployeeList`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+            This parameter accepts the following values:
+            - `false` (default value) - Will not resolve numerical IDs.
+            - `true` - Enable support for Company Profile URLs with numerical IDs. 
+            Costs an extra `2` credit on top of the base cost of the endpoint.
+        :type resolve_numeric_id: str
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/company/employee/search',
             params={
-                'resolve_numeric_id': resolve_numeric_id,
-                'enrich_profiles': enrich_profiles,
-                'country': country,
                 'keyword_regex': keyword_regex,
                 'linkedin_company_profile_url': linkedin_company_profile_url,
                 'page_size': page_size,
+                'country': country,
+                'enrich_profiles': enrich_profiles,
+                'resolve_numeric_id': resolve_numeric_id,
             },
             data={
             },
             result_class=EmployeeList
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def profile_picture(
         self,
         linkedin_company_profile_url: str,
-    ) -> ProfilePicture:
+    ) -> Deferred:
         """Company Profile Picture Endpoint
         
                 Cost: 0 credit / successful request.
         Get the profile picture of a company.
 
         Profile pictures are served from cached company profiles found within [LinkDB](https://nubela.co/proxycurl/linkdb).
         If the profile does not exist within [LinkDB](https://nubela.co/proxycurl/linkdb), then the API will return a `404` status code.
         
         :param linkedin_company_profile_url: LinkedIn Profile URL of the company that you are trying to get the profile picture of.
         :type linkedin_company_profile_url: str
-        :return: An object of :class:`proxycurl.models.ProfilePicture` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.ProfilePicture`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/company/profile-picture',
             params={
                 'linkedin_company_profile_url': linkedin_company_profile_url,
             },
             data={
             },
             result_class=ProfilePicture
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def find_role(
         self,
         company_name: str,
         role: str,
-        enrich_profile: str,
-    ) -> RoleSearchErichedResult:
+        enrich_profile: str = '',
+    ) -> Deferred:
         """Role Lookup Endpoint
         
                 Cost: 3 credits / successful request.
         Finds the closest (person) profile with a given role in a Company.
         For example, you can use this endpoint to find the "CTO" of "Apple".
         This API endpoint returns only one result that is the closest match.
 
@@ -1358,215 +1399,222 @@
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
             please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
-        :return: An object of :class:`proxycurl.models.RoleSearchErichedResult` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.RoleSearchErichedResult`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/find/company/role',
             params={
                 'company_name': company_name,
                 'role': role,
                 'enrich_profile': enrich_profile,
             },
             data={
             },
             result_class=RoleSearchErichedResult
         )
+        defer.returnValue(resp)
 
 
 class _LinkedinSchool:
     def __init__(self, linkedin):
         self.linkedin = linkedin
 
+    @inlineCallbacks
     def get(
         self,
-        use_cache: str,
         url: str,
-    ) -> LinkedinSchool:
+        use_cache: str = '',
+    ) -> Deferred:
         """School Profile Endpoint
         
                 Cost: 1 credit / successful request.
         Get structured data of a LinkedIn School Profile
         
-        :param use_cache: `if-present` The default behavior. Fetches profile from cache regardless of age of profile. If profile is not available in cache, API will attempt to source profile externally.
-
-            `if-recent` API will make a best effort to return a fresh profile no older than 29 days.Costs an extra `1` credit on top of the cost of the base endpoint.
-        :type use_cache: str
         :param url: URL of the LinkedIn School Profile to crawl.
 
             URL should be in the format of `https://www.linkedin.com/school/<public_identifier>`
         :type url: str
-        :return: An object of :class:`proxycurl.models.LinkedinSchool` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.LinkedinSchool`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :param use_cache: `if-present` The default behavior. Fetches profile from cache regardless of age of profile. If profile is not available in cache, API will attempt to source profile externally.
+
+            `if-recent` API will make a best effort to return a fresh profile no older than 29 days.Costs an extra `1` credit on top of the cost of the base endpoint.
+        :type use_cache: str
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/school',
             params={
-                'use_cache': use_cache,
                 'url': url,
+                'use_cache': use_cache,
             },
             data={
             },
             result_class=LinkedinSchool
         )
+        defer.returnValue(resp)
 
+    @inlineCallbacks
     def students(
         self,
         linkedin_school_url: str,
-        resolve_numeric_id: str,
-        sort_by: str,
-        student_status: str,
-        page_size: str,
-        search_keyword: str,
-        enrich_profiles: str,
-        country: str,
-    ) -> StudentList:
+        country: str = '',
+        enrich_profiles: str = '',
+        search_keyword: str = '',
+        page_size: str = '',
+        student_status: str = '',
+        sort_by: str = '',
+        resolve_numeric_id: str = '',
+    ) -> Deferred:
         """Student Listing Endpoint
         
                 Cost: 3 credits / student returned.
         Get a list of students of a school or university.
         
         :param linkedin_school_url: URL of the LinkedIn School Profile to target.
 
             URL should be in the format of `https://www.linkedin.com/school/<public_identifier>`
         :type linkedin_school_url: str
-        :param resolve_numeric_id: Enable support for School Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
-            For example, we will turn `https://www.linkedin.com/school/1234567890` to `https://www.linkedin.com/school/acme-corp` -- for which the API endpoint only supports the latter.
-
-            This parameter accepts the following values:
-            - `false` (default value) - Will not resolve numerical IDs.
-            - `true` - Enable support for School Profile URLs with numerical IDs. 
-            Costs an extra `2` credit on top of the base cost of the endpoint.
-        :type resolve_numeric_id: str
-        :param sort_by: Sort students by matriculation or graduation dates.
-
-            Valid values are:
-            * `recently-matriculated` - Sort students by their matriculation date. Students who had had most recently started school is on the top of the list.
-            * `recently-graduated` - Sort students by their graduation date. The most recently graduated student is on the top of this list.
-            * `none` - The default value. Do not sort.
+        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
 
-            If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per student returned.
-        :type sort_by: str
-        :param student_status: Parameter to tell the API to return past or current students.
+            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
 
-            Valid values are `current`, `past`, and `all`:
+            Costs an extra `3` credit per result returned.
+        :type country: str
+        :param enrich_profiles: Get the full profile of students instead of only their profile urls.
 
-            * `current` (default) : lists current students
-            * `past` : lists past students
-            * `all` : lists current & past students
-        :type student_status: str
-        :param page_size: Tune the maximum results returned per API call.
+            Each request respond with a streaming response of profiles.
 
-            The default value of this parameter is `200000`.
+            The valid values are:
 
-            Accepted values for this parameter is an integer ranging from `1` to `200000`.
+            * `skip` (default): lists student's profile url
+            * `enrich`: lists full profile of students
 
-            When `enrich_profiles=enrich`, this parameter accepts value ranging from `1` to `100`.
-        :type page_size: str
+            *Calling this API endpoint with this parameter would add `1` credit per student returned.*
+        :type enrich_profiles: str
         :param search_keyword: Filter students by their major by matching the student's major against a *regular expression*.
 
             The default value of this parameter is `null`.
 
             The accepted value is a *regular expression* (regex).
 
             (The base cost of calling this API endpoint with this parameter would be `10` credits.
             Each student matched and returned would cost `6` credits per student returned.)
         :type search_keyword: str
-        :param enrich_profiles: Get the full profile of students instead of only their profile urls.
+        :param page_size: Tune the maximum results returned per API call.
 
-            Each request respond with a streaming response of profiles.
+            The default value of this parameter is `200000`.
 
-            The valid values are:
+            Accepted values for this parameter is an integer ranging from `1` to `200000`.
 
-            * `skip` (default): lists student's profile url
-            * `enrich`: lists full profile of students
+            When `enrich_profiles=enrich`, this parameter accepts value ranging from `1` to `100`.
+        :type page_size: str
+        :param student_status: Parameter to tell the API to return past or current students.
 
-            *Calling this API endpoint with this parameter would add `1` credit per student returned.*
-        :type enrich_profiles: str
-        :param country: Limit the result set to the country locality of the profile. For example, set the parameter of `country=us` if you only want profiles from the US.
+            Valid values are `current`, `past`, and `all`:
 
-            This parameter accepts a **case-insensitive** [Alpha-2 ISO3166 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
+            * `current` (default) : lists current students
+            * `past` : lists past students
+            * `all` : lists current & past students
+        :type student_status: str
+        :param sort_by: Sort students by matriculation or graduation dates.
 
-            Costs an extra `3` credit per result returned.
-        :type country: str
-        :return: An object of :class:`proxycurl.models.StudentList` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.StudentList`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+            Valid values are:
+            * `recently-matriculated` - Sort students by their matriculation date. Students who had had most recently started school is on the top of the list.
+            * `recently-graduated` - Sort students by their graduation date. The most recently graduated student is on the top of this list.
+            * `none` - The default value. Do not sort.
+
+            If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per student returned.
+        :type sort_by: str
+        :param resolve_numeric_id: Enable support for School Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
+            For example, we will turn `https://www.linkedin.com/school/1234567890` to `https://www.linkedin.com/school/acme-corp` -- for which the API endpoint only supports the latter.
+
+            This parameter accepts the following values:
+            - `false` (default value) - Will not resolve numerical IDs.
+            - `true` - Enable support for School Profile URLs with numerical IDs. 
+            Costs an extra `2` credit on top of the base cost of the endpoint.
+        :type resolve_numeric_id: str
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/school/students',
             params={
                 'linkedin_school_url': linkedin_school_url,
-                'resolve_numeric_id': resolve_numeric_id,
-                'sort_by': sort_by,
-                'student_status': student_status,
-                'page_size': page_size,
-                'search_keyword': search_keyword,
-                'enrich_profiles': enrich_profiles,
                 'country': country,
+                'enrich_profiles': enrich_profiles,
+                'search_keyword': search_keyword,
+                'page_size': page_size,
+                'student_status': student_status,
+                'sort_by': sort_by,
+                'resolve_numeric_id': resolve_numeric_id,
             },
             data={
             },
             result_class=StudentList
         )
+        defer.returnValue(resp)
 
 
 class _LinkedinJob:
     def __init__(self, linkedin):
         self.linkedin = linkedin
 
+    @inlineCallbacks
     def get(
         self,
         url: str,
-    ) -> JobProfile:
+    ) -> Deferred:
         """Job Profile Endpoint
         
                 Cost: 2 credits / successful request.
         Get structured data of a LinkedIn Job Profile
         
         :param url: URL of the LinkedIn Job Profile to target.
 
             URL should be in the format of
             `https://www.linkedin.com/jobs/view/<job_id>`.
             [Jobs Listing Endpoint](#jobs-api-jobs-listing-endpoint)
             can be used to retrieve a job URL.
         :type url: str
-        :return: An object of :class:`proxycurl.models.JobProfile` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.JobProfile`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/linkedin/job',
             params={
                 'url': url,
             },
             data={
             },
             result_class=JobProfile
         )
+        defer.returnValue(resp)
 
 
 class _Linkedin:
     person: _LinkedinPerson
     company: _LinkedinCompany
     school: _LinkedinSchool
     job: _LinkedinJob
@@ -1593,30 +1641,32 @@
         self.api_key = api_key
         self.base_url = base_url
         self.timeout = timeout
         self.max_retries = max_retries
         self.max_backoff_seconds = max_backoff_seconds
         self.linkedin = _Linkedin(self)
 
+    @inlineCallbacks
     def get_balance(
         self,
-    ) -> CreditBalance:
+    ) -> Deferred:
         """View Credit Balance Endpoint
         
                 Cost: 0 credit / successful request.
         Get your current credit(s) balance
         
-        :return: An object of :class:`proxycurl.models.CreditBalance` or **None** if there is an error.
-        :rtype: :class:`proxycurl.models.CreditBalance`
-        :raise ProxycurlException: Every error will raise a :class:`proxycurl.gevent.ProxycurlException`
+        :return: An object of Deferred or **None** if there is an error.
+        :rtype: Deferred
+        :raise ProxycurlException: Every error will raise a :class:`proxycurl.twisted.ProxycurlException`
 
         """
 
-        return self.linkedin.proxycurl.request(
+        resp = yield self.linkedin.proxycurl.request(
             method='GET',
             url='/proxycurl/api/credit-balance',
             params={
             },
             data={
             },
             result_class=CreditBalance
         )
+        defer.returnValue(resp)
```

### Comparing `proxycurl-py-0.0.20/proxycurl_py/models.py` & `proxycurl_py-0.0.21/proxycurl_py/models.py`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.20/proxycurl_py/twisted/base.py` & `proxycurl_py-0.0.21/proxycurl_py/twisted/base.py`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.20/pyproject.toml` & `proxycurl_py-0.0.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proxycurl_py"
-version = "0.0.20"
+version = "0.0.21"
 description = ""
 readme = "README.md"
 authors = ["Nubela <tech@nubela.co>"]
 packages = [
     { include = "proxycurl_py"}
 ]
```

