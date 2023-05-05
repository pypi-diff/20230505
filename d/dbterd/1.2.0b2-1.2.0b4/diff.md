# Comparing `tmp/dbterd-1.2.0b2.tar.gz` & `tmp/dbterd-1.2.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbterd-1.2.0b2.tar", max compression
+gzip compressed data, was "dbterd-1.2.0b4.tar", max compression
```

## Comparing `dbterd-1.2.0b2.tar` & `dbterd-1.2.0b4.tar`

### file list

```diff
@@ -1,35 +1,41 @@
--rw-r--r--   0        0        0      203 2023-05-04 06:25:22.667425 dbterd-1.2.0b2/LICENSE
--rw-r--r--   0        0        0     2937 2023-05-04 06:25:22.667425 dbterd-1.2.0b2/README.md
--rw-r--r--   0        0        0        0 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/__init__.py
--rw-r--r--   0        0        0       37 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/__main__.py
--rw-r--r--   0        0        0        0 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/algos/__init__.py
--rw-r--r--   0        0        0     4801 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/algos/base.py
--rw-r--r--   0        0        0     3157 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/algos/filter.py
--rw-r--r--   0        0        0      571 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/algos/meta.py
--rw-r--r--   0        0        0     3724 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/algos/test_relationship.py
--rw-r--r--   0        0        0     2575 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/base.py
--rw-r--r--   0        0        0      560 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/factory.py
--rw-r--r--   0        0        0        0 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/targets/__init__.py
--rw-r--r--   0        0        0      132 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/targets/constants.py
--rw-r--r--   0        0        0      304 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/targets/dbml/__init__.py
--rw-r--r--   0        0        0     1729 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/targets/dbml/dbml_test_relationship.py
--rw-r--r--   0        0        0      168 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/targets/default.py
--rw-r--r--   0        0        0      316 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/targets/mermaid/__init__.py
--rw-r--r--   0        0        0     1597 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
--rw-r--r--   0        0        0      222 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/adapters/worker.py
--rw-r--r--   0        0        0        0 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/cli/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-04 06:25:22.671426 dbterd-1.2.0b2/dbterd/cli/main.py
--rw-r--r--   0        0        0     1928 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/cli/params.py
--rw-r--r--   0        0        0      114 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/constants.py
--rw-r--r--   0        0        0      284 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/default.py
--rw-r--r--   0        0        0        0 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/helpers/__init__.py
--rw-r--r--   0        0        0      721 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/helpers/cli_messaging.py
--rw-r--r--   0        0        0      877 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/helpers/dict.py
--rw-r--r--   0        0        0     4494 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/helpers/file.py
--rw-r--r--   0        0        0     1022 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/helpers/jsonify.py
--rw-r--r--   0        0        0      976 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/helpers/log.py
--rw-r--r--   0        0        0     1605 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/helpers/yaml.py
--rw-r--r--   0        0        0       94 2023-05-04 06:25:22.675426 dbterd-1.2.0b2/dbterd/main.py
--rw-r--r--   0        0        0     2097 2023-05-04 06:25:36.563597 dbterd-1.2.0b2/pyproject.toml
--rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 dbterd-1.2.0b2/PKG-INFO
+-rw-r--r--   0        0        0      203 2023-05-05 06:58:50.218731 dbterd-1.2.0b4/LICENSE
+-rw-r--r--   0        0        0     2972 2023-05-05 06:58:50.218731 dbterd-1.2.0b4/README.md
+-rw-r--r--   0        0        0        0 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/algos/__init__.py
+-rw-r--r--   0        0        0     4801 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/algos/base.py
+-rw-r--r--   0        0        0     3157 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/algos/filter.py
+-rw-r--r--   0        0        0      592 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/algos/meta.py
+-rw-r--r--   0        0        0     4558 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/algos/test_relationship.py
+-rw-r--r--   0        0        0     2575 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/base.py
+-rw-r--r--   0        0        0      560 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/factory.py
+-rw-r--r--   0        0        0        0 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/targets/__init__.py
+-rw-r--r--   0        0        0      306 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/targets/constants.py
+-rw-r--r--   0        0        0      296 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/targets/d2/__init__.py
+-rw-r--r--   0        0        0     1591 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/targets/d2/d2_test_relationship.py
+-rw-r--r--   0        0        0      304 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/targets/dbml/__init__.py
+-rw-r--r--   0        0        0     2167 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/targets/dbml/dbml_test_relationship.py
+-rw-r--r--   0        0        0      168 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/targets/default.py
+-rw-r--r--   0        0        0      320 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/targets/graphviz/__init__.py
+-rw-r--r--   0        0        0     2778 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/targets/graphviz/graphviz_test_relationship.py
+-rw-r--r--   0        0        0      316 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/targets/mermaid/__init__.py
+-rw-r--r--   0        0        0     2162 2023-05-05 06:58:50.222731 dbterd-1.2.0b4/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
+-rw-r--r--   0        0        0      320 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/adapters/targets/plantuml/__init__.py
+-rw-r--r--   0        0        0     2012 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/adapters/targets/plantuml/plantuml_test_relationship.py
+-rw-r--r--   0        0        0      222 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/adapters/worker.py
+-rw-r--r--   0        0        0        0 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/cli/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/cli/main.py
+-rw-r--r--   0        0        0     1928 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/cli/params.py
+-rw-r--r--   0        0        0      164 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/constants.py
+-rw-r--r--   0        0        0      284 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/default.py
+-rw-r--r--   0        0        0        0 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/helpers/__init__.py
+-rw-r--r--   0        0        0      721 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/helpers/cli_messaging.py
+-rw-r--r--   0        0        0      877 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/helpers/dict.py
+-rw-r--r--   0        0        0     4494 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/helpers/file.py
+-rw-r--r--   0        0        0     1022 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/helpers/jsonify.py
+-rw-r--r--   0        0        0      976 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/helpers/log.py
+-rw-r--r--   0        0        0     1605 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/helpers/yaml.py
+-rw-r--r--   0        0        0       94 2023-05-05 06:58:50.226731 dbterd-1.2.0b4/dbterd/main.py
+-rw-r--r--   0        0        0     2097 2023-05-05 06:59:07.858634 dbterd-1.2.0b4/pyproject.toml
+-rw-r--r--   0        0        0     4021 1970-01-01 00:00:00.000000 dbterd-1.2.0b4/PKG-INFO
```

### Comparing `dbterd-1.2.0b2/README.md` & `dbterd-1.2.0b4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 # dbterd
-CLI to generate Diagram-as-a-code file ([DBML](https://dbdiagram.io/d), [Mermaid](https://mermaid-js.github.io/mermaid-live-editor/)) from dbt artifact files (required: `manifest.json`, `catalog.json`)
+
+CLI to generate Diagram-as-a-code file ([DBML](https://dbdiagram.io/d), [Mermaid](https://mermaid-js.github.io/mermaid-live-editor/), [PlantUML](https://plantuml.com/ie-diagram), [GraphViz](https://graphviz.org/), [D2](https://d2lang.com/)) from dbt artifact files (required: `manifest.json`, `catalog.json`)
 
 [![PyPI version](https://badge.fury.io/py/dbterd.svg)](https://pypi.org/project/dbterd/)
 ![python-cli](https://img.shields.io/badge/CLI-Python-FFCE3E?labelColor=14354C&logo=python&logoColor=white)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![python](https://img.shields.io/badge/Python-3.9|3.10|3.11-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![codecov](https://codecov.io/gh/datnguye/dbterd/branch/main/graph/badge.svg?token=N7DMQBLH4P)](https://codecov.io/gh/datnguye/dbterd)
 
-```
+```bash
 pip install dbterd --upgrade
 ```
 
 Verify installed version:
-```
+
+```bash
 dbterd --version
 ```
 
 ## Quick examine with existing samples
+
 ```bash
 # select all models in dbt_resto
-dbterd run -ad samples/dbtresto -o target
+dbterd run -ad samples/dbtresto
 # select all models in dbt_resto, Select multiple dbt resources
-dbterd run -ad samples/dbtresto -o target -rt model -rt source
+dbterd run -ad samples/dbtresto -rt model -rt source
 # select only models in dbt_resto excluding staging
-dbterd run -ad samples/dbtresto -o target -s model.dbt_resto -ns model.dbt_resto.staging
+dbterd run -ad samples/dbtresto -s model.dbt_resto -ns model.dbt_resto.staging
 # select only models in schema name mart excluding staging
-dbterd run -ad samples/dbtresto -o target -s schema:mart -ns model.dbt_resto.staging
+dbterd run -ad samples/dbtresto -s schema:mart -ns model.dbt_resto.staging
 # select only models in schema full name dbt.mart excluding staging
-dbterd run -ad samples/dbtresto -o target -s schema:dbt.mart -ns model.dbt_resto.staging
+dbterd run -ad samples/dbtresto -s schema:dbt.mart -ns model.dbt_resto.staging
 
 # other samples
-dbterd run -ad samples/fivetranlog -o target
-dbterd run -ad samples/fivetranlog -o target -rt model -rt source
+dbterd run -ad samples/fivetranlog
+dbterd run -ad samples/fivetranlog -rt model -rt source
 
-dbterd run -ad samples/facebookad -o target
-dbterd run -ad samples/facebookad -o target -rt model -rt source
+dbterd run -ad samples/facebookad
+dbterd run -ad samples/facebookad -rt model -rt source
 
-dbterd run -ad samples/shopify -o target
-dbterd run -ad samples/shopify -o target -rt model -rt source
+dbterd run -ad samples/shopify -s wildcard:*shopify.shopify__*
+dbterd run -ad samples/shopify -rt model -rt source
 
-dbterd run -ad samples/dbt-constraints \
-  -a "test_relationship:(name:foreign_key|c_from:fk_column_name|c_to:pk_column_name)"
+dbterd run -ad samples/dbt-constraints -a "test_relationship:(name:foreign_key|c_from:fk_column_name|c_to:pk_column_name)"
 
 # your own sample without commiting to repo
-dbterd run -ad samples/local -o target -rt model -rt source
+dbterd run -ad samples/local -rt model -rt source
 ```
 
 ## Quick DEMO
-Check [Quick Demo](https://dbterd.datnguyen.de/latest/nav/guide/generate-dbml.html) out! And, following is the sample result using `dbdocs`:
 
-![screencapture-dbdocs-io-datnguye-poc-2023-02-25-10_29_32.png](https://raw.githubusercontent.com/datnguye/dbterd/main/assets/images/screencapture-dbdocs-io-datnguye-poc-2023-02-25-10_29_32.png)
+Check [Quick Demo](https://dbterd.datnguyen.de/latest/nav/guide/targets/generate-dbml.html) out! And, following is the sample result using `dbdocs`:
 
+![screencapture-dbdocs-io-datnguye-poc-2023-02-25-10_29_32.png](https://raw.githubusercontent.com/datnguye/dbterd/main/assets/images/screencapture-dbdocs-io-datnguye-poc-2023-02-25-10_29_32.png)
 
 ## Contributing ✨
+
 If you've ever wanted to contribute to this tool, and a great cause, now is your chance!
 
 See the contributing docs [CONTRIBUTING](https://dbterd.datnguyen.de/latest/nav/development/contributing-guide.html) for more information.
 
 Finally, super thanks to our *Contributors*:
 
 <a href="https://github.com/datnguye/dbterd/graphs/contributors">
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
 # dbterd CLI to generate Diagram-as-a-code file ([DBML](https://dbdiagram.io/
-d), [Mermaid](https://mermaid-js.github.io/mermaid-live-editor/)) from dbt
-artifact files (required: `manifest.json`, `catalog.json`) [![PyPI version]
-(https://badge.fury.io/py/dbterd.svg)](https://pypi.org/project/dbterd/) !
-[python-cli](https://img.shields.io/badge/CLI-Python-
-FFCE3E?labelColor=14354C&logo=python&logoColor=white) [![License: MIT](https://
-img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/
-MIT) [![python](https://img.shields.io/badge/Python-3.9|3.10|3.11-
+d), [Mermaid](https://mermaid-js.github.io/mermaid-live-editor/), [PlantUML]
+(https://plantuml.com/ie-diagram), [GraphViz](https://graphviz.org/), [D2]
+(https://d2lang.com/)) from dbt artifact files (required: `manifest.json`,
+`catalog.json`) [![PyPI version](https://badge.fury.io/py/dbterd.svg)](https://
+pypi.org/project/dbterd/) ![python-cli](https://img.shields.io/badge/CLI-
+Python-FFCE3E?labelColor=14354C&logo=python&logoColor=white) [![License: MIT]
+(https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/
+licenses/MIT) [![python](https://img.shields.io/badge/Python-3.9|3.10|3.11-
 3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org) [!
 [codecov](https://codecov.io/gh/datnguye/dbterd/branch/main/graph/
-badge.svg?token=N7DMQBLH4P)](https://codecov.io/gh/datnguye/dbterd) ``` pip
-install dbterd --upgrade ``` Verify installed version: ``` dbterd --version ```
-## Quick examine with existing samples ```bash # select all models in dbt_resto
-dbterd run -ad samples/dbtresto -o target # select all models in dbt_resto,
-Select multiple dbt resources dbterd run -ad samples/dbtresto -o target -rt
-model -rt source # select only models in dbt_resto excluding staging dbterd run
--ad samples/dbtresto -o target -s model.dbt_resto -ns model.dbt_resto.staging #
-select only models in schema name mart excluding staging dbterd run -ad
-samples/dbtresto -o target -s schema:mart -ns model.dbt_resto.staging # select
-only models in schema full name dbt.mart excluding staging dbterd run -ad
-samples/dbtresto -o target -s schema:dbt.mart -ns model.dbt_resto.staging #
-other samples dbterd run -ad samples/fivetranlog -o target dbterd run -ad
-samples/fivetranlog -o target -rt model -rt source dbterd run -ad samples/
-facebookad -o target dbterd run -ad samples/facebookad -o target -rt model -rt
-source dbterd run -ad samples/shopify -o target dbterd run -ad samples/shopify
--o target -rt model -rt source dbterd run -ad samples/dbt-constraints \ -
+badge.svg?token=N7DMQBLH4P)](https://codecov.io/gh/datnguye/dbterd) ```bash pip
+install dbterd --upgrade ``` Verify installed version: ```bash dbterd --version
+``` ## Quick examine with existing samples ```bash # select all models in
+dbt_resto dbterd run -ad samples/dbtresto # select all models in dbt_resto,
+Select multiple dbt resources dbterd run -ad samples/dbtresto -rt model -rt
+source # select only models in dbt_resto excluding staging dbterd run -ad
+samples/dbtresto -s model.dbt_resto -ns model.dbt_resto.staging # select only
+models in schema name mart excluding staging dbterd run -ad samples/dbtresto -
+s schema:mart -ns model.dbt_resto.staging # select only models in schema full
+name dbt.mart excluding staging dbterd run -ad samples/dbtresto -s schema:
+dbt.mart -ns model.dbt_resto.staging # other samples dbterd run -ad samples/
+fivetranlog dbterd run -ad samples/fivetranlog -rt model -rt source dbterd run
+-ad samples/facebookad dbterd run -ad samples/facebookad -rt model -rt source
+dbterd run -ad samples/shopify -s wildcard:*shopify.shopify__* dbterd run -ad
+samples/shopify -rt model -rt source dbterd run -ad samples/dbt-constraints -
 a "test_relationship:(name:foreign_key|c_from:fk_column_name|c_to:
 pk_column_name)" # your own sample without commiting to repo dbterd run -ad
-samples/local -o target -rt model -rt source ``` ## Quick DEMO Check [Quick
-Demo](https://dbterd.datnguyen.de/latest/nav/guide/generate-dbml.html) out!
-And, following is the sample result using `dbdocs`: ![screencapture-dbdocs-io-
+samples/local -rt model -rt source ``` ## Quick DEMO Check [Quick Demo](https:/
+/dbterd.datnguyen.de/latest/nav/guide/targets/generate-dbml.html) out! And,
+following is the sample result using `dbdocs`: ![screencapture-dbdocs-io-
 datnguye-poc-2023-02-25-10_29_32.png](https://raw.githubusercontent.com/
 datnguye/dbterd/main/assets/images/screencapture-dbdocs-io-datnguye-poc-2023-
 02-25-10_29_32.png) ## Contributing â¨ If you've ever wanted to contribute to
 this tool, and a great cause, now is your chance! See the contributing docs
 [CONTRIBUTING](https://dbterd.datnguyen.de/latest/nav/development/contributing-
 guide.html) for more information. Finally, super thanks to our *Contributors*:
 [https://contrib.rocks/image?repo=datnguye/dbterd]
```

### Comparing `dbterd-1.2.0b2/dbterd/adapters/algos/base.py` & `dbterd-1.2.0b4/dbterd/adapters/algos/base.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b2/dbterd/adapters/algos/filter.py` & `dbterd-1.2.0b4/dbterd/adapters/algos/filter.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b2/dbterd/adapters/algos/meta.py` & `dbterd-1.2.0b4/dbterd/adapters/algos/meta.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,7 +26,8 @@
 @dataclass
 class Ref:
     """Parsed Relationship object"""
 
     name: str
     table_map: Tuple[str, str]
     column_map: Tuple[str, str]
+    type: str = "n1"
```

### Comparing `dbterd-1.2.0b2/dbterd/adapters/algos/test_relationship.py` & `dbterd-1.2.0b4/dbterd/adapters/algos/test_relationship.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from dbterd.adapters.algos import base
 from dbterd.adapters.algos.filter import is_selected_table
 from dbterd.adapters.algos.meta import Ref
-from dbterd.constants import DEFAULT_ALGO_RULE, TEST_META_IGNORE_IN_ERD
+from dbterd.constants import (
+    DEFAULT_ALGO_RULE,
+    TEST_META_IGNORE_IN_ERD,
+    TEST_META_RELATIONSHIP_TYPE,
+)
 
 
 def parse(manifest, catalog, **kwargs):
     """Get all information (tables, relationships) needed for building diagram
 
     Args:
         manifest (dict): Manifest json
@@ -88,14 +92,17 @@
                     or "_and_".join(
                         manifest.nodes[x].test_metadata.kwargs.get(
                             f'{rules.get("c_from")}s', "unknown"
                         )
                     )
                 ).lower(),
             ],
+            type=get_relationship_type(
+                manifest.nodes[x].meta.get(TEST_META_RELATIONSHIP_TYPE, "")
+            ),
         )
         for x in manifest.nodes
         if (
             x.startswith("test")
             and rules.get("name").lower() in x.lower()
             and manifest.nodes[x].meta.get(TEST_META_IGNORE_IN_ERD, "0") == "0"
         )
@@ -108,7 +115,31 @@
             distinct_maps = [str((x.table_map, x.column_map)) for x in distinct_list]
             if str((ref.table_map, ref.column_map)) not in distinct_maps:
                 distinct_list.append(ref)
 
         return distinct_list
 
     return []
+
+
+def get_relationship_type(meta: str) -> str:
+    """Get short form of the relationship type configured in test meta
+
+    Args:
+        meta (str): meta value
+
+    Returns:
+        str: |
+            Short relationship type. Accepted values: '0n','01','11','nn','n1' and '1n'.
+            And `1n` is default/fallback value
+    """
+    if meta.lower() == "zero-to-many":
+        return "0n"
+    if meta.lower() == "zero-to-one":
+        return "01"
+    if meta.lower() == "one-to-one":
+        return "11"
+    if meta.lower() == "many-to-many":
+        return "nn"
+    if meta.lower() == "one-to-many":
+        return "1n"
+    return "n1"  # "many-to-one"
```

### Comparing `dbterd-1.2.0b2/dbterd/adapters/base.py` & `dbterd-1.2.0b4/dbterd/adapters/base.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b2/dbterd/adapters/factory.py` & `dbterd-1.2.0b4/dbterd/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b2/dbterd/adapters/targets/dbml/dbml_test_relationship.py` & `dbterd-1.2.0b4/dbterd/adapters/targets/d2/d2_test_relationship.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 from dbterd.adapters.algos import test_relationship
 
 
 def run(manifest, catalog, **kwargs):
-    """Parse dbt artifacts and export DBML file
+    """Parse dbt artifacts and export D2 file
 
     Args:
         manifest (dict): Manifest json
         catalog (dict): Catalog json
 
     Returns:
-        Tuple(str, str): File name and the DBML content
+        Tuple(str, str): File name and the D2 content
     """
-    return ("output.dbml", parse(manifest, catalog, **kwargs))
+    return ("output.d2", parse(manifest, catalog, **kwargs))
 
 
 def parse(manifest, catalog, **kwargs):
-    """Get the DBML content from dbt artifacts
+    """Get the D2 content from dbt artifacts
 
     Args:
         manifest (dict): Manifest json
         catalog (dict): Catalog json
 
     Returns:
-        str: DBML content
+        str: D2 content
     """
     tables, relationships = test_relationship.parse(
         manifest=manifest, catalog=catalog, **kwargs
     )
 
-    # Build DBML content
-    dbml = "//Tables (based on the selection criteria)\n"
+    # Build D2 content
+    # https://play.d2lang.com/?script=qlDQtVOo5AIEAAD__w%3D%3D&, https://github.com/terrastruct/d2
+    d2 = ""
     for table in tables:
-        dbml += f"//--configured at schema: {table.database}.{table.schema}\n"
-        dbml += """Table \"{table}\" {{\n{columns}\n}}\n""".format(
+        d2 += '"{table}": {{\n  shape: sql_table\n{columns}\n}}\n'.format(
             table=table.name,
-            columns="\n".join(
-                [
-                    str.format(
-                        '"{0}" "{1}"{2}',
-                        x.name,
-                        x.data_type,
-                        str.format(" [note: {1}{0}{1}]", x.description, chr(34))
-                        if x.description
-                        else "",
-                    )
-                    for x in table.columns
-                ]
-            ),
+            columns="\n".join([f"  {x.name}: {x.data_type}" for x in table.columns]),
         )
 
-    dbml += "//Refs (based on the DBT Relationship Tests)\n"
     for rel in relationships:
-        key_from = f'"{rel.table_map[1]}"."{rel.column_map[1]}"'
-        key_to = f'"{rel.table_map[0]}"."{rel.column_map[0]}"'
-        dbml += f"Ref: {key_from} > {key_to}\n"
-    return dbml
+        key_from = f'"{rel.table_map[1]}"'
+        key_to = f'"{rel.table_map[0]}"'
+        connector = f"{rel.column_map[1]} = {rel.column_map[0]}"
+        d2 += f'{key_from} {get_rel_symbol(rel.type)} {key_to}: "{connector}"\n'
+
+    return d2
+
+
+def get_rel_symbol(relationship_type: str) -> str:
+    """Get D2 relationship symbol
+
+    Args:
+        relationship_type (str): relationship type
+
+    Returns:
+        str: Relation symbol supported in D2
+    """
+    return "->"  # no supports for rel type
```

### Comparing `dbterd-1.2.0b2/dbterd/cli/main.py` & `dbterd-1.2.0b4/dbterd/cli/main.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b2/dbterd/cli/params.py` & `dbterd-1.2.0b4/dbterd/cli/params.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b2/dbterd/helpers/cli_messaging.py` & `dbterd-1.2.0b4/dbterd/helpers/cli_messaging.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b2/dbterd/helpers/dict.py` & `dbterd-1.2.0b4/dbterd/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b2/dbterd/helpers/file.py` & `dbterd-1.2.0b4/dbterd/helpers/file.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b2/dbterd/helpers/jsonify.py` & `dbterd-1.2.0b4/dbterd/helpers/jsonify.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b2/dbterd/helpers/log.py` & `dbterd-1.2.0b4/dbterd/helpers/log.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b2/dbterd/helpers/yaml.py` & `dbterd-1.2.0b4/dbterd/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.2.0b2/pyproject.toml` & `dbterd-1.2.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbterd"
-version = "1.2.0b2"
+version = "1.2.0b4"
 description = "dbterd is a Command Line Interface (CLI) to convert dbt manifest.json file to diagram file"
 authors = ["Dat Nguyen <datnguyen.it09@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/datnguye/dbterd"
 repository = "https://github.com/datnguye/dbterd"
 keywords = ["flake8", "markdown", "lint"]
```

### Comparing `dbterd-1.2.0b2/PKG-INFO` & `dbterd-1.2.0b4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbterd
-Version: 1.2.0b2
+Version: 1.2.0b4
 Summary: dbterd is a Command Line Interface (CLI) to convert dbt manifest.json file to diagram file
 Home-page: https://github.com/datnguye/dbterd
 License: MIT
 Keywords: flake8,markdown,lint
 Author: Dat Nguyen
 Author-email: datnguyen.it09@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -20,68 +20,71 @@
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dbt-artifacts-parser (>=0.2.3,<0.3.0)
 Project-URL: Repository, https://github.com/datnguye/dbterd
 Description-Content-Type: text/markdown
 
 # dbterd
-CLI to generate Diagram-as-a-code file ([DBML](https://dbdiagram.io/d), [Mermaid](https://mermaid-js.github.io/mermaid-live-editor/)) from dbt artifact files (required: `manifest.json`, `catalog.json`)
+
+CLI to generate Diagram-as-a-code file ([DBML](https://dbdiagram.io/d), [Mermaid](https://mermaid-js.github.io/mermaid-live-editor/), [PlantUML](https://plantuml.com/ie-diagram), [GraphViz](https://graphviz.org/), [D2](https://d2lang.com/)) from dbt artifact files (required: `manifest.json`, `catalog.json`)
 
 [![PyPI version](https://badge.fury.io/py/dbterd.svg)](https://pypi.org/project/dbterd/)
 ![python-cli](https://img.shields.io/badge/CLI-Python-FFCE3E?labelColor=14354C&logo=python&logoColor=white)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![python](https://img.shields.io/badge/Python-3.9|3.10|3.11-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![codecov](https://codecov.io/gh/datnguye/dbterd/branch/main/graph/badge.svg?token=N7DMQBLH4P)](https://codecov.io/gh/datnguye/dbterd)
 
-```
+```bash
 pip install dbterd --upgrade
 ```
 
 Verify installed version:
-```
+
+```bash
 dbterd --version
 ```
 
 ## Quick examine with existing samples
+
 ```bash
 # select all models in dbt_resto
-dbterd run -ad samples/dbtresto -o target
+dbterd run -ad samples/dbtresto
 # select all models in dbt_resto, Select multiple dbt resources
-dbterd run -ad samples/dbtresto -o target -rt model -rt source
+dbterd run -ad samples/dbtresto -rt model -rt source
 # select only models in dbt_resto excluding staging
-dbterd run -ad samples/dbtresto -o target -s model.dbt_resto -ns model.dbt_resto.staging
+dbterd run -ad samples/dbtresto -s model.dbt_resto -ns model.dbt_resto.staging
 # select only models in schema name mart excluding staging
-dbterd run -ad samples/dbtresto -o target -s schema:mart -ns model.dbt_resto.staging
+dbterd run -ad samples/dbtresto -s schema:mart -ns model.dbt_resto.staging
 # select only models in schema full name dbt.mart excluding staging
-dbterd run -ad samples/dbtresto -o target -s schema:dbt.mart -ns model.dbt_resto.staging
+dbterd run -ad samples/dbtresto -s schema:dbt.mart -ns model.dbt_resto.staging
 
 # other samples
-dbterd run -ad samples/fivetranlog -o target
-dbterd run -ad samples/fivetranlog -o target -rt model -rt source
+dbterd run -ad samples/fivetranlog
+dbterd run -ad samples/fivetranlog -rt model -rt source
 
-dbterd run -ad samples/facebookad -o target
-dbterd run -ad samples/facebookad -o target -rt model -rt source
+dbterd run -ad samples/facebookad
+dbterd run -ad samples/facebookad -rt model -rt source
 
-dbterd run -ad samples/shopify -o target
-dbterd run -ad samples/shopify -o target -rt model -rt source
+dbterd run -ad samples/shopify -s wildcard:*shopify.shopify__*
+dbterd run -ad samples/shopify -rt model -rt source
 
-dbterd run -ad samples/dbt-constraints \
-  -a "test_relationship:(name:foreign_key|c_from:fk_column_name|c_to:pk_column_name)"
+dbterd run -ad samples/dbt-constraints -a "test_relationship:(name:foreign_key|c_from:fk_column_name|c_to:pk_column_name)"
 
 # your own sample without commiting to repo
-dbterd run -ad samples/local -o target -rt model -rt source
+dbterd run -ad samples/local -rt model -rt source
 ```
 
 ## Quick DEMO
-Check [Quick Demo](https://dbterd.datnguyen.de/latest/nav/guide/generate-dbml.html) out! And, following is the sample result using `dbdocs`:
 
-![screencapture-dbdocs-io-datnguye-poc-2023-02-25-10_29_32.png](https://raw.githubusercontent.com/datnguye/dbterd/main/assets/images/screencapture-dbdocs-io-datnguye-poc-2023-02-25-10_29_32.png)
+Check [Quick Demo](https://dbterd.datnguyen.de/latest/nav/guide/targets/generate-dbml.html) out! And, following is the sample result using `dbdocs`:
 
+![screencapture-dbdocs-io-datnguye-poc-2023-02-25-10_29_32.png](https://raw.githubusercontent.com/datnguye/dbterd/main/assets/images/screencapture-dbdocs-io-datnguye-poc-2023-02-25-10_29_32.png)
 
 ## Contributing ✨
+
 If you've ever wanted to contribute to this tool, and a great cause, now is your chance!
 
 See the contributing docs [CONTRIBUTING](https://dbterd.datnguyen.de/latest/nav/development/contributing-guide.html) for more information.
 
 Finally, super thanks to our *Contributors*:
 
 <a href="https://github.com/datnguye/dbterd/graphs/contributors">
```

#### html2text {}

```diff
@@ -1,52 +1,52 @@
-Metadata-Version: 2.1 Name: dbterd Version: 1.2.0b2 Summary: dbterd is a
+Metadata-Version: 2.1 Name: dbterd Version: 1.2.0b4 Summary: dbterd is a
 Command Line Interface (CLI) to convert dbt manifest.json file to diagram file
 Home-page: https://github.com/datnguye/dbterd License: MIT Keywords:
 flake8,markdown,lint Author: Dat Nguyen Author-email: datnguyen.it09@gmail.com
 Requires-Python: >=3.9,<4.0 Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Software Development :: Documentation Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Topic :: Software
 Development :: Quality Assurance Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dbt-artifacts-parser (>=0.2.3,<0.3.0) Project-URL: Repository,
 https://github.com/datnguye/dbterd Description-Content-Type: text/markdown #
 dbterd CLI to generate Diagram-as-a-code file ([DBML](https://dbdiagram.io/d),
-[Mermaid](https://mermaid-js.github.io/mermaid-live-editor/)) from dbt artifact
-files (required: `manifest.json`, `catalog.json`) [![PyPI version](https://
-badge.fury.io/py/dbterd.svg)](https://pypi.org/project/dbterd/) ![python-cli]
-(https://img.shields.io/badge/CLI-Python-
-FFCE3E?labelColor=14354C&logo=python&logoColor=white) [![License: MIT](https://
-img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/
-MIT) [![python](https://img.shields.io/badge/Python-3.9|3.10|3.11-
+[Mermaid](https://mermaid-js.github.io/mermaid-live-editor/), [PlantUML](https:
+//plantuml.com/ie-diagram), [GraphViz](https://graphviz.org/), [D2](https://
+d2lang.com/)) from dbt artifact files (required: `manifest.json`,
+`catalog.json`) [![PyPI version](https://badge.fury.io/py/dbterd.svg)](https://
+pypi.org/project/dbterd/) ![python-cli](https://img.shields.io/badge/CLI-
+Python-FFCE3E?labelColor=14354C&logo=python&logoColor=white) [![License: MIT]
+(https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/
+licenses/MIT) [![python](https://img.shields.io/badge/Python-3.9|3.10|3.11-
 3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org) [!
 [codecov](https://codecov.io/gh/datnguye/dbterd/branch/main/graph/
-badge.svg?token=N7DMQBLH4P)](https://codecov.io/gh/datnguye/dbterd) ``` pip
-install dbterd --upgrade ``` Verify installed version: ``` dbterd --version ```
-## Quick examine with existing samples ```bash # select all models in dbt_resto
-dbterd run -ad samples/dbtresto -o target # select all models in dbt_resto,
-Select multiple dbt resources dbterd run -ad samples/dbtresto -o target -rt
-model -rt source # select only models in dbt_resto excluding staging dbterd run
--ad samples/dbtresto -o target -s model.dbt_resto -ns model.dbt_resto.staging #
-select only models in schema name mart excluding staging dbterd run -ad
-samples/dbtresto -o target -s schema:mart -ns model.dbt_resto.staging # select
-only models in schema full name dbt.mart excluding staging dbterd run -ad
-samples/dbtresto -o target -s schema:dbt.mart -ns model.dbt_resto.staging #
-other samples dbterd run -ad samples/fivetranlog -o target dbterd run -ad
-samples/fivetranlog -o target -rt model -rt source dbterd run -ad samples/
-facebookad -o target dbterd run -ad samples/facebookad -o target -rt model -rt
-source dbterd run -ad samples/shopify -o target dbterd run -ad samples/shopify
--o target -rt model -rt source dbterd run -ad samples/dbt-constraints \ -
+badge.svg?token=N7DMQBLH4P)](https://codecov.io/gh/datnguye/dbterd) ```bash pip
+install dbterd --upgrade ``` Verify installed version: ```bash dbterd --version
+``` ## Quick examine with existing samples ```bash # select all models in
+dbt_resto dbterd run -ad samples/dbtresto # select all models in dbt_resto,
+Select multiple dbt resources dbterd run -ad samples/dbtresto -rt model -rt
+source # select only models in dbt_resto excluding staging dbterd run -ad
+samples/dbtresto -s model.dbt_resto -ns model.dbt_resto.staging # select only
+models in schema name mart excluding staging dbterd run -ad samples/dbtresto -
+s schema:mart -ns model.dbt_resto.staging # select only models in schema full
+name dbt.mart excluding staging dbterd run -ad samples/dbtresto -s schema:
+dbt.mart -ns model.dbt_resto.staging # other samples dbterd run -ad samples/
+fivetranlog dbterd run -ad samples/fivetranlog -rt model -rt source dbterd run
+-ad samples/facebookad dbterd run -ad samples/facebookad -rt model -rt source
+dbterd run -ad samples/shopify -s wildcard:*shopify.shopify__* dbterd run -ad
+samples/shopify -rt model -rt source dbterd run -ad samples/dbt-constraints -
 a "test_relationship:(name:foreign_key|c_from:fk_column_name|c_to:
 pk_column_name)" # your own sample without commiting to repo dbterd run -ad
-samples/local -o target -rt model -rt source ``` ## Quick DEMO Check [Quick
-Demo](https://dbterd.datnguyen.de/latest/nav/guide/generate-dbml.html) out!
-And, following is the sample result using `dbdocs`: ![screencapture-dbdocs-io-
+samples/local -rt model -rt source ``` ## Quick DEMO Check [Quick Demo](https:/
+/dbterd.datnguyen.de/latest/nav/guide/targets/generate-dbml.html) out! And,
+following is the sample result using `dbdocs`: ![screencapture-dbdocs-io-
 datnguye-poc-2023-02-25-10_29_32.png](https://raw.githubusercontent.com/
 datnguye/dbterd/main/assets/images/screencapture-dbdocs-io-datnguye-poc-2023-
 02-25-10_29_32.png) ## Contributing â¨ If you've ever wanted to contribute to
 this tool, and a great cause, now is your chance! See the contributing docs
 [CONTRIBUTING](https://dbterd.datnguyen.de/latest/nav/development/contributing-
 guide.html) for more information. Finally, super thanks to our *Contributors*:
 [https://contrib.rocks/image?repo=datnguye/dbterd]
```

