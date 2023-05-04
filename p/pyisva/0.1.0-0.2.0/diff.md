# Comparing `tmp/pyisva-0.1.0.tar.gz` & `tmp/pyisva-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyisva-0.1.0.tar", last modified: Thu Mar  9 01:55:57 2023, max compression
+gzip compressed data, was "pyisva-0.2.0.tar", last modified: Thu May  4 22:03:20 2023, max compression
```

## Comparing `pyisva-0.1.0.tar` & `pyisva-0.2.0.tar`

### file list

```diff
@@ -1,105 +1,132 @@
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-03-09 01:55:57.033030 pyisva-0.1.0/
--rw-rw-r--   0 lowkey    (1000) lowkey    (1000)      510 2020-05-23 07:18:14.000000 pyisva-0.1.0/AUTHORS.md
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1048 2023-03-02 22:49:47.000000 pyisva-0.1.0/LICENSE.txt
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)      306 2023-03-09 01:55:57.033030 pyisva-0.1.0/PKG-INFO
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1816 2023-03-02 22:49:47.000000 pyisva-0.1.0/README.md
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-03-09 01:55:57.004030 pyisva-0.1.0/pyisva/
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)       50 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/__init__.py
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-03-09 01:55:57.007030 pyisva-0.1.0/pyisva/core/
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)        0 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/__init__.py
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-03-09 01:55:57.014030 pyisva-0.1.0/pyisva/core/access/
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)        0 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/__init__.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    13926 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/accesscontrol.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2506 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/advancedconfig.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    31758 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/apiprotection.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5423 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/attributes.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    20793 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/authentication.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    17753 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/fido2config.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3253 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/fido2registrations.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6448 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/mappingrules.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5480 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/mmfaconfig.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6417 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/pushnotification.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5992 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/riskprofiles.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4210 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/runtimeparameters.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     8935 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/scimconfig.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    28001 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/serverconnections.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     8682 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/templatefiles.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     8918 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/access/userregistry.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     7246 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/accesscontrol.py
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-03-09 01:55:57.015030 pyisva-0.1.0/pyisva/core/analysis/
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)        0 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/analysis/__init__.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2855 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/analysis/applicationlog.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3672 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/analysisdiagnostics.py
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-03-09 01:55:57.017030 pyisva-0.1.0/pyisva/core/federation/
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)        0 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/federation/__init__.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3961 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/federation/accesspolicy.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5199 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/federation/attributesources.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    71415 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/federation/federations.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    14526 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/federation/pointofcontact.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    14095 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/federation/securitytokenservice.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4152 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/federationsettings.py
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-03-09 01:55:57.026030 pyisva-0.1.0/pyisva/core/system/
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)        0 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/__init__.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    10518 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/adminsettings.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3699 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/advancedtuning.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1463 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/clicommands.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    14344 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/cluster.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5509 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/configuration.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1654 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/datetime.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2339 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/dns.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1404 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/docker.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2764 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/filedownloads.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2561 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/firststeps.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2989 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/fixpacks.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4836 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/hostsfile.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    11457 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/interfaces.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3497 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/licensing.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    10473 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/managementauthorization.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6059 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/restartshutdown.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3025 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/runtimedb.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1001 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/snapshot.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    12036 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/sslcertificates.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4926 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/staticroutes.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     9736 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/system/sysaccount.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6933 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/systemsettings.py
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-03-09 01:55:57.030030 pyisva-0.1.0/pyisva/core/web/
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)        0 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/__init__.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)      904 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/api_access_control.py
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-03-09 01:55:57.032030 pyisva-0.1.0/pyisva/core/web/apiac/
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)        0 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/apiac/__init__.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    12533 2023-03-08 22:03:08.000000 pyisva-0.1.0/pyisva/core/web/apiac/authorization_server.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6657 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/apiac/cors.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5633 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/apiac/document_root.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3971 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/apiac/policies.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    27662 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/apiac/resources.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1355 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/apiac/utilities.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4550 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/clientcertmapping.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4662 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/dscadmin.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3925 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/fsso.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4326 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/httptransform.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4620 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/junctionmapping.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     8126 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/kerberos.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4585 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/passwordstrength.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1549 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/policyadmin.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3691 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/ratelimit.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    46839 2023-03-08 21:57:03.000000 pyisva-0.1.0/pyisva/core/web/reverseproxy.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3567 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/rsa.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    19491 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/runtimecomponent.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4053 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/urlmapping.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4448 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/web/usermapping.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5462 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/core/websettings.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6542 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/factory.py
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-03-09 01:55:57.033030 pyisva-0.1.0/pyisva/util/
--rwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/util/__init__.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1201 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/util/model.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5711 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/util/policies.py
--rwxr-xr-x   0 lowkey    (1000) lowkey    (1000)     6437 2023-03-02 22:49:47.000000 pyisva-0.1.0/pyisva/util/restclient.py
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-03-09 01:55:57.005030 pyisva-0.1.0/pyisva.egg-info/
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)      306 2023-03-09 01:55:56.000000 pyisva-0.1.0/pyisva.egg-info/PKG-INFO
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2948 2023-03-09 01:55:56.000000 pyisva-0.1.0/pyisva.egg-info/SOURCES.txt
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)        1 2023-03-09 01:55:56.000000 pyisva-0.1.0/pyisva.egg-info/dependency_links.txt
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)        1 2023-03-09 01:55:56.000000 pyisva-0.1.0/pyisva.egg-info/not-zip-safe
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)       17 2023-03-09 01:55:56.000000 pyisva-0.1.0/pyisva.egg-info/requires.txt
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)        7 2023-03-09 01:55:56.000000 pyisva-0.1.0/pyisva.egg-info/top_level.txt
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)       38 2023-03-09 01:55:57.034030 pyisva-0.1.0/setup.cfg
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)      459 2023-03-02 22:49:47.000000 pyisva-0.1.0/setup.py
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.558504 pyisva-0.2.0/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      422 2023-04-03 07:30:27.000000 pyisva-0.2.0/.deploy.sh
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.517504 pyisva-0.2.0/.github/
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.522504 pyisva-0.2.0/.github/workflows/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      899 2023-05-04 21:56:07.000000 pyisva-0.2.0/.github/workflows/main.yaml
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)       85 2023-05-04 21:47:22.000000 pyisva-0.2.0/.gitignore
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.522504 pyisva-0.2.0/.tests/
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.517504 pyisva-0.2.0/.tests/core/
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.522504 pyisva-0.2.0/.tests/core/sys/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      252 2023-04-03 07:30:27.000000 pyisva-0.2.0/.tests/core/sys/versions
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      929 2023-04-03 07:30:27.000000 pyisva-0.2.0/.tests/unit_test.sh
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      470 2023-05-04 21:47:22.000000 pyisva-0.2.0/.travis.yml
+-rw-rw-r--   0 lowkey    (1000) lowkey    (1000)      510 2020-05-23 07:18:14.000000 pyisva-0.2.0/AUTHORS.md
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     7854 2023-04-03 07:30:27.000000 pyisva-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1048 2023-04-03 07:30:27.000000 pyisva-0.2.0/LICENSE.txt
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2105 2023-05-04 22:03:20.558504 pyisva-0.2.0/PKG-INFO
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1791 2023-05-04 22:00:55.000000 pyisva-0.2.0/README.md
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)       53 2023-05-04 21:49:17.000000 pyisva-0.2.0/dev-requirements.txt
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.525504 pyisva-0.2.0/docs/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      813 2023-04-03 07:30:27.000000 pyisva-0.2.0/docs/Makefile
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2230 2023-05-04 21:47:22.000000 pyisva-0.2.0/docs/accesscontrol.rst
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      451 2023-05-04 21:47:22.000000 pyisva-0.2.0/docs/analysisdiagnostics.rst
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2156 2023-05-04 21:47:22.000000 pyisva-0.2.0/docs/conf.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1316 2023-05-04 21:47:22.000000 pyisva-0.2.0/docs/factory.rst
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1080 2023-05-04 21:47:22.000000 pyisva-0.2.0/docs/federation.rst
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1460 2023-05-04 21:47:22.000000 pyisva-0.2.0/docs/index.rst
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      794 2023-04-03 07:30:27.000000 pyisva-0.2.0/docs/make.bat
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2573 2023-05-04 21:47:22.000000 pyisva-0.2.0/docs/systemsettings.rst
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2822 2023-05-04 21:47:22.000000 pyisva-0.2.0/docs/websettings.rst
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.525504 pyisva-0.2.0/pyisva/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)       50 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/__init__.py
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.529504 pyisva-0.2.0/pyisva/core/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)        0 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/__init__.py
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.535504 pyisva-0.2.0/pyisva/core/access/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)        0 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/access/__init__.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    17626 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/accesscontrol.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2559 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/advancedconfig.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    29687 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/apiprotection.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    11057 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/attributes.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    21256 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/authentication.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    37480 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/fido2config.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3663 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/fido2registrations.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6497 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/mappingrules.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5522 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/mmfaconfig.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6252 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/pip.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    11210 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/pushnotification.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6214 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/riskprofiles.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4586 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/runtimeparameters.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     9557 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/scimconfig.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    28044 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/serverconnections.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     8689 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/templatefiles.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     8945 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/access/userregistry.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     7629 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/accesscontrol.py
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.536504 pyisva-0.2.0/pyisva/core/analysis/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)        0 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/analysis/__init__.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2855 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/analysis/applicationlog.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3672 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/analysisdiagnostics.py
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.539504 pyisva-0.2.0/pyisva/core/federation/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)        0 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/federation/__init__.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4537 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/federation/accesspolicy.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6191 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/federation/aliasservice.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5202 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/federation/attributesources.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    92837 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/federation/federations.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    15254 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/federation/pointofcontact.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    21781 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/federation/securitytokenservice.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4493 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/federationsettings.py
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.547504 pyisva-0.2.0/pyisva/core/system/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)        0 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/system/__init__.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    10518 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/system/adminsettings.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3699 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/system/advancedtuning.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1463 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/system/clicommands.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    14344 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/system/cluster.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5509 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/system/configuration.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1654 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/system/datetime.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2339 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/system/dns.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1404 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/system/docker.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3423 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/system/extensions.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2764 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/system/filedownloads.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2561 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/system/firststeps.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2989 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/system/fixpacks.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4836 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/system/hostsfile.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    11457 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/system/interfaces.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3497 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/system/licensing.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    10473 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/system/managementauthorization.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6059 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/system/restartshutdown.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3025 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/system/runtimedb.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1001 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/system/snapshot.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    12036 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/system/sslcertificates.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4926 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/system/staticroutes.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     9732 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/system/sysaccount.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     7115 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/systemsettings.py
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.553504 pyisva-0.2.0/pyisva/core/web/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)        0 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/web/__init__.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      927 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/web/api_access_control.py
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.556504 pyisva-0.2.0/pyisva/core/web/apiac/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)        0 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/web/apiac/__init__.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    12534 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/web/apiac/authorization_server.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6657 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/web/apiac/cors.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5633 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/web/apiac/document_root.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3971 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/web/apiac/policies.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    27749 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/web/apiac/resource_server.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1355 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/web/apiac/utilities.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4550 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/web/clientcertmapping.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4662 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/web/dscadmin.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3925 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/web/fsso.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4326 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/web/httptransform.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4620 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/web/junctionmapping.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     8126 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/web/kerberos.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4585 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/web/passwordstrength.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1549 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/web/policyadmin.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3691 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/web/ratelimit.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    46854 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/web/reverseproxy.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3771 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/web/rsa.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    19491 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/web/runtimecomponent.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4053 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/web/urlmapping.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4448 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/core/web/usermapping.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5462 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/core/websettings.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6543 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/factory.py
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.558504 pyisva-0.2.0/pyisva/util/
+-rwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/util/__init__.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1246 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/util/model.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5711 2023-04-03 07:30:27.000000 pyisva-0.2.0/pyisva/util/policies.py
+-rwxr-xr-x   0 lowkey    (1000) lowkey    (1000)     7017 2023-05-04 21:47:22.000000 pyisva-0.2.0/pyisva/util/restclient.py
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 22:03:20.527504 pyisva-0.2.0/pyisva.egg-info/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2105 2023-05-04 22:03:19.000000 pyisva-0.2.0/pyisva.egg-info/PKG-INFO
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3386 2023-05-04 22:03:20.000000 pyisva-0.2.0/pyisva.egg-info/SOURCES.txt
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)        1 2023-05-04 22:03:19.000000 pyisva-0.2.0/pyisva.egg-info/dependency_links.txt
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)        1 2023-05-04 22:03:19.000000 pyisva-0.2.0/pyisva.egg-info/not-zip-safe
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)       17 2023-05-04 22:03:19.000000 pyisva-0.2.0/pyisva.egg-info/requires.txt
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)        7 2023-05-04 22:03:19.000000 pyisva-0.2.0/pyisva.egg-info/top_level.txt
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)       38 2023-05-04 22:03:20.558504 pyisva-0.2.0/setup.cfg
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      671 2023-05-04 22:03:17.000000 pyisva-0.2.0/setup.py
```

### Comparing `pyisva-0.1.0/LICENSE.txt` & `pyisva-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/README.md` & `pyisva-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # PyISAM
 
 PyISAM is a Python library that wraps the IBM Security Verify Access RESTful Web services to provide a
 quick and easy way to construct configuration scripts for appliances.
 
 **Supported Versions**
 
+- IBM Security Verify Access 10.0.6.0
 - IBM Security Verify Access 10.0.5.0
 - IBM Security Verify Access 10.0.4.0
 - IBM Security Verify Access 10.0.3.1
 - IBM Security Verify Access 10.0.3.0
 - IBM Security Verify Access 10.0.2.0
 - IBM Security Verify Access 10.0.1.0
 - IBM Security Verify Access 10.0.0.0
@@ -25,19 +26,18 @@
 For Linux/macOS: if you clone the library to `~/repos/pyisva`, add this to `~/.profile`:
 ```sh
 # add pyisva library to Python's search path
 export PYTHONPATH="${PYTHONPATH}:${HOME}/repos/pyisva"
 ```
 
 ## From IBM Security Verify Accesss 10.0.0.0 onwards:
-Module has been build into a package that can be installed using pip
+Module has been build into a package Currently hosted on PyPi that can be installed using pip:
 
-Currently hosted on IBM Artifactory, users will need W3Id credentials to download and install
 ```sh
-pip install pyisva --extra-index https://{username}:{password}@eu.artifactory.swg-devops.com/artifactory/api/pypi/sec-iam-isam-devops-team-pypi-local/simple
+pip install pyisva
 ```
 
 ## Usage
 
 ```python
 >>> import pyisva
 >>> factory = pyisva.Factory("https://isam.mmfa.ibm.com", "admin", "Passw0rd")
@@ -46,7 +46,10 @@
 >>> if resp.success:
 ...     print("Successfully restarted the default instance.")
 ... else:
 ...     print("Failed to restart the default instance. status_code: %s, data: %s" % (resp.status_code, resp.data))
 ...
 Successfully restarted the default instance.
 ```
+
+## Documentation
+Documentation for using this library can be found on [pyisva GitHub pages](https://lachlan-ibm.github.io/pyisva/index.html).
```

### Comparing `pyisva-0.1.0/pyisva/core/access/accesscontrol.py` & `pyisva-0.2.0/pyisva/core/access/accesscontrol.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,107 +18,110 @@
 
 class AccessControl(object):
 
     def __init__(self, base_url, username, password):
         super(AccessControl, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
-    def create_policy(
-            self, name=None, description=None, dialect="urn:oasis:names:tc:xacml:2.0:policy:schema:os", 
-            policy=None, attributes_required=False):
+    def create_policy(self, name=None, description=None, dialect="urn:oasis:names:tc:xacml:2.0:policy:schema:os", 
+                    policy=None, attributes_required=False):
         '''
         Create an AAC Access Policy. 
 
         Args:
             name (:obj:`str`): Name of policy to be created.
             description (:obj:`str`, optional): Description of policy to be created
             dialect (:obj:`str`, optional): Format of policy XML. Only "urn:oasis:names:tc:xacml:2.0:policy:schema:os" is supported
             policy (:obj:`str`, optional): XML of policy steps.
             attributes_required (:obj:`list` of :obj:`str`, optional): Additional attribute mappings used by the policy
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
+
+            If the request is successful the id of the created policy can be access from the 
+            response.id_from_location attribute.
 
-            If the request is successful the id of the created policy can be acess from the 
-            response.id_from_location attribute
         '''
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value_string("description", description)
         data.add_value_string("dialect", dialect)
         data.add_value_string("policy", policy)
-        data.add_value("attributesrequired", attributes_required)
-        data.add_value("predefined", False)
+        data.add_value_boolean("attributesRequired", attributes_required)
+        data.add_value_boolean("predefined", False)
 
         response = self.client.post_json(POLICIES, data.data)
         response.success = response.status_code == 201
 
         return response
 
+
     def delete_policy(self, id=None):
         '''
         Delete an AAC Access Policy.
 
         Args:
             id (:obj:`str`): Policy id to be removed.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "%s/%s" % (POLICIES, id)
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
         return response
 
+
     def list_policies(self, sort_by=None, filter=None):
         '''
         List all of the configured AAC Access Policies.
 
         Args:
             sort_by (:obj:`str`, optional): Optional sorting of returned policies
             filter (:obj:`str`, optional): Optional filter for returned policies
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the policies are returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         '''
         parameters = DataObject()
         parameters.add_value_string("sortBy", sort_by)
         parameters.add_value_string("filter", filter)
 
         response = self.client.get_json(POLICIES, parameters.data)
         response.success = response.status_code == 200
 
         return response
 
+
     def authenticate_security_access_manager(self, username=None, password=None, domain=None):
         '''
-        Authenticate to the Verify Access polic server. This is required before an administrator can modify 
+        Authenticate to the Verify Access policy server. This is required before an administrator can modify 
         mapping from policies to resources.
 
         Args:
             username (:obj:`str`): Username used to authenticate to the policy server.
             password (:obj:`str`): Password used to authenticate to the policy server.
             domain (:obj:`str`): Security domain to authenticate to.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         data = DataObject()
         data.add_value_string("username", username)
         data.add_value_string("password", password)
         data.add_value_string("domain", domain)
         data.add_value_string("command", "setCredential")
@@ -128,114 +131,120 @@
 
         return response
 
     def configure_resource(
             self, server=None, resource_uri=None,
             policy_combining_algorithm=None, policies=None):
         '''
-        Create a new resource in the polic server wheich can be attached to an authentication policy.
+        Create a new resource in the policy server which can be attached to an authentication policy.
 
         Args:
-            server (:obj:`str`): Name of WebSEAL instance in the policy server where resource will be created
-            resource_uri (:obj:`str`): URI of resource to be created
-            policy_combining_algorithm (:obj:`str`): Algorithm to use: "denyOverrides" or "permitOverrides"
-            policies (:obj:`list` of :obj:`str`): List of policies, policy sets or API protection clients
+            server (:obj:`str`): Name of WebSEAL instance in the policy server where resource will be created.
+            resource_uri (:obj:`str`): URI of resource to be created.
+            policy_combining_algorithm (:obj:`str`): Algorithm to use: "denyOverrides" or "permitOverrides".
+            policies (:obj:`list` of :obj:`str`): List of policies, policy sets or API protection clients.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
+
+            If the request is successful the id of the created policy can be accessed from the
+            response.id_from_location attribute.
 
         '''
         data = DataObject()
         data.add_value_string("server", server)
         data.add_value_string("resourceUri", resource_uri)
-        data.add_value_string(
-            "policyCombiningAlgorithm", policy_combining_algorithm)
+        data.add_value_string("policyCombiningAlgorithm", policy_combining_algorithm)
         data.add_value("policies", policies)
 
         response = self.client.post_json(POLICY_ATTACHMENTS, data.data)
         response.success = response.status_code == 201
 
         return response
 
+
     def remove_resource(self, id):
         '''
         Delete a resource from the policy server.
 
         Args:
-            id (:obj:`str`): THe id of the resource to be removed
+            id (:obj:`str`): The id of the resource to be removed.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "%s/%s" % (POLICY_ATTACHMENTS, id)
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
         return response
 
+
     def list_resources(self, sort_by=None, filter=None):
         '''
         Return the list of configured resources.
 
         Args:
-            sort_by (:obj:`str`, optional): optionally specify the attribute to sort the returned list by.
-            filter (:obj:`str`): optionally specify whether the returned list shouldb e filtered based on an attribute.
+            sort_by (:obj:`str`, optional): Optionally specify the attribute to sort the returned list by.
+            filter (:obj:`str`): Optionally specify whether the returned list shouldb e filtered based on an attribute.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         parameters = DataObject()
         parameters.add_value_string("sortBy", sort_by)
         parameters.add_value_string("filter", filter)
 
         response = self.client.get_json(POLICY_ATTACHMENTS, parameters.data)
         response.success = response.status_code == 200
 
         return response
 
+
     def publish_policy_attachment(self, id):
         '''
         Publish the changes to the policy server. This will require a restart of the corresponding WebSEAL instance.
 
         Args:
-            id (:obj:`str`): The id of the resource to publish
+            id (:obj:`str`): The id of the resource to publish.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "%s/deployment/%s" % (POLICY_ATTACHMENTS, id)
 
         response = self.client.put_json(endpoint)
         response.success = response.status_code == 204
 
         return response
 
-    def publish_multiple_policy_attachments(self, *ids):
+
+    def publish_multiple_policy_attachments(self, ids=[]):
         '''
-        Publish the change sto the policy server for one or nore resources. This will require a restart of the
-        correspondign WebSEAL instance.
+        Publish the changes to the policy server for one or more resources. This will require a restart of the
+        corresponding WebSEAL instance.
 
         Args:
-            ids (:obj:`list` of :obj:`str`): List of resource ids to publish
+            ids (:obj:`list` of :obj:`str`): List of resource ids to publish.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         id_string = ""
         for id in ids:
 
             if len(id_string) > 0:
                 id_string += ", "
@@ -247,130 +256,208 @@
         endpoint = "%s/deployment" % POLICY_ATTACHMENTS
 
         response = self.client.put_json(endpoint, data.data)
         response.success = response.status_code == 204
 
         return response
 
+
     def list_obligations(self, sort_by=None, filter=None):
         '''
         Return the list of configured obligations for AAC.
 
         Args:
-            sort_by (:obj:`str`, optional): Optional sorting of returned policies
-            filter (:obj:`str`, optional): Optional filter for returned policies
+            sort_by (:obj:`str`, optional): Optional sorting of returned policies.
+            filter (:obj:`str`, optional): Optional filter for returned policies.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the obligations are returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         '''
         parameters = DataObject()
         parameters.add_value_string("sortBy", sort_by)
         parameters.add_value_string("filter", filter)
 
         response = self.client.get_json(OBLIGATIONS, parameters.data)
         response.success = response.status_code == 200
 
         return response
 
-    def create_obligation(
-            self, name=None, predefined=False, description=None, obligationURI=None,
-            type=None, parameters=None, typeId=None, properties=None):
+
+    def create_obligation(self, name=None, description=None, obligation_uri=None,
+                        type="Obligation", type_id="1", parameters=None, properties=None):
+        '''
+        Create a new obligation for use with RBA.
+
+        Args:
+            name (:obj:`str`): Name of obligation.
+            description (:obj:`str`, optional): Description of the obligation.
+            obligation_uri (:obj:`str`): URI of the obligation.
+            type (:obj:`str`): The obligation type, "Obligation".
+            type_id (:obj:`str`, optional): The obligation type id. If not provided, the value will be set to "1", which is the "Enforcement Point" type.
+            parameters (:obj:`list` of :obj:`str`, optional): List of parameters used by the obligation when making a decision.
+            properties (:obj:`list` of :obj:`str`, optional): Properties used by the obligation.
+
+        Returns:
+            :obj:`~requests.Response`: The response from verify access. 
+
+            Success can be checked by examining the response.success boolean attribute.
+
+            If the request is successful the id of the created obligation can be accessed from the 
+            response.id_from_location attribute.
+
+        '''
+        data = DataObject()
+        data.add_value_string("name", name)
+        data.add_value_string("description", description)
+        data.add_value_string("obligationURI", obligation_uri)
+        data.add_value_string("type", type)
+        data.add_value("parameters", parameters)
+        data.add_value_string("typeId", type_id)
+        data.add_value("properties", properties)
+
+        response = self.client.post_json(OBLIGATIONS, data.data)
+        response.success = response.status_code == 201
+
+        return response
+
+
+    def update_obligation(self, id, name=None, description=None, obligationURI=None,
+                        type="Obligation", parameters=None, properties=None):
         '''
-        Create a new obligation for use with RBA
+        Update an existing obligation for use with RBA
 
         Args:
+            id (:obj:`str`): The generated unique id of the obligation to update.
             name (:obj:`str`): Name of obligation.
-            predefined (`bool`, optional): Is the obligation defined out of the box. Should be False.
-            description (:obj:`str`, optional): Description of the obligation,
+            description (:obj:`str`, optional): Description of the obligation.
             obligationURI (:obj:`str`): URI of the obligation.
-            type (:obj:`str`): The obligation type, "Obligation"
+            type (:obj:`str`, optional): The obligation type, "Obligation".
             parameters (:obj:`list` of :obj:`str`, optional): List of parameters used by the obligation when making a decision.
-            typeId (:obj:`str`): The obligation type id to create obligation with.
             properties (:obj:`list` of :obj:`str`, optional): Properties used by the obligation.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the id of the created obligation can be acess from the 
-            response.id_from_location attribute
+            If the request is successful the id of the created obligation can be accessed from the 
+            response.id_from_location attribute.
 
         '''
         data = DataObject()
         data.add_value_string("name", name)
-        data.add_value("predefined", predefined)
         data.add_value_string("description", description)
         data.add_value_string("obligationURI", obligationURI)
         data.add_value_string("type", type)
         data.add_value("parameters", parameters)
         data.add_value_string("typeId", typeId)
         data.add_value("properties", properties)
 
         response = self.client.post_json(OBLIGATIONS, data.data)
         response.success = response.status_code == 201
 
         return response
 
+
     def delete_obligation(self, id):
         '''
         Delete an existing obligation from the policy server
 
         Args:
-            id (:obj:`str`): The id of the obligation to be removed
+            id (:obj:`str`): The id of the obligation to be removed.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "%s/%s" % (OBLIGATIONS, id)
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
         return response
 
 
 class AccessControl9030(AccessControl):
 
     def __init__(self, base_url, username, password):
         super(AccessControl9030, self).__init__(base_url, username, password)
 
-    def configure_resource(
-            self, server=None, resource_uri=None,
-            policy_combining_algorithm=None, policies=None,
-            type="reverse_proxy"):
+
+    def configure_resource(self, server=None, resource_uri=None, policy_combining_algorithm=None, 
+                        policies=None, type="reverse_proxy"):
         '''
-        Create a new resource in the polic server wheich can be attached to an authentication policy.
+        Create a new resource in the policy server which can be attached to an authentication policy.
 
         Args:
-            server (:obj:`str`): Name of WebSEAL instance in the policy server where resource will be created
-            resource_uri (:obj:`str`): URI of resource to be created
-            policy_combining_algorithm (:obj:`str`): Algorithm to use: "denyOverrides" or "permitOverrides"
-            policies (:obj:`list` of :obj:`str`): List of policies, policy sets or API protection clients
+            server (:obj:`str`): Name of WebSEAL instance in the policy server where resource will be created.
+            resource_uri (:obj:`str`): URI of resource to be created.
+            policy_combining_algorithm (:obj:`str`): Algorithm to use: "denyOverrides" or "permitOverrides".
+            policies (:obj:`list` of :obj:`str`): List of policies, policy sets or API protection clients.
             type (:obj:`str`, optional): Resource type to be created. Default is "reverse_proxy".
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         data = DataObject()
         data.add_value_string("server", server)
         data.add_value_string("resourceUri", resource_uri)
         data.add_value_string(
             "policyCombiningAlgorithm", policy_combining_algorithm)
         data.add_value("policies", policies)
         data.add_value_string("type", type)
 
         response = self.client.post_json(POLICY_ATTACHMENTS, data.data)
         response.success = response.status_code == 201
 
         return response
+
+
+class AccessControl10000(AccessControl9030):
+
+    def __init__(self, base_url, username, password):
+        super(AccessControl10000, self).__init__(base_url, username, password)
+
+
+    def configure_resource(self, server=None, resource_uri=None, policy_combining_algorithm=None, 
+                        policies=None, cache=None):
+        '''
+        Create a new resource in the policy server which can be attached to an authentication policy.
+
+        Args:
+            server (:obj:`str`): Name of WebSEAL instance in the policy server where resource will be created.
+            resource_uri (:obj:`str`): URI of resource to be created.
+            policy_combining_algorithm (:obj:`str`): Algorithm to use: "denyOverrides" or "permitOverrides".
+            policies (:obj:`list` of :obj:`str`): List of policies, policy sets or API protection clients.
+            cache (`int`, optional): 0 to disable the cache for this resource, -1 to cache the decision for 
+                                    the lifetime of the session or any number greater than 1 to set a 
+                                    specific timeout (in seconds) for the cached decision. If not specified 
+                                    a default of 0 will be used. 
+
+        Returns:
+            :obj:`~requests.Response`: The response from verify access. 
+
+            Success can be checked by examining the response.success boolean attribute.
+
+        '''
+        data = DataObject()
+        data.add_value_string("server", server)
+        data.add_value_string("resourceUri", resource_uri)
+        data.add_value_string(
+            "policyCombiningAlgorithm", policy_combining_algorithm)
+        data.add_value("policies", policies)
+        data.add_value("cache", cache)
+
+        response = self.client.post_json(POLICY_ATTACHMENTS, data.data)
+        response.success = response.status_code == 201
+
+        return response
```

### Comparing `pyisva-0.1.0/pyisva/core/access/advancedconfig.py` & `pyisva-0.2.0/pyisva/core/access/advancedconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,62 +15,63 @@
 
 class AdvancedConfig(object):
 
     def __init__(self, base_url, username, password):
         super(AdvancedConfig, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
-    def list(self, sort_by=None, count=None, start=None, filter=None):
+
+    def list_properties(self, sort_by=None, count=None, start=None, filter=None):
         '''
         Get a list of all the advanced configuration parameters
 
         Args:
             sort_by (:obj:`str`, optional): Attribute to sort results by.
             count (:obj:`str`, optional): Maximum number of results to fetch.
-            start (:obj:`str`, optional): Pagenation offset of returned results.
+            start (:obj:`str`, optional): Pagination offset of returned results.
             filter (:obj:`str`): Attribute to filter results by
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the obligations are returned as JSON and can be accessed from
+            If the request is successful the Advanced Configuration Properties are returned as JSON and can be accessed from
             the response.json attribute
 
         '''
         parameters = DataObject()
-        parameters.add_value_string("sortBy", sortBy)
+        parameters.add_value_string("sortBy", sort_by)
         parameters.add_value_string("count", count)
         parameters.add_value_string("start", start)
         parameters.add_value_string("filter", filter)
 
         response = self.client.get_json(OVERRIDE_CONFIGS, parameters.data)
         response.success = response.status_code == 200
 
         return response
 
-    def update(self, id, value=None, sensitive=False):
+
+    def update_property(self, id, value=None, sensitive=False):
         '''
         Update an AAC advanced configuration property.
 
         Args;
             id (:obj:`str`): The id of the property to be updated.
             value (:obj:`str`): The new value of the configuration property.
-            sensitive (bool): Flag to indicate if value shoul be obsfucatedfrom logs/audit records.
+            sensitive (bool): Flag to indicate if value should be obfuscated from logs/audit records.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
         '''
         data = DataObject()
         data.add_value_string("value", value)
-        data.add_value("sensitive", sensitive)
+        data.add_value_boolean("sensitive", sensitive)
 
         endpoint = "%s/%s" % (OVERRIDE_CONFIGS, id)
-
         response = self.client.put_json(endpoint, data.data)
         response.success = response.status_code == 204
 
-        return response
+        return response
```

### Comparing `pyisva-0.1.0/pyisva/core/access/apiprotection.py` & `pyisva-0.2.0/pyisva/core/access/apiprotection.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,56 +6,52 @@
 
 from pyisva.util.model import DataObject, Response
 from pyisva.util.restclient import RESTClient
 
 
 CLIENTS = "/iam/access/v8/clients"
 DEFINITIONS = "/iam/access/v8/definitions"
-MAPPING_RULES = "/iam/access/v8/mapping-rules"
 
 logger = logging.getLogger(__name__)
 
 
 class APIProtection(object):
 
     def __init__(self, base_url, username, password):
         super(APIProtection, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
-    
 
-    def create_client(
-            self, name=None, redirect_uri=None, company_name=None,
-            company_url=None, contact_person=None, contact_type=None,
-            email=None, phone=None, other_info=None, definition=None,
-            client_id=None, client_secret=None):
+    def create_client(self, name=None, redirect_uri=None, company_name=None, company_url=None, 
+                    contact_person=None, contact_type=None, email=None, phone=None, other_info=None, 
+                    definition=None, client_id=None, client_secret=None):
         '''
-        Create an OIDC api protection client
+        Create an OIDC api protection client.
 
         Args:
             name (:obj:`str`): Name of the client.
             redirect_uri (:obj:`str`, optional): URL which client should redirect to.
             company_name (:obj:`str`, optional): Company to associate client with.
             company_url (:obj:`str`, optional): URL to associate client with.
             contact_person (:obj:`str`, optional): Person who is responsible for API client.
             contact_type (:obj:`str`, optional): Position of contact person.
             email (:obj:`str`, optional): Contact email address for client.
             phone (:obj:`str`, optional): Contact phone number for client.
-            other_info (:obj:`str`, optional): Other contact details assocaited with client.
-            definition (:obj:`str`): The id of the API protection definition to use
+            other_info (:obj:`str`, optional): Other contact details associated with client.
+            definition (:obj:`str`): The id of the API protection definition to use.
             client_id (:obj:`str`): The id of the client.
             client_secret (:obj:`str`, optional): The client secret to use. If not specified then a public client is created.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the id of the created obligation can be acess from the 
-            response.id_from_location attribute
+            If the request is successful the id of the created API client can be accessed from the 
+            response.id_from_location attribute.
 
         '''
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value_string("redirectUri", redirect_uri)
         data.add_value_string("companyName", company_name)
         data.add_value_string("companyUrl", company_url)
@@ -69,40 +65,39 @@
         data.add_value_string("clientSecret", client_secret)
 
         response = self.client.post_json(CLIENTS, data.data)
         response.success = response.status_code == 201
 
         return response
 
-    def update_client(
-            self, id=None, name=None, redirect_uri=None, company_name=None,
-            company_url=None, contact_person=None, contact_type=None,
-            email=None, phone=None, other_info=None, definition=None,
-            client_id=None, client_secret=None):
+
+    def update_client(self, id=None, name=None, redirect_uri=None, company_name=None, company_url=None, 
+                    contact_person=None, contact_type=None, email=None, phone=None, other_info=None, 
+                    definition=None, client_id=None, client_secret=None):
         '''
-        Update an API protection client.
+        Update an OIDC API protection client.
 
         Args:
             name (:obj:`str`): Name of the client.
             redirect_uri (:obj:`str`, optional): URL which client should redirect to.
             company_name (:obj:`str`, optional): Company to associate client with.
             company_url (:obj:`str`, optional): URL to associate client with.
             contact_person (:obj:`str`, optional): Person who is responsible for API client.
             contact_type (:obj:`str`, optional): Position of contact person.
             email (:obj:`str`, optional): Contact email address for client.
             phone (:obj:`str`, optional): Contact phone number for client.
-            other_info (:obj:`str`, optional): Other contact details assocaited with client.
-            definition (:obj:`str`): The id of the API protection definition to use
+            other_info (:obj:`str`, optional): Other contact details associated with client.
+            definition (:obj:`str`): The id of the API protection definition to use.
             client_id (:obj:`str`): The id of the client.
             client_secret (:obj:`str`, optional): The client secret to use. If not specified then a public client is created.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value_string("redirectUri", redirect_uri)
         data.add_value("companyName", company_name)
         data.add_value_string("companyUrl", company_url)
@@ -111,22 +106,24 @@
         data.add_value_string("email", email)
         data.add_value_string("phone", phone)
         data.add_value_string("otherInfo", other_info)
         data.add_value_string("definition", definition)
         data.add_value_string("clientId", client_id)
         data.add_value_string("clientSecret", client_secret)
 
-        response = self.client.put_json(CLIENTS+"/"+str(id), data.data)
+        endpoint = "{}/{}".format(CLIENTS, id)
+        response = self.client.put_json(endpoint, data.data)
         response.success = response.status_code == 204
 
         return response
 
+
     def delete_client(self, id):
         '''
-        Delete an API protection client.
+        Delete an OIDC API protection client.
 
         Args:
             id (:obj:`str`): The id of the client to be removed.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
@@ -136,63 +133,59 @@
         endpoint = "%s/%s" % (CLIENTS, id)
 
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
         return response
 
+
     def list_clients(self, sort_by=None, count=None, start=None, filter=None):
         '''
         Get a list of API clients.
 
         Args:
             sort_by (:obj:`str`, optional): Attribute to sort results by.
             count (:obj:`str`, optional): Maximum number of results to fetch.
-            start (:obj:`str`, optional): Pagenation offset of returned results.
+            start (:obj:`str`, optional): Pagination offset of returned results.
             filter (:obj:`str`): Attribute to filter results by
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the obligations are returned as JSON and can be accessed from
-            the response.json attribute
+            If the request is successful the API clients are returned as JSON and can be accessed from
+            the response.json attribute.
 
         '''
         parameters = DataObject()
         parameters.add_value_string("sortBy", sort_by)
         parameters.add_value_string("count", count)
         parameters.add_value_string("start", start)
         parameters.add_value_string("filter", filter)
 
         response = self.client.get_json(CLIENTS, parameters.data)
         response.success = response.status_code == 200
 
         return response
 
-    def create_definition(
-            self, name=None, description=None, tcm_behavior=None,
-            token_char_set=None, access_token_lifetime=None,
-            access_token_length=None, authorization_code_lifetime=None,
-            authorization_code_length=None, refresh_token_length=None,
-            max_authorization_grant_lifetime=None, pin_length=None,
-            enforce_single_use_authorization_grant=None,
-            issue_refresh_token=None,
-            enforce_single_access_token_per_grant=None,
-            enable_multiple_refresh_tokens_for_fault_tolerance=None,
+
+    def create_definition(self, name=None, description=None, tcm_behavior=None, token_char_set=None, access_token_lifetime=None,
+            access_token_length=None, authorization_code_lifetime=None, authorization_code_length=None, refresh_token_length=None,
+            max_authorization_grant_lifetime=None, pin_length=None, enforce_single_use_authorization_grant=None,
+            issue_refresh_token=None, enforce_single_access_token_per_grant=None, enable_multiple_refresh_tokens_for_fault_tolerance=None,
             pin_policy_enabled=None, grant_types=None):
         '''
         Create an OIDC API Protection definition. Definitions can be used to configure one or more clients.
 
         Args:
             name (:obj:`str`): Name of the OIDC definition.
             description (:obj:`str`, optional): Description of the OIDC definition.
             tcm_behavior (:obj:`str`, optional): Specify the Trust Client Manager's behavior.
-            token_char_set (:obj:`str`, optional): Specify the allowed characters for generated tokens. Default is alphanumeric set
+            token_char_set (:obj:`str`, optional): Specify the allowed characters for generated tokens. Default is alphanumeric set of characters.
             access_token_lifetime (int, optional): Length of time that access token is valid for.
             authorization_code_lifetime (int, optional): Length of time that authorization code is valid for.
             authorization_code_length (int, optional): Number of characters used to generate authorization code.
             refresh_token_length (int, optional): Number of characters used to generate refresh tokens.
             max_authorization_grant_lifetime (int, optional): The maximum duration of a grant, in seconds, where the resource owner authorized the client to access the protected resource.
             pin_length (int, optional): Length of PIN used to protect refresh token.
             enforce_single_use_authorization_grant (bool, optional): True if all tokens of the authorization grant should be revoked after an access token is validated.
@@ -203,15 +196,15 @@
             grant_types (:obj:`list` of :obj:`str`): A list of supported authorization grant types.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the id of the created obligation can be acess from the 
+            If the request is successful the id of the created OIDC definition can be accessed from the 
             response.id_from_location attribute
 
         '''
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value_string("description", description)
         data.add_value_string("tcmBehavior", tcm_behavior)
@@ -238,27 +231,22 @@
         data.add_value("grantTypes", grant_types)
 
         response = self.client.post_json(DEFINITIONS, data.data)
         response.success = response.status_code == 201
 
         return response
 
-    def update_definition(
-            self, definition_id=None, name=None, description=None, tcm_behavior=None,
-            token_char_set=None, access_token_lifetime=None,
-            access_token_length=None, authorization_code_lifetime=None,
-            authorization_code_length=None, refresh_token_length=None,
-            max_authorization_grant_lifetime=None, pin_length=None,
-            enforce_single_use_authorization_grant=None,
-            issue_refresh_token=None,
-            enforce_single_access_token_per_grant=None,
-            enable_multiple_refresh_tokens_for_fault_tolerance=None,
-            pin_policy_enabled=None, grant_types=None, oidc_enabled=False,
-            iss=None, poc=None, lifetime=None, alg=None, db=None, cert=None,
-            enc_enabled=False, enc_alg=None, enc_enc=None, access_policy_id=None):
+
+    def update_definition(self, definition_id=None, name=None, description=None, tcm_behavior=None,
+            token_char_set=None, access_token_lifetime=None, access_token_length=None, authorization_code_lifetime=None,
+            authorization_code_length=None, refresh_token_length=None, max_authorization_grant_lifetime=None, 
+            pin_length=None, enforce_single_use_authorization_grant=None, issue_refresh_token=None,
+            enforce_single_access_token_per_grant=None, enable_multiple_refresh_tokens_for_fault_tolerance=None,
+            pin_policy_enabled=None, grant_types=None, oidc_enabled=False, iss=None, poc=None, lifetime=None, alg=None, 
+            db=None, cert=None, enc_enabled=False, enc_alg=None, enc_enc=None, access_policy_id=None):
         '''
         Update an OIDC API Protection definition. Definitions can be used to configure one or more clients.
 
         Args:
             name (:obj:`str`): Name of the OIDC definition.
             description (:obj:`str`, optional): Description of the OIDC definition.
             tcm_behavior (:obj:`str`, optional): Specify the Trust Client Manager's behavior.
@@ -274,27 +262,27 @@
             enforce_single_access_token_per_grant (bool, optional): True if previously granted access tokens should be revoked after a new access token is generated via a refresh token.
             enable_multiple_refresh_tokens_for_fault_tolerance (bool, optional): True if multiple refresh tokens are stored so that the old refresh token is valid until the new refresh token is successfully delivered.
             pin_policy_enabled (bool, optional): True if the refresh token will be further protected with a PIN provided by the API protection client.
             grant_types (:obj:`list` of :obj:`str`): A list of supported authorization grant types.
             oidc_enabled (bool, optional): If OpenID Connect is enabled for this definition.
             iss (:obj:`str`): The issuer identifier of this definition.
             poc (:obj:`str`): The Point of Contact URL for this definition.
-            lifetime (int): The lifetime of the id_tokens issued
+            lifetime (int): The lifetime of the id_tokens issued.
             alg (:obj:`str`): The signing algorithm for the JWT.
             db (:obj:`str`): The SSL database containing the signing key for RS/ES signing methods.
             cert (:obj:`str`): The certificate label of the signing key for RS/ES signing methods.
             enc_enabled (bool): Is encryption enabled for this definition.
             enc_alg (:obj:`str`): The key agreement algorithm for encryption.
             enc_enc (:obj:`str`): The encryption algorithm.
             access_policy_id (int): The id of access policy assigned to this definition.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value_string("description", description)
         data.add_value_string("tcmBehavior", tcm_behavior)
         data.add_value_string("tokenCharSet", token_char_set)
@@ -338,160 +326,91 @@
             data.add_value("oidc",oidc.data)
 
         response = self.client.put_json(DEFINITIONS+"/"+str(definition_id), data.data)
         response.success = response.status_code == 204
 
         return response
 
+
     def delete_definition(self, id):
         '''
         Remove an OIDC API protection definition.
 
         Args:
             id (:obj:`str`): the id of the definition to be removed.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "%s/%s" % (DEFINITIONS, id)
 
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
         return response
 
+
     def list_definitions(self, sort_by=None, count=None, start=None, filter=None):
         '''
         Get a list of the configured API protection definitions.
 
         Args:
             sort_by (:obj:`str`, optional): Attribute to sort results by.
             count (:obj:`str`, optional): Maximum number of results to fetch.
-            start (:obj:`str`, optional): Pagenation offset of returned results.
+            start (:obj:`str`, optional): Pagination offset of returned results.
             filter (:obj:`str`): Attribute to filter results by.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the obligations are returned as JSON and can be accessed from
-            the response.json attribute
+            If the request is successful the OIDC definitions are returned as JSON and can be accessed from
+            the response.json attribute.
 
         '''
         parameters = DataObject()
         parameters.add_value_string("sortBy", sort_by)
         parameters.add_value_string("count", count)
         parameters.add_value_string("start", start)
         parameters.add_value_string("filter", filter)
 
         response = self.client.get_json(DEFINITIONS, parameters.data)
         response.success = response.status_code == 200
 
         return response
 
-    def create_mapping_rule(self, name=None, category=None, file_name=None, content=None):
-        '''
-        Should this even exist?
-        '''
-        data = DataObject()
-        data.add_value_string("name", name)
-        data.add_value_string("category", category)
-        data.add_value_string("fileName", file_name)
-        data.add_value_string("content", content)
-
-        response = self.client.post_json(MAPPING_RULES, data.data)
-        response.success = response.status_code == 201
-
-        return response
-
-    def list_mapping_rules(self, sort_by=None, count=None, start=None, filter=None):
-        '''
-        Should this even exist?
-        '''
-        parameters = DataObject()
-        parameters.add_value_string("sortBy", sort_by)
-        parameters.add_value_string("count", count)
-        parameters.add_value_string("start", start)
-        parameters.add_value_string("filter", filter)
-
-        response = self.client.get_json(MAPPING_RULES, parameters.data)
-        response.success = response.status_code == 200
-
-        return response
-
-    def import_mapping_rule(self, id, file_path):
-        '''
-        Should this even exist?
-        '''
-        response = Response()
-
-        try:
-            with open(file_path, 'rb') as mapping_rule:
-                files = {"file": mapping_rule}
-                endpoint = "%s/%s/file" % (MAPPING_RULES, id)
-                accept_type = "%s,%s" % ("application/json", "text/html")
-
-                response = self.client.post_file(
-                    endpoint, accept_type=accept_type, files=files)
-
-                response.success = response.status_code == 200
-        except IOError as e:
-            logger.error(e)
-            response.success = False
-
-        return response
-
-    def update_mapping_rule(self, id, content=None):
-        '''
-        Should this even exist?
-        '''
-        data = DataObject()
-        data.add_value_string("content", content)
-
-        endpoint = "%s/%s" % (MAPPING_RULES, id)
-
-        response = self.client.put_json(endpoint, data.data)
-        response.success = response.status_code == 204
-
-        return response
 
 class APIProtection9040(APIProtection):
 
     def __init__(self, base_url, username, password):
         super(APIProtection, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
     def get_valid_grant_types(self):
         return ["AUTHORIZATION_CODE","RESOURCE_OWNER_PASSWORD_CREDENTIALS","IMPLICIT_GRANT", "CLIENT_CREDENTIALS", "JWT_BEARER", "SAML_BEARER"]
 
-    def create_definition(
-            self, name=None, description=None, tcm_behavior=None,
-            token_char_set=None, access_token_lifetime=None,
-            access_token_length=None, authorization_code_lifetime=None,
-            authorization_code_length=None, refresh_token_length=None,
-            max_authorization_grant_lifetime=None, pin_length=None,
-            enforce_single_use_authorization_grant=None,
-            issue_refresh_token=None,
-            enforce_single_access_token_per_grant=None,
-            enable_multiple_refresh_tokens_for_fault_tolerance=None,
-            pin_policy_enabled=None, grant_types=None, oidc_enabled=False,
-            iss=None, poc=None, lifetime=None, alg=None, db=None, cert=None,
-            enc_enabled=False, enc_alg=None, enc_enc=None, access_policy_id=None):
+    def create_definition(self, name=None, description=None, tcm_behavior=None, token_char_set=None, access_token_lifetime=None,
+            access_token_length=None, authorization_code_lifetime=None, authorization_code_length=None, refresh_token_length=None,
+            max_authorization_grant_lifetime=None, pin_length=None, enforce_single_use_authorization_grant=None,
+            issue_refresh_token=None, enforce_single_access_token_per_grant=None,
+            enable_multiple_refresh_tokens_for_fault_tolerance=None, pin_policy_enabled=None, grant_types=None, oidc_enabled=False,
+            iss=None, poc=None, lifetime=None, alg=None, db=None, cert=None, enc_enabled=False, enc_alg=None, enc_enc=None, 
+            access_policy_id=None, attribute_sources=None):
         '''
         Create an OIDC API Protection definition. Definitions can be used to configure one or more clients.
 
         Args:
             name (:obj:`str`): Name of the OIDC definition.
             description (:obj:`str`, optional): Description of the OIDC definition.
             tcm_behavior (:obj:`str`, optional): Specify the Trust Client Manager's behavior.
-            token_char_set (:obj:`str`, optional): Specify the allowed characters for generated tokens. Default is alphanumeric set
+            token_char_set (:obj:`str`, optional): Specify the allowed characters for generated tokens. Default is alphanumeric set of characters.
             access_token_lifetime (int, optional): Length of time that access token is valid for.
             authorization_code_lifetime (int, optional): Length of time that authorization code is valid for.
             authorization_code_length (int, optional): Number of characters used to generate authorization code.
             refresh_token_length (int, optional): Number of characters used to generate refresh tokens.
             max_authorization_grant_lifetime (int, optional): The maximum duration of a grant, in seconds, where the resource owner authorized the client to access the protected resource.
             pin_length (int, optional): Length of PIN used to protect refresh token.
             enforce_single_use_authorization_grant (bool, optional): True if all tokens of the authorization grant should be revoked after an access token is validated.
@@ -506,22 +425,22 @@
             lifetime (int): The lifetime of the id_tokens issued
             alg (:obj:`str`): The signing algorithm for the JWT.
             db (:obj:`str`): The SSL database containing the signing key for RS/ES signing methods.
             cert (:obj:`str`): The certificate label of the signing key for RS/ES signing methods.
             enc_enabled (bool): Is encryption enabled for this definition.
             enc_alg (:obj:`str`): The key agreement algorithm for encryption.
             enc_enc (:obj:`str`): The encryption algorithm.
-            access_policy_id (int): The id of access policy assigned to this definition.
+            attribute_sources (:obj:`list` of :obj:`dict`): Array of configured attribute sources to use in id_token generation and userinfo requests.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the id of the created obligation can be acess from the 
+            If the request is successful the id of the created OIDC definition can be accessed from the 
             response.id_from_location attribute
 
         '''
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value_string("description", description)
         data.add_value_string("tcmBehavior", tcm_behavior)
@@ -530,83 +449,83 @@
         data.add_value("accessTokenLength", access_token_length)
         data.add_value("authorizationCodeLifetime", authorization_code_lifetime)
         data.add_value("authorizationCodeLength", authorization_code_length)
         data.add_value("refreshTokenLength", refresh_token_length)
         data.add_value(
             "maxAuthorizationGrantLifetime", max_authorization_grant_lifetime)
         data.add_value("pinLength", pin_length)
-        data.add_value(
+        data.add_value_boolean(
             "enforceSingleUseAuthorizationGrant",
             enforce_single_use_authorization_grant)
-        data.add_value("issueRefreshToken", issue_refresh_token)
-        data.add_value(
+        data.add_value_boolean("issueRefreshToken", issue_refresh_token)
+        data.add_value_boolean(
             "enforceSingleAccessTokenPerGrant",
             enforce_single_access_token_per_grant)
-        data.add_value(
+        data.add_value_boolean(
             "enableMultipleRefreshTokensForFaultTolerance",
             enable_multiple_refresh_tokens_for_fault_tolerance)
-        data.add_value("pinPolicyEnabled", pin_policy_enabled)
+        data.add_value_boolean("pinPolicyEnabled", pin_policy_enabled)
         data.add_value("grantTypes", grant_types)
         data.add_value("accessPolicyId", access_policy_id)
 
         if oidc_enabled:
             oidc = DataObject()
-            oidc.add_value("enabled",True)
+            oidc.add_value_boolean("enabled",True)
             oidc.add_value("iss",iss)
             oidc.add_value("poc",poc)
             oidc.add_value("lifetime",lifetime)
             oidc.add_value("alg",alg)
             oidc.add_value("db",db)
             oidc.add_value("cert",cert)
             if enc_enabled:
                 enc_data = DataObject()
-                enc_data.add_value("db",enc_db)
-                enc_data.add_value("cert",enc_cert)
+                enc_data.add_value_boolean("enabled",True)
+                enc_data.add_value("alg",enc_alg)
+                enc_data.add_value("enc",enc_enc)
                 oidc.add_value("enc",enc_data.data)
 
             data.add_value("oidc",oidc.data)
+        data.add_value("attributeSources", attribute_sources)
 
         response = self.client.post_json(DEFINITIONS, data.data)
         response.success = response.status_code == 201
 
         return response
 
-    def create_client(
-            self, name=None, redirect_uri=None, company_name=None,
-            company_url=None, contact_person=None, contact_type=None,
-            email=None, phone=None, other_info=None, definition=None,
-            client_id=None, client_secret=None, require_pkce_verification=None,
-            jwks_uri=None, encryption_db=None, encryption_cert=None):
+
+    def create_client(self, name=None, redirect_uri=None, company_name=None, company_url=None, contact_person=None, 
+            contact_type=None, email=None, phone=None, other_info=None, definition=None, client_id=None, 
+            client_secret=None, require_pkce_verification=None, jwks_uri=None, encryption_db=None, encryption_cert=None):
         '''
-        Create an OIDC api protection client
+        Create an OIDC api protection client.
 
         Args:
             name (:obj:`str`): Name of the client.
             redirect_uri (:obj:`str`, optional): URL which client should redirect to.
             company_name (:obj:`str`, optional): Company to associate client with.
             company_url (:obj:`str`, optional): URL to associate client with.
             contact_person (:obj:`str`, optional): Person who is responsible for API client.
             contact_type (:obj:`str`, optional): Position of contact person.
             email (:obj:`str`, optional): Contact email address for client.
             phone (:obj:`str`, optional): Contact phone number for client.
-            other_info (:obj:`str`, optional): Other contact details assocaited with client.
-            definition (:obj:`str`): The id of the API protection definition to use
+            other_info (:obj:`str`, optional): Other contact details associated with client.
+            definition (:obj:`str`): The id of the API protection definition to use.
             client_id (:obj:`str`): The id of the client.
             client_secret (:obj:`str`, optional): The client secret to use. If not specified then a public client is created.
             require_pkce_verification (bool, optional): Whether or not this client must perform proof of key exchange when performing an authorization code flow.
             jwks_uri (:obj:`str`): URI which is the location that a clients published JWK set.
             encryption_db (:obj:`str): The SSL database containing the JWT encryption key.
             encryption_cert (:obj:`str`): The certificate label of the JWT encryption key.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the id of the created obligation can be acess from the 
+            If the request is successful the id of the created OIDC client can be accessed from the 
             response.id_from_location attribute
 
         '''
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value("redirectUri", redirect_uri)
         data.add_value_string("companyName", company_name)
```

### Comparing `pyisva-0.1.0/pyisva/core/access/attributes.py` & `pyisva-0.2.0/pyisva/core/federation/attributesources.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,139 @@
 """
 @copyright: IBM
 """
 
 import logging
+import uuid
 
 from pyisva.util.model import DataObject
 from pyisva.util.restclient import RESTClient
 
-
-ATTRIBUTE_MATCHERS = "/iam/access/v8/attribute-matchers"
-ATTRIBUTES = "/iam/access/v8/attributes"
+ATTRIBUTE_SOURCES = "/mga/attribute_sources/"
 
 logger = logging.getLogger(__name__)
 
-
-class Attributes(object):
+class AttributeSources(object):
 
     def __init__(self, base_url, username, password):
-        super(Attributes, self).__init__()
+        super(AttributeSources, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
-    def create_attribute(
-            self, category=None, matcher=None, issuer=None, description=None,
-            name=None, datatype=None, uri=None, storage_session=None,
-            storage_behavior=None, storage_device=None, type_risk=None,
-            type_policy=None):
-        '''
-        Create an CBA attribute.
+    def create_attribute_source(self, attribute_name=None, attribute_type=None, attribute_value=True, properties=None):
+        """
+        Create a new attribute source
 
         Args:
-            category (:obj:`str`): The part of the XACML request that the attribute value comes from.
-            matcher (:obj:`str`): ID of the attribute matcher.
-            issuer (:obj:`str`): The name of the policy information point from which the value of the attribute is retrieved.
-            description (:obj:`str`, optional): Description of the attribute.
-            name (:obj:`str`): Name of the attribute
-            datatype (:obj:`str`): The type of values that the attribute can accept.
-            uri (:obj:`str`): The identifier of the attribute that is used in the generated XACML policy.
-            storage_session (bool): True if the attribute is collected in the user session.
-            storage_behavior (bool): True if historic data for this attribute is stored in the database and used for behavior-based attribute matching.
-            storage_device (bool): True if the attribute is stored when a device is registered as part of the device fingerprint.
-            type_risk (bool): True if the attribute is used in risk profiles.
-            type_policy (bool): True if the attribute is used in policies.
+            attribute_name (:obj:`str`): The name of the attribute.
+            attribute_type (:obj:`str`): The type of the attribute source. Valid types are: credential, value, ldap.
+            attribute_value (:obj:`str`): The value of the source attribute.
+            properties (:obj:`list` of :obj:`dict`): The properties associated with an attribute source.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the id of the created obligation can be acess from the 
+            If the request is successful the id of the created attribute source can be accessed from the
             response.id_from_location attribute
 
-        '''
-        storage_data = DataObject()
-        storage_data.add_value("session", storage_session)
-        storage_data.add_value("behavior", storage_behavior)
-        storage_data.add_value("device", storage_device)
-
-        type_data = DataObject()
-        type_data.add_value("risk", type_risk)
-        type_data.add_value("policy", type_policy)
-
+        """
         data = DataObject()
-        data.add_value_string("category", category)
-        data.add_value_string("matcher", matcher)
-        data.add_value_string("issuer", issuer)
-        data.add_value_string("description", description)
-        data.add_value_string("name", name)
-        data.add_value_string("datatype", datatype)
-        data.add_value_string("uri", uri)
-        data.add_value("predefined", False)
-        data.add_value_not_empty("storageDomain", storage_data.data)
-        data.add_value_not_empty("type", type_data.data)
+        data.add_value_string("name", attribute_name)
+        data.add_value_string("type", attribute_type)
+        data.add_value_string("value", attribute_value)
+        data.add_value("properties", properties)
 
-        response = self.client.post_json(ATTRIBUTES, data.data)
+        response = self.client.post_json(ATTRIBUTE_SOURCES, data.data)
         response.success = response.status_code == 201
-
         return response
 
-    def list_attributes(self, sort_by=None, count=None, start=None, filter=None):
-        '''
-        Get a list of the configured attributes.
+
+    def update_attribute_source(self, attribute_name=None, attribute_new_name=None, attribute_type=None, attribute_value=True, properties=None):
+        """
+        Update an existing attribute source
 
         Args:
-            sort_by (:obj:`str`, optional): Attribute to sort results by.
-            count (:obj:`str`, optional): Maximum number of results to fetch.
-            start (:obj:`str`, optional): Pagenation offset of returned results.
-            filter (:obj:`str`): Attribute to filter results by.
+            attribute_name (:obj:`str`): The name of the attribute.
+            attribute_new_name (:obj:`str`, optional): The new name of the attribute.
+            attribute_type (:obj:`str`): The type of the attribute source. Valid types are: credential, value, ldap.
+            attribute_value (:obj:`str`): The value of the source attribute.
+            properties (:obj:`list` of :obj:`str`): The properties associated with an attribute source.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the obligations are returned as JSON and can be accessed from
-            the response.json attribute
+            If the request is successful the id of the created attribute source can be accessed from the
+            response.id_from_location attribute
 
-        '''
-        parameters = DataObject()
-        parameters.add_value_string("sortBy", sort_by)
-        parameters.add_value_string("count", count)
-        parameters.add_value_string("start", start)
-        parameters.add_value_string("filter", filter)
+        """
+        data = DataObject()
+        name = attribute_new_name if attribute_new_name != None else attribute_name
+        data.add_value_string("name", name)
+        data.add_value_string("type", attribute_type)
+        data.add_value_string("value", attribute_value)
+        data.add_value("properties", properties)
+
+        endpoint = "%s/%s" % (ATTRIBUTE_SOURCES, attribute_name)
+        response = self.client.post_json(ATTRIBUTE_SOURCES, data.data)
+        response.success = response.status_code == 204
+        return response
 
-        response = self.client.get_json(ATTRIBUTES, parameters.data)
-        response.success = response.status_code == 200
 
+    def delete_attribute_source(self, attribute_name=None):
+        """
+        Delete a configured attribute source
+
+        Args:
+            attribute_name (:obj:`str`): The name of the attribute to be removed.
+
+        Returns:
+            :obj:`~requests.Response`: The response from verify access. 
+
+            Success can be checked by examining the response.success boolean attribute
+
+        """
+        endpoint = "%s/%s" % (ATTRIBUTE_SOURCES, attribute_name)
+        response = self.client.delete_json(endpoint)
+        response.success = response.status_code == 204
         return response
 
-    def list_attribute_matchers(self, sort_by=None, filter=None):
-        '''
-        Get a list of the configured attribute matchers.
+    def get_attribute_source(self, attribute_name=None):
+        """
+        Get a configured attribute source
 
         Args:
-            sort_by (:obj:`str`, optional): Attribute to sort results by.
-            filter (:obj:`str`): Attribute to filter results by.
+            attribute_name (:obj:`str`): THe name of the attribute to get config for.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the obligations are returned as JSON and can be accessed from
+            If the request is successful the attribute source is returned as JSON and can be accessed from
             the response.json attribute
 
-        '''
-        parameters = DataObject()
-        parameters.add_value_string("sortBy", sort_by)
-        parameters.add_value_string("filter", filter)
-
-        response = self.client.get_json(ATTRIBUTE_MATCHERS, parameters.data)
+        """
+        endpoint = "%s/%s" % (ATTRIBUTE_SOURCES, attribute_name)
+        response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
+        return response
+
+
+    def list_attribute_sources(self):
+        """
+        Get a list of the configured attribute sources
 
+        Returns:
+            :obj:`~requests.Response`: The response from verify access. 
+
+            Success can be checked by examining the response.success boolean attribute
+
+            If the request is successful the attribute sources are returned as JSON and can be accessed from
+            the response.json attribute
+
+        """
+        response = self.client.get_json(ATTRIBUTE_SOURCES)
+        response.success = response.status_code == 200
         return response
```

### Comparing `pyisva-0.1.0/pyisva/core/access/authentication.py` & `pyisva-0.2.0/pyisva/core/access/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,44 +25,44 @@
             properties=[], attributes=[]):
         '''
         Create an authentication mechanism.
 
         Args:
             description: (:obj:`str`): Description of the mechanism.
             name (:obj:`str`): Name of the mechanism.
-            uri (:obj:`str`): URI of the mechainsm.
+            uri (:obj:`str`): URI of the mechanism.
             type_id (:obj:`str`): Mechanism type to inherit from
-            properties (:obj:`list` of :obj:`dict`): List of properties for the mechaism. Properties are determined by 
+            properties (:obj:`list` of :obj:`dict`): List of properties for the mechanism. Properties are determined by 
                                                     the mechanism type. Properties should follow the 
                                                     format::
 
                                                             [
                                                                 {"key":"property.key.name", 
                                                                  "value":"property.value"
                                                                 }
                                                             ]
 
-            attributes: (:obj:`list` of :obj:`dict`): List of attributes to retireve from the request context before 
+            attributes: (:obj:`list` of :obj:`dict`): List of attributes to retrieve from the request context before 
                                                     executing the mechanism. Attributes should follow the 
                                                     format::
 
                                                             [
                                                                 {"selector":"Context.REQUEST", 
                                                                  "namespace": "urn:ibm:security:asf:request:parameter", 
                                                                  "name": "parameter"
                                                                 }
                                                             ]
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the id of the created mechanism can be acess from the 
-            response.id_from_location attribute
+            If the request is successful the id of the created mechanism can be accessed from the 
+            response.id_from_location attribute.
 
         '''
         data = DataObject()
         data.add_value_string("description", description)
         data.add_value_string("name", name)
         data.add_value_string("uri", uri)
         data.add_value_string("typeId", type_id)
@@ -70,97 +70,101 @@
         data.add_value_not_empty("attributes", attributes)
 
         response = self.client.post_json(AUTHENTICATION_MECHANISMS, data.data)
         response.success = response.status_code == 201
 
         return response
 
+
     def list_mechanism_types(self, sort_by=None, count=None, start=None, filter=None):
         '''
-        Get the list of avaliable mechanism types
+        Get the list of available mechanism types
 
         Args:
             sort_by (:obj:`str`, optional): Attribute to sort results by.
             count (:obj:`str`, optional): Maximum number of results to fetch.
-            start (:obj:`str`, optional): Pagenation offset of returned results.
+            start (:obj:`str`, optional): Pagination offset of returned results.
             filter (:obj:`str`): Attribute to filter results by.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the obligations are returned as JSON and can be accessed from
-            the response.json attribute
+            If the request is successful the authentication mechanism types are returned as JSON and can be accessed from
+            the response.json attribute.
 
         '''
         parameters = DataObject()
         parameters.add_value_string("sortBy", sort_by)
         parameters.add_value_string("count", count)
         parameters.add_value_string("start", start)
         parameters.add_value_string("filter", filter)
 
         response = self.client.get_json(
             AUTHENTICATION_MECHANISM_TYPES, parameters.data)
         response.success = response.status_code == 200
 
         return response
 
+
     def list_mechanisms(self, sort_by=None, count=None, start=None, filter=None):
         '''
-        Get the list of avaliable mechanisms
+        Get the list of available mechanisms
 
         Args:
             sort_by (:obj:`str`, optional): Attribute to sort results by.
             count (:obj:`str`, optional): Maximum number of results to fetch.
-            start (:obj:`str`, optional): Pagenation offset of returned results.
+            start (:obj:`str`, optional): Pagination offset of returned results.
             filter (:obj:`str`): Attribute to filter results by.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the obligations are returned as JSON and can be accessed from
-            the response.json attribute
+            If the request is successful the authentication mechanism are returned as JSON and can be accessed from
+            the response.json attribute.
 
         '''
         parameters = DataObject()
         parameters.add_value_string("sortBy", sort_by)
         parameters.add_value_string("count", count)
         parameters.add_value_string("start", start)
         parameters.add_value_string("filter", filter)
 
         response = self.client.get_json(
             AUTHENTICATION_MECHANISMS, parameters.data)
         response.success = response.status_code == 200
 
         return response
 
+
     def update_mechanism(self, id, description=None, name=None, uri=None, type_id=None,
-            predefined=None, properties=None, attributes=None):
+            predefined=True, properties=None, attributes=None):
         '''
         Update an authentication mechanism.
 
         Args:
             description: (:obj:`str`): Description of the mechanism.
             name (:obj:`str`): Name of the mechanism.
-            uri (:obj:`str`): URI of the mechainsm.
-            type_id (:obj:`str`): Mechanism type to inherit from
-            properties (:obj:`list` of :obj:`dict`): List of properties for the mechaism. Properties are determined by 
+            uri (:obj:`str`): URI of the mechanism.
+            type_id (:obj:`str`): Mechanism type to inherit from.
+            predefined (bool, optional): If this mechanism is pre-defined by Verify Access. Default value is ``true``.
+            properties (:obj:`list` of :obj:`dict`): List of properties for the mechanism. Properties are determined by 
                                                     the mechanism type. Properties should use the 
                                                     format::
 
                                                             [
                                                                 {"key":"property.key.name", 
                                                                  "value":"property.value"
                                                                 }
                                                             ]
 
-            attributes: (:obj:`list` of :obj:`dict`): List of attributes to retireve from the request context before 
+            attributes: (:obj:`list` of :obj:`dict`): List of attributes to retrieve from the request context before 
                                                     executing the mechanism. Attributes should use the 
                                                     format::
 
                                                             [
                                                                 {"selector":"Context.REQUEST", 
                                                                  "namespace": "urn:ibm:security:asf:request:parameter", 
                                                                  "name": "parameter"
@@ -168,70 +172,92 @@
                                                             ]
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the id of the created mechanism can be acess from the 
+            If the request is successful the id of the created mechanism can be accessed from the 
             response.id_from_location attribute
 
         '''
         data = DataObject()
         data.add_value_string("id", id)
         data.add_value_string("description", description)
         data.add_value_string("name", name)
         data.add_value_string("uri", uri)
         data.add_value_string("typeId", type_id)
-        data.add_value("predefined", predefined)
-        data.add_value("properties", properties)
-        data.add_value("attributes", attributes)
+        data.add_value_boolean("predefined", predefined)
+        data.add_value_not_empty("properties", properties)
+        data.add_value_not_empty("attributes", attributes)
 
         endpoint = "%s/%s" % (AUTHENTICATION_MECHANISMS, id)
 
         response = self.client.put_json(endpoint, data.data)
         response.success = response.status_code == 204
 
         return response
 
+
+    def delete_mechanism(self, mechanism_id):
+        '''
+        Delete an existing authentication mechanism. Only  administrator created (not pre-defined) mechanisms can be deleted.
+
+        Args:
+            mechanism_id (:obj:`str`): The identifier for the mechanism to be removed.
+        
+        Returns:
+            :obj:`~requests.Response`: The response from verify access. 
+
+            Success can be checked by examining the response.success boolean attribute.
+
+        '''
+        endpoint = "{}/{}".format(AUTHENTICATION_MECHANISMS, id)
+        response = self.client.delete_json(endpoint)
+        response.success = response.status_code == 204
+
+        return response
+
+
     def create_policy(self, name=None, policy=None, uri=None, description=None,
             dialect="urn:ibm:security:authentication:policy:1.0:schema", enabled=None):
         '''
         Create an authentication policy.
 
         Args:
-            name (:obj:`str`): Name of the policy to be created
+            name (:obj:`str`): Name of the policy to be created.
             policy (:obj:`str`): XML config of the policy.
             uri (:obj:`str`): URI used to identify the policy.
             description (:obj:`str`, optional): Description of the policy.
-            dialect (:obj:`str`, optional): Schema used to create policy. use the default "urn:ibm:security:authentication:policy:1.0:schema"
+            dialect (:obj:`str`, optional): Schema used to create policy. use the default "urn:ibm:security:authentication:policy:1.0:schema".
             enabled (bool): Flag to enable the policy for use by the AAC runtime.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the id of the created mechanism can be acess from the 
-            response.id_from_location attribute
+            If the request is successful the id of the created mechanism can be accessed from the 
+            response.id_from_location attribute.
 
         '''
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value_string("policy", policy)
         data.add_value_string("uri", uri)
         data.add_value_string("description", description)
         data.add_value_string("dialect", dialect)
-        data.add_value_string("enabled", enabled)
+        data.add_value_boolean("enabled", enabled)
 
         response = self.client.post_json(AUTHENTICATION_POLICIES, data.data)
         response.success = response.status_code == 201
 
         return response
 
+
     def get_policy(self, id):
         '''
         Retrieve a policy configuration.
 
         Args:
             id (:obj:`str`): the id of the policy to be deleted.
 
@@ -247,45 +273,47 @@
         endpoint = "%s/%s" % (AUTHENTICATION_POLICIES, id)
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
+
     def list_policies(self, sort_by=None, count=None, start=None, filter=None):
         '''
         Get a list of all of hte configured AAC policies.
 
         Args:
             sort_by (:obj:`str`, optional): Attribute to sort results by.
             count (:obj:`str`, optional): Maximum number of results to fetch.
-            start (:obj:`str`, optional): Pagenation offset of returned results.
+            start (:obj:`str`, optional): Pagination offset of returned results.
             filter (:obj:`str`): Attribute to filter results by
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the obligations are returned as JSON and can be accessed from
-            the response.json attribute
+            If the request is successful the authentication policies are returned as JSON and can be accessed from
+            the response.json attribute.
 
         '''
         parameters = DataObject()
         parameters.add_value_string("sortBy", sort_by)
         parameters.add_value_string("count", count)
         parameters.add_value_string("start", start)
         parameters.add_value_string("filter", filter)
 
         response = self.client.get_json(
             AUTHENTICATION_POLICIES, parameters.data)
         response.success = response.status_code == 200
 
         return response
 
+
     def update_policy(self, id, name=None, policy=None, uri=None, description=None,
             dialect="urn:ibm:security:authentication:policy:1.0:schema",
             user_last_modified=None, last_modified=None,
             date_created=None, predefined=None, enabled=None):
         '''
         Update an AAC authentication policy
 
@@ -293,38 +321,38 @@
             id (:obj:`str`): The id of the policy to be updated.
             name (:obj:`str`): Name of the policy.
             policy (:obj:`str`): XML config of the policy.
             uri (:obj:`str`): URI used to identify the policy.
             description (:obj:`str`, optional): Description of the policy.
             dialect (:obj:`str`, optional): Schema used to create policy. use the default 
                                             ``urn:ibm:security:authentication:policy:1.0:schema``
-            user_las_mdified (:obj:`str`): User id of the user who last made modifications to the authentication policy.
+            user_las_modified (:obj:`str`): User id of the user who last made modifications to the authentication policy.
             last_modified (:obj:`str`): Timestamp of when this policy was last modified.
             date_created (:obj:`str`): Timestamp of when this policy was created.
-            predefined (bool): Flag to indicate if this is a default policy avaliable out of the box.
+            predefined (bool): Flag to indicate if this is a default policy available out of the box.
             enabled (bool): Flag to enable the policy for use by the AAC runtime.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value_string("policy", policy)
         data.add_value_string("uri", uri)
         data.add_value_string("description", description)
         data.add_value_string("dialect", dialect)
         data.add_value_string("id", id)
-        data.add_value_string("enabled", enabled)
+        data.add_value_boolean("enabled", enabled)
         data.add_value_string("userlastmodified", user_last_modified)
         data.add_value_string("lastmodified", last_modified)
         data.add_value_string("datecreated", date_created)
-        data.add_value("predefined", predefined)
+        data.add_value_boolean("predefined", predefined)
 
         endpoint = "%s/%s" % (AUTHENTICATION_POLICIES, id)
 
         response = self.client.put_json(endpoint, data.data)
         response.success = response.status_code == 204
 
         return response
@@ -338,86 +366,87 @@
     def create_policy(self, name=None, policy=None, uri=None, description=None,
             dialect="urn:ibm:security:authentication:policy:1.0:schema",
             id=None, user_last_modified=None, last_modified=None,
             date_created=None, enabled=True):
         '''
         Create an authentication policy.
 
-        Agrs:
+        Args:
             name (:obj:`str`): Name of the policy to be created
             policy (:obj:`str`): XML config of the policy.
             uri (:obj:`str`): URI used to identify the policy.
             description (:obj:`str`, optional): Description of the policy.
             dialect (:obj:`str`, optional): Schema used to create policy. use the default "urn:ibm:security:authentication:policy:1.0:schema"
-            enabled (bool): Flag to enable the policy for use by the AAC runtime.
+            enabled (bool, optional): Flag to enable the policy for use by the AAC runtime. Default is ``true``.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the id of the created mechanism can be acess from the 
+            If the request is successful the id of the created mechanism can be accessed from the 
             response.id_from_location attribute
 
         '''
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value_string("policy", policy)
         data.add_value_string("uri", uri)
         data.add_value_string("description", description)
         data.add_value_string("dialect", dialect)
         data.add_value_string("id", id)
         data.add_value_string("userlastmodified", user_last_modified)
         data.add_value_string("lastmodified", last_modified)
         data.add_value_string("datecreated", date_created)
-        data.add_value("enabled", enabled)
+        data.add_value_boolean("enabled", enabled)
 
         response = self.client.post_json(AUTHENTICATION_POLICIES, data.data)
         response.success = response.status_code == 201
 
         return response
 
+
     def update_policy(self, id, name=None, policy=None, uri=None, description=None,
             dialect="urn:ibm:security:authentication:policy:1.0:schema",
             user_last_modified=None, last_modified=None,
             date_created=None, predefined=None, enabled=True):
         '''
         Update an AAC authentication policy
 
-        Agrs:
+        Args:
             id (:obj:`str`): The id of the policy to be updated.
             name (:obj:`str`): Name of the policy.
             policy (:obj:`str`): XML config of the policy.
             uri (:obj:`str`): URI used to identify the policy.
             description (:obj:`str`, optional): Description of the policy.
             dialect (:obj:`str`, optional): Schema used to create policy. use the default "urn:ibm:security:authentication:policy:1.0:schema"
             user_las_modified (:obj:`str`): User id of the user who last made modifications to the authentication policy.
             last_modified (:ob:`str`): Timestamp of when this policy was last modified.
             date_created (:obj:`str`): Timestamp of when this policy was created.
-            predefined (bool): Flag to indicate if this is a default policy avaliable out of the box.
-            enabled (bool): Flag to enable the policy for use by the AAC runtime.
+            predefined (bool): Flag to indicate if this is a default policy available out of the box.
+            enabled (bool, optional): Flag to enable the policy for use by the AAC runtime. Default is ``true``.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value_string("policy", policy)
         data.add_value_string("uri", uri)
         data.add_value_string("description", description)
         data.add_value_string("dialect", dialect)
         data.add_value_string("id", id)
         data.add_value_string("userlastmodified", user_last_modified)
         data.add_value_string("lastmodified", last_modified)
         data.add_value_string("datecreated", date_created)
-        data.add_value("predefined", predefined)
-        data.add_value("enabled", enabled)
+        data.add_value_boolean("predefined", predefined)
+        data.add_value_boolean("enabled", enabled)
 
         endpoint = "%s/%s" % (AUTHENTICATION_POLICIES, id)
 
         response = self.client.put_json(endpoint, data.data)
         response.success = response.status_code == 204
 
         return response
@@ -426,44 +455,44 @@
     def disable_all_policies(self):
         '''
         Disable all authentication policies.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         data = DataObject()
-        data.add_value("enabled", False)
+        data.add_value_boolean("enabled", False)
         response = self.client.put_json(AUTHENTICATION_POLICIES, data.data)
         response.success = response.status_code == 204
         return response
 
 
     def enable_all_policies(self):
         '''
         Enable all authentication policies.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         data = DataObject()
-        data.add_value("enabled", True)
+        data.add_value_boolean("enabled", True)
         response = self.client.put_json(AUTHENTICATION_POLICIES, data.data)
         response.success = response.status_code == 204
         return response
 
 
     def delete_policy(self, _id):
         '''
-        Remove an authenication policy.
+        Remove an authentication policy.
 
         Args:
             _id (:obj:`str`): The id of the policy to be removed.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
@@ -471,29 +500,8 @@
 
         '''
         endpoint = "%s/%s" % (AUTHENTICATION_POLICIES, _id)
 
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
-        return response
-
-
-    def delete_mechanism(self, _id):
-        '''
-        Remove an authenication mechanism.
-
-        Args:
-            _id (:obj:`str`): The id of the mechanism to be removed.
-
-        Returns:
-            :obj:`~requests.Response`: The response from verify access. 
-
-            Success can be checked by examining the response.success boolean attribute
-
-        '''
-        endpoint = "%s/%s" % (AUTHENTICATION_MECHANISMS, _id)
-
-        response = self.client.delete_json(endpoint)
-        response.success = response.status_code == 204
-
-        return response
+        return response
```

### Comparing `pyisva-0.1.0/pyisva/core/access/fido2config.py` & `pyisva-0.2.0/pyisva/core/web/runtimecomponent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,447 +1,380 @@
 """
 @copyright: IBM
 """
 
-import ntpath
 import logging
 
-from pyisva.util.model import DataObject, Response
+from pyisva.util.model import DataObject
 from pyisva.util.restclient import RESTClient
 
 
-"""
-Allows basic management of FIDO2 relying party configurations and metadata
-"""
-FIDO2_RELYING_PARTIES="/iam/access/v8/fido2/relying-parties"
-FIDO2_METADATA="/iam/access/v8/fido2/metadata"
-FIDO2_MEDIATOR="/iam/access/v8/mapping-rules"
+EMBEDDED_LDAP_PASSWORD = "/isam/embedded_ldap/change_pwd/v1"
+RUNTIME_COMPONENT = "/isam/runtime_components"
+UNCONFIGURE_RUNTIME_COMPONENT = RUNTIME_COMPONENT + "/RTE"
+FEDERATED_DIRECTORIES = RUNTIME_COMPONENT + "/federated_directories"
+RUNTIME_STANZA_FILE_BASE = "/isam/runtime"
 
 logger = logging.getLogger(__name__)
 
 
-class FIDO2Config(object):
+class RuntimeComponent(object):
 
     def __init__(self, base_url, username, password):
-        super(FIDO2Config, self).__init__()
+        super(RuntimeComponent, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
+    def configure(
+            self, ps_mode=None, user_registry=None, admin_password=None,
+            ldap_password=None, admin_cert_lifetime=None, ssl_compliance=None,
+            ldap_host=None, ldap_port=None, isam_domain=None, ldap_dn=None,
+            ldap_suffix=None, ldap_ssl_db=None, ldap_ssl_label=None,
+            isam_host=None, isam_port=None):
+        """
+        Configure the reverse proxy runtime component, including the policy server and user registry.
 
-    def list_relying_parties(self):
-        '''
-        Get a list of all the configured FIDO2 relying parties.
+        Args:
+            ps_mode (:obj:`str`): The mode for the policy server. Valid values are local and remote.
+            user_registry (:obj:`str`): The type of user registry to be configured against. Valid values are local, ldap
+            admin_password (:obj:`str`): The security administrator's password (also known as sec_master).
+            ldap_password (:obj:`str`, optional): The password for the DN. If the ps_mode is local and the user registry is remote, this field is required.
+            admin_cert_lifetime (:obj:`str`, optional): The lifetime in days for the SSL server certificate. If ps_mode is local, this field is required.
+            ssl_compliance (:obj:`str`): Specifies whether SSL is compliant with any additional computer security standard.
+            ldap_host (:obj:`str`): The name of the LDAP server.
+            ldap_port (:obj:`str`): The port to be used when the system communicates with the LDAP server.
+            isam_domain (:obj:`str`): The Security Verify Access domain name. This field is required unless ps_mode is local and user_registry is local.
+            ldap_dn (:obj:`str`): The DN that is used when the system contacts the user registry.
+            ldap_suffix (:obj:`str`): The LDAP suffix that is used to hold the Security Verify Access secAuthority data.
+            ldap_ssl_db (:obj:`str`): The key file (no path information is required) that contains the certificate that 
+                                is used to communicate with the user registry. If no keyfile is provided, the SSL is 
+                                not used when the system communicates with the user registry.
+            ldap_ssl_label (:obj:`str`, optional): The label of the SSL certificate that is used when the system 
+                                communicates with the user registry. This option is only valid if the ldap_ssl_db option 
+                                is provided.
+            isam_host (:obj:`str`): The name of the host that hosts the Security Verify Access policy server.
+            isam_port (:obj:`str`, optional): The port over which communication with the Security Verify Access policy 
+                                server takes place. If ps_mode is remote, this field is required.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the relying parties are returned as JSON and can be accessed from
-            the response.json attribute
+        """
+        data = DataObject()
+        data.add_value_string("ps_mode", ps_mode)
+        data.add_value_string("user_registry", user_registry)
+        data.add_value_string("admin_cert_lifetime", admin_cert_lifetime)
+        data.add_value_string("ssl_compliance", ssl_compliance)
+        data.add_value_string("admin_pwd", admin_password)
+        data.add_value_string("ldap_pwd", ldap_password)
+        data.add_value_string("ldap_host", ldap_host)
+        data.add_value_string("domain", isam_domain)
+        data.add_value_string("ldap_dn", ldap_dn)
+        data.add_value_string("ldap_suffix", ldap_suffix)
+        if ldap_ssl_db is not None:
+            data.add_value_string("ldap_ssl_db", ldap_ssl_db if ldap_ssl_db.endswith(".kdb") else ldap_ssl_db+".kdb")
+            data.add_value_string("usessl", "on")
+        data.add_value_string("ldap_ssl_label", ldap_ssl_label)
+        data.add_value_string("isam_host", isam_host)
+        data.add_value("ldap_port", ldap_port)
+        data.add_value("isam_port", isam_port)
+        response = self.client.post_json(RUNTIME_COMPONENT, data.data)
 
-        '''
-        response = self.client.get_json(FIDO2_RELYING_PARTIES)
         response.success = response.status_code == 200
-
         return response
 
 
-    def get_relying_party(self, _id):
-        '''
-        Get the configuration of a FIDO2 relying party.
-
-        Args:
-            _id (:obj:`str`): The id of the FIDO2 relying party.
+    def get_status(self):
+        """
+        Get the status of the runtime server.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the relying party is returned as JSON and can be accessed from
+            If the request is successful the rate limiting policy is returned as JSON and can be accessed from
             the response.json attribute
 
-        '''
-        endpoint = "{}/{}".format(FIDO2_RELYING_PARTIES, _id)
-        response = self.client.get_json(endpoint)
+        """
+        response = self.client.get_json(RUNTIME_COMPONENT)
         response.success = response.status_code == 200
-
         return response
 
 
-    def create_relying_party(self, name=None, rp_id=None, origins=None, metadata_set=None, metadata_soft_fail=True,
-            mediator_mapping_rule_id=None, attestation_statement_types=None, attestation_statement_formats=None,
-            attestation_public_key_algorithms=None, attestation_android_safetynet_max_age=None,
-            attestation_android_safetynet_clock_skew=None, relying_party_impersonation_group="adminGroup"):
-        '''
-        Create a FIDO2 relying party.
+    def update_embedded_ldap_password(self, password):
+        """
+        Change the admin password on the embedded LDAP server.
 
         Args:
-            name (:obj:`str`): Name of relying party.
-            rp_id (:obj:`str`): The domain that the relying aprty acts for This shold be a valid domain name.
-            origins (:obj:`list` of :obj:`str`): List of allowed origns for he relying party. 
-                                    Origins must be a valid URI and https origins should be a subdomain of the ``rp_id``.
-            metadata_set (:obj:`list` of :obj:`str`): List of document id's to included as metadata.
-            metadata_soft_fail (bool): Flag o indicate if a registration attempt should fail if metadata cannot be found.
-            mediator_mapping_rule_id (:obj:`str`): The id of the FIDO JavaScript mapping rule to use as a mediator.
-            attestation_statement_types (:obj:`list` of :obj:`str`): List of allowed attestation types.
-            attestation_statement_formats (:obj:`list` of :obj:`str`): List of allowed attestation formats.
-            attestation_public_key_algorithms (:obj:`list` of :obj:`str`): List of supported cryptographic signing algorithms.
-            attestation_android_safetynet_max_age (int): Length of time that an "android-safetynet" attestation is valid for.
-            attestation_android_safetynet_clock_skew (int): Clock skew allowed for "android-safetynet" attestations.
-            relying_party_impersonation_group (:obj:`str`): Group which permits users to perform FIDO flows on behalf of another user.
+            password (:obj:`str`): The new administrator password.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the id of the created obligation can be acess from the 
-            response.id_from_location attribute
-
-        '''
+        """
         data = DataObject()
-        data.add_value("name", name)
-        data.add_value("rpId", rp_id)
-
-        fidoServerOptions = DataObject()
-        fidoServerOptions.add_value_not_empty("origins", origins)
-        fidoServerOptions.add_value("metadataSet", metadata_set)
-        fidoServerOptions.add_value("metadataSoftFail", metadata_soft_fail)
-        fidoServerOptions.add_value("mediatorMappingRuleId", mediator_mapping_rule_id)
-
-        attestation = DataObject()
-        attestation.add_value("statementTypes", attestation_statement_types)
-        attestation.add_value("statementFormats", attestation_statement_formats)
-        attestation.add_value("publicKeyAlgorithms", attestation_public_key_algorithms)
-        fidoServerOptions.add_value("attestation", attestation.data)
-
-        attestationAndroidSafetyNetOptions = DataObject()
-        attestationAndroidSafetyNetOptions.add_value("attestationMaxAge", attestation_android_safetynet_max_age)
-        attestationAndroidSafetyNetOptions.add_value("clockSkew", attestation_android_safetynet_clock_skew)
-        fidoServerOptions.add_value("android-safetynet", attestationAndroidSafetyNetOptions.data)
-
-        data.add_value("fidoServerOptions", fidoServerOptions.data)
-
-        relyingPartyOptions = DataObject()
-        relyingPartyOptions.add_value("impersonationGroup", relying_party_impersonation_group)
-        data.add_value("relyingPartyOptions", relyingPartyOptions.data)
-
-        response = self.client.post_json(FIDO2_RELYING_PARTIES, data.data)
-        response.success = response.status_code == 201
+        data.add_value_string("password", password)
 
+        response = self.client.post_json(EMBEDDED_LDAP_PASSWORD, data.data)
+        response.success = response.status_code == 200
         return response
 
 
-    def update_relying_party(self, id, name=None, rp_id=None, origins=None, metadata_set=None, metadata_soft_fail=True,
-            mediator_mapping_rule_id=None, attestation_statement_types=None, attestation_statement_formats=None,
-            attestation_public_key_algorithms=None, attestation_android_safety_net_max_age=None,
-            attestation_android_safetynet_clock_skew=None, relying_party_impersonation_group="adminGroup"):
-        '''
-        Update a FIDO2 relying party.
+    def create_federated_user_registry(self, _id, hostname=None, port=None, bind_dn=None, bind_pwd=None, 
+            ignore_if_down=None, use_ssl=None, client_cert_label=None, suffix=[]):
+        """
+        Add a federated LDAP server to the user registry for use as basic or full Verify Access users.
 
         Args:
-            name (:obj:`str`): Name of relying party.
-            rp_id (:obj:`str`): The domain that the relying aprty acts for This shold be a valid domain name.
-            origins (:obj:`list` of :obj:`str`): List of allowed origns for he relying party. 
-                                    Origins must be a valid URI and https origins should be a subdomain of the ``rp_id``.
-            metadata_set (:obj:`list` of :obj:`str`): List of document id's to included as metadata.
-            metadata_soft_fail (bool): Flag o indicate if a registration attempt should fail if metadata cannot be found.
-            mediator_mapping_rule_id (:obj:`str`): The id of the FIDO JavaScript mapping rule to use as a mediator.
-            attestation_statement_types (:obj:`list` of :obj:`str`): List of allowed attestation types.
-            attestation_statement_formats (:obj:`list` of :obj:`str`): List of allowed attestation formats.
-            attestation_public_key_algorithms (:obj:`list` of :obj:`str`): List of supported cryptographic signing algorithms.
-            attestation_android_safetynet_max_age (int): Length of time that an "android-safetynet" attestation is valid for.
-            attestation_android_safetynet_clock_skew (int): Clock skew allowed for "android-safetynet" attestations.
-            relying_party_impersonation_group (:obj:`str`): Group which permits users to perform FIDO flows on behalf of another user.
+            _id (:obj:`str`): The identifier of the federated LDAP server.
+            hostname (:obj:`str`): The hostname or address of the LDAP server.
+            port (:obj:`str`): The port that the LSAP server is listening on.
+            bind_dn (:obj:`str`): The Distinguished Name to bind to the LDAP server as to perform admin operations.
+            bind_pwd (:obj:`str`): The secret to authenticate as the ``bind_dn`` user.
+            ignore_if_down (`bool`, optional): Whether the server will continue to operate using the other configured 
+                                               federated registries if this user registry is unavailable.
+            use_ssl (`bool`): Whether or not SSL is used to communicate with the directory.
+            client_cert_label (:obj:`str`, optional): The client certificate to use when communicating with the 
+                                                      directory using SSL. Only valid if ``use_ssl`` is true.
+            suffix (:obj:`list` of :obj:`dict`): List of suffixes to use, eg::
+
+                                                                                [
+                                                                                 {"id": "dc=ibm,dc=com"},
+                                                                                 {"id": "o=ibm"}
+                                                                                ]
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-        '''
+        """
         data = DataObject()
-        data.add_value("id", id)
-        data.add_value("name", name)
-        data.add_value("rpId", rp_id)
-
-        fidoServerOptions = DataObject()
-        fidoServerOptions.add_value_not_empty("origins", origins)
-        fidoServerOptions.add_value("metadataSet", metadata_set)
-        fidoServerOptions.add_value("metadataSoftFail", metadata_soft_fail)
-        fidoServerOptions.add_value("mediatorMappingRuleId", mediator_mapping_rule_id)
-
-        attestation = DataObject()
-        attestation.add_value("statementTypes", attestation_statement_types)
-        attestation.add_value("statementFormats", attestation_statement_formats)
-        attestation.add_value("publicKeyAlgorithms", attestation_public_key_algorithms)
-        attestation.add_value("publicKeyAlgorithms", attestation_public_key_algorithms)
-        fidoServerOptions.add_value("attestation", attestation.data)
-
-        attestationAndroidSafetyNetOptions = DataObject()
-        attestationAndroidSafetyNetOptions.add_value("attestationMaxAge", attestation_android_safetynet_max_age)
-        attestationAndroidSafetyNetOptions.add_value("clockSkew", attestation_android_safetynet_clock_skew)
-        fidoServerOptions.add_value("android-safetynet", attestationAndroidSafetyNetOptions.data)
-
-        data.add_value("fidoServerOptions", fidoServerOptions.data)
-
-        relyingPartyOptions = DataObject()
-        relyingPartyOptions.add_value("impersonationGroup", relying_party_impersonation_group)
-        data.add_value("relyingPartyOptions", relyingPartyOptions.data)
-
-        endpoint = "%s/%s" % (FIDO2_RELYING_PARTIES, id)
+        data.add_value_string("id", _id)
+        data.add_value_string("hostname", hostname)
+        data.add_value("port", port)
+        data.add_value_string("bind_dn", bind_dn)
+        data.add_value_string("bind_pwd", bind_pwd)
+        data.add_value_boolean("ignore_if_down", ignore_if_down)
+        data.add_value_boolean("use_ssl", use_ssl)
+        data.add_value_string("client_cert_label", client_cert_label)
+        data.add_value("suffix", suffix)
 
-        response = self.client.put_json(endpoint, data.data)
-        response.success = response.status_code == 204
+        response = self.client.post_json(FEDERATED_DIRECTORIES + "/v1", data.data)
+        response.success = response.status_code == 200
 
         return response
 
 
-    def list_metadata(self):
-        '''
-        Get a list of all the configured metadata documents.
+    def delete_federated_user_registry(self, _id):
+        """
+        Remove a configured federated user registry
+
+        Args:
+            _id (:obj:`str`): The identifier of the federated user registry to remove.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the metadata documents are returned as JSON and can be accessed from
-            the response.json attribute
+        """
+        url = FEDERATED_DIRECTORIES + "/{}/v1".format(_id)
+        response = self.client.delete_json(url)
+        response.success = response.status_code == 204
 
-        '''
-        endpoint = FIDO2_METADATA
+        return response
 
-        response = self.client.get_json(endpoint)
-        response.success = response.status_code == 200
 
-        return response
+    def create_configuration_file_entry(self, resource=None, stanza=None, entries=None):
+        """
+        Create a new stanza or entry in a runtime component configuration file.
 
+        Args:
+            resource (:obj:`str`): The configuration file to modify. For example: ldap.conf, pd.conf, instance.conf
+            stanza (:obj:`str`): The name of the resource stanza entry.
+            entries (:obj:`list` of :obj:`list`, optional): Entry name and value in the format of key value pairs. If 
+                                                            this property is not supplied then the stanza is created
+                                                            instead. Format of list is::
 
-    def get_metadata(self, _id):
-        '''
-        Get a configured metadata documents.
+                                                                                        [
+                                                                                          ["entryName", "entryValue"],
+                                                                                          ["anotherName", "theValue"]
+                                                                                        ]
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the metadata document is returned as JSON and can be accessed from
-            the response.json attribute
-
-        '''
-        endpoint = "{}/{}".format(FIDO2_METADATA, _id)
+        """
+        url = RUNTIME_STANZA_FILE_BASE + "/{}/configuration/stanza/{}".format(resource, stanza)
+        data = DataObject()
+        if entries:
+            data.add_value("entries", entrites)
+            url += "/entry_name"
 
-        response = self.client.get_json(endpoint)
+        response = self.client.post_json(url, data.data)
         response.success = response.status_code == 200
 
         return response
 
 
-    def create_metadata(self, filename=None):
-        '''
-        Create a metadata document from a file.
+    def update_configuration_file_entry(self, resource=None, stanza=None, entries=None):
+        """
+        Update a stanza entry in a runtime component configuration file.
 
         Args:
-            filename (:obj:`str`): Absolute path to a FIDO2 Metadata document
-
-        Returns:
-            :obj:`~requests.Response`: The response from verify access. 
-
-            Success can be checked by examining the response.success boolean attribute
-
-            If the request is successful the id of the created metadata can be acess from the 
-            response.id_from_location attribute
-
-        '''
-        response = Response()
-        try:
-            with open(filename, 'rb') as content:
-                data = DataObject()
-                data.add_value_string("filename", ntpath.basename(filename))
-                data.add_value_string("contents", content.read().decode('utf-8'))
-
-                endpoint = FIDO2_METADATA
-
-                response = self.client.post_json(endpoint, data.data)
-                response.success = response.status_code == 201
-
-        except IOError as e:
-            logger.error(e)
-            response.success = False
+            resource (:obj:`str`): The configuration file to modify. For example: ldap.conf, pd.conf, instance.conf
+            stanza (:obj:`str`): The name of the resource stanza entry.
+            entries (:obj:`list` of :obj:`list`): Entry name and value in the format of key value pairs. If 
+                                                            this property is not supplied then the stanza is created
+                                                            instead. Format of list is::
 
-        return response
-
-    def update_metadata(self, id, filename=None):
-        '''
-        Update an existing metadata document from a file.
-
-        Args:
-            id (:obj:`str`): The id of the FIDO2 metadata docuemtn to be updated.
-            filename (:obj:`str`): Absolute path to a FIDO2 Metadata document.
+                                                                                        [
+                                                                                          ["entryName", "entryValue"],
+                                                                                          ["anotherName", "theValue"]
+                                                                                        ]
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
-
-        '''
-        response = Response()
-        try:
-            with open(filename, 'rb') as content:
-                files = {"file": content}
-
-                endpoint = ("%s/%s/file" % (FIDO2_METADATA, id))
-
-                response = self.client.post_file(endpoint, accept_type="application/json,text/html,application/*", files=files)
-                response.success = response.status_code == 200
-
-        except IOError as e:
-            logger.error(e)
-            response.success = False
+        """
+        url = RUNTIME_STANZA_FILE_BASE + "/{}/configuration/stanza/{}/entry_name".format(resource, stanza)
+        data = DataObject()
+        data.add_value("entries", entrites)
+        response = self.client.put_json(url, data.data)
+        response.success = response.status_code == 200
 
         return response
 
-    def delete_metadata(self, id):
-        '''
-        Remove an existing metadata documetn from the store
-
-        Args:
-            id (:obj:`str`): The id of the metadata document to be removed.
-
-        Returns
-            :obj:`~requests.Response`: The response from verify access. 
-
-            Success can be checked by examining the response.success boolean attribute
-
-        '''
-        endpoint = ("%s/%s/file" % (FIDO2_METADATA, id))
-
-        response = self.client.delete_json(endpoint)
-        response.success = response.status_code == 204
 
-    def create_mediator(self, name=None, filename=None):
-        '''
-        Create a FDIO2 mediator JavaScript mapping rule.
+    def delete_configuration_file_entry(self, resource=None, stanza=None, entry=None, value=None):
+        """
+        Delete a stanza or entry in a runtime component configuration file.
 
         Args:
-            name (:obj:`str`): The name of the mapping rule to be created.
-            filename (:obj:`str`): The contents of the mapping rule.
+            resource (:obj:`str`): The configuration file to modify. For example: ldap.conf, pd.conf, instance.conf
+            stanza (:obj:`str`): The name of the resource stanza entry.
+            entry (:obj:`str`, optional): The entry name to be removed. If not supplied then the entire stanza is removed.
+            value (:obj:`str`, optional): The entry value to be removed. This must be set if the ``entry`` property is
+                                          supplied.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
+        """
+        response = None
+        url = RUNTIME_STANZA_FILE_BASE + "/{}/configuration/stanza/{}".format(resource, stanza)
+        if entry:
+            url += "/entry_name/{}/value/{}".format(entry, value)
 
-            If the request is successful the id of the created mediator can be acess from the 
-            response.id_from_location attribute
-        '''
-        response = Response()
-        try:
-            with open(filename, 'rb') as content:
-                data = DataObject()
-                data.add_value_string("filename", ntpath.basename(filename))
-                data.add_value_string("content", content.read().decode('utf-8'))
-                data.add_value_string("type", "FIDO2")
-                data.add_value_string("name", name)
-
-                response = self.client.post_json(FIDO2_MEDIATOR, data.data)
-                response.success = response.status_code == 201
-
-        except IOError as e:
-            logger.error(e)
-            response.success = False
+        response = self.client.delete_json(url)
+        response.success = response.status_code == 200
 
         return response
 
-    def update_mediator(self, id, filename=None):
-        '''
-        Update an exisiting mediator mapping rule with new contents
+
+class RuntimeComponent10000(RuntimeComponent):
+    
+    def configure(
+            self, ps_mode=None, user_registry=None, admin_password=None,
+            ldap_password=None, admin_cert_lifetime=None, ssl_compliance=None,
+            ldap_host=None, ldap_port=None, isam_domain=None, ldap_dn=None,
+            ldap_suffix=None, ldap_ssl_db=None, ldap_ssl_label=None,
+            isam_host=None, isam_port=None, clean_ldap=None):
+        """
+        Configure the reverse proxy runtime component, including the policy server and user registry.
 
         Args:
-            id (:obj:`str`): The id of the existing mapping rule.
-            filename (:obj:`str`): Absolute path to the file containing the new mapping rule contents.
+            ps_mode (:obj:`str`): The mode for the policy server. Valid values are local and remote.
+            user_registry (:obj:`str`): The type of user registry to be configured against. Valid values are local, ldap
+            admin_password (:obj:`str`): The security administrator's password (also known as sec_master).
+            ldap_password (:obj:`str`, optional): The password for the DN. If the ps_mode is local and the user registry is remote, this field is required.
+            admin_cert_lifetime (:obj:`str`, optional): The lifetime in days for the SSL server certificate. If ps_mode is local, this field is required.
+            ssl_compliance (:obj:`str`): Specifies whether SSL is compliant with any additional computer security standard.
+            ldap_host (:obj:`str`): The name of the LDAP server.
+            ldap_port (:obj:`str`): The port to be used when the system communicates with the LDAP server.
+            isam_domain (:obj:`str`): The Security Verify Access domain name. This field is required unless ps_mode is local and user_registry is local.
+            ldap_dn (:obj:`str`): The DN that is used when the system contacts the user registry.
+            ldap_suffix (:obj:`str`): The LDAP suffix that is used to hold the Security Verify Access secAuthority data.
+            ldap_ssl_db (:obj:`str`): The key file (no path information is required) that contains the certificate that 
+                                is used to communicate with the user registry. If no keyfile is provided, the SSL is 
+                                not used when the system communicates with the user registry.
+            ldap_ssl_label (:obj:`str`, optional): The label of the SSL certificate that is used when the system 
+                                communicates with the user registry. This option is only valid if the ldap_ssl_db option 
+                                is provided.
+            isam_host (:obj:`str`): The name of the host that hosts the Security Verify Access policy server.
+            isam_port (:obj:`str`, optional): The port over which communication with the Security Verify Access policy 
+                                server takes place. If ps_mode is remote, this field is required.
+            clean_ldap (:obj:`str`, optional): Whether any existing data within the LDAP server should be cleaned prior 
+                                to the configuration. Only valid if the user registry is local.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-        '''
-        response = Response()
-        try:
-            with open(filename, 'rb') as content:
-                data = DataObject()
-                data.add_value_string("content", content.read().decode('utf-8'))
-
-                endpoint = ("%s/%s" % (FIDO2_MEDIATOR, id))
-
-                response = self.client.put_json(endpoint, data.data)
-                response.success = response.status_code == 204
-
-        except IOError as e:
-            logger.error(e)
-            response.success = False
-
-        return response
-
-    def get_mediator(self, id):
-        '''
-        Get the contents of a configured mediator.
-
-        Agrs:
-            id (:obj:`str`): The id of the mediator to return.
-
-        Returns:
-            :obj:`~requests.Response`: The response from verify access. 
-
-            Success can be checked by examining the response.success boolean attribute
+        """
+        data = DataObject()
+        data.add_value_string("ps_mode", ps_mode)
+        data.add_value_string("user_registry", user_registry)
+        data.add_value_string("admin_cert_lifetime", admin_cert_lifetime)
+        data.add_value_string("ssl_compliance", ssl_compliance)
+        data.add_value_string("admin_pwd", admin_password)
+        data.add_value_string("ldap_pwd", ldap_password)
+        data.add_value_string("ldap_host", ldap_host)
+        data.add_value_string("domain", isam_domain)
+        data.add_value_string("ldap_dn", ldap_dn)
+        data.add_value_string("ldap_suffix", ldap_suffix)
+        data.add_value_string("clean_ldap", clean_ldap)
+        if ldap_ssl_db is not None:
+            data.add_value_string("ldap_ssl_db", ldap_ssl_db if ldap_ssl_db.endswith(".kdb") else ldap_ssl_db+".kdb")
+            data.add_value_string("usessl", "on")
+        data.add_value_string("ldap_ssl_label", ldap_ssl_label)
+        data.add_value_string("isam_host", isam_host)
+        data.add_value("ldap_port", ldap_port)
+        data.add_value("isam_port", isam_port)
 
-            If the request is successful the mediator is returned as JSON and can be accessed from
-            the response.json attribute
+        logger.info(data.data)
+        response = self.client.post_json(RUNTIME_COMPONENT, data.data)
 
-        '''
-        endpoint = ("%s/%s" % (FIDO2_MEDIATOR, id))
-        response = self.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
-    def list_mediators(self):
-        '''
-        Get a list of all of the configured mediators.
-
-        Returns:
-            :obj:`~requests.Response`: The response from verify access. 
-
-            Success can be checked by examining the response.success boolean attribute
-
-            If the request is successful the metadata document is returned as JSON and can be accessed from
-            the response.json attribute
-
-        '''
-        response = self.client.get_json(FIDO2_MEDIATOR)
-        rsponse.success = response.status_code == 200
-
-        return response
-
 
-    def delete_mediator(self, id):
-        '''
-        Remove a configured mediator mapping rule.
+    def unconfigure(self, operation="unconfigure", ldap_dn=None, ldap_pwd=None, clean=False, force=False):
+        """
+        Unconfigure the runtime component. This is only possible if there are no WebSEAL reverse proxy instances configured.
 
         Args:
-            id (:obj:`str`): The id of the mediator mapping rule to be removed.
+            ldap_dn (:obj:`str`): The DN that is used when the system contacts the user registry.
+            ldap_password (:obj:`str`, optional): The password for the DN.
+            clean (`bool`, optional): Whether the unconfigure operation removes all Security Verify Access domain, user, and 
+                            group information.
+            force (`bool`, optional): This option is used to force the unconfiguration if it is failing.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-        '''
-        endpoint = ("%s/%s" % (FIDO2_MEDIATOR, id))
-        response = self.delete_json(endpoint)
-        response.success = response.status_code == 204
+        """
+        data = DataObject()
+        data.add_value_string("operation", operation)
+        data.add_value_string("ldap_dn", ldap_dn)
+        data.add_value_string("ldap_pwd", ldap_pwd)
+        data.add_value_string("clean", clean)
+        data.add_value_string("force", force)
+
+        response = self.client.post_json(UNCONFIGURE_RUNTIME_COMPONENT, data.data)
+
+        response.success = response.status_code == 200
 
         return response
```

### Comparing `pyisva-0.1.0/pyisva/core/access/fido2registrations.py` & `pyisva-0.2.0/pyisva/core/access/fido2registrations.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,95 +2,110 @@
 @copyright: IBM
 """
 import logging
 from pyisva.util.model import DataObject
 from pyisva.util.restclient import RESTClient
 
 
-"""
-Allows basic management of FIDO2 egistrations
-"""
 FIDO2_REGISTRATIONS="/iam/access/v8/fido2/registrations"
 FIDO2_USER_REGISTRATIONS="/iam/access/v8/fido2/registrations/username"
 FIDO2_CRED_ID_REGISTRATIONS="/iam/access/v8/fido2/registrations/credentialId"
 
 logger = logging.getLogger(__name__)
 
 
 class FIDO2Registrations(object):
 
     def __init__(self, base_url, username, password):
         super(FIDO2Registrations, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
+
     def list_registrations(self, username=None, credential_id=None):
         '''
         Get a list all of the known FIDO2 registrations.
 
         Args:
             username (:obj:`str`, optional): Specify a username to filter registrations by.
             credential_id (:obj:`str`): Specify a credential id to filter registrations by.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the FIDO2 registrations are returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         '''
         endpoint = FIDO2_REGISTRATIONS
         if username:
             endpoint = "{}/{}".format(FIDO2_USER_REGISTRATIONS, username)
         elif credential_id:
             endpoint = "{}/{}".format(FIDO2_REGISTRATIONS, credential_id)
         response = self.client.get_json(endpoint)
-        response.success = response.stauts_code == 200
+        response.success = response.status_code == 200
 
         return response
 
 
     def delete_registration_by_user(self, username=None):
         '''
         Remove all registrations associated with a username.
 
         Args:
-            username (:obj:`str`): The username to remove registratiosn for.
+            username (:obj:`str`): The username to remove registrations for.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
-
-            If the request is successful the FIDO2 registrations are returned as JSON and can be accessed from
-            the response.json attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "{}/{}".format(FIDO2_USER_REGISTRATIONS, username)
         response = self.client.delete_json(endpoint)
-        response.success = response.stauts_code == 200
+        response.success = response.status_code == 204
 
         return response
 
 
     def delete_registration_by_credential_id(self, credential_id=None):
         '''
-        Delete a registration associated with the specified credential id
+        Delete a registration associated with the specified credential id.
 
         Args:
-            credential_id (:obj:`str`): The credential id to be removed
+            credential_id (:obj:`str`): The credential id to be removed.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
-
-            If the request is successful the FIDO2 registrations are returned as JSON and can be accessed from
-            the response.json attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "{}/{}".format(FIDO2_CRED_ID_REGISTRATIONS, credential_id)
         response = self.client.delete_json(endpoint)
-        response.success = response.stauts_code == 200
+        response.success = response.status_code == 204
 
         return response
+
+
+    def get_registration(self, credential_id):
+        '''
+        Get a specific registration by credential id.
+
+        Args:
+            credential_id (:obj:`str`): The unique identifier for the authenticator.
+
+        Returns:
+            :obj:`~requests.Response`: The response from verify access. 
+
+            Success can be checked by examining the response.success boolean attribute.
+
+            If the request is successful the FIDO2 registration is returned as JSON and can be accessed from
+            the response.json attribute.
+
+        '''
+        endpoint = "{}/{}".format(FIDO2_REGISTRATIONS, credential_id)
+        response = self.client.delete_json(endpoint)
+        response.success = response.status_code == 204
+
+        return response
```

### Comparing `pyisva-0.1.0/pyisva/core/access/mappingrules.py` & `pyisva-0.2.0/pyisva/core/access/mappingrules.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,30 +16,31 @@
 
 class MappingRules(object):
 
     def __init__(self, base_url, username, password):
         super(MappingRules, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
+
     def create_rule(self, rule_name=None, category=None, content=None):
         '''
-        Create a JavaScript mapping rule from a file.
+        Create a JavaScript mapping rule.
 
         Args:
             rule_name (:obj:`str`): The name of the new mapping rule.
             category (:obj:`str`): Type of mapping rule to create.
             contents (:obj:`str`): The JavaScript content of the new mapping rule.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the id of the created obligation can be acess from the
-            response.id_from_location attribute
+            If the request is successful the id of the created mapping rule can be accessed from the
+            response.id_from_location attribute.
 
         '''
         data = DataObject()
         data.add_value_string("fileName", ("%s_%s.js" % (category, rule_name)))
         data.add_value_string("category", category)
         data.add_value_string("name", rule_name)
         data.add_value_string("content", content)
@@ -52,25 +53,25 @@
 
 
     def import_rule(self, rule_name=None, category=None, file_name=None):
         '''
         Create a JavaScript mapping rule from a file.
 
         Args:
-            file_name (:obj:`str`, optional): The file to be uploaded as a new mapping rule.
+            rule_name (:obj:`str`): The name of the rule to be created.
             category (:obj:`str`): Type of mapping rule to create.
-            contents (:obj:`str`): The JavaScript content of the new mapping rule.
+            file_name (:obj:`str`): The absolute path to the JavaScript mapping rule.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the id of the created obligation can be acess from the
-            response.id_from_location attribute
+            If the request is successful the id of the created obligation can be accessed from the
+            response.id_from_location attribute.
 
         '''
         response = Response()
         try:
             data = DataObject()
             data.add_value_string("fileName", ("%s_%s.js" % (category, rule_name)))
             data.add_value_string("category", category)
@@ -87,27 +88,27 @@
             response.success = False
 
         return response
 
 
     def update_rule(self, rule_id, file_name=None, content=None):
         '''
-        Update an existing JavaScript mappign rule with new contents
+        Update an existing JavaScript mapping rule with new contents
 
         Args:
             rule_id (:obj:`str`): The id of the rule to be updated.
             file_name (:obj:`str`, optional): Absolute path to file containing new mapping rule. Must specify either
                                             file_name or content.
-            content (:obj:`str`, optional): The javascript code to replace current mappign rule. Must specify either
+            content (:obj:`str`, optional): The javascript code to replace current mapping rule. Must specify either
                                             file_name or content.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         response = Response()
         try:
             data = DataObject()
             if content == None:
                 with open(file_name, 'rb') as content:
@@ -124,53 +125,56 @@
         except IOError as e:
             logger.error(e)
             response.success = False
 
         return response
 
 
-    def get_rule(self, rule_id=None, filter=None):
+    def get_rule(self, rule_id=None,):
         '''
-        Get a mapping rule based on a rule id or filter.
+        Get a mapping rule based on a rule id.
 
         Args:
             rule_id (:obj:`str`, optional): The id of the mapping rule to return.
-            filter (:obj:`str`, optional): Filter to apply to returned rules. eg. "name startswith Test"
+
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the mapping rules are returned as JSON and can be accessed from
-            the response.json attribute
+            If the request is successful the mapping rule is returned as JSON and can be accessed from
+            the response.json attribute.
 
         '''
-        endpoint = ("%s/%s?filter=%s" % (MAPPING_RULES, rule_id if rule_id != None else "", filter))
-
+        endpoint = "{}/{}".format(MAPPING_RULES, rule_id)
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
 
-    def get_rules(self):
+    def list_rules(self, filter=None):
         '''
-        Return list of all mapping rules.
+        Return a list of all mapping rules.
+
+        Args:
+            filter (:obj:`str`, optional): Filter to apply to returned rules. eg. "name startswith Test".
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
             If the request is successful the mapping rules are returned as JSON and can be accessed from
             the response.json attribute
 
         '''
-        response = self.client.get_json(MAPPING_RULES)
+        endpoint = ("%s%s" % (MAPPING_RULES, "?filter=" + filter if isinstance(filter, str) else ""))
+        response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
 
     def delete_rule(self, rule_id=None):
         '''
@@ -178,15 +182,15 @@
 
         Args:
             rule_id (:obj:`str`): The id of the mapping rule to be removed.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
-        endpoint = MAPPING_RULES + "/{}".format(rule_id)
+        endpoint = "{}/{}".format(MAPPING_RULES, rule_id)
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
-        return response
+        return response
```

### Comparing `pyisva-0.1.0/pyisva/core/access/mmfaconfig.py` & `pyisva-0.2.0/pyisva/core/access/mmfaconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,23 @@
 
 class MMFAConfig(object):
 
     def __init__(self, base_url, username, password):
         super(MMFAConfig, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
+
     def update(self, client_id=None, hostname=None, junction=None, options=None,
             port=None):
         '''
-        Update the mobile multifactor authentication configuration.
+        Update the mobile multi-factor authentication (MMFA) configuration.
 
         Args:
-            client_id (:obj:`str`): The id of the OIDC client to use.
-            hostname (:obj:`str`): The hostname of the webseal instance configured for MMFA.
+            client_id (:obj:`str`): The id of the Open-Id Connect client to use.
+            hostname (:obj:`str`): The hostname of the WebSEAL instance configured for MMFA.
             junction (:obj:`astr`): The junction prefix configured for MMFA.
             options (:obj:`str`): A list of configurable key-value pairs to be presented in the QR code.
             port (:obj:`str`): The port the MMFA endpoint is listening on.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
@@ -51,35 +52,36 @@
 
 
 class MMFAConfig9021(MMFAConfig):
 
     def __init__(self, base_url, username, password):
         super(MMFAConfig9021, self).__init__(base_url, username, password)
 
+
     def update(self, client_id=None, hostname=None, junction=None, port=None,
             details_url=None, enrollment_endpoint=None,
             hotp_shared_secret_endpoint=None, totp_shared_secret_endpoint=None,
             token_endpoint=None, authntrxn_endpoint=None,
             mobile_endpoint_prefix=None, qrlogin_endpoint=None,
-            discovery_mechanisms=None, options=None):
+            discovery_mechanisms=[], options=None):
         '''
-        Update the mobile multifactor authentication configuration.
+        Update the mobile multi-factor authentication (MMFA) configuration.
 
         Args:
             client_id (:obj:`str`): The id of the OIDC client to use.
-            hostname (:obj:`str`, optional): The hosname of the WebSEAL instance configured for MMFA.
+            hostname (:obj:`str`, optional): The hostname of the WebSEAL instance configured for MMFA.
             junction (:obj:`str`, optional): The junction prefix configured for MMFA.
             port (int, optional): The port the MMFA endpoint is listening on.
             hotp_shared_secret_endpoint (:obj:`str`): The HOTP shared secret endpoint returned from the discovery endpoint.
             totp_shared_secret_endpoint (:obj:`str`): The TOTP shared secret endpoint returned from the discovery endpoint.
             token_endpoint (:obj:`str`): The OAuth token endpoint returned from the discovery endpoint.
             authntrxn_endpoint (:obj:`str`): The SCIM Transaction endpoint returned from the discovery endpoint.
-            mobile_endpoint_prefix (:obj:`str`): The prefix of the runtime endpoint that is constructed and saved as the requestUrl of a transaction. 
+            mobile_endpoint_prefix (:obj:`str`): The prefix of the runtime endpoint that is constructed and saved as the request URL of a transaction. 
             qrlogin_endpoint (:obj:`str`): The QR Code login endpoint returned from the discovery endpoint.
-            discovery_mechanisms (:obj:`str`): A list of authentication mechanism URIs to be included in the discovery endpoint response.
+            discovery_mechanisms (:obj:`list` of :obj:`str`): A list of authentication mechanism URIs to be included in the discovery endpoint response.
             options (:obj:`str`): A list of configurable key-value pairs to be presented in the QR code.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
@@ -91,15 +93,15 @@
             "hotp_shared_secret_endpoint",hotp_shared_secret_endpoint)
         endpoints.add_value_string(
             "totp_shared_secret_endpoint",totp_shared_secret_endpoint)
         endpoints.add_value_string("token_endpoint", token_endpoint)
         endpoints.add_value_string("authntrxn_endpoint", authntrxn_endpoint)
         endpoints.add_value_string(
             "mobile_endpoint_prefix", mobile_endpoint_prefix)
-        endpoints.add_value_not_empty("qrlogin_endpoint", qrlogin_endpoint)
+        endpoints.add_value_string("qrlogin_endpoint", qrlogin_endpoint)
 
         data = DataObject()
         data.add_value_string("client_id", client_id)
         data.add_value_string("hostname", hostname)
         data.add_value_string("junction", junction)
         data.add_value_string("options", options)
         data.add_value("port", port)
@@ -107,21 +109,22 @@
         data.add_value_not_empty("discovery_mechanisms", discovery_mechanisms)
 
         response = self.client.post_json(MMFA_CONFIG, data.data)
         response.success = response.status_code == 204
 
         return response
 
+
     def delete(self):
         '''
-        Delete the mobile multifactor authentication configuration.
+        Delete the mobile multi-factor authentication configuration.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
         '''
         response = self.client.delete_json(MMFA_CONFIG)
         response.success = response.status_code == 204
 
-        return response
+        return response
```

### Comparing `pyisva-0.1.0/pyisva/core/access/pushnotification.py` & `pyisva-0.2.0/pyisva/core/access/pushnotification.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,35 +15,36 @@
 
 class PushNotification(object):
 
     def __init__(self, base_url, username, password):
         super(PushNotification, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
-    def create(self, app_id=None, platform=None, provider_address=None,
+
+    def create_provider(self, app_id=None, platform=None, provider_address=None,
             apple_key_store=None, apple_key_label=None,
             firebase_server_key=None):
         '''
         Create a push notification provider.
 
         Args:
             app_id (:obj:`str`): The application identifier associated with the registration.
             platform (:obj:`str`): The platform the registration is for.
             provider_address (:obj:`str`): The "host:port" address of the push notification service.
-            apple_key_store (:obj:`str`, optinal): The key store database containing the APNS certificate.
+            apple_key_store (:obj:`str`, optional): The key store database containing the APNS certificate.
             apple_key_label (:obj:`str`, optional) The key label of the imported APNS certificate.
             firebase_server_key (:obj:`str`): The server key for access to the Firebase push notification service.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the push notification provider uuid is returned as JSON and can be accessed from
-            the response.json attribute
+            If the request is successful the push notification provider id is returned as JSON and can be accessed from
+            the response.json attribute.
 
         '''
         apple = DataObject()
         apple.add_value_string("key_store", apple_key_store)
         apple.add_value_string("key_label", apple_key_label)
         if apple.data:
             apple.add_value_string("provider_address", provider_address)
@@ -69,45 +70,65 @@
 
 
 class PushNotification9021(PushNotification):
 
     def __init__(self, base_url, username, password):
         super(PushNotification9021, self).__init__(base_url, username, password)
 
-    def list_registrations(self):
+    def list_providers(self):
         '''
-        List the configured push notification service proviers.
+        List the configured push notification service providers.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the push notification providers are returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         '''
         response = self.client.get_json(PUSH_NOTIFICATION)
         response.success = response.status_code == 200
 
         return response
 
+    def get_provider(self, pnr_id):
+        '''
+        Get a specific push notification provider.
 
-    def create(self, app_id=None, platform=None, provider_address=None,
-            apple_key_store=None, apple_key_label=None,
-            firebase_server_key=None, imc_client_id=None,
-            imc_client_secret=None, imc_refresh_token=None, imc_app_key=None):
+        Args:
+            pnr_id (:obj:`str`): The unique identifier for the push notification resource.
+        
+        Returns:
+            :obj:`~requests.Response`: The response from verify access. 
+
+            Success can be checked by examining the response.success boolean attribute.
+
+            If the request is successful the push notification provider is returned as JSON and can be accessed from
+            the response.json attribute.
+        
+        '''
+        endpoint = '{}/{}'.format(PUSH_NOTIFICATION, pnr_id)
+        response = self.client.get_json(endpoint)
+        response.success = response.status_code == 200
+
+        return response
+
+
+    def create_provider(self, app_id=None, platform=None, provider_address=None, apple_key_store=None, apple_key_label=None,
+            firebase_server_key=None, imc_client_id=None, imc_client_secret=None, imc_refresh_token=None, imc_app_key=None):
         '''
         Create a push notification provider.
 
         Args:
             app_id (:obj:`str`): The application identifier associated with the registration.
             platform (:obj:`str`): The platform the registration is for.
             provider_address (:obj:`str`): The "host:port" address of the push notification service.
-            apple_key_store (:obj:`str`, optinal): The key store database containing the APNS certificate.
+            apple_key_store (:obj:`str`, optional): The key store database containing the APNS certificate.
             apple_key_label (:obj:`str`, optional) The key label of the imported APNS certificate.
             firebase_server_key (:obj:`str`): The server key for access to the Firebase push notification service.
             imc_client_id (:obj:`str`, optional): The IBM Marketing Cloud issued Oauth client ID.
             imc_client_secret (:obj:`str`, optional): The IBM Marketing Cloud issued Oauth client secret.
             imc_refresh_token (:obj:`str`, optional): The IBM Marketing Cloud issued Oauth refresh token.
             imc_app_key (:obj:`str`, optional): The app key issued by IBM Marketing Cloud for the associated application.
 
@@ -149,7 +170,95 @@
         data.add_value_string("platform", platform)
         data.add_value_not_empty("provider", provider.data)
 
         response = self.client.post_json(PUSH_NOTIFICATION, data.data)
         response.success = response.status_code == 200
 
         return response
+
+
+    def update_provider(self, pnr_id, app_id=None, platform=None, provider_address=None,
+            apple_key_store=None, apple_key_label=None,
+            firebase_server_key=None, imc_client_id=None,
+            imc_client_secret=None, imc_refresh_token=None, imc_app_key=None):
+        '''
+        Update an existing a push notification provider.
+
+        Args:
+            pnr_id (:obj:`str`): The unique identifier for the push notification resource.
+            app_id (:obj:`str`): The application identifier associated with the registration.
+            platform (:obj:`str`): The platform the registration is for.
+            provider_address (:obj:`str`): The "host:port" address of the push notification service.
+            apple_key_store (:obj:`str`, optional): The key store database containing the APNS certificate.
+            apple_key_label (:obj:`str`, optional) The key label of the imported APNS certificate.
+            firebase_server_key (:obj:`str`): The server key for access to the Firebase push notification service.
+            imc_client_id (:obj:`str`, optional): The IBM Marketing Cloud issued Oauth client ID.
+            imc_client_secret (:obj:`str`, optional): The IBM Marketing Cloud issued Oauth client secret.
+            imc_refresh_token (:obj:`str`, optional): The IBM Marketing Cloud issued Oauth refresh token.
+            imc_app_key (:obj:`str`, optional): The app key issued by IBM Marketing Cloud for the associated application.
+
+        Returns:
+            :obj:`~requests.Response`: The response from verify access. 
+
+            Success can be checked by examining the response.success boolean attribute.
+
+            If the request is successful the push notification provider uuid is returned as JSON and can be accessed from
+            the response.json attribute.
+
+        '''
+        apple = DataObject()
+        apple.add_value_string("key_store", apple_key_store)
+        apple.add_value_string("key_label", apple_key_label)
+        if apple.data:
+            apple.add_value_string("provider_address", provider_address)
+
+        firebase = DataObject()
+        firebase.add_value_string("server_key", firebase_server_key)
+        if firebase.data:
+            firebase.add_value_string("provider_address", provider_address)
+
+        imc = DataObject()
+        imc.add_value_string("client_id", imc_client_id)
+        imc.add_value_string("client_secret", imc_client_secret)
+        imc.add_value_string("refresh_token", imc_refresh_token)
+        imc.add_value_string("app_key", imc_app_key)
+        if imc.data:
+            imc.add_value_string("provider_address", provider_address)
+
+        provider = DataObject()
+        provider.add_value_not_empty("apple", apple.data)
+        provider.add_value_not_empty("firebase", firebase.data)
+        provider.add_value_not_empty("imc", imc.data)
+
+        data = DataObject()
+        data.add_value_string("app_id", app_id)
+        data.add_value_string("platform", platform)
+        data.add_value_not_empty("provider", provider.data)
+
+        endpoint = PUSH_NOTIFICATION + '/{}'.format(pnr_id)
+        response = self.client.pout_json(endpoint, data.data)
+        response.success = response.status_code == 200
+
+        return response
+
+
+    def delete_provider(self, pnr_id):
+        '''
+        Delete an existing push notification provider.
+
+        Args:
+            pnr_id (:obj:`str`): The identifier for the push notification resource to be removed.
+        
+        Returns:
+            :obj:`~requests.Response`: The response from verify access. 
+
+            Success can be checked by examining the response.success boolean attribute.
+
+            If the request is successful the push notification provider is returned as JSON and can be accessed from
+            the response.json attribute.
+        
+        '''
+        endpoint = '{}/{}'.format(PUSH_NOTIFICATION, pnr_id)
+        response = self.client.delete_json(endpoint)
+        response.success = response.status_code == 204
+
+        return response
```

### Comparing `pyisva-0.1.0/pyisva/core/access/riskprofiles.py` & `pyisva-0.2.0/pyisva/core/access/riskprofiles.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 
 class RiskProfiles(object):
 
     def __init__(self, base_url, username, password):
         super(RiskProfiles, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
-    def create(self, description=None, name=None, active=None, attributes=None):
+    def create_profile(self, description=None, name=None, active=None, attributes=None, predefined=False):
         '''
         Create a risk profile.
 
         Args:
             description (:obj:`str`): A description associated with the risk profile.
-            name (:obj:`str`): A unique name of the risk profile
+            name (:obj:`str`): A unique name of the risk profile.
             active (bool): Indicate if this is the active risk profile.
             attributes (:obj:`list` of :obj:`dict`):Array of attributes comprising this risk profile and the weight 
                                                 value of each attribute which is used in determining the risk score.
                                                 eg::
 
                                                     [
                                                         {"weight":50,
@@ -39,128 +39,131 @@
                                                          "attributeID":"34"
                                                         }
                                                     ]
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the id of the created risk profile can be acess from the 
-            response.id_from_location attribute
+            If the request is successful the id of the created risk profile can be accessed from the 
+            response.id_from_location attribute.
 
         '''
         data = DataObject()
         data.add_value_string("description", description)
         data.add_value_string("name", name)
         data.add_value("active", active)
         data.add_value("attributes", attributes)
-        data.add_value("predefined", False)
+        data.add_value("predefined", predefined)
 
         response = self.client.post_json(RISK_PROFILES, data.data)
         response.success = response.status_code == 201
 
         return response
 
 
-    def update(self, _id, description=None, name=None, active=None, attributes=None):
+    def update_profile(self, _id, description=None, name=None, active=None, attributes=None, predefined=False):
         '''
         Update an existing risk profile.
 
         Args:
             _id (:obj:`str`): The id of the risk profile to be updated.
             description (:obj:`str`): A description associated with the risk profile.
-            name (:obj:`str`): A unique name of the risk profile
+            name (:obj:`str`): A unique name of the risk profile.
             active (bool): Indicate if this is the active risk profile.
             attributes (:obj:`list` of :obj:`dict`):Array of attributes comprising this risk profile and the weight 
                                                 value of each attribute which is used in determining the risk score.
                                                 eg::
 
                                                     [
                                                         {"weight":50,
                                                          "attributeID":"28"
                                                         },
                                                         {"weight":10,
                                                          "attributeID":"34"
                                                         }
                                                     ]
 
+            predefined (`bool`, optional): Is this risk profile pre-defined by Verify Access.
+
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         data = DataObject()
         data.add_value_string("description", description)
         data.add_value_string("name", name)
-        data.add_value("active", active)
-        data.add_value("attributes", attributes)
-        data.add_value("predefined", False)
+        data.add_value_boolean("active", active)
+        data.add_value_not_empty("attributes", attributes)
+        data.add_value_boolean("predefined", predefined)
+
 
         response = self.client.post_json(RISK_PROFILES, data.data)
         response.success = response.status_code == 204
 
         return response
 
 
-    def list(self):
+    def list_profiles(self):
         '''
         List all of the configured risk profiles.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the rsik profiles are returned as JSON and can be accessed from
-            the response.json attribute
+            If the request is successful the risk profiles are returned as JSON and can be accessed from
+            the response.json attribute.
 
         '''
         response = self.client.get_json(RISK_PROFILES)
         response.success = response.status_code == 200
 
         return response
 
 
-    def get(self, _id):
+    def get_profile(self, _id):
         '''
         Get the configuration of a specific risk profile
 
         Args:
             _id (:obj:`str`): The id of the risk profile to return.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the rsik profiles are returned as JSON and can be accessed from
-            the response.json attribute
+            If the request is successful the risk profiles are returned as JSON and can be accessed from
+            the response.json attribute.
 
         '''
         endpoint = "{}/{}".format(RISK_PROFILES, _id)
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
 
-    def delete(self, _id):
+    def delete_profile(self, _id):
         '''
         Delete an existing risk profile.
 
         Args:
             _id (:obj:`str`): The id of the risk profile to be removed.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "{}/{}".format(RISK_PROFILES, _id)
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 204
```

### Comparing `pyisva-0.1.0/pyisva/core/access/runtimeparameters.py` & `pyisva-0.2.0/pyisva/core/access/runtimeparameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class RuntimeParameters(object):
 
     def __init__(self, base_url, username, password):
         super(RuntimeParameters, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
-    def update(self, parameter, value=None):
+    def update_parameter(self, parameter, value=None):
         '''
         Update a single runtime tuning parameter.
 
         Args:
             value (:obj:`str`): The parameter to be updated.
 
         Returns:
@@ -41,25 +41,25 @@
 
         response = self.client.put_json(endpoint, data.data)
         response.success = response.status_code == 204
 
         return response
 
 
-    def get_runtime_tuning(self):
+    def list_parameters(self):
         '''
         Get a list of all of the configured runtime tuning parameters.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the runtime tuning parameters are returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         '''
         endpoint = "%s/v1" % RUNTIME_TUNING
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
@@ -75,18 +75,18 @@
                                     eg: ``38a69185-a61a-44a1-b574-a3b502f01414.f980aabe-80b7-4738-9cda-bccede8d34f2``
             port (int): The port that the endpoint will listen on.
             secure (bool): Flag to indicate if endpoint uses SSL
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the new runtime endpoint id is returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         '''
         data = DataObject()
         data.add_value("interface", interface)
         data.add_value("port", port)
         data.add_value("secure", secure)
 
@@ -107,26 +107,37 @@
                                     eg: ``38a69185-a61a-44a1-b574-a3b502f01414.f980aabe-80b7-4738-9cda-bccede8d34f2``
             port (int): The port that the endpoint will listen on.
             secure (bool): Flag to indicate if endpoint uses SSL
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "%s/%s/%s:%d/v1" % (RUNTIME_TUNING, ENDPOINTS, interface, port)
 
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
         return response
 
 
     def update_trace(self, trace_string=""):
+        '''
+        Update the JVM trace settings for the Runtime Liberty server.
+
+        Args:
+            trace_string (:obj:`str`): The new JVM trace settings.
+
+        Returns:
+            :obj:`~requests.Response`: The response from verify access. 
+
+            Success can be checked by examining the response.success boolean attribute.        
+        '''
         parameters = DataObject()
         parameters.add_value("value", trace_string)
 
         response = self.client.put_json(RUNTIME_TRACE, parameters.data)
         response.success = response.status_code == 204
 
         return response
```

### Comparing `pyisva-0.1.0/pyisva/core/access/scimconfig.py` & `pyisva-0.2.0/pyisva/core/access/scimconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,60 +16,60 @@
 
 class SCIMConfig(object):
 
     def __init__(self, base_url, username, password):
         super(SCIMConfig, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
-    def get(self):
+    def get_config(self):
         '''
         Get the current SCIM configuration profile.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the SCIM profile is returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         '''
         response = self.client.get_json(SCIM_CONFIGURATION)
         response.success = response.status_code == 200
 
         return response
 
 
-    def get_schema(self,schema_name):
+    def get_schema(self, schema_name):
         '''
         Get the current SCIM configuration for a specific schema.
 
         Args:
             schema_name (:obj:`str`): The name of the SCIM schema to fetch configuration for.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the SCIM schema profile is returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         '''
         endpoint = "%s/%s" % (SCIM_CONFIGURATION,schema_name)
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
 
     def update(self, data):
         '''
-        Update the SCIM confiuration profile. This method could be better
+        Update the SCIM configuration profile. This method could be better.
         '''
         response = self.client.put_json(SCIM_CONFIGURATION, data)
         response.success = response.status_code == 200
 
         return response
 
 
@@ -98,53 +98,71 @@
     def update_config(self, admin_group="adminGroup", enable_header_authentication=True, enable_authz_filter=True,
             max_user_responses=None):
         '''
         Update the general configuration settings of the SCIM profile.
 
         Args:
             admin_group (:obj:`str`, optional): The name of the group used to identify SCIM admin users. 
-                                                Default is "adminGroup"
+                                                Default is "adminGroup".
             enable_header_authentication (bool, optional): Whether or not SCIM header authentication is enabled. 
-                                                Default is ``true``
+                                                Default is ``true``.
             enable_authz_filter (bool, optional): Whether or not the authorization filter is enabled.
             max_user_response (int, optional): The maximum number of entries that can be returned from a single call to the /User endpoint.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         data = DataObject()
         data.add_value_string("admin_group", admin_group)
         data.add_value_string("enable_header_authentication", enable_header_authentication)
         data.add_value_string("enable_authz_filter", enable_authz_filter)
         data.add_value("max_user_responses", max_user_responses)
 
         response = self.client.put_json(SCIM_CONFIGURATION_GENERAL, data.data)
         response.success = response.status_code == 200
 
         return response
 
+    def get_general_config(self):
+        '''
+        Get the general SCIM configuration settings:
+
+        Returns:
+            :obj:`~requests.Response`: The response from verify access.
+
+            Success can be checked by examining the response.success boolean attribute.
+
+            If the request is successful the general SCIM properties are returned as JSON and can be accessed from
+            the response.json attribute.
+        '''
+        response = self.client.get_json(SCIM_CONFIGURATION_GENERAL)
+        response.success = response.status_code == 200
+
+        return response
+
+
     def update_attribute_mode(self, schema_name, scim_attribute, scim_subattribute=None, mode=None):
         '''
         Update the attribute model used for SCIM attribute mapping.
 
         Args:
             schema_name (:obj:`str`): Name of ths SCIM schema to update attribute modes for.
-            scim_attribute (:obj:`str`): Name of the SCIM attribute to update mode for
-            scim_subattribute (:obj:`str`, optional): If the SCIM attribute is a mult-valued attribute this is the second 
+            scim_attribute (:obj:`str`): Name of the SCIM attribute to update mode for.
+            scim_subattribute (:obj:`str`, optional): If the SCIM attribute is a multi-valued attribute this is the second 
                                 level attribute name.
             mode (:obj:`str`): New mode for the SCIM attribute. Valid values are: "readonly", "writeonly", "readwrite", 
-                                "adminwrite" or "immutable"
+                                "adminwrite" or "immutable".
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
 
         data = DataObject()
         data.add_value_string("mode", mode)
 
         endpoint = "%s/attribute_modes/%s/%s" % (
@@ -166,18 +184,18 @@
             isam_domain (:obj:`str`): The name of the Verify Access domain.
             update_native_users (bool): Whether the UID of native users should be updated with the Verify Access user 
                                         identity when an Verify Access user is created.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the updated SCIM user configuration is returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         '''
         data = DataObject()
         data.add_value_string("ldap_connection", ldap_connection)
         data.add_value_string("isam_domain", isam_domain)
         data.add_value("update_native_users", update_native_users)
 
@@ -205,18 +223,18 @@
                                         "isamruntime".
             update_native_users (bool): Whether the UID of native users should be updated with the Verify Access user 
                                         identity when an Verify Access user is created.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the updated SCIM user configuration is returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         '''
         data = DataObject()
         data.add_value_string("ldap_connection", ldap_connection)
         data.add_value_string("isam_domain", isam_domain)
         data.add_value_string("connection_type", connection_type)
         data.add_value("update_native_users", update_native_users)
```

### Comparing `pyisva-0.1.0/pyisva/core/access/serverconnections.py` & `pyisva-0.2.0/pyisva/core/access/serverconnections.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,44 +22,45 @@
 
 class ServerConnections(object):
 
     def __init__(self, base_url, username, password):
         super(ServerConnections, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
+
     def create_ldap(self, name=None, description=None, locked=None,
             connection_host_name=None, connection_bind_dn=None,
             connection_bind_pwd=None, connection_ssl_truststore=None,
             connection_ssl_auth_key=None, connection_host_port=None,
             connection_ssl=None, connect_timeout=None, servers=None):
         '''
         Create a LDAP server connection.
 
         Args:
             name (:obj:`str`): Unique name for the server connection.
             description (:obj:`str`): Description of the server connection.
             locked (bool): Controls whether the connection is allowed to be deleted.
             connection_host_name (:obj:`str`): Host name for the LDAP server.
             connection_bind_dn (:obj:`str`): Name to bind to LDAP server for admin operations.
-            connection_bind_pwd (:obj:`str`): Password associted with admin domain name.
+            connection_bind_pwd (:obj:`str`): Password associated with admin domain name.
             connection_ssl_truststore (:obj:`str`, optional): The SSL database to use. Only valid if ssl is enabled.
-            connection_ssl_auth_key (:obj:`str`, optional): The cetificate to use to authentication connections. Only 
+            connection_ssl_auth_key (:obj:`str`, optional): The certificate to use to authentication connections. Only 
                                                             valid if ssl is enabled.
             connection_host_port (:obj:`str`): The port that the LDAP server is listening on.
             connection_ssl (bool): Enable SSL encryption on connections.
             connect_timeout (int): Length of time Verify Access will wait before timing out a connection.
             servers: (:obj:`list` of :obj:`dict`): Additional LDAP servers for this connection.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the uuid of the created LDAP connection can be acess from the 
-            response.id_from_location attribute
+            If the request is successful the uuid of the created LDAP connection can be accessed from the 
+            response.id_from_location attribute.
 
         '''
         connection_data = DataObject()
         connection_data.add_value_string("hostName", connection_host_name)
         connection_data.add_value_string("bindDN", connection_bind_dn)
         connection_data.add_value_string("bindPwd", connection_bind_pwd)
         connection_data.add_value_string(
@@ -83,79 +84,82 @@
         endpoint = SERVER_CONNECTION_LDAP + "/v1"
 
         response = self.client.post_json(endpoint, data.data)
         response.success = response.status_code == 201
 
         return response
 
+
     def delete_ldap(self, uuid):
         '''
         Delete an existing LDAP server connection.
 
         Args:
             uuid (:obj:`str`): The id of the LDAP server connection to be removed.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "%s/%s/v1" % (SERVER_CONNECTION_LDAP, uuid)
 
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
         return response
 
+
     def list_ldap(self):
         '''
         List the configured LDAP server connections.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the LDAP server connections are returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         '''
         endpoint = SERVER_CONNECTION_LDAP + "/v1"
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
+
     def create_smtp(self, name=None, description=None, locked=None, connect_timeout=None, 
             connection_host_name=None, connection_host_port=None,
             connection_ssl=None, connection_user=None, connection_password=None):
         '''
         Create a SMTP server connection.
 
         Args:
             name (:obj:`str`): Unique name for the server connection.
             description (:obj:`str`): Description of the server connection.
             locked (bool): Controls whether the connection is allowed to be deleted.
             connect_timeout (int): Amount of time Verify Access will wait before timing out a connection.
             connection_host_name (:obj:`str`, optional): The hostname of the SMTP server. Only valid if SSL is enabled.
-            connection_host_port (:obj:`str`, optional): The port that the SMTP server is listenting on. Only valid if
+            connection_host_port (:obj:`str`, optional): The port that the SMTP server is listening on. Only valid if
                                                         SSL is enabled.
             connection_ssl (bool): Enable SSL encryption on connections.
             connection_user (:obj:`str`, optional): User to authenticate to SMTP server.
-            connection_password (:obj:`str`, optonal): Password to authenticate to SMTP server.
+            connection_password (:obj:`str`, optional): Password to authenticate to SMTP server.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the uuid of the created LDAP connection can be acess from the 
-            response.id_from_location attribute
+            If the request is successful the uuid of the created LDAP connection can be accessed from the 
+            response.id_from_location attribute.
 
         '''
         connection_data = DataObject()
         connection_data.add_value_string("hostName", connection_host_name)
         connection_data.add_value("hostPort", connection_host_port)
         connection_data.add_value("ssl", connection_ssl)
         connection_data.add_value("user", connection_user)
@@ -175,14 +179,15 @@
         endpoint = SERVER_CONNECTION_SMTP + "/v1"
 
         response = self.client.post_json(endpoint, data.data)
         response.success = response.status_code == 201
 
         return response
 
+
     def delete_smtp(self, uuid):
         '''
         Delete an existing SMTP server connection.
 
         Args:
             uuid (:obj:`str`) The id of the SMTP server connection to remove.
 
@@ -227,25 +232,25 @@
         '''
         Create a Cloud Identity server connection.
 
         Args:
             name (:obj:`str`): Unique name for the server connection.
             description (:obj:`str`): Description of the server connection.
             locked (bool): Controls whether the connection is allowed to be deleted.
-            connection_host_name (:obj:`str`): The hostname of the Clud Idenity Tenant.
+            connection_host_name (:obj:`str`): The hostname of the Cloud Identity Tenant.
             connection_client_id (:obj:`str`): The id of the OIDC client to authenticate to Cloud Identity.
             connection_client_secret (:obj:`str`): The OIDC client secret to authenticate to Cloud Identity.
             connection_ssl_truststore (:obj:`str`): The SSL database to authenticate connections.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the uuid of the created Cloud Identity connection can be acess from the 
+            If the request is successful the uuid of the created Cloud Identity connection can be accessed from the 
             response.id_from_location attribute
 
         '''
         connection_data = DataObject()
         connection_data.add_value_string("adminHost", connection_host_name)
         connection_data.add_value("clientId", connection_client_id)
         connection_data.add_value("clientSecret", connection_client_secret)
@@ -267,80 +272,82 @@
         endpoint = SERVER_CONNECTION_CI + "/v1"
 
         response = self.client.post_json(endpoint, data.data)
         response.success = response.status_code == 201
 
         return response
 
+
     def delete_ci(self, uuid):
         '''
-        Delete an existing Cloid Identity server connection.
+        Delete an existing Cloud Identity server connection.
 
         Args:
             uuid (:obj:`str`): The id of the Cloud Identity connection to remove.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "%s/%s/v1" % (SERVER_CONNECTION_CI, uuid)
 
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
         return response
 
+
     def list_ci(self):
         '''
-        List the configured Cloid Identity server connections.
+        List the configured Cloud Identity server connections.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the Cloud Identity server connections are returned as JSON and can be accessed from
             the response.json attribute
 
         '''
         endpoint = SERVER_CONNECTION_CI + "/v1"
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
+
     def create_web_service(self, name=None, description=None, locked=None, connection_url=None,
-            connection_user=None, connection_password=None,
-            connection_ssl_truststore=None, connection_ssl_auth_key=None,
-            connection_ssl=None):
+            connection_user=None, connection_password=None, connection_ssl_truststore=None, 
+            connection_ssl_auth_key=None, connection_ssl=None):
         '''
-        Create a Web Serivece server connection.
+        Create a Web Service server connection.
 
         Args:
             name (:obj:`str`): Unique name for the server connection.
             description (:obj:`str`): Description of the server connection.
             locked (bool): Controls whether the connection is allowed to be deleted.
             connection_url (:obj:`str`): The URL to the server.
             connection_user (:obj:`str`, optional): The user to authenticate to the Web Service.
             connection_password (:obj:`str`, optional): The password to authenticate to the Web Service.
             connection_ssl_truststore (:obj:`str`, optional): The SSL database to authenticate connections. Only valid 
                                                             if SSL is enabled.
             connection_ssl_auth_key (:obj:`str`): The certificate to authenticate connections. Only valid if SSL is 
                                                 enabled.
-            connection_ssl (bool): Flag to enable SSL encryption ofr connections.
+            connection_ssl (bool): Flag to enable SSL encryption for connections.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the uuid of the created Web Service connection can be acess from the 
+            If the request is successful the uuid of the created Web Service connection can be accessed from the 
             response.id_from_location attribute
 
         '''
         connection_data = DataObject()
         connection_data.add_value_string("url", connection_url)
         connection_data.add_value_string("user", connection_user)
         connection_data.add_value_string("password", connection_password)
@@ -381,23 +388,23 @@
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
         return response
 
     def list_web_service(self):
         '''
-        List the configure Web Service server connections
+        List the configure Web Service server connections.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the Web Service server connections are returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         '''
         endpoint = SERVER_CONNECTION_WEB_SERVICE + "/v1"
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
@@ -433,22 +440,22 @@
             connection_max_idle (:obj:`str`): Amount of time after which an unused or idle connection can be discarded.
             connection_max_pool_size (int): Maximum number of physical connections for a pool. A value of 0 is unlimited.
             connection_min_pool_size (int): Minimum number of physical connections to maintain in the pool.
             connection_per_local_thread (int): Caches the specified number of connections for each thread.
             connection_purge_policy (:obj:`str`): Specifies which connections to destroy when a stale connection is 
                                                 detected in a pool.
             connection_reap_time (:obj:`str`): Amount of time between runs of the pool maintenance thread. A value of -1
-                                                disables pool maintenace.
+                                                disables pool maintenance.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the uuid of the created JDBC can be acess from the 
+            If the request is successful the uuid of the created JDBC can be accessed from the 
             response.id_from_location attribute
 
         '''
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value_string("description", description)
         data.add_value_string("locked", locked)
@@ -494,15 +501,15 @@
 
         Args:
             uuid (:obj:`str`): The id of the JDBC to be removed.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "%s/%s/v1" % (SERVER_CONNECTION_JDBC, uuid)
 
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
@@ -512,39 +519,39 @@
     def list_jdbc(self):
         '''
         List the configured JDBC server connections.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the JDBC's are returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         '''
         endpoint = SERVER_CONNECTION_JDBC + "/v1"
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
 
     def list_all(self):
         '''
-        List all of the configued server connections.
+        List all of the configured server connections.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the server connections are returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         '''
         endpoint = SERVER_CONNECTION_ROOT + "/v1"
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
@@ -565,28 +572,28 @@
         Create an Verify Access Runtime server connection.
 
         Args:
             name (:obj:`str`): Unique name for the server connection.
             description (:obj:`str`): Description of the server connection.
             locked (bool): Controls whether the connection is allowed to be deleted.
             connection_bind_dn (:obj:str`): The domain name to bind to the runtime server.
-            connection_bind_pwd (:obj:`str`): The passwrod to bind to the runtime server.
+            connection_bind_pwd (:obj:`str`): The password to bind to the runtime server.
             connection_ssl_truststore (:obj:`str`): The SSL database to authenticate connections. Only valid if SSL is
                                                 enabled.
-            connetion_ssl_auth_key (:obj:`str`): The certificate to authenticate connections. Only valid if SSL is enabled.
-            connection_ssl (bool): Flag to enable SSL encryption for connetions.
+            connection_ssl_auth_key (:obj:`str`): The certificate to authenticate connections. Only valid if SSL is enabled.
+            connection_ssl (bool): Flag to enable SSL encryption for connections.
             connect_timeout (int): Length of time Verify Access will wait before timing out a connection.
             servers: (:obj:`list` of :obj:`dict`): Additional LDAP servers for this connection.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the uuid of the created LDAP connection can be acess from the 
+            If the request is successful the uuid of the created LDAP connection can be accessed from the 
             response.id_from_location attribute
 
         '''
         connection_data = DataObject()
         connection_data.add_value_string("bindDN", connection_bind_dn)
         connection_data.add_value_string("bindPwd", connection_bind_pwd)
         connection_data.add_value_string(
@@ -611,23 +618,23 @@
         response.success = response.status_code == 201
 
         return response
 
 
     def list_runtime(self):
         '''
-        List the configured Verify Accss runtime server connections.
+        List the configured Verify Access runtime server connections.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the Verify Access runtime server connections are returned as JSON and can be 
-            accessed from the response.json attribute
+            accessed from the response.json attribute.
 
         '''
         endpoint = SERVER_CONNECTION_ISAM_RUNTIME + "/v1"
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
         return response
@@ -639,15 +646,15 @@
 
         Args:
             uuid (:obj:`str`): The id of the Verify Access runtime connection to remove.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "%s/%s/v1" % (SERVER_CONNECTION_ISAM_RUNTIME, uuid)
 
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
         return response
```

### Comparing `pyisva-0.1.0/pyisva/core/access/templatefiles.py` & `pyisva-0.2.0/pyisva/core/access/templatefiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,26 @@
     def __init__(self, base_url, username, password):
         super(TemplateFiles, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
 
     def create_directory(self, path, dir_name=None):
         '''
-        Create a new directory for template files
+        Create a new directory for template files.
 
         Args:
             path (:obj:`str`): Path to directory where new directory will be created.
             dir_name (:obj:`str`): Name of new directory
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the id of the direcotry is returned as JSON and can be accessed from
+            If the request is successful the id of the directory is returned as JSON and can be accessed from
             the response.json attribute
 
         '''
         data = DataObject()
         data.add_value_string("dir_name", dir_name)
         data.add_value_string("type", "dir")
 
@@ -50,24 +50,24 @@
 
 
     def get_directory(self, path, recursive=None):
         '''
         List the contents of a directory.
 
         Args:
-            path (:obj:`str`): Path to direcotry to list.
+            path (:obj:`str`): Path to directory to list.
             recursive (bool): Flag to recursively list subdirectories.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the contents of the direcotry is returned as JSON and can be accessed from
-            the response.json attribute
+            If the request is successful the contents of the directory is returned as JSON and can be accessed from
+            the response.json attribute.
 
         '''
         parameters = DataObject()
         parameters.add_value("recursive", recursive)
 
         endpoint = "%s/%s" % (TEMPLATE_FILES, path)
 
@@ -82,24 +82,24 @@
 
     def create_file(self, path, file_name=None, contents=None):
         '''
         Create a new template file.
 
         Args:
             name (:obj:`str`): Name of new file
-            file_name (:obj:`str`, optional): Absolute path to file with contents of new tempalte file. Either file_name
+            file_name (:obj:`str`, optional): Absolute path to file with contents of new template file. Either file_name
                                             or contents must be specified.
             contents (:obj:`str`, optional): Contents of new template file. Either file_name or contents must be specified.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the contents of the direcotry is returned as JSON and can be accessed from
+            If the request is successful the contents of the directory is returned as JSON and can be accessed from
             the response.json attribute.
 
         '''
         data = DataObject()
         data.add_value_string("file_name", file_name)
 
         data.add_value_string("contents", contents)
@@ -111,19 +111,19 @@
         response.success = response.status_code == 200
 
         return response
 
 
     def delete_file(self, path, file_name):
         '''
-        Delete a templafile from Verify Access.
+        Delete a template file from Verify Access.
 
         Args:
             path (:obj:`str`): Path to template file.
-            file_name (:obj:`str`): Name of tempalte file to be removed.
+            file_name (:obj:`str`): Name of template file to be removed.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
             If the request is successful the id of the file is returned as JSON and can be accessed from
@@ -195,18 +195,18 @@
             response.success = False
 
         return response
 
 
     def import_files(self, file_path, force=True):
         '''
-        Import a compressed (zip) file of tempalte files.
+        Import a compressed (zip) file of template files.
 
         Args:
-            file_path (:obj:`str`): Absolute path to compessed file to be imported.
+            file_path (:obj:`str`): Absolute path to compressed file to be imported.
             force (bool): Flag to overwrite any existing template files in Verify Access.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
```

### Comparing `pyisva-0.1.0/pyisva/core/access/userregistry.py` & `pyisva-0.2.0/pyisva/core/access/userregistry.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         Args:
             username (:obj:`str`): User to update password for.
             password (:obj:`str`): New password for user.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         data = DataObject()
         data.add_value_string("password", password)
 
         endpoint = "%s/users/%s/v1" % (USER_REGISTRY, username)
 
@@ -58,18 +58,18 @@
         Args:
             _id (:obj:`str`): A unique name for the new group.
             users (:obj:`list` of :obj:`str`, optional): List of users to add to group.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the id of the created group is returned as JSON and can be acessed from the
-            response.JSON attribute
+            If the request is successful the id of the created group is returned as JSON and can be accessed from the
+            response.JSON attribute.
 
         '''
         data = DataObject()
         data.add_value_string("id", _id)
         data.add_value("users", users)
 
         endpoint = USER_REGISTRY + "/groups/v1"
@@ -77,52 +77,52 @@
         response.success = response.status_code == 200
 
         return response
 
 
     def delete_group(self, group_id):
         '''
-        Delete a group from the AAC runtime user registry
+        Delete a group from the AAC runtime user registry.
 
         Args:
             group_id (:obj:`str`): The id of the group to be removed.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "{}/groups/{}/v1".format(USER_REGISTRY, group_id)
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
         return response
 
 
     def create_user(self, user_id, password=None, groups=None):
         '''
-        Creata a new AAC Runtime user.
+        Create a new AAC Runtime user.
 
         Args:
             _id (:obj:`str`): The unique id of the new user.
             password (:obj:`str`): Password for the user.
             groups (:obj:`list` of :obj:`str`): List of groups to add user to.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the id of the created user is returned as JSON and can be acessed from the
+            If the request is successful the id of the created user is returned as JSON and can be accessed from the
             response.JSON attribute
 
         '''
         data = DataObject()
-        data.add_vaule_string("id", user_id)
+        data.add_value_string("id", user_id)
         data.add_value_string("password", password)
         data.add_value("groups", groups)
 
         endpoint = USER_REGISTRY + "/users/v1"
         response = self.client.post_json(endpoint, data.data)
         response.success = response.status_code == 200
 
@@ -135,15 +135,15 @@
 
         Args:
             user_id (:obj:`str`): The id of the user to be removed.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         endpoint = "{}/users/{}/v1".format(USER_REGISTRY, user_id)
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
         return response
@@ -156,24 +156,24 @@
         Args:
             user_id (:obj:`str`): The id of the user being modified.
             group (:obj:`str`): The id of the group the user is being added to.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the id of the modified group is returned as JSON and can be acessed from the
-            response.JSON attribute
+            If the request is successful the id of the modified group is returned as JSON and can be accessed from the
+            response.JSON attribute.
 
         '''
         data = DataObject()
         data.add_value_string("id", group_id)
 
-        endpoint = "{}/users/{}/groups/v1".fomat(USER_REGISTRY, user_id)
+        endpoint = "{}/users/{}/groups/v1".format(USER_REGISTRY, user_id)
         response = self.client.put_json(endpoint, data.data)
         response.success = response.status_code == 200
 
         return response
 
 
     def remove_user_from_group(self, user_id=None, group=None):
@@ -183,22 +183,22 @@
         Args:
             user_id (:obj:`str`): The id of the user being modified.
             group_id (:obj:`str`): The id of the group the user is being removed from.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         '''
         data = DataObject()
         data.add_value_string("id", group_id)
 
         endpoint = "{}/users/{}/groups/v1".format(USER_REGISTRY, user_id)
-        response = self.client.delete_json(enpoint, data.data)
+        response = self.client.delete_json(endpoint, data.data)
         response.success = response.status_code == 204
 
         return response
 
 
     def get_user(self, user_id):
         '''
@@ -206,18 +206,18 @@
 
         Args:
             user_id (:obj:`str`): The id of the user.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the user's properties is returned as JSON and can be acessed from the
-            response.JSON attribute
+            If the request is successful the user's properties is returned as JSON and can be accessed from the
+            response.JSON attribute.
 
         '''
         endpoint = "{}/users/{}/v1".format(USER_REGISTRY, user_id)
         self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
@@ -229,18 +229,18 @@
 
         Args:
             group_id (:obj:`str`): The id of the group.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the user's properties is returned as JSON and can be acessed from the
-            response.JSON attribute
+            If the request is successful the user's properties is returned as JSON and can be accessed from the
+            response.JSON attribute.
 
         '''
         endpoint = "{}/groups/{}/v1".format(USER_REGISTRY, group_id)
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
@@ -249,18 +249,18 @@
     def list_groups(self):
         '''
         List the groups in the AAC runtime user registry.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the list of users is returned as JSON and can be acessed from the
-            response.JSON attribute
+            If the request is successful the list of users is returned as JSON and can be accessed from the
+            response.JSON attribute.
 
         '''
         endpoint = "{}/users/v1".format(USER_REGISTRY)
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
@@ -269,18 +269,18 @@
     def list_users(self):
         '''
         List the users in the AAC runtime user registry.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the list of groups is returned as JSON and can be acessed from the
-            response.JSON attribute
+            If the request is successful the list of groups is returned as JSON and can be accessed from the
+            response.JSON attribute.
 
         '''
         endpoint = "{}/groups/v1".format(USER_REGISTRY)
-        response = self.client.get_json(enpoint)
+        response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
```

### Comparing `pyisva-0.1.0/pyisva/core/accesscontrol.py` & `pyisva-0.2.0/pyisva/core/accesscontrol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 """
 @copyright: IBM
 """
 
 from .access.accesscontrol import AccessControl
 from .access.accesscontrol import AccessControl9030 as AC9030
+from .access.accesscontrol import AccessControl10000 as AC10000
 from .access.advancedconfig import AdvancedConfig
 from .access.apiprotection import APIProtection, APIProtection9040
 from .access.attributes import Attributes
 from .access.authentication import Authentication, Authentication9021
 from .access.mmfaconfig import MMFAConfig, MMFAConfig9021
 from .access.pushnotification import PushNotification, PushNotification9021
 from .access.riskprofiles import RiskProfiles
 from .access.runtimeparameters import RuntimeParameters
 from .access.scimconfig import SCIMConfig, SCIMConfig9050
 from .access.serverconnections import ServerConnections, ServerConnections9050
 from .access.templatefiles import TemplateFiles
 from .access.userregistry import UserRegistry, UserRegistry10020
 from .access.mappingrules import MappingRules
-from .access.fido2config import FIDO2Config
+from .access.fido2config import FIDO2Config, FIDO2Config10050
 from .access.fido2registrations import FIDO2Registrations
+from .access.pip import PIP
 
 
 class AccessControl9020(object):
     '''
-    Object used to managed Advanced Access Control endpoints. Avaliable modules are:
+    Object used to managed Advanced Access Control endpoints. Available modules are:
 
     :var access_control: Create and manage :ref:`Access Control` policies.
     :var advanced_config: Manage :ref:`Advanced Configuration` parameters.
     :var api_protection: Create and manage OIDC :ref:`API Protection` definitions and clients.
-    :var attributes: Craete and manage Risk Based Access :ref:`Attribute <Attributes>` mappings.
+    :var attributes: Create and manage Risk Based Access :ref:`Attribute <Attributes>` mappings.
     :var authentication: Create and manage :ref:Authentication` policies and mechanisms.
     :var mapping_rules: Create and manage JavaScript :ref:`Mapping Rules` used for customized authentication.
     :var mmfa_config: Configure :ref:`Mobile Multi-Factor Authentication` for Verify Access.
     :var push_notifications: Configure and manage :ref:`Push Notification Providers`.
     :var risk_profiles: Create and manage Risk Based Access :ref:`Risk Profiles`.
     :var runtime_parameters: Manage :ref:`Runtime Parameters` of the Liberty runtime server.
-    :var scim_config: Create and manage :ref:`SCIM<SCIM Configuration>` attribute mapping.
+    :var scim_config: Create and manage :ref:`SCIM<System for Cross-Domain Identity Management (SCIM) Configuration>` attribute mapping.
     :var server_connections: Create :ref:`Server Connections` to external service providers.
     :var template_files: Create and manage HTML and JSON i:ref:`Template Files`.
     :var user_registry: Manage :ref:`user authentication<User Registry>` to the Liberty runtime server.
+    :var pip: Manage :ref:`policy information points<PIP>`.
     '''
 
     def __init__(self, base_url, username, password):
         super(AccessControl9020, self).__init__()
         self.access_control = AccessControl(base_url, username, password)
         self.advanced_config = AdvancedConfig(base_url, username, password)
         self.api_protection = APIProtection(base_url, username, password)
@@ -55,14 +58,15 @@
             base_url, username, password)
         self.scim_config = SCIMConfig(base_url, username, password)
         self.server_connections = ServerConnections(
             base_url, username, password)
         self.template_files = TemplateFiles(base_url, username, password)
         self.user_registry = UserRegistry(base_url, username, password)
         self.mapping_rules = MappingRules(base_url, username, password)
+        self.pip = PIP(base_url, username, password)
 
 
 class AccessControl9021(AccessControl9020):
 
     def __init__(self, base_url, username, password):
         super(AccessControl9021, self).__init__(base_url, username, password)
         self.mmfa_config = MMFAConfig9021(base_url, username, password)
@@ -122,40 +126,43 @@
         super(AccessControl10000, self).__init__(base_url, username, password)
 
 
 class AccessControl10010(AccessControl10000):
 
     def __init__(self, base_url, username, password):
         super(AccessControl10010, self).__init__(base_url, username, password)
+        self.access_control = AC10000(base_url, username, password)
 
 
 class AccessControl10020(AccessControl10010):
 
     def __init__(self, base_url, username, password):
         super(AccessControl10020, self).__init__(base_url, username, password)
         self.user_registry = UserRegistry10020(base_url, username, password)
 
 
 class AccessControl10030(AccessControl10020):
 
     def __init__(self, base_url, username, password):
-              super(AccessControl10030, self).__init__(base_url, username, password)
+        super(AccessControl10030, self).__init__(base_url, username, password)
 
 class AccessControl10031(AccessControl10030):
 
     def __init__(self, base_url, username, password):
-              super(AccessControl10031, self).__init__(base_url, username, password)
+        super(AccessControl10031, self).__init__(base_url, username, password)
 
 class AccessControl10040(AccessControl10031):
 
     def __init__(self, base_url, username, password):
-              super(AccessControl10040, self).__init__(base_url, username, password)
+        super(AccessControl10040, self).__init__(base_url, username, password)
 
 class AccessControl10050(AccessControl10040):
 
     def __init__(self, base_url, username, password):
-              super(AccessControl10050, self).__init__(base_url, username, password)
+        super(AccessControl10050, self).__init__(base_url, username, password)
+        self.fido2_config = FIDO2Config10050(base_url, username, password)
+
 
 class AccessControl10060(AccessControl10050):
 
     def __init__(self, base_url, username, password):
-              super(AccessControl10060, self).__init__(base_url, username, password)
+        super(AccessControl10060, self).__init__(base_url, username, password)
```

### Comparing `pyisva-0.1.0/pyisva/core/analysis/applicationlog.py` & `pyisva-0.2.0/pyisva/core/analysis/applicationlog.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/analysisdiagnostics.py` & `pyisva-0.2.0/pyisva/core/analysisdiagnostics.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/federation/accesspolicy.py` & `pyisva-0.2.0/pyisva/core/federation/accesspolicy.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 
 class AccessPolicy(object):
 
     def __init__(self, base_url, username, password):
         super(AccessPolicy, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
-    def get_policies(self, _filter=None):
+    def list_policies(self, _filter=None):
         """
         Get the configured access policies.
 
         Args:
             _filter (:obj:`str`, optional
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the access policies are returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         """
         endpoint = ACCESS_POLICY
         if _filter != None:
             endpoint += "?filter=%s" % (_filter)
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
@@ -43,23 +43,23 @@
         return response
 
     def get_policy(self, policy_id=None):
         """
         Get a specific access policy.
 
         Args:
-            policy_id (:obj:`str`): The id of the policy to gfetch.
+            policy_id (:obj:`str`): The id of the policy to fetch.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
             If the request is successful the access policy is returned as JSON and can be accessed from
-            the response.json attribute
+            the response.json attribute.
 
         """
 
         endpoint = "%s/%s" % (ACCESS_POLICY, policy_id)
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
@@ -75,18 +75,18 @@
             category (:obj:`str`): A grouping of related access policies. Valid values are: "InfoMap", "AuthSVC", "OAUTH","OTP", "OIDC" and "SAML2_0".
             policy_type (:obj:`str`, optional): System default type for each access policy.
             content (:obj:`str`): Contents of the access policy rule.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the id of the create access policy can be acess from the
-            response.id_from_location attribute
+            If the request is successful the id of the create access policy can be accessed from the
+            response.id_from_location attribute.
 
         """
         data = DataObject()
         data.add_value_string('category',category)
         data.add_value_string('type',policy_type)
         data.add_value_string('name',policy_name)
         data.add_value_string("content", content)
@@ -99,21 +99,42 @@
 
     def update_policy(self, policy_id=None, content=None):
         """
         Update asn existing access policy
 
         Args:
             policy_id (:obj:`str`): The name of the access policy to be updated.
-            content (:obj:`str`): The serialsed content of the new JavaScript access policy
+            content (:obj:`str`): The serialized content of the new JavaScript access policy.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
         """
         data = DataObject()
         data.add_value_string("content", content)
         endpoint = "%s/%s" % (ACCESS_POLICY, policy_id)
         response = self.client.put_json(endpoint, data.data)
         response.success = response.status_code == 204
         return response
+
+
+    def delete_policy(self, policy_id=None):
+        """
+        Delete a specific access policy.
+
+        Args:
+            policy_id (:obj:`str`): The id of the policy to fetch.
+
+        Returns:
+            :obj:`~requests.Response`: The response from verify access. 
+
+            Success can be checked by examining the response.success boolean attribute.
+
+        """
+
+        endpoint = "%s/%s" % (ACCESS_POLICY, policy_id)
+        response = self.client.delete_json(endpoint)
+        response.success = response.status_code == 204
+
+        return response
```

### Comparing `pyisva-0.1.0/pyisva/core/federation/federations.py` & `pyisva-0.2.0/pyisva/core/federation/federations.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,43 +16,47 @@
 class Federations(object):
 
     def __init__(self, base_url, username, password):
         super(Federations, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
     def create_oidc_federation(self, name=None, role=None, redirect_uri_prefix=None, response_types_supported=None, 
-            attribute_mappings=None, identity_delegate_id=None, identity_rule_type="JAVASCRIPT", identity_mapping_rule=None, 
+            attribute_mappings=[], identity_delegate_id=None, identity_rule_type="JAVASCRIPT", identity_mapping_rule=None, 
             identity_applies_to=None, identity_auth_type=None, identity_ba_user=None, identity_ba_password=None,
             identity_client_keystore=None, identity_client_key_alias=None, identity_issuer_uri=None, 
             identity_message_format=None, identity_ssl_keystore=None, identity_uri=None, adv_delegate_id=None,
             adv_rule_type="JAVASCRIPT", adv_mapping_rule=None):
         """
         Create an OIDC Federation.
 
         Args:
             name (:obj:`str`): 	A meaningful name to identify this federation.
             role (:obj:`str`): The role of a federation, valid values are "ip", "sp", "op" and "rp".
-            response_types_supported (:obj:`str`): 
+            redirect_uri_prefix (:obj:`str`): The reverse proxy address to prepend to the redirect URI sent to the provider to 
+                                              communicate with this instance.
+            response_types_supported (:obj:`str`): List of response types which determine the flow to be executed. Valid values 
+                                                   to be included are "code", "token", "id_token". This selects the default flow
+                                                   to run when a metadata URL is specified in the partner configuration.
             attribute_mappings (:obj:`list` of :obj:`dict`): The attribute mapping data. format 
                                                             is::
 
                                                                 [
                                                                     {"name":"email",
                                                                      "source":"ldap_email"
                                                                     },
                                                                     {"name":"mobile",
                                                                      "source":"ldap_phone"
                                                                     }
                                                                 ]
 
             identity_delegate_id (:obj:`str`): The active mapping module instance.
-            identity_rule_type (:obj:`str`): The type of the mapping rule. The only supported type currently is JAVASCRIPT.
+            identity_rule_type (:obj:`str`): The type of the mapping rule. The only supported type currently is "JAVASCRIPT".
             identity_mapping_rule (:obj:`str`): A reference to an ID of an identity mapping rule. 
-            identity_applies_to (:obj:`str`): Refers to STS chain that consumes callout response. Required if WSTRUST 
-                            messageFormat is specified, ignored otherwise.
+            identity_applies_to (:obj:`str`): Refers to the STS chain that consumes callout responses. Required if WSTRUST 
+                                              messageFormat is specified, ignored otherwise.
             identity_auth_type (:obj:`str`): Authentication method used when contacting external service. Supported 
                             values are NONE, BASIC or CERTIFICATE.
             identity_ba_user (:obj:`str`): Username for authentication to external service. Required if BASIC authType 
                             is specified, ignored otherwise.
             identity_ba_password (:obj:`str`): Password for authentication to external service. Required if BASIC 
                             authType is specified, ignored otherwise.
             identity_client_keystore (:obj:`str`): Contains key for HTTPS client authentication. Required if CERTIFICATE 
@@ -68,28 +72,28 @@
             adv_delegate_id (:obj:`str`): The active module instance. Valid values are "skip-advance-map" and "default-map".
             adv_rule_type (:obj:`str`): The type of the mapping rule. The only supported type currently is JAVASCRIPT.
             adv_mapping_rule (:obj:`str`): A reference to an ID of an advance configuration mapping rule.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the id of the created obligation can be acess from the
-            response.id_from_location attribute
+            If the request is successful the id of the created obligation can be access from the
+            response.id_from_location attribute.
 
         """
         attributeMapping = DataObject()
         attributeMapping.add_value_not_empty("map", attribute_mappings)
 
         advConfig = DataObject()
         advConfig.add_value_string("activeDelegateId", adv_delegate_id)
         advConfigProps = DataObject()
         advConfigProps.add_value_string("ruleType", adv_rule_type)
-        advConfigProps.add_vaule_string("advanceMappingRuleReference", adv_mapping_rule)
+        advConfigProps.add_value_string("advanceMappingRuleReference", adv_mapping_rule)
         advConfig.add_value_not_empty("properties", advConfigProps.data)
 
         identityMapping = DataObject()
         identityMapping.add_value_string("activeDelegateId", identity_delegate_id)
         properties = DataObject()
         if identity_delegate_id == "default-map":
             properties.add_value_string("ruleType", identity_rule_type)
@@ -122,170 +126,144 @@
         data.add_value_not_empty("configuration", configuration.data)
 
         response = self.client.post_json(FEDERATIONS, data.data)
         response.success = response.status_code == 201
 
         return response
 
-    def create_oidc_partner(self, federation_id, name=None, enabled=False, role="rp", template_name=None, client_id=None, 
-        client_secret="", active_delegate_id=None, metadata_endpoint_url=None, issuer_identifier=None, response_types=[],
-        authorization_endpoint=None, token_endpoint=None, user_info_endpoint=None, signature_alg=None, 
-        verification_keystore=None, verification_key_label=None, jwk_endopoint_url=None, key_mgmt_alg=None, 
-        content_encrypt_alg=None, decrypt_keystore=None, decrypt_key_label=None, scope=[], perform_user_info=None, 
-        token_endpoint_auth_method=None, attribute_mapping=None, identity_delegate_id=None, identity_mapping_rule=None,
+
+    def create_oidc_partner(self, federation_id, name=None, role="rp", redirect_uri_prefix=None,
+        response_types=[], attribute_mappings=[], identity_delegate_id=None, identity_mapping_rule=None,
         identity_auth_type=None, identity_ba_user=None, identity_ba_password=None, identity_client_keystore=None, 
         identity_client_key_alias=None, identity_issuer_uri=None, identity_msg_fmt=None, identity_ssl_keystore=None,
         identity_uri=None, adv_config_delegate_id=None, adv_config_rule_type="JAVASCRIPT", adv_config_mapping_rule=None):
         """
         Add a partner configuration to an ODIC RP.
 
         Args:
             federation_id (:obj:`str`): The id of the ODIC federation to create a partner for.
-            name (:obj:`str`): THe name o the partner to be created.
-            enabled (:obj:`str`): Whether to enable the partner.
+            name (:obj:`str`): The name o the partner to be created.
             role (:obj:`str`, optional): The role this partner plays in its federation. Default is "rp"
-            template_name (:obj:`str`): An identifier for the template on which to base this partner.
-            client_id (:obj:`str`): The id that identifies this client to the provider.
-            client_secret(:obj:`str`, optional): The secret associated with the client ID. Set as "" if using a public 
-                            client.
-            active_delegate_id (:obj:`str`): The active module instance. Valid values are "noMetadata" and "metadataEndpointUrl".
-            metadata_endpoint (:obj:`str`, optional): The /metadata endpoint URL of the provider.
-            issuer_identifier (:obj:`str`, optional): The issuer ("iss") value of the provider.
             response_types (:obj:`str`, optional): List of response type which determines which flow to be executed.
-            authorization_endpoint (:obj:`str`, optional): The /authorize endpoint URL of the provider.
-            token_endpoint (:obj:`str`, optional): The /token endpoint URL of the provider. Required if "code" response 
-                            type is selected.
-            user_info_endpoint (:obj:`str`, optional): The /userinfo endpoint URL of the provider.
-            signature_alg (:obj:`str`, optional): The signing algorithm to use. Supported values are "none", "HS256", 
-                            "HS384", "HS512", "RS256", "RS384", "RS512", "ES256", "ES384", "ES512", "PS256", "PS384", 
-                            "PS512". Default is none.
-            verification_keystore (:obj:`str`, optional): When signature algorithm requires a certificate, the keystore 
-                            which contains the selected certificate to perform the signing.
-            verification_key_label (:obj:`str`, optional): When signature algorithm requires a certificate, the alias 
-                            of the public key in the selected keystore to use in signature verification.
-            jwk_endopoint_url (:obj:`str`): When signature algorithm requires a certificate, the JWK endpoint of the provider.
-            key_mgmt_alg (:obj:`str`, optional): The key management algorithm to use. Supported values are "none", "dir", 
-                            "A128KW", "A192KW", "A256KW", "A128GCMKW", "A192GCMKW", "A256GCMKW", "ECDH-ES", "ECDH-ES+A128KW", 
-                            "ECDH-ES+A192KW", "ECDH-ES+A256KW", "RSA1_5", "RSA-OAEP", "RSA-OAEP-256".
-            content_encrypt_alg (:obj:`str`, optional): The content encryption algorithm to use. Supported values are 
-                            "none", "A128CBC-HS256", "A192CBC-HS384", "A256CBC-HS512", "A128GCM", "A192GCM", "A256GCM".
-            decrypt_keystore (:obj:`str`): When key management algorithm requires a certificate, the keystore which 
-                            contains the selected certificate to perform JWT decryption.
-            decrypt_key_label (:obj:`str`): When key management algorithm requires a certificate, the alias of the 
-                            private key in the selected keystore to perform JWT decryption.
-            scope (:obj:`list` of :obj:`str`, optional): An array of strings that identify the scopes to request from 
-                            the provider. Defaults to ["openid"].
-            perform_user_info (`bool`, optional): A setting that specifies whether to perform user info request 
-                            automatically whenever possible.
-            token_endpoint_auth_method (:obj:`str`): The token endpoint authentication method. Valid values are 
-                            "client_secret_basic" and "client_secret_post".
-            attribute_mapping (:obj:`list` of :obj:`dict`, optional): List of configured attribute sources. Format of
+            attribute_mappings (:obj:`list` of :obj:`dict`, optional): List of configured attribute sources. Format of
                             dictionary is::
 
                                                 [
                                                     {"name":"email", 
                                                      "source": "ldap"
                                                     }, 
                                                     {"name":"preferred_name", 
                                                      "source":"credential"
                                                     }
                                                 ]
 
             identity_delegate_id (:obj:`str`): The active mapping module instance. Valid values are "skip-identity-map", 
-                            "default-map" and "default-http-custom-map".
+                                               "default-map" and "default-http-custom-map".
+            identity_mapping_rule (:obj:`str`): A reference to an ID of an identity mapping rule.
             identity_auth_type (:obj:`str`, optional): Authentication method used when contacting external service. Supported 
-                            values are NONE, BASIC or CERTIFICATE.
+                                                       values are NONE, BASIC or CERTIFICATE.
             identity_ba_user (:obj:`str`, optional): Username for authentication to external service.
             identity_ba_password (:obj:`str`, optional): Password for authentication to external service.
             identity_client_keystore (:obj:`str`, optional): Contains key for HTTPS client authentication.
-            identity_cliekt_key_alias (:obj:`str`, optional): Alias of the key for HTTPS client authentication.
+            identity_client_key_alias (:obj:`str`, optional): Alias of the key for HTTPS client authentication.
             identity_issuer_uri (:obj:`str`, optional): Refers to STS chain that provides input for callout request.
             identity_msg_fmt (:obj:`str`, optional): Message format of callout request.
             identity_ssl_keystore (:obj:`str`, optional): SSL certificate trust store to use when validating SSL 
-                            certificate of external service.
+                                                          certificate of external service.
             identity_uri (:obj:`str`): Address of destination server to call out to.
             adv_config_delegate_id (:obj:`str`): The active module instance. Valid values are "skip-advance-map" and 
-                            "default-map".
+                                                 "default-map".
             adv_config_rule_type (:obj:`str`, optional): The type of the mapping rule. The only supported type currently 
-                            is JAVASCRIPT.
+                                                         is "JAVASCRIPT".
             adv_config_mapping_rule (:obj:`str`, optional): A reference to an ID of an advance configuration.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the id of the created obligation can be acess from the
-            response.id_from_location attribute
+            If the request is successful the id of the created obligation can be access from the
+            response.id_from_location attribute.
 
         """
-        #TODO
         data = DataObject()
         data.add_value_string("name", name)
-        data.add_value("enabled", enabled)
         data.add_value_string("role", role)
 
-        attributeMapping = DataObject()
         identityMapping = DataObject()
+        identityMapping.add_value_string("activeDelegateId", identity_delegate_id)
+        identityProps = DataObject()
+        if identity_mapping_rule:
+            identityProps.add_value_string("identityMappingRuleReference", identity_mapping_rule)
+            identityProps.add_value_string("ruleType", "JAVASCRIPT")
+        else:
+            identityProps.add_value_string("authType", identity_auth_type)
+            identityProps.add_value_string("basicAuthUsername", identity_ba_user)
+            identityProps.add_value_string("basicAuthPassword", identity_ba_password)
+            identityProps.add_value_string("clientKeyStore", identity_client_keystore)
+            identityProps.add_value_string("clientKeyAlias", identity_client_key_alias)
+            identityProps.add_value_string("issuerUri", identity_issuer_uri)
+            identityProps.add_value_string("messageFormat", identity_msg_fmt)
+            identityProps.add_value_string("sslKeyStore", identity_ssl_keystore)
+            identityProps.add_value_string("uri", identity_uri)
+        identityMapping.add_value_not_empty("properties", identityProps.data)
+
+        advConfig = DataObject()
+        advConfProps = DataObject()
+        advConfProps.add_value_string("ruleType", adv_config_rule_type)
+        advConfProps.add_value_string("advanceMappingRuleReference", adv_config_mapping_rule)
+        advConfig.add_value_not_empty("properties", advConfProps.data)
+        advConfig.add_value_string("activeDelegateId", adv_config_delegate_id)
 
         configuration = DataObject()
+        configuration.add_value_not_empty("advanceConfiguration", advConfig.data)
         configuration.add_value_not_empty("identityMapping", identityMapping.data)
+        attributeMapping = DataObject()
+        attributeMapping.add_value_not_empty("map", attribute_mappings)
         configuration.add_value_not_empty("attributeMapping", attributeMapping.data)
-
-        configuration.add_value_not_empty("templateName", template_name)
-        configuration.add_value_not_empty("clientId", client_id)
-        configuration.add_value_not_empty("clientSecret", client_secret)
-        configuration.add_value_not_empty("appliesTo", applies_to)
-        configuration.add_value_not_empty("grantType", grant_type)
-        configuration.add_value_not_empty("authorizationEndpointUrl", authorization_endpoint_url)
-        configuration.add_value_not_empty("tokenEndpointUrl", token_endpoint_url)
-        configuration.add_value_not_empty("signatureAlgorithm", signature_algorithm)
-        configuration.add_value_not_empty("signingKeystore", signing_keystore)
-        configuration.add_value_not_empty("signingKeyLabel", signing_key_label)
-        configuration.add_value_not_empty("issuerIdentifier", issuer_identifier)
-        configuration.add_value_not_empty("redirectUriPrefix", redirect_uri_prefix)
-        configuration.add_value_not_empty("jwkEndpointUrl", jwk_endopoint_url)
-        configuration.add_value("scope", scope)
+        configuration.add_value_string("redirect_uri_prefix", redirect_uri_prefix)
+        configuration.add_value_not_empty("responseTypes", response_types)
 
         data.add_value_not_empty("configuration", configuration.data)
 
         endpoint = "%s/%s/partners" % (FEDERATIONS, federation_id)
 
         response = self.client.post_json(endpoint, data.data)
         response.success = response.status_code == 201
 
         return response
 
 
-    def create_saml_federation(self, name=None, role=None, access_policy=None, artifact_lifetime=None, assertion_attr_types=[],
-            assertion_session_not_on_or_after=None, assertion_multi_attr_stmt=None, assertion_valid_before=None, 
-            assertion_valid_after=None, artifact_resolution_service=[], attribute_mapping=[], company_name=None,
-            encrypt_block_alg=None, encrypt_key_transport_alg=None, encrypt_key_alias=None, encrypt_key_store=None, 
-            encrypt_name_id=None, encrypt_assertions=None, encrypt_assertion_attrs=None, decrypt_key_alias=None, 
-            decrypt_key_store=None, identity_delegate_id=None, identity_rule_type='JAVASCRIPT', identity_rule_id=None,
-            identity_applies_to=None, identity_auth_type=None, identity_ba_user=None, identity_ba_password=None,
-            identity_client_keystore=None, identity_client_key_alias=None, identity_issuer_uri=None, identity_msg_fmt=None,
-            identity_ssl_keystore=None, identity_uri=None, ext_delegate_id=None, ext_mapping_rule=None, manage_name_id_services=[],
-            msg_valid_time=None, msg_issuer_fmt=None, msg_issuer_name_qualifier=None, name_id_format=None, name_id_supported=[],
-            consent_to_federate=True, exclude_session_index_logout_request=False, poc_url=None, provider_id=None, 
-            session_timeout=None, sign_alg=None, sign_digest_alg=None, sign_valid_key_store=None, sign_valid_key_alias=None, 
-            sign_assertion=None, sign_auth_rsp=None, sign_arti_req=None, sign_arti_rsp=None, 
+    def create_saml_federation(self, name=None, role=None, template_name=None, access_policy=None, artifact_lifetime=None, 
+            assertion_attr_types=[], assertion_session_not_on_or_after=None, assertion_multi_attr_stmt=None, 
+            assertion_valid_before=None, assertion_valid_after=None, artifact_resolution_service=[], attribute_mappings=[], 
+            company_name=None, encrypt_block_alg=None, encrypt_key_transport_alg=None, encrypt_key_alias=None, 
+            encrypt_key_store=None, encrypt_name_id=None, encrypt_assertions=None, encrypt_assertion_attrs=None, 
+            decrypt_key_alias=None, decrypt_key_store=None, identity_delegate_id=None, identity_rule_type='JAVASCRIPT', 
+            identity_rule_id=None, identity_applies_to=None, identity_auth_type=None, identity_ba_user=None, 
+            identity_ba_password=None, identity_client_keystore=None, identity_client_key_alias=None, identity_issuer_uri=None, 
+            identity_msg_fmt=None, identity_ssl_keystore=None, identity_uri=None, ext_delegate_id=None, ext_mapping_rule=None, 
+            manage_name_id_services=[], msg_valid_time=None, msg_issuer_fmt=None, msg_issuer_name_qualifier=None, 
+            name_id_default=None, name_id_supported=[], consent_to_federate=True, exclude_session_index_logout_request=False, 
+            poc_url=None, provider_id=None, session_timeout=None, sign_alg=None, sign_digest_alg=None, sign_valid_key_store=None, 
+            sign_valid_key_alias=None, sign_assertion=None, sign_auth_rsp=None, sign_arti_req=None, sign_arti_rsp=None, 
             sign_logout_req=None, sign_logout_rsp=None, sign_name_id_req=None, sign_name_id_rsp=None, validate_auth_req=None,
             validate_assert=None, validate_arti_req=None, validate_arti_rsp=None, validate_logout_req=None, validate_logout_rsp=None,
             validate_name_id_req=None, validate_name_id_rsp=None, transform_include_namespace=None, sign_include_pubkey=None,
             sign_include_cert=None, sign_include_issuer=None, sign_include_ski=None, sign_include_subject=None, sign_keystore=None,
             sign_key_alias=None, sso_svc_data=[], slo_svc_data=[], alias_svc_db_type=None, alias_svc_ldap_con=None,
             alias_svc_ldap_base_dn=None, assertion_consume_svc=[], authn_req_delegate_id=None, authn_req_mr=None):
         """
         Create a SAML 2.0 IDP or SP federation.
 
         Args:
             name (:obj:`str`): The name of the federation
             role (:obj:`str`): The role of a federation: "ip" for a SAML 2.0 identity provider federation, and "sp" for 
                             a SAML 2.0 service provider federation.
+            template_name (:obj:`str`): An identifier for the template on which to base this federation.
             access_policy (:obj:`str`, optional): The access policy that should be applied during single sign-on.
             artifact_lifetime(`int`, optional): The number of seconds that an artifact is valid. The default value is 120.
             assertion_attr_types (:obj:`list` of :obj:`str`, optional): A setting that specifies the types of attributes 
                             to include in the assertion.
             assertion_session_not_on_or_after (`int`, optional): The number of seconds that the security context established for 
                             the principal should be discarded by the service provider.The default value is 3600.
             assertion_mult_attr_stmt (`bool`, optional): A setting that specifies whether to keep multiple attribute 
@@ -306,15 +284,15 @@
                                                             {"binding":"soap",
                                                              "default":true,
                                                              "index":1,
                                                              "url":"https://domain.com/endpoint"
                                                             }
                                                         ]
 
-            attribute_mapping (:obj:`list` of :obj:`dict`, optional): The attribute mapping data. format 
+            attribute_mappings (:obj:`list` of :obj:`dict`, optional): The attribute mapping data. format 
                             is::
 
                                 [
                                     {"name":"email",
                                      "source":"ldap_email"
                                     },
                                     {"name":"mobile",
@@ -350,15 +328,15 @@
             identity_uri (:obj:`str`): Address of destination server to call out to.
             ext_delegate_id (:obj:`str`): The active extension mapping module instance.
             ext_mapping_rule (:obj:`str`): A reference to an ID of an extension mapping rule.
             manage_name_id_services (:obj:`list` of :obj:`dict`): Endpoints that accept SAML name ID management requests or responses.
             msg_valid_time (`int`, optional): The number of seconds that a message is valid. The default value is 300.
             msg_issuer_fmt (:obj:`str`, optional): The format of the issuer of SAML message.
             msg_issuer_name_qualifier (:obj:`str`): The name qualifier of the issuer of SAML messaged.
-            name_id_format (:obj:`str`): The name identifier format to use when the format attribute is not set, or is 
+            name_id_default (:obj:`str`): The name identifier format to use when the format attribute is not set, or is 
                             set to ``urn:oasis:names:tc:SAML:1.1:nameid-format:unspecified``.
             name_id_supported (:obj:`list` of :obj:`str`): The list of supported name identifier formats.
             consent_to_federate (`bool`, optional): A setting that specifies whether to ask user's consent before linking 
                             the account.
             exclude_session_index_logout_request (`bool`, optional): A setting that specifies whether the LogoutRequest 
                             messages sent out from this entity will exclude SessionIndex during IP init SLO flow. 
                             The default value is false.
@@ -438,63 +416,140 @@
             authn_req_delegate_id (:obj:`str`): The active mapping module instance. Valid values are 
                             "skip-authn-request-map" and "default-map".
             authn_req_mr (:obj:`str`): A reference to an ID of an authentication request rule.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
-            Success can be checked by examining the response.success boolean attribute
+            Success can be checked by examining the response.success boolean attribute.
 
-            If the request is successful the id of the created obligation can be acess from the
-            response.id_from_location attribute
+            If the request is successful the id of the created obligation can be access from the
+            response.id_from_location attribute.
         """
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value_string("protocol", "SAML2_0")
         data.add_value_string("role", role)
         data.add_value_string("templateName", template_name)
 
         encryptionSettings = DataObject()
         signatureSettings = DataObject()
+        assertionSettings = DataObject()
+        nameIdFmt = DataObject()
 
         identityMapping = None
-        if (active_delegate_id is not None):
+        if (identity_delegate_id is not None):
             identityMapping = DataObject()
-            identityMapping.add_value_string("activeDelegateId", active_delegate_id)
+            identityMapping.add_value_string("activeDelegateId", identity_delegate_id)
+            if (identity_mapping_rule is not None):
+                identityMapping.add_value_not_empty("properties", 
+                        {"identityMappingRuleReference": identity_rule_id,
+                         "ruleType": identity_rule_type})
+            else:
+                identProps = DataObject()
+                identProps.add_value_string("appliesTo", identity_applies_to)
+                identProps.add_value_string("authType", identity_auth_type)
+                identProps.add_value_string("basicAuthUsername", identity_ba_user)
+                identProps.add_value_string("basicAuthPassword", identity_ba_password)
+                identProps.add_value_string("clientKeyStore", identity_client_keystore)
+                identProps.add_value_string("clientKeyAlias", identity_client_key_alias)
+                identProps.add_value_string("issuerUri", identity_issuer_uri)
+                identProps.add_value_string("messageFormat", identity_msg_fmt)
+                identProps.add_value_string("sslKeyStore", identity_ssl_keystore)
+                identProps.add_value_string("uri", identity_uri)
+                identityMapping.add_value_not_empty("properties", identProps.data)
+
+        extensionMapping = None
+        if(ext_delegate_id is not None):
+            extensionMapping = DataObject()
+            extensionMapping.add_value_string("activeDelegateId")
+            if ext_mapping_rule is not None:
+                extensionMapping.add_value("properties", {"extensionMappingRuleReference", ext_mapping_rule})
 
         decryptionKeyIdentifier = DataObject()
         decryptionKeyIdentifier.add_value_string("keystore", decrypt_keystore)
         decryptionKeyIdentifier.add_value_string("label", decrypt_key_label)
+
+        encryptionSettings.add_value_not_empty("decryptionKeyIdentifier", decryptionKeyIdentifier.data)
+        signatureSettings.add_value_not_empty("signingKeyIdentifier", signingKeyIdentifier.data)
+        signatureSettings.add_value_string("signatureAlgorithm", sign_alg)
+        signatureSettings.add_value_string("digestAlgorithm", sign_digest_alg)
+        signOpts = DataObject()
+        signOpts.add_value_boolean("signAssertion", sign_assertion)
+        signOpts.add_value_boolean("signAuthnResponse", sign_authn_rsp)
+        signOpts.add_value_boolean("signArtifactRequest", sign_arti_req)
+        signOpts.add_value_boolean("signArtifactResponse", sign_arti_rsp)
+        signOpts.add_value_boolean("signLogoutRequest", sign_logout_req)
+        signOpts.add_value_boolean("signLogoutResponse", sign_logout_rsp)
+        signOpts.add_value_boolean("signNameIDManagementRequest", sign_name_id_req)
+        signOpts.add_value_boolean("signNameIDManagementResponse", sign_name_id_rsp)
+        signatureSettings.add_value_not_empty("signingOptions", signOpts.data)
+
+        validOpts = DataObject()
+        validOpts.add_value_boolean("validateAuthnRequest", validate_auth_req)
+        validOpts.add_value_boolean("validateAssertion", validate_assert)
+        validOpts.add_value_boolean("validateArtifactRequest", validate_arti_req)
+        validOpts.add_value_boolean("validateArtifactResponse", validate_arti_rsp)
+        validOpts.add_value_boolean("validateLogoutRequest", validate_logout_req)
+        validOpts.add_value_boolean("validateLogoutResponse", validate_logout_rsp)
+        validOpts.add_value_boolean("validateNameIDManagementRequest", validate_name_id_req)
+        validOpts.add_value_boolean("validateNameIDManagementResponse", validate_name_id_rsp)
+        signatureSettings.add_value_not_empty("validationOptions", validOpts.data)
+        if transform_include_namespace is not None:
+            signatureSettings.add_value(
+                "transformAlgorithmElements", {"includeInclusiveNamespaces": transform_include_namespace})
+        keyInfo = DataObject()
+        keyInfo.add_value_boolean("includePublicKey", sign_include_pubkey)
+        keyInfo.add_value_boolean("includeX509CertificateData", sign_include_cert)
+        keyInfo.add_value_boolean("includeX509IssuerDetails", sign_include_issuer)
+        keyInfo.add_value_boolean("includeX509SubjectKeyIdentifier", sign_include_ski)
+        keyInfo.add_value_boolean("includeX509SubjectName", sign_include_subject)
+        keyInfo.add_value_boolean("includeX509SubjectName", sign_include_subject)
+        signatureSettings.add_value_not_empty("keyInfoElements", keyInfo.data)
         signingKeyIdentifier = DataObject()
         signingKeyIdentifier.add_value_string("keystore", signing_keystore)
         signingKeyIdentifier.add_value_string("label", signing_key_label)
 
-        encryptionSettings.add_value_not_empty("decryptionKeyIdentifier", decryptionKeyIdentifier.data)
-        signatureSettings.add_value_not_empty("signingKeyIdentifier", signingKeyIdentifier.data)
 
-        ssoServiceBinding = None
-        if (sso_service_binding is not None):
-            ssoServiceBinding = DataObject()
-            ssoServiceBinding.add_value_string("binding", sso_service_binding)
+        if name_id_default is not None or name_id_supported is not None:
+            nameIdFmt.add_value_string("default", name_id_default)
+            nameIdFmt.add_value_not_empty("supported", name_id_supported)
+
+        aliasSvc = DataObject()
+        aliasSvc.add_value_string("aliasServiceDBType", alias_svc_db_type)
+        aliasSvc.add_value_string("aliasServiceLDAPConnection", alias_svc_ldap_con)
+        aliasSvc.add_value_string("aliasServiceLDAPBaseDN", alias_svc_ldap_base_dn)
 
         configuration = DataObject()
+        configuration.add_value_string("accessPolicy", access_policy)
+        configuration.add_value("artifactLifeTime", artifact_lifetime)
+        configuration.add_value_not_empty("assertionConsumerService", assertion_consume_svc)
+        configuration.add_value_not_empty("assertionSettings", assertionSettings.data)
+        configuration.add_value_not_empty("artifactResolutionService", artifact_resolution_service)
+        configuration.add_value_not_empty("attributeMapping", {} if not attribute_mappings else {"map": attribute_mappings})
+        configuration.add_value_string("companyName", company_name)
         configuration.add_value_not_empty("encryptionSettings", encryptionSettings.data)
-        configuration.add_value_not_empty("signatureSettings", signatureSettings.data)
+        configuration.add_value_not_empty("identityMapping", identityMapping.data)
+        configuration.add_value_not_empty("extensionMapping", extensionMapping.data)
+        configuration.add_value_not_empty("manageNameIDService", manage_name_id_services)
+        configuration.add_value("messageValidTime", msg_valid_time)
+        configuration.add_value_string("messageIssuerFormat", msg_issuer_fmt)
+        configuration.add_value_string("messageIssuerNameQualifier", msg_issuer_name_qualifier)
+        configuration.add_value_not_empty("nameIDFormat", nameIdFmt.data)
+        configuration.add_value_boolean("needConsentToFederate", consent_to_federate)
+        configuration.add_value_boolean("excludeSessionIndexInSingleLogoutRequest", exclude_session_index_logout_request)
+        configuration.add_value_string("pointOfContactUrl", poc_url)
         configuration.add_value_string("providerId", provider_id)
-        configuration.add_value_string("pointOfContactUrl", point_of_contact_url)
-        configuration.add_value_string("companyName", company_name)
-        if (ssoServiceBinding is not None):
-            configuration.add_value("singleSignOnService", [ssoServiceBinding.data])
-        if (identityMapping is not None):
-            configuration.add_value("identityMapping", identityMapping.data)
-        configuration.add_value("needConsentToFederate", need_consent_to_federate)
-        configuration.add_value_string("messageIssuerFormat", message_issuer_format)
+        configuration.add_value("sessionTimeout", session_timeout)
+        configuration.add_value_not_empty("signatureSettings", signatureSettings.data)
+        configuration.add_value_not_empty("singleSignOnService", sso_svc_data)
+        configuration.add_value_not_empty("singleLogoutService", slo_svc_data)
+        configuration.add_value_not_empty("aliasServiceSettings", aliasSvc.data)
 
         data.add_value_not_empty("configuration", configuration.data)
-
         response = self.client.post_json(FEDERATIONS, data.data)
         response.success = response.status_code == 201
 
         return response
 
 
     def create_saml_partner(self, federation_id, name=None, enabled=False, role=None, template_name=None, access_policy=None,
@@ -510,15 +565,15 @@
             provider_id=None, session_timeout=None, sign_include_pub_key=None, sign_include_cert=None, sign_include_issuer=None, 
             sign_include_ski=None, sign_include_subject=None, sign_key_store=None, sign_key_alias=None, sign_arti_request=None, 
             sign_arti_rsp=None, sign_assertion=None, sign_authn_rsp=None, sign_logout_req=None, sign_logout_rsp=None, 
             sign_name_id_req=None, sign_name_id_rsp=None, transform_include_namespace=None, validate_assertion=None, 
             validate_authn_req=None, validate_arti_req=None, validate_arti_rsp=None, validate_logout_req=None, 
             validate_logout_rsp=None, validate_name_id_req=None, validate_name_id_rsp=None, sign_alg=None, sign_digest_alg=None, 
             validation_key_store=None, validation_key_alias=None, slo_svc=[], soap_key_store=None, soap_key_alias=None, 
-            soap_client_auth_method=None, soap_client_auth_ba_user=None, soap_client_auth_ba_pasword=None, 
+            soap_client_auth_method=None, soap_client_auth_ba_user=None, soap_client_auth_ba_password=None, 
             soap_client_auth_key_store=None, soap_client_auth_key_alias=None, anon_user_name=None, force_authn_to_federate=None, 
             authn_req_delegate_id=None, authn_req_mr=None, map_unknown_alias=None, sso_svc=[], default_target_url=None):
         """
         Create a SAML 2.0 IDP or SP Partner
 
         Args:
             federation_id (:obj:`str`): The system-assigned federation identifier.
@@ -828,247 +883,487 @@
         """
         endpoint = "%s/%s/partners/%s" % (FEDERATIONS, federation_id, partner_id)
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
         return response
 
 
-class Federations9040(Federations):
+    def delete_federation(self, federation_id):
+        """
+        Delete a federation configuration.
 
-    def create_oidc_rp_federation(self, name=None, redirect_uri_prefix=None,
-            response_types=None, active_delegate_id=None, identity_mapping_rule_reference=None,
-            advanced_configuration_active_delegate=None, advanced_configuration_rule_id=None):
+        Args:
+            federation_id (:obj:`str`): The id of the federation to modify.
+
+        Returns:
+            :obj:`~requests.Response`: The response from verify access. 
+
+            Success can be checked by examining the response.success boolean attribute
+
+        """
+        endpoint = "%s/%s" % (FEDERATIONS, federation_id)
+        response = self.client.delete_json(endpoint)
+        response.success = response.status_code == 204
+        return response
+
+
+    def delete_partner(self, federation_id, partner_id):
+        """
+        Delete a partner configuration from a federation
+
+        Args:
+            federation_id (:obj:`str`): The id of the federation to modify.
+            partner_id (:obj:`str`): The id of the partner to remove.
+
+        Returns:
+            :obj:`~requests.Response`: The response from verify access. 
+
+            Success can be checked by examining the response.success boolean attribute
+
+        """
+        endpoint = "%s/%s/partners/%s" % (FEDERATIONS, federation_id, partner_id)
+        response = self.client.delete_json(endpoint)
+        response.success = response.status_code == 204
+        return response
 
-        data = DataObject()
-        data.add_value_string("name", name)
-        data.add_value_string("protocol", "OIDC10")
-        data.add_value_string("role", 'rp')
 
+class Federations9040(Federations):
+
+    def create_oidc_federation(self, name=None, role=None, redirect_uri_prefix=None, response_types_supported=None, 
+            attribute_mappings=[], identity_delegate_id=None, identity_rule_type="JAVASCRIPT", identity_mapping_rule=None, 
+            identity_applies_to=None, identity_auth_type=None, identity_ba_user=None, identity_ba_password=None,
+            identity_client_keystore=None, identity_client_key_alias=None, identity_issuer_uri=None, 
+            identity_message_format=None, identity_ssl_keystore=None, identity_uri=None, adv_delegate_id=None,
+            adv_rule_type="JAVASCRIPT", adv_mapping_rule=None):
         attributeMapping = DataObject()
-        
+        attributeMapping.add_value_not_empty("map", attribute_mappings)
+
+        advConfig = DataObject()
+        advConfig.add_value_string("activeDelegateId", adv_delegate_id)
+        advConfigProps = DataObject()
+        advConfigProps.add_value_string("ruleType", adv_rule_type)
+        advConfigProps.add_value_string("advanceMappingRuleReference", adv_mapping_rule)
+        advConfig.add_value_not_empty("properties", advConfigProps.data)
+
         identityMapping = DataObject()
-        identityMapping.add_value_string("activeDelegateId", active_delegate_id)
+        identityMapping.add_value_string("activeDelegateId", identity_delegate_id)
         properties = DataObject()
-        properties.add_value_string("identityMappingRuleReference", identity_mapping_rule_reference)
-        identityMapping.add_value_not_empty("properties", properties.data)
+        if identity_delegate_id == "default-map":
+            properties.add_value_string("ruleType", identity_rule_type)
+            properties.add_value_string("identityMappingRuleReference", identity_mapping_rule_reference)
 
-        advancedConfiguration = DataObject()
-        if advanced_configuration_active_delegate == None : 
-            advancedConfiguration.add_value_string("activeDelegateId", 'skip-advance-map')
-        else:
-            advancedConfiguration.add_value_string("activeDelegateId", advanced_configuration_active_delegate)
-            properties = DataObject()
-            properties.add_value_string("advanceMappingRuleReference", advanced_configuration_rule_id)
-            advancedConfiguration.add_value_not_empty("properties", properties.data)
+        elif identity_delegate_id == "default-http-custom-map":
+            properties.add_value_string("appliesTo", identity_applies_to)
+            properties.add_value_string("authType", identity_auth_type)
+            properties.add_value_string("basicAuthUsername", identity_ba_user)
+            properties.add_value_string("basicAuthPassword", identity_ba_password)
+            properties.add_value_string("clientKeyStore", identity_client_keystore)
+            properties.add_value_string("clientKeyAlias", identity_client_key_alias)
+            properties.add_value_string("issuerUri", identity_issuer_uri)
+            properties.add_value_string("messageFormat", identity_message_format)
+            properties.add_value_string("sslKeyStore", identity_ssl_keystore)
+            properties.add_value_string("uri", identity_uri)
+        identityMapping.add_value_not_empty("properties", properties.data)
 
         configuration = DataObject()
-        configuration.add_value_string("redirectUriPrefix", redirect_uri_prefix)
-        configuration.add_value("responseTypes", response_types)
-        configuration.add_value_not_empty("advanceConfiguration", advancedConfiguration.data)
         configuration.add_value_not_empty("identityMapping", identityMapping.data)
         configuration.add_value_not_empty("attributeMapping", attributeMapping.data)
+        configuration.add_value_not_empty("advancedConfiguration", advConfig.data)
+        configuration.add_value_string("redirectUriPrefix", redirect_uri_prefix)
+        configuration.add_value_string("responseTypes", response_types_supported)
 
+        data = DataObject()
+        data.add_value_string("name", name)
+        data.add_value_string("protocol", "OIDC")
+        data.add_value_string("role", role)
         data.add_value_not_empty("configuration", configuration.data)
 
         response = self.client.post_json(FEDERATIONS, data.data)
         response.success = response.status_code == 201
 
         return response
 
-    def create_oidc_rp_partner(self, federation_id, name=None, enabled=False, client_id=None, 
-            client_secret=None, metadata_endpoint=None, scope=None,
-            token_endpoint_auth_method=None, perform_userinfo=False,
-            advanced_configuration_active_delegate='skip-advance-map', advanced_configuration_rule_id=None,
-            signing_algorithm=None):
-
+    def create_oidc_rp_partner(self, federation_id, name=None, role="rp", redirect_uri_prefix=None,
+        response_types=[], attribute_mappings=[], identity_delegate_id=None, identity_mapping_rule=None,
+        identity_auth_type=None, identity_ba_user=None, identity_ba_password=None, identity_client_keystore=None, 
+        identity_client_key_alias=None, identity_issuer_uri=None, identity_msg_fmt=None, identity_ssl_keystore=None,
+        identity_uri=None, adv_config_delegate_id=None, adv_config_rule_type="JAVASCRIPT", adv_config_mapping_rule=None):
         data = DataObject()
         data.add_value_string("name", name)
-        data.add_value("enabled", enabled)
-        data.add_value_string("role", 'rp')
+        data.add_value_string("role", role)
 
-        attributeMapping = DataObject()
         identityMapping = DataObject()
+        identityMapping.add_value_string("activeDelegateId", identity_delegate_id)
+        identityProps = DataObject()
+        if identity_mapping_rule:
+            identityProps.add_value_string("identityMappingRuleReference", identity_mapping_rule)
+            identityProps.add_value_string("ruleType", "JAVASCRIPT")
+        else:
+            identityProps.add_value_string("authType", identity_auth_type)
+            identityProps.add_value_string("basicAuthUsername", identity_ba_user)
+            identityProps.add_value_string("basicAuthPassword", identity_ba_password)
+            identityProps.add_value_string("clientKeyStore", identity_client_keystore)
+            identityProps.add_value_string("clientKeyAlias", identity_client_key_alias)
+            identityProps.add_value_string("issuerUri", identity_issuer_uri)
+            identityProps.add_value_string("messageFormat", identity_msg_fmt)
+            identityProps.add_value_string("sslKeyStore", identity_ssl_keystore)
+            identityProps.add_value_string("uri", identity_uri)
+        identityMapping.add_value_not_empty("properties", identityProps.data)
 
-        configuration = DataObject()
-
-
-        configuration.add_value_not_empty("clientId", client_id)
-        configuration.add_value_not_empty("signatureAlgorithm", signing_algorithm)
-        configuration.add_value_not_empty("clientSecret", client_secret)
-        configuration.add_value_not_empty("scope", scope)
-        configuration.add_value_not_empty("tokenEndpointAuthMethod", token_endpoint_auth_method)
-        configuration.add_value_not_empty("performUserinfo", perform_userinfo)
-
-        basic = DataObject()
-        basic.add_value_not_empty("activeDelegateId","metadataEndpointUrl")
-
-        basic_properties = DataObject()
-        basic_properties.add_value_not_empty("metadataEndpointUrl", metadata_endpoint)
-        basic.add_value("properties",basic_properties.data)
-        
-        configuration.add_value("scope", scope)
+        advConfig = DataObject()
+        advConfProps = DataObject()
+        advConfProps.add_value_string("ruleType", adv_config_rule_type)
+        advConfProps.add_value_string("advanceMappingRuleReference", adv_config_mapping_rule)
+        advConfig.add_value_not_empty("properties", advConfProps.data)
+        advConfig.add_value_string("activeDelegateId", adv_config_delegate_id)
 
+        configuration = DataObject()
+        configuration.add_value_not_empty("advanceConfiguration", advConfig.data)
         configuration.add_value_not_empty("identityMapping", identityMapping.data)
-
-        if advanced_configuration_active_delegate: 
-            advancedConfiguration = DataObject()
-            advancedConfiguration.add_value_string("activeDelegateId", advanced_configuration_active_delegate)
-            if (advanced_configuration_active_delegate != 'skip-advance-map'):
-                properties = DataObject()
-                properties.add_value_string("advanceMappingRuleReference", advanced_configuration_rule_id)
-                advancedConfiguration.add_value_not_empty("properties", properties.data)
-            configuration.add_value_not_empty("advanceConfiguration", advancedConfiguration.data)
-
-        configuration.add_value_not_empty("basicConfiguration", basic.data)
+        attributeMapping = DataObject()
+        attributeMapping.add_value_not_empty("map", attribute_mappings)
+        configuration.add_value_not_empty("attributeMapping", attributeMapping.data)
+        configuration.add_value_string("redirect_uri_prefix", redirect_uri_prefix)
+        configuration.add_value_not_empty("responseTypes", response_types)
 
         data.add_value_not_empty("configuration", configuration.data)
 
         endpoint = "%s/%s/partners" % (FEDERATIONS, federation_id)
 
         response = self.client.post_json(endpoint, data.data)
         response.success = response.status_code == 201
 
         return response
 
 class Federations10000(Federations9040):
 
-    def create_saml_federation(self, name=None, role=None, template_name=None, active_delegate_id=None, need_consent_to_federate=None,
-            signature_algorithm=None, signing_keystore=None, signing_key_label=None, sso_service_binding=None, message_issuer_format=None,
-            decrypt_keystore=None, decrypt_key_label=None, point_of_contact_url=None, provider_id=None, company_name=None):
-
+    def create_saml_federation(self, name=None, role=None, template_name=None, access_policy=None, artifact_lifetime=None, 
+            assertion_attr_types=[], assertion_session_not_on_or_after=None, assertion_multi_attr_stmt=None, 
+            assertion_valid_before=None, assertion_valid_after=None, artifact_resolution_service=[], attribute_mappings=[], 
+            company_name=None, encrypt_block_alg=None, encrypt_key_transport_alg=None, encrypt_key_alias=None, 
+            encrypt_key_store=None, encrypt_name_id=None, encrypt_assertions=None, encrypt_assertion_attrs=None, 
+            decrypt_key_alias=None, decrypt_key_store=None, identity_delegate_id=None, identity_rule_type='JAVASCRIPT', 
+            identity_rule_id=None, identity_applies_to=None, identity_auth_type=None, identity_ba_user=None, 
+            identity_ba_password=None, identity_client_keystore=None, identity_client_key_alias=None, identity_issuer_uri=None, 
+            identity_msg_fmt=None, identity_ssl_keystore=None, identity_uri=None, ext_delegate_id=None, ext_mapping_rule=None, 
+            manage_name_id_services=[], msg_valid_time=None, msg_issuer_fmt=None, msg_issuer_name_qualifier=None, 
+            name_id_default=None, name_id_supported=[], consent_to_federate=True, exclude_session_index_logout_request=False, 
+            poc_url=None, provider_id=None, session_timeout=None, sign_alg=None, sign_digest_alg=None, sign_valid_key_store=None, 
+            sign_valid_key_alias=None, sign_assertion=None, sign_auth_rsp=None, sign_arti_req=None, sign_arti_rsp=None, 
+            sign_logout_req=None, sign_logout_rsp=None, sign_name_id_req=None, sign_name_id_rsp=None, validate_auth_req=None,
+            validate_assert=None, validate_arti_req=None, validate_arti_rsp=None, validate_logout_req=None, validate_logout_rsp=None,
+            validate_name_id_req=None, validate_name_id_rsp=None, transform_include_namespace=None, sign_include_pubkey=None,
+            sign_include_cert=None, sign_include_issuer=None, sign_include_ski=None, sign_include_subject=None, sign_keystore=None,
+            sign_key_alias=None, sso_svc_data=[], slo_svc_data=[], alias_svc_db_type=None, alias_svc_ldap_con=None,
+            alias_svc_ldap_base_dn=None, assertion_consume_svc=[], authn_req_delegate_id=None, authn_req_mr=None):
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value_string("protocol", "SAML2_0")
         data.add_value_string("role", role)
         data.add_value_string("templateName", template_name)
 
         encryptionSettings = DataObject()
         signatureSettings = DataObject()
+        assertionSettings = DataObject()
+        nameIdFmt = DataObject()
 
         identityMapping = None
-        if (active_delegate_id is not None):
+        if (identity_delegate_id is not None):
             identityMapping = DataObject()
-            identityMapping.add_value_string("activeDelegateId", active_delegate_id)
+            identityMapping.add_value_string("activeDelegateId", identity_delegate_id)
+            if (identity_mapping_rule is not None):
+                identityMapping.add_value_not_empty("properties", 
+                        {"identityMappingRuleReference": identity_rule_id,
+                         "ruleType": identity_rule_type})
+            else:
+                identProps = DataObject()
+                identProps.add_value_string("appliesTo", identity_applies_to)
+                identProps.add_value_string("authType", identity_auth_type)
+                identProps.add_value_string("basicAuthUsername", identity_ba_user)
+                identProps.add_value_string("basicAuthPassword", identity_ba_password)
+                identProps.add_value_string("clientKeyStore", identity_client_keystore)
+                identProps.add_value_string("clientKeyAlias", identity_client_key_alias)
+                identProps.add_value_string("issuerUri", identity_issuer_uri)
+                identProps.add_value_string("messageFormat", identity_msg_fmt)
+                identProps.add_value_string("sslKeyStore", identity_ssl_keystore)
+                identProps.add_value_string("uri", identity_uri)
+                identityMapping.add_value_not_empty("properties", identProps.data)
+
+        extensionMapping = None
+        if(ext_delegate_id is not None):
+            extensionMapping = DataObject()
+            extensionMapping.add_value_string("activeDelegateId")
+            if ext_mapping_rule is not None:
+                extensionMapping.add_value("properties", {"extensionMappingRuleReference", ext_mapping_rule})
 
         decryptionKeyIdentifier = DataObject()
         decryptionKeyIdentifier.add_value_string("keystore", decrypt_keystore)
         decryptionKeyIdentifier.add_value_string("label", decrypt_key_label)
+
+        encryptionSettings.add_value_not_empty("decryptionKeyIdentifier", decryptionKeyIdentifier.data)
+        signatureSettings.add_value_not_empty("signingKeyIdentifier", signingKeyIdentifier.data)
+        signatureSettings.add_value_string("signatureAlgorithm", sign_alg)
+        signatureSettings.add_value_string("digestAlgorithm", sign_digest_alg)
+        signOpts = DataObject()
+        signOpts.add_value_boolean("signAssertion", sign_assertion)
+        signOpts.add_value_boolean("signAuthnResponse", sign_authn_rsp)
+        signOpts.add_value_boolean("signArtifactRequest", sign_arti_req)
+        signOpts.add_value_boolean("signArtifactResponse", sign_arti_rsp)
+        signOpts.add_value_boolean("signLogoutRequest", sign_logout_req)
+        signOpts.add_value_boolean("signLogoutResponse", sign_logout_rsp)
+        signOpts.add_value_boolean("signNameIDManagementRequest", sign_name_id_req)
+        signOpts.add_value_boolean("signNameIDManagementResponse", sign_name_id_rsp)
+        signatureSettings.add_value_not_empty("signingOptions", signOpts.data)
+
+        validOpts = DataObject()
+        validOpts.add_value_boolean("validateAuthnRequest", validate_auth_req)
+        validOpts.add_value_boolean("validateAssertion", validate_assert)
+        validOpts.add_value_boolean("validateArtifactRequest", validate_arti_req)
+        validOpts.add_value_boolean("validateArtifactResponse", validate_arti_rsp)
+        validOpts.add_value_boolean("validateLogoutRequest", validate_logout_req)
+        validOpts.add_value_boolean("validateLogoutResponse", validate_logout_rsp)
+        validOpts.add_value_boolean("validateNameIDManagementRequest", validate_name_id_req)
+        validOpts.add_value_boolean("validateNameIDManagementResponse", validate_name_id_rsp)
+        signatureSettings.add_value_not_empty("validationOptions", validOpts.data)
+        if transform_include_namespace is not None:
+            signatureSettings.add_value(
+                "transformAlgorithmElements", {"includeInclusiveNamespaces": transform_include_namespace})
+        keyInfo = DataObject()
+        keyInfo.add_value_boolean("includePublicKey", sign_include_pubkey)
+        keyInfo.add_value_boolean("includeX509CertificateData", sign_include_cert)
+        keyInfo.add_value_boolean("includeX509IssuerDetails", sign_include_issuer)
+        keyInfo.add_value_boolean("includeX509SubjectKeyIdentifier", sign_include_ski)
+        keyInfo.add_value_boolean("includeX509SubjectName", sign_include_subject)
+        keyInfo.add_value_boolean("includeX509SubjectName", sign_include_subject)
+        signatureSettings.add_value_not_empty("keyInfoElements", keyInfo.data)
         signingKeyIdentifier = DataObject()
         signingKeyIdentifier.add_value_string("keystore", signing_keystore)
         signingKeyIdentifier.add_value_string("label", signing_key_label)
 
-        encryptionSettings.add_value_not_empty("decryptionKeyIdentifier", decryptionKeyIdentifier.data)
-        signatureSettings.add_value_not_empty("signingKeyIdentifier", signingKeyIdentifier.data)
 
-        ssoServiceBinding = None
-        if (sso_service_binding is not None):
-            ssoServiceBinding = DataObject()
-            ssoServiceBinding.add_value_string("binding", sso_service_binding)
+        if name_id_default is not None or name_id_supported is not None:
+            nameIdFmt.add_value_string("default", name_id_default)
+            nameIdFmt.add_value_not_empty("supported", name_id_supported)
+
+        aliasSvc = DataObject()
+        aliasSvc.add_value_string("aliasServiceDBType", alias_svc_db_type)
+        aliasSvc.add_value_string("aliasServiceLDAPConnection", alias_svc_ldap_con)
+        aliasSvc.add_value_string("aliasServiceLDAPBaseDN", alias_svc_ldap_base_dn)
 
         configuration = DataObject()
+        configuration.add_value_string("accessPolicy", access_policy)
+        configuration.add_value("artifactLifeTime", artifact_lifetime)
+        configuration.add_value_not_empty("assertionConsumerService", assertion_consume_svc)
+        configuration.add_value_not_empty("assertionSettings", assertionSettings.data)
+        configuration.add_value_not_empty("artifactResolutionService", artifact_resolution_service)
+        configuration.add_value_not_empty("attributeMapping", {} if not attribute_mappings else {"map": attribute_mappings})
+        configuration.add_value_string("companyName", company_name)
         configuration.add_value_not_empty("encryptionSettings", encryptionSettings.data)
-        configuration.add_value_not_empty("signatureSettings", signatureSettings.data)
+        configuration.add_value_not_empty("identityMapping", identityMapping.data)
+        configuration.add_value_not_empty("extensionMapping", extensionMapping.data)
+        configuration.add_value_not_empty("manageNameIDService", manage_name_id_services)
+        configuration.add_value("messageValidTime", msg_valid_time)
+        configuration.add_value_string("messageIssuerFormat", msg_issuer_fmt)
+        configuration.add_value_string("messageIssuerNameQualifier", msg_issuer_name_qualifier)
+        configuration.add_value_not_empty("nameIDFormat", nameIdFmt.data)
+        configuration.add_value_boolean("needConsentToFederate", consent_to_federate)
+        configuration.add_value_boolean("excludeSessionIndexInSingleLogoutRequest", exclude_session_index_logout_request)
+        configuration.add_value_string("pointOfContactUrl", poc_url)
         configuration.add_value_string("providerId", provider_id)
-        configuration.add_value_string("pointOfContactUrl", point_of_contact_url)
-        configuration.add_value_string("companyName", company_name)
-        if (ssoServiceBinding is not None):
-            configuration.add_value("singleSignOnService", [ssoServiceBinding.data])
-        if (identityMapping is not None):
-            configuration.add_value("identityMapping", identityMapping.data)
-        configuration.add_value("needConsentToFederate", need_consent_to_federate)
-        configuration.add_value_string("messageIssuerFormat", message_issuer_format)
+        configuration.add_value("sessionTimeout", session_timeout)
+        configuration.add_value_not_empty("signatureSettings", signatureSettings.data)
+        configuration.add_value_not_empty("singleSignOnService", sso_svc_data)
+        configuration.add_value_not_empty("singleLogoutService", slo_svc_data)
+        configuration.add_value_not_empty("aliasServiceSettings", aliasSvc.data)
 
         data.add_value_not_empty("configuration", configuration.data)
-
         response = self.client.post_json(FEDERATIONS, data.data)
         response.success = response.status_code == 201
 
         return response
 
 
-    def create_saml_partner(self, federation_id, name=None, enabled=False, role=None, template_name=None, acs_binding=None, block_encryption_algorithm=None,
-        encryption_key_transport_algorithm = None, encryption_keystore=None, encryption_key_label=None, signature_digest_algorithm=None, acs=None, single_logout_service=None,
-        acs_default=True, acs_index=0, acs_url=None, attribute_mapping=[], active_delegate_id=None, client_auth_method=None, signature_algorithm=None,
-        validate_logout_request=None,validate_logout_response=None,
-        provider_id=None, signature_validation=None, validate_authn_request=None, validation_keystore=None, validation_key_label=None, mapping_rule=None):
+    def create_saml_partner(self, federation_id, name=None, enabled=False, role=None, template_name=None, access_policy=None,
+            arti_resolution_svc=[], assert_consume_svc=[], assert_valid_before=None, assert_valid_after=None, assert_attr_types=[],
+            assert_session_not_after=None, assert_multi_attr_stmt=None, attr_mapping=[], decrypt_key_store=None, 
+            decrypt_key_alias=None, encrypt_block_alg=None, encrypt_transport_alg=None, encrypt_key_store=None, 
+            encrypt_key_alias=None, encrypt_name_id=None, encrypt_assertion=None, encrypt_assertion_attrs=None,
+            identity_delegate_id=None, identity_rule_type='JAVASCRIPT', identity_mr=None, identity_applies_to=None,
+            identity_auth_type=None, identity_ba_user=None, identity_ba_password=None,
+            identity_client_key_store=None, identity_client_key_alias=None, identity_issuer_uri=None, identity_mgs_fmt=None,
+            identity_ssl_key_store=None, identity_uri=None, ext_delegate_id=None, ext_mr=None, include_fed_id_in_partner_id=None, 
+            logout_req_lifetime=None, manage_name_id_services=[], name_id_default=None, name_id_supported=[],
+            provider_id=None, session_timeout=None, sign_include_pub_key=None, sign_include_cert=None, sign_include_issuer=None, 
+            sign_include_ski=None, sign_include_subject=None, sign_key_store=None, sign_key_alias=None, sign_arti_request=None, 
+            sign_arti_rsp=None, sign_assertion=None, sign_authn_rsp=None, sign_logout_req=None, sign_logout_rsp=None, 
+            sign_name_id_req=None, sign_name_id_rsp=None, transform_include_namespace=None, validate_assertion=None, 
+            validate_authn_req=None, validate_arti_req=None, validate_arti_rsp=None, validate_logout_req=None, 
+            validate_logout_rsp=None, validate_name_id_req=None, validate_name_id_rsp=None, sign_alg=None, sign_digest_alg=None, 
+            validation_key_store=None, validation_key_alias=None, slo_svc=[], soap_key_store=None, soap_key_alias=None, 
+            soap_client_auth_method=None, soap_client_auth_ba_user=None, soap_client_auth_ba_password=None, 
+            soap_client_auth_key_store=None, soap_client_auth_key_alias=None, anon_user_name=None, force_authn_to_federate=None, 
+            authn_req_delegate_id=None, authn_req_mr=None, map_unknown_alias=None, sso_svc=[], default_target_url=None):
         
         data = DataObject()
         data.add_value_string("name", name)
         data.add_value("enabled", enabled)
         data.add_value_string("role", role)
         data.add_value_string("templateName", template_name)
 
         attributeMapping = DataObject()
         attributeMapping.add_value_not_empty("map", attribute_mapping)
 
         properties = DataObject()
-
+        properties.add_value_string("username", soap_client_auth_ba_user)
+        properties.add_value_string("password", soap_client_auth_ba_password)
+        properties.add_value_string("keystore", soap_client_auth_key_store)
+        properties.add_value_string("label", soap_client_auth_key_alias)
         clientAuth = DataObject()
-        clientAuth.add_value_string("method", client_auth_method)
+        clientAuth.add_value_string("method", soap_client_auth_method)
         clientAuth.add_value_not_empty("properties", properties.data)
 
         serverCertValidation = DataObject()
-        # serverCertValidation.add_value_string("keystore", "")
+        serverCertValidation.add_value_string("keystore", soap_key_store)
+        serverCertValidation.add_value_string("label", soap_key_alias)
 
         soapSettings = DataObject()
         soapSettings.add_value_not_empty("clientAuth", clientAuth.data)
-        if clientAuth.data or serverCertValidation.data:
-            soapSettings.add_value("serverCertValidation", serverCertValidation.data)
+        soapSettings.add_value_not_empty("serverCertValidation", serverCertValidation.data)
 
         properties = DataObject()
-        properties.add_value_string("identityMappingRule", mapping_rule)
-
+        if identity_mr != None:
+            properties.add_value_string("identityMappingRuleReference", identity_mr)
+            properties.add_value_string("ruleType", identity_rule_type)
+        else:
+            properties.add_value_string("appliesTo", identity_applies_to)
+            properties.add_value_string("authType", identity_auth_type)
+            properties.add_value_string("basicAuthUsername", identity_ba_user)
+            properties.add_value_string("basicAuthPassword", identity_ba_password)
+            properties.add_value_string("clientKeyStore", identity_client_key_store)
+            properties.add_value_string("clientKeyAlias", identity_client_key_alias)
+            properties.add_value_string("issuerUri",identity_issuer_uri)
+            properties.add_value_string("messageFormat", identity_mgs_fmt)
+            properties.add_value_string("sslKeyStore", identity_ssl_key_store)
+            properties.add_value_string("uri", identity_uri)
         identityMapping = DataObject()
         identityMapping.add_value_not_empty("properties", properties.data)
         identityMapping.add_value_string("activeDelegateId", active_delegate_id)
 
-        assertionConsumerService = DataObject()
-        assertionConsumerService.add_value_string("binding", acs_binding)
-        assertionConsumerService.add_value("default", acs_default)
-        assertionConsumerService.add_value("index", acs_index)
-        assertionConsumerService.add_value_string("url", acs_url)
-
         encryptionKeyIdentifier = DataObject()
-        encryptionKeyIdentifier.add_value("keystore", encryption_keystore)
-        encryptionKeyIdentifier.add_value("label", encryption_key_label)
+        encryptionKeyIdentifier.add_value("keystore", encrypt_key_store)
+        encryptionKeyIdentifier.add_value("label", encrypt_key_alias)
+
+        decryptKeyIdent = DataObject()
+        decryptKeyIdent.add_value_string("keystore", decrypt_key_store)
+        decryptKeyIdent.add_value_string("label", decrypt_key_alias)
+
+        encryptionOptions = DataObject()
+        encryptionOptions.add_value_string("encryptNameId", encrypt_name_id)
+        encryptionOptions.add_value_string("encryptAssertion", encrypt_assertion_attrs)
+        encryptionOptions.add_value_string("encryptAssertionAttributes", encrypt_assertion)
 
         encryptionSettings = DataObject()
-        encryptionSettings.add_value_not_empty("encryptionKeyIdentifier", encryptionKeyIdentifier.data)
+        encryptionSettings.add_value_not_empty("decryptionKeyIdentifier", decryptKeyIdent.data)
         encryptionSettings.add_value_string("blockEncryptionAlgorithm", block_encryption_algorithm)
         encryptionSettings.add_value_string("encryptionKeyTransportAlgorithm", encryption_key_transport_algorithm)
+        encryptionSettings.add_value_not_empty("encryptionKeyIdentifier", encryptionKeyIdentifier.data)
+        encryptionSettings.add_value_not_empty("encryptionOptions", encryptionOptions.data)
 
         validationKeyIdentifier = DataObject()
         validationKeyIdentifier.add_value("keystore", validation_keystore)
         validationKeyIdentifier.add_value("label", validation_key_label)
 
         validationOptions = DataObject()
-        validationOptions.add_value("validateAuthnRequest", validate_authn_request)
-        validationOptions.add_value("validateLogoutRequest", validate_logout_request)
-        validationOptions.add_value("validateLogoutResponse", validate_logout_response)
+        validationOptions.add_value_boolean("validateAssertion", validate_assert)
+        validationOptions.add_value_boolean("validateAuthnRequest", validate_authn_request)
+        validationOptions.add_value_boolean("validateArtifactRequest", validate_arti_req)
+        validationOptions.add_value_boolean("validateArtifactResponse",validate_arti_rsp)
+        validationOptions.add_value_boolean("validateLogoutRequest", validate_logout_req)
+        validationOptions.add_value_boolean("validateLogoutResponse", validate_logout_rsp)
+        validationOptions.add_value_boolean("validateNameIDManagementRequest", validate_name_id_req)
+        validationOptions.add_value_boolean("validateNameIDManagementResponse", validate_name_id_rsp)
+
+        transformOptions = DataObject()
+        transformOptions.add_value_boolean("includeInclusiveNamespaces", transform_include_namespace)
+
+        keyInfo = DataObject()
+        keyInfo.add_value_boolean("includePublicKey", sign_include_pub_key)
+        keyInfo.add_value_boolean("includeX509CertificateData", sign_include_cert)
+        keyInfo.add_value_boolean("includeX509IssuerDetails", sign_include_issuer)
+        keyInfo.add_value_boolean("includeX509SubjectKeyIdentifier", sign_include_ski)
+        keyInfo.add_value_boolean("includeX509SubjectName", sign_include_subject)
+
+        signingKeyIdentifier = DataObject()
+        signingKeyIdentifier.add_value_string("keystore", sign_key_store)
+        signingKeyIdentifier.add_value_string("label", sign_key_alias)
+
+        signingOptions = DataObject()
+        signingOptions.add_value_boolean("signArtifactRequest", sign_arti_req)
+        signingOptions.add_value_boolean("signArtifactResponse", sign_arti_rsp)
+        signingOptions.add_value_boolean("signAssertion", sign_assertion)
+        signingOptions.add_value_boolean("signAuthnResponse", sign_authn_rsp)
+        signingOptions.add_value_boolean("signLogoutRequest", sign_logout_req)
+        signingOptions.add_value_boolean("signLogoutResponse", sign_logout_rsp)
+        signingOptions.add_value_boolean("signNameIDManagementRequest", sign_name_id_req)
+        signingOptions.add_value_boolean("signNameIDManagementResponse", sign_name_id_rsp)
 
         signatureSettings = DataObject()
-        signatureSettings.add_value_not_empty("validationOptions", validationOptions.data)
-        signatureSettings.add_value_not_empty("validationKeyIdentifier", validationKeyIdentifier.data)
+        signatureSettings.add_value_not_empty("keyInfoElements", keyInfo.data)
+        signatureSettings.add_value_not_empty("signingKeyIdentifier", signingKeyIdentifier.data)
+        signatureSettings.add_value_not_empty("signingOptions", signingOptions.data)
+        signatureSettings.add_value_not_empty("transformAlgorithmElements", transformOptions.data)
         signatureSettings.add_value_string("signatureAlgorithm", signature_algorithm)
         signatureSettings.add_value_string("digestAlgorithm", signature_digest_algorithm)
+        signatureSettings.add_value_not_empty("validationKeyIdentifier", validationKeyIdentifier.data)
+        signatureSettings.add_value_not_empty("validationOptions", validationOptions.data)
+
+        assertionSettings = DataObject()
+        assertionSettings.add_value("assertionValidBefore", assert_valid_before)
+        assertionSettings.add_value_not_empty("assertionAttributeTypes", assert_attr_types)
+        assertionSettings.add_value("sessionNotOnOrAfter", assert_session_not_after)
+        assertionSettings.add_value_boolean("createMultipleAttributeStatements", assert_multi_attr_stmt)
+
+        extensionMapping = DataObject()
+        extProps = DataObject()
+        extProps.add_value_string("extensionMappingRuleReference", ext_mr)
+        extensionMapping.add_value_string("activeDelegateId", ext_delegate_id)
+        extensionMapping.add_value_not_empty("properties", extProps.data)
+
+        nameIdFmt = DataObject()
+        nameIdFmt.add_value_string("default", name_id_default)
+        nameIdFmt.add_value_not_empty("supported", name_id_supported)
+
+        authnReqMapping = DataObject()
+        authnReqProps = DataObject()
+        authnReqProps.add_value_string("authnReqMappingRuleReference", authn_req_mr)
+        authnReqMapping.add_value_string("activeDelegateId", authn_req_delegate_id)
+        authnReqMapping.add_value_not_empty("properties", authnReqProps.data)
 
         configuration = DataObject()
-        configuration.add_value_not_empty("identityMapping", identityMapping.data)
+        configuration.add_value_string("anonymousUserName", anon_user_name)
+        configuration.add_value_string("accessPolicy", access_policy)
+        configuration.add_value_not_empty("artifactResolutionService", arti_resolution_svc)
+        configuration.add_value_not_empty("assertionConsumerService", assert_consume_svc)
+        configuration.add_value_not_empty("assertionSettings", assertionSettings.data)
         configuration.add_value_not_empty("attributeMapping", attributeMapping.data)
-        configuration.add_value_not_empty("assertionConsumerService", [assertionConsumerService.data])
-        configuration.add_value_not_empty("assertionConsumerService", acs)
-        configuration.add_value_not_empty("singleLogoutService", single_logout_service)
-        configuration.add_value_not_empty("signatureSettings", signatureSettings.data)
         configuration.add_value_not_empty("encryptionSettings", encryptionSettings.data)
-        configuration.add_value_not_empty("soapSettings", soapSettings.data)
+        configuration.add_value_boolean("forceAuthnToFederate", force_authn_to_federate)
+        configuration.add_value_not_empty("identityMapping", identityMapping.data)
+        configuration.add_value_not_empty("extensionMapping", extensionMapping.data)
+        configuration.add_value_not_empty("authnReqMapping", authnReqMapping.data)
+        configuration.add_value_boolean("includeFedIdInAliasPartnerId", include_fed_id_in_partner_id)
+        configuration.add_value("logoutRequestLifeTime", logout_req_lifetime)
+        configuration.add_value_not_empty("manageNameIDService", manage_name_id_services)
+        configuration.add_value_boolean("mapUnknownAlias", map_unknown_alias)
+        configuration.add_value_not_empty("nameIDFormat", nameIdFmt.data)
         configuration.add_value_not_empty("providerId", provider_id)
+        configuration.add_value_not_empty("signatureSettings", signatureSettings.data)
+        configuration.add_value_not_empty("singleLogoutService", single_logout_service)
+        configuration.add_value_not_empty("soapSettings", soapSettings.data)
+        configuration.add_value_string("defaultTargetURL", default_target_url)
 
         data.add_value_not_empty("configuration", configuration.data)
-
         endpoint = "%s%s/partners" % (FEDERATIONS, federation_id)
-
-        print(json.dumps(data.data))
-
         response = self.client.post_json(endpoint, data.data)
         response.success = response.status_code == 201
 
-        return response
+        return response
```

### Comparing `pyisva-0.1.0/pyisva/core/federation/pointofcontact.py` & `pyisva-0.2.0/pyisva/core/federation/pointofcontact.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             Success can be checked by examining the response.success boolean attribute
 
         """
         #TODO
         return
 
 
-    def get_profiles(self):
+    def list_profiles(self):
         """
         Get the list of configured Point of Contact profiles.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
@@ -197,14 +197,37 @@
         endpoint = POC_PROFILES
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
+
+    def get_profile(self, poc_id):
+        """
+        Get a configured Point of Contact profiles.
+
+        Args:
+            poc_id (:obj:`str`): The system-assigned point of contact profile identifier.
+
+        Returns:
+            :obj:`~requests.Response`: The response from verify access. 
+
+            Success can be checked by examining the response.success boolean attribute
+
+            If the request is successful the POC profile is returned as JSON and can be accessed from
+            the response.json attribute
+        """
+
+        endpoint = "{}/{}".format(POC_PROFILES, poc_id)
+        response = self.client.get_json(endpoint)
+        response.success = response.status_code == 200
+        return response
+
+
     def get_current_profile(self):
         """
         Get the active Point of Contact profile.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access.
```

### Comparing `pyisva-0.1.0/pyisva/core/federation/securitytokenservice.py` & `pyisva-0.2.0/pyisva/core/system/sslcertificates.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,329 +3,291 @@
 """
 
 import logging
 
 from pyisva.util.model import DataObject, Response
 from pyisva.util.restclient import RESTClient
 
-STS_BASE = "/iam/access/v8/sts/"
-STS_MODULES = STS_BASE + "modules"
-STS_MODULE_TYPES = STS_BASE + "module-types"
-STS_TEMPLATES = STS_BASE + "templates"
-STS_CHAINS = STS_BASE + "chains"
+
+SSL_CERTIFICATES = "/isam/ssl_certificates"
 
 logger = logging.getLogger(__name__)
 
-class SecurityTokenService(object):
+
+class SSLCertificates(object):
 
     def __init__(self, base_url, username, password):
-        super(SecurityTokenService, self).__init__()
+        super(SSLCertificates, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
-    def get_module_types(self):
+    def import_personal(self, kdb_id, file_path, password=None):
         """
-        Get the list of Security Token Service module types.
+        Import a personal certificate (private key & X509 certificate) into a SSL database
+
+        Args:
+            kdb_id (:obj:`str`): Name of the certificate database.
+            file_path (:obj:`str`): Absolute path to file containing #PKCS12 PKI
+            password (:obj:`str`): Password to unlock personal certificate
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
-
-            If the request is successful the STS module types are returned as JSON and can be accessed from
-            the response.json attribute
         """
+        response = Response()
 
-        endpoint = STS_MODULE_TYPES
+        try:
+            with open(file_path, 'rb') as certificate:
+                data = DataObject()
+                data.add_value_string("operation", "import")
+                data.add_value_string("password", password)
 
-        response = self.client.get_json(endpoint)
-        response.success = response.status_code == 200
+                files = {"cert": certificate}
+
+                endpoint = ("%s/%s/personal_cert" % (SSL_CERTIFICATES, kdb_id))
+
+                response = self.client.post_file(
+                    endpoint, data=data.data, files=files)
+                response.success = response.status_code == 200
+        except IOError as e:
+            logger.error(e)
+            response.success = False
 
         return response
 
-    def get_modules(self):
+    def import_signer(self, kdb_id, file_path, label=None):
         """
-        Get a list of the configured Security Token Service modules.
+        Import a X509 certificate into a SSL database
+
+        Args:
+            kdb_id (:obj:`str`): Name of the certificate database.
+            file_path (:obj:`str`): Absolute path to file containing PEM encoded certificate.
+            label (:obj:`str`): Alias for certificate in SSL database
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
-
-            If the request is successful the STS module are returned as JSON and can be accessed from
-            the response.json attribute
         """
+        response = Response()
 
-        endpoint = STS_MODULES
+        try:
+            with open(file_path, 'rb') as certificate:
+                data = DataObject()
+                data.add_value_string("label", label)
 
-        response = self.client.get_json(endpoint)
-        response.success = response.status_code == 200
+                files = {"cert": certificate}
+
+                endpoint = ("%s/%s/signer_cert" % (SSL_CERTIFICATES, kdb_id))
+
+                response = self.client.post_file(
+                    endpoint, data=data.data, files=files)
+                response.success = response.status_code == 200
+        except IOError as e:
+            logger.error(e)
+            response.success = False
 
         return response
 
 
-    def get_module(self, module_id):
+    def load_signer(self, kdb_id, server=None, port=None, label=None):
         """
-        Get the configuration of A Security Token Service module.
+        Load a X509 certificate from a TLS connection.
 
         Args:
-            module_id (:obj:`str`): The system-assigned STS module ID value.
+            kdb_id (:obj:`str`): Name of the certificate database.
+            server (:obj:`str`): The name or address of the server which holds the server certificate.
+            port (`int`): The port over which the certificate request will be made to the server. 
+            label (:obj:`str`): The label which will be used to identify the certificate within the key file.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the STS module configuration are returned as JSON and can be accessed from
+            If the request is successful the id of the loaded certificate is returned as JSON and can be accessed from
             the response.json attribute
         """
+        data = DataObject()
+        data.add_value_string("operation", "load")
+        data.add_value_string("label", label)
+        data.add_value_string("server", server)
+        data.add_value("port", port)
 
-        endpoint = "%s/%s" % (STS_MODULES, module_id)
+        endpoint = ("%s/%s/signer_cert" % (SSL_CERTIFICATES, kdb_id))
 
-        response = self.client.get_json(endpoint)
+        response = self.client.post_json(endpoint, data.data)
         response.success = response.status_code == 200
 
         return response
 
-
-    def get_templates(self):
+    def get_database(self, kdb_id):
         """
-        Get a list of STS chain templates.
+        Get a SSL certificate database details
+
+        Args:
+            kdb_id (:obj:`str`): Name of the certificate database.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the STS chain templates are returned as JSON and can be accessed from
+            If the request is successful the SSL database details are returned as JSON and can be accessed from
             the response.json attribute
         """
-
-        endpoint = STS_TEMPLATES
+        endpoint = ("%s/%s/details" % (SSL_CERTIFICATES, kdb_id))
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
 
-    def get_template(self, template_id):
+    def list_databases(self):
         """
-        Get a STS cain tempalte.
+        List the SSL databases
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the STS chain template is returned as JSON and can be accessed from
+            If the request is successful the SSL databases are returned as JSON and can be accessed from
             the response.json attribute
         """
-        endpoint = "%s/%s" % (STS_TEMPLATES, template_id)
+        endpoint = SSL_CERTIFICATES
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
 
-    def create_template(self, name, description=None, modules=[]):
-        """
-        Create a STS chain template.
-
-        Args:
-            name (:obj:`str`): A friendly name for the STS Chain Template
-            description (:obj:`str`): A description of the STS Chain Template
-            modules (:obj:`list` of :obj:`str`): An array of the modules that make up the STS Chain Template. Each 
-                        module contains:
-                        - id: The token id of an STS module
-                        - mode: The mode the STS module is used in in the chain. Must be one of the supported 
-                        - modes of the STS module
-                        - prefix: The prefix for the chain item.
-                        example: ``{"id":"default-map","mode":"map","prefix":"uuid3dbf4c6a-013d-15d5-bb8b-c2665e02a402"}``
-
-        Returns:
-            :obj:`~requests.response`: the response from verify access. 
-
-            success can be checked by examining the response.success boolean attribute
-
-            If the request is successful the id of the created template can be acess from the 
-            response.id_from_location attribute
-        """
-        data = DataObject()
-        data.add_value_string("name", name)
-        data.add_value_string("description", description)
-        data.add_value("chainItems", modules)
-
-        response = self.client.post_json(STS_TEMPLATES, data.data)
-        response.success = response.status_code == 201
-
-        return response
-
-
-    def delete_template(self, template_id):
+    def get_personal(self, kdb_id, label=None):
         """
-        Remove a STS template
+        Get the X509 certificate from a personal certificate in a SSL database
 
         Args:
-            template_id (:obj:`str`): The system-assigned STS chain ID value.
-
-        Returns:
-            :obj:`~requests.response`: the response from verify access. 
-
-            success can be checked by examining the response.success boolean attribute
-        """
-        endpoint = "%s/%s" % (STS_TEMPLATES, template_id)
-
-        response = self.client.delete_json(endpoint)
-        response.success = response.status_code == 204
-
-        return response
-
-
-    def get_chains(self):
-        """
-        Get a list of the configured STS chains.
+            kdb_id (:obj:`str`): Name of the certificate database.
+            label (:obj:`str`): Name of the personal certificate to retrieve.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the STS chains are returned as JSON and can be accessed from
+            If the request is successful the certificate is returned as JSON and can be accessed from
             the response.json attribute
         """
-        response = self.client.get_json(STS_CHAINS)
+        endpoint = ("%s/%s/personal_cert" % (SSL_CERTIFICATES, kdb_id))
+
+        if label is not None:
+            endpoint += "/%s" %(label)
+
+        response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
-
-    def get_chain(self, chain_id):
+    def get_signer(self, kdb_id, label=None):
         """
-        Get a configured STS chain.
+        Get a X509 certificate from the lsit of signer certificates.
 
         Args:
-            chain_id (:obj:`str`): The system-assigned STS chain template ID value.
+            kdb_id (:obj:`str`): Name of the certificate database.
+            label (:obj;`str`): Name of the signer certificate.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the STS chain is returned as JSON and can be accessed from
+            If the request is successful the X509 certificate is returned as JSON and can be accessed from
             the response.json attribute
         """
-        endpoint = "%s/%s" % (STS_CHAINS, chain_id)
+        endpoint = ("%s/%s/signer_cert" % (SSL_CERTIFICATES, kdb_id))
+
+        if label is not None:
+            endpoint += "/%s" %(label)
 
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
-    def create_chain(self, name, description=None, template_id=None, request_type=None, token_type=None, xpath=None,
-            sign_responses=None, sign_key_store=None, sign_key_alias=None, sign_include_cert=None, sign_include_pubkey=None, 
-            sign_include_ski=None, sign_include_issuer=None, sign_include_subject=None, validate_requests=None, 
-            validation_key_store=None, validtion_key_alias=None, validation_include_cert=None, validation_include_pubkey=None,
-            validation_include_ski=None, validation_include_issuer=None , validation_include_subject=None, 
-            send_validation_confirmation=None, issuer_address=None, issuer_port_type_namespace=None, issuer_port_type_name=None,
-            issuer_service_namespace=None, issuer_service_name=None, applies_to_address=None, applies_to_port_type_namespace=None, 
-            applies_to_port_type_name=None, applies_to_service_namespace=None, applies_to_service_name=None, 
-            self_properties=[], partner_properties=[]):
+    def create_database(self, kdb_name, db_type=None, token_label=None, passcode=None, hsm_type=None, ip=None, port=None, 
+            kneti_hash=None, esn=None, secondary_ip=None, secondary_port=None, secondary_kneti_hash=None, secondary_esn=None,
+            use_rfs=None, rfs=None, rfs_port=None, rfs_auth=None, update_zip=None, safenet_pw=None):
         """
-        Create a STS chain
+        Create a SSL database
 
         Args:
-            name (:obj:`str`): A friendly name for the STS Chain
-            description (:obj:`str`, optional): A description of the STS Chain
-            template_id (:obj:`str`): The Id of the STS Chain Template that is referenced by this STS Chain
-            request_type (:obj:`str`): The type of request to associate with this chain. The request is one of the types 
-                            that are supported by the WS-Trust specification.
-            token_type (:obj:`str`, optional): The STS module type to map a request message to an STS Chain Template
-            xpath (:obj:`str`, optional): The custom lookup rule in XML Path Language to map a requet message to an STS 
-                            Chain Template
-            sign_responses (`bool`, optional): Whether to sign the Trust Server SOAP response messages.
-            sign_key_store (:obj:`str`, optional): SSL database which contains pribate key to sign messages.
-            sign_key_alias (:obj:`str`, optional): private key to sign messages.
-            sign_include_cert (`bool`, optional): Whether to include the BASE64 encoded certificate data with your 
-                            signature.
-            sign_include_pubkey (`bool`, optional): Whether to include the public key with the signature.
-            sign_include_ski (`bool`, optional): Whether to include the X.509 subject key identifier with the signature
-            sign_include_issuer (`bool`, optional): Whether to include the issuer name and the certificate serial 
-                            number with the signature
-            sign_include_subject (`bool`, optional): Whether to include the subject name with the signature.
-            validate_requests (`bool`, optional): Whether requires a signature on the received SOAP request message 
-                            that contains the RequestSecurityToken message.
-            validation_key_store (:obj:`str`, optional): The SSL database which contains the private key to validate
-                            messages.
-            validtion_key_alias (:obj:`str`, optional): The key to validate the received SOAP request message
-            validation_include_cert (`bool`, optional): Whether the BASE64 encoded certificate data is included with 
-                            the signature.
-            validation_include_pubkey (`bool`, optional):
-            validation_include_ski (`bool`, optional):
-            validation_include_issuer (`bool`, optional): 
-            validation_include_subject (`bool`, optional):
-            send_validation_confirmation (`bool`, optional): Whether to send signature validation confirmation.
-            issuer_address (:obj:`str`): The URI of the issuer company or enterprise
-            issuer_port_type_namespace (:obj:`str`, optional): The namespace URI part of a qualified name for the issuer
-                            Web service port type.
-            issuer_port_type_name (:obj:`str`, optional): The local part of a qualified name for the issuer Web service 
-                            port type.
-            issuer_service_namespace (:obj:`str`, optional): The namespace URI part of a qualified name for the issuer 
-                            Web service.
-            issuer_service_name (:obj:`str`, optional): The local part of a qualified name for the issuer Web service.
-            applies_to_address (:obj:`str`): The URI of the scope company or enterprise
-            applies_to_port_type_namespace (:obj:`str`, optional): The namespace URI part of a qualified name for the scope
-                            Web service port 
-            applies_to_port_type_name (:obj:`str`, optional): The local part of a qualified name for the scope Web 
-                            service port type.
-            applies_to_service_namespace (:obj:`str`, optional): The namespace URI part of a qualified name for the scope
-                            Web service
-            applies_to_service_name (:obj:`str`, optional): The local part of a qualified name for the scope Web service.
-            self_properties (:obj:`list` of :obj:`dict`): The self properties for all modules within the STS Chain Template 
-                            referenced in the STS Chain. A property has the format `{"name":"STS Property","value":["demo","values"]}`
-            partner_properties (:obj:`list` of :obj:`dict`): The partner properties for all modules within the STS Chain Template 
-                            referenced in the STS Chain. A property has the format `{"name":"STS Property","value":["demo","values"]}`
-
-        """
-        data = DataObject()
-        data.add_value_string("name", name)
-        data.add_value_string("description", description)
-        data.add_value_string("chainId", template_id)
-        data.add_value_string("requestType", request_type)
-
-        data.add_value("appliesTo", {"address": applies_to})
-
-        data.add_value("issuer", {"address": issuer})
-
-        data.add_value_boolean("validateRequests", validate_requests)
-        data.add_value_boolean("signResponses", sign_responses)
-        data.add_value_boolean("sendValidationConfirmation", send_validation_confirmation)
-
-
-        data.add_value("properties", {
-            "self": properties
-        })
-
-        response = self.client.post_json(STS_CHAINS, data.data)
-        response.success = response.status_code == 201
-
-        return response
-
-    def delete_chain(self, chain_id):
-        """
-        Delete a STS chain
-
-        Args:
-            chain_id (:obj:`str`): The system-assigned STS chain ID value.
+            kdb_name (:obj:`str`): The new certificate database name that is used to uniquely identify the certificate 
+                            database.
+            db_type (:obj:`str`): The type of the new certificate database. Valid options are "kdb" for local databases 
+                            and "p11" for network databases.
+            token_label (:obj:`str`): The token label of the certificate database.
+            passcode (:obj:`str`): The passcode of the certificate database.
+            hsm_type (:obj:`str`): The type of network HSM device which is being used. Required if the database type is 
+                            "p11". Valid types are "ncipher" or "safenet".
+            ip (:obj:`str`): The IP address of the module. Required if the database type is "p11".
+            port (`int`, optional) :The port of the module. Only valid if the hsm_type is "ncipher".
+            kneti_hash (:obj:`str`, optional): The hash of the KNETI key. Only valid if the hsm_type is "ncipher".
+            esn (:obj:`str`, optional): The Electronic Serial Number (ESN) of the module. Only valid if the hsm_type is 
+                            "ncipher".
+            secondary_ip (:obj:`str`, optional): The IP address of the secondary module. Only valid if the hsm_type is 
+                            "ncipher".
+            secondary_port (`int`, optional): The port of the secondary module. Only valid if the hsm_type is "ncipher"
+            secondary_kneti_hash (:obj:`str`): The hash of the secondary's KNETI key. Only valid if the hsm_type is "ncipher".
+            secondary_esn (:obj:`str`, optional): The Electronic Serial Number (ESN) of the secondary module. Only valid 
+                            if the hsm_type is "ncipher".
+            use_rfs (`bool`, optional): A flag indicating if an RFS will be used. Default is true. Only valid if the 
+                            hsm_type is "ncipher".
+            rfs (:obj:`str`, optional): The IP address of the Remote File System (RFS). Required if the hsm_type is "ncipher" 
+                            and use_rfs is "true".
+            rfs_port (`int`, optional): The port of the Remote File System (RFS). Only valid if the hsm_type is "ncipher".
+            rfs_auth (`bool`, optional): Specifies whether KNETI authentication is used when connecting to the RFS.
+            update_zip (:obj:`str`, optional): A zip file containing local data to be uploaded from the device. Only 
+                            valid if the hsm_type is "ncipher" and use_rfs is "false".
+            safenet_pw (:obj:`str`, optional): The password of the SafeNet device admin account. Only valid if the HSM 
+                            type is "safenet". 
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
+
+            If the request is successful the id of the SSL database is returned as JSON and can be accessed from
+            the response.json attribute
         """
-        endpoint = "%s/%s" % (STS_CHAINS, chain_id)
+        endpoint = SSL_CERTIFICATES
 
-        response = self.client.delete_json(endpoint)
-        response.success = response.status_code == 204
+        data = DataObject()
+        data.add_value_string("kdb_name", kdb_name)
+        data.add_value_string("token_label", token_label)
+        data.add_value_string("passcode", passcode)
+        data.add_value_string("type", db_type)
+        data.add_value_string("token_label", token_label)
+        data.add_value_string("passcode", passcode)
+        data.add_value_string("hsm_type", hsm_type)
+        data.add_value_string("ip", ip)
+        data.add_value("port", port)
+        data.add_value_string("kneti_hash", kneti_hash)
+        data.add_value_string("esn", esn)
+        data.add_value_string("secondary_ip", secondary_ip)
+        data.add_value("secondary_port", secondary_port)
+        data.add_value_string("secondary_kneti_hash", secondary_kneti_hash)
+        data.add_value_string("secondary_esn", secondary_esn)
+        data.add_value_string("use_rfs", use_rfs)
+        data.add_value("rfs", rfs)
+        data.add_value("rfs_port", rfs_port)
+        data.add_value("rfs_auth", rfs_auth)
+        data.add_value_string("safenet_pw", safenet_pw)
 
-        return response
+        if update_zip:
+            raise NotImplementedError
+
+        response = self.client.post_json(endpoint, data.data)
+        response.success = response.status_code == 200
 
+        return response
```

### Comparing `pyisva-0.1.0/pyisva/core/federationsettings.py` & `pyisva-0.2.0/pyisva/core/federationsettings.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,32 +3,35 @@
 """
 
 from .federation.federations import Federations, Federations9040, Federations10000
 from .federation.pointofcontact import PointOfContact
 from .federation.accesspolicy import AccessPolicy
 from .federation.attributesources import AttributeSources
 from .federation.securitytokenservice import SecurityTokenService
+from .federation.aliasservice import AliasService
 
 class Federation9020(object):
     '''
     Object is used to manage the Federations endpoints of a Verify Access deployment.
 
-    :var federations: Create and mnanage Federation and Partners
-    :var attribute_sources: Manage attributes added to identities in federation flows
-    :var sts: Create and manage Security Token Service chains
-    :var poc: Create and manage Point of Contact profiles
-    :var access_policy: Create and manage Access policy rules.
+    :var federations: Create and manage :ref:`Federation<Federations>` and Partners.
+    :var attribute_sources: Manage :ref:`attributes<AttributeSources>` added to identities in federation flows.
+    :var alias_service: Manage user :ref:`aliases<AliasService>` for federated identity sources.
+    :var sts: Create and manage :ref:`Security Token Service<SecurityTokenService>` chains.
+    :var poc: Create and manage :ref:`Point of Contact<PointOfContact>` profiles.
+    :var access_policy: Create and manage :ref:`Access Policy<AccessPolicy>` rules.
     '''
 
     def __init__(self, base_url, username, password):
         super(Federation9020, self).__init__()
         self.federations = Federations(base_url, username, password)
         self.attribute_sources = AttributeSources(base_url, username, password)
         self.sts = SecurityTokenService(base_url, username, password)
 
+
 class Federation9021(Federation9020):
 
     def __init__(self, base_url, username, password):
         super(Federation9021, self).__init__(base_url, username, password)
 
 class Federation9030(Federation9021):
 
@@ -38,14 +41,15 @@
 class Federation9040(Federation9030):
 
     def __init__(self, base_url, username, password):
         super(Federation9040, self).__init__(base_url, username, password)
         self.federations = Federations9040(base_url, username, password)
         self.poc = PointOfContact(base_url, username, password)
         self.access_policy = AccessPolicy(base_url, username, password)
+        self.alias_service = AliasService(base_url, username, password)
 
 
 class Federation9050(Federation9040):
 
     def __init__(self, base_url, username, password):
         super(Federation9050, self).__init__(base_url, username, password)
```

### Comparing `pyisva-0.1.0/pyisva/core/system/adminsettings.py` & `pyisva-0.2.0/pyisva/core/system/adminsettings.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/advancedtuning.py` & `pyisva-0.2.0/pyisva/core/system/advancedtuning.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/clicommands.py` & `pyisva-0.2.0/pyisva/core/system/clicommands.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/cluster.py` & `pyisva-0.2.0/pyisva/core/system/cluster.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/configuration.py` & `pyisva-0.2.0/pyisva/core/system/configuration.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/datetime.py` & `pyisva-0.2.0/pyisva/core/system/datetime.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/dns.py` & `pyisva-0.2.0/pyisva/core/system/dns.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/docker.py` & `pyisva-0.2.0/pyisva/core/system/docker.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/filedownloads.py` & `pyisva-0.2.0/pyisva/core/system/filedownloads.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/firststeps.py` & `pyisva-0.2.0/pyisva/core/system/firststeps.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/fixpacks.py` & `pyisva-0.2.0/pyisva/core/system/fixpacks.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/hostsfile.py` & `pyisva-0.2.0/pyisva/core/system/hostsfile.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/interfaces.py` & `pyisva-0.2.0/pyisva/core/system/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/licensing.py` & `pyisva-0.2.0/pyisva/core/system/licensing.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/managementauthorization.py` & `pyisva-0.2.0/pyisva/core/system/managementauthorization.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/restartshutdown.py` & `pyisva-0.2.0/pyisva/core/system/restartshutdown.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/runtimedb.py` & `pyisva-0.2.0/pyisva/core/system/runtimedb.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/snapshot.py` & `pyisva-0.2.0/pyisva/core/system/snapshot.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/sslcertificates.py` & `pyisva-0.2.0/pyisva/core/web/apiac/authorization_server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,293 +1,299 @@
 """
 @copyright: IBM
 """
 
 import logging
 
-from pyisva.util.model import DataObject, Response
+from pyisva.util.model import DataObject
 from pyisva.util.restclient import RESTClient
 
-
-SSL_CERTIFICATES = "/isam/ssl_certificates"
-
 logger = logging.getLogger(__name__)
 
+API_AUTHZ_SERVER = "/isam/authzserver/"
 
-class SSLCertificates(object):
+class AuthorizationServer(object):
 
     def __init__(self, base_url, username, password):
-        super(SSLCertificates, self).__init__()
+        super(AuthorizationServer, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
-    def import_personal(self, kdb_id, file_path, password=None):
-        """
-        Import a personal certificate (private key & X509 certificate) into a SSL database
+
+    def create_server(self, inst_name, hostname=None, auth_port=None, admin_port=None, domain=None, admin_id=None, 
+               admin_pwd=None, addresses=[], ssl=None, ssl_port=None, keyfile=None, keyfile_label=None):
+        '''
+        Create new API authorization server.
 
         Args:
-            kdb_id (:obj:`str`): Name of the certificate database.
-            file_path (:obj:`str`): Absolute path to file containing #PKCS12 PKI
-            password (:obj:`str`): Password to unlock personal certificate
+            inst_name (:obj:`str`): Name of the instance to be created.
+            hostname (:obj:`str`): The host name of the local host. This name is used when constructing the 
+                                   authorization server name.
+            auth_port (`int`): The port on which authorization requests will be received.
+            admin_port (`int`): The port on which Security Verify Access administration requests will be received.
+            domain (:obj:`str`): The Security Verify Access domain.
+            admin_id (:obj:`str`, optional): The Security Verify Access administrator name. This parameter is optional 
+                                             and will be set to "sec_master" if not specified.
+            admin_pwd (:obj:`str`): The Security Verify Access administrator password.
+            addresses (:obj:`list` of :obj:`str`): A list of local addresses on which the authorization server will 
+                                                   listen for requests.
+            ssl (:obj:`str`): Whether or not to enable SSL between the Security Verify Access authorization server and 
+                                                   the LDAP server. "yes" | "no".
+            ssl_port (`int`): The SSL port on which the LDAP server will be contacted.
+            keyfile (:obj:`str`): The name of the keyfile that will be used when communicating with the LDAP server 
+                                  over SSL.
+            keyfile_label (:obj:`str`): The label of the certificate within the keyfile to use.
 
         Returns:
-            :obj:`~requests.Response`: The response from verify access. 
+            :obj:`~requests.Response`: The response from verify access.
 
             Success can be checked by examining the response.success boolean attribute
-        """
-        response = Response()
 
-        try:
-            with open(file_path, 'rb') as certificate:
-                data = DataObject()
-                data.add_value_string("operation", "import")
-                data.add_value_string("password", password)
+        '''
+        data = DataObject()
 
-                files = {"cert": certificate}
+        endpoint = API_AUTHZ_SERVER + "v1"
+        response = self.client.post_json(endpoint, data.data)
+        response.success = response.status_code == 200
+
+        return response
+
+
+    def update_server(self, inst_name, admin_id=None, admin_pwd=None, operation='renew', force=None):
+        '''
+        Update an API authorization server. This can be used to update the certificate used to communicate with
+        the Verify Access policy server.
+        
+        Args:
+            inst_name (:obj:`str`): Name of the authorization server to update.
+            admin_id (:obj:`str`): The Security Verify Access administrator name.
+            admin_pwd (:obj:`str`): Secret to authenticate as ``admin_id``.
+            operation (:obj:`str`): A flag that is used to indicate the operation to perform. This value is set to 
+                                    "renew" for the renew operation.
+
+        Returns:
+            :obj:`~requests.Response`: The response from verify access.
 
-                endpoint = ("%s/%s/personal_cert" % (SSL_CERTIFICATES, kdb_id))
+            Success can be checked by examining the response.success boolean attribute
 
-                response = self.client.post_file(
-                    endpoint, data=data.data, files=files)
-                response.success = response.status_code == 200
-        except IOError as e:
-            logger.error(e)
-            response.success = False
+        '''
+        data = DataObject()
+        endpoint = API_AUTHZ_SERVER + '{}/v1'.format(inst_name)
+        response = self.client.put_json(endpoint, data.data)
+        response.success = response.status_code == 204
 
         return response
 
-    def import_signer(self, kdb_id, file_path, label=None):
+
+    def delete_server(self, inst_name, admin_id=None, admin_pwd=None, operation='unconfigure', force=None):
         """
-        Import a X509 certificate into a SSL database
+        Delete a configured API Authorization Server.
 
         Args:
-            kdb_id (:obj:`str`): Name of the certificate database.
-            file_path (:obj:`str`): Absolute path to file containing PEM encoded certificate.
-            label (:obj:`str`): Alias for certificate in SSL database
+            inst_name (:obj:`str`): Name of the authorization server to update.
+            admin_id (:obj:`str`): The Security Verify Access administrator name.
+            admin_pwd (:obj:`str`): Secret to authenticate as ``admin_id``.
+            operation (:obj:`str`): A flag that is used to indicate the operation to perform. Accepted value is 
+                                    "unconfigure".
+            force (:obj:`str`): Whether or not to force the unconfiguration of the instance in the event the policy 
+                                server is unreachable. "yes" | "no"
 
         Returns:
-            :obj:`~requests.Response`: The response from verify access. 
+            :obj:`~requests.Response`: The response from verify access.
 
             Success can be checked by examining the response.success boolean attribute
+
         """
-        response = Response()
+        endpoint = API_AUTHZ_SERVER + "{}/v1".format(inst_name)
+        data = dataObject()
+        data.add_value_string("admin_id", admin_id)
+        data.add_value_string("admin_pwd", admin_pwd)
+        data.add_value_string("operation", operation)
+        data.add_value_string("force", force)
+        response = self.client.delete_json(endpoint, data.data)
+        response.success = response.status_code == 204
 
-        try:
-            with open(file_path, 'rb') as certificate:
-                data = DataObject()
-                data.add_value_string("label", label)
+        return response
 
-                files = {"cert": certificate}
 
-                endpoint = ("%s/%s/signer_cert" % (SSL_CERTIFICATES, kdb_id))
+    def list_servers(self):
+        """
+        Get a list of all the configured API Authorization Servers.
 
-                response = self.client.post_file(
-                    endpoint, data=data.data, files=files)
-                response.success = response.status_code == 200
-        except IOError as e:
-            logger.error(e)
-            response.success = False
+        Returns:
+            :obj:`~requests.Response`: The response from verify access.
+
+            Success can be checked by examining the response.success boolean attribute
+
+            If the request is successful a list of the configured API Authorization Servers is returned as JSON
+            and can be accessed from the ``response.json`` property.
+
+        """
+        endpoint = APIAC + "/v1"
+        response = self.client.get_json(endpoint)
+        response.success = response.status_code == 200
 
         return response
 
 
-    def load_signer(self, kdb_id, server=None, port=None, label=None):
+    def add_configuration_stanza_entry(self, instance, stanza=None, entries=[]):
         """
-        Load a X509 certificate from a TLS connection.
+        Add an entry to the configuration properties file of an API Authorization Server.
 
         Args:
-            kdb_id (:obj:`str`): Name of the certificate database.
-            server (:obj:`str`): The name or address of the server which holds the server certificate.
-            port (`int`): The port over which the certificate request will be made to the server. 
-            label (:obj:`str`): The label which will be used to identify the certificate within the key file.
+            instance (:obj:`str`): The API Authorization server instance to modify.
+            stanza (:obj:`str`): The stanza to modify.
+            entries (:obj:`list` of :obj:`dict`): List of entries to add to the stanza. Dictionary is in the
+                                                  format::
+
+                                                            [
+                                                                {"entryName": "value"},
+                                                                {"anotherEntryName": "theValue"}
+                                                            ]
 
         Returns:
-            :obj:`~requests.Response`: The response from verify access. 
+            :obj:`~requests.Response`: The response from verify access.
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the id of the loaded certificate is returned as JSON and can be accessed from
-            the response.json attribute
         """
+        endpoint = API_AUTHZ_SERVER + "{}/configuration/stanza/{}/entry_name/v1".format(instance, stanza)
         data = DataObject()
-        data.add_value_string("operation", "load")
-        data.add_value_string("label", label)
-        data.add_value_string("server", server)
-        data.add_value("port", port)
-
-        endpoint = ("%s/%s/signer_cert" % (SSL_CERTIFICATES, kdb_id))
+        data.add.value("entries", entries)
 
         response = self.client.post_json(endpoint, data.data)
         response.success = response.status_code == 200
 
         return response
 
-    def get_database(self, kdb_id):
+    def delete_configuration_stanza_entry(self, instance, stanza=None, entry_id=None, value=None):
         """
-        Get a SSL certificate database details
+        Remove an entry from a stanza properties file for an API Authorization Server.
 
         Args:
-            kdb_id (:obj:`str`): Name of the certificate database.
+            instance (:obj:`str`): The API Authorization server instance to modify.
+            stanza (:obj:`str`): The stanza to modify.
+            entry_id (:obj:`str`): The entry to remove.
+            value (:obj:`str`): The value of the configuration entry to remove.
 
         Returns:
-            :obj:`~requests.Response`: The response from verify access. 
+            :obj:`~requests.Response`: The response from verify access.
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the SSL database details are returned as JSON and can be accessed from
-            the response.json attribute
         """
-        endpoint = ("%s/%s/details" % (SSL_CERTIFICATES, kdb_id))
-
-        response = self.client.get_json(endpoint)
-        response.success = response.status_code == 200
+        endpoint = API_AUTHZ_SERVER + "{}/configuration/stanza/{}/entry_name/{}/value/{}/v1".format(instance, stanza,
+                                                                                                   entry_id, value)
+        response = self.client.delete_json(endpoint)
+        response.success = response.status_code == 204
 
         return response
 
-
-    def list_databases(self):
+    def update_configuration_stanza_entry(self, instance, stanza=None, entry_id=None, value=None):
         """
-        List the SSL databases
+        Update an entry in a stanza properties file for an API Authorization Server.
+
+        Args:
+            instance (:obj:`str`): The API Authorization server instance to modify.
+            stanza (:obj:`str`): The stanza to modify.
+            entry_id (:obj:`str`): The entry to be updated.
+            value (:obj:`str`): The new value of the configuration entry.
 
         Returns:
-            :obj:`~requests.Response`: The response from verify access. 
+            :obj:`~requests.Response`: The response from verify access.
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the SSL databases are returned as JSON and can be accessed from
-            the response.json attribute
         """
-        endpoint = SSL_CERTIFICATES
+        endpoint = API_AUTHZ_SERVER + "{}/configuration/stanza/{}/entry_name/{}/v1".format(instance, stanza,
+                                                                                            entry_id)
+        data = DataObject()
+        data.add_value_string("value", value)
 
-        response = self.client.get_json(endpoint)
-        response.success = response.status_code == 200
+        response = self.client.put_json(endpoint, data.data)
+        response.success = response.status_code == 204
 
         return response
 
-
-    def get_personal(self, kdb_id, label=None):
+    def get_configuration_stanza_entry(self, instance, stanza=None, entry_id=None):
         """
-        Get the X509 certificate from a personal certificate in a SSL database
+        Get the value of an entry in a stanza properties file for an API Authorization Server.
 
         Args:
-            kdb_id (:obj:`str`): Name of the certificate database.
-            label (:obj:`str`): Name of the personal certificate to retrieve.
+            instance (:obj:`str`): The API Authorization server instance to return.
+            stanza (:obj:`str`): The stanza to get.
+            entry_id (:obj:`str`): The entry to get.
 
         Returns:
-            :obj:`~requests.Response`: The response from verify access. 
+            :obj:`~requests.Response`: The response from verify access.
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the certificate is returned as JSON and can be accessed from
-            the response.json attribute
-        """
-        endpoint = ("%s/%s/personal_cert" % (SSL_CERTIFICATES, kdb_id))
-
-        if label is not None:
-            endpoint += "/%s" %(label)
+            If the request is successful then the entry value is returned as JSON and is available in the 
+            ``response.json`` property.
 
+        """
+        endpoint = API_AUTHZ_SERVER + "{}/configuration/stanza/{}/entry_name/{}/v1".format(instance, stanza, entry_id)
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
-    def get_signer(self, kdb_id, label=None):
+    def add_configuration_stanza(self, instance, stanza=None):
         """
-        Get a X509 certificate from the lsit of signer certificates.
+        Add a stanza to the properties file for an API Authorization Server.
 
         Args:
-            kdb_id (:obj:`str`): Name of the certificate database.
-            label (:obj;`str`): Name of the signer certificate.
+            instance (:obj:`str`): The API Authorization server instance to modify.
+            stanza (:obj:`str`): The stanza to add.
 
         Returns:
-            :obj:`~requests.Response`: The response from verify access. 
+            :obj:`~requests.Response`: The response from verify access.
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the X509 certificate is returned as JSON and can be accessed from
-            the response.json attribute
         """
-        endpoint = ("%s/%s/signer_cert" % (SSL_CERTIFICATES, kdb_id))
-
-        if label is not None:
-            endpoint += "/%s" %(label)
-
-        response = self.client.get_json(endpoint)
+        endpoint = API_AUTHZ_SERVER + "{}/configuration/stanza/{}/v1".format(instance, stanza)
+        response = self.client.post_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
-    def create_database(self, kdb_name, db_type=None, token_label=None, passcode=None, hsm_type=None, ip=None, port=None, 
-            kneti_hash=None, esn=None, secondary_ip=None, secondary_port=None, secondary_kneti_hash=None, secondary_esn=None,
-            use_rfs=None, rfs=None, rfs_port=None, rfs_auth=None, update_zip=None, safenet_pw=None):
+    def delete_configuration_stanza(self, instance, stanza=None):
         """
-        Create a SSL database
+        Delete a stanza from the properties file for an API Authorization Server.
 
         Args:
-            kdb_name (:obj:`str`): The new certificate database name that is used to uniquely identify the certificate 
-                            database.
-            db_type (:obj:`str`): The type of the new certificate database. Valid options are "kdb" for local databases 
-                            and "p11" for network databases.
-            token_label (:obj:`str`): The token label of the certificate database.
-            passcode (:obj:`str`): The passcode of the certificate database.
-            hsm_type (:obj:`str`): The type of network HSM device which is being used. Required if the database type is 
-                            "p11". Valid types are "ncipher" or "safenet".
-            ip (:obj:`str`): The IP address of the module. Required if the database type is "p11".
-            port (`int`, optional) :The port of the module. Only valid if the hsm_type is "ncipher".
-            kneti_hash (:obj:`str`, optional): The hash of the KNETI key. Only valid if the hsm_type is "ncipher".
-            esn (:obj:`str`, optional): The Electronic Serial Number (ESN) of the module. Only valid if the hsm_type is 
-                            "ncipher".
-            secondary_ip (:obj:`str`, optional): The IP address of the secondary module. Only valid if the hsm_type is 
-                            "ncipher".
-            secondary_port (`int`, optional): The port of the secondary module. Only valid if the hsm_type is "ncipher"
-            secondary_kneti_hash (:obj:`str`): The hash of the secondary's KNETI key. Only valid if the hsm_type is "ncipher".
-            secondary_esn (:obj:`str`, optional): The Electronic Serial Number (ESN) of the secondary module. Only valid 
-                            if the hsm_type is "ncipher".
-            use_rfs (`bool`, optional): A flag indicating if an RFS will be used. Default is true. Only valid if the 
-                            hsm_type is "ncipher".
-            rfs (:obj:`str`, optional): The IP address of the Remote File System (RFS). Required if the hsm_type is "ncipher" 
-                            and use_rfs is "true".
-            rfs_port (`int`, optional): The port of the Remote File System (RFS). Only valid if the hsm_type is "ncipher".
-            rfs_auth (`bool`, optional): Specifies whether KNETI authentication is used when connecting to the RFS.
-            update_zip (:obj:`str`, optional): A zip file containing local data to be uploaded from the device. Only 
-                            valid if the hsm_type is "ncipher" and use_rfs is "false".
-            safenet_pw (:obj:`str`, optional): The password of the SafeNet device admin account. Only valid if the HSM 
-                            type is "safenet". 
+            instance (:obj:`str`): The API Authorization server instance to modify.
+            stanza (:obj:`str`): The stanza to remove.
 
         Returns:
-            :obj:`~requests.Response`: The response from verify access. 
+            :obj:`~requests.Response`: The response from verify access.
 
             Success can be checked by examining the response.success boolean attribute
 
-            If the request is successful the id of the SSL database is returned as JSON and can be accessed from
-            the response.json attribute
         """
-        endpoint = SSL_CERTIFICATES
+        endpoint = API_AUTHZ_SERVER + "{}/configuration/stanza/{}/v1".format(instance, stanza)
+        response.success = response.status_code == 204
 
-        data = DataObject()
-        data.add_value_string("kdb_name", kdb_name)
-        data.add_value_string("token_label", token_label)
-        data.add_value_string("passcode", passcode)
-        data.add_value_string("type", db_type)
-        data.add_value_string("token_label", token_label)
-        data.add_value_string("passcode", passcode)
-        data.add_value_string("hsm_type", hsm_type)
-        data.add_value_string("ip", ip)
-        data.add_value("port", port)
-        data.add_value_string("kneti_hash", kneti_hash)
-        data.add_value_string("esn", esn)
-        data.add_value_string("secondary_ip", secondary_ip)
-        data.add_value("secondary_port", secondary_port)
-        data.add_value_string("secondary_kneti_hash", secondary_kneti_hash)
-        data.add_value_string("secondary_esn", secondary_esn)
-        data.add_value_string("use_rfs", use_rfs)
-        data.add_value("rfs", rfs)
-        data.add_value("rfs_port", rfs_port)
-        data.add_value("rfs_auth", rfs_auth)
-        data.add_value_string("safenet_pw", safenet_pw)
+        return response
 
-        if update_zip:
-            raise NotImplementedError
+    def list_configuration_stanza(self, instance):
+        """
+        Get a list of stanza's from the properties file for an API Authorization Server.
 
-        response = self.client.post_json(endpoint, data.data)
+        Args:
+            instance (:obj:`str`): The API Authorization server instance to return.
+
+        Returns:
+            :obj:`~requests.Response`: The response from verify access.
+
+            Success can be checked by examining the response.success boolean attribute
+
+            If the request is successful then the list of stanza are returned as JSON and is available in the 
+            ``response.json`` property.
+
+        """
+        endpoint = API_AUTHZ_SERVER· + "{}/configuration/stanza".format(instance)
+        response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyisva-0.1.0/pyisva/core/system/staticroutes.py` & `pyisva-0.2.0/pyisva/core/system/staticroutes.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/system/sysaccount.py` & `pyisva-0.2.0/pyisva/core/system/sysaccount.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
             Success can be checked by examining the response.success boolean attribute
 
             If the request is successful the id of the updated group is returned as JSON and can be accessed from
             the response.json attribute
         """
         data = DataObject()
-        data.add_alue_string("id", group)
+        data.add_value_string("id", group)
         endpoint = SYSACCOUNT_GROUPS + '/{}/groups/v1'.format(user)
         response = self.client.put_json(endpoint, data.data)
         response.success = response.status_code == 200
 
         return response
 
 
@@ -275,15 +275,15 @@
             password (:obj:`str`): The new password for the user. This can contain any ASCII characters.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
         """
-        endpoint = SYSACCOUNT_GROUPS + '/self/v1'
+        endpoint = SYSACCOUNT + '/self/v1'
         data = DataObject()
         data.add_value_string('old_password', old_password)
         data.add_value_string('password', password)
-        response.self.client.put_json(endpoint, data.data)
+        response = self.client.put_json(endpoint, data.data)
         response.success = response.status_code == 204
 
         return response
```

### Comparing `pyisva-0.1.0/pyisva/core/systemsettings.py` & `pyisva-0.2.0/pyisva/core/systemsettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,34 +19,36 @@
 from .system.runtimedb import RuntimeDb
 from .system.cluster import Cluster
 from .system.docker import Docker
 from .system.fixpacks import Fixpacks
 from .system.sysaccount import SysAccount
 from .system.managementauthorization import ManagementAuthorization
 from .system.snapshot import Snapshot
+from .system.extensions import Extensions
 
 
 class SystemSettings9020(object):
     '''
     Object is used to manage system wide settings for Verify Access
 
     :var advanced_tuning: Create and manage Advanced Tuning Parameters
     :var admin_settings: Manage settings for the LMI
     :var configuration: Manage the staged pending changes
     :var date_time: Update the system data/time settings
-    :var dns: Update the DNS settigns used by Verify Access
+    :var dns: Update the DNS settings used by Verify Access
     :var file_downloads: Fetch files hosted by Verify Access
-    :var first_steps: Complete the fisrt steps of Verify Access configuration and accept the EULA
-    :var hosts_file: Modify the host file used by Verify Access (Applaince only)
-    :var interfaces: Manage the networking interfaces used by Verify Access (Applaicne only)
+    :var first_steps: Complete the first steps of Verify Access configuration and accept the EULA
+    :var hosts_file: Modify the host file used by Verify Access (Appliance only)
+    :var interfaces: Manage the networking interfaces used by Verify Access (Appliance only)
     :var static_routes: Manage the networking gateway settings used by Verify Access
     :var fixpacks: Upload and apply FixPacks generated by support
+    :var extensions: Upload and install Extensions form the IBM App-Xchange.
     :var licensing: Apply license codes to activate Verify Access modules
     :var restartshutdown: Manage the state of Verify Access appliance
-    :var ssl_certificates: Craete and manage the SSL databases used by Verify Access components
+    :var ssl_certificates: Create and manage the SSL databases used by Verify Access components
     :var cli_commands: Use the API interface to run CLI commands
     :var cluster: Manage the cluster configuration (& database configuration).
     '''
 
     def __init__(self, base_url, username, password):
         super(SystemSettings9020, self).__init__()
         self.advanced_tuning = AdvancedTuning(base_url, username, password)
@@ -56,14 +58,15 @@
         self.dns = DNS(base_url, username, password)
         self.file_downloads = FileDownloads(base_url, username, password)
         self.first_steps = FirstSteps(base_url, username, password)
         self.hosts_file = HostsFile(base_url, username, password)
         self.interfaces = Interfaces(base_url, username, password)
         self.static_routes = StaticRoutes(base_url, username, password)
         self.fixpacks = Fixpacks(base_url, username, password)
+        self.extensions = Extensions(base_url, username, password)
         self.licensing = Licensing(base_url, username, password)
         self.restartshutdown = RestartShutdown(base_url, username, password)
         self.ssl_certificates = SSLCertificates(base_url, username, password)
         self.cli_commands = CLICommands(base_url, username, password)
         self.sysaccount = SysAccount(base_url, username, password)
         self.runtime_db = RuntimeDb(base_url, username, password)
         self.cluster = Cluster(base_url, username, password)
@@ -121,17 +124,18 @@
 
 class SystemSettings10000(SystemSettings9080):
 
     def __init__(self, base_url, username, password):
         super(SystemSettings10000, self).__init__(base_url, username, password)
         self.static_routes = StaticRoutes10000(base_url, username, password)
         self.interfaces = Interfaces10000(base_url, username, password)
-        self.managementauthorization = ManagementAuthorization(base_url, username, password)
+        self.mgmt_authorization = ManagementAuthorization(base_url, username, password)
         self.snapshot = Snapshot(base_url, username, password)
 
+
 class SystemSettings10010(SystemSettings10000):
 
     def __init__(self, base_url, username, password):
         super(SystemSettings10010, self).__init__(base_url, username, password)
 
 
 class SystemSettings10020(SystemSettings10010):
@@ -159,11 +163,12 @@
 
 
 class SystemSettings10050(SystemSettings10040):
 
     def __init__(self, base_url, username, password):
             super(SystemSettings10050, self).__init__(base_url, username, password)
 
+
 class SystemSettings10060(SystemSettings10050):
 
     def __init__(self, base_url, username, password):
-            super(SystemSettings10060, self).__init__(base_url, username, password)
+            super(SystemSettings10060, self).__init__(base_url, username, password)
```

### Comparing `pyisva-0.1.0/pyisva/core/web/api_access_control.py` & `pyisva-0.2.0/pyisva/core/web/api_access_control.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/bin/python
 """
 @copyright: IBM
 """
 
 from .apiac.cors import CORS
 from .apiac.policies import Policies
-from .apiac.resources import Resources
+from .apiac.resource_server import ResourceServer
 from .apiac.utilities import Utilities
 from .apiac.document_root import DocumentRoot
 from .apiac.authorization_server import AuthorizationServer
 
 class APIAccessControl(object):
     '''
     Class is resposible for WebSEAL API Access Control endpoints
     '''
 
     def __init__(self, base_url, username, password):
         super(APIAccessControl, self).__init__()
         self.cors = CORS(base_url, username, password)
         self.policies = Policies(base_url, username, password)
-        self.resoures = Resources(base_url, username, password)
+        self.resource_server = ResourceServer(base_url, username, password)
         self.utilities = Utilities(base_url, username, password)
         self.document_root = DocumentRoot(base_url, username, password)
-        self.authz_server = AuthoriztaionServer(base_url, username, password)
+        self.authz_server = AuthorizationServer(base_url, username, password)
```

### Comparing `pyisva-0.1.0/pyisva/core/web/apiac/cors.py` & `pyisva-0.2.0/pyisva/core/web/apiac/cors.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/web/apiac/document_root.py` & `pyisva-0.2.0/pyisva/core/web/apiac/document_root.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/web/apiac/policies.py` & `pyisva-0.2.0/pyisva/core/web/apiac/policies.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/web/apiac/resources.py` & `pyisva-0.2.0/pyisva/core/web/apiac/resource_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,38 +7,39 @@
 from pyisva.util.model import DataObject
 from pyisva.util.restclient import RESTClient
 
 logger = logging.getLogger(__name__)
 
 APIAC = "/wga/apiac"
 
-class Resources(object):
+class ResourceServer(object):
 
     def __init__(self, base_url, username, password):
-        super(Resources, self).__init__()
+        super(ResourceServer, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
 
     def create_server(self, instance, server_hostname=None, junction_point=None, junction_type=None,
             policy_type=None, policy_name=None, authentication_type=None, oauth_introspection_transport=None,
-            oauth_introspection_proxy=None, oauth_introspection_auth_method=None, ouath_introspection_endpoint=None, 
+            oauth_introspection_proxy=None, oauth_introspection_auth_method=None, oauth_introspection_endpoint=None, 
             oauth_introspection_client_id=None, oauth_introspection_client_secret=None, 
             oauth_introspection_client_id_hdr=None, oauth_introspection_token_type_hint=None, 
             oauth_introspection_mapped_id=None, oauth_introspection_external_user=None, 
             oauth_introspection_response_attributes=None, static_response_headers=None, jwt_header_name=None, 
             jwt_certificate=None, jwt_claims=None, description=None, junction_hard_limit=None, 
             junction_soft_limit=None, basic_auth_mode=None, tfim_sso=None, remote_http_header=None, 
-            stateful_junction=None, http2_junction=None, http2_proxy=None, sni_name=None, preserve_cookie=None, cookie_include_path=None, 
-            transparent_path_junction=None, mutual_auth=None, insert_ltpa_cookies=None, insert_session_cookies=None, 
-            request_encoding=None, enable_basic_auth=None, key_label=None, gso_respource_group=None, 
-            junction_cookie_javascript_block=None, client_ip_http=None, version_two_cookies=None, ltpa_keyfile=None, 
-            authz_rules=None, fsso_config_file=None, username=None, password=None, server_uuid=None, server_port=None, 
-            virtual_hostname=None, server_dn=None, server_cn=None, local_ip=None, query_contents=None, case_sensitive_url=None, 
-            windows_style_url=None, ltpa_keyfile_password=None, https_port=None, http_port=None, proxy_hostname=None, 
-            proxy_port=None, sms_environment=None, vhost_label=None, force=None, delegation_support=None, scripting_support=None):
+            stateful_junction=None, http2_junction=None, http2_proxy=None, sni_name=None, preserve_cookie=None, 
+            cookie_include_path=None, transparent_path_junction=None, mutual_auth=None, insert_ltpa_cookies=None, 
+            insert_session_cookies=None, request_encoding=None, enable_basic_auth=None, key_label=None, 
+            gso_resource_group=None, junction_cookie_javascript_block=None, client_ip_http=None, 
+            version_two_cookies=None, ltpa_keyfile=None, authz_rules=None, fsso_config_file=None, username=None, 
+            password=None, server_uuid=None, server_port=None, virtual_hostname=None, server_dn=None, server_cn=None, 
+            local_ip=None, query_contents=None, case_sensitive_url=None, windows_style_url=None, 
+            ltpa_keyfile_password=None, https_port=None, http_port=None, proxy_hostname=None, proxy_port=None, 
+            sms_environment=None, vhost_label=None, force=None, delegation_support=None, scripting_support=None):
         '''
         Create a new API Access Control resource server.
 
         Args:
             instance (:obj:`str`): Name of webseal instance being configured.
             server_hostname (:obj:`str`): The DNS host name or IP address of the target back-end server.
             junction_point (:obj:`str`): Name of the location in the Reverse Proxy namespace where the root of the 
@@ -51,15 +52,15 @@
             oauth_introspection_proxy (:obj:`str`): The proxy, if any, used to reach the introspection endpoint.
             oauth_introspection_auth_method (:obj:`str`): The method for passing the authentication data to the 
                         introspection endpoint.
             oauth_introspection_endpoint (:obj:`str`): This is the introspection endpoint which will be called to handle 
                         the token introspection.
             oauth_introspection_client_id (:obj:`str`): The client identifier which is used for OAuth introspection 
                         authentication.
-            oauth_introspection_client_secet (:obj:`str`): The client secret which is used for OAuth introspection 
+            oauth_introspection_client_secret (:obj:`str`): The client secret which is used for OAuth introspection 
                         authentication.
             oauth_introspection_client_id_hdr (:obj:`str`): The name of the HTTP header which contains the client 
                         identifier which is used to authenticate to the introspection endpoint.
             oauth_introspection_token_type_hint (:obj:`str`): A hint about the type of the token submitted for introspection.
             oauth_introspection_mapped_id (:obj:`str`): A formatted string which is used to construct the Verify Access 
                         principal name from elements of the introspection response. 
             oauth_introspection_external_user (bool): A boolean which is used to indicate whether the mapped identity 
@@ -67,15 +68,15 @@
             oauth_introspection_response_attributes (:obj:`list` of :obj:`dict`): A list of rules indicating which parts 
                         of the json response should be added to the credential. 
                         eg: ``{"pos":1,"action":"put","attribute":"givenName"}``
             static_response_headers (:obj:`list` of :obj:`dict`): A list of header names and values that should be 
                         added to the HTTP response. eg: ``{"name":"HeaderName","value":"HeaderValue"}``
             jwt_header_name (:obj:`str`): The name of the HTTP header that will contain the JWT.
             jwt_certificate (:obj:`str`): The label of the personal certificate that will sign the JWT.
-            jwt_claims (:obj:`str`): The list of claims to add to the JWT.
+            jwt_claims (:obj:`list` of :obj:`dict`): The list of claims to add to the JWT.
             description (:obj:`str`, optional): An optional description for this junction.
             junction_hard_limit (:obj:`str`): Defines the hard limit percentage for consumption of worker threads. 
                         Valid value is an integer from "0" to "100".
             junction_soft_limit (:obj:`str`): Defines the soft limit percentage for consumption of worker threads.
             basic_auth_mode (:obj:`str`): Defines how the Reverse Proxy server passes client identity information in 
                         HTTP basic authentication (BA) headers to the back-end server. 
             tfim_sso (:obj:`str`): Enables IBM Security Federated Identity Manager single sign-on.
@@ -93,15 +94,15 @@
                         Proxy server and a back-end Reverse Proxy server over SSL.
             insert_ltpa_cookies (:obj:`str`): Controls whether LTPA cookies are passed to the junctioned Web server.
             insert_session_cookies (:obj:`str`): Controls whether to send the session cookie to the junctioned Web server.
             request_encoding (:obj:`str`): Specifies the encoding to use when the system generates HTTP headers for junctions.
             enable_basic_auth (:obj:`str`): Specifies whether to use BA header information to authenticate to back-end server.
             key_label (:obj:`str`): The key label for the client-side certificate that is used when the system 
                         authenticates to the junctioned Web server.
-            gso_respource_group (:obj:`str`): The name of the GSO resource or resource group.
+            gso_resource_group (:obj:`str`): The name of the GSO resource or resource group.
             junction_cookie_javascript_block (:obj:`str`): Controls the junction cookie JavaScript block.
             client_ip_http (:obj:`str`): Specifies whether to insert the IP address of the incoming request into an 
                         HTTP header for transmission to the junctioned Web server.
             version_two_cookies (:obj:`str`): Specifies whether LTPA version 2 cookies (LtpaToken2) are used.
             ltpa_keyfile (:obj:`str`): Location of the key file that is used to encrypt the LTPA cookie data.
             authz_rules (:obj:`str`): Specifies whether to allow denied requests and failure reason information from 
                         authorization rules to be sent in the Boolean Rule header (AM_AZN_FAILURE) across the junction.
@@ -139,15 +140,15 @@
 
             Success can be checked by examining the response.success boolean attribute
 
         '''
         data = DataObject()
         data.add_value_string("server_hostname", server_hostname)
         data.add_value_string("junction_point", junction_point)
-        data.add_value_string("juncton_type", junction_type)
+        data.add_value_string("junction_type", junction_type)
         policy = DataObject()
         policy.add_value_string("name", policy_name)
         policy.add_value_string("type", policy_type)
         data.add_value_not_empty("policy", policy.data)
         authentication = DataObject()
         authentication.add_value_string("type", authentication_type)
         oauth_introspection = DataObject()
@@ -164,16 +165,16 @@
         oauth_introspection.add_value_not_empty("response_attributes", oauth_introspection_response_attributes)
         authentication.add_value_string("oauth_introspection", oauth_introspection.data)
         data.add_value_not_empty("authentication", authentication.data)
         data.add_value_not_empty("static_response_headers", static_response_headers)
         jwt = DataObject()
         jwt.add_value_string("header_name", jwt_header_name)
         jwt.add_value_string("certificate", jwt_certificate)
-        jwt.add_vaue_not_empty("claims", jwt_claims)
-        data.add_vaule_not_empty("jwt", jwt.data)
+        jwt.add_value_not_empty("claims", jwt_claims)
+        data.add_value_not_empty("jwt", jwt.data)
         data.add_value_string("description", description)
         data.add_value_string("junction_hard_limit", junction_hard_limit)
         data.add_value_string("junction_soft_limit", junction_soft_limit)
         data.add_value_string("basic_auth_mode", basic_auth_mode)
         data.add_value_string("tfim_sso", tfim_sso)
         data.add_value_not_empty("remote_http_header", remote_http_header)
         data.add_value_string("stateful_junction", stateful_junction)
@@ -221,45 +222,45 @@
         response = self.client.post_json(endpoint, data.data)
         response.success = response.status_code == 200
 
         return response
 
 
     def update_server(self, instance, resource_server, server_type="standard", server_hostname=None, 
-            junction_point=None, junction_type=None, policyi_type=None, policy_name=None, 
-            authenticationi_type=None, authentication_oauth_introspection=None,
+            junction_point=None, junction_type=None, policy_type=None, policy_name=None, 
+            authentication_type=None, authentication_oauth_introspection=None,
             static_response_headers=None, jwt_header_name=None, jwt_certificate=None, jwt_claims=None, description=None,
             junction_hard_limit=None, junction_soft_limit=None, basic_auth_mode=None, tfim_sso=None, 
             remote_http_header=None, stateful_junction=None, http2_junction=None, sni_name=None, 
             preserve_cookie=None, cookie_include_path=None, transparent_path_junction=None, mutual_auth=None,
             insert_ltpa_cookies=None, insert_session_cookies=None, request_encoding=None, enable_basic_auth=None,
-            key_label=None, gso_respource_group=None, junction_cookie_javascript_block=None, client_ip_http=None,
+            key_label=None, gso_resource_group=None, junction_cookie_javascript_block=None, client_ip_http=None,
             version_two_cookies=None, ltpa_keyfile=None, authz_rules=None, fsso_config_file=None, username=None,
             password=None, server_uuid=None, server_port=None, virtual_hostname=None, server_dn=None, server_cn=None,
             local_ip=None, query_contents=None, case_sensitive_url=None, windows_style_url=None,
             ltpa_keyfile_password=None, https_port=None, http_port=None, proxy_hostname=None, proxy_port=None,
             sms_environment=None, vhost_label=None, force=None, delegation_support=None, scripting_support=None):
         data = DataObject()
         data.add_value_string("server_hostname", server_hostname)
         data.add_value_string("junction_point", junction_point)
-        data.add_value_string("juncton_type", junction_type)
+        data.add_value_string("junction_type", junction_type)
         policy = DataObject()
         policy.add_value_string("name", policy_name)
         policy.add_value_string("type", policy_type)
         data.add_value_not_empty("policy", policy.data)
         authentication = DataObject()
         authentication.add_value_string("type", authentication_type)
         authentication.add_value_string("oauth_introspection", authentication_oauth_introspection)
         data.add_value_not_empty("authentication", authentication)
         data.add_value_not_empty("static_response_headers", static_response_headers)
         jwt = DataObject()
         jwt.add_value_string("header_name", jwt_header_name)
         jwt.add_value_string("certificate", jwt_certificate)
-        jwt.add_vaue_not_empty("claims", jwt_claims)
-        data.add_vaule_not_empty("jwt", jwt.data)
+        jwt.add_value_not_empty("claims", jwt_claims)
+        data.add_value_not_empty("jwt", jwt.data)
         data.add_value_string("description", description)
         data.add_value_string("junction_hard_limit", junction_hard_limit)
         data.add_value_string("junction_soft_limit", junction_soft_limit)
         data.add_value_string("basic_auth_mode", basic_auth_mode)
         data.add_value_string("tfim_sso", tfim_sso)
         data.add_value_not_empty("remote_http_header", remote_http_header)
         data.add_value_string("stateful_junction", stateful_junction)
@@ -331,15 +332,15 @@
         endpoint = APIAC + "/resource/instance/{}/server".format(instance)
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
 
         return response
 
 
-    def create(self, instance, resource_server, server_type=None, method=None, path=None, 
+    def create_resource(self, instance, resource_server, server_type=None, method=None, path=None, 
             name=None, policy_type=None, policy_name=None, static_response_headers=None, 
             rate_limiting_policy=None, url_aliases=None, documentation_content_type=None, 
             documentation_file=None):
         data = DataObject()
         data.add_value_string("method", method)
         data.add_value_string("path", path)
         data.add_value_string("name", name)
@@ -349,26 +350,26 @@
         data.add_value_not_empty("policy", policy.data)
         data.add_value_not_empty("static_response_headers", static_response_headers)
         data.add_value_string("rate_limiting_policy", rate_limiting_policy)
         data.add_value_not_empty("url_aliases", url_aliases)
         documentation = DataObject()
         documentation.add_value_string("content_type", documentation_content_type)
         documentation.add_value_string("file", documentation_file)
-        data.add_alue_not_empty("documentation", documentation.data)
+        data.add_value_not_empty("documentation", documentation.data)
         if not server_type:
             server_type = "standard"
         endpoint = APIAC + "/resource/instance/{}/server/{}/resource?server_type={}".format(
                 instance, resource_server, server_type)
         response = self.client.post_json(endpoint, data.data)
         response.success = response.status_code == 200
 
         return response
 
 
-    def update(self, instance, resource_server, resource_name=None, server_type="standard", 
+    def update_resource(self, instance, resource_server, resource_name=None, server_type="standard", 
             method=None, path=None, name=None, policy_type=None, policy_name=None, 
             static_response_headers=None, rate_limiting_policy=None, url_aliases=None, 
             documentation_content_type=None, documentation_file=None):
         data = DataObject()
         data.add_value_string("method", method)
         data.add_value_string("path", path)
         data.add_value_string("name", name)
@@ -378,39 +379,39 @@
         data.add_value_not_empty("policy", policy.daita)
         data.add_value_not_empty("static_response_headers", static_response_headers)
         data.add_value_string("rate_limiting_policy", rate_limiting_policy)
         data.add_value_not_empty("url_aliases", url_aliases)
         documentation = DataObject()
         documentation.add_value_string("content_type", documentation_content_type)
         documentation.add_value_string("file", documentation_file)
-        data.add_alue_not_empty("documentation", documentation.data)
+        data.add_value_not_empty("documentation", documentation.data)
 
         endpoint = APIAC + "/resource/instance/{}/server/{}/resource/{}?server_type={}".format(
                 instance, resource_server, resource_name, server_type)
         response = self.client.put_json(endpoint, data.data)
         response.success = response.status_code == 200
 
         return response
 
 
-    def get(self, instance=None, resource_server=None, resource_name=None, server_type="standard"):
+    def get_resource(self, instance=None, resource_server=None, resource_name=None, server_type="standard"):
         endpoint = APIAC + "/resource/instance/{}/server/{}/resource/{}?server_type={}".format(
                 instance, resource_server, resource_name, server_type)
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
         return response
 
 
-    def delete(self, instance=None, resource_server=None, resource_name=None, server_type="standard"):
+    def delete_resource(self, instance=None, resource_server=None, resource_name=None, server_type="standard"):
         endpoint = APIAC + "/resource/instance/{}/server/{}/resource/{}?server_type={}".format(
                 instance, resource_server, resource_name, server_type)
         response = self.client.delete_json(endpoint)
         response.success = response.status_code == 200
         return response
 
 
-    def list(self, instance=None, resource_server=None, server_type="standard"):
+    def list_resources(self, instance=None, resource_server=None, server_type="standard"):
         endpoint = APIAC + "/resource/instance/{}/server/{}/resource?server_type={}".format(
                 instance, resource_server, server_type)
         response = self.client.get_json(endpoint)
         response.success = response.status_code == 200
         return response
```

### Comparing `pyisva-0.1.0/pyisva/core/web/apiac/utilities.py` & `pyisva-0.2.0/pyisva/core/web/apiac/utilities.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/web/clientcertmapping.py` & `pyisva-0.2.0/pyisva/core/web/clientcertmapping.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/web/dscadmin.py` & `pyisva-0.2.0/pyisva/core/web/dscadmin.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/web/fsso.py` & `pyisva-0.2.0/pyisva/core/web/fsso.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/web/httptransform.py` & `pyisva-0.2.0/pyisva/core/web/httptransform.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/web/junctionmapping.py` & `pyisva-0.2.0/pyisva/core/web/junctionmapping.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/web/kerberos.py` & `pyisva-0.2.0/pyisva/core/web/kerberos.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/web/passwordstrength.py` & `pyisva-0.2.0/pyisva/core/web/passwordstrength.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/web/policyadmin.py` & `pyisva-0.2.0/pyisva/core/web/policyadmin.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/web/ratelimit.py` & `pyisva-0.2.0/pyisva/core/web/ratelimit.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/web/reverseproxy.py` & `pyisva-0.2.0/pyisva/core/web/reverseproxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,16 +331,15 @@
 
             If the request is successful the id of the created stanza is returned as JSON and can be accessed from
             the response.json attribute
 
         '''
         endpoint = ("%s/%s/configuration/stanza/%s"
                     % (REVERSEPROXY, webseal_id, stanza_id))
-
-        response = self.client.post_json(endpoint, data=data)
+        response = self.client.post_json(endpoint)
         response.success = response.status_code == 200
 
 
     def delete_configuration_stanza(self, webseal_id, stanza_id):
         '''
         Remove a configuration stanza if it exists.
 
@@ -353,15 +352,15 @@
 
             Success can be checked by examining the response.success boolean attribute
 
         '''
         endpoint = ("%s/%s/configuration/stanza/%s"
                     % (REVERSEPROXY, webseal_id, stanza_id))
 
-        response = self.client.delete_json(endpoint, data=data)
+        response = self.client.delete_json(endpoint)
         response.success = response.status_code == 204
 
 
     def add_configuration_stanza_entry(self, webseal_id, stanza_id, entry_name, value):
         '''
         Add a configuration entry to a stanza.
 
@@ -376,20 +375,19 @@
 
             Success can be checked by examining the response.success boolean attribute
 
             If the request is successful the configuration entry id is returned as JSON and can be accessed from
             the response.json attribute
 
         '''
-        data = {"entries": [[str(entry_name), str(value)]]}
-
+        data = DataObject()
+        data.add_value("entries", [[str(entry_name), str(value)]])
         endpoint = ("%s/%s/configuration/stanza/%s/entry_name"
                     % (REVERSEPROXY, webseal_id, stanza_id))
-
-        response = self.client.post_json(endpoint, data=data)
+        response = self.client.post_json(endpoint, data=data.data)
         response.success = response.status_code == 200
 
         return response
 
 
     def delete_configuration_stanza_entry(self, webseal_id, stanza_id, entry_name, value=None):
         '''
```

### Comparing `pyisva-0.1.0/pyisva/core/web/rsa.py` & `pyisva-0.2.0/pyisva/core/web/rsa.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,34 +15,36 @@
 class RSA(object):
 
     def __init__(self, base_url, username, password):
         super(RSA, self).__init__()
         self.client = RESTClient(base_url, username, password)
 
 
-    def create(self, server_config_file=None):
+    def create(self, server_config_file=None, server_options_file=None):
         """
         Configure WebSEAL to use a RSA token server for authentication.
 
         Args:
             server_config_file (:obj:`str`): Full path to RSA SecurID toke server configuration file.
+            server_options_file (:obj:`str`, optional): Full path to the server configuration options file to upload.
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
         """
         response = Response()
         endpoint = RSA_CONFIG + "/server_config"
         try:
-            with open(server_config_file, "r") as server_config:
-                files = {"server_config": server_config}
-                response = self.client.post_file(endpoint, files=files)
-                response.success = response.status_code == 200
+            files = {"server_config": open(server_config_file, "rb")}
+            if server_options_file:
+                files.update({"server_opts_file": open(server_options_file, 'rb')})
+            response = self.client.post_file(endpoint, files=files)
+            response.success = response.status_code == 200
         except IOError as e:
             logger.error(e)
             response.success = False
 
         return response
 
     def get(self):
@@ -66,15 +68,15 @@
 
     def test(self, username=None, password=None):
         """
         Test the RSA SecurID configuration.
 
         Args:
             username (:obj:`str`): The username to authenticate as
-            password (:obj:`str`): THe passcode of the user to authenticate with
+            password (:obj:`str`): The passcode of the user to authenticate with
 
         Returns:
             :obj:`~requests.Response`: The response from verify access. 
 
             Success can be checked by examining the response.success boolean attribute
 
         """
```

### Comparing `pyisva-0.1.0/pyisva/core/web/urlmapping.py` & `pyisva-0.2.0/pyisva/core/web/urlmapping.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/web/usermapping.py` & `pyisva-0.2.0/pyisva/core/web/usermapping.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/core/websettings.py` & `pyisva-0.2.0/pyisva/core/websettings.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/factory.py` & `pyisva-0.2.0/pyisva/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 class AuthenticationError(Exception):
     pass
 
 
 class Factory(object):
     """
-    The Factory class is used to initalise a singleton "appliance" object which cna be use for all subsequent API 
+    The Factory class is used to initialise a singleton "appliance" object which can be use for all subsequent API 
     requests.
 
     The factory has getter methods for the three modules: WebSEAL, Advanced Access Control; and Federation. It also 
     getter methods for the system and diagnostics API.
 
     Finally this class has helper methods to determine if the IBM Security Verify Access deployment is an appliance
     or container deployment model.
```

### Comparing `pyisva-0.1.0/pyisva/util/model.py` & `pyisva-0.2.0/pyisva/util/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
         return str(self.data)
 
     def add_value(self, key, value):
         if value is not None:
             self.data[key] = value
 
     def add_value_boolean(self, key, value):
+        if value == None:
+            return
         if value is True:
             self.data[key] = True
         else:
             self.data[key] = False
 
     def add_value_not_empty(self, key, value):
         if value:
```

### Comparing `pyisva-0.1.0/pyisva/util/policies.py` & `pyisva-0.2.0/pyisva/util/policies.py`

 * *Files identical despite different names*

### Comparing `pyisva-0.1.0/pyisva/util/restclient.py` & `pyisva-0.2.0/pyisva/util/restclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,22 +110,22 @@
 
         response = self._build_response(r)
         r.close()
 
         return response
 
     def post_file(
-            self, endpoint, accept_type="application/json", data="", files={}):
+            self, endpoint, accept_type="application/json", data="", files={}, parameters=None):
         url = self._base_url + endpoint
         headers = self._get_headers(accept_type)
 
         self._log_request("POST", url, headers)
 
         r = requests.post(
-            url=url, headers=headers, data=data, files=files, verify=False)
+            url=url, headers=headers, data=data, files=files, params=parameters, verify=False)
 
         self._log_response(r.status_code, r.headers, r.content)
 
         response = self._build_response(r)
         r.close()
 
         return response
@@ -152,14 +152,31 @@
 
         return response
 
     def put_json(self, endpoint, data=""):
         return self.put(
             endpoint, accept_type="application/json", data=json.dumps(data))
 
+    def put_file(
+            self, endpoint, accept_type="application/json", data="", files={}, parameters=None):
+        url = self._base_url + endpoint
+        headers = self._get_headers(accept_type)
+
+        self._log_request("PUT", url, headers)
+
+        r = requests.put(
+            url=url, headers=headers, data=data, files=files, params=parameters, verify=False)
+
+        self._log_response(r.status_code, r.headers, r.content)
+
+        response = self._build_response(r)
+        r.close()
+
+        return response
+
     def _build_response(self, request_response):
         response = Response()
         try:
             response.data = request_response.content.decode()
         except (UnicodeDecodeError, AttributeError):
             response.data = request_response.content
         response.status_code = request_response.status_code
```

### Comparing `pyisva-0.1.0/pyisva.egg-info/SOURCES.txt` & `pyisva-0.2.0/pyisva.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,29 @@
+.deploy.sh
+.gitignore
+.travis.yml
 AUTHORS.md
+CONTRIBUTING.md
 LICENSE.txt
 README.md
+dev-requirements.txt
 setup.py
+.github/workflows/main.yaml
+.tests/unit_test.sh
+.tests/core/sys/versions
+docs/Makefile
+docs/accesscontrol.rst
+docs/analysisdiagnostics.rst
+docs/conf.py
+docs/factory.rst
+docs/federation.rst
+docs/index.rst
+docs/make.bat
+docs/systemsettings.rst
+docs/websettings.rst
 pyisva/__init__.py
 pyisva/factory.py
 pyisva.egg-info/PKG-INFO
 pyisva.egg-info/SOURCES.txt
 pyisva.egg-info/dependency_links.txt
 pyisva.egg-info/not-zip-safe
 pyisva.egg-info/requires.txt
@@ -22,38 +40,41 @@
 pyisva/core/access/apiprotection.py
 pyisva/core/access/attributes.py
 pyisva/core/access/authentication.py
 pyisva/core/access/fido2config.py
 pyisva/core/access/fido2registrations.py
 pyisva/core/access/mappingrules.py
 pyisva/core/access/mmfaconfig.py
+pyisva/core/access/pip.py
 pyisva/core/access/pushnotification.py
 pyisva/core/access/riskprofiles.py
 pyisva/core/access/runtimeparameters.py
 pyisva/core/access/scimconfig.py
 pyisva/core/access/serverconnections.py
 pyisva/core/access/templatefiles.py
 pyisva/core/access/userregistry.py
 pyisva/core/analysis/__init__.py
 pyisva/core/analysis/applicationlog.py
 pyisva/core/federation/__init__.py
 pyisva/core/federation/accesspolicy.py
+pyisva/core/federation/aliasservice.py
 pyisva/core/federation/attributesources.py
 pyisva/core/federation/federations.py
 pyisva/core/federation/pointofcontact.py
 pyisva/core/federation/securitytokenservice.py
 pyisva/core/system/__init__.py
 pyisva/core/system/adminsettings.py
 pyisva/core/system/advancedtuning.py
 pyisva/core/system/clicommands.py
 pyisva/core/system/cluster.py
 pyisva/core/system/configuration.py
 pyisva/core/system/datetime.py
 pyisva/core/system/dns.py
 pyisva/core/system/docker.py
+pyisva/core/system/extensions.py
 pyisva/core/system/filedownloads.py
 pyisva/core/system/firststeps.py
 pyisva/core/system/fixpacks.py
 pyisva/core/system/hostsfile.py
 pyisva/core/system/interfaces.py
 pyisva/core/system/licensing.py
 pyisva/core/system/managementauthorization.py
@@ -80,13 +101,13 @@
 pyisva/core/web/urlmapping.py
 pyisva/core/web/usermapping.py
 pyisva/core/web/apiac/__init__.py
 pyisva/core/web/apiac/authorization_server.py
 pyisva/core/web/apiac/cors.py
 pyisva/core/web/apiac/document_root.py
 pyisva/core/web/apiac/policies.py
-pyisva/core/web/apiac/resources.py
+pyisva/core/web/apiac/resource_server.py
 pyisva/core/web/apiac/utilities.py
 pyisva/util/__init__.py
 pyisva/util/model.py
 pyisva/util/policies.py
 pyisva/util/restclient.py
```

