# Comparing `tmp/pibble-0.5.2.tar.gz` & `tmp/pibble-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pibble-0.5.2.tar", last modified: Wed May  3 23:41:37 2023, max compression
+gzip compressed data, was "pibble-0.5.3.tar", last modified: Fri May  5 02:51:02 2023, max compression
```

## Comparing `pibble-0.5.2.tar` & `pibble-0.5.3.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.684939 pibble-0.5.2/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-05-03 23:41:37.684939 pibble-0.5.2/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5919 2023-05-03 23:41:37.000000 pibble-0.5.2/README.md
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.672940 pibble-0.5.2/pibble/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     8955 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/__main__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.672940 pibble-0.5.2/pibble/api/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3374 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.672940 pibble-0.5.2/pibble/api/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.672940 pibble-0.5.2/pibble/api/client/apachethrift/
--rw-------   0 benjamin  (1000) benjamin  (1000)     6195 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/apachethrift/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1340 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.672940 pibble-0.5.2/pibble/api/client/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    14230 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/file/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9726 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/file/hdfs.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    12782 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/file/local.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    19652 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4132 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.672940 pibble-0.5.2/pibble/api/client/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4728 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16837 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2312 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/webservice/jsonapi.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.672940 pibble-0.5.2/pibble/api/client/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11386 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4766 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10690 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6689 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/webservice/soap.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7333 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/webservice/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/client/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/configuration.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6101 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/exceptions.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.672940 pibble-0.5.2/pibble/api/helpers/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/helpers/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15706 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/helpers/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    20612 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/helpers/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    24691 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/helpers/googlerpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13415 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/helpers/store.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13868 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/helpers/wrappers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/meta/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/meta/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9492 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/meta/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2952 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/meta/helpers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/middleware/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/middleware/apachethrift/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/apachethrift/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/apachethrift/screening.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/middleware/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3730 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/database/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/middleware/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      454 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/file/temp.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/middleware/googlerpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/googlerpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/googlerpc/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/googlerpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/googlerpc/metadata.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3703 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/middleware/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/webservice/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/middleware/webservice/authentication/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/webservice/authentication/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/webservice/authentication/basic.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/webservice/authentication/bearer.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13472 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/webservice/authentication/digest.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/webservice/authentication/header.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    17704 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/webservice/authentication/oauth.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3256 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/webservice/limit.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/middleware/webservice/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/protocol/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/protocol/__init__.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19486 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/protocol/apachethrift.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2451 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2080 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/server/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/server/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/server/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15640 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/server/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5453 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/server/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/api/server/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2296 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7311 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/awslambda.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    39095 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/server/webservice/drivers/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/drivers/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1489 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/drivers/driver_cherrypy.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2194 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/drivers/driver_gunicorn.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1078 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/drivers/driver_werkzeug.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15947 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/handler.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3164 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/jsonapi.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      969 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/server/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4150 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6457 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    12004 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16962 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/soap.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.676940 pibble-0.5.2/pibble/api/server/webservice/template/
--rw-------   0 benjamin  (1000) benjamin  (1000)     9717 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/template/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9201 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/template/extensions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9770 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/api/server/webservice/template/loader.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7797 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/database/dedupe.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10529 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/database/engine.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/database/exceptions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    26274 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/database/orm.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/database/util.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/cms/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/cms/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/cms/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/cms/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/cms/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/cms/database/interface.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/cms/database/menu.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/cms/database/view.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1366 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/cms/middleware.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/cms/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/cms/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6660 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/cms/server/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3012 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/cms/server/extension.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/dam/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/dam/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/dam/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/dam/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/dam/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/dam/database/files.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/dam/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/dam/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/dam/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/rest/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/rest/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/rest/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/rest/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/rest/database/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/rest/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/rest/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15662 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/rest/server/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7244 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/rest/server/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/session/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/session/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/session/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/session/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/session/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/session/database/session.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/session/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/session/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5087 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/session/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/user/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/user/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/user/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/user/client/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      985 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/user/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/user/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/user/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/user/database/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/user/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/user/database/notification.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/user/database/permission.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/user/database/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/ext/user/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/user/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    24935 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/ext/user/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/hooks/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/hooks/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6037 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/hooks/aws.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/media/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/media/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10388 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/media/thumbnail.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/resources/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/resources/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10655 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/resources/retriever.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.680940 pibble-0.5.2/pibble/scripts/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/scripts/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1909 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/scripts/importcheck.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1726 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/scripts/templatefiles.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/setup.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.684939 pibble-0.5.2/pibble/util/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/util/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     8357 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/util/encryption.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16171 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/util/files.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    32821 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/util/helpers.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/util/imaging.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6330 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/util/log.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1701 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/util/numeric.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    27116 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble/util/strings.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.684939 pibble-0.5.2/pibble/web/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/web/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3227 2023-05-03 23:41:36.000000 pibble-0.5.2/pibble/web/scraper.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-03 23:41:37.672940 pibble-0.5.2/pibble.egg-info/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble.egg-info/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5627 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble.egg-info/SOURCES.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble.egg-info/dependency_links.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble.egg-info/entry_points.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1936 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble.egg-info/requires.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-05-03 23:41:37.000000 pibble-0.5.2/pibble.egg-info/top_level.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-05-03 23:41:37.684939 pibble-0.5.2/setup.cfg
--rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-03 23:41:37.000000 pibble-0.5.2/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-05-05 02:51:02.911108 pibble-0.5.3/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5919 2023-05-05 02:51:02.000000 pibble-0.5.3/README.md
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     8955 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/__main__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble/api/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3374 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble/api/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble/api/client/apachethrift/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6195 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/apachethrift/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1340 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble/api/client/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    14230 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/file/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9726 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/file/hdfs.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    12782 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/file/local.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    19652 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4132 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble/api/client/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4728 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16837 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2312 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/webservice/jsonapi.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble/api/client/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11386 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4766 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10690 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6689 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/webservice/soap.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7333 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/webservice/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/client/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/configuration.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6101 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/exceptions.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble/api/helpers/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/helpers/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15706 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/helpers/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    20612 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/helpers/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    24691 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/helpers/googlerpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13415 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/helpers/store.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13868 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/helpers/wrappers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble/api/meta/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/meta/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9492 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/meta/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2952 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/meta/helpers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble/api/middleware/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble/api/middleware/apachethrift/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/apachethrift/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/apachethrift/screening.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble/api/middleware/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3730 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/database/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble/api/middleware/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      454 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/file/temp.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble/api/middleware/googlerpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/googlerpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/googlerpc/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/googlerpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/googlerpc/metadata.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3703 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.907108 pibble-0.5.3/pibble/api/middleware/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/webservice/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.907108 pibble-0.5.3/pibble/api/middleware/webservice/authentication/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/webservice/authentication/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/webservice/authentication/basic.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/webservice/authentication/bearer.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13472 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/webservice/authentication/digest.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/webservice/authentication/header.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    17704 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/webservice/authentication/oauth.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3256 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/webservice/limit.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/middleware/webservice/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.907108 pibble-0.5.3/pibble/api/protocol/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/protocol/__init__.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19486 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/protocol/apachethrift.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.907108 pibble-0.5.3/pibble/api/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2451 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2080 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.907108 pibble-0.5.3/pibble/api/server/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15640 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5453 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.907108 pibble-0.5.3/pibble/api/server/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2296 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7311 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/awslambda.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    39095 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.907108 pibble-0.5.3/pibble/api/server/webservice/drivers/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/drivers/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1489 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/drivers/driver_cherrypy.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2194 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/drivers/driver_gunicorn.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1078 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/drivers/driver_werkzeug.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15947 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/handler.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3164 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/jsonapi.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      969 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.907108 pibble-0.5.3/pibble/api/server/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4150 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6457 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    12004 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16962 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/soap.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.907108 pibble-0.5.3/pibble/api/server/webservice/template/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9717 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/template/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9201 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/template/extensions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9770 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/api/server/webservice/template/loader.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.907108 pibble-0.5.3/pibble/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7797 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/database/dedupe.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10529 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/database/engine.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/database/exceptions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    26274 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/database/orm.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/database/util.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.907108 pibble-0.5.3/pibble/ext/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.907108 pibble-0.5.3/pibble/ext/cms/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/cms/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.907108 pibble-0.5.3/pibble/ext/cms/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/cms/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/cms/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/cms/database/interface.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/cms/database/menu.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/cms/database/view.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1366 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/cms/middleware.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.907108 pibble-0.5.3/pibble/ext/cms/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/cms/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6660 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/cms/server/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3012 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/cms/server/extension.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/ext/dam/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/dam/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/ext/dam/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/dam/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/dam/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/dam/database/files.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/ext/dam/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/dam/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/dam/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/ext/rest/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/rest/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/ext/rest/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/rest/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/rest/database/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/ext/rest/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/rest/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15662 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/rest/server/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7244 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/rest/server/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/ext/session/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/session/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/ext/session/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/session/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/session/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/session/database/session.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/ext/session/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/session/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5087 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/session/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/ext/user/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/user/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/ext/user/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/user/client/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      985 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/user/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/ext/user/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/user/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/user/database/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/user/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/user/database/notification.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/user/database/permission.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/user/database/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/ext/user/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/user/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    24935 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/ext/user/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/hooks/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/hooks/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6037 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/hooks/aws.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/media/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/media/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10388 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/media/thumbnail.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/resources/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/resources/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10655 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/resources/retriever.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/scripts/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/scripts/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1909 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/scripts/importcheck.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1726 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/scripts/templatefiles.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/util/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/util/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     8357 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/util/encryption.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16171 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/util/files.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    32821 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/util/helpers.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/util/imaging.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6330 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/util/log.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1701 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/util/numeric.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    27348 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/util/strings.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.911108 pibble-0.5.3/pibble/web/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/web/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3227 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble/web/scraper.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-05 02:51:02.903108 pibble-0.5.3/pibble.egg-info/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble.egg-info/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5627 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble.egg-info/SOURCES.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble.egg-info/dependency_links.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble.egg-info/entry_points.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1936 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble.egg-info/requires.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-05-05 02:51:02.000000 pibble-0.5.3/pibble.egg-info/top_level.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-05-05 02:51:02.911108 pibble-0.5.3/setup.cfg
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-05 02:51:02.000000 pibble-0.5.3/setup.py
```

### Comparing `pibble-0.5.2/PKG-INFO` & `pibble-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.5.2
+Version: 0.5.3
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
```

### Comparing `pibble-0.5.2/README.md` & `pibble-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/__main__.py` & `pibble-0.5.3/pibble/__main__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/base.py` & `pibble-0.5.3/pibble/api/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/apachethrift/__init__.py` & `pibble-0.5.3/pibble/api/client/apachethrift/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/apachethrift/wrapper.py` & `pibble-0.5.3/pibble/api/client/apachethrift/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/base.py` & `pibble-0.5.3/pibble/api/client/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/file/base.py` & `pibble-0.5.3/pibble/api/client/file/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/file/ftp.py` & `pibble-0.5.3/pibble/api/client/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/file/hdfs.py` & `pibble-0.5.3/pibble/api/client/file/hdfs.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/file/local.py` & `pibble-0.5.3/pibble/api/client/file/local.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/file/sftp.py` & `pibble-0.5.3/pibble/api/client/file/sftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/googlerpc.py` & `pibble-0.5.3/pibble/api/client/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/webservice/apachethrift.py` & `pibble-0.5.3/pibble/api/client/webservice/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/webservice/base.py` & `pibble-0.5.3/pibble/api/client/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/webservice/jsonapi.py` & `pibble-0.5.3/pibble/api/client/webservice/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/webservice/rpc/base.py` & `pibble-0.5.3/pibble/api/client/webservice/rpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/webservice/rpc/jsonrpc.py` & `pibble-0.5.3/pibble/api/client/webservice/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/webservice/rpc/xmlrpc.py` & `pibble-0.5.3/pibble/api/client/webservice/rpc/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/webservice/soap.py` & `pibble-0.5.3/pibble/api/client/webservice/soap.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/webservice/wrapper.py` & `pibble-0.5.3/pibble/api/client/webservice/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/client/wrapper.py` & `pibble-0.5.3/pibble/api/client/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/configuration.py` & `pibble-0.5.3/pibble/api/configuration.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/exceptions.py` & `pibble-0.5.3/pibble/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/helpers/apachethrift.py` & `pibble-0.5.3/pibble/api/helpers/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/helpers/authentication.py` & `pibble-0.5.3/pibble/api/helpers/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/helpers/googlerpc.py` & `pibble-0.5.3/pibble/api/helpers/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/helpers/store.py` & `pibble-0.5.3/pibble/api/helpers/store.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/helpers/wrappers.py` & `pibble-0.5.3/pibble/api/helpers/wrappers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/meta/base.py` & `pibble-0.5.3/pibble/api/meta/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/meta/helpers.py` & `pibble-0.5.3/pibble/api/meta/helpers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/apachethrift/base.py` & `pibble-0.5.3/pibble/api/middleware/apachethrift/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/apachethrift/screening.py` & `pibble-0.5.3/pibble/api/middleware/apachethrift/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/database/orm.py` & `pibble-0.5.3/pibble/api/middleware/database/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/googlerpc/authentication.py` & `pibble-0.5.3/pibble/api/middleware/googlerpc/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/googlerpc/base.py` & `pibble-0.5.3/pibble/api/middleware/googlerpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/googlerpc/metadata.py` & `pibble-0.5.3/pibble/api/middleware/googlerpc/metadata.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/screening.py` & `pibble-0.5.3/pibble/api/middleware/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/webservice/authentication/basic.py` & `pibble-0.5.3/pibble/api/middleware/webservice/authentication/basic.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/webservice/authentication/bearer.py` & `pibble-0.5.3/pibble/api/middleware/webservice/authentication/bearer.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/webservice/authentication/digest.py` & `pibble-0.5.3/pibble/api/middleware/webservice/authentication/digest.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/webservice/authentication/header.py` & `pibble-0.5.3/pibble/api/middleware/webservice/authentication/header.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/webservice/authentication/oauth.py` & `pibble-0.5.3/pibble/api/middleware/webservice/authentication/oauth.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/webservice/base.py` & `pibble-0.5.3/pibble/api/middleware/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/webservice/limit.py` & `pibble-0.5.3/pibble/api/middleware/webservice/limit.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/middleware/webservice/screening.py` & `pibble-0.5.3/pibble/api/middleware/webservice/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/protocol/apachethrift.py` & `pibble-0.5.3/pibble/api/protocol/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/apachethrift.py` & `pibble-0.5.3/pibble/api/server/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/base.py` & `pibble-0.5.3/pibble/api/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/file/ftp.py` & `pibble-0.5.3/pibble/api/server/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/file/sftp.py` & `pibble-0.5.3/pibble/api/server/file/sftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/googlerpc.py` & `pibble-0.5.3/pibble/api/server/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/apachethrift.py` & `pibble-0.5.3/pibble/api/server/webservice/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/awslambda.py` & `pibble-0.5.3/pibble/api/server/webservice/awslambda.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/base.py` & `pibble-0.5.3/pibble/api/server/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/drivers/driver_cherrypy.py` & `pibble-0.5.3/pibble/api/server/webservice/drivers/driver_cherrypy.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/drivers/driver_gunicorn.py` & `pibble-0.5.3/pibble/api/server/webservice/drivers/driver_gunicorn.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/drivers/driver_werkzeug.py` & `pibble-0.5.3/pibble/api/server/webservice/drivers/driver_werkzeug.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/handler.py` & `pibble-0.5.3/pibble/api/server/webservice/handler.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/jsonapi.py` & `pibble-0.5.3/pibble/api/server/webservice/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/orm.py` & `pibble-0.5.3/pibble/api/server/webservice/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/rpc/base.py` & `pibble-0.5.3/pibble/api/server/webservice/rpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/rpc/jsonrpc.py` & `pibble-0.5.3/pibble/api/server/webservice/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/rpc/xmlrpc.py` & `pibble-0.5.3/pibble/api/server/webservice/rpc/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/soap.py` & `pibble-0.5.3/pibble/api/server/webservice/soap.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/template/__init__.py` & `pibble-0.5.3/pibble/api/server/webservice/template/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/template/extensions.py` & `pibble-0.5.3/pibble/api/server/webservice/template/extensions.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/api/server/webservice/template/loader.py` & `pibble-0.5.3/pibble/api/server/webservice/template/loader.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/database/dedupe.py` & `pibble-0.5.3/pibble/database/dedupe.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/database/engine.py` & `pibble-0.5.3/pibble/database/engine.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/database/orm.py` & `pibble-0.5.3/pibble/database/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/database/util.py` & `pibble-0.5.3/pibble/database/util.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/cms/database/__init__.py` & `pibble-0.5.3/pibble/ext/cms/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/cms/database/interface.py` & `pibble-0.5.3/pibble/ext/cms/database/interface.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/cms/database/menu.py` & `pibble-0.5.3/pibble/ext/cms/database/menu.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/cms/database/view.py` & `pibble-0.5.3/pibble/ext/cms/database/view.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/cms/middleware.py` & `pibble-0.5.3/pibble/ext/cms/middleware.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/cms/server/base.py` & `pibble-0.5.3/pibble/ext/cms/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/cms/server/extension.py` & `pibble-0.5.3/pibble/ext/cms/server/extension.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/dam/database/files.py` & `pibble-0.5.3/pibble/ext/dam/database/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/rest/server/base.py` & `pibble-0.5.3/pibble/ext/rest/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/rest/server/user.py` & `pibble-0.5.3/pibble/ext/rest/server/user.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/session/database/session.py` & `pibble-0.5.3/pibble/ext/session/database/session.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/session/server/base.py` & `pibble-0.5.3/pibble/ext/session/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/user/client/base.py` & `pibble-0.5.3/pibble/ext/user/client/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/user/database/__init__.py` & `pibble-0.5.3/pibble/ext/user/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/user/database/authentication.py` & `pibble-0.5.3/pibble/ext/user/database/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/user/database/notification.py` & `pibble-0.5.3/pibble/ext/user/database/notification.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/user/database/permission.py` & `pibble-0.5.3/pibble/ext/user/database/permission.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/user/database/user.py` & `pibble-0.5.3/pibble/ext/user/database/user.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/ext/user/server/base.py` & `pibble-0.5.3/pibble/ext/user/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/hooks/aws.py` & `pibble-0.5.3/pibble/hooks/aws.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/media/thumbnail.py` & `pibble-0.5.3/pibble/media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/resources/retriever.py` & `pibble-0.5.3/pibble/resources/retriever.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/scripts/importcheck.py` & `pibble-0.5.3/pibble/scripts/importcheck.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/scripts/templatefiles.py` & `pibble-0.5.3/pibble/scripts/templatefiles.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/setup.py` & `pibble-0.5.3/pibble/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
 version_minor = "5"
-version_patch = "2"
+version_patch = "3"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
```

### Comparing `pibble-0.5.2/pibble/util/encryption.py` & `pibble-0.5.3/pibble/util/encryption.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/util/files.py` & `pibble-0.5.3/pibble/util/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/util/helpers.py` & `pibble-0.5.3/pibble/util/helpers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/util/imaging.py` & `pibble-0.5.3/pibble/util/imaging.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/util/log.py` & `pibble-0.5.3/pibble/util/log.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/util/numeric.py` & `pibble-0.5.3/pibble/util/numeric.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble/util/strings.py` & `pibble-0.5.3/pibble/util/strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,17 +200,22 @@
                 raise ValueError(
                     "Can't parse {0}: {1}({2})".format(parameter, type(ex).__name__, ex)
                 )
         return parameter
 
     @classmethod
     def serialize(cls, parameter: Any, **kwargs: Any) -> str:
+        # Strict pass
         for typename in cls.SERIALIZE_FORMATS:
             if type(parameter) is typename:
                 return cls.SERIALIZE_FORMATS[typename](parameter, **kwargs)  # type: ignore
+        # Lenient pass
+        for typename in cls.SERIALIZE_FORMATS:
+            if isinstance(parameter, typename):
+                return cls.SERIALIZE_FORMATS[typename](parameter, **kwargs)  # type: ignore
         return str(parameter)
 
 
 class RandomWordGenerator(object):
     """
     A simple class to generate a random word. Reads from /usr/share/dict/words.
```

### Comparing `pibble-0.5.2/pibble/web/scraper.py` & `pibble-0.5.3/pibble/web/scraper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble.egg-info/PKG-INFO` & `pibble-0.5.3/pibble.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.5.2
+Version: 0.5.3
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
```

### Comparing `pibble-0.5.2/pibble.egg-info/SOURCES.txt` & `pibble-0.5.3/pibble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/pibble.egg-info/requires.txt` & `pibble-0.5.3/pibble.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pibble-0.5.2/setup.py` & `pibble-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
 version_minor = "5"
-version_patch = "2"
+version_patch = "3"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
```

