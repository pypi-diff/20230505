# Comparing `tmp/cog-0.7.0b9-py3-none-any.whl.zip` & `tmp/cog-0.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,43 +1,30 @@
-Zip file size: 60332 bytes, number of entries: 41
--rw-r--r--  2.0 unx       13 b- defN 23-Feb-10 14:45 cog/.gitignore
--rw-r--r--  2.0 unx      314 b- defN 23-Feb-10 14:45 cog/__init__.py
--rw-r--r--  2.0 unx      162 b- defN 23-Feb-10 14:47 cog/_version.py
--rw-r--r--  2.0 unx      286 b- defN 23-Feb-10 14:45 cog/errors.py
--rw-r--r--  2.0 unx     2066 b- defN 23-Feb-10 14:45 cog/files.py
--rw-r--r--  2.0 unx     1973 b- defN 23-Feb-10 14:45 cog/json.py
--rw-r--r--  2.0 unx     3130 b- defN 23-Feb-10 14:45 cog/logging.py
--rw-r--r--  2.0 unx     8698 b- defN 23-Feb-10 14:45 cog/predictor.py
--rw-r--r--  2.0 unx     2385 b- defN 23-Feb-10 14:45 cog/schema.py
--rw-r--r--  2.0 unx      645 b- defN 23-Feb-10 14:45 cog/suppress_output.py
--rw-r--r--  2.0 unx     6509 b- defN 23-Feb-10 14:45 cog/types.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-10 14:45 cog/command/__init__.py
--rw-r--r--  2.0 unx      880 b- defN 23-Feb-10 14:45 cog/command/openapi_schema.py
--rw-r--r--  2.0 unx      547 b- defN 23-Feb-10 14:45 cog/director/Dockerfile
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-10 14:45 cog/director/__init__.py
--rw-r--r--  2.0 unx     3628 b- defN 23-Feb-10 14:45 cog/director/__main__.py
--rw-r--r--  2.0 unx      353 b- defN 23-Feb-10 14:45 cog/director/cloudbuild.yaml
--rw-r--r--  2.0 unx    17504 b- defN 23-Feb-10 14:45 cog/director/director.py
--rw-r--r--  2.0 unx      321 b- defN 23-Feb-10 14:45 cog/director/eventtypes.py
--rw-r--r--  2.0 unx     4469 b- defN 23-Feb-10 14:45 cog/director/healthchecker.py
--rw-r--r--  2.0 unx     1259 b- defN 23-Feb-10 14:45 cog/director/http.py
--rw-r--r--  2.0 unx     3500 b- defN 23-Feb-10 14:45 cog/director/monitor.py
--rw-r--r--  2.0 unx     3454 b- defN 23-Feb-10 14:45 cog/director/prediction_tracker.py
--rw-r--r--  2.0 unx     3716 b- defN 23-Feb-10 14:45 cog/director/redis.py
--rwxr-xr-x  2.0 unx      195 b- defN 23-Feb-10 14:45 cog/director/script/build
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-10 14:45 cog/server/__init__.py
--rw-r--r--  2.0 unx      593 b- defN 23-Feb-10 14:45 cog/server/eventtypes.py
--rw-r--r--  2.0 unx      149 b- defN 23-Feb-10 14:45 cog/server/exceptions.py
--rw-r--r--  2.0 unx     5334 b- defN 23-Feb-10 14:45 cog/server/helpers.py
--rw-r--r--  2.0 unx    11394 b- defN 23-Feb-10 14:45 cog/server/http.py
--rw-r--r--  2.0 unx      950 b- defN 23-Feb-10 14:45 cog/server/probes.py
--rw-r--r--  2.0 unx    20694 b- defN 23-Feb-10 14:45 cog/server/redis_queue.py
--rw-r--r--  2.0 unx      650 b- defN 23-Feb-10 14:45 cog/server/response_throttler.py
--rw-r--r--  2.0 unx    12462 b- defN 23-Feb-10 14:45 cog/server/runner.py
--rw-r--r--  2.0 unx     3092 b- defN 23-Feb-10 14:45 cog/server/webhook.py
--rw-r--r--  2.0 unx     7765 b- defN 23-Feb-10 14:45 cog/server/worker.py
--rw-r--r--  2.0 unx    11347 b- defN 23-Feb-10 14:47 cog-0.7.0b9.dist-info/LICENSE
--rw-r--r--  2.0 unx    32941 b- defN 23-Feb-10 14:47 cog-0.7.0b9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-10 14:47 cog-0.7.0b9.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Feb-10 14:47 cog-0.7.0b9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3166 b- defN 23-Feb-10 14:47 cog-0.7.0b9.dist-info/RECORD
-41 files, 176640 bytes uncompressed, 55382 bytes compressed:  68.6%
+Zip file size: 41602 bytes, number of entries: 28
+-rw-r--r--  2.0 unx       13 b- defN 23-May-05 18:16 cog/.gitignore
+-rw-r--r--  2.0 unx      362 b- defN 23-May-05 18:16 cog/__init__.py
+-rw-r--r--  2.0 unx      160 b- defN 23-May-05 18:18 cog/_version.py
+-rw-r--r--  2.0 unx      286 b- defN 23-May-05 18:16 cog/errors.py
+-rw-r--r--  2.0 unx     2066 b- defN 23-May-05 18:16 cog/files.py
+-rw-r--r--  2.0 unx     1973 b- defN 23-May-05 18:16 cog/json.py
+-rw-r--r--  2.0 unx     3130 b- defN 23-May-05 18:16 cog/logging.py
+-rw-r--r--  2.0 unx    11025 b- defN 23-May-05 18:16 cog/predictor.py
+-rw-r--r--  2.0 unx     2385 b- defN 23-May-05 18:16 cog/schema.py
+-rw-r--r--  2.0 unx      645 b- defN 23-May-05 18:16 cog/suppress_output.py
+-rw-r--r--  2.0 unx     7206 b- defN 23-May-05 18:16 cog/types.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 18:16 cog/command/__init__.py
+-rw-r--r--  2.0 unx      781 b- defN 23-May-05 18:16 cog/command/openapi_schema.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 18:16 cog/server/__init__.py
+-rw-r--r--  2.0 unx      593 b- defN 23-May-05 18:16 cog/server/eventtypes.py
+-rw-r--r--  2.0 unx      149 b- defN 23-May-05 18:16 cog/server/exceptions.py
+-rw-r--r--  2.0 unx     5334 b- defN 23-May-05 18:16 cog/server/helpers.py
+-rw-r--r--  2.0 unx    11733 b- defN 23-May-05 18:16 cog/server/http.py
+-rw-r--r--  2.0 unx      950 b- defN 23-May-05 18:16 cog/server/probes.py
+-rw-r--r--  2.0 unx      650 b- defN 23-May-05 18:16 cog/server/response_throttler.py
+-rw-r--r--  2.0 unx    14135 b- defN 23-May-05 18:16 cog/server/runner.py
+-rw-r--r--  2.0 unx     3092 b- defN 23-May-05 18:16 cog/server/webhook.py
+-rw-r--r--  2.0 unx     7954 b- defN 23-May-05 18:16 cog/server/worker.py
+-rw-r--r--  2.0 unx    11347 b- defN 23-May-05 18:18 cog-0.7.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    34222 b- defN 23-May-05 18:18 cog-0.7.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 18:18 cog-0.7.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-May-05 18:18 cog-0.7.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2095 b- defN 23-May-05 18:18 cog-0.7.1.dist-info/RECORD
+28 files, 122382 bytes uncompressed, 38312 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -33,50 +33,14 @@
 
 Filename: cog/command/__init__.py
 Comment: 
 
 Filename: cog/command/openapi_schema.py
 Comment: 
 
-Filename: cog/director/Dockerfile
-Comment: 
-
-Filename: cog/director/__init__.py
-Comment: 
-
-Filename: cog/director/__main__.py
-Comment: 
-
-Filename: cog/director/cloudbuild.yaml
-Comment: 
-
-Filename: cog/director/director.py
-Comment: 
-
-Filename: cog/director/eventtypes.py
-Comment: 
-
-Filename: cog/director/healthchecker.py
-Comment: 
-
-Filename: cog/director/http.py
-Comment: 
-
-Filename: cog/director/monitor.py
-Comment: 
-
-Filename: cog/director/prediction_tracker.py
-Comment: 
-
-Filename: cog/director/redis.py
-Comment: 
-
-Filename: cog/director/script/build
-Comment: 
-
 Filename: cog/server/__init__.py
 Comment: 
 
 Filename: cog/server/eventtypes.py
 Comment: 
 
 Filename: cog/server/exceptions.py
@@ -87,38 +51,35 @@
 
 Filename: cog/server/http.py
 Comment: 
 
 Filename: cog/server/probes.py
 Comment: 
 
-Filename: cog/server/redis_queue.py
-Comment: 
-
 Filename: cog/server/response_throttler.py
 Comment: 
 
 Filename: cog/server/runner.py
 Comment: 
 
 Filename: cog/server/webhook.py
 Comment: 
 
 Filename: cog/server/worker.py
 Comment: 
 
-Filename: cog-0.7.0b9.dist-info/LICENSE
+Filename: cog-0.7.1.dist-info/LICENSE
 Comment: 
 
-Filename: cog-0.7.0b9.dist-info/METADATA
+Filename: cog-0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: cog-0.7.0b9.dist-info/WHEEL
+Filename: cog-0.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: cog-0.7.0b9.dist-info/top_level.txt
+Filename: cog-0.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: cog-0.7.0b9.dist-info/RECORD
+Filename: cog-0.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cog/__init__.py

```diff
@@ -1,19 +1,20 @@
 from pydantic import BaseModel
 
 from .predictor import BasePredictor
-from .types import File, Input, Path
+from .types import File, Input, Path, ConcatenateIterator
 
 try:
     from ._version import __version__
 except ImportError:
     __version__ = "0.0.0+unknown"
 
 
 __all__ = [
     "__version__",
     "BaseModel",
     "BasePredictor",
+    "ConcatenateIterator",
     "File",
     "Input",
     "Path",
 ]
```

## cog/_version.py

```diff
@@ -1,4 +1,4 @@
 # file generated by setuptools_scm
 # don't change, don't track in version control
-__version__ = version = '0.7.0b9'
-__version_tuple__ = version_tuple = (0, 7, 0)
+__version__ = version = '0.7.1'
+__version_tuple__ = version_tuple = (0, 7, 1)
```

## cog/predictor.py

```diff
@@ -1,42 +1,103 @@
 from abc import ABC, abstractmethod
 from collections.abc import Iterator
 import enum
 import importlib.util
 import inspect
+import io
 import os.path
 from pathlib import Path
 from pydantic import create_model, BaseModel, Field
 from pydantic.fields import FieldInfo
-from typing import Any, Callable, Dict, List, Type
+from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 # Added in Python 3.8. Can be from typing if we drop support for <3.8.
 from typing_extensions import get_origin, get_args, Annotated
 import yaml
 
 from .errors import ConfigDoesNotExist, PredictorNotSet
-from .types import Input, Path as CogPath, File as CogFile, URLPath
+from .types import (
+    Input,
+    Path as CogPath,
+    File as CogFile,
+    URLFile,
+    URLPath,
+    get_filename,
+)
 
 
 ALLOWED_INPUT_TYPES = [str, int, float, bool, CogFile, CogPath]
 
 
 class BasePredictor(ABC):
-    def setup(self) -> None:
+    def setup(self, weights: Optional[Union[CogFile, CogPath]] = None) -> None:
         """
         An optional method to prepare the model so multiple predictions run efficiently.
         """
 
     @abstractmethod
     def predict(self, **kwargs: Any) -> Any:
         """
         Run a single prediction on the model
         """
 
 
+def run_setup(predictor: BasePredictor) -> None:
+    weights_type = get_weights_type(predictor.setup)
+
+    # No weights need to be passed, so just run setup() without any arguments.
+    if weights_type is None:
+        predictor.setup()
+        return
+
+    weights: Union[io.IOBase, Path, None]
+
+    weights_url = os.environ.get("COG_WEIGHTS")
+    weights_path = "weights"
+
+    # TODO: Cog{File,Path}.validate(...) methods accept either "real"
+    # paths/files or URLs to those things. In future we can probably tidy this
+    # up a little bit.
+    if weights_url:
+        if weights_type == CogFile:
+            weights = CogFile.validate(weights_url)
+        elif weights_type == CogPath:
+            weights = CogPath.validate(weights_url)
+        else:
+            raise ValueError(
+                f"Predictor.setup() has an argument 'weights' of type {weights_type}, but only File and Path are supported"
+            )
+    elif os.path.exists(weights_path):
+        if weights_type == CogFile:
+            weights = open(weights_path, "rb")
+        elif weights_type == CogPath:
+            weights = CogPath(weights_path)
+        else:
+            raise ValueError(
+                f"Predictor.setup() has an argument 'weights' of type {weights_type}, but only File and Path are supported"
+            )
+    else:
+        weights = None
+
+    predictor.setup(weights=weights)
+
+
+def get_weights_type(setup_function) -> Optional[Any]:
+    signature = inspect.signature(setup_function)
+    if "weights" not in signature.parameters:
+        return None
+    Type = signature.parameters["weights"].annotation
+    # Handle Optional. It is Union[Type, None]
+    if get_origin(Type) == Union:
+        args = get_args(Type)
+        if len(args) == 2 and args[1] is type(None):
+            Type = get_args(Type)[0]
+    return Type
+
+
 def run_prediction(
     predictor: BasePredictor, inputs: Dict[Any, Any], cleanup_functions: List[Callable]
 ) -> Any:
     """
     Run the predictor on the inputs, and append resulting paths
     to cleanup functions for removal.
     """
@@ -68,33 +129,39 @@
     Constructs an instance of the user-defined Predictor class from a config.
     """
 
     ref = get_predictor_ref(config)
     return load_predictor_from_ref(ref)
 
 
-def get_predictor_ref(config: Dict[str, Any]) -> str:
-    if "predict" not in config:
+def get_predictor_ref(config: Dict[str, Any], mode: str = "predict") -> str:
+    if mode not in ["predict", "train"]:
+        raise ValueError(f"Invalid mode: {mode}")
+
+    if mode not in config:
         raise PredictorNotSet(
-            "Can't run predictions: 'predict' option not found in cog.yaml"
+            f"Can't run predictions: '{mode}' option not found in cog.yaml"
         )
 
-    return config["predict"]
+    return config[mode]
 
 
 def load_predictor_from_ref(ref: str) -> BasePredictor:
     module_path, class_name = ref.split(":", 1)
     module_name = os.path.basename(module_path).split(".py", 1)[0]
     spec = importlib.util.spec_from_file_location(module_name, module_path)
     assert spec is not None
     module = importlib.util.module_from_spec(spec)
     assert spec.loader is not None
     spec.loader.exec_module(module)
-    predictor_class = getattr(module, class_name)
-    return predictor_class()
+    predictor = getattr(module, class_name)
+    # It could be a class or a function
+    if inspect.isclass(predictor):
+        return predictor()
+    return predictor
 
 
 # Base class for inputs, constructed dynamically in get_input_type().
 # (This can't be a docstring or it gets passed through to the schema.)
 class BaseInput(BaseModel):
     class Config:
         # When using `choices`, the type is converted into an enum to validate
@@ -113,29 +180,36 @@
             # but both have an unlink() method, so may as well be safe.
             elif isinstance(value, Path):
                 # This could be missing_ok=True when we drop support for Python 3.7
                 if value.exists():
                     value.unlink()
 
 
+def get_predict(predictor):
+    if hasattr(predictor, "predict"):
+        return predictor.predict
+    return predictor
+
+
 def get_input_type(predictor: BasePredictor) -> Type[BaseInput]:
     """
     Creates a Pydantic Input model from the arguments of a Predictor's predict() method.
 
     class Predictor(BasePredictor):
         def predict(self, text: str):
             ...
 
     programmatically creates a model like this:
 
     class Input(BaseModel):
         text: str
     """
 
-    signature = inspect.signature(predictor.predict)
+    predict = get_predict(predictor)
+    signature = inspect.signature(predict)
     create_model_kwargs = {}
 
     order = 0
 
     for name, parameter in signature.parameters.items():
         InputType = parameter.annotation
 
@@ -194,16 +268,16 @@
     )
 
 
 def get_output_type(predictor: BasePredictor) -> Type[BaseModel]:
     """
     Creates a Pydantic Output model from the return type annotation of a Predictor's predict() method.
     """
-
-    signature = inspect.signature(predictor.predict)
+    predict = get_predict(predictor)
+    signature = inspect.signature(predict)
     if signature.return_annotation is inspect.Signature.empty:
         raise TypeError(
             """You must set an output type. If your model can return multiple output types, you can explicitly set `Any` as the output type.
 
 For example:
 
     from typing import Any
```

## cog/types.py

```diff
@@ -2,15 +2,15 @@
 import mimetypes
 import os
 import base64
 import pathlib
 import requests
 import shutil
 import tempfile
-from typing import Any, Callable, Dict, Iterator, List, Union
+from typing import Any, Callable, Dict, Iterator, List, TypeVar, Union
 from urllib.parse import urlparse
 
 from pydantic import Field
 from pydantic.typing import NoArgAnyCallable
 
 
 def Input(
@@ -200,7 +200,33 @@
         header, _ = parsed_url.path.split(",", 1)
         mime_type, _ = header.split(";", 1)
         extension = mimetypes.guess_extension(mime_type)
         if extension is None:
             return "file"
         return "file" + extension
     return os.path.basename(parsed_url.path)
+
+
+Item = TypeVar("Item")
+
+
+class ConcatenateIterator(Iterator[Item]):
+    @classmethod
+    def __modify_schema__(cls, field_schema: Dict[str, Any]) -> None:
+        """Defines what this type should be in openapi.json"""
+        field_schema.pop("allOf", None)
+        field_schema.update(
+            {
+                "type": "array",
+                "items": {"type": "string"},
+                "x-cog-array-type": "iterator",
+                "x-cog-array-display": "concatenate",
+            }
+        )
+
+    @classmethod
+    def __get_validators__(cls) -> Iterator[Any]:
+        yield cls.validate
+
+    @classmethod
+    def validate(cls, value: Any) -> Iterator:
+        return value
```

## cog/command/openapi_schema.py

```diff
@@ -12,17 +12,14 @@
 from ..server.http import create_app
 
 if __name__ == "__main__":
     schema = {}
     try:
         with suppress_output():
             config = load_config()
-            predictor_ref = get_predictor_ref(config)
+            app = create_app(config, shutdown_event=None)
+            schema = app.openapi()
     except (ConfigDoesNotExist, PredictorNotSet):
         # If there is no cog.yaml or 'predict' has not been set, then there is no type signature.
         # Not an error, there just isn't anything.
         pass
-    else:
-        with suppress_output():
-            app = create_app(predictor_ref, shutdown_event=None)
-        schema = app.openapi()
     print(json.dumps(schema, indent=2))
```

## cog/server/http.py

```diff
@@ -1,15 +1,15 @@
 import argparse
 import logging
 import os
 import signal
 import textwrap
 import threading
 from datetime import datetime, timezone
-from typing import Any, Callable, Optional, Union
+from typing import Any, Callable, Dict, Optional, Union
 
 import structlog
 import uvicorn
 from anyio import CapacityLimiter
 from anyio.lowlevel import RunVar
 from enum import Enum, auto, unique
 from fastapi import Body, FastAPI, Header, HTTPException, Path, Response
@@ -26,15 +26,14 @@
 from ..predictor import (
     get_input_type,
     get_output_type,
     get_predictor_ref,
     load_config,
     load_predictor_from_ref,
 )
-from .probes import ProbeHelper
 from .runner import PredictionRunner, RunnerBusyError, UnknownPredictionError
 
 log = structlog.get_logger("cog.server.http")
 
 
 @unique
 class Health(Enum):
@@ -42,26 +41,30 @@
     STARTING = auto()
     READY = auto()
     BUSY = auto()
     SETUP_FAILED = auto()
 
 
 def create_app(
-    predictor_ref: str,
+    config: Dict[str, Any],
     shutdown_event: threading.Event,
     threads: int = 1,
     upload_url: Optional[str] = None,
+    mode: str = "predict",
 ) -> FastAPI:
     app = FastAPI(
         title="Cog",  # TODO: mention model name?
         # version=None # TODO
     )
 
     app.state.health = Health.STARTING
     app.state.setup_result = None
+    app.state.setup_result_payload = None
+
+    predictor_ref = get_predictor_ref(config, mode)
 
     runner = PredictionRunner(
         predictor_ref=predictor_ref,
         shutdown_event=shutdown_event,
         upload_url=upload_url,
     )
     # TODO: avoid loading predictor code in this process
@@ -76,32 +79,15 @@
     )
 
     @app.on_event("startup")
     def startup() -> None:
         # https://github.com/tiangolo/fastapi/issues/4221
         RunVar("_default_thread_limiter").set(CapacityLimiter(threads))  # type: ignore
 
-        setup_start = datetime.now(timezone.utc)
-        setup_status, setup_logs = runner.setup()
-        setup_complete = datetime.now(timezone.utc)
-
-        app.state.setup_result = {
-            "logs": setup_logs,
-            "status": setup_status,
-            "started_at": setup_start,
-            "completed_at": setup_complete,
-        }
-
-        if setup_status == schema.Status.SUCCEEDED:
-            app.state.health = Health.READY
-        else:
-            app.state.health = Health.SETUP_FAILED
-
-        probes = ProbeHelper()
-        probes.ready()
+        app.state.setup_result = runner.setup()
 
     @app.on_event("shutdown")
     def shutdown() -> None:
         runner.shutdown()
 
     @app.get("/")
     def root() -> Any:
@@ -109,22 +95,23 @@
             # "cog_version": "", # TODO
             "docs_url": "/docs",
             "openapi_url": "/openapi.json",
         }
 
     @app.get("/health-check")
     def healthcheck() -> Any:
+        _check_setup_result()
         if app.state.health == Health.READY:
             health = Health.BUSY if runner.is_busy() else Health.READY
         else:
             health = app.state.health
         return jsonable_encoder(
             {
                 "status": health.name,
-                "setup": app.state.setup_result,
+                "setup": app.state.setup_result_payload,
             }
         )
 
     @app.post(
         "/predictions",
         response_model=PredictionResponse,
         response_model_exclude_unset=True,
@@ -237,14 +224,33 @@
 
     @app.post("/shutdown")
     def start_shutdown() -> Any:
         log.info("shutdown requested via http")
         shutdown_event.set()
         return JSONResponse({}, status_code=200)
 
+    def _check_setup_result() -> Any:
+        if app.state.setup_result is None:
+            return
+
+        if not app.state.setup_result.ready():
+            return
+
+        result = app.state.setup_result.get()
+
+        if result["status"] == schema.Status.SUCCEEDED:
+            app.state.health = Health.READY
+        else:
+            app.state.health = Health.SETUP_FAILED
+
+        app.state.setup_result_payload = result
+
+        # Reset app.state.setup_result so future calls are a no-op
+        app.state.setup_result = None
+
     return app
 
 
 def _log_invalid_output(error: Any) -> None:
     log.error(
         textwrap.dedent(
             f"""\
@@ -314,14 +320,22 @@
     parser.add_argument(
         "--await-explicit-shutdown",
         dest="await_explicit_shutdown",
         type=bool,
         default=False,
         help="Ignore SIGTERM and wait for a request to /shutdown (or a SIGINT) before exiting",
     )
+    parser.add_argument(
+        "--x-mode",
+        dest="mode",
+        type=str,
+        default="predict",
+        choices=["predict", "train"],
+        help="Experimental: Run in 'predict' or 'train' mode",
+    )
     args = parser.parse_args()
 
     # log level is configurable so we can make it quiet or verbose for `cog predict`
     # cog predict --debug       # -> debug
     # cog predict               # -> warning
     # docker run <image-name>   # -> info (default)
     log_level = logging.getLevelName(os.environ.get("COG_LOG_LEVEL", "INFO").upper())
@@ -333,20 +347,20 @@
     if threads is None:
         if config.get("build", {}).get("gpu", False):
             threads = 1
         else:
             threads = os.cpu_count()
 
     shutdown_event = threading.Event()
-    predictor_ref = get_predictor_ref(config)
     app = create_app(
-        predictor_ref=predictor_ref,
+        config=config,
         shutdown_event=shutdown_event,
         threads=threads,
         upload_url=args.upload_url,
+        mode=args.mode,
     )
 
     port = int(os.getenv("PORT", 5000))
     server_config = uvicorn.Config(
         app,
         host="0.0.0.0",
         port=port,
```

## cog/server/runner.py

```diff
@@ -12,14 +12,15 @@
 from requests.packages.urllib3.util.retry import Retry  # type: ignore
 
 from .. import schema
 from .. import types
 from ..files import put_file_to_signed_endpoint
 from ..json import upload_files
 from .eventtypes import Done, Heartbeat, Log, PredictionOutput, PredictionOutputType
+from .probes import ProbeHelper
 from .webhook import webhook_caller_filtered
 from .worker import Worker
 
 log = structlog.get_logger("cog.server.runner")
 
 
 class FileUploadError(Exception):
@@ -50,41 +51,46 @@
 
         self._worker = Worker(predictor_ref=predictor_ref)
         self._should_cancel = threading.Event()
 
         self._shutdown_event = shutdown_event
         self._upload_url = upload_url
 
-    def setup(self) -> Tuple[schema.Status, str]:
-        _logs = []
-        _status = None
-
-        try:
-            for event in self._worker.setup():
-                if isinstance(event, Log):
-                    _logs.append(event.message)
-                elif isinstance(event, Done):
-                    _status = (
-                        schema.Status.FAILED if event.error else schema.Status.SUCCEEDED
-                    )
-        except Exception:
-            _status = schema.Status.FAILED
+    def setup(self) -> AsyncResult:
+        if self.is_busy():
+            raise RunnerBusyError()
 
-        assert _status is not None, "must receive done event from setup"
+        def handle_error(error: BaseException) -> None:
+            # Re-raise the exception in order to more easily capture exc_info,
+            # and then trigger shutdown, as we have no easy way to resume
+            # worker state if an exception was thrown.
+            try:
+                raise error
+            except Exception:
+                log.error("caught exception while running setup", exc_info=True)
+                self._shutdown_event.set()
 
-        return (_status, "".join(_logs))
+        self._result = self._threadpool.apply_async(
+            func=setup,
+            kwds={"worker": self._worker},
+            error_callback=handle_error,
+        )
+        return self._result
 
     # TODO: Make the return type AsyncResult[schema.PredictionResponse] when we
     # no longer have to support Python 3.8
     def predict(
         self, prediction: schema.PredictionRequest, upload: bool = True
     ) -> Tuple[schema.PredictionResponse, AsyncResult]:
         # It's the caller's responsibility to not call us if we're busy.
         if self.is_busy():
-            assert self._response is not None
+            # If self._result is set, but self._response is not, we're still
+            # doing setup.
+            if self._response is None:
+                raise RunnerBusyError()
             assert self._result is not None
             if prediction.id is not None and prediction.id == self._response.id:
                 return (self._response, self._result)
             raise RunnerBusyError()
 
         # Set up logger context for main thread. The same thing happens inside
         # the predict thread.
@@ -272,14 +278,50 @@
         except Exception as error:
             # If something goes wrong uploading a file, it's irrecoverable.
             # The re-raised exception will be caught and cause the prediction
             # to be failed, with a useful error message.
             raise FileUploadError("Got error trying to upload output files") from error
 
 
+def setup(*, worker: Worker):
+    logs = []
+    status = None
+    started_at = datetime.now(tz=timezone.utc)
+
+    try:
+        for event in worker.setup():
+            if isinstance(event, Log):
+                logs.append(event.message)
+            elif isinstance(event, Done):
+                status = (
+                    schema.Status.FAILED if event.error else schema.Status.SUCCEEDED
+                )
+    except Exception:
+        logs.append(traceback.format_exc())
+        status = schema.Status.FAILED
+
+    if status is None:
+        logs.append("Error: did not receive 'done' event from setup!")
+        status = schema.Status.FAILED
+
+    completed_at = datetime.now(tz=timezone.utc)
+
+    # Only if setup succeeded, mark the container as "ready".
+    if status == schema.Status.SUCCEEDED:
+        probes = ProbeHelper()
+        probes.ready()
+
+    return {
+        "logs": "".join(logs),
+        "status": status,
+        "started_at": started_at,
+        "completed_at": completed_at,
+    }
+
+
 def predict(
     *,
     worker: Worker,
     request: schema.PredictionRequest,
     event_handler: PredictionEventHandler,
     should_cancel: threading.Event,
 ) -> schema.PredictionResponse:
@@ -312,15 +354,22 @@
     initial_prediction = request.dict()
 
     output_type = None
     input_dict = initial_prediction["input"]
 
     for k, v in input_dict.items():
         if isinstance(v, types.URLPath):
-            input_dict[k] = v.convert()
+            try:
+                input_dict[k] = v.convert()
+            except requests.exceptions.RequestException as e:
+                tb = traceback.format_exc()
+                event_handler.append_logs(tb)
+                event_handler.failed(error=str(e))
+                log.warn("failed to download url path from input", exc_info=True)
+                return event_handler.response
 
     for event in worker.predict(input_dict, poll=0.1):
         if should_cancel.is_set():
             worker.cancel()
             should_cancel.clear()
 
         if isinstance(event, Heartbeat):
```

## cog/server/worker.py

```diff
@@ -5,15 +5,15 @@
 import traceback
 import types
 from enum import Enum, auto, unique
 from multiprocessing.connection import Connection
 from typing import Any, Dict, Iterable, Optional, TextIO, Union
 
 from ..json import make_encodeable
-from ..predictor import BasePredictor, load_predictor_from_ref
+from ..predictor import BasePredictor, load_predictor_from_ref, get_predict, run_setup
 from .eventtypes import (
     Done,
     Heartbeat,
     Log,
     PredictionInput,
     PredictionOutput,
     PredictionOutputType,
@@ -119,15 +119,15 @@
             yield ev
 
             if isinstance(ev, Done):
                 done = ev
 
         if done:
             if done.error and raise_on_error:
-                raise FatalWorkerException(raise_on_error)
+                raise FatalWorkerException(raise_on_error + ": " + done.error_detail)
             else:
                 self._state = WorkerState.READY
                 self._allow_cancel = False
 
         # If we dropped off the end off the end of the loop, check if it's
         # because the child process died.
         if not self._child.is_alive() and not self._terminating:
@@ -176,15 +176,17 @@
 
         self._stream_redirector.shutdown()
 
     def _setup(self) -> None:
         done = Done()
         try:
             self._predictor = load_predictor_from_ref(self._predictor_ref)
-            self._predictor.setup()
+            # Could be a function or a class
+            if hasattr(self._predictor, "setup"):
+                run_setup(self._predictor)
         except Exception as e:
             traceback.print_exc()
             done.error = True
             done.error_detail = str(e)
         except BaseException as e:
             # For SystemExit and friends we attempt to add some useful context
             # to the logs, but reraise to ensure the process dies.
@@ -207,15 +209,17 @@
                 print(f"Got unexpected event: {ev}", file=sys.stderr)
 
     def _predict(self, payload: Dict[str, Any]) -> None:
         assert self._predictor
         done = Done()
         self._cancelable = True
         try:
-            result = self._predictor.predict(**payload)
+            predict = get_predict(self._predictor)
+            result = predict(**payload)
+
             if result:
                 if isinstance(result, types.GeneratorType):
                     self._events.send(PredictionOutputType(multi=True))
                     for r in result:
                         self._events.send(PredictionOutput(payload=make_encodeable(r)))
                 else:
                     self._events.send(PredictionOutputType(multi=False))
```

## Comparing `cog-0.7.0b9.dist-info/LICENSE` & `cog-0.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cog-0.7.0b9.dist-info/METADATA` & `cog-0.7.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog
-Version: 0.7.0b9
+Version: 0.7.1
 Summary: Containers for machine learning
 Author-email: Replicate <team@replicate.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -208,20 +208,16 @@
         
 Project-URL: Source, https://github.com/replicate/cog
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs (<23,>=20.1)
 Requires-Dist: fastapi (<1,>=0.75.2)
-Requires-Dist: opentelemetry-exporter-otlp (<2,>=1.11.1)
-Requires-Dist: opentelemetry-sdk (<2,>=1.11.1)
-Requires-Dist: protobuf (<=3.20.3)
 Requires-Dist: pydantic (<2,>=1.9)
 Requires-Dist: PyYAML
-Requires-Dist: redis (<5,>=4)
 Requires-Dist: requests (<3,>=2)
 Requires-Dist: structlog (<23,>=20)
 Requires-Dist: typing-extensions (>=4.1.0)
 Requires-Dist: uvicorn[standard] (<1,>=0.12)
 
 # Cog: Containers for machine learning
 
@@ -370,15 +366,14 @@
 - [Using Cog with notebooks](docs/notebooks.md)
 - [Using Cog with Windows 11](docs/wsl2/wsl2.md)
 - [Take a look at some examples of using Cog](https://github.com/replicate/cog-examples)
 - [Deploy models with Cog](docs/deploy.md)
 - [`cog.yaml` reference](docs/yaml.md) to learn how to define your model's environment
 - [Prediction interface reference](docs/python.md) to learn how the `Predictor` interface works
 - [HTTP API reference](docs/http.md) to learn how to use the HTTP API that models serve
-- [Redis queue API reference](docs/redis.md) to learn how to run models via Redis
 
 ## Need help?
 
 [Join us in #cog on Discord.](https://discord.gg/replicate)
 
 ## Contributors ✨
 
@@ -424,14 +419,18 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/afiaka87"><img src="https://avatars.githubusercontent.com/u/3994972?v=4?s=100" width="100px;" alt="Clay Mullis"/><br /><sub><b>Clay Mullis</b></sub></a><br /><a href="https://github.com/replicate/cog/commits?author=afiaka87" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/mattt"><img src="https://avatars.githubusercontent.com/u/7659?v=4?s=100" width="100px;" alt="Mattt"/><br /><sub><b>Mattt</b></sub></a><br /><a href="https://github.com/replicate/cog/commits?author=mattt" title="Code">💻</a> <a href="https://github.com/replicate/cog/commits?author=mattt" title="Documentation">📖</a> <a href="#infra-mattt" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Juneezee"><img src="https://avatars.githubusercontent.com/u/20135478?v=4?s=100" width="100px;" alt="Eng Zer Jun"/><br /><sub><b>Eng Zer Jun</b></sub></a><br /><a href="https://github.com/replicate/cog/commits?author=Juneezee" title="Tests">⚠️</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/bbedward"><img src="https://avatars.githubusercontent.com/u/550752?v=4?s=100" width="100px;" alt="BB"/><br /><sub><b>BB</b></sub></a><br /><a href="https://github.com/replicate/cog/commits?author=bbedward" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/williamluer"><img src="https://avatars.githubusercontent.com/u/85975676?v=4?s=100" width="100px;" alt="williamluer"/><br /><sub><b>williamluer</b></sub></a><br /><a href="https://github.com/replicate/cog/commits?author=williamluer" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://sirupsen.com"><img src="https://avatars.githubusercontent.com/u/97400?v=4?s=100" width="100px;" alt="Simon Eskildsen"/><br /><sub><b>Simon Eskildsen</b></sub></a><br /><a href="https://github.com/replicate/cog/commits?author=sirupsen" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://erbridge.co.uk"><img src="https://avatars.githubusercontent.com/u/1027364?v=4?s=100" width="100px;" alt="F"/><br /><sub><b>F</b></sub></a><br /><a href="https://github.com/replicate/cog/issues?q=author%3Aerbridge" title="Bug reports">🐛</a> <a href="https://github.com/replicate/cog/commits?author=erbridge" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/philandstuff"><img src="https://avatars.githubusercontent.com/u/581269?v=4?s=100" width="100px;" alt="Philip Potter"/><br /><sub><b>Philip Potter</b></sub></a><br /><a href="https://github.com/replicate/cog/issues?q=author%3Aphilandstuff" title="Bug reports">🐛</a> <a href="https://github.com/replicate/cog/commits?author=philandstuff" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/joannejchen"><img src="https://avatars.githubusercontent.com/u/33409024?v=4?s=100" width="100px;" alt="Joanne Chen"/><br /><sub><b>Joanne Chen</b></sub></a><br /><a href="https://github.com/replicate/cog/commits?author=joannejchen" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

