# Comparing `tmp/ieeh-powerfactory-tools-1.4.2.tar.gz` & `tmp/ieeh-powerfactory-tools-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieeh-powerfactory-tools-1.4.2.tar", last modified: Fri Mar 24 11:43:36 2023, max compression
+gzip compressed data, was "ieeh-powerfactory-tools-1.5.0.tar", last modified: Fri May  5 12:10:37 2023, max compression
```

## Comparing `ieeh-powerfactory-tools-1.4.2.tar` & `ieeh-powerfactory-tools-1.5.0.tar`

### file list

```diff
@@ -1,44 +1,16 @@
--rw-r--r--   0        0        0      272 2023-03-24 11:42:42.959414 ieeh-powerfactory-tools-1.4.2/AUTHORS.md
--rw-r--r--   0        0        0     1568 2023-03-24 11:42:42.959414 ieeh-powerfactory-tools-1.4.2/LICENSE
--rw-r--r--   0        0        0     3874 2023-03-24 11:42:42.959414 ieeh-powerfactory-tools-1.4.2/README.md
--rw-r--r--   0        0        0      316 2023-03-24 11:42:42.963414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/__init__.py
--rw-r--r--   0        0        0     1783 2023-03-24 11:42:42.963414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/constants.py
--rw-r--r--   0        0        0      428 2023-03-24 11:42:42.963414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/exporter/__init__.py
--rw-r--r--   0        0        0   101624 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/exporter/exporter.py
--rw-r--r--   0        0        0    30147 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/exporter/load_power.py
--rw-r--r--   0        0        0    30882 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/interface.py
--rw-r--r--   0        0        0    18231 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/powerfactory_types.py
--rw-r--r--   0        0        0        1 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/__init__.py
--rw-r--r--   0        0        0     1379 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/base.py
--rw-r--r--   0        0        0        1 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/steadystate_case/__init__.py
--rw-r--r--   0        0        0     1110 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/steadystate_case/active_power.py
--rw-r--r--   0        0        0     4070 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/steadystate_case/case.py
--rw-r--r--   0        0        0     4912 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/steadystate_case/controller.py
--rw-r--r--   0        0        0      453 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/steadystate_case/external_grid.py
--rw-r--r--   0        0        0      634 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/steadystate_case/load.py
--rw-r--r--   0        0        0     1191 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/steadystate_case/reactive_power.py
--rw-r--r--   0        0        0      388 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/steadystate_case/transformer.py
--rw-r--r--   0        0        0        1 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology/__init__.py
--rw-r--r--   0        0        0      586 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology/active_power.py
--rw-r--r--   0        0        0     1425 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology/branch.py
--rw-r--r--   0        0        0      358 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology/characteristic.py
--rw-r--r--   0        0        0      385 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology/coupler.py
--rw-r--r--   0        0        0      718 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology/external_grid.py
--rw-r--r--   0        0        0     3871 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology/load.py
--rw-r--r--   0        0        0     1715 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology/load_model.py
--rw-r--r--   0        0        0      341 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology/node.py
--rw-r--r--   0        0        0      544 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology/reactive_power.py
--rw-r--r--   0        0        0      384 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology/switch.py
--rw-r--r--   0        0        0     1254 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology/topology.py
--rw-r--r--   0        0        0     2389 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology/transformer.py
--rw-r--r--   0        0        0      892 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology/windings.py
--rw-r--r--   0        0        0        1 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology_case/__init__.py
--rw-r--r--   0        0        0      596 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology_case/case.py
--rw-r--r--   0        0        0      420 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/powerfactory_tools/schema/topology_case/element_state.py
--rw-r--r--   0        0        0     2486 2023-03-24 11:43:30.692015 ieeh-powerfactory-tools-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     1462 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/tests/test_active_power.py
--rw-r--r--   0        0        0      754 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/tests/test_branch.py
--rw-r--r--   0        0        0     9474 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/tests/test_controller.py
--rw-r--r--   0        0        0     1470 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/tests/test_reactive_power.py
--rw-r--r--   0        0        0     1627 2023-03-24 11:42:42.967414 ieeh-powerfactory-tools-1.4.2/tests/test_topology_load.py
--rw-r--r--   0        0        0     4330 1970-01-01 00:00:00.000000 ieeh-powerfactory-tools-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0      272 2023-05-05 12:09:38.305164 ieeh-powerfactory-tools-1.5.0/AUTHORS.md
+-rw-r--r--   0        0        0     1568 2023-05-05 12:09:38.305164 ieeh-powerfactory-tools-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3565 2023-05-05 12:09:38.305164 ieeh-powerfactory-tools-1.5.0/README.md
+-rw-r--r--   0        0        0      316 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/__init__.py
+-rw-r--r--   0        0        0     1783 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/constants.py
+-rw-r--r--   0        0        0      428 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/exporter/__init__.py
+-rw-r--r--   0        0        0   100878 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/exporter/exporter.py
+-rw-r--r--   0        0        0    30138 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/exporter/load_power.py
+-rw-r--r--   0        0        0    36084 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/interface.py
+-rw-r--r--   0        0        0    26605 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/powerfactory_types.py
+-rw-r--r--   0        0        0      287 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/utils/__init__.py
+-rw-r--r--   0        0        0      583 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/utils/io.py
+-rw-r--r--   0        0        0     2668 2023-05-05 12:10:30.117909 ieeh-powerfactory-tools-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      452 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      493 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/tests/test_interface.py
+-rw-r--r--   0        0        0     4021 1970-01-01 00:00:00.000000 ieeh-powerfactory-tools-1.5.0/PKG-INFO
```

### Comparing `ieeh-powerfactory-tools-1.4.2/LICENSE` & `ieeh-powerfactory-tools-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ieeh-powerfactory-tools-1.4.2/README.md` & `ieeh-powerfactory-tools-1.5.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -16,21 +16,15 @@
 ## <div id="application" /> Field of Application
 
 This application is intended to use for an external usage ('engine mode') of the power flow calculation program [DIgSILENT PowerFactory](https://www.digsilent.de/de/powerfactory.html).
 Therefore, the Python-PowerFactory-API, provided by the company, is utilized.
 
 The following functionalities are provided:
 
-* export of calculation relevant grid data from a PowerFactory project into three common readable JSON files utilizing predefined [schemas](./powerfactory_tools/schema):
-  * grid topology:
-    * base topology containing all elements of the exported grid
-  * topology case;
-    * information about disabled elements to represent a specific operational case based on the base topology
-  * steadystate case
-    * information about power draw/infeed for a specific operational case
+* export of calculation relevant grid data from a PowerFactory project to the [IEEH Power System Data Model](https://github.com/ieeh-tu-dresden/power-system-data-model)
 * [intended in future release] import from external grid data into the PowerFactory environment
 * [intended in future release] basic control of PowerFactory
 
 ## <div id="tutorials" /> Tutorials
 
 Jupyter notebooks are provided to get in touch with the usage of this toolbox:
```

### Comparing `ieeh-powerfactory-tools-1.4.2/powerfactory_tools/constants.py` & `ieeh-powerfactory-tools-1.5.0/powerfactory_tools/constants.py`

 * *Files identical despite different names*

### Comparing `ieeh-powerfactory-tools-1.4.2/powerfactory_tools/exporter/exporter.py` & `ieeh-powerfactory-tools-1.5.0/powerfactory_tools/exporter/exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,135 +1,120 @@
 # :author: Sasan Jacob Rasti <sasan_jacob.rasti@tu-dresden.de>
 # :author: Sebastian Krahmer <sebastian.krahmer@tu-dresden.de>
 # :copyright: Copyright (c) Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, 2022-2023.
 # :license: BSD 3-Clause
 
 from __future__ import annotations
 
-import dataclasses
 import datetime
 import itertools
 import math
 import multiprocessing
 import pathlib
 import textwrap
-from typing import TYPE_CHECKING
+import typing
 
+import pydantic
 from loguru import logger
+from psdm.base import CosphiDir
+from psdm.base import VoltageSystemType
+from psdm.meta import Meta
+from psdm.steadystate_case.case import Case as SteadystateCase
+from psdm.steadystate_case.controller import ControlCosphiConst
+from psdm.steadystate_case.controller import ControlCosphiP
+from psdm.steadystate_case.controller import ControlCosphiU
+from psdm.steadystate_case.controller import ControlledVoltageRef
+from psdm.steadystate_case.controller import Controller
+from psdm.steadystate_case.controller import ControlQConst
+from psdm.steadystate_case.controller import ControlQP
+from psdm.steadystate_case.controller import ControlQU
+from psdm.steadystate_case.controller import ControlTanphiConst
+from psdm.steadystate_case.controller import ControlUConst
+from psdm.steadystate_case.external_grid import ExternalGrid as ExternalGridSSC
+from psdm.steadystate_case.load import Load as LoadSSC
+from psdm.steadystate_case.transformer import Transformer as TransformerSSC
+from psdm.topology.active_power import ActivePower
+from psdm.topology.branch import Branch
+from psdm.topology.branch import BranchType
+from psdm.topology.external_grid import ExternalGrid
+from psdm.topology.external_grid import GridType
+from psdm.topology.load import Load
+from psdm.topology.load import LoadType
+from psdm.topology.load import Phase
+from psdm.topology.load import PhaseConnectionType
+from psdm.topology.load import SystemType
+from psdm.topology.load_model import LoadModel
+from psdm.topology.node import Node
+from psdm.topology.reactive_power import ReactivePower
+from psdm.topology.topology import Topology
+from psdm.topology.transformer import TapSide
+from psdm.topology.transformer import Transformer
+from psdm.topology.transformer import TransformerPhaseTechnologyType
+from psdm.topology.transformer import VectorGroup as TVectorGroup
+from psdm.topology.windings import VectorGroup as WVectorGroup
+from psdm.topology.windings import Winding
+from psdm.topology_case.case import Case as TopologyCase
+from psdm.topology_case.element_state import ElementState
 
 from powerfactory_tools.constants import DecimalDigits
 from powerfactory_tools.constants import Exponents
 from powerfactory_tools.exporter.load_power import LoadPower
+from powerfactory_tools.interface import PowerFactoryData
 from powerfactory_tools.interface import PowerFactoryInterface
 from powerfactory_tools.powerfactory_types import CosphiChar
 from powerfactory_tools.powerfactory_types import CtrlMode
 from powerfactory_tools.powerfactory_types import CtrlVoltageRef
 from powerfactory_tools.powerfactory_types import GeneratorPhaseConnectionType
 from powerfactory_tools.powerfactory_types import GeneratorSystemType
 from powerfactory_tools.powerfactory_types import IOpt
 from powerfactory_tools.powerfactory_types import LoadPhaseConnectionType
 from powerfactory_tools.powerfactory_types import LocalQCtrlMode
 from powerfactory_tools.powerfactory_types import Phase as PFPhase
+from powerfactory_tools.powerfactory_types import PowerFactoryTypes as PFTypes
 from powerfactory_tools.powerfactory_types import QChar
 from powerfactory_tools.powerfactory_types import TerminalVoltageSystemType
+from powerfactory_tools.powerfactory_types import TrfNeutralConnectionType
+from powerfactory_tools.powerfactory_types import TrfNeutralPointState
+from powerfactory_tools.powerfactory_types import TrfPhaseTechnology
+from powerfactory_tools.powerfactory_types import TrfTapSide
 from powerfactory_tools.powerfactory_types import Vector
 from powerfactory_tools.powerfactory_types import VectorGroup
 from powerfactory_tools.powerfactory_types import VoltageSystemType as ElementVoltageSystemType
-from powerfactory_tools.schema.base import CosphiDir
-from powerfactory_tools.schema.base import Meta
-from powerfactory_tools.schema.base import VoltageSystemType
-from powerfactory_tools.schema.steadystate_case.case import Case as SteadystateCase
-from powerfactory_tools.schema.steadystate_case.controller import ControlCosphiConst
-from powerfactory_tools.schema.steadystate_case.controller import ControlCosphiP
-from powerfactory_tools.schema.steadystate_case.controller import ControlCosphiU
-from powerfactory_tools.schema.steadystate_case.controller import ControlledVoltageRef
-from powerfactory_tools.schema.steadystate_case.controller import Controller
-from powerfactory_tools.schema.steadystate_case.controller import ControlQConst
-from powerfactory_tools.schema.steadystate_case.controller import ControlQP
-from powerfactory_tools.schema.steadystate_case.controller import ControlQU
-from powerfactory_tools.schema.steadystate_case.controller import ControlTanphiConst
-from powerfactory_tools.schema.steadystate_case.controller import ControlUConst
-from powerfactory_tools.schema.steadystate_case.external_grid import ExternalGrid as ExternalGridSSC
-from powerfactory_tools.schema.steadystate_case.load import Load as LoadSSC
-from powerfactory_tools.schema.steadystate_case.transformer import Transformer as TransformerSSC
-from powerfactory_tools.schema.topology.active_power import ActivePower
-from powerfactory_tools.schema.topology.branch import Branch
-from powerfactory_tools.schema.topology.branch import BranchType
-from powerfactory_tools.schema.topology.external_grid import ExternalGrid
-from powerfactory_tools.schema.topology.external_grid import GridType
-from powerfactory_tools.schema.topology.load import Load
-from powerfactory_tools.schema.topology.load import LoadType
-from powerfactory_tools.schema.topology.load import Phase
-from powerfactory_tools.schema.topology.load import PhaseConnectionType
-from powerfactory_tools.schema.topology.load import SystemType
-from powerfactory_tools.schema.topology.load_model import LoadModel
-from powerfactory_tools.schema.topology.node import Node
-from powerfactory_tools.schema.topology.reactive_power import ReactivePower
-from powerfactory_tools.schema.topology.topology import Topology
-from powerfactory_tools.schema.topology.transformer import TapSide
-from powerfactory_tools.schema.topology.transformer import Transformer
-from powerfactory_tools.schema.topology.transformer import TransformerPhaseTechnologyType
-from powerfactory_tools.schema.topology.transformer import VectorGroup as TVectorGroup
-from powerfactory_tools.schema.topology.windings import VectorGroup as WVectorGroup
-from powerfactory_tools.schema.topology.windings import Winding
-from powerfactory_tools.schema.topology_case.case import Case as TopologyCase
-from powerfactory_tools.schema.topology_case.element_state import ElementState
 
-if TYPE_CHECKING:
+if typing.TYPE_CHECKING:
     from collections.abc import Sequence
     from types import TracebackType
     from typing import Literal
 
-    from powerfactory_tools.powerfactory_types import PowerFactoryTypes as PFTypes
-    from powerfactory_tools.schema.steadystate_case.controller import ControlType
+    from psdm.steadystate_case.controller import ControlType
 
     ElementBase = PFTypes.GeneratorBase | PFTypes.LoadBase | PFTypes.ExternalGrid
 
 
 POWERFACTORY_PATH = pathlib.Path("C:/Program Files/DIgSILENT")
 POWERFACTORY_VERSION = "2022 SP2"
 PYTHON_VERSION = "3.10"
 
 FULL_DYNAMIC = 100
 M_TAB2015_MIN_THRESHOLD = 0.01
 
 
-@dataclasses.dataclass
+@pydantic.dataclasses.dataclass
 class LoadLV:
     fixed: LoadPower
     night: LoadPower
     flexible: LoadPower
 
 
-@dataclasses.dataclass
+@pydantic.dataclasses.dataclass
 class LoadMV:
     consumer: LoadPower
     producer: LoadPower
 
 
-@dataclasses.dataclass
-class PowerFactoryData:
-    name: str
-    date: datetime.date
-    project: str
-    external_grids: Sequence[PFTypes.ExternalGrid]
-    terminals: Sequence[PFTypes.Terminal]
-    lines: Sequence[PFTypes.Line]
-    transformers_2w: Sequence[PFTypes.Transformer2W]
-    transformers_3w: Sequence[PFTypes.Transformer3W]
-    loads: Sequence[PFTypes.Load]
-    loads_lv: Sequence[PFTypes.LoadLV]
-    loads_mv: Sequence[PFTypes.LoadMV]
-    generators: Sequence[PFTypes.Generator]
-    pv_systems: Sequence[PFTypes.PVSystem]
-    couplers: Sequence[PFTypes.Coupler]
-    switches: Sequence[PFTypes.Switch]
-    fuses: Sequence[PFTypes.Fuse]
-
-
 class PowerFactoryExporterProcess(multiprocessing.Process):
     def __init__(
         self,
         *,
         export_path: pathlib.Path,
         project_name: str,
         grid_name: str,
@@ -172,15 +157,15 @@
             powerfactory_path=self.powerfactory_path,
             powerfactory_version=self.powerfactory_version,
             python_version=self.python_version,
         )
         pfe.export(self.export_path, self.topology_name, self.topology_case_name, self.steadystate_case_name)
 
 
-@dataclasses.dataclass
+@pydantic.dataclasses.dataclass
 class PowerFactoryExporter:
     project_name: str
     grid_name: str
     powerfactory_user_profile: str = ""
     powerfactory_path: pathlib.Path = POWERFACTORY_PATH
     powerfactory_version: str = POWERFACTORY_VERSION
     python_version: str = PYTHON_VERSION
@@ -222,15 +207,15 @@
             export_path {pathlib.Path} -- the directory where the exported json files are saved
             topology_name {str} -- the chosen file name for 'topology' data
             topology_case_name {str} -- the chosen file name for related 'topology_case' data
             steadystate_case_name {str} -- the chosen file name for related 'steadystate_case' data
         """
 
         logger.debug("Exporting {project_name}...", project_name=self.project_name)
-        data = self.compile_powerfactory_data()
+        data = self.pfi.compile_powerfactory_data(self.grid_name)
         meta = self.create_meta_data(data=data)
 
         topology = self.create_topology(meta=meta, data=data)
         topology_case = self.create_topology_case(meta=meta, data=data)
         steadystate_case = self.create_steadystate_case(meta=meta, data=data)
 
         if steadystate_case.is_valid_topology(topology) is False:
@@ -270,17 +255,17 @@
             topology_case_name {str} -- the chosen file name for related 'topology_case' data
             steadystate_case_name {str} -- the chosen file name for related 'steadystate_case' data
             verify_steadystate_case {bool} -- if True, associated topology is created to be checked against
         """
 
         logger.debug("Exporting scenario {scenario_name}...", scenario_name=scenario_name)
         if scenario_name is not None:
-            self.switch_scenario(scenario_name)
+            self.pfi.switch_scenario(scenario_name)
 
-        data = self.compile_powerfactory_data()
+        data = self.pfi.compile_powerfactory_data(self.grid_name)
         meta = self.create_meta_data(data=data)
 
         topology_case = self.create_topology_case(meta=meta, data=data)
         steadystate_case = self.create_steadystate_case(meta=meta, data=data)
         if verify_steadystate_case is True:
             topology = self.create_topology(meta=meta, data=data)
             if steadystate_case.is_valid_topology(topology) is False:
@@ -365,65 +350,14 @@
             file_path.resolve()
         except OSError as e:
             msg = f"File path {file_path} is not a valid path."
             raise FileNotFoundError(msg) from e
 
         data.to_json(file_path)
 
-    def switch_study_case(self, sc: str) -> None:
-        study_case = self.pfi.study_case(name=sc)
-        if study_case is not None:
-            self.pfi.activate_study_case(study_case)
-        else:
-            msg = f"Study case {sc} does not exist."
-            raise RuntimeError(msg)
-
-    def switch_scenario(self, scen: str) -> None:
-        scenario = self.pfi.scenario(name=scen)
-        if scenario is not None:
-            self.pfi.activate_scenario(scenario)
-        else:
-            msg = f"Scenario {scen} does not exist."
-            raise RuntimeError(msg)
-
-    def compile_powerfactory_data(self) -> PowerFactoryData:
-        logger.debug("Compiling data from PowerFactory...")
-        if self.grid_name == "*":
-            name = self.project_name
-        else:
-            grids = self.pfi.grids()
-            try:
-                grid = [e for e in grids if e.loc_name == self.grid_name][0]
-                name = grid.loc_name
-            except IndexError as e:
-                msg = f"Grid {self.grid_name} does not exist."
-                raise RuntimeError(msg) from e
-
-        project = self.pfi.project.loc_name
-        date = datetime.datetime.now().astimezone().date()  # noqa: DTZ005
-
-        return PowerFactoryData(
-            name=name,
-            date=date,
-            project=project,
-            external_grids=self.pfi.external_grids(grid=self.grid_name),
-            terminals=self.pfi.terminals(grid=self.grid_name),
-            lines=self.pfi.lines(grid=self.grid_name),
-            transformers_2w=self.pfi.transformers_2w(grid=self.grid_name),
-            transformers_3w=self.pfi.transformers_3w(grid=self.grid_name),
-            loads=self.pfi.loads(grid=self.grid_name),
-            loads_lv=self.pfi.loads_lv(grid=self.grid_name),
-            loads_mv=self.pfi.loads_mv(grid=self.grid_name),
-            generators=self.pfi.generators(grid=self.grid_name),
-            pv_systems=self.pfi.pv_systems(grid=self.grid_name),
-            couplers=self.pfi.couplers(grid=self.grid_name),
-            switches=self.pfi.switches(grid=self.grid_name),
-            fuses=self.pfi.fuses(grid=self.grid_name),
-        )
-
     @staticmethod
     def create_meta_data(data: PowerFactoryData) -> Meta:
         logger.debug("Creating meta data...")
         grid_name = data.name.replace(" ", "-")
         project = data.project.replace(" ", "-")
         date = data.date
 
@@ -507,15 +441,15 @@
         if not export:
             logger.warning("Node {node_name} not set for export. Skipping.", node_name=name)
             return None
 
         u_n = round(terminal.uknom * Exponents.VOLTAGE, DecimalDigits.VOLTAGE)  # voltage in V
 
         if self.pfi.is_within_substation(terminal):
-            description = "substation internal" if description else "substation internal; " + description
+            description = "substation internal" if not description else "substation internal; " + description
 
         return Node(name=name, u_n=u_n, description=description)
 
     def create_branches(
         self,
         lines: Sequence[PFTypes.Line],
         couplers: Sequence[PFTypes.Coupler],
@@ -523,15 +457,15 @@
     ) -> Sequence[Branch]:
         logger.info("Creating branches...")
         blines = [self.create_line(line, grid_name) for line in lines]
         bcouplers = [self.create_coupler(coupler, grid_name) for coupler in couplers]
 
         return self.pfi.list_from_sequences(self.pfi.filter_none(blines), self.pfi.filter_none(bcouplers))
 
-    def create_line(self, line: PFTypes.Line, grid_name: str) -> Branch | None:
+    def create_line(self, line: PFTypes.Line, grid_name: str) -> Branch | None:  # noqa: PLR0915
         name = self.pfi.create_name(line, grid_name)
         logger.debug("Creating line {line_name}...", line_name=name)
         export, description = self.get_description(line)
         if not export:
             logger.warning("Line {line_name} not set for export. Skipping.", line_name=name)
             return None
 
@@ -570,14 +504,34 @@
         r0 = l_type.rline0 * line.dline / line.nlnum * Exponents.RESISTANCE
         x0 = l_type.xline0 * line.dline / line.nlnum * Exponents.REACTANCE
         g1 = l_type.gline * line.dline * line.nlnum * Exponents.CONDUCTANCE
         b1 = l_type.bline * line.dline * line.nlnum * Exponents.SUSCEPTANCE
         g0 = l_type.gline0 * line.dline * line.nlnum * Exponents.CONDUCTANCE
         b0 = l_type.bline0 * line.dline * line.nlnum * Exponents.SUSCEPTANCE
 
+        if l_type.nneutral:
+            l_type = typing.cast("PFTypes.LineNType", l_type)
+            rn = l_type.rnline * line.dline / line.nlnum * Exponents.RESISTANCE
+            xn = l_type.xnline * line.dline / line.nlnum * Exponents.REACTANCE
+            rpn = l_type.rpnline * line.dline / line.nlnum * Exponents.RESISTANCE
+            xpn = l_type.xpnline * line.dline / line.nlnum * Exponents.REACTANCE
+            gn = l_type.gnline * line.dline * line.nlnum * Exponents.CONDUCTANCE
+            bn = l_type.bnline * line.dline * line.nlnum * Exponents.SUSCEPTANCE
+            gpn = l_type.gpnline * line.dline * line.nlnum * Exponents.CONDUCTANCE
+            bpn = l_type.bpnline * line.dline * line.nlnum * Exponents.SUSCEPTANCE
+        else:
+            rn = None
+            xn = None
+            rpn = None
+            xpn = None
+            gn = None
+            bn = None
+            gpn = None
+            bpn = None
+
         f_nom = l_type.frnom  # usually 50 Hertz
         u_system_type = VoltageSystemType[ElementVoltageSystemType(l_type.systp).name]
 
         return Branch(
             name=name,
             node_1=t1_name,
             node_2=t2_name,
@@ -585,14 +539,22 @@
             x1=x1,
             r0=r0,
             x0=x0,
             g1=g1,
             b1=b1,
             g0=g0,
             b0=b0,
+            rn=rn,
+            xn=xn,
+            rpn=rpn,
+            xpn=xpn,
+            gn=gn,
+            bn=bn,
+            gpn=gpn,
+            bpn=bpn,
             i_r=i_r,
             description=description,
             u_n=u_nom,
             f_n=f_nom,
             type=BranchType.LINE,
             voltage_system_type=u_system_type,
         )
@@ -672,15 +634,15 @@
     def get_coupler_description(
         self,
         terminal1: PFTypes.Terminal,
         terminal2: PFTypes.Terminal,
         description: str,
     ) -> str:
         if self.pfi.is_within_substation(terminal1) and self.pfi.is_within_substation(terminal2):
-            if description:
+            if not description:
                 return "substation internal"
 
             return "substation internal; " + description
 
         return description
 
     def create_transformers(
@@ -696,15 +658,19 @@
         transformers_2w: Sequence[PFTypes.Transformer2W],
         grid_name: str,
     ) -> Sequence[Transformer]:
         logger.info("Creating 2-winding transformers...")
         transformers = [self.create_transformer_2w(transformer_2w, grid_name) for transformer_2w in transformers_2w]
         return self.pfi.filter_none(transformers)
 
-    def create_transformer_2w(self, transformer_2w: PFTypes.Transformer2W, grid_name: str) -> Transformer | None:
+    def create_transformer_2w(  # noqa: PLR0915
+        self,
+        transformer_2w: PFTypes.Transformer2W,
+        grid_name: str,
+    ) -> Transformer | None:
         name = self.pfi.create_name(element=transformer_2w, grid_name=grid_name)
         logger.debug("Creating 2-winding transformer {transformer_name}...", transformer_name=name)
         export, description = self.get_description(transformer_2w)
         if not export:
             logger.warning(
                 "2-winding transformer {transformer_name} not set for export. Skipping.",
                 transformer_name=name,
@@ -724,25 +690,24 @@
         t_high_name = self.pfi.create_name(element=t_high, grid_name=grid_name)
         t_low_name = self.pfi.create_name(element=t_low, grid_name=grid_name)
 
         t_type = transformer_2w.typ_id
 
         if t_type is not None:
             t_number = transformer_2w.ntnum
-            vector_group = TVectorGroup[VectorGroup(t_type.vecgrp).name]
 
-            ph_technology = self.transformer_phase_technology(t_type)
+            ph_technology = TransformerPhaseTechnologyType[TrfPhaseTechnology(t_type.nt2ph).name]
 
             # Transformer Tap Changer
             tap_u_abs = t_type.dutap
             tap_u_phi = t_type.phitr
             tap_min = t_type.ntpmn
             tap_max = t_type.ntpmx
             tap_neutral = t_type.nntap0
-            tap_side = self.transformer_tap_side(t_type)
+            tap_side = TapSide[TrfTapSide(t_type.tap_side).name] if t_type.itapch else None
 
             if bool(t_type.itapch2) is True:
                 logger.warning(
                     "2-winding transformer {transformer_name} has second tap changer. Not supported so far. Skipping.",
                     transformer_name=name,
                 )
                 return None
@@ -765,42 +730,69 @@
             pu2abs = u_ref_h**2 / s_r
             r_1 = t_type.r1pu * pu2abs
             r_0 = t_type.r0pu * pu2abs
             x_1 = t_type.x1pu * pu2abs
             x_0 = t_type.x0pu * pu2abs
 
             # Wiring group
-            vector_phase_angle_clock = t_type.nt2ag
+            vector_group = TVectorGroup[VectorGroup(t_type.vecgrp).name]
             vector_group_h = WVectorGroup[Vector(t_type.tr2cn_h).name]
             vector_group_l = WVectorGroup[Vector(t_type.tr2cn_l).name]
+            vector_phase_angle_clock = t_type.nt2ag
+
+            # Neutral point phase connection
+            neutral_connected_h, neutral_connected_l = self.transformer_neutral_connection_hvlv(
+                transformer_2w,
+                vector_group,
+            )
+
+            # Neutral point earthing
+            if "N" in vector_group_h and transformer_2w.cgnd_h == TrfNeutralPointState.EARTHED:
+                re_h = transformer_2w.re0tr_h
+                xe_h = transformer_2w.xe0tr_h
+            else:
+                re_h = None
+                xe_h = None
+            if "N" in vector_group_l and transformer_2w.cgnd_l == TrfNeutralPointState.EARTHED:
+                re_l = transformer_2w.re0tr_l
+                xe_l = transformer_2w.xe0tr_l
+            else:
+                re_l = None
+                xe_l = None
 
             wh = Winding(
                 node=t_high_name,
                 s_r=round(s_r * Exponents.POWER, DecimalDigits.POWER),
                 u_r=round(u_ref_h * Exponents.VOLTAGE, DecimalDigits.VOLTAGE),
                 u_n=round(u_nom_h * Exponents.VOLTAGE, DecimalDigits.VOLTAGE),
                 r1=r_1,
                 r0=r_0,
                 x1=x_1,
                 x0=x_0,
+                re_h=re_h,
+                xe_h=xe_h,
                 vector_group=vector_group_h,
                 phase_angle_clock=0,
+                neutral_connected=neutral_connected_h,
             )
 
             wl = Winding(
                 node=t_low_name,
                 s_r=round(s_r * Exponents.POWER, DecimalDigits.POWER),
                 u_r=round(u_ref_l * Exponents.VOLTAGE, DecimalDigits.VOLTAGE),
                 u_n=round(u_nom_l * Exponents.VOLTAGE, DecimalDigits.VOLTAGE),
                 r1=float(0),
                 r0=float(0),
                 x1=float(0),
                 x0=float(0),
+                re_l=re_l,
+                xe_l=xe_l,
                 vector_group=vector_group_l,
                 phase_angle_clock=int(vector_phase_angle_clock),
+                neutral_connected=neutral_connected_l,
             )
 
             return Transformer(
                 node_1=t_high_name,
                 node_2=t_low_name,
                 name=name,
                 number=t_number,
@@ -818,46 +810,39 @@
                 windings=[wh, wl],
             )
 
         logger.warning("Type not set for 2-winding transformer {transformer_name}. Skipping.", transformer_name=name)
         return None
 
     @staticmethod
+    def transformer_neutral_connection_hvlv(t: PFTypes.Transformer2W, vector_group: VectorGroup) -> tuple[bool, bool]:
+        if "n" in vector_group.name.lower():
+            if t.cneutcon == TrfNeutralConnectionType.ABC_N:
+                return True, True
+            if t.cneutcon == TrfNeutralConnectionType.HV:
+                return True, False
+            if t.cneutcon == TrfNeutralConnectionType.LV:
+                return False, True
+            if t.cneutcon == TrfNeutralConnectionType.HV_LV:
+                return True, True
+        return False, False  # corresponds to TrfNeutralConnectionType.NO
+
+    @staticmethod
     def get_description(
         element: PFTypes.Terminal | PFTypes.LineBase | PFTypes.Element | PFTypes.Coupler | PFTypes.ExternalGrid,
     ) -> tuple[bool, str]:
         desc = element.desc
         if desc:
             if desc[0] == "do_not_export":
                 return False, ""
 
             return True, desc[0]
 
         return True, ""
 
-    @staticmethod
-    def transformer_phase_technology(t_type: PFTypes.Transformer2WType) -> TransformerPhaseTechnologyType | None:
-        tech_mapping = {
-            1: TransformerPhaseTechnologyType.SINGLE_PH_E,
-            2: TransformerPhaseTechnologyType.SINGLE_PH,
-            3: TransformerPhaseTechnologyType.THREE_PH,
-        }
-        return tech_mapping[t_type.nt2ph]
-
-    @staticmethod
-    def transformer_tap_side(t_type: PFTypes.Transformer2WType) -> TapSide | None:
-        side_mapping_2w = {
-            0: TapSide.HV,
-            1: TapSide.LV,
-        }
-        if t_type.itapch:
-            return side_mapping_2w.get(t_type.tap_side)
-
-        return None
-
     def create_loads(  # noqa: PLR0913 # fix
         self,
         consumers: Sequence[PFTypes.Load],
         consumers_lv: Sequence[PFTypes.LoadLV],
         consumers_mv: Sequence[PFTypes.LoadMV],
         generators: Sequence[PFTypes.Generator],
         pv_systems: Sequence[PFTypes.PVSystem],
@@ -2140,85 +2125,80 @@
     def create_q_controller_builtin(  # noqa: PLR0911
         self,
         gen: PFTypes.GeneratorBase,
         u_n: float,
     ) -> Controller | None:
         logger.debug("Creating producer {gen_name} internal Q controller...", gen_name=gen.loc_name)
         if gen.bus1 is not None:
-            node_target = self.pfi.create_name(gen.bus1.cterm, self.grid_name)
+            node_target_name = self.pfi.create_name(gen.bus1.cterm, self.grid_name)
         else:
             return None
 
         av_mode = LocalQCtrlMode(gen.av_mode)
 
         if av_mode == LocalQCtrlMode.COSPHI_CONST:
             cosphi = gen.cosgini
             cosphi_dir = CosphiDir.UE if gen.pf_recap == 1 else CosphiDir.UE
             q_controller: ControlType = ControlCosphiConst(
-                node_target=node_target,
                 cosphi=round(cosphi, DecimalDigits.COSPHI),
                 cosphi_dir=cosphi_dir,
             )
-            return Controller(control_type=q_controller)
+            return Controller(node_target=node_target_name, control_type=q_controller)
 
         if av_mode == LocalQCtrlMode.Q_CONST:
             q_set = gen.qgini * -1  # has to be negative as power is now counted demand based
             q_controller = ControlQConst(
-                node_target=node_target,
                 q_set=round(q_set * Exponents.POWER * gen.ngnum, DecimalDigits.POWER),
             )
-            return Controller(control_type=q_controller)
+            return Controller(node_target=node_target_name, control_type=q_controller)
 
         if av_mode == LocalQCtrlMode.Q_U:
             cosphi_a = gen.cosn
             q_max_ue = abs(gen.Qfu_min)  # absolute value
             q_max_oe = abs(gen.Qfu_max)  # absolute value
             u_q0 = gen.udeadbup - (gen.udeadbup - gen.udeadblow) / 2  # p.u.
             u_deadband_low = abs(u_q0 - gen.udeadblow)  # delta in p.u.
             u_deadband_up = abs(u_q0 - gen.udeadbup)  # delta in p.u.
             m_tg_2015 = 100 / abs(gen.ddroop) * 100 / u_n / cosphi_a * Exponents.VOLTAGE  # (% von Pr) / kV
             m_tg_2018 = self.transform_qu_slope(slope=m_tg_2015, given_format="2015", target_format="2018", u_n=u_n)
             q_controller = ControlQU(
-                node_target=node_target,
                 m_tg_2015=round(m_tg_2015, DecimalDigits.PU),
                 m_tg_2018=round(m_tg_2018, DecimalDigits.PU),
                 u_q0=round(u_q0 * u_n, DecimalDigits.VOLTAGE),
                 u_deadband_up=round(u_deadband_up * u_n, DecimalDigits.VOLTAGE),
                 u_deadband_low=round(u_deadband_low * u_n, DecimalDigits.VOLTAGE),
                 q_max_ue=round(q_max_ue * Exponents.POWER * gen.ngnum, DecimalDigits.POWER),
                 q_max_oe=round(q_max_oe * Exponents.POWER * gen.ngnum, DecimalDigits.POWER),
             )
-            q_controller.control_strategy
-            return Controller(control_type=q_controller)
+            return Controller(node_target=node_target_name, control_type=q_controller)
 
         if av_mode == LocalQCtrlMode.Q_P:
             if gen.pQPcurve is None:
                 return None
 
-            q_controller = ControlQP(node_target=node_target, q_p_characteristic_name=gen.pQPcurve.loc_name)
-            return Controller(control_type=q_controller)
+            q_controller = ControlQP(q_p_characteristic_name=gen.pQPcurve.loc_name)
+            return Controller(node_target=node_target_name, control_type=q_controller)
 
         if av_mode == LocalQCtrlMode.COSPHI_P:
             cosphi_ue = gen.pf_under
             cosphi_oe = gen.pf_over
             p_threshold_ue = gen.p_under * -1  # P-threshold for cosphi_ue
             p_threshold_oe = gen.p_over * -1  # P-threshold for cosphi_oe
             q_controller = ControlCosphiP(
-                node_target=node_target,
                 cosphi_ue=round(cosphi_ue, DecimalDigits.COSPHI),
                 cosphi_oe=round(cosphi_oe, DecimalDigits.COSPHI),
                 p_threshold_ue=round(p_threshold_ue * Exponents.POWER * gen.ngnum, DecimalDigits.POWER),
                 p_threshold_oe=round(p_threshold_oe * Exponents.POWER * gen.ngnum, DecimalDigits.POWER),
             )
-            return Controller(control_type=q_controller)
+            return Controller(node_target=node_target_name, control_type=q_controller)
 
         if av_mode == LocalQCtrlMode.U_CONST:
             u_set = gen.usetp
-            q_controller = ControlUConst(node_target=node_target, u_set=round(u_set * u_n, DecimalDigits.VOLTAGE))
-            return Controller(control_type=q_controller)
+            q_controller = ControlUConst(u_set=round(u_set * u_n, DecimalDigits.VOLTAGE))
+            return Controller(node_target=node_target_name, control_type=q_controller)
 
         if av_mode == LocalQCtrlMode.U_Q_DROOP:
             logger.warning(
                 "Generator {gen_name}: Voltage control with Q-droop is not implemented yet. Skipping.",
                 gen_name=gen.loc_name,
             )
             return None
@@ -2260,27 +2240,31 @@
         ctrl_mode = controller.i_ctrl
         if ctrl_mode == CtrlMode.U:  # voltage control mode -> const. U
             u_set = controller.usetp
             u_meas_ref = ControlledVoltageRef[CtrlVoltageRef(controller.i_phase).name]
             q_controller: ControlType = ControlUConst(
                 u_set=round(u_set * u_n, DecimalDigits.VOLTAGE),
                 u_meas_ref=u_meas_ref,
+            )
+            return Controller(
                 node_target=node_target_name,
+                control_type=q_controller,
+                external_controller_name=controller_name,
             )
-            return Controller(control_type=q_controller, external_controller_name=controller_name)
 
         if ctrl_mode == CtrlMode.Q:  # reactive power control mode
             if controller.qu_char == QChar.CONST:  # const. Q
                 q_dir = -1 if controller.iQorient else 1
                 q_set = controller.qsetp * q_dir * -1  # has to be negative as power is now counted demand based
-                q_controller = ControlQConst(
-                    q_set=round(q_set * Exponents.POWER * gen.ngnum, DecimalDigits.POWER),
+                q_controller = ControlQConst(q_set=round(q_set * Exponents.POWER * gen.ngnum, DecimalDigits.POWER))
+                return Controller(
                     node_target=node_target_name,
+                    control_type=q_controller,
+                    external_controller_name=controller_name,
                 )
-                return Controller(control_type=q_controller, external_controller_name=controller_name)
 
             if controller.qu_char == QChar.U:  # Q(U)
                 s_r = gen.sgn
                 cosphi_a = gen.cosn
                 u_nom = round(controller.refbar.uknom * Exponents.VOLTAGE, DecimalDigits.VOLTAGE)  # voltage in V
 
                 q_max_ue = abs(controller.Qmin)
@@ -2319,88 +2303,106 @@
                     m_tg_2015=round(m_tg_2015, DecimalDigits.PU),
                     m_tg_2018=round(m_tg_2018, DecimalDigits.PU),
                     u_q0=round(u_q0 * u_n, DecimalDigits.VOLTAGE),
                     u_deadband_up=round(u_deadband_up * u_n, DecimalDigits.VOLTAGE),
                     u_deadband_low=round(u_deadband_low * u_n, DecimalDigits.VOLTAGE),
                     q_max_ue=round(q_max_ue * Exponents.POWER * gen.ngnum, DecimalDigits.POWER),
                     q_max_oe=round(q_max_oe * Exponents.POWER * gen.ngnum, DecimalDigits.POWER),
+                )
+                return Controller(
                     node_target=node_target_name,
+                    control_type=q_controller,
+                    external_controller_name=controller_name,
                 )
-                return Controller(control_type=q_controller, external_controller_name=controller_name)
 
             if controller.qu_char == QChar.P:  # Q(P)
                 q_p_char_name = controller.pQPcurve.loc_name
                 q_max_ue = abs(controller.Qmin)
                 q_max_oe = abs(controller.Qmax)
                 q_dir = q_dir = -1 if controller.iQorient else 1
                 q_controller = ControlQP(
                     q_p_characteristic_name=q_p_char_name,
                     q_max_ue=round(q_max_ue * Exponents.POWER * gen.ngnum, DecimalDigits.POWER),
                     q_max_oe=round(q_max_oe * Exponents.POWER * gen.ngnum, DecimalDigits.POWER),
+                )
+                return Controller(
                     node_target=node_target_name,
+                    control_type=q_controller,
+                    external_controller_name=controller_name,
                 )
-                return Controller(control_type=q_controller, external_controller_name=controller_name)
 
             msg = "unreachable"
             raise RuntimeError(msg)
 
         if ctrl_mode == CtrlMode.COSPHI:  # cosphi control mode
             if controller.cosphi_char == CosphiChar.CONST:  # const. cosphi
                 cosphi = controller.pfsetp
                 ue = controller.pf_recap ^ controller.iQorient  # OE/UE XOR +Q/-Q
                 # in PF for producer: ind. cosphi = over excited; cap. cosphi = under excited
                 q_dir = q_dir = -1 if controller.iQorient else 1
                 cosphi_dir = CosphiDir.UE if ue else CosphiDir.OE
                 q_controller = ControlCosphiConst(
                     cosphi=round(cosphi, DecimalDigits.COSPHI),
                     cosphi_dir=cosphi_dir,
+                )
+                return Controller(
                     node_target=node_target_name,
+                    control_type=q_controller,
+                    external_controller_name=controller_name,
                 )
-                return Controller(control_type=q_controller, external_controller_name=controller_name)
 
             if controller.cosphi_char == CosphiChar.P:  # cosphi(P)
                 cosphi_ue = controller.pf_under
                 cosphi_oe = controller.pf_over
                 p_threshold_ue = controller.p_under * -1  # P-threshold for cosphi_ue
                 p_threshold_oe = controller.p_over * -1  # P-threshold for cosphi_oe
                 q_controller = ControlCosphiP(
                     cosphi_ue=round(cosphi_ue, DecimalDigits.COSPHI),
                     cosphi_oe=round(cosphi_oe, DecimalDigits.COSPHI),
                     p_threshold_ue=round(p_threshold_ue * Exponents.POWER * gen.ngnum, DecimalDigits.POWER),
                     p_threshold_oe=round(p_threshold_oe * Exponents.POWER * gen.ngnum, DecimalDigits.POWER),
+                )
+                return Controller(
                     node_target=node_target_name,
+                    control_type=q_controller,
+                    external_controller_name=controller_name,
                 )
-                return Controller(control_type=q_controller, external_controller_name=controller_name)
 
             if controller.cosphi_char == CosphiChar.U:  # cosphi(U)
                 cosphi_ue = controller.pf_under
                 cosphi_oe = controller.pf_over
                 u_threshold_ue = controller.u_under  # U-threshold for cosphi_ue
                 u_threshold_oe = controller.u_over  # U-threshold for cosphi_oe
                 q_controller = ControlCosphiU(
                     cosphi_ue=round(cosphi_ue, DecimalDigits.COSPHI),
                     cosphi_oe=round(cosphi_oe, DecimalDigits.COSPHI),
                     u_threshold_ue=round(u_threshold_ue * u_n, DecimalDigits.VOLTAGE),
                     u_threshold_oe=round(u_threshold_oe * u_n, DecimalDigits.VOLTAGE),
+                )
+                return Controller(
                     node_target=node_target_name,
+                    control_type=q_controller,
+                    external_controller_name=controller_name,
                 )
-                return Controller(control_type=q_controller, external_controller_name=controller_name)
 
             msg = "unreachable"
             raise RuntimeError(msg)
 
         if ctrl_mode == CtrlMode.TANPHI:  # tanphi control mode --> const. tanphi
             cosphi = math.cos(math.atan(controller.tansetp))
             cosphi_dir = CosphiDir.UE if controller.iQorient else CosphiDir.OE
             q_controller = ControlTanphiConst(
                 cosphi=round(cosphi, DecimalDigits.COSPHI),
                 cosphi_dir=cosphi_dir,
+            )
+            return Controller(
                 node_target=node_target_name,
+                control_type=q_controller,
+                external_controller_name=controller_name,
             )
-            return Controller(control_type=q_controller, external_controller_name=controller_name)
 
         msg = "unreachable"
         raise RuntimeError(msg)
 
     @staticmethod
     def transform_qu_slope(
         slope: float,
```

### Comparing `ieeh-powerfactory-tools-1.4.2/powerfactory_tools/exporter/load_power.py` & `ieeh-powerfactory-tools-1.5.0/powerfactory_tools/exporter/load_power.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from __future__ import annotations
 
 import math
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 from loguru import logger
+from psdm.base import CosphiDir
+from psdm.steadystate_case.active_power import ActivePower
+from psdm.steadystate_case.reactive_power import ReactivePower
+from psdm.topology.load import RatedPower
 
 from powerfactory_tools.constants import DecimalDigits
 from powerfactory_tools.constants import Exponents
-from powerfactory_tools.schema.base import CosphiDir
-from powerfactory_tools.schema.steadystate_case.active_power import ActivePower
-from powerfactory_tools.schema.steadystate_case.reactive_power import ReactivePower
-from powerfactory_tools.schema.topology.load import RatedPower
 
 if TYPE_CHECKING:
     from typing import TypedDict
 
-    from powerfactory_tools.schema.steadystate_case.controller import Controller
+    from psdm.steadystate_case.controller import Controller
 
     class PowerDict(TypedDict):
         power_apparent: float
         power_active: float
         power_reactive: float
         cosphi: float
         cosphi_dir: CosphiDir
@@ -159,15 +159,15 @@
         voltage: float,
         current: float,
         cosphi: float,
         cosphi_dir: CosphiDir,
         scaling: float,
     ) -> PowerDict:
         pow_app = abs(voltage * current * scaling) * Exponents.POWER / math.sqrt(3)
-        pow_act = pow_app * cosphi
+        pow_act = math.copysign(pow_app * cosphi, scaling)
         fac = 1 if cosphi_dir == CosphiDir.UE else -1
         pow_react = fac * math.sqrt(pow_app**2 - pow_act**2)
         return {
             "power_apparent": pow_app,
             "power_active": pow_act,
             "power_reactive": pow_react,
             "cosphi": cosphi,
@@ -179,15 +179,15 @@
         *,
         pow_app: float,
         cosphi: float,
         cosphi_dir: CosphiDir,
         scaling: float,
     ) -> PowerDict:
         pow_app = abs(pow_app * scaling) * Exponents.POWER
-        pow_act = pow_app * cosphi
+        pow_act = math.copysign(pow_app * cosphi, scaling)
         fac = 1 if cosphi_dir == CosphiDir.UE else -1
         pow_react = fac * math.sqrt(pow_app**2 - pow_act**2)
         return {
             "power_apparent": pow_app,
             "power_active": pow_act,
             "power_reactive": pow_react,
             "cosphi": cosphi,
@@ -211,15 +211,15 @@
                 "power_apparent": 0,
                 "power_active": 0,
                 "power_reactive": 0,
                 "cosphi": COSPHI_DEFAULT,
                 "cosphi_dir": cosphi_dir,
             }
 
-        pow_act = pow_app * cosphi
+        pow_act = math.copysign(pow_app * cosphi, scaling)
         return {
             "power_apparent": pow_app,
             "power_active": pow_act,
             "power_reactive": pow_react,
             "cosphi": cosphi,
             "cosphi_dir": cosphi_dir,
         }
@@ -280,15 +280,15 @@
         *,
         pow_app: float,
         pow_react: float,
         scaling: float,
     ) -> PowerDict:
         pow_app = abs(pow_app * scaling) * Exponents.POWER
         pow_react = pow_react * scaling * Exponents.POWER
-        pow_act = math.sqrt(pow_app**2 - pow_react**2)
+        pow_act = math.copysign(math.sqrt(pow_app**2 - pow_react**2), scaling)
         try:
             cosphi = abs(pow_act / pow_app)
         except ZeroDivisionError:
             cosphi = COSPHI_DEFAULT
 
         cosphi_dir = CosphiDir.OE if pow_react < 0 else CosphiDir.UE
         return {
```

### Comparing `ieeh-powerfactory-tools-1.4.2/powerfactory_tools/interface.py` & `ieeh-powerfactory-tools-1.5.0/powerfactory_tools/interface.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,57 +2,62 @@
 # :author: Sebastian Krahmer <sebastian.krahmer@tu-dresden.de>
 # :copyright: Copyright (c) Institute of Electrical Power Systems and High Voltage Engineering - TU Dresden, 2022-2023.
 # :license: BSD 3-Clause
 
 from __future__ import annotations
 
 import contextlib
+import dataclasses
+import datetime
 import importlib.util
 import itertools
 import pathlib
-import typing
-from collections.abc import Sequence  # noqa: TCH003 # bug
-from typing import TYPE_CHECKING
+import typing as t
+from collections.abc import Sequence
 
 import pydantic
 from loguru import logger
 
 from powerfactory_tools.constants import BaseUnits
 from powerfactory_tools.powerfactory_types import Currency
 from powerfactory_tools.powerfactory_types import MetricPrefix
 from powerfactory_tools.powerfactory_types import UnitSystem
-from powerfactory_tools.schema.base import Base
 
-if TYPE_CHECKING:
+if t.TYPE_CHECKING:
     from collections.abc import Iterable
-    from typing import Any
-    from typing import TypeVar
+    from types import TracebackType
 
     from powerfactory_tools.powerfactory_types import PowerFactoryTypes as PFTypes
 
-    T = TypeVar("T")
+    T = t.TypeVar("T")
 
 POWERFACTORY_PATH = pathlib.Path("C:/Program Files/DIgSILENT")
 POWERFACTORY_VERSION = "2022 SP2"
 PYTHON_VERSION = "3.10"
 PATH_SEP = "/"
 
 
-class UnitConversionSetting(Base):
+class Config:
+    use_enum_values = True
+
+
+@pydantic.dataclasses.dataclass(config=Config)
+class UnitConversionSetting:
     filtclass: Sequence[str]
     filtvar: str
     digunit: str
     cdigexp: MetricPrefix
     userunit: str
     cuserexp: MetricPrefix
     ufacA: float  # noqa: N815
     ufacB: float  # noqa: N815
 
 
-class ProjectUnitSetting(Base):
+@pydantic.dataclasses.dataclass(config=Config)
+class ProjectUnitSetting:
     ilenunit: UnitSystem
     clenexp: MetricPrefix  # Lengths
     cspqexp: MetricPrefix  # Loads etc.
     cspqexpgen: MetricPrefix  # Generators etc.
     currency: Currency
 
 
@@ -61,52 +66,90 @@
     clenexp=BaseUnits.LENGTH,
     cspqexp=BaseUnits.POWER,
     cspqexpgen=BaseUnits.POWER,
     currency=BaseUnits.CURRENCY,
 )
 
 
+@dataclasses.dataclass
+class PowerFactoryData:
+    name: str
+    date: datetime.date
+    project: str
+    external_grids: Sequence[PFTypes.ExternalGrid]
+    terminals: Sequence[PFTypes.Terminal]
+    lines: Sequence[PFTypes.Line]
+    transformers_2w: Sequence[PFTypes.Transformer2W]
+    transformers_3w: Sequence[PFTypes.Transformer3W]
+    loads: Sequence[PFTypes.Load]
+    loads_lv: Sequence[PFTypes.LoadLV]
+    loads_mv: Sequence[PFTypes.LoadMV]
+    generators: Sequence[PFTypes.Generator]
+    pv_systems: Sequence[PFTypes.PVSystem]
+    couplers: Sequence[PFTypes.Coupler]
+    switches: Sequence[PFTypes.Switch]
+    fuses: Sequence[PFTypes.Fuse]
+    ac_current_sources: Sequence[PFTypes.AcCurrentSource]
+
+
 @pydantic.dataclasses.dataclass
 class PowerFactoryInterface:
     project_name: str
     powerfactory_user_profile: str | None = None
+    powerfactory_user_password: str | None = None
     powerfactory_path: pathlib.Path = POWERFACTORY_PATH
     powerfactory_version: str = POWERFACTORY_VERSION
+    powerfactory_ini_name: str | None = None
     python_version: str = PYTHON_VERSION
 
     def __post_init__(self) -> None:
         try:
             logger.info("Starting PowerFactory Interface...")
             pf = self.load_powerfactory_module_from_path()
             self.app = self.connect_to_app(pf)
             self.project = self.connect_to_project(self.project_name)
-            self.load_project_folders_from_pf_db()
+            self.load_project_setting_folders_from_pf_db()
             self.stash_unit_conversion_settings()
             self.set_default_unit_conversion()
+            self.load_project_folders_from_pf_db()
             logger.info("Starting PowerFactory Interface... Done.")
         except RuntimeError:
             logger.exception("Could not start PowerFactory Interface. Shutting down...")
             self.close()
 
+    def __enter__(self) -> PowerFactoryInterface:
+        return self
+
+    def __exit__(
+        self,
+        exc_type: type[BaseException],
+        exc_val: BaseException,
+        exc_tb: TracebackType,
+    ) -> None:
+        self.close()
+
+    def load_project_setting_folders_from_pf_db(self) -> None:
+        self.project_settings = self.load_project_settings_dir_from_pf()
+        self.settings_dir = self.load_settings_dir_from_pf()
+        self.unit_settings_dir = self.load_unit_settings_dir_from_pf()
+
     def load_project_folders_from_pf_db(self) -> None:
+        self.load_project_setting_folders_from_pf_db()
+
         self.grid_model = self.app.GetProjectFolder("netmod")
         self.types_dir = self.app.GetProjectFolder("equip")
         self.op_dir = self.app.GetProjectFolder("oplib")
         self.chars_dir = self.app.GetProjectFolder("chars")
 
-        project_settings_dir = self.load_project_settings_dir_from_pf()
-
-        self.ext_data_dir = project_settings_dir.extDataDir
-
         self.grid_data = self.app.GetProjectFolder("netdat")
         self.study_case_dir = self.app.GetProjectFolder("study")
         self.scenario_dir = self.app.GetProjectFolder("scen")
         self.grid_graphs_dir = self.app.GetProjectFolder("dia")
-        self.settings_dir = self.load_settings_dir_from_pf()
-        self.unit_settings_dir = self.load_unit_settings_dir_from_pf()
+
+        self.ext_data_dir = self.project_settings.extDataDir
 
     def load_powerfactory_module_from_path(self) -> PFTypes.PowerFactoryModule:
         logger.debug("Loading PowerFactory Python module...")
         module_path = (
             self.powerfactory_path / ("PowerFactory " + self.powerfactory_version) / "Python" / self.python_version
         )
         spec = importlib.util.spec_from_file_location(
@@ -115,34 +158,36 @@
         )
         if (spec is None) or (spec.loader is None):
             msg = "Could not load PowerFactory Module."
             raise RuntimeError(msg)
 
         pfm = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(pfm)
-        return typing.cast("PFTypes.PowerFactoryModule", pfm)
+        return t.cast("PFTypes.PowerFactoryModule", pfm)
 
     def load_settings_dir_from_pf(self) -> PFTypes.DataDir:
         logger.debug("Loading settings from PowerFactory...")
-        settings_dir = self.element_of(element=self.project, pattern="*.SetFold", recursive=False)
+        _settings_dirs = self.elements_of(element=self.project, pattern="*.SetFold", recursive=False)
+        settings_dir = self.first_of(elements=_settings_dirs)
         if settings_dir is None:
             msg = "Could not access settings."
             raise RuntimeError(msg)
 
         logger.debug("Loading settings from PowerFactory... Done.")
-        return typing.cast("PFTypes.DataDir", settings_dir)
+        return t.cast("PFTypes.DataDir", settings_dir)
 
     def load_unit_settings_dir_from_pf(self) -> PFTypes.DataDir | None:
         logger.debug("Loading unit settings from PowerFactory...")
-        unit_settings_dir = self.element_of(element=self.settings_dir, pattern="*.IntUnit", recursive=False)
+        _unit_settings_dirs = self.elements_of(element=self.settings_dir, pattern="*.IntUnit", recursive=False)
+        unit_settings_dir = self.first_of(elements=_unit_settings_dirs)
         if unit_settings_dir is None:
             return None
 
         logger.debug("Loading unit settings from PowerFactory... Done.")
-        return typing.cast("PFTypes.DataDir", unit_settings_dir)
+        return t.cast("PFTypes.DataDir", unit_settings_dir)
 
     def close(self) -> None:
         logger.info("Closing PowerFactory Interface...")
         with contextlib.suppress(AttributeError):
             self.pop_unit_conversion_settings_stash()
 
         with contextlib.suppress(AttributeError):
@@ -157,41 +202,124 @@
             pf {PFTypes.PowerFactoryModule} -- the Python module contributed via the PowerFactory system installation
 
         Returns:
             PFTypes.Application -- the application handle (root)
         """
 
         logger.debug("Connecting to PowerFactory application...")
+        if self.powerfactory_ini_name is None:
+            command_line_arg = None
+        else:
+            ini_path = (
+                self.powerfactory_path
+                / ("PowerFactory " + self.powerfactory_version)
+                / (self.powerfactory_ini_name + ".ini")
+            )
+            command_line_arg = '/ini "' + str(ini_path) + '"'
         try:
-            return pf.GetApplicationExt(self.powerfactory_user_profile)
+            return pf.GetApplicationExt(
+                self.powerfactory_user_profile,
+                self.powerfactory_user_password,
+                command_line_arg,
+            )
         except pf.ExitError as element:
             msg = "Could not start application."
             raise RuntimeError(msg) from element
 
     def connect_to_project(self, project_name: str) -> PFTypes.Project:
         """Connect to a PowerFactory project.
 
         Arguments:
             project_name {str} -- the name of the project to be connected/activated
 
         Returns:
             PFTypes.Project -- the project handle
         """
 
-        logger.debug("Activating project {project_name} application...", project_name=project_name)
+        logger.debug(
+            "Activating project {project_name} application...",
+            project_name=project_name,
+        )
         self.activate_project(project_name)
 
         project = self.app.GetActiveProject()
         if project is None:
             msg = "Could not access project."
             raise RuntimeError(msg)
 
-        logger.debug("Activating project {project_name} application... Done.", project_name=project_name)
+        logger.debug(
+            "Activating project {project_name} application... Done.",
+            project_name=project_name,
+        )
         return project
 
+    def switch_study_case(self, sc: str) -> None:
+        study_case = self.study_case(name=sc)
+        if study_case is not None:
+            self.activate_study_case(study_case)
+        else:
+            msg = f"Study case {sc} does not exist."
+            raise RuntimeError(msg)
+
+    def switch_scenario(self, scen: str) -> None:
+        scenario = self.scenario(name=scen)
+        if scenario is not None:
+            self.activate_scenario(scenario)
+        else:
+            msg = f"Scenario {scen} does not exist."
+            raise RuntimeError(msg)
+
+    def compile_powerfactory_data(self, grid_name: str) -> PowerFactoryData:
+        logger.debug("Compiling data from PowerFactory...")
+        if grid_name == "*":
+            name = self.project_name
+        else:
+            grids = self.grids()
+            try:
+                grid = [e for e in grids if e.loc_name == grid_name][0]
+                name = grid.loc_name
+            except IndexError as e:
+                msg = f"Grid {grid_name} does not exist."
+                raise RuntimeError(msg) from e
+
+        project_name = self.project.loc_name
+        date = datetime.datetime.now().astimezone().date()  # noqa: DTZ005
+
+        return PowerFactoryData(
+            name=name,
+            date=date,
+            project=project_name,
+            external_grids=self.external_grids(grid=grid_name),
+            terminals=self.terminals(grid=grid_name),
+            lines=self.lines(grid=grid_name),
+            transformers_2w=self.transformers_2w(grid=grid_name),
+            transformers_3w=self.transformers_3w(grid=grid_name),
+            loads=self.loads(grid=grid_name),
+            loads_lv=self.loads_lv(grid=grid_name),
+            loads_mv=self.loads_mv(grid=grid_name),
+            generators=self.generators(grid=grid_name),
+            pv_systems=self.pv_systems(grid=grid_name),
+            couplers=self.couplers(grid=grid_name),
+            switches=self.switches(grid=grid_name),
+            fuses=self.fuses(grid=grid_name),
+            ac_current_sources=self.ac_current_sources(grid=grid_name),
+        )
+
+    def set_result_variables(
+        self,
+        *,
+        result: PFTypes.Result,
+        elements: Sequence[PFTypes.DataObject],
+        variables: Sequence[str],
+    ) -> None:
+        logger.debug("Set Variables for result object {result_name} ...", result_name=result.loc_name)
+        for elm in elements:
+            for variable in variables:
+                result.AddVariable(elm, variable)
+
     def activate_grid(self, grid: PFTypes.Grid) -> None:
         logger.debug("Activating grid {grid_name} application...", grid_name=grid.loc_name)
         if grid.Activate():
             msg = "Could not activate grid."
             raise RuntimeError(msg)
 
     def deactivate_grids(self) -> None:
@@ -201,46 +329,57 @@
     def deactivate_grid(self, grid: PFTypes.Grid) -> None:
         logger.debug("Deactivating grid {grid_name} application...", grid_name=grid.loc_name)
         if grid.Deactivate():
             msg = "Could not deactivate grid."
             raise RuntimeError(msg)
 
     def activate_scenario(self, scen: PFTypes.Scenario) -> None:
-        logger.debug("Activating scenario {scenario_name} application...", scenario_name=scen.loc_name)
+        logger.debug(
+            "Activating scenario {scenario_name} application...",
+            scenario_name=scen.loc_name,
+        )
         active_scen = self.app.GetActiveScenario()
         if active_scen != scen and scen.Activate():
             msg = "Could not activate scenario."
             raise RuntimeError(msg)
 
     def deactivate_scenario(self, scen: PFTypes.Scenario) -> None:
-        logger.debug("Deactivating scenario {scenario_name} application...", scenario_name=scen.loc_name)
+        logger.debug(
+            "Deactivating scenario {scenario_name} application...",
+            scenario_name=scen.loc_name,
+        )
         if scen.Deactivate():
             msg = "Could not deactivate scenario."
             raise RuntimeError(msg)
 
     def activate_study_case(self, stc: PFTypes.StudyCase) -> None:
-        logger.debug("Activating study_case {study_case_name} application...", study_case_name=stc.loc_name)
+        logger.debug(
+            "Activating study_case {study_case_name} application...",
+            study_case_name=stc.loc_name,
+        )
         if stc.Activate():
             msg = "Could not activate case study."
             raise RuntimeError(msg)
 
     def deactivate_study_case(self, stc: PFTypes.StudyCase) -> None:
-        logger.debug("Deactivating study_case {study_case_name} application...", study_case_name=stc.loc_name)
+        logger.debug(
+            "Deactivating study_case {study_case_name} application...",
+            study_case_name=stc.loc_name,
+        )
         if stc.Deactivate():
             msg = "Could not deactivate case study."
             raise RuntimeError(msg)
 
     def set_default_unit_conversion(self) -> None:
         logger.debug("Applying exporter default unit conversion settings...")
-        project_settings = self.load_project_settings_dir_from_pf()
-        project_settings.ilenunit = DEFAULT_PROJECT_UNIT_SETTING.ilenunit
-        project_settings.clenexp = DEFAULT_PROJECT_UNIT_SETTING.clenexp
-        project_settings.cspqexp = DEFAULT_PROJECT_UNIT_SETTING.cspqexp
-        project_settings.cspqexpgen = DEFAULT_PROJECT_UNIT_SETTING.cspqexpgen
-        project_settings.currency = DEFAULT_PROJECT_UNIT_SETTING.currency
+        self.project_settings.ilenunit = DEFAULT_PROJECT_UNIT_SETTING.ilenunit
+        self.project_settings.clenexp = DEFAULT_PROJECT_UNIT_SETTING.clenexp
+        self.project_settings.cspqexp = DEFAULT_PROJECT_UNIT_SETTING.cspqexp
+        self.project_settings.cspqexpgen = DEFAULT_PROJECT_UNIT_SETTING.cspqexpgen
+        self.project_settings.currency = DEFAULT_PROJECT_UNIT_SETTING.currency
         for cls, data in BaseUnits.UNITCONVERSIONS.items():
             for unit, base_exp, exp in data:
                 name = f"{cls}-{unit}"
                 uc = UnitConversionSetting(
                     filtclass=[cls],
                     filtvar="*",
                     digunit=unit,
@@ -253,21 +392,20 @@
                 self.create_unit_conversion_setting(name, uc)
 
         self.reset_project()
         logger.debug("Applying exporter default unit conversion settings... Done.")
 
     def stash_unit_conversion_settings(self) -> None:
         logger.debug("Stashing PowerFactory default unit conversion settings...")
-        project_settings = self.load_project_settings_dir_from_pf()
         self.project_unit_setting = ProjectUnitSetting(
-            ilenunit=UnitSystem(project_settings.ilenunit),
-            clenexp=MetricPrefix(project_settings.clenexp),
-            cspqexp=MetricPrefix(project_settings.cspqexp),
-            cspqexpgen=MetricPrefix(project_settings.cspqexpgen),
-            currency=Currency(project_settings.currency),
+            ilenunit=UnitSystem(self.project_settings.ilenunit),
+            clenexp=MetricPrefix(self.project_settings.clenexp),
+            cspqexp=MetricPrefix(self.project_settings.cspqexp),
+            cspqexpgen=MetricPrefix(self.project_settings.cspqexpgen),
+            currency=Currency(self.project_settings.currency),
         )
         unit_conversion_settings = self.unit_conversion_settings()
         self.unit_conv_settings: dict[str, UnitConversionSetting] = {}
         for uc in unit_conversion_settings:
             ucs = UnitConversionSetting(
                 filtclass=uc.filtclass,
                 filtvar=uc.filtvar,
@@ -281,20 +419,19 @@
             self.unit_conv_settings[uc.loc_name] = ucs
 
         self.delete_unit_conversion_settings()
         logger.debug("Stashing PowerFactory default unit conversion settings... Done.")
 
     def pop_unit_conversion_settings_stash(self) -> None:
         logger.debug("Applying PowerFactory default unit conversion settings...")
-        project_settings = self.load_project_settings_dir_from_pf()
-        project_settings.ilenunit = self.project_unit_setting.ilenunit
-        project_settings.clenexp = self.project_unit_setting.clenexp
-        project_settings.cspqexp = self.project_unit_setting.cspqexp
-        project_settings.cspqexpgen = self.project_unit_setting.cspqexpgen
-        project_settings.currency = self.project_unit_setting.currency
+        self.project_settings.ilenunit = self.project_unit_setting.ilenunit
+        self.project_settings.clenexp = self.project_unit_setting.clenexp
+        self.project_settings.cspqexp = self.project_unit_setting.cspqexp
+        self.project_settings.cspqexpgen = self.project_unit_setting.cspqexpgen
+        self.project_settings.currency = self.project_unit_setting.currency
         self.delete_unit_conversion_settings()
         for name, uc in self.unit_conv_settings.items():
             self.create_unit_conversion_setting(name, uc)
 
         self.reset_project()
         logger.debug("Applying PowerFactory default unit conversion settings... Done.")
 
@@ -324,254 +461,311 @@
         logger.debug("Deactivating current project {name}...")
         if self.project.Deactivate():
             msg = "Could not deactivate project."
             raise RuntimeError(msg)
 
     def subloads_of(self, load: PFTypes.LoadLV) -> Sequence[PFTypes.LoadLVP]:
         elements = self.elements_of(element=load, pattern="*.ElmLodlvp")
-        return [typing.cast("PFTypes.LoadLVP", element) for element in elements]
+        return [t.cast("PFTypes.LoadLVP", element) for element in elements]
+
+    def result(self, name: str = "*", study_case_name: str = "*") -> PFTypes.Result | None:
+        return self.first_of(elements=self.results(name=name, study_case_name=study_case_name))
+
+    def results(self, name: str = "*", study_case_name: str = "*") -> Sequence[PFTypes.Result]:
+        elements = self.study_case_elements(class_name="ElmRes", name=name, study_case_name=study_case_name)
+        return [t.cast("PFTypes.Result", element) for element in elements]
 
     def study_case(self, name: str = "*") -> PFTypes.StudyCase | None:
-        element = self.element_of(element=self.study_case_dir, pattern=name)
-        return typing.cast("PFTypes.StudyCase", element) if element is not None else None
+        return self.first_of(elements=self.study_cases(name=name))
 
     def study_cases(self, name: str = "*") -> Sequence[PFTypes.StudyCase]:
-        elements = self.elements_of(element=self.study_case_dir, pattern=name)
-        return [typing.cast("PFTypes.StudyCase", element) for element in elements]
+        elements = self.elements_of(element=self.study_case_dir, pattern=name + ".IntCase")
+        return [t.cast("PFTypes.StudyCase", element) for element in elements]
 
     def scenario(self, name: str = "*") -> PFTypes.Scenario | None:
-        element = self.element_of(element=self.scenario_dir, pattern=name)
-        return typing.cast("PFTypes.Scenario", element) if element is not None else None
+        return self.first_of(elements=self.scenarios(name=name))
 
     def scenarios(self, name: str = "*") -> Sequence[PFTypes.Scenario]:
         elements = self.elements_of(element=self.scenario_dir, pattern=name)
-        return [typing.cast("PFTypes.Scenario", element) for element in elements]
+        return [t.cast("PFTypes.Scenario", element) for element in elements]
 
     def line_type(self, name: str = "*") -> PFTypes.LineType | None:
-        element = self.grid_model_element("TypLne", name)
-        return typing.cast("PFTypes.LineType", element) if element is not None else None
+        return self.first_of(elements=self.line_types(name=name))
 
     def line_types(self, name: str = "*") -> Sequence[PFTypes.LineType]:
-        elements = self.grid_model_elements("TypLne", name)
-        return [typing.cast("PFTypes.LineType", element) for element in elements]
+        elements = self.equipment_type_elements("TypLne", name)
+        return [t.cast("PFTypes.LineType", element) for element in elements]
 
     def load_type(self, name: str = "*") -> PFTypes.DataObject | None:
-        return self.grid_model_element("TypLod", name)
+        return self.first_of(elements=self.load_types(name=name))
 
     def load_types(self, name: str = "*") -> Sequence[PFTypes.DataObject]:
-        return self.grid_model_elements("TypLod", name)
+        elements = self.equipment_type_elements("TypLod", name)
+        return [t.cast("PFTypes.LoadType", element) for element in elements]
 
     def transformer_2w_type(self, name: str = "*") -> PFTypes.Transformer2WType | None:
-        element = self.grid_model_element("TypTr2", name)
-        return typing.cast("PFTypes.Transformer2WType", element) if element is not None else None
+        return self.first_of(elements=self.transformer_2w_types(name=name))
 
     def transformer_2w_types(self, name: str = "*") -> Sequence[PFTypes.Transformer2WType]:
-        elements = self.grid_model_elements("TypTr2", name)
-        return [typing.cast("PFTypes.Transformer2WType", element) for element in elements]
+        elements = self.equipment_type_elements("TypTr2", name)
+        return [t.cast("PFTypes.Transformer2WType", element) for element in elements]
+
+    def harmonic_source_type(self, name: str = "*") -> PFTypes.HarmonicSourceType | None:
+        return self.first_of(elements=self.harmonic_source_types(name=name))
+
+    def harmonic_source_types(self, name: str = "*") -> Sequence[PFTypes.HarmonicSourceType]:
+        elements = self.equipment_type_elements("TypHmccur", name)
+        return [t.cast("PFTypes.HarmonicSourceType", element) for element in elements]
 
     def area(self, name: str = "*") -> PFTypes.DataObject | None:
-        return self.grid_model_element("ElmArea", name)
+        return self.first_of(elements=self.areas(name=name))
 
     def areas(self, name: str = "*") -> Sequence[PFTypes.DataObject]:
         return self.grid_model_elements("ElmArea", name)
 
     def zone(self, name: str = "*") -> PFTypes.DataObject | None:
-        return self.grid_model_element("ElmZone", name)
+        return self.first_of(elements=self.zones(name=name))
 
     def zones(self, name: str = "*") -> Sequence[PFTypes.DataObject]:
         return self.grid_model_elements("ElmZone", name)
 
     def grid_diagram(self, grid: str = "*") -> PFTypes.GridDiagram | None:
-        element = self.grid_element("IntGrfnet", grid=grid)
-        return typing.cast("PFTypes.GridDiagram", element) if element is not None else None
+        return self.first_of(elements=self.grid_diagrams(grid=grid))
 
     def grid_diagrams(self, grid: str = "*") -> Sequence[PFTypes.GridDiagram]:
         elements = self.grid_elements("IntGrfnet", grid=grid)
-        return [typing.cast("PFTypes.GridDiagram", element) for element in elements]
+        return [t.cast("PFTypes.GridDiagram", element) for element in elements]
 
     def external_grid(self, name: str = "*", grid: str = "*") -> PFTypes.ExternalGrid | None:
-        element = self.grid_element("ElmXNet", name, grid)
-        return typing.cast("PFTypes.ExternalGrid", element) if element is not None else None
+        return self.first_of(elements=self.external_grids(name=name, grid=grid))
 
     def external_grids(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.ExternalGrid]:
         elements = self.grid_elements("ElmXNet", name, grid)
-        return [typing.cast("PFTypes.ExternalGrid", element) for element in elements]
+        return [t.cast("PFTypes.ExternalGrid", element) for element in elements]
 
     def terminal(self, name: str = "*", grid: str = "*") -> PFTypes.Terminal | None:
-        element = self.grid_element("ElmTerm", name, grid)
-        return typing.cast("PFTypes.Terminal", element) if element is not None else None
+        return self.first_of(elements=self.terminals(name=name, grid=grid))
 
     def terminals(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.Terminal]:
         elements = self.grid_elements("ElmTerm", name, grid)
-        return [typing.cast("PFTypes.Terminal", element) for element in elements]
+        return [t.cast("PFTypes.Terminal", element) for element in elements]
 
     def cubicle(self, name: str = "*", grid: str = "*") -> PFTypes.StationCubicle | None:
-        element = self.grid_elements("StaCubic", name, grid)
-        return typing.cast("PFTypes.StationCubicle", element) if element is not None else None
+        return self.first_of(elements=self.cubicles(name=name, grid=grid))
 
     def cubicles(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.StationCubicle]:
         elements = self.grid_elements("StaCubic", name, grid)
-        return [typing.cast("PFTypes.StationCubicle", element) for element in elements]
+        return [t.cast("PFTypes.StationCubicle", element) for element in elements]
 
     def coupler(self, name: str = "*", grid: str = "*") -> PFTypes.Coupler | None:
-        element = self.grid_element("ElmCoup", name, grid)
-        return typing.cast("PFTypes.Coupler", element) if element is not None else None
+        return self.first_of(elements=self.couplers(name=name, grid=grid))
 
     def couplers(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.Coupler]:
         elements = self.grid_elements("ElmCoup", name, grid)
-        return [typing.cast("PFTypes.Coupler", element) for element in elements]
+        return [t.cast("PFTypes.Coupler", element) for element in elements]
 
     def switch(self, name: str = "*", grid: str = "*") -> PFTypes.Switch | None:
-        element = self.grid_element("StaSwitch", name, grid)
-        return typing.cast("PFTypes.Switch", element) if element is not None else None
+        return self.first_of(elements=self.switches(name=name, grid=grid))
 
     def switches(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.Switch]:
         elements = self.grid_elements("StaSwitch", name, grid)
-        return [typing.cast("PFTypes.Switch", element) for element in elements]
+        return [t.cast("PFTypes.Switch", element) for element in elements]
 
     def fuse(self, name: str = "*", grid: str = "*") -> PFTypes.Fuse | None:
-        element = self.grid_element("RelFuse", name, grid)
-        return typing.cast("PFTypes.Fuse", element) if element is not None else None
+        return self.first_of(elements=self.fuses(name=name, grid=grid))
 
     def fuses(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.Fuse]:
         elements = self.grid_elements("RelFuse", name, grid)
-        return [typing.cast("PFTypes.Fuse", element) for element in elements]
+        return [t.cast("PFTypes.Fuse", element) for element in elements]
 
     def line(self, name: str = "*", grid: str = "*") -> PFTypes.Line | None:
-        element = self.grid_element("ElmLne", name, grid)
-        return typing.cast("PFTypes.Line", element) if element is not None else None
+        return self.first_of(elements=self.lines(name=name, grid=grid))
 
     def lines(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.Line]:
         elements = self.grid_elements("ElmLne", name, grid)
-        return [typing.cast("PFTypes.Line", element) for element in elements]
+        return [t.cast("PFTypes.Line", element) for element in elements]
 
     def transformer_2w(self, name: str = "*", grid: str = "*") -> PFTypes.Transformer2W | None:
-        element = self.grid_element("ElmTr2", name, grid)
-        return typing.cast("PFTypes.Transformer2W", element) if element is not None else None
+        return self.first_of(elements=self.transformers_2w(name=name, grid=grid))
 
     def transformers_2w(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.Transformer2W]:
         elements = self.grid_elements("ElmTr2", name, grid)
-        return [typing.cast("PFTypes.Transformer2W", element) for element in elements]
+        return [t.cast("PFTypes.Transformer2W", element) for element in elements]
 
     def transformer_3w(self, name: str = "*", grid: str = "*") -> PFTypes.Transformer3W | None:
-        element = self.grid_element("ElmTr3", name, grid)
-        return typing.cast("PFTypes.Transformer3W", element) if element is not None else None
+        return self.first_of(elements=self.transformers_3w(name=name, grid=grid))
 
     def transformers_3w(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.Transformer3W]:
         elements = self.grid_elements("ElmTr3", name, grid)
-        return [typing.cast("PFTypes.Transformer3W", element) for element in elements]
+        return [t.cast("PFTypes.Transformer3W", element) for element in elements]
 
     def load(self, name: str = "*", grid: str = "*") -> PFTypes.Load | None:
-        element = self.grid_element("ElmLod", name, grid)
-        return typing.cast("PFTypes.Load", element) if element is not None else None
+        return self.first_of(elements=self.loads(name=name, grid=grid))
 
     def loads(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.Load]:
         elements = self.grid_elements("ElmLod", name, grid)
-        return [typing.cast("PFTypes.Load", element) for element in elements]
+        return [t.cast("PFTypes.Load", element) for element in elements]
 
     def load_lv(self, name: str = "*", grid: str = "*") -> PFTypes.LoadLV | None:
-        element = self.grid_element("ElmLodLv", name, grid)
-        return typing.cast("PFTypes.LoadLV", element) if element is not None else None
+        return self.first_of(elements=self.loads_lv(name=name, grid=grid))
 
     def loads_lv(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.LoadLV]:
         elements = self.grid_elements("ElmLodLv", name, grid)
-        return [typing.cast("PFTypes.LoadLV", element) for element in elements]
+        return [t.cast("PFTypes.LoadLV", element) for element in elements]
 
     def load_mv(self, name: str = "*", grid: str = "*") -> PFTypes.LoadMV | None:
-        element = self.grid_element("ElmLodMv", name, grid)
-        return typing.cast("PFTypes.LoadMV", element) if element is not None else None
+        return self.first_of(elements=self.loads_mv(name=name, grid=grid))
 
     def loads_mv(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.LoadMV]:
         elements = self.grid_elements("ElmLodMv", name, grid)
-        return [typing.cast("PFTypes.LoadMV", element) for element in elements]
+        return [t.cast("PFTypes.LoadMV", element) for element in elements]
 
     def generator(self, name: str = "*", grid: str = "*") -> PFTypes.Generator | None:
-        element = self.grid_element("ElmGenstat", name, grid)
-        return typing.cast("PFTypes.Generator", element) if element is not None else None
+        return self.first_of(elements=self.generators(name=name, grid=grid))
 
     def generators(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.Generator]:
         elements = self.grid_elements("ElmGenstat", name, grid)
-        return [typing.cast("PFTypes.Generator", element) for element in elements]
+        return [t.cast("PFTypes.Generator", element) for element in elements]
 
     def pv_system(self, name: str = "*", grid: str = "*") -> PFTypes.PVSystem | None:
-        element = self.grid_element("ElmPvsys", name, grid)
-        return typing.cast("PFTypes.PVSystem", element) if element is not None else None
+        return self.first_of(elements=self.pv_systems(name=name, grid=grid))
 
     def pv_systems(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.PVSystem]:
         elements = self.grid_elements("ElmPvsys", name, grid)
-        return [typing.cast("PFTypes.PVSystem", element) for element in elements]
+        return [t.cast("PFTypes.PVSystem", element) for element in elements]
+
+    def ac_current_source(self, name: str = "*", grid: str = "*") -> PFTypes.AcCurrentSource | None:
+        return self.first_of(elements=self.ac_current_sources(name=name, grid=grid))
+
+    def ac_current_sources(self, name: str = "*", grid: str = "*") -> Sequence[PFTypes.AcCurrentSource]:
+        elements = self.grid_elements("ElmIac", name, grid)
+        return [t.cast("PFTypes.AcCurrentSource", element) for element in elements]
+
+    def grid(self, name: str = "*") -> PFTypes.Grid | None:
+        return self.first_of(elements=self.grids(name=name))
+
+    def grids(self, name: str = "*") -> Sequence[PFTypes.Grid]:
+        elements = self.grid_model_elements("ElmNet", name)
+        return [t.cast("PFTypes.Grid", element) for element in elements]
+
+    def grid_elements(self, class_name: str, name: str = "*", grid: str = "*") -> Sequence[PFTypes.DataObject]:
+        rv = [self.elements_of(element=g, pattern=name + "." + class_name) for g in self.grids(grid)]
+        return self.list_from_sequences(*rv)
+
+    def grid_model_elements(self, class_name: str, name: str = "*") -> Sequence[PFTypes.DataObject]:
+        return self.elements_of(element=self.grid_model, pattern=name + "." + class_name)
 
-    def grid_element(self, class_name: str, name: str = "*", grid: str = "*") -> PFTypes.DataObject | None:
-        elements = self.grid_elements(class_name=class_name, name=name, grid=grid)
+    def equipment_type_elements(self, class_name: str, name: str = "*") -> Sequence[PFTypes.DataObject]:
+        return self.elements_of(element=self.types_dir, pattern=name + "." + class_name)
+
+    def study_case_element(
+        self,
+        class_name: str,
+        name: str = "*",
+        study_case_name: str = "*",
+    ) -> PFTypes.DataObject | None:
+        elements = self.study_case_elements(class_name=class_name, name=name, study_case_name=study_case_name)
         if len(elements) == 0:
             return None
 
         if len(elements) > 1:
             logger.warning("Found more then one element, returning only the first one.")
 
         return elements[0]
 
-    def grid_elements(self, class_name: str, name: str = "*", grid: str = "*") -> Sequence[PFTypes.DataObject]:
-        rv = [self.elements_of(element=g, pattern=name + "." + class_name) for g in self.grids(grid)]
+    def study_case_elements(
+        self,
+        class_name: str,
+        name: str = "*",
+        study_case_name: str = "*",
+    ) -> Sequence[PFTypes.DataObject]:
+        rv = [self.elements_of(element=sc, pattern=name + "." + class_name) for sc in self.study_cases(study_case_name)]
         return self.list_from_sequences(*rv)
 
-    def grid(self, name: str = "*") -> PFTypes.Grid | None:
-        element = self.grid_model_element("ElmNet", name)
-        return typing.cast("PFTypes.Grid", element) if element is not None else None
+    def first_of(self, *, elements: Sequence[T]) -> T | None:
+        if len(elements) == 0:
+            return None
 
-    def grids(self, name: str = "*") -> Sequence[PFTypes.Grid]:
-        elements = self.grid_model_elements("ElmNet", name)
-        return [typing.cast("PFTypes.Grid", element) for element in elements]
+        if len(elements) > 1:
+            logger.warning("Found more then one element, returning only the first one.")
 
-    def grid_model_element(self, class_name: str, name: str = "*") -> PFTypes.DataObject | None:
-        return self.element_of(element=self.grid_model, pattern=name + "." + class_name)
+        return elements[0]
 
-    def grid_model_elements(self, class_name: str, name: str = "*") -> Sequence[PFTypes.DataObject]:
-        return self.elements_of(element=self.grid_model, pattern=name + "." + class_name)
+    def elements_of(
+        self,
+        *,
+        element: PFTypes.DataObject,
+        pattern: str = "*",
+        recursive: bool = True,
+    ) -> Sequence[PFTypes.DataObject]:
+        return element.GetContents(pattern, recursive)
 
     def create_unit_conversion_setting(
         self,
         name: str,
         uc: UnitConversionSetting,
     ) -> PFTypes.UnitConversionSetting | None:
         if self.unit_settings_dir is not None:
-            data = uc.dict()
+            data = dataclasses.asdict(uc)
             element = self.create_object(
                 name=name,
                 class_name="SetVariable",
                 location=self.unit_settings_dir,
                 data=data,
             )
-            return typing.cast("PFTypes.UnitConversionSetting", element) if element is not None else None
+            return t.cast("PFTypes.UnitConversionSetting", element) if element is not None else None
 
         return None
 
     def delete_unit_conversion_settings(self) -> None:
         ucs = self.unit_conversion_settings()
         for uc in ucs:
             self.delete_object(uc)
 
     def unit_conversion_settings(self) -> Sequence[PFTypes.UnitConversionSetting]:
         if self.unit_settings_dir is not None:
             elements = self.elements_of(element=self.unit_settings_dir, pattern="*.SetVariable")
-            return [typing.cast("PFTypes.UnitConversionSetting", element) for element in elements]
+            return [t.cast("PFTypes.UnitConversionSetting", element) for element in elements]
 
         return []
 
+    def create_result(
+        self,
+        *,
+        name: str,
+        study_case: PFTypes.StudyCase,
+        data: dict | None = None,
+        force: bool = False,
+        update: bool = True,
+    ) -> PFTypes.Result | None:
+        logger.debug("Create result object {name} ...", name=name)
+        if data is None:
+            data = {}
+        element = self.create_object(
+            name=name,
+            class_name="ElmRes",
+            location=study_case,
+            data=data,
+            force=force,
+            update=update,
+        )
+        return t.cast("PFTypes.Result", element) if element is not None else None
+
     def create_object(
         self,
         *,
         name: str,
         class_name: str,
-        location: PFTypes.DataDir,
-        data: dict[str, Any],
+        location: PFTypes.DataDir | PFTypes.StudyCase,
+        data: dict[str, t.Any],
         force: bool = False,
         update: bool = True,
     ) -> PFTypes.DataObject | None:
-        element = self.element_of(element=location, pattern=f"{name}.{class_name}")
+        _elements = self.elements_of(element=location, pattern=f"{name}.{class_name}")
+        element = self.first_of(elements=_elements)
         if element is not None and force is False:
             if update is False:
                 logger.warning(
                     "{object_name}.{class_name} already exists. Use force=True to create it anyway or update=True to update it.",
                     object_name=name,
                     class_name=class_name,
                 )
@@ -580,41 +774,16 @@
             update = True
 
         if element is not None and update is True:
             return self.update_object(element, data)
 
         return element
 
-    def element_of(
-        self,
-        *,
-        element: PFTypes.DataObject,
-        pattern: str = "*",
-        recursive: bool = True,
-    ) -> PFTypes.DataObject | None:
-        elements = self.elements_of(element=element, pattern=pattern, recursive=recursive)
-        if len(elements) == 0:
-            return None
-
-        if len(elements) > 1:
-            logger.warning("Found more then one element, returning only the first one.")
-
-        return elements[0]
-
-    def elements_of(
-        self,
-        *,
-        element: PFTypes.DataObject,
-        pattern: str = "*",
-        recursive: bool = True,
-    ) -> Sequence[PFTypes.DataObject]:
-        return element.GetContents(pattern, recursive)
-
     @staticmethod
-    def update_object(element: PFTypes.DataObject, data: dict[str, Any]) -> PFTypes.DataObject:
+    def update_object(element: PFTypes.DataObject, data: dict[str, t.Any]) -> PFTypes.DataObject:
         for key, value in data.items():
             if getattr(element, key, None) is not None:
                 setattr(element, key, value)
 
         return element
 
     @staticmethod
```

### Comparing `ieeh-powerfactory-tools-1.4.2/powerfactory_tools/powerfactory_types.py` & `ieeh-powerfactory-tools-1.5.0/powerfactory_tools/powerfactory_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -172,59 +172,74 @@
     EXTERNAL_GRID_EQUIVALENT = "net"
     OTHER = "othg"
 
 
 class VectorGroup(enum.Enum):
     Dd0 = "Dd0"
     Yy0 = "Yy0"
-    YNy0 = "Ny0"
+    YNy0 = "YNy0"
     Yyn0 = "Yyn0"
-    YNyn0 = "Nyn0"
+    YNyn0 = "YNyn0"
     Dz0 = "Dz0"
     Dzn0 = "Dzn0"
     Zd0 = "Zd0"
-    ZNd0 = "Nd0"
+    ZNd0 = "ZNd0"
+    Dyn1 = "Dyn1"
     Dy5 = "Dy5"
     Dyn5 = "Dyn5"
     Yd5 = "Yd5"
-    YNd5 = "Nd5"
+    YNd5 = "YNd5"
     Yz5 = "Yz5"
-    YNz5 = "Nz5"
+    YNz5 = "YNz5"
     Yzn5 = "Yzn5"
-    YNzn5 = "Nzn5"
+    YNzn5 = "YNzn5"
     Dd6 = "Dd6"
     Yy6 = "Yy6"
-    YNy6 = "Ny6"
+    YNy6 = "YNy6"
     Yyn6 = "Yyn6"
-    YNyn6 = "Nyn6"
+    YNyn6 = "YNyn6"
     Dz6 = "Dz6"
     Dzn6 = "Dzn6"
     Zd6 = "Zd6"
-    ZNd6 = "Nd6"
+    ZNd6 = "ZNd6"
+    Dyn7 = "Dyn7"
     Dy11 = "Dy11"
     Dyn11 = "Dyn11"
     Yd11 = "Yd11"
-    YNd11 = "Nd11"
+    YNd11 = "YNd11"
     Yz11 = "Yz11"
-    YNz11 = "Nz11"
+    YNz11 = "YNz11"
     Yzn11 = "Yzn11"
-    YNzn11 = "Nzn11"
+    YNzn11 = "YNzn11"
 
 
 class TrfPhaseTechnology(enum.IntEnum):
     SINGLE_PH_E = 1
     SINGLE_PH = 2
     THREE_PH = 3
 
 
 class TrfTapSide(enum.IntEnum):
     HV = 0
     LV = 1
 
 
+class TrfNeutralConnectionType(enum.IntEnum):
+    NO = 0
+    ABC_N = 1
+    HV = 2  # separat at HV side
+    LV = 3  # separat at LV side
+    HV_LV = 4  # separat at HV and LV side
+
+
+class TrfNeutralPointState(enum.IntEnum):
+    EARTHED = 0
+    ISOLATED = 1
+
+
 class MetricPrefix(enum.Enum):
     a = "a"
     f = "f"
     p = "p"
     n = "n"
     u = "u"
     m = "m"
@@ -286,14 +301,82 @@
 
 class TerminalVoltageSystemType(enum.IntEnum):
     DC = 0
     AC = 1
     ACBI = 2
 
 
+class HarmonicSourceSystemType(enum.IntEnum):
+    SYMMETIRC = 0
+    UNSYMMETRIC = 1
+    IEC_61000 = 2
+
+
+class HarmonicLoadModelType(enum.IntEnum):
+    IMPEDANCE_TYPE_1 = 0
+    CURRENT_SOURCE = 1
+    IMPEDANCE_TYPE_2 = 2
+
+
+class NetworkCalcType(enum.IntEnum):
+    AC_SYM_POSITIVE_SEQUENCE = 0
+    AC_UNSYM_ABC = 1  # unsym. 3-Phase(abc)
+
+
+class NetworkExtendedCalcType(enum.IntEnum):
+    AC_SYM_POSITIVE_SEQUENCE = 0
+    AC_UNSYM_ABC = 1  # unsym. 3-Phase(abc)
+    DC = 2
+
+
+class TemperatureDependencyType(enum.IntEnum):
+    DEFAULT_20_DEGREE = 0
+    MAX_OPERATION_TEMP = 1
+    OPERATION_TEMP = 2
+    USER_TEMP = 3
+
+
+class CalculationType(enum.IntEnum):  # only excerpt
+    ALL_CALCULATIONS = 0
+    RELIABILITY_MONTE_CARLO = 1
+    RELIABILITY_ENUMERATION = 2
+    MODAL_ANALYSIS = 5  # Eigenvalues
+    HARMONICS = 6
+    MONITORING = 7
+    TRIGGERED = 8
+    FREQUENCY_SWEEP = 9
+    VOLTAGE_SAGS = 10
+    SHORT_CIRCUIT_SWEEP = 11
+    ONLINE_PFM = 12
+    CONTINGENCY_ANALYSIS = 13
+    OPF_BEFORE_OPTIMISATION = 14
+    OPF_AFTER_OPTIMISATION = 15
+    SHORT_CIRCUIT = 16
+    FFT_CALCULATION = 17
+    SHORT_CIRCUIT_EMT = 18
+    FLICKER = 19
+    QUASI_DYNAMIC_SIMULATION = 29
+    PROTECTION = 30
+    SENSITIVITY_FACTORS = 31
+
+
+class CalculationCommand(enum.Enum):  # only excerpt
+    LOAD_FLOW = "ComLdf"
+    CONTINGENCY_ANALYSIS = "ComContingency"
+    FLICKER = "ComFlickermeter"
+    SHORT_CIRCUIT_SWEEP = "ComShctrace"
+    SHORT_CIRCUIT = "ComShc"
+    TIME_DOMAIN_SIMULATION = "ComSim"
+    TIME_DOMAIN_SIMULATION_START = "ComInc"
+    MODAL_ANALYSIS = "ComMod"
+    SENSITIVITY_ANALYSIS = "ComVstab"
+    HARMONICS = "ComHldf"
+    FREQUENCY_SWEEP = "ComFsweep"
+
+
 class PowerFactoryTypes:
     class DataObject(Protocol):
         loc_name: str
         fold_id: PowerFactoryTypes.DataObject | None
 
         def GetContents(  # noqa: N802
             self,
@@ -390,65 +473,89 @@
         aQ: float  # noqa: N815  # a-portion of the reactive power in relation to ZIP load model
         bQ: float  # noqa: N815  # b-portion of the reactive power in relation to ZIP load model
         cQ: float  # noqa: N815  # c-portion of the reactive power in relation to ZIP load model
         kqu0: float  # exponent of the a-portion of the reactive power in relation to ZIP load model
         kqu1: float  # exponent of the b-portion of the reactive power in relation to ZIP load model
         kqu: float  # exponent of the c-portion of the reactive power in relation to ZIP load model
 
+        i_crsc: HarmonicLoadModelType
+        i_pure: int  # for harmonic load model type IMPEDANCE_TYPE_1; 0 - pure inductive/capacitive; 1 - mixed inductive/capacitive
+        Prp: float  # for harmonic load model type IMPEDANCE_TYPE_2; static portion in percent
+        pcf: float  # for harmonic load model type IMPEDANCE_TYPE_2; load factor correction in percent
+
     class LineType(DataObject, Protocol):
         uline: float  # rated voltage (kV)
         sline: float  # rated current (kA) when installed in soil
         InomAir: float  # rated current (kA) when installed in air
         rline: float  # resistance (Ohm/km) positive sequence components
         rline0: float  # resistance (Ohm/km) zero sequence components
         xline: float  # reactance (Ohm/km) positive sequence components
         xline0: float  # reactance (Ohm/km) zero sequence components
         gline: float  # conductance (µS/km) positive sequence components
         gline0: float  # conductance (µS/km) zero sequence components
         bline: float  # susceptance (µS/km) positive sequence components
         bline0: float  # susceptance (µS/km) zero sequence components
+
+        nneutral: bool  # no. of neutral conductors
+
         systp: VoltageSystemType
         frnom: float  # nominal frequency the values x and b apply
 
+    class LineNType(LineType, Protocol):
+        rnline: float  # resistance (Ohm/km) natural neutral components
+        rpnline: float  # resistance (Ohm/km) natural neutral-line couple components
+        xnline: float  # reactance (Ohm/km) natural neutral components
+        xpnline: float  # reactance (Ohm/km) natural neutral-line couple components
+        gnline: float  # conductance (µS/km) natural neutral components
+        gpnline: float  # conductance (µS/km) natural neutral-line couple components
+        bnline: float  # susceptance (µS/km) natural neutral components
+        bpnline: float  # susceptance (µS/km) natural neutral-line couple components
+
     class Transformer2WType(DataObject, Protocol):
-        vecgrp: VectorGroup
-        dutap: float
-        phitr: float
-        ntpmn: int
-        ntpmx: int
-        nntap0: int
-        utrn_l: float
-        utrn_h: float
-        pfe: float
-        curmg: float
-        pcutr: float
-        strn: float
-        uktr: float
-        zx0hl_n: float
-        rtox0_n: float
+        utrn_l: float  # reference voltage LV side
+        utrn_h: float  # reference voltage HV side
+        pfe: float  # Iron losses
+        curmg: float  # no-load current
+        pcutr: float  # Cupper losses
+        strn: float  # rated power
+        uktr: float  # short-circuit voltage in percentage
         r1pu: float
         r0pu: float
         x1pu: float
         x0pu: float
-        tr2cn_l: Vector
-        tr2cn_h: Vector
+        zx0hl_n: float
+        rtox0_n: float
+
+        vecgrp: VectorGroup
+        tr2cn_l: Vector  # vector at LV side
+        tr2cn_h: Vector  # vector at HV side
         nt2ag: float
-        nt2ph: TrfPhaseTechnology
+
         tap_side: TrfTapSide
+        ntpmn: int
+        ntpmx: int
+        nntap0: int
+        dutap: float
+        phitr: float
         itapch: int
         itapch2: int
 
+        nt2ph: TrfPhaseTechnology
+
     class Transformer3WType(DataObject, Protocol):
         ...
 
     class SwitchType(DataObject, Protocol):
         Inom: float
         R_on: float
         X_on: float
 
+    class HarmonicSourceType(DataObject, Protocol):
+        i_usym: HarmonicSourceSystemType
+
     class Coupler(DataObject, Protocol):
         bus1: PowerFactoryTypes.StationCubicle | None
         bus2: PowerFactoryTypes.StationCubicle | None
         typ_id: PowerFactoryTypes.SwitchType | None
         cpSubstat: PowerFactoryTypes.Substation | None  # noqa: N815
         isclosed: bool
         desc: Sequence[str]
@@ -463,18 +570,20 @@
     class LineBase(DataObject, Protocol):
         cDisplayName: str  # noqa: N815
         desc: Sequence[str]
         outserv: bool
 
     class Terminal(DataObject, Protocol):
         cDisplayName: str  # noqa: N815
+        ciEnergized: bool  # noqa: N815
         desc: Sequence[str]
         uknom: float
         iUsage: NodeType  # noqa: N815
         outserv: bool
+        cStatName: str  # noqa: N815
         cpSubstat: PowerFactoryTypes.Substation | None  # noqa: N815
         cubics: Sequence[PowerFactoryTypes.StationCubicle]
         systype: TerminalVoltageSystemType
 
     class StationCubicle(DataObject, Protocol):
         cterm: PowerFactoryTypes.Terminal
         obj_id: PowerFactoryTypes.Line | PowerFactoryTypes.Element | None
@@ -484,14 +593,24 @@
     class Transformer2W(LineBase, Protocol):
         buslv: PowerFactoryTypes.StationCubicle | None
         bushv: PowerFactoryTypes.StationCubicle | None
         ntnum: int
         typ_id: PowerFactoryTypes.Transformer2WType | None
         nntap: int
 
+        cneutcon: TrfNeutralConnectionType
+        cgnd_h: TrfNeutralPointState
+        cgnd_l: TrfNeutralPointState
+        cpeter_h: bool
+        cpeter_l: bool
+        re0tr_h: float
+        re0tr_l: float
+        xe0tr_h: float
+        xe0tr_l: float
+
     class Transformer3W(LineBase, Protocol):
         buslv: PowerFactoryTypes.StationCubicle | None
         busmv: PowerFactoryTypes.StationCubicle | None
         bushv: PowerFactoryTypes.StationCubicle | None
         nt3nm: int
         typ_id: PowerFactoryTypes.Transformer3WType | None
         n3tapl: int
@@ -680,16 +799,137 @@
         pgini: float  # in MW
         qgini: float  # in Mvar
         phiini: float  # in deg
         snss: float  # in MVA
         snssmin: float  # in MVA
         outserv: bool
 
+    class SourceBase(DataObject, Protocol):
+        bus1: PowerFactoryTypes.StationCubicle | None
+        outserv: bool
+        nphase: int
+        desc: Sequence[str]
+        c_pmod: PowerFactoryTypes.CompoundModel | None  # Compound Parent Model/Template
+
+    class AcCurrentSource(SourceBase, Protocol):
+        Ir: float
+        isetp: float
+        cosini: float
+        i_cap: PFRecap
+        G1: float
+        B1: float
+        isetp2: float
+        phisetp2: float
+        G2: float
+        B2: float
+        isetp0: float
+        phisetp0: float
+        G0: float
+        B0: float
+        phmc: PowerFactoryTypes.HarmonicSourceType | None
+
+    class Result(DataObject, Protocol):
+        desc: Sequence[str]
+        calTp: CalculationType  # noqa: N815
+
+        def AddVariable(  # noqa: N802
+            self,
+            element: PowerFactoryTypes.DataObject,
+            varname: str,
+            /,
+        ) -> int:
+            ...
+
+        def Clear(self) -> int:  # noqa: N802  # Always 0 and can be ignored
+            ...
+
+        def FindColumn(  # noqa: N802
+            self,
+            obj: PowerFactoryTypes.DataObject,
+            varName: str,  # noqa: N803
+            startCol: int,  # noqa: N803
+            /,
+        ) -> int:
+            ...
+
+        def GetNumberOfColumns(self) -> None:  # noqa: N802
+            ...
+
+        def GetNumberOfRows(self) -> None:  # noqa: N802
+            ...
+
+        def GetValue(  # noqa: N802  # Returns a value from a result object for row iX of curve col.
+            self,
+            iX: int,  # noqa: N803
+            col: int,
+            /,
+        ) -> int:
+            ...
+
+        def Load(self) -> None:  # noqa: N802
+            ...
+
+        def Release(self) -> None:  # noqa: N802
+            ...
+
+    class CommandBase(DataObject, Protocol):
+        def Execute(self) -> int:  # noqa: N802
+            ...
+
+    class CommandLoadFlow(CommandBase, Protocol):
+        iopt_net: NetworkExtendedCalcType
+        iPST_at: bool  # noqa: N815  # automatic step control of phase shifting transformers
+        iopt_plim: bool  # apply active power limits
+        iopt_at: bool  # automatic step control of transformers
+        iopt_asht: bool  # automatic step control of compensators/filters
+        iopt_lim: bool  # apply reactive power limits
+        iopt_tem: TemperatureDependencyType
+        temperature: float
+        iopt_pq: bool  # apply voltage dependecy of loads
+        iopt_fls: bool  # load scaling at defined feeders
+
+        i_power: int  # load flow method; 0 - NewtonRaphson (current eq.); 1 - Newton Raphson (power eq.)[default]
+
+        scLoadFac: float  # noqa: N815  # load scaling factor in percentage
+        scGenFac: float  # noqa: N815  # generator scaling factor in percentage
+        scMotFac: float  # noqa: N815  # motor scaling factor in percentage
+        zoneScale: int  # noqa: N815  # zone scaling; 0 - apply for all loads; 1 - apply only for scalable loads
+
+    class CommandHarmonicCalculation(CommandBase, Protocol):
+        iopt_sweep: int
+        iopt_allfrq: int
+        iopt_flicker: bool
+        iopt_SkV: bool  # noqa: N815
+        iopt_pseq: bool
+        iopt_net: NetworkCalcType
+        frnom: float
+        fshow: float
+        ifshow: float
+        p_resvar: PowerFactoryTypes.Result
+
+        errmax: float
+        errinc: float
+        ninc: float
+        iopt_thd: int
+
+    class CommandFrequencySweep(CommandBase, Protocol):
+        iopt_net: NetworkCalcType
+        ildfinit: bool  # load flow initialisation
+        fstart: float
+        fstep: float
+        fstop: float
+        i_adapt: bool  # automatic step size adaption
+
     class Script(Protocol):
-        def SetExternalObject(self, name: str, value: PowerFactoryTypes.DataObject) -> int:  # noqa: N802
+        def SetExternalObject(  # noqa: N802
+            self,
+            name: str,
+            value: PowerFactoryTypes.DataObject,
+            /,
+        ) -> int:
             ...
 
         def Execute(self) -> int:  # noqa: N802
             ...
 
     class Application(Protocol):
         def ActivateProject(self, name: str) -> int:  # noqa: N802
@@ -697,23 +937,65 @@
 
         def GetActiveProject(self) -> PowerFactoryTypes.Project:  # noqa: N802
             ...
 
         def GetActiveScenario(self) -> PowerFactoryTypes.Scenario | None:  # noqa: N802
             ...
 
-        def GetProjectFolder(self, name: str) -> PowerFactoryTypes.DataObject:  # noqa: N802
+        def GetActiveStudyCase(self) -> PowerFactoryTypes.StudyCase:  # noqa: N802
             ...
 
-        def PostCommand(self, command: Literal["exit"]) -> None:  # noqa: N802
+        def GetProjectFolder(  # noqa: N802
+            self,
+            name: str,
+            /,
+        ) -> PowerFactoryTypes.DataObject:
+            ...
+
+        def GetFromStudyCase(  # noqa: N802
+            self,
+            className: str,  # noqa: N803
+            /,
+        ) -> PowerFactoryTypes.DataObject:
+            ...
+
+        def PostCommand(  # noqa: N802
+            self,
+            command: Literal["exit"],
+            /,
+        ) -> None:
+            ...
+
+        def ExecuteCmd(  # noqa: N802
+            self,
+            command: str,
+            /,
+        ) -> None:
+            ...
+
+        def EchoOff(self) -> None:  # noqa: N802
+            ...
+
+        def EchoOn(self) -> None:  # noqa: N802
+            ...
+
+        def GetCalcRelevantObjects(  # noqa: N802
+            self,
+            nameFilter: str,  # noqa: N803
+            includeOutOfService: int,  # noqa: N803
+            topoElementsOnly: int,  # noqa: N803
+            bAcSchemes: int,  # noqa: N803
+            /,
+        ) -> set:
             ...
 
     class PowerFactoryModule(Protocol):
         ExitError: tuple[type[Exception], ...]
 
         def GetApplicationExt(  # noqa: N802
             self,
             username: str | None = None,
             password: str | None = None,
             commandLineArguments: str | None = None,  # noqa: N803
+            /,
         ) -> PowerFactoryTypes.Application:
             ...
```

### Comparing `ieeh-powerfactory-tools-1.4.2/pyproject.toml` & `ieeh-powerfactory-tools-1.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [project]
 authors = [
     { name = "Sasan Jacob Rasti", email = "sasan_jacob.rasti@tu-dresden.de" },
     { name = "Maximilian Schmidt", email = "maximilian.schmidt@tu-dresden.de" },
     { name = "Sebastian Krahmer", email = "sebastian.krahmer@tu-dresden.de" },
 ]
 dependencies = [
+    "ieeh-power-system-data-model==1.3.0",
     "loguru",
     "pydantic",
 ]
 description = "A toolbox for Python based control of DIgSILENT PowerFactory"
 name = "ieeh-powerfactory-tools"
 readme = "README.md"
 requires-python = ">=3.10,<3.11"
-version = "1.4.2"
+version = "1.5.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/ieeh-tu-dresden/powerfactory-tools"
 
@@ -75,14 +76,19 @@
     "E501",
 ]
 line-length = 120
 select = [
     "ALL",
 ]
 
+[tool.ruff.flake8-type-checking]
+runtime-evaluated-decorators = [
+    "pydantic.dataclasses.dataclass",
+]
+
 [tool.ruff.isort]
 force-single-line = true
 
 [tool.ruff.pydocstyle]
 convention = "pep257"
 
 [tool.ruff.pep8-naming]
@@ -94,17 +100,18 @@
 
 [tool.black]
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
-version = "1.4.2"
+version = "1.5.0"
 version_files = [
     ".zenodo.json:version",
+    "CITATION.cff:cff-version",
     "pyproject.toml:version",
 ]
 
 [tool.mypy]
 follow_imports = "normal"
 ignore_missing_imports = true
 mypy_path = "powerfactory_tools"
```

### Comparing `ieeh-powerfactory-tools-1.4.2/PKG-INFO` & `ieeh-powerfactory-tools-1.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieeh-powerfactory-tools
-Version: 1.4.2
+Version: 1.5.0
 Summary: A toolbox for Python based control of DIgSILENT PowerFactory
 Author-email: Sasan Jacob Rasti <sasan_jacob.rasti@tu-dresden.de>,Maximilian Schmidt <maximilian.schmidt@tu-dresden.de>,Sebastian Krahmer <sebastian.krahmer@tu-dresden.de>
 Requires-Python: >=3.10,<3.11
 Project-URL: Source, https://github.com/ieeh-tu-dresden/powerfactory-tools
 Description-Content-Type: text/markdown
 
 # IEEH PowerFactory Tools
@@ -25,21 +25,15 @@
 ## <div id="application" /> Field of Application
 
 This application is intended to use for an external usage ('engine mode') of the power flow calculation program [DIgSILENT PowerFactory](https://www.digsilent.de/de/powerfactory.html).
 Therefore, the Python-PowerFactory-API, provided by the company, is utilized.
 
 The following functionalities are provided:
 
-* export of calculation relevant grid data from a PowerFactory project into three common readable JSON files utilizing predefined [schemas](./powerfactory_tools/schema):
-  * grid topology:
-    * base topology containing all elements of the exported grid
-  * topology case;
-    * information about disabled elements to represent a specific operational case based on the base topology
-  * steadystate case
-    * information about power draw/infeed for a specific operational case
+* export of calculation relevant grid data from a PowerFactory project to the [IEEH Power System Data Model](https://github.com/ieeh-tu-dresden/power-system-data-model)
 * [intended in future release] import from external grid data into the PowerFactory environment
 * [intended in future release] basic control of PowerFactory
 
 ## <div id="tutorials" /> Tutorials
 
 Jupyter notebooks are provided to get in touch with the usage of this toolbox:
```

