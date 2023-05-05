# Comparing `tmp/gscipy-0.1.2.tar.gz` & `tmp/gscipy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gscipy-0.1.2.tar", last modified: Wed Apr  5 15:03:49 2023, max compression
+gzip compressed data, was "gscipy-0.1.3.tar", last modified: Fri May  5 11:10:58 2023, max compression
```

## Comparing `gscipy-0.1.2.tar` & `gscipy-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 15:03:49.198500 gscipy-0.1.2/
--rw-rw-rw-   0        0        0    17095 2022-12-14 10:37:12.000000 gscipy-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0    20525 2023-04-05 15:03:49.198500 gscipy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       55 2022-11-03 15:15:37.000000 gscipy-0.1.2/README.md
--rw-rw-rw-   0        0        0     1710 2023-04-05 15:03:10.000000 gscipy-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 15:03:49.199432 gscipy-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-05 15:03:49.152226 gscipy-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-05 15:03:49.172887 gscipy-0.1.2/src/gscipy/
--rw-rw-rw-   0        0        0        2 2023-01-05 22:19:22.000000 gscipy-0.1.2/src/gscipy/__init__.py
--rw-rw-rw-   0        0        0     5682 2023-01-11 15:19:15.000000 gscipy-0.1.2/src/gscipy/csv_io.py
--rw-rw-rw-   0        0        0      775 2023-01-11 09:29:40.000000 gscipy-0.1.2/src/gscipy/decorators.py
--rw-rw-rw-   0        0        0     2312 2023-04-04 14:48:36.000000 gscipy-0.1.2/src/gscipy/general.py
--rw-rw-rw-   0        0        0     6873 2023-01-17 15:49:12.000000 gscipy-0.1.2/src/gscipy/json_io.py
--rw-rw-rw-   0        0        0     8938 2023-04-04 14:48:36.000000 gscipy-0.1.2/src/gscipy/operators.py
--rw-rw-rw-   0        0        0    21953 2023-04-04 14:48:36.000000 gscipy-0.1.2/src/gscipy/signals.py
--rw-rw-rw-   0        0        0    13089 2023-04-04 14:48:36.000000 gscipy-0.1.2/src/gscipy/time.py
--rw-rw-rw-   0        0        0    20383 2023-04-04 14:48:36.000000 gscipy-0.1.2/src/gscipy/trajectories.py
--rw-rw-rw-   0        0        0     2987 2023-04-05 09:49:36.000000 gscipy-0.1.2/src/gscipy/utils.py
--rw-rw-rw-   0        0        0    17794 2023-04-04 14:48:36.000000 gscipy-0.1.2/src/gscipy/vectors.py
--rw-rw-rw-   0        0        0     4103 2023-04-05 13:11:11.000000 gscipy-0.1.2/src/gscipy/visualization.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:03:49.194860 gscipy-0.1.2/src/gscipy.egg-info/
--rw-rw-rw-   0        0        0    20525 2023-04-05 15:03:49.000000 gscipy-0.1.2/src/gscipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2023-04-05 15:03:49.000000 gscipy-0.1.2/src/gscipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 15:03:49.000000 gscipy-0.1.2/src/gscipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-04-05 15:03:49.000000 gscipy-0.1.2/src/gscipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-05 15:03:49.000000 gscipy-0.1.2/src/gscipy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 15:03:49.196856 gscipy-0.1.2/tests/
--rw-rw-rw-   0        0        0       34 2022-11-14 14:39:43.000000 gscipy-0.1.2/tests/test_data_io.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:10:58.886693 gscipy-0.1.3/
+-rw-rw-rw-   0        0        0    17095 2022-12-14 10:37:12.000000 gscipy-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    20525 2023-05-05 11:10:58.886191 gscipy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2022-11-03 15:15:37.000000 gscipy-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1710 2023-05-05 11:09:10.000000 gscipy-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 11:10:58.887194 gscipy-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 11:10:58.748727 gscipy-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 11:10:58.855614 gscipy-0.1.3/src/gscipy/
+-rw-rw-rw-   0        0        0        2 2023-01-05 22:19:22.000000 gscipy-0.1.3/src/gscipy/__init__.py
+-rw-rw-rw-   0        0        0      421 2023-04-06 13:52:32.000000 gscipy-0.1.3/src/gscipy/config.py
+-rw-rw-rw-   0        0        0     5682 2023-01-11 15:19:15.000000 gscipy-0.1.3/src/gscipy/csv_io.py
+-rw-rw-rw-   0        0        0      775 2023-01-11 09:29:40.000000 gscipy-0.1.3/src/gscipy/decorators.py
+-rw-rw-rw-   0        0        0     2312 2023-04-04 14:48:36.000000 gscipy-0.1.3/src/gscipy/general.py
+-rw-rw-rw-   0        0        0     6969 2023-04-15 22:24:08.000000 gscipy-0.1.3/src/gscipy/json_io.py
+-rw-rw-rw-   0        0        0     9000 2023-04-15 22:25:56.000000 gscipy-0.1.3/src/gscipy/operators.py
+-rw-rw-rw-   0        0        0    28233 2023-04-15 22:19:10.000000 gscipy-0.1.3/src/gscipy/signals.py
+-rw-rw-rw-   0        0        0    13336 2023-04-15 22:25:16.000000 gscipy-0.1.3/src/gscipy/time.py
+-rw-rw-rw-   0        0        0    20689 2023-04-15 22:23:18.000000 gscipy-0.1.3/src/gscipy/trajectories.py
+-rw-rw-rw-   0        0        0     3585 2023-04-15 14:24:09.000000 gscipy-0.1.3/src/gscipy/utils.py
+-rw-rw-rw-   0        0        0    17978 2023-04-15 22:27:23.000000 gscipy-0.1.3/src/gscipy/vectors.py
+-rw-rw-rw-   0        0        0     5158 2023-04-06 13:52:11.000000 gscipy-0.1.3/src/gscipy/visualization.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:10:58.877863 gscipy-0.1.3/src/gscipy.egg-info/
+-rw-rw-rw-   0        0        0    20525 2023-05-05 11:10:58.000000 gscipy-0.1.3/src/gscipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2023-05-05 11:10:58.000000 gscipy-0.1.3/src/gscipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 11:10:58.000000 gscipy-0.1.3/src/gscipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-05-05 11:10:58.000000 gscipy-0.1.3/src/gscipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 11:10:58.000000 gscipy-0.1.3/src/gscipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 11:10:58.884166 gscipy-0.1.3/tests/
+-rw-rw-rw-   0        0        0       34 2022-11-14 14:39:43.000000 gscipy-0.1.3/tests/test_data_io.py
```

### Comparing `gscipy-0.1.2/LICENSE.txt` & `gscipy-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.2/PKG-INFO` & `gscipy-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscipy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Gabba Scientific utilities
 Author: Matteo Gabba
 Author-email: m.gabba083@gmail.com
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
```

### Comparing `gscipy-0.1.2/pyproject.toml` & `gscipy-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 where = ["src"]  # ["."] by default
 # include = ["mypackage*"]  # ["*"] by default
 # exclude = ["mypackage.tests*"]  # empty by default
 # namespaces = false  # true by default
 
 [project]
 name = "gscipy"
-version = "0.1.2"
+version = "0.1.3"
 description = "Gabba Scientific utilities"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 keywords = ["gabba scientific", ]
 authors  =[
     {name = "Matteo Gabba"},
```

### Comparing `gscipy-0.1.2/src/gscipy/csv_io.py` & `gscipy-0.1.3/src/gscipy/csv_io.py`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.2/src/gscipy/decorators.py` & `gscipy-0.1.3/src/gscipy/decorators.py`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.2/src/gscipy/general.py` & `gscipy-0.1.3/src/gscipy/general.py`

 * *Files identical despite different names*

### Comparing `gscipy-0.1.2/src/gscipy/json_io.py` & `gscipy-0.1.3/src/gscipy/json_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,16 @@
             return json_dict
 
         else:
             try:
                 return obj.to_json()
             except AttributeError as error:
                 raise JsonIOInterfaceError(
-                    f"missing method to_json() in class: '{obj.__class__.__name__}'"
+                    f"missing method to_json() in class:"
+                    f" '{obj.__class__.__name__}'"
                 ) from error
             except TypeError:
                 pass
 
         # Let the base class default method raise the TypeError
         return super().default(obj)
 
@@ -117,15 +118,16 @@
 
         if hasattr(cls, "from_json"):
             obj = cls().from_json(json_dict)
             return obj
 
         else:
             raise JsonIOInterfaceError(
-                f"missing method from_json() in class: '{cls.__class__.__name__}'"
+                f"missing method from_json() in class:"
+                f" '{cls.__class__.__name__}'"
             )
 
 
 class JSONLoader:
     """Load JSON object using CustomJSONEncoder."""
 
     def __init__(self, input_path: Path) -> None:
@@ -173,15 +175,16 @@
 
         for key, value in json_dict.items():
 
             try:
                 getattr(obj, key)
             except AttributeError as error:
                 raise AttributeError(
-                    f"invalid attribute '{key}' for class: '{cls.__class__.__name__}'"
+                    f"invalid attribute '{key}' for class:"
+                    f" '{cls.__class__.__name__}'"
                 ) from error
 
             try:
                 __class__ = value.pop("__class__")
             except (KeyError, AttributeError, TypeError):
                 obj.__dict__[key] = value
                 continue
@@ -210,15 +213,16 @@
                         value, cls=CustomJSONDecoder
                     )
                 except TypeError:
                     pass
 
             elif not hasattr(_cls, "from_json"):
                 raise JsonIOInterfaceError(
-                    f"missing method from_json() in class: '{obj.__class__.__name__}'"
+                    f"missing method from_json() in class:"
+                    f" '{obj.__class__.__name__}'"
                 )
 
         # Let the base class default method raise the TypeError
         return obj
 
     def _get__class__(self) -> str:
         return ".".join([self.__module__, self.__class__.__name__])
```

### Comparing `gscipy-0.1.2/src/gscipy/operators.py` & `gscipy-0.1.3/src/gscipy/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,16 @@
         vectors.append(vector_i)
         times.append(time_i)
 
     return Trajectory(vectors, times)
 
 
 class BaseTrajectoryOperator(ABC):
-    """Represents a mathematical function or operation transforming (mapping) a time-series of 3D vectors."""
+    """Represents a mathematical function or operation transforming (mapping)
+     a time-series of 3D vectors."""
 
     @abstractmethod
     def __init__(self, *args, **kwargs) -> None:
         # Instantiate args and kwargs
         # self.args = args, self.kwargs = kwargs
         ...
 
@@ -176,15 +177,16 @@
             x_refilled, y_refilled, z_refilled, time
         )
 
         return r_refilled
 
 
 class SequentialPipeline(BaseTrajectoryOperator):
-    """Process the input trajectory sequentially using a list of Operator(s) instances."""
+    """Process the input trajectory sequentially using a list of Operator(s)
+     instances."""
 
     def __init__(self, steps: list[BaseTrajectoryOperator]) -> None:
         self.steps = steps
 
     def transform(self, trajectory: Trajectory) -> Trajectory:
         transformed_trajectory = trajectory
 
@@ -197,19 +199,21 @@
         """Get single operator (by indexing) or sub-pipeline (by slicing)."""
         if isinstance(index, slice):
             return SequentialPipeline(self.steps[index])
         elif isinstance(index, int):
             return self.steps[index]
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(steps={[operator for operator in self.steps]})"
+        return f"{self.__class__.__name__}" \
+               f"(steps={[operator for operator in self.steps]})"
 
 
 class ParallelPipeline(BaseTrajectoryOperator):
-    """Process one input trajectory to many output trajectories using a list of Operator(s) instances."""
+    """Process one input trajectory to many output trajectories using a list of
+     Operator(s) instances."""
 
     def __init__(self, operators: list[BaseTrajectoryOperator]) -> None:
         self.operators = operators
 
     def transform(self, trajectory: Trajectory) -> list[Trajectory]:
 
         trajectories = [trajectory]
@@ -224,15 +228,16 @@
         """Get single operator (by indexing) or sub-pipeline (by slicing)."""
         if isinstance(index, slice):
             return ParallelPipeline(self.operators[index])
         elif isinstance(index, int):
             return self.operators[index]
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(operators={[operator for operator in self.operators]})"
+        return f"{self.__class__.__name__}" \
+               f"(operators={[operator for operator in self.operators]})"
 
 
 class NthVectorDiff(SequentialPipeline):
     def __init__(self, kernel_half_size: int = 1, order: int = 1):
 
         pipeline_steps = [
             VectorFirstDiff(kernel_half_size) for _ in range(order)
```

### Comparing `gscipy-0.1.2/src/gscipy/signals.py` & `gscipy-0.1.3/src/gscipy/signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,71 +19,133 @@
 
 from gscipy.general import TypeCheckedList
 from gscipy.utils import _isnan, cluster_size_generator
 
 
 @dataclass
 class Peak:
+    """Represents a peak detected from the analysis of a signal.
+
+    Parameters
+    ----------
+    is_type : str, optional, default to "unknown"
+        Peak label name.
+
+    index : int, optional, default to None
+        Index of the signal array corresponding to the peak contour
+        maximum.
+
+    position : float, optional, default to NaN
+        x-position of the peak contour maximum.
+
+    fwhm : float, optional, default to None
+        Full-width-half-maximum of the peak contour.
+
+    std : float, optional, default to None
+        Standard deviation of the peak contour under the assumption
+            of a gaussian peak: std = fwhm / 2.355.
+
+    width_height : float, optional, default to None
+        The peak contour height at which the fwhm is evaluated.
+
+    width_start : float, optional, default to None
+        Interpolated position of the left intersection point between the
+        peak contour line and the fwhm horizontal line.
+
+    width_end : float, optional, default to None
+        Interpolated position of the right intersection point between the
+        peak contour line and the fwhm horizontal line.
+
+    height : float, optional, default to None
+        Maximum peak contour height.
+
+    contour_height : float, optional, default to None
+        Height of the contour baseline at the maximum peak position.
+
+    prominence : float, optional, default to None
+        Peak contour height with respect to the baseline contour both
+        evaluated at the maximum peak position:
+        prominence = height - contour_height
+    """
+
     is_type: str = "unknown"
     index: int = None
-    position: float = None
+    position: float = np.nan
     fwhm: float = None
     std: float = None
     width_height: float = None
     width_start: float = None
     width_end: float = None
     height: float = None
     contour_height: float = None
     prominence: float = None
 
     @property
     def area(self) -> float:
-        """See: # https://www.savarese.org/math/gaussianintegral.html#S3.E20."""
+        """Area under the peak computed under the assumption of having a
+         gaussian peak.
+
+        Notes
+        -----
+        About calculation of the peak area:
+        <https://www.savarese.org/math/gaussianintegral.html#S3.E20.>
+        """
         return self.prominence * self.std * np.sqrt(2 * math.pi)
 
     def __lt__(self, other: Peak) -> bool:
+        """Sort peaks according to position."""
         if isinstance(other, Peak):
             return self.position < other.position
         return NotImplemented
 
     def __eq__(self, other: Peak) -> bool:
+        """Compare peaks according to: index, position, fwhm and height."""
         if isinstance(other, Peak):
             return (
                 (self.index == other.index)
                 & (self.position == other.position)
                 & (self.fwhm == other.fwhm)
                 & (self.height == other.height)
             )
         return NotImplemented
 
     def __ne__(self, other: Peak) -> bool:
+        """Determine peaks inequality."""
         return not self == other
 
     def __hash__(self):
+        """Return hash value."""
         return hash((self.is_type, self.position, self.std, self.height))
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(type={self.is_type}, position={self.position:.1f})"
+        return (
+            f"{self.__class__.__name__}"
+            f"(type={self.is_type}, position={self.position:.1f})"
+        )
 
 
 class PeaksList(TypeCheckedList):
+    """Represents a list of peaks obtained from the analysis of a signal.
+
+    Parameters
+    ----------
+    iterator_arg : Iterable[Peak], optional, default to None.
+        List of Peak instances.
+    """
+
     def __init__(
         self,
         iterator_arg: Iterable[Peak] = None,
     ):
-        """
-        Iterator_arg : List[Peak], optional, default to None.
-
-            List of Peak
-        """
         # Initialize the parent class to type check for Peak instances
         super().__init__(iterator_arg=iterator_arg, instance_type=Peak)
 
     @property
     def indexes(self) -> np.ndarray:
+        """Indexes of the signal array corresponding to the peak's maxima."""
         return np.array([peak.index for peak in self])
 
     @property
     def positions(self) -> np.ndarray:
         return np.array([peak.position for peak in self])
 
     @property
@@ -123,14 +185,33 @@
         return np.array([peak.area for peak in self])
 
     def compute_features(
         self,
         y: np.ndarray,
         x: np.ndarray,
     ) -> None:
+        """Compute features of peaks in the PeaksList.
+
+        Parameters
+        ----------
+        y : np.ndarray, (N,)
+            y-values of the signal used to populate the PeaksList.
+
+        x : np.ndarray, (N,)
+            x-values of the signal used to populate the PeaksList.
+
+        Returns
+        -------
+            None
+
+        See Also
+        --------
+        gscipy.signals.compute_peaks_width_features
+        gscipy.signals.compute_peaks_height_features
+        """
         compute_peaks_width_features(
             y,
             x,
             self,
         )
 
         compute_peaks_height_features(
@@ -141,15 +222,36 @@
     def detect(
         self,
         y: np.ndarray,
         x: np.ndarray,
         min_peak_prominence: float,
         min_inter_peak_distance: float,
     ) -> None:
-        """Populate input list with detected peaks."""
+        """Populate PeaksList with peaks detected from signal.
+
+        Parameters
+        ----------
+        y : numpy.ndarray, (N,)
+            Signal y-values.
+
+        x : numpy.ndarray, (N,)
+            Signal x-values.
+
+        min_peak_prominence : float
+            Required minimal prominence of peaks.
+
+        min_inter_peak_distance : float
+            Required minimal horizontal distance between neighbouring peaks.
+             Smaller peaks are removed first until the condition is fulfilled
+              for all remaining peaks.
+
+        See Also
+        --------
+        scipy.signal.find_peaks
+        """
         inter_sample_distance = x[1] - x[0]
         min_inter_peak_distance_cts = int(
             min_inter_peak_distance / inter_sample_distance
         )
 
         peaks_indexes, _ = signal.find_peaks(
             y,
@@ -164,14 +266,36 @@
 
 
 def compute_peaks_width_features(
     y: np.ndarray,
     x: np.ndarray,
     peaks: PeaksList,
 ) -> None:
+    """Compute width-related features of peaks in PeaksList:
+    fwhm, std, width_height, width_start and width_end.
+
+    Parameters
+    ----------
+    y : np.ndarray, (N,)
+        y-values of the signal used to populate 'peaks'.
+
+    x : np.ndarray, (N,)
+        x-values of the signal used to populate 'peaks'.
+
+    peaks : PeaksList
+        List of peaks detected from signal (x, y).
+
+    Returns
+    -------
+    None.
+
+    See Also
+    --------
+    scipy.signal.peak_widths
+    """
     inter_sample_distance = x[1] - x[0]
     x0 = x[0]
 
     results_fwhm = signal.peak_widths(
         y,
         peaks.indexes,
         rel_height=0.5,
@@ -190,95 +314,125 @@
         peak.width_end = width_ends[n]
 
 
 def compute_peaks_height_features(
     y: np.ndarray,
     peaks: PeaksList,
 ) -> None:
+    """Compute height-related features of peaks in PeaksList:
+    prominence, contour_height and height.
+
+    Parameters
+    ----------
+    y : np.ndarray, (N,)
+         y-values of the signal used to populate 'peaks'.
+
+    peaks : PeaksList
+        List of peaks detected from signal (x, y).
+
+    Returns
+    -------
+        None.
+
+    See Also
+    --------
+    scipy.signal.peak_prominences
+    """
     prominences = signal.peak_prominences(y, peaks.indexes)[0]
     contour_heights = y[peaks.indexes] - prominences
     heights = y[peaks.indexes]
 
     for n, peak in enumerate(peaks):
         peak.prominence = prominences[n]
         peak.contour_height = contour_heights[n]
         peak.height = heights[n]
 
 
 def get_weights(n_train: int, n_steps: int) -> np.ndarray:
-    """
-    Compute weights (reliability) of predicted values.
+    """Compute weights (reliability) of predicted values.
 
     Parameters
     ----------
-        n_train : int
-            Number of points used for training the AR-model and making predictions.
+    n_train : int
+        Number of points used for training the AR-model and making
+            predictions.
 
-        n_steps : int
-            Number of predicted points.
+    n_steps : int
+        Number of predicted points.
 
     Returns
     -------
         w : np.ndarray
-            Weights indicating the reliability of the predicted values, dim(n_steps,).
-            The weights are linearly proportional to the number of points used for the prediction
-            and inversely proportional to the number of steps into the future.
-    """
-    # Total weights: are linearly proportional to the number of points used for the prediction
-    # and inversely proportional to the number of steps into the future
+            Weights indicating the reliability of the predicted values,
+             dim(n_steps,). The weights are linearly proportional to the number
+              of points used for the prediction and inversely proportional
+              to the number of steps into the future.
+    """
+    # Total weights: are linearly proportional to the number of points used
+    # for the prediction and inversely proportional to the number of steps
+    # into the future
     linear_w = np.arange(1, n_steps + 1)[::-1]
 
     return n_train * linear_w
 
 
 def autoregress_predict(
     seg: np.ndarray, n_steps: int, max_lag: int
 ) -> np.ndarray:
-    """
-    Predict (forecast) n-steps into the future using an autoregressive (AR) model that minimizes the Akaike information.
-
-     criterion (AIC).
+    """Predict (forecast) n-steps into the future using an autoregressive
+     (AR) model that minimizes the Akaike information criterion (AIC).
      # TODO: implement possibility to choose the width of the region for prediction.
 
-    See:
-        https://www.statsmodels.org/devel/examples/notebooks/generated/autoregressions.html
-        https://vitalflux.com/autoregressive-ar-models-with-python-examples/#:~:text=Autoregressive%20(AR)%20models%20are%20a,order%20to%20make%20accurate%20predictions.
-        https://machinelearningmastery.com/autoregression-models-time-series-forecasting-python/
-
     Parameters
     ----------
-        seg : np.ndarray
-            Segment of a time-series used for training the AR-model.
+    seg : np.ndarray
+        Segment of a time-series used for training the AR-model.
 
-        n_steps : np.ndarray
-            Forecast n-steps into the future based on the past behavior of the time-series.
+    n_steps : np.ndarray
+        Forecast n-steps into the future based on the past behavior of the
+            time-series.
 
-        max_lag : int
-            Select max lag for automatic selection of the lags structure.
-            See: https://www.statsmodels.org/devel/generated/statsmodels.tsa.ar_model.ar_select_order.html
+    max_lag : int
+        Select max lag for automatic selection of the lags structure.
 
     Returns
     -------
-        prediction : np.ndarray
-            Array of len = n_steps with AR-predicted values.
+    prediction : np.ndarray
+        Array of len = n_steps with AR-predicted values.
+
+    See Also
+    --------
+    statsmodels.tsa.stattools.adfuller
+    statsmodels.tsa.ar_model.ar_select_order
+
+    Notes
+    -----
+    About AR-model:
+        <https://www.statsmodels.org/devel/examples/notebooks/generated/autoregressions.html>
+        <https://vitalflux.com/autoregressive-ar-models-with-python-examples/#:~:text=Autoregressive%20(AR)%20models%20are%20a,order%20to%20make%20accurate%20predictions.>
+        <https://machinelearningmastery.com/autoregression-models-time-series-forecasting-python/>
+
+    About automatic max_lag selection:
+        <https://www.statsmodels.org/devel/generated/statsmodels.tsa.ar_model.ar_select_order.html>
     """
     # Number of points used for training of the AR-model
     n_samples = len(seg)
 
     # Check for stationarity of the time-series data
-    # We will look for p-value. In case, p-value is less than 0.05, the time series
-    # data can be said to have stationarity
+    # We will look for p-value. In case, p-value is less than 0.05,
+    # the time series data can be said to have stationarity
     df_stationarityTest = adfuller(seg, autolag="AIC")
     p_value = df_stationarityTest[1]
 
-    # Raise warning if time-series segment used for prediction is not stationary
+    # Raise warning if time-series segment used for prediction is not
+    # stationary
     if p_value > 0.05:
         warnings.warn(
-            "P-value = {} is > 0.05! The time-series segment used for prediction may "
-            "not be stationary!".format(p_value)
+            "P-value = {} is > 0.05! The time-series segment used"
+            " for prediction may not be stationary!".format(p_value)
         )
 
     # Automatically select AR-model lag
     select = ar_select_order(seg, ic="aic", maxlag=max_lag)
 
     # Train AR-model
     trained_model = select.model.fit()
@@ -288,33 +442,34 @@
         start=n_samples, end=n_samples + n_steps - 1, dynamic=True
     )
 
     return prediction
 
 
 def find_gaps_and_segments(x: np.ndarray | list[float]) -> list[np.ndarray]:
-    """
-    Get indexes of gaps (of NaN's) and segments (not-NaN) in the input array.
+    """Get indexes of gaps (of NaN's) and segments (not-NaN) in the input
+     array.
 
     Parameters
     ----------
         x : array-like
             Array with NaN gaps.
 
     Returns
     -------
-        A list of indexes arrays corresponding to the segments and gaps in the input array.
+        A list of indexes arrays corresponding to the segments and gaps in the
+         input array.
     """
     # Get indexes of segments (not-NaN) and gaps (NaN) in the array
     return [idx for (value, _, idx) in cluster_size_generator(np.isnan(x))]
 
 
 def gap_is_first(x: np.ndarray | list[float]) -> bool:
-    """
-    Check if a gap (of NaN's) or a segment is in first position of the input array.
+    """Check if a gap (of NaN's) or a segment is in first position of the
+     input array.
 
     Parameters
     ----------
         x : array-like
             Array with NaN gaps.
 
     Returns
@@ -329,43 +484,50 @@
     return False
 
 
 def autoregress_fill(
     x: np.ndarray, max_lag: int
 ) -> tuple[np.ndarray, np.ndarray]:
     """
-    Fill gaps of NaN's in a time-series using an autoregressive model that minimizes the Akaike information.
+    Fill gaps of NaN's in a time-series using an autoregressive model that
+     minimizes the Akaike information.
 
     criterion (AIC).
-    # TODO: implement possibility to choose the width of the region for prediction.
+    # TODO: implement possibility to choose the width of the region
+    # for prediction.
 
     Parameters
     ----------
         x : array-like
             Array with NaN gaps, dim(n,).
 
         max_lag : int
             Select max lag for automatic selection of the lags structure.
 
     Returns
     -------
         y : np.ndarray
-            A copy of the input array with gaps filled with the AR-predicted values, dim(n,).
+            A copy of the input array with gaps filled with the AR-predicted
+             values, dim(n,).
 
         w : np.ndarray
-            Weights indicating the reliability of the predicted values, dim(n,).
+            Weights indicating the reliability of predicted values, dim(n,).
+
+    See Also
+    --------
+    gscipy.signals.find_gaps_and_segments
     """
     # Copy input array
     y = np.copy(x)
 
     # Initialize weights
     w = np.ones_like(x)
 
-    # Get labels and indexes of NaN gaps (label: True) and segments (label: False)
-    # in the input array
+    # Get labels and indexes of NaN gaps (label: True) and segments
+    # (label: False) in the input array
     idx = find_gaps_and_segments(y)
 
     # Total number of segments and gaps
     n = len(idx)
 
     # Initialize variables
     idx_first_seg = 0
@@ -391,15 +553,16 @@
 
     # array starts with a segment
     elif not gap_is_first(y):
 
         # position of the first segment in the array
         idx_first_seg = 0
 
-    # Predict from segment immediately prior to the gap starting from first segment in the array
+    # Predict from segment immediately prior to the gap starting from first
+    # segment in the array
     for i in range(idx_first_seg, n - 1, 2):
 
         # get segment and gap indexes
         idx_seg = idx[i]
         idx_gap = idx[i + 1]
 
         # initialize segment and gap arrays with right length
@@ -422,120 +585,158 @@
         # fill gap with predicted values
         y[idx_gap] = prediction
         w[idx_gap] = w_i
 
     return y, w
 
 
-def refill_gaps(x: np.ndarray, max_lag: int) -> np.ndarray:
-    """
-    Replaces NaN values of an input vector, X, by fitting an autoregressive (AR) model that.
+def refill_gaps(
+    x: np.ndarray,
+    max_lag: int,
+) -> np.ndarray:
+    """Replaces NaN values of an input vector.
 
-    minimizes the Akaike information criterion. Each NaN value is replaced by a weighted average
-    of the values estimated by forward and backward prediction.
+    Replacement is performed by fitting an autoregressive (AR) model that
+     minimizes the Akaike information criterion. Each NaN value is replaced by
+      a weighted average of the values estimated by forward and backward
+       prediction.
 
     # TODO: implement possibility to choose the width of the region for prediction.
 
     Parameters
     ----------
         x : array-like
             Array with NaN gaps, dim(n,).
 
         max_lag : int
             Select max lag for automatic selection of the lags structure.
 
     Returns
     -------
         y : np.ndarray
-            A copy of the input array with NaN gaps refilled with AR-predicted values.
+            A copy of the input array with NaN gaps refilled with AR-predicted
+             values.
     """
     # Refill NaN's gaps in forward direction
     x_fwd, w_fwd = autoregress_fill(x, max_lag)
 
     # Refill NaN's gaps in backward direction
     x_bwd, w_bwd = autoregress_fill(x[::-1], max_lag)
 
     # Invert refilled array
     x_bwd = x_bwd[::-1]
     w_bwd = w_bwd[::-1]
 
-    # Compute weighted average of the refilled arrays in backward and forward directions
+    # Compute weighted average of the refilled arrays in backward and
+    # forward directions
     y = (x_bwd * w_bwd + x_fwd * w_fwd) / (w_bwd + w_fwd)
 
     return y
 
 
 def cumulative_integral(
     y: np.ndarray,
     x: np.ndarray = None,
     dx: float = None,
     max_lag: int = 5,
 ) -> np.ndarray:
+    """Compute cumulative integral of signal.
+
+    NaN values are refilled with an autoregressive model before computation
+    of the integral.
+    The numerical integration is computed using the trapezoidal method.
+
+    Parameters
+    ----------
+    y, x : array-like, (N,)
+        Signal y and x values.
+
+    dx : float
+        inter-sample increment of the x-array.
+
+    max_lag : float, optional, default to 5
+        Select max lag for automatic selection of the lags structure.
+
+    Returns
+    -------
+    np.ndarray, (N,)
+
+    See Also
+    --------
+    gscipy.signals.refill_gaps
+    gscipy.signals.cumulative_trapezoid
+    """
     y_filled = refill_gaps(y, max_lag)
     return cumulative_trapezoid(y_filled, x, dx, initial=0)
 
 
 def central_diff(
     y: np.ndarray | list[float],
     axis: int = -1,
     kernel_half_size: int = 1,
 ) -> np.ndarray:
     """
-    Compute sum of central finite differences of input array along the given axis using a convolution kernel.
+    Compute sum of central finite differences of input array along the given
+    axis using a convolution kernel.
 
-    The half width M of the kernel determines the number of terms in the summation:
-    dy[i] = sum_m (dy[i+m] - dy[i-m]) with m in [-M, M].
+    The half width M of the kernel determines the number of terms in the
+    summation: dy[i] = sum_m (dy[i+m] - dy[i-m]) with m in [-M, M].
 
-    See: https://numpy.org/doc/stable/reference/generated/numpy.convolve.html
-
-    Keep in mind that: "the convolution operator flips the second array before “sliding” the two across one another."
+    Keep in mind that: "the convolution operator flips the second array before
+    “sliding” the two across one another."
 
     Parameters
     ----------
         y : array-like
             One or multidimensional array.
 
         axis : int
-            The axis along which the difference is taken, default is the last axis.
+            The axis along which the difference is taken, default is the last
+             axis.
 
         kernel_half_size : int
-            Half size M of the family of convolution kernels: g[m] = [1, 0, -1], [1, 1, 0, -1, -1], ...
+            Half size M of the family of convolution kernels:
+             g[m] = [1, 0, -1], [1, 1, 0, -1, -1], ...
 
     Returns
     -------
         dy : np.ndarray
-        The summation of the m-th central finite differences of the input array:
-        dy[i] = sum_m (dy[i+m] - dy[i-m]) with m in [-M, M]
-        The output array is padded with NaN along the chosen axis to keep the same dimensions of the input array.
-
-    Version history
-    ---------------
-        v1 : 18-05-2022 (m.gabba)
+        The summation of the m-th central finite differences of the input
+         array: dy[i] = sum_m (dy[i+m] - dy[i-m]) with m in [-M, M]
+        The output array is padded with NaN along the chosen axis to keep the
+         same dimensions of the input array.
+
+    Notes
+    -----
+    About convolution:
+        <https://numpy.org/doc/stable/reference/generated/numpy.convolve.html>
     """
     assert (
         kernel_half_size > 0
     ), "kernel_half_size: must be a not-zero positive integer!"
 
     # Base convolution kernel
     base_kernel = [0]
 
-    # Create convolution kernel for calculation of central difference with chosen half-width histrange: M // 2
+    # Create convolution kernel for calculation of central difference with
+    # chosen half-width histrange: M // 2
     kernel = np.pad(
         base_kernel,
         pad_width=kernel_half_size,
         mode="constant",
         constant_values=[1, -1],
     )
 
     # Apply convolution kernel along the given axis
     dy = np.apply_along_axis(
         lambda m: np.convolve(m, kernel, mode="valid"), axis=axis, arr=y
     )
 
-    # Pad with NaN along the given axis to keep the same dimensions of the input array.
+    # Pad with NaN along the given axis to keep the same dimensions of the
+    # input array.
     dy_padded = np.apply_along_axis(
         lambda m: np.pad(
             m,
             pad_width=kernel_half_size,
             mode="constant",
             constant_values=np.nan,
         ),
@@ -547,60 +748,88 @@
 
 
 def smooth_signal_by_differentiation_and_reintegration(
     y: np.ndarray,
     x: np.ndarray,
     kernel_half_size: int,
 ) -> np.ndarray:
+    """Smooth a signal performing numerical differentiation and re-integration.
+
+    The signal is differentiated by means of the central difference
+    algorithme and re-integrated with the cumulative trapezoidal method.
+
+    Parameters
+    ----------
+    y, x : array-like, (N,)
+        Signal y and x values.
+
+    kernel_half_size : int
+        Half size M of the convolution kernel used for numerical
+        differentiation of the signal.
+
+    Returns
+    -------
+    np.ndarray, (N,)
+        Smoothed signal.
+
+    See Also
+    --------
+    gscipy.signals.central_diff
+    gscipy.signals.cumulative_integral
+    """
     delta_y = central_diff(y, kernel_half_size=kernel_half_size)
     delta_x = central_diff(x, kernel_half_size=kernel_half_size)
     derivative = delta_y / delta_x
     return cumulative_integral(derivative, x)
 
 
 def correlation(
     sig1: np.ndarray | list[float],
     sig2: np.ndarray | list[float],
     freq: float,
     normed: bool,
 ) -> tuple[np.ndarray, np.ndarray, float]:
-    """
-    Compute correlation between two signals.
-
-    See:
-        https://en.wikipedia.org/wiki/Cross-correlation
-        https://scicoding.com/cross-correlation-in-python-3-popular-packages/
-        https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.correlate.html
+    """Compute correlation between two signals.
 
     Parameters
     ----------
         sig1, sig2 : array-like
-            Signal(s) to correlate. If sig1=sig2 returns the auto-correlation; otherwise,
-            the cross-correlation.
+            Signal(s) to correlate. If sig1=sig2 returns the auto-correlation;
+             otherwise, the cross-correlation.
 
         freq : float
             Sampling frequency of the input signal(s).
 
         normed : bool
-            If True return the normalized correlation with values between [-1, 1]
-            as per definition; if False, the not-normalized correlation.
+            If True return the normalized correlation with values between
+             [-1, 1] as per definition; if False, the not-normalized
+              correlation.
 
     Returns
     -------
         corr, lag_times, lags, lag : tuple
-            The correlation function, the lag times and the lag time corresponding to the max
-            correlation.
+            The correlation function, the lag times and the lag time
+             corresponding to the max correlation.
+
+    See Also
+    --------
+    About normalization of the correlation function:
+        <https://en.wikipedia.org/wiki/Cross-correlation>
+        <https://scicoding.com/cross-correlation-in-python-3-popular-packages/>
+        <ttps://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.correlate.html>
     """
     # Length of the signals
     n1 = len(sig1)
     n2 = len(sig2)
 
     # Length of longer signal
     N = np.max([n1, n2])
 
+    corr = np.empty([0])
+
     if normed:
 
         # subtract mean signal value
         nsig1 = sig1 - np.mean(sig1)
         nsig2 = sig2 - np.mean(sig2)
 
         # correlate normed signals
@@ -632,71 +861,86 @@
 
 def wavelet_filter(
     signal: np.ndarray,
     wavelet_type: str,
     extension_mode: str,
     filtered_levels: tuple[int, ...],
 ) -> tuple[np.ndarray, list[float]]:
-    """
-    Filter signal with discrete wavelet transformation (DWT) and reconstruction.
-
-    See : https://ataspinar.com/2018/12/21/a-guide-for-using-the-wavelet-transform-in-machine-learning/
+    """Filter signal with discrete wavelet transformation (DWT) and
+     reconstruction.
 
     Parameters
     ----------
         signal : np.ndarray
             Input data series.
 
         wavelet_type : wavelet object or str
             Valid discrete wavelet type.
-                See :
-                    https://pywavelets.readthedocs.io/en/latest/ref/wavelets.html
-                    http://wavelets.pybytes.com/wavelet/
 
         extension_mode : str
             Signal extension mode.
-                See : https://pywavelets.readthedocs.io/en/latest/ref/signal-extension-modes.html#ref-modes
 
         filtered_levels : tuple
-            Choose decomposition levels to remove from signal reconstruction in order to filter specific frequencies.
-            Levels are positive integers. Low values corresponds to high-frequency wavelets, high values to
-             low-frequency wavelets. Thus, removing low (high) value levels corresponds to a  low(high)pass wavelet
-              filter.
-                See : https://pywavelets.readthedocs.io/en/latest/ref/idwt-inverse-discrete-wavelet-transform.html
+            Choose decomposition levels to remove from signal reconstruction
+             in order to filter specific frequencies. Levels are positive
+              integers. Low values corresponds to high-frequency wavelets,
+               high values to low-frequency wavelets. Thus, removing low (high)
+                value levels corresponds to a  low(high)pass wavelet filter.
 
     Returns
     -------
         reconstructed_signal : np.ndarray
-            The input signal after wavelet decomposition and recomposition with filtered coefficients.
+            The input signal after wavelet decomposition and recomposition with
+             filtered coefficients.
 
-         coefficients : List
+         coefficients : list
             The wavelet decomposition coefficients after filtering.
 
-    Version history
-    ---------------
-        v1 : 18-05-2022 (m.gabba)
-    """
-    # Discrete wavelet transformation DWT of signal with automatic selection of the decomposition level
-    # See: https://pywavelets.readthedocs.io/en/latest/ref/dwt-discrete-wavelet-transform.html
-    # The output coefficients are ordered as follows: [cA_n, cD_n, cD_n-1, …, cD2, cD1] with decreasing level order
+    See Also
+    --------
+    PyWavelets.pwavedec
+    PyWavelets.waverec
+
+    Notes
+    --------
+    About discrete and continuous wavelet transformation:
+        <ttps://ataspinar.com/2018/12/21/a-guide-for-using-the-wavelet-transform-in-machine-learning/>
+
+    About wavelet types:
+        <https://pywavelets.readthedocs.io/en/latest/ref/wavelets.html>
+        <http://wavelets.pybytes.com/wavelet/>
+
+    About signal extension modes:
+        <https://pywavelets.readthedocs.io/en/latest/ref/signal-extension-modes.html#ref-modes>
+
+    About the interpretation of filtered_levels
+        <https://pywavelets.readthedocs.io/en/latest/ref/idwt-inverse-discrete-wavelet-transform.html>
+
+    About the output 'coefficients'
+        <https://pywavelets.readthedocs.io/en/latest/ref/dwt-discrete-wavelet-transform.html>
+    """
+    # Discrete wavelet transformation DWT of signal with automatic selection
+    # of the decomposition level
+    # The output coefficients are ordered as follows:
+    # [cA_n, cD_n, cD_n-1, …, cD2, cD1] with decreasing level order
     coefficients = wavedec(
         signal, wavelet_type, mode=extension_mode, level=None
     )
 
     # Set to zero coefficients at the chosen levels
     for level in filtered_levels:
         coefficients[-level] = np.zeros_like(coefficients[-level])
 
     # Reconstruct wavelet filtered signal
     reconstructed_signal = waverec(
         coefficients, wavelet_type, mode=extension_mode
     )
 
-    # Handle issues with reconstructed signal longer than the original signal, I don't understand the origin of
-    # this behavior!!
+    # Handle issues with reconstructed signal longer than the original signal,
+    # I don't understand the origin of this behavior!!
 
     # If the reconstructed signal is longer than the original signal
     if len(reconstructed_signal) > len(signal):
         # remove last point
         reconstructed_signal = reconstructed_signal[:-1]
 
     return reconstructed_signal, coefficients
```

### Comparing `gscipy-0.1.2/src/gscipy/time.py` & `gscipy-0.1.3/src/gscipy/time.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,18 @@
     >>> t = Time(1)
     >>> t
     Time(1)
     >>> t.time = 2
     >>> t
     Time(2)
 
-    Magic methods for addition, subtraction, multiplication, division, rising to the power, abs()
-    and comparison (<, <=, ==, !=, >=, >) of Time instances or a Time instance with a constant (int, float)
-    are implemented.
+    Magic methods for addition, subtraction, multiplication, division,
+     rising to the power, abs() and comparison (<, <=, ==, !=, >=, >)
+      of Time instances or a Time instance with a constant (int, float)
+      are implemented.
     """
 
     # __slots__ = ["time", "_time_str"]
 
     # Default string format for string parsing to a timestamp
     _time_str = "%Y-%m-%d %H:%M:%S.%f%Z"
 
@@ -66,17 +67,20 @@
         """
         ---
 
             value : (datetime, float, int, str), optional, default to 0
         """
         if not isinstance(value, (datetime, float, int, str)):
             raise TypeError(
-                f"{self.__class__.__name__}() argument must be a timestamp ('float' or 'int'), a datetime"
-                f" that can be converted to one, or a string of the format {self.__class__._time_str}"
-                f" that can be parsed into one, not '{value.__class__.__name__}'"
+                f"{self.__class__.__name__}() argument must be a timestamp"
+                f" ('float' or 'int'), a datetime"
+                f" that can be converted to one, or a string of the format"
+                f" {self.__class__._time_str}"
+                f" that can be parsed into one,"
+                f" not '{value.__class__.__name__}'"
             )
         self._time = value
         self.time = self._time
 
     @classmethod
     def from_json(cls, json_dict: CustomJSONDict) -> Time:
         return cls(json_dict["time"])
@@ -94,49 +98,56 @@
         >>> t.time
         1
         """
         return self._time
 
     @time.setter
     def time(self, value: float | int | str | datetime) -> None:
-        """Set time property from a datetime instance, a timestamp (float, int) or a timestamp-convertible string.
+        """Set time property from a datetime instance, a timestamp (float, int)
+         or a timestamp-convertible string.
 
         >>> t = Time(1)
         >>> t.time = 2
         >>> t.time
         2
         >>> t
         Time(2)
 
         Parameters
         ----------
          value : (float, int, str, datetime), required
         """
         if not isinstance(value, (datetime, float, int, str)):
             raise TypeError(
-                f"{self.__class__.__name__}() argument must be a timestamp ('float' or 'int'), a datetime"
-                f" that can be converted to one, or a string of the format {self.__class__._time_str}"
-                f" that can be parsed into one, not '{value.__class__.__name__}'"
+                f"{self.__class__.__name__}() argument must be a timestamp"
+                f" ('float' or 'int'), a datetime"
+                f" that can be converted to one, or a string of the format"
+                f" {self.__class__._time_str}"
+                f" that can be parsed into one,"
+                f" not '{value.__class__.__name__}'"
             )
 
         if isinstance(value, datetime):
             try:
                 value = value.timestamp()
             except Exception as error:
                 raise ValueError(
-                    f"{self.__class__.__name__}() could not create a valid timestamp from 'value'"
+                    f"{self.__class__.__name__}()"
+                    f" could not create a valid timestamp from 'value'"
                 ) from error
 
         elif isinstance(value, str):
             try:
                 value = to_datetime(value).timestamp()
             except Exception as error:
                 raise ValueError(
-                    f"{self.__class__.__name__}() could not parse a valid timestamp "
-                    f"from 'value' \n (provide a string with format: {self._time_str})"
+                    f"{self.__class__.__name__}"
+                    f"() could not parse a valid timestamp "
+                    f"from 'value' \n (provide a string with format:"
+                    f" {self._time_str})"
                 ) from error
 
         self._time = value
 
     def __call__(self, value: datetime | float | int | str):
         """Make Time instance callable.
 
@@ -358,15 +369,16 @@
 class TimeList(TypeCheckedList):
     """Type checked list of Time instances.
 
     >>> times = TimeList([])
     >>> times
     TimeList([])
 
-    Implement a load() method for loading times from an iterator (for example from a .csv file row iterator).
+    Implement a load() method for loading times from an iterator
+     (for example from a .csv file row iterator).
     """
 
     def __init__(self, iterator_arg: list[Time] = None) -> None:
         """
         ---
 
         iterator_arg : List[Time], optional, default to None
@@ -398,28 +410,28 @@
 
             self.append(Time(row["time"]))
 
         return None
 
 
 class TimeListLoader:
-    """Loads times into a type-checked list given the column name corresponding to the time values,.
-
-     as stored in the input file.
+    """Loads times into a type-checked list given the column name corresponding
+     to the time values as stored in the input file.
 
     >>> source = Path.cwd() / "data" / "sub1.csv"
     >>> usecols = ['time']
     >>> times_loader = TimeListLoader(source, usecols)
     >>> times = times_loader.load()
     >>> times[:3]
     TimeList([Time(1651585280.77981),
              Time(1651585280.78481),
              Time(1651585280.78981)])
 
-    The time, as given by the column name, is automatically re-named to pre-defined name: 'time'
+    The time, as given by the column name, is automatically re-named to
+     pre-defined name: 'time'
 
     >>> times[0].time
     1651585280.77981
     """
 
     # Pre-defined time name
     new_colnames = ["time"]
@@ -428,15 +440,16 @@
         """
         ---
 
             source : Path, required
                 Path of the input file.
 
             usecols : List or Tuple, required
-                Names corresponding to the time values as stored in the input file.
+                Names corresponding to the time values as stored in the input
+                 file.
         """
         self.source = source
         self.usecols = usecols
 
         # Map given time name to pre-defined name
         self.col_map_dict = dict(zip(self.usecols, self.new_colnames))
```

### Comparing `gscipy-0.1.2/src/gscipy/trajectories.py` & `gscipy-0.1.3/src/gscipy/trajectories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""Module for creation (and handling) of multidimensional vectors and trajectories."""
+"""Module for creation (and handling) of multidimensional vectors
+ and trajectories."""
 from __future__ import annotations
 
 __author__ = "Matteo Gabba"
 __copyright__ = "Copyright 2022, all right reserved Gabba Scientific"
 __status__ = "Development"
 
-from abc import abstractmethod
 from collections.abc import Collection, Iterator
 from dataclasses import dataclass
 from pathlib import Path
 
 import numpy as np
 
 from gscipy.decorators import check_args_len
@@ -22,16 +22,17 @@
 # TODO: unit test the VectorNDim class
 
 
 @dataclass(frozen=True)
 class Trajectory(JsonIOInterface):
     """Represents a time series of 3D vectors instances.
 
-    A Trajectory instance is instantiated by a list of 3D vectors and the corresponding times, a type error is raised
-    otherwise. The two lists must contain the same number of Vector and Time instances.
+    A Trajectory instance is instantiated by a list of 3D vectors and the
+     corresponding times, a type error is raised otherwise. The two lists must
+      contain the same number of Vector and Time instances.
 
     >>> source = Path.cwd() / "data" / "sub1.csv"
     >>> time_colnames = ['time']
     >>> coord_colnames = ['gaze_deg_coord_x', 'gaze_deg_coord_y']
     >>> times = TimeListLoader(source, usecols=time_colnames).load()
     >>> vectors = VectorListLoader(source, usecols=coord_colnames).load()
     >>> trajectory = Trajectory(vectors, times)
@@ -39,16 +40,17 @@
     (VectorsList([Vector(0.4622481497169438, 3.76608427632374, 0.0),
                   Vector(0.46393828577858687, 3.7411490072433953, 0.0),
                   Vector(0.456283375837779, 3.7295640810489856, 0.0)]),
      TimeList([Time(1651585280.77981),
                Time(1651585280.78481),
                Time(1651585280.78981)]))
 
-    A Trajectory instance contains the following properties: vector coordinates (x, y, z), vector magnitudes,
-     time values, time zero (t0), relative time from start of the time-series:
+    A Trajectory instance contains the following properties: vector coordinates
+     (x, y, z), vector magnitudes, time values, time zero (t0), relative time
+      from start of the time-series:
 
     >>> trajectory.x[:5]
     array([0.46224815, 0.46393829, 0.45628338, 0.50202114, 0.51964137])
     >>> trajectory.y[:5]
     array([3.76608428, 3.74114901, 3.72956408, 3.70602158, 3.94218248])
     >>> trajectory.z[:5]
     array([0., 0., 0., 0., 0.])
@@ -61,15 +63,16 @@
            1.65158528e+09])
 
     >>> trajectory.t0
     1651585280.77981
     >>> trajectory.rtime[:5]
     array([0.        , 0.00500011, 0.00999999, 0.0150001 , 0.01999998])
 
-    A Trajectory instance supports dot and cross vector products both trajectory-wise
+    A Trajectory instance supports dot and cross vector products both
+     trajectory-wise
 
     >>> dot_prod = trajectory.dot(trajectory)
     >>> dot_prod[:3]
     [14.397064128289646, 14.211434627409416, 14.117842753716685]
 
     >>> cross_prod = trajectory.cross(trajectory)
     >>> cross_prod[:3]
@@ -101,15 +104,16 @@
                Time(1651585280.78481),
                Time(1651585280.78981)]))
 
     The following operations are implemented by operator overlaoding
 
     Get item(s) (Vector, Time) by indexing or slicing
     >>> trajectory[1]
-    (Vector(0.46393828577858687, 3.7411490072433953, 0.0), Time(1651585280.78481))
+    (Vector(0.46393828577858687, 3.7411490072433953, 0.0),
+     Time(1651585280.78481))
     >>> trajectory[:2]
     (VectorsList([Vector(0.4622481497169438, 3.76608427632374, 0.0),
                   Vector(0.46393828577858687, 3.7411490072433953, 0.0)]),
     TimeList([Time(1651585280.77981), Time(1651585280.78481)]))
 
     Iteration
     >>> ((vector, time) for (vector, time) in trajectory)
@@ -194,24 +198,27 @@
     @classmethod
     def from_json(cls, json_dict: CustomJSONDict) -> Trajectory:
         return cls(json_dict["vectors"], json_dict["times"])
 
     def __post_init__(self):
         if not isinstance(self.vectors, VectorsList):
             raise TypeError(
-                f"{self.__class__.__name__}() argument 'vector' must be a type-checked list of Vector(s),"
+                f"{self.__class__.__name__}() argument 'vector' must be a"
+                f" type-checked list of Vector(s),"
                 f" not '{self.vectors.__class__.__name__}'"
             )
         if not isinstance(self.times, TimeList):
             raise TypeError(
-                f"{self.__class__.__name__}() argument 'times' must be a type-checked list of Time(s),"
+                f"{self.__class__.__name__}() argument 'times' must be"
+                f" a type-checked list of Time(s),"
                 f" not '{self.times.__class__.__name__}'"
             )
         assert len(self.vectors) == len(self.times), (
-            f"Trajectory instance arguments 'vectors' and 'times' must have same dimension, not {len(self.vectors)}"
+            f"Trajectory instance arguments 'vectors' and 'times' must have"
+            f" same dimension, not {len(self.vectors)}"
             f" and {len(self.times)}"
         )
 
     @property
     def magnitude(self) -> np.ndarray:
         """Magnitudes of Trajectory vectors."""
         return np.array([vector.magnitude for vector in self.vectors])
@@ -245,48 +252,52 @@
         """First point of the time series."""
         return self.time[0]
 
     @check_args_len
     def dot(self, other: Trajectory | Vector) -> list[float]:
         """Dot product of Trajectory vectors.
 
-        If 'other' is a Trajectory instance the vectors of the two trajectories ('self' and 'other') are multiplied
-        element by element.
-        If 'other' is a Vector instance all vectors of 'self' are multiplied by the 'other' vector.
+        If 'other' is a Trajectory instance the vectors of the two trajectories
+         ('self' and 'other') are multiplied element by element.
+        If 'other' is a Vector instance all vectors of 'self' are multiplied by
+         the 'other' vector.
 
         Raise AssertionError if the two trajectories have different dimension.
         Raise TypeError if 'other' is not a Trajectory or Vector instance.
 
         Returns
         -------
-            A list of float values corresponding to the dot products for each vector of the input Trajectory(s).
+            A list of float values corresponding to the dot products for each
+             vector of the input Trajectory(s).
         """
         if isinstance(other, self.__class__):
             return [r1.dot(r2) for r1, r2 in zip(self.vectors, other.vectors)]
         if isinstance(other, Vector):
             return [r.dot(other) for r in self.vectors]
         raise TypeError(
             f"unsupported operand type(s) for {self.__class__.__name__}.dot():"
             f" '{other.__class__.__name__}'"
         )
 
     @check_args_len
     def cross(self, other: Trajectory | Vector) -> Trajectory:
         """Cross product of Trajectory vectors.
 
-        If 'other' is a Trajectory instance the vectors of the two trajectories ('self' and 'other') are multiplied
-        element by element.
-        If 'other' is a Vector instance all vectors of 'self' are multiplied by the 'other' vector.
+        If 'other' is a Trajectory instance the vectors of the two trajectories
+         ('self' and 'other') are multiplied element by element.
+        If 'other' is a Vector instance all vectors of 'self' are multiplied
+         by the 'other' vector.
 
         Raise AssertionError if the two trajectories have different dimension.
         Raise TypeError if 'other' is not a Trajectory or Vector instance.
 
         Returns
         -------
-            A Trajectory instance corresponding to the cross products for each vector of the input Trajectory(s).
+            A Trajectory instance corresponding to the cross products for each
+             vector of the input Trajectory(s).
         """
         if isinstance(other, self.__class__):
             return self(
                 VectorsList(
                     [
                         r1.cross(r2)
                         for r1, r2 in zip(self.vectors, other.vectors)
@@ -296,16 +307,16 @@
             )
         if isinstance(other, Vector):
             return self(
                 VectorsList([r.cross(other) for r in self.vectors]),
                 self.times,
             )
         raise TypeError(
-            f"unsupported operand type(s) for {self.__class__.__name__}.cross():"
-            f" '{other.__class__.__name__}'"
+            f"unsupported operand type(s) for"
+            f" {self.__class__.__name__}.cross(): '{other.__class__.__name__}'"
         )
 
     def __call__(self, vectors: VectorsList, times: TimeList) -> Trajectory:
         """Makes Trajectory instance callable."""
         return self.__class__(vectors, times)
 
     def __getitem__(self, index: int) -> tuple[Vector, Time]:
@@ -320,17 +331,18 @@
         """Returns Trajectory length (number of items in the time-series)."""
         return len(self.vectors)
 
     @check_args_len
     def __add__(self, other: Trajectory | Vector) -> Trajectory:
         """Addition of Trajectory vectors.
 
-        If 'other' is a Trajectory instance the vectors of the two trajectories ('self' and 'other') are added
-        element by element.
-        If 'other' is a Vector instance the 'other' vector is added to all vectors of 'self'.
+        If 'other' is a Trajectory instance the vectors of the two trajectories
+         ('self' and 'other') are added element by element.
+        If 'other' is a Vector instance the 'other' vector is added to all
+         vectors of 'self'.
 
         Raise AssertionError if the two trajectories have different dimension.
         Raise TypeError if 'other' is not a Trajectory or Vector instance.
         """
         if isinstance(other, self.__class__):
             return self(
                 VectorsList(
@@ -348,17 +360,18 @@
     def __radd__(self, other: Trajectory | Vector) -> Trajectory:
         return self + other
 
     @check_args_len
     def __sub__(self, other: Trajectory | Vector) -> Trajectory:
         """Subtraction of Trajectory vectors.
 
-        If 'other' is a Trajectory instance the vectors of the two trajectories ('self' and 'other') are subtracted
-        element by element.
-        If 'other' is a Vector instance the 'other' vector is subtracted to all vectors of 'self'.
+        If 'other' is a Trajectory instance the vectors of the two trajectories
+         ('self' and 'other') are subtracted element by element.
+        If 'other' is a Vector instance the 'other' vector is subtracted to all
+         vectors of 'self'.
 
         Raise AssertionError if the two trajectories have different dimension.
         Raise TypeError if 'other' is not a Trajectory or Vector instance.
         """
         return self + (-other)
 
     def __rsub__(self, other: Trajectory | Vector) -> Trajectory:
@@ -367,21 +380,24 @@
     @check_args_len
     def __mul__(
         self,
         other: Trajectory | Vector | int | float,
     ) -> Trajectory:
         """Coordinate-wise multiplication of Trajectory vectors.
 
-        If 'other' is a Trajectory instance the vectors of the two trajectories ('self' and 'other') are multiplied
-        coordinate-wise vector by vector.
-        If 'other' is a Vector instance the 'other' vector is multiplied coordinate-wise to all vectors of 'self'.
-        If 'other' is a number (float or int) all vectors of 'self' are scalar multiplied by 'other'.
+        If 'other' is a Trajectory instance the vectors of the two trajectories
+         ('self' and 'other') are multiplied coordinate-wise vector by vector.
+        If 'other' is a Vector instance the 'other' vector is multiplied
+         coordinate-wise to all vectors of 'self'.
+        If 'other' is a number (float or int) all vectors of 'self' are scalar
+         multiplied by 'other'.
 
         Raise AssertionError if the two trajectories have different dimension.
-        Raise TypeError if 'other' is not a Trajectory, Vector, float or int type.
+        Raise TypeError if 'other' is not a Trajectory, Vector, float or int
+         type.
         """
         if isinstance(other, self.__class__):
             return self(
                 VectorsList(
                     [r1 * r2 for r1, r2 in zip(self.vectors, other.vectors)]
                 ),
                 self.times,
@@ -416,40 +432,44 @@
 
     def __abs__(self) -> np.ndarray:
         """Absolute value (magnitude) of Trajectory vectors."""
         return self.magnitude
 
     @check_args_len
     def __eq__(self, other: Trajectory) -> bool:
-        """Check equality between each item (Vector, Time) of two Trajectory instances."""
+        """Check equality between each item (Vector, Time) of two Trajectory
+         instances."""
         if isinstance(other, self.__class__):
             return (self.vectors == other.vectors) and (
                 self.times == other.times
             )
         return NotImplemented
 
     def __ne__(self, other: Trajectory) -> bool:
-        """Check inequality between each item (Vector, Time) of two Trajectory instances."""
+        """Check inequality between each item (Vector, Time) of two Trajectory
+         instances."""
         return not self == other
 
     def __hash__(self) -> int:
         """Return hash value of the given instance."""
         return hash(tuple(self))
 
     def __bool__(self) -> bool:
         """Check that all vectors and times are null."""
         return all(r == 0 for r, t in self) and all(t == 0 for r, t in self)
 
     def __repr__(self) -> str:
         """Returns a representation of a Vector object."""
-        return f"{self.__class__.__name__}({[(r, t) for r, t in zip(self.vectors, self.times)]})"
+        return f"{self.__class__.__name__}" \
+               f"({[(r, t) for r, t in zip(self.vectors, self.times)]})"
 
     def __str__(self) -> str:
         """Returns a string representation of a Vector object."""
-        return f"length={len(self)}, \n{[(r, t) for r, t in zip(self.vectors, self.times)]}"
+        return f"length={len(self)}," \
+               f" \n{[(r, t) for r, t in zip(self.vectors, self.times)]}"
 
 
 class TrajectoryLoader:
     """Create a Trajectory instance from file.
 
     >>> source = Path.cwd() / "data" / "sub1.csv"
     >>> time_colnames = ['time']
@@ -468,21 +488,23 @@
         time_colnames: list[str],
         coord_colnames: list[str],
     ) -> None:
         """
         ---
 
             source : Path, required
-                Path of the file storing the vector coordinates and the corresponding times.
+                Path of the file storing the vector coordinates and the
+                 corresponding times.
 
             time_colnames : list[str], required
                 Name of the column storing the time values.
 
             coord_colnames : list[str], required
-                Names of the columns storing the 3D coordinates, or a subset of those, of the vectors.
+                Names of the columns storing the 3D coordinates, or a subset of
+                 those, of the vectors.
         """
         self.source = source
         self.time_colnames = time_colnames
         self.coord_colnames = coord_colnames
 
     def load(self) -> Trajectory:
         """
@@ -500,23 +522,25 @@
 
 @dataclass
 class BaseTrajectoryCollection(Collection):
     def __post_init__(self):
         for name, value in self.__dict__.items():
             if not isinstance(value, Trajectory):
                 raise TypeError(
-                    f"unsupported '{name}' argument type for {self.__class__.__name__}():"
+                    f"unsupported '{name}' argument type for"
+                    f" {self.__class__.__name__}():"
                     f" '{value.__class__.__name__}'"
                 )
 
     def __iter__(self) -> Iterator[tuple[str, Trajectory]]:
         for (name, trajectory) in self.__dict__.items():
             yield name, trajectory
 
     def __contains__(self, trajectory) -> bool:
         return trajectory in self.__dict__.values()
 
     def __len__(self) -> int:
         return len(self.__dict__)
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(attrs={[key for key in self.__dict__.keys()]})"
+        return f"{self.__class__.__name__}" \
+               f"(attrs={[key for key in self.__dict__.keys()]})"
```

### Comparing `gscipy-0.1.2/src/gscipy/utils.py` & `gscipy-0.1.3/src/gscipy/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,66 @@
 """Module with general utility functions."""
 from __future__ import annotations
 
 __author__ = "Matteo Gabba"
 __copyright__ = "Copyright 2022, all right reserved Gabba Scientific"
 __status__ = "Development"
 
+import inspect
 import itertools
 import math
 from collections.abc import Iterator
 from typing import Iterable
 
 import more_itertools
 import numpy as np
 
 
-def all_zeros_array(
+def get_class_properties(
+    obj: object,
+) -> dict[str, ...]:
+    properties = {}
+
+    for attr, value in inspect.getmembers(obj):
+        # Remove private and protected functions
+        if not attr.startswith("_"):
+            # Remove methods
+            if not inspect.ismethod(value):
+                # Remove class attributes
+                if isinstance(getattr(type(obj), attr, None), property):
+                    properties[attr] = value
+    return properties
+
+
+def is_all_zeros_array(
     data: np.ndarray,
 ) -> bool:
     return not np.any(data)
 
 
 def bin_edge_to_center(bin_edges: np.ndarray) -> np.ndarray:
     """
     Convert bin edges to bin center.
 
     Parameters
     ----------
-        bin_edges : 'array'
+        bin_edges : np.ndarray, (N,)
             Bin edges. For example as defined by numpy.histogram().
 
     Returns
     -------
-        bin_center : 'array'
+        bin_centers : np.ndarray, (N,)
             Bin center position calculated as (left_edges + right_edges) / 2.
     """
     # Compute the bin center:
     left_edges = bin_edges[1:]
     right_edges = bin_edges[:-1]
-    bin_center = (left_edges + right_edges) / 2
+    bin_centers = (left_edges + right_edges) / 2
 
-    return bin_center
+    return bin_centers
 
 
 def build_histogram(
     data: np.ndarray,
     hist_range: tuple[float, float],
     bins: int | str = "auto",
     density: bool = True,
@@ -62,37 +79,41 @@
     return values, bin_centers, bin_width
 
 
 def cluster_size_generator(
     values: Iterable[float],
 ) -> Iterator[tuple[float, np.ndarray, np.ndarray]]:
     """
-    Yield generator with value, counts and index of groups of consecutive equal values in a 1D-list.
-
-    Adapted from:
-        https://stackoverflow.com/questions/23023805/how-to-get-the-index-and-occurance-of-each-item-using-itertools-groupby
+    Yield generator with value, counts and index of groups of consecutive equal
+     values in a 1D-list.
 
     Parameters
     ----------
         values : list
             1D list of values.
 
-    Returns
-    -------
-        (value, counts, idx) : generator
+    Yields
+    ------
+        (value, counts, idx) : tuple[float, np.ndarray, np.ndarray]
+
+    Notes
+    -----
+    Adapted from:
+        <https://stackoverflow.com/questions/23023805/how-to-get-the-index-and-occurance-of-each-item-using-itertools-groupby>
     """
     # Set index indicating start of the first group
     group_start_idx = 0
 
     # For each group of consecutive equal values
     for value, group in itertools.groupby(values):
         # counts the consecutive equal values
         counts = len(list(group))
 
-        # generate array of index corresponding to each group of consecutive values
+        # generate array of index corresponding to each group of consecutive
+        # values
         idx = np.arange(group_start_idx, group_start_idx + counts)
 
         # yield generator with value, counts and index of each group
         yield value, counts, idx
 
         # re-set the start index for next group
         group_start_idx += counts
```

### Comparing `gscipy-0.1.2/src/gscipy/vectors.py` & `gscipy-0.1.3/src/gscipy/vectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,16 +123,18 @@
 
         # Set keyword arguments to attributes
         for key, value in coordinates.items():
             try:
                 setattr(self, key, float(value))
             except ValueError as error:
                 raise TypeError(
-                    f"{self._class_name}() argument must be a list of float(s) or int(s),"
-                    f" or float-convertible string numbers, not '{value.__class__.__name__}'"
+                    f"{self._class_name}() argument must be a list of float(s)"
+                    f" or int(s),"
+                    f" or float-convertible string numbers, not"
+                    f" '{value.__class__.__name__}'"
                 ) from error
 
         # Set coordinates attribute
         self._coordinates = list(map(float, coordinates.values()))
         self._keys = list(coordinates.keys())
 
     @property
@@ -201,15 +203,16 @@
             unprotected_keys = [
                 key for key in self.__dict__.keys() if not key.startswith("_")
             ]
             for i, key in enumerate(unprotected_keys):
                 setattr(self, key, self._coordinates[i])
         else:
             raise TypeError(
-                f"unsupported operand type(s) for {self._class_name}.__setitem__():"
+                f"unsupported operand type(s) for"
+                f" {self._class_name}.__setitem__():"
                 f" '{value.__class__.__name__}'"
             )
 
     def __iter__(self) -> Iterator[float]:
         """Allows iteration over the vector coordinates.
 
         >>> v = VectorNDim(x1=1, x2=2)
@@ -289,25 +292,27 @@
         return NotImplemented
 
     def __rsub__(self, other: VectorNDim) -> VectorNDim:
         return other + (-self)
 
     @check_args_len
     def __mul__(self, other: VectorNDim | int | float) -> VectorNDim:
-        """Coordinate-wise vector multiplication and scalar multiplication of a vector.
+        """Coordinate-wise vector multiplication and scalar multiplication of
+         a vector.
 
         >>> v1 = VectorNDim(x0=1, x1=1)
         >>> v2 = VectorNDim(x0=2, x1=2)
         >>> v1 * v2
         Vector(2.0, 2.0)
         >>> v1 * 10
         Vector(10.0, 10.0)
 
         Raise AssertionError if the two vectors have different dimension.
-        Raise TypeError if 'other' is not a Vector instance or a number (int, float).
+        Raise TypeError if 'other' is not a Vector instance or a number
+         (int, float).
         """
         if isinstance(other, self.__class__):
             return self(
                 **{
                     self._keys[i]: a * b
                     for i, (a, b) in enumerate(zip(self, other))
                 }
@@ -379,15 +384,16 @@
         if isinstance(other, self.__class__):
             return all(
                 a == b for a, b in zip(self._coordinates, other._coordinates)
             )
         return NotImplemented
 
     def __ne__(self, other: VectorNDim | int | float) -> bool:
-        """Check vector vector inequality in terms of both magnitude and direction.
+        """Check vector vector inequality in terms of both magnitude and
+         direction.
 
         >>> v1 = VectorNDim(x0=1, x1=2)
         >>> v2 = VectorNDim(x0=2, x1=3)
         >>> v1 != v2
         True
         >>> v1 != v1
         False
@@ -405,24 +411,26 @@
     def __repr__(self) -> str:
         """Returns a representation of a Vector object.
 
         >>> v = VectorNDim(x1=1, x2=3)
         >>> v
         Vector(1.0, 3.0)
         """
-        return f"{self._class_name}({', '.join(str(c) for c in self._coordinates)})"
+        return f"{self._class_name}" \
+               f"({', '.join(str(c) for c in self._coordinates)})"
 
     def __str__(self) -> str:
         """Returns a string representation of a Vector object.
 
         >>> v = VectorNDim(x1=1, x2=3)
         >>> print(v)
         Vector(1.0, 3.0)
         """
-        return f"{self._class_name}({', '.join(str(c) for c in self._coordinates)})"
+        return f"{self._class_name}" \
+               f"({', '.join(str(c) for c in self._coordinates)})"
 
 
 class Vector(VectorNDim, JsonIOInterface):
     """Represents a vector in 3-dimensions with coordinates (x, y, z).
 
     >>> r = Vector(x=1, y=2, z=3)
     >>> r
@@ -501,16 +509,18 @@
 class VectorsList(TypeCheckedList):
     """Type checked list of 3D vectors.
 
     >>> vectors = VectorsList([])
     >>> vectors
     VectorsList([])
 
-    Implement a load() method for loading vectors from an iterator (for example from a .csv file row iterator).
-    Raise TypeError if a not Vector instance is appended or inserted (in)to the list.
+    Implement a load() method for loading vectors from an iterator (for example
+     from a .csv file row iterator).
+    Raise TypeError if a not Vector instance is appended or inserted
+     (in)to the list.
     """
 
     def __init__(self, iterator_arg: list[Vector] = None):
         """
         Iterator_arg : List[Vector], optional, default to None.
 
             List of Vector vectors
@@ -525,41 +535,44 @@
 
     def load(self, row_iter: Iterable[dict[str, Any]]) -> None:
         """Load 3D vectors into the type checked list.
 
         Parameters
         ----------
         row_iter : Iterable[dict[str, Any]]
-            Iterable generating a dictionary dict[str, Any] with keys {'x', 'y', 'z'}.
+            Iterable generating a dictionary dict[str, Any] with keys
+             {'x', 'y', 'z'}.
             For example, the row-iterator of a .csv file.
 
         Returns
         -------
             A type checked list populated with Vector vectors
         """
         for row in row_iter:
 
             self.append(Vector(**row))
 
 
 class VectorListLoader:
-    """Loads 3D vectors into a type-checked list given the column names corresponding to the 3D coordinates values.
+    """Loads 3D vectors into a type-checked list given the column names
+     corresponding to the 3D coordinates values.
 
     (x, y, z), or a subset of those, as stored in the input file.
 
     >>> source = Path.cwd() / "data" / "sub1.csv"
     >>> usecols = ['gaze_deg_coord_x', 'gaze_deg_coord_y']
     >>> vectors_loader = VectorListLoader(source, usecols)
     >>> vectors = vectors_loader.load()
     >>> vectors[:3]
     VectorsList([Vector(0.4622481497169438, 3.76608427632374, 0.0),
              Vector(0.46393828577858687, 3.7411490072433953, 0.0),
              Vector(0.456283375837779, 3.7295640810489856, 0.0)])
 
-    The coordinates, as given by the column names, are automatically re-named to pre-defined names: 'x', 'y', 'z'
+    The coordinates, as given by the column names, are automatically re-named
+     to pre-defined names: 'x', 'y', 'z'
 
     >>> vectors[0].__dict__
     {'_class_name': 'Vector',
      'x': 0.4622481497169438,
      'y': 3.76608427632374,
      'z': 0.0,
      '_coordinates': [0.4622481497169438, 3.76608427632374, 0.0],
@@ -573,16 +586,16 @@
         """
         ---
 
             source : Path, required
                 Path of the input file.
 
             usecols : List or Tuple, required
-                Names corresponding to the coordinates (x, y, z) of a 3D vector, or a subset of those,
-                as stored in the input file.
+                Names corresponding to the coordinates (x, y, z) of a 3D
+                 vector, or a subset of those, as stored in the input file.
         """
         self.source = source
         self.usecols = usecols
 
         # Map given coordinates names to pre-defined names
         self.col_map_dict = dict(zip(self.usecols, self.new_names))
```

### Comparing `gscipy-0.1.2/src/gscipy.egg-info/PKG-INFO` & `gscipy-0.1.3/src/gscipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscipy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Gabba Scientific utilities
 Author: Matteo Gabba
 Author-email: m.gabba083@gmail.com
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
```

