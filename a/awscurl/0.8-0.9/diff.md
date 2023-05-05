# Comparing `tmp/awscurl-0.8.tar.gz` & `tmp/awscurl-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/awscurl-0.8.tar", last modified: Thu Oct 13 07:30:41 2016, max compression
+gzip compressed data, was "dist/awscurl-0.9.tar", last modified: Tue Jul 25 20:59:11 2017, max compression
```

## Comparing `awscurl-0.8.tar` & `awscurl-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 iokulist   (502) staff       (20)        0 2016-10-13 07:30:41.000000 awscurl-0.8/
-drwxr-xr-x   0 iokulist   (502) staff       (20)        0 2016-10-13 07:30:41.000000 awscurl-0.8/awscurl/
--rw-r--r--   0 iokulist   (502) staff       (20)        0 2016-10-12 16:26:20.000000 awscurl-0.8/awscurl/__init__.py
--rw-r--r--   0 iokulist   (502) staff       (20)      183 2016-10-12 16:26:20.000000 awscurl-0.8/awscurl/__main__.py
--rwxr-xr-x   0 iokulist   (502) staff       (20)    10774 2016-10-12 16:26:20.000000 awscurl-0.8/awscurl/awscurl.py
-drwxr-xr-x   0 iokulist   (502) staff       (20)        0 2016-10-13 07:30:41.000000 awscurl-0.8/awscurl.egg-info/
--rw-r--r--   0 iokulist   (502) staff       (20)        1 2016-10-13 07:30:41.000000 awscurl-0.8/awscurl.egg-info/dependency_links.txt
--rw-r--r--   0 iokulist   (502) staff       (20)       51 2016-10-13 07:30:41.000000 awscurl-0.8/awscurl.egg-info/entry_points.txt
--rw-r--r--   0 iokulist   (502) staff       (20)        1 2016-10-12 16:37:32.000000 awscurl-0.8/awscurl.egg-info/not-zip-safe
--rw-r--r--   0 iokulist   (502) staff       (20)      246 2016-10-13 07:30:41.000000 awscurl-0.8/awscurl.egg-info/PKG-INFO
--rw-r--r--   0 iokulist   (502) staff       (20)       53 2016-10-13 07:30:41.000000 awscurl-0.8/awscurl.egg-info/requires.txt
--rw-r--r--   0 iokulist   (502) staff       (20)      285 2016-10-13 07:30:41.000000 awscurl-0.8/awscurl.egg-info/SOURCES.txt
--rw-r--r--   0 iokulist   (502) staff       (20)        8 2016-10-13 07:30:41.000000 awscurl-0.8/awscurl.egg-info/top_level.txt
--rw-r--r--   0 iokulist   (502) staff       (20)      246 2016-10-13 07:30:41.000000 awscurl-0.8/PKG-INFO
--rw-r--r--   0 iokulist   (502) staff       (20)       59 2016-10-13 07:30:41.000000 awscurl-0.8/setup.cfg
--rw-r--r--   0 iokulist   (502) staff       (20)      573 2016-10-12 16:26:20.000000 awscurl-0.8/setup.py
+drwxr-xr-x   0 iokulist   (501) staff       (20)        0 2017-07-25 20:59:11.000000 awscurl-0.9/
+drwxr-xr-x   0 iokulist   (501) staff       (20)        0 2017-07-25 20:59:11.000000 awscurl-0.9/awscurl/
+-rw-r--r--   0 iokulist   (501) staff       (20)        0 2017-07-25 19:55:22.000000 awscurl-0.9/awscurl/__init__.py
+-rw-r--r--   0 iokulist   (501) staff       (20)      183 2017-07-25 19:55:22.000000 awscurl-0.9/awscurl/__main__.py
+-rwxr-xr-x   0 iokulist   (501) staff       (20)    11207 2017-07-25 19:55:22.000000 awscurl-0.9/awscurl/awscurl.py
+drwxr-xr-x   0 iokulist   (501) staff       (20)        0 2017-07-25 20:59:11.000000 awscurl-0.9/awscurl.egg-info/
+-rw-r--r--   0 iokulist   (501) staff       (20)        1 2017-07-25 20:59:11.000000 awscurl-0.9/awscurl.egg-info/dependency_links.txt
+-rw-r--r--   0 iokulist   (501) staff       (20)       51 2017-07-25 20:59:11.000000 awscurl-0.9/awscurl.egg-info/entry_points.txt
+-rw-r--r--   0 iokulist   (501) staff       (20)        1 2017-07-25 20:30:41.000000 awscurl-0.9/awscurl.egg-info/not-zip-safe
+-rw-r--r--   0 iokulist   (501) staff       (20)      246 2017-07-25 20:59:11.000000 awscurl-0.9/awscurl.egg-info/PKG-INFO
+-rw-r--r--   0 iokulist   (501) staff       (20)       53 2017-07-25 20:59:11.000000 awscurl-0.9/awscurl.egg-info/requires.txt
+-rw-r--r--   0 iokulist   (501) staff       (20)      285 2017-07-25 20:59:11.000000 awscurl-0.9/awscurl.egg-info/SOURCES.txt
+-rw-r--r--   0 iokulist   (501) staff       (20)        8 2017-07-25 20:59:11.000000 awscurl-0.9/awscurl.egg-info/top_level.txt
+-rw-r--r--   0 iokulist   (501) staff       (20)      246 2017-07-25 20:59:11.000000 awscurl-0.9/PKG-INFO
+-rw-r--r--   0 iokulist   (501) staff       (20)       38 2017-07-25 20:59:11.000000 awscurl-0.9/setup.cfg
+-rw-r--r--   0 iokulist   (501) staff       (20)      573 2017-07-25 20:31:27.000000 awscurl-0.9/setup.py
```

### Comparing `awscurl-0.8/awscurl/awscurl.py` & `awscurl-0.9/awscurl/awscurl.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,14 +91,17 @@
     def get_signature_key(key, date_stamp, region_name, service_name):
         k_date = sign(('AWS4' + key).encode('utf-8'), date_stamp)
         k_region = sign(k_date, region_name)
         k_service = sign(k_region, service_name)
         k_signing = sign(k_service, 'aws4_request')
         return k_signing
 
+    def sha256_hash(val):
+        return hashlib.sha256(val.encode('utf-8')).hexdigest()
+
     if access_key is None or secret_key is None:
         try:
             config = configparser.ConfigParser()
             config.read(expanduser("~") + "/.aws/credentials")
 
             access_key = access_key or config.get(profile, "aws_access_key_id")
             secret_key = secret_key or config.get(profile,
@@ -145,24 +148,30 @@
         fullhost = host + ':' + port
     # Step 4: Create the canonical headers and signed headers. Header names
     # and value must be trimmed and lowercase, and sorted in ASCII order.
     # Note that there is a trailing \n.
     canonical_headers = ('host:' + fullhost + '\n' +
                          'x-amz-date:' + amzdate + '\n')
 
+    if security_token:
+        canonical_headers += ('x-amz-security-token:' + security_token + '\n')
+
     # Step 5: Create the list of signed headers. This lists the headers
     # in the canonical_headers list, delimited with ";" and in alpha order.
     # Note: The request can include any headers; canonical_headers and
     # signed_headers lists those that you want to be included in the
     # hash of the request. "Host" and "x-amz-date" are always required.
     signed_headers = 'host;x-amz-date'
 
+    if security_token:
+        signed_headers += ';x-amz-security-token'
+
     # Step 6: Create payload hash (hash of the request body content). For GET
     # requests, the payload is an empty string ("").
-    payload_hash = hashlib.sha256(data).hexdigest()
+    payload_hash = sha256_hash(data)
 
     # Step 7: Combine elements to create create canonical request
     canonical_request = (method + '\n' +
                          canonical_uri + '\n' +
                          canonical_querystring + '\n' +
                          canonical_headers + '\n' +
                          signed_headers + '\n' +
@@ -176,15 +185,15 @@
     credential_scope = (datestamp + '/' +
                         region + '/' +
                         service + '/' +
                         'aws4_request')
     string_to_sign = (algorithm + '\n' +
                       amzdate + '\n' +
                       credential_scope + '\n' +
-                      hashlib.sha256(canonical_request).hexdigest())
+                      sha256_hash(canonical_request))
 
     log('\nSTRING_TO_SIGN = ' + string_to_sign)
     # ************* TASK 3: CALCULATE THE SIGNATURE *************
     # Create the signing key using the function defined above.
     signing_key = get_signature_key(secret_key, datestamp, region, service)
 
     # Sign the string_to_sign using the signing_key
@@ -264,25 +273,29 @@
                         help='verbose flag', default=False)
     parser.add_argument('-X', '--request',
                         help='Specify request command to use',
                         default='GET')
     parser.add_argument('-d', '--data', help='HTTP POST data', default='')
     parser.add_argument('-H', '--header', help='HTTP header', action='append')
 
-    parser.add_argument('--region', help='AWS region', default='us-east-1')
+    parser.add_argument('--region',
+                        help='AWS region',
+                        default='us-east-1',
+                        env_var='AWS_DEFAULT_REGION')
     parser.add_argument('--profile',
                         help='AWS profile',
                         default='default',
                         env_var='AWS_PROFILE')
     parser.add_argument('--service',
                         help='AWS service',
                         default='execute-api')
     parser.add_argument('--access_key', env_var='AWS_ACCESS_KEY_ID')
     parser.add_argument('--secret_key', env_var='AWS_SECRET_ACCESS_KEY')
     parser.add_argument('--security_token', env_var='AWS_SECURITY_TOKEN')
+    parser.add_argument('--session_token', env_var='AWS_SESSION_TOKEN')
 
     parser.add_argument('uri')
 
     args = parser.parse_args()
 
     if args.verbose:
         log(vars(parser.parse_args()))
@@ -304,13 +317,13 @@
                         args.region,
                         args.uri,
                         headers,
                         data,
                         args.profile,
                         args.access_key,
                         args.secret_key,
-                        args.security_token
+                        args.security_token or args.session_token
                         )
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `awscurl-0.8/setup.py` & `awscurl-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = 'iokulist'
 
 from setuptools import setup
 
 setup(
     name='awscurl',
-    version='0.8',
+    version='0.9',
     description='Curl like tool with AWS request signing',
     url='http://github.com/okigan/awscurl',
     author='Igor Okulist',
     author_email='okigan@gmail.com',
     license='MIT',
     packages=['awscurl'],
     entry_points={
```

