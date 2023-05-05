# Comparing `tmp/mypy-boto3-mediatailor-1.26.59.tar.gz` & `tmp/mypy-boto3-mediatailor-1.26.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediatailor-1.26.59.tar", last modified: Fri Jan 27 20:32:52 2023, max compression
+gzip compressed data, was "mypy-boto3-mediatailor-1.26.62.tar", last modified: Wed Feb  1 20:26:24 2023, max compression
```

## Comparing `mypy-boto3-mediatailor-1.26.59.tar` & `mypy-boto3-mediatailor-1.26.62.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:52.636097 mypy-boto3-mediatailor-1.26.59/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-27 20:32:16.000000 mypy-boto3-mediatailor-1.26.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-01-27 20:32:52.636097 mypy-boto3-mediatailor-1.26.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-01-27 20:32:16.000000 mypy-boto3-mediatailor-1.26.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:52.632097 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-01-27 20:32:16.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-01-27 20:32:16.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-01-27 20:32:16.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32850 2023-01-27 20:32:16.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32792 2023-01-27 20:32:16.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-01-27 20:32:16.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-01-27 20:32:16.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-01-27 20:32:16.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-01-27 20:32:16.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:16.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    49537 2023-01-27 20:32:17.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49476 2023-01-27 20:32:16.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-27 20:32:16.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:32:52.636097 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-01-27 20:32:52.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-01-27 20:32:52.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:52.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:32:52.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-27 20:32:52.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-27 20:32:52.000000 mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 20:32:52.636097 mypy-boto3-mediatailor-1.26.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-01-27 20:32:15.000000 mypy-boto3-mediatailor-1.26.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:26:24.135656 mypy-boto3-mediatailor-1.26.62/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-01 20:26:10.000000 mypy-boto3-mediatailor-1.26.62/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19302 2023-02-01 20:26:24.127657 mypy-boto3-mediatailor-1.26.62/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17799 2023-02-01 20:26:10.000000 mypy-boto3-mediatailor-1.26.62/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:26:24.127657 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-02-01 20:26:10.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-02-01 20:26:10.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-02-01 20:26:10.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33557 2023-02-01 20:26:10.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33498 2023-02-01 20:26:10.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-02-01 20:26:10.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-02-01 20:26:10.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-02-01 20:26:10.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-02-01 20:26:10.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:26:10.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    51799 2023-02-01 20:26:12.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51734 2023-02-01 20:26:11.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-01 20:26:10.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:26:24.127657 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19302 2023-02-01 20:26:23.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-02-01 20:26:24.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 20:26:23.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 20:26:23.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-01 20:26:23.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-01 20:26:23.000000 mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 20:26:24.135656 mypy-boto3-mediatailor-1.26.62/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-01 20:26:10.000000 mypy-boto3-mediatailor-1.26.62/setup.py
```

### Comparing `mypy-boto3-mediatailor-1.26.59/LICENSE` & `mypy-boto3-mediatailor-1.26.62/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.26.59/PKG-INFO` & `mypy-boto3-mediatailor-1.26.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediatailor
-Version: 1.26.59
-Summary: Type annotations for boto3.MediaTailor 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.62
+Summary: Type annotations for boto3.MediaTailor 1.26.62 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediatailor.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediatailor)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediatailor?color=blue)](https://pypistats.org/packages/mypy-boto3-mediatailor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaTailor 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
+[boto3.MediaTailor 1.26.62](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -371,14 +371,15 @@
     AdMarkerPassthroughTypeDef,
     AlertTypeDef,
     AvailMatchingCriteriaTypeDef,
     AvailSuppressionTypeDef,
     BumperTypeDef,
     CdnConfigurationTypeDef,
     LogConfigurationForChannelTypeDef,
+    ClipRangeTypeDef,
     ConfigureLogsForChannelRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef,
     HttpPackageConfigurationTypeDef,
     PrefetchRetrievalTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
     HttpConfigurationTypeDef,
@@ -420,14 +421,15 @@
     ScheduleAdBreakTypeDef,
     TransitionTypeDef,
     SegmentationDescriptorTypeDef,
     StartChannelRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateProgramTransitionTypeDef,
     AccessConfigurationTypeDef,
     ManifestProcessingRulesTypeDef,
     PrefetchConsumptionTypeDef,
     ConfigureLogsForChannelResponseTypeDef,
     ConfigureLogsForPlaybackConfigurationResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelPolicyResponseTypeDef,
@@ -454,14 +456,15 @@
     ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
     ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     RequestOutputItemTypeDef,
     ResponseOutputItemTypeDef,
     ScheduleEntryTypeDef,
     ScheduleConfigurationTypeDef,
     TimeSignalMessageTypeDef,
+    UpdateProgramScheduleConfigurationTypeDef,
     CreateSourceLocationRequestRequestTypeDef,
     CreateSourceLocationResponseTypeDef,
     DescribeSourceLocationResponseTypeDef,
     SourceLocationTypeDef,
     UpdateSourceLocationRequestRequestTypeDef,
     UpdateSourceLocationResponseTypeDef,
     GetPlaybackConfigurationResponseTypeDef,
@@ -485,14 +488,16 @@
     ListSourceLocationsResponseTypeDef,
     ListPlaybackConfigurationsResponseTypeDef,
     ListPrefetchSchedulesResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateProgramRequestRequestTypeDef,
     CreateProgramResponseTypeDef,
     DescribeProgramResponseTypeDef,
+    UpdateProgramRequestRequestTypeDef,
+    UpdateProgramResponseTypeDef,
 )
 
 
 def get_structure() -> SecretsManagerAccessTokenConfigurationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mediatailor-1.26.59/README.md` & `mypy-boto3-mediatailor-1.26.62/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediatailor.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediatailor)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediatailor?color=blue)](https://pypistats.org/packages/mypy-boto3-mediatailor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaTailor 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
+[boto3.MediaTailor 1.26.62](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -339,14 +339,15 @@
     AdMarkerPassthroughTypeDef,
     AlertTypeDef,
     AvailMatchingCriteriaTypeDef,
     AvailSuppressionTypeDef,
     BumperTypeDef,
     CdnConfigurationTypeDef,
     LogConfigurationForChannelTypeDef,
+    ClipRangeTypeDef,
     ConfigureLogsForChannelRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef,
     HttpPackageConfigurationTypeDef,
     PrefetchRetrievalTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
     HttpConfigurationTypeDef,
@@ -388,14 +389,15 @@
     ScheduleAdBreakTypeDef,
     TransitionTypeDef,
     SegmentationDescriptorTypeDef,
     StartChannelRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateProgramTransitionTypeDef,
     AccessConfigurationTypeDef,
     ManifestProcessingRulesTypeDef,
     PrefetchConsumptionTypeDef,
     ConfigureLogsForChannelResponseTypeDef,
     ConfigureLogsForPlaybackConfigurationResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelPolicyResponseTypeDef,
@@ -422,14 +424,15 @@
     ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
     ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     RequestOutputItemTypeDef,
     ResponseOutputItemTypeDef,
     ScheduleEntryTypeDef,
     ScheduleConfigurationTypeDef,
     TimeSignalMessageTypeDef,
+    UpdateProgramScheduleConfigurationTypeDef,
     CreateSourceLocationRequestRequestTypeDef,
     CreateSourceLocationResponseTypeDef,
     DescribeSourceLocationResponseTypeDef,
     SourceLocationTypeDef,
     UpdateSourceLocationRequestRequestTypeDef,
     UpdateSourceLocationResponseTypeDef,
     GetPlaybackConfigurationResponseTypeDef,
@@ -453,14 +456,16 @@
     ListSourceLocationsResponseTypeDef,
     ListPlaybackConfigurationsResponseTypeDef,
     ListPrefetchSchedulesResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateProgramRequestRequestTypeDef,
     CreateProgramResponseTypeDef,
     DescribeProgramResponseTypeDef,
+    UpdateProgramRequestRequestTypeDef,
+    UpdateProgramResponseTypeDef,
 )
 
 
 def get_structure() -> SecretsManagerAccessTokenConfigurationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/__init__.py` & `mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/__init__.pyi` & `mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/__main__.py` & `mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaTailor 1.26.59\nVersion:         1.26.59\nBuilder version:"
+        "Type annotations for boto3.MediaTailor 1.26.62\nVersion:         1.26.62\nBuilder version:"
         " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.59")
+    print("1.26.62")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/client.py` & `mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,16 @@
     PutPlaybackConfigurationResponseTypeDef,
     RequestOutputItemTypeDef,
     ScheduleConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
     SlateSourceTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateLiveSourceResponseTypeDef,
+    UpdateProgramResponseTypeDef,
+    UpdateProgramScheduleConfigurationTypeDef,
     UpdateSourceLocationResponseTypeDef,
     UpdateVodSourceResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -601,14 +603,29 @@
         """
         Updates a live source's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_live_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_live_source)
         """
 
+    def update_program(
+        self,
+        *,
+        ChannelName: str,
+        ProgramName: str,
+        ScheduleConfiguration: UpdateProgramScheduleConfigurationTypeDef,
+        AdBreaks: Sequence[AdBreakTypeDef] = ...
+    ) -> UpdateProgramResponseTypeDef:
+        """
+        Updates a program within a channel.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_program)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_program)
+        """
+
     def update_source_location(
         self,
         *,
         HttpConfiguration: HttpConfigurationTypeDef,
         SourceLocationName: str,
         AccessConfiguration: AccessConfigurationTypeDef = ...,
         DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,
```

### Comparing `mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/client.pyi` & `mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,16 @@
     PutPlaybackConfigurationResponseTypeDef,
     RequestOutputItemTypeDef,
     ScheduleConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
     SlateSourceTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateLiveSourceResponseTypeDef,
+    UpdateProgramResponseTypeDef,
+    UpdateProgramScheduleConfigurationTypeDef,
     UpdateSourceLocationResponseTypeDef,
     UpdateVodSourceResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -552,14 +554,28 @@
     ) -> UpdateLiveSourceResponseTypeDef:
         """
         Updates a live source's configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_live_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_live_source)
         """
+    def update_program(
+        self,
+        *,
+        ChannelName: str,
+        ProgramName: str,
+        ScheduleConfiguration: UpdateProgramScheduleConfigurationTypeDef,
+        AdBreaks: Sequence[AdBreakTypeDef] = ...
+    ) -> UpdateProgramResponseTypeDef:
+        """
+        Updates a program within a channel.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_program)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/client/#update_program)
+        """
     def update_source_location(
         self,
         *,
         HttpConfiguration: HttpConfigurationTypeDef,
         SourceLocationName: str,
         AccessConfiguration: AccessConfigurationTypeDef = ...,
         DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,
```

### Comparing `mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/literals.py` & `mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,14 +119,15 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
```

### Comparing `mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/literals.pyi` & `mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,15 @@
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
```

### Comparing `mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/paginator.py` & `mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/paginator.pyi` & `mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/type_defs.py` & `mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "SecretsManagerAccessTokenConfigurationTypeDef",
     "SlateSourceTypeDef",
     "SpliceInsertMessageTypeDef",
     "AdMarkerPassthroughTypeDef",
     "AlertTypeDef",
     "AvailMatchingCriteriaTypeDef",
     "AvailSuppressionTypeDef",
     "BumperTypeDef",
     "CdnConfigurationTypeDef",
     "LogConfigurationForChannelTypeDef",
+    "ClipRangeTypeDef",
     "ConfigureLogsForChannelRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
     "HttpPackageConfigurationTypeDef",
     "PrefetchRetrievalTypeDef",
     "DefaultSegmentDeliveryConfigurationTypeDef",
     "HttpConfigurationTypeDef",
@@ -94,14 +94,15 @@
     "ScheduleAdBreakTypeDef",
     "TransitionTypeDef",
     "SegmentationDescriptorTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateProgramTransitionTypeDef",
     "AccessConfigurationTypeDef",
     "ManifestProcessingRulesTypeDef",
     "PrefetchConsumptionTypeDef",
     "ConfigureLogsForChannelResponseTypeDef",
     "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetChannelPolicyResponseTypeDef",
@@ -128,14 +129,15 @@
     "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
     "ListVodSourcesRequestListVodSourcesPaginateTypeDef",
     "RequestOutputItemTypeDef",
     "ResponseOutputItemTypeDef",
     "ScheduleEntryTypeDef",
     "ScheduleConfigurationTypeDef",
     "TimeSignalMessageTypeDef",
+    "UpdateProgramScheduleConfigurationTypeDef",
     "CreateSourceLocationRequestRequestTypeDef",
     "CreateSourceLocationResponseTypeDef",
     "DescribeSourceLocationResponseTypeDef",
     "SourceLocationTypeDef",
     "UpdateSourceLocationRequestRequestTypeDef",
     "UpdateSourceLocationResponseTypeDef",
     "GetPlaybackConfigurationResponseTypeDef",
@@ -159,14 +161,16 @@
     "ListSourceLocationsResponseTypeDef",
     "ListPlaybackConfigurationsResponseTypeDef",
     "ListPrefetchSchedulesResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateProgramRequestRequestTypeDef",
     "CreateProgramResponseTypeDef",
     "DescribeProgramResponseTypeDef",
+    "UpdateProgramRequestRequestTypeDef",
+    "UpdateProgramResponseTypeDef",
 )
 
 SecretsManagerAccessTokenConfigurationTypeDef = TypedDict(
     "SecretsManagerAccessTokenConfigurationTypeDef",
     {
         "HeaderName": str,
         "SecretArn": str,
@@ -253,14 +257,21 @@
     "LogConfigurationForChannelTypeDef",
     {
         "LogTypes": List[Literal["AS_RUN"]],
     },
     total=False,
 )
 
+ClipRangeTypeDef = TypedDict(
+    "ClipRangeTypeDef",
+    {
+        "EndOffsetMillis": int,
+    },
+)
+
 ConfigureLogsForChannelRequestRequestTypeDef = TypedDict(
     "ConfigureLogsForChannelRequestRequestTypeDef",
     {
         "ChannelName": str,
         "LogTypes": Sequence[Literal["AS_RUN"]],
     },
 )
@@ -304,21 +315,19 @@
     {
         "DynamicVariables": Mapping[str, str],
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class PrefetchRetrievalTypeDef(
     _RequiredPrefetchRetrievalTypeDef, _OptionalPrefetchRetrievalTypeDef
 ):
     pass
 
-
 DefaultSegmentDeliveryConfigurationTypeDef = TypedDict(
     "DefaultSegmentDeliveryConfigurationTypeDef",
     {
         "BaseUrl": str,
     },
     total=False,
 )
@@ -496,22 +505,20 @@
         "DurationMinutes": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetChannelScheduleRequestRequestTypeDef(
     _RequiredGetChannelScheduleRequestRequestTypeDef,
     _OptionalGetChannelScheduleRequestRequestTypeDef,
 ):
     pass
 
-
 GetPlaybackConfigurationRequestRequestTypeDef = TypedDict(
     "GetPlaybackConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -566,21 +573,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAlertsRequestRequestTypeDef(
     _RequiredListAlertsRequestRequestTypeDef, _OptionalListAlertsRequestRequestTypeDef
 ):
     pass
 
-
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -597,21 +602,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListLiveSourcesRequestRequestTypeDef(
     _RequiredListLiveSourcesRequestRequestTypeDef, _OptionalListLiveSourcesRequestRequestTypeDef
 ):
     pass
 
-
 ListPlaybackConfigurationsRequestRequestTypeDef = TypedDict(
     "ListPlaybackConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -629,22 +632,20 @@
         "MaxResults": int,
         "NextToken": str,
         "StreamId": str,
     },
     total=False,
 )
 
-
 class ListPrefetchSchedulesRequestRequestTypeDef(
     _RequiredListPrefetchSchedulesRequestRequestTypeDef,
     _OptionalListPrefetchSchedulesRequestRequestTypeDef,
 ):
     pass
 
-
 ListSourceLocationsRequestRequestTypeDef = TypedDict(
     "ListSourceLocationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -668,21 +669,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListVodSourcesRequestRequestTypeDef(
     _RequiredListVodSourcesRequestRequestTypeDef, _OptionalListVodSourcesRequestRequestTypeDef
 ):
     pass
 
-
 PutChannelPolicyRequestRequestTypeDef = TypedDict(
     "PutChannelPolicyRequestRequestTypeDef",
     {
         "ChannelName": str,
         "Policy": str,
     },
 )
@@ -711,19 +710,17 @@
         "DurationMillis": int,
         "RelativeProgram": str,
         "ScheduledStartTimeMillis": int,
     },
     total=False,
 )
 
-
 class TransitionTypeDef(_RequiredTransitionTypeDef, _OptionalTransitionTypeDef):
     pass
 
-
 SegmentationDescriptorTypeDef = TypedDict(
     "SegmentationDescriptorTypeDef",
     {
         "SegmentNum": int,
         "SegmentationEventId": int,
         "SegmentationTypeId": int,
         "SegmentationUpid": str,
@@ -761,14 +758,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateProgramTransitionTypeDef = TypedDict(
+    "UpdateProgramTransitionTypeDef",
+    {
+        "DurationMillis": int,
+        "ScheduledStartTimeMillis": int,
+    },
+    total=False,
+)
+
 AccessConfigurationTypeDef = TypedDict(
     "AccessConfigurationTypeDef",
     {
         "AccessType": AccessTypeType,
         "SecretsManagerAccessTokenConfiguration": SecretsManagerAccessTokenConfigurationTypeDef,
     },
     total=False,
@@ -793,21 +799,19 @@
     {
         "AvailMatchingCriteria": Sequence[AvailMatchingCriteriaTypeDef],
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class PrefetchConsumptionTypeDef(
     _RequiredPrefetchConsumptionTypeDef, _OptionalPrefetchConsumptionTypeDef
 ):
     pass
 
-
 ConfigureLogsForChannelResponseTypeDef = TypedDict(
     "ConfigureLogsForChannelResponseTypeDef",
     {
         "ChannelName": str,
         "LogTypes": List[Literal["AS_RUN"]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -866,21 +870,19 @@
     "_OptionalCreateLiveSourceRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateLiveSourceRequestRequestTypeDef(
     _RequiredCreateLiveSourceRequestRequestTypeDef, _OptionalCreateLiveSourceRequestRequestTypeDef
 ):
     pass
 
-
 CreateLiveSourceResponseTypeDef = TypedDict(
     "CreateLiveSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
@@ -903,21 +905,19 @@
     "_OptionalCreateVodSourceRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateVodSourceRequestRequestTypeDef(
     _RequiredCreateVodSourceRequestRequestTypeDef, _OptionalCreateVodSourceRequestRequestTypeDef
 ):
     pass
 
-
 CreateVodSourceResponseTypeDef = TypedDict(
     "CreateVodSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
@@ -971,19 +971,17 @@
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class LiveSourceTypeDef(_RequiredLiveSourceTypeDef, _OptionalLiveSourceTypeDef):
     pass
 
-
 UpdateLiveSourceRequestRequestTypeDef = TypedDict(
     "UpdateLiveSourceRequestRequestTypeDef",
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
         "LiveSourceName": str,
         "SourceLocationName": str,
     },
@@ -1041,19 +1039,17 @@
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class VodSourceTypeDef(_RequiredVodSourceTypeDef, _OptionalVodSourceTypeDef):
     pass
 
-
 _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
     "_RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
     {
         "ChannelName": str,
     },
 )
 _OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
@@ -1061,44 +1057,40 @@
     {
         "DurationMinutes": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef(
     _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
     _OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
     "_RequiredListAlertsRequestListAlertsPaginateTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
     "_OptionalListAlertsRequestListAlertsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAlertsRequestListAlertsPaginateTypeDef(
     _RequiredListAlertsRequestListAlertsPaginateTypeDef,
     _OptionalListAlertsRequestListAlertsPaginateTypeDef,
 ):
     pass
 
-
 ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
     "ListChannelsRequestListChannelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1113,22 +1105,20 @@
     "_OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListLiveSourcesRequestListLiveSourcesPaginateTypeDef(
     _RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
     _OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
 ):
     pass
 
-
 ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef = TypedDict(
     "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1144,22 +1134,20 @@
     {
         "StreamId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef(
     _RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
     _OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
 ):
     pass
 
-
 ListSourceLocationsRequestListSourceLocationsPaginateTypeDef = TypedDict(
     "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1174,22 +1162,20 @@
     "_OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListVodSourcesRequestListVodSourcesPaginateTypeDef(
     _RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef,
     _OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredRequestOutputItemTypeDef = TypedDict(
     "_RequiredRequestOutputItemTypeDef",
     {
         "ManifestName": str,
         "SourceGroup": str,
     },
 )
@@ -1198,21 +1184,19 @@
     {
         "DashPlaylistSettings": DashPlaylistSettingsTypeDef,
         "HlsPlaylistSettings": HlsPlaylistSettingsTypeDef,
     },
     total=False,
 )
 
-
 class RequestOutputItemTypeDef(
     _RequiredRequestOutputItemTypeDef, _OptionalRequestOutputItemTypeDef
 ):
     pass
 
-
 _RequiredResponseOutputItemTypeDef = TypedDict(
     "_RequiredResponseOutputItemTypeDef",
     {
         "ManifestName": str,
         "PlaybackUrl": str,
         "SourceGroup": str,
     },
@@ -1222,21 +1206,19 @@
     {
         "DashPlaylistSettings": DashPlaylistSettingsTypeDef,
         "HlsPlaylistSettings": HlsPlaylistSettingsTypeDef,
     },
     total=False,
 )
 
-
 class ResponseOutputItemTypeDef(
     _RequiredResponseOutputItemTypeDef, _OptionalResponseOutputItemTypeDef
 ):
     pass
 
-
 _RequiredScheduleEntryTypeDef = TypedDict(
     "_RequiredScheduleEntryTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ProgramName": str,
         "SourceLocationName": str,
@@ -1251,34 +1233,53 @@
         "ScheduleAdBreaks": List[ScheduleAdBreakTypeDef],
         "ScheduleEntryType": ScheduleEntryTypeType,
         "VodSourceName": str,
     },
     total=False,
 )
 
-
 class ScheduleEntryTypeDef(_RequiredScheduleEntryTypeDef, _OptionalScheduleEntryTypeDef):
     pass
 
-
-ScheduleConfigurationTypeDef = TypedDict(
-    "ScheduleConfigurationTypeDef",
+_RequiredScheduleConfigurationTypeDef = TypedDict(
+    "_RequiredScheduleConfigurationTypeDef",
     {
         "Transition": TransitionTypeDef,
     },
 )
+_OptionalScheduleConfigurationTypeDef = TypedDict(
+    "_OptionalScheduleConfigurationTypeDef",
+    {
+        "ClipRange": ClipRangeTypeDef,
+    },
+    total=False,
+)
+
+class ScheduleConfigurationTypeDef(
+    _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
+):
+    pass
 
 TimeSignalMessageTypeDef = TypedDict(
     "TimeSignalMessageTypeDef",
     {
         "SegmentationDescriptors": Sequence[SegmentationDescriptorTypeDef],
     },
     total=False,
 )
 
+UpdateProgramScheduleConfigurationTypeDef = TypedDict(
+    "UpdateProgramScheduleConfigurationTypeDef",
+    {
+        "ClipRange": ClipRangeTypeDef,
+        "Transition": UpdateProgramTransitionTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateSourceLocationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSourceLocationRequestRequestTypeDef",
     {
         "HttpConfiguration": HttpConfigurationTypeDef,
         "SourceLocationName": str,
     },
 )
@@ -1289,22 +1290,20 @@
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
         "SegmentDeliveryConfigurations": Sequence[SegmentDeliveryConfigurationTypeDef],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateSourceLocationRequestRequestTypeDef(
     _RequiredCreateSourceLocationRequestRequestTypeDef,
     _OptionalCreateSourceLocationRequestRequestTypeDef,
 ):
     pass
 
-
 CreateSourceLocationResponseTypeDef = TypedDict(
     "CreateSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
@@ -1350,19 +1349,17 @@
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class SourceLocationTypeDef(_RequiredSourceLocationTypeDef, _OptionalSourceLocationTypeDef):
     pass
 
-
 _RequiredUpdateSourceLocationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSourceLocationRequestRequestTypeDef",
     {
         "HttpConfiguration": HttpConfigurationTypeDef,
         "SourceLocationName": str,
     },
 )
@@ -1372,22 +1369,20 @@
         "AccessConfiguration": AccessConfigurationTypeDef,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
         "SegmentDeliveryConfigurations": Sequence[SegmentDeliveryConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateSourceLocationRequestRequestTypeDef(
     _RequiredUpdateSourceLocationRequestRequestTypeDef,
     _OptionalUpdateSourceLocationRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateSourceLocationResponseTypeDef = TypedDict(
     "UpdateSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
@@ -1474,22 +1469,20 @@
         "Tags": Mapping[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
     },
     total=False,
 )
 
-
 class PutPlaybackConfigurationRequestRequestTypeDef(
     _RequiredPutPlaybackConfigurationRequestRequestTypeDef,
     _OptionalPutPlaybackConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 PutPlaybackConfigurationResponseTypeDef = TypedDict(
     "PutPlaybackConfigurationResponseTypeDef",
     {
         "AdDecisionServerUrl": str,
         "AvailSuppression": AvailSuppressionTypeDef,
         "Bumper": BumperTypeDef,
         "CdnConfiguration": CdnConfigurationTypeDef,
@@ -1525,22 +1518,20 @@
     "_OptionalCreatePrefetchScheduleRequestRequestTypeDef",
     {
         "StreamId": str,
     },
     total=False,
 )
 
-
 class CreatePrefetchScheduleRequestRequestTypeDef(
     _RequiredCreatePrefetchScheduleRequestRequestTypeDef,
     _OptionalCreatePrefetchScheduleRequestRequestTypeDef,
 ):
     pass
 
-
 CreatePrefetchScheduleResponseTypeDef = TypedDict(
     "CreatePrefetchScheduleResponseTypeDef",
     {
         "Arn": str,
         "Consumption": PrefetchConsumptionTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
@@ -1577,19 +1568,17 @@
     "_OptionalPrefetchScheduleTypeDef",
     {
         "StreamId": str,
     },
     total=False,
 )
 
-
 class PrefetchScheduleTypeDef(_RequiredPrefetchScheduleTypeDef, _OptionalPrefetchScheduleTypeDef):
     pass
 
-
 ListLiveSourcesResponseTypeDef = TypedDict(
     "ListLiveSourcesResponseTypeDef",
     {
         "Items": List[LiveSourceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1618,21 +1607,19 @@
         "FillerSlate": SlateSourceTypeDef,
         "Tags": Mapping[str, str],
         "Tier": TierType,
     },
     total=False,
 )
 
-
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelName": str,
         "Outputs": Sequence[RequestOutputItemTypeDef],
     },
 )
@@ -1640,21 +1627,19 @@
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "FillerSlate": SlateSourceTypeDef,
     },
     total=False,
 )
 
-
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredChannelTypeDef = TypedDict(
     "_RequiredChannelTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": str,
         "LogConfiguration": LogConfigurationForChannelTypeDef,
@@ -1670,19 +1655,17 @@
         "FillerSlate": SlateSourceTypeDef,
         "LastModifiedTime": datetime,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
     pass
 
-
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": ChannelStateType,
         "CreationTime": datetime,
@@ -1803,28 +1786,28 @@
         "AdBreaks": Sequence[AdBreakTypeDef],
         "LiveSourceName": str,
         "VodSourceName": str,
     },
     total=False,
 )
 
-
 class CreateProgramRequestRequestTypeDef(
     _RequiredCreateProgramRequestRequestTypeDef, _OptionalCreateProgramRequestRequestTypeDef
 ):
     pass
 
-
 CreateProgramResponseTypeDef = TypedDict(
     "CreateProgramResponseTypeDef",
     {
         "AdBreaks": List[AdBreakTypeDef],
         "Arn": str,
         "ChannelName": str,
+        "ClipRange": ClipRangeTypeDef,
         "CreationTime": datetime,
+        "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1832,15 +1815,56 @@
 
 DescribeProgramResponseTypeDef = TypedDict(
     "DescribeProgramResponseTypeDef",
     {
         "AdBreaks": List[AdBreakTypeDef],
         "Arn": str,
         "ChannelName": str,
+        "ClipRange": ClipRangeTypeDef,
+        "CreationTime": datetime,
+        "DurationMillis": int,
+        "LiveSourceName": str,
+        "ProgramName": str,
+        "ScheduledStartTime": datetime,
+        "SourceLocationName": str,
+        "VodSourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUpdateProgramRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProgramRequestRequestTypeDef",
+    {
+        "ChannelName": str,
+        "ProgramName": str,
+        "ScheduleConfiguration": UpdateProgramScheduleConfigurationTypeDef,
+    },
+)
+_OptionalUpdateProgramRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProgramRequestRequestTypeDef",
+    {
+        "AdBreaks": Sequence[AdBreakTypeDef],
+    },
+    total=False,
+)
+
+class UpdateProgramRequestRequestTypeDef(
+    _RequiredUpdateProgramRequestRequestTypeDef, _OptionalUpdateProgramRequestRequestTypeDef
+):
+    pass
+
+UpdateProgramResponseTypeDef = TypedDict(
+    "UpdateProgramResponseTypeDef",
+    {
+        "AdBreaks": List[AdBreakTypeDef],
+        "Arn": str,
+        "ChannelName": str,
+        "ClipRange": ClipRangeTypeDef,
         "CreationTime": datetime,
+        "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor/type_defs.pyi` & `mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,25 +33,27 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "SecretsManagerAccessTokenConfigurationTypeDef",
     "SlateSourceTypeDef",
     "SpliceInsertMessageTypeDef",
     "AdMarkerPassthroughTypeDef",
     "AlertTypeDef",
     "AvailMatchingCriteriaTypeDef",
     "AvailSuppressionTypeDef",
     "BumperTypeDef",
     "CdnConfigurationTypeDef",
     "LogConfigurationForChannelTypeDef",
+    "ClipRangeTypeDef",
     "ConfigureLogsForChannelRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
     "HttpPackageConfigurationTypeDef",
     "PrefetchRetrievalTypeDef",
     "DefaultSegmentDeliveryConfigurationTypeDef",
     "HttpConfigurationTypeDef",
@@ -93,14 +95,15 @@
     "ScheduleAdBreakTypeDef",
     "TransitionTypeDef",
     "SegmentationDescriptorTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateProgramTransitionTypeDef",
     "AccessConfigurationTypeDef",
     "ManifestProcessingRulesTypeDef",
     "PrefetchConsumptionTypeDef",
     "ConfigureLogsForChannelResponseTypeDef",
     "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetChannelPolicyResponseTypeDef",
@@ -127,14 +130,15 @@
     "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
     "ListVodSourcesRequestListVodSourcesPaginateTypeDef",
     "RequestOutputItemTypeDef",
     "ResponseOutputItemTypeDef",
     "ScheduleEntryTypeDef",
     "ScheduleConfigurationTypeDef",
     "TimeSignalMessageTypeDef",
+    "UpdateProgramScheduleConfigurationTypeDef",
     "CreateSourceLocationRequestRequestTypeDef",
     "CreateSourceLocationResponseTypeDef",
     "DescribeSourceLocationResponseTypeDef",
     "SourceLocationTypeDef",
     "UpdateSourceLocationRequestRequestTypeDef",
     "UpdateSourceLocationResponseTypeDef",
     "GetPlaybackConfigurationResponseTypeDef",
@@ -158,14 +162,16 @@
     "ListSourceLocationsResponseTypeDef",
     "ListPlaybackConfigurationsResponseTypeDef",
     "ListPrefetchSchedulesResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateProgramRequestRequestTypeDef",
     "CreateProgramResponseTypeDef",
     "DescribeProgramResponseTypeDef",
+    "UpdateProgramRequestRequestTypeDef",
+    "UpdateProgramResponseTypeDef",
 )
 
 SecretsManagerAccessTokenConfigurationTypeDef = TypedDict(
     "SecretsManagerAccessTokenConfigurationTypeDef",
     {
         "HeaderName": str,
         "SecretArn": str,
@@ -252,14 +258,21 @@
     "LogConfigurationForChannelTypeDef",
     {
         "LogTypes": List[Literal["AS_RUN"]],
     },
     total=False,
 )
 
+ClipRangeTypeDef = TypedDict(
+    "ClipRangeTypeDef",
+    {
+        "EndOffsetMillis": int,
+    },
+)
+
 ConfigureLogsForChannelRequestRequestTypeDef = TypedDict(
     "ConfigureLogsForChannelRequestRequestTypeDef",
     {
         "ChannelName": str,
         "LogTypes": Sequence[Literal["AS_RUN"]],
     },
 )
@@ -303,19 +316,21 @@
     {
         "DynamicVariables": Mapping[str, str],
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class PrefetchRetrievalTypeDef(
     _RequiredPrefetchRetrievalTypeDef, _OptionalPrefetchRetrievalTypeDef
 ):
     pass
 
+
 DefaultSegmentDeliveryConfigurationTypeDef = TypedDict(
     "DefaultSegmentDeliveryConfigurationTypeDef",
     {
         "BaseUrl": str,
     },
     total=False,
 )
@@ -493,20 +508,22 @@
         "DurationMinutes": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetChannelScheduleRequestRequestTypeDef(
     _RequiredGetChannelScheduleRequestRequestTypeDef,
     _OptionalGetChannelScheduleRequestRequestTypeDef,
 ):
     pass
 
+
 GetPlaybackConfigurationRequestRequestTypeDef = TypedDict(
     "GetPlaybackConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -561,19 +578,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAlertsRequestRequestTypeDef(
     _RequiredListAlertsRequestRequestTypeDef, _OptionalListAlertsRequestRequestTypeDef
 ):
     pass
 
+
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -590,19 +609,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListLiveSourcesRequestRequestTypeDef(
     _RequiredListLiveSourcesRequestRequestTypeDef, _OptionalListLiveSourcesRequestRequestTypeDef
 ):
     pass
 
+
 ListPlaybackConfigurationsRequestRequestTypeDef = TypedDict(
     "ListPlaybackConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -620,20 +641,22 @@
         "MaxResults": int,
         "NextToken": str,
         "StreamId": str,
     },
     total=False,
 )
 
+
 class ListPrefetchSchedulesRequestRequestTypeDef(
     _RequiredListPrefetchSchedulesRequestRequestTypeDef,
     _OptionalListPrefetchSchedulesRequestRequestTypeDef,
 ):
     pass
 
+
 ListSourceLocationsRequestRequestTypeDef = TypedDict(
     "ListSourceLocationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -657,19 +680,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListVodSourcesRequestRequestTypeDef(
     _RequiredListVodSourcesRequestRequestTypeDef, _OptionalListVodSourcesRequestRequestTypeDef
 ):
     pass
 
+
 PutChannelPolicyRequestRequestTypeDef = TypedDict(
     "PutChannelPolicyRequestRequestTypeDef",
     {
         "ChannelName": str,
         "Policy": str,
     },
 )
@@ -698,17 +723,19 @@
         "DurationMillis": int,
         "RelativeProgram": str,
         "ScheduledStartTimeMillis": int,
     },
     total=False,
 )
 
+
 class TransitionTypeDef(_RequiredTransitionTypeDef, _OptionalTransitionTypeDef):
     pass
 
+
 SegmentationDescriptorTypeDef = TypedDict(
     "SegmentationDescriptorTypeDef",
     {
         "SegmentNum": int,
         "SegmentationEventId": int,
         "SegmentationTypeId": int,
         "SegmentationUpid": str,
@@ -746,14 +773,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateProgramTransitionTypeDef = TypedDict(
+    "UpdateProgramTransitionTypeDef",
+    {
+        "DurationMillis": int,
+        "ScheduledStartTimeMillis": int,
+    },
+    total=False,
+)
+
 AccessConfigurationTypeDef = TypedDict(
     "AccessConfigurationTypeDef",
     {
         "AccessType": AccessTypeType,
         "SecretsManagerAccessTokenConfiguration": SecretsManagerAccessTokenConfigurationTypeDef,
     },
     total=False,
@@ -778,19 +814,21 @@
     {
         "AvailMatchingCriteria": Sequence[AvailMatchingCriteriaTypeDef],
         "StartTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class PrefetchConsumptionTypeDef(
     _RequiredPrefetchConsumptionTypeDef, _OptionalPrefetchConsumptionTypeDef
 ):
     pass
 
+
 ConfigureLogsForChannelResponseTypeDef = TypedDict(
     "ConfigureLogsForChannelResponseTypeDef",
     {
         "ChannelName": str,
         "LogTypes": List[Literal["AS_RUN"]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -849,19 +887,21 @@
     "_OptionalCreateLiveSourceRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateLiveSourceRequestRequestTypeDef(
     _RequiredCreateLiveSourceRequestRequestTypeDef, _OptionalCreateLiveSourceRequestRequestTypeDef
 ):
     pass
 
+
 CreateLiveSourceResponseTypeDef = TypedDict(
     "CreateLiveSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
@@ -884,19 +924,21 @@
     "_OptionalCreateVodSourceRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateVodSourceRequestRequestTypeDef(
     _RequiredCreateVodSourceRequestRequestTypeDef, _OptionalCreateVodSourceRequestRequestTypeDef
 ):
     pass
 
+
 CreateVodSourceResponseTypeDef = TypedDict(
     "CreateVodSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
@@ -950,17 +992,19 @@
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class LiveSourceTypeDef(_RequiredLiveSourceTypeDef, _OptionalLiveSourceTypeDef):
     pass
 
+
 UpdateLiveSourceRequestRequestTypeDef = TypedDict(
     "UpdateLiveSourceRequestRequestTypeDef",
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
         "LiveSourceName": str,
         "SourceLocationName": str,
     },
@@ -1018,17 +1062,19 @@
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class VodSourceTypeDef(_RequiredVodSourceTypeDef, _OptionalVodSourceTypeDef):
     pass
 
+
 _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
     "_RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
     {
         "ChannelName": str,
     },
 )
 _OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
@@ -1036,40 +1082,44 @@
     {
         "DurationMinutes": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef(
     _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
     _OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
     "_RequiredListAlertsRequestListAlertsPaginateTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
     "_OptionalListAlertsRequestListAlertsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAlertsRequestListAlertsPaginateTypeDef(
     _RequiredListAlertsRequestListAlertsPaginateTypeDef,
     _OptionalListAlertsRequestListAlertsPaginateTypeDef,
 ):
     pass
 
+
 ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
     "ListChannelsRequestListChannelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1084,20 +1134,22 @@
     "_OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListLiveSourcesRequestListLiveSourcesPaginateTypeDef(
     _RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
     _OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
 ):
     pass
 
+
 ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef = TypedDict(
     "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1113,20 +1165,22 @@
     {
         "StreamId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef(
     _RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
     _OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
 ):
     pass
 
+
 ListSourceLocationsRequestListSourceLocationsPaginateTypeDef = TypedDict(
     "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1141,20 +1195,22 @@
     "_OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListVodSourcesRequestListVodSourcesPaginateTypeDef(
     _RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef,
     _OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredRequestOutputItemTypeDef = TypedDict(
     "_RequiredRequestOutputItemTypeDef",
     {
         "ManifestName": str,
         "SourceGroup": str,
     },
 )
@@ -1163,19 +1219,21 @@
     {
         "DashPlaylistSettings": DashPlaylistSettingsTypeDef,
         "HlsPlaylistSettings": HlsPlaylistSettingsTypeDef,
     },
     total=False,
 )
 
+
 class RequestOutputItemTypeDef(
     _RequiredRequestOutputItemTypeDef, _OptionalRequestOutputItemTypeDef
 ):
     pass
 
+
 _RequiredResponseOutputItemTypeDef = TypedDict(
     "_RequiredResponseOutputItemTypeDef",
     {
         "ManifestName": str,
         "PlaybackUrl": str,
         "SourceGroup": str,
     },
@@ -1185,19 +1243,21 @@
     {
         "DashPlaylistSettings": DashPlaylistSettingsTypeDef,
         "HlsPlaylistSettings": HlsPlaylistSettingsTypeDef,
     },
     total=False,
 )
 
+
 class ResponseOutputItemTypeDef(
     _RequiredResponseOutputItemTypeDef, _OptionalResponseOutputItemTypeDef
 ):
     pass
 
+
 _RequiredScheduleEntryTypeDef = TypedDict(
     "_RequiredScheduleEntryTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ProgramName": str,
         "SourceLocationName": str,
@@ -1212,32 +1272,57 @@
         "ScheduleAdBreaks": List[ScheduleAdBreakTypeDef],
         "ScheduleEntryType": ScheduleEntryTypeType,
         "VodSourceName": str,
     },
     total=False,
 )
 
+
 class ScheduleEntryTypeDef(_RequiredScheduleEntryTypeDef, _OptionalScheduleEntryTypeDef):
     pass
 
-ScheduleConfigurationTypeDef = TypedDict(
-    "ScheduleConfigurationTypeDef",
+
+_RequiredScheduleConfigurationTypeDef = TypedDict(
+    "_RequiredScheduleConfigurationTypeDef",
     {
         "Transition": TransitionTypeDef,
     },
 )
+_OptionalScheduleConfigurationTypeDef = TypedDict(
+    "_OptionalScheduleConfigurationTypeDef",
+    {
+        "ClipRange": ClipRangeTypeDef,
+    },
+    total=False,
+)
+
+
+class ScheduleConfigurationTypeDef(
+    _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
+):
+    pass
+
 
 TimeSignalMessageTypeDef = TypedDict(
     "TimeSignalMessageTypeDef",
     {
         "SegmentationDescriptors": Sequence[SegmentationDescriptorTypeDef],
     },
     total=False,
 )
 
+UpdateProgramScheduleConfigurationTypeDef = TypedDict(
+    "UpdateProgramScheduleConfigurationTypeDef",
+    {
+        "ClipRange": ClipRangeTypeDef,
+        "Transition": UpdateProgramTransitionTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateSourceLocationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSourceLocationRequestRequestTypeDef",
     {
         "HttpConfiguration": HttpConfigurationTypeDef,
         "SourceLocationName": str,
     },
 )
@@ -1248,20 +1333,22 @@
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
         "SegmentDeliveryConfigurations": Sequence[SegmentDeliveryConfigurationTypeDef],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateSourceLocationRequestRequestTypeDef(
     _RequiredCreateSourceLocationRequestRequestTypeDef,
     _OptionalCreateSourceLocationRequestRequestTypeDef,
 ):
     pass
 
+
 CreateSourceLocationResponseTypeDef = TypedDict(
     "CreateSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
@@ -1307,17 +1394,19 @@
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class SourceLocationTypeDef(_RequiredSourceLocationTypeDef, _OptionalSourceLocationTypeDef):
     pass
 
+
 _RequiredUpdateSourceLocationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSourceLocationRequestRequestTypeDef",
     {
         "HttpConfiguration": HttpConfigurationTypeDef,
         "SourceLocationName": str,
     },
 )
@@ -1327,20 +1416,22 @@
         "AccessConfiguration": AccessConfigurationTypeDef,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
         "SegmentDeliveryConfigurations": Sequence[SegmentDeliveryConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateSourceLocationRequestRequestTypeDef(
     _RequiredUpdateSourceLocationRequestRequestTypeDef,
     _OptionalUpdateSourceLocationRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateSourceLocationResponseTypeDef = TypedDict(
     "UpdateSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
@@ -1427,20 +1518,22 @@
         "Tags": Mapping[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
     },
     total=False,
 )
 
+
 class PutPlaybackConfigurationRequestRequestTypeDef(
     _RequiredPutPlaybackConfigurationRequestRequestTypeDef,
     _OptionalPutPlaybackConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 PutPlaybackConfigurationResponseTypeDef = TypedDict(
     "PutPlaybackConfigurationResponseTypeDef",
     {
         "AdDecisionServerUrl": str,
         "AvailSuppression": AvailSuppressionTypeDef,
         "Bumper": BumperTypeDef,
         "CdnConfiguration": CdnConfigurationTypeDef,
@@ -1476,20 +1569,22 @@
     "_OptionalCreatePrefetchScheduleRequestRequestTypeDef",
     {
         "StreamId": str,
     },
     total=False,
 )
 
+
 class CreatePrefetchScheduleRequestRequestTypeDef(
     _RequiredCreatePrefetchScheduleRequestRequestTypeDef,
     _OptionalCreatePrefetchScheduleRequestRequestTypeDef,
 ):
     pass
 
+
 CreatePrefetchScheduleResponseTypeDef = TypedDict(
     "CreatePrefetchScheduleResponseTypeDef",
     {
         "Arn": str,
         "Consumption": PrefetchConsumptionTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
@@ -1526,17 +1621,19 @@
     "_OptionalPrefetchScheduleTypeDef",
     {
         "StreamId": str,
     },
     total=False,
 )
 
+
 class PrefetchScheduleTypeDef(_RequiredPrefetchScheduleTypeDef, _OptionalPrefetchScheduleTypeDef):
     pass
 
+
 ListLiveSourcesResponseTypeDef = TypedDict(
     "ListLiveSourcesResponseTypeDef",
     {
         "Items": List[LiveSourceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1565,19 +1662,21 @@
         "FillerSlate": SlateSourceTypeDef,
         "Tags": Mapping[str, str],
         "Tier": TierType,
     },
     total=False,
 )
 
+
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelName": str,
         "Outputs": Sequence[RequestOutputItemTypeDef],
     },
 )
@@ -1585,19 +1684,21 @@
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "FillerSlate": SlateSourceTypeDef,
     },
     total=False,
 )
 
+
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredChannelTypeDef = TypedDict(
     "_RequiredChannelTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": str,
         "LogConfiguration": LogConfigurationForChannelTypeDef,
@@ -1613,17 +1714,19 @@
         "FillerSlate": SlateSourceTypeDef,
         "LastModifiedTime": datetime,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
     pass
 
+
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": ChannelStateType,
         "CreationTime": datetime,
@@ -1744,26 +1847,30 @@
         "AdBreaks": Sequence[AdBreakTypeDef],
         "LiveSourceName": str,
         "VodSourceName": str,
     },
     total=False,
 )
 
+
 class CreateProgramRequestRequestTypeDef(
     _RequiredCreateProgramRequestRequestTypeDef, _OptionalCreateProgramRequestRequestTypeDef
 ):
     pass
 
+
 CreateProgramResponseTypeDef = TypedDict(
     "CreateProgramResponseTypeDef",
     {
         "AdBreaks": List[AdBreakTypeDef],
         "Arn": str,
         "ChannelName": str,
+        "ClipRange": ClipRangeTypeDef,
         "CreationTime": datetime,
+        "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1771,15 +1878,58 @@
 
 DescribeProgramResponseTypeDef = TypedDict(
     "DescribeProgramResponseTypeDef",
     {
         "AdBreaks": List[AdBreakTypeDef],
         "Arn": str,
         "ChannelName": str,
+        "ClipRange": ClipRangeTypeDef,
+        "CreationTime": datetime,
+        "DurationMillis": int,
+        "LiveSourceName": str,
+        "ProgramName": str,
+        "ScheduledStartTime": datetime,
+        "SourceLocationName": str,
+        "VodSourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredUpdateProgramRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateProgramRequestRequestTypeDef",
+    {
+        "ChannelName": str,
+        "ProgramName": str,
+        "ScheduleConfiguration": UpdateProgramScheduleConfigurationTypeDef,
+    },
+)
+_OptionalUpdateProgramRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateProgramRequestRequestTypeDef",
+    {
+        "AdBreaks": Sequence[AdBreakTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateProgramRequestRequestTypeDef(
+    _RequiredUpdateProgramRequestRequestTypeDef, _OptionalUpdateProgramRequestRequestTypeDef
+):
+    pass
+
+
+UpdateProgramResponseTypeDef = TypedDict(
+    "UpdateProgramResponseTypeDef",
+    {
+        "AdBreaks": List[AdBreakTypeDef],
+        "Arn": str,
+        "ChannelName": str,
+        "ClipRange": ClipRangeTypeDef,
         "CreationTime": datetime,
+        "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor.egg-info/PKG-INFO` & `mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediatailor
-Version: 1.26.59
-Summary: Type annotations for boto3.MediaTailor 1.26.59 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.62
+Summary: Type annotations for boto3.MediaTailor 1.26.62 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediatailor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediatailor.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediatailor)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediatailor?color=blue)](https://pypistats.org/packages/mypy-boto3-mediatailor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaTailor 1.26.59](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
+[boto3.MediaTailor 1.26.62](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -371,14 +371,15 @@
     AdMarkerPassthroughTypeDef,
     AlertTypeDef,
     AvailMatchingCriteriaTypeDef,
     AvailSuppressionTypeDef,
     BumperTypeDef,
     CdnConfigurationTypeDef,
     LogConfigurationForChannelTypeDef,
+    ClipRangeTypeDef,
     ConfigureLogsForChannelRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef,
     HttpPackageConfigurationTypeDef,
     PrefetchRetrievalTypeDef,
     DefaultSegmentDeliveryConfigurationTypeDef,
     HttpConfigurationTypeDef,
@@ -420,14 +421,15 @@
     ScheduleAdBreakTypeDef,
     TransitionTypeDef,
     SegmentationDescriptorTypeDef,
     StartChannelRequestRequestTypeDef,
     StopChannelRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateProgramTransitionTypeDef,
     AccessConfigurationTypeDef,
     ManifestProcessingRulesTypeDef,
     PrefetchConsumptionTypeDef,
     ConfigureLogsForChannelResponseTypeDef,
     ConfigureLogsForPlaybackConfigurationResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChannelPolicyResponseTypeDef,
@@ -454,14 +456,15 @@
     ListSourceLocationsRequestListSourceLocationsPaginateTypeDef,
     ListVodSourcesRequestListVodSourcesPaginateTypeDef,
     RequestOutputItemTypeDef,
     ResponseOutputItemTypeDef,
     ScheduleEntryTypeDef,
     ScheduleConfigurationTypeDef,
     TimeSignalMessageTypeDef,
+    UpdateProgramScheduleConfigurationTypeDef,
     CreateSourceLocationRequestRequestTypeDef,
     CreateSourceLocationResponseTypeDef,
     DescribeSourceLocationResponseTypeDef,
     SourceLocationTypeDef,
     UpdateSourceLocationRequestRequestTypeDef,
     UpdateSourceLocationResponseTypeDef,
     GetPlaybackConfigurationResponseTypeDef,
@@ -485,14 +488,16 @@
     ListSourceLocationsResponseTypeDef,
     ListPlaybackConfigurationsResponseTypeDef,
     ListPrefetchSchedulesResponseTypeDef,
     ListChannelsResponseTypeDef,
     CreateProgramRequestRequestTypeDef,
     CreateProgramResponseTypeDef,
     DescribeProgramResponseTypeDef,
+    UpdateProgramRequestRequestTypeDef,
+    UpdateProgramResponseTypeDef,
 )
 
 
 def get_structure() -> SecretsManagerAccessTokenConfigurationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mediatailor-1.26.59/mypy_boto3_mediatailor.egg-info/SOURCES.txt` & `mypy-boto3-mediatailor-1.26.62/mypy_boto3_mediatailor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediatailor-1.26.59/setup.py` & `mypy-boto3-mediatailor-1.26.62/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-mediatailor",
-    version="1.26.59",
+    version="1.26.62",
     packages=["mypy_boto3_mediatailor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaTailor 1.26.59 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.MediaTailor 1.26.62 service generated with mypy-boto3-builder"
         " 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

