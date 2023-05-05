# Comparing `tmp/project_lighter-0.0.1.tar.gz` & `tmp/project_lighter-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_lighter-0.0.1.tar", max compression
+gzip compressed data, was "project_lighter-0.0.2a0.tar", max compression
```

## Comparing `project_lighter-0.0.1.tar` & `project_lighter-0.0.2a0.tar`

### file list

```diff
@@ -1,28 +1,20 @@
--rw-r--r--   0        0        0     1080 2023-01-24 00:45:56.220636 project_lighter-0.0.1/LICENSE
--rw-r--r--   0        0        0      485 2023-01-26 09:48:05.966439 project_lighter-0.0.1/README.md
--rw-r--r--   0        0        0       56 2023-01-27 14:28:21.068686 project_lighter-0.0.1/lighter/__init__.py
--rw-r--r--   0        0        0       35 2023-01-26 05:51:20.966136 project_lighter-0.0.1/lighter/callbacks/__init__.py
--rw-r--r--   0        0        0    16281 2023-01-26 05:55:46.564062 project_lighter-0.0.1/lighter/callbacks/logger.py
--rw-r--r--   0        0        0       43 2023-01-19 19:46:01.246798 project_lighter-0.0.1/lighter/contrib/.git
--rw-r--r--   0        0        0     1799 2023-01-19 19:46:01.246798 project_lighter-0.0.1/lighter/contrib/.gitignore
--rw-r--r--   0        0        0     1502 2023-01-19 19:46:01.246798 project_lighter-0.0.1/lighter/contrib/LICENSE
--rw-r--r--   0        0        0       55 2023-01-19 19:46:01.246798 project_lighter-0.0.1/lighter/contrib/README.md
--rw-r--r--   0        0        0        0 2023-01-19 19:46:01.246798 project_lighter-0.0.1/lighter/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-01-19 19:46:01.246798 project_lighter-0.0.1/lighter/contrib/models/__init__.py
--rw-r--r--   0        0        0     3645 2023-01-20 08:55:10.188166 project_lighter-0.0.1/lighter/contrib/models/swav.py
--rw-r--r--   0        0        0        0 2023-01-19 19:46:01.246798 project_lighter-0.0.1/lighter/contrib/optimizer/__init__.py
--rw-r--r--   0        0        0     1145 2023-01-20 08:55:10.124166 project_lighter-0.0.1/lighter/contrib/optimizer/utils.py
--rw-r--r--   0        0        0        0 2023-01-19 19:46:01.246798 project_lighter-0.0.1/lighter/contrib/transforms/__init__.py
--rw-r--r--   0        0        0     3146 2023-01-26 05:55:00.376426 project_lighter-0.0.1/lighter/contrib/transforms/sitk.py
--rw-r--r--   0        0        0     1974 2023-01-20 08:55:10.124166 project_lighter-0.0.1/lighter/contrib/transforms/ssl.py
--rw-r--r--   0        0        0        0 2023-01-19 19:46:01.254798 project_lighter-0.0.1/lighter/contrib/utils/__init__.py
--rw-r--r--   0        0        0    16655 2023-01-26 14:03:29.989102 project_lighter-0.0.1/lighter/system.py
--rw-r--r--   0        0        0        0 2023-01-20 08:09:33.734298 project_lighter-0.0.1/lighter/utils/__init__.py
--rw-r--r--   0        0        0     3411 2023-01-26 05:53:17.413232 project_lighter-0.0.1/lighter/utils/cli.py
--rw-r--r--   0        0        0     1802 2023-01-20 08:09:33.734298 project_lighter-0.0.1/lighter/utils/collate.py
--rw-r--r--   0        0        0     1401 2023-01-24 00:45:56.220636 project_lighter-0.0.1/lighter/utils/dynamic_imports.py
--rw-r--r--   0        0        0     2184 2023-01-26 05:51:20.970136 project_lighter-0.0.1/lighter/utils/misc.py
--rw-r--r--   0        0        0     2415 2023-01-24 00:45:56.220636 project_lighter-0.0.1/lighter/utils/model.py
--rw-r--r--   0        0        0     4370 2023-01-27 14:36:01.833011 project_lighter-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1791 1970-01-01 00:00:00.000000 project_lighter-0.0.1/setup.py
--rw-r--r--   0        0        0     2111 1970-01-01 00:00:00.000000 project_lighter-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-05 21:09:25.315727 project_lighter-0.0.2a0/LICENSE
+-rw-r--r--   0        0        0      485 2023-05-05 21:09:25.315727 project_lighter-0.0.2a0/README.md
+-rw-r--r--   0        0        0       58 2023-05-05 21:11:47.209691 project_lighter-0.0.2a0/lighter/__init__.py
+-rw-r--r--   0        0        0      125 2023-05-05 21:09:25.315727 project_lighter-0.0.2a0/lighter/callbacks/__init__.py
+-rw-r--r--   0        0        0    13987 2023-05-05 21:09:25.315727 project_lighter-0.0.2a0/lighter/callbacks/logger.py
+-rw-r--r--   0        0        0     5784 2023-05-05 21:09:25.315727 project_lighter-0.0.2a0/lighter/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2023-05-05 21:09:25.315727 project_lighter-0.0.2a0/lighter/callbacks/writer/__init__.py
+-rw-r--r--   0        0        0     7593 2023-05-05 21:09:25.315727 project_lighter-0.0.2a0/lighter/callbacks/writer/base.py
+-rw-r--r--   0        0        0     2662 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/callbacks/writer/file.py
+-rw-r--r--   0        0        0     2427 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/callbacks/writer/table.py
+-rw-r--r--   0        0        0    21386 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/system.py
+-rw-r--r--   0        0        0       36 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/utils/__init__.py
+-rw-r--r--   0        0        0     3510 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/utils/cli.py
+-rw-r--r--   0        0        0     2352 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/utils/collate.py
+-rw-r--r--   0        0        0     1424 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/utils/dynamic_imports.py
+-rw-r--r--   0        0        0     3431 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/utils/freezer.py
+-rw-r--r--   0        0        0     2618 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/utils/misc.py
+-rw-r--r--   0        0        0     5881 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/utils/model.py
+-rw-r--r--   0        0        0     4400 2023-05-05 21:11:47.153690 project_lighter-0.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 project_lighter-0.0.2a0/PKG-INFO
```

### Comparing `project_lighter-0.0.1/LICENSE` & `project_lighter-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.1/lighter/callbacks/logger.py` & `project_lighter-0.0.2a0/lighter/callbacks/logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,40 @@
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, Union
 
-import re
 import sys
 from datetime import datetime
 from pathlib import Path
 
 import torch
-import torch.distributed as dist
-import torchvision
 from loguru import logger
 from monai.utils.module import optional_import
 from pytorch_lightning import Callback, Trainer
-from torch.utils import tensorboard
-from yaml import safe_load
 
 from lighter import LighterSystem
-
-LIGHTNING_TO_LIGHTER_STAGE = {"train": "train", "validate": "val", "test": "test"}
-OPTIONAL_IMPORTS = {}
+from lighter.callbacks.utils import get_lighter_mode, is_data_type_supported, parse_data, preprocess_image
+from lighter.utils.dynamic_imports import OPTIONAL_IMPORTS
 
 
 class LighterLogger(Callback):
     def __init__(
         self,
-        project,
-        log_dir,
-        tensorboard=False,
-        wandb=False,
-        input_type=None,
-        target_type=None,
-        pred_type=None,
-        max_samples=None,
+        project: str,
+        log_dir: str,
+        tensorboard: bool = False,
+        wandb: bool = False,
+        input_type: str = None,
+        target_type: str = None,
+        pred_type: str = None,
+        max_samples: int = None,
     ) -> None:
         self.project = project
         # Only used on rank 0, the dir is created in setup().
         self.log_dir = Path(log_dir) / project / datetime.now().strftime("%Y%m%d_%H%M%S")
 
-        self.data_types = {"input": input_type, "target": target_type, "pred": pred_type}
+        self.log_types = {"input": input_type, "target": target_type, "pred": pred_type}
         # Max number of samples from the batch to log.
         self.max_samples = max_samples
 
         self.tensorboard = tensorboard
         self.wandb = wandb
 
         # Running loss. Resets at each epoch. Loss is not calculated for `test` mode.
@@ -61,215 +55,238 @@
             pl_module (LighterSystem): LighterSystem, passed automatically by PyTorch Lightning.
             stage (str): stage of the training process. Passed automatically by PyTorch Lightning.
         """
         if trainer.logger is not None:
             logger.error("When using LighterLogger, set Trainer(logger=None).")
             sys.exit()
 
-        if dist.is_initialized() and dist.get_rank() != 0:
+        if not trainer.is_global_zero:
             return
 
         self.log_dir.mkdir(parents=True)
 
         # Load the dumped config file to log it to the loggers.
-        # config = safe_load(open(self.log_dir / "config.yaml"))
+        # config = yaml.safe_load(open(self.log_dir / "config.yaml"))
 
         # Loguru log file.
         # logger.add(sink=self.log_dir / f"{stage}.log")
 
         # Tensorboard initialization.
         if self.tensorboard:
+            # Tensorboard is a part of PyTorch, no need to check if it is not available.
+            OPTIONAL_IMPORTS["tensorboard"], _ = optional_import("torch.utils.tensorboard")
             tensorboard_dir = self.log_dir / "tensorboard"
             tensorboard_dir.mkdir()
-            self.tensorboard = tensorboard.SummaryWriter(log_dir=tensorboard_dir)
+            self.tensorboard = OPTIONAL_IMPORTS["tensorboard"].SummaryWriter(log_dir=tensorboard_dir)
             # self.tensorboard.add_hparams(config)
 
         # Wandb initialization.
         if self.wandb:
             OPTIONAL_IMPORTS["wandb"], wandb_available = optional_import("wandb")
             if not wandb_available:
                 logger.error("Weights & Biases not installed. To install it, run `pip install wandb`. Exiting.")
                 sys.exit()
             wandb_dir = self.log_dir / "wandb"
             wandb_dir.mkdir()
             self.wandb = OPTIONAL_IMPORTS["wandb"].init(project=self.project, dir=wandb_dir)
             # self.wandb.config.update(config)
 
     def teardown(self, trainer: Trainer, pl_module: LighterSystem, stage: str) -> None:
-        if dist.is_initialized() and dist.get_rank() != 0:
+        if not trainer.is_global_zero:
             return
-        self.tensorboard.close()
+        if self.tensorboard:
+            self.tensorboard.close()
 
-    def _log(self, outputs: dict, mode: str, global_step: int, is_epoch=False) -> None:
-        """Logs the outputs to TensorBoard and Weights & Biases (if enabled).
-        The outputs are logged as scalars and images, depending on the configuration.
+    def _log_by_type(self, name: str, data: Any, log_type: str, global_step: int) -> None:
+        """Logs data according to the specified type.
 
         Args:
-            outputs (dict): model outputs.
-            mode (str): current mode (train/val/test).
+            name (str): name of the data being logged.
+            data (Any): data to be logged.
+            log_type (str): type of the data. Supported types are 'scalar', 'image', and 'histogram'.
             global_step (int): current global step.
-            is_epoch (bool): whether the log is being done at the end
-                of an epoch or astep. Default is False.
-        """
-        if dist.is_initialized() and dist.get_rank() != 0:
-            return
-
-        step_or_epoch = "epoch" if is_epoch else "step"
-
-        # Loss
-        if outputs["loss"] is not None:
-            name = f"{mode}/loss/{step_or_epoch}"
-            self._log_scalar(name, outputs["loss"], global_step)
-
-        # Metrics
-        if outputs["metrics"] is not None:
-            for name, metric in outputs["metrics"].items():
-                name = f"{mode}/metrics/{name}_{step_or_epoch}"
-                self._log_scalar(name, metric, global_step)
 
-        # Epoch does not log input, target, and pred.
-        if is_epoch:
-            return
+        Raises:
+            TypeError: if the specified `log_type` is not supported.
+        """
+        # Log scalar
+        if log_type == "scalar":
+            self._log_scalar(name, data, global_step)
+
+        # Log image
+        elif log_type == "image":
+            # Slice to `max_samples` only if it less than the batch size.
+            if self.max_samples is not None and self.max_samples < data.shape[0]:
+                data = data[: self.max_samples]
+            # Preprocess a batch of images into a single, loggable, image.
+            data = preprocess_image(data)
+            self._log_image(name, data, global_step)
+
+        # Log histogram
+        elif log_type == "histogram":
+            self._log_histogram(name, data, global_step)
 
-        # Input, Target, Pred
-        for data_name in ["input", "target", "pred"]:
-            if self.data_types[data_name] is None:
-                continue
-
-            data_type = self.data_types[data_name]
-            data = outputs[data_name]
-            name = f"{mode}/data/{data_name}_{step_or_epoch}"
-
-            # Scalar
-            if data_type == "scalar":
-                self._log_scalar(name, data, global_step)
-
-            # Image
-            elif data_type == "image":
-                # Check if the data type is valid.
-                check_image_data_type(data, data_name)
-                for identifier, image in parse_image_data(data):
-                    name = name if identifier is None else f"{name}_{identifier}"
-                    # Slice to `max_samples` only if it less than the batch size.
-                    if self.max_samples is not None and self.max_samples < image.shape[0]:
-                        image = image[: self.max_samples]
-                    # Preprocess a batch of images into a single, loggable, image.
-                    image = preprocess_image(image)
-                    self._log_image(name, image, global_step)
-            else:
-                logger.error(f"`{data_name}_type` does not support `{data_type}`.")
-                sys.exit()
+        else:
+            raise TypeError(f"`{log_type}` not supported for logging.")
 
     def _log_scalar(self, name: str, scalar: Union[int, float, torch.Tensor], global_step: int) -> None:
-        """Logs the scalar to TensorBoard and Weights & Biases (if enabled).
+        """Logs the scalar.
 
         Args:
             name (str): name of the image to be logged.
-            scalar (Union[int, float, torch.Tensor]): image to be logged.
+            scalar (int, float, torch.Tensor): image to be logged.
             global_step (int): current global step.
         """
         if not isinstance(scalar, (int, float, torch.Tensor)):
             raise NotImplementedError("LighterLogger currently supports only single scalars.")
         if isinstance(scalar, torch.Tensor) and scalar.dim() > 0:
             raise NotImplementedError("LighterLogger currently supports only single scalars.")
 
+        if isinstance(scalar, torch.Tensor):
+            scalar = scalar.item()
+
         if self.tensorboard:
             self.tensorboard.add_scalar(name, scalar, global_step=global_step)
         if self.wandb:
             self.wandb.log({name: scalar}, step=global_step)
 
     def _log_image(self, name: str, image: torch.Tensor, global_step: int) -> None:
-        """Logs the image to TensorBoard and Weights & Biases (if enabled).
+        """Logs the image.
 
         Args:
             name (str): name of the image to be logged.
             image (torch.Tensor): image to be logged.
             global_step (int): current global step.
         """
         if self.tensorboard:
             self.tensorboard.add_image(name, image, global_step=global_step)
         if self.wandb:
             self.wandb.log({name: OPTIONAL_IMPORTS["wandb"].Image(image)}, step=global_step)
 
+    def _log_histogram(self, name: str, tensor: torch.Tensor, global_step: int) -> None:
+        """Logs the histogram.
+
+        Args:
+            name (str): name of the image to be logged.
+            tensor (torch.Tensor): tensor to be logged.
+            global_step (int): current global step.
+        """
+        tensor = tensor.detach().cpu()
+
+        if self.tensorboard:
+            self.tensorboard.add_histogram(name, tensor, global_step=global_step)
+        if self.wandb:
+            self.wandb.log({name: OPTIONAL_IMPORTS["wandb"].Histogram(tensor)}, step=global_step)
+
     def _on_batch_end(self, outputs: Dict, trainer: Trainer) -> None:
         """Performs logging at the end of a batch/step. It logs the loss and metrics,
-        and, if specified how, the input, target, and pred data.
+        and, if their logging type is specified, the input, target, and pred data.
 
         Args:
             outputs (Dict): output dict from the model.
             trainer (Trainer): Trainer, passed automatically by PyTorch Lightning.
         """
         if not trainer.sanity_checking:
-            mode = LIGHTNING_TO_LIGHTER_STAGE[trainer.state.stage]
+            mode = get_lighter_mode(trainer.state.stage)
             # Accumulate the loss.
             if mode in ["train", "val"]:
                 self.loss[mode] += outputs["loss"].item()
-            # Logging frequency.
-            if self.global_step_counter[mode] % trainer.log_every_n_steps == 0:
-                # Log. Done only on rank 0.
-                self._log(outputs, mode, global_step=self._get_global_step(trainer))
+            # Logging frequency. Log only on rank 0.
+            if trainer.is_global_zero and self.global_step_counter[mode] % trainer.log_every_n_steps == 0:
+                # Get global step.
+                global_step = self._get_global_step(trainer)
+
+                # Log loss.
+                if outputs["loss"] is not None:
+                    self._log_scalar(f"{mode}/loss/step", outputs["loss"], global_step)
+
+                # Log metrics.
+                if outputs["metrics"] is not None:
+                    for name, metric in outputs["metrics"].items():
+                        self._log_scalar(f"{mode}/metrics/{name}/step", metric, global_step)
+
+                # Log input, target, and pred.
+                for name in ["input", "target", "pred"]:
+                    if self.log_types[name] is None:
+                        continue
+                    # Ensure data is of a valid type.
+                    if not is_data_type_supported(outputs[name]):
+                        raise ValueError(
+                            f"`{name}` has to be a Tensor, List[Tensor], Tuple[Tensor],  Dict[str, Tensor], "
+                            f"Dict[str, List[Tensor]], or Dict[str, Tuple[Tensor]]. `{type(outputs[name])}` is not supported."
+                        )
+                    for identifier, item in parse_data(outputs[name]).items():
+                        item_name = f"{mode}/data/{name}" if identifier is None else f"{mode}/data/{name}_{identifier}"
+                        self._log_by_type(item_name, item, self.log_types[name], global_step)
+
             # Increment the step counters.
             self.global_step_counter[mode] += 1
             if mode in ["train", "val"]:
                 self.epoch_step_counter[mode] += 1
 
     def _on_epoch_end(self, trainer: Trainer, pl_module: LighterSystem) -> None:
-        """Performs logging at the end of an epoch. It calculates the average
-        loss and metrics for the epoch and logs them. In distributed mode, it averages
-        the losses and metrics from all processes.
+        """Performs logging at the end of an epoch. Logs the epoch number, the loss, and the metrics.
+        It averages the loss and metrics over the epoch. In distributed mode, it averages over all ranks.
 
         Args:
             trainer (Trainer): Trainer, passed automatically by PyTorch Lightning.
             pl_module (LighterSystem): LighterSystem, passed automatically by PyTorch Lightning.
         """
         if not trainer.sanity_checking:
-            mode = LIGHTNING_TO_LIGHTER_STAGE[trainer.state.stage]
-            outputs = {"loss": None, "metrics": None}
+            mode = get_lighter_mode(trainer.state.stage)
+            loss, metrics = None, None
 
             # Loss
             if mode in ["train", "val"]:
                 # Get the accumulated loss.
                 loss = self.loss[mode]
-                # Reduce the loss to rank 0 and average it.
-                if dist.is_initialized():
-                    # Distributed communication works only tensors.
-                    loss = torch.tensor(loss).to(pl_module.device)
-                    # On rank 0, sum the losses from all ranks. Other ranks remain with the same loss as before.
-                    dist.reduce(loss, dst=0)
-                    # On rank 0, average the loss sum by dividing it with the number of processes.
-                    loss = loss.item() / dist.get_world_size() if dist.get_rank() == 0 else loss.item()
+                # Reduce the loss and average it on each rank.
+                loss = trainer.strategy.reduce(loss, reduce_op="mean")
                 # Divide the accumulated loss by the number of steps in the epoch.
                 loss /= self.epoch_step_counter[mode]
-                outputs["loss"] = loss
 
             # Metrics
             # Get the torchmetrics.
-            metrics = getattr(pl_module, f"{mode}_metrics")
-            if metrics is not None:
+            metric_collection = getattr(pl_module, f"{mode}_metrics")
+            if metric_collection is not None:
                 # Compute the epoch metrics.
-                outputs["metrics"] = metrics.compute()
+                metrics = metric_collection.compute()
                 # Reset the metrics for the next epoch.
-                metrics.reset()
+                metric_collection.reset()
 
-            # Log. Done only on rank 0.
-            self._log(outputs, mode, is_epoch=True, global_step=self._get_global_step(trainer))
+            # Log. Only on rank 0.
+            if trainer.is_global_zero:
+                # Get global step.
+                global_step = self._get_global_step(trainer)
+
+                # Log epoch number.
+                self._log_scalar("epoch", trainer.current_epoch, global_step)
+
+                # Log loss.
+                if loss is not None:
+                    self._log_scalar(f"{mode}/loss/epoch", loss, global_step)
+
+                # Log metrics.
+                if metrics is not None:
+                    for name, metric in metrics.items():
+                        self._log_scalar(f"{mode}/metrics/{name}/epoch", metric, global_step)
 
     def _get_global_step(self, trainer: Trainer) -> int:
         """Return the global step for the current mode. Note that when Trainer
         is running Trainer.fit() and is in `val` mode, this method will return
         the global step of the `train` mode in order to correctly log the validation
         steps against training steps.
 
         Args:
             trainer (Trainer): Trainer, passed automatically by PyTorch Lightning.
 
         Returns:
             int: global step.
         """
-        mode = LIGHTNING_TO_LIGHTER_STAGE[trainer.state.stage]
+        mode = get_lighter_mode(trainer.state.stage)
         # When validating in Trainer.fit(), return the train steps instead of the
         # val steps to correctly
         if mode == "val" and trainer.state.fn == "fit":
             return self.global_step_counter["train"]
         return self.global_step_counter[mode]
 
     def on_train_epoch_start(self, trainer: Trainer, pl_module: LighterSystem) -> None:
@@ -299,90 +316,7 @@
         self._on_epoch_end(trainer, pl_module)
 
     def on_validation_epoch_end(self, trainer: Trainer, pl_module: LighterSystem) -> None:
         self._on_epoch_end(trainer, pl_module)
 
     def on_test_epoch_end(self, trainer: Trainer, pl_module: LighterSystem) -> None:
         self._on_epoch_end(trainer, pl_module)
-
-
-def preprocess_image(image: torch.Tensor) -> torch.Tensor:
-    """Preprocess the image before logging it. If it is a batch of multiple images,
-    it will create a grid image of them. In case of 3D, a single image is displayed
-    with slices stacked vertically, while a batch as a grid where each column is
-    a different 3D image.
-    Args:
-        image (torch.Tensor): 2D or 3D image tensor.
-    Returns:
-        torch.Tensor: image ready for logging.
-    """
-    image = image.detach().cpu()
-    # 3D image (NCDHW)
-    has_three_dims = image.ndim == 5
-    if has_three_dims:
-        # Reshape 3D image from NCDHW to NC(D*H)W format
-        shape = image.shape
-        image = image.view(shape[0], shape[1], shape[2] * shape[3], shape[4])
-    if image.shape[0] == 1:
-        image = image[0]
-    else:
-        # If more than one image, create a grid
-        nrow = image.shape[0] if has_three_dims else 8
-        image = torchvision.utils.make_grid(image, nrow=nrow)
-    return image
-
-
-def check_image_data_type(data: Any, name: str) -> None:
-    """Check the input image data for its type. Valid image data types are:
-        - torch.Tensor
-        - List[torch.Tensor]
-        - Dict[str, torch.Tensor]
-        - Dict[str, List[torch.Tensor]]
-
-    Args:
-        data (Any): image data to check
-        name (str): name of the image data, for logging purposes.
-    """
-    if isinstance(data, dict):
-        is_valid = all(check_image_data_type(elem) for elem in data.values())
-    elif isinstance(data, list):
-        is_valid = all(check_image_data_type(elem) for elem in data)
-    elif isinstance(data, torch.Tensor):
-        is_valid = True
-    else:
-        is_valid = False
-
-    if not is_valid:
-        logger.error(
-            f"`{name}` has to be a Tensor, List[Tensors], Dict[str, Tensor]"
-            f", or Dict[str, List[Tensor]]. `{type(data)}` is not supported."
-        )
-        sys.exit()
-
-
-def parse_image_data(
-    data: Union[Dict[str, torch.Tensor], Dict[str, List[torch.Tensor]], List[torch.Tensor], torch.Tensor]
-) -> List[Tuple[Optional[str], torch.Tensor]]:
-    """Given input data, this function will parse it and return a list of tuples where
-    each tuple contains an identifier and a tensor.
-
-    Args:
-        data (Union[Dict[str, torch.Tensor], Dict[str, List[torch.Tensor]], List[torch.Tensor], torch.Tensor]): image tensor(s).
-
-    Returns:
-        List[Tuple[Optional[str], torch.Tensor]]: a list of tuples where the first element is
-            a string identifier (or `None` if there is only one image) and the second an image tensor.
-    """
-    result = []
-    if isinstance(data, dict):
-        for key, value in data.items():
-            if isinstance(value, list):
-                for i, tensor in enumerate(value):
-                    result.append((f"{key}_{i}", tensor) if len(value > 1) else (key, tensor))
-            else:
-                result.append((key, value))
-    elif isinstance(data, list):
-        for i, tensor in enumerate(data):
-            result.append((str(i), tensor))
-    else:
-        result.append((None, data))
-    return result
```

### Comparing `project_lighter-0.0.1/lighter/system.py` & `project_lighter-0.0.2a0/lighter/system.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,90 +8,104 @@
 from loguru import logger
 from torch.nn import Module
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader, Dataset, Sampler
 from torchmetrics import Metric, MetricCollection
 
 from lighter.utils.collate import collate_fn_replace_corrupted
-from lighter.utils.misc import ensure_list, get_name, hasarg
+from lighter.utils.misc import countargs, ensure_list, get_name, hasarg
 from lighter.utils.model import reshape_pred_if_single_value_prediction
 
 
 class LighterSystem(pl.LightningModule):
+    """_summary_
+
+    Args:
+        model (Module): the model.
+        batch_size (int): batch size.
+        drop_last_batch (bool, optional): whether the last batch in the dataloader
+            should be dropped. Defaults to False.
+        num_workers (int, optional): number of dataloader workers. Defaults to 0.
+        pin_memory (bool, optional): whether to pin the dataloaders memory. Defaults to True.
+        optimizers (Optional[Union[Optimizer, List[Optimizer]]], optional):
+            a single or a list of optimizers. Defaults to None.
+        schedulers (Optional[Union[Callable, List[Callable]]], optional):
+            a single or a list of schedulers. Defaults to None.
+        criterion (Optional[Callable], optional):
+            criterion/loss function. Defaults to None.
+        cast_target_dtype_to (Optional[str], optional): whether to cast the target to the
+            specified type before calculating the loss. May be necessary for some criterions.
+            Defaults to None.
+        post_criterion_activation (Optional[str], optional): some criterions
+            (e.g. BCEWithLogitsLoss) require non-activated prediction for their calculaiton.
+            However, to calculate the metrics and log the data, it may be necessary to activate
+            the predictions. Defaults to None.
+        inferer (Optional[Callable], optional): the inferer must be a class with a `__call__`
+            method that accepts two arguments - the input to infer over, and the model itself.
+            Used in 'val', 'test', and 'predict' mode, but not in 'train'. Typically, an inferer
+            is a sliding window or a patch-based inferer that will infer over the smaller parts of
+            the input, combine them, and return a single output. The inferers provided by MONAI
+            cover most of such cases (https://docs.monai.io/en/stable/inferers.html). Defaults to None.
+        freezer (Optional[Callable], optional): the freezer must be a class with a `__call__`
+            method that accepts three arguments - the model, the step, and the epoch number.
+            Use `lighter.utils.freezer.LighterFreezer` or implement your own based on it. Defaults to None.
+        train_metrics (Optional[Union[Metric, List[Metric]]], optional): training metric(s).
+            They have to be implemented using `torchmetrics`. Defaults to None.
+        val_metrics (Optional[Union[Metric, List[Metric]]], optional): validation metric(s).
+            They have to be implemented using `torchmetrics`. Defaults to None.
+        test_metrics (Optional[Union[Metric, List[Metric]]], optional): test metric(s).
+            They have to be implemented using `torchmetrics`. Defaults to None.
+        train_dataset (Optional[Union[Dataset, List[Dataset]]], optional): training dataset(s).
+            Defaults to None.
+        val_dataset (Optional[Union[Dataset, List[Dataset]]], optional): validation dataset(s).
+            Defaults to None.
+        test_dataset (Optional[Union[Dataset, List[Dataset]]], optional): test dataset(s).
+            Defaults to None.
+        predict_dataset (Optional[Union[Dataset, List[Dataset]]], optional): predict dataset(s).
+            Defaults to None.
+        train_sampler (Optional[Sampler], optional): training sampler(s). Defaults to None.
+        val_sampler (Optional[Sampler], optional): validation sampler(s). Defaults to None.
+        test_sampler (Optional[Sampler], optional):  test sampler(s). Defaults to None.
+        predict_sampler (Optional[Sampler], optional):  predict sampler(s). Defaults to None.
+        train_collate (Optional[Callable], optional): custom training collate function. Defaults to None.
+        val_collate (Optional[Callable], optional): custom validation collate function. Defaults to None.
+        test_collate (Optional[Callable], optional):  custom test collate function. Defaults to None.
+        predict_collate (Optional[Callable], optional):  custom predict collate function. Defaults to None.
+    """
+
     def __init__(
         self,
         model: Module,
         batch_size: int,
         drop_last_batch: bool = False,
         num_workers: int = 0,
         pin_memory: bool = True,
         optimizers: Optional[Union[Optimizer, List[Optimizer]]] = None,
         schedulers: Optional[Union[Callable, List[Callable]]] = None,
         criterion: Optional[Callable] = None,
         cast_target_dtype_to: Optional[str] = None,
         post_criterion_activation: Optional[str] = None,
-        patch_based_inferer: Optional[Callable] = None,
+        inferer: Optional[Callable] = None,
+        freezer: Optional[Callable] = None,
         train_metrics: Optional[Union[Metric, List[Metric]]] = None,
         val_metrics: Optional[Union[Metric, List[Metric]]] = None,
         test_metrics: Optional[Union[Metric, List[Metric]]] = None,
         train_dataset: Optional[Union[Dataset, List[Dataset]]] = None,
         val_dataset: Optional[Union[Dataset, List[Dataset]]] = None,
         test_dataset: Optional[Union[Dataset, List[Dataset]]] = None,
         predict_dataset: Optional[Union[Dataset, List[Dataset]]] = None,
         train_sampler: Optional[Sampler] = None,
         val_sampler: Optional[Sampler] = None,
         test_sampler: Optional[Sampler] = None,
         predict_sampler: Optional[Sampler] = None,
+        train_collate: Optional[Callable] = None,
+        val_collate: Optional[Callable] = None,
+        test_collate: Optional[Callable] = None,
+        predict_collate: Optional[Callable] = None,
     ) -> None:
-        """_summary_
-
-        Args:
-            model (Module): the model.
-            batch_size (int): batch size.
-            drop_last_batch (bool, optional): whether the last batch in the dataloader
-                should be dropped. Defaults to False.
-            num_workers (int, optional): number of dataloader workers. Defaults to 0.
-            pin_memory (bool, optional): whether to pin the dataloaders memory. Defaults to True.
-            optimizers (Optional[Union[Optimizer, List[Optimizer]]], optional):
-                a single or a list of optimizers. Defaults to None.
-            schedulers (Optional[Union[Callable, List[Callable]]], optional):
-                a single or a list of schedulers. Defaults to None.
-            criterion (Optional[Callable], optional):
-                criterion/loss function. Defaults to None.
-            cast_target_dtype_to (Optional[str], optional): whether to cast the target to the
-                specified type before calculating the loss. May be necessary for some criterions.
-                Defaults to None.
-            post_criterion_activation (Optional[str], optional): some criterions
-                (e.g. BCEWithLogitsLoss) require non-activated prediction for their calculaiton.
-                However, to calculate the metrics and log the data, it may be necessary to activate
-                the predictions. Defaults to None.
-            patch_based_inferer (Optional[Callable], optional): the patch based inferer needs to be
-                either a class with a `__call__` method or function that accepts two arguments -
-                first one is the input tensor, and the other one the model itself. It should
-                perform the inference over the patches and return the aggregated/averaged output.
-                Defaults to None.
-            train_metrics (Optional[Union[Metric, List[Metric]]], optional): training metric(s).
-                They have to be implemented using `torchmetrics`. Defaults to None.
-            val_metrics (Optional[Union[Metric, List[Metric]]], optional): validation metric(s).
-                They have to be implemented using `torchmetrics`. Defaults to None.
-            test_metrics (Optional[Union[Metric, List[Metric]]], optional): test metric(s).
-                They have to be implemented using `torchmetrics`. Defaults to None.
-            train_dataset (Optional[Union[Dataset, List[Dataset]]], optional): training dataset(s).
-                Defaults to None.
-            val_dataset (Optional[Union[Dataset, List[Dataset]]], optional): validation dataset(s).
-                Defaults to None.
-            test_dataset (Optional[Union[Dataset, List[Dataset]]], optional): test dataset(s).
-                Defaults to None.
-            predict_dataset (Optional[Union[Dataset, List[Dataset]]], optional): predict dataset(s).
-                Defaults to None.
-            train_sampler (Optional[Sampler], optional): training sampler(s). Defaults to None.
-            val_sampler (Optional[Sampler], optional): validation sampler(s). Defaults to None.
-            test_sampler (Optional[Sampler], optional):  test sampler(s). Defaults to None.
-            predict_sampler (Optional[Sampler], optional):  predict sampler(s). Defaults to None.
-        """
         super().__init__()
         # Bypass LightningModule's check for default methods. We define them in self.setup().
         self._init_placeholders_for_dataloader_and_step_methods()
 
         # Model setup
         self.model = model
         self.batch_size = batch_size
@@ -112,198 +126,241 @@
 
         # Samplers
         self.train_sampler = train_sampler
         self.val_sampler = val_sampler
         self.test_sampler = test_sampler
         self.predict_sampler = predict_sampler
 
+        # Collate functions
+        self.train_collate = train_collate
+        self.val_collate = val_collate
+        self.test_collate = test_collate
+        self.predict_collate = predict_collate
+
         # Metrics
         self.train_metrics = MetricCollection(ensure_list(train_metrics))
         self.val_metrics = MetricCollection(ensure_list(val_metrics))
         self.test_metrics = MetricCollection(ensure_list(test_metrics))
 
         # Criterion-specific activation function and data type casting
         self._post_criterion_activation = post_criterion_activation
         self._cast_target_dtype_to = cast_target_dtype_to
 
-        # Patch-based inference
-        self._patch_based_inferer = patch_based_inferer
+        # Inferer for val, test, and predict
+        self.inferer = inferer
+
+        # Layer freezer
+        self.freezer = freezer
 
         # Checks
         self._lightning_module_methods_defined = False
         self._target_not_used_reported = False
+        self._batch_type_reported = False
 
-    def forward(self, input: Union[torch.Tensor, List, Tuple]) -> Union[torch.Tensor, List, Tuple]:
+    def forward(self, input: Union[torch.Tensor, List[torch.Tensor], Tuple[torch.Tensor], Dict[str, torch.Tensor]]) -> Any:
         """Forward pass. Multi-input models are supported.
 
         Args:
-            input (Union[torch.Tensor, List, Tuple]): input to the model.
+            input (torch.Tensor, List[torch.Tensor], Tuple[torch.Tensor], Dict[str, torch.Tensor]): input to the model.
 
         Returns:
-            Union[torch.Tensor, List, Tuple]: output of the model.
+            Any: output of the model.
         """
+        # Keyword arguments to pass to the forward method
         kwargs = {}
         if hasarg(self.model.forward, "epoch"):
+            # Add `epoch` argument if forward accepts it
             kwargs["epoch"] = self.current_epoch
         if hasarg(self.model.forward, "step"):
+            # Add `step` argument if forward accepts it
             kwargs["step"] = self.global_step
 
-        if isinstance(input, list):
+        # Type not supported.
+        if not isinstance(input, (torch.Tensor, tuple, list, dict)):
+            logger.error(f"Input type '{type(input)}' not supported.")
+            sys.exit()
+
+        # Freeze the layers if specified so.
+        if self.freezer is not None:
+            self.freezer(self.model, self.global_step, self.current_epoch)
+
+        # Unpack Tuple or List. Only if num of args passed is less than or equal to num of args accepted.
+        if isinstance(input, (tuple, list)) and (len(input) + len(kwargs)) <= countargs(self.model):
             return self.model(*input, **kwargs)
-        return self.model(input, **kwargs)
+        # Unpack Dict. Only if dict's keys match criterion's keyword arguments.
+        elif isinstance(input, dict) and all(hasarg(self.model, name) for name in input):
+            return self.model(**input, **kwargs)
+        # Tensor, Tuple, List, or Dict, as-is, not unpacked.
+        else:
+            return self.model(input, **kwargs)
 
-    def _base_step(self, batch: Tuple, batch_idx: int, mode: str) -> Union[Dict[str, Any], Any]:
-        """Base step for all modes ('train', 'val', 'test', 'predict')
+    def _base_step(self, batch: Union[List, Tuple], batch_idx: int, mode: str) -> Union[Dict[str, Any], Any]:
+        """Base step for all modes ("train", "val", "test", "predict")
 
         Args:
-            batch (Tuple):
+            batch (List, Tuple):
                 output of the DataLoader and input to the model.
             batch_idx (int): index of the batch. Not used, but PyTorch Lightning requires it.
             mode (str): mode in which the system is.
 
         Returns:
             Union[Dict[str, Any], Any]: For the training, validation and test step, it returns
                 a dict containing loss, metrics, input, target, and pred. Loss will be `None`
                 for the test step. Metrics will be `None` if no metrics are specified.
 
                 For predict step, it returns pred only.
         """
-        input, target = batch if len(batch) == 2 else (batch[:-1], batch[-1])
+        # Split the batch into input and target. Target will be `None` if not provided.
+        input, target = self._split_batch(batch)
 
-        # Predict
-        if self._patch_based_inferer and mode in ["val", "test", "predict"]:
-            # TODO: Patch-based inference doesn't support multiple inputs yet
-            pred = self._patch_based_inferer(input, self)
+        # Forward
+        if self.inferer and mode in ["val", "test", "predict"]:
+            pred = self.inferer(input, self)
         else:
             pred = self(input)
 
         pred = reshape_pred_if_single_value_prediction(pred, target)
 
-        # Calculate the loss
+        # Calculate the loss.
         loss = None
         if mode in ["train", "val"]:
             loss = self._calculate_loss(pred, target)
 
         # Apply the post-criterion activation. Necessary for measuring the metrics
         # correctly in cases when using a criterion such as `BCELossWithLogits`` which
         # requires the model to output logits, i.e. non-activated outputs.
         if self._post_criterion_activation is not None:
             pred = self._post_criterion_activation(pred)
 
-        # In predict mode, skip metrics and logging parts and return the predicted value
         if mode == "predict":
+            # In predict mode, skip the metrics and return the predicted value only.
             return pred
-
-        # Calculate the metrics for the step
-        step_metrics = getattr(self, f"{mode}_metrics")(pred, target)
-
-        return {"loss": loss, "metrics": step_metrics, "input": input, "target": target, "pred": pred}
-
-    def _calculate_loss(self, pred: Union[torch.Tensor, List, Tuple], target: Union[torch.Tensor, None]) -> torch.Tensor:
+        else:
+            # Calculate the metrics for the step.
+            metrics = getattr(self, f"{mode}_metrics")(pred, target)
+            # Log the loss and metrics for monitoring purposes only.
+            self.log("loss" if mode == "train" else f"{mode}_loss", loss, on_step=True, on_epoch=True, logger=False)
+            self.log_dict(metrics, on_step=True, on_epoch=True, logger=False)
+            # Return the loss, metrics, input, target, and pred.
+            return {"loss": loss, "metrics": metrics, "input": input, "target": target, "pred": pred}
+
+    def _calculate_loss(
+        self, pred: Union[torch.Tensor, List, Tuple, Dict], target: Union[torch.Tensor, List, Tuple, Dict, None]
+    ) -> torch.Tensor:
         """_summary_
 
         Args:
-            pred (Union[torch.Tensor, List, Tuple]): the predicted values from the model.
-            target (Union[torch.Tensor, None]): the target/label.
+            pred (torch.Tensor, List, Tuple, Dict, None): the predicted values from the model.
+            target (torch.Tensor, List, Tuple, Dict, None): the target/label.
 
         Returns:
             torch.Tensor: the calculated loss.
         """
+        # Keyword arguments to pass to the loss/criterion function
+        kwargs = {}
         if hasarg(self.criterion.forward, "target"):
-            loss = self.criterion(pred, target.to(self._cast_target_dtype_to))
+            # Add `target` argument if forward accepts it. Casting performed if specified.
+            kwargs["target"] = target.to(self._cast_target_dtype_to)
         else:
-            loss = self.criterion(pred)
-
             if not self._target_not_used_reported and not self.trainer.sanity_checking:
                 self._target_not_used_reported = True
                 logger.info(
                     f"The criterion `{get_name(self.criterion, True)}` "
                     "has no `target` argument. In such cases, the LighterSystem "
                     "passes only the predicted values to the criterion. "
                     "This is intended as a support for self-supervised "
                     "losses where target is not used. If this is not the "
                     "behavior you expected, redefine your criterion "
                     "so that it has a `target` argument."
                 )
-        return loss
+
+        # Type not supported.
+        if not isinstance(pred, (torch.Tensor, tuple, list, dict)):
+            logger.error(f"Pred type '{type(pred)}' not supported.")
+            sys.exit()
+
+        # Unpack Tuple or List. Only if num of args passed is less than or equal to num of args accepted.
+        if isinstance(pred, (tuple, list)) and (len(pred) + len(kwargs)) <= countargs(self.criterion):
+            return self.criterion(*pred, **kwargs)
+        # Unpack Dict. Only if dict's keys match criterion's keyword arguments' names.
+        elif isinstance(pred, dict) and all(hasarg(self.criterion, name) for name in pred):
+            return self.criterion(**pred, **kwargs)
+        # Tensor, Tuple, List, or Dict, as-is, not unpacked.
+        else:
+            return self.criterion(pred, **kwargs)
 
     def _base_dataloader(self, mode: str) -> DataLoader:
-        """Instantiate the dataloader for a mode (train/val/test).
+        """Instantiate the dataloader for a mode (train/val/test/predict).
         Includes a collate function that enables the DataLoader to replace
         None's (alias for corrupted examples) in the batch with valid examples.
         To make use of it, write a try-except in your Dataset that handles
         corrupted data by returning None instead.
 
         Args:
-            mode (str): mode for which to create the dataloader ['train', 'val', 'test'].
+            mode (str): mode for which to create the dataloader ["train", "val", "test", "predict"].
 
         Returns:
             DataLoader: instantiated DataLoader.
         """
         dataset = getattr(self, f"{mode}_dataset")
         sampler = getattr(self, f"{mode}_sampler")
+        collate_fn = getattr(self, f"{mode}_collate")
 
         if dataset is None:
             logger.error(f"Please specify '{mode}_dataset' in the config. Exiting")
             sys.exit()
 
-        # Batch size is 1 when using patch based inference for two reasons:
-        # 1) Patch based inference splits an input into a batch of patches,
-        # so the batch size will actually be defined for it;
-        # 2) In settings where patch based inference is needed, the input data often
-        # varies in shape, preventing the data loader to stack them into a batch.
+        # Batch size is 1 when using an inference for two reasons:
+        # 1) Inferer separates an input into multiple parts, forming a batch of its own.
+        # 2) The val/test/pred data usually differ in their shape, so they cannot be stacked into a batch.
         batch_size = self.batch_size
-        if self._patch_based_inferer is not None and mode in ["val", "test", "predict"]:
-            logger.info(f"Setting the general batch size to 1 for {mode} " "mode because a patch-based inferer is used.")
+        if self.inferer is not None and mode in ["val", "test", "predict"]:
+            logger.info(f"Setting the '{mode}' mode dataloader to batch size of 1 because an inferer is provided.")
             batch_size = 1
 
         # A dataset can return None when a corrupted example occurs. This collate
         # function replaces None's with valid examples from the dataset.
-        collate_fn = partial(collate_fn_replace_corrupted, dataset=dataset)
+        collate_fn = partial(collate_fn_replace_corrupted, dataset=dataset, default_collate_fn=collate_fn)
         return DataLoader(
             dataset,
             sampler=sampler,
             shuffle=(mode == "train" and sampler is None),
             batch_size=batch_size,
             drop_last=self.drop_last_batch,
             num_workers=self.num_workers,
             pin_memory=self.pin_memory,
             collate_fn=collate_fn,
         )
 
-    def configure_optimizers(self) -> Dict:
+    def configure_optimizers(self) -> Union[Optimizer, List[Dict[str, Union[Optimizer, "Scheduler"]]]]:
         """LightningModule method. Returns optimizers and, if defined, schedulers.
 
         Returns:
-            Single optimizer: If only a optimizer is provided
-            Tuple of dictionaries: a tuple of `dict` with keys `optimizer` and `lr_scheduler`
+            Optimizer or a List of Dict of paired Optimizers and Schedulers: instantiated
+                optimizers and/or schedulers.
         """
         if not self.optimizers:
-            logger.error("Please specify 'optimizers' in the config. Exiting.")
+            logger.error("Please specify 'system.optimizers' in the config. Exiting.")
             sys.exit()
         if not self.schedulers:
             return self.optimizers
 
         if len(self.optimizers) != len(self.schedulers):
-            logger.error("'optimizers' and 'schedulers' should be paired")
+            logger.error("Each optimizer must have its own scheduler.")
             sys.exit()
 
-        optim_sched_paired = []
-        for optimizer, scheduler in zip(self.optimizers, self.schedulers):
-            optim_sched_paired.append({"optimizer": optimizer, "lr_scheduler": scheduler})
-
-        return tuple(optim_sched_paired)
+        return [{"optimizer": opt, "lr_scheduler": sched} for opt, sched in zip(self.optimizers, self.schedulers)]
 
     def setup(self, stage: str) -> None:
         """Automatically called by the LightningModule after the initialization.
         `LighterSystem`'s setup checks if the required dataset is provided in the config and
         sets up LightningModule methods for the stage in which the system is.
 
         Args:
-            stage (str): passed by PyTorch Lightning. ['fit', 'validate', 'test'].
+            stage (str): passed by PyTorch Lightning. ["fit", "validate", "test"].
         """
         # Stage-specific PyTorch Lightning methods. Defined dynamically so that the system
         # only has methods used in the stage and for which the configuration was provided.
         if not self._lightning_module_methods_defined:
             del (
                 self.train_dataloader,
                 self.training_step,
@@ -334,14 +391,42 @@
             self.test_step = partial(self._base_step, mode="test")
 
         # Predict methods.
         if stage == "predict":
             self.predict_dataloader = partial(self._base_dataloader, mode="predict")
             self.predict_step = partial(self._base_step, mode="predict")
 
+    def _split_batch(self, batch) -> Tuple[torch.Tensor, Optional[Any]]:
+        """Split the batch into input and target. Target will be `None` if not provided.
+
+        Args:
+            batch (List, Tuple): output of the DataLoader and input to the model.
+
+        Returns:
+            Tuple(torch.Tensor, Optional[Any]): input and target.
+        """
+        # Check if the batch format is correct.
+        if len(batch) > 2:
+            raise ValueError(
+                "Found more than 2 items in the batch. `LighterSystem` requires the dataloader to return either "
+                "input tensor(s) only, or a two-element tuple/list consisting of input tensor(s) and target(s)."
+            )
+
+        # Report the batch split type. Only on the first call.
+        if not self._batch_type_reported:
+            self._batch_type_reported = True
+            if len(batch) == 1:
+                logger.info("Target not provided. Using `None` as target. Ignore if intended.")
+            else:
+                logger.info("Using the first item as input and the second item as target.")
+
+        # Split the batch into input and target. Target will be `None` if not provided.
+        input, target = (batch, None) if len(batch) == 1 else batch
+        return input, target
+
     def _init_placeholders_for_dataloader_and_step_methods(self) -> None:
         """`LighterSystem` dynamically defines the `..._dataloader()`and `..._step()` methods
         in the `self.setup()` method. However, `LightningModule` excepts them to be defined at
         the initialization. To prevent it from throwing an error, the `..._dataloader()` and
         `..._step()` are initially defined as `lambda: None`, before `self.setup()` is called.
         """
         self.train_dataloader = self.training_step = lambda: None
```

### Comparing `project_lighter-0.0.1/lighter/utils/collate.py` & `project_lighter-0.0.2a0/lighter/utils/collate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,44 @@
+from typing import Any, Callable, List
+
 import random
 
 import torch
 from torch.utils.data import DataLoader
+from torch.utils.data.dataloader import default_collate
 
 
-def collate_fn_replace_corrupted(batch: torch.Tensor, dataset: DataLoader) -> torch.Tensor:
+def collate_fn_replace_corrupted(batch: List[Any], dataset: DataLoader, default_collate_fn: Callable = None) -> torch.Tensor:
     """Collate function that allows to replace corrupted examples in the batch.
     The dataloader should return `None` when that occurs.
     The `None`s in the batch are replaced with other, randomly-selected, examples.
 
     Args:
-        batch (torch.Tensor): batch from the DataLoader.
+        batch (List[Any]): batch from the DataLoader.
         dataset (Dataset): dataset that the DataLoader is passing through. Needs to be fixed
             in place with functools.partial before passing it to DataLoader's 'collate_fn' option
             as 'collate_fn' should only have a single argument - batch. Example:
                 ```
                 collate_fn = functools.partial(collate_fn_replace_corrupted, dataset=dataset)`
                 loader = DataLoader(dataset, ..., collate_fn=collate_fn).
                 ```
+        default_collate_fn (Callable): the collate function to call once the batch has no corrupted examples.
+            If `None`, `torch.utils.data.dataloader.default_collate` is called. Defaults to None.
     Returns:
         torch.Tensor: batch with new examples instead of corrupted ones.
     """
+    # Use `torch.utils.data.dataloader.default_collate` if no other default collate function is specified.
+    default_collate_fn = default_collate_fn if default_collate_fn is not None else default_collate
     # Idea from https://stackoverflow.com/a/57882783
     original_batch_len = len(batch)
-    # Filter out all the Nones (corrupted examples)
+    # Filter out all the Nones (corrupted examples).
     batch = list(filter(lambda x: x is not None, batch))
     filtered_batch_len = len(batch)
-    # Num of corrupted examples
+    # Num of corrupted examples.
     num_corrupted = original_batch_len - filtered_batch_len
     if num_corrupted > 0:
-        # Replace a corrupted example with another randomly selected example
-        batch.extend([dataset[random.randint(0, len(dataset))] for _ in range(num_corrupted)])
-        # Recursive call to replace the replacements if they are corrupted
+        # Replace a corrupted example with another randomly selected example.
+        batch.extend([dataset[random.randint(0, len(dataset) - 1)] for _ in range(num_corrupted)])
+        # Recursive call to replace the replacements if they are corrupted.
         return collate_fn_replace_corrupted(batch, dataset)
-    # Finally, when the whole batch is fine, return it
-    return torch.utils.data.dataloader.default_collate(batch)
+    # Finally, when the whole batch is fine, apply the default collate function.
+    return default_collate_fn(batch)
```

### Comparing `project_lighter-0.0.1/lighter/utils/dynamic_imports.py` & `project_lighter-0.0.2a0/lighter/utils/dynamic_imports.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import importlib
 import sys
 from pathlib import Path
 
 from loguru import logger
 
+OPTIONAL_IMPORTS = {}
+
 
 def import_module_from_path(module_name: str, module_path: str) -> None:
     """Given the path to a module, import it, and name it as specified.
 
     Args:
         module_name (str): what to name the imported module.
         module_path (str): path to the module to load.
```

### Comparing `project_lighter-0.0.1/lighter/utils/misc.py` & `project_lighter-0.0.2a0/lighter/utils/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,75 +2,87 @@
 
 import inspect
 import sys
 
 from loguru import logger
 
 
-def ensure_list(x: Any) -> List:
+def ensure_list(vals: Any) -> List:
     """Wrap the input into a list if it is not a list. If it is a None, return an empty list.
 
     Args:
-        x (Any): input to wrap into a list.
+        vals (Any): input to wrap into a list.
 
     Returns:
         List: output list.
     """
-    if isinstance(x, list):
-        return x
-    if isinstance(x, tuple):
-        return list(x)
-    if x is None:
+    if isinstance(vals, list):
+        return vals
+    if isinstance(vals, tuple):
+        return list(vals)
+    if vals is None:
         return []
-    return [x]
+    return [vals]
 
 
-def dot_notation_setattr(obj: Callable, attr: str, value: Any):
-    """Set object's attribute. May use dot notation.
+def setattr_dot_notation(obj: Callable, attr: str, value: Any):
+    """Set object's attribute. Supports dot notation.
 
     Args:
         obj (Callable): object.
         attr (str): attribute name of the object.
-        value (Any): attribute value to be set.
+        value (Any): value to set the attribute to.
     """
     if "." not in attr:
         if not hasattr(obj, attr):
             logger.info(f"`{get_name(obj, True)}` has no attribute `{attr}`. Exiting.")
             sys.exit()
         setattr(obj, attr, value)
     # Solve recursively if the attribute is defined in dot-notation
     else:
         obj_name, attr = attr.split(".", maxsplit=1)
-        dot_notation_setattr(getattr(obj, obj_name), attr, value)
+        setattr_dot_notation(getattr(obj, obj_name), attr, value)
 
 
 def hasarg(_callable: Callable, arg_name: str) -> bool:
     """Check if a function, class, or method has an argument with the specified name.
 
     Args:
-        callable (Callable): function, class, or method to inspect.
+        _callable (Callable): function, class, or method to inspect.
         arg_name (str): argument name to check for.
 
     Returns:
         bool: `True` if the argument if the specified name exists.
     """
 
     args = inspect.signature(_callable).parameters.keys()
     return arg_name in args
 
 
-def get_name(x: Callable, include_module_name: bool = False) -> str:
+def countargs(_callable: Callable) -> bool:
+    """Count the number of arguments that a function, class, or method accepts.
+
+    Args:
+        callable (Callable): function, class, or method to inspect.
+
+    Returns:
+        int: number of arguments that it accepts.
+    """
+    return len(inspect.signature(_callable).parameters.keys())
+
+
+def get_name(_callable: Callable, include_module_name: bool = False) -> str:
     """Get the name of an object, class or function.
 
     Args:
-        x (Callable): object, class or function.
+        _callable (Callable): object, class or function.
         include_module_name (bool, optional): whether to include the name of the module from
             which it comes. Defaults to False.
 
     Returns:
         str: name
     """
-    name = type(x).__name__ if isinstance(x, object) else x.__name__
+    name = type(_callable).__name__ if isinstance(_callable, object) else _callable.__name__
     if include_module_name:
-        module = type(x).__module__ if isinstance(x, object) else x.__module__
+        module = type(_callable).__module__ if isinstance(_callable, object) else _callable.__module__
         name = f"{module}.{name}"
     return name
```

### Comparing `project_lighter-0.0.1/pyproject.toml` & `project_lighter-0.0.2a0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 lighter = "lighter.utils.cli:interface"
 
 [tool.poetry]
 name = "project-lighter"
-version = "0.0.1"
+version = "0.0.2a0"
 description = "YAML-based automated rapid prototyping framework for deep learning experiments"
 readme = "README.md"
 authors = ["Ibrahim Hadzic <ibrahimhadzic45@gmail.com>" ,
             "Suraj Pai <b.pai@maastrichtuniversity.nl>", 
             "Keno Bressem <kbressem@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/lighter/lighter"
@@ -38,25 +38,25 @@
   "Programming Language :: Python :: 3.11",
 ]
 
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-torch = "^1.13.1"
+torch = "^2.0"
 pandas = "^1.5.3"
-torchvision = "^0.14.1"
-pytorch-lightning = "^1.9.0"
+torchvision = "^0.15"
+pytorch-lightning = "^2.0.0"
 fire = "^0.5.0"
 loguru = "^0.6.0"
 lightly = "^1.2.43"
 torchmetrics = "^0.11.0"
 py = "^1.11.0"
 tensorboard = "^2.11.2"
-monai-weekly = "^1.2.dev2304"
+monai-weekly = "^1.2.dev2305"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.4"
 black = {version = "^23.1a1", allow-prereleases = true}
 isort = {extras = ["colors"], version = "^5.11.4"}
 mypy = "^0.991"
 mypy-extensions = "^0.4.3"
@@ -171,14 +171,15 @@
 show_missing = true
 
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 127
 disable = """
     too-many-arguments,
-    not-callable
+    no-else-return,
 """
+generated-members = "torch.*"
 
 [tool.pylint.master]
 fail-under=8
 
 [tool.poetry_bumpversion.file."lighter/__init__.py"]
```

### Comparing `project_lighter-0.0.1/PKG-INFO` & `project_lighter-0.0.2a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-lighter
-Version: 0.0.1
+Version: 0.0.2a0
 Summary: YAML-based automated rapid prototyping framework for deep learning experiments
 Home-page: https://github.com/lighter/lighter
 License: MIT
 Author: Ibrahim Hadzic
 Author-email: ibrahimhadzic45@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -21,22 +21,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: lightly (>=1.2.43,<2.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: monai-weekly (>=1.2.dev2304,<2.0)
+Requires-Dist: monai-weekly (>=1.2.dev2305,<2.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: py (>=1.11.0,<2.0.0)
-Requires-Dist: pytorch-lightning (>=1.9.0,<2.0.0)
+Requires-Dist: pytorch-lightning (>=2.0.0,<3.0.0)
 Requires-Dist: tensorboard (>=2.11.2,<3.0.0)
-Requires-Dist: torch (>=1.13.1,<2.0.0)
+Requires-Dist: torch (>=2.0,<3.0)
 Requires-Dist: torchmetrics (>=0.11.0,<0.12.0)
-Requires-Dist: torchvision (>=0.14.1,<0.15.0)
+Requires-Dist: torchvision (>=0.15,<0.16)
 Project-URL: Repository, https://github.com/lighter/lighter
 Description-Content-Type: text/markdown
 
 # Lighter
 [![build](https://github.com/project-lighter/lighter/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/project-lighter/lighter/actions/workflows/build.yml) ![Coverage](./assets/images/coverage.svg)
```

