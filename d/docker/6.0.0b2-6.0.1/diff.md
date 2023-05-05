# Comparing `tmp/docker-6.0.0b2.tar.gz` & `tmp/docker-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-6.0.0b2.tar", last modified: Thu Aug 11 21:29:29 2022, max compression
+gzip compressed data, was "docker-6.0.1.tar", last modified: Wed Nov  2 19:42:18 2022, max compression
```

## Comparing `docker-6.0.0b2.tar` & `docker-6.0.1.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.821933 docker-6.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (122)      118 2022-08-11 21:29:22.000000 docker-6.0.0b2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)      121 2022-08-11 21:29:22.000000 docker-6.0.0b2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      208 2022-08-11 21:29:22.000000 docker-6.0.0b2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.797933 docker-6.0.0b2/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      188 2022-08-11 21:29:22.000000 docker-6.0.0b2/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.797933 docker-6.0.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2022-08-11 21:29:22.000000 docker-6.0.0b2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2022-08-11 21:29:22.000000 docker-6.0.0b2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)      164 2022-08-11 21:29:22.000000 docker-6.0.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      212 2022-08-11 21:29:22.000000 docker-6.0.0b2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4736 2022-08-11 21:29:22.000000 docker-6.0.0b2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)      361 2022-08-11 21:29:22.000000 docker-6.0.0b2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)      310 2022-08-11 21:29:22.000000 docker-6.0.0b2/Dockerfile-docs
--rw-r--r--   0 runner    (1001) docker     (122)     5081 2022-08-11 21:29:22.000000 docker-6.0.0b2/Jenkinsfile
--rw-r--r--   0 runner    (1001) docker     (122)    10758 2022-08-11 21:29:22.000000 docker-6.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1601 2022-08-11 21:29:22.000000 docker-6.0.0b2/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (122)      259 2022-08-11 21:29:22.000000 docker-6.0.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4612 2022-08-11 21:29:22.000000 docker-6.0.0b2/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     3177 2022-08-11 21:29:29.821933 docker-6.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2022-08-11 21:29:22.000000 docker-6.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.797933 docker-6.0.0b2/docker/
--rw-r--r--   0 runner    (1001) docker     (122)      228 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      178 2022-08-11 21:29:29.000000 docker-6.0.0b2/docker/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.801933 docker-6.0.0b2/docker/api/
--rw-r--r--   0 runner    (1001) docker     (122)       45 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14667 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/api/build.py
--rw-r--r--   0 runner    (1001) docker     (122)    18831 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/api/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     2706 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/api/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    51452 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/api/container.py
--rw-r--r--   0 runner    (1001) docker     (122)     6008 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/api/daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     5894 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/api/exec_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    20255 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/api/image.py
--rw-r--r--   0 runner    (1001) docker     (122)    10476 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/api/network.py
--rw-r--r--   0 runner    (1001) docker     (122)     8982 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/api/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2883 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/api/secret.py
--rw-r--r--   0 runner    (1001) docker     (122)    18863 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/api/service.py
--rw-r--r--   0 runner    (1001) docker     (122)    17561 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/api/swarm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5133 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/api/volume.py
--rw-r--r--   0 runner    (1001) docker     (122)    13241 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     7832 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.801933 docker-6.0.0b2/docker/context/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6433 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/context/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2149 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/context/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     7906 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.801933 docker-6.0.0b2/docker/credentials/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      142 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/credentials/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      573 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/credentials/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     3229 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/credentials/store.py
--rw-r--r--   0 runner    (1001) docker     (122)      224 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/credentials/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5344 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.805933 docker-6.0.0b2/docker/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/models/configs.py
--rw-r--r--   0 runner    (1001) docker     (122)    45178 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/models/containers.py
--rw-r--r--   0 runner    (1001) docker     (122)    18010 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/models/images.py
--rw-r--r--   0 runner    (1001) docker     (122)     7963 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/models/networks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2928 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/models/nodes.py
--rw-r--r--   0 runner    (1001) docker     (122)     5970 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/models/plugins.py
--rw-r--r--   0 runner    (1001) docker     (122)     2611 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (122)     1845 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)    13680 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/models/services.py
--rw-r--r--   0 runner    (1001) docker     (122)     7986 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/models/swarm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2848 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/models/volumes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3267 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/tls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.805933 docker-6.0.0b2/docker/transport/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/transport/basehttpadapter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3589 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/transport/npipeconn.py
--rw-r--r--   0 runner    (1001) docker     (122)     5723 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/transport/npipesocket.py
--rw-r--r--   0 runner    (1001) docker     (122)     7986 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/transport/sshconn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2249 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/transport/ssladapter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3201 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/transport/unixconn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.805933 docker-6.0.0b2/docker/types/
--rw-r--r--   0 runner    (1001) docker     (122)      595 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      110 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/types/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    27481 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/types/containers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/types/daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     2776 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/types/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (122)     3954 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/types/networks.py
--rw-r--r--   0 runner    (1001) docker     (122)    32872 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/types/services.py
--rw-r--r--   0 runner    (1001) docker     (122)     4653 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/types/swarm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.805933 docker-6.0.0b2/docker/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      606 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8019 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/utils/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     1724 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1547 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3295 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/utils/fnmatch.py
--rw-r--r--   0 runner    (1001) docker     (122)     2178 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/utils/json_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     2800 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/utils/ports.py
--rw-r--r--   0 runner    (1001) docker     (122)     2203 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (122)     4370 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/utils/socket.py
--rw-r--r--   0 runner    (1001) docker     (122)    13741 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      536 2022-08-11 21:29:22.000000 docker-6.0.0b2/docker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.797933 docker-6.0.0b2/docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3177 2022-08-11 21:29:29.000000 docker-6.0.0b2/docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5516 2022-08-11 21:29:29.000000 docker-6.0.0b2/docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-08-11 21:29:29.000000 docker-6.0.0b2/docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-08-11 21:29:29.000000 docker-6.0.0b2/docker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      145 2022-08-11 21:29:29.000000 docker-6.0.0b2/docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2022-08-11 21:29:29.000000 docker-6.0.0b2/docker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.809933 docker-6.0.0b2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.809933 docker-6.0.0b2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.809933 docker-6.0.0b2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (122)     3073 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)    75067 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/change-log.md
--rw-r--r--   0 runner    (1001) docker     (122)      920 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/client.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10281 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      505 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/configs.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/containers.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1475 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/favicon_whale.png
--rw-r--r--   0 runner    (1001) docker     (122)     1089 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/images.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2212 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      792 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/networks.rst
--rw-r--r--   0 runner    (1001) docker     (122)      615 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/nodes.rst
--rw-r--r--   0 runner    (1001) docker     (122)      723 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (122)      505 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/secrets.rst
--rw-r--r--   0 runner    (1001) docker     (122)      919 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/services.rst
--rw-r--r--   0 runner    (1001) docker     (122)      754 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/swarm.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1168 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/tls.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.809933 docker-6.0.0b2/docs/user_guides/
--rw-r--r--   0 runner    (1001) docker     (122)      110 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/user_guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/user_guides/multiplex.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/user_guides/swarm_services.md
--rw-r--r--   0 runner    (1001) docker     (122)      559 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs/volumes.rst
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-08-11 21:29:22.000000 docker-6.0.0b2/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      129 2022-08-11 21:29:22.000000 docker-6.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       87 2022-08-11 21:29:22.000000 docker-6.0.0b2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (122)      129 2022-08-11 21:29:22.000000 docker-6.0.0b2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.809933 docker-6.0.0b2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (122)      938 2022-08-11 21:29:22.000000 docker-6.0.0b2/scripts/release.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     2186 2022-08-11 21:29:22.000000 docker-6.0.0b2/scripts/versions.py
--rw-r--r--   0 runner    (1001) docker     (122)      109 2022-08-11 21:29:29.821933 docker-6.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2596 2022-08-11 21:29:22.000000 docker-6.0.0b2/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2022-08-11 21:29:22.000000 docker-6.0.0b2/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.809933 docker-6.0.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1725 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/Dockerfile-dind-certs
--rw-r--r--   0 runner    (1001) docker     (122)      439 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/Dockerfile-ssh-dind
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.809933 docker-6.0.0b2/tests/gpg-keys/
--rw-r--r--   0 runner    (1001) docker     (122)      166 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/gpg-keys/ownertrust
--rw-r--r--   0 runner    (1001) docker     (122)      966 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/gpg-keys/secret
--rw-r--r--   0 runner    (1001) docker     (122)     4087 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.813933 docker-6.0.0b2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20173 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/api_build_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/api_client_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2831 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/api_config_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    55983 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/api_container_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    11874 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/api_exec_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/api_healthcheck_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    12867 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/api_image_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    18361 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/api_network_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5134 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/api_plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2302 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/api_secret_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    60914 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/api_service_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     9408 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/api_swarm_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2307 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/api_volume_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3997 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1201 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/client_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      771 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/context_api_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.813933 docker-6.0.0b2/tests/integration/credentials/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      227 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/credentials/create_gpg_key.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/credentials/store_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      485 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/credentials/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      634 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    17859 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/models_containers_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5830 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/models_images_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/models_networks_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/models_nodes_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      613 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/models_resources_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    13199 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/models_services_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1619 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/models_swarm_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1106 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/models_volumes_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2245 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/regression_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.793933 docker-6.0.0b2/tests/integration/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.813933 docker-6.0.0b2/tests/integration/testdata/dummy-plugin/
--rw-r--r--   0 runner    (1001) docker     (122)      420 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/testdata/dummy-plugin/config.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.793933 docker-6.0.0b2/tests/integration/testdata/dummy-plugin/rootfs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.813933 docker-6.0.0b2/tests/integration/testdata/dummy-plugin/rootfs/dummy/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/integration/testdata/dummy-plugin/rootfs/dummy/file.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.813933 docker-6.0.0b2/tests/ssh/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19725 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/ssh/api_build_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4261 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/ssh/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.793933 docker-6.0.0b2/tests/ssh/config/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.817933 docker-6.0.0b2/tests/ssh/config/client/
--rw-r--r--   0 runner    (1001) docker     (122)     2578 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/ssh/config/client/id_rsa
--rw-r--r--   0 runner    (1001) docker     (122)      554 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/ssh/config/client/id_rsa.pub
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.817933 docker-6.0.0b2/tests/ssh/config/server/
--rw-r--r--   0 runner    (1001) docker     (122)      411 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/ssh/config/server/known_ed25519
--rw-r--r--   0 runner    (1001) docker     (122)      115 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/ssh/config/server/known_ed25519.pub
--rw-r--r--   0 runner    (1001) docker     (122)       70 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/ssh/config/server/sshd_config
--rw-r--r--   0 runner    (1001) docker     (122)      411 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/ssh/config/server/unknown_ed25519
--rw-r--r--   0 runner    (1001) docker     (122)      117 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/ssh/config/server/unknown_ed25519.pub
--rw-r--r--   0 runner    (1001) docker     (122)      753 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/ssh/connect_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.821933 docker-6.0.0b2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7162 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/api_build_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    56938 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/api_container_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2396 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/api_exec_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    10949 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/api_image_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5667 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/api_network_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    21964 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/api_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3886 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/api_volume_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    28287 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/auth_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    10083 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/client_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/context_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    18285 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/dockertypes_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5532 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    17894 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/fake_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2425 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/fake_api_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3757 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/fake_stat.py
--rw-r--r--   0 runner    (1001) docker     (122)    21812 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/models_containers_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5925 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/models_images_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2176 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/models_networks_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      873 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/models_resources_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      362 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/models_secrets_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2385 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/models_services_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1143 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/sshadapter_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2443 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/ssladapter_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2150 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/swarm_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.793933 docker-6.0.0b2/tests/unit/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:29.821933 docker-6.0.0b2/tests/unit/testdata/certs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/testdata/certs/ca.pem
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/testdata/certs/cert.pem
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/testdata/certs/key.pem
--rw-r--r--   0 runner    (1001) docker     (122)      186 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/types_containers_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    16046 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/utils_build_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4035 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/utils_config_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/utils_json_stream_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2784 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/utils_proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    23196 2022-08-11 21:29:22.000000 docker-6.0.0b2/tests/unit/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      324 2022-08-11 21:29:22.000000 docker-6.0.0b2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.708934 docker-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2022-11-02 19:42:12.000000 docker-6.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2022-11-02 19:42:12.000000 docker-6.0.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2022-11-02 19:42:12.000000 docker-6.0.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.684933 docker-6.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2022-11-02 19:42:12.000000 docker-6.0.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.684933 docker-6.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2022-11-02 19:42:12.000000 docker-6.0.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2022-11-02 19:42:12.000000 docker-6.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2022-11-02 19:42:12.000000 docker-6.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2022-11-02 19:42:12.000000 docker-6.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4736 2022-11-02 19:42:12.000000 docker-6.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2022-11-02 19:42:12.000000 docker-6.0.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2022-11-02 19:42:12.000000 docker-6.0.1/Dockerfile-docs
+-rw-r--r--   0 runner    (1001) docker     (122)     5081 2022-11-02 19:42:12.000000 docker-6.0.1/Jenkinsfile
+-rw-r--r--   0 runner    (1001) docker     (122)    10758 2022-11-02 19:42:12.000000 docker-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2022-11-02 19:42:12.000000 docker-6.0.1/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2022-11-02 19:42:12.000000 docker-6.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4612 2022-11-02 19:42:12.000000 docker-6.0.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2022-11-02 19:42:18.708934 docker-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2022-11-02 19:42:12.000000 docker-6.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.688933 docker-6.0.1/docker/
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2022-11-02 19:42:12.000000 docker-6.0.1/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2022-11-02 19:42:18.000000 docker-6.0.1/docker/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.692933 docker-6.0.1/docker/api/
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2022-11-02 19:42:12.000000 docker-6.0.1/docker/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14667 2022-11-02 19:42:12.000000 docker-6.0.1/docker/api/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18831 2022-11-02 19:42:12.000000 docker-6.0.1/docker/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2706 2022-11-02 19:42:12.000000 docker-6.0.1/docker/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51761 2022-11-02 19:42:12.000000 docker-6.0.1/docker/api/container.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6008 2022-11-02 19:42:12.000000 docker-6.0.1/docker/api/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5894 2022-11-02 19:42:12.000000 docker-6.0.1/docker/api/exec_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20255 2022-11-02 19:42:12.000000 docker-6.0.1/docker/api/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10691 2022-11-02 19:42:12.000000 docker-6.0.1/docker/api/network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8982 2022-11-02 19:42:12.000000 docker-6.0.1/docker/api/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2883 2022-11-02 19:42:12.000000 docker-6.0.1/docker/api/secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18863 2022-11-02 19:42:12.000000 docker-6.0.1/docker/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18116 2022-11-02 19:42:12.000000 docker-6.0.1/docker/api/swarm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5133 2022-11-02 19:42:12.000000 docker-6.0.1/docker/api/volume.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13241 2022-11-02 19:42:12.000000 docker-6.0.1/docker/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7832 2022-11-02 19:42:12.000000 docker-6.0.1/docker/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2022-11-02 19:42:12.000000 docker-6.0.1/docker/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.692933 docker-6.0.1/docker/context/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2022-11-02 19:42:12.000000 docker-6.0.1/docker/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6433 2022-11-02 19:42:12.000000 docker-6.0.1/docker/context/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2149 2022-11-02 19:42:12.000000 docker-6.0.1/docker/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7906 2022-11-02 19:42:12.000000 docker-6.0.1/docker/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.692933 docker-6.0.1/docker/credentials/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2022-11-02 19:42:12.000000 docker-6.0.1/docker/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2022-11-02 19:42:12.000000 docker-6.0.1/docker/credentials/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2022-11-02 19:42:12.000000 docker-6.0.1/docker/credentials/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2022-11-02 19:42:12.000000 docker-6.0.1/docker/credentials/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2022-11-02 19:42:12.000000 docker-6.0.1/docker/credentials/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5344 2022-11-02 19:42:12.000000 docker-6.0.1/docker/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.692933 docker-6.0.1/docker/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:12.000000 docker-6.0.1/docker/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2022-11-02 19:42:12.000000 docker-6.0.1/docker/models/configs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45259 2022-11-02 19:42:12.000000 docker-6.0.1/docker/models/containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18010 2022-11-02 19:42:12.000000 docker-6.0.1/docker/models/images.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7963 2022-11-02 19:42:12.000000 docker-6.0.1/docker/models/networks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2928 2022-11-02 19:42:12.000000 docker-6.0.1/docker/models/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5970 2022-11-02 19:42:12.000000 docker-6.0.1/docker/models/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2611 2022-11-02 19:42:12.000000 docker-6.0.1/docker/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1845 2022-11-02 19:42:12.000000 docker-6.0.1/docker/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13799 2022-11-02 19:42:12.000000 docker-6.0.1/docker/models/services.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8289 2022-11-02 19:42:12.000000 docker-6.0.1/docker/models/swarm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2848 2022-11-02 19:42:12.000000 docker-6.0.1/docker/models/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3267 2022-11-02 19:42:12.000000 docker-6.0.1/docker/tls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.696934 docker-6.0.1/docker/transport/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2022-11-02 19:42:12.000000 docker-6.0.1/docker/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2022-11-02 19:42:12.000000 docker-6.0.1/docker/transport/basehttpadapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3589 2022-11-02 19:42:12.000000 docker-6.0.1/docker/transport/npipeconn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5723 2022-11-02 19:42:12.000000 docker-6.0.1/docker/transport/npipesocket.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7986 2022-11-02 19:42:12.000000 docker-6.0.1/docker/transport/sshconn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2249 2022-11-02 19:42:12.000000 docker-6.0.1/docker/transport/ssladapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3201 2022-11-02 19:42:12.000000 docker-6.0.1/docker/transport/unixconn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.696934 docker-6.0.1/docker/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2022-11-02 19:42:12.000000 docker-6.0.1/docker/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2022-11-02 19:42:12.000000 docker-6.0.1/docker/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27481 2022-11-02 19:42:12.000000 docker-6.0.1/docker/types/containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2022-11-02 19:42:12.000000 docker-6.0.1/docker/types/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2776 2022-11-02 19:42:12.000000 docker-6.0.1/docker/types/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4240 2022-11-02 19:42:12.000000 docker-6.0.1/docker/types/networks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33158 2022-11-02 19:42:12.000000 docker-6.0.1/docker/types/services.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4653 2022-11-02 19:42:12.000000 docker-6.0.1/docker/types/swarm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.696934 docker-6.0.1/docker/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      606 2022-11-02 19:42:12.000000 docker-6.0.1/docker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8019 2022-11-02 19:42:12.000000 docker-6.0.1/docker/utils/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1724 2022-11-02 19:42:12.000000 docker-6.0.1/docker/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1547 2022-11-02 19:42:12.000000 docker-6.0.1/docker/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3295 2022-11-02 19:42:12.000000 docker-6.0.1/docker/utils/fnmatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2178 2022-11-02 19:42:12.000000 docker-6.0.1/docker/utils/json_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2800 2022-11-02 19:42:12.000000 docker-6.0.1/docker/utils/ports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2203 2022-11-02 19:42:12.000000 docker-6.0.1/docker/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4881 2022-11-02 19:42:12.000000 docker-6.0.1/docker/utils/socket.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13741 2022-11-02 19:42:12.000000 docker-6.0.1/docker/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2022-11-02 19:42:12.000000 docker-6.0.1/docker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.688933 docker-6.0.1/docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2022-11-02 19:42:18.000000 docker-6.0.1/docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5516 2022-11-02 19:42:18.000000 docker-6.0.1/docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-02 19:42:18.000000 docker-6.0.1/docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-02 19:42:18.000000 docker-6.0.1/docker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2022-11-02 19:42:18.000000 docker-6.0.1/docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2022-11-02 19:42:18.000000 docker-6.0.1/docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.700934 docker-6.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.700934 docker-6.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2022-11-02 19:42:12.000000 docker-6.0.1/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.700934 docker-6.0.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2022-11-02 19:42:12.000000 docker-6.0.1/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3073 2022-11-02 19:42:12.000000 docker-6.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    75067 2022-11-02 19:42:12.000000 docker-6.0.1/docs/change-log.md
+-rw-r--r--   0 runner    (1001) docker     (122)      920 2022-11-02 19:42:12.000000 docker-6.0.1/docs/client.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10281 2022-11-02 19:42:12.000000 docker-6.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2022-11-02 19:42:12.000000 docker-6.0.1/docs/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2022-11-02 19:42:12.000000 docker-6.0.1/docs/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1475 2022-11-02 19:42:12.000000 docker-6.0.1/docs/favicon_whale.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2022-11-02 19:42:12.000000 docker-6.0.1/docs/images.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2212 2022-11-02 19:42:12.000000 docker-6.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2022-11-02 19:42:12.000000 docker-6.0.1/docs/networks.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2022-11-02 19:42:12.000000 docker-6.0.1/docs/nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2022-11-02 19:42:12.000000 docker-6.0.1/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2022-11-02 19:42:12.000000 docker-6.0.1/docs/secrets.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      919 2022-11-02 19:42:12.000000 docker-6.0.1/docs/services.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2022-11-02 19:42:12.000000 docker-6.0.1/docs/swarm.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1168 2022-11-02 19:42:12.000000 docker-6.0.1/docs/tls.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.700934 docker-6.0.1/docs/user_guides/
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2022-11-02 19:42:12.000000 docker-6.0.1/docs/user_guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2022-11-02 19:42:12.000000 docker-6.0.1/docs/user_guides/multiplex.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2022-11-02 19:42:12.000000 docker-6.0.1/docs/user_guides/swarm_services.md
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2022-11-02 19:42:12.000000 docker-6.0.1/docs/volumes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2022-11-02 19:42:12.000000 docker-6.0.1/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2022-11-02 19:42:12.000000 docker-6.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2022-11-02 19:42:12.000000 docker-6.0.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2022-11-02 19:42:12.000000 docker-6.0.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.700934 docker-6.0.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      938 2022-11-02 19:42:12.000000 docker-6.0.1/scripts/release.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2186 2022-11-02 19:42:12.000000 docker-6.0.1/scripts/versions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2022-11-02 19:42:18.708934 docker-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2596 2022-11-02 19:42:12.000000 docker-6.0.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2022-11-02 19:42:12.000000 docker-6.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.700934 docker-6.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1723 2022-11-02 19:42:12.000000 docker-6.0.1/tests/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2022-11-02 19:42:12.000000 docker-6.0.1/tests/Dockerfile-dind-certs
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-02 19:42:12.000000 docker-6.0.1/tests/Dockerfile-ssh-dind
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:12.000000 docker-6.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.700934 docker-6.0.1/tests/gpg-keys/
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2022-11-02 19:42:12.000000 docker-6.0.1/tests/gpg-keys/ownertrust
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2022-11-02 19:42:12.000000 docker-6.0.1/tests/gpg-keys/secret
+-rw-r--r--   0 runner    (1001) docker     (122)     4087 2022-11-02 19:42:12.000000 docker-6.0.1/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.704934 docker-6.0.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20173 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/api_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/api_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2831 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/api_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56459 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/api_container_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11874 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/api_exec_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/api_healthcheck_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12867 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/api_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18933 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/api_network_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5134 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/api_plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2302 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/api_secret_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61793 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/api_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9608 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/api_swarm_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2281 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/api_volume_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3997 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/context_api_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.704934 docker-6.0.1/tests/integration/credentials/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/credentials/create_gpg_key.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/credentials/store_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      485 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/credentials/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17859 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/models_containers_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5830 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/models_images_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/models_networks_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/models_nodes_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/models_resources_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13199 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/models_services_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1619 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/models_swarm_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1106 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/models_volumes_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2245 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/regression_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.680933 docker-6.0.1/tests/integration/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.704934 docker-6.0.1/tests/integration/testdata/dummy-plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)      420 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/testdata/dummy-plugin/config.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.680933 docker-6.0.1/tests/integration/testdata/dummy-plugin/rootfs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.704934 docker-6.0.1/tests/integration/testdata/dummy-plugin/rootfs/dummy/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:12.000000 docker-6.0.1/tests/integration/testdata/dummy-plugin/rootfs/dummy/file.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.704934 docker-6.0.1/tests/ssh/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:12.000000 docker-6.0.1/tests/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19725 2022-11-02 19:42:12.000000 docker-6.0.1/tests/ssh/api_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4261 2022-11-02 19:42:12.000000 docker-6.0.1/tests/ssh/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.680933 docker-6.0.1/tests/ssh/config/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.704934 docker-6.0.1/tests/ssh/config/client/
+-rw-r--r--   0 runner    (1001) docker     (122)     2578 2022-11-02 19:42:12.000000 docker-6.0.1/tests/ssh/config/client/id_rsa
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2022-11-02 19:42:12.000000 docker-6.0.1/tests/ssh/config/client/id_rsa.pub
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.704934 docker-6.0.1/tests/ssh/config/server/
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2022-11-02 19:42:12.000000 docker-6.0.1/tests/ssh/config/server/known_ed25519
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2022-11-02 19:42:12.000000 docker-6.0.1/tests/ssh/config/server/known_ed25519.pub
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2022-11-02 19:42:12.000000 docker-6.0.1/tests/ssh/config/server/sshd_config
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2022-11-02 19:42:12.000000 docker-6.0.1/tests/ssh/config/server/unknown_ed25519
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2022-11-02 19:42:12.000000 docker-6.0.1/tests/ssh/config/server/unknown_ed25519.pub
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2022-11-02 19:42:12.000000 docker-6.0.1/tests/ssh/connect_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.708934 docker-6.0.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7162 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/api_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58335 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/api_container_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2396 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/api_exec_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10949 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/api_image_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5667 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/api_network_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21964 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3886 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/api_volume_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28287 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10083 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/context_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18285 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/dockertypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5532 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17894 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/fake_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2425 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/fake_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3757 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/fake_stat.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21812 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/models_containers_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5925 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/models_images_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/models_networks_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      873 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/models_resources_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      362 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/models_secrets_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2435 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/models_services_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/sshadapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2443 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/ssladapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2150 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/swarm_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.680933 docker-6.0.1/tests/unit/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:18.708934 docker-6.0.1/tests/unit/testdata/certs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/testdata/certs/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/testdata/certs/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/testdata/certs/key.pem
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/types_containers_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16046 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/utils_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4035 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/utils_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/utils_json_stream_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2784 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/utils_proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23196 2022-11-02 19:42:12.000000 docker-6.0.1/tests/unit/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2022-11-02 19:42:12.000000 docker-6.0.1/tox.ini
```

### Comparing `docker-6.0.0b2/.github/workflows/ci.yml` & `docker-6.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/.github/workflows/release.yml` & `docker-6.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/CONTRIBUTING.md` & `docker-6.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/Jenkinsfile` & `docker-6.0.1/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/LICENSE` & `docker-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/MAINTAINERS` & `docker-6.0.1/MAINTAINERS`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/Makefile` & `docker-6.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/PKG-INFO` & `docker-6.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker
-Version: 6.0.0b2
+Version: 6.0.1
 Summary: A Python library for the Docker Engine API.
 Home-page: https://github.com/docker/docker-py
 Maintainer: Ulysses Souza
 Maintainer-email: ulysses.souza@docker.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docker-py.readthedocs.io
 Project-URL: Changelog, https://docker-py.readthedocs.io/en/stable/change-log.html
```

### Comparing `docker-6.0.0b2/README.md` & `docker-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/api/build.py` & `docker-6.0.1/docker/api/build.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/api/client.py` & `docker-6.0.1/docker/api/client.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/api/config.py` & `docker-6.0.1/docker/api/config.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/api/container.py` & `docker-6.0.1/docker/api/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -822,19 +822,20 @@
             stdout (bool): Get ``STDOUT``. Default ``True``
             stderr (bool): Get ``STDERR``. Default ``True``
             stream (bool): Stream the response. Default ``False``
             timestamps (bool): Show timestamps. Default ``False``
             tail (str or int): Output specified number of lines at the end of
                 logs. Either an integer of number of lines or the string
                 ``all``. Default ``all``
-            since (datetime or int): Show logs since a given datetime or
-                integer epoch (in seconds)
+            since (datetime, int, or float): Show logs since a given datetime,
+                integer epoch (in seconds) or float (in fractional seconds)
             follow (bool): Follow log output. Default ``False``
-            until (datetime or int): Show logs that occurred before the given
-                datetime or integer epoch (in seconds)
+            until (datetime, int, or float): Show logs that occurred before
+                the given datetime, integer epoch (in seconds), or
+                float (in fractional seconds)
 
         Returns:
             (generator or str)
 
         Raises:
             :py:class:`docker.errors.APIError`
                 If the server returns an error.
@@ -851,32 +852,36 @@
         params['tail'] = tail
 
         if since is not None:
             if isinstance(since, datetime):
                 params['since'] = utils.datetime_to_timestamp(since)
             elif (isinstance(since, int) and since > 0):
                 params['since'] = since
+            elif (isinstance(since, float) and since > 0.0):
+                params['since'] = since
             else:
                 raise errors.InvalidArgument(
-                    'since value should be datetime or positive int, '
+                    'since value should be datetime or positive int/float, '
                     'not {}'.format(type(since))
                 )
 
         if until is not None:
             if utils.version_lt(self._version, '1.35'):
                 raise errors.InvalidVersion(
                     'until is not supported for API version < 1.35'
                 )
             if isinstance(until, datetime):
                 params['until'] = utils.datetime_to_timestamp(until)
             elif (isinstance(until, int) and until > 0):
                 params['until'] = until
+            elif (isinstance(until, float) and until > 0.0):
+                params['until'] = until
             else:
                 raise errors.InvalidArgument(
-                    'until value should be datetime or positive int, '
+                    'until value should be datetime or positive int/float, '
                     'not {}'.format(type(until))
                 )
 
         url = self._url("/containers/{0}/logs", container)
         res = self._get(url, params=params, stream=stream)
         output = self._get_result(container, stream, res)
```

### Comparing `docker-6.0.0b2/docker/api/daemon.py` & `docker-6.0.1/docker/api/daemon.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/api/exec_api.py` & `docker-6.0.1/docker/api/exec_api.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/api/image.py` & `docker-6.0.1/docker/api/image.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/api/network.py` & `docker-6.0.1/docker/api/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,15 +212,16 @@
         res = self._get(url, params=params)
         return self._result(res, json=True)
 
     @check_resource('container')
     def connect_container_to_network(self, container, net_id,
                                      ipv4_address=None, ipv6_address=None,
                                      aliases=None, links=None,
-                                     link_local_ips=None, driver_opt=None):
+                                     link_local_ips=None, driver_opt=None,
+                                     mac_address=None):
         """
         Connect a container to a network.
 
         Args:
             container (str): container-id/name to be connected to the network
             net_id (str): network id
             aliases (:py:class:`list`): A list of aliases for this endpoint.
@@ -231,21 +232,24 @@
                 container. Defaults to ``None``.
             ipv4_address (str): The IP address of this container on the
                 network, using the IPv4 protocol. Defaults to ``None``.
             ipv6_address (str): The IP address of this container on the
                 network, using the IPv6 protocol. Defaults to ``None``.
             link_local_ips (:py:class:`list`): A list of link-local
                 (IPv4/IPv6) addresses.
+            mac_address (str): The MAC address of this container on the
+                network. Defaults to ``None``.
         """
         data = {
             "Container": container,
             "EndpointConfig": self.create_endpoint_config(
                 aliases=aliases, links=links, ipv4_address=ipv4_address,
                 ipv6_address=ipv6_address, link_local_ips=link_local_ips,
-                driver_opt=driver_opt
+                driver_opt=driver_opt,
+                mac_address=mac_address
             ),
         }
 
         url = self._url("/networks/{0}/connect", net_id)
         res = self._post_json(url, data=data)
         self._raise_for_status(res)
```

### Comparing `docker-6.0.0b2/docker/api/plugin.py` & `docker-6.0.1/docker/api/plugin.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/api/secret.py` & `docker-6.0.1/docker/api/secret.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/api/service.py` & `docker-6.0.1/docker/api/service.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/api/swarm.py` & `docker-6.0.1/docker/api/swarm.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         """
         return self._result(self._get(self._url('/swarm/unlockkey')), True)
 
     @utils.minimum_version('1.24')
     def init_swarm(self, advertise_addr=None, listen_addr='0.0.0.0:2377',
                    force_new_cluster=False, swarm_spec=None,
                    default_addr_pool=None, subnet_size=None,
-                   data_path_addr=None):
+                   data_path_addr=None, data_path_port=None):
         """
         Initialize a new Swarm using the current connected engine as the first
         node.
 
         Args:
             advertise_addr (string): Externally reachable address advertised
                 to other nodes. This can either be an address/port combination
@@ -114,14 +114,17 @@
                 default subnet pools for global scope networks. Each pool
                 should be specified as a CIDR block, like '10.0.0.0/8'.
                 Default: None
             subnet_size (int): SubnetSize specifies the subnet size of the
                 networks created from the default subnet pool. Default: None
             data_path_addr (string): Address or interface to use for data path
                 traffic. For example, 192.168.1.1, or an interface, like eth0.
+            data_path_port (int): Port number to use for data path traffic.
+                Acceptable port range is 1024 to 49151. If set to ``None`` or
+                0, the default port 4789 will be used. Default: None
 
         Returns:
             (str): The ID of the created node.
 
         Raises:
             :py:class:`docker.errors.APIError`
                 If the server returns an error.
@@ -162,14 +165,22 @@
             if utils.version_lt(self._version, '1.30'):
                 raise errors.InvalidVersion(
                     'Data address path is only available for '
                     'API version >= 1.30'
                 )
             data['DataPathAddr'] = data_path_addr
 
+        if data_path_port is not None:
+            if utils.version_lt(self._version, '1.40'):
+                raise errors.InvalidVersion(
+                    'Data path port is only available for '
+                    'API version >= 1.40'
+                )
+            data['DataPathPort'] = data_path_port
+
         response = self._post_json(url, data=data)
         return self._result(response, json=True)
 
     @utils.minimum_version('1.24')
     def inspect_swarm(self):
         """
         Retrieve low-level information about the current swarm.
```

### Comparing `docker-6.0.0b2/docker/api/volume.py` & `docker-6.0.1/docker/api/volume.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/auth.py` & `docker-6.0.1/docker/auth.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/client.py` & `docker-6.0.1/docker/client.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/constants.py` & `docker-6.0.1/docker/constants.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/context/api.py` & `docker-6.0.1/docker/context/api.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/context/config.py` & `docker-6.0.1/docker/context/config.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/context/context.py` & `docker-6.0.1/docker/context/context.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/credentials/errors.py` & `docker-6.0.1/docker/credentials/errors.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/credentials/store.py` & `docker-6.0.1/docker/credentials/store.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/errors.py` & `docker-6.0.1/docker/errors.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/models/configs.py` & `docker-6.0.1/docker/models/configs.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/models/containers.py` & `docker-6.0.1/docker/models/containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,19 +286,20 @@
             stdout (bool): Get ``STDOUT``. Default ``True``
             stderr (bool): Get ``STDERR``. Default ``True``
             stream (bool): Stream the response. Default ``False``
             timestamps (bool): Show timestamps. Default ``False``
             tail (str or int): Output specified number of lines at the end of
                 logs. Either an integer of number of lines or the string
                 ``all``. Default ``all``
-            since (datetime or int): Show logs since a given datetime or
-                integer epoch (in seconds)
+            since (datetime, int, or float): Show logs since a given datetime,
+                integer epoch (in seconds) or float (in nanoseconds)
             follow (bool): Follow log output. Default ``False``
-            until (datetime or int): Show logs that occurred before the given
-                datetime or integer epoch (in seconds)
+            until (datetime, int, or float): Show logs that occurred before
+                the given datetime, integer epoch (in seconds), or
+                float (in nanoseconds)
 
         Returns:
             (generator or str): Logs from the container.
 
         Raises:
             :py:class:`docker.errors.APIError`
                 If the server returns an error.
```

### Comparing `docker-6.0.0b2/docker/models/images.py` & `docker-6.0.1/docker/models/images.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/models/networks.py` & `docker-6.0.1/docker/models/networks.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/models/nodes.py` & `docker-6.0.1/docker/models/nodes.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/models/plugins.py` & `docker-6.0.1/docker/models/plugins.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/models/resource.py` & `docker-6.0.1/docker/models/resource.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/models/secrets.py` & `docker-6.0.1/docker/models/secrets.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/models/services.py` & `docker-6.0.1/docker/models/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,14 +213,16 @@
                 to the service.
             privileges (Privileges): Security options for the service's
                 containers.
             cap_add (:py:class:`list`): A list of kernel capabilities to add to
                 the default set for the container.
             cap_drop (:py:class:`list`): A list of kernel capabilities to drop
                 from the default set for the container.
+            sysctls (:py:class:`dict`): A dict of sysctl values to add to the
+                container
 
         Returns:
             :py:class:`Service`: The created service.
 
         Raises:
             :py:class:`docker.errors.APIError`
                 If the server returns an error.
@@ -301,14 +303,15 @@
     'read_only',
     'secrets',
     'stop_grace_period',
     'stop_signal',
     'tty',
     'user',
     'workdir',
+    'sysctls',
 ]
 
 # kwargs to copy straight over to TaskTemplate
 TASK_TEMPLATE_KWARGS = [
     'networks',
     'resources',
     'restart_policy',
```

### Comparing `docker-6.0.0b2/docker/models/swarm.py` & `docker-6.0.1/docker/models/swarm.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 
     def get_unlock_key(self):
         return self.client.api.get_unlock_key()
     get_unlock_key.__doc__ = APIClient.get_unlock_key.__doc__
 
     def init(self, advertise_addr=None, listen_addr='0.0.0.0:2377',
              force_new_cluster=False, default_addr_pool=None,
-             subnet_size=None, data_path_addr=None, **kwargs):
+             subnet_size=None, data_path_addr=None, data_path_port=None,
+             **kwargs):
         """
         Initialize a new swarm on this Engine.
 
         Args:
             advertise_addr (str): Externally reachable address advertised to
                 other nodes. This can either be an address/port combination in
                 the form ``192.168.1.1:4567``, or an interface followed by a
@@ -61,14 +62,17 @@
                 default subnet pools for global scope networks. Each pool
                 should be specified as a CIDR block, like '10.0.0.0/8'.
                 Default: None
             subnet_size (int): SubnetSize specifies the subnet size of the
                 networks created from the default subnet pool. Default: None
             data_path_addr (string): Address or interface to use for data path
                 traffic. For example, 192.168.1.1, or an interface, like eth0.
+            data_path_port (int): Port number to use for data path traffic.
+                Acceptable port range is 1024 to 49151. If set to ``None`` or
+                0, the default port 4789 will be used. Default: None
             task_history_retention_limit (int): Maximum number of tasks
                 history stored.
             snapshot_interval (int): Number of logs entries between snapshot.
             keep_old_snapshots (int): Number of snapshots to keep beyond the
                 current snapshot.
             log_entries_for_slow_followers (int): Number of log entries to
                 keep around to sync up slow followers after a snapshot is
@@ -117,14 +121,15 @@
         init_kwargs = {
             'advertise_addr': advertise_addr,
             'listen_addr': listen_addr,
             'force_new_cluster': force_new_cluster,
             'default_addr_pool': default_addr_pool,
             'subnet_size': subnet_size,
             'data_path_addr': data_path_addr,
+            'data_path_port': data_path_port,
         }
         init_kwargs['swarm_spec'] = self.client.api.create_swarm_spec(**kwargs)
         node_id = self.client.api.init_swarm(**init_kwargs)
         self.reload()
         return node_id
 
     def join(self, *args, **kwargs):
```

### Comparing `docker-6.0.0b2/docker/models/volumes.py` & `docker-6.0.1/docker/models/volumes.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/tls.py` & `docker-6.0.1/docker/tls.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/transport/npipeconn.py` & `docker-6.0.1/docker/transport/npipeconn.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/transport/npipesocket.py` & `docker-6.0.1/docker/transport/npipesocket.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/transport/sshconn.py` & `docker-6.0.1/docker/transport/sshconn.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/transport/ssladapter.py` & `docker-6.0.1/docker/transport/ssladapter.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/transport/unixconn.py` & `docker-6.0.1/docker/transport/unixconn.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/types/__init__.py` & `docker-6.0.1/docker/types/__init__.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/types/containers.py` & `docker-6.0.1/docker/types/containers.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/types/daemon.py` & `docker-6.0.1/docker/types/daemon.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/types/healthcheck.py` & `docker-6.0.1/docker/types/healthcheck.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/types/networks.py` & `docker-6.0.1/docker/types/networks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .. import errors
 from ..utils import normalize_links, version_lt
 
 
 class EndpointConfig(dict):
     def __init__(self, version, aliases=None, links=None, ipv4_address=None,
-                 ipv6_address=None, link_local_ips=None, driver_opt=None):
+                 ipv6_address=None, link_local_ips=None, driver_opt=None,
+                 mac_address=None):
         if version_lt(version, '1.22'):
             raise errors.InvalidVersion(
                 'Endpoint config is not supported for API version < 1.22'
             )
 
         if aliases:
             self["Aliases"] = aliases
@@ -19,14 +20,21 @@
         ipam_config = {}
         if ipv4_address:
             ipam_config['IPv4Address'] = ipv4_address
 
         if ipv6_address:
             ipam_config['IPv6Address'] = ipv6_address
 
+        if mac_address:
+            if version_lt(version, '1.25'):
+                raise errors.InvalidVersion(
+                    'mac_address is not supported for API version < 1.25'
+                )
+            self['MacAddress'] = mac_address
+
         if link_local_ips is not None:
             if version_lt(version, '1.24'):
                 raise errors.InvalidVersion(
                     'link_local_ips is not supported for API version < 1.24'
                 )
             ipam_config['LinkLocalIPs'] = link_local_ips
```

### Comparing `docker-6.0.0b2/docker/types/services.py` & `docker-6.0.1/docker/types/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,23 +111,25 @@
             containers. Only used for Windows containers.
         init (boolean): Run an init inside the container that forwards signals
             and reaps processes.
         cap_add (:py:class:`list`): A list of kernel capabilities to add to the
             default set for the container.
         cap_drop (:py:class:`list`): A list of kernel capabilities to drop from
             the default set for the container.
+        sysctls (:py:class:`dict`): A dict of sysctl values to add to
+            the container
     """
 
     def __init__(self, image, command=None, args=None, hostname=None, env=None,
                  workdir=None, user=None, labels=None, mounts=None,
                  stop_grace_period=None, secrets=None, tty=None, groups=None,
                  open_stdin=None, read_only=None, stop_signal=None,
                  healthcheck=None, hosts=None, dns_config=None, configs=None,
                  privileges=None, isolation=None, init=None, cap_add=None,
-                 cap_drop=None):
+                 cap_drop=None, sysctls=None):
         self['Image'] = image
 
         if isinstance(command, str):
             command = split_command(command)
         self['Command'] = command
         self['Args'] = args
 
@@ -201,14 +203,20 @@
 
         if cap_drop is not None:
             if not isinstance(cap_drop, list):
                 raise TypeError('cap_drop must be a list')
 
             self['CapabilityDrop'] = cap_drop
 
+        if sysctls is not None:
+            if not isinstance(sysctls, dict):
+                raise TypeError('sysctls must be a dict')
+
+            self['Sysctls'] = sysctls
+
 
 class Mount(dict):
     """
     Describes a mounted folder's configuration inside a container. A list of
     :py:class:`Mount` would be used as part of a
     :py:class:`~docker.types.ContainerSpec`.
```

### Comparing `docker-6.0.0b2/docker/types/swarm.py` & `docker-6.0.1/docker/types/swarm.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/utils/__init__.py` & `docker-6.0.1/docker/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/utils/build.py` & `docker-6.0.1/docker/utils/build.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/utils/config.py` & `docker-6.0.1/docker/utils/config.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/utils/decorators.py` & `docker-6.0.1/docker/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/utils/fnmatch.py` & `docker-6.0.1/docker/utils/fnmatch.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/utils/json_stream.py` & `docker-6.0.1/docker/utils/json_stream.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/utils/ports.py` & `docker-6.0.1/docker/utils/ports.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/utils/proxy.py` & `docker-6.0.1/docker/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/utils/socket.py` & `docker-6.0.1/docker/utils/socket.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 STDERR = 2
 
 
 class SocketError(Exception):
     pass
 
 
+# NpipeSockets have their own error types
+# pywintypes.error: (109, 'ReadFile', 'The pipe has been ended.')
+NPIPE_ENDED = 109
+
+
 def read(socket, n=4096):
     """
     Reads at most n bytes from socket
     """
 
     recoverable_errors = (errno.EINTR, errno.EDEADLK, errno.EWOULDBLOCK)
 
@@ -33,14 +38,23 @@
             return socket.recv(n)
         if isinstance(socket, getattr(pysocket, 'SocketIO')):
             return socket.read(n)
         return os.read(socket.fileno(), n)
     except OSError as e:
         if e.errno not in recoverable_errors:
             raise
+    except Exception as e:
+        is_pipe_ended = (isinstance(socket, NpipeSocket) and
+                         len(e.args) > 0 and
+                         e.args[0] == NPIPE_ENDED)
+        if is_pipe_ended:
+            # npipes don't support duplex sockets, so we interpret
+            # a PIPE_ENDED error as a close operation (0-length read).
+            return 0
+        raise
 
 
 def read_exactly(socket, n):
     """
     Reads exactly n bytes from socket
     Raises SocketError if there isn't enough data
     """
```

### Comparing `docker-6.0.0b2/docker/utils/utils.py` & `docker-6.0.1/docker/utils/utils.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker/version.py` & `docker-6.0.1/docker/version.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docker.egg-info/PKG-INFO` & `docker-6.0.1/docker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker
-Version: 6.0.0b2
+Version: 6.0.1
 Summary: A Python library for the Docker Engine API.
 Home-page: https://github.com/docker/docker-py
 Maintainer: Ulysses Souza
 Maintainer-email: ulysses.souza@docker.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docker-py.readthedocs.io
 Project-URL: Changelog, https://docker-py.readthedocs.io/en/stable/change-log.html
```

### Comparing `docker-6.0.0b2/docker.egg-info/SOURCES.txt` & `docker-6.0.1/docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/api.rst` & `docker-6.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/change-log.md` & `docker-6.0.1/docs/change-log.md`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/client.rst` & `docker-6.0.1/docs/client.rst`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/conf.py` & `docker-6.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/containers.rst` & `docker-6.0.1/docs/containers.rst`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/favicon_whale.png` & `docker-6.0.1/docs/favicon_whale.png`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/images.rst` & `docker-6.0.1/docs/images.rst`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/index.rst` & `docker-6.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/networks.rst` & `docker-6.0.1/docs/networks.rst`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/nodes.rst` & `docker-6.0.1/docs/nodes.rst`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/plugins.rst` & `docker-6.0.1/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/services.rst` & `docker-6.0.1/docs/services.rst`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/swarm.rst` & `docker-6.0.1/docs/swarm.rst`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/tls.rst` & `docker-6.0.1/docs/tls.rst`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/user_guides/multiplex.rst` & `docker-6.0.1/docs/user_guides/multiplex.rst`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/user_guides/swarm_services.md` & `docker-6.0.1/docs/user_guides/swarm_services.md`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/docs/volumes.rst` & `docker-6.0.1/docs/volumes.rst`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/scripts/release.sh` & `docker-6.0.1/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/scripts/versions.py` & `docker-6.0.1/scripts/versions.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/setup.py` & `docker-6.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/Dockerfile` & `docker-6.0.1/tests/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-# syntax = docker/dockerfile:1.4
+# syntax=docker/dockerfile:1
+
 ARG PYTHON_VERSION=3.10
+
 FROM python:${PYTHON_VERSION}
 
 ARG APT_MIRROR
 RUN sed -ri "s/(httpredir|deb).debian.org/${APT_MIRROR:-deb.debian.org}/g" /etc/apt/sources.list \
     && sed -ri "s/(security).debian.org/${APT_MIRROR:-security.debian.org}/g" /etc/apt/sources.list
 
 RUN apt-get update && apt-get -y install --no-install-recommends \
```

### Comparing `docker-6.0.0b2/tests/Dockerfile-dind-certs` & `docker-6.0.1/tests/Dockerfile-dind-certs`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# syntax=docker/dockerfile:1
+
 ARG PYTHON_VERSION=3.10
 
 FROM python:${PYTHON_VERSION}
 RUN mkdir /tmp/certs
 VOLUME /certs
 
 WORKDIR /tmp/certs
```

### Comparing `docker-6.0.0b2/tests/gpg-keys/secret` & `docker-6.0.1/tests/gpg-keys/secret`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/helpers.py` & `docker-6.0.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/api_build_test.py` & `docker-6.0.1/tests/integration/api_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/api_client_test.py` & `docker-6.0.1/tests/integration/api_client_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/api_config_test.py` & `docker-6.0.1/tests/integration/api_config_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/api_container_test.py` & `docker-6.0.1/tests/integration/api_container_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,28 @@
 
         self.client.start(container)
         res = self.client.inspect_container(container['Id'])
         assert mac_address_expected == res['NetworkSettings']['MacAddress']
 
         self.client.kill(id)
 
+    @requires_api_version('1.41')
+    def test_create_with_cgroupns(self):
+        host_config = self.client.create_host_config(cgroupns='private')
+
+        container = self.client.create_container(
+            image=TEST_IMG,
+            command=['sleep', '60'],
+            host_config=host_config,
+        )
+        self.tmp_containers.append(container)
+
+        res = self.client.inspect_container(container)
+        assert 'private' == res['HostConfig']['CgroupnsMode']
+
     def test_group_id_ints(self):
         container = self.client.create_container(
             TEST_IMG, 'id -G',
             host_config=self.client.create_host_config(group_add=[1000, 1001])
         )
         self.tmp_containers.append(container)
         self.client.start(container)
```

### Comparing `docker-6.0.0b2/tests/integration/api_exec_test.py` & `docker-6.0.1/tests/integration/api_exec_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/api_healthcheck_test.py` & `docker-6.0.1/tests/integration/api_healthcheck_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/api_image_test.py` & `docker-6.0.1/tests/integration/api_image_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/api_network_test.py` & `docker-6.0.1/tests/integration/api_network_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,14 +404,30 @@
             container, net_name, ipv6_address='2001:389::f00d'
         )
 
         container_data = self.client.inspect_container(container)
         net_data = container_data['NetworkSettings']['Networks'][net_name]
         assert net_data['IPAMConfig']['IPv6Address'] == '2001:389::f00d'
 
+    @requires_api_version('1.25')
+    def test_connect_with_mac_address(self):
+        net_name, net_id = self.create_network()
+
+        container = self.client.create_container(TEST_IMG, 'top')
+        self.tmp_containers.append(container)
+
+        self.client.connect_container_to_network(
+            container, net_name, mac_address='02:42:ac:11:00:02'
+        )
+
+        container_data = self.client.inspect_container(container)
+
+        net_data = container_data['NetworkSettings']['Networks'][net_name]
+        assert net_data['MacAddress'] == '02:42:ac:11:00:02'
+
     @requires_api_version('1.23')
     def test_create_internal_networks(self):
         _, net_id = self.create_network(internal=True)
         net = self.client.inspect_network(net_id)
         assert net['Internal'] is True
 
     @requires_api_version('1.23')
```

### Comparing `docker-6.0.0b2/tests/integration/api_plugin_test.py` & `docker-6.0.1/tests/integration/api_plugin_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/api_secret_test.py` & `docker-6.0.1/tests/integration/api_secret_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/api_service_test.py` & `docker-6.0.1/tests/integration/api_service_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1415,7 +1415,27 @@
         svc_id = self.client.create_service(task_tmpl, name=name)
         assert self.client.inspect_service(svc_id)
         services = self.client.services(filters={'name': name})
         assert len(services) == 1
         assert services[0]['ID'] == svc_id['ID']
         spec = services[0]['Spec']['TaskTemplate']['ContainerSpec']
         assert 'CAP_SYSLOG' in spec['CapabilityDrop']
+
+    @requires_api_version('1.40')
+    def test_create_service_with_sysctl(self):
+        name = self.get_service_name()
+        sysctls = {
+            'net.core.somaxconn': '1024',
+            'net.ipv4.tcp_syncookies': '0',
+        }
+        container_spec = docker.types.ContainerSpec(
+            TEST_IMG, ['echo', 'hello'], sysctls=sysctls
+        )
+        task_tmpl = docker.types.TaskTemplate(container_spec)
+        svc_id = self.client.create_service(task_tmpl, name=name)
+        assert self.client.inspect_service(svc_id)
+        services = self.client.services(filters={'name': name})
+        assert len(services) == 1
+        assert services[0]['ID'] == svc_id['ID']
+        spec = services[0]['Spec']['TaskTemplate']['ContainerSpec']
+        assert spec['Sysctls']['net.core.somaxconn'] == '1024'
+        assert spec['Sysctls']['net.ipv4.tcp_syncookies'] == '0'
```

### Comparing `docker-6.0.0b2/tests/integration/api_swarm_test.py` & `docker-6.0.1/tests/integration/api_swarm_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,7 +249,12 @@
         key_2 = self.client.get_unlock_key()
         assert key_1['UnlockKey'] != key_2['UnlockKey']
 
     @requires_api_version('1.30')
     @pytest.mark.xfail(reason='Can fail if eth0 has multiple IP addresses')
     def test_init_swarm_data_path_addr(self):
         assert self.init_swarm(data_path_addr='eth0')
+
+    @requires_api_version('1.40')
+    def test_init_swarm_data_path_port(self):
+        assert self.init_swarm(data_path_port=4242)
+        assert self.client.inspect_swarm()['DataPathPort'] == 4242
```

### Comparing `docker-6.0.0b2/tests/integration/api_volume_test.py` & `docker-6.0.1/tests/integration/api_volume_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,17 +53,16 @@
         name = 'shootthebullet'
         self.tmp_volumes.append(name)
         self.client.create_volume(name)
         self.client.remove_volume(name, force=True)
 
     @requires_api_version('1.25')
     def test_prune_volumes(self):
-        name = 'hopelessmasquerade'
-        self.client.create_volume(name)
-        self.tmp_volumes.append(name)
+        v = self.client.create_volume()
+        self.tmp_volumes.append(v["Name"])
         result = self.client.prune_volumes()
-        assert name in result['VolumesDeleted']
+        assert v["Name"] in result['VolumesDeleted']
 
     def test_remove_nonexistent_volume(self):
         name = 'shootthebullet'
         with pytest.raises(docker.errors.NotFound):
             self.client.remove_volume(name)
```

### Comparing `docker-6.0.0b2/tests/integration/base.py` & `docker-6.0.1/tests/integration/base.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/client_test.py` & `docker-6.0.1/tests/integration/client_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/conftest.py` & `docker-6.0.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/context_api_test.py` & `docker-6.0.1/tests/integration/context_api_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/credentials/store_test.py` & `docker-6.0.1/tests/integration/credentials/store_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/errors_test.py` & `docker-6.0.1/tests/integration/errors_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/models_containers_test.py` & `docker-6.0.1/tests/integration/models_containers_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/models_images_test.py` & `docker-6.0.1/tests/integration/models_images_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/models_networks_test.py` & `docker-6.0.1/tests/integration/models_networks_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/models_nodes_test.py` & `docker-6.0.1/tests/integration/models_nodes_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/models_resources_test.py` & `docker-6.0.1/tests/integration/models_resources_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/models_services_test.py` & `docker-6.0.1/tests/integration/models_services_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/models_swarm_test.py` & `docker-6.0.1/tests/integration/models_swarm_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/models_volumes_test.py` & `docker-6.0.1/tests/integration/models_volumes_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/integration/regression_test.py` & `docker-6.0.1/tests/integration/regression_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/ssh/api_build_test.py` & `docker-6.0.1/tests/ssh/api_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/ssh/base.py` & `docker-6.0.1/tests/ssh/base.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/ssh/config/client/id_rsa` & `docker-6.0.1/tests/ssh/config/client/id_rsa`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/ssh/config/client/id_rsa.pub` & `docker-6.0.1/tests/ssh/config/client/id_rsa.pub`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/ssh/connect_test.py` & `docker-6.0.1/tests/ssh/connect_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/api_build_test.py` & `docker-6.0.1/tests/unit/api_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/api_container_test.py` & `docker-6.0.1/tests/unit/api_container_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1065,14 +1065,33 @@
                 "CpuPercent": 20,
                 "NanoCpus": 1000,
                 "NetworkMode": "default"
             }}
         ''')
         assert args[1]['headers'] == {'Content-Type': 'application/json'}
 
+    @requires_api_version('1.41')
+    def test_create_container_with_cgroupns(self):
+        self.client.create_container(
+            image='busybox',
+            command='true',
+            host_config=self.client.create_host_config(
+                cgroupns='private',
+            ),
+        )
+
+        args = fake_request.call_args
+        assert args[0][1] == url_prefix + 'containers/create'
+
+        expected_payload = self.base_create_payload()
+        expected_payload['HostConfig'] = self.client.create_host_config()
+        expected_payload['HostConfig']['CgroupnsMode'] = 'private'
+        assert json.loads(args[1]['data']) == expected_payload
+        assert args[1]['headers'] == {'Content-Type': 'application/json'}
+
 
 class ContainerTest(BaseAPIClientTest):
     def test_list_containers(self):
         self.client.containers(all=True)
 
         fake_request.assert_called_with(
             'GET',
@@ -1256,14 +1275,30 @@
             url_prefix + 'containers/' + fake_api.FAKE_CONTAINER_ID + '/logs',
             params={'timestamps': 0, 'follow': 0, 'stderr': 1, 'stdout': 1,
                     'tail': 'all', 'since': ts},
             timeout=DEFAULT_TIMEOUT_SECONDS,
             stream=False
         )
 
+    def test_log_since_with_float(self):
+        ts = 809222400.000000
+        with mock.patch('docker.api.client.APIClient.inspect_container',
+                        fake_inspect_container):
+            self.client.logs(fake_api.FAKE_CONTAINER_ID, stream=False,
+                             follow=False, since=ts)
+
+        fake_request.assert_called_with(
+            'GET',
+            url_prefix + 'containers/' + fake_api.FAKE_CONTAINER_ID + '/logs',
+            params={'timestamps': 0, 'follow': 0, 'stderr': 1, 'stdout': 1,
+                    'tail': 'all', 'since': ts},
+            timeout=DEFAULT_TIMEOUT_SECONDS,
+            stream=False
+        )
+
     def test_log_since_with_datetime(self):
         ts = 809222400
         time = datetime.datetime.utcfromtimestamp(ts)
         with mock.patch('docker.api.client.APIClient.inspect_container',
                         fake_inspect_container):
             self.client.logs(fake_api.FAKE_CONTAINER_ID, stream=False,
                              follow=False, since=time)
@@ -1278,15 +1313,15 @@
         )
 
     def test_log_since_with_invalid_value_raises_error(self):
         with mock.patch('docker.api.client.APIClient.inspect_container',
                         fake_inspect_container):
             with pytest.raises(docker.errors.InvalidArgument):
                 self.client.logs(fake_api.FAKE_CONTAINER_ID, stream=False,
-                                 follow=False, since=42.42)
+                                 follow=False, since="42.42")
 
     def test_log_tty(self):
         m = mock.Mock()
         with mock.patch('docker.api.client.APIClient.inspect_container',
                         fake_inspect_container_tty):
             with mock.patch('docker.api.client.APIClient._stream_raw_result',
                             m):
```

### Comparing `docker-6.0.0b2/tests/unit/api_exec_test.py` & `docker-6.0.1/tests/unit/api_exec_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/api_image_test.py` & `docker-6.0.1/tests/unit/api_image_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/api_network_test.py` & `docker-6.0.1/tests/unit/api_network_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/api_test.py` & `docker-6.0.1/tests/unit/api_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/api_volume_test.py` & `docker-6.0.1/tests/unit/api_volume_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/auth_test.py` & `docker-6.0.1/tests/unit/auth_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/client_test.py` & `docker-6.0.1/tests/unit/client_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/context_test.py` & `docker-6.0.1/tests/unit/context_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/dockertypes_test.py` & `docker-6.0.1/tests/unit/dockertypes_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/errors_test.py` & `docker-6.0.1/tests/unit/errors_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/fake_api.py` & `docker-6.0.1/tests/unit/fake_api.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/fake_api_client.py` & `docker-6.0.1/tests/unit/fake_api_client.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/fake_stat.py` & `docker-6.0.1/tests/unit/fake_stat.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/models_containers_test.py` & `docker-6.0.1/tests/unit/models_containers_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/models_images_test.py` & `docker-6.0.1/tests/unit/models_images_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/models_networks_test.py` & `docker-6.0.1/tests/unit/models_networks_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/models_resources_test.py` & `docker-6.0.1/tests/unit/models_resources_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/models_services_test.py` & `docker-6.0.1/tests/unit/models_services_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,16 @@
             'workdir': '/',
             'user': 'bob',
             'mounts': [{'some': 'mounts'}],
             'stop_grace_period': 5,
             'constraints': ['foo=bar'],
             'preferences': ['bar=baz'],
             'platforms': [('x86_64', 'linux')],
-            'maxreplicas': 1
+            'maxreplicas': 1,
+            'sysctls': {'foo': 'bar'}
         })
 
         task_template = kwargs.pop('task_template')
 
         assert kwargs == {
             'name': 'somename',
             'labels': {'key': 'value'},
@@ -55,9 +56,9 @@
         assert task_template['LogDriver'] == {
             'Name': 'logdriver',
             'Options': {'foo': 'bar'}
         }
         assert task_template['Networks'] == [{'Target': 'somenet'}]
         assert set(task_template['ContainerSpec'].keys()) == {
             'Image', 'Command', 'Args', 'Hostname', 'Env', 'Dir', 'User',
-            'Labels', 'Mounts', 'StopGracePeriod'
+            'Labels', 'Mounts', 'StopGracePeriod', 'Sysctls'
         }
```

### Comparing `docker-6.0.0b2/tests/unit/sshadapter_test.py` & `docker-6.0.1/tests/unit/sshadapter_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/ssladapter_test.py` & `docker-6.0.1/tests/unit/ssladapter_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/swarm_test.py` & `docker-6.0.1/tests/unit/swarm_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/utils_build_test.py` & `docker-6.0.1/tests/unit/utils_build_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/utils_config_test.py` & `docker-6.0.1/tests/unit/utils_config_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/utils_json_stream_test.py` & `docker-6.0.1/tests/unit/utils_json_stream_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/utils_proxy_test.py` & `docker-6.0.1/tests/unit/utils_proxy_test.py`

 * *Files identical despite different names*

### Comparing `docker-6.0.0b2/tests/unit/utils_test.py` & `docker-6.0.1/tests/unit/utils_test.py`

 * *Files identical despite different names*

