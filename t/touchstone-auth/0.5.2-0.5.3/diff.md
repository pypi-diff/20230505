# Comparing `tmp/touchstone-auth-0.5.2.tar.gz` & `tmp/touchstone-auth-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "touchstone-auth-0.5.2.tar", last modified: Thu May  4 19:40:17 2023, max compression
+gzip compressed data, was "touchstone-auth-0.5.3.tar", last modified: Fri May  5 00:26:55 2023, max compression
```

## Comparing `touchstone-auth-0.5.2.tar` & `touchstone-auth-0.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-05-04 19:40:17.399894 touchstone-auth-0.5.2/
--rw-r--r--   0 christopher  (1000) christopher  (1000)     1075 2022-09-12 21:18:16.000000 touchstone-auth-0.5.2/LICENSE
--rw-r--r--   0 christopher  (1000) christopher  (1000)     9484 2023-05-04 19:40:17.396561 touchstone-auth-0.5.2/PKG-INFO
--rw-r--r--   0 christopher  (1000) christopher  (1000)     8842 2023-05-04 19:40:06.000000 touchstone-auth-0.5.2/README.md
--rw-r--r--   0 christopher  (1000) christopher  (1000)      103 2022-09-12 21:18:16.000000 touchstone-auth-0.5.2/pyproject.toml
--rw-r--r--   0 christopher  (1000) christopher  (1000)       38 2023-05-04 19:40:17.399894 touchstone-auth-0.5.2/setup.cfg
--rw-r--r--   0 christopher  (1000) christopher  (1000)     1104 2023-05-04 19:39:19.000000 touchstone-auth-0.5.2/setup.py
-drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-05-04 19:40:17.389894 touchstone-auth-0.5.2/src/
-drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-05-04 19:40:17.393227 touchstone-auth-0.5.2/src/touchstone_auth/
--rw-r--r--   0 christopher  (1000) christopher  (1000)    20936 2023-05-04 19:38:30.000000 touchstone-auth-0.5.2/src/touchstone_auth/__init__.py
-drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-05-04 19:40:17.396561 touchstone-auth-0.5.2/src/touchstone_auth.egg-info/
--rw-r--r--   0 christopher  (1000) christopher  (1000)     9484 2023-05-04 19:40:17.000000 touchstone-auth-0.5.2/src/touchstone_auth.egg-info/PKG-INFO
--rw-r--r--   0 christopher  (1000) christopher  (1000)      287 2023-05-04 19:40:17.000000 touchstone-auth-0.5.2/src/touchstone_auth.egg-info/SOURCES.txt
--rw-r--r--   0 christopher  (1000) christopher  (1000)        1 2023-05-04 19:40:17.000000 touchstone-auth-0.5.2/src/touchstone_auth.egg-info/dependency_links.txt
--rw-r--r--   0 christopher  (1000) christopher  (1000)       82 2023-05-04 19:40:17.000000 touchstone-auth-0.5.2/src/touchstone_auth.egg-info/requires.txt
--rw-r--r--   0 christopher  (1000) christopher  (1000)       16 2023-05-04 19:40:17.000000 touchstone-auth-0.5.2/src/touchstone_auth.egg-info/top_level.txt
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-05-05 00:26:55.129576 touchstone-auth-0.5.3/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     1075 2022-09-12 21:18:16.000000 touchstone-auth-0.5.3/LICENSE
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     9491 2023-05-05 00:26:55.129576 touchstone-auth-0.5.3/PKG-INFO
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     8849 2023-05-05 00:25:02.000000 touchstone-auth-0.5.3/README.md
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      103 2022-09-12 21:18:16.000000 touchstone-auth-0.5.3/pyproject.toml
+-rw-r--r--   0 christopher  (1000) christopher  (1000)       38 2023-05-05 00:26:55.129576 touchstone-auth-0.5.3/setup.cfg
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     1104 2023-05-05 00:24:10.000000 touchstone-auth-0.5.3/setup.py
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-05-05 00:26:55.126242 touchstone-auth-0.5.3/src/
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-05-05 00:26:55.126242 touchstone-auth-0.5.3/src/touchstone_auth/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)    21019 2023-05-05 00:24:03.000000 touchstone-auth-0.5.3/src/touchstone_auth/__init__.py
+drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-05-05 00:26:55.129576 touchstone-auth-0.5.3/src/touchstone_auth.egg-info/
+-rw-r--r--   0 christopher  (1000) christopher  (1000)     9491 2023-05-05 00:26:55.000000 touchstone-auth-0.5.3/src/touchstone_auth.egg-info/PKG-INFO
+-rw-r--r--   0 christopher  (1000) christopher  (1000)      287 2023-05-05 00:26:55.000000 touchstone-auth-0.5.3/src/touchstone_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 christopher  (1000) christopher  (1000)        1 2023-05-05 00:26:55.000000 touchstone-auth-0.5.3/src/touchstone_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 christopher  (1000) christopher  (1000)       82 2023-05-05 00:26:55.000000 touchstone-auth-0.5.3/src/touchstone_auth.egg-info/requires.txt
+-rw-r--r--   0 christopher  (1000) christopher  (1000)       16 2023-05-05 00:26:55.000000 touchstone-auth-0.5.3/src/touchstone_auth.egg-info/top_level.txt
```

### Comparing `touchstone-auth-0.5.2/LICENSE` & `touchstone-auth-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `touchstone-auth-0.5.2/PKG-INFO` & `touchstone-auth-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: touchstone-auth
-Version: 0.5.2
+Version: 0.5.3
 Summary: Access Touchstone SSO sites without a web browser.
 Home-page: https://github.com/meson800/touchstone-auth
 Author: Christopher Johnstone
 Author-email: meson800@gmail.com
 Project-URL: Bug Tracker, https://github.com/meson800/touchstone-auth/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -216,14 +216,14 @@
 ```
 After this 'local install', you can use and import `touchstone-auth` freely without
 having to re-install after each update.
 
 ## Changelog
 See the [CHANGELOG](CHANGELOG.md) for detailed changes.
 ```
-## [0.5.2] - 2023-05-04
+## [0.5.3] - 2023-05-04
 ### Updated
-- Switched to using a Firefox user-agent, and added XSRF token GET call.
+- Added explicit Kerberos post-auth request to accommodate Touchstone changes. 
 ```
 
 ## License
 This is licensed by the MIT license. Use freely!
```

### Comparing `touchstone-auth-0.5.2/README.md` & `touchstone-auth-0.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,14 @@
 ```
 After this 'local install', you can use and import `touchstone-auth` freely without
 having to re-install after each update.
 
 ## Changelog
 See the [CHANGELOG](CHANGELOG.md) for detailed changes.
 ```
-## [0.5.2] - 2023-05-04
+## [0.5.3] - 2023-05-04
 ### Updated
-- Switched to using a Firefox user-agent, and added XSRF token GET call.
+- Added explicit Kerberos post-auth request to accommodate Touchstone changes. 
 ```
 
 ## License
 This is licensed by the MIT license. Use freely!
```

### Comparing `touchstone-auth-0.5.2/setup.py` & `touchstone-auth-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='touchstone-auth',
-    version='0.5.2',
+    version='0.5.3',
     author='Christopher Johnstone',
     author_email='meson800@gmail.com',
     description='Access Touchstone SSO sites without a web browser.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/meson800/touchstone-auth',
     project_urls={
```

### Comparing `touchstone-auth-0.5.2/src/touchstone_auth/__init__.py` & `touchstone-auth-0.5.3/src/touchstone_auth/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,15 @@
         """
         Performs Touchstone and Duo login procedures (handling redirects to/from Duo)
 
         Arguments
         ---------
         conversation: A string specifying the Touchstone conversation type.
         """
+        auth_kwargs = {}
         if type(self._auth) == CertificateAuth:
             if type(self._auth.pkcs12_cert) == bytes:
                 self._session.mount('https://idp.mit.edu', Pkcs12Adapter(
                     pkcs12_data=self._auth.pkcs12_cert,
                     pkcs12_password=self._auth.pkcs12_pass))
             else:
                 self._session.mount('https://idp.mit.edu', Pkcs12Adapter(
@@ -209,18 +210,19 @@
             r = self._session.post('https://idp.mit.edu:446/idp/Authn/UsernamePassword',params={
                 'j_username': self._auth.username,
                 'j_password': self._auth.password,
                 'Submit': 'Login',
                 'conversation': conversation
             })
         elif type(self._auth) == KerberosAuth:
+            auth_kwargs['auth'] = HTTPKerberosAuth()
             r = self._session.get('https://idp.mit.edu:446/idp/Authn/Kerberos',params={
                 'login_kerberos': 'Use existing tickets - Go',
                 'conversation': conversation
-            }, auth=HTTPKerberosAuth())
+            }, **auth_kwargs)
         else:
             raise TypeError("Incorrect auth type passed!")
 
         duo_html = BeautifulSoup(r.text, features='html.parser')
         duo_container = duo_html.find(id='duo_container')
         if duo_container is None:
             raise TouchstoneError("Initial authentication with {} failed".format(type(self._auth).__name__))
@@ -381,15 +383,15 @@
 
 
         self.vlog('Acquired Touchstone auth token')
         # Post back to the parent, returning the request back to use for SSO login
         return self._session.post(duo_auth_info['parent'],
             data={
                 'sig_response': f"{duo_auth_info['cookie']}:{duo_app}"
-            })
+            }, **auth_kwargs)
 
     def perform_sso(self, request) -> None:
         """
         Given a Request object, attempts to perform Touchstone SSO redirect by
         extracting form fields and POSTing to the right location.
         """
         touchstone_html = BeautifulSoup(request.text, features='html.parser')
```

### Comparing `touchstone-auth-0.5.2/src/touchstone_auth.egg-info/PKG-INFO` & `touchstone-auth-0.5.3/src/touchstone_auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: touchstone-auth
-Version: 0.5.2
+Version: 0.5.3
 Summary: Access Touchstone SSO sites without a web browser.
 Home-page: https://github.com/meson800/touchstone-auth
 Author: Christopher Johnstone
 Author-email: meson800@gmail.com
 Project-URL: Bug Tracker, https://github.com/meson800/touchstone-auth/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -216,14 +216,14 @@
 ```
 After this 'local install', you can use and import `touchstone-auth` freely without
 having to re-install after each update.
 
 ## Changelog
 See the [CHANGELOG](CHANGELOG.md) for detailed changes.
 ```
-## [0.5.2] - 2023-05-04
+## [0.5.3] - 2023-05-04
 ### Updated
-- Switched to using a Firefox user-agent, and added XSRF token GET call.
+- Added explicit Kerberos post-auth request to accommodate Touchstone changes. 
 ```
 
 ## License
 This is licensed by the MIT license. Use freely!
```

