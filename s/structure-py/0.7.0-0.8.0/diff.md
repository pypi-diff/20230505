# Comparing `tmp/structure_py-0.7.0.tar.gz` & `tmp/structure_py-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structure_py-0.7.0.tar", last modified: Wed May  3 01:00:07 2023, max compression
+gzip compressed data, was "structure_py-0.8.0.tar", last modified: Fri May  5 00:55:42 2023, max compression
```

## Comparing `structure_py-0.7.0.tar` & `structure_py-0.8.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:00:07.148160 structure_py-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 00:59:54.000000 structure_py-0.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-03 01:00:07.148160 structure_py-0.7.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3703 2023-05-03 00:59:54.000000 structure_py-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 01:00:07.148160 structure_py-0.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-05-03 00:59:54.000000 structure_py-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:00:07.144160 structure_py-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:00:07.144160 structure_py-0.7.0/src/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4614 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/companies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:00:07.144160 structure_py-0.7.0/src/sdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:00:07.144160 structure_py-0.7.0/src/sdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      695 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/operations/enrich_company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      701 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/operations/enrich_person.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/operations/list_employees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1072 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/operations/list_jobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      482 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/operations/list_users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      969 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/operations/login.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/operations/me.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1531 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/operations/search_companies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1514 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/operations/search_people.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:00:07.148160 structure_py-0.7.0/src/sdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/shared/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2597 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/shared/company.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7409 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/shared/person.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2695 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/people.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3225 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2603 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:00:07.148160 structure_py-0.7.0/src/sdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25540 2023-05-03 00:59:54.000000 structure_py-0.7.0/src/sdk/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:00:07.148160 structure_py-0.7.0/src/structure_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-03 01:00:06.000000 structure_py-0.7.0/src/structure_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-03 01:00:07.000000 structure_py-0.7.0/src/structure_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 01:00:06.000000 structure_py-0.7.0/src/structure_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-03 01:00:06.000000 structure_py-0.7.0/src/structure_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-03 01:00:06.000000 structure_py-0.7.0/src/structure_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:55:42.856708 structure_py-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 00:55:26.000000 structure_py-0.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-05 00:55:42.856708 structure_py-0.8.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3702 2023-05-05 00:55:26.000000 structure_py-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 00:55:42.856708 structure_py-0.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-05-05 00:55:26.000000 structure_py-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:55:42.852708 structure_py-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:55:42.852708 structure_py-0.8.0/src/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1518 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4634 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/companies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:55:42.852708 structure_py-0.8.0/src/sdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:55:42.856708 structure_py-0.8.0/src/sdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      695 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/operations/enrich_company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      701 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/operations/enrich_person.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/operations/list_employees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1072 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/operations/list_jobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      482 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/operations/list_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      969 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/operations/login.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/operations/me.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1531 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/operations/search_companies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1514 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/operations/search_people.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:55:42.856708 structure_py-0.8.0/src/sdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/shared/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2597 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/shared/company.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7409 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/shared/person.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2705 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/people.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3225 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2613 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:55:42.856708 structure_py-0.8.0/src/sdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25963 2023-05-05 00:55:26.000000 structure_py-0.8.0/src/sdk/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:55:42.856708 structure_py-0.8.0/src/structure_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-05 00:55:42.000000 structure_py-0.8.0/src/structure_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-05 00:55:42.000000 structure_py-0.8.0/src/structure_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:55:42.000000 structure_py-0.8.0/src/structure_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 00:55:42.000000 structure_py-0.8.0/src/structure_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 00:55:42.000000 structure_py-0.8.0/src/structure_py.egg-info/top_level.txt
```

### Comparing `structure_py-0.7.0/LICENSE.md` & `structure_py-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `structure_py-0.7.0/PKG-INFO` & `structure_py-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structure_py
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Structure
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -45,15 +45,14 @@
 
 s = sdk.SDK(
     security=shared.Security(
         bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE",
     ),
 )
 
-
 req = operations.EnrichCompanyRequest(
     id='89bd9d8d-69a6-474e-8f46-7cc8796ed151',
 )
 
 res = s.companies.enrich(req)
 
 if res.body is not None:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structure_py Version: 0.7.0 Summary: Python Client
+Metadata-Version: 2.1 Name: structure_py Version: 0.8.0 Summary: Python Client
 SDK Generated by Speakeasy Home-page: UNKNOWN Author: Structure License:
 UNKNOWN Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE.md
    [https://user-images.githubusercontent.com/6267663/229523981-b357a689-adc6-
                          4905-ac0e-e432aee5800b.png]
                            ****** Python SDK ******
                Discover rich information on people and companies
```

### Comparing `structure_py-0.7.0/README.md` & `structure_py-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
 s = sdk.SDK(
     security=shared.Security(
         bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE",
     ),
 )
 
-
 req = operations.EnrichCompanyRequest(
     id='89bd9d8d-69a6-474e-8f46-7cc8796ed151',
 )
 
 res = s.companies.enrich(req)
 
 if res.body is not None:
```

### Comparing `structure_py-0.7.0/setup.py` & `structure_py-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="structure_py",
-    version="0.7.0",
+    version="0.8.0",
     author="Structure",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `structure_py-0.7.0/src/sdk/accounts.py` & `structure_py-0.8.0/src/sdk/accounts.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
+    
     def list_users(self) -> operations.ListUsersResponse:
         r"""Show current user accounts"""
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/accounts'
```

### Comparing `structure_py-0.7.0/src/sdk/companies.py` & `structure_py-0.8.0/src/sdk/companies.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
+    
     def enrich(self, request: operations.EnrichCompanyRequest) -> operations.EnrichCompanyResponse:
         r"""Enrich a company profile"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.EnrichCompanyRequest, base_url, '/companies/{id}/enrich', request)
         
         
@@ -39,14 +40,15 @@
             if utils.match_content_type(content_type, '*/*'):
                 res.body = http_res.content
         elif http_res.status_code in [401, 403, 404, 422]:
             pass
 
         return res
 
+    
     def list_employees(self, request: operations.ListEmployeesRequest) -> operations.ListEmployeesResponse:
         r"""List company employees"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListEmployeesRequest, base_url, '/companies/{id}/employees', request)
         
         query_params = utils.get_query_params(operations.ListEmployeesRequest, request)
@@ -62,14 +64,15 @@
             if utils.match_content_type(content_type, '*/*'):
                 res.body = http_res.content
         elif http_res.status_code in [401, 403, 404]:
             pass
 
         return res
 
+    
     def list_jobs(self, request: operations.ListJobsRequest) -> operations.ListJobsResponse:
         r"""List company jobs"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListJobsRequest, base_url, '/companies/{id}/jobs', request)
         
         query_params = utils.get_query_params(operations.ListJobsRequest, request)
@@ -85,14 +88,15 @@
             if utils.match_content_type(content_type, '*/*'):
                 res.body = http_res.content
         elif http_res.status_code in [401, 403, 404]:
             pass
 
         return res
 
+    
     def search(self, request: operations.SearchCompaniesApplicationJSON) -> operations.SearchCompaniesResponse:
         r"""Search Companies"""
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/companies/search'
         
         headers = {}
```

### Comparing `structure_py-0.7.0/src/sdk/models/operations/__init__.py` & `structure_py-0.8.0/src/sdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.7.0/src/sdk/models/operations/enrich_company.py` & `structure_py-0.8.0/src/sdk/models/operations/enrich_company.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.7.0/src/sdk/models/operations/enrich_person.py` & `structure_py-0.8.0/src/sdk/models/operations/enrich_person.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.7.0/src/sdk/models/operations/list_employees.py` & `structure_py-0.8.0/src/sdk/models/operations/list_employees.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.7.0/src/sdk/models/operations/list_jobs.py` & `structure_py-0.8.0/src/sdk/models/operations/list_jobs.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.7.0/src/sdk/models/operations/login.py` & `structure_py-0.8.0/src/sdk/models/operations/login.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.7.0/src/sdk/models/operations/search_companies.py` & `structure_py-0.8.0/src/sdk/models/operations/search_companies.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.7.0/src/sdk/models/operations/search_people.py` & `structure_py-0.8.0/src/sdk/models/operations/search_people.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.7.0/src/sdk/models/shared/account.py` & `structure_py-0.8.0/src/sdk/models/shared/account.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.7.0/src/sdk/models/shared/company.py` & `structure_py-0.8.0/src/sdk/models/shared/company.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.7.0/src/sdk/models/shared/person.py` & `structure_py-0.8.0/src/sdk/models/shared/person.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.7.0/src/sdk/people.py` & `structure_py-0.8.0/src/sdk/people.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
+    
     def enrich(self, request: operations.EnrichPersonRequest) -> operations.EnrichPersonResponse:
         r"""Enrich a person profile"""
         base_url = self._server_url
         
         url = utils.generate_url(operations.EnrichPersonRequest, base_url, '/people/{id}/enrich', request)
         
         
@@ -39,14 +40,15 @@
             if utils.match_content_type(content_type, '*/*'):
                 res.body = http_res.content
         elif http_res.status_code in [401, 403, 404, 422]:
             pass
 
         return res
 
+    
     def search(self, request: operations.SearchPeopleApplicationJSON) -> operations.SearchPeopleResponse:
         r"""Search People"""
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/people/search'
         
         headers = {}
```

### Comparing `structure_py-0.7.0/src/sdk/sdk.py` & `structure_py-0.8.0/src/sdk/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     user: User
     r"""User"""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.7.0"
-    _gen_version: str = "2.24.0"
+    _sdk_version: str = "0.8.0"
+    _gen_version: str = "2.26.0"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `structure_py-0.7.0/src/sdk/user.py` & `structure_py-0.8.0/src/sdk/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
+    
     def login(self, request: operations.LoginApplicationJSON) -> operations.LoginResponse:
         r"""Login user"""
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/auths'
         
         headers = {}
@@ -45,14 +46,15 @@
             if utils.match_content_type(content_type, '*/*'):
                 res.body = http_res.content
         elif http_res.status_code == 401:
             pass
 
         return res
 
+    
     def me(self) -> operations.MeResponse:
         r"""Show current user"""
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/me'
```

### Comparing `structure_py-0.7.0/src/sdk/utils/retries.py` & `structure_py-0.8.0/src/sdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `structure_py-0.7.0/src/sdk/utils/utils.py` & `structure_py-0.8.0/src/sdk/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,16 @@
         if field_name == 'password':
             password = value
 
     data = f'{username}:{password}'.encode()
     client.client.headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> str:
+def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass,
+                 gbls: dict[str, dict[str, dict[str, Any]]] = None) -> str:
     path_param_fields: Tuple[Field, ...] = fields(clazz)
     for field in path_param_fields:
         request_metadata = field.metadata.get('request')
         if request_metadata is not None:
             continue
 
         param_metadata = field.metadata.get('path_param')
@@ -229,15 +230,16 @@
     for key, value in params.items():
         url_with_params = url_with_params.replace(
             '{' + key + '}', value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> dict[str, list[str]]:
+def get_query_params(clazz: type, query_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> dict[
+    str, list[str]]:
     params: dict[str, list[str]] = {}
 
     param_fields: Tuple[Field, ...] = fields(clazz)
     for field in param_fields:
         request_metadata = field.metadata.get('request')
         if request_metadata is not None:
             continue
@@ -263,16 +265,19 @@
                     params[key] = [value]
         else:
             style = metadata.get('style', 'form')
             if style == 'deepObject':
                 params = params | _get_deep_object_query_params(
                     metadata, f_name, value)
             elif style == 'form':
-                params = params | _get_form_query_params(
-                    metadata, f_name, value)
+                params = params | _get_delimited_query_params(
+                    metadata, f_name, value, ",")
+            elif style == 'pipeDelimited':
+                params = params | _get_delimited_query_params(
+                    metadata, f_name, value, "|")
             else:
                 raise Exception('not yet implemented')
     return params
 
 
 def get_headers(headers_params: dataclass) -> dict[str, str]:
     if headers_params is None:
@@ -323,20 +328,23 @@
                 continue
 
             if isinstance(obj_val, list):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
-                        params[f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
+                    if params.get(
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                        params[
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                         ]
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(_val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
+                        _val_to_string(val))
             else:
                 params[
                     f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                     _val_to_string(obj_val)]
     elif isinstance(obj, dict):
         for key, value in obj.items():
             if value is None:
@@ -364,48 +372,52 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_form_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name)
+def _get_delimited_query_params(metadata: dict, field_name: str, obj: any, array_delimiter: str) -> dict[
+    str, list[str]]:
+    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, array_delimiter)
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json':      'application/json',
-    'form':      'application/x-www-form-urlencoded',
+    'json': 'application/json',
+    'form': 'application/x-www-form-urlencoded',
     'multipart': 'multipart/form-data',
-    'raw':       'application/octet-stream',
-    'string':    'text/plain',
+    'raw': 'application/octet-stream',
+    'string': 'text/plain',
 }
 
 
-def serialize_request_body(request: dataclass, request_field_name: str, serialization_method: str) -> Tuple[str, any, any]:
+def serialize_request_body(request: dataclass, request_field_name: str, serialization_method: str) -> Tuple[
+    str, any, any]:
     if request is None:
         return None, None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method], request)
+        return serialize_content_type(request_field_name, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
+                                      request)
 
     request_val = getattr(request, request_field_name)
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
             request_metadata = field.metadata.get('request')
             break
 
     if request_metadata is None:
         raise Exception('invalid request type')
 
-    return serialize_content_type(request_field_name, request_metadata.get('media_type', 'application/octet-stream'), request_val)
+    return serialize_content_type(request_field_name, request_metadata.get('media_type', 'application/octet-stream'),
+                                  request_val)
 
 
 def serialize_content_type(field_name: str, media_type: str, request: dataclass) -> Tuple[str, any, list[list[any]]]:
     if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
         return media_type, marshal_json(request), None
     if re.match(r'multipart\/.*', media_type) is not None:
         return serialize_multipart_form(media_type, request)
@@ -470,15 +482,15 @@
                         [field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
 def serialize_dict(original: dict, explode: bool, field_name, existing: Optional[dict[str, list[str]]]) -> dict[
-        str, list[str]]:
+    str, list[str]]:
     if existing is None:
         existing = []
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -510,15 +522,15 @@
             field_name = metadata.get('field_name', field.name)
 
             if metadata.get('json'):
                 form[field_name] = [marshal_json(val)]
             else:
                 if metadata.get('style', 'form') == 'form':
                     form = form | _populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name)
+                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")
                 else:
                     raise Exception(
                         f'Invalid form style for field {field.name}')
     elif isinstance(data, dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
@@ -532,15 +544,16 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable) -> dict[str, list[str]]:
+def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable, array_delimiter: str) -> \
+        dict[str, list[str]]:
     params: dict[str, list[str]] = {}
 
     if obj is None:
         return params
 
     if is_dataclass(obj):
         items = []
@@ -587,15 +600,15 @@
                 if not field_name in params:
                     params[field_name] = []
                 params[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [','.join([str(item) for item in items])]
+            params[field_name] = [array_delimiter.join([str(item) for item in items])]
     else:
         params[field_name] = [_val_to_string(obj)]
 
     return params
 
 
 def _serialize_header(explode: bool, obj: any) -> str:
```

### Comparing `structure_py-0.7.0/src/structure_py.egg-info/PKG-INFO` & `structure_py-0.8.0/src/structure_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structure-py
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Structure
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -45,15 +45,14 @@
 
 s = sdk.SDK(
     security=shared.Security(
         bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE",
     ),
 )
 
-
 req = operations.EnrichCompanyRequest(
     id='89bd9d8d-69a6-474e-8f46-7cc8796ed151',
 )
 
 res = s.companies.enrich(req)
 
 if res.body is not None:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structure-py Version: 0.7.0 Summary: Python Client
+Metadata-Version: 2.1 Name: structure-py Version: 0.8.0 Summary: Python Client
 SDK Generated by Speakeasy Home-page: UNKNOWN Author: Structure License:
 UNKNOWN Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE.md
    [https://user-images.githubusercontent.com/6267663/229523981-b357a689-adc6-
                          4905-ac0e-e432aee5800b.png]
                            ****** Python SDK ******
                Discover rich information on people and companies
```

### Comparing `structure_py-0.7.0/src/structure_py.egg-info/SOURCES.txt` & `structure_py-0.8.0/src/structure_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

