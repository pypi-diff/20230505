# Comparing `tmp/optiframe-0.4.0.tar.gz` & `tmp/optiframe-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optiframe-0.4.0.tar", max compression
+gzip compressed data, was "optiframe-0.5.0.tar", max compression
```

## Comparing `optiframe-0.4.0.tar` & `optiframe-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1069 2023-03-12 14:09:36.025204 optiframe-0.4.0/LICENSE
--rw-r--r--   0        0        0     2108 2023-04-27 09:43:25.701305 optiframe-0.4.0/README.md
--rw-r--r--   0        0        0      385 2023-04-16 20:21:48.040887 optiframe-0.4.0/optiframe/__init__.py
--rw-r--r--   0        0        0      412 2023-04-27 09:43:25.705305 optiframe-0.4.0/optiframe/framework/__init__.py
--rw-r--r--   0        0        0     2561 2023-04-16 20:21:48.040887 optiframe-0.4.0/optiframe/framework/default_tasks.py
--rw-r--r--   0        0        0      267 2023-04-16 20:21:48.040887 optiframe-0.4.0/optiframe/framework/errors.py
--rw-r--r--   0        0        0     1042 2023-04-27 10:01:50.790921 optiframe-0.4.0/optiframe/framework/metrics.py
--rw-r--r--   0        0        0     8957 2023-04-27 10:01:50.790921 optiframe-0.4.0/optiframe/framework/optimizer.py
--rw-r--r--   0        0        0     1042 2023-04-27 10:01:50.790921 optiframe-0.4.0/optiframe/framework/tasks.py
--rw-r--r--   0        0        0        0 2023-04-01 14:13:27.609904 optiframe-0.4.0/optiframe/py.typed
--rw-r--r--   0        0        0      306 2023-04-16 20:21:48.040887 optiframe-0.4.0/optiframe/workflow_engine/__init__.py
--rw-r--r--   0        0        0      496 2023-04-27 10:01:50.790921 optiframe-0.4.0/optiframe/workflow_engine/errors.py
--rw-r--r--   0        0        0     6909 2023-04-27 10:01:50.790921 optiframe-0.4.0/optiframe/workflow_engine/step.py
--rw-r--r--   0        0        0     1055 2023-04-27 10:01:50.790921 optiframe-0.4.0/optiframe/workflow_engine/task.py
--rw-r--r--   0        0        0     2322 2023-04-27 10:01:50.790921 optiframe-0.4.0/optiframe/workflow_engine/workflow.py
--rw-r--r--   0        0        0     1087 2023-04-27 10:42:09.187081 optiframe-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 optiframe-0.4.0/setup.py
--rw-r--r--   0        0        0     2675 1970-01-01 00:00:00.000000 optiframe-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-12 14:09:36.025204 optiframe-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2108 2023-04-27 09:43:25.701305 optiframe-0.5.0/README.md
+-rw-r--r--   0        0        0      713 2023-05-05 16:47:57.468253 optiframe-0.5.0/optiframe/__init__.py
+-rw-r--r--   0        0        0      614 2023-05-05 16:47:57.468253 optiframe-0.5.0/optiframe/framework/__init__.py
+-rw-r--r--   0        0        0     2562 2023-05-05 16:47:57.468253 optiframe-0.5.0/optiframe/framework/default_tasks.py
+-rw-r--r--   0        0        0      267 2023-04-16 20:21:48.040887 optiframe-0.5.0/optiframe/framework/errors.py
+-rw-r--r--   0        0        0     1042 2023-04-27 10:01:50.790921 optiframe-0.5.0/optiframe/framework/metrics.py
+-rw-r--r--   0        0        0     9165 2023-05-05 16:47:57.468253 optiframe-0.5.0/optiframe/framework/optimizer.py
+-rw-r--r--   0        0        0     3875 2023-05-05 16:47:57.468253 optiframe-0.5.0/optiframe/framework/tasks.py
+-rw-r--r--   0        0        0        0 2023-04-01 14:13:27.609904 optiframe-0.5.0/optiframe/py.typed
+-rw-r--r--   0        0        0      306 2023-05-02 10:36:41.391576 optiframe-0.5.0/optiframe/workflow_engine/__init__.py
+-rw-r--r--   0        0        0      496 2023-04-27 10:01:50.790921 optiframe-0.5.0/optiframe/workflow_engine/errors.py
+-rw-r--r--   0        0        0     6909 2023-05-05 16:47:57.468253 optiframe-0.5.0/optiframe/workflow_engine/step.py
+-rw-r--r--   0        0        0     1522 2023-05-05 16:47:57.468253 optiframe-0.5.0/optiframe/workflow_engine/task.py
+-rw-r--r--   0        0        0     2322 2023-05-02 10:36:41.391576 optiframe-0.5.0/optiframe/workflow_engine/workflow.py
+-rw-r--r--   0        0        0     1092 2023-05-05 17:04:50.228434 optiframe-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 optiframe-0.5.0/setup.py
+-rw-r--r--   0        0        0     2675 1970-01-01 00:00:00.000000 optiframe-0.5.0/PKG-INFO
```

### Comparing `optiframe-0.4.0/LICENSE` & `optiframe-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optiframe-0.4.0/README.md` & `optiframe-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `optiframe-0.4.0/optiframe/framework/default_tasks.py` & `optiframe-0.5.0/optiframe/framework/default_tasks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 """The default tasks of the optimization framework.
 
 These tasks are added to the steps automatically when constructing the optimizer.
 """
 from dataclasses import dataclass
 from typing import Any, Optional
 
-from pulp import LpProblem, LpMinimize, LpAffineExpression, LpStatus, LpMaximize
+from pulp import LpAffineExpression, LpMaximize, LpMinimize, LpProblem, LpStatus
 
-from optiframe.framework.errors import InfeasibleError
-from optiframe.framework.tasks import BuildMipTask, ExtractSolutionTask
 from optiframe.workflow_engine import Task
 
+from .errors import InfeasibleError
+from .tasks import MipConstructionTask, SolutionExtractionTask
+
 
 @dataclass
 class ProblemSettings:
     """The settings to configure the MIP."""
 
     name: str
     sense: LpMinimize | LpMaximize
 
 
-class CreateProblemTask(BuildMipTask[LpProblem]):
+class CreateProblemTask(MipConstructionTask[LpProblem]):
     """A task to initialize the MIP object."""
 
     problem_settings: ProblemSettings
 
     def __init__(self, problem_settings: ProblemSettings):
         self.problem_settings = problem_settings
 
-    def execute(self) -> LpProblem:
+    def construct_mip(self) -> LpProblem:
         """Create the `LpProblem` instance to make it available to other tasks."""
         problem = LpProblem(self.problem_settings.name, self.problem_settings.sense)
         # Initialize the objective to an empty expression
         problem.setObjective(LpAffineExpression())
         return problem
 
 
@@ -72,20 +73,20 @@
 @dataclass
 class SolutionObjValue:
     """The objective value of the solution."""
 
     objective_value: float
 
 
-class ExtractSolutionObjValueTask(ExtractSolutionTask[SolutionObjValue]):
+class SolutionObjValueExtractionTask(SolutionExtractionTask[SolutionObjValue]):
     """A task to extract the objective value from the solved MIP."""
 
     problem: LpProblem
 
     def __init__(self, problem: LpProblem):
         self.problem = problem
 
-    def execute(self) -> SolutionObjValue:
+    def extract_solution(self) -> SolutionObjValue:
         """Extract the objective value from the solved MIP."""
         cost = self.problem.objective.value()
 
         return SolutionObjValue(cost)
```

### Comparing `optiframe-0.4.0/optiframe/framework/metrics.py` & `optiframe-0.5.0/optiframe/framework/metrics.py`

 * *Files identical despite different names*

### Comparing `optiframe-0.4.0/optiframe/framework/optimizer.py` & `optiframe-0.5.0/optiframe/framework/optimizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """The optimizer classes used to configure and execute the optimization process."""
 from __future__ import annotations
 
 import tempfile
 from dataclasses import dataclass
 from datetime import datetime, timedelta
-from typing import Optional, Self, Type, Any
+from typing import Any, Optional, Self, Type
 
-from pulp import LpProblem, LpMinimize, LpMaximize
+from pulp import LpMaximize, LpMinimize, LpProblem
 
 from optiframe.workflow_engine import Step, StepData
-from optiframe.workflow_engine.workflow import Workflow, InitializedWorkflow
+from optiframe.workflow_engine.workflow import InitializedWorkflow, Workflow
 
 from .default_tasks import (
     CreateProblemTask,
-    SolveTask,
-    SolveSettings,
-    ExtractSolutionObjValueTask,
     ProblemSettings,
+    SolutionObjValueExtractionTask,
+    SolveSettings,
+    SolveTask,
 )
-from .metrics import StepTimes, ModelSize
-from .tasks import BuildMipTask, ValidateTask, PreProcessingTask, ExtractSolutionTask
+from .metrics import ModelSize, StepTimes
+from .tasks import MipConstructionTask, PreProcessingTask, SolutionExtractionTask, ValidationTask
 
 
 @dataclass
 class OptimizationModule:
     """A modules bundling tasks for each steps of the optimization process."""
 
-    build_mip: Type[BuildMipTask[Any]]
-    validate: Optional[Type[ValidateTask]] = None
+    validation: Optional[Type[ValidationTask]] = None
     pre_processing: Optional[Type[PreProcessingTask[Any]]] = None
-    extract_solution: Optional[Type[ExtractSolutionTask[Any]]] = None
+    mip_construction: Optional[Type[MipConstructionTask[Any]]] = None
+    solution_extraction: Optional[Type[SolutionExtractionTask[Any]]] = None
 
 
 class Optimizer:
     """An optimizer for an optimization problem.
 
     Can be configured by adding optimization modules,
     which implement the actual optimization process.
@@ -67,40 +67,43 @@
 
     def initialize(self, *data: Any) -> InitializedOptimizer:
         """Initialize the optimizer with the data defining the problem instance.
 
         Which data classes need to be added here depends on the modules
         that have been added to the optimizer.
         """
-        validate_step = Step("validate")
+        validation_step = Step("validation")
         pre_processing_step = Step("pre_processing")
-        build_mip_step = Step("build_mip").add_tasks(CreateProblemTask)
-        solve_step = Step("solve").add_tasks(SolveTask)
-        extract_solution_step = Step("extract_solution").add_tasks(ExtractSolutionObjValueTask)
+        mip_construction_step = Step("mip_construction").add_tasks(CreateProblemTask)
+        solving_step = Step("solving").add_tasks(SolveTask)
+        solution_extraction_step = Step("solution_extraction").add_tasks(
+            SolutionObjValueExtractionTask
+        )
 
         for module in self.modules:
-            if module.validate is not None:
-                validate_step.add_tasks(module.validate)
+            if module.validation is not None:
+                validation_step.add_tasks(module.validation)
 
             if module.pre_processing is not None:
                 pre_processing_step.add_tasks(module.pre_processing)
 
-            build_mip_step.add_tasks(module.build_mip)
+            if module.mip_construction is not None:
+                mip_construction_step.add_tasks(module.mip_construction)
 
-            if module.extract_solution is not None:
-                extract_solution_step.add_tasks(module.extract_solution)
+            if module.solution_extraction is not None:
+                solution_extraction_step.add_tasks(module.solution_extraction)
 
         workflow = (
             Workflow()
             .add_steps(
-                validate_step,
+                validation_step,
                 pre_processing_step,
-                build_mip_step,
-                solve_step,
-                extract_solution_step,
+                mip_construction_step,
+                solving_step,
+                solution_extraction_step,
             )
             .initialize(*data)
             .add_data(ProblemSettings(name=self.name, sense=self.sense))
         )
         return InitializedOptimizer(workflow)
```

### Comparing `optiframe-0.4.0/optiframe/workflow_engine/step.py` & `optiframe-0.5.0/optiframe/workflow_engine/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 
 from __future__ import annotations
 
 import inspect
 import logging
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Self, Type, Any
+from typing import Any, Self, Type, TypeVar
 
 from .errors import InjectionError, ScheduleError
 from .task import Task
 
-
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class TaskDependency:
     """A dependency required by a task, as defined in the `.__init__` method."""
 
@@ -122,15 +121,15 @@
             for task in tasks_to_execute:
                 if len(missing_dependencies[task]) == 0:
                     # Create the data parameters to instantiate the task
                     dep_data = {
                         dep.param: self.step_data[dep.annotation] for dep in dependencies[task]
                     }
                     # Determine what type of data is created by the task
-                    data_annotation = inspect.signature(task.execute).return_annotation
+                    data_annotation = task.get_return_type()
 
                     # Instantiate the task, using the data it requires
                     task_obj = task(**dep_data)
 
                     # Execute the action of the task and save the returned data
                     data = task_obj.execute()
 
@@ -193,7 +192,10 @@
                     )
 
                 task_dependencies.append(TaskDependency(param=param, annotation=annotation))
 
             dependencies[task] = task_dependencies
 
         return dependencies
+
+
+X = TypeVar("X")
```

### Comparing `optiframe-0.4.0/optiframe/workflow_engine/task.py` & `optiframe-0.5.0/optiframe/workflow_engine/task.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """A task in the workflow which executes a specific action."""
 import abc
-from typing import TypeVar, Generic
+import inspect
+from typing import Any, Generic, TypeVar
 
 T = TypeVar("T")
 
 
 class Task(abc.ABC, Generic[T]):
     """A task in the workflow which executes a specific action.
 
@@ -22,7 +23,20 @@
 
         This method is called once all the dependencies of the task have been gathered.
         It can access the data of the dependencies through the `self` parameter.
 
         The data that is returned from this method can be used by other tasks.
         """
         pass
+
+    @classmethod
+    def get_return_type(cls) -> Any:
+        """Get the type of data returned by the task.
+
+        Defaults to the return annotation defined for `.execute`.
+
+        This is important for the task scheduler to determine which
+        type of data is generated by the task.
+
+        For subclasses that define other methods, this needs to be overriden.
+        """
+        return inspect.signature(cls.execute).return_annotation
```

### Comparing `optiframe-0.4.0/optiframe/workflow_engine/workflow.py` & `optiframe-0.5.0/optiframe/workflow_engine/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Complete workflows, composed of steps which are composed of tasks."""
 from __future__ import annotations
 
-from typing import Self, Any
+from typing import Any, Self
 
 from .step import Step, StepData
 
 
 class Workflow:
     """A complete workflow.
```

### Comparing `optiframe-0.4.0/pyproject.toml` & `optiframe-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optiframe"
-version = "0.4.0"
+version = "0.5.0"
 description = "A modular framework for mixed integer programming."
 authors = ["Tim Jentzsch <optiframe.projects@timjen.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/TimJentzsch/optiframe"
 exclude = ["examples", "tests"]
 
@@ -22,15 +22,15 @@
 mypy = "^1.1.1"
 
 [tool.black]
 line-length = 100
 
 [tool.ruff]
 line-length = 100
-select = ["E", "F", "D"]
+select = ["E", "F", "D", "I"]
 ignore = [
     # multi-line-summary-second-line
     # Collides with other lint rule and is non-standard
     "D213",
     # one-blank-line-before-class
     # Collides with other lint rule and is non-standard
     "D203",
```

### Comparing `optiframe-0.4.0/setup.py` & `optiframe-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['pulp>=2.7.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['knapsack = examples.knapsack:demo']}
 
 setup_kwargs = {
     'name': 'optiframe',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'A modular framework for mixed integer programming.',
     'long_description': '# Optiframe [![PyPI Version](https://img.shields.io/pypi/v/optiframe)](https://pypi.org/project/optiframe/) [![License](https://img.shields.io/pypi/l/optiframe)](LICENSE)\n\nOptiframe is an **opti**mization **frame**work for writing mixed integer programs (MIPs).\n\nIt allows you to structure your MIPs in a way that allows clear separation of concerns,\nhigh modularity and testability.\n\n## Core Concepts\n\n- The optimization process is divided into multiple **steps** which are clearly separated:\n  1. **Validation** allows you to validate the input data.\n  2. **Pre-processing** allows you to optimize the provided data to reduce the size of the final model.\n  3. **MIP building** allows you to modify the MIP to define the optimization problem.\n  4. **Solving** is a pre-defined step that obtains an optimal solution for the problem.\n  5. **Solution extraction** allows you to process the variable values of the solution into something more meaningful.\n- **Tasks** are the core components that allow you to implement functionality for each step.\n  - The constructor of a task allows you to define *dependencies* for that task,\n    which are automatically injected by the optimizer based on their type annotation.\n  - The **execute** method allows you to implement the functionality.\n    It may return data which can then be used by other tasks as a dependency.\n- **Modules** combine tasks that belong together.\n    Each module must contain a task for building the MIP and can additionally contain tasks\n    for validation, pre-processing and solution extraction.\n    The modules are what makes Optiframe so extendable:\n    You can define extensions of a problem in a separate module and only include it if needed.\n- The **optimizer** allows you to configure the packages that you need.\n    Afterwards, you can initialize it with the instance data and then solve the optimization problem.\n\n## Installation & Usage\n\n```cli\npip install optiframe\n```\n\nTake a look at the `examples` folder for examples on how to use Optiframe!\n\n## License\n\nThis project is available under the terms of the [MIT license](LICENSE).\n',
     'author': 'Tim Jentzsch',
     'author_email': 'optiframe.projects@timjen.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/TimJentzsch/optiframe',
```

### Comparing `optiframe-0.4.0/PKG-INFO` & `optiframe-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optiframe
-Version: 0.4.0
+Version: 0.5.0
 Summary: A modular framework for mixed integer programming.
 Home-page: https://github.com/TimJentzsch/optiframe
 License: MIT
 Author: Tim Jentzsch
 Author-email: optiframe.projects@timjen.net
 Requires-Python: >=3.11.0rc1
 Classifier: License :: OSI Approved :: MIT License
```

