# Comparing `tmp/slack-watchman-4.0.0.tar.gz` & `tmp/slack-watchman-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-watchman-4.0.0.tar", last modified: Wed May  3 19:18:55 2023, max compression
+gzip compressed data, was "slack-watchman-4.0.1.tar", last modified: Fri May  5 08:08:19 2023, max compression
```

## Comparing `slack-watchman-4.0.0.tar` & `slack-watchman-4.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:18:55.456387 slack-watchman-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-05-03 19:18:55.456387 slack-watchman-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-03 19:18:55.456387 slack-watchman-4.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:18:55.444386 slack-watchman-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:18:55.448386 slack-watchman-4.0.0/src/slack_watchman/
--rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:18:55.456387 slack-watchman-4.0.0/src/slack_watchman/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/models/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/models/post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/models/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/signature_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/slack_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-05-03 19:18:34.000000 slack-watchman-4.0.0/src/slack_watchman/sw_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:18:55.452387 slack-watchman-4.0.0/src/slack_watchman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-05-03 19:18:55.000000 slack-watchman-4.0.0/src/slack_watchman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-03 19:18:55.000000 slack-watchman-4.0.0/src/slack_watchman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:18:55.000000 slack-watchman-4.0.0/src/slack_watchman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 19:18:55.000000 slack-watchman-4.0.0/src/slack_watchman.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:18:55.000000 slack-watchman-4.0.0/src/slack_watchman.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 19:18:55.000000 slack-watchman-4.0.0/src/slack_watchman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 19:18:55.000000 slack-watchman-4.0.0/src/slack_watchman.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:08:19.374801 slack-watchman-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-05-05 08:08:19.374801 slack-watchman-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-05 08:08:19.378800 slack-watchman-4.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:08:19.370800 slack-watchman-4.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:08:19.370800 slack-watchman-4.0.1/src/slack_watchman/
+-rw-r--r--   0 runner    (1001) docker     (123)    14762 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:08:19.374801 slack-watchman-4.0.1/src/slack_watchman/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/models/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/models/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/models/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/signature_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/slack_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-05-05 08:07:40.000000 slack-watchman-4.0.1/src/slack_watchman/sw_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:08:19.374801 slack-watchman-4.0.1/src/slack_watchman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-05-05 08:08:19.000000 slack-watchman-4.0.1/src/slack_watchman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-05 08:08:19.000000 slack-watchman-4.0.1/src/slack_watchman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:08:19.000000 slack-watchman-4.0.1/src/slack_watchman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 08:08:19.000000 slack-watchman-4.0.1/src/slack_watchman.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:08:19.000000 slack-watchman-4.0.1/src/slack_watchman.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 08:08:19.000000 slack-watchman-4.0.1/src/slack_watchman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 08:08:19.000000 slack-watchman-4.0.1/src/slack_watchman.egg-info/top_level.txt
```

### Comparing `slack-watchman-4.0.0/CHANGELOG.md` & `slack-watchman-4.0.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-## 4.0.0 - 2023-05-03
+## [4.0.1] - 2023-05-05
+### Changed
+- User output in stdout logging now includes display name and email. The accounts for cases where usernames are nonsensical.
+
+## [4.0.0] - 2023-05-03
 This major version release brings multiple updates to Slack Watchman in usability, functionality and behind the scenes improvements.
 
 **Note**: While efforts have been made to make sure there is some backwards compatibility, this release may have some breaking changes on previous versions. Make sure to look at the removed secion
 
 ### Added
 - Support for centralised signatures from the [Watchman Signatures repository](https://github.com/PaperMtn/watchman-signatures)
   - This makes it much easier to keep the signature base for all Watchman applications up to date, and to add functionality to Slack Watchman with new signatures. New signatures are downloaded, and updates to existing signatures are applied, at runtime, meaning Slack Watchman will always be using the most up to date signatures.
@@ -27,66 +31,66 @@
 - Some CSV output
   - For the same reason as above, logging results to CSV has been removed. Enumerating users and channels can still be output to CSV, but formatting a CSV file for a complex nested datastructure is a nightmare, and makes future modifications time consuming.
 - Logging to file
   - To keep logging as simple as possible, the file output option has also been removed. This can easily be reproduced by piping the output of running Slack Watchman to a file:
     - ```slack-watchman --timeframe w --all --output json >> sw-log.json```
 - Local/custom signatures - Centralised signatures mean that user-created custom signatures can't be used with Slack Watchman for Enterprise Grid anymore. If you have made a signature you think would be good for sharing with the community, feel free to add it to the Watchman Signatures repository, so it can be used in all Watchman applications
 
-## 3.0.10 - 2020-11-08
+## [3.0.10] - 2020-11-08
 ### Fixed
 - Retry added for occasional Requests HTTPSConnectionPool error
 ### Added
 - Version added to Stdout logging
 - Better exception handling and logging exceptions correctly
 - Workspace field added to critical error
 
-## 3.0.9 - 2020-10-31
+## [3.0.9] - 2020-10-31
 ### Added
 - Mailgun API token rule
 - Mailchimp API token rule
 - Twilio API token rule
 - Stripe API token rule
 - Heroku API token rule
 - Shodan API token rule
 - Cloudflare API token rule
 
-## 3.0.8 - 2020-10-10
+## [3.0.8] - 2020-10-10
 ### Added
 - Exact regex string match added to output from message searches
 - Check added for when the given token doesn't have the required API scope. On incorrect scope, and exception will be raised and the required scope will be output to log
 
-## 3.0.7 - 2020-10-02
+## [3.0.7] - 2020-10-02
 ### Added
 - Rule to detect MasterCard Datacash credentials
 
-## 3.0.6 - 2020-09-22
+## [3.0.6] - 2020-09-22
 ### Changed
 - File searching now includes user who posted file via users.list API method
 - Logging field name changes = 'type' -> 'detection_type', 'detection' -> 'detection_data'
 
-## 3.0.5 - 2020-09-18
+## [3.0.5] - 2020-09-18
 ### Changed
 - Updated output to strip quotes from query strings. This should allow better JSON parsing with more log ingestors
 - File searching was missing file type output in log data in some occasions, now fixed
 
-## 3.0.4 - 2020-09-10
+## [3.0.4] - 2020-09-10
 ### Added
 - Added rules to search for:
   - CV files
   - Files and spreadsheets containing budget and salary information
 
-## 3.0.2 - 2020-09-06
+## [3.0.2] - 2020-09-06
 ### Added
 - CHANGELOG to track updates
 - Small bug meant that PyPI installations weren't including the YAML rule files. This has now been fixed.
 
 ### Changed
 - Top level dir renamed from `watchman` to `slack_watchman` to place nicer with PyPI
 
-## 3.0.0 - 2020-09-04
+## [3.0.0] - 2020-09-04
 ### Added
 - Rules based searching
 - Logging options: Log file, Stdout, TCP stream
 - Deduplication of output
 - Refactor into slack_wrapper to use a class to create an API client
 
 ### Changed
```

### Comparing `slack-watchman-4.0.0/LICENSE` & `slack-watchman-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.0/PKG-INFO` & `slack-watchman-4.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-watchman
-Version: 4.0.0
+Version: 4.0.1
 Summary: Monitoring and enumerating Slack for exposed secrets
 Home-page: https://github.com/PaperMtn/slack-watchman
 Author: PaperMtn
 Author-email: papermtn@protonmail.com
 License: GPL-3.0
 Keywords: audit,slack,slack-watchman,watchman,blue-team,red-team,threat-hunting
 Classifier: Intended Audience :: Information Technology
@@ -201,15 +201,19 @@
 You may be interested in the other apps in the Watchman family:
 - [Slack Watchman for Enterprise Grid](https://github.com/PaperMtn/slack-watchman-enterprise-grid)
 - [GitLab Watchman](https://github.com/PaperMtn/gitlab-watchman)
 - [GitHub Watchman](https://github.com/PaperMtn/github-watchman)
 
 ## License
 The source code for this project is released under the [GNU General Public Licence](https://www.gnu.org/licenses/licenses.html#GPL). This project is not associated with Slack Technologies or Salesforce.
-## 4.0.0 - 2023-05-03
+## [4.0.1] - 2023-05-05
+### Changed
+- User output in stdout logging now includes display name and email. The accounts for cases where usernames are nonsensical.
+
+## [4.0.0] - 2023-05-03
 This major version release brings multiple updates to Slack Watchman in usability, functionality and behind the scenes improvements.
 
 **Note**: While efforts have been made to make sure there is some backwards compatibility, this release may have some breaking changes on previous versions. Make sure to look at the removed secion
 
 ### Added
 - Support for centralised signatures from the [Watchman Signatures repository](https://github.com/PaperMtn/watchman-signatures)
   - This makes it much easier to keep the signature base for all Watchman applications up to date, and to add functionality to Slack Watchman with new signatures. New signatures are downloaded, and updates to existing signatures are applied, at runtime, meaning Slack Watchman will always be using the most up to date signatures.
@@ -234,66 +238,66 @@
 - Some CSV output
   - For the same reason as above, logging results to CSV has been removed. Enumerating users and channels can still be output to CSV, but formatting a CSV file for a complex nested datastructure is a nightmare, and makes future modifications time consuming.
 - Logging to file
   - To keep logging as simple as possible, the file output option has also been removed. This can easily be reproduced by piping the output of running Slack Watchman to a file:
     - ```slack-watchman --timeframe w --all --output json >> sw-log.json```
 - Local/custom signatures - Centralised signatures mean that user-created custom signatures can't be used with Slack Watchman for Enterprise Grid anymore. If you have made a signature you think would be good for sharing with the community, feel free to add it to the Watchman Signatures repository, so it can be used in all Watchman applications
 
-## 3.0.10 - 2020-11-08
+## [3.0.10] - 2020-11-08
 ### Fixed
 - Retry added for occasional Requests HTTPSConnectionPool error
 ### Added
 - Version added to Stdout logging
 - Better exception handling and logging exceptions correctly
 - Workspace field added to critical error
 
-## 3.0.9 - 2020-10-31
+## [3.0.9] - 2020-10-31
 ### Added
 - Mailgun API token rule
 - Mailchimp API token rule
 - Twilio API token rule
 - Stripe API token rule
 - Heroku API token rule
 - Shodan API token rule
 - Cloudflare API token rule
 
-## 3.0.8 - 2020-10-10
+## [3.0.8] - 2020-10-10
 ### Added
 - Exact regex string match added to output from message searches
 - Check added for when the given token doesn't have the required API scope. On incorrect scope, and exception will be raised and the required scope will be output to log
 
-## 3.0.7 - 2020-10-02
+## [3.0.7] - 2020-10-02
 ### Added
 - Rule to detect MasterCard Datacash credentials
 
-## 3.0.6 - 2020-09-22
+## [3.0.6] - 2020-09-22
 ### Changed
 - File searching now includes user who posted file via users.list API method
 - Logging field name changes = 'type' -> 'detection_type', 'detection' -> 'detection_data'
 
-## 3.0.5 - 2020-09-18
+## [3.0.5] - 2020-09-18
 ### Changed
 - Updated output to strip quotes from query strings. This should allow better JSON parsing with more log ingestors
 - File searching was missing file type output in log data in some occasions, now fixed
 
-## 3.0.4 - 2020-09-10
+## [3.0.4] - 2020-09-10
 ### Added
 - Added rules to search for:
   - CV files
   - Files and spreadsheets containing budget and salary information
 
-## 3.0.2 - 2020-09-06
+## [3.0.2] - 2020-09-06
 ### Added
 - CHANGELOG to track updates
 - Small bug meant that PyPI installations weren't including the YAML rule files. This has now been fixed.
 
 ### Changed
 - Top level dir renamed from `watchman` to `slack_watchman` to place nicer with PyPI
 
-## 3.0.0 - 2020-09-04
+## [3.0.0] - 2020-09-04
 ### Added
 - Rules based searching
 - Logging options: Log file, Stdout, TCP stream
 - Deduplication of output
 - Refactor into slack_wrapper to use a class to create an API client
 
 ### Changed
```

### Comparing `slack-watchman-4.0.0/README.md` & `slack-watchman-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.0/setup.cfg` & `slack-watchman-4.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.0/src/slack_watchman/__init__.py` & `slack-watchman-4.0.1/src/slack_watchman/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,16 +264,16 @@
         OUTPUT_LOGGER.log('INFO', 'Importing signatures...')
         signature_list = load_signatures()
         OUTPUT_LOGGER.log('SUCCESS', f'{len(signature_list)} signatures loaded')
         if cookie:
             OUTPUT_LOGGER.log('SUCCESS', 'Successfully authenticated using cookie')
             OUTPUT_LOGGER.log('SUCCESS', f"This user's SESSION_TOKEN: {slack_con.session_token}")
         OUTPUT_LOGGER.log('SUCCESS',
-                          f'You are authenticated to this workspace as: USER: {auth_data.get("user")}'
-                          f' ID: {auth_data.get("user_id")}')
+                          f'You are authenticated to this workspace as: USER: {calling_user.display_name} '
+                          f'- {calling_user.email} ID: {calling_user.id}')
         OUTPUT_LOGGER.log('USER', calling_user, detect_type='User', notify_type='user')
         OUTPUT_LOGGER.log('WORKSPACE', workspace_information, detect_type='Workspace', notify_type='workspace')
 
         if users:
             OUTPUT_LOGGER.log('INFO', 'Enumerating users...')
             user_list = slack.get_users(slack_con, verbose)
             OUTPUT_LOGGER.log('SUCCESS', f'{len(user_list)} users discovered')
```

### Comparing `slack-watchman-4.0.0/src/slack_watchman/__version__.py` & `slack-watchman-4.0.1/src/slack_watchman/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     '__version__',
     '__author__',
     '__email__',
     '__license__',
 ]
 
 __title__ = 'Slack Watchman'
-__version__ = '4.0.0'
+__version__ = '4.0.1'
 __summary__ = 'Monitoring and enumerating Slack for exposed secrets'
 __author__ = 'PaperMtn'
 __email__ = 'papermtn@protonmail.com'
 __license__ = 'GPL-3.0'
 __uri__ = 'https://github.com/PaperMtn/slack-watchman'
 __copyright__ = f'2023 {__author__}'
```

### Comparing `slack-watchman-4.0.0/src/slack_watchman/exceptions.py` & `slack-watchman-4.0.1/src/slack_watchman/exceptions.py`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.0/src/slack_watchman/models/conversation.py` & `slack-watchman-4.0.1/src/slack_watchman/models/conversation.py`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.0/src/slack_watchman/models/post.py` & `slack-watchman-4.0.1/src/slack_watchman/models/post.py`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.0/src/slack_watchman/models/signature.py` & `slack-watchman-4.0.1/src/slack_watchman/models/signature.py`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.0/src/slack_watchman/models/user.py` & `slack-watchman-4.0.1/src/slack_watchman/models/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 @dataclass(slots=True)
 class UserSuccinct(object):
     """ Class that defines User objects for Slack users"""
 
     id: str
     name: str
     email: str
+    display_name: str
     has_2fa: str
     is_admin: str
 
 
 def create_from_dict(user_dict: Dict,
                      verbose: bool) -> User or UserSuccinct:
     """ Create a User object from a dict response from the Slack API
@@ -97,11 +98,12 @@
             updated=_convert_timestamp(user_dict.get('updated')),
             has_2fa=user_dict.get('has_2fa')
         )
     else:
         return UserSuccinct(
             id=user_dict.get('id'),
             name=user_dict.get('name'),
+            display_name=user_dict.get('profile').get('display_name'),
             has_2fa=user_dict.get('has_2fa'),
             is_admin=user_dict.get('is_admin'),
             email=user_dict.get('profile').get('email')
         )
```

### Comparing `slack-watchman-4.0.0/src/slack_watchman/models/workspace.py` & `slack-watchman-4.0.1/src/slack_watchman/models/workspace.py`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.0/src/slack_watchman/signature_updater.py` & `slack-watchman-4.0.1/src/slack_watchman/signature_updater.py`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.0/src/slack_watchman/slack_wrapper.py` & `slack-watchman-4.0.1/src/slack_watchman/slack_wrapper.py`

 * *Files identical despite different names*

### Comparing `slack-watchman-4.0.0/src/slack_watchman/sw_logger.py` & `slack-watchman-4.0.1/src/slack_watchman/sw_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                       f'    NAME: {message.get("name")}  \n' \
                       f'    DOMAIN: {message.get("domain")}  \n' \
                       f'    URL: {message.get("url")}'
             mes_type = 'WORKSPACE'
         if notify_type == "user":
             message = f'USER: \n' \
                       f'    ID: {message.get("id")}  \n' \
-                      f'    NAME: {message.get("name")}  \n' \
+                      f'    NAME: {message.get("display_name")}  \n' \
                       f'    EMAIL: {message.get("email")}  \n' \
                       f'    JOB_TITLE: {message.get("title")} \n' \
                       f'    ADMIN: {message.get("is_admin")} \n' \
                       f'    OWNER: {message.get("is_owner")} \n' \
                       f'    HAS_2FA: {message.get("has_2fa")}'
             mes_type = 'USER'
         if notify_type == "result":
@@ -55,30 +55,32 @@
                     conversation_type = 'Direct Message'
                 elif message.get('message').get('conversation').get('is_private'):
                     conversation_type = 'Private Channel'
                 else:
                     conversation_type = 'Public Channel'
 
                 if isinstance(message.get('message').get('user'), Mapping):
-                    user = message.get('message', {}).get('user', {}).get('email')
+                    user = f"{message.get('message', {}).get('user', {}).get('display_name')} -" \
+                           f" {message.get('message', {}).get('user', {}).get('email')}"
                 else:
                     user = message.get('message').get('user')
 
                 message = 'POST_TYPE: Message' \
                           f'    POSTED_BY: {user}' \
                           f'    POSTED_ON: {message.get("message").get("created")} \n' \
                           f'    CONVERSATION: {message.get("message").get("conversation").get("name")}' \
                           f'    CONVERSATION_TYPE: {conversation_type}' \
                           f'    URL: {message.get("message").get("permalink")} \n' \
                           f'    POTENTIAL_SECRET: {message.get("match_string")} \n' \
                           f'    -----'
 
             elif message.get('file'):
                 message = 'POST_TYPE: File' \
-                          f'    POSTED_BY: {message.get("user").get("email")}' \
+                          f'    POSTED_BY: {message.get("user", {}).get("display_name")} ' \
+                                f'- {message.get("user").get("email")}' \
                           f'    CREATED: {message.get("file").get("created")} \n' \
                           f'    FILE_NAME: {message.get("file").get("name")} \n' \
                           f'    PRIVATE_URL: {message.get("file").get("url_private_download")} \n' \
                           f'    PUBLIC_PERMALINK: {message.get("file").get("permalink_public")} \n' \
                           f'    -----'
             mes_type = 'RESULT'
         try:
```

### Comparing `slack-watchman-4.0.0/src/slack_watchman.egg-info/PKG-INFO` & `slack-watchman-4.0.1/src/slack_watchman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-watchman
-Version: 4.0.0
+Version: 4.0.1
 Summary: Monitoring and enumerating Slack for exposed secrets
 Home-page: https://github.com/PaperMtn/slack-watchman
 Author: PaperMtn
 Author-email: papermtn@protonmail.com
 License: GPL-3.0
 Keywords: audit,slack,slack-watchman,watchman,blue-team,red-team,threat-hunting
 Classifier: Intended Audience :: Information Technology
@@ -201,15 +201,19 @@
 You may be interested in the other apps in the Watchman family:
 - [Slack Watchman for Enterprise Grid](https://github.com/PaperMtn/slack-watchman-enterprise-grid)
 - [GitLab Watchman](https://github.com/PaperMtn/gitlab-watchman)
 - [GitHub Watchman](https://github.com/PaperMtn/github-watchman)
 
 ## License
 The source code for this project is released under the [GNU General Public Licence](https://www.gnu.org/licenses/licenses.html#GPL). This project is not associated with Slack Technologies or Salesforce.
-## 4.0.0 - 2023-05-03
+## [4.0.1] - 2023-05-05
+### Changed
+- User output in stdout logging now includes display name and email. The accounts for cases where usernames are nonsensical.
+
+## [4.0.0] - 2023-05-03
 This major version release brings multiple updates to Slack Watchman in usability, functionality and behind the scenes improvements.
 
 **Note**: While efforts have been made to make sure there is some backwards compatibility, this release may have some breaking changes on previous versions. Make sure to look at the removed secion
 
 ### Added
 - Support for centralised signatures from the [Watchman Signatures repository](https://github.com/PaperMtn/watchman-signatures)
   - This makes it much easier to keep the signature base for all Watchman applications up to date, and to add functionality to Slack Watchman with new signatures. New signatures are downloaded, and updates to existing signatures are applied, at runtime, meaning Slack Watchman will always be using the most up to date signatures.
@@ -234,66 +238,66 @@
 - Some CSV output
   - For the same reason as above, logging results to CSV has been removed. Enumerating users and channels can still be output to CSV, but formatting a CSV file for a complex nested datastructure is a nightmare, and makes future modifications time consuming.
 - Logging to file
   - To keep logging as simple as possible, the file output option has also been removed. This can easily be reproduced by piping the output of running Slack Watchman to a file:
     - ```slack-watchman --timeframe w --all --output json >> sw-log.json```
 - Local/custom signatures - Centralised signatures mean that user-created custom signatures can't be used with Slack Watchman for Enterprise Grid anymore. If you have made a signature you think would be good for sharing with the community, feel free to add it to the Watchman Signatures repository, so it can be used in all Watchman applications
 
-## 3.0.10 - 2020-11-08
+## [3.0.10] - 2020-11-08
 ### Fixed
 - Retry added for occasional Requests HTTPSConnectionPool error
 ### Added
 - Version added to Stdout logging
 - Better exception handling and logging exceptions correctly
 - Workspace field added to critical error
 
-## 3.0.9 - 2020-10-31
+## [3.0.9] - 2020-10-31
 ### Added
 - Mailgun API token rule
 - Mailchimp API token rule
 - Twilio API token rule
 - Stripe API token rule
 - Heroku API token rule
 - Shodan API token rule
 - Cloudflare API token rule
 
-## 3.0.8 - 2020-10-10
+## [3.0.8] - 2020-10-10
 ### Added
 - Exact regex string match added to output from message searches
 - Check added for when the given token doesn't have the required API scope. On incorrect scope, and exception will be raised and the required scope will be output to log
 
-## 3.0.7 - 2020-10-02
+## [3.0.7] - 2020-10-02
 ### Added
 - Rule to detect MasterCard Datacash credentials
 
-## 3.0.6 - 2020-09-22
+## [3.0.6] - 2020-09-22
 ### Changed
 - File searching now includes user who posted file via users.list API method
 - Logging field name changes = 'type' -> 'detection_type', 'detection' -> 'detection_data'
 
-## 3.0.5 - 2020-09-18
+## [3.0.5] - 2020-09-18
 ### Changed
 - Updated output to strip quotes from query strings. This should allow better JSON parsing with more log ingestors
 - File searching was missing file type output in log data in some occasions, now fixed
 
-## 3.0.4 - 2020-09-10
+## [3.0.4] - 2020-09-10
 ### Added
 - Added rules to search for:
   - CV files
   - Files and spreadsheets containing budget and salary information
 
-## 3.0.2 - 2020-09-06
+## [3.0.2] - 2020-09-06
 ### Added
 - CHANGELOG to track updates
 - Small bug meant that PyPI installations weren't including the YAML rule files. This has now been fixed.
 
 ### Changed
 - Top level dir renamed from `watchman` to `slack_watchman` to place nicer with PyPI
 
-## 3.0.0 - 2020-09-04
+## [3.0.0] - 2020-09-04
 ### Added
 - Rules based searching
 - Logging options: Log file, Stdout, TCP stream
 - Deduplication of output
 - Refactor into slack_wrapper to use a class to create an API client
 
 ### Changed
```

### Comparing `slack-watchman-4.0.0/src/slack_watchman.egg-info/SOURCES.txt` & `slack-watchman-4.0.1/src/slack_watchman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

