# Comparing `tmp/ieeh-power-system-data-model-1.2.0.tar.gz` & `tmp/ieeh-power-system-data-model-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieeh-power-system-data-model-1.2.0.tar", last modified: Mon Mar 20 12:08:18 2023, max compression
+gzip compressed data, was "ieeh-power-system-data-model-1.3.0.tar", last modified: Fri May  5 11:06:33 2023, max compression
```

## Comparing `ieeh-power-system-data-model-1.2.0.tar` & `ieeh-power-system-data-model-1.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      348 2023-03-20 12:07:22.206623 ieeh-power-system-data-model-1.2.0/AUTHORS.md
--rw-r--r--   0        0        0     1568 2023-03-20 12:07:22.206623 ieeh-power-system-data-model-1.2.0/LICENSE
--rw-r--r--   0        0        0     2718 2023-03-20 12:07:22.206623 ieeh-power-system-data-model-1.2.0/README.md
--rw-r--r--   0        0        0        1 2023-03-20 12:07:22.206623 ieeh-power-system-data-model-1.2.0/psdm/__init__.py
--rw-r--r--   0        0        0     1068 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/base.py
--rw-r--r--   0        0        0      579 2023-03-20 12:08:11.722583 ieeh-power-system-data-model-1.2.0/psdm/meta.py
--rw-r--r--   0        0        0        1 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/steadystate_case/__init__.py
--rw-r--r--   0        0        0     1047 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/steadystate_case/active_power.py
--rw-r--r--   0        0        0     3880 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/steadystate_case/case.py
--rw-r--r--   0        0        0     4870 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/steadystate_case/controller.py
--rw-r--r--   0        0        0      432 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/steadystate_case/external_grid.py
--rw-r--r--   0        0        0      539 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/steadystate_case/load.py
--rw-r--r--   0        0        0     1091 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/steadystate_case/reactive_power.py
--rw-r--r--   0        0        0      367 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/steadystate_case/transformer.py
--rw-r--r--   0        0        0        1 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology/__init__.py
--rw-r--r--   0        0        0      491 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology/active_power.py
--rw-r--r--   0        0        0     1383 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology/branch.py
--rw-r--r--   0        0        0      337 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology/characteristic.py
--rw-r--r--   0        0        0      364 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology/coupler.py
--rw-r--r--   0        0        0      697 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology/external_grid.py
--rw-r--r--   0        0        0     3727 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology/load.py
--rw-r--r--   0        0        0     1694 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology/load_model.py
--rw-r--r--   0        0        0      320 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology/node.py
--rw-r--r--   0        0        0      486 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology/reactive_power.py
--rw-r--r--   0        0        0      363 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology/switch.py
--rw-r--r--   0        0        0     1011 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology/topology.py
--rw-r--r--   0        0        0     2315 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology/transformer.py
--rw-r--r--   0        0        0      871 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology/windings.py
--rw-r--r--   0        0        0        1 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology_case/__init__.py
--rw-r--r--   0        0        0      501 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology_case/case.py
--rw-r--r--   0        0        0      399 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/psdm/topology_case/element_state.py
--rw-r--r--   0        0        0     2626 2023-03-20 12:08:11.746583 ieeh-power-system-data-model-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1441 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/tests/test_active_power.py
--rw-r--r--   0        0        0      659 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/tests/test_branch.py
--rw-r--r--   0        0        0     8953 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/tests/test_controller.py
--rw-r--r--   0        0        0     1449 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/tests/test_reactive_power.py
--rw-r--r--   0        0        0     1606 2023-03-20 12:07:22.210623 ieeh-power-system-data-model-1.2.0/tests/test_topology_load.py
--rw-r--r--   0        0        0     3210 1970-01-01 00:00:00.000000 ieeh-power-system-data-model-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      348 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/AUTHORS.md
+-rw-r--r--   0        0        0     1568 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2680 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/README.md
+-rw-r--r--   0        0        0        1 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/__init__.py
+-rw-r--r--   0        0        0     1068 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/base.py
+-rw-r--r--   0        0        0      579 2023-05-05 11:06:26.610995 ieeh-power-system-data-model-1.3.0/psdm/meta.py
+-rw-r--r--   0        0        0        1 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/__init__.py
+-rw-r--r--   0        0        0     1047 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/active_power.py
+-rw-r--r--   0        0        0     3880 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/case.py
+-rw-r--r--   0        0        0     5062 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/controller.py
+-rw-r--r--   0        0        0      432 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/external_grid.py
+-rw-r--r--   0        0        0      539 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/load.py
+-rw-r--r--   0        0        0     1091 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/reactive_power.py
+-rw-r--r--   0        0        0      367 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/transformer.py
+-rw-r--r--   0        0        0        1 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/__init__.py
+-rw-r--r--   0        0        0      491 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/active_power.py
+-rw-r--r--   0        0        0     1931 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/branch.py
+-rw-r--r--   0        0        0      337 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/characteristic.py
+-rw-r--r--   0        0        0      364 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/coupler.py
+-rw-r--r--   0        0        0      697 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/external_grid.py
+-rw-r--r--   0        0        0     3739 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/load.py
+-rw-r--r--   0        0        0     1694 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/load_model.py
+-rw-r--r--   0        0        0      320 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/node.py
+-rw-r--r--   0        0        0      486 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/reactive_power.py
+-rw-r--r--   0        0        0      363 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/switch.py
+-rw-r--r--   0        0        0     1011 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/topology.py
+-rw-r--r--   0        0        0     2351 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/transformer.py
+-rw-r--r--   0        0        0     1081 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology/windings.py
+-rw-r--r--   0        0        0        1 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology_case/__init__.py
+-rw-r--r--   0        0        0      501 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology_case/case.py
+-rw-r--r--   0        0        0      399 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/psdm/topology_case/element_state.py
+-rw-r--r--   0        0        0     2658 2023-05-05 11:06:26.634995 ieeh-power-system-data-model-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1441 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/tests/test_active_power.py
+-rw-r--r--   0        0        0      659 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/tests/test_branch.py
+-rw-r--r--   0        0        0     8953 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/tests/test_controller.py
+-rw-r--r--   0        0        0     1449 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/tests/test_reactive_power.py
+-rw-r--r--   0        0        0     1606 2023-05-05 11:05:33.974229 ieeh-power-system-data-model-1.3.0/tests/test_topology_load.py
+-rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 ieeh-power-system-data-model-1.3.0/PKG-INFO
```

### Comparing `ieeh-power-system-data-model-1.2.0/LICENSE` & `ieeh-power-system-data-model-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.2.0/README.md` & `ieeh-power-system-data-model-1.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,40 @@
+Metadata-Version: 2.1
+Name: ieeh-power-system-data-model
+Version: 1.3.0
+Summary: A data model for describing power systems
+Author-email: Sasan Jacob Rasti <sasan_jacob.rasti@tu-dresden.de>,Laura Fiedler <laura.fiedler1@tu-dresden.de>,Maximilian Schmidt <maximilian.schmidt@tu-dresden.de>,Sebastian Krahmer <sebastian.krahmer@tu-dresden.de>
+Requires-Python: >=3.10,<3.11
+Project-URL: Source, https://github.com/ieeh-tu-dresden/power-system-data-model
+Description-Content-Type: text/markdown
+
 # IEEH Power System Data Model
 
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
-A data model for describing power systems.
+A data model for the description of electrical power systems.
 
 - [IEEH Power System Data Model](#ieeh-power-system-data-model)
-  - [ Field of Application](#-field-of-application)
-  - [ Tutorials](#-tutorials)
-  - [ Installation](#-installation)
-  - [ Development](#-development)
-  - [ Attribution](#-attribution)
+  - [Field of Application](#-field-of-application)
+  - [Installation](#-installation)
+  - [Development](#-development)
+  - [Attribution](#-attribution)
 
 ## <div id="application" /> Field of Application
 
-This data model is intended to use to describe power systems...TODO
+This data model is intended to describe electrical power systems. It provides a hierarchical structure/schema to describe unique entity relations as well as parameter sets.
 
 The data model is structured as the following schema:
 
-* grid topology:
-  * base topology containing all elements of the exported grid
-* topology case;
-  * information about disabled elements to represent a specific operational case based on the base topology
-* steadystate case
-  * information about power draw/infeed for a specific operational case
-
-## <div id="tutorials" /> Tutorials
-
-Jupyter notebooks are provided to get in touch with the usage of this toolbox:
-
-* for export: [powerfactory_export.ipynb](./examples/powerfactory_export.ipynb)
+- grid topology:
+  - base topology containing all elements of the exported grid
+- topology case;
+  - information about disabled elements to represent a specific operational case based on the base topology
+- steadystate case
+  - information about power draw/infeed for a specific operational case
 
 ## <div id="installation" /> Installation
 
 Just install via pip:
 
 ```bash
 pip install ieeh-power-system-data-model
@@ -81,22 +83,23 @@
 
 ```bash
 pdm install
 ```
 
 For development in [Visual Studio Code](https://github.com/microsoft/vscode), all configurations are already provided:
 
-* [flake8](https://github.com/PyCQA/flake8)
-* [black](https://github.com/psf/black)
-* [mypy](https://github.com/python/mypy)
+- [flake8](https://github.com/PyCQA/flake8)
+- [black](https://github.com/psf/black)
+- [mypy](https://github.com/python/mypy)
 
 ## <div id="attribution" /> Attribution
 
 Please provide a link to this repository:
 
 <https://github.com/ieeh-tu-dresden/power-system-data-model>
 
 Please cite as:
 
-Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, _Power System Data Model_, Zenodo, 2022. <https://doi.org/10.5281/zenodo.TODO>.
+Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, _Power System Data Model - A data model for the description of electrical power systems_, Zenodo, 2023. <https://doi.org/10.5281/zenodo.7781375>.
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7781375.svg)](https://doi.org/10.5281/zenodo.7781375)
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7074968.svg)](https://doi.org/10.5281/zenodo.TODO)
```

### Comparing `ieeh-power-system-data-model-1.2.0/psdm/base.py` & `ieeh-power-system-data-model-1.3.0/psdm/base.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.2.0/psdm/meta.py` & `ieeh-power-system-data-model-1.3.0/psdm/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import datetime
 import uuid
 
 import pydantic
 
 from psdm.base import Base
 
-VERSION = "1.2.0"
+VERSION = "1.3.0"
 
 
 class Meta(Base):
     version = VERSION
     name: str
     date: datetime.date  # date of export
     id: uuid.UUID = pydantic.Field(default_factory=uuid.uuid4)  # noqa: A003
```

### Comparing `ieeh-power-system-data-model-1.2.0/psdm/steadystate_case/active_power.py` & `ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/active_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.2.0/psdm/steadystate_case/case.py` & `ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/case.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.2.0/psdm/steadystate_case/controller.py` & `ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # :author: Sebastian Krahmer <sebastian.krahmer@tu-dresden.de>
 # :copyright: Copyright (c) Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, 2022-2023.
 # :license: BSD 3-Clause
 
 from __future__ import annotations
 
 import enum
+from typing import Annotated
 
 import pydantic
 
 from psdm.base import Base
 from psdm.base import CosphiDir
 
 
@@ -32,50 +33,46 @@
     B = "B"
     C = "C"
     AB = "AB"
     BC = "BC"
     CA = "CA"
 
 
-class ControlType(Base):
-    node_target: str  # the controlled node (which can be differ from node the load is connected to)
-
-
-class ControlQConst(ControlType):
+class ControlQConst(Base):
     # q-setpoint control mode
     q_set: float  # Setpoint of reactive power. Counted demand based.
 
     control_strategy = ControlStrategy.Q_CONST
 
 
-class ControlUConst(ControlType):
+class ControlUConst(Base):
     # u-setpoint control mode
     u_set: float = pydantic.Field(ge=0)  # Setpoint of voltage.
     u_meas_ref: ControlledVoltageRef = ControlledVoltageRef.POS_SEQ  # voltage reference
 
     control_strategy = ControlStrategy.U_CONST
 
 
-class ControlTanphiConst(ControlType):
+class ControlTanphiConst(Base):
     # cos(phi) control mode
     cosphi_dir: CosphiDir
     cosphi: float = pydantic.Field(ge=0, le=1)  # cos(phi) for calculation of Q in relation to P.
 
     control_strategy = ControlStrategy.TANPHI_CONST
 
 
-class ControlCosphiConst(ControlType):
+class ControlCosphiConst(Base):
     # cos(phi) control mode
     cosphi_dir: CosphiDir
     cosphi: float = pydantic.Field(ge=0, le=1)  # cos(phi) for calculation of Q in relation to P.
 
     control_strategy = ControlStrategy.COSPHI_CONST
 
 
-class ControlCosphiP(ControlType):
+class ControlCosphiP(Base):
     # cos(phi(P)) control mode
     cosphi_ue: float = pydantic.Field(
         ge=0,
         le=1,
     )  # under excited: cos(phi) for calculation of Q in relation to P.
     cosphi_oe: float = pydantic.Field(
         ge=0,
@@ -83,15 +80,15 @@
     )  # over excited: cos(phi) for calculation of Q in relation to P.
     p_threshold_ue: float = pydantic.Field(le=0)  # under excited: threshold for P.
     p_threshold_oe: float = pydantic.Field(le=0)  # over excited: threshold for P.
 
     control_strategy = ControlStrategy.COSPHI_P
 
 
-class ControlCosphiU(ControlType):
+class ControlCosphiU(Base):
     # cos(phi(U)) control mode
     cosphi_ue: float = pydantic.Field(
         ...,
         ge=0,
         le=1,
     )  # under excited: cos(phi) for calculation of Q in relation to P.
     cosphi_oe: float = pydantic.Field(
@@ -101,15 +98,15 @@
     )  # over excited: cos(phi) for calculation of Q in relation to P.
     u_threshold_ue: float = pydantic.Field(..., ge=0)  # under excited: threshold for U.
     u_threshold_oe: float = pydantic.Field(..., ge=0)  # over excited: threshold for U.
 
     control_strategy = ControlStrategy.COSPHI_U
 
 
-class ControlQU(ControlType):
+class ControlQU(Base):
     # Q(U) characteristic control mode
     m_tg_2015: float = pydantic.Field(
         ...,
         ge=0,
     )  # Droop/Slope based on technical guideline VDE-AR-N 4120:2015: '%/kV'-value --> Q = m_% * Pr * dU_kV
     m_tg_2018: float = pydantic.Field(
         ...,
@@ -133,22 +130,36 @@
 def validate_pos(value: float | None) -> float | None:
     if value is not None and value < 0:
         raise ValueError
 
     return value
 
 
-class ControlQP(ControlType):
+class ControlQP(Base):
     # Q(P) characteristic control mode
     q_p_characteristic_name: str
     q_max_ue: float | None = None  # Under excited limit of Q: absolut value
     q_max_oe: float | None = None  # Over excited limit of Q: absolut value
 
     control_strategy = ControlStrategy.Q_P
 
     validate_q_max_ue = pydantic.validator("q_max_ue", allow_reuse=True)(validate_pos)
     validate_q_max_oe = pydantic.validator("q_max_oe", allow_reuse=True)(validate_pos)
 
 
+ControlType = Annotated[
+    ControlQConst
+    | ControlUConst
+    | ControlTanphiConst
+    | ControlCosphiConst
+    | ControlCosphiP
+    | ControlCosphiU
+    | ControlQU
+    | ControlQP,
+    pydantic.Field(discriminator="control_strategy"),
+]
+
+
 class Controller(Base):
+    node_target: str  # the controlled node (which can be differ from node the load is connected to)
     control_type: ControlType | None = None
     external_controller_name: str | None = None  # if external controller is specified --> name
```

### Comparing `ieeh-power-system-data-model-1.2.0/psdm/steadystate_case/load.py` & `ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/load.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.2.0/psdm/steadystate_case/reactive_power.py` & `ieeh-power-system-data-model-1.3.0/psdm/steadystate_case/reactive_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.2.0/psdm/topology/branch.py` & `ieeh-power-system-data-model-1.3.0/psdm/topology/windings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 # :author: Sasan Jacob Rasti <sasan_jacob.rasti@tu-dresden.de>
 # :copyright: Copyright (c) Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, 2022-2023.
 # :license: BSD 3-Clause
 
 from __future__ import annotations
 
-from enum import Enum
+import enum
 
 from psdm.base import Base
-from psdm.base import VoltageSystemType
 
 
-class BranchType(Enum):
-    LINE = "LINE"
-    COUPLER = "COUPLER"
-
-
-class Branch(Base):
-    node_1: str
-    node_2: str
-    name: str
-    u_n: float  # nominal voltage of the branch connected nodes
-    i_r: float  # rated current of branch (thermal limit in continuous operation)
-    r1: float  # positive sequence values of PI-representation
-    x1: float  # positive sequence values of PI-representation
-    g1: float  # positive sequence values of PI-representation
-    b1: float  # positive sequence values of PI-representation
-    type: BranchType  # noqa: A003
-    voltage_system_type: VoltageSystemType
-    r0: float | None = None  # zero sequence values of PI-representation
-    x0: float | None = None  # zero sequence values of PI-representation
-    g0: float | None = None  # zero sequence values of PI-representation
-    b0: float | None = None  # zero sequence values of PI-representation
-    f_n: float | None = None  # nominal frequency the values x and b apply
-    description: str | None = None
-    energized: bool | None = None
+class VectorGroup(enum.Enum):
+    Y = "Y"
+    YN = "YN"
+    Z = "Z"
+    ZN = "ZN"
+    D = "D"
+
+
+class Winding(Base):
+    node: str
+    s_r: float
+    u_n: float  # Nominal Voltage of connected nodes (CIM: BaseVoltage)
+    u_r: float  # Rated Voltage of the transformer windings itself (CIM: ratedU)
+    r1: float  # positive sequence values of transformer T-representation
+    x1: float
+    r0: float | None = None  # zero sequence values of transformer T-representation
+    x0: float | None = None
+    re: float | None = None  # earthing of neutral point
+    xe: float | None = None  # earthing of neutral point
+    phase_angle_clock: int | None = None
+    vector_group: VectorGroup | None = None
+    neutral_connected: bool = False  # indicates if neutral line is connected to winding object
```

### Comparing `ieeh-power-system-data-model-1.2.0/psdm/topology/external_grid.py` & `ieeh-power-system-data-model-1.3.0/psdm/topology/external_grid.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.2.0/psdm/topology/load.py` & `ieeh-power-system-data-model-1.3.0/psdm/topology/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     ONE_PH_PH_N = "ONE_PH_PH_N"
 
 
 class Phase(enum.Enum):
     A = "A"
     B = "B"
     C = "C"
+    N = "N"
 
 
 THRESHOLD = 0.51  # acceptable rounding error (0.5 W) + epsilon for calculation accuracy (0.01 W)
 
 
 def validate_total(values: dict[str, float]) -> dict[str, float]:
     pow_total = values["value_a"] + values["value_b"] + values["value_c"]
```

### Comparing `ieeh-power-system-data-model-1.2.0/psdm/topology/load_model.py` & `ieeh-power-system-data-model-1.3.0/psdm/topology/load_model.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.2.0/psdm/topology/topology.py` & `ieeh-power-system-data-model-1.3.0/psdm/topology/topology.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.2.0/psdm/topology/transformer.py` & `ieeh-power-system-data-model-1.3.0/psdm/topology/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     YNy0 = "YNy0"
     Yyn0 = "Yyn0"
     YNyn0 = "YNyn0"
     Dz0 = "Dz0"
     Dzn0 = "Dzn0"
     Zd0 = "Zd0"
     ZNd0 = "ZNd0"
+    Dyn1 = "Dyn1"
     Dy5 = "Dy5"
     Dyn5 = "Dyn5"
     Yd5 = "Yd5"
     YNd5 = "YNd5"
     Yz5 = "Yz5"
     YNz5 = "YNz5"
     Yzn5 = "Yzn5"
@@ -48,14 +49,15 @@
     YNy6 = "YNy6"
     Yyn6 = "Yyn6"
     YNyn6 = "YNyn6"
     Dz6 = "Dz6"
     Dzn6 = "Dzn6"
     Zd6 = "Zd6"
     ZNd6 = "ZNd6"
+    Dyn7 = "Dyn7"
     Dy11 = "Dy11"
     Dyn11 = "Dyn11"
     Yd11 = "Yd11"
     YNd11 = "YNd11"
     Yz11 = "Yz11"
     YNz11 = "YNz11"
     Yzn11 = "Yzn11"
```

### Comparing `ieeh-power-system-data-model-1.2.0/pyproject.toml` & `ieeh-power-system-data-model-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "loguru",
     "pydantic",
 ]
 description = "A data model for describing power systems"
 name = "ieeh-power-system-data-model"
 readme = "README.md"
 requires-python = ">=3.10,<3.11"
-version = "1.2.0"
+version = "1.3.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/ieeh-tu-dresden/power-system-data-model"
 
@@ -101,16 +101,17 @@
 
 [tool.black]
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
-version = "1.2.0"
+version = "1.3.0"
 version_files = [
+    "CITATION.cff:cff-version",
     "psdm/meta.py:VERSION",
     "pyproject.toml:version",
 ]
 
 [tool.mypy]
 follow_imports = "normal"
 ignore_missing_imports = true
```

### Comparing `ieeh-power-system-data-model-1.2.0/tests/test_active_power.py` & `ieeh-power-system-data-model-1.3.0/tests/test_active_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.2.0/tests/test_branch.py` & `ieeh-power-system-data-model-1.3.0/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.2.0/tests/test_controller.py` & `ieeh-power-system-data-model-1.3.0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.2.0/tests/test_reactive_power.py` & `ieeh-power-system-data-model-1.3.0/tests/test_reactive_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-power-system-data-model-1.2.0/tests/test_topology_load.py` & `ieeh-power-system-data-model-1.3.0/tests/test_topology_load.py`

 * *Files identical despite different names*

