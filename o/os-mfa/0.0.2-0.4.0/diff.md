# Comparing `tmp/os-mfa-0.0.2.tar.gz` & `tmp/os-mfa-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os-mfa-0.0.2.tar", last modified: Sun Apr 30 13:45:14 2023, max compression
+gzip compressed data, was "os-mfa-0.4.0.tar", last modified: Fri May  5 10:23:48 2023, max compression
```

## Comparing `os-mfa-0.0.2.tar` & `os-mfa-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-30 13:45:14.461474 os-mfa-0.0.2/
--rw-r--r--   0 simon     (1000) simon     (1000)     1060 2023-04-30 09:59:27.000000 os-mfa-0.0.2/LICENSE
--rw-r--r--   0 simon     (1000) simon     (1000)     7230 2023-04-30 13:45:14.461474 os-mfa-0.0.2/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     6691 2023-04-30 13:25:11.000000 os-mfa-0.0.2/README.md
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-30 13:45:14.461474 os-mfa-0.0.2/os_mfa/
--rw-r--r--   0 simon     (1000) simon     (1000)       22 2023-04-30 13:44:34.000000 os-mfa-0.0.2/os_mfa/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1763 2023-04-30 09:55:50.000000 os-mfa-0.0.2/os_mfa/__main__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     4996 2023-04-30 13:35:30.000000 os-mfa-0.0.2/os_mfa/config_helpers.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-30 13:45:14.461474 os-mfa-0.0.2/os_mfa.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1000)     7230 2023-04-30 13:45:14.000000 os-mfa-0.0.2/os_mfa.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)      358 2023-04-30 13:45:14.000000 os-mfa-0.0.2/os_mfa.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        1 2023-04-30 13:45:14.000000 os-mfa-0.0.2/os_mfa.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       48 2023-04-30 13:45:14.000000 os-mfa-0.0.2/os_mfa.egg-info/entry_points.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       59 2023-04-30 13:45:14.000000 os-mfa-0.0.2/os_mfa.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        7 2023-04-30 13:45:14.000000 os-mfa-0.0.2/os_mfa.egg-info/top_level.txt
--rw-r--r--   0 simon     (1000) simon     (1000)     1273 2023-04-30 13:44:32.000000 os-mfa-0.0.2/pyproject.toml
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-04-30 13:45:14.461474 os-mfa-0.0.2/setup.cfg
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-04-30 13:35:56.000000 os-mfa-0.0.2/setup.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-30 13:45:14.461474 os-mfa-0.0.2/tests/
--rw-r--r--   0 simon     (1000) simon     (1000)     1107 2023-04-30 12:54:26.000000 os-mfa-0.0.2/tests/test_create_long_term_config.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1221 2023-04-30 12:54:26.000000 os-mfa-0.0.2/tests/test_create_token_config.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-05 10:23:48.156529 os-mfa-0.4.0/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1060 2023-04-30 09:59:27.000000 os-mfa-0.4.0/LICENSE
+-rw-r--r--   0 simon     (1000) simon     (1000)     7763 2023-05-05 10:23:48.156529 os-mfa-0.4.0/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     7225 2023-05-05 09:49:25.000000 os-mfa-0.4.0/README.md
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-05 10:23:48.156529 os-mfa-0.4.0/os_mfa/
+-rw-r--r--   0 simon     (1000) simon     (1000)       22 2023-05-05 10:16:19.000000 os-mfa-0.4.0/os_mfa/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1918 2023-05-05 09:49:25.000000 os-mfa-0.4.0/os_mfa/__main__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     4932 2023-05-05 09:49:25.000000 os-mfa-0.4.0/os_mfa/clouds_configs.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1405 2023-05-05 09:49:25.000000 os-mfa-0.4.0/os_mfa/tokens.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-05 10:23:48.156529 os-mfa-0.4.0/os_mfa.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1000)     7763 2023-05-05 10:23:48.000000 os-mfa-0.4.0/os_mfa.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)      375 2023-05-05 10:23:48.000000 os-mfa-0.4.0/os_mfa.egg-info/SOURCES.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        1 2023-05-05 10:23:48.000000 os-mfa-0.4.0/os_mfa.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       48 2023-05-05 10:23:48.000000 os-mfa-0.4.0/os_mfa.egg-info/entry_points.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       64 2023-05-05 10:23:48.000000 os-mfa-0.4.0/os_mfa.egg-info/requires.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        7 2023-05-05 10:23:48.000000 os-mfa-0.4.0/os_mfa.egg-info/top_level.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)     1192 2023-05-05 10:23:15.000000 os-mfa-0.4.0/pyproject.toml
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-05-05 10:23:48.156529 os-mfa-0.4.0/setup.cfg
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-05-01 08:59:46.000000 os-mfa-0.4.0/setup.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-05 10:23:48.156529 os-mfa-0.4.0/tests/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1107 2023-05-05 09:49:25.000000 os-mfa-0.4.0/tests/test_create_long_term_config.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1221 2023-05-05 09:49:25.000000 os-mfa-0.4.0/tests/test_create_token_config.py
```

### Comparing `os-mfa-0.0.2/LICENSE` & `os-mfa-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `os-mfa-0.0.2/PKG-INFO` & `os-mfa-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,78 @@
 Metadata-Version: 2.1
 Name: os-mfa
-Version: 0.0.2
+Version: 0.4.0
 Summary: A minimal utility for managing cli authentication with openstack more securely and conveniently
 Author-email: Simon Merrick <s.m3rrick@gmail.com>
 Project-URL: Homepage, https://github.com/iokiwi/os-mfa
 Keywords: openstack,mfa,auth
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # os-mfa
 
-Convenient and secure OpenStack authentication and credential management inspired by [broamski/aws-mfa](broamski/aws-mfa)
+Convenient and secure OpenStack authentication and credential management inspired by [broamski/aws-mfa](https://github.com/broamski/aws-mfa)
 
 ## What problem does os-mfa solve?
 
 First some quick background. OpenStack provides two main methods of setting credentials for programmatic authentication:
 
 **A) [Environment variables set via 'openrc.sh' files](https://docs.openstack.org/newton/user-guide/common/cli-set-environment-variables-using-openstack-rc.html)**
 
-* 🛡️ Avoids storing passwords in plaintext on disk 👍<br>
-* 🤦 Session credentials are lost if you close or restart your terminal window 👎<br>
-* 🔒 Sessions can't be shared/accessed across multiple terminal sessions 👎<br>
-* 💔 Not compatible with windows clients 👎<br>
+* 🛡️ Avoids storing passwords in plaintext on disk 👍
+* 🤦 Session credentials are lost if you close or restart your terminal window 👎
+* 🔒 Sessions can't be shared/accessed across multiple terminal sessions 👎
+* 💔 Not compatible with windows clients 👎
 
 **B) [clouds.yaml configuration files](https://docs.openstack.org/python-openstackclient/latest/configuration/index.html#configuration-files)**
 
- * 🌏 Are accessible in every terminal session 👍
- * 💪 Are durable to restarts/shutdowns 👍
+ * 💪 Session tokens are durable to terminal restarts/shutdowns 👍
  * 💗 Compatible and consistent user experience across platforms 👍
+ * 🌏 OpenStack sessions are accessible in from any terminal session 👍
  * 🙈 Encourages credentials to be stored in plain text 👎
- * ⌛ Tokens expire after 12 hours and need to be manually refreshed and updated in clouds.yaml 👎
+ * ⌛ Tokens that expire after 12 hours need to be manually refreshed and updated in clouds.yaml 👎
 
 As we can see both have advantages and disadvantages. But what if we could have the best parts of both options?
 
 **🌈 os-mfa 🦄 leverages the convenience and durability of using `clouds.yaml` and automates the secure management of credentials and tokens**
 
  * 🛡️ Avoids storing passwords in plaintext on disk 👍
- * 🌏 Session credentials are accessible in all terminals sessions 👍
- * 💪 Are durable to restarts/shutdowns 👍
- * 🔀 Trivially switch between multiple authenticated OpenStack sessions 👍
- * 🤝 Ensures native compatibility with the OpenStack ecosystem 👍
+ * 💪 Session tokens are durable to terminal restarts/shutdowns 👍
  * 💗 Compatible and consistent user experience across platforms 👍
+ * 🌏 OpenStack sessions are accessible in from any terminal session 👍
+ * 🔀 Trivially switch between multiple authenticated OpenStack sessions 👍
+ * 🤝 Ensured compatibility with the OpenStack ecosystem 👍
 
 ## Quick start
 
 Install os-mfa
 
 ```bash
 pip install -U os-mfa
 ```
 
 Download `clouds.yaml` file from your OpenStack dashboard. For example
 
- 1. Click API Access https://dashboard.catalystcloud.nz/project/api_access/
+ 1. Click **[API Access](https://dashboard.catalystcloud.nz/project/api_access/)** from the top left of the dashboard
  2. Click **Download OpenStack RC File** on the top right
  3. Select **OpenStack clouds.yaml File** from the drop down
 
-
-
 Place the file in your current working directory (`.`) or an alternate [location described by the docs](https://docs.openstack.org/python-openstackclient/latest/configuration/index.html#clouds-yaml)
 
 Linux
   * `~/.config/openstack/clouds.yaml`
   * `/etc/openstack/clouds.yaml`
 
 Windows
-  * `C:\Users\you\.config\openstack\clouds.yaml`
+  * `C:\Users\<username>\.config\openstack\clouds.yaml`
   * `C:\ProgramData\openstack\clouds.yaml`
 
 E.g.
 
 ```yaml
 # /home/john/clouds.yaml
 clouds:
@@ -87,19 +85,22 @@
       username: john.smith@acme.com
       password: 1ns3curE123!
     identity_api_version: 3
     interface: public
     region_name: nz-hlz-1
 ```
 
-Run os-mfa
+Set `$OS_CLOUD` in your environment.
 
 ```bash
 $ export OS_CLOUD=catalystcloud
 ```
+
+Run `os-mfa`
+
 ```bash
 $ os-mfa
 Authenticating 'john.smith@example.com' in project 'john-smith'
 Enter Password:
 MFA Code (Press enter to skip): 654321
 Getting token...
 ```
@@ -111,34 +112,34 @@
 +--------------------------------------+------------+--------------------------------------------+
 | f10ad6de-a26d-4c29-8c64-2a7418d47f8f | public-net | 5063aab1-aa08-48b2-b81d-730ac732fc51,      |
 |                                      |            | 8a7fe804-7fbe-43d0-aa1d-cfa03034ef22,      |
 |                                      |            | a1549e09-4176-4322-860c-cadc68608b48       |
 +--------------------------------------+------------+--------------------------------------------+
 ```
 
-If you close/restart or start a new terminal window, resume your openstack session simply by exporting `$OS_CLOUD` again.
+Now if you close/restart or start a new terminal window, resume your existing OpenStack session simply by exporting `$OS_CLOUD` again.
 
 ```bash
 export OS_CLOUD=catalystcloud
 ```
 
 ## What happened when we ran os-mfa?
 
-os-mfa created a *"long-term"* configuration without any passwords or secrets.
+The first time we run os-mfa is creates a *"long-term"* configuration in our clouds.yaml without any passwords or secrets.
 
- * *"long-term"* configurations are distinguished with a suffix of `-long-term`
- * We do not use the long term configs with the openstack client tools.
- 
-The long term config used as a foundation for authentication by os-mfa which then:
+Long term configurations contain the minimum information required for os-mfa to use to initialize a token based authentication.
 
-1) Prompts the user for their password and totp token
+ * They should *not* contain any secrets such as tokens or passwords.
+ * They are distinguished by a suffix of `-long-term`
 
-2) Swaps the password and totp for an openstack auth token
+os-mfa will then use the `-long-term` configuration to create a token based configuration as follows.
 
-3) Updates the original configuration to use the new token for authentication
+ 1. Prompts the user for their password and MFA code
+ 2. Swaps the password and MFA code for an OpenStack auth token
+ 3. Updates the original configuration to use the new token for authentication
 
 The resulting clouds.yaml should look like this
 
 ```yaml
 # /home/john/clouds.yaml
 clouds:
   catalystcloud:
@@ -161,37 +162,46 @@
     interface: public
     region_name: nz-hlz-1
 
 ```
 
 ## Going further
 
+### Multiple projects, users and sessions
 
-### Switching between multiple cloud accounts and sessions
+
+Since clouds.yaml supports multiple configurations, you can create configurations for any combination of
+
+ * user
+ * project
+ * region
+ * openstack cloud
 
 ```yaml
 clouds:
-  project1-long-term:
+  project1:
     region: nz-hlz-1
     auth:
         project_name: project1
         username: john.smith@acme.com
         # ...
-  project2-long-term:
+  project2:
     region: nz-por-1
     auth:
         project_name: project2
         username: john.smith@acme.com
         # ...
 ```
 
-After running os-mfa once for each project you can switch between them 
+After initializing a token based authentication for each configuration using os-mfa, you can change between sessions at will
 
-```
+```bash
 OS_CLOUD=project1
+```
+```bash
 OS_CLOUD=project2
 ```
 
 ## Contributing
 
 Nothing special to report, just raise a PR
 
@@ -202,26 +212,27 @@
 ```
 
 ### Building Package
 
 Source: https://realpython.com/pypi-publish-python-package/
 
 ```
-python -m pip install pip-tools build twine bumpver
+python -m pip install pip-tools twine
 pip-compile pyproject.toml
+rm -rf dist/*
 python -m build
 twine check dist/*
 twine upload -r testpypi dist/*
 twine upload dist/*
 ```
 
 ## TODO
 
  * ☑️ TBH I am probably going to port this back to python
  * ☑️ Alert if no clouds.yaml found
  * ☑️ Better error message if OS_CLOUD not set
- * ☑️ CI/CD
- * 🟦 Non-interactive mode
- * 🟦 Sanitize long-term config better
+ * 🟦 CI/CD
+ * 🟦 Optionally disable prompt for MFA token
  * 🟦 Store and check expiry of token
-    * 🟦 Only reauthenticate if token is not valid
-    * 🟦 -f, --force cli option to force authentication
+ * 🟦 Only reauthenticate if token is not valid
+ * 🟦 -f, --force cli option to force authentication
+ * 🟦 more unit and integration tests
```

### Comparing `os-mfa-0.0.2/README.md` & `os-mfa-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,63 @@
 # os-mfa
 
-Convenient and secure OpenStack authentication and credential management inspired by [broamski/aws-mfa](broamski/aws-mfa)
+Convenient and secure OpenStack authentication and credential management inspired by [broamski/aws-mfa](https://github.com/broamski/aws-mfa)
 
 ## What problem does os-mfa solve?
 
 First some quick background. OpenStack provides two main methods of setting credentials for programmatic authentication:
 
 **A) [Environment variables set via 'openrc.sh' files](https://docs.openstack.org/newton/user-guide/common/cli-set-environment-variables-using-openstack-rc.html)**
 
-* 🛡️ Avoids storing passwords in plaintext on disk 👍<br>
-* 🤦 Session credentials are lost if you close or restart your terminal window 👎<br>
-* 🔒 Sessions can't be shared/accessed across multiple terminal sessions 👎<br>
-* 💔 Not compatible with windows clients 👎<br>
+* 🛡️ Avoids storing passwords in plaintext on disk 👍
+* 🤦 Session credentials are lost if you close or restart your terminal window 👎
+* 🔒 Sessions can't be shared/accessed across multiple terminal sessions 👎
+* 💔 Not compatible with windows clients 👎
 
 **B) [clouds.yaml configuration files](https://docs.openstack.org/python-openstackclient/latest/configuration/index.html#configuration-files)**
 
- * 🌏 Are accessible in every terminal session 👍
- * 💪 Are durable to restarts/shutdowns 👍
+ * 💪 Session tokens are durable to terminal restarts/shutdowns 👍
  * 💗 Compatible and consistent user experience across platforms 👍
+ * 🌏 OpenStack sessions are accessible in from any terminal session 👍
  * 🙈 Encourages credentials to be stored in plain text 👎
- * ⌛ Tokens expire after 12 hours and need to be manually refreshed and updated in clouds.yaml 👎
+ * ⌛ Tokens that expire after 12 hours need to be manually refreshed and updated in clouds.yaml 👎
 
 As we can see both have advantages and disadvantages. But what if we could have the best parts of both options?
 
 **🌈 os-mfa 🦄 leverages the convenience and durability of using `clouds.yaml` and automates the secure management of credentials and tokens**
 
  * 🛡️ Avoids storing passwords in plaintext on disk 👍
- * 🌏 Session credentials are accessible in all terminals sessions 👍
- * 💪 Are durable to restarts/shutdowns 👍
- * 🔀 Trivially switch between multiple authenticated OpenStack sessions 👍
- * 🤝 Ensures native compatibility with the OpenStack ecosystem 👍
+ * 💪 Session tokens are durable to terminal restarts/shutdowns 👍
  * 💗 Compatible and consistent user experience across platforms 👍
+ * 🌏 OpenStack sessions are accessible in from any terminal session 👍
+ * 🔀 Trivially switch between multiple authenticated OpenStack sessions 👍
+ * 🤝 Ensured compatibility with the OpenStack ecosystem 👍
 
 ## Quick start
 
 Install os-mfa
 
 ```bash
 pip install -U os-mfa
 ```
 
 Download `clouds.yaml` file from your OpenStack dashboard. For example
 
- 1. Click API Access https://dashboard.catalystcloud.nz/project/api_access/
+ 1. Click **[API Access](https://dashboard.catalystcloud.nz/project/api_access/)** from the top left of the dashboard
  2. Click **Download OpenStack RC File** on the top right
  3. Select **OpenStack clouds.yaml File** from the drop down
 
-
-
 Place the file in your current working directory (`.`) or an alternate [location described by the docs](https://docs.openstack.org/python-openstackclient/latest/configuration/index.html#clouds-yaml)
 
 Linux
   * `~/.config/openstack/clouds.yaml`
   * `/etc/openstack/clouds.yaml`
 
 Windows
-  * `C:\Users\you\.config\openstack\clouds.yaml`
+  * `C:\Users\<username>\.config\openstack\clouds.yaml`
   * `C:\ProgramData\openstack\clouds.yaml`
 
 E.g.
 
 ```yaml
 # /home/john/clouds.yaml
 clouds:
@@ -72,19 +70,22 @@
       username: john.smith@acme.com
       password: 1ns3curE123!
     identity_api_version: 3
     interface: public
     region_name: nz-hlz-1
 ```
 
-Run os-mfa
+Set `$OS_CLOUD` in your environment.
 
 ```bash
 $ export OS_CLOUD=catalystcloud
 ```
+
+Run `os-mfa`
+
 ```bash
 $ os-mfa
 Authenticating 'john.smith@example.com' in project 'john-smith'
 Enter Password:
 MFA Code (Press enter to skip): 654321
 Getting token...
 ```
@@ -96,34 +97,34 @@
 +--------------------------------------+------------+--------------------------------------------+
 | f10ad6de-a26d-4c29-8c64-2a7418d47f8f | public-net | 5063aab1-aa08-48b2-b81d-730ac732fc51,      |
 |                                      |            | 8a7fe804-7fbe-43d0-aa1d-cfa03034ef22,      |
 |                                      |            | a1549e09-4176-4322-860c-cadc68608b48       |
 +--------------------------------------+------------+--------------------------------------------+
 ```
 
-If you close/restart or start a new terminal window, resume your openstack session simply by exporting `$OS_CLOUD` again.
+Now if you close/restart or start a new terminal window, resume your existing OpenStack session simply by exporting `$OS_CLOUD` again.
 
 ```bash
 export OS_CLOUD=catalystcloud
 ```
 
 ## What happened when we ran os-mfa?
 
-os-mfa created a *"long-term"* configuration without any passwords or secrets.
+The first time we run os-mfa is creates a *"long-term"* configuration in our clouds.yaml without any passwords or secrets.
 
- * *"long-term"* configurations are distinguished with a suffix of `-long-term`
- * We do not use the long term configs with the openstack client tools.
- 
-The long term config used as a foundation for authentication by os-mfa which then:
+Long term configurations contain the minimum information required for os-mfa to use to initialize a token based authentication.
 
-1) Prompts the user for their password and totp token
+ * They should *not* contain any secrets such as tokens or passwords.
+ * They are distinguished by a suffix of `-long-term`
 
-2) Swaps the password and totp for an openstack auth token
+os-mfa will then use the `-long-term` configuration to create a token based configuration as follows.
 
-3) Updates the original configuration to use the new token for authentication
+ 1. Prompts the user for their password and MFA code
+ 2. Swaps the password and MFA code for an OpenStack auth token
+ 3. Updates the original configuration to use the new token for authentication
 
 The resulting clouds.yaml should look like this
 
 ```yaml
 # /home/john/clouds.yaml
 clouds:
   catalystcloud:
@@ -146,37 +147,46 @@
     interface: public
     region_name: nz-hlz-1
 
 ```
 
 ## Going further
 
+### Multiple projects, users and sessions
 
-### Switching between multiple cloud accounts and sessions
+
+Since clouds.yaml supports multiple configurations, you can create configurations for any combination of
+
+ * user
+ * project
+ * region
+ * openstack cloud
 
 ```yaml
 clouds:
-  project1-long-term:
+  project1:
     region: nz-hlz-1
     auth:
         project_name: project1
         username: john.smith@acme.com
         # ...
-  project2-long-term:
+  project2:
     region: nz-por-1
     auth:
         project_name: project2
         username: john.smith@acme.com
         # ...
 ```
 
-After running os-mfa once for each project you can switch between them 
+After initializing a token based authentication for each configuration using os-mfa, you can change between sessions at will
 
-```
+```bash
 OS_CLOUD=project1
+```
+```bash
 OS_CLOUD=project2
 ```
 
 ## Contributing
 
 Nothing special to report, just raise a PR
 
@@ -187,26 +197,27 @@
 ```
 
 ### Building Package
 
 Source: https://realpython.com/pypi-publish-python-package/
 
 ```
-python -m pip install pip-tools build twine bumpver
+python -m pip install pip-tools twine
 pip-compile pyproject.toml
+rm -rf dist/*
 python -m build
 twine check dist/*
 twine upload -r testpypi dist/*
 twine upload dist/*
 ```
 
 ## TODO
 
  * ☑️ TBH I am probably going to port this back to python
  * ☑️ Alert if no clouds.yaml found
  * ☑️ Better error message if OS_CLOUD not set
- * ☑️ CI/CD
- * 🟦 Non-interactive mode
- * 🟦 Sanitize long-term config better
+ * 🟦 CI/CD
+ * 🟦 Optionally disable prompt for MFA token
  * 🟦 Store and check expiry of token
-    * 🟦 Only reauthenticate if token is not valid
-    * 🟦 -f, --force cli option to force authentication
+ * 🟦 Only reauthenticate if token is not valid
+ * 🟦 -f, --force cli option to force authentication
+ * 🟦 more unit and integration tests
```

### Comparing `os-mfa-0.0.2/os_mfa/__main__.py` & `os-mfa-0.4.0/os_mfa/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import os
 from argparse import ArgumentParser
 
-from .config_helpers import *
+from .clouds_configs import *
+from .tokens import *
 
 
 def main():
     parser = ArgumentParser()
     parser.add_argument(
         "--os-cloud", help="Specify the name of the cloud configuration you want to use"
     )
@@ -36,21 +37,23 @@
         print(
             "Neither '{}' or '{}' found in {}".format(
                 os_cloud, long_term_config_name, manager.config_path
             )
         )
         sys.exit(1)
 
-    # Create long term config if it doesn't exist
+    # Create a long-term config if it doesn't exist
     if not manager.config_exists(long_term_config_name):
+        print("Creating config: {}".format(long_term_config_name))
         default_config = manager.get_config_by_name(os_cloud)
         long_term_config = create_long_term_config(default_config)
         manager.put_config_by_name(long_term_config_name, long_term_config)
 
     # Create token based config from long term config
     long_term_config = manager.get_config_by_name(long_term_config_name)
     token_config = get_token_config(long_term_config)
+    print("The '{}' config has been updated.".format(os_cloud))
     manager.put_config_by_name(os_cloud, token_config)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `os-mfa-0.0.2/os_mfa.egg-info/PKG-INFO` & `os-mfa-0.4.0/os_mfa.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,78 @@
 Metadata-Version: 2.1
 Name: os-mfa
-Version: 0.0.2
+Version: 0.4.0
 Summary: A minimal utility for managing cli authentication with openstack more securely and conveniently
 Author-email: Simon Merrick <s.m3rrick@gmail.com>
 Project-URL: Homepage, https://github.com/iokiwi/os-mfa
 Keywords: openstack,mfa,auth
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # os-mfa
 
-Convenient and secure OpenStack authentication and credential management inspired by [broamski/aws-mfa](broamski/aws-mfa)
+Convenient and secure OpenStack authentication and credential management inspired by [broamski/aws-mfa](https://github.com/broamski/aws-mfa)
 
 ## What problem does os-mfa solve?
 
 First some quick background. OpenStack provides two main methods of setting credentials for programmatic authentication:
 
 **A) [Environment variables set via 'openrc.sh' files](https://docs.openstack.org/newton/user-guide/common/cli-set-environment-variables-using-openstack-rc.html)**
 
-* 🛡️ Avoids storing passwords in plaintext on disk 👍<br>
-* 🤦 Session credentials are lost if you close or restart your terminal window 👎<br>
-* 🔒 Sessions can't be shared/accessed across multiple terminal sessions 👎<br>
-* 💔 Not compatible with windows clients 👎<br>
+* 🛡️ Avoids storing passwords in plaintext on disk 👍
+* 🤦 Session credentials are lost if you close or restart your terminal window 👎
+* 🔒 Sessions can't be shared/accessed across multiple terminal sessions 👎
+* 💔 Not compatible with windows clients 👎
 
 **B) [clouds.yaml configuration files](https://docs.openstack.org/python-openstackclient/latest/configuration/index.html#configuration-files)**
 
- * 🌏 Are accessible in every terminal session 👍
- * 💪 Are durable to restarts/shutdowns 👍
+ * 💪 Session tokens are durable to terminal restarts/shutdowns 👍
  * 💗 Compatible and consistent user experience across platforms 👍
+ * 🌏 OpenStack sessions are accessible in from any terminal session 👍
  * 🙈 Encourages credentials to be stored in plain text 👎
- * ⌛ Tokens expire after 12 hours and need to be manually refreshed and updated in clouds.yaml 👎
+ * ⌛ Tokens that expire after 12 hours need to be manually refreshed and updated in clouds.yaml 👎
 
 As we can see both have advantages and disadvantages. But what if we could have the best parts of both options?
 
 **🌈 os-mfa 🦄 leverages the convenience and durability of using `clouds.yaml` and automates the secure management of credentials and tokens**
 
  * 🛡️ Avoids storing passwords in plaintext on disk 👍
- * 🌏 Session credentials are accessible in all terminals sessions 👍
- * 💪 Are durable to restarts/shutdowns 👍
- * 🔀 Trivially switch between multiple authenticated OpenStack sessions 👍
- * 🤝 Ensures native compatibility with the OpenStack ecosystem 👍
+ * 💪 Session tokens are durable to terminal restarts/shutdowns 👍
  * 💗 Compatible and consistent user experience across platforms 👍
+ * 🌏 OpenStack sessions are accessible in from any terminal session 👍
+ * 🔀 Trivially switch between multiple authenticated OpenStack sessions 👍
+ * 🤝 Ensured compatibility with the OpenStack ecosystem 👍
 
 ## Quick start
 
 Install os-mfa
 
 ```bash
 pip install -U os-mfa
 ```
 
 Download `clouds.yaml` file from your OpenStack dashboard. For example
 
- 1. Click API Access https://dashboard.catalystcloud.nz/project/api_access/
+ 1. Click **[API Access](https://dashboard.catalystcloud.nz/project/api_access/)** from the top left of the dashboard
  2. Click **Download OpenStack RC File** on the top right
  3. Select **OpenStack clouds.yaml File** from the drop down
 
-
-
 Place the file in your current working directory (`.`) or an alternate [location described by the docs](https://docs.openstack.org/python-openstackclient/latest/configuration/index.html#clouds-yaml)
 
 Linux
   * `~/.config/openstack/clouds.yaml`
   * `/etc/openstack/clouds.yaml`
 
 Windows
-  * `C:\Users\you\.config\openstack\clouds.yaml`
+  * `C:\Users\<username>\.config\openstack\clouds.yaml`
   * `C:\ProgramData\openstack\clouds.yaml`
 
 E.g.
 
 ```yaml
 # /home/john/clouds.yaml
 clouds:
@@ -87,19 +85,22 @@
       username: john.smith@acme.com
       password: 1ns3curE123!
     identity_api_version: 3
     interface: public
     region_name: nz-hlz-1
 ```
 
-Run os-mfa
+Set `$OS_CLOUD` in your environment.
 
 ```bash
 $ export OS_CLOUD=catalystcloud
 ```
+
+Run `os-mfa`
+
 ```bash
 $ os-mfa
 Authenticating 'john.smith@example.com' in project 'john-smith'
 Enter Password:
 MFA Code (Press enter to skip): 654321
 Getting token...
 ```
@@ -111,34 +112,34 @@
 +--------------------------------------+------------+--------------------------------------------+
 | f10ad6de-a26d-4c29-8c64-2a7418d47f8f | public-net | 5063aab1-aa08-48b2-b81d-730ac732fc51,      |
 |                                      |            | 8a7fe804-7fbe-43d0-aa1d-cfa03034ef22,      |
 |                                      |            | a1549e09-4176-4322-860c-cadc68608b48       |
 +--------------------------------------+------------+--------------------------------------------+
 ```
 
-If you close/restart or start a new terminal window, resume your openstack session simply by exporting `$OS_CLOUD` again.
+Now if you close/restart or start a new terminal window, resume your existing OpenStack session simply by exporting `$OS_CLOUD` again.
 
 ```bash
 export OS_CLOUD=catalystcloud
 ```
 
 ## What happened when we ran os-mfa?
 
-os-mfa created a *"long-term"* configuration without any passwords or secrets.
+The first time we run os-mfa is creates a *"long-term"* configuration in our clouds.yaml without any passwords or secrets.
 
- * *"long-term"* configurations are distinguished with a suffix of `-long-term`
- * We do not use the long term configs with the openstack client tools.
- 
-The long term config used as a foundation for authentication by os-mfa which then:
+Long term configurations contain the minimum information required for os-mfa to use to initialize a token based authentication.
 
-1) Prompts the user for their password and totp token
+ * They should *not* contain any secrets such as tokens or passwords.
+ * They are distinguished by a suffix of `-long-term`
 
-2) Swaps the password and totp for an openstack auth token
+os-mfa will then use the `-long-term` configuration to create a token based configuration as follows.
 
-3) Updates the original configuration to use the new token for authentication
+ 1. Prompts the user for their password and MFA code
+ 2. Swaps the password and MFA code for an OpenStack auth token
+ 3. Updates the original configuration to use the new token for authentication
 
 The resulting clouds.yaml should look like this
 
 ```yaml
 # /home/john/clouds.yaml
 clouds:
   catalystcloud:
@@ -161,37 +162,46 @@
     interface: public
     region_name: nz-hlz-1
 
 ```
 
 ## Going further
 
+### Multiple projects, users and sessions
 
-### Switching between multiple cloud accounts and sessions
+
+Since clouds.yaml supports multiple configurations, you can create configurations for any combination of
+
+ * user
+ * project
+ * region
+ * openstack cloud
 
 ```yaml
 clouds:
-  project1-long-term:
+  project1:
     region: nz-hlz-1
     auth:
         project_name: project1
         username: john.smith@acme.com
         # ...
-  project2-long-term:
+  project2:
     region: nz-por-1
     auth:
         project_name: project2
         username: john.smith@acme.com
         # ...
 ```
 
-After running os-mfa once for each project you can switch between them 
+After initializing a token based authentication for each configuration using os-mfa, you can change between sessions at will
 
-```
+```bash
 OS_CLOUD=project1
+```
+```bash
 OS_CLOUD=project2
 ```
 
 ## Contributing
 
 Nothing special to report, just raise a PR
 
@@ -202,26 +212,27 @@
 ```
 
 ### Building Package
 
 Source: https://realpython.com/pypi-publish-python-package/
 
 ```
-python -m pip install pip-tools build twine bumpver
+python -m pip install pip-tools twine
 pip-compile pyproject.toml
+rm -rf dist/*
 python -m build
 twine check dist/*
 twine upload -r testpypi dist/*
 twine upload dist/*
 ```
 
 ## TODO
 
  * ☑️ TBH I am probably going to port this back to python
  * ☑️ Alert if no clouds.yaml found
  * ☑️ Better error message if OS_CLOUD not set
- * ☑️ CI/CD
- * 🟦 Non-interactive mode
- * 🟦 Sanitize long-term config better
+ * 🟦 CI/CD
+ * 🟦 Optionally disable prompt for MFA token
  * 🟦 Store and check expiry of token
-    * 🟦 Only reauthenticate if token is not valid
-    * 🟦 -f, --force cli option to force authentication
+ * 🟦 Only reauthenticate if token is not valid
+ * 🟦 -f, --force cli option to force authentication
+ * 🟦 more unit and integration tests
```

### Comparing `os-mfa-0.0.2/pyproject.toml` & `os-mfa-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "os-mfa"
-version = "0.0.2"
+version = "0.4.0"
 description = "A minimal utility for managing cli authentication with openstack more securely and conveniently"
 readme = "README.md"
 authors = [{ name = "Simon Merrick", email = "s.m3rrick@gmail.com" }]
 # license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -18,38 +18,31 @@
 dependencies = [
     "requests",
     "PyYaml"
 ]
 requires-python = ">= 3.6"
 
 [project.optional-dependencies]
-dev = ["black", "bumpver", "pip-tools", "twine", "build"]
+dev = ["black", "bumpver", "pip-tools", "twine", "build", "mypy"]
 
 [project.urls]
 Homepage = "https://github.com/iokiwi/os-mfa"
 
 [project.scripts]
 os-mfa = "os_mfa.__main__:main"
 
 [tool.bumpver]
-current_version = "0.0.2"
+current_version = "0.4.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
-]
-"setup.py" = [
-    "{version}",
-    "{pep440_version}",
-]
-"README.md" = [
-    "{version}",
-    "{pep440_version}",
+    'version = "{version}"'
 ]
 "os_mfa/__init__.py" = [
     "{version}"
 ]
```

### Comparing `os-mfa-0.0.2/tests/test_create_long_term_config.py` & `os-mfa-0.4.0/tests/test_create_long_term_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from os_mfa.config_helpers import create_long_term_config
+from os_mfa.clouds_configs import create_long_term_config
 
 
 class TestCreateLongTermConfig(unittest.TestCase):
     def setUp(self):
         self.config = {
             "auth": {
                 "auth_url": "https://api.nz-hlz-1.catalystcloud.io:5000",
```

### Comparing `os-mfa-0.0.2/tests/test_create_token_config.py` & `os-mfa-0.4.0/tests/test_create_token_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from os_mfa.config_helpers import create_token_config
+from os_mfa.clouds_configs import create_token_config
 
 
 class TestCreateLongTermConfig(unittest.TestCase):
     def setUp(self):
         self.config = {
             "auth": {
                 "auth_url": "https://api.nz-hlz-1.catalystcloud.io:5000",
```

