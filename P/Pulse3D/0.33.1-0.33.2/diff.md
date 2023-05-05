# Comparing `tmp/Pulse3D-0.33.1.tar.gz` & `tmp/Pulse3D-0.33.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pulse3D-0.33.1.tar", last modified: Thu May  4 23:48:48 2023, max compression
+gzip compressed data, was "Pulse3D-0.33.2.tar", last modified: Fri May  5 18:01:07 2023, max compression
```

## Comparing `Pulse3D-0.33.1.tar` & `Pulse3D-0.33.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-04 23:48:48.672560 Pulse3D-0.33.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/mantarray-magnet-finding/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-04 23:47:40.000000 Pulse3D-0.33.1/mantarray-magnet-finding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/mantarray-magnet-finding/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/mantarray-magnet-finding/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 23:47:40.000000 Pulse3D-0.33.1/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-04 23:47:40.000000 Pulse3D-0.33.1/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-04 23:47:40.000000 Pulse3D-0.33.1/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-04 23:47:40.000000 Pulse3D-0.33.1/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-04 23:48:48.672560 Pulse3D-0.33.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/src/Pulse3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-04 23:48:48.000000 Pulse3D-0.33.1/src/Pulse3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-04 23:48:48.000000 Pulse3D-0.33.1/src/Pulse3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 23:48:33.000000 Pulse3D-0.33.1/src/Pulse3D.egg-info/not-zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 23:48:11.000000 Pulse3D-0.33.1/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-04 23:48:11.000000 Pulse3D-0.33.1/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-04 23:48:11.000000 Pulse3D-0.33.1/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-04 23:48:11.000000 Pulse3D-0.33.1/src/mantarray_magnet_finding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:48:48.668560 Pulse3D-0.33.1/src/pulse3D/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/compression_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    45310 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34854 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    33981 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/plate_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/stimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-04 23:47:36.000000 Pulse3D-0.33.1/src/pulse3D/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.349611 Pulse3D-0.33.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 18:01:07.349611 Pulse3D-0.33.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.345611 Pulse3D-0.33.2/mantarray-magnet-finding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-05 18:00:03.000000 Pulse3D-0.33.2/mantarray-magnet-finding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.341611 Pulse3D-0.33.2/mantarray-magnet-finding/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.345611 Pulse3D-0.33.2/mantarray-magnet-finding/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 18:00:03.000000 Pulse3D-0.33.2/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-05 18:00:03.000000 Pulse3D-0.33.2/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-05 18:00:03.000000 Pulse3D-0.33.2/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-05 18:00:03.000000 Pulse3D-0.33.2/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 18:01:07.353612 Pulse3D-0.33.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.341611 Pulse3D-0.33.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.349611 Pulse3D-0.33.2/src/Pulse3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 18:01:07.000000 Pulse3D-0.33.2/src/Pulse3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-05 18:01:07.000000 Pulse3D-0.33.2/src/Pulse3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:00:52.000000 Pulse3D-0.33.2/src/Pulse3D.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.345611 Pulse3D-0.33.2/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 18:00:31.000000 Pulse3D-0.33.2/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-05 18:00:31.000000 Pulse3D-0.33.2/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-05 18:00:31.000000 Pulse3D-0.33.2/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-05 18:00:31.000000 Pulse3D-0.33.2/src/mantarray_magnet_finding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.349611 Pulse3D-0.33.2/src/pulse3D/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/compression_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46415 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34854 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/nb_peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33482 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/plate_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/utils.py
```

### Comparing `Pulse3D-0.33.1/LICENSE` & `Pulse3D-0.33.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.1/PKG-INFO` & `Pulse3D-0.33.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.1
+Version: 0.33.2
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.1/mantarray-magnet-finding/setup.py` & `Pulse3D-0.33.2/mantarray-magnet-finding/setup.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.1/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.2/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.1/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.2/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.1/setup.py` & `Pulse3D-0.33.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 extensions = [Extension("pulse3D.compression_cy", [os.path.join("src", "pulse3D", "compression_cy") + ext])]
 if USE_CYTHON:
     # cythonizing compression_cy.pyx with kwarg annotate=True will help when optimizing the code by enabling generation of the html annotation file
     extensions = cythonize(extensions, annotate=False)
 
 setup(
     name="Pulse3D",
-    version="0.33.1",
+    version="0.33.2",
     description="Pulse3D Analysis Platform",
     url="https://github.com/CuriBio/Pulse3D",
     project_urls={"Documentation": "https://pulse3D.readthedocs.io/en/latest/"},
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `Pulse3D-0.33.1/src/Pulse3D.egg-info/PKG-INFO` & `Pulse3D-0.33.2/src/Pulse3D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.1
+Version: 0.33.2
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.1/src/Pulse3D.egg-info/SOURCES.txt` & `Pulse3D-0.33.2/src/Pulse3D.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -15,13 +15,14 @@
 src/pulse3D/__init__.py
 src/pulse3D/compression_cy.pyx
 src/pulse3D/constants.py
 src/pulse3D/excel_writer.py
 src/pulse3D/exceptions.py
 src/pulse3D/magnet_finding.py
 src/pulse3D/metrics.py
+src/pulse3D/nb_peak_detection.py
 src/pulse3D/peak_detection.py
 src/pulse3D/plate_recording.py
 src/pulse3D/plotting.py
 src/pulse3D/stimulation.py
 src/pulse3D/transforms.py
 src/pulse3D/utils.py
```

### Comparing `Pulse3D-0.33.1/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.2/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.1/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.2/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.1/src/pulse3D/compression_cy.pyx` & `Pulse3D-0.33.2/src/pulse3D/compression_cy.pyx`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.1/src/pulse3D/constants.py` & `Pulse3D-0.33.2/src/pulse3D/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,22 @@
 
 DEFAULT_TWITCH_WIDTHS = (10, 50, 90)
 DEFAULT_BASELINE_WIDTHS = (10, 90)
 DEFAULT_TWITCH_WIDTH_PERCENTS = tuple(range(10, 95, 5))
 DEFAULT_PROMINENCE_FACTORS = (6, 6)
 DEFAULT_WIDTH_FACTORS = (7, 7)
 
+DEFAULT_NB_NOISE_PROMINENCE_FACTOR = 2.5
+DEFAULT_NB_RELATIVE_PROMINENCE_FACTOR = 0.2
+DEFAULT_NB_WIDTH_FACTORS = (0, 5)
+DEFAULT_NB_HEIGHT_FACTOR = 0
+DEFAULT_NB_VALLEY_SEARCH_DUR = 1
+DEFAULT_NB_UPSLOPE_DUR = 0.07
+DEFAULT_NB_UPSLOPE_NOISE_ALLOWANCE_DUR = 0.01
+
 # twitch indices keys
 PRIOR_PEAK_INDEX_UUID = uuid.UUID("80df90dc-21f8-4cad-a164-89436909b30a")
 PRIOR_VALLEY_INDEX_UUID = uuid.UUID("72ba9466-c203-41b6-ac30-337b4a17a124")
 SUBSEQUENT_PEAK_INDEX_UUID = uuid.UUID("7e37325b-6681-4623-b192-39f154350f36")
 SUBSEQUENT_VALLEY_INDEX_UUID = uuid.UUID("fd47ba6b-ee4d-4674-9a89-56e0db7f3d97")
 
 # filters
```

### Comparing `Pulse3D-0.33.1/src/pulse3D/excel_writer.py` & `Pulse3D-0.33.2/src/pulse3D/excel_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 from typing import Literal
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
-from pulse3D.transforms import get_time_window_indices
 from scipy import interpolate
 
 from .constants import *
 from .exceptions import *
 from .metrics import WellGroupMetric
+from .nb_peak_detection import noise_based_peak_finding
 from .peak_detection import concat
 from .peak_detection import data_metrics
 from .peak_detection import get_windowed_peaks_valleys
 from .peak_detection import init_dfs
-from .peak_detection import peak_detector
 from .plate_recording import PlateRecording
 from .plotting import plotting_parameters
 from .stimulation import aggregate_timepoints
 from .stimulation import realign_interpolated_stim_data
+from .transforms import get_time_window_indices
 from .utils import get_experiment_id
 from .utils import get_stiffness_label
 from .utils import truncate
 from .utils import truncate_float
 from .utils import xl_col_to_name
 
 
@@ -197,33 +197,39 @@
     plate_recording: PlateRecording,
     normalize_y_axis: bool = True,
     max_y: Union[int, float] = None,
     start_time: Union[float, int] = 0,
     end_time: Union[float, int] = np.inf,
     twitch_widths: Tuple[int, ...] = DEFAULT_TWITCH_WIDTHS,
     baseline_widths_to_use: Tuple[int, ...] = DEFAULT_BASELINE_WIDTHS,
-    prominence_factors: Tuple[Union[int, float], Union[int, float]] = DEFAULT_PROMINENCE_FACTORS,
-    width_factors: Tuple[Union[int, float], Union[int, float]] = DEFAULT_WIDTH_FACTORS,
+    noise_prominence_factor: Union[int, float] = DEFAULT_NB_NOISE_PROMINENCE_FACTOR,
+    relative_prominence_factor: Union[int, float] = DEFAULT_NB_RELATIVE_PROMINENCE_FACTOR,
+    width_factors: Tuple[Union[int, float], Union[int, float]] = DEFAULT_NB_WIDTH_FACTORS,
+    height_factor: Union[int, float] = DEFAULT_NB_HEIGHT_FACTOR,
+    max_frequency=None,
+    valley_search_duration=DEFAULT_NB_VALLEY_SEARCH_DUR,
+    upslope_duration=DEFAULT_NB_UPSLOPE_DUR,
+    upslope_noise_allowance_duration=DEFAULT_NB_UPSLOPE_NOISE_ALLOWANCE_DUR,
     peaks_valleys: Dict[str, List[List[int]]] = None,
     include_stim_protocols: bool = False,
     stim_waveform_format: Optional[Union[Literal["stacked"], Literal["overlayed"]]] = None,
 ):
     """Write plate recording waveform and computed metrics to Excel spredsheet.
 
     Args:
         plate_recording: loaded PlateRecording object
         normalize_y_axis: whether or not to set the max bound of the y-axis of all waveform graphs to the same value
         max_y: Sets the maximum bound for y-axis in the output graphs. Ignored if normalize_y_axis is False
         start_time: Start time of windowed analysis. Defaults to 0.
         end_time: End time of windowed analysis. Defaults to infinity.
         twitch_widths: Requested widths to add to output file
         baseline_widths_to_use: Twitch widths to use as baseline metrics
-        prominence_factors: factors used to determine the prominence peaks/valleys must have
-        width_factors: factors used to determine the width peaks/valleys must have
-        peaks_valleys: User-defined peaks and valleys to use instead of peak_detector
+        prominence_factor: factor used to determine the min prominence peaks must have
+        width_factors: factors used to determine the width peaks must have
+        peaks_valleys: User-defined peaks and valleys to use instead of peak detection results
         include_stim_protocols: Toggles the addition of stimulation-protocols sheet in the output excel
         stim_waveform_format: Toggles the output format of the stim waveforms if provided, o/w no waveforms are displayed
     Raises:
         NotImplementedError: if peak finding algorithm fails for unexpected reason
         ValueError: if start and end times are outside of expected bounds, or do not ?
     """
     # get metadata from first well file
@@ -336,14 +342,15 @@
         error_msg = None
 
         # necessary for concatenating DFs together, in event that peak-finding fails and produces empty DF
         dfs = init_dfs(twitch_widths_range=twitch_width_percents)
         metrics = tuple(
             concat([dfs[k][j] for j in dfs[k].keys()], axis=1) for k in ("per_twitch", "aggregate")
         )
+        peaks_and_valleys = (np.array([]), np.array([]))
 
         if well_file is None:
             continue
 
         well_index = well_file[WELL_INDEX_UUID]
         well_name = TWENTY_FOUR_WELL_PLATE.get_well_name_from_well_index(well_index)
 
@@ -380,17 +387,31 @@
         max_force_of_recording = max(max_force_of_recording, max_force_of_well)
 
         try:
             # compute peaks / valleys on interpolated well data
             log.info(f"Finding peaks and valleys for well {well_name}")
 
             if peaks_valleys is None:
-                log.info("No user defined peaks and valleys were found, so calculating with peak_detector")
-                peaks_and_valleys = peak_detector(
-                    interpolated_well_data, prominence_factors=prominence_factors, width_factors=width_factors
+                log.info("No user defined peaks and valleys were found, so finding peaks now")
+
+                # noise based peak finding requires the time values to be in seconds
+                well_data_for_peak_finding = np.array(
+                    [interpolated_well_data[0] / MICRO_TO_BASE_CONVERSION, interpolated_well_data[1]]
+                )
+
+                peaks_and_valleys = noise_based_peak_finding(
+                    well_data_for_peak_finding,
+                    noise_prominence_factor=noise_prominence_factor,
+                    relative_prominence_factor=relative_prominence_factor,
+                    width_factors=width_factors,
+                    height_factor=height_factor,
+                    max_frequency=max_frequency,
+                    valley_search_duration=valley_search_duration,
+                    upslope_duration=upslope_duration,
+                    upslope_noise_allowance_duration=upslope_noise_allowance_duration,
                 )
             else:
                 # convert peak and valley lists into a format compatible with find_twitch_indices
                 peaks, valleys = [np.array(peaks_or_valleys) for peaks_or_valleys in peaks_valleys[well_name]]
                 # get correct indices specific to windowed start and end
                 peaks_and_valleys = get_windowed_peaks_valleys(
                     window_start_idx, window_end_idx, peaks, valleys
```

### Comparing `Pulse3D-0.33.1/src/pulse3D/exceptions.py` & `Pulse3D-0.33.2/src/pulse3D/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,13 +49,17 @@
         super().__init__(back_to_back_points, feature_name="peak")
 
 
 class TooFewPeaksDetectedError(PeakDetectionError):
     pass
 
 
+class InvalidValleySearchDurationError(PeakDetectionError):
+    pass
+
+
 class NoRecordingFilesLoadedError(Exception):
     pass
 
 
 class SubprotocolFormatIncompatibleWithInterpolationError(Exception):
     pass
```

### Comparing `Pulse3D-0.33.1/src/pulse3D/magnet_finding.py` & `Pulse3D-0.33.2/src/pulse3D/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.1/src/pulse3D/metrics.py` & `Pulse3D-0.33.2/src/pulse3D/metrics.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.1/src/pulse3D/peak_detection.py` & `Pulse3D-0.33.2/src/pulse3D/peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.1/src/pulse3D/plate_recording.py` & `Pulse3D-0.33.2/src/pulse3D/plate_recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -544,26 +544,18 @@
             if self.wells[well_file[WELL_INDEX_UUID]] is not None:
                 raise DuplicateWellsFoundError(f"Duplicate well found for {well_file[WELL_NAME_UUID]}")
 
             self.wells[well_file[WELL_INDEX_UUID]] = well_file
 
     def to_dataframe(self, include_stim_data=True) -> pd.DataFrame:
         """Creates DataFrame from PlateRecording with all the data
-        interpolated, normalized, and scaled. The returned dataframe contains
-        one column for time in ms and one column for each well.
+        interpolated, normalized, and scaled.
 
-        The dataframe returned by this method can be used in calls to peak_detector by selecting the
-        'time' column and the well column that peak detection should be run on after transposing the
-        data, e.g.
-
-        >>> df = to_dataframe()
-        >>> peak_detector(df[['time', 'A1']].transpose().values)
-
-        The dataframe needs to be transposed before converting to NDArray because peak_detector
-        wants an ndarray of shape (2, N) while dataframe[['time', 'A1']] is in shape (N,2)
+        The returned dataframe contains one column for time in ms and
+        one column for each well.
         """
         # get first valid well and set interpolation period. Creating new iter to be safe
         first_well = next(iter(self))
 
         # add interpolated force timepoints
         if self._created_from_dataframe:
             raise NotImplementedError("Cannot export a DF if created from a DF. Just use the original")
```

### Comparing `Pulse3D-0.33.1/src/pulse3D/plotting.py` & `Pulse3D-0.33.2/src/pulse3D/plotting.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.1/src/pulse3D/stimulation.py` & `Pulse3D-0.33.2/src/pulse3D/stimulation.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.1/src/pulse3D/transforms.py` & `Pulse3D-0.33.2/src/pulse3D/transforms.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.1/src/pulse3D/utils.py` & `Pulse3D-0.33.2/src/pulse3D/utils.py`

 * *Files identical despite different names*

