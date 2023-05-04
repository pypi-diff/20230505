# Comparing `tmp/verify_access_autoconf-0.1.0.tar.gz` & `tmp/verify_access_autoconf-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verify_access_autoconf-0.1.0.tar", last modified: Fri Apr  7 07:19:40 2023, max compression
+gzip compressed data, was "verify_access_autoconf-0.3.0.tar", last modified: Thu May  4 23:31:13 2023, max compression
```

## Comparing `verify_access_autoconf-0.1.0.tar` & `verify_access_autoconf-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,61 @@
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-04-07 07:19:40.264891 verify_access_autoconf-0.1.0/
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)      553 2023-04-07 07:16:51.000000 verify_access_autoconf-0.1.0/LICENCE.md
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)      338 2023-04-07 07:19:40.263891 verify_access_autoconf-0.1.0/PKG-INFO
--rw-rw-r--   0 lowkey    (1000) lowkey    (1000)     4157 2023-01-11 23:25:00.000000 verify_access_autoconf-0.1.0/README.md
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)       38 2023-04-07 07:19:40.264891 verify_access_autoconf-0.1.0/setup.cfg
--rw-rw-r--   0 lowkey    (1000) lowkey    (1000)     1621 2023-04-07 07:19:23.000000 verify_access_autoconf-0.1.0/setup.py
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-04-07 07:19:40.258891 verify_access_autoconf-0.1.0/src/
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-04-07 07:19:40.261891 verify_access_autoconf-0.1.0/src/verify_access_autoconf/
--rw-rw-r--   0 lowkey    (1000) lowkey    (1000)      531 2023-04-07 07:10:07.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf/__init__.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)      114 2023-04-07 07:10:14.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf/__main__.py
--rw-rw-r--   0 lowkey    (1000) lowkey    (1000)   111896 2023-04-07 07:09:04.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf/access_control.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    16135 2023-04-07 07:09:15.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf/appliance.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    28634 2023-04-07 07:09:25.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf/configure.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3512 2023-04-07 07:09:41.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf/container.py
--rw-rw-r--   0 lowkey    (1000) lowkey    (1000)    78682 2023-04-07 07:09:53.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf/federation.py
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-04-07 07:19:40.263891 verify_access_autoconf-0.1.0/src/verify_access_autoconf/util/
--rw-rw-r--   0 lowkey    (1000) lowkey    (1000)       24 2023-04-07 07:11:09.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf/util/__init__.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)     9185 2023-04-07 07:10:41.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf/util/configure_util.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)      705 2023-04-07 07:10:51.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf/util/constants.py
--rw-rw-r--   0 lowkey    (1000) lowkey    (1000)     5662 2023-04-07 07:11:00.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf/util/data_util.py
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)    88463 2023-04-07 07:10:29.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf/webseal.py
-drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-04-07 07:19:40.262891 verify_access_autoconf-0.1.0/src/verify_access_autoconf.egg-info/
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)      338 2023-04-07 07:19:40.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf.egg-info/PKG-INFO
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)      833 2023-04-07 07:19:40.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf.egg-info/SOURCES.txt
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)        1 2023-04-07 07:19:40.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf.egg-info/dependency_links.txt
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)        1 2023-04-07 07:19:40.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf.egg-info/not-zip-safe
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)       82 2023-04-07 07:19:40.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf.egg-info/requires.txt
--rw-r--r--   0 lowkey    (1000) lowkey    (1000)       23 2023-04-07 07:19:40.000000 verify_access_autoconf-0.1.0/src/verify_access_autoconf.egg-info/top_level.txt
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 23:31:13.962801 verify_access_autoconf-0.3.0/
+-rwxr-xr-x   0 lowkey    (1000) lowkey    (1000)      592 2022-11-29 01:22:30.000000 verify_access_autoconf-0.3.0/.deploy.sh
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 23:31:13.949801 verify_access_autoconf-0.3.0/.github/
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 23:31:13.952801 verify_access_autoconf-0.3.0/.github/workflows/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      899 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/.github/workflows/main.yaml
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)       75 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/.gitignore
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 23:31:13.953801 verify_access_autoconf-0.3.0/.tests/
+-rw-rw-r--   0 lowkey    (1000) lowkey    (1000)        0 2020-05-23 07:54:08.000000 verify_access_autoconf-0.3.0/.tests/__init__.py
+-rw-rw-r--   0 lowkey    (1000) lowkey    (1000)      636 2022-08-03 00:48:04.000000 verify_access_autoconf-0.3.0/.tests/import_test.sh
+-rw-rw-r--   0 lowkey    (1000) lowkey    (1000)       23 2020-07-06 22:00:57.000000 verify_access_autoconf-0.3.0/.tests/unit_test.sh
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      654 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/.travis.yml
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 23:31:13.953801 verify_access_autoconf-0.3.0/.vscode/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)       52 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/.vscode/settings.json
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      188 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/Dockerfile
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      553 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/LICENCE.md
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5437 2023-05-04 23:31:13.961801 verify_access_autoconf-0.3.0/PKG-INFO
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5082 2023-05-04 23:28:27.000000 verify_access_autoconf-0.3.0/README.md
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)       88 2023-05-04 23:19:11.000000 verify_access_autoconf-0.3.0/dev-requirements.txt
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 23:31:13.956801 verify_access_autoconf-0.3.0/docs/
+-rw-rw-r--   0 lowkey    (1000) lowkey    (1000)      634 2022-07-19 04:23:54.000000 verify_access_autoconf-0.3.0/docs/Makefile
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     9936 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/docs/access-control.rst
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3098 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/docs/appliance.rst
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5116 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/docs/base.rst
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     2192 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/docs/conf.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4526 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/docs/container.rst
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1377 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/docs/examples.rst
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     8556 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/docs/federations.rst
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6117 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/docs/index.rst
+-rw-rw-r--   0 lowkey    (1000) lowkey    (1000)      795 2022-07-19 04:23:54.000000 verify_access_autoconf-0.3.0/docs/make.bat
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    12340 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/docs/webseal.rst
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 23:31:13.957801 verify_access_autoconf-0.3.0/examples/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1627 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/examples/first_steps.yaml
+-rw-rw-r--   0 lowkey    (1000) lowkey    (1000)     2984 2020-05-23 07:54:08.000000 verify_access_autoconf-0.3.0/examples/hello_world.yaml
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     4231 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/examples/webseal.yaml
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3473 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/examples/webseal_authsvc_login.yaml
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)       38 2023-05-04 23:31:13.962801 verify_access_autoconf-0.3.0/setup.cfg
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1890 2023-05-04 23:30:50.000000 verify_access_autoconf-0.3.0/setup.py
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 23:31:13.950801 verify_access_autoconf-0.3.0/src/
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 23:31:13.959801 verify_access_autoconf-0.3.0/src/verify_access_autoconf/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      531 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf/__init__.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      114 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf/__main__.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)   127520 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf/access_control.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    16126 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf/appliance.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    28606 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf/configure.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     3564 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf/container.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)   101630 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf/federation.py
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 23:31:13.961801 verify_access_autoconf-0.3.0/src/verify_access_autoconf/util/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)       24 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf/util/__init__.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     9201 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf/util/configure_util.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)      764 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf/util/constants.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     6439 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf/util/data_util.py
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    92878 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf/webseal.py
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 23:31:13.960801 verify_access_autoconf-0.3.0/src/verify_access_autoconf.egg-info/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     5437 2023-05-04 23:31:13.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf.egg-info/PKG-INFO
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)     1339 2023-05-04 23:31:13.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf.egg-info/SOURCES.txt
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)        1 2023-05-04 23:31:13.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf.egg-info/dependency_links.txt
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)        1 2023-05-04 23:31:13.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf.egg-info/not-zip-safe
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)       82 2023-05-04 23:31:13.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf.egg-info/requires.txt
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)       23 2023-05-04 23:31:13.000000 verify_access_autoconf-0.3.0/src/verify_access_autoconf.egg-info/top_level.txt
+drwxr-xr-x   0 lowkey    (1000) lowkey    (1000)        0 2023-05-04 23:31:13.961801 verify_access_autoconf-0.3.0/templates/
+-rw-r--r--   0 lowkey    (1000) lowkey    (1000)    12363 2023-05-04 23:16:18.000000 verify_access_autoconf-0.3.0/templates/config_template.yaml
```

### Comparing `verify_access_autoconf-0.1.0/LICENCE.md` & `verify_access_autoconf-0.3.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `verify_access_autoconf-0.1.0/README.md` & `verify_access_autoconf-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,87 @@
 # IBM Security Verify Access Configuration Automation
 This repository is used to configure IBM Security Verify Access (ISVA) using a yaml file of the required configuration. 
 
 This project aims to be idempotent, ie if the configuration is run multiple times on the same appliance it should not break and should pick up any configuration changes in the yaml configuration file.
 
 ## Example deployments
-To get started several example deployments are avaliable in the [Examples](examples/) directory. The example yaml files must be updated with deployment specific parameters, usually this is network addresses and ISVA activation codes.
+To get started several example deployments are available in the [Examples](examples/) directory. The example yaml files must be updated with deployment specific parameters, usually this is network addresses and ISVA activation codes.
 
 # Setup
 ## Environment
-- `ISVA_CONFIGURATION_BASE_DIR` = direcotry which contains the YAML configuration file as well as any http template pages, PKI, mapping rules, ect.
-- `ISVA_YAML_CONFIGURATION` = path to ISVA configuration yaml file. Path should be relative to `ISVA_CONFIGURATION_BASEDIR`
-- `ISVA_MGMT_BASE_URL` = address to access ISVA LMI, eg. https://\<isva appliance\>:\<isva port\>. This propert can also be specified in the configuration yaml file. If present, this proprty will take precedence.
-- `_ISVA_MGMT_PASSWORD` = administrator password for the `admin` account. This property can also be specified in the configuration yaml file. If present, this property will take precedence.
-- `ISVA_MGMT_OLD_PASSWORD` = if a password change for the administrator account (eg. from the dafualt) is required, the old password can be specified with this environment variable. If present the administrator's password will be chagned from `MGMT_OLD_PASSWORD` to `MGMT_PASSWORD`
+- `ISVA_CONFIG_BASE` = directory which contains the YAML configuration file as well as any http template pages, PKI, mapping rules, ect.
+- `ISVA_CONFIG_YAML` = path to ISVA configuration yaml file. Path should be relative to `ISVA_CONFIG_BASE`
+- `ISVA_MGMT_BASE_URL` = address to access ISVA LMI, eg. https://\<isva appliance\>:\<isva port\>. This property can also be specified in the configuration yaml file. If present, this property will take precedence.
+- `ISVA_MGMT_USER` = The user to perform configuration as. If not supplied the `admin` user is used.
+- `ISVA_MGMT_PWD` = administrator password for the administrator account performing configuration. This property can also be specified in the configuration yaml file. If present, this property will take precedence.
+- `ISVA_MGMT_OLD_PWD` = if a password change for the administrator account (eg. from the default) is required, the old password can be specified with this environment variable. If present the administrator's password will be changed from `MGMT_OLD_PASSWORD` to `MGMT_PASSWORD`
 - `ISVA_KUBERNETES_YAML_CONFIG` (optional) = path to Kubernetes configuration yaml for kubernetes deployments. 
-  - Note: If your kubernetes cluster requires mutual authentication (TLS) then a pem certificate file must also be avaliable to ISVA Configurator
+  - Note: If your kubernetes cluster requires mutual authentication (TLS) then a pem certificate file must also be available to ISVA Configurator
   - Note: When run from a Kubernetes cluster a Service Account can be used in place of a YAML configuration file
 
 ## Deployment
 ### Local environment
 IBM Security Verify Access Configuration Automation is simple to run locally. 
-1. First the required python packages are installed from [IBM Security Verify Access DevOps PyPi](https://na.artifactory.swg-devops.com/artifactory/sec-iam-isam-devops-team-pypi-local/). 
+1. First the required python packages are installed from [PyPi](https://pypi.org/project/verify-access-autoconf/). 
 2. Set the required environment variables
-3. a python interactive shell or python script can be used to configure applainces:
+3. a python interactive shell or python script can be used to configure appliances:
 ```python
->>> import isva_configurator
->>> isva_configurator.configurator.configure()
+>>> import verify_access_autoconf
+>>> verify_access_autoconf.configurator.configure()
 ```
 
 ### Docker
-IBM Security Verify Access Configuration Automation can also be run within a docker container. Use to [Dockerfile](Dockerfile) to build a local docer image or pull the latest image from [ISVA Devops Artifactory](https://na.artifactory.swg-devops.com/artifactory/sec-iam-isam-devops-team-docker-local/)\(IBM w3 login is required\). This uses a multi-stage build process to ensure that the username / access token used to fetch pacakges from artifactory does not show up in any metadata in the final container.
+IBM Security Verify Access Automated Configurator can also be run within a docker container. Use to [Dockerfile](Dockerfile) to build a local docker image.
+
+The docker container can be built and run with the following command executed from the top level directory of the configurator source code. When starting the container the required environment variables must be set and the docker container must be able to route to the ISVA appliances/containers which are to be configured.
 
-The docker container can be built with the following command executed from the top level directory of the configurator source code:
-```
-docker build --no-cache --force-rm --build-arg "ART_API_USER=user@name" --build-arg "ART_API_KEY=api_access_token" -t verify-access-configurator .
 ```
+docker build --no-cache --force-rm -t verify-access-configurator .
 
-When starting the container the required environment variables must be set and the docker container must be able to route to the ISVA appliances/containers which are to be configured.
+docker run --volume /path/to/config/yaml:/config --env "ISVA_CONFIGURATION_BASE_DIR=/config" --env ISVA_MGMT_BASE_URL="https://<mgmt address>:<mgmt port>" --env "ISVA_MGMT_PASSWORD=Passw0rd1!" verify-access-configurator
+```
 
-An example docker run command is:
-`docker run -it --rm --volume /path/to/kubernetes/config.yaml:/root/kube-config.yaml --volume /path/to/kubernetes/ssl.pem:/root/ssl.pem --env KUBECONFIG='/root/kube-config.yaml' --env MGMT_BASE_URL='https://<mgmt address>:<mgmt port>' --env MGMT_PASSWORD='admin' sec-iam-isam-devops-team-docker-local.artifactory.swg-devops.com/isva-configurator`
 
 ### Kubernetes
-ISVA Configurator can also be run from within a Kubernetes cluster. This is useful if there are routing issues between the deployment host and the kubernetes external addresses this option will allow for configuration using the kubernetes internal network.
+IBM Security Verify Access Automated Configurator can be run from within a Kubernetes cluster. This is useful if there are routing issues between the deployment host and the kubernetes external addresses this option will allow for configuration using the kubernetes internal network.
+
+Here is an example Kubernetes batch" object which deploys a container to apply a configuration to a cluster.
+> note This requires a user to create the `verify-config` ConfigMap object with the required configuration files plus any additional Secrets which are referenced.
+
+```
+apiVersion: batch/v1
+kind: Job
+metadata:
+  name: verify-access-configurator
+spec:
+  template:
+    spec:
+      containers:
+      - name: verify-access-configurator
+        image: python3:latest
+        command: ["python3", "-m", "verify_access_autoconf"]
+        volumeMounts:
+        - name: verify-access-config
+          mountPath: /verify_access_config
+        env:
+        - name: ISVA_CONFIG_BASE
+          value: "/verify_access_config"
+        - name: ISVA_MGMT_BASE_URL
+          value: "https://isamconfig:9443"
+        - name: ISVA_MGMT_PASSWORD
+          value: "Passw0rd1!"
+        - name: ISVA_CONFIGURATOR_LOG_LEVEL
+          value: "ALL"
+      restartPolicy: Never
+      volumes:
+      - name: verify-access-config
+        configMap:
+          name: verify-access-config
+      initContainers:
+        - name: install-verify-access-autoconf
+          image: python3:latest
+          command: ["bash", "-c", "pip3 install verify-access-autoconf"]
+  backoffLimit: 4
+```
 
+## Documentation
+Documentation for using this library can be found on [Verify Access Automated Configurator's GitHub pages](https://lachlan-ibm.github.io/verify_access_autoconf/index.html).
```

### Comparing `verify_access_autoconf-0.1.0/src/verify_access_autoconf/__init__.py` & `verify_access_autoconf-0.3.0/src/verify_access_autoconf/__init__.py`

 * *Files identical despite different names*

### Comparing `verify_access_autoconf-0.1.0/src/verify_access_autoconf/access_control.py` & `verify_access_autoconf-0.3.0/src/verify_access_autoconf/access_control.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 import json
 import os
 import typing
 import copy
 
 from .util.configure_util import config_base_dir, deploy_pending_changes
-from .util.data_util import Map, FILE_LOADER
+from .util.data_util import Map, FILE_LOADER, optional_list, filter_list
 
 _logger = logging.getLogger(__name__)
 
 class AAC_Configurator(object):
 
     config = Map()
     aac = None
@@ -70,30 +70,30 @@
         imc_refresh_token: typing.Optional[str]
         'The IBM Marketing Cloud issued Oauth refresh token.'
         imc_app_key: typing.Optional[str]
         'The app key issued by IBM Marketing Cloud for the associated application.'
 
     def push_notifications(self, config):
         if config.push_notification_providers:
-            existing = self.aac.push_notification.list_providers().json
+            existing_pnp = optional_list(self.aac.push_notification.list_providers().json)
             for provider in config.push_notification_providers:
-                rsp = None
-                verb = 'None'
-                old = list(filter(lambda x: (provider.app_id != None and x['app_id'] == provider.app_id), existing))
-                if old.length != 0:
-                    rsp = self.aac.push_notification.update(old[0]['pnr_id'], **provider)
+                rsp = None; verb = 'None'
+                old_pnp = optional_list(filter_list('app_id', provider.app_id, existing_pnp))[0]
+                if old_pnp:
+                    rsp = self.aac.push_notification.update_provider(old_pnp['pnr_id'], **provider)
                     verb = 'modified' if rsp.success == True else 'modify'
                 else:
-                    rsp = self.aac.push_notification.create(**provider)
+                    rsp = self.aac.push_notification.create_provider(**provider)
                     verb = 'created' if rsp.success == True else 'create'
                 if rsp.success == True:
+                    self.needsRestart = True
                     _logger.info("Successfully {} {} push notification provider".format(verb, provider.app_id))
                 else:
                     _logger.error("Failed to {} push notification provider:\n{}\n{}".format(verb, 
-                                                                json.dumps(provider, indent=4), rsp.content))
+                                                                json.dumps(provider, indent=4), rsp.data))
 
 
     class Risk_Profiles(typing.TypedDict):
         '''
         Example::
 
                 risk_profiles:
@@ -123,75 +123,73 @@
         'A unique name for the risk profile.'
         description: typing.Optional[str]
         'An optional brief description of the risk profile.'
         active: bool
         'True indicates this risk profile is the currently active risk profile. Only one profile can be active at a time.'
         attributes: typing.Optional[typing.List[Attribute]]
         'Array of attributes comprising this risk profile and the weight value of each attribute which is used in determining the risk score.'
-        predefined: bool
+        predefined: typing.Optional[bool]
         'False to indicate this risk profile is custom defined.'
 
     def _remap_attribute_name_to_id(self, all_attributes, risk_profile):
         for attribute in risk_profile['attributes']:
             for attribute_def in all_attributes:
                 if "name" in attribute and attribute['name'] == attribute_def['name']:
                     attribute.pop('name')
                     attribute["attributeID"] = attribute_def["id"]
                 elif "id" in attr:
                     attribute["attributeID"] = attribute.pop("id")
 
     def risk_profiles(self, config):
         if config.risk_profiles:
-            attributes = self.aac.attributes.list_attributes().json
-            old_profiles = self.aac.risk_profiles.list().json
-            if not attributes: attributes = []
-            if not old_profiles: old_profiles = []
+            attributes = optional_list(self.aac.attributes.list_attributes().json)
+            old_profiles = optional_list(self.aac.risk_profiles.list().json)
             for profile in config.risk_profiles:
                 methodArgs = copy.deepcopy(profile)
                 #Re-map attribute name and id keys to correct property
-                if "attributes" in methodArgs:
+                if "attributes" in methodArgs.keys():
                     self._remap_attribute_name_to_id(attributes, methodArgs)
-                
                 rsp = None
                 verb = None
-                old = list(filter(lambda x: 'name' in x and x['name'] == profile.name, old_profiles))
-                if old:
-                    rsp = self.aac.risk_profiles.update(old[0]['id'], **methodArgs)
+                old_profile = optional_list(filter_list('name', profile.name, old_profiles))[0]
+                if old_profile:
+                    rsp = self.aac.risk_profiles.update(old_profile['id'], **methodArgs)
                     verb = "updated" if rsp.success == True else "update"
                 else:
                     rsp = self.aac.risk_profiles.create(**methodArgs)
                     verb = "created" if rsp.success == True else "create"
                 if rsp.success == True:
+                    self.needsRestart = True
                     _logger.info("Successfully {} {} risk profile".format(verb, profile.name))
                 else:
-                    _logger.error("Failed to {} risk profile:\n{}\n{}".format(verb, 
-                                                            json.dumps(profile, indent=4), rsp.data))
+                    _logger.error("Failed to {} risk profile:\n{}\n{}".format(
+                                            verb, json.dumps(profile, indent=4), rsp.data))
 
 
     class Policy_Information_Points(typing.TypedDict):
         '''
         Example::
 
                 pips:
                 - name: "myJSpip"
                   description: "Custom JavaScript PIP."
                   type: "JavaScript"                  
                   properties:
-                  - readOnly: false
+                  - read_only: false
                     value: |
                         /** Import packages necessary for the script to execute. */
                         importPackage(com.ibm. . .);
                         /** Your code here */
                         ....
                         var name = getName();
                         return
                     datatype: "JavaScript"
                     key: "javascript.code"
                     sensitive: false
-                  - readOnly: false
+                  - read_only: false
                     value: "89"
                     datatype: "Integer"
                     key: "limit"
                     sensitive: false
 
         '''
         class Policy_Information_Point(typing.TypedDict):
@@ -229,97 +227,120 @@
         'List of policy information points to configure.'
 
     def pip_configuration(self, config):
         if config.pips:
             existing = self.aac.pip.list_pips().json
             if not existing: existing = []
             for pip in config.pips:
-                old = list(filter(lambda x: x['name'] == pip.name, existing))
+                methodArgs = copy.deepcopy(pip)
+                if "properties" in methodArgs.keys():
+                    for k, v in methodArgs["properties"].items():
+                        if k == "read_only":
+                            methodArgs["properties"]["readOnly"] = methodArgs["properties"].pop("read_only")
+                old = filter_list('name', pip.name, existing)
                 rsp = None
                 verb = None
                 if old:
                     old = old[0]
                     rsp = self.aac.pip.update_pip(old['id'], **pip)
                     verb = "updated" if rsp.success == True else "update"
                 else:
                     rsp = self.aac.pip.create_pip(**pip)
                     verb = "created" if rsp.success == True else "create"
                 if rsp.success == True:
+                    self.needsRestart = True
                     _logger.info("Successfully {} {} PIP".format(verb, pip.name))
                 else:
                     _logger.error("Failed to {} PIP:\n{}\n{}".format(verb, json.dumps(pip, indent=4), rsp.data))
                     
 
-    def _cba_resource(self, resource):
+    def _cba_resource(self, resource, policies, policy_sets, definitions):
         methodArgs = {
             "server": resource.server,
-            "resourceUri": resource.uri,
-            "policies": resource.policies,
+            "resource_uri": resource.uri,
+            "policies": [],
             "policy_combining_algorithm": resource.policy_combining_algorithm,
             "cache": resource.cache
         }
+        if resource.policies: #remap policy names to Verify Access uuids
+            policyArg = []
+            for policy in resource.policy:
+                policy_id = "-1"
+                if policy.type == "policy":
+                    policy_id = optional_list(filter_list("name", policy.name, policies)).get('id', "-1")
+                elif policy.type == "policyset":
+                    policy_id = optional_list(filter_list('name', policy.name, policy_sets))[0].get('id', "-1")
+                elif policy.type == "definition":
+                    policy_id = optional_list(filter_list('name', policy.name, definitions))[0].get('id', '-1')
+                policyArg += [{"id": policy_id, "type": policy.type}]
+            methodArgs['policies'] = policyArg
         rsp = self.aac.access_control.configure_resource(**methodArgs)
         if rsp.success == True:
+            self.needsRestart = True
             _logger.info("Successfully configured {} resource for {}".format(resource.uri, resource.server))
         else:
             _logger.error("Failed to create resource with configuration:\n{}\n{}".format(
                 json.dumps(resource, indent=4), rsp.data))
 
     def _cba_policy(self, old_policies, policy):
-        plc_id = None
+        policy_id = None
         for p in old_policies:
             if p['name'] == policy.name:
-                plc_id = p['id']
+                policy_id = p['id']
                 break
         methodArgs = {
                 "name": policy.name,
                 "description": policy.description,
                 "dialect": policy.dialect if policy.dialect else "urn:oasis:names:tc:xacml:2.0:policy:schema:os",
                 "policy": policy.policy,
                 "attributes_required": policy.attributes_required
             }
         rsp = None
         verb = None
-        if plc_id:
-            rsp = self.aac.access_control.update_policy(plc_id, **methodArgs)
+        if policy_id:
+            rsp = self.aac.access_control.update_policy(policy_id, **methodArgs)
             verb = "updated" if rsp.success == True else "update"
         else:
             rsp = self.aac.access_control.create_policy(**methodArgs)
             verb = "created" if rsp.success == True else "create"
         if rsp.success == True:
+            self.needsRestart = True
             _logger.info("Successfully {} {} Access Control Policy".format(verb, policy.name))
         else:
             _logger.error("Failed to {} Access Control Policy with config:\n{}\n{}".format(verb,
                                                                     json.dumps(policy, indent=4), rsp.data))
 
 
     class Access_Control(typing.TypedDict):
         '''
         Example::
 
                 access_control:
                   policies:
-                      - name: "Verify Demo - MFA Login Policy"
-                      policy: "<?xml version=\"1.0\" encoding=\"UTF-8\"?><!-- PolicyTag=urn:ibm:security:isam:8.0:xacml:2.0:config-policy --><!-- PolicyName='Verify Demo - MFA Login Policy' --><PolicySet xmlns=\"urn:oasis:names:tc:xacml:2.0:policy:schema:os\" xmlns:xacml-context=\"urn:oasis:names:tc:xacml:2.0:context:schema:os\" xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\" xsi:schemaLocation=\"urn:oasis:names:tc:xacml:2.0:policy:schema:os http://docs.oasis-open.org/xacml/access_control-xacml-2.0-policy-schema-os.xsd\" PolicySetId=\"urn:ibm:security:config-policy\" PolicyCombiningAlgId=\"urn:oasis:names:tc:xacml:1.0:policy-combining-algorithm:deny-overrides\"><Description>Example CBA Policy for the MFA Banking Demo password-less login</Description><Target/><Policy PolicyId=\"urn:ibm:security:rule-container:0\" RuleCombiningAlgId=\"urn:oasis:names:tc:xacml:1.0:rule-combining-algorithm:first-applicable\"><Target/><Rule RuleId=\"urn:ibm:security:rule:0\" Effect=\"Permit\"></Rule><Obligations><Obligation ObligationId=\"urn:ibm:security:authentication:asf:verify_mmfa_request_fingerprint\" FulfillOn=\"Permit\"/></Obligations></Policy></PolicySet>"
-                      - name: "Verify Demo - EULA"
-                      policy: "<?xml version=\"1.0\" encoding=\"UTF-8\"?><!-- PolicyTag=urn:ibm:security:isam:8.0:xacml:2.0:config-policy --><!-- PolicyName='Verify Demo - EULA' --><PolicySet xmlns=\"urn:oasis:names:tc:xacml:2.0:policy:schema:os\" xmlns:xacml-context=\"urn:oasis:names:tc:xacml:2.0:context:schema:os\" xmlns:xsi=\"http:\/\/www.w3.org\/2001\/XMLSchema-instance\" xsi:schemaLocation=\"urn:oasis:names:tc:xacml:2.0:policy:schema:os http:\/\/docs.oasis-open.org\/xacml\/access_control-xacml-2.0-policy-schema-os.xsd\" PolicySetId=\"urn:ibm:security:config-policy\" PolicyCombiningAlgId=\"urn:oasis:names:tc:xacml:1.0:policy-combining-algorithm:first-applicable\"><Description>GDPR Compliance (Acceptance of ToS)<\/Description><Target\/><Policy PolicyId=\"urn:ibm:security:rule-container:0\" RuleCombiningAlgId=\"urn:oasis:names:tc:xacml:1.0:rule-combining-algorithm:first-applicable\"><Target\/><Rule RuleId=\"urn:ibm:security:rule:0\" Effect=\"Permit\"><Condition><Apply FunctionId=\"urn:oasis:names:tc:xacml:1.0:function:and\"><Apply FunctionId=\"urn:oasis:names:tc:xacml:1.0:function:string-at-least-one-member-of\"><Apply FunctionId=\"urn:oasis:names:tc:xacml:1.0:function:string-bag\"><AttributeValue DataType=\"http:\/\/www.w3.org\/2001\/XMLSchema#string\">urn:ibm:security:authentication:asf:mechanism:eula<\/AttributeValue><\/Apply><SubjectAttributeDesignator AttributeId=\"urn:ibm:security:subject:authenticationMechanismTypes\" DataType=\"http:\/\/www.w3.org\/2001\/XMLSchema#string\" MustBePresent=\"false\"\/><\/Apply><\/Apply><\/Condition><\/Rule><\/Policy><Policy PolicyId=\"urn:ibm:security:rule-container:1\" RuleCombiningAlgId=\"urn:oasis:names:tc:xacml:1.0:rule-combining-algorithm:first-applicable\"><Target\/><Rule RuleId=\"urn:ibm:security:rule:1\" Effect=\"Permit\"><\/Rule><Obligations><Obligation ObligationId=\"urn:ibm:security:authentication:asf:eula\" FulfillOn=\"Permit\"\/><\/Obligations><\/Policy><\/PolicySet>"
-                      description: "GDPR Compliance (Acceptance of ToS)"
+                  - name: "Verify Demo - MFA Login Policy"
+                  policy: "<?xml version=\"1.0\" encoding=\"UTF-8\"?><!-- PolicyTag=urn:ibm:security:isam:8.0:xacml:2.0:config-policy --><!-- PolicyName='Verify Demo - MFA Login Policy' --><PolicySet xmlns=\"urn:oasis:names:tc:xacml:2.0:policy:schema:os\" xmlns:xacml-context=\"urn:oasis:names:tc:xacml:2.0:context:schema:os\" xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\" xsi:schemaLocation=\"urn:oasis:names:tc:xacml:2.0:policy:schema:os http://docs.oasis-open.org/xacml/access_control-xacml-2.0-policy-schema-os.xsd\" PolicySetId=\"urn:ibm:security:config-policy\" PolicyCombiningAlgId=\"urn:oasis:names:tc:xacml:1.0:policy-combining-algorithm:deny-overrides\"><Description>Example CBA Policy for the MFA Banking Demo password-less login</Description><Target/><Policy PolicyId=\"urn:ibm:security:rule-container:0\" RuleCombiningAlgId=\"urn:oasis:names:tc:xacml:1.0:rule-combining-algorithm:first-applicable\"><Target/><Rule RuleId=\"urn:ibm:security:rule:0\" Effect=\"Permit\"></Rule><Obligations><Obligation ObligationId=\"urn:ibm:security:authentication:asf:verify_mmfa_request_fingerprint\" FulfillOn=\"Permit\"/></Obligations></Policy></PolicySet>"
+                  - name: "Verify Demo - EULA"
+                  policy: "<?xml version=\"1.0\" encoding=\"UTF-8\"?><!-- PolicyTag=urn:ibm:security:isam:8.0:xacml:2.0:config-policy --><!-- PolicyName='Verify Demo - EULA' --><PolicySet xmlns=\"urn:oasis:names:tc:xacml:2.0:policy:schema:os\" xmlns:xacml-context=\"urn:oasis:names:tc:xacml:2.0:context:schema:os\" xmlns:xsi=\"http:\/\/www.w3.org\/2001\/XMLSchema-instance\" xsi:schemaLocation=\"urn:oasis:names:tc:xacml:2.0:policy:schema:os http:\/\/docs.oasis-open.org\/xacml\/access_control-xacml-2.0-policy-schema-os.xsd\" PolicySetId=\"urn:ibm:security:config-policy\" PolicyCombiningAlgId=\"urn:oasis:names:tc:xacml:1.0:policy-combining-algorithm:first-applicable\"><Description>GDPR Compliance (Acceptance of ToS)<\/Description><Target\/><Policy PolicyId=\"urn:ibm:security:rule-container:0\" RuleCombiningAlgId=\"urn:oasis:names:tc:xacml:1.0:rule-combining-algorithm:first-applicable\"><Target\/><Rule RuleId=\"urn:ibm:security:rule:0\" Effect=\"Permit\"><Condition><Apply FunctionId=\"urn:oasis:names:tc:xacml:1.0:function:and\"><Apply FunctionId=\"urn:oasis:names:tc:xacml:1.0:function:string-at-least-one-member-of\"><Apply FunctionId=\"urn:oasis:names:tc:xacml:1.0:function:string-bag\"><AttributeValue DataType=\"http:\/\/www.w3.org\/2001\/XMLSchema#string\">urn:ibm:security:authentication:asf:mechanism:eula<\/AttributeValue><\/Apply><SubjectAttributeDesignator AttributeId=\"urn:ibm:security:subject:authenticationMechanismTypes\" DataType=\"http:\/\/www.w3.org\/2001\/XMLSchema#string\" MustBePresent=\"false\"\/><\/Apply><\/Apply><\/Condition><\/Rule><\/Policy><Policy PolicyId=\"urn:ibm:security:rule-container:1\" RuleCombiningAlgId=\"urn:oasis:names:tc:xacml:1.0:rule-combining-algorithm:first-applicable\"><Target\/><Rule RuleId=\"urn:ibm:security:rule:1\" Effect=\"Permit\"><\/Rule><Obligations><Obligation ObligationId=\"urn:ibm:security:authentication:asf:eula\" FulfillOn=\"Permit\"\/><\/Obligations><\/Policy><\/PolicySet>"
+                  description: "GDPR Compliance (Acceptance of ToS)"
                   resources:
-                      - server: "my.ibmsec.idp"
-                      resource_uri: "/login"
-                      policies:
-                          - "Verify Demo - MFA Login Policy"
-                      - server: "my.ibmsec.idp"
-                      resource_uri: "/protected/transfer"
-                      policies:
-                          - "Verify Demo - MFA Transaction Policy"
-                      - server: "my.ibmsec.idp"
-                      resource_uri: "/isam/sps/SP-SAML-QC/saml20/login"
-                      policies:
-                          - "Verify Demo - MFA Office 365 Login"
+                  - server: "my.ibmsec.idp"
+                    resource_uri: "/login"
+                    policies:
+                    - name: "Verify Demo - MFA Login Policy"
+                      type: "policy"
+                  - server: "my.ibmsec.idp"
+                    resource_uri: "/protected/transfer"
+                    policies:
+                    - name: "Verify Demo - MFA Transaction Policy"
+                      type: "policy"
+                  - server: "my.ibmsec.idp"
+                    resource_uri: "/isam/sps/SP-SAML-QC/saml20/login"
+                    policies:
+                    - name: "Verify Demo - MFA Office 365 Login"
+                      type: "policy"
 
         '''
         class Policy(typing.TypedDict):
             name: str
             'The name of the policy.'
             description: typing.Optional[str]
             'An optional description of the policy.'
@@ -327,19 +348,25 @@
             'The XACML specification used within the policy. Only valid value is XACML Version 2, "urn:oasis:names:tc:xacml:2.0:policy:schema:os".'
             policy: str
             'The configured policy in XACML 2.0.'
             attributes_required: typing.Optional[typing.List[str]]
             'True if the values for any attributes specified in the policy must be present in the incoming request. False if the attribute values may optionally be present.'
 
         class Resource(typing.TypedDict):
+            class Policy_Attachment(typing.TypedDict):
+                name: str
+                'Name of the policy, policy set, or API protection definition.'
+                type: str
+                'The type of attachment. Values include "policy", "policyset", or "definition".'
+
             server: str
             'The web container that contains the protected object space for a server instance.'
             resource_uri: str
             'The resource URI of the resource in the protected object space.'
-            policies: str
+            policies: typing.List[Policy_Attachment]
             'Array of attachments (policy, policy sets, and API protection definitions) that define the access protection for this resource.'
             policy_combining_algorithm: typing.Optional[str]
             '"permitOverrides" to allow access to the resource if any of the attachments return permit; "denyOverrides" to deny access to the resource if any of the attachments return deny. Default is "denyOverrides".'
             cache: int
             '0 to disable the cache for this resource, -1 to cache the decision for the lifetime of the session or any number greater than 1 to set a specific timeout (in seconds) for the cached decision. If not specified a default of 0 will be used.'
 
         policies: typing.Optional[typing.List[Policy]]
@@ -376,30 +403,27 @@
         name: typing.Optional[str]
         'The name of the advanced configuration property. Either the property ID or name must be defined.'
         value: str
         'The updated value of the advanced configuration property.'
 
     def advanced_config(self, aac_config):
         if aac_config.advanced_configuration != None:
-            old_config = self.aac.advanced_configuration.list().json
+            old_config = optional_list(self.aac.advanced_config.list_properties().json)
             for advConf in aac_config.advanced_configuration:
-                old = None; id=None; sensitive=None
-                if advConfig.name:
-                    old = list(filter(lambda x: x['key'] == advConf.name, old_config))
+                old = None
+                if advConf.name:
+                    old = optional_list(filter_list('key', advConf.name, old_config))[0]
                 else:
-                    old = list(filter(lambda x: x['id'] == advConf.id, old_config))
-                if old.length != 1:
+                    old = optional_list(filter_list('id', advConf.id, old_config))[0]
+                if not old:
                     _logger.error("Could not find {} in list of advanced configuration parameters".format(advConf.name))
                     continue
-                else:
-                    old = old[0]
-                    id = old['id']
-                    sensitive = old['sensitive']
-                rsp = self.aac.advanced_config.update(id, value=advConf.value, sensitive=sensitive)
+                rsp = self.aac.advanced_config.update_property(old['id'], value=advConf.value, sensitive=old.get('sensitive', None))
                 if rsp.success == True:
+                    self.needsRestart = True
                     _logger.info("Successfully updated advanced configuration {}".format(old['key']))
                 else:
                     _logger.error("Failed to update advanced configuration with:\n{}\n{}".format(
                         json.dumps(advConf, indent=4), rsp.data))
 
 
 
@@ -551,22 +575,42 @@
         attribute_modes: typing.Optional[typing.List[AttributeMode]]
         'The customized attribute modes.'
         max_user_response: typing.Optional[int]
         'The maximum number of entries that can be returned from a single call to the /User endpoint.'
 
     def scim_configuration(self, aac_config):
         if aac_config.scim != None:
+            generalConfig = self.aac.scim_config.get_general_config().json
+            needToUpdate = False
+            for prop in ["admin_group", "enable_header_authentication", "enable_authz_filter", "max_user_response"]:
+                if prop in aac_config.scim:
+                    generalConfig[prop] = aac_config.scim.get(prop)
+                    needToUpdate = True
+            if aac_config.scim.attribute_modes:
+                attrModes = generalConfig.pop("attribute_modes", {})
+                attrModes.update(aac_config.scim.attribute_modes)
+                generalConfig["attribute_modes"] = attrModes
+                needToUpdate = True
+            if needToUpdate == True:
+                rsp = self.aac.scim_config.update_config(**generalConfig)
+                if rsp.success == True:
+                    self.needsRestart = True
+                    _logger.info("Successfully updated the SCIM general configuration")
+                else:
+                    _logger.error("Failed to update SCIM general configuration:\n{}\n{}".format(
+                                                        json.dumps(generalConfig, indent=4), rsp.data))
             for schema in aac_config.scim:
                 rsp = self.aac.scim_config.get_schema(schema.uri)
                 if rsp.success == False:
                     _logger.error("Failed to get config for schema [{}]".format(schema.uri))
                     return
-                config = {**rsp.json, **schema.properties}
+                config = {**rsp.json, **schema.properties} # I wonder how this resolves conflicts
                 rsp = self.aac.scim_config.update_schema(schema.uri, config)
                 if rsp.success == True:
+                    self.needsRestart = True
                     _logger.info("Successfully updated schema [{}]".format(schema.uri))
                 else:
                     _logger.error("Failed to update schema [{}] with configuration:\n{}".format(
                         schema.uri, config))
 
 
     def _ci_server_connection(self, connection):
@@ -619,25 +663,27 @@
             print(connectionType)
             for c in configured_connections[connectionType]:
                 print(c)
                 if c.get('name') == connection.name and c.get('locked') == True:
                     _logger.error("Connection {} exists and is locked, skipping".format(connection.name))
                     return False
                 elif c.get('name') == connection.name:
+                    default_fcn = lambda x: _logger.error("Server connection id [{}] not found".format(x))
                     logger.info("connection {} exists, deleting before recreating".format(connection.name))
                     rsp = {"ci": self.aac.server_connections.delete_ci,
                           "ldap": self.aac.server_connections.delete_ldap,
                           "isamruntime": self.aac.server_connections.delete_runtime,
                           "oracle": self.aac.server_connections.delete_jdbc,
                           "db2": self.aac.server_connections.delete_jdbc,
                           "soliddb": self.aac.server_connections.delete_jdbc,
                           "postgresql": self.aac.server_connections.delete_jdbc,
                           "smtp": self.aac.server_connections.delete_smtp,
-                          "ws": self.aac.server_connections.delete_web_service}.get(connection.type, None)(c['uuid'])
-                    return rsp.success
+                          "ws": self.aac.server_connections.delete_web_service}.get(
+                                                                    connection.type, default_fcn)(c['uuid'])
+                    return False if rsp == None else rsp.success
         return True
 
 
 
     class Server_Connections(typing.TypedDict):
         '''
         Example::
@@ -651,15 +697,15 @@
                       user: ""
                       password: ""
                       ssl: false
                   - name: "Cloud Identity tenant connection"
                     type: "ci"
                     description: "A connection to the companion CI Tenant."
                     properties:
-                      ci_tenant: !secret default/isva-secrets:ci_tenatn
+                      ci_tenant: !secret default/isva-secrets:ci_tenant
                       ci_client_id: !secret default/isva-secrets:ci_client_id
                       ci_client_secret: !secret default/isva-secrets:ci_client_secret
                       ssl_truststore: "rt_profile_keys.kdb"
                   - name: "Local LDAP connection"
                     type: "ldap"
                     description: "A connection to this ISAMs LDAP."
                     locked: false
@@ -924,23 +970,29 @@
                  - login.html
                  - 2fa.html
 
         '''
         template_files: typing.List[str]
         'List of files or zip-files to upload as HTML template pages. Path to files can be relative to the ``ISVA_CONFIG_BASE`` property or fully-qualified file paths.'
 
+    def _strip_base_dir(self, path):
+        return path.lstrip(config_base_dir())
+
     def upload_template_files(self, template_files):
         for file_pointer in template_files:
             rsp = None
-            if file_pointer.get("type") == "file":
+            if file_pointer['name'].endswith(".zip"):
+                rsp = self.aac.template_files.import_files(file_pointer['path'])
+            elif file_pointer.get("type") == "file":
                 rsp = self.aac.template_files.create_file(file_pointer['directory'], file_name=file_pointer['name'],
                         contents=file_pointer['contents'])
             else:
                 rsp = self.aac.template_files.create_directory(file_pointer['directory'], dir_name=file_pointer['name'])
             if rsp.success == True:
+                self.needsRestart = True
                 _logger.info("Successfully created template file {}".format(file_pointer['path']))
             else:
                 _logger.error("Failed to create template file {}".format(file_pointer['path']))
 
 
     class Mapping_Rules(typing.TypedDict):
         '''
@@ -971,23 +1023,28 @@
         mapping_rules: typing.List[Mapping_Rule]
         'List of mapping rule types/files to upload.'
 
     def upload_mapping_rules(self, _type, mapping_rules):
         for mapping_rule in mapping_rules:
             rsp = self.aac.mapping_rule.create_rule(rule_name=mapping_rule['name'], category=_type, content=mapping_rule['contents'])
             if rsp.success == True:
+                self.needsRestart = True
                 _logger.info("Successfully uploaded {} mapping rule".format(mapping_rule['name']))
             else:
                 _logger.error("Failed to upload {} mapping rule from [{}]".format(mapping_rule['name'], mapping_rule['path']))
 
 
     def upload_files(self, config):
         if config.template_files != None:
             for entry in config.template_files:
-                parsed_files = FILE_LOADER.read_files(entry, include_directories=True)
+                #Convert list of files/directories to flattened list of files
+                #include directories if we are a directory
+                incDirs = os.path.isdir(os.path.join(config_base_dir(), entry))
+                parsed_files = FILE_LOADER.read_files(entry, include_directories=incDirs)
+                self._remove_prefix_from_paths(parsed_files, entry)
                 self.upload_template_files(parsed_files)
         if config.mapping_rules != None:
             for entry in config.mapping_rules:
                 for file_pointer in entry.files:
                     parsed_files = FILE_LOADER.read_files(file_pointer)
                 self.upload_mapping_rules(entry.type, parsed_files)
 
@@ -1027,49 +1084,50 @@
             'A unique name for the obligation.'
             description: typing.Optional[str]
             'An optional description of the obligation.'
             uri: str
             'The identifier of the obligation that is used in generated XACML.'
             type: typing.Optional[str]
             'Should be set to "Obligation".'
+            type_id: typing.Optional[str]
+            'The obligation type id. If not provided, the value will be set to "1", which is the "Enforcement Point" type.'
             parameters: typing.List[Parameter]
             'Array of parameters associated with the obligation.'
             properties: typing.Optional[typing.List[Property]]
             'Array of properties associated with the obligations.'
         
         obligations: typing.List[Obligation]
         'List of access control obligations to create.'
 
     def obligation_configuration(self, aac_config):
+        if aac_config.obligations != None:
             existing = self.aac.access_control.list_obligations().json
             if existing == None: existing = []
             for obligation in aac_config.obligations:
-                obg_id = None
-                for obl in existing:
-                    if obl["obligationURI"] == obligation.uri:
-                        obg_id = obl['id']
-                        break
+                obg_id = optional_list(filter_list(
+                    "obligationURI", obligation.uri, existing))[0].get('id', None)
                 rsp = None
                 if obg_id:
                     rsp = self.aac.access_control.update_obligation(obg_id, name=obligation.name, 
-                            description=obligation.description, obligationURI=obligation.uri, 
-                            type=obligation.type, parameters=obligation.parameters, 
-                            properties=obligation.properties)
+                            description=obligation.description, obligation_uri=obligation.uri, 
+                            type=obligation.type, type_id=obligation.get("type_id", "1"), 
+                            parameters=obligation.parameters, properties=obligation.properties)
                     verb = "created" if rsp.success == True else "create"
                 else:
                     rsp = self.aac.access_control.create_obligation(name=obligation.name, 
-                            description=obligation.description, obligationURI=obligation.uri, 
-                            type=obligation.type, parameters=obligation.parameters, 
-                            properties=obligation.properties)
+                            description=obligation.description, obligation_uri=obligation.uri, 
+                            type=obligation.type, type_id=obligation.get("type_id", "1"), 
+                            parameters=obligation.parameters, properties=obligation.properties)
                     verb = "updated" if rsp.success == True else "update"
                 if rsp.success == True:
+                    self.needsRestart = True
                     _logger.info("Successfully {} {} obligation.".format(verb, obligation.name))
                 else:
                     _logger.error("Failed to {} obligation:\n{}\n{}".format(verb, 
-                                                                json.dumps(obligation, indent=4), rsp.content))
+                                                                json.dumps(obligation, indent=4), rsp.data))
                 return
 
 
     class Attributes(typing.TypedDict):
         '''
         Example::
 
@@ -1125,30 +1183,35 @@
         'Define where the attribute is stored.'
 
     def attributes_configuration(self, aac_config):
         if aac_config.attributes != None:
             existing = self.aac.attribute.list_attributes().json
             if existing == None: existing = []
             for attribute in aac_config.attributes:
-                attr_id = None
-                for attr in existing:
-                    if attr['name'] == attribute.name and attr['uri'] == attribute.uri:
-                        attr_id = attr['id']
-                        break
+                methodArgs = copy.deepcopy(attribute)
+                attr_id = optional_list(filter_list("uri", attribute.uri, existing))[0].get("id", None)
+                for k in ["storage", "type"]: #remap keys "key": {"di": "ct"} -> "key_di": "ct"
+                    if k in methodArgs.keys():
+                        old = methodArgs.pop(k)
+                        for oldKey, value in old.items():
+                            methodArgs[k + "_" + old_key] = value
+
                 rsp = None
                 if attr_id:
-                    rsp = self.aac.attribute.update_attribute(attr_id, **attribute)
+                    rsp = self.aac.attribute.update_attribute(attr_id, **methodArgs)
                     verb = "updated" if rsp.success else "update"
                 else:
-                    rsp = self.aac.attrbute.create_attribute(**attribute)
+                    rsp = self.aac.attribute.create_attribute(**methodArgs)
                     verb = "created" if rsp.success == True else "create"
                 if rsp.success == True:
+                    self.needsRestart = True
                     _logger.info("Successfully {} {} attribute.".format(verb, attribute.name))
                 else:
-                    _logger.error("Failed to {} attribute:\n{}\n{}".format(verb, json.dumps(attribute, indent=4), rsp.content))
+                    _logger.error("Failed to {} attribute:\n{}\n{}".format(verb, json.dumps(
+                                                                                    attribute, indent=4), rsp.data))
 
 
     def _configure_api_protection_definition(self, definition):
         methodArgs = {"name": definition.name, "description": definition.description, "token_char_set": definition.access_token_char_set,
                 "access_token_lifetime": definition.access_token_lifetime, "access_token_length": definition.access_token_length, 
                 "authorization_code_lifetime": definition.authorization_code_lifetime, "authorization_code_length": definition.authorization_code_length,
                 "refresher_token_length": definition.refresh_token_length, "max_authorization_grant_lifetime": definition.max_authorization_grant_lifetime,
@@ -1164,37 +1227,38 @@
             })
             if definition.oidc.enc:
                 methodArgs.update({
                     "enc_enabled": True, "enc_alg": definition.oidc.enc.alg, "enc_enc": definition.oidc.enc.enc
                 })
         rsp = self.aac.api_protection.create_definition(**methodArgs)
         if rsp.success == True:
+            self.needsRestart = True
             _logger.info("Successfully created {} API Protection definition".format(definition.name))
         else:
             _logger.error("Failed to create {} API Protection definition with config:\n{}\n{}".format(
                 definition.name, json.dumps(definition, indent=4), rsp.data))
         if definition.pre_token_mapping_rule:
             mapping_rule = FILE_LOADER.read_file(definition.pre_token_mapping_rule)
             if len(mapping_rule) != 1:
                 _logger.error("Can only specify one Pre-Token Mapping Rule")
             else:
                 mapping_rule = mapping_rule[0]
-                rsp = self.aac.api_protection.create_mapping_rule(name=definition.name + "PreTokenGeneration",
+                rsp = self.aac.api_protection.create_rule(name=definition.name + "PreTokenGeneration",
                         category="OAUTH", file_name=mapping_rule["name"], content=mapping_rule['contents'])
                 if rsp.success == True:
                     _logger.info("Successfully uploaded {} Pre-Token Mapping Rule".format(definition.name))
                 else:
                     _logger.error("Failed to upload {} Pre-Token Mapping Rule".format(definition.name))
         if definition.post_token_mapping_rule:
             mapping_rule = FILE_LOADER.read_file(definition.post_token_mapping_rule)
             if len(mapping_rule) != 1:
                 _logger.error("Can only specify one Post-Token Mapping Rule")
             else:
                 mapping_rule = mapping_rule[0]
-                rsp = self.aac.api_protection.import_mapping_rule(name=definition.name + "PostTokenGeneration",
+                rsp = self.aac.api_protection.create_rule(name=definition.name + "PostTokenGeneration",
                         category="OAUTH", file_name=mapping_rule['name'], content=mapping_rule['contents'])
                 if rsp.success == True:
                     _logger.info("Successfully created {} Post-Token Mapping Rule".format(definition.name))
                 else:
                     _logger.error("Failed to create {} Post-Token Mapping Rule".format(definition.name))
 
     def _configure_api_protection_client(self, definitions, client):
@@ -1203,14 +1267,15 @@
                 client.api_definition = definition['id']
                 break
         rsp = self.aac.api_protection.create_client(name=client.name, redirect_uri=client.redirect_uri,
                 company_name=client.company_name, company_url=client.company_url, contact_person=client.contact_person,
                 contact_type=client.contact_type, email=client.email, phone=client.phone, other_info=client.other_info,
                 definition=client.api_definition, client_id=client.client_id, client_secret=client.client_secret)
         if rsp.success == True:
+            self.needsRestart = True
             _logger.info("Successfully created {} API Protection client.".format(client.name))
         else:
             _logger.error("Failed to create {} API Protection client with config:\n{}\n{}".format(
                 client.name, json.dumps(client, indent=4), rsp.data))
 
     class API_Protection(typing.TypedDict):
         '''
@@ -1332,14 +1397,19 @@
             pin_length: typing.Optional[int]
             'The length of a PIN. Applicable when pinPolicyEnabled is true. Maximum value is 12 characters. Minimum value is 3 characters. If not provided, the PIN length is set to 4 characters.'
             token_char_set: typing.Optional[str]
             'String of characters that can be used to generate tokens. If not provided, the value will be set to alphanumeric character set, "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz". The maximum number of token characters that can be specified is 200.'
             oidc: typing.Optional[OIDC]
             'The OIDC configuration for this API protection definition.'
             attribute_sources: typing.Optional[typing.List[Attribute_Source]]
+            'Array of configured attribute sources to use in id_token generation and userinfo requests.'
+            pre_token_mapping_rule: typing.Optional[str]
+            'Path to file to upload as JavaScript pre-token rule.'
+            post_token_mapping_rule: typing.Optional[str]
+            'Path to file to upload as JavaScript post-token rule.'
 
         class Client(typing.TypedDict):
             name: str
             'A meaningful name to identify this API protection client.'
             defintition: str
             'The name of the related API protection definition which owns and defines this client. A client registration can only belong to one definition, but a definition can own many client registrations. The definition cannot be modified.'
             redirect_uri: typing.Optional[str]
@@ -1389,60 +1459,55 @@
             if aac_config.api_protection.clients != None:
                 definitions = self.aac.api_protection.list_definitions()
                 for client in aac_config.api_protection.clients:
                     self._configure_api_protection_client(definitions, client)
 
 
     def _configure_mechanism(self, mechTypes, existing_mechanisms, mechanism):
-        try:
-            typeId = list(filter(lambda _type: _type['type'] == mechanism.type, mechTypes))[0]['id']
-        except (IndexError, KeyError):
-            _logger.error("Mechanism [{}] specified an invalid type, skipping".format(mechanism))
+        typeId = optional_list(filter_list('type', mechanism.type, mechTypes))[0].get('id', None)
+        if not typeId:
+            _logger.error("Mechanism [{}] specified an invalid type, skipping.".format(mechanism))
             return
         props = None
         if mechanism.properties != None and isinstance(mechanism.properties, list):
             props = []
             for e in mechanism.properties: 
                 props += [{"key": k, "value": v} for k, v in e.items()]
-        old_mech = list(filter( lambda m: m['uri'] == mechanism.uri, existing_mechanisms))
+        old_mech = optional_list(filter_list('uri', mechanism.uri, existing_mechanisms))[0]
         rsp = None
         if old_mech:
-            old_mech = old_mech[0]
             rsp = self.aac.authentication.update_mechanism(id=old_mech['id'], description=mechanism.description, 
                     name=mechanism.name, uri=mechanism.uri, type_id=typeId, predefined=old_mech['predefined'], 
                     properties=props, attributes=mechanism.attributes)
         else:
             rsp = self.aac.authentication.create_mechanism(description=mechanism.description, name=mechanism.name,
                     uri=mechanism.uri, type_id=typeId,  properties=props, attributes=mechanism.attributes)
         if rsp.success == True:
-            _logger.info("Successfully set configuration for {} mechanism".format(mechanism.name))
+            _logger.info("Successfully set configuration for {} mechanism.".format(mechanism.name))
             self.needsRestart = True
         else:
             _logger.error("Failed to set configuration for {} mechanism with:\n{}\n{}".format(
                 mechanism.name, json.dumps(mechanism, indent=4), rsp.data))
 
     def _configure_policy(self, existing_policies, policy):
         rsp = None
-        old_policy = list(filter(lambda p: p['uri'] == policy.uri, existing_policies))
+        old_policy = optional_list(filter_list('uri', policy.uri, existing_policies))[0]
         if old_policy:
-            old_policy = old_policy[0]
             rsp = self.aac.authentication.update_policy(old_policy['id'], name=policy.name, policy=policy.policy, uri=policy.uri,
                     description=policy.description, predefined=old_policy['predefined'], enabled=policy.enabled)
         else:
             rsp = self.aac.authentication.create_policy(name=policy.name, policy=policy.policy, uri=policy.uri, description=policy.description,
                     enabled=policy.enabled)
         if rsp.success == True:
             _logger.info("Successfully set configuration for {} policy".format(policy.name))
             self.needsRestart = True
         else:
             _logger.error("Failed to set configuration for {} policy with:\n{}\n{}".format(
                 policy.name, json.dumps(policy, indent=4), rsp.data))
 
-
-
     class Authentication(typing.TypedDict):
         '''
         Example::
 
                   authentication:
                     mechanisms:
                     - name: "Verify Demo - QR Code Initiate"
@@ -1462,22 +1527,22 @@
                     - name: "Username Password"
                       uri: "urn:ibm:security:authentication:asf:mechanism:password"
                       description: "Username password authentication"
                       type: "Username Password"
                       properties:
                       - usernamePasswordAuthentication.ldapHostName: "openldap"
                       - usernamePasswordAuthentication.loginFailuresPersistent: "false"
-                      - usernamePasswordAuthentication.ldapBindDN: "cn=root,secAuthority=Default"
+                      - usernamePasswordAuthentication.ldapBindDN: !secret default/isva-secrets:ldap_bind_dn
                       - usernamePasswordAuthentication.maxServerConnections: "16"
                       - usernamePasswordAuthentication.mgmtDomain: "Default"
                       - usernamePasswordAuthentication.sslEnabled: "true"
                       - usernamePasswordAuthentication.ldapPort: "636"
                       - usernamePasswordAuthentication.sslTrustStore: "lmi_trust_store"
                       - usernamePasswordAuthentication.userSearchFilter: "usernamePasswordAuthentication.userSearchFilter"
-                      - usernamePasswordAuthentication.ldapBindPwd: "Passw0rd""
+                      - usernamePasswordAuthentication.ldapBindPwd: !secret default/isva-secrets:ldap_bind_pwd
                       - usernamePasswordAuthentication.useFederatedDirectoriesConfig: "false"
                     - name: "TOTP One-time Password"
                       uri: "urn:ibm:security:authentication:asf:mechanism:totp"
                       description: "Time-based one-time password authentication"
                       type: "TOTP One-time Password"
                       properties:
                       - otp.totp.length: "6"
@@ -1491,15 +1556,15 @@
                       - otp.totp.timeStepSkew: "10"
                     - name: "reCAPTCHA Verification"
                       uri: "urn:ibm:security:authentication:asf:mechanism:recaptcha"
                       description: "Human user verification using reCAPTCHA Version 2.0."
                       type: "ReCAPTCHAAuthenticationName"
                       properties:
                       - reCAPTCHA.HTMLPage: "/authsvc/authenticator/recaptcha/standalone.html"
-                        reCAPTCHA.apiKey: "6LchOAgUAAAAAAqUuuyy8XLDkO8LJOq-bCLynVoj"
+                        reCAPTCHA.apiKey: !secret default/isva-secrets:recaptcha_key
                     - name: "End-User License Agreement"
                       uri: "urn:ibm:security:authentication:asf:mechanism:eula"
                       description: "End-user license agreement authentication"
                       type: "End-User License Agreement"
                       properties:
                       - eulaAuthentication.acceptIfLastAcceptedBefore: "true"
                       - eulaAuthentication.alwaysShowLicense: "false"
@@ -1588,15 +1653,15 @@
                     return
                 existing_mechanisms = self.aac.authentication.list_mechanisms().json
                 if existing_mechanisms == None:
                     existing_mechanisms = []
                 for mechanism in aac_config.authentication.mechanisms:
                     self._configure_mechanism(mech_types, existing_mechanisms, mechanism)
             if self.needsRestart == True:
-                deploy_pending_changes() # Mechanisms must be deployed before they are usable in policies
+                deploy_pending_changes(self.factory, self.config) # Mechanisms must be deployed before they are usable in policies
                 self.needsRestart = False
             if aac_config.authentication.policies != None:
                 existing_policies = self.aac.authentication.list_policies().json
                 if existing_policies == None:
                     existing_policies = []
                 for policy in aac_config.authentication.policies:
                     self._configure_policy(existing_policies, policy)
@@ -1649,75 +1714,89 @@
         endpoints: typing.Optional[Endpoints]
         'An object containing the endpoints returned from the registration QR code or the discovery endpoint. If configured, overwrites hostname, port, and junction configuration.'
         discovery_mechanisms: typing.Optional[typing.List[str]]
         'A list of authentication mechanism URIs to be included in the discovery endpoint response.'
 
     def mmfa_configuration(self, aac_config):
         if aac_config.mmfa != None:
+            methodArgs = copy.deepcopy(aac_config.mmfa)
             if aac_config.api_protection != None and aac_config.api_protection.clients != None:
-                api_clients = self.aac.api_protection.list_clients()
-                for client in api_clietns:
-                    if client.name == aac_config.mmfa.client_id:
-                        aac_config.mmfa.client_id = client.name
+                api_clients = self.aac.api_protection.list_clients().json
+                for client in api_clients:
+                    if client['name'] == aac_config.mmfa.client_id:
+                        methodArgs['client_id'] = client['clientId']
                         break
-            methodArgs = copy.deepcopy(aac_config.mmfa)
             endpoints = methodArgs.pop("endpoints", None)
             if endpoints:
                 methodArgs.update({**endpoints})
-            rsp = self.aac.mmfaconfig.update(**aac_config.mmfa)
+            rsp = self.aac.mmfaconfig.update(**methodArgs)
             if rsp.success == True:
                 _logger.info("Successfully updated MMFA configuration")
                 self.needsRestart = True
             else:
                 _logger.error("Failed to update MMFA configuration with:\n{}\n{}".format(
                     json.dumps(aac_config.mmfa, indent=4), rsp.data))
 
 
     def _upload_metadata(self, metadata):
         metadata_list = FILE_LOADER.read_files(metadata)
         for metadata_file in metadata_list:
             rsp = self.aac.fido2_config.create_metadata(filename=metadata_list['path'])
             if rsp.success == True:
+                self.needsRestart = True
                 _logger.info("Successfully created {} FIDO metadata".foramt(metadata_file['name']))
             else:
                 _logger.error("Failed to create {} FIDO metadata".format(metadata_file["name"]))
 
+
+    def _create_mds(self, mds):
+        rsp = self.aac.fido2_config.create_metadata_service(**mds)
+        if rsp.success == True:
+            self.needsRestart = True
+            _logger.info("Successfully created {} FIDO metadata service".foramt(mds.url))
+        else:
+            _logger.error("Failed to create FIDO metadata service:\n{}\n{}".format(
+                                                                json.dumps(mds, indent=4), rsp.data))
+
+
     def _upload_mediator(self, mediator):
         mediator_list = FILE_LOADER.read_files(mediator)
         for mediator_rule in mediator_list:
             rsp = self.aac.fido2_config.create_mediator(name=mediator_rule['name'], filename=mediator_rule['path'])
             if rsp.success == True:
+                self.needsRestart = True
                 _logger.info("Successfully created {} FIDO2 Mediator".format(mediator_rule['name']))
             else:
                 _logger.error("Failed to create {} FIDO2 Mediator".format(mediator_rule['name']))
 
     def _create_relying_party(self, rp):
+        rp_metadata = rp.get("metadata", []) # Need empty list instead of None
         if rp.metadata:
-            metadata_list = self.aac.fido2_config.list_metadata().json
+            metadata_list = optional_list(self.aac.fido2_config.list_metadata().json)
             for pos, metadata in enumerate(rp.metadata):
                 for uploaded_metadata in metadata_list:
                     if uploaded_metadata['filename'] == metadata:
-                        rp.metadata[pos] = uploaded_metadata['id']
+                        rp_metadata[pos] = uploaded_metadata['id']
                         break
         if rp.use_all_metadata:
-            metadata_list = self.aac.fido2_config.list_metadata().json
+            metadata_list = optional_list(self.aac.fido2_config.list_metadata().json)
             for uploaded_metadata in metadata_list:
-                rp.metadata += [uploaded_metadata['id']]
+                rp_metadata += [uploaded_metadata['id']]
 
         if rp.mediator:
             medaitor_list = self.aac.fido2_config.list_mediator().json
             for mediator in mediator_list:
                 if mediator['fileName'] == rp.mediator:
                     rp.mediator = mediator['id']
                     break
         methodArgs = {
                 "name": rp.name,
                 "rp_id": rp.rp_id,
                 "origins": rp.origins,
-                "metadata_set": rp.metadata,
+                "metadata_set": rp_metadata,
                 "metadata_soft_fail": rp.metadata_soft_fail,
                 "mediator_mapping_rule_id": rp.mediator,
                 "relying_party_impersonation_group": rp.impersonation_group
             }
         if rp.attestation:
             methodArgs.update({
                 "attestation_statement_types": rp.attestation.statement_types,
@@ -1727,25 +1806,58 @@
             if rp.android:
                 methodArgs.update({
                         "attestation_android_safetynet_max_age": rp.attestation.android.max_age,
                         "attestation_android_safetynet_clock_skew": rp.attestation.android.clock_skew
                     })
         rsp = self.aac.fido2_config.create_relying_party(**methodArgs)
         if rsp.success == True:
+            self.needsRestart = True
             _logger.info("Successfully created {} FIDO2 Relying Party".format(rp.name))
         else:
             _logger.error("Failed to create {} FIDO2 Relying Party with configuration:\n{}\n{}".format(rp.name,
-                json.dumps(rp, indent=4), rsp.content))
+                json.dumps(rp, indent=4), rsp.data))
 
 
     class Fast_Identity_Online2(typing.TypedDict):
         '''
         Example::
 
-                TO: DO
+                fido2:
+                  relying_parties:
+                  - name: "fidointerop.securitypoc.com"
+                    rp_id: "fidointerop.securitypoc.com"
+                    origins:
+                    - "https://fidointerop.securitypoc.com"
+                    - "urn:ibm:security:verify:app:namespace"
+                    use_all_metadata: true
+                    metadata_soft_fail: false
+                    metadata_services:
+                    - url: "https://mds3.fidoalliance.org"
+                      truststore: "rt_profile_keys"
+                      jws_truststore: "fido_mds_certs"
+                    mediator: "fido2_mediator_verifysecuritypoc.js"
+                    attestation:
+                      statement_types:
+                      - "basic"
+                      - "self"
+                      - "attCA"
+                      - "anonCA"
+                      - "none"
+                      statement_formats:
+                      - "fido-u2f"
+                      - "packed"
+                      - "self"
+                      - "android-key"
+                      - "android-safetynet"
+                      - "tpm"
+                      - "none"
+                  metadata:
+                    metadata:
+                    - "fido2/metadata"
+                    metadata_services:
 
         '''
         class Relying_Party(typing.TypedDict):
             class Attestation:
                 statement_types: typing.Optional[typing.List[str]]
                 'List of attestation types to permit.'
                 statement_formats: typing.Optional[typing.List[str]]
@@ -1779,16 +1891,44 @@
             'Attestation properties permitted for this relying party.'
             android: typing.Optional[Android]
             'Androind attestation specific configuration.'
 
         class Metadata(typing.TypedDict):
 
             class Metadata_Service(typing.TypedDict):
+                class Header(typing.TypedDict):
+                    name: str
+                    'The name of the HTTP header.'
+                    value: str
+                    'The value of the HTTP header.'
+
                 url: str
                 'Address of the metadata service.'
+                retry_interval: typing.Optional[int]
+                'When the lifetime of a downloaded metadata has expired and a request to retrieve the new metadata fails, this defines the wait interval (in seconds) before retrying the download. If not specified the default value of 3600 seconds will be used. A value of 0 will result in a retry on each attestation validation.'
+                jws_truststore: typing.Optional[str]
+                'The name of the JWS verification truststore. The truststore contains the certificate used to verify the signature of the downloaded metadata blob. If not specified the SSL trust store or the trust store configured in the HTTPClientV2 advanced configuration will be used.'
+                truststore: typing.Optional[str]
+                'The name of the truststore to use. The truststore has a dual purpose. Firstly it is used when making a HTTPS connection to the Metadata Service. Secondly if the jwsTruststore is not specified it must contain the certificate used to verify the signature of the downloaded metadata blob. If not specified and a HTTPS connection is specified, the trust store configured in the HTTPClientV2 advanced configuration will be used.'
+                username: typing.Optional[str]
+                'The basic authentication username. If not specified BA will not be used.'
+                password: typing.Optional[str]
+                'The basic authentication password. If not specified BA will not be used.'
+                keystore: typing.Optional[str]
+                'The client keystore. If not specified client certificate authentication will not be used.'
+                certificate: typing.Optional[str]
+                'The client key alias. If not specified client certificate authentication will not be used.'
+                protocol: typing.Optional[str]
+                'The SSL protocol to use for the HTTPS connection. Valid values are TLS, TLSv1, TLSv1.1 and TLSv1.2. If not specified the protocol configured in the HTTPClientV2 advanced configuration will be used.'
+                timeout: typing.Optional[int]
+                'The request timeout in seconds. A value of 0 will result in no timeout. If not specified the connect timeout configured in the HTTPClientV2 advanced configuration will be used.'
+                proxy: typing.Optional[str]
+                'The URL of the proxy server used to connect to the metadata service (including the protocol).'
+                headers: typing.Optional[typing.List[Header]]
+                'A list of HTTP headers to be added to the HTTP request when retrieving the metadata from the service. '
 
             metadata_services: typing.Optional[typing.List[Metadata_Service]]
             'List of metadata services to enable for the relying party.'
             metadata: typing.Optional[typing.List[str]]
             'List of metadata documents to enable for the relying party.'
 
         mediators: typing.Optional[typing.List[str]]
@@ -1799,16 +1939,18 @@
         'List of relying parties to configure.'
 
 
     def fido2_configuration(self, aac_config):
         if aac_config.fido2 != None:
             fido2 = aac_config.fido2
             if fido2.metadata != None:
-                for metadata in fido2.metadata:
+                for metadata in fido2.metadata.get("metadata", []):
                     self._upload_metadata(metadata)
+                for mds in fido2.metadata.get("metadata_services", []):
+                    self._create_mds(mds)
             if fido2.mediators != None:
                 for mediator in fido2.mediators:
                     self._upload_mediator(mediator)
             if fido2.relying_parties != None:
                 for rp in fido2.relying_parties:
                     self._create_relying_party(rp)
 
@@ -1821,24 +1963,24 @@
                   users:
                   - name: "easuser"
                     password: !secret default/isva-secrets:runtime_password
                     groups:
                     - "scimAdmin"
                     - "fidoAdmin"
                   tuning_parameters:
-                  - name: https_proxy_host
-                    value: http://my.proxy
-                  - name: https_proxy_port
-                    value: 3128
+                  - name: "https_proxy_host"
+                    value: "http://my.proxy"
+                  - name: "https_proxy_port"
+                    value: "3128"
                   endpoints:
-                  - interface: 1.1
-                    address: 192.168.42.102
+                  - interface: "1.1"
+                    address: "192.168.42.102"
                     port: 444
                     ssl: true
-                  - interface: 1.2
+                  - interface: "1.2"
                     dhcp4: true
                     dhcp6: false
                     port: 443
                     ssl: true
 
         '''
 
@@ -1846,14 +1988,20 @@
             name: str
             'Name of the user to create or update.'
             password: str
             'The password for the new user. This can contain any ASCII characters.'
             groups: typing.Optional[typing.List[str]]
             'A list of groups the new user will belong to.'
 
+        class Group(typing.TypedDict):
+            name: str
+            'Name of the group to create or update.'
+            users: typing.Optional[typing.List[str]]
+            'List of users to add to the group.'
+
         class Endpoint(typing.TypedDict):
             interface: str
             'The interface the runtime endpoint will listen on.'
             address: typing.Optional[str]
             'The static address that the runtime endpoint will listen on.'
             dhcp4: typing.Optional[bool]
             'Endpoint should listen on the DHCP IPv4 address for the given interface.'
@@ -1867,42 +2015,120 @@
         class Runtime_Tuning_Parameter(typing.TypedDict):
             name: str
             'The tuning parameter to set.'
             value: str
             'The new value for the specified parameter.'
 
         users: typing.Optional[typing.List[User]]
+        'List of users to add/update in the AAC/Federation runtime user registry. Users are created before groups, so if you are creating a user and a group in the same autoconf; then only add you user to the list of users when creating the group.'
+        groups: typing.Optional[typing.List[Group]]
+        'List of groups to add/update in the AAC/Federation runtime user registry'
         tuning_parameters: typing.Optional[typing.List[Runtime_Tuning_Parameter]]
+        'List of AAC/Federation runtime JVM tuning parameters.'
         endpoints: typing.Optional[typing.List[Endpoint]]
+        'List of http(s) endpoints that the AAC/Federation runtime is listenting on.'
 
     def runtime_configuration(self, aac_config):
         if aac_config.runtime_properties:
-            #TODO
-            return
+            for parameter in aac_config.runtime_properties.get("tuning_parameters", []):
+                rsp = self.aac.runtime_parameters.update_parameter(
+                        parameter=parameter.name, value=parameter.value)
+                if rsp.success == True:
+                    self.needsRestart = True
+                    _logger.info("Successfully updated {} runtime tuning parameter.".format(
+                                                                                    parameter.name))
+                else:
+                    _logger.error("Failed to update parameter:\n{}\n{}".format(
+                                                            json.dumps(parameter, ident=4), rsp.data))
+            if aac_config.runtime_properties.endpoints: # Readable name to Verify Access uuid
+                iface_cfg = optional_list(self.factory.get_system_settings().interfaces.list_interfaces().json)
+                for endpoint in aac_config.runtime_properties.endpoints:
+                    iface_address_uuids = ""
+                    for iface in iface_cfg:
+                        if iface['name'] == endpoint.interface:
+                            iface_address_uuids += iface['uuid']
+                            if endpoint.dhcp4 == True:
+                                iface_address_uuids += ".dhcp.ipv4"
+                            elif endpoint.dhcp6 == True:
+                                iface_address_uuids += ".dhcp.ipv6"
+                            elif endpoint.address:
+                                for address in iface["ipv4"].get("addresses"):
+                                    if address['address'] == endpoint.address:
+                                        iface_address_uuids += "." + address['uuid']
+                                        break
+                    rsp = self.aac.runtime_parameters.add_listening_interface(
+                                                iface_address_uuids, port=endpoint.port, secure=endpoint.ssl)
+                    if rsp.success == True:
+                        self.needsRestart = True
+                        _logger.info("Successfully added runtime endpoint at {}:{}".format(address, port))
+                    else:
+                        _logger.error("Failed to create endpoint:\n:{}\n{}".format(
+                                                                        json.dumps(endpoint, indent=4), rsp.data))
+            if aac_config.runtime_properties.users:
+                old_users = optional_list(self.aac.user_registry.list_users().json)
+                for user in aac_config.runtime_properties.users:
+                    old_user = optional_list(filter_list("id", user.name, old_users))
+                    if old_user:
+                        rsp = self.aac.user_registry.delete_user(old_user['id'])
+                        if rsp.success == True:
+                            self.needsRestart = True
+                            _logger.info("Successfully removed old user from user registry.")
+                        else:
+                            _logger.error("Failed to remove old user from registry, skipping create {} user.".format(
+                                                                                                        user.name))
+                            continue
+                    rsp = self.aac.user_registry.create_user(user.name, passowrd=user.password, groups=user.groups)
+                    if rsp.success == True:
+                        self.needsRestart = True
+                        _logger.info("Successfully added {} to the runtime user registry".format(user.name))
+                    else:
+                        _logger.error("Failed to create user:\n{}\n{}".format(json.dumps(user, indent=4), rsp.data))
+            if aac_config.runtime_properties.groups:
+                old_groups = optional_list(self.aac.user_registry.list_groups().json)
+                for group in aac_config.runtime_properties.groups:
+                    old_group = optional_list(filter_list("id", group.name, old_groups))
+                    if old_group:
+                        rsp = self.aac.user_registry.deletegroup(old_group['id'])
+                        if rsp.success == True:
+                            _logger.info("Successfully removed old group from user registry.")
+                        else:
+                            _logger.error("Failed to remove old group from registry, skipping create {} group.".format(
+                                                                                                        group.name))
+                            continue
+                    rsp = self.aac.user_registry.create_group(group.name, users=groups.users)
+                    if rsp.success == True:
+                        self.needsRestart = True
+                        _logger.info("Successfully added {} to the runtime user registry".format(group.name))
+                    else:
+                        _logger.error("Failed to create group:\n{}\n{}".format(json.dumps(user, indent=4), rsp.data))
+
 
     def configure(self):
         if self.config.access_control == None:
             _logger.info("No Access Control configuration detected, skipping")
             return
         self.runtime_configuration(self.config.access_control)
         self.upload_files(self.config.access_control)
         self.attributes_configuration(self.config.access_control)
         self.obligation_configuration(self.config.access_control)
         self.pip_configuration(self.config.access_control)
         self.push_notifications(self.config.access_control)
         self.server_connections(self.config.access_control)
         self.fido2_configuration(self.config.access_control)
         if self.needsRestart == True:
-            deploy_pending_changes()
+            deploy_pending_changes(self.factory, self.config)
+            self.needsRestart = False
 
-        self.risk_profile(self.config.access_control)
+        self.risk_profiles(self.config.access_control)
         self.access_control(self.config.access_control)
         self.api_protection_configuration(self.config.access_control)
         if self.needsRestart == True:
-            deploy_pending_changes()
+            deploy_pending_changes(self.factory, self.config)
+            self.needsRestart = False
 
         self.authentication_configuration(self.config.access_control)
         self.scim_configuration(self.config.access_control)
         self.mmfa_configuration(self.config.access_control)
         self.advanced_config(self.config.access_control)
         if self.needsRestart == True:
-           deploy_pending_changes()
+           deploy_pending_changes(self.factory, self.config)
+           self.needsRestart = False
```

### Comparing `verify_access_autoconf-0.1.0/src/verify_access_autoconf/appliance.py` & `verify_access_autoconf-0.3.0/src/verify_access_autoconf/appliance.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,36 +326,36 @@
                           'extra_config': confDbExtraConfig
                 }
             rsp = self.appliance.get_system_settings().cluster.set_config_db(**methodArgs)
             if rsp.success == True:
                 _logger.info("Successfully set the configuration database")
             else:
                 _logger.error("Failed to set the configuration database with:{}\n{}".format(
-                    json.dumps(config.config_database, indent=4), rsp.content))
+                    json.dumps(config.config_database, indent=4), rsp.data))
         if config.runtime_database != None:
             hvdbExtraConfig = config.runtime_database.copy()
             methodArgs = {'embedded': False, 'db_type': hvdbExtraConfig.pop('type'), 'host': hvdbExtraConfig.pop('host'),
                           'port': hvdbExtraConfig.po('port'), 'secure': hvdbExtraConfig.pop('ssl'),
                           'db_keystore': hvdbExtraConfig.pop('ssl_keystore'), 'user': hvdbExtraConfig.pop('user'),
                           'passwd': hvdbExtraConfig.pop('password'), 'db_name': hvdbExtraConfig.pop('db_name'),
                           'extra_config': hvdbExtraConfig
                 }
             rsp = self.appliance.get_system_settings().cluster.set_runtime_db(**methodArgs)
             if rsp.success == True:
                 _logger.info("Successfully set the runtime database")
             else:
                 _logger.error("Failed to set the runtime database with: {}\n{}".format(json.dumps(
-                    config.runtime_database, indent=4), rsp.content))
+                    config.runtime_database, indent=4), rsp.data))
         if config.cluster != None:
             rsp = self.appliance.get_system_settings().cluster.update_cluster(**config.cluster)
             if rsp.success == True:
                 _logger.info("Successfully set the cluster configuration")
             else:
                 _logger.error("Failed to set the cluster configuration with:{}\n{}".format(
-                    json.dumps(config.cluster, indent=4), rsp.content))
+                    json.dumps(config.cluster, indent=4), rsp.data))
 
 
     def configure(self):
         self.update_network(self.config.appliance)
         self.date_time(self.config.appliance)
         self.cluster(self.config.appliance)
```

### Comparing `verify_access_autoconf-0.1.0/src/verify_access_autoconf/configure.py` & `verify_access_autoconf-0.3.0/src/verify_access_autoconf/configure.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         if not any(module.get('id', None) == 'wga' and module.get('enabled', "False") == "True" for module in activations):
             self._activateBaseAppliance(config)
         if not any(module.get('id', None) == 'mga' and module.get('enabled', "False") == "True" for module in activations):
             self._activateAdvancedAccessControl(config)
         if not any(module.get('id', None) == 'federation' and module.get('enabled', "False") == "True" for module in activations):
             self._activateFederation(config)
         if self.needsRestart == True:
-            deploy_pending_changes(self.factory, self.config, restartContainers=False)
+            deploy_pending_changes(self.factory, self.config)
             self.needsRestart = False
         _logger.info("appliance activated")
 
 
     def _import_signer_certs(self, database, parsed_file):
         ssl = self.factory.get_system_settings().ssl_certificates
         rsp = ssl.import_signer(database, os.path.abspath(parsed_file['path']), label=parsed_file['name'])
@@ -595,15 +595,15 @@
             snapshotConfig = config.snapshot
             rsp = self.factory.get_system_settings().snapshot.upload(snapshotConfig.snapshot)
             if rsp.success == True:
                 _logger.info("Successfully applied snapshot [{}]".format(snapshotConfig.snapshot))
                 deploy_pending_changes(self.factory, self.config)
             else:
                 _logger.error("Failed to apply snapshot [{}]\n{}".format(snapshotConfig.snapshot),
-                        rsp.content)
+                        rsp.data)
 
 
     def configure_base(self, appliance, container):
         base_config = None
         model = None
         if self.config.appliance is not None:
             base_config = self.config.applianc
```

### Comparing `verify_access_autoconf-0.1.0/src/verify_access_autoconf/container.py` & `verify_access_autoconf-0.3.0/src/verify_access_autoconf/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 @copyright: IBM
 """
 import logging
 import requests
 import json
 import typing
+import copy
 
 from .util.constants import HEADERS
 from .util.configure_util import deploy_pending_changes
 from .util.data_util import Map
 
 _logger = logging.getLogger(__name__)
 
@@ -66,17 +67,17 @@
 
     def configure_database(self, clusterConfig):
         system = self.factory.get_system_settings()
         if clusterConfig == None or clusterConfig.runtime_database == None:
             _logger.info("Cannot find HVDB configuration, in a docker environment this is probably bad")
             return
         self.needsRestart = True
-        database = clusterConfig.runtime_database.copy()
+        database = copy.deepcopy(clusterConfig.runtime_database)
         methodArgs = {'db_type': database.pop('type'), 'host': database.pop('host'), 'port': database.pop('port'),
-                      'secure': database.pop('ssl'), 'db_keystore': database.pop('ssl_keystore'), 
+                      'secure': database.pop('ssl'), 'db_key_store': database.pop('ssl_keystore', None), 
                       'user': database.pop('user'), 'passwd': database.pop('password'), 'db_name': database.pop('db_name'), 
                       'extra_config': database
             }
         rsp = system.cluster.set_runtime_db(**methodArgs)
         if rsp.success == True:
             _logger.info("Successfully configured HVDB")
         else:
@@ -87,11 +88,11 @@
     def configure(self):
         containerConfig = self.config.container
         if containerConfig == None:
             _logger.info("Unable to find container specific configuration")
             return
         self.configure_database(containerConfig.cluster)
         if self.needsRestart == True:
-            deploy_pending_changes(self.factory, self.config)
+            deploy_pending_changes(self.factory, self.config, restartContainers=False)
 
 if __name__ == "__main__":
     configure()
```

### Comparing `verify_access_autoconf-0.1.0/src/verify_access_autoconf/federation.py` & `verify_access_autoconf-0.3.0/src/verify_access_autoconf/federation.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 import json
 import os
 import logging
 import typing
 
 from .util.configure_util import deploy_pending_changes
-from .util.data_util import Map, FILE_LOADER
+from .util.data_util import Map, FILE_LOADER, optional_list, filter_list, to_camel_case
 
 _logger = logging.getLogger(__name__)
 
 class Federation_Common(typing.TypedDict):
     '''
-    Data structures which are shared between the different types of Federation protocols/roles
+    Data structures which are shared between the different types of Federation protocols/roles.
     '''
     class Basic_Configuration(typing.TypedDict):
         active_delegate_id: str
         'The active module instance. Valid values are "noMetadata" and "metadataEndpointUrl".'
         metadata_endpoint_url: typing.Optional[str]
         'The /metadata endpoint URL of the provider. Only valid if ``active_delegate_id`` is "metadataEndpointUrl".'
         issuer_identifier: typing.Optional[str]
@@ -38,27 +38,29 @@
         'The certificate database name.'
         label: str
         'The certificate or key label.'
 
     class Advanced_Configuration(typing.TypedDict):
         active_delegate_id: str
         'The active module instance. Valid values are "skip-advance-map" and "default-map".'
-        mapping_rule_reference: str
+        mapping_rule: str
         'A reference to an ID or name of an advance configuration mapping rule.'
+        rule_type: str
+        'The type of the mapping rule. The only supported type currently is "JAVASCRIPT".'
 
     class Assertion_Settings(typing.TypedDict):
-        assertion_attribute_types: typing.Optional[typing.List[str]]
+        attribute_types: typing.Optional[typing.List[str]]
         'A setting that specifies the types of attributes to include in the assertion. An asterisk (*) indicates that all of the attribute types that are specified in the identity mapping file or by the custom mapping module will be included in the assertion. The default value is ["*"]. This configuration is applicable to an identity provider federation partner.'
         session_not_on_or_after: typing.Optional[int]
         'The number of seconds that the security context established for the principal should be discarded by the service provider. The default value is 3600. This configuration is applicable to an identity provider federation partner.'
         create_multiple_attribute_statements: typing.Optional[bool]
         'A setting that specifies whether to keep multiple attribute statements in the groups in which they were received. This option might be necessary if your custom identity mapping rules are written to operate on one or more specific groups of attribute statements.'
-        assertion_valid_before: typing.Optional[int]
+        valid_before: typing.Optional[int]
         'The number of seconds before the issue date that an assertion is considered valid. This configuration is applicable to an identity provider federation. The default value is 60.'
-        assertion_valid_after: typing.Optional[int]
+        valid_after: typing.Optional[int]
         'The number of seconds the assertion is valid after being issued. This configuration is applicable to an identity provider federation. The default value is 60.'
 
     class Assertion_Consumer_Service(typing.TypedDict):
         binding: str
         'A setting that specifies the communication method used to transport the SAML messages. The valid values are "artifact", "post", and "redirect".'
         default: bool
         'A setting that specifies whether it is the default endpoint.'
@@ -74,71 +76,69 @@
         'A setting that specifies whether it is the default endpoint.  If not provided, the default value is ``false``.'
         index: typing.Optional[int]
         'A reference to a particular endpoint. The default value is 0.'
         url: typing.Optional[str]
         'The URL of the endpoint. If not provided, the value is automatically generated from the point of contact URL.'
 
     class Attribute_Mapping(typing.TypedDict):
-        class Source:
-            name: str
-            'Name of the source.'
-            source: str
-            'Attribute Source ID. '
-
-        map: typing.List[Source]
-        'List of configured attribute sources. '
+        name: str
+        'Name of the source.'
+        source: str
+        'Attribute Source ID. '
 
     class Encryption_Settings(typing.TypedDict):
+
         class Key_Identifier(typing.TypedDict):
             store: str
             'The certificate database name.'
             label: str
             'The certificate or key label.'
 
-        class Encryption_Options(typing.TypedDict):
-            encrypt_name_id: bool
-            'A setting that specifies whether the name identifiers should be encrypted.'
-            encrypt_assertion: bool
-            'A setting that specifies whether to encrypt assertions.'
-            encrypt_assertion_attributes: bool
-            'A setting that specifies whether to encrypt assertion attributes.'
-
-        block_encryption_algorithm: typing.Optional[str]
+        block_algorithm: typing.Optional[str]
         'Block encryption algorithm used to encrypt and decrypt SAML message. Valid values are "AES-128", "AES-192", "AES-256", and "TRIPLEDES". If not provided, the default value is "AES-128".'
-        encryption_key_transport_algorithm: typing.Optional[str]
+        key_transport_algorithm: typing.Optional[str]
         'Key transport algorithm used to encrypt and decrypt keys. Valid values are "RSA-v1.5" and "RSA-OAEP". If not provided, the default value is "RSA-OAEP". If the supplied encryptionKeyIdentifier corresponds to a network HSM device, the "RSA-OAEP" key transport is not allowed.'
-        encryption_key_identifier: typing.Optional[Key_Identifier]
+        key_identifier: typing.Optional[Key_Identifier]
         'The certificate for encryption of outgoing SAML messages. If not provided, the default value is null.'
-        encryption_options: typing.Optional[Encryption_Options]
-        'The encryption options.'
         decryption_key_identifier: typing.Optional[Key_Identifier]
         'A public/private key pair that the federation partners can use to encrypt certain message content. The default value is null.'
+        key_store: str
+        'The certificate database name.'
+        key_alias: str
+        'The certificate or key label.'
+        encrypt_name_id: bool
+        'A setting that specifies whether the name identifiers should be encrypted.'
+        encrypt_assertion: bool
+        'A setting that specifies whether to encrypt assertions.'
+        encrypt_assertion_attributes: bool
+        'A setting that specifies whether to encrypt assertion attributes.'
+
 
     class Identity_Mapping(typing.TypedDict):
         class Default_Mapping_Properties(typing.TypedDict):
             rule_type: str
             'The type of the mapping rule. The only supported type currently is "JAVASCRIPT".'
-            mapping_rule_reference: str
+            mapping_rule: str
             'A reference to an ID or name of a mapping rule.'
         
         class Custom_Mapping_Properties(typing.TypedDict):
             applies_to: str
-            'Refers to STS chain that consumes call-out response. Required if WSTRUST messageFormat is specified, invalid otherwise.'
+            'Refers to STS chain that consumes call-out response. Required if "WSTRUST" ``message_format`` is specified, invalid otherwise.'
             auth_type: str
             'Authentication method used when contacting external service. Supported values are "NONE", "BASIC" or "CERTIFICATE"'
             basic_auth_username: typing.Optional[str]
-            'Username for authentication to external service. Required if "BASIC" authType is specified, invalid otherwise.'
+            'Username for authentication to external service. Required if "BASIC" ``auth_type`` is specified, invalid otherwise.'
             basic_auth_password: typing.Optional[str]
-            'Password for authentication to external service. Required if "BASIC" authType is specified, invalid otherwise.'
+            'Password for authentication to external service. Required if "BASIC" ``auth_type`` is specified, invalid otherwise.'
             client_key_store: typing.Optional[str]
-            'Contains key for HTTPS client authentication. Required if "CERTIFICATE" authType is specified, invalid otherwise.'
+            'Contains key for HTTPS client authentication. Required if "CERTIFICATE" ``auth_type`` is specified, invalid otherwise.'
             client_key_alias: typing.Optional[str]
-            'Alias of the key for HTTPS client authentication. Required if "CERTIFICATE" authType is specified, invalid otherwise.'
+            'Alias of the key for HTTPS client authentication. Required if "CERTIFICATE" ``auth_type`` is specified, invalid otherwise.'
             issuer_uri: typing.Optional[str]
-            'Refers to STS chain that provides input for call-out request. Required if WSTRUST messageFormat is specified, invalid otherwise.'
+            'Refers to STS chain that provides input for call-out request. Required if "WSTRUST" ``message_format`` is specified, invalid otherwise.'
             message_format: str
             'Message format of call-out request. Supported values are "XML" or "WSTRUST".'
             ssl_key_store: str
             'SSL certificate trust store to use when validating SSL certificate of external service.'
             uri: str
             'Address of destination server to call out to.'
 
@@ -146,21 +146,21 @@
         'The active mapping module instance. Valid values are "skip-identity-map", "default-map" and "default-http-custom-map".'
         properties: typing.Union[Default_Mapping_Properties, Custom_Mapping_Properties]
         'The mapping module specific properties.'
 
     class Extension_Mapping(typing.TypedDict):
         active_delegate_id: str
         'The active mapping module instance. Valid values are "skip-extension-map" and "default-map". If this is a partner the value "federation-config" is also valid.'
-        mapping_rule_reference: str
+        mapping_rule: str
         'A reference to an ID or name of an extension mapping rule.'
 
     class Authn_Req_Mapping(typing.TypedDict):
         active_delegate_id: str
         'The active mapping module instance. Valid values are "skip-authn-request-map" and "default-map". If this is a partner the value "federation-config" is also valid.'
-        mapping_rule_reference: str
+        mapping_rule: str
         'A reference to an ID or name of an authentication request mapping rule.'
 
     class Service_Data(typing.TypedDict):
         binding: str
         'A setting that specifies the communication method used to transport the SAML messages. The valid values are "artifact", "post", "redirect" and "soap".'
         url: typing.Optional[str]
         'The URL of the endpoint. Except for "soap" binding, the value is automatically generated from the point of contact URL and will not be updated by POST or PUT operation. For "soap" binding, if not provided, the value is automatically generated from the point of contact URL.'
@@ -187,65 +187,65 @@
             'A setting that specifies whether to sign the artifact request. The default value is ``false``.'
             sign_artifact_response: typing.Optional[bool]
             'A setting that specifies whether to sign the artifact response. The default value is ``false``.'
             sign_logout_request: typing.Optional[bool]
             'A setting that specifies whether to sign the authentication responses. The default value is ``false``.'
             sign_logout_response: typing.Optional[bool]
             'A setting that specifies whether to sign the logout response. The default value is ``false``.'
-            sign_name_id_mgmt_request: typing.Optional[bool]
+            sign_name_id_management_request: typing.Optional[bool]
             'A setting that specifies whether to sign the name ID management request. The default value is ``false``.'
-            sign_name_id_mgmt_response: typing.Optional[bool]
+            sign_name_id_management_response: typing.Optional[bool]
             'A setting that specifies whether to sign the name ID management response. The default value is ``false``.'
 
         class Validation_Options(typing.TypedDict):
             validate_authn_request: typing.Optional[bool]
             'A setting that specifies whether to validate the digital signature of an authentication request. The default value is ``false``.'
             validate_assertion: typing.Optional[bool]
             'A setting that specifies whether to validate the digital signature of an assertion. The default value is ``false``.'
             validate_artifact_request: typing.Optional[bool]
             'A setting that specifies whether to validate the digital signature of an artifact request.'
-            validate_artifact_reqpose: typing.Optional[bool]
+            validate_artifact_response: typing.Optional[bool]
             'A setting that specifies whether to validate the digital signature of an artifact response.'
             validate_logout_request: typing.Optional[bool]
             'A setting that specifies whether to validate the digital signature of a logout request.'
             validate_logout_response: typing.Optional[bool]
             'A setting that specifies whether to validate the digital signature of a logout response.'
             validate_name_id_management_request: typing.Optional[bool]
             'A setting that specifies whether to validate the digital signature of a name ID management request.'
-            validate_name_id_mgmt_reqponse: typing.Optional[bool]
+            validate_name_id_management_response: typing.Optional[bool]
             'A setting that specifies whether to validate the digital signature of a name ID management response. '
 
         class Key_Info_Elements(typing.TypedDict):
             include_public_key: typing.Optional[bool]
             'A setting that specifies whether to include the public key in the KeyInfo element in the digital signature when signing a SAML message or assertion. The default value is ``false``.'
             include_x509_certificate_data: typing.Optional[bool]
             'A setting that specifies whether to include the base 64 encoded certificate data to be included in the KeyInfo element in the digital signature when signing a SAML message or assertion. The default value is ``true``.'
-            include_x509_issuer_detials: typing.Optional[bool]
+            include_x509_issuer_details: typing.Optional[bool]
             'A setting that specifies whether to include the issuer name and the certificate serial number in the KeyInfo element in the digital signature when signing a SAML message or assertion. The default value is ``false``.'
             include_x509_subject_key_identifier: typing.Optional[bool]
             'A setting that specifies whether to include the X.509 subject key identifier in the KeyInfo element in the digital signature when signing a SAML message or assertion. The default value is ``false``.'
             include_x509_subject_name: typing.Optional[bool]
             'A setting that specifies whether to include the subject name in the KeyInfo element in the digital signature when signing a SAML message or assertion. The default value is ``false``.'
 
         signature_algorithm: str
         'The signature algorithm to sign and validate SAML messages and assertions. Valid values are "RSA-SHA1", "RSA-SHA256", and "RSA-SHA512". If not provided, the default value is "RSA-SHA256".'
         digest_algorithm: str
         'The hash algorithm to apply to the transformed resources and validate its integrity. Valid values are "SHA1", "SHA256" and "SHA512". If not provided, the default value matches the configured signature algorithm - "SHA1" for "RSA-SHA1", "SHA256" for "RSA-SHA256", and "SHA512" for "RSA-SHA512".'
-        validation_key_identifier: typing.Optional[Key_Identifier]
-        'The certificate to use to validate the signatures on the incoming SAML assertions and messages. The default value is null.'
         signing_options: typing.Optional[Signing_Options]
         'The signing options.'
         validation_options: typing.Optional[Validation_Options]
         'The validation options.'
         include_inclusive_namespaces: typing.Optional[bool]
         'A setting that specifies whether to include the InclusiveNamespaces element in the digital signature. If provided, it takes precedence over the value that is configured for this partner\'s federation. If not provided, the value that is configured for this partner\'s federation is used.'
         key_info_elements: typing.Optional[Key_Info_Elements]
         'The KeyInfo elements to include in the digital signature.'
         signing_key_identifier: typing.Optional[Key_Identifier]
         'A public/private key pair for signing the SAML messages and the assertion. If not provided, the default value is null.'
+        validation_key_identifier: typing.Optional[Key_Identifier]
+        'The certificate to use to validate the signatures on the incoming SAML assertions and messages. The default value is null.'
 
     class Single_Sign_On_Service(typing.TypedDict):
         binding: str
         'A setting that specifies the communication method used to transport the SAML messages. The valid values are "artifact", "post" and "redirect".'
         url: str
         'The URL of the endpoint.'
 
@@ -261,29 +261,24 @@
         class Server_Certificate_Validation(typing.TypedDict):
             store: str
             'The certificate database name.'
             label: typing.Optional[str]
             'The certificate label. If not provided, all certificates in the specified certificate database will be trusted. '
 
         class Client_Auth_Data(typing.TypedDict):
-            class Basic_Authentication(typing.TypedDict):
-                username: str
-                'The basic authentication username.'
-                password: str
-                'The basic authentication password.'
-
-            class Certificate_Authentication(typing.TypedDict):
-                keystore: str
-                'The certificate database name.'
-                label: str
-                'The personal certificate label.'
-
             method: str
             'The authentication method. To enable the basic authentication method, enter "ba". To enable the client certificate authentication, enter "cert". To disable client authentication, enter "none".'
-            properties: typing.Optional[typing.Union[Certificate_Authentication, Basic_Authentication]]
+            basic_auth_username: typing.Optional[str]
+            'The basic authentication username.'
+            basic_auth_password: typing.Optional[str]
+            'The basic authentication password.'
+            client_key_store: typing.Optional[str]
+            'The certificate database name.'
+            client_key_alias: typing.Optional[str]
+            'The personal certificate label.'
     
         server_cert_validation: Server_Certificate_Validation
         'The server certificate validation data.'
         client_auth_data: Client_Auth_Data
         'The client authentication data.'
 
 ############################################################################################################
@@ -299,14 +294,15 @@
     config = Map()
 
 
     def __init__(self, config, factory): 
         self.fed = factory.get_federation()
         self.factory = factory
         self.config = config
+        self.needsRestart = False
 
 
     class Point_Of_Contact_Profiles(typing.TypedDict):
         '''
         Example::
 
                 point_of_contact_profiles:
@@ -325,15 +321,15 @@
                     - name: "fim.user.response.header.name"
 	                  value: "am-fim-eai-user-id"
                   local_id_callbacks:
                   - index: 0
                     module_reference_id: "websealPocLocalIdentityCallback"
                     parameters:
                     - name: "fim.cred.request.header.name"
-                      "value": "iv-creds"
+                      value: "iv-creds"
                   sign_out_callbacks:
                   - index: 0
                     module_reference_id: "websealPocSignOutCallback"
                     parameters:
                     - name: "fim.user.session.id.request.header.name"
 	                  value: "user_session_id"
                   authn_policy_callbacks:
@@ -379,50 +375,79 @@
         point_of_contact_profiles: typing.List[Point_Of_Contact_Profile]
         'List of point of contact profiles to configure'
         active_profile: str
         'The name of the Point of Contact profile which should be the active profile. Only one profile can be active at a time.'
 
     def configure_poc(self, federation_config):
         if federation_config.point_of_contact_profiles != None:
+            old_pocs = optional_list(self.fed.poc.list_profiles().json)
             for poc in federation_config.point_of_contact_profiles:
+                old_poc = optional_list(filter_list('name', poc.name, old_pocs))[0]
                 methodArgs = copy.deepcopy(poc)
                 #Convert keys from snake to camel case
                 for prop in ["sign_in_callbacks", "local_id_callbacks", "sign_out_callbacks", "authn_policy_callbacks"]:
                     if prop in methodArgs:
-                        methodArgs[prop] = remap_dict(methodArgs.pop(prop), {"module_reference_id", "moduleReferenceId"})
+                        methodArgs[to_camel_case(prop)] = remap_dict(methodArgs.pop(prop), {"module_reference_id", "moduleReferenceId"})
 
-                rsp = self.fed.poc.create_like_credential(**methodArgs)
+                rsp = None; verb = None
+                if old_poc:
+                    rsp = self.fed.poc.update_profile(old_poc['id'], **methodArgs)
+                    verb = "updated" if rsp.success == True else "update"
+                else:
+                    rsp = self.fed.poc.create_profile(**methodArgs)
+                    verb = "created" if rsp.success == True else "create"
                 if rsp.success == True:
-                    _logger.info("Successfully configured {} Point of Contact".format(poc.name))
+                    _logger.info("Successfully {} {} Point of Contact".format(verb, poc.name))
                 else:
-                    _logger.error("Failed to configure {} point of contact with config:\n{}\n{}".format(
-                        poc.name, json.dumps(poc, indent=4), rsp.data))
+                    _logger.error("Failed to {} {} point of contact with config:\n{}\n{}".format(
+                                            verb, poc.name, json.dumps(poc, indent=4), rsp.data))
 
             if "active_profile" in federation_config.point_of_contact_profiles:
-                poc_profiles = self.fed.poc.get_profiles().json
+                poc_profiles = self.fed.poc.list_profiles().json
                 if poc_profiles:
-                    profile_to_activate = list(filter(lambda x: x['name'] == federation_config.point_of_contact_profiles.active_profile))
-                    if profile_to_activate and len(profile_to_activate) == 1:
-                        rsp = self.fed.poc.set_current_profile(profile_to_activate[0]['id'])
+                    profile_to_activate = optional_list(filter_list(
+                            'name', federation_config.point_of_contact_profiles.active_profile, poc_profiles))[0]
+                    if profile_to_activate:
+                        rsp = self.fed.poc.set_current_profile(profile_to_activate['id'])
                         if rsp.success == True:
                             _logger.info("Successfully updated the active POC profile to {}".format(
                                                             federation_config.point_of_contact_profiles.active_profile))
                         else:
                             _logger.error("Failed to update the active POC profile to {}".format(
                                                             federation_config.point_of_contact_profiles.active_profile))
                     else:
-                        _logger.error("Could not find the {} POC profile to activate".format(
+                        _logger.error("Could not find the {} POC profile to activate.".format(
                                                             federation_config.point_of_contact_profiles.active_profile))
 
 
     class Security_Token_Service(typing.TypedDict):
         '''
         Example::
 
-                TO: DO
+                sts:
+                  chains:
+                  - id: "appliance-post-token-map-module"
+                    name: "OAuth20 Appliance Post Token Map Module"
+                    description: "appliance-post-token-map-module"
+                    moduleId: "OAuth20AppliancePostTokenMapModule"
+                    configuration :
+                    - name: "example_config_name_1"
+                        value: "example_config_value_1"
+                    supportedModes:
+                    - "map"
+                  chain_templates:
+                  - name:	"STS Chain Template name"
+		            description: "STS Chain Template description"
+		            chain_items: 
+                    - id: "default-map"
+				      mode: "map"
+				      prefix: "uuid3dbf4c6a-013d-15d5-bb8b-c2665e02a402"
+				    - id: "default-dynamic_chain"
+				      mode": verify"
+				      prefix: "uuid3dbf4c6c-013d-1c48-85c8-c2665e02a402"
 
         '''
         class Chain_Template(typing.TypedDict):
             class Item(typing.TypedDict):
                 id: str
                 'The token id of an STS module.'
                 mode: str
@@ -435,17 +460,17 @@
             description: str
             'A description of the STS Chain Template.'
             modules: typing.List[Item]
             'An array of the modules that make up the STS Chain Template.'
         
         class Chain(typing.TypedDict):
             class Key_Identifier(typing.TypedDict):
-                keystore: str
+                key_store: str
                 'The keystore name for the key.'
-                cert_alias: str
+                key_alias: str
                 'The label of the key.'
                 include_certificate_data: typing.Optional[bool]
                 'Whether to include the BASE64 encoded certificate data with your signature.'
                 include_public_key: typing.Optional[bool]
                 'Whether to include the public key with the signature.'
                 include_subject_key_identifier: typing.Optional[bool]
                 'Whether to include the X.509 subject key identifier with the signature.'
@@ -471,165 +496,183 @@
                     name: str
                     'The name of the configuration property.'
                     value: typing.List[str]
                     'The values of the configuration property.'
 
                 partner: typing.Optional[typing.List[Item]]
                 'The partner properties for all modules within the STS Chain Template referenced in the STS Chain'
-                _self: typing.Optional[typing.List[Item]]
+                myself: typing.Optional[typing.List[Item]]
                 'The self properties for all modules within the STS Chain Template referenced in the STS Chain '
 
             name: str
             'A friendly name for the STS Chain.'
             description: str
             'A description of the STS Chain.'
             chain_id: str
             'The Id of the STS Chain Template that is referenced by this STS Chain.'
             request_type: str
             'The type of request to associate with this chain. The request is one of the types that are supported by the WS-Trust specification.'
             token_type: typing.Optional[str]
             'The STS module type to map a request message to an STS Chain Template.'
-            x_path: typing.Optional[str]
+            xpath: typing.Optional[str]
             'The custom lookup rule in XML Path Language to map a request message to an STS Chain Template.'
             sign_responses: typing.Optional[bool]
             'Whether to sign the Trust Server SOAP response messages.'
             signature_key: typing.Optional[Key_Identifier]
             'The key to sign the Trust Server SOAP response messages.'
             validate_requests: typing.Optional[bool]
             'Whether requires a signature on the received SOAP request message that contains the RequestSecurityToken message.'
             validation_key: typing.Optional[Key_Identifier]
             'The key to validate the received SOAP request message.'
             send_validation_confirmation: typing.Optional[bool]
-            'Whether to send signature validation confirmation'
+            'Whether to send signature validation confirmation.'
             issuer: typing.Optional[Name_Address]
             'The issuer of the token.'
             applies_to: typing.Optional[Name_Address]
             'The scope of the token.'
             properties: typing.Optional[Properties]
             'The properties for all modules within the STS Chain Template referenced in the STS Chain.'
 
         chain_templates: typing.Optional[typing.List[Chain_Template]]
         'List of STS chain templates to create or update.'
         chains: typing.Optional[typing.List[Chain]]
         'List of STS chains to create or update.'
 
     def _remap_sts_chain_keys(self, chain):
             remap = {"issuer": "issuer_",
-                     "validation": "validation_",
+                     "validation_key": "validation_",
                      "signature": "sign_",
                      "applies_to": "applies_to_"
             }
             if "properties" in chain:
-                chain["self_properties"] = chain['properties'].get("_self", [])
+                chain["self_properties"] = chain['properties'].get("myself", [])
                 chain["partner_properties"] = chain['properties'].get("partner", [])
                 del chain['properties']
+            temp = {}
             for key, new_key_prefix in remap.items():
                 if key in chain and isinstance(chain.get(key), dict):
-                    for old_key, value in chain.get(key).items():
-                        chain[new_key_prefix + old_key] = value
-                    del chain[key]
+                    for old_key, value in chain.pop(key).items():
+                        temp[new_key_prefix + old_key] = value
+            chain.update(temp)
+            remap = {"sign_include_certificate_data": "sign_include_cert",
+                     "sign_include_public_key": "sign_include_pubkey",
+                     "sign_include_subject_key_identifier": "sign_include_ski",
+                     "sign_include_issuer_details": "sign_include_issuer",
+                     "sign_include_subject_name": "sign_include_subject",
+                     "validation_include_certificate_data": "validation_include_cert",
+                     "validation_include_public_key": "validation_include_pubkey",
+                     "validation_include_subject_key_identifier": "validation_include_ski",
+                     "validation_include_issuer_details": "validation_include_issuer",
+                     "validation_include_subject_name": "validation_include_subject"
+                }
+            remap_keys(chain, remap)
+
 
     def configure_sts(self, federation_config):
         if federation_config.sts != None:
             sts = federation_config.sts
             if sts.chain_templates:
-                old_templates = fed.sts.list_templates().json
-                if not old_templates: old_templates = []
+                old_templates = optional_list(fed.sts.list_templates().json)
                 for template in sts.chain_templates:
-                    existing = list(filter(lambda x: x['name'] == template.name, old_templates))
-                    rsp = None
-                    verb = None
+                    existing = optional_list(filter_list('name', template.name, old_templates))[0]
+                    rsp = None; verb = None
                     if existing:
-                        existing = existing[0]
                         rsp = self.fed.sts.update_template(existing['id'], **template)
                         verb = "updated" if rsp.success == True else "update"
                     else:
                         rsp = self.fed.sts.create_template(**template)
                         verb = "created" if rsp.success == True else "create"
                     if rsp.success == True:
-                        _logger.info("Successfully {} {} STS chain template".format(verb, template.name))
+                        _logger.info("Successfully {} {} STS chain template.".format(verb, template.name))
                     else:
                         _logger.error("Failed to {} STS chain template:\n{}\n{}".format(verb, json.dumps(
                                                                                             template, indent=4), rsp.data))
 
             if sts.chains:
-                old_chains = fed.sts.list_chains().json
-                if not old_chains: old_chains = []
+                old_chains = optional_list(fed.sts.list_chains().json)
                 for chain in sts.chains:
-                    existing = list(filter(lambda x: x['name'] == chain.name, old_chains))
+                    existing = optional_list(filter_list('name', chain.name, old_chains))[0]
                     rsp = None
                     verb = None
                     methodArgs = copy.deepcopy(chain)
                     self._remap_sts_chain_keys(methodArgs)
                     if existing:
-                        existing = existing[0]
                         rsp = self.fed.sts.update_chain(existing['id'], **chain)
                         verb = "updated" if rsp.success else "update"
                     else:
                         rsp = self.fed.sts.create_chain(**chain)
                         verb = "created" if rsp.success == True else "create"
                     if rsp.success == True:
                         _logger.info("Successfully {} {} STS chain.".format(verb, chain.name))
                     else:
                         _logger.error("Failed to {} {} STS chain:\n{}\n{}".format(verb, json.dumps(
                                                                                         chain, indent=4), rsp.data))
 
 
         else:
-            _logger.debug("No Security TOken Service configuration found")
+            _logger.debug("No Security Token Service configuration found.")
 
 
     class Access_Policies(typing.TypedDict):
         '''
         Example::
 
-                TO: DO
+                access_policies:
+                - name: "MyNewAccessPolicy"
+                  type: "JavaScript"
+                  policy_file: "path/to/policy.file"
+                  category: "OTP"
 
         '''
 
         name: str
         'A unique name for the access policy. Maximum of 256 bytes.'
-        type: str
+        type: typing.Optional[str]
         'System default type for each access policy. For example, "JavaScript".'
         category: typing.Optional[str]
         'A grouping of related access polices. For example, category "OAUTH" identifies all the rules associated with the OAUTH flow. Maximum 256 bytes. Valid values are: "InfoMap", "AuthSVC", "OAUTH","OTP", "OIDC" and "SAML2_0".'
         policy_file: str
         'The content of the access policy.'
 
     def configure_access_policies(self, federation_config):
         if "access_policies" in federation_config:
-            existing_policies = self.fed.access_policy.get_policies().json
-            if not existing_policies: existing_policies = []
+            existing_policies = optional_list(self.fed.access_policy.list_policies().json)
             for policy in federation_config.access_policies:
-                old_policy = list(filter(lambda x: x['name'] == policy.name), existing_policies)
-                rsp = None
-                verb = None
+                old_policy = optional_list(filter_list('name', policy.name, existing_policies))[0]
+                rsp = None; verb = None
                 methodArgs = copy.deepcopy(policy)
                 policy_file = FILE_LOADER.read_file(policy.policy_file)
                 del methodArgs['policy_file']
                 methodArgs['content'] = policy_file['content']
                 if old_policy:
-                    old_policy = old_policy[0]
-                    rsp = self.fed.access_policy.update_policy(old_policy['id'], **methodArgs)
+                    rsp = self.fed.access_policy.update_policy(policy_id=old_policy['id'], content=methodArgs['content'])
                     verb = "updated" if rsp.success == True else "update"
                 else:
                     rsp = self.fed.access_policy.create_policy(**methodArgs)
                     verb = "created" if rsp.success == True else "create"
                 if rsp.success == True:
-                    _logger.info("Successfully {} {} access policy".format(verb, policy.name))
+                    _logger.info("Successfully {} {} access policy.".format(verb, policy.name))
                 else:
                     _logger.error("Failed to {} access policy:\n{}\n{}".format(verb, json.dumps(
                                                                                         policy, indent=4), rsp.data))
 
 
     class Alias_Service(typing.TypedDict):
         '''
         Example::
 
-                TO: DO
+                alias_service:
+                  ldap_connection: "LocalLDAP"
+                  aliases:
+                  - username: "mary"
+                    federation_id: "https://mysp.com/isam/sps/samlsp/saml20"
+                    type: "partner"
+                    aliases:
+                    - "mary@ibm.com"
+                    - "mary@au.ibm.com"
 
         '''
         class Alias(typing.TypedDict):
             username: str
             'The user to associate aliases with.'
             federation: str
             'The federation this alias is for.'
@@ -640,29 +683,68 @@
             aliases: typing.List[str]
             'An array of aliases to associate with the user.'
 
         db_type: str
         'The alias database type, "JDBC" or "LDAP".'
         ldap_connection: str
         'The LDAP server connection name.'
-        ldap_bind_dn: str
+        ldap_base_dn: str
         'The baseDN to search for the user entry.'
         aliases: typing.Optional[typing.List[Alias]]
         'The SAML aliases to create.'
 
-
     def configure_alias_service(self, federation_config):
-        #TODO
-        return
+        if federation_config.alias_service:
+            methodArgs = copy.deepcopy(federation_config.alias_service)
+            aliases = methodArgs.pop("aliases", [])
+            rsp = self.fed.alias_service.update_alias_settings(**methodArgs)
+            if rsp.success == True:
+                _logger.info("Successfully updated the Federation Alias Service Settings.")
+            else:
+                _logger.error("Failed to update the Federation Alias Service Settings:\n{}\n{}".format(
+                                                                json.dumps(methodArgs, indent=4), rsp.data))
+            if aliases:
+                existing_aliases = optional_list(self.fed.alias_service.list_alias_associations().json)
+                #Map federations and partners to dict by name so we can look up the id if needed
+                existing_federations = {f['name']: f for f in optional_list(self.fed.federations.list_federations())}
+                for _, fed in existing_federations:
+                        fed['partners'] = {p['name']: p for p in optional_list(self.fed.federations.list_partners(fed['id']))}
+                for alias in aliases:
+                    old_alias = optional_list(filter_list('name', alias.name, existing_aliases))[0]
+                    rsp = None; verb = None
+                    #Convert name to id if required
+                    if alias['partner'] != None:
+                        alias['federation_id'] = existing_federations.get(alias.get("federation"), "UNKNOWN") + "|" + \
+                                    existing_federations.get(alias.pop("federation"), {}).get(alias.pop("partner"), "UNKNOWN")
+                    else:
+                        alias["federation_id"] = existing_federations.get(alias.pop("federation"), "UNKNOWN")
+                    if old_alias:
+                        rsp = self.fed.alias_service.update_alias_association(old_alias['id'], **alias)
+                        verb = "Updated" if rsp.success == True else "Update"
+                    else:
+                        rsp = self.fed.alias_service.update_alias_association(**alias)
+                        verb = "Created" if rsp.success == True else "Create"
+                    if rsp.success == True:
+                        _logger.info("Successfully {} {} alias.".format(verb, alias.name))
+                    else:
+                        _logger.error("Failed to {} alias:\n{}\n{}".format(
+                            verb, json.dumps(alias, indent=4), rsp.data))
+
 
     class Attribute_Sources(typing.TypedDict):
         '''
         Example::
 
-                TO: DO
+                attribute_sources:
+                - name: "username"
+                  type: "credential"
+                  value: "PrincipalName"
+                  properties:
+                  - key: "searchFilter"
+                    value: "(&(ObjectClass=inetOrgPerson)(memberOf=dc=ibm,dc=com))"
 
         '''
         class Attribute_Source(typing.TypedDict):
             class Property(typing.TypedDict):
                 key: str
                 'The property key. Valid fields for LDAP include "serverConnection", "scope", "selector", "searchFilter", "baseDN".'
                 value: str
@@ -686,91 +768,232 @@
             'The properties associated with an attribute source.'
 
         attribute_sources: typing.List[Attribute_Source]
         'List of attribute sources to create or update.'
 
     def configure_attribute_sources(self, federation_config):
         if "attribute_sources" in federation_config:
-            existing_sources = self.fed.attribute_sources.list_attribute_sources().json
-            if not existing_sources: existing_sources = []
+            existing_sources = optional_list(self.fed.attribute_sources.list_attribute_sources().json)
             for source in federation_config.attribute_sources:
                 methodArgs = copy.deepcopy(source)
                 for key in ["name", "type", "value"]:
                     if key in methodArgs:  
                         methodArgs["attribute_" + key] = methodArgs.pop(key)
-                old_soruce = list(filter(lambda x: x['name'] == source.name, existing_sources)) 
-                rsp = None
-                verb = None
-                if old_soruce:
-                    old_soruce = old_soruce[0]
+                old_source = optional_list(filter_list('name', source.name, existing_sources))[0]
+                rsp = None; verb = None
+                if old_source:
                     rsp = self.fed.attribute_sources.update_attribute_source(old_source['id'], **methodArgs)
                     verb = "updated" if rsp.success == true else "update"
                 else:
                     rsp = self.fed.attribute_sources.create_attribute_source(**methodArgs)
                     verb = "created" if rsp.success == True else "create"
                 if rsp.success == True:
                     _logger.info("Successfully {} {} attribute source".format(verb, source.name))
                 else:
-                    _logger.error("Failed to {} attribute source:\n{}\n{}".format(verb, json.dumps(source, indent=4), rsp.data))
+                    _logger.error("Failed to {} attribute source:\n{}\n{}".format(
+                                            verb, json.dumps(source, indent=4), rsp.data))
 
 
     def _configure_saml_partner(self, fedId, partner):
         methodArgs = {
                 "name": partner.name,
                 "enabled": partner.enabled,
                 "role": partner.role,
                 "template_name": partner.template_name
             }
         if partner.configuration != None:
             methodArgs.update({
-                "include_federation_id": config.include_federation_id,
+                "access_policy": config.access_policy,
+                "arti_resolution_svc": config.artifact_resolution_services,
+                "assert_consume_svc": config.assertion_consumer_services,
+                "attribute_mappings": config.attribute_mappings,
+                "include_fed_id_in_partner_id": config.include_fed_id_in_alias_partner_id,
                 "logout_request_lifetime": config.logout_request_lifetime,
-                "name_id_format": config.name_id_format,
+                "manage_name_id_services": config.manage_name_id_services,
                 "provider_id": config.provider_id,
-                "artifact_resolution_service": config.artifact_resolution_service,
-                "assertion_consumer_service": config.assertion_consumer_service
+                "session_timeout": config.session_timeout,
+                "slo_svc": config.single_logout_service,
+                "sso_svc": config.single_sign_on_service,
+                "default_target_url": config.default_target_url,
+                "anon_user_name": config.anonymous_user_name,
+                "force_authn_to_federate": config.force_authn_to_federate,
+                "map_unknown_alias": config.map_unknown_aliases
                 })
+            if config.authn_req_mapping != None:
+                methodArgs.update({
+                        "authn_req_delegate_id": config.authn_req_mapping.active_delegate_id,
+                        "authn_req_mr": config.authn_req_mapping.mapping_rule
+                    })
             if config.assertion_settings != None:
                 assert_settings = config.assertion_settings
                 methodArgs.update({
-                        "assertion_attribute_types": assert_settings.attribute_types,
-                        "assertion_session_not_after": assert_settings.session_not_after,
-                        "create_multiple_attribute_statements": assert_settings.create_multiple_attribute_statements
+                        "assert_valid_before": assert_settings.valid_before,
+                        "assert_valid_after": assert_settings.valid_after,
+                        "assert_attribute_types": assert_settings.attribute_types,
+                        "assert_session_not_after": assert_settings.session_not_after,
+                        "assert_multi_attr_stmt": assert_settings.create_multiple_attribute_statements
                     })
             if config.encryption_settings != None:
                 encryption = config.encryption_settings
+                methodArgs.update({
+                        "decrypt_key_store": encryption.decryption_key_identifier.store if encryption.decryption_key_identifier else None,
+                        "decrypt_key_alias": encryption.decryption_key_identifier.label if encryption.decryption_key_identifier else None,
+                        "encrypt_block_alg": encryption.block_algorithm,
+                        "encrypt_transport_alg": encryption.key_transport_algorithm,
+                        "encrypt_key_store": encryption.key_store,
+                        "encrypt_key_alias": encryption.key_alias,
+                        "encrypt_name_id": encryption.encrypt_name_id,
+                        "encrypt_assertion": encryption.encrypt_assertion,
+                        "encrypt_assertion_attrs": encryption.encrypt_assertion_attributes
+                    })
 
+            if config.identity_mapping != None:
+                idMap = config.identity_mapping
+                methodArgs.update({ "identity_delegate_id": idMap.active_delegate_id })
+                if idMap.properties.mapping_rule:
+                    methodArgs.update({
+                            "identity_rule_type": idMap.properties.rule_type if idMap.properties.rule_type else 'JAVASCRIPT',
+                            "identity_mr": idMap.properties.mapping_rule
+                        })
+                else:
+                    methodArgs.update({
+                        "identity_applies_to": idMap.properties.applies_to,
+                        "identity_auth_type": idMap.properties.auth_type,
+                        "identity_ba_user": idMap.properties.basic_auth_username,
+                        "identity_ba_password": idMap.properties.basic_auth_password,
+                        "identity_client_key_store": idMap.properties.client_key_store,
+                        "identity_client_key_alias": idMap.properties.client_key_alias,
+                        "identity_issuer_uri": idMap.properties.issuer_uri,
+                        "identity_mgs_fmt": idMap.properties.message_format,
+                        "identity_ssl_key_store": idMap.properties.ssl_key_store,
+                        "identity_uri": idMap.properties.uri
+                    })
+            if config.extension_mapping != None:
+                methodArgs.update({
+                        "ext_delegate_id": config.extension_mapping.active_delegate_id,
+                        "ext_mr": config.extension_mapping.mapping_rule
+                    })
+
+            if config.name_id_format != None:
+                methodArgs.update({
+                        "name_id_default": config.name_id_format.default,
+                        "name_id_supported": config.name_id_format.supported
+                    })
+            if config.signature_settings != None:
+                sigSetting = config.signature_settings
+                methodArgs.update({
+                        "sign_alg": sigSetting.signing_algorithm,
+                        "sign_digest_alg": sigSetting.digest_algorithm,
+                    })
+                if sigSetting.key_info_elements != None:
+                    methodArgs.update({
+                            "sign_include_pub_key": sigSetting.key_info_elements.include_public_key,
+                            "sign_include_cert": sign_include_pub_key.include_x509_certificate_data,
+                            "sign_include_issuer": sign_include_pub_key.include_x509_issuer_details,
+                            "sign_include_ski": sign_include_pub_key.include_x509_subject_key_identifier,
+                            "sign_include_subject": sign_include_pub_key.include_x509_subject_name
+                        })
+                if sigSetting.signing_key_identifier != None:
+                    methodArgs.update({
+                            "sign_key_store": sigSetting.signing_key_identifier.store,
+                            "sign_key_alias": sigSetting.signing_key_identifier.label
+                        })
+                if sigSetting.validation_key_identifier != None:
+                    methodArgs.update({
+                            "validation_key_store": sigSetting.validation_key_identifier.store,
+                            "validation_key_alias": sigSetting.validation_key_identifier.label
+                        })
+                if sigSetting.signing_options != None:
+                    methodArgs.update({
+                            "sign_arti_request": sigSetting.signing_options.sign_artifact_request,
+                            "sign_arti_rsp": sigSetting.signing_options.sign_artifact_response,
+                            "sign_assertion": sigSetting.signing_options.sign_assertion,
+                            "sign_authn_rsp": sigSetting.signing_options.sign_authn_response,
+                            "sign_logout_req": sigSetting.signing_options.sign_logout_request,
+                            "sign_logout_rsp": sigSetting.signing_options.sign_logout_response,
+                            "sign_name_id_req": sigSetting.signing_options.sign_name_id_management_request,
+                            "sign_name_id_rsp": sigSetting.signing_options.sign_name_id_management_response,
+                            "transform_include_namespace": sigSetting.signing_options.transform_include_namespace
+                        })
+                if sigSetting.validation_options != None:
+                    methodArgs.update({
+                            "validate_assertion": sigSetting.validation_options.validate_assertion,
+                            "validate_authn_req": sigSetting.validation_options.validate_authn_request,
+                            "validate_arti_req": sigSetting.validation_options.validate_artifact_request,
+                            "validate_arti_rsp": sigSetting.validation_options.validate_artifact_response,
+                            "validate_logout_req": sigSetting.validation_options.validate_logout_request,
+                            "validate_logout_rsp": sigSetting.validation_options.validate_logout_response,
+                            "validate_name_id_req": sigSetting.validation_options.validate_name_id_management_request,
+                            "validate_name_id_rsp": sigSetting.validation_options.validate_name_id_management_response
+                        })
+                if config.soap_settings != None and isinstance(config.soap_settings.server_cert_validation, dict):
+                    methodArgs.update({
+                            "soap_key_store": config.soap_settings.server_cert_validation.store,
+                            "soap_key_alias":  config.soap_settings.server_cert_validation.label,
+                            
+                        })
+                if config.soap_settings != None and isinstance(config.soap_settings.client_auth_data, dict):
+                    methodArgs.update({
+                            "soap_client_auth_method": config.soap_settings.client_auth_data.method,
+                            "soap_client_auth_ba_user": config.soap_settings.client_auth_data.basic_auth_username,
+                            "soap_client_auth_ba_password": config.soap_settings.client_auth_data.basic_auth_password,
+                            "soap_client_auth_key_store": config.soap_settings.client_auth_data.client_key_store,
+                            "soap_client_auth_key_alias": config.soap_settings.client_auth_data.client_key_alias
+                        })
         rsp = self.fed.federations.create_saml_partner(fedId, **methodArgs)
         if rsp.success == True:
-            _logger.info("Successfully created {} SAML {} Partner".format(
+            _logger.info("Successfully created {} {} SAML Partner".format(
                 partner.name, partner.role))
         else:
             _logger.error("Failed to create {} SAML Partner with config:\n{}\n{}".format(
-                partner.name, json.dumps(partner, indent=4), rsp.data))
+                                        partner.name, json.dumps(partner, indent=4), rsp.data))
 
     def _configure_oidc_partner(self, fedId, partner):
         methodArgs = {
                 "name": partner.name,
-                "enabled": partner.enabled
+                "enabled": partner.enabled,
+                "template_name": partner.template_name
             }
         if partner.configuration != None:
             config = partner.configuration
             methodArgs.update({
-                    "client_id": config.client_id,
-                    "client_secret": config.client_secret,
-                    "metadata_endpoint": config.metadata_endpoint,
-                    "scope": config.scope,
-                    "token_endpoint_auth_method": config.token_endpoint_auth_method,
-                    "perform_userinfo": config.perform_userinfo,
-                    "signing_algorithm": config.signature_algorithm
+                    "redirect_uri_prefix": config.redirect_uri_prefix,
+                    "response_type": config.response_types,
+                    "attribute_mapping": config.attribute_mapping
                 })
+            if config.basic_configuration:
+                methodArgs.update({
+                        "active_delegate_id": config.basic_configuration.active_delegate_id,
+                        "metadata_endpoint_url": config.basic_configuration.metadata_endpoint_url,
+                        "issuer_identifier": config.basic_configuration.issuer_identifier,
+                        "response_types": config.basic_configuration.response_types,
+                        "authorization_endpoint": config.basic_configuration.authorization_endpoint_url,
+                        "token_endpoint": config.basic_configuration.token_endpoint_url,
+                        "user_info_endpoint": config.basic_configuration.user_info_endpoint_url
+                    })
+            if config.identity_mapping and config.identity_mapping.properties:
+                methodArgs.update({
+                        "identity_delegate_id": config.identity.active_delegate_id,
+                        "identity_mapping_rule": config.identity.properties.mapping_rule,
+                        "identity_auth_type": config.identity_mapping.properties.auth_type,
+                        "identity_ba_user": config.identity_mapping.properties.basic_auth_username,
+                        "identity_ba_password": config.identity_mapping.properties.basic_auth_password,
+                        "identity_client_keystore": config.identity_mapping.properties.client_key_store,
+                        "identity_client_key_alias": config.identity_mapping.properties.client_key_alias,
+                        "identity_issuer_uri": config.identity_mapping.properties.issuer_uri,
+                        "identity_msg_fmt": config.identity_mapping.properties.message_format,
+                        "identity_ssl_keystore": config.identity_mapping.properties.ssl_keystore,
+                        "identity_uri": config.identity_mapping.properties.uri
+                    })                    
+
             if config.advanced_configuration != None:
                 methodArgs.update({
                         "advanced_configuration_active_delegate": config.advanced_configuration.active_delegate_id,
-                        "advanced_configuration_rule_id": config.advanced_configuration.mapping_rule
+                        "advanced_configuration_rule_id": config.advanced_configuration.mapping_rule,
+                        "advanced_configuration_rule_type": config.advanced_configuration.rule_type if config.advanced_configuration.rule_type else "JAVASCRIPT"
                     })
 
         rsp = self.fed.federations.create_oidc_rp_partner(fedId, **methodArgs)
         if rsp.success == True:
             _logger.info("Successfully created {} OIDC RP Partner for Federation {}".format(
                 partner.name, fedId))
         else:
@@ -798,94 +1021,186 @@
                     "name": federation.name,
                     "role": federation.role,
                     "template_name": federation.template_name,
                 }
         if federation.configuration != None:
             config = federation.configuration
             methodArgs.update({
+                    "access_policy": config.access_policy,
                     "artifact_lifetime": config.artifact_lifetime,
+                    "artifact_resolution_service": config.artifact_resolution_services,
+                    "attribute_mapping": config.attribute_mappings,
                     "company_name": config.company_name,
-                    "message_valid_time": config.message_valid_time,
-                    "message_issuer_format": config.message_issuer_format,
-                    "message_issuer_name_qualifier": config.message_issuer_name_qualifier,
-                    "point_of_contact_url": config.point_of_contact_url,
+                    "manage_name_id_services": config.manage_name_id_services,
+                    "msg_valid_time": config.message_valid_time,
+                    "msg_issuer_fmt": config.message_issuer_format,
+                    "msg_issuer_name_qualifier": config.message_issuer_name_qualifier,
+                    "consent_to_federate": config.need_consent_to_federate,
+                    "exclude_session_index_logout_request": config.exclude_session_index_in_single_logout_request,
+                    "poc_url": config.point_of_contact_url,
+                    "provider_id": config.provider_id,
                     "session_timeout": config.session_timeout,
-                    "assertion_consumer_service": config.assertion_consumer_service,
-                    "name_id_format": config.name_id_format
+                    "sso_svc_data": config.single_sign_on_service,
+                    "slo_svc_data": config.single_logout_service,
+                    "assertion_consume_svc": config.assertion_consumer_services
                 })
-            if config.identity_mapping != None:
+
+            if config.name_id_format != None:
                 methodArgs.update({
-                        "identity_mapping_delegate_id": config.identity_mapping.active_delegate_id,
-                        "identity_mapping_rule_reference": config.identity_mapping.mapping_rule
+                        "name_id_default": config.name_id_format.default,
+                        "name_id_supported": config.name_id_format.supported
+                    })
+
+            if config.encryption_settings != None:
+                methodArgs.update({
+                        "encrypt_block_alg": config.encryption_settings.block_algorithm,
+                        "encrypt_key_transport_alg": config.encryption_settings.key_transport_algorithm,
+                        "encrypt_key_alias": config.encryption_settings.key_alias,
+                        "encrypt_key_store": config.encryption_settings.key_store,
+                        "encrypt_name_id": config.encryption_settings.encrypt_name_id,
+                        "encrypt_assertions": config.encryption_settings.encrypt_assertions,
+                        "encrypt_assertion_attrs": config.encryption_settings.encrypt_assertion_attributes,
+                        "decrypt_key_alias": config.encryption_settings.decryption_key_identifier.label if encryption.decryption_key_identifier else None,
+                        "decrypt_key_store": config.encryption_settings.decryption_key_identifier.store if encryption.decryption_key_identifier else None
+                    })
+
+            if config.assert_settings != None:
+                methodArgs.update({
+                        "assertion_attr_types": config.assert_settings.attribute_types,
+                        "assertion_session_not_on_or_after": config.assert_settings.session_not_on_or_after,
+                        "assertion_multi_attr_stmt": config.assert_settings.create_multiple_attribute_statements,
+                        "assertion_valid_before": config.assert_settings.assertion_valid_before,
+                        "assertion_valid_after": config.assert_settings.assertion_valid_after
+                    })
+            if config.identity_mapping != None and config.identity_mapping.properties != None:
+                methodArgs.update({
+                        "identity_delegate_id": config.identity_mapping.active_delegate_id,
+                        "identity_rule_id": config.identity_mapping.properties.mapping_rule,
+                        "identity_rule_type": config.identity_mapping.properties.rule_type if config.identity_mapping.properties.rule_type else 'JAVASCRIPT',
+                        "identity_applies_to": config.identity_mapping.properties.applies_to,
+                        "identity_auth_type": config.identity_mapping.properties.auth_type,
+                        "identity_ba_user": config.identity_mapping.properties.basic_auth_username,
+                        "identity_ba_password": config.identity_mapping.properties.basic_auth_password,
+                        "identity_client_keystore": config.identity_mapping.properties.client_key_store,
+                        "identity_client_key_alias": config.identity_mapping.properties.client_key_alias,
+                        "identity_issuer_uri": config.identity_mapping.properties.issuer_uri,
+                        "identity_msg_fmt": config.identity_mapping.properties.message_format,
+                        "identity_ssl_keystore": config.identity_mapping.properties.ssl_key_store,
+                        "identity_uri": config.identity_mapping.properties.uri
                     })
             if config.extension_mapping != None:
                 methodArgs.update({
-                        "extension_mapping_delegate_id": config.extension_mapping.active_delegate_id,
-                        "extension_mapping_rule_reference": config.extension_mapping.mapping_rule
+                        "ext_delegate_id": config.extension_mapping.active_delegate_id,
+                        "ext_mapping_rule": config.extension_mapping.mapping_rule
                     })
             if config.signature_settings != None:
                 sigSetting = config.signature_settings
                 methodArgs.update({
-                        "include_inclusive_namespaces": sigSetting.include_inclusive_namespaces,
+                        "sign_alg": sigSetting.signature_algorithm,
+                        "sign_digest_alg": sigSetting.digest_algorithm,
+                        "transform_include_namespace": sigSetting.include_inclusive_namespaces,
                         "validate_assertion": sigSetting.validate_assertion
                     })
                 if sigSettings.key_info_elements != None:
                     methodArgs.update({
-                            "include_x509_certificate_data": sigSettings.key_info_elements.include_x509_certificate_data,
-                            "include_x509_subject_name": sigSettings.key_info_elements.include_x509_subject_name,
-                            "include_x509_subject_key_identifier": sigSettings.key_info_elements.include_x509_subject_key_identifier,
-                            "include_x509_issuer_details": sigSettings.key_info_elements.include_x509_issuer_details,
-                            "include_public_key": sigSettings.key_info_elements.include_public_key
+                            "sign_include_cert": sigSettings.key_info_elements.include_x509_certificate_data,
+                            "sign_include_subject": sigSettings.key_info_elements.include_x509_subject_name,
+                            "sign_include_ski": sigSettings.key_info_elements.include_x509_subject_key_identifier,
+                            "sign_include_issuer": sigSettings.key_info_elements.include_x509_issuer_details,
+                            "sign_include_pubkey": sigSettings.key_info_elements.include_public_key
                         })
                 if sigSettings.signing_key_identifier != None:
                     methodArgs.update({
                             "signing_keystore": sigSettings.signing_key_identifier.keystore,
-                            "signing_cert": sigSettings.signing_key_identifier.certificate
+                            "sign_key_alias": sigSettings.signing_key_identifier.certificate
+                        })
+                if sigSetting.validation_key_identifier != None:
+                    methodArgs.update({
+                            "sign_valid_key_store": sigSettings.validation_key_identifier.keystore,
+                            "sign_valid_key_alias": sigSettings.validation_key_identifier.certificate
                         })
                 if sigSettings.signing_options != None:
                     methodArgs.update({
-                            "sign_authn_request": sigSettings.signing_options.sign_authn_request,
-                            "sign_artifact_request": sigSettings.signing_options.sign_artifact_request,
-                            "sign_artifact_response": sigSettings.signing_options.sign_artifact_response
+                            "sign_assertion": sigSettings.signing_options.sign_assertion,
+                            "sign_auth_rsp": sigSettings.signing_options.sign_authn_response,
+                            "sign_arti_req": sigSettings.signing_options.sign_artifact_request,
+                            "sign_arti_rsp": sigSettings.signing_options.sign_artifact_response,
+                            "sign_logout_req": sigSettings.signing_options.sign_logout_request,
+                            "sign_logout_rsp": sigSettings.signing_options.sign_logout_response,
+                            "sign_name_id_req": sigSettings.signing_options.sign_name_id_management_request,
+                            "sign_name_id_rsp": sigSettings.signing_options.sign_name_id_management_response
                         })
+                if sigSettings.validation_options != None:
+                    methodArgs.update({
+                            "validate_auth_req": sigSettings.validation_options.validate_authn_request,
+                            "validate_assert": sigSettings.validation_options.validate_assertion,
+                            "validate_arti_req": sigSettings.validation_options.validate_artifact_request,
+                            "validate_arti_rsp": sigSettings.validation_options.validate_artifact_response,
+                            "validate_logout_req": sigSettings.validation_options.validate_logout_request,
+                            "validate_logout_rsp": sigSettings.validation_options.validate_logout_response,
+                            "validate_name_id_req": sigSettings.validation_options.validate_name_id_management_request,
+                            "validate_name_id_rsp": sigSettings.validation_options.validate_name_id_management_response
+                        })
+            if config.alias_service_settings != None:
+                methodArgs.update({
+                        "alias_svc_db_type": config.alias_service_settings.db_type,
+                        "alias_svc_ldap_con": config.alias_service_settings.ldap_connection,
+                        "alias_svc_ldap_base_dn": config.alias_service_settings.ldap_base_dn
+                    })
+            
+            if config.authn_req_mapping != None:
+                methodArgs.update({
+                        "authn_req_delegate_id": config.authn_req_mapping.active_delegate_id,
+                        "authn_req_mr": config.authn_req_mapping.mapping_rule
+                    })
             
         rsp = self.fed.federations.create_saml_federation(**methodArgs)
         if rsp.success == True:
             _logger.info("Successfully created {} SAML2.0 Federation".format(federation.name))
         else:
             _logger.error("Failed to create {} SAML2.0 Federation with config:\n{}\n{}".format(
                 federation.name, json.dumps(federation, indent=4), rsp.data))
             return
         if federation.partners != None:
             for partner in federation.partners:
-                _create_partner(federation, partner)
+                self._create_partner(federation, partner)
 
 
     def _configure_oidc_federation(self, federation):
         methodArgs = {
                 "name": federation.name,
                 "role": federation.role,
                 "template": federation.template
             }
         if federation.configuration != None:
             config = federation.configuration
             methodArgs.update({
                     "redirect_uri_prefix": config.redirect_uri_prefix,
                     "response_type": config.response_types,
-                    "attribute_mapping": config.attribute_mapping
+                    "attribute_mapping": config.attribute_mappings
                 })
-            if config.identity_mapping != None:
+            if config.identity_mapping != None and config.identity_mapping.properties != None:
                 methodArgs.update({
                         "identity_mapping_delegate_id": config.identity_mapping.active_delegate_id,
-                        "identity_mapping_rule": config.identity_mapping.rule
+                        "identity_mapping_rule": config.identity_mapping.properties.mapping_rule,
+                        "identity_auth_type": config.identity_mapping.properties.auth_type,
+                        "identity_ba_user": config.identity_mapping.properties.basic_auth_username,
+                        "identity_ba_password": config.identity_mapping.properties.basic_auth_password,
+                        "identity_client_keystore": config.identity_mapping.properties.client_key_store,
+                        "identity_client_key_alias": config.identity_mapping.properties.client_key_alias,
+                        "identity_issuer_uri": config.identity_mapping.properties.issuer_uri,
+                        "identity_message_format": config.identity_mapping.properties.message_format,
+                        "identity_ssl_keystore": config.identity_mapping.properties.ssl_key_store,
+                        "identity_uri": config.identity_mapping.properties.uri
                     })
             if config.advance_configuration != None:
                 methodArgs.update({
-                        "advance_configuration_delegate_id": config.advance_configuration.active_delegate_id,
-                        "advanced_configuration_mapping_rule": config.advance_configuration.rule
+                        "adv_delegate_id": config.advance_configuration.active_delegate_id,
+                        "adv_mapping_rule": config.advance_configuration.mapping_rule,
+                        "adv_rule_type": config.advance_configuration.rule_type if config.advance_configuration.rule_type != None else "JAVASCRIPT"
                     })
         rsp = self.fed.federations.create_oidc_rp_federation(**methodArgs)
         if rsp.success == True:
             _logger.info("Successfully created {} OIDC RP Federation".format(federation.name))
         else:
             _logger.error("Failed to create {} OIDC RP Federation with config:\n{}\n{}".format(
                     federation.name, json.dumps(federation, indent=4), rsp.data))
@@ -907,17 +1222,17 @@
 
                 access_policy: typing.Optional[str]
                 'The access policy that should be applied during single sign-on.'
                 artifact_lifetime: typing.Optional[int]
                 'The number of seconds that an artifact is valid. The default value is 120. This setting is enabled only when HTTP artifact binding has been enabled.'
                 assertion_settings: typing.Optional[Federation_Common.Assertion_Settings]
                 'The assertion settings.'
-                artifact_resolution_service: typing.Optional[typing.List[Federation_Common.Artifact_Resolution_Service]]
+                artifact_resolution_services: typing.Optional[typing.List[Federation_Common.Artifact_Resolution_Service]]
                 'Endpoints where artifacts are exchanged for actual SAML messages. Required if artifact binding is enabled.'
-                attribute_mapping: typing.Optional[Federation_Common.Attribute_Mapping]
+                attribute_mappings: typing.Optional[Federation_Common.Attribute_Mapping]
                 'The attribute mapping data.'
                 company_name: str
                 'The name of the company that creates the identity provider or service provider.'
                 encryption_settings: typing.Optional[Federation_Common.Encryption_Settings]
                 'The encryption and decryption configurations for SAML messages.'
                 identity_mapping: Federation_Common.Identity_Mapping
                 'The identity mapping data.'
@@ -952,31 +1267,31 @@
                 alias_service_settings: typing.Optional[Federation_Common.Alias_Service_Settings]
                 'The alias service settings to store the user alias.'
 
             class SAML20_Service_Provider(typing.TypedDict):
 
                 artifact_lifetime: typing.Optional[int]
                 'The number of seconds that an artifact is valid. The default value is 120. This setting is enabled only when HTTP artifact binding has been enabled.'
-                assertion_consumer_service: typing.List[Federation_Common.Assertion_Consumer_Service]
+                assertion_consumer_services: typing.List[Federation_Common.Assertion_Consumer_Service]
                 'Endpoints at a Service Provider that receive SAML assertions.'
-                artifact_resolution_service: typing.List[Federation_Common.Artifact_Resolution_Service]
+                artifact_resolution_services: typing.List[Federation_Common.Artifact_Resolution_Service]
                 'Endpoints where artifacts are exchanged for actual SAML messages. Required if artifact binding is enabled.'
-                attribute_mapping: typing.Optional[Federation_Common.Attribute_Mapping]
+                attribute_mappings: typing.Optional[Federation_Common.Attribute_Mapping]
                 'The attribute mapping data.'
                 company_name: str
                 'The name of the company that creates the identity provider or service provider.'
                 encryption_settings: typing.Optional[Federation_Common.Encryption_Settings]
                 'The encryption and decryption configurations for SAML messages.'
                 identity_mapping: Federation_Common.Identity_Mapping
                 'The identity mapping data.'
                 extension_mapping: Federation_Common.Extension_Mapping
                 'The extension mapping data.'
                 authn_req_mapping: Federation_Common.Authn_Req_Mapping
                 'The authentication request mapping data.'
-                manage_name_id_service: typing.Optional[typing.List[Federation_Common.Service_Data]]
+                manage_name_id_services: typing.Optional[typing.List[Federation_Common.Service_Data]]
                 'Endpoints that accept SAML name ID management requests or responses.'
                 message_valid_time: typing.Optional[int]
                 'The number of seconds that a message is valid. The default value is 300.'
                 message_issuer_format: typing.Optional[str]
                 'The format of the issuer of SAML message. The default value is "urn:oasis:names:tc:SAML:2.0:nameid-format:entity".'
                 message_issuer_name_qualifier: typing.Optional[str]
                 'The name qualifier of the issuer of SAML messaged.'
@@ -995,33 +1310,33 @@
                 alias_service_settings: typing.Optional[Federation_Common.Alias_Service_Settings]
                 'The alias service settings to store the user alias.'
 
             class SAML20_Identity_Provider_Partner(typing.TypedDict):
 
                 access_policy: typing.Optional[str]
                 'The access policy that should be applied during single sign-on.'
-                artifact_resolution_service: typing.Optional[Federation_Common.Artifact_Resolution_Service]
+                artifact_resolution_services: typing.Optional[Federation_Common.Artifact_Resolution_Service]
                 'Partner\'s endpoints where artifacts are exchanged for actual SAML messages. Required if artifact binding is enabled.'
-                assertion_consumer_service: Federation_Common.Assertion_Consumer_Service
+                assertion_consumer_services: typing.List[Federation_Common.Assertion_Consumer_Service]
                 'Partner\'s endpoints that receive SAML assertions.'
                 assertion_settings: Federation_Common.Assertion_Settings
                 'The assertion settings.'
-                attribute_mapping: typing.Optional[Federation_Common.Attribute_Mapping]
+                attribute_mappings: typing.Optional[Federation_Common.Attribute_Mapping]
                 'The attribute mapping data.'
                 encryption_settings: typing.Optional[Federation_Common.Encryption_Settings]
                 'The encryption and decryption configurations for SAML messages.'
                 identity_mapping: typing.Optional[Federation_Common.Identity_Mapping]
                 'The identity mapping data.'
                 extension_mapping: Federation_Common.Extension_Mapping
                 'The extension mapping data.'
                 include_fed_id_in_alias_partner_id: typing.Optional[bool]
                 'A setting that specifies whether to append federation ID to partner ID when mapping user aliases. The default value is false.'
                 logout_request_lifetime: typing.Optional[int]
                 'A setting that specifies Logout request lifetime in number of seconds. If not provided, the default value is 120.'
-                manage_name_id_service: typing.Optional[typing.List[Federation_Common.Service_Data]]
+                manage_name_id_services: typing.Optional[typing.List[Federation_Common.Service_Data]]
                 'Partner\'s endpoints that accept SAML name ID management requests or responses.'
                 name_id_format: typing.Optional[Federation_Common.Name_Id_Format]
                 'The name identifier format configurations.'
                 provider_id: str
                 'A unique identifier that identifies the partner.'
                 signature_settings: typing.Optional[Federation_Common.Signature_Settings]
                 'The signing and validation configurations for SAML messages and assertions.'
@@ -1029,41 +1344,41 @@
                 'Partner\'s endpoints that accept SAML logout requests or responses.'
                 soap_settings: typing.Optional[Federation_Common.SOAP_Settings]
                 'A setting that specifies the connection parameters for the SOAP endpoints.'
 
             class SAML20_Service_Provider_Partner(typing.TypedDict):
                 anonymous_user_name: typing.Optional[str]
                 'This is a one-time name identifier that allows a user to access a service through an anonymous identity. The user name entered here is one that the service provider will recognize as a one-time name identifier for a legitimate user in the local user registry.'
-                artifact_resolution_service: typing.Optional[Federation_Common.Artifact_Resolution_Service]
+                artifact_resolution_services: typing.Optional[Federation_Common.Artifact_Resolution_Service]
                 'Partner\'s endpoints where artifacts are exchanged for actual SAML messages. Required if artifact binding is enabled.'
                 assertion_settings: typing.Optional[Federation_Common.Assertion_Settings]
                 'The assertion settings.'
-                attribute_mapping: typing.Optional[Federation_Common.Attribute_Mapping]
+                attribute_mappings: typing.Optional[Federation_Common.Attribute_Mapping]
                 'The attribute mapping data.'
                 encryption_settings: typing.Optional[Federation_Common.Encryption_Settings]
                 'The encryption and decryption configurations for SAML messages.'
                 force_authn_to_federate: typing.Optional[bool]
                 'A setting that specifies whether to force user to authenticate before linking the account.'
                 identity_mapping: typing.Optional[Federation_Common.Identity_Mapping]
                 'The identity mapping data.'
                 extension_mapping: typing.Optional[Federation_Common.Extension_Mapping]
                 'The extension mapping data.'
                 authn_req_mapping: Federation_Common.Authn_Req_Mapping
                 'The authentication request mapping data.'
                 include_fed_id_in_alias_partner_id: typing.Optional[bool]
                 'A setting that specifies whether to append federation ID to partner ID when mapping user aliases.'
-                manage_name_id_service: typing.Optional[typing.List[Federation_Common.Service_Data]]
+                manage_name_id_services: typing.Optional[typing.List[Federation_Common.Service_Data]]
                 'Partner\'s endpoints that accept SAML name ID management requests or responses.'
                 map_unknown_aliases: typing.Optional[bool]
                 'A setting that specifies whether to map non-linked persistent name ID to one-time username.'
                 name_id_format: typing.Optional[Federation_Common.Name_Id_Format]
                 'The name identifier format configurations.'
                 provider_id: str
                 'A unique identifier that identifies the partner.'
-                Signature_Settings: typing.Optional[Federation_Common.Signature_Settings]
+                signature_settings: typing.Optional[Federation_Common.Signature_Settings]
                 'The signing and validation configurations for SAML messages and assertions.'
                 single_logout_service: typing.Optional[typing.List[Federation_Common.Service_Data]]
                 'Partner\'s endpoints that accept SAML logout requests or responses.'
                 single_sign_on_service: typing.Optional[typing.List[Federation_Common.Single_Sign_On_Service]]
                 'Partner\'s endpoints that accept SAML authentication requests.'
                 soap_settings: typing.Optional[Federation_Common.SOAP_Settings]
                 'A setting that specifies the connection parameters for the SOAP endpoints.'
@@ -1072,15 +1387,15 @@
 
             class OIDC_Relying_Party(typing.TypedDict):
 
                 redirect_uri_prefix: str
                 'The reverse proxy address to prepend to the redirect URI sent to the provider to communicate with this instance. An example is "https://www.reverse.proxy.com/mga". For the value "https://www.reverse.proxy.com/mga", the kickoff uri would be: "https://www.reverse.proxy.com/mga/sps/oidc/rp/<FEDERATION_NAME>/kickoff/<PARTNER_NAME>" and the redirect uri: "https://www.reverse.proxy.com/mga/sps/oidc/rp/<FEDERATION_NAME>/redirect/<PARTNER_NAME>"'
                 response_types: typing.List[str]
                 'List of response types which determine the flow to be executed. Valid values to be included are "code", "token", "id_token". This selects the default flow to run when a metadata URL is specified in the partner configuration.'
-                attribute_mapping: typing.Optional[Federation_Common.Attribute_Mapping]
+                attribute_mappings: typing.Optional[Federation_Common.Attribute_Mapping]
                 'The attribute mapping data.'
                 identity_mapping: Federation_Common.Identity_Mapping
                 'The identity mapping data.'
                 advanced_configuration: Federation_Common.Advanced_Configuration
                 'The advanced configuration data.'
 
             class OIDC_Relying_Party_Partner(typing.TypedDict):
@@ -1093,31 +1408,31 @@
                 'The basic configuration data.'
                 signature_algorithm: typing.Optional[str]
                 'The signing algorithm to use. Supported values are "none", "HS256", "HS384", "HS512", "RS256", "RS384", "RS512", "ES256", "ES384", "ES512", "PS256", "PS384", "PS512".'
                 verification_keystore: typing.Optional[str]
                 'When signature algorithm requires a certificate, the keystore which contains the selected certificate to perform the signing.'
                 verification_key_label: typing.Optional[str]
                 'When signature algorithm requires a certificate, the alias of the public key in the selected keystore to use in signature verification.'
-                jwsk_endpoint_url: typing.Optional[str]
+                jwks_endpoint_url: typing.Optional[str]
                 'When signature algorithm requires a certificate, the JWK endpoint of the provider. If a metadata endpoint is specified in BasicConfigurationData, the JWK URL will be read from metadata information. Cannot be specified if using a signingKeyLabel.'
                 key_management_algorithm: typing.Optional[str]
                 'The key management algorithm to use. Supported values are "none", "dir", "A128KW", "A192KW", "A256KW", "A128GCMKW", "A192GCMKW", "A256GCMKW", "ECDH-ES", "ECDH-ES+A128KW", "ECDH-ES+A192KW", "ECDH-ES+A256KW", "RSA1_5", "RSA-OAEP", "RSA-OAEP-256".'
                 content_encryption_algorithm: typing.Optional[str]
                 'The content encryption algorithm to use. Supported values are "none", "A128CBC-HS256", "A192CBC-HS384", "A256CBC-HS512", "A128GCM", "A192GCM", "A256GCM".'
                 decryption_keystore: typing.Optional[str]
                 'When key management algorithm requires a certificate, the keystore which contains the selected certificate to perform JWT decryption.'
                 decryption_key_label: typing.Optional[str]
                 'When key management algorithm requires a certificate, the alias of the private key in the selected keystore to perform JWT decryption.'
                 scope: typing.Optional[typing.List[str]]
                 'An array of strings that identify the scopes to request from the provider. Defaults to ["openid"].'
-                perform_user_infO: typing.Optional[bool]
+                perform_user_info: typing.Optional[bool]
                 'A setting that specifies whether to perform user info request automatically whenever possible.'
                 token_endpoint_auth_method: str
                 'The token endpoint authentication method. Valid values are "client_secret_basic" and "client_secret_post".'
-                attribute_mapping: typing.Optional[Federation_Common.Attribute_Mapping]
+                attribute_mappings: typing.Optional[Federation_Common.Attribute_Mapping]
                 'The attribute mapping data.'
                 identity_mapping: typing.Optional[Federation_Common.Identity_Mapping]
                 'The identity mapping data.'
                 advance_configuration: typing.Optional[Federation_Common.Advanced_Configuration]
                 'The advance configuration data. '
 
             class WSFed_Identity_Provider(typing.TypedDict):
@@ -1258,10 +1573,9 @@
             return
         self.configure_poc(self.config.federation)
         self.configure_sts(self.config.federation)
         self.configure_access_policies(self.config.federation)
         self.configure_alias_service(self.config.federation)
         self.configure_attribute_sources(self.config.federation)
         self.configure_federations(self.config.federation)
-
-if __name__ == "__main__":
-    configure()
+        if self.needsRestart == True:
+            deploy_pending_changes(self.factory, self.config)
```

### Comparing `verify_access_autoconf-0.1.0/src/verify_access_autoconf/util/configure_util.py` & `verify_access_autoconf-0.3.0/src/verify_access_autoconf/util/configure_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/bin/python
 """
 @copyright: IBM
 """
 import os, kubernetes, logging, sys, yaml, pyisva, datetime, subprocess, shutil, time, json
 from . import constants as const
-from .data_util import Map, FileLoader, CustomLoader, KUBE_CLIENT
+from .data_util import Map, FileLoader, CustomLoader, KUBE_CLIENT, KUBE_CLIENT_SLEEP
 from kubernetes.stream import stream
 
 logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
 _logger = logging.getLogger(__name__)
 
 def config_base_dir():
     if const.CONFIG_BASE_DIR in os.environ.keys():
@@ -119,15 +119,15 @@
         } }
     try:
         client.AppsV1Api().patch_namespaced_deployment(deployment, namespace, body, pretty='true')
     except kubernetes.client.rest.ApiException as e:
         _logger.error("Exception when calling AppsV1Api->patch_namespaced_deployment: %s" % e)
         sys.exit(1)
 
-    #Now request for the pods to be deleted; when this thows the pods are gone
+    #Now request for the pods to be deleted; when this throws the pods are gone
     for pod in pods:
         count = 1
         while count < 10:
             try:
                 client.CoreV1Api().delete_namespaced_pod(name=pod, namespace=namespace)
             except kubernetes.client.rest.ApiException as e:
                 if json.loads(e.body).get('code', -1) == 404:
@@ -135,57 +135,53 @@
             time.sleep(count * 10)
             count += 1
         if count == 10:
             _logger.error("Failed to delete pod {} for deployment {}".format(pod, deployment))
             sys.exit(1)
 
     #Finally wait for the new pod list to be ready
-    #count = 1
-    #while count < 10:
-    #    try:
-    #        rsp = client.AppsV1Api().read_namespaced_deployment_status(name=deployment, namespace=namespace)
-    #        if rsp.spec and rsp.status and rsp.spec.replicas == rsp.status.available_replicas:
-    #            _logger.debug("Deployment {} is reported as available again".format(deployment))
-    #            break
-    #        else:
-    #            _logger.debug("Waiting for deployment {}; status {}".format(deployment, rsp.status))
-    #            time.sleep(count * 10)
-    #            count += 1
-    #    except kubernetes.client.rest.ApiException as e:
-    #        _logger.error("Exception when calling AppsV1Api -> read_namespaced_deployment_status: %s" % e)
-    #        sys.exit(1)
-    #if count == 10:
-    #    _logger.error("Failed to wait for deployment to be ready.")
-    #    sys.exit(1)
-    return
+    watcher = kubernetes.watch.Watch()
+    for event in watcher.stream(func=client.CoreV1Api().list_namespaced_pod,
+                                namespace=namespace,
+                                label_selector="app=" + deployment,
+                                timeout_seconds=30):
+        if event['object'].status.phase == "Running":
+            watcher.stop()
+            _logger.info("{} deployment is running".format(deployment))
+            return
+        elif event['type'] == "DELETED":
+            watcher.stop()
+            _logger.error("{} deployment was deleted while waiting to be restarted".format(deployment))
+    sys.exit(1) #Pod did not get marked as running :(
+
 
 def _compose_restart_service(service, config):
     if shutil.which("docker-compose") == None:
         _logger.error("docker-compose not found on $PATH")
         sys.exit(1)
     composeYaml = None
     if const.DOCKER_COMPOSE_CONFIG in os.environ.keys():
         composeYaml = os.environ.get(const.DOCKER_COMPOSE_CONFIG)
     elif config.container.docker_compose_yaml is not None:
         composeYaml = config.container.docker_compose_yaml
     else:
-        _logger.error("Unable to find docekr-compose YAML configuration")
+        _logger.error("Unable to find docker-compose YAML configuration")
         sys.exit(1)
     if not composeYaml.startswith('/'):
         composeYaml = config_base_dir() + '/' + composeYaml
     ps = subprocess.run(['docker-compose', '-f' , composeYaml, 'restart', service])
     if ps.returncode != 0:
         _logger.error("Error restarting docker-compose container:\nstdout: {}\nstderr{}".format(ps.stdout, ps.stderr))
         sys.exit(1)
 
 def _docker_restart_container(container, config):
     if shutil.which("docker") == None:
         _logger.error("docker  not found on $PATH")
         sys.exit(1)
-    ps = subprocess.run(['docker', 'resart', container])
+    ps = subprocess.run(['docker', 'restart', container])
     if ps.returncode != 0:
         _logger.error("Error restarting docker container:\nstdout: {}\nstderr{}".format(ps.stdout, ps.stderr))
         sys.exit(1)
 
 
 def deploy_pending_changes(factory=None, isvaConfig=None, restartContainers=True):
     if not isvaConfig:
@@ -195,15 +191,15 @@
 
     factory.get_system_settings().configuration.deploy_pending_changes()
     if factory.is_docker() == True and isvaConfig.container is not None:
         factory.get_system_settings().docker.publish()
         if restartContainers == True:
             if isvaConfig.container.k8s_deployments is not None:
                 namespace = isvaConfig.container.k8s_deployments.namespace
-                #Are we restarting the containers or rolling out a restard to the deployment descriptor
+                #Are we restarting the containers or rolling out a restart to the deployment descriptor
                 if isvaConfig.container.k8s_deployments.deployments is not None:
                     for deployment in isvaConfig.container.k8s_deployments.deployments:
                         _kube_rollout_restart(KUBE_CLIENT, namespace, deployment)
 
                 elif isvaConfig.container.k8s_deployments.pods is not None:
                     for pod in isvaConfig.container.pods:
                         _kube_restart_container(KUBE_CLIENT, namespace, pod)
@@ -213,9 +209,11 @@
                     _compose_restart_service(service, isvaConfig)
 
             elif isvaConfig.container.containers is not None:
                 _docker_restart_container(container, isvaConfig)
 
             else:
                 _logger.error("Unable to perform container restart, this may lead to errors")
+            _logger.info("Idle for {}s to allow orchestration to recover and Verify Access components to initialize.".format(KUBE_CLIENT_SLEEP))
+            time.sleep(KUBE_CLIENT_SLEEP)
         else:
             _logger.debug("Not asked to restart containers")
```

### Comparing `verify_access_autoconf-0.1.0/src/verify_access_autoconf/util/data_util.py` & `verify_access_autoconf-0.3.0/src/verify_access_autoconf/util/data_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,28 +3,40 @@
 @copyright: IBM
 """
 import os
 import yaml
 import base64
 import kubernetes
 import pathlib
+from copy import deepcopy
 from . import constants as const
 
 def to_camel_case(snake_case):
     parts = snake_case.split('_')
     return parts[0] + ''.join(x.title() for x in parts[1:])
 
-
 def remap_keys(data_dict, remap_dict):
     '''
     old_dict: dictionary with keys to be remapped
     remap_dict: dictionary with mapping {old_key: new_key}
     '''
+    if not isinstance(data_dict, dict) or not isinstance(remap_dict, dict):
+        raise TypeError("give me dictionaries")
     return {remap_dict.get(k, k): v for k, v in data_dict.items()}
 
+#Method guaranteed to return a list with at least dictionary in it (if its not empty)
+def optional_list(x):
+    if isinstance(x, list) and len(x) > 0:
+        return x
+    else:
+        return [{}]
+
+#Filter a list of dicts on a given key for a given value
+def filter_list(attribute, value, _list):
+    return list(filter(lambda x: attribute in x and x[attribute] == value, _list))
 
 class Map(dict):
     def __init__(self, *args, **kwargs):
         super(Map, self).__init__(*args, **kwargs)
         for a in args:
             if isinstance(a, dict):
                 for k, v in a.items():
@@ -63,14 +75,17 @@
         super(Map, self).__setitem__(k, v)
         self.__dict__.update({k: v})
 
     def __delitem__(self, k):
         super(Map, self).__delitem__(k)
         del self.__dict__[k]
 
+    def __deepcopy__(self, memo=None):
+        return Map(deepcopy(dict(self), memo=memo)) 
+
 
 class CustomLoader(yaml.SafeLoader):
 
     def __init__(self, path):
         self._root = os.path.split(path.name)[0]
         super(CustomLoader, self).__init__(path)
         CustomLoader.add_constructor('!include', CustomLoader.include)
@@ -150,7 +165,12 @@
                     kubernetes.config.load_config()
                 except kubernetes.config.config_exception.ConfigException:
                     cls._caught = True
             cls._client = kubernetes.client
         return cls._client
 
 KUBE_CLIENT = ISVA_Kube_Client.get_client()
+KUBE_CLIENT_SLEEP = 15
+try:
+    KUBE_CLIENT_SLEEP = int(os.environ.get("ISVA_KUBERNETES_RESTART_SLEEP", 15))
+except ValueError:
+    KUBE_CLIENT_SLEEP = 15
```

### Comparing `verify_access_autoconf-0.1.0/src/verify_access_autoconf/webseal.py` & `verify_access_autoconf-0.3.0/src/verify_access_autoconf/webseal.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 import logging
 import json
 import typing
 
 from .util.configure_util import deploy_pending_changes
-from .util.data_util import Map, FILE_LOADER
+from .util.data_util import Map, FILE_LOADER, optional_list, filter_list
 
 _logger = logging.getLogger(__name__)
 
 
 class WEB_Configurator(object):
 
     factory = None
@@ -27,46 +27,46 @@
     def __update_stanza(self, proxy_id, entry):
         rsp = self.web.reverse_proxy.update_configuration_stanza_entry(
                 proxy_id, entry.stanza, entry.entry_id, entry.value)
         if rsp.success == True:
             _logger.info("Successfully updated stanza [{}] with [{}:{}]".format(
                     entry.stanza, entry.entry_id, entry.value))
         else:
-            _logger.error("Failed to update stanza [{}] with [{}:{}]".format(
-                    entry.stanza, entry.entry_id, entry.value))
+            _logger.error("Failed to update stanza [{}] with [{}:{}]\n{}".format(
+                    entry.stanza, entry.entry_id, entry.value, rsp.data))
 
     def __add_stanza(self, proxy_id, entry):
         rsp = None
         if entry.entry_id:
             rsp = self.web.reverse_proxy.add_configuration_stanza_entry(
                     proxy_id, entry.stanza, entry.entry_id, entry.value)
         elif entry.stanza:
             rsp = self.web.reverse_proxy.add_configuration_stanza(proxy_id, entry.stanza)
         else:
             _logger.error("Configuration invalid:\n{}".format(json.dumps(entry, indent=4)))
             return
         if rsp.success == True:
             _logger.info("Successfully created stanza entry")
         else:
-            _logger.error("Failed to create stanza entry:\n{}\n{}".format(json.dumps(entry, indent=4), rsp.content))
+            _logger.error("Failed to create stanza entry:\n{}\n{}".format(json.dumps(entry, indent=4), rsp.data))
 
     def __delete_stanza(self, proxy_id, entry):
         rsp = None
         if entry.entry_id:
             rsp = self.web.reverse_proxy.delete_configuration_stanza_entry(proxy_id, entry.stanza, entry.entry_id,
                     entry.value)
         elif entry.stanza:
             rsp = self.web.reverse_proxy.delete_configuration_stanza(proxy_id, entry.stana)
         else:
             _logger.error("Stanza configuration entry invalid:\n{}".format(json.dumps(entry, indent=4)))
             return
         if rsp.success == True:
             _logger.info("Successfully deleted stanza entry")
         else:
-            _logger.error("Failed to delete stanza entry:\n{}\n{}".format(json.dumps(entry, indent=4), rsp.content))
+            _logger.error("Failed to delete stanza entry:\n{}\n{}".format(json.dumps(entry, indent=4), rsp.data))
 
     def _configure_stanza(self, proxy_id, config):
         for entry in config:
             if entry.operation == "delete":
                 self.__delete_stanza(proxy_id, entry)
             elif entry.operation == "add":
                 self.__add_stanza(proxy_id, entry)
@@ -89,16 +89,16 @@
                                 "runtime_username": aac_config.runtime.user,
                                 "runtime_password": aac_config.runtime.password
                             })
         rsp = self.web.reverse_proxy.configure_aac(proxy_id, **methodArgs)
         if rsp.success == True:
             _logger.info("Successfully ran Advanced Access Control configuration wizard on {} proxy instance".format(proxy_id))
         else:
-            _logger.error("Failed to run AAC configuration wizard on {} proxy instance with config:\n{}".format(
-                proxy_id, json.dumps(aac_config, indent=4)))
+            _logger.error("Failed to run AAC configuration wizard on {} proxy instance with config:\n{}\n{}".format(
+                proxy_id, json.dumps(aac_config, indent=4), rsp.data))
 
 
     def _configure_mmfa(self, proxy_id, mmfa_config):
         methodArgs = {
                 "reuse_acls": mmfa_config.reuse_acls,
                 "reuse_pops": mmfa_config.reuse_pops,
                 "reuse_certs": mmfa_config.reuse_certs,
@@ -120,55 +120,55 @@
                     "runtime_username": runtime.username,
                     "runtime_password": runtime.password
                 })
         rsp = self.web.reverse_proxy.configure_mmfa(proxy_id, **methodArgs)
         if rsp.success == True:
             _logger.info("Successfully ran MMFA configuration wizard on {} proxy instance".format(proxy_id))
         else:
-            _logger.error("Failed to run MMFA configuration wizard on {} proxy instance with config:\n{}".format(
-                proxy_id, json.dumps(mmfa_config, indent=4)))
+            _logger.error("Failed to run MMFA configuration wizard on {} proxy instance with config:\n{}\n{}".format(
+                proxy_id, json.dumps(mmfa_config, indent=4), rsp.data))
 
 
     def _configure_federations(self, proxy_id, fed_config):
         rsp = self.web.reverse_proxy.configure_fed(proxy_id, **fed_config )
         if rsp.success == True:
             _logger.info("Successfully ran federation configuration utility with")
         else:
-            _logger.error("Federation configuration wizard did not run successfully with config:\n{}".format(
-                json.dumps(fed_config, indent=4)))
+            _logger.error("Federation configuration wizard did not run successfully with config:\n{}\n{}".format(
+                json.dumps(fed_config, indent=4), rsp.data))
 
 
     def _add_junction(self, proxy_id, junction):
         forceJunction = False
-        junctions = self.web.reverse_proxy.list_junctions(proxy_id).json
+        junctions = optional_list(self.web.reverse_proxy.list_junctions(proxy_id).json)
         for jct in junctions:
-            if jct["id"] == junction.junction_point:
+            if jct and jct["id"] == junction.junction_point:
                 junction['force'] = "yes"
 
         rsp = self.web.reverse_proxy.create_junction(proxy_id, **junction)
 
         if rsp.success == True:
             _logger.info("Successfully added junction to {} proxy".format(proxy_id))
         else:
-            _logger.error("Failed to add junction to {} with config:\n{}".format(
-                proxy_id, json.dumps(junction, indnet=4)))
+            _logger.error("Failed to add junction to {} with config:\n{}\n{}".format(
+                proxy_id, json.dumps(junction, indent=4), rsp.data))
 
     class Reverse_Proxy(typing.TypedDict):
         '''
         .. note:: Configuration to connect to the user registry is read from the ``webseal.runtime`` entry.
 
         .. note:: Federations configured in ths step must already exist. If federations are being created and configured
                   for WebSEAL at the same time then the reverse proxy configuration should be added to the federation
-                  configuration dictionary.
+                  configuration properties.
 
         Example::
 
                   reverse_proxy:
                   - name: "default"
-                    host: "hostname"
+                    host: "ibmsec.verify.access"
                     listening_port: 7234
                     domain: "Default"
                     http:
                     - enabled: "no"
                     https:
                     - enabled: "yes"
                       port: 443
@@ -176,22 +176,22 @@
                     - name: "/app"
                       transparent_path: True
                       server:
                         host: "1.2.3.4"
                         port: 443
                       ssl:
                       - enabled: "yes"
-                        key_file: "example.kdb",
+                        key_file: "pdsrv.kdb",
                         cert_file: "server"
-                    aac_configuration_wizard:
+                    aac_configuration:
                       hostname: "localhost"
                       port: 443
                       runtime:
-                        user: "easuser"
-                        password: "password"
+                        user: !secret default/isva-secrets:runtime_user
+                        password: !secret default/isva-secrets:runtime_password
                       junction: "/mga"
                       reuse_acls: True
                       reuse_certs: True
 
         '''
 
         class AAC_Configuration(typing.TypedDict):
@@ -396,29 +396,27 @@
         'LDAP policy server properties.'
         http: Endpoint
         'HTTP traffic endpoint properties.'
         https: Endpoint
         'HTTPS traffic endpoint properties.'
         junctions: typing.Optional[typing.List[Junction]]
         'Junctions to backend resource servers for this reverse proxy instance.'
-        aac_config: typing.Optional[AAC_Configuration]
+        aac_configuration: typing.Optional[AAC_Configuration]
         'Properties for configuring this reverse proxy instance for use with advanced access control authentication and context based access service.'
-        mmfa_config: typing.Optional[MMFA_Configuration]
+        mmfa_configuration: typing.Optional[MMFA_Configuration]
         'Properties for configuring this reverse proxy instance to deliver MMFA capabilities.'
-        federation: typing.Optional[Federation_Configuration]
+        federation_configuration: typing.Optional[Federation_Configuration]
         'Properties for integrating with a running Federation runtime.'
         stanza_configuration: typing.Optional[Stanza_Configuration]
         'List of modifications to perform on the ``webseald.conf`` configuration file for this reverse proxy instance.'
 
     def wrp(self, runtime, proxy):
-        wrp_instances = self.web.reverse_proxy.list_instances().json
-        if wrp_instances == None:
-            wrp_instances = []
+        wrp_instances = optional_list(self.web.reverse_proxy.list_instances().json)
         for instance in wrp_instances:
-            if instance['id'] == proxy.name:
+            if instance and instance['id'] == proxy.name:
                 rsp = self.web.reverse_proxy.delete_instance(proxy.name,
                         runtime.admin_user if runtime.admin_user else "sec_master",
                         runtime.admin_password)
                 if rsp.success != True:
                     _logger.error("WebSEAL Reverse proxy {} already exists with config: \n{}\nand cannot be removed".format(
                         proxy.name, proxy))
                     return
@@ -473,19 +471,17 @@
         if proxy.stanza_configuration != None:
             self._configure_stanza(proxy.name, proxy.stanza_configuration)
 
         deploy_pending_changes(self.factory, self.config)
         if self.factory.is_docker() == False:
             rsp = self.web.reverse_proxy.restart_instance(proxy.name)
             if rsp.success == True:
-                _logger.info("Successfully restart {} proxy instance after applying configuration".format(
-                    proxy.name))
+                _logger.info("Successfully restart {} proxy instance after applying configuration".format(proxy.name))
             else:
-                _logger.error("Failed to restart {} proxy instance after applying configuration".format(
-                    proxy.name))
+                _logger.error("Failed to restart {} proxy instance after applying configuration".format(proxy.name))
 
 
     def _runtime_stanza(self, stanza_config):
         for entry in stanza_config:
             rsp = None
             if entry.operation == "add":
                 entries = [ [entry.entry, entry.value] ] if entry.entry else None
@@ -497,20 +493,20 @@
                     _logger.error("Update operation for {} is missing entry or value property, skipping".format(entry))
                     continue
                 entries = [ [entry.entry, entry.value] ]
                 rsp = self.web.runtime_component.update_configuration_file_entry(resource=entry.resource,
                                                                                 stanza=entry.stanza, entries=entries)
 
             elif entry.operation == "delete":
-                rsp = self.web.runtime_component.delete_configuration_file_entry(respource=entry.resource,
+                rsp = self.web.runtime_component.delete_configuration_file_entry(resource=entry.resource,
                                                                                  stanza=entry.stanza, entry=entry.entry,
                                                                                  value=entry.value)
             else:
-                _logger.error("Unable to determine operation for stanza file modification:\n{}\n. . . skipping".format(
-                                                                                                                entry))
+                _logger.error("Unable to determine operation for stanza file modification:" + 
+                                "\n{}\n. . . skipping".format(entry))
                 continue
             if rsp.success == True:
                 _logger.info("Successfully modified the {} stanza file".format(entry.stanza))
             else:
                 _logger.error("Failed to modify stanza properties file with config:\n{}\n{}".format(
                                                                                 json.dumps(entry, indent=4), rsp.data))
 
@@ -590,15 +586,15 @@
         'Remove any existing user data from registry. Only valid if ``user_registry == "local"``.'
         isam_domain: str
         'The Security Verify Access domain name.'
         admin_password: str
         'The password for the ``sec_master`` user.'
         admin_cert_lifetime: int
         'The lifetime in days for the SSL server certificate.'
-        ssl_complaince: str
+        ssl_compliance: str
         'Specifies whether SSL is compliant with any additional computer security standard. "fips" | "sp800-131-transition" | "sp800-131-strict" | "suite-b-128" | "suite-b-192".'
         ldap: LDAP
         'LDAP server properties.'
         isam: typing.Optional[ISAM]
         'Verify Access policy server properties.'
         stanza_configuration: typing.Optional[typing.List[Stanza_Configuration]]
         'Optional list of modifications to configuration files.'
@@ -675,26 +671,26 @@
         if acl.unauthenticated:
             pdadminCommands += ["acl modify {} set unauthenticated {}".format(acl.name, acl.unauthenticated)]
 
         rsp = self.web.policy_administration.execute(runtime.admin_user, runtime.admin_password, pdadminCommands)
         if rsp.success == True:
             _logger.info("Successfully created acl {}".format(acl.name))
         else:
-            _logger.error("Failed to create acl {} with config:\n{}\n{}".format(acl.name, json.dumps(acl, indent=4),
-                rsp.content))
+            _logger.error("Failed to create acl {} with config:\n{}\n{}".format(
+                    acl.name, json.dumps(acl, indent=4), rsp.data))
 
     def _pdadmin_pop(self, runtime, pop):
         pdadminCommands = ["pop create {}".format(pop.name)]
         if pop.description:
             pdadminCommands += ["pop modify {} set description {}".format(pop.name, pop.description)]
 
         if pop.attributes:
             for attribute in pop.attributes:
-                pdadminCommands += ["pop modify {} set attribute {} {}".format(pop.name, attrbute.name,
-                    attribute.value)]
+                pdadminCommands += ["pop modify {} set attribute {} {}".format(
+                                    pop.name, attribute.name, attribute.value)]
 
         if pop.tod_access:
             pdadminCommands += ["pop modify {} set tod-access {}".format(pop.name, pop.tod_access)]
 
         if pop.audit_level:
             pdadminCommands += ["pop modify {} set audit-level {}".format(pop.name, pop.audit_level)]
 
@@ -707,16 +703,16 @@
                     pdadminCommands += ["pop modify {} set ipauth {} {}".format(pop.name, network.network,
                         network.netmask, network.auth_level)]
 
         rsp = self.web.policy_administration.execute(runtime.admin_user, runtime.admin_password, pdadminCommands)
         if rsp.success == True:
             _logger.info("Successfully created pop {}".format(pop.name))
         else:
-            _logger.error("Failed to create pop {} with config:\n{}\n{}".format(pop.name, json.dumps(pop, indent=4),
-                rsp.content))
+            _logger.error("Failed to create pop {} with config:\n{}\n{}".format(
+                        pop.name, json.dumps(pop, indent=4), rsp.data))
 
     def _pdadmin_proxy(self, runtime, proxy_config):
         pdadminCommands = []
         if proxy_config.acls:
             for acl in proxy_config.acls:
                 for junction in acl.junctions:
                     pdadminCommands += ["acl attach /{}/{} {}".format(proxy_config.host, junction, acl.name)]
@@ -726,62 +722,60 @@
                 for junction in pop.junctions:
                     pdadminCommands += ["pop attach /{}/{} {}".format(proxy_config.host, junction, pop.name)]
 
         rsp = self.web.policy_administration.execute(runtime.admin_user, runtime.admin_password, pdadminCommands)
         if rsp.success == True:
             _logger.info("Successfully attached acls/pops to {}".format(proxy_config.host))
         else:
-            _logger.error("Failed to attach acls/pops to {} with config:\n{}\n{}".format(proxy_config.host,
-                json.dumps(proxy_config, indent=4),
-                rsp.content))
+            _logger.error("Failed to attach acls/pops to {} with config:\n{}\n{}".format(
+                    proxy_config.host, json.dumps(proxy_config, indent=4), rsp.data))
 
     def _pdadmin_user(self, runtime, user):
         firstName = user.first_name if user.first_name else user.name
         lastName = user.last_name if user.last_name else user.name
         pdadminCommands = [
                 "user create {} {} {} {} {}".format(
                     user.name, user.dn, firstName, lastName, user.password),
                 "user modify {} account-valid yes".format(user.name)
             ]
         rsp = self.web.policy_administration.execute(runtime.admin_user, runtime.admin_password, pdadminCommands)
         if rsp.success == True:
             _logger.info("Successfully created user {}".format(user.name))
         else:
-            _logger.error("Failed to create user {} with config:\n{}\n{}".format(user.name, json.dumps(user, indent=4),
-                rsp.content))
+            _logger.error("Failed to create user {} with config:\n{}\n{}".format(
+                        user.name, json.dumps(user, indent=4), rsp.data))
 
     def _pdadmin_groups(self, runtime, group):
         pdadminCommands = ["group create {} {} {}".format(group.name, group.dn, group.description)]
         if group.users:
             for user in group.users:
                 pdadminCommands += ["group modify {} add user {}".format(group.name, user)]
         rsp = self.web.policy_administration.execute(runtime.admin_user, runtime.admin_password, pdadminCommands)
         if rsp.success == True:
             _logger.info("Successfully created group {}".format(group.name))
         else:
-            _logger.error("Failed to create group {} with config:\n{}\n{}".format(group.name,
-                json.dumps(group, indent=4), rsp.content))
-
+            _logger.error("Failed to create group {} with config:\n{}\n{}".format(
+                        group.name, json.dumps(group, indent=4), rsp.data))
 
     class PD_Admin(typing.TypedDict):
         '''
         .. note:: Configuration to connect to the user registry is read from the ``webseal.runtime`` entry.
 
         Example::
 
                 pdadmin:
                   users:
                     - username: "testuser"
-                      password: "Passw0rd"
+                      password: !secret default/isva-secrets:test_password
                       dn: "cn=testuser,dc=iswga"
                     - username: "aaascc"
-                      password: "S3cr37"
+                      password: !secret default/isva-secrets:aac_user_password
                       dn: "cn=aaascc,dc=iswga"
                     - username: "ob_client"
-                      password: "abcd1234"
+                      password: !secret default/isva-secrets:ob_client_password
                       dn: "cn=ob_client,dc=iswga"
                   reverse_proxies:
                     - host: "default-proxy"
                       acls:
                         - name: "isam_mobile_anyauth"
                           junctions:
                             - "/mga/sps/authsvc"
@@ -961,15 +955,15 @@
         if config.users != None:
             for user in config.users:
                 self._pdadmin_user(runtime, user)
 
         if config.reverse_proxies != None:
             for proxy in config.reverse_proxies:
                 self._pdadmin_proxy(proxy)
-        deploy_pending_changes(self.factory, self.config)
+        #deploy_pending_changes(self.factory, self.config)
 
 
     class Client_Certificate_Mapping(typing.TypedDict):
         '''
         Example::
 
                    client_cert_mapping:
@@ -987,15 +981,16 @@
             if len(cert_mapping_file) != 1:
                 _logger.error("Can only specify one cert mapping file")
                 return
             rsp = self.web.client_cert_mapping.create(name=cert_mapping_file['name'], content=cert_mapping_file['content'])
             if rsp.success == True:
                 _logger.info("Successfully configured certificate mapping")
             else:
-                _logger.error("Failed to configure certificate mapping using {} config file".format(cert_mapping_file['name']))
+                _logger.error("Failed to configure certificate mapping using {} config file:\n{}".format(
+                            cert_mapping_file['name'], rsp.data))
 
 
 
     class Junction_Mapping(typing.TypedDict):
         '''
         Example::
 
@@ -1015,15 +1010,16 @@
             if len(jct_mapping_file) != 1:
                 _logger.error("Can only specify one jct mapping file")
                 return
             rsp = self.web.jct_mapping.create(name=jct_mapping_file['name'], jmt_config_data=jct_mapping_file['content'])
             if rsp.success == True:
                 _logger.info("Successfully configured junction mapping")
             else:
-                _logger.error("Failed to configure junction mapping using {} config file".format(jct_mapping_file['name']))
+                _logger.error("Failed to configure junction mapping using {} config file:\n{}".format(
+                                jct_mapping_file['name'], rsp.data))
 
 
     class Url_Mapping(typing.TypedDict):
         '''
         Examples::
 
                   url-mapping:
@@ -1040,15 +1036,16 @@
             if len(url_mapping_file) != 1:
                 _logger.error("Can only specify one url mapping file")
                 return
             rsp = self.web.url_mapping.create(name=url_mapping_file['name'], dynurl_config_data=url_mapping_file['content'])
             if rsp.success == True:
                 _logger.info("Successfully configured URL mapping")
             else:
-                _logger.error("Failed to configure URL mapping using {} config file".format(url_mapping_file['name']))
+                _logger.error("Failed to configure URL mapping using {} config file:\n{}".format(
+                                url_mapping_file['name'], rsp.data))
 
 
     class User_Mapping(typing.TypedDict):
         '''
         Example::
 
                   user_mapping:
@@ -1065,15 +1062,16 @@
             if len(user_mapping_file) != 1:
                 _logger.error("Can only specify one user mapping file")
                 return
             rsp = self.web.user_mapping.create(name=user_mapping_file['name'], content=user_mapping_file['content'])
             if rsp.success == True:
                 _logger.info("Successfully configured user mapping")
             else:
-                _logger.error("Failed to configure user mapping using {} config file".format(user_mapping_file['name']))
+                _logger.error("Failed to configure user mapping using {} config file:\n{}".format(
+                                user_mapping_file['name'], rsp.data))
 
 
     class Form_Single_Sign_On(typing.TypedDict):
         '''
         Example::
 
                 fsso:
@@ -1090,15 +1088,16 @@
             if len(user_mapping_file) != 1:
                 _logger.error("Can only specify one FSSO configuration file")
                 return
             rsp = self.web.fsso.create(name=fsso_config_file['name'], fsso_config_data=fsso_config_file['content'])
             if rsp.success == True:
                 _logger.info("Successfully configured Federated Singe Sign On configuration")
             else:
-                _logger.error("Failed to configure FSSO using {} config file".format(user_mapping_file['name']))
+                _logger.error("Failed to configure FSSO using {} config file:\n{}".format(
+                                user_mapping_file['name'], rsp.data))
 
 
     class Http_Transformations(typing.TypedDict):
         '''
         Example::
 
                    http_transforms:
@@ -1122,16 +1121,16 @@
 
 
     def __create_kerberos_property(self, _id, subsection, name, value):
         rsp = self.web.kerberos.create(_id=_id, name=name, value=value)
         if rsp.success == True:
             _logger.info("Successfully configured Kerberos property")
         else:
-            _logger.error("Failed to configure Kerberos property:\nsubsection: {} name: {} value:{}\n{}".format(subsection,
-                name, value, rsp.content))
+            _logger.error("Failed to configure Kerberos property:\nsubsection: {} name: {} value:{}\n{}".format(
+                            subsection, name, value, rsp.data))
 
 
     class Kerberos(typing.TypedDict):
         '''
         Example::
 
                    kerberos:
@@ -1183,26 +1182,26 @@
         if config.domain_realms != None:
             for domain_realm in config.domain_realms: self.__create_kerberos_property("domain_realm", None,
                     domain_ream.name, domain_realm.dns)
         if config.capaths != None:
             for capath in config.capaths:
                 self.__create_kerberos_property("capaths", capath.name, None, None)
                 if capath.properties != None:
-                    for prop, value  in capath.properties: elf.__create_kerberos_property("capaths/" + capath.name,
+                    for prop, value in capath.properties: self.__create_kerberos_property("capaths/" + capath.name,
                             None, prop, value)
         if config.keytabs != None:
             for kf in config.keytabs:
                 if not kf.startswith('/'):
                     kf = config_base_dir() + kf
                 rsp = self.web.kerberos.import_keytab(kf)
                 if rsp.success == True:
                     _logger.info("Successfully imported Kerberos Keytab file")
                 else:
-                    _logger.error("Failed to import Kerberos Keytab file:\n{}\n{}".format(json.dumps(prop, indent=4),
-                        rsp.content))
+                    _logger.error("Failed to import Kerberos Keytab file:\n{}\n{}".format(
+                                json.dumps(prop, indent=4), rsp.data))
 
 
     class Password_Strength(typing.TypedDict):
         '''
         Example::
 
                    password_strength:
@@ -1217,15 +1216,16 @@
         if len(pwd_mapping_file) != 1:
             _logger.error("Can only specify one password strength rule file")
             return
         rsp = self.web.password_strength.create(name=pwd_config_file['name'], content=pwd_config_file['content'])
         if rsp.success == True:
             _logger.info("Successfully configured password strength rules")
         else:
-            _logger.error("Failed to configure password strength rules using {}".format(pwd_mapping_file['name']))
+            _logger.error("Failed to configure password strength rules using {}\n{}".format(
+                            pwd_mapping_file['name'], rsp.data))
 
 
     class RSA(typing.TypedDict):
         '''
         Example::
 
                    rsa_config:
@@ -1235,363 +1235,466 @@
         '''
         server_config: str
         'The server configuration file to upload.'
         optional_server_config: str
         'The server configuration options file to upload.'
 
     def rsa(self, rsa_config):
-        rsp = self.web.rsa.create(name=rsa_config.server_config if rsa_config.server_config.startswith("/") else
-              config_base_dir() + rsa_config.server_config)
+        server_config = FILE_LOADER.read_file(rsa_config.server_config)
+        methodArgs = { "server_config_file": server_config['path']}
+        if rsa_config.optional_server_config:
+            opts_config = FILE_LOADER.read_file(rsa_config.optional_server_config)
+            methodArgs.update({"server_options_file": opts_config['path']})
+        rsp = self.web.rsa.create(**methodArgs)
         if rsp.success == True:
             _logger.info("Successfully configured RSA")
         else:
-            _logger.error("Failed to configure RSA using {}".format(rsa_config.server_config))
-        rsa_optional_config_file = None
-        if rsa_config.optional_server_config != None:
-            rsa_optional_config_file = rsa_config.optional_server_config
+            _logger.error("Failed to configure RSA using:\n{}\n{}".format(
+                            json.dumps(rsa_config, indent=4), rsp.data))
 
 
-    def __apiac_resources(self, proxy_id, resources):
-        for resource in resources:
+    def __apiac_authz_server(self, runtime, authz_servers):
+        for authz_server in authz_servers:
+            methodArgs = {"hostname": authz_server.hostname,
+                          "auth_port": authz_server.auth_port,
+                          "admin_port": authz_server.admin_port,
+                          "domain": authz_server.domain,
+                          "admin_id": runtime.admin_id,
+                          "admin_pwd": runtime.admin_password,
+                          "addresses": authz_server.addresses,
+                          "ssl": authz_server.ssl,
+                          "ssl_port": authz_server.ssl_port,
+                          "key_file": authz_server.key_file,
+                          "key_label": authz_server.key_label
+                }
+            rsp = self.web.apiac.authz_server.create_server(authz_server.name, **methodArgs)
+            if rsp.success == True:
+                _logger.info("Successfully created {} API Access Control Authorization Server".format(authz_server.name))
+            else:
+                _logger.error("Failed to create API Authorization Server:\n{}\n{}".format(
+                                                            json.dumps(authz_server, indent=4), rsp.data))
+
+    def __apiac_resource_server(self, resource_servers):
+        for resource_server in resource_servers:
             methodArgs = {
-                    "server_hostname": resource.server_hostname,
-                    "junction_point": resource.junction_point,
-                    "junction_type": resource.junction_type,
-                    "static_response_headers": resource.static_response_headers,
-                    "description": resource.description,
-                    "junction_hard_limit": resource.junction_hard_limit,
-                    "junction_soft_limit": resource.junction_soft_limit,
-                    "basic_auth_mode": resource.basic_auth_mode,
-                    "tfim_sso": resource.tfim_sso,
-                    "remote_http_header": resource.remote_http_header,
-                    "stateful_junction": resource.stateful_junction,
-                    "http2_junction": resource.http2_junction,
-                    "sni_name": resource.sni_name,
-                    "preserve_cookie": resource.preserve_cookie,
-                    "cookie_include_path": resource.cookie_include_path,
-                    "transparent_path_junction": resource.transparent_path_junction,
-                    "mutual_auth": resource.mutual_auth,
-                    "insert_ltpa_cookies": resource.insert_ltpa_cookies,
-                    "insert_session_cookies": resource.insert_session_cookies,
-                    "request_encoding": resource.request_encoding,
-                    "enable_basic_auth": resource.enable_basic_auth,
-                    "key_labelkey_label": resource.key_label,
-                    "gso_resource_group": resource.gso_resource_group,
-                    "junction_cookie_javascript_block": resource.junction_cookie_javascript_block,
-                    "client_ip_http": resource.client_ip_http,
-                    "version_two_cookies": resource.version_two_cookies,
-                    "ltpa_keyfile": resource.ltpa_keyfile,
-                    "authz_rules": resource.authz_rules,
-                    "fsso_config_file": resource.fsso_config_file,
-                    "username": resource.username,
-                    "password": resource.password,
-                    "server_uuid": resource.server_uuid,
-                    "server_port": resource.server_port,
-                    "virtual_hostname" : resource.virtual_hostname,
-                    "server_dn": resource.server_dn,
-                    "local_ip": resource.local_ip,
-                    "query_contents": resource.query_contents,
-                    "case_sensitive_url": resource.case_sensitive_url,
-                    "windows_style_url": resource.windows_style_url,
-                    "ltpa_keyfile_password": resource.ltpa_keyfile_password,
-                    "https_port": resource.https_port,
-                    "http_port": resource.http_port,
-                    "proxy_hostname": resource.proxy_hostname,
-                    "proxy_port": resource.proxy_port,
-                    "sms_environment": resource.sms_environment,
-                    "vhost_label": resource.vhost_label,
-                    "force": resource.force,
-                    "delegation_support": resource.delegation_support,
-                    "scripting_support": resource.scripting_support
+                    "server_hostname": resource_server.server_hostname,
+                    "junction_point": resource_server.junction_point,
+                    "junction_type": resource_server.junction_type,
+                    "static_response_headers": resource_server.static_response_headers,
+                    "description": resource_server.description,
+                    "junction_hard_limit": resource_server.junction_hard_limit,
+                    "junction_soft_limit": resource_server.junction_soft_limit,
+                    "basic_auth_mode": resource_server.basic_auth_mode,
+                    "tfim_sso": resource_server.tfim_sso,
+                    "remote_http_header": resource_server.remote_http_header,
+                    "stateful_junction": resource_server.stateful_junction,
+                    "http2_junction": resource_server.http2_junction,
+                    "sni_name": resource_server.sni_name,
+                    "preserve_cookie": resource_server.preserve_cookie,
+                    "cookie_include_path": resource_server.cookie_include_path,
+                    "transparent_path_junction": resource_server.transparent_path_junction,
+                    "mutual_auth": resource_server.mutual_auth,
+                    "insert_ltpa_cookies": resource_server.insert_ltpa_cookies,
+                    "insert_session_cookies": resource_server.insert_session_cookies,
+                    "request_encoding": resource_server.request_encoding,
+                    "enable_basic_auth": resource_server.enable_basic_auth,
+                    "key_labelkey_label": resource_server.key_label,
+                    "gso_resource_group": resource_server.gso_resource_group,
+                    "junction_cookie_javascript_block": resource_server.junction_cookie_javascript_block,
+                    "client_ip_http": resource_server.client_ip_http,
+                    "version_two_cookies": resource_server.version_two_cookies,
+                    "ltpa_keyfile": resource_server.ltpa_keyfile,
+                    "authz_rules": resource_server.authz_rules,
+                    "fsso_config_file": resource_server.fsso_config_file,
+                    "username": resource_server.username,
+                    "password": resource_server.password,
+                    "server_port": resource_server.server_port,
+                    "virtual_hostname" : resource_server.virtual_hostname,
+                    "server_dn": resource_server.server_dn,
+                    "local_ip": resource_server.local_ip,
+                    "query_contents": resource_server.query_contents,
+                    "case_sensitive_url": resource_server.case_sensitive_url,
+                    "windows_style_url": resource_server.windows_style_url,
+                    "ltpa_keyfile_password": resource_server.ltpa_keyfile_password,
+                    "https_port": resource_server.https_port,
+                    "http_port": resource_server.http_port,
+                    "proxy_hostname": resource_server.proxy_hostname,
+                    "proxy_port": resource_server.proxy_port,
+                    "sms_environment": resource_server.sms_environment,
+                    "vhost_label": resource_server.vhost_label,
+                    "force": resource_server.force,
+                    "delegation_support": resource_server.delegation_support,
+                    "scripting_support": resource_server.scripting_support
                 }
-            if resource.policy:
-                policy = resurce.policy
+            if resource_server.policy:
+                policy = resource_server.policy
                 methodArgs.update({
-                        "name": policy.name,
-                        "type": policy.type
+                        "policy_name": policy.name,
+                        "policy_type": policy.type
                     })
-            if resource.authentication:
-                methodArgs.update({"type": resource.authentication.type})
-                if resource.autehntication.oauth_introspection:
-                    oauth_introspection = resource.autehntication.oauth_introspection
+            if resource_server.authentication:
+                methodArgs.update({"authentication_type": resource_server.authentication.type})
+                if resource_server.authentication.oauth_introspection:
+                    oauth_introspection = resource_server.authentication.oauth_introspection
                     methodArgs.update({
                             "oauth_introspection_transport": oauth_introspection.transport,
                             "oauth_introspection_endpoint": oauth_introspection.endpoint,
                             "oauth_introspection_proxy": oauth_introspection.proxy,
                             "oauth_introspection_auth_method": oauth_introspection.auth_method,
                             "oauth_introspection_client_id": oauth_introspection.client_id,
                             "oauth_introspection_client_secret": oauth_introspection.client_secret,
                             "oauth_introspection_client_id_hdr": oauth_introspection.client_id_hdr,
                             "oauth_introspection_token_type_hint": oauth_introspection.token_type_hint,
                             "oauth_introspection_mapped_id": oauth_introspection.mapped_id,
                             "oauth_introspection_external_user": oauth_introspection.external_user,
                             "oauth_introspection_response_attributes": oauth_introspection.response_attributes
                         })
-                if resource.authentication.jwt:
-                    jwt = resource.authentication.jwt
+                if resource_server.authentication.jwt:
+                    jwt = resource_server.authentication.jwt
                     methodArgs.update({
                             "jwt_header_name": jwt.header_name,
                             "jwt_certificate": jwt.certificate,
                             "jwt_claims": jwt.claims
                         })
-            rsp = self.web.api_access_control.resources.create_server(proxy_id, **methodArgs)
+            rsp = self.web.api_access_control.resource_server.create_server(resource_server.reverse_proxy, **methodArgs)
             if rsp.success == True:
                 _logger.info("Successfully created {} API AC Resource server".format(resource.server_hostname))
             else:
-                _logger.error("Failed to create {} API AC Resource serveer with config:\n{}\n{}".format(
-                    resource.server_hostname, json.dumps(resource, indent=4), rsp.content))
+                _logger.error("Failed to create {} API AC Resource server with config:\n{}\n{}".format(
+                    resource.server_hostname, json.dumps(resource, indent=4), rsp.data))
                 continue
-            if resource.junctions:
-                for junction in resource.junctions:
+            if resource_server.resources:
+                for resource in resource_server.resource:
                     methodArgs = {
-                            "server_type": junction.server_type,
-                            "method": junction.method,
-                            "path": junction.path,
-                            "name": junction.name,
-                            "static_response_headers": junction.static_response_headers,
-                            "rate_limiting_policy": junction.rate_limiting_policy,
-                            "url_aliases": junction.url_aliases
+                            "server_type": resource.server_type,
+                            "method": resource.method,
+                            "path": resource.path,
+                            "name": resource.name,
+                            "static_response_headers": resource.static_response_headers,
+                            "rate_limiting_policy": resource.rate_limiting_policy,
+                            "url_aliases": resource.url_aliases,
+                            "policy_type": resource.policy_type,
+                            "policy_name": resource.policy_name
                         }
-                    if junction.policy:
-                        policy = junction.policy
-                        methodArgs.update({
-                                "policy_type": policy.type,
-                                "policy_name": policy.name
-                            })
-                    if junction.documentation:
-                        doc = junction.documentation
+                    if resource.documentation:
+                        doc = resource.documentation
                         methodArgs.update({
                             "documentation_content_type": doc.content_type,
                             "documentation_file": doc.file
                         })
-                    rsp = self.web.api_access_control.resources.create(proxy_id, resource.junction_point, **methodArgs)
+                    rsp = self.web.api_access_control.resource_server.create_resource(
+                                resource_server.reverse_proxy, resource_server.junction_point, **methodArgs)
                     if rsp.success == True:
                         _logger.info("Successfully created {} junctioned resource".format(junction.name))
                     else:
                         _logger.error("Failed to create {} junctioned resource with config;\n{}\n{}".format(
-                            junction.name, json.dumps(junction, indent=4), rsp.content))
+                            junction.name, json.dumps(junction, indent=4), rsp.data))
+
 
     def __apiac_policies(self, policies):
         for policy in policies:
             rsp = self.web.api_access_control.policies.create(name=policy.name, groups=policy.groups, 
                                                               attributes=policy.attributes)
             if rsp.success == True:
                 _logger.info("Successfully created {} policy".format(policy.name))
             else:
-                _logger.error("Failed to create API Access Control policy {}:\n{}\n{}".format(policy.name,
-                                                                            json.dumps(policy, indent=4), rsp.content))
+                _logger.error("Failed to create API Access Control policy {}:\n{}\n{}".format(
+                                        policy.name, json.dumps(policy, indent=4), rsp.data))
 
     def __apiac_cors(self, cors_policies):
         for cors in cors_policies:
             rsp = self.web.api_access_control.cors.create(**cors)
             if rsp.success == True:
                 _logger.info("Successfully created {} CORS policy".format(cors.name))
             else:
                 _logger.error("Failed to create {} CORS policy using config:\n{}\n{}".format(cors.name,
-                    json.dumps(cors, indent=4), rsp.content))
+                    json.dumps(cors, indent=4), rsp.data))
 
     def __apiac_document_root(self, proxy_id, doc_roots):
         for doc_root in doc_roots:
             files = FILE_LOADER.read_files(doc_root, include_directories=True)
             for _file in files:
                 rsp = self.web.api_access_control.document_root.create(proxy_id, filename=_file['name'],
                         file_type=_file['type'], contents=_file.get('contents'))
                 if rsp.success == True:
                     _logger.info("Successfully uploaded {} {}".format(_file['name'], _file['type']))
                 else:
-                    _logger.error("Failed to upload {} {}\n{}".format(_file["name"], _file["type"], rsp.content))
+                    _logger.error("Failed to upload {} {}\n{}".format(_file["name"], _file["type"], rsp.data))
 
 
     class Api_Access_Control(typing.TypedDict):
         '''
         .. note:: Configuration to connect to the user registry is read from the ``webseal.runtime`` entry.
 
         Example::
 
                 api_access_control:
-                  authz_servers:
+                  authorization_servers:
+                  - name: "api_server"
+                    hostname: "localhost"
+                    auth_port: 9443
+                    admin_port: 7138
+                    domain: "Deafult"
+                    addresses:
+                    - "192.168.42.102"
+                    ssl: "yes"
+                    ssl_port: 636
+                    key_file: "pdsrv.kdb"
+                    key_alias: "webseal-cert"
+                  resource_servers:
                   - name: "authz_server"
-                    hostname: "isvaconfig"
+                    hostname: "isvaruntime"
+                    junction_point: "/scim"
+                    junction_type:"SSL"
+                    authentication:
+                      type: "oauth"
+                      oauth_introspection:
+                        transport: "both"
+                        auth_method: "client_secret_basic"
+                        endpoint: "external.com/oauth"
+                        client_id: !secret default/isva-secrets:apiac_authz_client_id
+                        mapped_id: "{iss}/{sub}"
+                        external_user: true
+                        response_attributes:
+                        - pos: 0
+                          action: "put"
+                          attribute: "test_attribute"
+                      jwt:
+                        header_name: "iv-jwt"
+                        certiciate: "cert"
+                        claims:
+                        - type: "attr"
+                          value: "AZN_CRED_PRINCIPAL_NAME"
+                          claim_name: "sub"
                     document_root:
                     - webseal_root.zip
                     resources:
                     - name: "api_ac_instance"
-                      hostname: "TODO"
+                      hostname: "ibmsec.verify.access"
                   cors:
                   - name:
-                    allowed_origins
-                    allowed_credentials
-                    exposed_headers
-                    handle_preflight
-                    allowed_methods
+                    allowed_origins:
+                    - "https://webseal.ibm.com"
+                    - "https://webseal.ibm.com:9443"
+                    - "http://static.webseal.ibm.com"
+                    - "http://static.webseal.ibm.com:9080"
+                    allowed_credentials: true
+                    exposed_headers:
+                    - "X-ISAM-VERSION"
+                    - "X-ISAM-KEY"
+                    handle_preflight: true
+                    allowed_methods:
+                    - "retry"
+                    - "IBMPost"
+                    - "Remove"
                     allowed_headers:
-                    max_age:
-
+                    - "X-ISAM-MODE"
+                    - "Content-type"
+                    max_age: 86400
 
         '''
-        class Authorization_Server(typing.TypedDict):
+        class Resource_Server(typing.TypedDict):
 
             class Resource(typing.TypedDict):
 
                 class Response_Header(typing.TypedDict):
                     name: str
                     'The name of the response header.'
                     value: str
-                    'The value of the response header'
+                    'The value of the response header.'
 
-                class Attribute(typing.TypedDict):
-                    pos: str
-                    'The position of this attribute in the ordered list of all attributes.'
-                    action: str
-                    'The action to perform for this attribute. Valid values are "put" and "remove".'
-                    attribute: str
-                    'The name of the attribute.'
-
-                class Claim(typing.TypedDict):
-                    type: str
-                    'The type of claim to add to the JWT. Valid values are either "text" for a literal text claim or "attr" for a credential attribute claim.'
-                    value: str
-                    'The value for the claim. If the type is "text" this will be the literal text that is added to the JWT. If the type is "attr" this will be the name of the credential attribute to add to the JWT.'
-                    claim_name: str
-                    'The name of the claim that is added to the JWT. For attr type claims this is optional and if not specified the claim name will be set as the name of the credential attribute. If the type is attr and the value contains a wildcard this field is invalid and if specified will result in an error. '
-
-                server_hostname: str
-                'The DNS host name or IP address of the target back-end server.'
-                server_port: int
-                'TCP port of the back-end third-party server. Default is 80 for TCP junctions and 443 for SSL junctions.'
-                virtual_hostname: typing.Optional[str]
-                'Virtual host name that is used for the junctioned Web server.'
-                server_dn: typing.Optional[str]
-                'Specifies the distinguished name of the junctioned Web server.'
-                sever_cn: typing.Optional[str]
-                'Specifies the common name, or subject alternative name, of the junctioned Web server.'
-                description: typing.Optional[str]
-                'An optional description for this junction.'
-                junction_point: str
-                'Name of the location in the Reverse Proxy namespace where the root of the back-end application server namespace is mounted.'
-                junction_type: str
-                'Type of junction. Valid values: "tcp", "ssl", "tcpproxy", "sslproxy",'
-                stateful_junction: typing.Optional[str]
-                'Specifies whether the junction supports stateful applications. By default, junctions are not stateful. Valid value is "yes" or "no".'
+                method: str
+                'The HTTP action for this resource.'
+                path: str
+                'The URI path for this resource. This is a full server relative path including the junction point.'
+                name: typing.Optional[str]
+                'A description for this resource.'
+                policy_name: str
+                'The name of the custom policy if the type is custom.'
                 policy_type: str
                 'The type of Policy. The valid values are "unauthenticated", "anyauthenticated", "none", "default" or "custom".'
-                policy_name: typing.Optional[str]
-                'The name of the custom policy if the type is custom. '
-                authentication_type: str
-                'The type of Oauth authentication. The valid values are "default" or "oauth".'
-                oauth_introspection_transport: typing.Optional[str]
-                'The transport type. The valid values are "none", "http", "https" or "both".'
-                oauth_introspection_proxy: typing.Optional[str]
-                'The proxy, if any, used to reach the introspection endpoint.'
-                oauth_introspection_auth_method: typing.Optional[str]
-                'The method for passing the authentication data to the introspection endpoint. Valid values are "client_secret_basic" or "client_secret_post".'
-                oauth_introspection_endpoint: typing.Optional[str]
-                'This is the introspection endpoint which will be called to handle the token introspection.'
-                oauth_introspection_client_id: typing.Optional[str]
-                'The client identifier which is used for authentication with the external OAuth introspection endpoint.'
-                oauth_introspection_client_secret: typing.Optional[str]
-                'The client secret which is used for authentication with the external OAuth introspection endpoint.'
-                oauth_introspection_client_id_hdr: typing.Optional[str]
-                'The name of the HTTP header which contains the client identifier which is used to authenticate to the introspection endpoint. Only valid if client_id has not been set.'
-                oauth_introspection_token_type_hint: typing.Optional[str]
-                'A hint about the type of the token submitted for introspection.'
-                oauth_introspection_mapped_id: typing.Optional[str]
-                'A formatted string which is used to construct the Verify Access principal name from elements of the introspection response. Claims can be added to the identity string, surrounded by "{}".'
-                oauth_introspection_external_user: typing.Optional[str]
-                'A boolean which is used to indicate whether the mapped identity should correspond to a known Verify Access identity or not.'
-                oauth_introspection_response_attributes: typing.List[Attribute]
-                'A list of rules indicating which parts of the json response should be added to the credential.'
-                static_response_headers: typing.List[Response_Header]
-                'A list of header names and values that should be added to the HTTP response. List of key value pairs eg: ``{"name":"Access-Control-Max-Age", "value":"600"}``'
-                jwt_header_name: typing.Optional[str]
-                'The name of the HTTP header that will contain the JWT.'
-                jwt_certificate: typing.Optional[str]
-                'The label of the personal certificate that will sign the JWT.'
-                jwt_claims: typing.Optional[Claim]
-                'The list of claims to add to the JWT.'
-                junction_hard_limit: str
-                'Defines the hard limit percentage for consumption of worker threads. Valid value is an integer from "0" to "100".'
-                junction_soft_limit: str
-                'Defines the soft limit percentage for consumption of worker threads. Valid value is an integer from "0" to "100".'
-                basic_auth_mode: typing.Optional[str]
-                'Defines how the Reverse Proxy server passes client identity information in HTTP basic authentication (BA) headers to the back-end server. The value is one of: "filter" (default), "ignore", "supply", "gso".'
-                tfim_sso: str
-                'Enables IBM Security Federated Identity Manager single sign-on (SSO) for the junction. Valid value is "yes" or "no".'
-                remote_http_header: typing.Optional[typing.List[str]]
-                'Controls the insertion of Security Verify Access specific client identity information in HTTP headers across the junction. The value is an array containing a combination of: "iv-user", "iv-user-l", "iv-groups", "iv-creds" or "all".'
-                http2_junction: typing.Optional[str]
-                'Specifies whether the junction supports the HTTP/2 protocol. By default, junctions do not support the HTTP/2 protocol. A valid value is "yes" or "no".'
-                http2_proxy: typing.Optional[str]
-                'Specifies whether the junction proxy support the HTTP/2 protocol. By default, junction proxies do not support the HTTP/2 protocol. A valid value is "yes" or "no".'
-                sni_name: typing.Optional[str]
-                'The server name indicator (SNI) to send to TLS junction servers. By default, no SNI is sent.'
-                preserve_cookie: typing.Optional[str]
-                'Specifies whether modifications of the names of non-domain cookies are to be made. Valid value is "yes" or "no".'
-                cookie_include_path: str
-                'Specifies whether script generated server-relative URLs are included in cookies for junction identification. Valid value is "yes" or "no".'
-                transparent_path_junction: str
-                'Specifies whether a transparent path junction is created. Valid value is "yes" or "no".'
-                mutual_auth: str
-                'Specifies whether to enforce mutual authentication between a front-end Reverse Proxy server and a back-end Reverse Proxy server over SSL. Valid value is "yes" or "no".'
-                insert_ltpa_cookies: str
-                'Controls whether LTPA cookies are passed to the junctioned Web server. Valid value is "yes" or "no".'
-                insert_session_cookies: str
-                'Controls whether to send the session cookie to the junctioned Web server. Valid value is "yes" or "no".'
-                request_encoding: str
-                'Specifies the encoding to use when the system generates HTTP headers for junctions. Possible values for encoding are: "utf8_bin", "utf8_uri", "lcp_bin", and "lcp_uri".'
-                enable_basic_auth: str
-                'Specifies whether to use BA header information to authenticate to back-end server. Valid value is "yes" or "no".'
-                key_label: typing.Optional[str]
-                'The key label for the client-side certificate that is used when the system authenticates to the junctioned Web server.'
-                gso_respource_group: typing.Optional[str]
-                'The name of the GSO resource or resource group.'
-                junction_cookie_javascript_block: str
-                'Controls the junction cookie JavaScript block. The value should be one of: "trailer", "inhead", "onfocus", "xhtml10".'
-                client_ip_http: str
-                'Specifies whether to insert the IP address of the incoming request into an HTTP header for transmission to the junctioned Web server. Valid value is "yes" or "no".'
-                version_two_cookies: typing.Optional[str]
-                'Specifies whether LTPA version 2 cookies (LtpaToken2) are used. Valid value is "yes" or "no".'
-                ltpa_keyfile: typing.Optional[str]
-                'Location of the key file that is used to encrypt the LTPA cookie data.'
-                authz_rules: str
-                'Specifies whether to allow denied requests and failure reason information from authorization rules to be sent in the Boolean Rule header (AM_AZN_FAILURE) across the junction. Valid value is "yes" or "no".'
-                fsso_config_file: str
-                'The name of the configuration file that is used for forms based single sign-on.'
-                username: typing.Optional[str]
-                'The Reverse Proxy user name. Used to send BA header information to the back-end server.'
-                password: typing.Optional[str]
-                'The Reverse Proxy password. Used to send BA header information to the back-end server.'
-                local_ip: typing.Optional[str]
-                'Specifies the local IP address that the Reverse Proxy uses when the system communicates with the target back-end server.'
-                query_contents: str
-                'Provides the Reverse Proxy with the correct name of the query_contents program file and where to find the file. By default, the Windows file is called query_contents.exe and the UNIX file is called query_contents.sh.'
-                case_sensitive_url: str
-                'Specifies whether the Reverse Proxy server treats URLs as case sensitive. Valid value is "yes" or "no".'
-                windows_style_url: str
-                'Specifies whether Windows style URLs are supported. Valid value is "yes" or "no".'
-                ltpa_keyfile_password: typing.Optional[str]
-                'Password for the key file that is used to encrypt LTPA cookie data.'
-                https_port: int
-                'HTTPS port of the back-end third-party server. Applicable when the junction type is "ssl".'
-                http_port: int
-                'HTTP port of the back-end third-party server. Applicable when the junction type is "tcp".'
-                proxy_hostname: typing.Optional[str]
-                'The DNS host name or IP address of the proxy server. Applicable when the junction type is "sslproxy".'
-                proxy_port: typing.Optional[int]
-                'The TCP port of the proxy server. Applicable when the junction type is "tcpproxy".'
-                sms_environment: typing.Optional[str]
-                'Only applicable for virtual junctions. Specifies the replica set that sessions on the virtual junction are managed under.'
-                vhost_label: typing.Optional[str]
-                'Only applicable for virtual junctions. Causes a second virtual junction to share the protected object space with the initial virtual junction.'
-                delegation_support: typing.Optional[str]
-                'This option is valid only with junctions that were created with the type of "ssl" or "sslproxy". Indicates single sign-on from a front-end Reverse Proxy server to a back-end Reverse Proxy server.'
-                scripting_support: typing.Optional[str]
-                'Supplies junction identification in a cookie to handle script-generated server-relative URLs. '
-                force: str
-                'Specifies whether to overwrite an existing junction of the same name. Valid value is "yes" or "no".'
+                static_response_headers: typing.Optional[typing.List[Response_Header]]
+                'A list of header names and values that should be added to the HTTP response.'
+                rate_limiting_policy: typing.Optional[str]
+                'The name of the rate limiting policy that has been set for this resource.'
+                url_aliases: typing.Optional[typing.List[str]]
+                'A list of aliases that all map to the path of this resource.'
+                doc_type: str
+                'The value of the accept header that will trigger a documentation response.'
+                doc_file: str
+                'The name and path of the documentation file to respond with, relative to the junction root.'
+
+            class Response_Header(typing.TypedDict):
+                name: str
+                'The name of the response header.'
+                value: str
+                'The value of the response header'
+
+            class Attribute(typing.TypedDict):
+                pos: str
+                'The position of this attribute in the ordered list of all attributes.'
+                action: str
+                'The action to perform for this attribute. Valid values are "put" and "remove".'
+                attribute: str
+                'The name of the attribute.'
+
+            class Policy(typing.TypedDict):
+                type: str
+                'The type of Policy. The valid values are "unauthenticated", "anyauthenticated", "none", "default" or "custom".'
+                name: typing.Optional[str]
+                'The name of the custom policy if the type is custom.'
+
+            class Claim(typing.TypedDict):
+                type: str
+                'The type of claim to add to the JWT. Valid values are either "text" for a literal text claim or "attr" for a credential attribute claim.'
+                value: str
+                'The value for the claim. If the type is "text" this will be the literal text that is added to the JWT. If the type is "attr" this will be the name of the credential attribute to add to the JWT.'
+                claim_name: str
+                'The name of the claim that is added to the JWT. For attr type claims this is optional and if not specified the claim name will be set as the name of the credential attribute. If the type is attr and the value contains a wildcard this field is invalid and if specified will result in an error. '
+
+            reverse_proxy: str
+            'Name of the WebSEAL Reverse Proxy instance this resource server is attached to.'
+            server_hostname: str
+            'The DNS host name or IP address of the target back-end server.'
+            server_port: int
+            'TCP port of the back-end third-party server. Default is 80 for TCP junctions and 443 for SSL junctions.'
+            virtual_hostname: typing.Optional[str]
+            'Virtual host name that is used for the junctioned Web server.'
+            server_dn: typing.Optional[str]
+            'Specifies the distinguished name of the junctioned Web server.'
+            sever_cn: typing.Optional[str]
+            'Specifies the common name, or subject alternative name, of the junctioned Web server.'
+            description: typing.Optional[str]
+            'An optional description for this junction.'
+            junction_point: str
+            'Name of the location in the Reverse Proxy namespace where the root of the back-end application server namespace is mounted.'
+            junction_type: str
+            'Type of junction. Valid values: "tcp", "ssl", "tcpproxy", "sslproxy",'
+            stateful_junction: typing.Optional[str]
+            'Specifies whether the junction supports stateful applications. By default, junctions are not stateful. Valid value is "yes" or "no".'
+            policy: Policy
+            'The Policy that is associated with this Resource Server.'
+            authentication_type: str
+            'The type of Oauth authentication. The valid values are "default" or "oauth".'
+            oauth_introspection_transport: typing.Optional[str]
+            'The transport type. The valid values are "none", "http", "https" or "both".'
+            oauth_introspection_proxy: typing.Optional[str]
+            'The proxy, if any, used to reach the introspection endpoint.'
+            oauth_introspection_auth_method: typing.Optional[str]
+            'The method for passing the authentication data to the introspection endpoint. Valid values are "client_secret_basic" or "client_secret_post".'
+            oauth_introspection_endpoint: typing.Optional[str]
+            'This is the introspection endpoint which will be called to handle the token introspection.'
+            oauth_introspection_client_id: typing.Optional[str]
+            'The client identifier which is used for authentication with the external OAuth introspection endpoint.'
+            oauth_introspection_client_secret: typing.Optional[str]
+            'The client secret which is used for authentication with the external OAuth introspection endpoint.'
+            oauth_introspection_client_id_hdr: typing.Optional[str]
+            'The name of the HTTP header which contains the client identifier which is used to authenticate to the introspection endpoint. Only valid if client_id has not been set.'
+            oauth_introspection_token_type_hint: typing.Optional[str]
+            'A hint about the type of the token submitted for introspection.'
+            oauth_introspection_mapped_id: typing.Optional[str]
+            'A formatted string which is used to construct the Verify Access principal name from elements of the introspection response. Claims can be added to the identity string, surrounded by "{}".'
+            oauth_introspection_external_user: typing.Optional[str]
+            'A boolean which is used to indicate whether the mapped identity should correspond to a known Verify Access identity or not.'
+            oauth_introspection_response_attributes: typing.List[Attribute]
+            'A list of rules indicating which parts of the json response should be added to the credential.'
+            static_response_headers: typing.List[Response_Header]
+            'A list of header names and values that should be added to the HTTP response. List of key value pairs eg: ``{"name":"Access-Control-Max-Age", "value":"600"}``'
+            jwt_header_name: typing.Optional[str]
+            'The name of the HTTP header that will contain the JWT.'
+            jwt_certificate: typing.Optional[str]
+            'The label of the personal certificate that will sign the JWT.'
+            jwt_claims: typing.Optional[Claim]
+            'The list of claims to add to the JWT.'
+            junction_hard_limit: str
+            'Defines the hard limit percentage for consumption of worker threads. Valid value is an integer from "0" to "100".'
+            junction_soft_limit: str
+            'Defines the soft limit percentage for consumption of worker threads. Valid value is an integer from "0" to "100".'
+            basic_auth_mode: typing.Optional[str]
+            'Defines how the Reverse Proxy server passes client identity information in HTTP basic authentication (BA) headers to the back-end server. The value is one of: "filter" (default), "ignore", "supply", "gso".'
+            tfim_sso: str
+            'Enables IBM Security Federated Identity Manager single sign-on (SSO) for the junction. Valid value is "yes" or "no".'
+            remote_http_header: typing.Optional[typing.List[str]]
+            'Controls the insertion of Security Verify Access specific client identity information in HTTP headers across the junction. The value is an array containing a combination of: "iv-user", "iv-user-l", "iv-groups", "iv-creds" or "all".'
+            http2_junction: typing.Optional[str]
+            'Specifies whether the junction supports the HTTP/2 protocol. By default, junctions do not support the HTTP/2 protocol. A valid value is "yes" or "no".'
+            http2_proxy: typing.Optional[str]
+            'Specifies whether the junction proxy support the HTTP/2 protocol. By default, junction proxies do not support the HTTP/2 protocol. A valid value is "yes" or "no".'
+            sni_name: typing.Optional[str]
+            'The server name indicator (SNI) to send to TLS junction servers. By default, no SNI is sent.'
+            preserve_cookie: typing.Optional[str]
+            'Specifies whether modifications of the names of non-domain cookies are to be made. Valid value is "yes" or "no".'
+            cookie_include_path: str
+            'Specifies whether script generated server-relative URLs are included in cookies for junction identification. Valid value is "yes" or "no".'
+            transparent_path_junction: str
+            'Specifies whether a transparent path junction is created. Valid value is "yes" or "no".'
+            mutual_auth: str
+            'Specifies whether to enforce mutual authentication between a front-end Reverse Proxy server and a back-end Reverse Proxy server over SSL. Valid value is "yes" or "no".'
+            insert_ltpa_cookies: str
+            'Controls whether LTPA cookies are passed to the junctioned Web server. Valid value is "yes" or "no".'
+            insert_session_cookies: str
+            'Controls whether to send the session cookie to the junctioned Web server. Valid value is "yes" or "no".'
+            request_encoding: str
+            'Specifies the encoding to use when the system generates HTTP headers for junctions. Possible values for encoding are: "utf8_bin", "utf8_uri", "lcp_bin", and "lcp_uri".'
+            enable_basic_auth: str
+            'Specifies whether to use BA header information to authenticate to back-end server. Valid value is "yes" or "no".'
+            key_label: typing.Optional[str]
+            'The key label for the client-side certificate that is used when the system authenticates to the junctioned Web server.'
+            gso_respource_group: typing.Optional[str]
+            'The name of the GSO resource or resource group.'
+            junction_cookie_javascript_block: str
+            'Controls the junction cookie JavaScript block. The value should be one of: "trailer", "inhead", "onfocus", "xhtml10".'
+            client_ip_http: str
+            'Specifies whether to insert the IP address of the incoming request into an HTTP header for transmission to the junctioned Web server. Valid value is "yes" or "no".'
+            version_two_cookies: typing.Optional[str]
+            'Specifies whether LTPA version 2 cookies (LtpaToken2) are used. Valid value is "yes" or "no".'
+            ltpa_keyfile: typing.Optional[str]
+            'Location of the key file that is used to encrypt the LTPA cookie data.'
+            authz_rules: str
+            'Specifies whether to allow denied requests and failure reason information from authorization rules to be sent in the Boolean Rule header (AM_AZN_FAILURE) across the junction. Valid value is "yes" or "no".'
+            fsso_config_file: str
+            'The name of the configuration file that is used for forms based single sign-on.'
+            username: typing.Optional[str]
+            'The Reverse Proxy user name. Used to send BA header information to the back-end server.'
+            password: typing.Optional[str]
+            'The Reverse Proxy password. Used to send BA header information to the back-end server.'
+            local_ip: typing.Optional[str]
+            'Specifies the local IP address that the Reverse Proxy uses when the system communicates with the target back-end server.'
+            query_contents: str
+            'Provides the Reverse Proxy with the correct name of the query_contents program file and where to find the file. By default, the Windows file is called query_contents.exe and the UNIX file is called query_contents.sh.'
+            case_sensitive_url: str
+            'Specifies whether the Reverse Proxy server treats URLs as case sensitive. Valid value is "yes" or "no".'
+            windows_style_url: str
+            'Specifies whether Windows style URLs are supported. Valid value is "yes" or "no".'
+            ltpa_keyfile_password: typing.Optional[str]
+            'Password for the key file that is used to encrypt LTPA cookie data.'
+            https_port: int
+            'HTTPS port of the back-end third-party server. Applicable when the junction type is "ssl".'
+            http_port: int
+            'HTTP port of the back-end third-party server. Applicable when the junction type is "tcp".'
+            proxy_hostname: typing.Optional[str]
+            'The DNS host name or IP address of the proxy server. Applicable when the junction type is "sslproxy".'
+            proxy_port: typing.Optional[int]
+            'The TCP port of the proxy server. Applicable when the junction type is "tcpproxy".'
+            sms_environment: typing.Optional[str]
+            'Only applicable for virtual junctions. Specifies the replica set that sessions on the virtual junction are managed under.'
+            vhost_label: typing.Optional[str]
+            'Only applicable for virtual junctions. Causes a second virtual junction to share the protected object space with the initial virtual junction.'
+            delegation_support: typing.Optional[str]
+            'This option is valid only with junctions that were created with the type of "ssl" or "sslproxy". Indicates single sign-on from a front-end Reverse Proxy server to a back-end Reverse Proxy server.'
+            scripting_support: typing.Optional[str]
+            'Supplies junction identification in a cookie to handle script-generated server-relative URLs. '
+            force: str
+            'Specifies whether to overwrite an existing junction of the same name. Valid value is "yes" or "no".'
+            resources: typing.Optional[typing.List[Resource]]
+            'List of resources to add to resource server.'
+            document_root: typing.Optional[typing.List[str]]
+            'List of documents to upload to the document root.'
+
+        class Authorization_Server(typing.TypedDict):
 
             name: str
             'This is the new instance name, which is a unique name that identifies the instance.'
             hostname: str
             'The host name of the local host. This name is used when constructing the authorization server name.'
             auth_port: int
             'The port on which authorization requests will be received.'
@@ -1604,19 +1707,15 @@
             ssl: str
             'Whether or not to enable SSL between the Security Verify Access authorization server and the LDAP server.'
             ssl_port: str
             'The SSL port on which the LDAP server will be contacted. Only valid if ``ssl`` set to "yes".'
             key_file: str
             'The name of the keyfile that will be used when communicating with the LDAP server over SSL.'
             key_label: str
-            'The label of the certificate within the keyfile to use. '
-            resources: typing.Optional[typing.List[Resource]]
-            'List of resource servers to configure'
-            document_root: typing.Optional[typing.List[str]]
-            'List of documents to upload to the document root.'
+            'The label of the certificate within the keyfile to use.'
 
         class Policy(typing.TypedDict):
             name: str
             'The name of the policy.'
             groups: typing.Optional[typing.List[str]]
             'The groups referenced by this policy. User must be a member of at least one group for this policy to be authorised. The default is no groups if not specified.'
             attributes: typing.Optional[typing.List[str]]
@@ -1636,18 +1735,20 @@
             allowed_methods: typing.Optional[typing.List[str]]
             'Controls the methods permitted in pre-flight requests and the subsequent Access-Control-Allow-Methods header. This option only relates to pre-flight requests handled by the Reverse Proxy and will be ignored if handle_preflight is set to false. Methods are case sensitive and simple methods (ie: GET, HEAD and POST) are always implicitly allowed.'
             allowed_headers: typing.Optional[typing.List[str]]
             'Controls the headers permitted in pre-flight requests and the subsequent Access-Control-Allow-Headers header. This option only relates to pre-flight requests handled by the Reverse Proxy and will be ignored if handle_preflight is set to false.'
             max_age: typing.Optional[int]
             'Controls the Access-Control-Max-Age header added to pre-flight requests. If set to zero, the header will not be added to pre-flight responses. If set to -1, clients will be told not to cache at all. If not present, this value will default to zero.'
 
-        authz_servers: typing.Optional[typing.List[Authorization_Server]]
+        authorization_servers: typing.Optional[typing.List[Authorization_Server]]
         'List of API Authorization servers to create.'
+        resource_servers: typing.Optional[typing.List[Resource_Server]]
+        'List of API Resource servers to create.'
         policies: typing.Optional[typing.List[Policy]]
-        'List of API access control policies to create'
+        'List of API access control policies to create.'
         cors: typing.Optional[typing.List[Cross_Origin_Resource_Sharing]]
         'List of Cross-Origin Resource Sharing policies to create.'
 
 
     def api_access_control(self, runtime, config):
         rsp = self.web.api_access.control.utilities.store_credential(admin_id=runtime.admin_user,
                 admin_pwd=runtime.admin_password, admin_doman=runtime.domain)
@@ -1659,34 +1760,19 @@
 
         if config.policies != None:
             self.__apiac_policies(config.policies)
 
         if config.cors != None:
             self.__apiac_cors(config.cors)
             
-        if config.authz_servers != None:
-            for auth_server in config.authz_servers:
-                rsp = self.web.api_access_control.authz_server.create_server(auth_server.name, hostname=auth_server.hostname,
-                            auth_port=auth_server.auth_port, admin_port=auth_server.admin_port, domain=auth_server.domain,
-                            admin_id="sec_master", admin_pwd=runtime.admin_password, addresses=auth_server.addresses,
-                            ssl=auth_server.ssl, ssl_port=auth_server.ssl_port, keyfile=auth_server.key_file, 
-                            keyfile_label=auth_server.key_label)
-                if rsp.success == True:
-                    _logger.info("Successfully created {} API authorization server".format(auth_server.name))
-                else:
-                    _logger.error("Failed to create the {} API authorization server;\n{}\n{}".format(auth_server.name,
-                                                                            json.dumps(auth_server, indent=4), rsp.content))
-                    continue
-
-                if auth_server.document_root != None:
-                    self.__apiac_document_root(auth_server.document_root)
-
-                if auth_server.resources != None:
-                    self.__apiac_resources(auth_server.resources)
+        if config.authorization_servers != None:
+            self.__apiac_authz_server(runtime, config.authorization_servers)
 
+        if config.resource_servers != None:
+            self.__apiac_resource_server(resourcconfig.resource_serverse_server)
 
 
     def configure(self):
 
         if self.config.webseal == None:
             _logger.info("No WebSEAL configuration detected, skipping")
             return
@@ -1720,19 +1806,19 @@
 
         if websealConfig.runtime != None:
             self.runtime(websealConfig.runtime)
             if websealConfig.reverse_proxy != None:
                 for proxy in websealConfig.reverse_proxy:
                     self.wrp(websealConfig.runtime, proxy)
 
-            if webseal.authroization_servers != None:
-                self.api_access_control(websealConfig.runtime, websealConfig.authroization_server)
-
             if websealConfig.pdadmin != None:
                 self.pdadmin(websealConfig.runtime, websealConfig.pdadmin)
+            
+            if websealConfig.api_access_control != None:
+                self.api_access_control(websealConfig.runtime, websealConfig.api_access_control)
 
         else:
             _logger.info("No runtime configuration detected, unable to set up any reverse proxy config or run pdadmin commands")
 
 
 if __name__ == "__main__":
         configure()
```

### Comparing `verify_access_autoconf-0.1.0/src/verify_access_autoconf.egg-info/SOURCES.txt` & `verify_access_autoconf-0.3.0/src/verify_access_autoconf.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,35 @@
+.deploy.sh
+.gitignore
+.travis.yml
+Dockerfile
 LICENCE.md
 README.md
+dev-requirements.txt
 setup.py
+.github/workflows/main.yaml
+.tests/__init__.py
+.tests/import_test.sh
+.tests/unit_test.sh
+.vscode/settings.json
+docs/Makefile
+docs/access-control.rst
+docs/appliance.rst
+docs/base.rst
+docs/conf.py
+docs/container.rst
+docs/examples.rst
+docs/federations.rst
+docs/index.rst
+docs/make.bat
+docs/webseal.rst
+examples/first_steps.yaml
+examples/hello_world.yaml
+examples/webseal.yaml
+examples/webseal_authsvc_login.yaml
 src/verify_access_autoconf/__init__.py
 src/verify_access_autoconf/__main__.py
 src/verify_access_autoconf/access_control.py
 src/verify_access_autoconf/appliance.py
 src/verify_access_autoconf/configure.py
 src/verify_access_autoconf/container.py
 src/verify_access_autoconf/federation.py
@@ -14,8 +39,9 @@
 src/verify_access_autoconf.egg-info/dependency_links.txt
 src/verify_access_autoconf.egg-info/not-zip-safe
 src/verify_access_autoconf.egg-info/requires.txt
 src/verify_access_autoconf.egg-info/top_level.txt
 src/verify_access_autoconf/util/__init__.py
 src/verify_access_autoconf/util/configure_util.py
 src/verify_access_autoconf/util/constants.py
-src/verify_access_autoconf/util/data_util.py
+src/verify_access_autoconf/util/data_util.py
+templates/config_template.yaml
```

