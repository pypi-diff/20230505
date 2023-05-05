# Comparing `tmp/slapstack-0.0.24.tar.gz` & `tmp/slapstack-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\slapstack-0.0.24.tar", last modified: Sat Jun  4 22:11:11 2022, max compression
+gzip compressed data, was "D:\1_research\2_publications\5_slap_crossdock\publlikationsrepo\1_environment\slapstack\dist\tmpmjqrf0bg\slapstack-0.1.1.tar", last modified: Fri May  5 00:32:48 2023, max compression
```

## Comparing `slapstack-0.0.24.tar` & `slapstack-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,37 @@
-drwxrwxrwx   0        0        0        0 2022-06-04 22:11:11.000000 slapstack-0.0.24/
--rw-rw-rw-   0        0        0      352 2022-06-04 22:11:11.000000 slapstack-0.0.24/MANIFEST.in
--rw-rw-rw-   0        0        0    10609 2022-06-04 22:11:11.000000 slapstack-0.0.24/PKG-INFO
--rw-rw-rw-   0        0        0      127 2022-05-25 10:21:11.000000 slapstack-0.0.24/pyproject.toml
--rw-rw-rw-   0        0        0     9329 2022-06-04 19:57:18.000000 slapstack-0.0.24/README.md
--rw-rw-rw-   0        0        0       70 2022-06-04 22:11:11.000000 slapstack-0.0.24/setup.cfg
--rw-rw-rw-   0        0        0     2131 2022-06-04 22:11:06.000000 slapstack-0.0.24/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-04 22:11:11.000000 slapstack-0.0.24/slapstack/
--rw-rw-rw-   0        0        0    37016 2022-05-18 23:20:25.000000 slapstack-0.0.24/slapstack/core.py
--rw-rw-rw-   0        0        0    31778 2022-05-18 23:29:25.000000 slapstack-0.0.24/slapstack/core_events.py
--rw-rw-rw-   0        0        0     1869 2022-05-17 13:39:52.000000 slapstack-0.0.24/slapstack/core_logger.py
--rw-rw-rw-   0        0        0    27747 2022-05-18 23:36:54.000000 slapstack-0.0.24/slapstack/core_state.py
--rw-rw-rw-   0        0        0     9969 2022-05-18 22:04:27.000000 slapstack-0.0.24/slapstack/core_state_agv_manager.py
--rw-rw-rw-   0        0        0    16625 2022-05-18 23:16:22.000000 slapstack-0.0.24/slapstack/core_state_lane_manager.py
--rw-rw-rw-   0        0        0    34380 2022-05-18 23:14:09.000000 slapstack-0.0.24/slapstack/core_state_location_manager.py
--rw-rw-rw-   0        0        0    32741 2022-05-26 12:01:04.000000 slapstack-0.0.24/slapstack/core_state_route_manager.py
--rw-rw-rw-   0        0        0     5007 2022-05-18 23:37:52.000000 slapstack-0.0.24/slapstack/core_state_zone_manager.py
-drwxrwxrwx   0        0        0        0 2022-06-04 22:11:11.000000 slapstack-0.0.24/slapstack/extensions/
--rw-rw-rw-   0        0        0   252086 2022-06-04 20:53:03.000000 slapstack-0.0.24/slapstack/extensions/c_dijkstra.cpp
--rw-rw-rw-   0        0        0    10847 2022-05-18 23:20:25.000000 slapstack-0.0.24/slapstack/extensions/c_dijkstra.pyx
--rw-rw-rw-   0        0        0   158415 2022-06-04 19:34:06.000000 slapstack-0.0.24/slapstack/extensions/c_helpers.cpp
--rw-rw-rw-   0        0        0     1180 2022-04-17 21:33:58.000000 slapstack-0.0.24/slapstack/extensions/c_helpers.pyx
--rw-rw-rw-   0        0        0      138 2022-04-17 16:43:44.000000 slapstack-0.0.24/slapstack/extensions/__init__.py
--rw-rw-rw-   0        0        0     9649 2022-05-25 12:23:47.000000 slapstack-0.0.24/slapstack/helpers.py
--rw-rw-rw-   0        0        0    19265 2022-05-18 22:12:53.000000 slapstack-0.0.24/slapstack/interface.py
--rw-rw-rw-   0        0        0      254 2022-05-18 22:12:53.000000 slapstack-0.0.24/slapstack/interface_input.py
--rw-rw-rw-   0        0        0     6086 2022-05-18 22:00:35.000000 slapstack-0.0.24/slapstack/interface_templates.py
--rw-rw-rw-   0        0        0     8745 2022-05-25 12:23:47.000000 slapstack-0.0.24/slapstack/use_case.py
-drwxrwxrwx   0        0        0        0 2022-06-04 22:11:11.000000 slapstack-0.0.24/slapstack/WEPAStacks/
--rw-rw-rw-   0        0        0      947 2022-05-04 18:13:55.000000 slapstack-0.0.24/slapstack/WEPAStacks/Initial_fill_lvl.json
-drwxrwxrwx   0        0        0        0 2022-06-04 22:11:11.000000 slapstack-0.0.24/slapstack/WEPAStacks/layouts/
--rw-rw-rw-   0        0        0    21394 2022-05-04 18:13:55.000000 slapstack-0.0.24/slapstack/WEPAStacks/layouts/layout1_middle_aisles.csv
--rw-rw-rw-   0        0        0     5943 2022-05-04 18:13:55.000000 slapstack-0.0.24/slapstack/WEPAStacks/layouts/layout1_mini_middle_aisles.csv
--rw-rw-rw-   0        0        0 43414069 2022-05-04 18:13:55.000000 slapstack-0.0.24/slapstack/WEPAStacks/Orders_v5.json
--rw-rw-rw-   0        0        0       78 2022-05-17 13:39:52.000000 slapstack-0.0.24/slapstack/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-04 22:11:11.000000 slapstack-0.0.24/slapstack.egg-info/
--rw-rw-rw-   0        0        0        1 2022-06-04 22:11:11.000000 slapstack-0.0.24/slapstack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    10609 2022-06-04 22:11:11.000000 slapstack-0.0.24/slapstack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       24 2022-06-04 22:11:11.000000 slapstack-0.0.24/slapstack.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1019 2022-06-04 22:11:11.000000 slapstack-0.0.24/slapstack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2022-06-04 22:11:11.000000 slapstack-0.0.24/slapstack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 00:32:48.000000 slapstack-0.1.1/
+-rw-rw-rw-   0        0        0     1093 2023-05-04 18:07:13.000000 slapstack-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      298 2023-05-05 00:32:48.000000 slapstack-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    12625 2023-05-05 00:32:48.000000 slapstack-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    12332 2023-05-05 00:15:16.000000 slapstack-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 00:32:48.000000 slapstack-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-05-04 18:08:15.000000 slapstack-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:32:48.000000 slapstack-0.1.1/slapstack/
+-rw-rw-rw-   0        0        0    41370 2023-05-03 16:24:35.000000 slapstack-0.1.1/slapstack/core.py
+-rw-rw-rw-   0        0        0    47947 2023-05-03 15:55:27.000000 slapstack-0.1.1/slapstack/core_events.py
+-rw-rw-rw-   0        0        0     1865 2023-04-06 08:47:23.000000 slapstack-0.1.1/slapstack/core_logger.py
+-rw-rw-rw-   0        0        0    30071 2023-05-03 15:55:27.000000 slapstack-0.1.1/slapstack/core_state.py
+-rw-rw-rw-   0        0        0    12630 2023-04-03 18:05:53.000000 slapstack-0.1.1/slapstack/core_state_agv_manager.py
+-rw-rw-rw-   0        0        0    18390 2023-05-03 15:38:04.000000 slapstack-0.1.1/slapstack/core_state_lane_manager.py
+-rw-rw-rw-   0        0        0    35814 2023-05-03 16:13:13.000000 slapstack-0.1.1/slapstack/core_state_location_manager.py
+-rw-rw-rw-   0        0        0    18128 2023-05-03 16:20:31.000000 slapstack-0.1.1/slapstack/core_state_route_manager.py
+-rw-rw-rw-   0        0        0     5007 2022-05-18 23:37:52.000000 slapstack-0.1.1/slapstack/core_state_zone_manager.py
+-rw-rw-rw-   0        0        0    10422 2023-05-03 21:39:02.000000 slapstack-0.1.1/slapstack/helpers.py
+-rw-rw-rw-   0        0        0    19265 2023-04-27 11:36:40.000000 slapstack-0.1.1/slapstack/interface.py
+-rw-rw-rw-   0        0        0      254 2022-05-18 22:12:53.000000 slapstack-0.1.1/slapstack/interface_input.py
+-rw-rw-rw-   0        0        0    12252 2023-05-03 21:39:02.000000 slapstack-0.1.1/slapstack/interface_templates.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:32:48.000000 slapstack-0.1.1/slapstack/use_cases/
+drwxrwxrwx   0        0        0        0 2023-05-05 00:32:48.000000 slapstack-0.1.1/slapstack/use_cases/crossstacks/
+-rw-rw-rw-   0        0        0    14477 2023-04-01 09:57:32.000000 slapstack-0.1.1/slapstack/use_cases/crossstacks/1_layout.csv
+-rw-rw-rw-   0        0        0  1413432 2023-04-01 09:57:31.000000 slapstack-0.1.1/slapstack/use_cases/crossstacks/2_orders.json
+-rw-rw-rw-   0        0        0       14 2023-04-01 09:57:32.000000 slapstack-0.1.1/slapstack/use_cases/crossstacks/3_initial_fill_lvl.json
+drwxrwxrwx   0        0        0        0 2023-05-05 00:32:48.000000 slapstack-0.1.1/slapstack/use_cases/wepastacks/
+-rw-rw-rw-   0        0        0    21394 2022-05-04 18:13:55.000000 slapstack-0.1.1/slapstack/use_cases/wepastacks/1_layout.csv
+-rw-rw-rw-   0        0        0 43414069 2023-04-01 09:34:16.000000 slapstack-0.1.1/slapstack/use_cases/wepastacks/2_orders.json
+-rw-rw-rw-   0        0        0      947 2022-05-04 18:13:55.000000 slapstack-0.1.1/slapstack/use_cases/wepastacks/3_initial_fill_lvl.json
+-rw-rw-rw-   0        0        0       78 2022-05-17 13:39:52.000000 slapstack-0.1.1/slapstack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:32:48.000000 slapstack-0.1.1/slapstack.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-05 00:32:48.000000 slapstack-0.1.1/slapstack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    12625 2023-05-05 00:32:48.000000 slapstack-0.1.1/slapstack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-05-05 00:32:48.000000 slapstack-0.1.1/slapstack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      902 2023-05-05 00:32:48.000000 slapstack-0.1.1/slapstack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 00:32:48.000000 slapstack-0.1.1/slapstack.egg-info/top_level.txt
```

### Comparing `slapstack-0.0.24/PKG-INFO` & `slapstack-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,273 @@
-Metadata-Version: 2.1
-Name: slapstack
-Version: 0.0.24
-Summary: An Event Discrete Simulation Framework for Block-Stacking Warehouses.
-Home-page: UNKNOWN
-License: UNKNOWN
-Description: # SLAPStack 
-        SLAPStack is a block-stacking warehouse simulation for the Autonomous Block Stacking Warehouse Problem (ABSWP) [[1]](#pfrommer2020) implementing the [OpenAI](https://gym.openai.com/) gym interface. The code can be used to test out Storage Location Allocation Problem (SLAP) and Unit Load Selection Problem (ULSP) algorithms individually or in conjunction. The simulation project includes the WEPAStacks data which includes the layout and 3 months of order information of a large-scale real-world clock stacking warehouse from [WEPA Hygieneprodukte GmbH](https://www.wepa.eu/de/)
-        
-        ## SLAPStack Simulation
-        ### Architecture
-        
-        The project architecture follows the one introduced in [[2]](#rinciog2020), as can be seen in the partial class diagram below. The simulation entry point, which implements the gym interface is located in the `SlapEnv` class located in the `interface.py` module. `SlapEnv`, whose primary function is action- and state-space configuration and transformation, is a wrapper around the `SlapCore` which contains the simulation logic. 
-        
-        `SlapCore` is responsible for advancing the simulation when calling `step`. It uses an `EventManager` object to maintain the `Event` queues. The central SLAPStack communication structure is given by the `State` object contained by the `SlapCore`.  
-        
-        The `State` contains several manager objects dedicated to distinct tasks. The `RouteManager`, for instance, is used to compute routes on the storage matrix `S` grid during `Transport` event initialization. The 3D state matrices `S`  (pallet SKUs information), `V` (vehicle positions), `B` (pallet batch information), and `T` (pallet arrival information) are shared between `State` and manager objects as needed (e.g. `V` is shared between `AmrManager` and `State`). 
-        
-        The `interface_templates.py` module defines and documents the simulation parameter as well as the `SlapEnv` configuration objects, i.e. `Strategy` for allowing indirect actions and `OutputConverter` for transforming both the state representation and the reward returned by `SlapEnv.step()`.
-        
-        <p align="center">
-        	<img src="readme/SLAPStack - UML Class.png" alt="class_diagram" width="1000"/>
-        </p>
-        
-        
-        ### Events
-        At the core of the simulation lies the `future_events` queue. `future_events` is a time-sorted heap of self-handling events. During a simulation step, events are popped from this heap and their handle function is called leading to a state update. If a triggered event requires an external ULSP or SLAP decision, the execution halts, and the state is returned.
-        Events are either orders or transport events. Orders (`Delivery` or `Retrieval`) get added to the queue during initialization. Transport events (`Delivery/RetrievalFirst/SecondLeg`) are created on-demand. Of the 6 events present in the simulation, 2 are blocking, namely `Retrieval` and `DeliverySecondLeg`. The relationship between them is depicted event chain summary below.
-        
-        <p align="center">
-        	<img src="readme/event_overview.png" alt="event_chains" width="1000"/>
-        </p>
-        
-        
-        ### Routing and Runtime
-        
-        The design lain down in [[2]](#rinciog2020) and implemented by SLAPStack leads to an efficient runtime in terms of event management and state updates. All state updates are run in constant or amortized constant time. Since, `future_events` is a binary heap, pushing `Order` events to it during initialization and  `Transport` events to it during `step` takes logarithmic time with respect to the total number of orders. This yields an asymptotic runtime of O(n log(n)), where n is the number of orders.
-        
-        However, a particularity of SLAPStack is the fine-grained routing mechanism implemented. Whenever a `Transport` event is created, the exact closest grid cell route between the AMRs current position and its destination is computed. Dijkstra takes O(m log(m + l)) where m is the number of nodes and l is the number of edges in the routing graph. In our case, that would amount to O(m log m) with m being the number of grid cells in the BSWP (each grid cell is a routing graph node and each cell has four bidirectional edges, i.e. O(m log(m + l) = O(m log(m + 4m)) = O(m log(m)). To deal with this routing bottleneck, SLAPStack's `RouteManager` uses a Cython implementation of Dijkstra, route caching, and uses only an aisle grid tiles for routing (the light blue tiles in the figure below).
-        
-        Simulating a total of 400000 orders on CPU take around 2 hours.
-        
-        <p align="center">
-        	<img src="readme/routing_scheme.png" alt="routing" width="350"/>
-        </p>
-        
-        
-        
-        ## Use Case Data: WEPAStacks 
-        
-        This dataset is based on a real-world block stacking warehouse from WEPA.
-        
-        WEPA is one of the largest hygienic paper manufacturers in Europe with production plants and warehouses in currently six European countries (www.wepa.eu).
-        
-        The dataset consists of three components:
-        
-        1. the warehouse layout
-        2. the initial fill level
-        3. the order stream
-        
-        ### Warehouse Layout
-        
-        The grid-based warehouse layout shown in the figure below is used to store finished goods on standardized EUR-pallets that can be stacked up to 3 levels. The capacity of the warehouse is up to 19512 storage locations (6504 on the ground with stacking). The light-gray area shows the bidirectional pathways (aisles). Dependent on the type of vehicle they are double/three-lanes wide. The storage bays/lanes are the white areas with separating lines. The dark-gray surrounding wall and truck loading zone define the boundaries of the storage system. Interfaces to the outside world are 4 Inputs (I-points) that represent the production lines and 10 Outputs (O-points) for shipping. At I-points the delivered pallets are picked up and transported to a storage location. Upon the arrival of a retrieval order, pallets are provided at the O-points. O-points are the staging areas in front of the dock doors. The truck loading process is not part of the use-case since it is executed by the truck drivers.
-        
-        The warehouse layout is provided as csv-file with numbers from -5 to 0. A -5 represents a travel path, -4 an O-point, -3 an I-point, -2 an aisle, -1 the warehouse boundaries and 0 the available storage locations.
-        
-        <p align="center">
-        	<img src="readme/setup_a_layout_v3.png" alt="layout" width="700"/>
-        </p>
-        
-        ### Initial fill level
-        
-        The initial fill level is a dictionary of Stock Keeping Unit (SKUs) with the respective amount currently on stock at time zero. 
-        
-        <p align="center">
-        	<img src="readme/initial_fill_lvl_1.png" alt="ini_fill" width="350"/>
-        </p>
-        
-        ### Order stream
-        
-        The order stream represents the daily in- and outbound flow with the exact arrival times of each delivery or retrieval order for a time period of 89 days (amounting to 4e5 orderes). Each order corresponds to a single pallet. While the inbound flow is based on a production frequency of 60 to 120 seconds, the outbound flow is mainly in full truck loads (FTL) with 33 pallets.
-        
-        The orders are provided as a nested list. Each order comes with six parameters namely the type (delivery or retrieval), the SKU (number from 1 to 136), the order arrival time (absolute time in seconds counting from zero), the dock door (number from 1 to 4 from top to bottom for delivery and 1 to 10 from left to right for retrieval), the batch number (number of production batches from 1 to 1498 for delivery and of truckload batches from 1 to 7496 for retrieval) and the week number (from 1 to 14).
-        
-        <p align="center">
-        	<img src="readme/order_stream_v1.png" alt="orders" width="500"/>
-        </p>
-        
-        
-        ## Getting Started
-        ### Installation
-        We publish this project alongside our experiment script and a control package containing various SLAP heuristics as well as a ULSP heuristic. To set up your environment and recreate our experiment results, the following steps can be taken:
-        1. Cloning the repository:
-        	```
-        	git clone https://github.com/malerinc/slapstack.git
-        	```
-        2. To install the SLAPStack simulation and its controls run the following commands from the project root directory (this will build the Cython extensions and copy the use case data at the appropriate locations):
-        	```
-        	pip install 1_environment/slapstack
-        	pip install 2_control/slapstack-controls
-        	```
-        3. To run the experiment script, simply execute the `storage_strategy_comparison.py` script located in the experiments directory directly under the root:
-        	```
-           python storage_strategy_comparison.py
-           ```
-        
-        ## Citing the Project
-        If you use `SLAPStack` or `WEPAStacks` in your research, you can cite this repository as follows:
-        
-        ```
-        @misc{rinciog2022slapstack
-            author = {Rinciog, Alexandru and Pfrommer, Jakob and Morrissey Michael and Sohaib Zahid and Meyer Anne},
-            title = {FabricatioRL},
-            year = {2021},
-            publisher = {GitHub},
-            journal = {GitHub Repository},
-            howpublished = {\url{https://github.com/malerinc/slapstack.git}},
-        }
-        ```
-        
-        ## References
-        <a id="pfrommer2020">[1]</a> Pfrommer, J., Meyer, A.: Autonomously organized block stacking warehouses: A
-        review of decision problems and major challenges. Logistics Journal: Proceedings
-        2020(12) (2020)
-        
-        <a id="rinciog2020">[2]</a> Rinciog, A., Meyer, A.: Fabricatio-rl: a reinforcement learning simulation frame-
-        work for production scheduling. In: 2021 Winter Simulation Conference (WSC).
-        pp. 1â€“12. IEEE (2021)
-        
-        
-        
-        
-Platform: UNKNOWN
-Requires-Python: >3.6.8
-Description-Content-Type: text/markdown
+# SLAPStack 
+SLAPStack is a block-stacking warehouse simulation for the Autonomous Block 
+Stacking Warehouse Problem (ABSWP) [[1]](#pfrommer2020) implementing the 
+[OpenAI](https://gym.openai.com/) gym interface. 
+The code can be used to test out Storage Location Allocation Problem (SLAP) and 
+Unit Load Selection Problem (ULSP) algorithms individually or in conjunction. 
+
+The simulation project includes the `WEPAStacks` data which includes the layout 
+and 3 months of order information of a large-scale real-world clock stacking 
+warehouse from [WEPA Hygieneprodukte GmbH](https://www.wepa.eu/de/).
+Additionally, an anonymized use case dataset, `CrossStacks` associated with a 
+medium-sized cross-docking terminal is made available. `CrossStacks` 
+
+## SLAPStack Simulation
+### Architecture
+
+The project architecture follows the one introduced in [[2]](#rinciog2020), 
+as can be seen in the partial class diagram below. The simulation entry point, 
+which implements the gym interface is located in the `SlapEnv` class located in 
+the `interface.py` module. `SlapEnv`, whose primary function is action- and 
+state-space configuration and transformation, is a wrapper around the `SlapCore`
+which contains the simulation logic. 
+
+`SlapCore` is responsible for advancing the simulation when calling `step`. It 
+uses an `EventManager` object to maintain the `Event` queues. The central 
+SLAPStack communication structure is given by the `State` object contained by 
+the `SlapCore`.  
+
+The `State` contains several manager objects dedicated to distinct tasks. 
+The `RouteManager`, for instance, is used to compute routes on the storage 
+matrix `S` grid during `Transport` event initialization. The 3D state matrices 
+`S`  (pallet SKUs information), `V` (vehicle positions), 
+`B` (pallet batch information), and `T` (pallet arrival information) are shared 
+between `State` and manager objects as needed (e.g. `V` is shared between 
+`AmrManager` and `State`). 
+
+The `interface_templates.py` module defines and documents the simulation 
+parameter as well as the `SlapEnv` configuration objects, i.e. `Strategy` for 
+allowing indirect actions and `OutputConverter` for transforming both the state 
+representation and the reward returned by `SlapEnv.step()`.
+
+<p align="center">
+	<img src="readme/SLAPStack - UML Class.png" alt="class_diagram" width="1000"/>
+</p>
+
+
+### Events
+At the core of the simulation lies the `future_events` queue. `future_events` is 
+a time-sorted heap of self-handling events. During a simulation step, events are 
+popped from this heap and their handle function is called leading to a state 
+update. If a triggered event requires an external ULSP or SLAP decision, the 
+execution halts, and the state is returned.
+Events are either orders or transport events. Orders (`Delivery` or `Retrieval`) 
+get added to the queue during initialization. Transport events 
+(`Delivery/RetrievalFirst/SecondLeg`) are created on-demand. Of the 6 events 
+present in the simulation, 2 are blocking, namely `Retrieval` and 
+`DeliverySecondLeg`. The relationship between them is depicted event chain 
+summary below.
+
+<p align="center">
+	<img src="readme/event_overview.png" alt="event_chains" width="1000"/>
+</p>
+
+
+### Routing and Runtime
+
+The design lain down in [[2]](#rinciog2020) and implemented by SLAPStack leads 
+to an efficient runtime in terms of event management and state updates. 
+All state updates are run in constant or amortized constant time. 
+Since, `future_events` is a binary heap, pushing `Order` events to it during 
+initialization and  `Transport` events to it during `step` takes logarithmic 
+time with respect to the total number of orders. This yields an asymptotic 
+runtime of O(n log(n)), where n is the number of orders.
+
+However, a particularity of SLAPStack is the fine-grained routing mechanism 
+implemented. Whenever a `Transport` event is created, the exact closest grid 
+cell route between the AMRs current position and its destination is computed. 
+Dijkstra takes O(m log(m + l)) where m is the number of nodes and l is the 
+number of edges in the routing graph. In our case, that would amount to 
+O(m log m) with m being the number of grid cells in the BSWP (each grid cell is 
+a routing graph node and each cell has four bidirectional edges, 
+i.e. O(m log(m + l) = O(m log(m + 4m)) = O(m log(m)). 
+To deal with this routing bottleneck, SLAPStack's `RouteManager` precomputes 
+all routes over aisle tiles (the light blue tiles in the figure below) using 
+the Floyed Warshall algorithm implemented in `scipy`. The exact route 
+computation is then completed by adding lane traversal segments which runs in 
+constant time (see figure).
+
+Simulating a total of 400000 orders on CPU take around 1 hour.
+
+<p align="center">
+	<img src="readme/routing_scheme.png" alt="routing" width="350"/>
+</p>
+
+### Extensions
+
+The latest version of this simulation contains extensions necessary to 
+accommodate cross-docking use-cases and dual command cycle heuristics. These 
+extensions are:
+* dock to dock transports
+* order queueing on AMRs
+
+Additionally, AMRs are capable or transporting more than one load at a time 
+(multiple forks).  
+
+## Use Case Data
+
+### WEPAStacks 
+
+This dataset is based on a real-world block stacking warehouse from WEPA.
+
+WEPA is one of the largest hygienic paper manufacturers in Europe with 
+production plants and warehouses in currently six European countries 
+(www.wepa.eu).
+
+The dataset consists of three components:
+
+1. the warehouse layout
+2. the initial fill level
+3. the order stream
+
+#### Warehouse Layout
+
+The grid-based warehouse layout shown in the figure below is used to store 
+finished goods on standardized EUR-pallets that can be stacked up to 3 levels. 
+The capacity of the warehouse is up to 19512 storage locations (6504 on the 
+ground with stacking). The light-gray area shows the bidirectional pathways 
+(aisles). Dependent on the type of vehicle they are double/three-lanes wide. 
+The storage bays/lanes are the white areas with separating lines. The dark-gray 
+surrounding wall and truck loading zone define the boundaries of the storage 
+system. Interfaces to the outside world are 4 Inputs (I-points) that represent 
+the production lines and 10 Outputs (O-points) for shipping. At I-points the 
+delivered pallets are picked up and transported to a storage location. Upon the 
+arrival of a retrieval order, pallets are provided at the O-points. O-points are
+the staging areas in front of the dock doors. The truck loading process is not 
+part of the use-case since it is executed by the truck drivers.
+
+The warehouse layout is provided as csv-file with numbers from -5 to 0. A -5 
+represents a travel path, -4 an O-point, -3 an I-point, -2 an aisle, -1 the 
+warehouse boundaries and 0 the available storage locations.
+
+<p align="center">
+	<img src="readme/setup_a_layout_v3.png" alt="layout" width="700"/>
+</p>
+
+#### Initial fill level
+
+The initial fill level is a dictionary of Stock Keeping Unit (SKUs) with the 
+respective amount currently on stock at time zero. 
+
+<p align="center">
+	<img src="readme/initial_fill_lvl_1.png" alt="ini_fill" width="350"/>
+</p>
+
+#### Order stream
+
+The order stream represents the daily in- and outbound flow with the exact 
+arrival times of each delivery or retrieval order for a time period of 89 days 
+(amounting to 4e5 orderes). Each order corresponds to a single pallet. 
+While the inbound flow is based on a production frequency of 60 to 120 seconds, 
+the outbound flow is mainly in full truck loads (FTL) with 33 pallets.
+
+The orders are provided as a nested list. Each order comes with six parameters 
+namely the type (delivery or retrieval), the SKU (number from 1 to 136), 
+the order arrival time (absolute time in seconds counting from zero), 
+the dock door (number from 1 to 4 from top to bottom for delivery and 1 to 10 
+from left to right for retrieval), the batch number (number of production 
+batches from 1 to 1498 for delivery and of truckload batches from 1 to 7496 
+for retrieval) and the week number (from 1 to 14).
+
+<p align="center">
+	<img src="readme/order_stream_v1.png" alt="orders" width="500"/>
+</p>
+
+### CrossStacks
+`CROSSStacks`, that was constructed based on two weeks of orders of a 
+medium-sized, manually operated cross-docking terminal for food industry goods 
+run by a large freight company. The data we provide was gathered with the help 
+of a process mining company focusing on increasing the transparency of (manual) 
+industrial processes without revealing any sensitive customer information.
+
+As opposed to `WEPAStacks` the `CrossStacks` dataset consists of only two 
+components, bacause the warehouse is empty at the beginning of a new day.
+
+1. the warehouse layout
+3. the order stream
+
+#### Layout
+
+The figure below depicts an overlay of the warehouse layout and storage regions 
+tracked by the process mining company.
+Yellow boxes represent inbound docks, brown boxes represent outboutnd docks.
+The storage bays are represented by empty black rectangles.
+The green-filled rectangles represent the storage regions tracked by the process
+mining company.
+Within the current use case stacking is not allowed.
+
+<p align="center">
+	<img src="readme/crossstacks_layout__real_sim_overlay_anon-1.png" alt="orders" width="500"/>
+</p>
+
+#### Order Stream
+Cross-docking orders contain add a sixth field, namely the destination dock, to 
+the structure previously described (cmp. figure below). 
+This field is only relevant for delivery orders. 
+
+The destination field was unavailable to us in an explicit form and needed to be 
+inferred from the data. 
+To that end, we used the motion tracking information together with a FIFO 
+assumption to extract the destination dock of inbound orders: We aligned the 
+orders entering and exiting the green storage regions in the layout figures 
+using tracking timestamps and assigned the outbound docks to the corresponding 
+inbound orders.
+
+<p align="center">
+	<img src="readme/order_stream_CROSSSTACKS.png" alt="orders" width="500"/>
+</p>
+
+
+## Getting Started
+### Installation
+We publish this project alongside our experiment script and a control package containing various SLAP heuristics as well as a ULSP heuristic. To set up your environment and recreate our experiment results, the following steps can be taken:
+1. Cloning the repository:
+	```
+	git clone https://github.com/malerinc/slapstack.git
+	```
+2. To install the SLAPStack simulation and its controls run the following commands from the project root directory (this will build the Cython extensions and copy the use case data at the appropriate locations):
+	```
+	pip install 1_environment/slapstack
+	pip install 2_control/slapstack-controls
+	```
+3. To run the experiment script, simply execute the `cmp` scripts located in the 
+experiments directory directly under the root:
+	```
+   python slap_strategy_cmp_crossstacks.py
+   python slap_strategy_cmp_wepastacks.py
+   ```
+
+Note that both the `slapstack` and `slapstack-controls` packages are available 
+through pypi as well. To install from pypi, simply run
+
+```
+pip install slapstack
+pip install slapstack-controls
+```
+
+## Citing the Project
+If you use `SLAPStack` or `WEPAStacks` in your research, you can cite this repository as follows:
+
+```
+@misc{rinciog2023slapstack
+    author = {Rinciog, Alexandru and Pfrommer, Jakob and Morrissey Michael 
+      and Sohaib Zahid and Vasileva, Anna and Ogorelysheva, Natalia and 
+      Rathod, Hardik and Meyer Anne},
+    title = {SLAPStack},
+    year = {2023},
+    publisher = {GitHub},
+    journal = {GitHub Repository},
+    howpublished = {\url{https://github.com/malerinc/slapstack.git}},
+}
+```
+
+## References
+<a id="pfrommer2020">[1]</a> Pfrommer, J., Meyer, A.: Autonomously organized block stacking warehouses: A
+review of decision problems and major challenges. Logistics Journal: Proceedings
+2020(12) (2020)
+
+<a id="rinciog2020">[2]</a> Rinciog, A., Meyer, A.: Fabricatio-rl: a reinforcement learning simulation frame-
+work for production scheduling. In: 2021 Winter Simulation Conference (WSC).
+pp. 1–12. IEEE (2021)
+
+
+
```

### Comparing `slapstack-0.0.24/README.md` & `slapstack-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,125 +1,286 @@
+Metadata-Version: 2.1
+Name: slapstack
+Version: 0.1.1
+Summary: An Event Discrete Simulation Framework for Block-Stacking Warehouses.
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >3.6.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # SLAPStack 
-SLAPStack is a block-stacking warehouse simulation for the Autonomous Block Stacking Warehouse Problem (ABSWP) [[1]](#pfrommer2020) implementing the [OpenAI](https://gym.openai.com/) gym interface. The code can be used to test out Storage Location Allocation Problem (SLAP) and Unit Load Selection Problem (ULSP) algorithms individually or in conjunction. The simulation project includes the WEPAStacks data which includes the layout and 3 months of order information of a large-scale real-world clock stacking warehouse from [WEPA Hygieneprodukte GmbH](https://www.wepa.eu/de/)
+SLAPStack is a block-stacking warehouse simulation for the Autonomous Block 
+Stacking Warehouse Problem (ABSWP) [[1]](#pfrommer2020) implementing the 
+[OpenAI](https://gym.openai.com/) gym interface. 
+The code can be used to test out Storage Location Allocation Problem (SLAP) and 
+Unit Load Selection Problem (ULSP) algorithms individually or in conjunction. 
+
+The simulation project includes the `WEPAStacks` data which includes the layout 
+and 3 months of order information of a large-scale real-world clock stacking 
+warehouse from [WEPA Hygieneprodukte GmbH](https://www.wepa.eu/de/).
+Additionally, an anonymized use case dataset, `CrossStacks` associated with a 
+medium-sized cross-docking terminal is made available. `CrossStacks` 
 
 ## SLAPStack Simulation
 ### Architecture
 
-The project architecture follows the one introduced in [[2]](#rinciog2020), as can be seen in the partial class diagram below. The simulation entry point, which implements the gym interface is located in the `SlapEnv` class located in the `interface.py` module. `SlapEnv`, whose primary function is action- and state-space configuration and transformation, is a wrapper around the `SlapCore` which contains the simulation logic. 
-
-`SlapCore` is responsible for advancing the simulation when calling `step`. It uses an `EventManager` object to maintain the `Event` queues. The central SLAPStack communication structure is given by the `State` object contained by the `SlapCore`.  
-
-The `State` contains several manager objects dedicated to distinct tasks. The `RouteManager`, for instance, is used to compute routes on the storage matrix `S` grid during `Transport` event initialization. The 3D state matrices `S`  (pallet SKUs information), `V` (vehicle positions), `B` (pallet batch information), and `T` (pallet arrival information) are shared between `State` and manager objects as needed (e.g. `V` is shared between `AmrManager` and `State`). 
-
-The `interface_templates.py` module defines and documents the simulation parameter as well as the `SlapEnv` configuration objects, i.e. `Strategy` for allowing indirect actions and `OutputConverter` for transforming both the state representation and the reward returned by `SlapEnv.step()`.
+The project architecture follows the one introduced in [[2]](#rinciog2020), 
+as can be seen in the partial class diagram below. The simulation entry point, 
+which implements the gym interface is located in the `SlapEnv` class located in 
+the `interface.py` module. `SlapEnv`, whose primary function is action- and 
+state-space configuration and transformation, is a wrapper around the `SlapCore`
+which contains the simulation logic. 
+
+`SlapCore` is responsible for advancing the simulation when calling `step`. It 
+uses an `EventManager` object to maintain the `Event` queues. The central 
+SLAPStack communication structure is given by the `State` object contained by 
+the `SlapCore`.  
+
+The `State` contains several manager objects dedicated to distinct tasks. 
+The `RouteManager`, for instance, is used to compute routes on the storage 
+matrix `S` grid during `Transport` event initialization. The 3D state matrices 
+`S`  (pallet SKUs information), `V` (vehicle positions), 
+`B` (pallet batch information), and `T` (pallet arrival information) are shared 
+between `State` and manager objects as needed (e.g. `V` is shared between 
+`AmrManager` and `State`). 
+
+The `interface_templates.py` module defines and documents the simulation 
+parameter as well as the `SlapEnv` configuration objects, i.e. `Strategy` for 
+allowing indirect actions and `OutputConverter` for transforming both the state 
+representation and the reward returned by `SlapEnv.step()`.
 
 <p align="center">
 	<img src="readme/SLAPStack - UML Class.png" alt="class_diagram" width="1000"/>
 </p>
 
 
 ### Events
-At the core of the simulation lies the `future_events` queue. `future_events` is a time-sorted heap of self-handling events. During a simulation step, events are popped from this heap and their handle function is called leading to a state update. If a triggered event requires an external ULSP or SLAP decision, the execution halts, and the state is returned.
-Events are either orders or transport events. Orders (`Delivery` or `Retrieval`) get added to the queue during initialization. Transport events (`Delivery/RetrievalFirst/SecondLeg`) are created on-demand. Of the 6 events present in the simulation, 2 are blocking, namely `Retrieval` and `DeliverySecondLeg`. The relationship between them is depicted event chain summary below.
+At the core of the simulation lies the `future_events` queue. `future_events` is 
+a time-sorted heap of self-handling events. During a simulation step, events are 
+popped from this heap and their handle function is called leading to a state 
+update. If a triggered event requires an external ULSP or SLAP decision, the 
+execution halts, and the state is returned.
+Events are either orders or transport events. Orders (`Delivery` or `Retrieval`) 
+get added to the queue during initialization. Transport events 
+(`Delivery/RetrievalFirst/SecondLeg`) are created on-demand. Of the 6 events 
+present in the simulation, 2 are blocking, namely `Retrieval` and 
+`DeliverySecondLeg`. The relationship between them is depicted event chain 
+summary below.
 
 <p align="center">
 	<img src="readme/event_overview.png" alt="event_chains" width="1000"/>
 </p>
 
 
 ### Routing and Runtime
 
-The design lain down in [[2]](#rinciog2020) and implemented by SLAPStack leads to an efficient runtime in terms of event management and state updates. All state updates are run in constant or amortized constant time. Since, `future_events` is a binary heap, pushing `Order` events to it during initialization and  `Transport` events to it during `step` takes logarithmic time with respect to the total number of orders. This yields an asymptotic runtime of O(n log(n)), where n is the number of orders.
+The design lain down in [[2]](#rinciog2020) and implemented by SLAPStack leads 
+to an efficient runtime in terms of event management and state updates. 
+All state updates are run in constant or amortized constant time. 
+Since, `future_events` is a binary heap, pushing `Order` events to it during 
+initialization and  `Transport` events to it during `step` takes logarithmic 
+time with respect to the total number of orders. This yields an asymptotic 
+runtime of O(n log(n)), where n is the number of orders.
+
+However, a particularity of SLAPStack is the fine-grained routing mechanism 
+implemented. Whenever a `Transport` event is created, the exact closest grid 
+cell route between the AMRs current position and its destination is computed. 
+Dijkstra takes O(m log(m + l)) where m is the number of nodes and l is the 
+number of edges in the routing graph. In our case, that would amount to 
+O(m log m) with m being the number of grid cells in the BSWP (each grid cell is 
+a routing graph node and each cell has four bidirectional edges, 
+i.e. O(m log(m + l) = O(m log(m + 4m)) = O(m log(m)). 
+To deal with this routing bottleneck, SLAPStack's `RouteManager` precomputes 
+all routes over aisle tiles (the light blue tiles in the figure below) using 
+the Floyed Warshall algorithm implemented in `scipy`. The exact route 
+computation is then completed by adding lane traversal segments which runs in 
+constant time (see figure).
 
-However, a particularity of SLAPStack is the fine-grained routing mechanism implemented. Whenever a `Transport` event is created, the exact closest grid cell route between the AMRs current position and its destination is computed. Dijkstra takes O(m log(m + l)) where m is the number of nodes and l is the number of edges in the routing graph. In our case, that would amount to O(m log m) with m being the number of grid cells in the BSWP (each grid cell is a routing graph node and each cell has four bidirectional edges, i.e. O(m log(m + l) = O(m log(m + 4m)) = O(m log(m)). To deal with this routing bottleneck, SLAPStack's `RouteManager` uses a Cython implementation of Dijkstra, route caching, and uses only an aisle grid tiles for routing (the light blue tiles in the figure below).
-
-Simulating a total of 400000 orders on CPU take around 2 hours.
+Simulating a total of 400000 orders on CPU take around 1 hour.
 
 <p align="center">
 	<img src="readme/routing_scheme.png" alt="routing" width="350"/>
 </p>
 
+### Extensions
+
+The latest version of this simulation contains extensions necessary to 
+accommodate cross-docking use-cases and dual command cycle heuristics. These 
+extensions are:
+* dock to dock transports
+* order queueing on AMRs
 
+Additionally, AMRs are capable or transporting more than one load at a time 
+(multiple forks).  
 
-## Use Case Data: WEPAStacks 
+## Use Case Data
+
+### WEPAStacks 
 
 This dataset is based on a real-world block stacking warehouse from WEPA.
 
-WEPA is one of the largest hygienic paper manufacturers in Europe with production plants and warehouses in currently six European countries (www.wepa.eu).
+WEPA is one of the largest hygienic paper manufacturers in Europe with 
+production plants and warehouses in currently six European countries 
+(www.wepa.eu).
 
 The dataset consists of three components:
 
 1. the warehouse layout
 2. the initial fill level
 3. the order stream
 
-### Warehouse Layout
-
-The grid-based warehouse layout shown in the figure below is used to store finished goods on standardized EUR-pallets that can be stacked up to 3 levels. The capacity of the warehouse is up to 19512 storage locations (6504 on the ground with stacking). The light-gray area shows the bidirectional pathways (aisles). Dependent on the type of vehicle they are double/three-lanes wide. The storage bays/lanes are the white areas with separating lines. The dark-gray surrounding wall and truck loading zone define the boundaries of the storage system. Interfaces to the outside world are 4 Inputs (I-points) that represent the production lines and 10 Outputs (O-points) for shipping. At I-points the delivered pallets are picked up and transported to a storage location. Upon the arrival of a retrieval order, pallets are provided at the O-points. O-points are the staging areas in front of the dock doors. The truck loading process is not part of the use-case since it is executed by the truck drivers.
+#### Warehouse Layout
 
-The warehouse layout is provided as csv-file with numbers from -5 to 0. A -5 represents a travel path, -4 an O-point, -3 an I-point, -2 an aisle, -1 the warehouse boundaries and 0 the available storage locations.
+The grid-based warehouse layout shown in the figure below is used to store 
+finished goods on standardized EUR-pallets that can be stacked up to 3 levels. 
+The capacity of the warehouse is up to 19512 storage locations (6504 on the 
+ground with stacking). The light-gray area shows the bidirectional pathways 
+(aisles). Dependent on the type of vehicle they are double/three-lanes wide. 
+The storage bays/lanes are the white areas with separating lines. The dark-gray 
+surrounding wall and truck loading zone define the boundaries of the storage 
+system. Interfaces to the outside world are 4 Inputs (I-points) that represent 
+the production lines and 10 Outputs (O-points) for shipping. At I-points the 
+delivered pallets are picked up and transported to a storage location. Upon the 
+arrival of a retrieval order, pallets are provided at the O-points. O-points are
+the staging areas in front of the dock doors. The truck loading process is not 
+part of the use-case since it is executed by the truck drivers.
+
+The warehouse layout is provided as csv-file with numbers from -5 to 0. A -5 
+represents a travel path, -4 an O-point, -3 an I-point, -2 an aisle, -1 the 
+warehouse boundaries and 0 the available storage locations.
 
 <p align="center">
 	<img src="readme/setup_a_layout_v3.png" alt="layout" width="700"/>
 </p>
 
-### Initial fill level
+#### Initial fill level
 
-The initial fill level is a dictionary of Stock Keeping Unit (SKUs) with the respective amount currently on stock at time zero. 
+The initial fill level is a dictionary of Stock Keeping Unit (SKUs) with the 
+respective amount currently on stock at time zero. 
 
 <p align="center">
 	<img src="readme/initial_fill_lvl_1.png" alt="ini_fill" width="350"/>
 </p>
 
-### Order stream
+#### Order stream
 
-The order stream represents the daily in- and outbound flow with the exact arrival times of each delivery or retrieval order for a time period of 89 days (amounting to 4e5 orderes). Each order corresponds to a single pallet. While the inbound flow is based on a production frequency of 60 to 120 seconds, the outbound flow is mainly in full truck loads (FTL) with 33 pallets.
-
-The orders are provided as a nested list. Each order comes with six parameters namely the type (delivery or retrieval), the SKU (number from 1 to 136), the order arrival time (absolute time in seconds counting from zero), the dock door (number from 1 to 4 from top to bottom for delivery and 1 to 10 from left to right for retrieval), the batch number (number of production batches from 1 to 1498 for delivery and of truckload batches from 1 to 7496 for retrieval) and the week number (from 1 to 14).
+The order stream represents the daily in- and outbound flow with the exact 
+arrival times of each delivery or retrieval order for a time period of 89 days 
+(amounting to 4e5 orderes). Each order corresponds to a single pallet. 
+While the inbound flow is based on a production frequency of 60 to 120 seconds, 
+the outbound flow is mainly in full truck loads (FTL) with 33 pallets.
+
+The orders are provided as a nested list. Each order comes with six parameters 
+namely the type (delivery or retrieval), the SKU (number from 1 to 136), 
+the order arrival time (absolute time in seconds counting from zero), 
+the dock door (number from 1 to 4 from top to bottom for delivery and 1 to 10 
+from left to right for retrieval), the batch number (number of production 
+batches from 1 to 1498 for delivery and of truckload batches from 1 to 7496 
+for retrieval) and the week number (from 1 to 14).
 
 <p align="center">
 	<img src="readme/order_stream_v1.png" alt="orders" width="500"/>
 </p>
 
+### CrossStacks
+`CROSSStacks`, that was constructed based on two weeks of orders of a 
+medium-sized, manually operated cross-docking terminal for food industry goods 
+run by a large freight company. The data we provide was gathered with the help 
+of a process mining company focusing on increasing the transparency of (manual) 
+industrial processes without revealing any sensitive customer information.
+
+As opposed to `WEPAStacks` the `CrossStacks` dataset consists of only two 
+components, bacause the warehouse is empty at the beginning of a new day.
+
+1. the warehouse layout
+3. the order stream
+
+#### Layout
+
+The figure below depicts an overlay of the warehouse layout and storage regions 
+tracked by the process mining company.
+Yellow boxes represent inbound docks, brown boxes represent outboutnd docks.
+The storage bays are represented by empty black rectangles.
+The green-filled rectangles represent the storage regions tracked by the process
+mining company.
+Within the current use case stacking is not allowed.
+
+<p align="center">
+	<img src="readme/crossstacks_layout__real_sim_overlay_anon-1.png" alt="orders" width="500"/>
+</p>
+
+#### Order Stream
+Cross-docking orders contain add a sixth field, namely the destination dock, to 
+the structure previously described (cmp. figure below). 
+This field is only relevant for delivery orders. 
+
+The destination field was unavailable to us in an explicit form and needed to be 
+inferred from the data. 
+To that end, we used the motion tracking information together with a FIFO 
+assumption to extract the destination dock of inbound orders: We aligned the 
+orders entering and exiting the green storage regions in the layout figures 
+using tracking timestamps and assigned the outbound docks to the corresponding 
+inbound orders.
+
+<p align="center">
+	<img src="readme/order_stream_CROSSSTACKS.png" alt="orders" width="500"/>
+</p>
+
 
 ## Getting Started
 ### Installation
 We publish this project alongside our experiment script and a control package containing various SLAP heuristics as well as a ULSP heuristic. To set up your environment and recreate our experiment results, the following steps can be taken:
 1. Cloning the repository:
 	```
 	git clone https://github.com/malerinc/slapstack.git
 	```
 2. To install the SLAPStack simulation and its controls run the following commands from the project root directory (this will build the Cython extensions and copy the use case data at the appropriate locations):
 	```
 	pip install 1_environment/slapstack
 	pip install 2_control/slapstack-controls
 	```
-3. To run the experiment script, simply execute the `storage_strategy_comparison.py` script located in the experiments directory directly under the root:
+3. To run the experiment script, simply execute the `cmp` scripts located in the 
+experiments directory directly under the root:
 	```
-   python storage_strategy_comparison.py
+   python slap_strategy_cmp_crossstacks.py
+   python slap_strategy_cmp_wepastacks.py
    ```
 
+Note that both the `slapstack` and `slapstack-controls` packages are available 
+through pypi as well. To install from pypi, simply run
+
+```
+pip install slapstack
+pip install slapstack-controls
+```
+
 ## Citing the Project
 If you use `SLAPStack` or `WEPAStacks` in your research, you can cite this repository as follows:
 
 ```
-@misc{rinciog2022slapstack
-    author = {Rinciog, Alexandru and Pfrommer, Jakob and Morrissey Michael and Sohaib Zahid and Meyer Anne},
-    title = {FabricatioRL},
-    year = {2021},
+@misc{rinciog2023slapstack
+    author = {Rinciog, Alexandru and Pfrommer, Jakob and Morrissey Michael 
+      and Sohaib Zahid and Vasileva, Anna and Ogorelysheva, Natalia and 
+      Rathod, Hardik and Meyer Anne},
+    title = {SLAPStack},
+    year = {2023},
     publisher = {GitHub},
     journal = {GitHub Repository},
     howpublished = {\url{https://github.com/malerinc/slapstack.git}},
 }
 ```
 
 ## References
 <a id="pfrommer2020">[1]</a> Pfrommer, J., Meyer, A.: Autonomously organized block stacking warehouses: A
 review of decision problems and major challenges. Logistics Journal: Proceedings
 2020(12) (2020)
 
 <a id="rinciog2020">[2]</a> Rinciog, A., Meyer, A.: Fabricatio-rl: a reinforcement learning simulation frame-
 work for production scheduling. In: 2021 Winter Simulation Conference (WSC).
-pp. 1–12. IEEE (2021)
+pp. 1â€“12. IEEE (2021)
+
+
```

### Comparing `slapstack-0.0.24/slapstack/core.py` & `slapstack-0.1.1/slapstack/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import time
-from typing import Tuple, List, Any
+from typing import Tuple, List, Any, Union
 
 import gym
 import numpy as np
 from slapstack.core_events import (Retrieval, RetrievalFirstLeg,
                                    DeliverySecondLeg, Travel, Delivery, Event,
                                    DeliveryFirstLeg, RetrievalSecondLeg)
 from slapstack.core_state import State
 from slapstack.core_state_agv_manager import AGV
 from slapstack.core_state_lane_manager import LaneManager
 from slapstack.core_state_location_manager import LocationManager
-from slapstack.extensions import c_unravel
-from slapstack.helpers import faster_deepcopy
+from slapstack.helpers import faster_deepcopy, unravel
 from slapstack.core_logger import MatrixLogger
 from slapstack.core_events import EventManager, EventHandleInfo
 from slapstack.interface_input import Input
 from slapstack.interface_templates import SimulationParameters, SlapLogger
 
 
 # from line_profiler_pycharm import profile
@@ -110,14 +109,15 @@
         elif isinstance(logger, SlapLogger):
             self.logger = logger
         else:
             raise ValueError("Unsupported logger type. Pass either a relative "
                              "directory path or an object of type 'SlapLogger' "
                              "as defined by the interface_templates.py module. "
                              "To deactivate logging pass the empty string.")
+        self.logger.set_state(self.state)
 
     # def __init_legal_actions(self):
     #     sc = self.state.sc
     #     ual = sc.get_unassigned_open_storage_locations()
     #     for sku in range(1, self.state.n_skus + 1):
     #         if sku in sc.occupied_lanes.keys():
     #             sc.legal_retrieval_actions[sku] = (
@@ -249,15 +249,15 @@
         if not self.orders.generate_orders:
             self.create_orders_from_list()
         else:
             self.create_orders_from_distribution()
         self.state.add_orders(self.events.running)
         self._add_initial_pallets()
         assert self.events.running
-        self.logger.log_state(self.state)
+        self.logger.log_state()
         # self.add_silent_storage_state()
         # self.__init_legal_actions()
         self.step_no_action()
 
     # @profile
     def step_no_action(self):
         """
@@ -281,15 +281,16 @@
         retrieval_ok = e.available_retrieval(s)
         delivery_ok = e.available_delivery(s)
         while (not action_needed
                and (e.running or retrieval_ok or delivery_ok)):
             self.print("~" * 150 + "\n" + "step no action \n" + "~" * 150)
             next_event = None
             # if there are serviceable queued events, take care of them first.
-            if (retrieval_ok or delivery_ok) and s.agv_manager.agv_available():
+            if (retrieval_ok or delivery_ok) and\
+                    s.agv_manager.agv_available(order_type=None, only_new=True):
                 next_event = e.pop_queued_event(s)
             if next_event is None:
                 if not e.running:
                     return True
                 next_event = e.pop_future_event()
             action_needed = self.handle_event_and_update_env(next_event)
             sc.invalidate_sku_location_cache()
@@ -329,28 +330,34 @@
         self.print("current time: " + str(next_event.time))
         self.print("popped event: " + str(next_event))
         elapsed_time = round(next_event.time -
                              self.state.time, 2)
         self.state.trackers.update_time(elapsed_time)
         #  travel events need to be updated by time_to_simulate
         self.process_travel_events(elapsed_time)
-        if next_event.time > self.state.time:
-            self.state.time = next_event.time
+        # if next_event.time > self.state.time:
+        #     self.state.time = next_event.time
         # handle event and see if an action is needed and what data
         # structures should the next (or same) event be added to
-        event_queueing_info: EventHandleInfo = next_event.handle(self.state)
-        self.events.add_current_events(event_queueing_info)
+        if isinstance(next_event, DeliverySecondLeg) or\
+                isinstance(next_event, RetrievalSecondLeg)\
+                or isinstance(next_event, Delivery):
+            event_queueing_info: EventHandleInfo =\
+                next_event.handle(self.state, self)
+        else:
+            event_queueing_info: EventHandleInfo = next_event.handle(self.state)
+        self.events.add_current_events(event_queueing_info, self.state)
         self.update_prev_event_and_curr_order(
             next_event, event_queueing_info.queued_retrieval_order_to_add)
         self.print(self.state)
         self.print("SKU counts: " + str(self.SKU_counts))
         if self.verbose:
             self.print_any_events()
         self.state.n_silent_steps += 1
-        self.logger.log_state(self.state)
+        self.logger.log_state()
         # self.add_silent_storage_state()
         return event_queueing_info.action_needed
 
     def __print_debug_info(self, action: Tuple[int, int, int]):
         """just prints time and action taken"""
         self.print("~" * 150 + "\n" + "step with action \n" + "~" * 150)
         self.print("time: " + str(self.state.time))
@@ -361,25 +368,25 @@
         """key function that takes an action from an agent, randomly, or from
         a storage or retrieval strategy. first action is converted from an int
         to a 3D tuple that fits the warehouse shape, then depending on if the
         current order is a delivery or retrieval order, it creates a
         DeliverySecondLeg or RetrievalFirstLeg event, respectively. Updates
         event data structures, and executes step_no_action(). If the simulation
         is done afterwards, it can be ended here."""
-        action = c_unravel(action, self.inpt.params.shape)
+        action = unravel(action, self.inpt.params.shape)
         self.state.n_steps += 1
         self.__print_debug_info(tuple(action))
         travel_event = None
         if self.decision_mode == "delivery":
             travel_event = self.__create_event_on_delivery(action)
         elif self.decision_mode == "retrieval":
             travel_event = self.__create_event_on_retrieval(action)
         self.state.add_travel_event(travel_event)
-        self.events.add_travel_event(travel_event)
-        self.logger.log_state(self.state)
+        self.events.add_travel_event(travel_event, self.state)
+        self.logger.log_state()
         done_prematurely = self.step_no_action()
         return self.__has_ended(done_prematurely)
 
     def __has_ended(self, done_prematurely: bool) -> (State, bool):
         # sc, e = self.state.location_manager, self.events
         # free_agvs = sum([v for _, v in sc.free_agv_positions.items()])
         # busy_agvs = len(self.events.current_travel)
@@ -396,56 +403,110 @@
         else:
             return self.state, False,  # state, done
 
     def __create_event_on_delivery(
             self, action: Tuple[int, int, int]) -> DeliverySecondLeg:
         lm: LaneManager = self.state.location_manager.lane_manager
         prev_e: DeliveryFirstLeg = self.previous_event
-        if lm.pure_lanes:
+        state_cache_sink = self.state.location_manager.sink_location
+        self.state.location_manager.sink_location = None
+        retrieval_order: Retrieval = None
+        if state_cache_sink and\
+                unravel(state_cache_sink,
+                          self.state.location_manager.S.shape) == action:
+            agv: AGV = self.state.agv_manager.agv_index[prev_e.agv_id]
+            found_in_dcc_orders = False
+            for ret_dcc_order in agv.dcc_retrieval_order:
+                if ret_dcc_order.SKU == prev_e.order.SKU:
+                    found_in_dcc_orders = True
+                    retrieval_order = ret_dcc_order
+            if not found_in_dcc_orders:
+                retrieval_order = self.events.queued_retrieval_orders[
+                    prev_e.order.SKU].popleft()
+                self.events.n_queued_retrieval_orders -= 1
+            if len(self.events.queued_retrieval_orders[prev_e.order.SKU]) == 0:
+                del self.events.queued_retrieval_orders[prev_e.order.SKU]
+        if lm.pure_lanes and not retrieval_order:
             lm.add_lane_assignment(action, prev_e.order.SKU)
         travel_event = DeliverySecondLeg(
             state=self.state,
-            start_point=self.state.source_positions[prev_e.source],
+            start_point=prev_e.last_node,
             end_point=action[0:2],
             travel_type="delivery_second_leg",
             level=int(action[2]),
             source=prev_e.source,
+            orders=prev_e.orders,
             order=prev_e.order,
-            agv_id=prev_e.agv_id
+            agv_id=prev_e.agv_id,
+            servicing_retrieval_order=retrieval_order
         )
         return travel_event
 
     def __create_event_on_retrieval(
             self, action: Tuple[int, int, int]) -> RetrievalFirstLeg:
-        sc: LocationManager = self.state.location_manager
+        lm: LocationManager = self.state.location_manager
         prev_e: Retrieval = self.previous_event
-        agv: AGV = self.state.agv_manager.book_agv(action[0:2], self.state.time)
-        self.state.agv_manager.update_v_matrix(agv.position, None)
-        travel_event = RetrievalFirstLeg(
-            state=self.state, start_point=agv.position,
-            end_point=action[0:2],
-            travel_type="retrieval_first_leg",
-            level=int(action[2]),
-            sink=self.previous_event.sink,
-            order=prev_e, agv_id=agv.id)
+        agv_pos, index = self.state.agv_manager.get_close_agv(
+            action[0:2], prev_e.type)
+        agv: AGV = self.state.agv_manager.book_agv(
+            agv_pos, self.state.time, index, prev_e.type)
+        cross_dock = lm.source_location
+        lm.source_location = None
+        delivery_order: Union[Delivery, None] = None
+        # cross-docking action; agv will travel to the source to get ret pallet
+        if cross_dock and unravel(cross_dock, lm.S.shape) == action:
+            previous_sku = self.previous_event.SKU
+            delivery_order = self.events.queued_delivery_orders[
+                previous_sku].popleft()
+            self.events.n_queued_delivery_orders -= 1
+            if len(self.events.queued_delivery_orders[previous_sku]) == 0:
+                del self.events.queued_delivery_orders[previous_sku]
+
+        if len(agv.dcc_retrieval_order) == 0 and agv.forks > 1 and\
+                agv.available_forks < agv.forks - 1:
+            travel_event: RetrievalFirstLeg = self.events.find_travel_event(
+                agv.id, RetrievalFirstLeg)
+            self.events.remove_travel_event(travel_event)
+            self.events.running.remove(travel_event)
+            self.events.re_heapify_heap()
+            travel_event.orders.append(prev_e)
+            travel_event.actions.append(action)
+            if delivery_order is not None:
+                travel_event.delivery_orders = (
+                    travel_event.delivery_orders.append(delivery_order))
+            else:
+                lm.lock_lane(action[0:2])
+        else:
+            self.state.agv_manager.update_v_matrix(agv.position, None)
+            travel_event = RetrievalFirstLeg(
+                state=self.state, start_point=agv.position,
+                end_point=action[0:2],
+                travel_type="retrieval_first_leg",
+                level=int(action[2]),
+                sink=self.previous_event.sink,
+                orders=[prev_e],
+                order=prev_e,
+                actions=[action], agv_id=agv.id,
+                servicing_delivery_order=[delivery_order]
+                if delivery_order is not None else [])
         return travel_event
 
     def update_prev_event_and_curr_order(
             self, this_event: Event, queued_retrieval_order_to_add: Retrieval):
         """
         Updates the decision_mode and previous_event fields in the case of a
         blocking event.
 
-        The previous_event field is used to associate order information with 
+        The previous_event field is used to associate order information with
         travel events, on decisions. It only gets instantiated if the current_
         event is blocking, i.e. DeliveryFirstLeg or RetrievalOrder. After the
-        decision, the order information saved will be used to generate 
+        decision, the order information saved will be used to generate
         DeliverySecondLeg and RetreivalFirstLeg information events.
-         
-        :param this_event: The event to be saved if a decision is to be made in 
+
+        :param this_event: The event to be saved if a decision is to be made in
             the next step.
         :param queued_retrieval_order_to_add: The Retrieval that was added to
             the queue of currently unseviceable orders (event was unblocking and
             these updates will be overriden) or None if the oreder can be
             serviced.
         :return: None
         """
@@ -455,27 +516,30 @@
                 or isinstance(this_event, DeliveryFirstLeg)
                 or isinstance(this_event, DeliverySecondLeg)):
             self.decision_mode = "delivery"
             if isinstance(this_event, DeliveryFirstLeg):
                 self.previous_event = this_event
             if isinstance(this_event, DeliverySecondLeg):
                 self.SKU_counts[this_event.order.SKU] += 1
+                self.previous_event = this_event
         if (isinstance(this_event, Retrieval)
                 or isinstance(this_event, RetrievalFirstLeg)
                 or isinstance(this_event, RetrievalSecondLeg)):
             self.decision_mode = "retrieval"
             if (isinstance(this_event, Retrieval)
                     and not queued_retrieval_order_to_add):
                 self.previous_event = this_event
                 self.SKU_counts[this_event.SKU] -= 1
                 self.print("SKU counts: " + str(self.SKU_counts))
 
     def process_travel_events(self, elapsed_time: float):
         """ if time has elapsed, update any currently active travel events"""
-        if self.events.current_travel and elapsed_time > 0:
+        if (self.events.current_travel
+                and elapsed_time > 0
+                and self.state.params.update_partial_paths):
             self.print("simulating travel events by " + str(elapsed_time))
             self.simulate_travel_events(elapsed_time)
 
     def print_any_events(self):
         """debugging purposes - print any event data structures that aren't
         empty
         """
@@ -488,16 +552,17 @@
             self.print("currently queued retrieval orders: ")
             for i in self.events.queued_retrieval_orders.values():
                 for j in i:
                     self.print("queued: " + str(j))
 
         if self.events.queued_delivery_orders:
             self.print("currently queued delivery orders: ")
-            for i in self.events.queued_delivery_orders:
-                self.print("queued: " + str(i))
+            for i in self.events.queued_delivery_orders.values()():
+                for j in i:
+                    self.print("queued: " + str(j))
 
     def _add_initial_pallets(self):
         """ this function adds pallets/SKUs to the initial storage and arrival
         time matrices. It is versatile and can add a random quantity of SKU
         numbers or it can read from a dictionary from self.orders. The location
         of the initial pallets can either be random free locations, or they can
         follow a storage strategy (i.e. closest to source, furthest from source)
@@ -543,24 +608,24 @@
                                                   chosen_sku] + 1
             else:
                 chosen_sku = int(SKU_choices[i])
             self.state.current_sku = chosen_sku
             if self.orders.follow_storage_strategy():
                 index = self.orders.initial_pallets_storage_strategy.get_action(
                     self.state)
-                index = c_unravel(index, self.inpt.params.shape)
+                index = unravel(index, self.inpt.params.shape)
             else:
                 possible_locations = sc.get_open_locations(chosen_sku)
                 for agv in self.state.agv_manager.get_agv_locations():
                     if agv in possible_locations:
                         possible_locations.remove(agv)
                 assert len(possible_locations), 'warehouse full'
                 index = SlapCore.rng.integers(0, len(possible_locations))
                 index = list(possible_locations)[index]
-                index = c_unravel(index, self.inpt.params.shape)
+                index = unravel(index, self.inpt.params.shape)
             assert len(index) == 3
             # TODO: Add randomization for initial pallets
             batch_id += np.float32(0.0001)
             timestamp += np.float32(0.0001)
             sc.update_on_delivery_second_leg(
                 index, chosen_sku, timestamp, batch_id, init=True
             )
@@ -608,16 +673,22 @@
         the stack (of pallets)
         """
         if self.previous_event:  # DeliveryFirstLeg is the event type
             prev_e: DeliveryFirstLeg = self.previous_event
             self.state.set_current_sku(prev_e.order.SKU)
             self.state.set_current_source_sink(prev_e.source)
             self.state.set_current_order_arrival_time(prev_e.order.time)
+            self.state.set_current_destination(prev_e.order.destination)
         legal_actions = self.state.location_manager.get_open_locations(
             self.state.current_sku)
+        if self.state.door_to_door:
+            legal_sink = self.state.location_manager.get_direct_sink_action(
+                self.state.current_sku)
+            if legal_sink is not None:
+                legal_actions.add(legal_sink)
         self.state.set_current_order(self.decision_mode)
         self.state.set_legal_actions(legal_actions)
         # converts tuple legal actions to linear index
         # legal_actions = [int(np.ravel_multi_index(i, self.warehouse.shape))
         #                  for i in legal_actions]
         if not legal_actions:
             print('herehere!')
@@ -649,24 +720,38 @@
                 batch = 1
                 source_sink -= 1
                 period = None
             elif len(order) == 6:  # coming from use case
                 order_type, sku, arrival_time, source_sink, batch = order[:-1]
                 period = order[-1]
                 source_sink -= 1
+            elif len(order) == 7:
+                order_type, sku, arrival_time, source_sink, destination, batch\
+                    = order[:-1]
+                period = order[-1]
+                source_sink -= 1
+                destination -= 1
             else:
                 raise ValueError("Unknown Order Structure!")
             if order_type == "retrieval":
                 self.events.add_future_event(
                     Retrieval(arrival_time, sku, order_number,
-                              self.verbose, source_sink, batch, period))
+                              self.verbose, source_sink, batch, period),
+                    self.state)
             elif order_type == "delivery":
-                self.events.add_future_event(
-                    Delivery(arrival_time, sku, order_number,
-                             self.verbose, source_sink, batch, period))
+                if len(order) == 6:
+                    self.events.add_future_event(
+                        Delivery(arrival_time, sku, order_number,
+                                 self.verbose, source_sink, batch, period),
+                    self.state)
+                elif len(order) == 7:
+                    self.events.add_future_event(
+                        Delivery(arrival_time, sku, order_number,
+                                 self.verbose, source_sink, batch, period,
+                                 destination), self.state)
             order_number += 1
         self.events.order_times = [i.time for i in self.events.running]
         self.print("")
 
     def print(self, string: Any):
         """this function can be used instead of the python default print(). It
         allows all print statements to be turned on/off with one parameter:
```

### Comparing `slapstack-0.0.24/slapstack/core_events.py` & `slapstack-0.1.1/slapstack/core_events.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import math
 from collections import deque
 
 import numpy as np
 import heapq as heap
-
-from slapstack.core_state_route_manager import Route
 from slapstack.core_state import State
 from slapstack.core_state_agv_manager import AGV
 from slapstack.core_state_location_manager import LocationManager
 from slapstack.helpers import faster_deepcopy, StorageKeys, VehicleKeys, \
-    BatchKeys, TimeKeys, TravelEventKeys
-from typing import Tuple, MutableSequence, Set, Dict, Deque, Any
+    BatchKeys, TimeKeys, TravelEventKeys, ravel, unravel
+from typing import Tuple, MutableSequence, Set, Dict, Deque, Any, Type, List, \
+    Union
+from slapstack.core_state_route_manager import Route
 
 
 class EventHandleInfo:
     def __init__(
             self,
             action_needed: bool,
             event_to_add,
@@ -59,15 +59,17 @@
     def __ge__(self, other):
         return self.time >= other.time
 
     def __gt__(self, other):
         return self.time > other.time
 
     def handle(self, state: State):
-        raise NotImplementedError
+        if self.time > state.time:
+            state.time = self.time
+        # raise NotImplementedError
 
 
 class Order(Event):
     def __init__(self, time: float, SKU: int, order_number: int, batch_id: int,
                  verbose: bool, io_type=None, period=None):
         super().__init__(time, verbose)
         self.SKU = SKU
@@ -84,14 +86,15 @@
         """used for sorting events in heaps"""
         if isinstance(other, Order):
             return self.order_number == other.order_number
         else:
             return False
 
     def handle(self, state: State):
+        super().handle(state)
         state.n_skus_inout_now[self.SKU] += 1
         if self.period != state.params.sku_period:
             state.params.sku_period = self.period
 
     def set_completion_time(self, time: float):
         self.completion_time = time
 
@@ -99,39 +102,50 @@
 class Delivery(Order):
     """delivery order contains a SKU number and source position. seizes a free
     AGV, moves it to source to pick up a pallet, then moves it to a desired
     position in the warehouse and drops off the pallet.
 
     """
     def __init__(self, time: float, SKU: int, order_number: int, verbose: bool,
-                 source: int, batch_id: int = 0, period=None):
+                 source: int, batch_id: int = 0, period=None,
+                 destination: int = None):
         super().__init__(time, SKU, order_number, batch_id, verbose, 'delivery',
                          period)
         self.source = source
+        self.destination = destination
         if self.verbose:
             print("event created: ", self)
 
-    def handle(self, state: State) -> EventHandleInfo:
+    def handle(self, state: State, core=None) -> EventHandleInfo:
         """creates a delivery first leg travel event if there are free AGVs,
         updates agv cache. if there are no free AGVs, the event gets added
         to queued_delivery_orders"""
         super().handle(state)
-        sc: LocationManager = state.location_manager
-        if state.agv_manager.agv_available() and state.delivery_possible():
+        agv_pos, index = state.agv_manager.get_close_agv(
+            state.I_O_positions[self.source], self.type)
+        if (state.agv_manager.agv_available('delivery')
+                and state.delivery_possible(agv_pos, index)):
             agv: AGV = state.agv_manager.book_agv(
-                state.source_positions[self.source], state.time)
-            state.agv_manager.update_v_matrix(agv.position, None)
-            travel_event = DeliveryFirstLeg(
-                state=state, start_point=agv.position,
-                end_point=state.source_positions[self.source],
-                travel_type="delivery_first_leg",
-                level=0, source=self.source, order=self, agv_id=agv.id)
-            state.add_travel_event(travel_event)
-            return EventHandleInfo(
-                False, travel_event, travel_event, None, None)
+                agv_pos, state.time, index, self.type)
+            if agv.forks > 1 and agv.available_forks < agv.forks - 1:
+                existing_event = core.events.find_travel_event(
+                    agv.id, DeliveryFirstLeg)
+                existing_event.orders.append(self)
+                return EventHandleInfo(False, None, None, None, None)
+            else:
+                state.agv_manager.update_v_matrix(agv.position, None)
+                travel_event = DeliveryFirstLeg(
+                    state=state, start_point=agv.position,
+                    end_point=state.I_O_positions[self.source],
+                    travel_type="delivery_first_leg",
+                    level=0, source=self.source, orders=[self],
+                    order=self, agv_id=agv.id)
+                state.add_travel_event(travel_event)
+                return EventHandleInfo(
+                    False, travel_event, travel_event, None, None)
         else:
             if self.verbose:
                 print("no delivery AGV available, adding to queued events")
             return EventHandleInfo(False, None, None, None, self)
 
     def __str__(self):
         return (f'delivery order #{self.order_number} for SKU {self.SKU} that '
@@ -163,30 +177,54 @@
         returns True so that the agent can create a retrieval order with the
         specific pallet location coming from an agent or retrieval policy
         3) if there are no free AGVs, the retrieval order gets queued and is
         added to the queued_retrieval_orders dictionary
         """
         super().handle(state)
         lm: LocationManager = state.location_manager
+        source = None
+        # TODO: check and refactor this method!
         if self.SKU not in lm.lane_manager.occupied_lanes:
             if self.verbose:
-                print("SKU not available.")
-            return EventHandleInfo(False, None, None, self, None)
+                print("SKU not available, adding to unserviceable SKUs")
+            found_waiting_delivery_order = False
+            if self.SKU in lm.events.queued_delivery_orders.keys():
+                delivery_order = lm.events.queued_delivery_orders[self.SKU][0]
+                if isinstance(delivery_order, Delivery):
+                    found_waiting_delivery_order = True
+                    source = delivery_order.source
+            if not found_waiting_delivery_order:
+                return EventHandleInfo(False, None, None, self, None)
+            else:
+                if state.agv_manager.agv_available():
+                    io_locations = State.get_io_locations(state.S)
+                    source_location = ravel(
+                        io_locations[source] + (0,), state.S.shape)
+                    lm.source_location = source_location
+                    return EventHandleInfo(True, None, None, None, None)
+                else:
+                    lm.source_location = None
+                    return EventHandleInfo(False, None, None, self, None)
+            # state.state_cache.unserviceable_retrieval_skus.add(self.SKU)
+            # return EventHandleInfo(False, None, None, self, None)
         if not lm.get_sku_locations(
                 self.SKU, state.trackers.travel_event_statistics):
             if self.verbose:
                 print("SKU available but is currently locked")
+            lm.source_location = None
             return EventHandleInfo(False, None, None, self, None)
 
         # let step() and agent create the retrieval travel event
         if state.agv_manager.agv_available():
+            lm.source_location = None
             return EventHandleInfo(True, None, None, None, None)
         else:
             if self.verbose:
                 print("no retrieval AGV available, adding to queued events")
+            lm.source_location = None
             return EventHandleInfo(False, None, None, self, None)
 
     def __str__(self):
         return (f'retrieval order #{self.order_number} for SKU {self.SKU} '
                 f'arrives at {self.time} at sink {self.sink}')
 
     def __deepcopy__(self, memo):
@@ -195,15 +233,16 @@
 
 class Travel(Event):
     """travel events always have a route and describe what tiles an AGV should
     go through in order to reach a destination
     """
     def __init__(self, state: State, start_point: Tuple[int, int],
                  end_point: Tuple[int, int], travel_type: str,
-                 level: int, order: Order, key: TravelEventKeys, agv_id: int):
+                 level: int, orders: [Order], order: Order,
+                 key: TravelEventKeys, agv_id: int):
         """
         state: State
         start_point: Tuple[int, int]
             first node/tile in the route
         end_point: Tuple[int, int]
             last node/tile in the route
         SKU: int
@@ -221,66 +260,60 @@
             for retrieval travel events, defines the level that a pallet is
             being retrieved from. for delivery travel events, defines the
             level where a pallet should be placed.
 
         """
         self.key = key
         self.agv_id = agv_id
-        route = Route(state.routing, state.location_manager.grid,
-                      start_point, end_point)
-        super().__init__(state.time + route.get_duration(), order.verbose)
+        route = Route(state.routing, start_point, end_point)
+        duration = route.get_duration()
+        self.matriel_handling_time = state.params.material_handling_time
+        super().__init__(state.time + duration + self.matriel_handling_time,
+                         order.verbose)
         self.route = route
         state.add_route(route.get_indices())
         self.travel_type = travel_type
         self.level = level
         if self.verbose:
             print("event created: ", self)
             print("route created:")
-            print(self.route.plot_route())
         # convenience variables set during handle
-        self.first_node = self.route.get_first_node()
-        self.last_node = self.route.get_last_node()
+        self.first_node = start_point
+        self.last_node = end_point
         self.order = order
+        self.orders = orders
+        self.distance_penalty = 0  # from pallet shifts
         state.update_on_travel_event_creation(self.key)
 
     def __hash__(self):
         return hash(str(self.order.order_number) + self.travel_type)
 
     def __eq__(self, other):
         """used for sorting events in heaps"""
         return (self.order.order_number == other.order.order_number
                 and self.travel_type == other.travel_type)
 
-    def handle(self, state: State):
+    def handle(self, state: State, core=None):
         """executed for all types of travel events - correct nodes are set
         based on current route, travel time and distance traveled are calculated
         for trackers"""
+        super().handle(state)
         tk = self.key
         d = self.route.get_total_distance()
         t = self.route.get_duration()
-        state.update_on_travel_event_completion(tk, t, d)
+        p = self.distance_penalty
+        state.update_on_travel_event_completion(tk, t, d, p)
 
     def partial_step_handle(self, state: State, elapsed_time: float):
         previous_first_node = self.route.get_first_node()
         state.remove_route(self.route.get_indices())
-        n_tiles = len(self.route.midpoints)
-        i = 0
-        while i < n_tiles:
-            if self.route.midpoints[i] <= elapsed_time:
-                i += 1
-            else:
-                # pointless to keep iterating since midpoint times are
-                # monotonously increasing ;)
-                break
-        for j in range(i):
-            del self.route.indices[0]
-            del self.route.midpoints[0]
+        self.route.update_path(elapsed_time)
         state.add_route(self.route.get_indices())
         cur_total_time = self.route.get_duration()
-        new_first_node = self.route.get_indices()[0]
+        new_first_node = self.route.get_first_node()
         state.agv_manager.update_v_matrix(
             previous_first_node, new_first_node)
 
     def __str__(self):
         return (f'{self.travel_type} travel with SKU {self.order.SKU} finishes '
                 f'at {self.time} and takes route {self.route} with duration '
                 f'{self.route.get_duration()} to level {self.level}')
@@ -289,23 +322,30 @@
 class RetrievalFirstLeg(Travel):
     """first leg of a travel event used to complete a retrieval order. a free
      AGV is seized and moves from its current position to the tile from where
     it is picking up a pallet
     """
     def __init__(self, state: State, start_point: Tuple[int, int],
                  end_point: Tuple[int, int], travel_type: str,
-                 level: int, sink: int,
-                 order: Order, agv_id: int):
+                 level: int, sink: int, orders: [Order],
+                 order: Order, actions: List[Tuple[int, int, int]],
+                 agv_id: int, servicing_delivery_order: [Delivery]):
         super().__init__(state, start_point, end_point, travel_type,
-                         level, order, TravelEventKeys.RETRIEVAL_1STLEG, agv_id)
+                         level, orders, order,
+                         TravelEventKeys.RETRIEVAL_1STLEG, agv_id)
         self.sink = sink
-        self.delivery_action, self.retrieval_actions = (state.location_manager
-                                                        .lock_lane(end_point))
+        self.delivery_orders = servicing_delivery_order
+        self.actions = actions
+        if len(self.delivery_orders) > 0:
+            self.delivery_action = end_point
+        else:
+            self.delivery_action, self.retrieval_actions = \
+                (state.location_manager.lock_lane(end_point))
 
-    def handle(self, state: State):
+    def handle(self, state: State, core=None):
         """updates agv position in vehicle matrix, removes sku from storage
         and arrival time matrix, removes SKU from occupied locations in cache,
         removes route, removes travel event, creates retrieval second leg travel
         event.
 
         returns:
         action_needed = False
@@ -313,124 +353,239 @@
         travel_event_to_add = travel_event
         queued_retrieval_order_to_add = None
         queued_delivery_order_to_add = None
         """
         super().handle(state)
         pallet_position = self.last_node + (self.level,)
         pallet_cycle_time = state.time - state.T[pallet_position]
-        state.update_s_t_b_matrices(pallet_position, StorageKeys.EMPTY.value,
-                                    TimeKeys.NAN.value, BatchKeys.NAN.value)
-        state.location_manager.unlock_lane(self.delivery_action,
-                                           self.retrieval_actions)
+
+        shift_penalty = \
+            self.update_metrix_lanes(state, pallet_position, pallet_cycle_time)
         assert len(pallet_position) == 3
 
         state.agv_manager.update_v_matrix(self.first_node, self.last_node)
         state.remove_route(self.route.get_indices())
         state.remove_travel_event(self.order.order_number)
-
-        shift_penalty = state.location_manager.update_on_retrieval_first_leg(
-            pallet_position, self.order.SKU, pallet_cycle_time, self.time)
         state.trackers.number_of_pallet_shifts += shift_penalty
         state.n_skus_inout_now[self.order.SKU] -= 1
-        travel_event = RetrievalSecondLeg(
-            state=state, start_point=self.last_node,
-            end_point=state.sink_positions[self.sink],
-            travel_type="retrieval_second_leg",
-            level=0, sink=self.sink,
-            n_shifts=shift_penalty, order=self.order, agv_id=self.agv_id)
-        state.add_travel_event(travel_event)
-        return EventHandleInfo(False, travel_event, travel_event, None, None)
+
+        index = self.orders.index(self.order)
+        if index != len(self.orders) - 1:
+            return self.update_current_event_second_order(state, index,
+                                                          shift_penalty)
+        else:
+            travel_event = RetrievalSecondLeg(
+                state=state, start_point=self.last_node,
+                end_point=state.I_O_positions[self.orders[0].sink],
+                travel_type="retrieval_second_leg",
+                level=0, sink=self.orders[0].sink,
+                n_shifts=shift_penalty, orders=self.orders,
+                order=self.orders[0], agv_id=self.agv_id,
+                servicing_delivery_orders=self.delivery_orders)
+            state.add_travel_event(travel_event)
+            return EventHandleInfo(False, travel_event, travel_event,
+                                   None, None)
 
     def __str__(self):
         return super().__str__()
 
     def __deepcopy__(self, memo):
         return faster_deepcopy(self, memo)
 
+    def update_metrix_lanes(self, state: State,
+                            pallet_position: Tuple[int, int],
+                            pallet_cycle_time: int):
+        shift_penalty = 0
+        if hasattr(self, 'retrieval_actions')\
+                and self.retrieval_actions is not None:
+            state.update_s_t_b_matrices(pallet_position,
+                                        StorageKeys.EMPTY.value,
+                                        TimeKeys.NAN.value, BatchKeys.NAN.value)
+            state.location_manager.unlock_lane(self.delivery_action,
+                                               self.retrieval_actions)
+            state.location_manager.events.\
+                finished_ret_first_leg_skus.append(self.order.SKU)
+            shift_penalty = \
+                state.location_manager.update_on_retrieval_first_leg(
+                    pallet_position, self.order.SKU, pallet_cycle_time,
+                    self.time)
+        else:
+            state.update_s_t_b_matrices(pallet_position,
+                                        StorageKeys.SOURCE.value,
+                                        TimeKeys.NAN.value, BatchKeys.NAN.value)
+        return shift_penalty
+
+    def update_current_event_second_order(self, state: State, index: int,
+                                          shift_penalty: int):
+        self.order = self.orders[index + 1]
+        agv: AGV = state.agv_manager.agv_index.get(self.agv_id)
+        if self.order in agv.dcc_retrieval_order:
+            action = self.find_closest_sku_loc(state, self.order.SKU)
+        else:
+            action = self.actions[index + 1]
+        if action:
+            self.sink = self.order.sink
+            super().__init__(state, self.last_node, action[0:2],
+                             "retrieval_first_leg", action[2], self.orders,
+                             self.order, TravelEventKeys.RETRIEVAL_1STLEG,
+                             self.agv_id)
+            found = False
+            for order in self.delivery_orders:
+                if self.order.SKU == order.SKU:
+                    found = True
+                    self.delivery_action = action[0:2]
+                    self.retrieval_actions = None
+                    break
+            if not found:
+                self.delivery_action, self.retrieval_actions =\
+                    (state.location_manager.lock_lane(action[0:2]))
+            state.add_travel_event(self)
+            return EventHandleInfo(False, self, self, None, None)
+        else:
+            travel_event = RetrievalSecondLeg(
+                state=state, start_point=self.last_node,
+                end_point=state.I_O_positions[self.orders[index].sink],
+                travel_type="retrieval_second_leg",
+                level=0, sink=self.orders[index].sink,
+                n_shifts=shift_penalty, orders=[self.orders[index]],
+                order=self.orders[index], agv_id=self.agv_id,
+                servicing_delivery_orders=self.delivery_orders)
+            state.add_travel_event(travel_event)
+            return EventHandleInfo(False, travel_event, travel_event,
+                                   self.order, None)
+
 
 class RetrievalSecondLeg(Travel):
     """second leg of a travel event used to complete a retrieval order. a busy
      AGV moves from its current position (where it just picked up a pallet) to
      the sink tile where it will drop off the pallet
     """
     def __init__(self, state: State, start_point: Tuple[int, int],
                  end_point: Tuple[int, int], travel_type: str,
                  level: int, sink: int,
-                 n_shifts: int, order: Order, agv_id: int):
+                 n_shifts: int, orders: [Order], order: Order,
+                 agv_id: int, servicing_delivery_orders: [Delivery]):
         super().__init__(state, start_point, end_point, travel_type, level,
-                         order, TravelEventKeys.RETRIEVAL_2ND_LEG, agv_id)
+                         orders, order, TravelEventKeys.RETRIEVAL_2ND_LEG,
+                         agv_id)
         self.sink = sink
         self.time += n_shifts * state.params.shift_penalty
+        self.distance_penalty = n_shifts * state.params.unit_distance * 2
+        self.delivery_orders = servicing_delivery_orders
+        state.agv_manager.agv_index[agv_id].servicing_order_type =\
+            'retrieval_second_leg'
+        self.backtracking_offset = (-1 if self.route.get_indices()[0][0] != 0
+                                    else 1)
 
-    def handle(self, state: State):
+    def handle(self, state: State, core=None):
         """updates agv position in vehicle matrix, removes route, removes travel
         event.
+
         Since multiple AGVs can end up at the same spot (sink tile), this
         function tries to make sure that they are placed on different tiles in
-        the vehicle matrix
+        the vehicle matrix.
+
+        The presence of an AGV at the sink tile is marked by the FREE vehicle
+        key. Busy AGVs are otherwise allowed to overlap, since they are expected
+        to move away in a next step.
 
         returns:
         action_needed = False
         event_to_add = None
         travel_event_to_add = None
         queued_retrieval_order_to_add = None
         queued_delivery_order_to_add = None
         """
         super().handle(state)
         # if the AGV has not reached the sink tile yet or if it's already
         # there (possibly from a simulate_travel_events() advancing it
         # to the last node in its route
         tile_found = False
         offset = 0
-        state.remove_route(self.route.get_indices())
         while not tile_found:
-            vehicle_position = (self.last_node[0] + offset, self.last_node[1])
+            vehicle_position = (self.last_node[0], self.last_node[1] + offset)
             value_at_sink = state.V[vehicle_position]
-            if (value_at_sink == VehicleKeys.N_AGV or
-                    value_at_sink == VehicleKeys.BUSY):
-                last_node = (self.last_node[0] + offset, self.last_node[1])
-                state.agv_manager.update_v_matrix(
-                    self.first_node, self.last_node, True)
-                state.agv_manager.release_agv(
-                    last_node, state.time, self.agv_id)
-                state.remove_route(self.route.get_indices())
-                state.remove_order(self.order.order_number)
-                state.remove_travel_event(self.order.order_number)
-                tile_found = True
-            else:
-                if self.verbose:
-                    print("already an AGV at this tile, "
-                          "checking next tile for free space")
-                offset += 1
+            # if (value_at_sink == VehicleKeys.N_AGV or
+            #         value_at_sink == VehicleKeys.BUSY):
+            # TODO: implement send back to waiting station scheme ;)
+            state.agv_manager.update_v_matrix(self.first_node, self.last_node)
+            state.remove_route(self.route.get_indices())
+            state.remove_order(self.order.order_number)
+            state.remove_travel_event(self.order.order_number)
+            state.update_when_vehicle_free(self.last_node)
+            tile_found = True
+            # else:
+            #     if self.verbose:
+            #         print("already an AGV at this tile, "
+            #               "checking next tile for free space")
+            #     offset = self.backtracking_offset
         if self.verbose:
             print(f"finished retrieval order #{self.order.order_number}")
+
+        self.complete_direct_delivery_order(state, core)
+        state.location_manager.events.\
+            finished_ret_second_leg_skus.append(self.order.SKU)
         self.order.set_completion_time(state.time)
-        state.trackers.update_on_order_completion(self.order)
-        return EventHandleInfo(False, None, None, None, None)
+        state.trackers.update_on_order_completion(
+            self.order, self.distance_penalty)
+        self.orders.pop(0)
+
+        if len(self.orders) > 0:
+            return self.update_current_event_next_order(state)
+        else:
+            last_node = (self.last_node[0] + offset, self.last_node[1])
+            state.agv_manager.update_v_matrix(self.first_node,
+                                              self.last_node, True)
+            state.agv_manager.agv_index.get(self.agv_id).dcc_retrieval_order\
+                = []
+            state.agv_manager.release_agv(last_node, state.time, self.agv_id)
+            return EventHandleInfo(False, None, None, None, None)
 
     def __str__(self):
         return super().__str__()
 
     def __deepcopy__(self, memo):
         return faster_deepcopy(self, memo)
 
+    def complete_direct_delivery_order(self, state: State, core):
+        for order in self.delivery_orders:
+            if self.order.SKU == order.SKU:
+                delivery_order_index = self.delivery_orders.index(order)
+                delivery_order = self.delivery_orders.pop(delivery_order_index)
+                delivery_order.set_completion_time(state.time)
+                state.trackers.update_on_order_completion(delivery_order)
+                state.remove_order(delivery_order.order_number)
+                core.logger.log_state()
+
+    def update_current_event_next_order(self, state: State):
+        self.order = self.orders[0]
+        self.sink = self.order.sink
+        super().__init__(state, self.last_node,
+                         state.I_O_positions[self.orders[0].sink],
+                         "retrieval_second_leg", 0, self.orders, self.order,
+                         TravelEventKeys.RETRIEVAL_2ND_LEG, self.agv_id)
+        state.add_travel_event(self)
+        return EventHandleInfo(False, self, self, None, None)
+
 
 class DeliveryFirstLeg(Travel):
     """first leg of a travel event used to complete a delivery order. a free
      AGV is seized and moves from its current position to the source tile where
     it will pick up a pallet
     """
     def __init__(self, state: State, start_point: Tuple[int, int],
                  end_point: Tuple[int, int], travel_type: str,
-                 level: int, source: int, order: Order, agv_id: int):
+                 level: int, source: int, orders: [Order],
+                 order: Order, agv_id: int):
         super().__init__(state, start_point, end_point, travel_type,
-                         level, order, TravelEventKeys.DELIVERY_1ST_LEG, agv_id)
+                         level, orders, order, TravelEventKeys.DELIVERY_1ST_LEG,
+                         agv_id)
         self.source = source
 
-    def handle(self, state: State):
+    def handle(self, state: State, core=None):
         """vehicle position is updated. since delivery second leg needs an
         action from the agent or policy, it is not created here.
 
         returns:
         action_needed = True
         event_to_add = None
         travel_event_to_add = None
@@ -438,15 +593,28 @@
         queued_delivery_order_to_add = None
         """
         super().handle(state)
         state.remove_travel_event(self.order.order_number)
         state.agv_manager.update_v_matrix(
             self.first_node, self.last_node, False)
         state.remove_route(self.route.get_indices())
-        return EventHandleInfo(True, None, None, None, None)
+
+        current_order_index = self.orders.index(self.order)
+        if current_order_index != len(self.orders) - 1:
+            self.order = self.orders[current_order_index + 1]
+            super().__init__(state, self.last_node,
+                             state.I_O_positions[self.order.source],
+                             "delivery_first_leg", 0, self.orders, self.order,
+                             TravelEventKeys.DELIVERY_1ST_LEG, self.agv_id)
+            self.source = self.order.source
+            state.add_travel_event(self)
+            return EventHandleInfo(False, self, self, None, None)
+        else:
+            self.order = self.orders[0]
+            return EventHandleInfo(True, None, None, None, None)
 
     def __str__(self):
         return super().__str__()
 
     def __deepcopy__(self, memo):
         return faster_deepcopy(self, memo)
 
@@ -454,129 +622,251 @@
 class DeliverySecondLeg(Travel):
     """second leg of a travel event used to complete a retrieval order. a busy
      AGV moves from its current position (where it just picked up a pallet) to
      the sink tile where it will drop off the pallet
     """
     def __init__(self, state: State, start_point: Tuple[int, int],
                  end_point: Tuple[int, int], travel_type: str,
-                 level: int, source: int, order, agv_id: int):
+                 level: int, source: int, orders, order, agv_id: int,
+                 servicing_retrieval_order: Retrieval = None):
         super().__init__(state, start_point, end_point, travel_type,
-                         level, order, TravelEventKeys.DELIVERY_2ND_LEG, agv_id)
+                         level, orders, order, TravelEventKeys.DELIVERY_2ND_LEG,
+                         agv_id)
         self.source = source
-        self.delivery_action, self.retrieval_actions = (state.location_manager
-                                                        .lock_lane(end_point))
+        self.retrieval_order = servicing_retrieval_order
+        state.agv_manager.agv_index[agv_id].servicing_order_type = \
+            'delivery_second_leg'
+        if self.retrieval_order:
+            self.delivery_action = end_point
+        else:
+            self.delivery_action, self.retrieval_actions =\
+                (state.location_manager.lock_lane(end_point))
 
-    def handle(self, state: State):
+    def handle(self, state: State, core=None):
         """updates agv position in vehicle matrix, removes route, removes travel
         event. adds correct SKU number to storage matrix and the current time
         to the arrival time matrix
 
         returns:
         action_needed = False
         event_to_add = None
         travel_event_to_add = None
         queued_retrieval_order_to_add = None
         queued_delivery_order_to_add = None
         """
         super().handle(state)
+        self.orders.pop(0)
+        state.update_when_vehicle_free(self.last_node)
         state.remove_travel_event(self.order.order_number)
         state.agv_manager.update_v_matrix(self.first_node, self.last_node, True)
         state.remove_route(self.route.get_indices())
         pallet_position = self.last_node + (self.level,)
-        state.location_manager.unlock_lane(self.delivery_action,
-                                           self.retrieval_actions)
-        state.update_s_t_b_matrices(pallet_position, self.order.SKU, state.time,
-                                    self.order.batch_id)
-        storage_location = self.last_node + (self.level,)
-        state.location_manager.zone_manager.add_out_of_zone_sku(
-            pallet_position, self.order.SKU)
-        assert len(storage_location) == 3
+        if not self.retrieval_order:
+            state.location_manager.unlock_lane(self.delivery_action,
+                                               self.retrieval_actions)
+            state.update_s_t_b_matrices(pallet_position, self.order.SKU,
+                                        state.time, self.order.batch_id)
+            storage_location = self.last_node + (self.level,)
+            state.location_manager.zone_manager.add_out_of_zone_sku(
+                pallet_position, self.order.SKU)
+            assert len(storage_location) == 3
+            # no shift penalty can occur at this point, at least not for the
+            # "pure lane" simulation mode
+            _ = state.location_manager.update_on_delivery_second_leg(
+                pallet_position, self.order.SKU, self.time, self.order.batch_id)
+        else:
+            self.perform_direct_retrieval(state, core)
 
         state.remove_order(self.order.order_number)
-        # no shift penalty can occur at this point, at least not for the
-        # "pure lane" simulation mode
         state.n_skus_inout_now[self.order.SKU] += 1
-        state.agv_manager.release_agv(
-            pallet_position[:-1], self.time, self.agv_id)
-        _ = state.location_manager.update_on_delivery_second_leg(
-            pallet_position, self.order.SKU, self.time, self.order.batch_id)
-
         if self.verbose:
             print("finished delivery order #{0}".format(
                 self.order.order_number))
         self.order.set_completion_time(state.time)
         state.trackers.update_on_order_completion(self.order)
-        return EventHandleInfo(False, None, None, None, None)
+        if len(self.orders) > 0:
+            self.order = self.orders[0]
+            self.source = self.order.source
+            return EventHandleInfo(True, None, None, None, None)
+        else:
+            state.agv_manager.update_v_matrix(
+                self.first_node, self.last_node, True)
+            agv: AGV = state.agv_manager.agv_index.get(self.agv_id)
+            is_exit = False
+            for dcc_ret_order in agv.dcc_retrieval_order:
+                if self.retrieval_order and dcc_ret_order.SKU ==\
+                        self.retrieval_order.SKU:
+                    is_exit = True
+            if is_exit or len(agv.dcc_retrieval_order) == 0:
+                agv.dcc_retrieval_order = []
+                state.agv_manager.release_agv(
+                    pallet_position[:-1], self.time, self.agv_id)
+                return EventHandleInfo(False, None, None, None, None)
+            else:
+                actions = []
+                pending_ret_orders = []
+                possible_ret_orders = []
+                for dcc_order in agv.dcc_retrieval_order:
+                    action = self.find_closest_sku_loc(state, dcc_order.SKU)
+                    if action:
+                        possible_ret_orders.append(dcc_order)
+                        actions.append(action)
+                    else:
+                        pending_ret_orders.append(dcc_order)
+                if agv.forks > len(actions) > 0 or agv.forks == len(actions):
+                    order = possible_ret_orders[0]
+                    action = actions[0]
+                    travel_event = RetrievalFirstLeg(
+                        state=state, start_point=self.last_node,
+                        end_point=action[0:2],
+                        travel_type="retrieval_first_leg",
+                        level=int(action[2]),
+                        sink=order.sink,
+                        orders=possible_ret_orders,
+                        order=order,
+                        actions=actions, agv_id=agv.id,
+                        servicing_delivery_order=[])
+                    state.add_travel_event(travel_event)
+                    return EventHandleInfo(False, travel_event, travel_event,
+                                           pending_ret_orders, None)
+                else:
+                    event = agv.dcc_retrieval_order
+                    agv.dcc_retrieval_order = []
+                    state.agv_manager.release_agv(
+                        pallet_position[:-1], self.time, self.agv_id)
+                    return EventHandleInfo(False, None, None, event, None)
+
+    def find_closest_sku_loc(self, state: State, sku: int)\
+            -> Tuple[int, int, int]:
+        sc, tes = state.location_manager, state.trackers.travel_event_statistics
+        locations = sc.get_sku_locations(sku, tes)
+        closest_distance = np.infty
+        closest_tgt_loc = None
+        for loc in list(locations):
+            loc_tuple = unravel(loc, state.S.shape)
+            distance = state.routing.get_distance(self.last_node, loc_tuple[:2])
+            if distance < closest_distance:
+                closest_distance = distance
+                closest_tgt_loc = loc_tuple
+        return closest_tgt_loc
+
+    def get_next_sku(self):
+        return self.order.sku
 
     def __str__(self):
         return super().__str__()
 
     def __deepcopy__(self, memo):
         return faster_deepcopy(self, memo)
 
+    def perform_direct_retrieval(self, state: State, core):
+        tile_found = False
+        offset = 0
+        state.remove_route(self.route.get_indices())
+        while not tile_found:
+            vehicle_position = (self.last_node[0] + offset, self.last_node[1])
+            value_at_sink = state.V[vehicle_position]
+            if (value_at_sink == VehicleKeys.N_AGV or
+                    value_at_sink == VehicleKeys.BUSY):
+                state.agv_manager.update_v_matrix(
+                    self.first_node, self.last_node, False)
+                state.remove_route(self.route.get_indices())
+                state.remove_order(self.retrieval_order.order_number)
+                tile_found = True
+            else:
+                if self.verbose:
+                    print("already an AGV at this tile, "
+                          "checking next tile for free space")
+                offset += 1
+        if self.verbose:
+            print(f"finished retrieval order #{self.retrieval_order.order_number}")
+        self.retrieval_order.set_completion_time(state.time)
+        state.trackers.update_on_order_completion(self.retrieval_order)
+        core.logger.log_state()
+
 
 class EventManager:
     def __init__(self):
         self.running: MutableSequence[Event] = []
-        self.queued_delivery_orders: Deque[Delivery] = deque([])
+        self.queued_delivery_orders: Dict[int, Deque[Delivery]] = {}
         self.queued_retrieval_orders: Dict[int, Deque[Retrieval]] = {}
         self.current_travel: Set[Travel] = set({})
         self.__verbose = False
         self.__retrieval_possible = False
         self.__delivery_possible = False
         self.__state_changed_retrieval = True
         self.__state_changed_delivery = True
         self.__n_queued_retrieval_orders = 0
         self.__n_queued_delivery_orders = 0
         self.__earliest_delivery_order = None
         self.__earliest_retrieval_order = None
+        self.finished_ret_first_leg_skus = []
+        self.finished_ret_second_leg_skus = []
 
     @property
     def n_queued_retrieval_orders(self):
         return self.__n_queued_retrieval_orders
 
     @property
     def n_queued_delivery_orders(self):
         return self.__n_queued_delivery_orders
 
-    def add_future_event(self, event: Event):
+    @n_queued_retrieval_orders.setter
+    def n_queued_retrieval_orders(self, n_orders):
+        self.__n_queued_retrieval_orders = n_orders
+
+    @n_queued_delivery_orders.setter
+    def n_queued_delivery_orders(self, n_orders):
+        self.__n_queued_delivery_orders = n_orders
+
+    def add_future_event(self, event: Event, state):
         self.__state_changed_retrieval = True
         self.__state_changed_delivery = True
         heap.heappush(self.running, event)
 
     def add_current_events(
-            self, event_queueing_info: EventHandleInfo):
+            self, event_queueing_info: EventHandleInfo, state):
         """this function takes the events that were returned from handling an
         event and adds them to their appropriate data structures. For example,
         if a travel event was created when handling a delivery order, it will
         be added to self.events.current_travel.
         """
         if event_queueing_info.event_to_add:
-            self.add_future_event(event_queueing_info.event_to_add)
+            self.add_future_event(event_queueing_info.event_to_add, state)
         if event_queueing_info.travel_event_to_add:
             self.__state_changed_retrieval = True
             self.__state_changed_delivery = True
             initial_len = len(self.current_travel)
             self.current_travel.add(event_queueing_info.travel_event_to_add)
             assert initial_len + 1 == len(self.current_travel)
         if event_queueing_info.queued_retrieval_order_to_add:
             self.__print(f"added retrieval order to queue: "
                          f"{event_queueing_info.queued_retrieval_order_to_add}")
-            self.__queue_retrieval_order(
-                event_queueing_info.queued_retrieval_order_to_add)
+            if type(event_queueing_info.queued_retrieval_order_to_add) == list:
+                for queue_ret_order_to_add in\
+                        event_queueing_info.queued_retrieval_order_to_add:
+                    self.__queue_retrieval_order(queue_ret_order_to_add)
+            else:
+                self.__queue_retrieval_order(
+                    event_queueing_info.queued_retrieval_order_to_add)
         if event_queueing_info.queued_delivery_order_to_add:
             self.__print(f"added delivery order to queue: "
                          f"{event_queueing_info.queued_delivery_order_to_add}")
             self.__queue_delivery_order(
                 event_queueing_info.queued_delivery_order_to_add)
 
     def __queue_delivery_order(self, order: Delivery):
         self.__state_changed_delivery = True
         self.__n_queued_delivery_orders += 1
-        self.queued_delivery_orders.append(order)
+        sku = order.SKU
+        if sku in self.queued_delivery_orders:
+            self.queued_delivery_orders[sku].append(order)
+        else:
+            self.queued_delivery_orders[sku] = deque([order])
+        # self.queued_delivery_orders.append(order)
 
     def __queue_retrieval_order(self, order: Retrieval):
         self.__n_queued_retrieval_orders += 1
         self.__state_changed_retrieval = True
         sku = order.SKU
         if sku in self.queued_retrieval_orders:
             self.queued_retrieval_orders[sku].append(order)
@@ -584,14 +874,21 @@
             self.queued_retrieval_orders[sku] = deque([order])
 
     def pop_future_event(self):
         self.__state_changed_retrieval = True
         self.__state_changed_delivery = True
         return heap.heappop(self.running)
 
+    def pop_retrieval_event(self, event: RetrievalFirstLeg):
+        heap.heapify(self.running)
+        return heap.heappop(self.running, event)
+
+    def re_heapify_heap(self):
+        heap.heapify(self.running)
+
     def pop_queued_event(self, state: State) -> Event:
         """this method is only executed if there are queued orders that can be
         handled and there are free AGVs. It is a bit hairy because of many
         specific if statements but these are the three conditions below. Note
         that retrieval orders have higher priority than delivery orders.
         1) if there is at least one serviceable retrieval order, handle
         whichever order one is oldest (i.e. queued first)
@@ -622,27 +919,47 @@
                 next_event = self.pop_queued_delivery_order()
         # the queued order's time has already passed so it must be
         # updated to current time
         # TODO: Fix service times?
         # if next_event:
         #     next_event.time = state.time
         self.__state_changed_retrieval = True
+        self.__state_changed_delivery = True
         return next_event
 
-    def add_travel_event(self, event: Travel):
+    def add_travel_event(self, event: Travel, state):
         """
         Adds the travel event to both the future events queue and the running
         travel events queue.
 
         :param event: The new travel event wich is to finish at some time in the
             future.
         :return: None.
         """
         self.current_travel.add(event)
-        self.add_future_event(event)
+        self.add_future_event(event, state)
+
+    def find_travel_event(
+            self, agv_id: int, event_type: Type[Travel]
+    ) -> Union[DeliveryFirstLeg, DeliverySecondLeg,
+               RetrievalFirstLeg, RetrievalSecondLeg, Travel]:
+        """
+        Finds an already running travel event given the agv_id and the type of
+        the desired event.
+
+        When multiple forks are involved, already running RetrievalFirstLeg
+        events sometimes need to be updated to service additional orders.
+
+        :param agv_id: The target agv.
+        :param event_type: The type of travel event.
+        :return: The desired Travel event.
+        """
+        for event in self.current_travel:
+            if isinstance(event, event_type) and event.agv_id == agv_id:
+                return event
 
     def remove_travel_event(self, next_event: Travel):
         self.__state_changed_retrieval = True
         self.__state_changed_delivery = True
         initial_len = len(self.current_travel)
         self.current_travel.remove(next_event)
         assert initial_len - 1 == len(self.current_travel)
@@ -663,48 +980,56 @@
             if oldest_order_possible:
                 self.__earliest_retrieval_order = oldest_order_possible
                 query_result = True
         self.__state_changed_retrieval = False
         self.__retrieval_possible = query_result
         return query_result
 
+    def get_retrieval_possible(self):
+        return self.__retrieval_possible
+
     def available_delivery(self, state: State):
         """
 
         :param state:
         :return:
         """
         if not self.__state_changed_delivery:
             return self.__delivery_possible
-        if not self.queued_delivery_orders:
+        if len(self.queued_delivery_orders) == 0:
             query_result = False
         else:
             query_result = state.delivery_possible()
-            self.__earliest_delivery_order = self.queued_delivery_orders[0]
+            sku = next(iter(self.queued_delivery_orders))
+            self.__earliest_delivery_order = self.queued_delivery_orders[sku][0]
         self.__delivery_possible = query_result
         self.__state_changed_delivery = False
         return query_result
 
     def all_orders_complete(self):
         if (not self.running
                 and self.__n_queued_retrieval_orders == 0
                 and self.__n_queued_delivery_orders == 0):
             return True
         else:
             return False
 
     def pop_queued_delivery_order(self) -> Delivery:
         """
-        Returns the oldest serviceable queued retrieval order.
+        Returns the oldest serviceable queued delivery order.
 
         :return: The oldest order.
         """
         self.__state_changed_retrieval = True
         self.__n_queued_delivery_orders -= 1
-        return self.queued_delivery_orders.popleft()
+        oldest_sku = next(iter(self.queued_delivery_orders))
+        order = self.queued_delivery_orders[oldest_sku].popleft()
+        if len(self.queued_delivery_orders[oldest_sku]) == 0:
+            del self.queued_delivery_orders[oldest_sku]
+        return order
 
     def pop_queued_retrieval_order(self) -> Retrieval:
         """
         Return the oldest serviceable retrieval order and removes it from the
         queue. Since the queued retrieval orders are stored in a sku indexed
         dictionary of deques, and orders are queued by appending to the right,
         we only need to look at all the deque heads to find the oldest queued
@@ -717,14 +1042,19 @@
         self.__n_queued_retrieval_orders -= 1
         target_sku = self.__earliest_retrieval_order.SKU
         order = self.queued_retrieval_orders[target_sku].popleft()
         if not self.queued_retrieval_orders[target_sku]:
             del self.queued_retrieval_orders[target_sku]
         return order
 
+    def get_earliest_retrieval_order(self) -> Retrieval:
+        target_sku = self.__earliest_retrieval_order.SKU
+        order = self.queued_retrieval_orders[target_sku][0]
+        return order
+
     def get_min_retrival_order_time(self):
         """
         Computes the minimum retrieval order time.
 
         :return: The time of the oldest retrieval order.
         """
         min_time = np.inf
```

### Comparing `slapstack-0.0.24/slapstack/core_logger.py` & `slapstack-0.1.1/slapstack/core_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,17 @@
                 rmtree(self.log_dir)
             create_folders(f'{self.log_dir}/dummy')
             # write logger object
             self.on = True
         else:
             self.on = False
 
-    def log_state(self, state: State):
+    def log_state(self):
         if self.on:
-            self.__write_heatmaps(state)
+            self.__write_heatmaps(self.slap_state)
 
     def __write_heatmaps(self, state: State):
         """
         Creates a json file with the information from the state matrices. The
         file can be used to create heatmap visualizations for the individual
         matrices. The json structure is as follows:
         {matrix_name_1: {
```

### Comparing `slapstack-0.0.24/slapstack/core_state.py` & `slapstack-0.1.1/slapstack/core_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import numpy as np
 
 from slapstack.core_state_route_manager import RouteManager
 from slapstack.core_state_agv_manager import AgvManager
 from slapstack.core_state_lane_manager import LaneManager
 from slapstack.core_state_location_manager import LocationManager
-from slapstack.extensions.c_helpers import c_unravel
 
-from typing import List, Union, TYPE_CHECKING
+from typing import List, Union, TYPE_CHECKING, Tuple
 import sys
 
 from collections import defaultdict
 from slapstack.helpers import faster_deepcopy, StorageKeys, TravelEventKeys
 from slapstack.interface_templates import SimulationParameters
 
 if TYPE_CHECKING:
-    from slapstack.core_events import (EventManager, DeliveryFirstLeg,
-                                       RetrievalSecondLeg, Order)
+    from slapstack.core_events import EventManager, Order, DeliveryFirstLeg
+    from slapstack.core_events import RetrievalSecondLeg, RetrievalFirstLeg
 
 
 class TravelEventTrackers:
     def __init__(self):
         self.n_finished_retrieval_1st_leg = 0
         self.n_finished_retrieval_2nd_leg = 0
         self.n_finished_delivery_1st_leg = 0
@@ -28,22 +27,26 @@
         self.n_running_retrieval_2nd_leg = 0
         self.n_running_delivery_1st_leg = 0
         self.n_running_delivery_2nd_leg = 0
         self.d_delivery_1st_leg = 0
         self.d_delivery_2nd_leg = 0
         self.d_retrieval_1st_leg = 0
         self.d_retrieval_2nd_leg = 0
+        self.total_shift_distance = 0
         self.t_delivery_1st_leg = 0
         self.t_delivery_2nd_leg = 0
         self.t_retrieval_1st_leg = 0
         self.t_retrieval_2nd_leg = 0
         self.total_finished_travel = 0
         self.total_travel_time = 0
         self.total_distance_traveled = 0
         self.last_travel_distance = 0
+        self.avg_dy = 0
+        self.avg_dx = 0
+        self.avg_count = 0
 
     @staticmethod
     def __get_suffix(event_key: TravelEventKeys):
         if event_key == TravelEventKeys.RETRIEVAL_1STLEG:
             attr_suffix = 'retrieval_1st_leg'
         elif event_key == TravelEventKeys.RETRIEVAL_2ND_LEG:
             attr_suffix = 'retrieval_2nd_leg'
@@ -52,38 +55,43 @@
         elif event_key == TravelEventKeys.DELIVERY_2ND_LEG:
             attr_suffix = 'delivery_2nd_leg'
         else:
             raise ValueError('Unknown TravelEventKey')
         return attr_suffix
 
     def __update_trackers(
-            self, distance: float, duration: float, attr_suffix: str):
+            self, distance: float, duration: float, shift_distance: float,
+            attr_suffix: str, mark_complete):
         self.total_distance_traveled += distance
         self.total_travel_time += duration
-        if not distance:  # event was just initialized
+        if not mark_complete:  # event was just initialized
             assert duration == 0.
             setattr(self, f'n_running_{attr_suffix}',
                     getattr(self, f'n_running_{attr_suffix}') + 1)
         else:  # eent has ended
             self.total_finished_travel += 1
             self.last_travel_distance = distance
+            self.total_shift_distance += shift_distance
             setattr(self, f'n_running_{attr_suffix}',
                     getattr(self, f'n_running_{attr_suffix}') - 1)
             setattr(self, f'd_{attr_suffix}',
                     getattr(self, f'd_{attr_suffix}') + distance)
             setattr(self, f't_{attr_suffix}',
                     getattr(self, f't_{attr_suffix}') + duration)
             setattr(self, f'n_finished_{attr_suffix}',
                     getattr(self, f'n_finished_{attr_suffix}') + 1)
 
     def update_travel_events(self, event: TravelEventKeys,
-                             duration: float = 0, distance: float = 0):
+                             duration: float = 0, distance: float = 0,
+                             shift_distance: float = 0,
+                             is_completion: bool = False):
         attr_suffix = self.__get_suffix(event)
         self.__update_trackers(
-            distance=distance, duration=duration, attr_suffix=attr_suffix)
+            distance=distance, duration=duration, attr_suffix=attr_suffix,
+            shift_distance=shift_distance, mark_complete=is_completion)
 
     def get_unbound_travel_events(self):
         return self.n_running_delivery_1st_leg
 
     def average_travel_time(self, travel_type: TravelEventKeys = None):
         if travel_type is None:
             if self.total_finished_travel > 0:
@@ -141,15 +149,15 @@
         # other
         self.n_storage_locations = 0
         self.n_pallets_in_storage = 0
         self.number_of_pallet_shifts = 0
         # flag
         self.compute_feature_trackers: bool = compute_feature_trackers
 
-    def update_on_order_completion(self, order: 'Order'):
+    def update_on_order_completion(self, order: 'Order', distance_penalty=0.0):
         self.finished_orders.append(order)
         service_time = order.completion_time - order.time
         self.total_service_time += service_time
         self.average_service_time = (self.total_service_time /
                                      len(self.finished_orders))
         if order.type == 'retrieval':
             self.n_pallets_in_storage -= 1
@@ -159,17 +167,19 @@
     def add_pallet(self):
         self.n_pallets_in_storage += 1
 
     def update_on_travel_event_creation(self, travel_type: TravelEventKeys):
         self.travel_event_statistics.update_travel_events(travel_type)
 
     def update_on_travel_event_completion(
-            self, travel_type: TravelEventKeys, duration, distance):
+            self, travel_type: TravelEventKeys, duration, distance,
+            shift_distance):
         self.travel_event_statistics.update_travel_events(
-            travel_type, duration=duration, distance=distance)
+            travel_type, duration=duration, distance=distance,
+            shift_distance=shift_distance, is_completion=True)
 
     def get_fill_level(self):
         return self.n_pallets_in_storage / self.n_storage_locations
 
     @property
     def n_queued_retrieval_orders(self):
         return sum([
@@ -245,39 +255,44 @@
         self.T = State.__init_arrival_time_matrix(params)
         self.B = State.__init_batch_id_matrix(params)
         # state managers
         self.agv_manager = AgvManager(params, self.S, rng)
         self.V = self.agv_manager.V  # Location of Vehicles
         lane_manager = LaneManager(self.S, params)
         self.routing = RouteManager(
-            lane_manager, self.S, params.agv_speed, params.unit_distance)
+            lane_manager, self.S, params.agv_speed, params.unit_distance,
+            params.use_case_name)
         self.location_manager = LocationManager(
-            self.S, self.V, self.T, self.B, params, lane_manager)
+            self.S, self.T, self.B, lane_manager, events)
         # KPIs and trackers
         self.trackers = Trackers(events, params.compute_feature_trackers)
         # simple progression trackers
         self.time = 0
         self.n_steps = 0
         self.n_silent_steps = 0
         self.n_skus_inout_now = defaultdict(int)
         # paths relevant variables
-        self.source_positions = State.get_source_locations(self.S)
-        self.sink_positions = State.get_sink_locations(self.S)
-        self.routing.precompute_paths(
-            self.source_positions + self.sink_positions)
+        self.I_O_positions = State.get_io_locations(self.S)
         self.routes = set()
         # past event links
         self.current_order: Union[str, None] = None
         self.current_source_sink = 0
         self.current_sku = None
         self.order_arrival_time = None
         # debugging information
         self.incomplete_orders = {}
         self.travel_events = {}
         self.done = False
+        self.current_destination = None
+        self.door_to_door = params.door_to_door
+
+    def get_mid_aisles(self):
+        mid_aisles = [tuple(i[0:2]) for i in np.argwhere(self.S[:, :, 0] ==
+                                                         StorageKeys.MID_AISLE)]
+        return mid_aisles
 
     @staticmethod
     def __init_storage_matrix(p: SimulationParameters) -> np.ndarray:
         """
         Creates the initially empty storage matrix either by following a
         simple pattern or by reading the layout parameter.
 
@@ -386,36 +401,43 @@
         tes = self.trackers.travel_event_statistics
         return tes.average_travel_time() / 3600
 
     def get_average_service_time(self):
         return self.trackers.average_service_time / 60
 
     def add_travel_event(
-            self, travel_event: Union['DeliveryFirstLeg',
+            self, travel_event: Union['DeliveryFirstLeg', 'RetrievalFirstLeg',
                                       'RetrievalSecondLeg', None]):
         """adds a Travel event to self.travel_events"""
         if travel_event:
             t = travel_event
             order_type, leg, _ = t.travel_type.split('_')
             parameters = {"SKU": int(t.order.SKU),
                           "type": order_type,
                           "leg": leg,
                           "time": t.time,
                           "path": [list(([int(i) for i in node]))
                                    for node in t.route.get_indices()]}
 
             self.travel_events[t.order.order_number] = parameters
 
-    def delivery_possible(self):
+    def delivery_possible(self, agv_pos: Tuple[int, int] = None,
+                          index: int = None) -> bool:
         sc, tes = self.location_manager, self.trackers.travel_event_statistics
         n_open_lanes = (sc.lane_manager.n_lanes
                         - len(sc.lane_manager.locked_lanes)
                         - len(sc.lane_manager.full_lanes))
         n_unbound_delivery = tes.get_unbound_travel_events()
-        return n_open_lanes > n_unbound_delivery
+        if agv_pos is not None and index is not None:
+            n_forks = self.agv_manager.free_agv_positions[agv_pos][index].forks
+            return n_open_lanes - (n_forks - 1) >\
+                n_unbound_delivery
+        else:
+            return n_open_lanes - (self.agv_manager.maximum_forks - 1) >\
+                n_unbound_delivery
 
     def retrieval_possible(self, sku: int):
         """returns true if the given SKU is serviceable"""
         sc, tes = self.location_manager, self.trackers.travel_event_statistics
         locations = sc.get_sku_locations(sku, tes)
         if locations:
             return True
@@ -474,14 +496,27 @@
 
     @staticmethod
     def get_sink_locations(storage_matrix: np.ndarray):
         """called once. gets location of tiles marked as sink"""
         return [tuple(i[0:2]) for i in
                 np.argwhere(storage_matrix[:, :, 0] == StorageKeys.SINK)]
 
+    @staticmethod
+    def get_io_locations(storage_matrix: np.ndarray):
+        """called once. gets location of tiles marked as source and sink"""
+        source_positions = [tuple(i[0:2]) for i in
+                            np.argwhere(storage_matrix[:, :, 0] ==
+                                        StorageKeys.SOURCE)]
+
+        sink_positions = [tuple(i[0:2]) for i in
+                          np.argwhere(storage_matrix[:, :, 0] ==
+                                      StorageKeys.SINK)]
+
+        return source_positions + sink_positions
+
     def concatenate(self):
         """"reshapes multi-level/3D storage and time matrices, then concatenates
         them along with the vehicle matrix
         """
         n_rows = self.S.shape[0]
         s = np.copy(self.S).transpose((1, 0, 2)).reshape(n_rows, -1)
         t = np.copy(self.T).transpose((1, 0, 2)).reshape(n_rows, -1)
@@ -667,13 +702,32 @@
     def set_current_order_arrival_time(self, time):
         self.order_arrival_time = time
 
     def update_on_travel_event_creation(self, travel_type: TravelEventKeys):
         self.trackers.update_on_travel_event_creation(travel_type)
 
     def update_on_travel_event_completion(
-            self, travel_type: TravelEventKeys, duration, distance: float):
+            self, travel_type: TravelEventKeys, duration, distance: float,
+            penalty: float):
         self.trackers.update_on_travel_event_completion(
-            travel_type, duration, distance)
+            travel_type, duration, distance, penalty)
+
+    def update_when_vehicle_free(self, end_position: Tuple[int, int]):
+        """
+        Updates the vehicle position running averages.
+
+        :param end_position: The position of the freed vehicle.
+        :return: None.
+        """
+        tes = self.trackers.travel_event_statistics
+        avg = tes.avg_dx
+        n = tes.avg_count + 1
+        tes.avg_dx = (avg * (n - 1)) / n + end_position[0] / n
+        avg = tes.avg_dy
+        tes.avg_dy = (avg * (n - 1)) / n + end_position[1] / n
+        tes.avg_count += 1
+
+    def set_current_destination(self, destination):
+            self.current_destination = destination
 
     def __deepcopy__(self, memo):
         return faster_deepcopy(self, memo)
```

### Comparing `slapstack-0.0.24/slapstack/core_state_agv_manager.py` & `slapstack-0.1.1/slapstack/core_state_agv_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 import numpy as np
 
 from slapstack.helpers import VehicleKeys, StorageKeys
 from slapstack.interface_templates import SimulationParameters
 
 
 class AGV:
-    def __init__(self, transport_id: int, pos: Tuple[int, int]):
+    def __init__(self, transport_id: int, pos: Tuple[int, int], forks=1):
         """
         AGV object constructor. Instances of this class represent the warehouse
         transports.
 
         :param transport_id: The unique transport id.
         :param pos: The current AGV position.
         """
         self.id = transport_id
         self.position = pos
         self.free = True
         self.booking_time = -1
         self.utilization = 0
+        self.forks = forks
+        self.servicing_order_type = None
+        self.available_forks = self.forks
+        self.dcc_retrieval_order = []
 
     def log_booking(self, booking_time: float):
         """
         Marks the AGV as busy and notes down the time at which the booking
         occurred.
 
         :param booking_time: The time at which the AGV was selected for a job.
@@ -65,14 +69,15 @@
         :param storage_matrix: The vehicle matrix from which to extract the
             initial AGV positions.
         """
         self.free_agv_positions: Dict[Tuple[int, int], List[AGV]] = {}
         self.agv_index: Dict[int, AGV] = {}
         self.V = np.full((p.n_rows, p.n_columns),
                          VehicleKeys.N_AGV.value, dtype='int8')
+        self.maximum_forks = p.n_forks
         self.__initialize_agvs(storage_matrix, rng, p.n_agvs)
         self.n_free_agvs = len(self.free_agv_positions)
         self.n_busy_agvs = 0
         self.n_agvs = p.n_agvs
         self.n_visible_agvs = p.n_agvs
 
     def __initialize_agvs(self, S: np.ndarray, rng, n_agvs):
@@ -84,17 +89,18 @@
         """
         # agv_counter = 2  # initial position (column) of AGVs
         storage_locations = np.argwhere(S[:, :, 0] == StorageKeys.MID_AISLE)
         transport_id = 0
         for i in range(0, n_agvs):
             index = rng.integers(0, len(storage_locations))
             pos_t = tuple(storage_locations[index])
+            no_forks = self.maximum_forks
             if pos_t in self.free_agv_positions:
                 continue
-            new_agv = AGV(transport_id, pos_t)
+            new_agv = AGV(transport_id, pos_t, no_forks)
             self.free_agv_positions[pos_t] = [new_agv]
             self.agv_index[transport_id] = new_agv
             transport_id += 1
             self.V[pos_t] = VehicleKeys.FREE.value
 
     def update_v_matrix(self, first_position: Tuple[int, int],
                         second_position: Union[Tuple[int, int], None],
@@ -131,24 +137,37 @@
                 self.V[src_x, src_y] = VehicleKeys.N_AGV.value
                 self.V[tgt_x, tgt_y] = VehicleKeys.BUSY.value
 
     def update_on_retrieval_second_leg(
             self, position: Tuple[int, int], system_time: float, agv_id: int):
         self.release_agv(position, system_time, agv_id)
 
-    def agv_available(self) -> bool:
+    def agv_available(self, order_type='retrieval', only_new=False) -> bool:
         """
         Checks if there are any available AGVs to use for transport.
 
         :return: True if the free_agv_positions dictionary is not empty and
             false otherwise.
         """
-        return bool(self.free_agv_positions)
+        is_free_agv = False
+        for agv_pos in self.free_agv_positions:
+            for current_agv in self.free_agv_positions[agv_pos]:
+                if only_new:
+                    if current_agv.servicing_order_type is None:
+                        is_free_agv = True
+                elif current_agv.servicing_order_type == order_type\
+                        or current_agv.servicing_order_type is None:
+                    is_free_agv = True
+                    break
+            if is_free_agv:
+                break
+        return is_free_agv
 
-    def book_agv(self, position: Tuple[int, int], system_time: float):
+    def book_agv(self, agv_pos: Tuple[int, int], system_time: float,
+                 agv_id: int, order_type: str):
         """
         Called whenever a fist leg transport event starts. Depending on the
         event trigger position (source for delivery first leg or chosen pallet
         in the case of retrieval first leg) the closest agv from the
         free_agv_positions is selected for booking. The euclidean distance is
         used for distance comparison.
 
@@ -156,23 +175,28 @@
         free_agv_positions and its booking time is marked by calling the
         log_booking method. Finally, if the chosen AGV was the last located at
         the given position, the position is removed from the index entirely.
 
         :param position: The position of the triggering event (either source or
             chosen sku).
         :param system_time: The current simulation time.
+        #TODO reword docstring comments to reflect the external agv selection
         :return: The AGV booked AGV.
         """
-        selected_agv_pos = self.__get_close_agv(position)
-        agv = self.free_agv_positions[selected_agv_pos].pop()
-        agv.log_booking(system_time)
-        self.n_busy_agvs += 1
-        self.n_free_agvs -= 1
-        if not self.free_agv_positions[selected_agv_pos]:
-            del self.free_agv_positions[selected_agv_pos]
+        agv = self.free_agv_positions[agv_pos][agv_id]
+        if agv.available_forks == agv.forks:
+            agv.log_booking(system_time)
+            agv.servicing_order_type = order_type
+        agv.available_forks -= 1
+        if agv.available_forks == 0:
+            self.n_busy_agvs += 1
+            self.n_free_agvs -= 1
+            self.free_agv_positions[agv_pos].pop(agv_id)
+        if not self.free_agv_positions[agv_pos]:
+            del self.free_agv_positions[agv_pos]
         return agv
 
     def release_agv(self, position, system_time: float, agv_id: int):
         """
         Called on occurrence of second leg transport events to release the
         associated AGV.
 
@@ -188,39 +212,69 @@
         :param agv_id: The id of the release AGV; note that the AGV ids are set
             on first leg Transport event creation and then passed to the
             corresponding second leg transport.
         :return: None.
         """
         released_agv = self.agv_index[agv_id]
         released_agv.log_release(system_time, position)
-        if position in self.free_agv_positions:
+        if position in self.free_agv_positions\
+                and released_agv.available_forks == 0:
             self.free_agv_positions[position].append(released_agv)
-        else:
+            self.n_busy_agvs -= 1
+            self.n_free_agvs += 1
+        elif released_agv.available_forks == 0:
             self.free_agv_positions[position] = [released_agv]
-        self.n_busy_agvs -= 1
-        self.n_free_agvs += 1
+            self.n_busy_agvs -= 1
+            self.n_free_agvs += 1
+        elif released_agv.available_forks > 0:
+            free_agvs_cp = self.free_agv_positions.copy()
+            for agv in free_agvs_cp:
+                index = 0
+                for current_agv in free_agvs_cp[agv]:
+                    if agv_id == current_agv.id:
+                        self.free_agv_positions[agv].pop(index)
+                        if len(self.free_agv_positions[agv]) == 0:
+                            del self.free_agv_positions[agv]
+                        if position in self.free_agv_positions:
+                            self.free_agv_positions[position].append(
+                                released_agv)
+                        else:
+                            self.free_agv_positions[position] = [released_agv]
+                        break
+                    index += 1
+        released_agv.available_forks = released_agv.forks
+        released_agv.servicing_order_type = None
 
-    def __get_close_agv(self, position: Tuple[int, int]) -> Tuple[int, int]:
+    def get_close_agv(self, position: Tuple[int, int], order_type: str)\
+            -> Tuple[int, int]:
         """
         Iterates over the free AGVs in the free_agv_positions and selects the
         one closest to the passed position with respect to euclidean distance.
 
         :param position: The position relative to which the closest AGV is to
             be selected.
         :return: The closest AGV position.
         """
         selected_agv = None
         min_distance = inf
+        agv_index = 0
         for agv in self.free_agv_positions:
-            distance = hypot(position[0]-agv[0], position[1]-agv[1])
-            if distance < min_distance:
-                selected_agv = agv
-                min_distance = distance
+            # current_agv = self.free_agv_positions[agv][-1]
+            index = 0
+            for current_agv in self.free_agv_positions[agv]:
+                if current_agv.servicing_order_type == order_type or\
+                        current_agv.servicing_order_type is None:
+                    distance = hypot(position[0] - agv[0], position[1] - agv[1])
+                    if distance < min_distance:
+                        agv_index = index
+                        selected_agv = agv
+                        min_distance = distance
+                index += 1
         # assert selected_agv in self.free_agv_positions
-        return selected_agv
+        return selected_agv, agv_index
 
     def get_agv_locations(self) -> Dict[Tuple[int, int], List[AGV]]:
         """
         Returns the free_agv_positions index.
 
         :return: The dictionary mapping free agv positions to lists of AGV
             objects.
```

### Comparing `slapstack-0.0.24/slapstack/core_state_lane_manager.py` & `slapstack-0.1.1/slapstack/core_state_lane_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Tuple, Dict, List, Union, Set, Iterable
+from collections import deque
+from typing import Tuple, Dict, List, Union, Set, Iterable, Deque
 
 import numpy as np
 
-from slapstack.extensions import c_ravel
-from slapstack.helpers import AccessDirection, StorageKeys
+from slapstack.helpers import AccessDirection, StorageKeys, ravel
 from slapstack.interface_templates import SimulationParameters
 
 
 class TileAccessPoint:
     def __init__(self,
                  position: Tuple[int, int],
                  distance: int,
@@ -52,14 +52,15 @@
             (i[0], i[1]) for i in
             np.argwhere(storage_matrix == StorageKeys.EMPTY)
         }
         for tile in tiles:
             # get the aisle tiles in the column
             ap_x, ap_dist = TileAccessPointIndex.__get_access_point(
                 storage_matrix, tile)
+            assert storage_matrix[ap_x, tile[1]] == -5
             assert ap_x
             if tile[0] < ap_x:
                 direction = AccessDirection.ABOVE
             else:
                 direction = AccessDirection.BELOW
             self.idx[tile] = TileAccessPoint(
                 position=(ap_x, tile[1]),
@@ -125,23 +126,65 @@
 
         :param tile_location: The tile position to check membership for.
         :return: True if the tile is in the index and false otherwise.
         """
         return tile_location in self.idx
 
 
+class Lane:
+    def __init__(self, tiles: List[Tuple[int, int]]):
+        self.tiles = tiles
+        self.sku_pos: Dict[int, Deque[Tuple[int, int, int]]] = dict()
+
+    def update_sku_border(self, sku, pos, added=True):
+        # TODO: assertion to ensure that added tile is always below/above prev
+        #  border
+        if added:
+            if sku in self.sku_pos:
+                self.sku_pos[sku].append(pos)
+            else:
+                self.sku_pos[sku] = deque([pos])
+        else:
+            # when pallet shifting, the hole is plugged with the forward pallet
+            # before removing the forward pallet; as such, the pallet to be
+            # removed should be found at the position -2 in the stack
+            stack_top_buff = deque([self.sku_pos[sku].pop()])
+            while stack_top_buff[-1] != pos:
+                stack_top_buff.append(self.sku_pos[sku].pop())
+            pos_popped = stack_top_buff.pop()
+            while stack_top_buff:
+                self.sku_pos[sku].append(stack_top_buff.pop())
+            # pos_popped = self.sku_pos[sku].pop()
+            try:
+                assert pos_popped == pos
+            except AssertionError:
+                print(pos_popped, pos)
+
+    def get_border_tile(self, sku):
+        return self.sku_pos[sku][-1]
+
+    def __getitem__(self, key):
+        return self.tiles[key]
+
+    def __bool__(self):
+        return True if len(self.tiles) else False
+
+    def __len__(self):
+        return len(self.tiles)
+
+
 class LaneManager:
     def __init__(
             self, storage_matrix: np.ndarray, params: SimulationParameters):
         self.tile_access_points = TileAccessPointIndex(storage_matrix)
         self.lane_clusters, self.n_lanes = self.create_lane_clusters()
         self.locked_lanes = set()
         self.full_lanes = set()
         self.pure_lanes = params.pure_lanes
-        self.sku_lanes = dict()
+        self.sku_lanes: Dict[int, List[Tuple[int, int, int]]] = dict()
         self.lane_assigned = self.create_lane_assigned_dict()
         self.occupied_lanes = dict({})  # maps sku to lanes
         self.S = storage_matrix
 
     def lock_lane(self, location: Tuple[int, int]):
         """
         Identifies the lane corresponding to the passed tile, adds it to the
@@ -262,34 +305,38 @@
                 else:
                     lane_below.append(tile)
                 access_point = self.tile_access_points[tile]
             lane_above.sort(key=lambda x: x[0])  # sort lane by aisle distance
             lane_above.reverse()
             lane_below.sort(key=lambda x: x[0])
             lane_clusters_dict_with_keys[access_point.position] = {
-                AccessDirection.BELOW: lane_above,
-                AccessDirection.ABOVE: lane_below
+                AccessDirection.BELOW: Lane(lane_above),
+                AccessDirection.ABOVE: Lane(lane_below)
             }
             n_lanes += 1 if lane_above else 0
             n_lanes += 1 if lane_below else 0
             # {'below': lane_above, 'above': lane_below, 'locked': set()}
         return lane_clusters_dict_with_keys, n_lanes
 
-    def get_lane(self, storage_position: Tuple[int, int, int]):
+    def get_lane(self, storage_position):
+        xy_position = storage_position[0:2]
+        aisle, direction = self.locate_access_point(xy_position)
+        lane: Lane = self.lane_clusters[aisle][direction]
+        return lane
+
+    def get_lane_locations(self, storage_position: Tuple[int, int, int]):
         """
         Returns all the positions in the lane that storage_position belongs to.
 
         :param storage_position: The storage position for which to retrieve
             all lane positions.
         :return:
         """
-        xy_position = storage_position[0:2]
-        aisle, direction = self.locate_access_point(xy_position)
-        lane = self.lane_clusters[aisle][direction.value]
-        return lane
+        lane = self.get_lane(storage_position)
+        return lane.tiles
 
     def get_access_point_direction(self, storage_position):
         xy_pos = storage_position[0:2]
         direction = self.tile_access_points[xy_pos].direction
         return direction.value
 
     def locate_access_point(
@@ -342,15 +389,15 @@
             direction = (AccessDirection.ABOVE
                          if lane[2] == -1 else AccessDirection.BELOW)
             lane_cluster = self.lane_clusters[lane[0:2]][direction]
             for storage_tile in lane_cluster:
                 for i in range(self.S.shape[2]):
                     if asint:
                         locations_in_lanes.add(
-                            c_ravel(storage_tile + (i,), self.S.shape))
+                            ravel(storage_tile + (i,), self.S.shape))
                     else:
                         locations_in_lanes.add(storage_tile + (i,))
             # if 'above' in lane_cluster:
             #     for storage_tile in lane_cluster['above']:
             #         for i in range(self.n_levels):
             #             locations_in_lanes.append(storage_tile + (i,))
             # if 'below' in lane_cluster:
@@ -359,15 +406,15 @@
             #             locations_in_lanes.append(storage_tile + (i,))
         return locations_in_lanes
 
     def remove_from_occupied_lane(
             self, storage_position: Tuple[int, int, int], sku: int):
         ap_pos, ap_dir = self.locate_access_point(storage_position[:2])
         self.occupied_lanes[sku][ap_pos][ap_dir].remove(
-            c_ravel(storage_position, self.S.shape))
+            ravel(storage_position, self.S.shape))
         if len(self.occupied_lanes[sku][ap_pos][ap_dir]) == 0:
             del self.occupied_lanes[sku][ap_pos][ap_dir]
         if len(self.occupied_lanes[sku][ap_pos]) == 0:
             del self.occupied_lanes[sku][ap_pos]
         if len(self.occupied_lanes[sku]) == 0:
             del self.occupied_lanes[sku]
 
@@ -376,8 +423,8 @@
         if sku not in self.occupied_lanes:
             self.occupied_lanes[sku] = {}
         if aisle not in self.occupied_lanes[sku]:
             self.occupied_lanes[sku][aisle] = {}
         if direction not in self.occupied_lanes[sku][aisle]:
             self.occupied_lanes[sku][aisle][direction] = set()
         self.occupied_lanes[sku][aisle][direction].add(
-            c_ravel(storage_location, self.S.shape))
+            ravel(storage_location, self.S.shape))
```

### Comparing `slapstack-0.0.24/slapstack/core_state_location_manager.py` & `slapstack-0.1.1/slapstack/core_state_location_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,58 @@
 from collections import defaultdict
 from typing import Dict, Tuple, Set, Optional, List, cast, Union, TYPE_CHECKING
 
 import numpy as np
 
-from slapstack.core_state_route_manager import Grid
-from slapstack.core_state_lane_manager import LaneManager
+from slapstack.core_state_lane_manager import LaneManager, Lane
 from slapstack.core_state_zone_manager import ZoneManager
-from slapstack.extensions import c_unravel, c_ravel, get_first_tile
 from slapstack.helpers import (StorageKeys, AccessDirection, TimeKeys,
-                               BatchKeys, faster_deepcopy)
-from slapstack.interface_templates import SimulationParameters
+                               BatchKeys, faster_deepcopy, unravel, ravel)
 
 if TYPE_CHECKING:
-    from slapstack.core_state import TravelEventTrackers
+    from slapstack.core_state import TravelEventTrackers, EventManager
 
 
 class LocationManager:
-    """this class is used for datastructures whose values change frequently,
+    """
+    This class is used for datastructures whose values change frequently,
     such as open storage locations, occupied storage locations, and free agv
-    positions. It is better computationally because these data structures are
-    updated often instead of needing to search for specific values in matrices.
+    positions.
 
-    open_storage_locations: set
-        open_storage_locations = {(0, 5, 0), (0, 6, 1), ...}
-    occupied_lanes:
-        dictionary[sku : dictionary[aisle:
-            dictionary[lane_direction: occupied_locations]]]
-        occupied_lanes = {
-            1: {(0, 1): {
-                "above": [(0, 5, 1), (0, 6, 1)],
-                "below": []
-            }, {(0, 2): ...
-                ...
-                ...
-            },
-            2: ...
-        }
-    free_agv_positions: set
-        free_agv_positions = {(0, 5, 0), (0, 6, 1), ...}
+    Attributes:
+        open_storage_locations (Set[int]): Locations in lanes which can be used
+        next for storage. For all lanes, the only location usable for storage is
+        the one directly adjacent to the last occupied lane location, or, if the
+        lane is empty, the first lane position from the back. Not to be confused
+        with the total number of open locations (n_open_locations).
+
+        ...
     """
-    def __init__(self, storage_matrix: np.ndarray, vehicle_matrix: np.ndarray,
-                 arrival_matrix: np.ndarray, batch_id_matrix: np.ndarray,
-                 params: SimulationParameters, lane_manager: LaneManager):
+    def __init__(self, storage_matrix: np.ndarray, arrival_matrix: np.ndarray,
+                 batch_id_matrix: np.ndarray, lane_manager: LaneManager,
+                 events: 'EventManager'):
         self.S = storage_matrix
         self.T = arrival_matrix
         self.B = batch_id_matrix
         self.batch_arrivals: Dict[np.float32, float] = {}
         self.n_levels = storage_matrix.shape[2]
         self.lane_manager = lane_manager
         self.zone_manager = ZoneManager()
-        # These correspond to one location per lane which can be used next
-        # for storage. It does not represent all of the open locations.
-        # There is no correlation between len(self.open_storage_locations) and
-        # self.n_open_locations or self.n_unlocked_open_locations.
+
         # The length of this list can be at most equal to the number of lanes.
         self.open_storage_locations = self.find_open_locations()
         self.open_storage_loc_prev = set()
         # location supersets and locked locations subsets
         self.occupied_locations = dict({})  # maps sku to occupied locations
         self.occupied_locations_cache = dict({})
         self.locked_open_storage = set()
         self.locked_occupied_storage = set()
         # locations from lanes reserved for 1st delivery legs being executed.
         self.reserved_locations = set()
 
-        self.grid = Grid(storage_matrix)
         self.sku_pick_time = {}
         self.sku_cycle_time: Dict[int, float] = {}
         # cycle_time = alpha * cycle_time + (1-alpha) * current_cycle_time
         self.CYCLE_TIME_ALPHA = 0.7
 
         self.legal_actions = []
         self.legal_retrieval_actions = defaultdict(set)
@@ -80,29 +64,47 @@
         self.n_legal_actions_total = 0
         self.n_legal_actions_squared_total = 0
         self.n_legal_actions_current = 0
 
         self.n_actions_taken = 0
         # Conditional
         self.lane_wise_entropies = {
-            (aisle, direction): 1
+            (aisle, direction): 0
             for aisle, dirs in self.lane_manager.lane_clusters.items()
             for direction, locs in dirs.items()
         }
         self.lane_wise_sku_counts: Dict[Dict[Dict[int, int]]] = {}
         self.sku_counts = defaultdict(int)
         self.n_open_locations_per_lane: \
             Dict[Tuple[Tuple[int, int], str], int] = {
                 (aisle, direction): len(locs) * self.n_levels
                 for aisle, dirs in self.lane_manager.lane_clusters.items()
                 for direction, locs in dirs.items()
             }
         self.n_total_locations_per_lane = self.n_open_locations_per_lane.copy()
+        self.events = events
+        self.sink_location = None
+        self.source_location = None
+        outline = self.S[:, :, 0]
+        io_locations = np.argwhere((outline == StorageKeys.SOURCE)
+                                   | (outline == StorageKeys.SINK))
+        self.raveled_io_locs = [ravel(tuple(i) + (0,), self.S.shape)
+                                for i in io_locations]
         # self.perform_sanity_check()
 
+    def set_source_location(self, source_loc: int):
+        """
+        Used in cross-docking to force the next delivery event to go from dock
+        to dock. See BatchLIFO retrieval policy.
+
+        :param source_loc:
+        :return:
+        """
+        self.source_location = source_loc
+
     def perform_sanity_check(self):
         """
         Performs some sanity checks to ensure that the information stored
         within various datastructures is not contradictory. The list of
         attributes tested here are non-exhaustive and can be expanded as seen
         fit.
         :return:
@@ -130,15 +132,15 @@
         :return: None.
         """
         self.occupied_locations_cache = dict({})
 
     # TODO: move all distance/routing computation to this class
     def get_free_spaces_in_lane(self, storage_location):
         assert storage_location[0:2] in self.lane_manager.tile_access_points
-        tiles_in_lane = self.lane_manager.get_lane(storage_location)
+        tiles_in_lane = self.lane_manager.get_lane_locations(storage_location)
         assert storage_location[0:2] in tiles_in_lane
         n_free_spaces = 0
         for tile in tiles_in_lane:
             for i in range(0, self.n_levels):
                 tile_with_level = tile + (i,)
                 if self.S[tile_with_level] == StorageKeys.EMPTY:
                     n_free_spaces += 1
@@ -159,30 +161,30 @@
         ubound_delivery = travel_event_stats.get_unbound_travel_events()
         if ubound_delivery >= len(self.open_storage_locations):
             if (self.open_storage_loc_prev
                     != self.open_storage_locations):
                 self.open_storage_loc_prev = self.open_storage_locations
                 self.reserved_locations = set()
                 for loc_i in self.open_storage_locations:
-                    loc = c_unravel(loc_i, self.S.shape)
-                    locations = self.lane_manager.get_lane(loc)
+                    loc = unravel(loc_i, self.S.shape)
+                    locations = self.lane_manager.get_lane_locations(loc)
                     for loc in locations:
                         for level in range(self.n_levels):
                             self.reserved_locations.add(loc + (level,))
             return self.reserved_locations
         return set()
 
     # <editor-fold desc="OUT OF ZONE LOCATION FUNCTIONS">
     def get_out_of_zone_sku_locations(
             self, sku: int, tes: 'TravelEventTrackers') -> Set[Tuple[int, int]]:
         locations = self.zone_manager.out_of_zone_skus[sku]
         if self.locked_occupied_storage != set({}):
             exclusion_set = set()
             for loc in self.locked_occupied_storage:
-                loc_tup = c_unravel(loc, self.S.shape)
+                loc_tup = unravel(loc, self.S.shape)
                 exclusion_set.add(loc_tup)
             locations = set.difference(locations, exclusion_set)
         reserved_locs = self.get_locs_lanes_reserved_for_delivery(tes)
         if reserved_locs:
             # As a minor optimization,
             # only compute intersection if reserved_locs is non-empty
             locations = set.difference(locations, reserved_locs)
@@ -205,20 +207,21 @@
         """
         # get other locations in lane
         stacks_in_lane = self.lane_manager.lock_lane(location)
         # go through each location and run lock_stack:
         delivery_action_to_return = None
         retrieval_actions_to_return = []
         # go through each stack in the lane
+        # TODO: consider using Lane object to eliminate loop
         for stack in stacks_in_lane:
             # go through each level in a stack
             for i in range(self.n_levels):
                 position = (stack + (i,))
                 # if there is a legal delivery action, lock it
-                if self.ravel(position) in self.open_storage_locations:
+                if ravel(position, self.S.shape) in self.open_storage_locations:
                     delivery_action_to_return = position
                     self.__add_locked_open_location(position)
                     self.__discard_open_location(position)
                 elem = self.S[position]
                 # if there are pallets, lock them
                 if elem != StorageKeys.EMPTY:
                     retrieval_actions_to_return.append(position)
@@ -241,27 +244,31 @@
             self.__discard_locked_occupied_location(act)
 
     def __update_sku_pick_time(self, sku, time):
         # Todo: Save only for defined time period
         self.sku_pick_time.setdefault(sku, []).append(time)
 
     def find_open_locations(self) -> Set[int]:
-        """intended to be used in initialization, when storage matrix is empty.
-        goes through each lane and gets the tuple for the storage location
-         furthest from the middle aisle"""
+        """
+        Creates a list of open locations immediately after simulation
+        initialization, when all lanes are empty.
+
+        Since this method is called exactly once, the overhead incurred by
+        looping is acceptable.
+
+        :return: A list of open locations in raveled form.
+        """
         open_locations = set({})
         for _, lanes in self.lane_manager.lane_clusters.items():
             if lanes[AccessDirection.ABOVE]:
-                open_locations.add(
-                    c_ravel(
-                        lanes[AccessDirection.ABOVE][0] + (0, ), self.S.shape))
+                open_locations.add(ravel(
+                    lanes[AccessDirection.ABOVE][0] + (0, ), self.S.shape))
             if lanes[AccessDirection.BELOW]:
-                open_locations.add(
-                    c_ravel(
-                        lanes[AccessDirection.BELOW][0] + (0, ), self.S.shape))
+                open_locations.add(ravel(
+                    lanes[AccessDirection.BELOW][0] + (0, ), self.S.shape))
         return open_locations
 
     def update_legal_actions_statistics(self):
         self.n_legal_actions_current = len(self.legal_actions)
         self.n_legal_actions_total += self.n_legal_actions_current
         self.n_legal_actions_squared_total += (self.n_legal_actions_current
                                                * self.n_legal_actions_current)
@@ -348,17 +355,21 @@
             self, storage_position: Tuple[int, int, int], pallet_sku: int):
         """remove the given SKU from the storage position in
         self.occupied_lanes
 
         Raises KeyError when trying to remove an inexistent position from the
         cache.
         """
-        self.occupied_locations[pallet_sku].remove(self.ravel(storage_position))
+        self.occupied_locations[pallet_sku].remove(
+            ravel(storage_position, self.S.shape))
         self.lane_manager.remove_from_occupied_lane(
             storage_position, pallet_sku)
+        tgt_lane: Lane = self.lane_manager.get_lane(storage_position)
+        tgt_lane.update_sku_border(pallet_sku, storage_position, added=False)
+
 
     def assert_storage_and_time_are_similar(self, storage_location):
         if self.S[storage_location] > StorageKeys.EMPTY:  # if storage
             # location is not empty
             assert self.T[storage_location] != -1
         else:  # if storage is empty
             assert self.T[storage_location] == -1,\
@@ -385,15 +396,14 @@
                 storage_location, pallet_sku)
         else:  # delivering a pallet.
             self.lane_manager.add_lane_assignment(storage_location, pallet_sku)
             self.__add_pallet(storage_location, pallet_sku)
             # self.open_storage_locations.discard(storage_location)
             self.__discard_open_location(storage_location)
             self.__open_next_location(storage_location)
-            self.grid.add_obstacle(storage_location[:2])
             # self.assert_storage_and_time_are_similar(storage_location)
 
         return shift_penalty
 
     def __update_location_cache_on_retrieval(
             self, location: Tuple[int, int, int], sku: int):
         # remove sku from storage_matrix (and arrival time from time matrix)
@@ -404,40 +414,20 @@
         self.__add_open_location(location)
         # if pallets need to be shifted
         shift_needed = self.__shift_needed(location)
         if shift_needed:
             shift_penalty, location = self.__shift_pallets_in_lane(location)
         else:
             shift_penalty = 0
-        self.grid.remove_obstacle(location[0:2])
         # self.assert_storage_and_time_are_similar(location)
         # if lane is empty, unassign it
         if self.lane_manager.pure_lanes:
             self.lane_manager.unassign_empty_lane(location, sku)
         return shift_penalty
 
-    def find_sku_previous_location(
-            self, storage_location: Tuple[int, int, int]) -> int:
-        """
-        UNUSED.
-
-        :param storage_location:
-        :return:
-        """
-        previous_position = list(storage_location)
-        previous_position[2] = previous_position[2] - 1
-        if previous_position[2] < 0:  # if stack is full
-            # TODO: Check if lane is already empty and
-            #  we're going out of bounds.
-            previous_position[2] = self.n_levels - 1
-            direction = self.lane_manager.get_access_point_direction(
-                tuple(storage_location))
-            previous_position[0] = previous_position[0] + direction
-        return max(self.S[tuple(previous_position)], StorageKeys.EMPTY)
-
     def __open_next_location(self, storage_location: Tuple[int, int, int]):
         """
         Called on the delivery of a pallet to add the next location relative to
         the access aisle to open locations.
 
         :param storage_location: The location where the pallet was delivered.
         :return: None.
@@ -452,17 +442,21 @@
 
         if self.S[tuple(next_position)] >= StorageKeys.EMPTY:
             next_position_t = cast(Tuple[int, int, int], tuple(next_position))
             self.__add_open_location(next_position_t)
 
     # <editor-fold desc="SHIFT MECHANISM">
     def __shift_needed(self, storage_position: Tuple[int, int, int]) -> bool:
-        """returns true if the current position is empty and the next position
-        is not
+        """
+        Checks if the retrieval of a pallet leads to the formation of a hole in
+        the lane (i.e. an unoccupied position surrounded by occupied locations).
 
+        :param storage_position: The position from which a pallet is to be
+            retrieved.
+        :return: True whether the retrieval creates a hole.
         """
         shift_candidate, _, _ = self.__get_shift_src(storage_position)
         if self.S[tuple(shift_candidate)] \
                 not in [StorageKeys.EMPTY, StorageKeys.AISLE]:
             return True
         return False
 
@@ -494,107 +488,119 @@
         if self.lane_manager.level_too_high(shift_src):
             shift_src[2] = 0  # z
             shift_src[0] = shift_src[0] + direction  # x
         return shift_src, shift_tgt, direction
 
     def __shift_pallets_in_lane(
             self, storage_location) -> (int, Tuple[int, int, int]):
-        """go through each pallet in a lane and move it one space away from the
-        aisle to prevent holes from. also gives a penalty for each pallet that
-        needed to be shifted"""
+        """
+        Goes through each pallet in a lane and moves it one space away from the
+        aisle to prevent holes from forming. A penalty proportional to the
+        number of shifts required to circumvent the hole formation is returned.
+
+        If the retrieval indicated by the storage_location parameter does not
+        create a hole, no action is taken.
+
+        :param storage_location: The location from which a pallet is retrieved.
+        :return: A tuple containing the number of shifts and the new position of
+            an empty tile.
+        """
         self.__discard_open_location(storage_location)
         # shift all pallets that are closer to aisle (or above retrieved pallet)
         shift_src, shift_tgt, direction = self.__get_shift_src(storage_location)
         shift_penalty = 0
         while not (self.lane_manager.is_lane(shift_src)
                    or self.is_empty(tuple(shift_src))):
             # perform shift!
-            self.__shift_pallet(direction, shift_src, shift_tgt)
+            self.__shift_pallet(shift_src, shift_tgt)
             self.zone_manager.update_any_out_of_zone_sku_locations(
                 shift_src, shift_tgt, self.S[tuple(shift_tgt)]
             )
             shift_src, shift_tgt, direction = self.__get_shift_src(shift_src)
             shift_penalty += 1
         released_tile = cast(Tuple[int, int, int], tuple(shift_tgt))
         self.__add_open_location(released_tile)
         return shift_penalty, released_tile
 
-    def __shift_pallet(self, direction, shift_src, shift_tgt):
-        """shifts one pallet one position away from the middle aisle in order
-        to 'plug up' holes. then gets next two positions to check if a shift is
-        needed"""
+    def __shift_pallet(self, shift_src, shift_tgt):
+        """
+        Updates the simulation structures reflecting the shift of a pallet from
+        shift_src (the next hole) to shift_tgt (the previous hole).
+
+        :param shift_src: The previous position of the pallet in lane
+            (now a hole).
+        :param shift_tgt: The next position of the pallet to be shifted.
+        :return: None.
+        """
         next_hole = tuple(shift_src)
         ex_hole = tuple(shift_tgt)
         shift_sku = self.S[next_hole]
         self.S[ex_hole] = shift_sku
         self.T[ex_hole] = self.T[next_hole]
         self.B[ex_hole] = self.B[next_hole]
         self.S[next_hole] = StorageKeys.EMPTY
         self.T[next_hole] = TimeKeys.NAN.value  # -1
         self.B[next_hole] = BatchKeys.NAN.value  # -1
         self.__add_pallet(ex_hole, shift_sku)
         self.__remove_pallet(next_hole, shift_sku)
-
     # <editor-fold desc="SHIFT MECHANISM">
 
     def __add_pallet(
             self, storage_location: Tuple[int, int, int], pallet_sku: int):
         """adds storage location tuple for new pallets to add to
          occupied_lanes"""
         self.lane_manager.add_to_occupied_lane(storage_location, pallet_sku)
+        tgt_lane: Lane = self.lane_manager.get_lane(storage_location)
+        tgt_lane.update_sku_border(pallet_sku, storage_location, added=True)
         if pallet_sku not in self.occupied_locations:
-            self.occupied_locations[pallet_sku] = {self.ravel(storage_location)}
+            self.occupied_locations[pallet_sku] = {
+                ravel(storage_location, self.S.shape)}
         else:
             self.occupied_locations[pallet_sku].add(
-                self.ravel(storage_location))
+                ravel(storage_location, self.S.shape))
 
     def is_empty(self, next_position):
         """returns true if storage position is empty"""
         if self.S[next_position] == StorageKeys.EMPTY:
             return True
         else:
             return False
 
-    def ravel(self, position: Tuple[int, int, int]) -> int:
-        """changes tuple (13, 6, 1) to integer 138"""
-        # assert isinstance(position, Tuple)
-        return c_ravel(position, self.S.shape)
-
     def __add_open_location(self, position: Tuple[int, int, int]):
         """takes a position tuple (3,1,4) and ravels it into one integer (154)
          based on the dimensions of the warehouse then adds it
          to the open_storage_location set."""
         if position is None:
             return
-        self.open_storage_locations.add(self.ravel(position))
+        self.open_storage_locations.add(ravel(position, self.S.shape))
 
     def __discard_open_location(self, position):
         if position is None:
             return
-        self.open_storage_locations.discard(self.ravel(position))
+        self.open_storage_locations.discard(ravel(position, self.S.shape))
 
     def __add_locked_open_location(self, position):
         if position is None:
             return
-        self.locked_open_storage.add(self.ravel(position))
+        self.locked_open_storage.add(ravel(position, self.S.shape))
 
     def __discard_locked_open_location(self, position):
         if position is None:
             return
-        self.locked_open_storage.discard(self.ravel(position))
+        self.locked_open_storage.discard(ravel(position, self.S.shape))
 
     def __add_locked_occupied_location(self, position):
         if position is None:
             return
-        self.locked_occupied_storage.add(self.ravel(position))
+        self.locked_occupied_storage.add(ravel(position, self.S.shape))
 
     def __discard_locked_occupied_location(self, position):
         if position is None:
             return
-        self.locked_occupied_storage.discard(self.ravel(position))
+        self.locked_occupied_storage.discard(ravel(position, self.S.shape))
 
     def get_open_locations(self, sku=None) -> Set[int]:
         """returns list of open storage locations. removes locations that are
         currently locked."""
         if self.lane_manager.pure_lanes and sku:
             open_locations = self.get_open_storage_locations_pure(sku)
         else:
@@ -640,17 +646,17 @@
         """goes through the lane_assigned dictionary, gets lanes that aren't
         assigned and returns all the storage locations in those lanes"""
         # print("getting unassigned storage locations")
         unassigned_lanes = set()
         for key, value in self.lane_manager.lane_assigned.items():
             if not value:   # if lane not assigned
                 unassigned_lanes.add(key)
-        unassigned_lane_locations = self.lane_manager.get_locations_in_lanes(
-            unassigned_lanes, asint=True)
-
+        unassigned_lane_locations: Set[int] = (
+            self.lane_manager.get_locations_in_lanes(
+                unassigned_lanes, asint=True))
         return set.intersection(unassigned_lane_locations,
                                 set(self.get_open_locations()))
 
     def get_sku_locations(
             self, sku: int, tes: 'TravelEventTrackers') -> Set[int]:
         """
         returns list of locations with specified SKU. removes locations that
@@ -674,14 +680,17 @@
         #             and self.occupied_locations_cache[sku]):
         #         locations = self.occupied_locations_cache[sku]
         #     else:
         #         # the following call also filters locked_occupied_storage
         #         locations = self.get_actions_closest_to_aisle(sku)
         #         self.occupied_locations_cache[sku] = locations
         # else:
+        if self.source_location:
+            locations = {self.source_location}
+            return locations
         if sku in self.occupied_locations and self.occupied_locations[sku]:
             locations = (self.occupied_locations[sku]
                          - self.locked_occupied_storage)
             reserved_locs = self.get_locs_lanes_reserved_for_delivery(tes)
             if reserved_locs:
                 # As a minor optimization,
                 # only compute intersection if reserved_locs is non-empty
@@ -695,28 +704,30 @@
     #     """updates storage and arrival matrices within given values"""
     #     p = position
     #     self.S[p[0], p[1], p[2]] = s_value
     #     self.T[p[0], p[1], p[2]] = t_value
     #     self.B[p[0], p[1], p[2]] = b_value
 
     def __get_first_suitable_tile(
-            self, lane: List[Tuple[int, int]], sku: int) -> Union[int, None]:
-        """
-        Note that the tiles within the lanes in the lane_cluster datastructure
-        are sorted descendingly with respect to their distance from the closest
-        aisle.
-
-        TODO: finish comment
-        :param lane:
-        :param sku:
-        :return:
+            self, lane: Lane, sku: int) -> Union[int, None]:
         """
-        int_loc = get_first_tile(
-            self.occupied_locations[sku], self.locked_occupied_storage,
-            lane, len(lane), self.n_levels, self.S.shape)
+        Given a lane and an sku, this method finds the sku position in the lane
+        which is closest to the aisle. Raises an error if the SKU is not
+        contained in the lane (see get_border_tile in Lane class), the retrieved
+        tile is not present in the occupied_locations[sku] or the tile is
+        present in the locked storage.
+
+        :param lane: The lane object to retrieve the border sku tile from.
+        :param sku: The sku for which to retrieve the border tile.
+        :return: The border sku tile in raveled form.
+        """
+        location = lane.get_border_tile(sku)
+        int_loc = ravel(location, self.S.shape)
+        assert int_loc in self.occupied_locations[sku]
+        assert int_loc not in self.locked_occupied_storage
         return int_loc
 
     def get_actions_closest_to_aisle(
             self, sku: int) -> Union[Set[int], List[int]]:
         """
         used for retrieval. if lanes are pure, then get_occupied_locations
         only returns the pallet that is closest to the aisle. This means an
@@ -727,18 +738,38 @@
         :param sku:
         :return:
         """
         closest_pallets = set({})
         if sku not in self.lane_manager.sku_lanes:
             return set({})
         else:
-            for lane in self.lane_manager.sku_lanes[sku]:
+            for lane_ap in self.lane_manager.sku_lanes[sku]:
                 direction = (AccessDirection.ABOVE
-                             if lane[2] == -1 else AccessDirection.BELOW)
-                lane = self.lane_manager.lane_clusters[lane[0:2]][direction]
+                             if lane_ap[2] == -1 else AccessDirection.BELOW)
+                lane = self.lane_manager.lane_clusters[lane_ap[0:2]][direction]
                 int_loc = self.__get_first_suitable_tile(lane, sku)
                 if int_loc is not None:
                     closest_pallets.add(int_loc)
             return closest_pallets  # closest_pallets_raveled
 
     def __deepcopy__(self, memo):
         return faster_deepcopy(self, memo)
+
+    def get_direct_sink_action(self, sku):
+        """
+        Checks if there is an order requiring the SKU passed as a parameter
+        waiting at one of the sink tiles.
+
+        :param sku: The order to check.
+        :return: The sink location requiring the sku or None if no such sink
+            location exists.
+        """
+        events = self.events
+        sink_location = None
+        if events.queued_retrieval_orders.get(sku):
+            retrieval_orders = events.queued_retrieval_orders.get(sku)
+            if len(retrieval_orders) > 0:
+                retrieval_order = retrieval_orders[0]
+                self.sink_location = self.raveled_io_locs[retrieval_order.sink]
+            else:
+                self.sink_location = None
+        return sink_location
```

### Comparing `slapstack-0.0.24/slapstack/core_state_zone_manager.py` & `slapstack-0.1.1/slapstack/core_state_zone_manager.py`

 * *Files identical despite different names*

### Comparing `slapstack-0.0.24/slapstack/helpers.py` & `slapstack-0.1.1/slapstack/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 # <editor-fold desc="Utility Functions">
 from typing import List, Callable, Tuple, Dict, Union
 
 import numpy as np
 # noinspection PyPackageRequirements, PyProtectedMember
 from joblib._multiprocessing_helpers import mp
+from numpy import ndarray
+
 
 # from slapstack.envs.interface_templates import SimulationParameters
 
 
 def hole_found(storage_matrix, locations):
     empty_space = False
     elements = []
@@ -181,15 +183,15 @@
 #         state_stack_size=1,
 #         resetting=False,
 #         order_list=None,
 #         initial_pallets_sku_counts=None,
 #         initial_pallets_storage_strategy=None,
 #         n_sources=1,
 #         n_sinks=1,
-#         WEPAStacks=None,
+#         use_cases=None,
 #         pure_lanes=False
 #     )
 #     seed = 123456
 #     # log_path = '../3_visualization_d3js/sim_data/'
 #     log_path = ''
 #     return environment_parameters, seed, log_path
 
@@ -313,7 +315,30 @@
     ACCESS_TO_STORAGE = 3
     AISLE_TO_ACCESS = 4
     AISLE_TO_AISLE = 5
     AISLE_TO_STORAGE = 6
     STORAGE_TO_AISLE = 7
     STORAGE_TO_STORAGE = 8
     STORAGE_TO_ACCESS = 9
+
+
+def ravel(position: Tuple[int, int, int], dims: Tuple[int, int, int]) -> int:
+    int_position = (position[0] * dims[1] * dims[2]
+                    + position[1] * dims[2] + position[2])
+    return int_position
+
+
+def ravel2(position: Tuple[int, int], shape: Tuple[int, int]) -> int:
+    return position[0] * shape[1] + position[1]
+
+
+def unravel(position_enc: int, dims) -> Tuple[int, int, int]:
+    z: int = position_enc % dims[2]
+    y: int = (position_enc // dims[2]) % dims[1]
+    x: int = (position_enc // dims[2]) // dims[1]
+    return x, y, z
+
+
+def unravel2(int_encoding: int, shape: Tuple[int, int]) -> Tuple[int, int]:
+    y: int = int_encoding % shape[1]
+    x: int = int_encoding // shape[1]
+    return x, y
```

### Comparing `slapstack-0.0.24/slapstack/interface.py` & `slapstack-0.1.1/slapstack/interface.py`

 * *Files identical despite different names*

### Comparing `slapstack-0.0.24/slapstack/WEPAStacks/Initial_fill_lvl.json` & `slapstack-0.1.1/slapstack/use_cases/wepastacks/3_initial_fill_lvl.json`

 * *Files identical despite different names*

### Comparing `slapstack-0.0.24/slapstack/WEPAStacks/layouts/layout1_middle_aisles.csv` & `slapstack-0.1.1/slapstack/use_cases/wepastacks/1_layout.csv`

 * *Files identical despite different names*

### Comparing `slapstack-0.0.24/slapstack/WEPAStacks/Orders_v5.json` & `slapstack-0.1.1/slapstack/use_cases/wepastacks/2_orders.json`

 * *Files identical despite different names*

