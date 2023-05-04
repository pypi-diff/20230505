# Comparing `tmp/estimenergy-2.1.0.tar.gz` & `tmp/estimenergy-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estimenergy-2.1.0.tar", max compression
+gzip compressed data, was "estimenergy-2.1.2.tar", max compression
```

## Comparing `estimenergy-2.1.0.tar` & `estimenergy-2.1.2.tar`

### file list

```diff
@@ -1,46 +1,44 @@
--rw-r--r--   0        0        0     1089 2023-05-04 07:49:15.010812 estimenergy-2.1.0/LICENSE
--rw-r--r--   0        0        0     4481 2023-05-04 07:49:15.010812 estimenergy-2.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/__init__.py
--rw-r--r--   0        0        0       38 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/client/__init__.py
--rw-r--r--   0        0        0      639 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/client/client.py
--rw-r--r--   0        0        0      451 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/config.py
--rw-r--r--   0        0        0     6030 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/const.py
--rw-r--r--   0        0        0      665 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/db.py
--rw-r--r--   0        0        0      133 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/devices/__init__.py
--rw-r--r--   0        0        0     2465 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/devices/base_device.py
--rw-r--r--   0        0        0       99 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/devices/device_error.py
--rw-r--r--   0        0        0     4048 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/devices/device_registry.py
--rw-r--r--   0        0        0     8414 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/devices/glow_device.py
--rw-r--r--   0        0        0      540 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/helpers.py
--rw-r--r--   0        0        0      315 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/influx.py
--rw-r--r--   0        0        0      613 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/log.py
--rw-r--r--   0        0        0     2088 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/main.py
--rw-r--r--   0        0        0       94 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/config/__init__.py
--rw-r--r--   0        0        0     1500 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/config/config.py
--rw-r--r--   0        0        0       86 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/config/dev_config.py
--rw-r--r--   0        0        0      132 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/config/influx_config.py
--rw-r--r--   0        0        0      208 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/config/logging_config.py
--rw-r--r--   0        0        0      279 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/config/networking_config.py
--rw-r--r--   0        0        0      186 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/config/sql_config.py
--rw-r--r--   0        0        0      896 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/day.py
--rw-r--r--   0        0        0      912 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/device_config.py
--rw-r--r--   0        0        0       76 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/message.py
--rw-r--r--   0        0        0      874 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/month.py
--rw-r--r--   0        0        0      371 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/total.py
--rw-r--r--   0        0        0      799 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/year.py
--rw-r--r--   0        0        0      479 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/prometheus.py
--rw-r--r--   0        0        0        0 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/routers/__init__.py
--rw-r--r--   0        0        0     4261 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/routers/day_router.py
--rw-r--r--   0        0        0     4293 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/routers/device_router.py
--rw-r--r--   0        0        0     1466 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/routers/month_router.py
--rw-r--r--   0        0        0     1466 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/routers/total_router.py
--rw-r--r--   0        0        0     1436 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/routers/year_router.py
--rw-r--r--   0        0        0        0 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/services/__init__.py
--rw-r--r--   0        0        0      835 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/services/data_service.py
--rw-r--r--   0        0        0     1299 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/services/influx_service.py
--rw-r--r--   0        0        0     4343 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/services/prediction_service.py
--rw-r--r--   0        0        0     1546 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/services/prometheus_service.py
--rw-r--r--   0        0        0    15063 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/services/sql_service.py
--rw-r--r--   0        0        0     2494 2023-05-04 07:49:48.879550 estimenergy-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     5868 1970-01-01 00:00:00.000000 estimenergy-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-04 23:22:51.056419 estimenergy-2.1.2/LICENSE
+-rw-r--r--   0        0        0     4481 2023-05-04 23:22:51.060419 estimenergy-2.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/__init__.py
+-rw-r--r--   0        0        0      451 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/config.py
+-rw-r--r--   0        0        0     6030 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/const.py
+-rw-r--r--   0        0        0      665 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/db.py
+-rw-r--r--   0        0        0      133 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/devices/__init__.py
+-rw-r--r--   0        0        0     2465 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/devices/base_device.py
+-rw-r--r--   0        0        0       99 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/devices/device_error.py
+-rw-r--r--   0        0        0     4048 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/devices/device_registry.py
+-rw-r--r--   0        0        0     8414 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/devices/glow_device.py
+-rw-r--r--   0        0        0      540 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/helpers.py
+-rw-r--r--   0        0        0      315 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/influx.py
+-rw-r--r--   0        0        0      613 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/log.py
+-rw-r--r--   0        0        0     2088 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/main.py
+-rw-r--r--   0        0        0       94 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/models/config/__init__.py
+-rw-r--r--   0        0        0     1500 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/models/config/config.py
+-rw-r--r--   0        0        0       86 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/models/config/dev_config.py
+-rw-r--r--   0        0        0      132 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/models/config/influx_config.py
+-rw-r--r--   0        0        0      208 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/models/config/logging_config.py
+-rw-r--r--   0        0        0      279 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/models/config/networking_config.py
+-rw-r--r--   0        0        0      186 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/models/config/sql_config.py
+-rw-r--r--   0        0        0      896 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/models/day.py
+-rw-r--r--   0        0        0      912 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/models/device_config.py
+-rw-r--r--   0        0        0       76 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/models/message.py
+-rw-r--r--   0        0        0      874 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/models/month.py
+-rw-r--r--   0        0        0      371 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/models/total.py
+-rw-r--r--   0        0        0      799 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/models/year.py
+-rw-r--r--   0        0        0      479 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/prometheus.py
+-rw-r--r--   0        0        0        0 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/routers/__init__.py
+-rw-r--r--   0        0        0     4261 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/routers/day_router.py
+-rw-r--r--   0        0        0     4293 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/routers/device_router.py
+-rw-r--r--   0        0        0     1466 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/routers/month_router.py
+-rw-r--r--   0        0        0     1466 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/routers/total_router.py
+-rw-r--r--   0        0        0     1436 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/routers/year_router.py
+-rw-r--r--   0        0        0        0 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/services/__init__.py
+-rw-r--r--   0        0        0      835 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/services/data_service.py
+-rw-r--r--   0        0        0     1299 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/services/influx_service.py
+-rw-r--r--   0        0        0     4343 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/services/prediction_service.py
+-rw-r--r--   0        0        0     1546 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/services/prometheus_service.py
+-rw-r--r--   0        0        0    15063 2023-05-04 23:22:51.064419 estimenergy-2.1.2/estimenergy/services/sql_service.py
+-rw-r--r--   0        0        0     1726 2023-05-04 23:23:20.005364 estimenergy-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5717 1970-01-01 00:00:00.000000 estimenergy-2.1.2/PKG-INFO
```

### Comparing `estimenergy-2.1.0/LICENSE` & `estimenergy-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/README.md` & `estimenergy-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/const.py` & `estimenergy-2.1.2/estimenergy/const.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/db.py` & `estimenergy-2.1.2/estimenergy/db.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/devices/base_device.py` & `estimenergy-2.1.2/estimenergy/devices/base_device.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/devices/device_registry.py` & `estimenergy-2.1.2/estimenergy/devices/device_registry.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/devices/glow_device.py` & `estimenergy-2.1.2/estimenergy/devices/glow_device.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/helpers.py` & `estimenergy-2.1.2/estimenergy/helpers.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/log.py` & `estimenergy-2.1.2/estimenergy/log.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/main.py` & `estimenergy-2.1.2/estimenergy/main.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/models/config/config.py` & `estimenergy-2.1.2/estimenergy/models/config/config.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/models/day.py` & `estimenergy-2.1.2/estimenergy/models/day.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/models/device_config.py` & `estimenergy-2.1.2/estimenergy/models/device_config.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/models/month.py` & `estimenergy-2.1.2/estimenergy/models/month.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/models/year.py` & `estimenergy-2.1.2/estimenergy/models/year.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/routers/day_router.py` & `estimenergy-2.1.2/estimenergy/routers/day_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/routers/device_router.py` & `estimenergy-2.1.2/estimenergy/routers/device_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/routers/month_router.py` & `estimenergy-2.1.2/estimenergy/routers/month_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/routers/total_router.py` & `estimenergy-2.1.2/estimenergy/routers/total_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/routers/year_router.py` & `estimenergy-2.1.2/estimenergy/routers/year_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/services/data_service.py` & `estimenergy-2.1.2/estimenergy/services/data_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/services/influx_service.py` & `estimenergy-2.1.2/estimenergy/services/influx_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/services/prediction_service.py` & `estimenergy-2.1.2/estimenergy/services/prediction_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/services/prometheus_service.py` & `estimenergy-2.1.2/estimenergy/services/prometheus_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/estimenergy/services/sql_service.py` & `estimenergy-2.1.2/estimenergy/services/sql_service.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.1.0/pyproject.toml` & `estimenergy-2.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,40 @@
 
 [build-system]
-requires = ["poetry-core", "poetry-dynamic-versioning"]
-build-backend = "poetry_dynamic_versioning.backend"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "estimenergy"
 description = "Estimate Energy Consumption"
 authors = ["Lennard Beers <l.beers@outlook.de>"]
 repository = "https://github.com/EuleMitKeule/EstimEnergy"
 readme = "README.md"
 packages = [{include = "estimenergy"}]
 license = "MIT"
-version = "2.1.0"
+version = "2.1.2"
 
 [tool.poetry.scripts]
 api = "estimenergy.main:start"
 drop = "estimenergy.db:drop_db"
 generate-openapi = "estimenergy.main:generate_openapi"
 
-[tool.poe.tasks]
-run = { "script" = "estimenergy.main:start" }
-test = "pytest --cov estimenergy --cov-report term-missing"
-black = "black estimenergy tests custom_components/estimenergy_integration"
-isort = "isort estimenergy tests custom_components/estimenergy_integration"
-mypy = "mypy estimenergy tests custom_components/estimenergy_integration"
-bandit = "bandit -r estimenergy custom_components/estimenergy_integration"
-format.sequence = ["black", "isort", "mypy"]
-format.ignore_fail = true
-security.sequence = ["bandit"]
-security.ignore_fail = true
-
-[tool.poetry-dynamic-versioning]
-enable = false
-vcs = "git"
-style = "semver"
-
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 uvicorn = {extras = ["standard"], version = "~0.20.0"}
 fastapi = "~0.92.0"
 fastapi-crudrouter = "~0.8.6"
 aioesphomeapi = "13.7.2"
-tortoise_orm = "~0.19.3"
 requests = "~2.28.2"
 prometheus_client = "~0.16.0"
 prometheus-fastapi-instrumentator = "~5.10.0"
 python-dotenv = "~0.21.1"
 PyYAML = "~6.0"
 types-requests = "^2.28.11.17"
 types-pyyaml = "^6.0.12.9"
-pydantic-settings-yaml = "^0.1.1"
 influxdb-client = {extras = ["async"], version = "^1.36.1"}
 sqlmodel = "^0.0.8"
 psycopg2-binary = "^2.9.6"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "~7.2.1"
 pytest-cov = "~4.0.0"
@@ -69,15 +50,14 @@
 ruff = "^0.0.260"
 bandit = "^1.7.5"
 pycodestyle = "^2.10.0"
 pydocstyle = "^6.3.0"
 pylint = "^2.17.2"
 
 [tool.poetry.group.build.dependencies]
-poetry-dynamic-versioning = "~0.21.4"
 twine = "~4.0.2"
 
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
 forced_separate = [
     "tests",
```

### Comparing `estimenergy-2.1.0/PKG-INFO` & `estimenergy-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: estimenergy
-Version: 2.1.0
+Version: 2.1.2
 Summary: Estimate Energy Consumption
 Home-page: https://github.com/EuleMitKeule/EstimEnergy
 License: MIT
 Author: Lennard Beers
 Author-email: l.beers@outlook.de
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<6.1)
 Requires-Dist: aioesphomeapi (==13.7.2)
 Requires-Dist: fastapi (>=0.92.0,<0.93.0)
 Requires-Dist: fastapi-crudrouter (>=0.8.6,<0.9.0)
 Requires-Dist: influxdb-client[async] (>=1.36.1,<2.0.0)
 Requires-Dist: prometheus-fastapi-instrumentator (>=5.10.0,<5.11.0)
 Requires-Dist: prometheus_client (>=0.16.0,<0.17.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
-Requires-Dist: pydantic-settings-yaml (>=0.1.1,<0.2.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: requests (>=2.28.2,<2.29.0)
 Requires-Dist: sqlmodel (>=0.0.8,<0.0.9)
-Requires-Dist: tortoise_orm (>=0.19.3,<0.20.0)
 Requires-Dist: types-pyyaml (>=6.0.12.9,<7.0.0.0)
 Requires-Dist: types-requests (>=2.28.11.17,<3.0.0.0)
 Requires-Dist: uvicorn[standard] (>=0.20.0,<0.21.0)
 Project-URL: Repository, https://github.com/EuleMitKeule/EstimEnergy
 Description-Content-Type: text/markdown
 
 [![PyPI](https://img.shields.io/pypi/v/estimenergy)](https://pypi.org/project/estimenergy)
```

