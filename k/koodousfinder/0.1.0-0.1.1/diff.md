# Comparing `tmp/koodousfinder-0.1.0.tar.gz` & `tmp/koodousfinder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koodousfinder-0.1.0.tar", max compression
+gzip compressed data, was "koodousfinder-0.1.1.tar", max compression
```

## Comparing `koodousfinder-0.1.0.tar` & `koodousfinder-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0     2150 2023-04-20 02:23:29.309642 koodousfinder-0.1.0/README.md
--rw-r--r--   0        0        0      531 2023-04-20 02:23:29.316486 koodousfinder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 02:23:29.316884 koodousfinder-0.1.0/src/koodousfinder/__init__.py
--rw-r--r--   0        0        0     2276 2023-04-20 02:23:29.317076 koodousfinder-0.1.0/src/koodousfinder/console.py
--rw-r--r--   0        0        0     2692 1970-01-01 00:00:00.000000 koodousfinder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2381 2023-05-05 10:41:54.333355 koodousfinder-0.1.1/README.md
+-rw-r--r--   0        0        0     1414 2023-05-05 10:41:54.349033 koodousfinder-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-05-05 10:41:54.349334 koodousfinder-0.1.1/src/koodousfinder/__init__.py
+-rw-r--r--   0        0        0     1428 2023-05-05 10:41:54.349584 koodousfinder-0.1.1/src/koodousfinder/client.py
+-rw-r--r--   0        0        0     4036 2023-05-05 10:41:54.349926 koodousfinder-0.1.1/src/koodousfinder/console.py
+-rw-r--r--   0        0        0      346 2023-05-05 10:41:54.350190 koodousfinder-0.1.1/src/koodousfinder/response.py
+-rw-r--r--   0        0        0     3238 1970-01-01 00:00:00.000000 koodousfinder-0.1.1/PKG-INFO
```

### Comparing `koodousfinder-0.1.0/README.md` & `koodousfinder-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # KoodousFinder
 A simple tool to allows users to search for and analyze android apps for potential security threats and vulnerabilities
 
 # Account and API Key
 Create a Koodous account and get your api key https://koodous.com/settings/developers
 
+# Install
+
+$ pip install koodousfinder
+
 # Arguments
   
   
 |        Param        |          description                |
 |----------------|-------------------------------|
 | -h, --help     |`'Show this help message and exit'`            |
 |--package-name  |`"General search for APK`s"`            |
@@ -17,24 +21,47 @@
 
 koodous.py --package-name "app: Brata AND package: com.brata" <br>
 koodous.py --package-name "package: com.google.android.videos AND trusted: true"<br>
 koodous.py --package-name "com.metasploit"<br>
 python3 koodous.py --app-name "WhatsApp MOD"<br>
 
 
-![alt text for screen readers](https://raw.githubusercontent.com/teixeira0xfffff/KoodousFinder/main/assets/sample%202.png "sample search for Brata Malware")
+![alt text for screen readers](https://raw.githubusercontent.com/teixeira0xfffff/KoodousFinder/main/assets/view2.png "sample search for Brata Malware")
 
 # Modifiers for advanced search
 
 |Attribute           |Modifier                          |Description                         |
 |----------------|-------------------------------|-----------------------------|
 |Hash           |`hash:`            |Performs the search depending on the automatically inserted hash. The admitted hashes are sha1, sha256 and md5.
 |App name          |`app:`            |Searches for the specified app name. If it is a compound name, it can be searched enclosed in quotes, for example: app: "Whatsapp premium".          |
 |Package name.          |`package:` |Searches the package name to see if it contains the indicated string, for example: package: com.whatsapp.|
 |Name of the developer or company.          |`developer:` |Searches whether the company or developer field includes the indicated string, for example: developer: "WhatsApp Inc.".|
 |Certificate         |`certificate:` |Searches the apps by their certificate. For example: cert: 60BBF1896747E313B240EE2A54679BB0CE4A5023 or certificate: 38A0F7D505FE18FEC64FBF343ECAAAF310DBD799.|
 
 More information: https://docs.koodous.com/apks.html. <br>
-#TODO
+
+# TODO
 
 * Discord Integration
 * Rulesets view
+
+# Development
+
+## Taskipy usage:
+
+To run the unit tests:
+
+```shell
+task test
+```
+
+To run the pylint tests:
+
+```shell
+task lint
+```
+
+To run the isort to sort the imports:
+
+```shell
+task sort
+```
```

### Comparing `koodousfinder-0.1.0/PKG-INFO` & `koodousfinder-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 Metadata-Version: 2.1
 Name: koodousfinder
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple tool to allows users to search for and analyze android apps for potential security threats and vulnerabilities
+Home-page: https://github.com/teixeira0xfffff/KoodousFinder
 Author: teixeira0xfffff
 Author-email: www@www.www
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.7.2,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: keyring (>=23.13.1,<24.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: stix2 (>=3.0.1,<4.0.0)
+Project-URL: Repository, https://github.com/teixeira0xfffff/KoodousFinder
 Description-Content-Type: text/markdown
 
 # KoodousFinder
 A simple tool to allows users to search for and analyze android apps for potential security threats and vulnerabilities
 
 # Account and API Key
 Create a Koodous account and get your api key https://koodous.com/settings/developers
 
+# Install
+
+$ pip install koodousfinder
+
 # Arguments
   
   
 |        Param        |          description                |
 |----------------|-------------------------------|
 | -h, --help     |`'Show this help message and exit'`            |
 |--package-name  |`"General search for APK`s"`            |
@@ -31,25 +41,47 @@
 
 koodous.py --package-name "app: Brata AND package: com.brata" <br>
 koodous.py --package-name "package: com.google.android.videos AND trusted: true"<br>
 koodous.py --package-name "com.metasploit"<br>
 python3 koodous.py --app-name "WhatsApp MOD"<br>
 
 
-![alt text for screen readers](https://raw.githubusercontent.com/teixeira0xfffff/KoodousFinder/main/assets/sample%202.png "sample search for Brata Malware")
+![alt text for screen readers](https://raw.githubusercontent.com/teixeira0xfffff/KoodousFinder/main/assets/view2.png "sample search for Brata Malware")
 
 # Modifiers for advanced search
 
 |Attribute           |Modifier                          |Description                         |
 |----------------|-------------------------------|-----------------------------|
 |Hash           |`hash:`            |Performs the search depending on the automatically inserted hash. The admitted hashes are sha1, sha256 and md5.
 |App name          |`app:`            |Searches for the specified app name. If it is a compound name, it can be searched enclosed in quotes, for example: app: "Whatsapp premium".          |
 |Package name.          |`package:` |Searches the package name to see if it contains the indicated string, for example: package: com.whatsapp.|
 |Name of the developer or company.          |`developer:` |Searches whether the company or developer field includes the indicated string, for example: developer: "WhatsApp Inc.".|
 |Certificate         |`certificate:` |Searches the apps by their certificate. For example: cert: 60BBF1896747E313B240EE2A54679BB0CE4A5023 or certificate: 38A0F7D505FE18FEC64FBF343ECAAAF310DBD799.|
 
 More information: https://docs.koodous.com/apks.html. <br>
-#TODO
+
+# TODO
 
 * Discord Integration
 * Rulesets view
 
+# Development
+
+## Taskipy usage:
+
+To run the unit tests:
+
+```shell
+task test
+```
+
+To run the pylint tests:
+
+```shell
+task lint
+```
+
+To run the isort to sort the imports:
+
+```shell
+task sort
+```
```

