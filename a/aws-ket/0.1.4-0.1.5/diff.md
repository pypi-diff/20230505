# Comparing `tmp/aws-ket-0.1.4.tar.gz` & `tmp/aws-ket-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ket-0.1.4.tar", last modified: Fri Apr 14 21:58:12 2023, max compression
+gzip compressed data, was "aws-ket-0.1.5.tar", last modified: Fri May  5 04:15:27 2023, max compression
```

## Comparing `aws-ket-0.1.4.tar` & `aws-ket-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-04-14 21:58:12.840353 aws-ket-0.1.4/
--rw-r--r--   0 sayefiqbal   (502) staff       (20)     1452 2023-03-18 01:01:48.000000 aws-ket-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 sayefiqbal   (502) staff       (20)    11357 2023-02-09 13:04:42.000000 aws-ket-0.1.4/LICENSE
--rw-r--r--   0 sayefiqbal   (502) staff       (20)      396 2023-03-24 00:07:58.000000 aws-ket-0.1.4/MANIFEST.in
--rw-r--r--   0 sayefiqbal   (502) staff       (20)     2150 2023-04-14 14:05:00.000000 aws-ket-0.1.4/Makefile
--rw-r--r--   0 sayefiqbal   (502) staff       (20)     3061 2023-04-14 21:58:12.840119 aws-ket-0.1.4/PKG-INFO
--rw-r--r--   0 sayefiqbal   (502) staff       (20)     2699 2023-04-14 13:55:20.000000 aws-ket-0.1.4/README.md
-drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-04-14 21:58:12.838457 aws-ket-0.1.4/aws_ket.egg-info/
--rw-r--r--   0 sayefiqbal   (502) staff       (20)     3061 2023-04-14 21:58:12.000000 aws-ket-0.1.4/aws_ket.egg-info/PKG-INFO
--rw-r--r--   0 sayefiqbal   (502) staff       (20)      230 2023-04-14 21:58:12.000000 aws-ket-0.1.4/aws_ket.egg-info/SOURCES.txt
--rw-r--r--   0 sayefiqbal   (502) staff       (20)        1 2023-04-14 21:58:12.000000 aws-ket-0.1.4/aws_ket.egg-info/dependency_links.txt
--rw-r--r--   0 sayefiqbal   (502) staff       (20)        1 2023-04-14 21:58:12.000000 aws-ket-0.1.4/aws_ket.egg-info/top_level.txt
-drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-04-14 21:58:12.839148 aws-ket-0.1.4/awsket/
--rwxr-xr-x   0 sayefiqbal   (502) staff       (20)     2882 2023-04-14 19:22:08.000000 aws-ket-0.1.4/awsket/app.py
--rw-r--r--   0 sayefiqbal   (502) staff       (20)    15104 2023-04-14 14:05:00.000000 aws-ket-0.1.4/awsket/ket.py
--rw-r--r--   0 sayefiqbal   (502) staff       (20)     2253 2023-04-14 21:56:24.000000 aws-ket-0.1.4/pyproject.toml
--rw-r--r--   0 sayefiqbal   (502) staff       (20)       38 2023-04-14 21:58:12.840427 aws-ket-0.1.4/setup.cfg
--rw-r--r--   0 sayefiqbal   (502) staff       (20)      772 2023-04-14 21:56:24.000000 aws-ket-0.1.4/setup.py
+drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-05-05 04:15:27.248945 aws-ket-0.1.5/
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     1452 2023-03-18 01:01:48.000000 aws-ket-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)    11357 2023-02-09 13:04:42.000000 aws-ket-0.1.5/LICENSE
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)      396 2023-03-24 00:07:58.000000 aws-ket-0.1.5/MANIFEST.in
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     2150 2023-04-14 14:05:00.000000 aws-ket-0.1.5/Makefile
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     4318 2023-05-05 04:15:27.248542 aws-ket-0.1.5/PKG-INFO
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     3956 2023-05-05 03:04:42.000000 aws-ket-0.1.5/README.md
+drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-05-05 04:15:27.246582 aws-ket-0.1.5/aws_ket.egg-info/
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     4318 2023-05-05 04:15:27.000000 aws-ket-0.1.5/aws_ket.egg-info/PKG-INFO
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)      230 2023-05-05 04:15:27.000000 aws-ket-0.1.5/aws_ket.egg-info/SOURCES.txt
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)        1 2023-05-05 04:15:27.000000 aws-ket-0.1.5/aws_ket.egg-info/dependency_links.txt
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)        1 2023-05-05 04:15:27.000000 aws-ket-0.1.5/aws_ket.egg-info/top_level.txt
+drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-05-05 04:15:27.247627 aws-ket-0.1.5/awsket/
+-rwxr-xr-x   0 sayefiqbal   (502) staff       (20)     2882 2023-05-04 02:24:22.000000 aws-ket-0.1.5/awsket/app.py
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)    15104 2023-04-14 14:05:00.000000 aws-ket-0.1.5/awsket/ket.py
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     2253 2023-05-05 04:12:35.000000 aws-ket-0.1.5/pyproject.toml
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)       38 2023-05-05 04:15:27.249072 aws-ket-0.1.5/setup.cfg
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)      772 2023-05-05 04:12:35.000000 aws-ket-0.1.5/setup.py
```

### Comparing `aws-ket-0.1.4/CONTRIBUTING.md` & `aws-ket-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aws-ket-0.1.4/LICENSE` & `aws-ket-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ket-0.1.4/Makefile` & `aws-ket-0.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `aws-ket-0.1.4/PKG-INFO` & `aws-ket-0.1.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ket
-Version: 0.1.4
+Version: 0.1.5
 Summary: Utility tool to encrypt data using AWS KMS and store it in preferred backend.
 Home-page: https://github.com/sayefiqb/aws-ket
 Author: Sayef Iqbal
 Author-email: s2400@columbia.edu
 Maintainer: Sayef Iqbal
 License: UNKNOWN
 Platform: UNKNOWN
@@ -19,25 +19,27 @@
 ## Overview
 AWS-KET (AWS KMS Encryption Tool) uses AWS KMS Key to encrypt and decrypt files/contents based on user provided kms keys and push them to a datastore backend (S3, RDS or DynamoDB).
 
 
 ![GitHub issues](https://img.shields.io/github/issues/sayefiqb/aws-ket)
 [![CodeQL](https://github.com/sayefiqb/aws-ket/actions/workflows/github-code-scanning/codeql/badge.svg?branch=main)](https://github.com/sayefiqb/aws-ket/actions/workflows/github-code-scanning/codeql) [![Build Status](https://github.com/sayefiqb/aws-ket/actions/workflows/build.yaml/badge.svg)](https://github.com/sayefiqb/aws-ket/actions/workflows/build.yaml) [![codecov](https://codecov.io/gh/sayefiqb/aws-ket/branch/main/graph/badge.svg?token=13922GT547)](https://codecov.io/gh/sayefiqb/aws-ket)[![PyPI](https://img.shields.io/pypi/v/aws-ket)](https://pypi.org/project/aws-ket)[![Documentation Status](https://readthedocs.org/projects/aws-ket/badge/?version=latest)](https://aws-ket.readthedocs.io/en/latest/?badge=latest)
 
-#### Setup
+### Setup
 
 This application will only work if you have AWS account with full privileges on KMS and S3 services in AWS. You should also have aws cli tool installed.
 
 [Setup AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)
 
 **Note:** Currently this tool only uses AWS region `us-east-2` for usage of kms and s3.
 
+### Using Source Code
 #### Initaliztion of app
 ```
-cd src
+git clone git@github.com:sayefiqb/aws-ket.git
+cd awsket
 python init.py
 ```
 
 #### Encrypt text/file
 ```
 python app.py --text <TEXT_TO_ENCRYPT> --save <FILE_NAME_IN_S3> 
 python app.py --file <PATH_OF_FILE_TO_ENCRYPT> --save <FILE_NAME_IN_S3>
@@ -57,24 +59,74 @@
 
 #### Cleanup
 To cleanup your S3 bucket and start over
 ```
 python cleanup.py
 ```
 
+### Using Library form Pypi
+```
+pip install aws-ket
+```
+#### Initaliztion of app
+```
+from awsket import ket
+
+AWS_REGION = 'us-east-2'
+KMS_ALIAS = 'alias/aws-ket'
+
+user_name = ket.get_iam_user()['UserId'].lower()
+bucket_name = f'aws-ket-{user_name}'
+ket.create_s3_bucket(bucket_name, AWS_REGION)
+alias_name = ket.check_alias(KMS_ALIAS, AWS_REGION)
+kms_key_id = ket.create_kms_key(AWS_REGION)
+alias_name = ket.create_kms_alias(kms_key_id, KMS_ALIAS, AWS_REGION)
+```
+
+#### Encrypt text
+```
+from awsket import ket
+
+AWS_REGION = 'us-east-2'
+KMS_ALIAS = 'alias/aws-ket'
+TEXT = 'This is a sample text for testing encryption! Happy coding :)'
+FILE = 'EXAMPLE.txt'
+
+
+user_name = ket.get_iam_user()['UserId'].lower()
+bucket_name = f'aws-ket-{user_name}'
+encrypted_string = ket.encrypt_text(KMS_ALIAS, TEXT, AWS_REGION)
+ket.push_to_s3(bucket_name, FILE, encrypted_string, AWS_REGION)
+```
+
+#### Decrypt text
+```
+from awsket import ket
+
+AWS_REGION = 'us-east-2'
+KMS_ALIAS = 'alias/aws-ket'
+FILE = 'EXAMPLE.txt'
+
+user_name = ket.get_iam_user()['UserId'].lower()
+bucket_name = f'aws-ket-{user_name}'
+decrypted_text = ket.decrypt_text(bucket_name, FILE, KMS_ALIAS, AWS_REGION)
+print(decrypted_text)
+
+```
+
 
-#### Details
+### Details
 This project uses `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make lint`: perform lint using `black`
 - `make scan`: run static analysis on code using `flake8`
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 
 `coverage` output can also be found in html format in `htmlcover` directory.
 
-#### Example
+### Example
 
 First download the source code
 ![](aws-ket.gif)
```

### Comparing `aws-ket-0.1.4/README.md` & `aws-ket-0.1.5/aws_ket.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,45 @@
+Metadata-Version: 2.1
+Name: aws-ket
+Version: 0.1.5
+Summary: Utility tool to encrypt data using AWS KMS and store it in preferred backend.
+Home-page: https://github.com/sayefiqb/aws-ket
+Author: Sayef Iqbal
+Author-email: s2400@columbia.edu
+Maintainer: Sayef Iqbal
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # aws-ket
 Utility tool to encrypt data using AWS KMS and store it in preferred backend.
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ## Overview
 AWS-KET (AWS KMS Encryption Tool) uses AWS KMS Key to encrypt and decrypt files/contents based on user provided kms keys and push them to a datastore backend (S3, RDS or DynamoDB).
 
 
 ![GitHub issues](https://img.shields.io/github/issues/sayefiqb/aws-ket)
 [![CodeQL](https://github.com/sayefiqb/aws-ket/actions/workflows/github-code-scanning/codeql/badge.svg?branch=main)](https://github.com/sayefiqb/aws-ket/actions/workflows/github-code-scanning/codeql) [![Build Status](https://github.com/sayefiqb/aws-ket/actions/workflows/build.yaml/badge.svg)](https://github.com/sayefiqb/aws-ket/actions/workflows/build.yaml) [![codecov](https://codecov.io/gh/sayefiqb/aws-ket/branch/main/graph/badge.svg?token=13922GT547)](https://codecov.io/gh/sayefiqb/aws-ket)[![PyPI](https://img.shields.io/pypi/v/aws-ket)](https://pypi.org/project/aws-ket)[![Documentation Status](https://readthedocs.org/projects/aws-ket/badge/?version=latest)](https://aws-ket.readthedocs.io/en/latest/?badge=latest)
 
-#### Setup
+### Setup
 
 This application will only work if you have AWS account with full privileges on KMS and S3 services in AWS. You should also have aws cli tool installed.
 
 [Setup AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)
 
 **Note:** Currently this tool only uses AWS region `us-east-2` for usage of kms and s3.
 
+### Using Source Code
 #### Initaliztion of app
 ```
-cd src
+git clone git@github.com:sayefiqb/aws-ket.git
+cd awsket
 python init.py
 ```
 
 #### Encrypt text/file
 ```
 python app.py --text <TEXT_TO_ENCRYPT> --save <FILE_NAME_IN_S3> 
 python app.py --file <PATH_OF_FILE_TO_ENCRYPT> --save <FILE_NAME_IN_S3>
@@ -44,23 +59,74 @@
 
 #### Cleanup
 To cleanup your S3 bucket and start over
 ```
 python cleanup.py
 ```
 
+### Using Library form Pypi
+```
+pip install aws-ket
+```
+#### Initaliztion of app
+```
+from awsket import ket
+
+AWS_REGION = 'us-east-2'
+KMS_ALIAS = 'alias/aws-ket'
+
+user_name = ket.get_iam_user()['UserId'].lower()
+bucket_name = f'aws-ket-{user_name}'
+ket.create_s3_bucket(bucket_name, AWS_REGION)
+alias_name = ket.check_alias(KMS_ALIAS, AWS_REGION)
+kms_key_id = ket.create_kms_key(AWS_REGION)
+alias_name = ket.create_kms_alias(kms_key_id, KMS_ALIAS, AWS_REGION)
+```
+
+#### Encrypt text
+```
+from awsket import ket
+
+AWS_REGION = 'us-east-2'
+KMS_ALIAS = 'alias/aws-ket'
+TEXT = 'This is a sample text for testing encryption! Happy coding :)'
+FILE = 'EXAMPLE.txt'
 
-#### Details
+
+user_name = ket.get_iam_user()['UserId'].lower()
+bucket_name = f'aws-ket-{user_name}'
+encrypted_string = ket.encrypt_text(KMS_ALIAS, TEXT, AWS_REGION)
+ket.push_to_s3(bucket_name, FILE, encrypted_string, AWS_REGION)
+```
+
+#### Decrypt text
+```
+from awsket import ket
+
+AWS_REGION = 'us-east-2'
+KMS_ALIAS = 'alias/aws-ket'
+FILE = 'EXAMPLE.txt'
+
+user_name = ket.get_iam_user()['UserId'].lower()
+bucket_name = f'aws-ket-{user_name}'
+decrypted_text = ket.decrypt_text(bucket_name, FILE, KMS_ALIAS, AWS_REGION)
+print(decrypted_text)
+
+```
+
+
+### Details
 This project uses `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make lint`: perform lint using `black`
 - `make scan`: run static analysis on code using `flake8`
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 
 `coverage` output can also be found in html format in `htmlcover` directory.
 
-#### Example
+### Example
 
 First download the source code
-![](aws-ket.gif)
+![](aws-ket.gif)
+
```

### Comparing `aws-ket-0.1.4/awsket/app.py` & `aws-ket-0.1.5/awsket/app.py`

 * *Files identical despite different names*

### Comparing `aws-ket-0.1.4/awsket/ket.py` & `aws-ket-0.1.5/awsket/ket.py`

 * *Files identical despite different names*

### Comparing `aws-ket-0.1.4/pyproject.toml` & `aws-ket-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "aws-ket"
 authors = [{name = "Sayef Iqbal", email = "si2400@columbia.edu"}]
 description="Utility tool to encrypt data using AWS KMS and store it in preferred backend."
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 requires-python = ">=3.9"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `aws-ket-0.1.4/setup.py` & `aws-ket-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 setup(
     name             = 'aws-ket',
     author           = 'Sayef Iqbal',
     author_email     = 's2400@columbia.edu',
     maintainer       = 'Sayef Iqbal',
     url              = 'https://github.com/sayefiqb/aws-ket',
     description      = 'Utility tool to encrypt data using AWS KMS and store it in preferred backend.',
```

