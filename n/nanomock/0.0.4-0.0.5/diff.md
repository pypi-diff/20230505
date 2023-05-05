# Comparing `tmp/nanomock-0.0.4.tar.gz` & `tmp/nanomock-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomock-0.0.4.tar", last modified: Thu May  4 20:56:09 2023, max compression
+gzip compressed data, was "nanomock-0.0.5.tar", last modified: Thu May  4 22:10:29 2023, max compression
```

## Comparing `nanomock-0.0.4.tar` & `nanomock-0.0.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.832810 nanomock-0.0.4/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-02 13:35:20.000000 nanomock-0.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2959 2023-05-04 20:56:09.832810 nanomock-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2743 2023-05-02 22:46:21.000000 nanomock-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-04 20:43:16.000000 nanomock-0.0.4/nanomock/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/docker/
--rw-r--r--   0 root         (0) root         (0)     1043 2023-05-04 20:29:22.000000 nanomock-0.0.4/nanomock/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-05-04 18:55:41.000000 nanomock-0.0.4/nanomock/docker/autoheal.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-05-04 20:35:54.000000 nanomock-0.0.4/nanomock/docker/interface.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-04 20:29:56.000000 nanomock-0.0.4/nanomock/docker/linux.py
--rw-r--r--   0 root         (0) root         (0)      389 2023-05-04 20:30:32.000000 nanomock-0.0.4/nanomock/docker/macos.py
--rw-r--r--   0 root         (0) root         (0)     3170 2023-05-04 18:48:04.000000 nanomock-0.0.4/nanomock/docker/mixin.py
--rw-r--r--   0 root         (0) root         (0)      401 2023-05-04 20:30:11.000000 nanomock-0.0.4/nanomock/docker/windows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 11:22:58.000000 nanomock-0.0.4/nanomock/internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 19:50:05.000000 nanomock-0.0.4/nanomock/internal/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 19:50:25.000000 nanomock-0.0.4/nanomock/internal/data/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/custom_Dockerfile
--rw-r--r--   0 root         (0) root         (0)      297 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/default_config-node.toml
--rw-r--r--   0 root         (0) root         (0)      298 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/default_config-node_voting-disabled.toml
--rw-r--r--   0 root         (0) root         (0)      220 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/default_config-rpc.toml
--rw-r--r--   0 root         (0) root         (0)     1824 2023-05-03 07:50:15.000000 nanomock-0.0.4/nanomock/internal/data/services/default_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/nanolooker/
--rw-r--r--   0 root         (0) root         (0)      960 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/nanolooker/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:41:55.000000 nanomock-0.0.4/nanomock/internal/data/services/nanolooker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-05-03 12:43:38.000000 nanomock-0.0.4/nanomock/internal/data/services/nanolooker/default_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/nanomonitor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:41:59.000000 nanomock-0.0.4/nanomock/internal/data/services/nanomonitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)      659 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/nanomonitor/default_config.php
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-03 09:06:45.000000 nanomock-0.0.4/nanomock/internal/data/services/nanomonitor/default_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/nanoticker/
--rw-r--r--   0 root         (0) root         (0)     1421 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/nanoticker/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:02.000000 nanomock-0.0.4/nanomock/internal/data/services/nanoticker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-05-03 12:43:51.000000 nanomock-0.0.4/nanomock/internal/data/services/nanoticker/default_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/nanovotevisu/
--rw-r--r--   0 root         (0) root         (0)      768 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/nanovotevisu/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:05.000000 nanomock-0.0.4/nanomock/internal/data/services/nanovotevisu/__init__.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-03 12:43:54.000000 nanomock-0.0.4/nanomock/internal/data/services/nanovotevisu/default_docker-compose.yml
--rw-r--r--   0 root         (0) root         (0)      325 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/nanovotevisu/environment.prod.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/promexporter/
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:14.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-04 19:53:21.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/default_docker-compose.yml
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-04 19:54:54.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/default_exporter_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/
--rw-r--r--   0 root         (0) root         (0)    78536 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/
--rw-r--r--   0 root         (0) root         (0)     1448 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml
--rw-r--r--   0 root         (0) root         (0)      515 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/promexporter/prometheus.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.832810 nanomock-0.0.4/nanomock/internal/data/services/tcpdump/
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/tcpdump/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:10.000000 nanomock-0.0.4/nanomock/internal/data/services/tcpdump/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      221 2023-05-03 21:35:04.000000 nanomock-0.0.4/nanomock/internal/data/services/tcpdump/default_docker-compose.yml
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-27 20:34:19.000000 nanomock-0.0.4/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-01 12:06:33.000000 nanomock-0.0.4/nanomock/internal/dependency_checker.py
--rw-rw-r--   0 root         (0) root         (0)      806 2023-05-03 21:35:04.000000 nanomock-0.0.4/nanomock/internal/feature_toggle.py
--rw-r--r--   0 root         (0) root         (0)    26984 2023-05-02 13:32:24.000000 nanomock-0.0.4/nanomock/internal/nl_block_tools.py
--rw-r--r--   0 root         (0) root         (0)     7682 2023-05-02 21:23:27.000000 nanomock-0.0.4/nanomock/internal/nl_initialise.py
--rw-r--r--   0 root         (0) root         (0)     5550 2023-05-04 19:25:42.000000 nanomock-0.0.4/nanomock/internal/utils.py
--rw-r--r--   0 root         (0) root         (0)     1539 2023-05-02 22:39:42.000000 nanomock-0.0.4/nanomock/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.832810 nanomock-0.0.4/nanomock/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 15:36:50.000000 nanomock-0.0.4/nanomock/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-04-27 18:47:46.000000 nanomock-0.0.4/nanomock/modules/nl_nanolib.py
--rw-rw-r--   0 root         (0) root         (0)    44005 2023-05-04 20:39:39.000000 nanomock-0.0.4/nanomock/modules/nl_parse_config.py
--rw-r--r--   0 root         (0) root         (0)    27670 2023-05-02 13:32:25.000000 nanomock-0.0.4/nanomock/modules/nl_rpc.py
--rw-rw-r--   0 root         (0) root         (0)    16991 2023-05-04 20:40:20.000000 nanomock-0.0.4/nanomock/nanomock_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.832810 nanomock-0.0.4/nanomock/os_operations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 18:54:54.000000 nanomock-0.0.4/nanomock/os_operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-04 18:54:54.000000 nanomock-0.0.4/nanomock/os_operations/interface.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 18:54:54.000000 nanomock-0.0.4/nanomock/os_operations/linux.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 18:54:54.000000 nanomock-0.0.4/nanomock/os_operations/macos.py
--rw-r--r--   0 root         (0) root         (0)      825 2023-05-04 19:05:01.000000 nanomock-0.0.4/nanomock/os_operations/mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 20:56:09.828810 nanomock-0.0.4/nanomock.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2959 2023-05-04 20:56:09.000000 nanomock-0.0.4/nanomock.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2989 2023-05-04 20:56:09.000000 nanomock-0.0.4/nanomock.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 20:56:09.000000 nanomock-0.0.4/nanomock.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-04 20:56:09.000000 nanomock-0.0.4/nanomock.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-05-04 20:56:09.000000 nanomock-0.0.4/nanomock.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-04 20:56:09.000000 nanomock-0.0.4/nanomock.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 20:56:09.832810 nanomock-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      784 2023-05-04 20:43:01.000000 nanomock-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.327367 nanomock-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-02 13:35:20.000000 nanomock-0.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-05-04 22:10:29.327367 nanomock-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2743 2023-05-02 22:46:21.000000 nanomock-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.323367 nanomock-0.0.5/nanomock/
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-04 22:10:11.000000 nanomock-0.0.5/nanomock/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.323367 nanomock-0.0.5/nanomock/docker/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-04 20:29:22.000000 nanomock-0.0.5/nanomock/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-04 18:55:41.000000 nanomock-0.0.5/nanomock/docker/autoheal.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-04 20:35:54.000000 nanomock-0.0.5/nanomock/docker/interface.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-04 20:29:56.000000 nanomock-0.0.5/nanomock/docker/linux.py
+-rw-r--r--   0 root         (0) root         (0)      389 2023-05-04 20:30:32.000000 nanomock-0.0.5/nanomock/docker/macos.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-05-04 18:48:04.000000 nanomock-0.0.5/nanomock/docker/mixin.py
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-04 20:30:11.000000 nanomock-0.0.5/nanomock/docker/windows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.323367 nanomock-0.0.5/nanomock/internal/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 11:22:58.000000 nanomock-0.0.5/nanomock/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.323367 nanomock-0.0.5/nanomock/internal/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 19:50:05.000000 nanomock-0.0.5/nanomock/internal/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.323367 nanomock-0.0.5/nanomock/internal/data/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 19:50:25.000000 nanomock-0.0.5/nanomock/internal/data/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/custom_Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      297 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/default_config-node.toml
+-rw-r--r--   0 root         (0) root         (0)      298 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/default_config-node_voting-disabled.toml
+-rw-r--r--   0 root         (0) root         (0)      220 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/default_config-rpc.toml
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-05-04 22:06:12.000000 nanomock-0.0.5/nanomock/internal/data/services/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.323367 nanomock-0.0.5/nanomock/internal/data/services/nanolooker/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/nanolooker/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:41:55.000000 nanomock-0.0.5/nanomock/internal/data/services/nanolooker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-05-03 12:43:38.000000 nanomock-0.0.5/nanomock/internal/data/services/nanolooker/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.323367 nanomock-0.0.5/nanomock/internal/data/services/nanomonitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:41:59.000000 nanomock-0.0.5/nanomock/internal/data/services/nanomonitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/nanomonitor/default_config.php
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-03 09:06:45.000000 nanomock-0.0.5/nanomock/internal/data/services/nanomonitor/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.323367 nanomock-0.0.5/nanomock/internal/data/services/nanoticker/
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/nanoticker/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:02.000000 nanomock-0.0.5/nanomock/internal/data/services/nanoticker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-03 12:43:51.000000 nanomock-0.0.5/nanomock/internal/data/services/nanoticker/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.323367 nanomock-0.0.5/nanomock/internal/data/services/nanovotevisu/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/nanovotevisu/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:05.000000 nanomock-0.0.5/nanomock/internal/data/services/nanovotevisu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-03 12:43:54.000000 nanomock-0.0.5/nanomock/internal/data/services/nanovotevisu/default_docker-compose.yml
+-rw-r--r--   0 root         (0) root         (0)      325 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/nanovotevisu/environment.prod.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.323367 nanomock-0.0.5/nanomock/internal/data/services/promexporter/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/promexporter/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:14.000000 nanomock-0.0.5/nanomock/internal/data/services/promexporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-04 19:53:21.000000 nanomock-0.0.5/nanomock/internal/data/services/promexporter/default_docker-compose.yml
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-04 19:54:54.000000 nanomock-0.0.5/nanomock/internal/data/services/promexporter/default_exporter_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.323367 nanomock-0.0.5/nanomock/internal/data/services/promexporter/grafana/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.323367 nanomock-0.0.5/nanomock/internal/data/services/promexporter/grafana/provisioning/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.327367 nanomock-0.0.5/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/
+-rw-r--r--   0 root         (0) root         (0)    78536 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.327367 nanomock-0.0.5/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml
+-rw-r--r--   0 root         (0) root         (0)      515 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/promexporter/prometheus.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.327367 nanomock-0.0.5/nanomock/internal/data/services/tcpdump/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/tcpdump/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:10.000000 nanomock-0.0.5/nanomock/internal/data/services/tcpdump/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      221 2023-05-03 21:35:04.000000 nanomock-0.0.5/nanomock/internal/data/services/tcpdump/default_docker-compose.yml
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-27 20:34:19.000000 nanomock-0.0.5/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-01 12:06:33.000000 nanomock-0.0.5/nanomock/internal/dependency_checker.py
+-rw-rw-r--   0 root         (0) root         (0)      806 2023-05-03 21:35:04.000000 nanomock-0.0.5/nanomock/internal/feature_toggle.py
+-rw-r--r--   0 root         (0) root         (0)    26984 2023-05-02 13:32:24.000000 nanomock-0.0.5/nanomock/internal/nl_block_tools.py
+-rw-r--r--   0 root         (0) root         (0)     7682 2023-05-02 21:23:27.000000 nanomock-0.0.5/nanomock/internal/nl_initialise.py
+-rw-r--r--   0 root         (0) root         (0)     5550 2023-05-04 19:25:42.000000 nanomock-0.0.5/nanomock/internal/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-05-02 22:39:42.000000 nanomock-0.0.5/nanomock/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.327367 nanomock-0.0.5/nanomock/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 15:36:50.000000 nanomock-0.0.5/nanomock/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-04-27 18:47:46.000000 nanomock-0.0.5/nanomock/modules/nl_nanolib.py
+-rw-rw-r--   0 root         (0) root         (0)    44005 2023-05-04 20:39:39.000000 nanomock-0.0.5/nanomock/modules/nl_parse_config.py
+-rw-r--r--   0 root         (0) root         (0)    27670 2023-05-02 13:32:25.000000 nanomock-0.0.5/nanomock/modules/nl_rpc.py
+-rw-rw-r--   0 root         (0) root         (0)    16991 2023-05-04 20:40:20.000000 nanomock-0.0.5/nanomock/nanomock_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.327367 nanomock-0.0.5/nanomock/os_operations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 18:54:54.000000 nanomock-0.0.5/nanomock/os_operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-04 18:54:54.000000 nanomock-0.0.5/nanomock/os_operations/interface.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 18:54:54.000000 nanomock-0.0.5/nanomock/os_operations/linux.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 18:54:54.000000 nanomock-0.0.5/nanomock/os_operations/macos.py
+-rw-r--r--   0 root         (0) root         (0)      825 2023-05-04 19:05:01.000000 nanomock-0.0.5/nanomock/os_operations/mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:10:29.323367 nanomock-0.0.5/nanomock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-05-04 22:10:29.000000 nanomock-0.0.5/nanomock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-05-04 22:10:29.000000 nanomock-0.0.5/nanomock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 22:10:29.000000 nanomock-0.0.5/nanomock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-04 22:10:29.000000 nanomock-0.0.5/nanomock.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-04 22:10:29.000000 nanomock-0.0.5/nanomock.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-04 22:10:29.000000 nanomock-0.0.5/nanomock.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 22:10:29.327367 nanomock-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-04 22:08:29.000000 nanomock-0.0.5/setup.py
```

### Comparing `nanomock-0.0.4/PKG-INFO` & `nanomock-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomock
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create local dockerized nano-currency networks
 Home-page: https://github.com/gr0vity-dev/nanomock
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 # nano-local
```

### Comparing `nanomock-0.0.4/README.md` & `nanomock-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/docker/__init__.py` & `nanomock-0.0.5/nanomock/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/docker/autoheal.py` & `nanomock-0.0.5/nanomock/docker/autoheal.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/docker/interface.py` & `nanomock-0.0.5/nanomock/docker/interface.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/docker/mixin.py` & `nanomock-0.0.5/nanomock/docker/mixin.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/data/services/default_docker-compose.yml` & `nanomock-0.0.5/nanomock/internal/data/services/default_docker-compose.yml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     env_file:
       - ./dc_nano_local_env
     networks:
       - nano-local  
   
   default_docker_custom: #if we use traffic control we need to install iproute2 
     build: 
-      context: ../
+      context: .
       dockerfile: ./services/custom_Dockerfile
       args:
         - NANO_IMAGE=nanocurrency/nano-beta:latest
         - UID=999
         - TC_ENABLE=FALSE
     user: "123" #replaced with UID during "create" command
     container_name: ${default_docker}
```

### Comparing `nanomock-0.0.4/nanomock/internal/data/services/nanolooker/Dockerfile` & `nanomock-0.0.5/nanomock/internal/data/services/nanolooker/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/data/services/nanolooker/default_docker-compose.yml` & `nanomock-0.0.5/nanomock/internal/data/services/nanolooker/default_docker-compose.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/data/services/nanomonitor/default_config.php` & `nanomock-0.0.5/nanomock/internal/data/services/nanomonitor/default_config.php`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/data/services/nanoticker/Dockerfile` & `nanomock-0.0.5/nanomock/internal/data/services/nanoticker/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/data/services/nanovotevisu/Dockerfile` & `nanomock-0.0.5/nanomock/internal/data/services/nanovotevisu/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/data/services/promexporter/default_docker-compose.yml` & `nanomock-0.0.5/nanomock/internal/data/services/promexporter/default_docker-compose.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json` & `nanomock-0.0.5/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml` & `nanomock-0.0.5/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/data/services/promexporter/prometheus.yml` & `nanomock-0.0.5/nanomock/internal/data/services/promexporter/prometheus.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json` & `nanomock-0.0.5/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/dependency_checker.py` & `nanomock-0.0.5/nanomock/internal/dependency_checker.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/feature_toggle.py` & `nanomock-0.0.5/nanomock/internal/feature_toggle.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/nl_block_tools.py` & `nanomock-0.0.5/nanomock/internal/nl_block_tools.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/nl_initialise.py` & `nanomock-0.0.5/nanomock/internal/nl_initialise.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/internal/utils.py` & `nanomock-0.0.5/nanomock/internal/utils.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/main.py` & `nanomock-0.0.5/nanomock/main.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/modules/nl_nanolib.py` & `nanomock-0.0.5/nanomock/modules/nl_nanolib.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/modules/nl_parse_config.py` & `nanomock-0.0.5/nanomock/modules/nl_parse_config.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/modules/nl_rpc.py` & `nanomock-0.0.5/nanomock/modules/nl_rpc.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/nanomock_manager.py` & `nanomock-0.0.5/nanomock/nanomock_manager.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock/os_operations/mixin.py` & `nanomock-0.0.5/nanomock/os_operations/mixin.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/nanomock.egg-info/PKG-INFO` & `nanomock-0.0.5/nanomock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomock
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create local dockerized nano-currency networks
 Home-page: https://github.com/gr0vity-dev/nanomock
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 # nano-local
```

### Comparing `nanomock-0.0.4/nanomock.egg-info/SOURCES.txt` & `nanomock-0.0.5/nanomock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.4/setup.py` & `nanomock-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="nanomock",
-      version="0.0.4",
+      version="0.0.5",
       author="gr0vity",
       description="Create local dockerized nano-currency networks",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/gr0vity-dev/nanomock",
       packages=find_packages(exclude=["unit_tests"]),
       include_package_data=True,
```

