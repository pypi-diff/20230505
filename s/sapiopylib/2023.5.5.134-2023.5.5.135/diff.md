# Comparing `tmp/sapiopylib-2023.5.5.134.tar.gz` & `tmp/sapiopylib-2023.5.5.135.tar.gz`

## Comparing `sapiopylib-2023.5.5.134.tar` & `sapiopylib-2023.5.5.135.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/INSTALL.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/sapio_input_config.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/sapio_input_data.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/sapio_native_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/csp/__init__.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/PyCspFieldMap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/__init__.py
--rw-r--r--   0        0        0    36940 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/plotly/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/jarvis/QQPlotComputer.py
--rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/AccessionService.py
--rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/CustomReportService.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/DashboardManager.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/DataMgmtService.py
--rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/DataRecordManagerService.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/DataTypeService.py
--rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/ELNService.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/GroupManagerService.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/PicklistService.py
--rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/User.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/UserManagerService.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/WebhookService.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/__init__.py
--rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/CustomReport.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecord.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecordPaging.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DateRange.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/Picklist.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/SapioAccessType.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/Sort.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/TableColumn.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/UserInfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/__init__.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/ChartData.py
--rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
--rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/__init__.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataType.py
--rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
--rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/__init__.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
--rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
--rw-r--r--   0        0        0    21385 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/__init__.py
--rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
--rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
--rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/__init__.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/DataRecordUtil.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/DataTypeCacheManager.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/FormBuilder.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/FoundationAccessioning.py
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/MultiMap.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/ProtocolUtils.py
--rw-r--r--   0        0        0    18079 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/Protocols.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/SapioDateUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/__init__.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/plates/PlatingUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/plates/__init__.py
--rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
--rw-r--r--   0        0        0    46781 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
--rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/tests/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/LICENSE
--rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/README.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/pyproject.toml
--rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/INSTALL.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/sapio_input_config.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/sapio_input_data.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/sapio_native_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/csp/__init__.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/PyCspFieldMap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/__init__.py
+-rw-r--r--   0        0        0    36940 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/plotly/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/jarvis/QQPlotComputer.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/AccessionService.py
+-rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/CustomReportService.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/DashboardManager.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/DataMgmtService.py
+-rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/DataRecordManagerService.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/DataTypeService.py
+-rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/ELNService.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/GroupManagerService.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/PicklistService.py
+-rw-r--r--   0        0        0    10810 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/User.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/UserManagerService.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/WebhookService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/__init__.py
+-rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/CustomReport.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecord.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecordPaging.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DateRange.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/Picklist.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/SapioAccessType.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/Sort.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/TableColumn.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/UserInfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/__init__.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/ChartData.py
+-rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
+-rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/__init__.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataType.py
+-rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
+-rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/__init__.py
+-rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
+-rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
+-rw-r--r--   0        0        0    21385 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/__init__.py
+-rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
+-rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
+-rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/__init__.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/DataRecordUtil.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/DataTypeCacheManager.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/FormBuilder.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/FoundationAccessioning.py
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/MultiMap.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/ProtocolUtils.py
+-rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/Protocols.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/SapioDateUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/__init__.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/plates/PlatingUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/plates/__init__.py
+-rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
+-rw-r--r--   0        0        0    46781 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
+-rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/tests/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/LICENSE
+-rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/README.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/pyproject.toml
+-rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.135/PKG-INFO
```

### Comparing `sapiopylib-2023.5.5.134/INSTALL.md` & `sapiopylib-2023.5.5.135/INSTALL.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/sapio_input_data.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/sapio_input_data.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/sapio_native_tools.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/sapio_native_tools.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/PyCspFieldMap.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/PyCspFieldMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/plotly/PlotlyCspData.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/plotly/PlotlyCspData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/jarvis/QQPlotComputer.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/jarvis/QQPlotComputer.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/AccessionService.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/AccessionService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/CustomReportService.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/CustomReportService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/DashboardManager.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/DashboardManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/DataMgmtService.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/DataMgmtService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/DataRecordManagerService.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/DataRecordManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/DataTypeService.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/DataTypeService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/ELNService.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/ELNService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/GroupManagerService.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/GroupManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/PicklistService.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/PicklistService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/User.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/User.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,57 @@
+from __future__ import annotations
 import sys
 import urllib.parse
 from base64 import b64encode
-from typing import Optional, Callable, List
+from typing import Optional, Callable, List, Dict, Any
 
 import requests
 from requests import Response
 from typing.io import IO
 import logging
 
 
+class UserSessionAdditionalData:
+    """
+    The session info for the current session. This is not necessary to establish connection from client to server,
+    but can provide useful info for a webservice user program.
+    """
+    current_group_id: Optional[int]
+    current_group_name: Optional[str]
+    first_name: Optional[str]
+    middle_name: Optional[str]
+    last_name: Optional[str]
+    email: Optional[str]
+    utc_offset_seconds: int
+
+    def __init__(self, current_group_id: Optional[int], current_group_name: Optional[str],
+                 first_name: Optional[str], middle_name: Optional[str], last_name: Optional[str], email: Optional[str],
+                 utc_offset_seconds: int):
+        self.current_group_id = current_group_id
+        self.current_group_name = current_group_name
+        self.first_name = first_name
+        self.middle_name = middle_name
+        self.last_name = last_name
+        self.email = email
+        self.utc_offset_seconds = utc_offset_seconds
+
+
+def parse_session_additional_data(json_dct: Dict[str, Any]) -> UserSessionAdditionalData:
+    current_group_id: Optional[int] = json_dct.get('currentGroupId')
+    current_group_name: Optional[str] = json_dct.get('currentGroupName')
+    first_name: Optional[str] = json_dct.get('firstName')
+    middle_name: Optional[str] = json_dct.get('middleName')
+    last_name: Optional[str] = json_dct.get('lastName')
+    email: Optional[str] = json_dct.get('email')
+    utc_offset_seconds: int = json_dct.get('utcOffsetSeconds')
+    return UserSessionAdditionalData(current_group_id=current_group_id, current_group_name=current_group_name,
+                                     first_name=first_name, middle_name=middle_name, last_name=last_name,
+                                     email=email, utc_offset_seconds=utc_offset_seconds)
+
+
 class SapioServerException(Exception):
     """
     This will be thrown when the client cannot perform an operation.
     """
     client_error: requests.exceptions.HTTPError
 
     def __init__(self, client_error: requests.exceptions.HTTPError):
@@ -53,18 +92,21 @@
     guid: Optional[str]
     account_name: Optional[str]
     verify_ssl_cert: bool
     timeout_seconds: int
     __next_temp_record_id: int
     logger: logging.Logger
 
+    _session_additional_data: Optional[UserSessionAdditionalData]
+
     def __init__(self, url: str,
                  verify_ssl_cert: bool = True, timeout_seconds: int = 60,
                  api_token: str = None, username: str = None, password: str = None,
-                 guid: str = None, account_name: str = None):
+                 guid: str = None, account_name: str = None,
+                 session_additional_data: Optional[UserSessionAdditionalData] = None):
         """
         Create a new Sapio REST API Client object using API Token. Typically ends with "/webservice/api".
 
         :param url: The URL of root of REST API APPLICATION. For example: https://localhost/webservice/api
         :param api_token: The API token to authenticate the platform API user. Use App Config Manager to obtain this.
         :param guid: When using username/password authentication, provide GUID of the app. Obtain from Sapio Portal.
         :param username: When using username/password authentication, the username of the credential.
@@ -78,14 +120,15 @@
         self.username = username
         self.password = password
         self.verify_ssl_cert = verify_ssl_cert
         self.timeout_seconds = timeout_seconds
         self.account_name = account_name
         self.__next_temp_record_id = -1
         self.logger = logging.getLogger("SapioUser")
+        self._session_additional_data = session_additional_data
         ensure_logger_initialized(self.logger)
 
     def get_http_headers(self) -> dict:
         ret = {
             'user-agent': 'SapioAnalyticsPyLib'
         }
         if self.account_name is not None:
@@ -195,8 +238,16 @@
         Prefix each log from this context with the username and URL of the service.
         """
         prefix: str = "<" + self.url + "> "
         if self.username:
             prefix = self.username + ": "
         return prefix
 
-
+    @property
+    def session_additional_data(self) -> UserSessionAdditionalData:
+        if self._session_additional_data is not None:
+            return self._session_additional_data
+        sub_url = '/user/currentsession/additionaldata'
+        response = self.get(sub_url)
+        self.raise_for_status(response)
+        self._session_additional_data = parse_session_additional_data(response.json())
+        return self._session_additional_data
```

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/UserManagerService.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/UserManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/WebhookService.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/WebhookService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/CustomReport.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/CustomReport.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecord.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecord.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecordPaging.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecordPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DateRange.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/DateRange.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/Picklist.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/Picklist.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/Sort.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/Sort.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/TableColumn.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/TableColumn.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/UserInfo.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/UserInfo.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/ChartData.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/ChartData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataType.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ElnExperiment.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ElnExperiment.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,18 +48,18 @@
 
     @staticmethod
     def parse_group_role(json_dct: Dict[str, Any]) -> ElnGroupExperimentRole:
         return _parse_group_role(json_dct)
 
 
 def _parse_abstract_role(json_dct: Dict[str, Any]) -> AbstractElnExperimentRole:
-    is_author: bool = json_dct.get('isAuthor')
-    is_witness: bool = json_dct.get('isWitness')
-    is_reviewer: bool = json_dct.get('isReviewer')
-    is_approver: bool = json_dct.get('isApprover')
+    is_author: bool = json_dct.get('author')
+    is_witness: bool = json_dct.get('witness')
+    is_reviewer: bool = json_dct.get('reviewer')
+    is_approver: bool = json_dct.get('approver')
     return AbstractElnExperimentRole(is_author=is_author, is_witness=is_witness,
                                      is_reviewer=is_reviewer, is_approver=is_approver)
 
 
 def _parse_user_role(json_dct: Dict[str, Any]) -> ElnUserExperimentRole:
     abstract_role: AbstractElnExperimentRole = _parse_abstract_role(json_dct)
     username = json_dct.get('username')
```

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/VeloxRules.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/VeloxRules.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookContext.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookContext.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from sapiopylib.rest.ELNService import ElnManager
 
 from sapiopylib.rest.DataRecordManagerService import DataRecordManager
 
 from sapiopylib.rest.pojo.DataRecord import DataRecord
 
-from sapiopylib.rest.User import SapioUser
+from sapiopylib.rest.User import SapioUser, UserSessionAdditionalData, parse_session_additional_data
 from sapiopylib.rest.pojo.eln.ElnExperiment import ElnExperiment, ELNExperimentParser
 from sapiopylib.rest.pojo.eln.ExperimentEntry import ExperimentEntry, ExperimentEntryParser
 from sapiopylib.rest.pojo.reportbuilder.VeloxReportBuilder import RbTemplatePopulatorData, VeloxReportBuilderParser
 from sapiopylib.rest.pojo.webhook.ClientCallbackResult import ClientCallbackResultParser, AbstractClientCallbackResult
 from sapiopylib.rest.pojo.webhook.VeloxRules import VeloxTypedRuleResult, ElnEntryRecordResult, VeloxRuleParser
 from sapiopylib.rest.pojo.webhook.WebhookEnums import WebhookEndpointType
 from sapiopylib.rest.utils.Protocols import AbstractProtocol, ElnExperimentProtocol, \
@@ -82,17 +82,21 @@
         # Remove trailing "/"
         if webservice_url.endswith('/'):
             webservice_url = webservice_url[:-len('/')]
         api_token: str = json_dct.get('webhookApiToken')
         username: str = json_dct.get('username')
         app_guid: str = json_dct.get('appGuid')
         context_data: str = json_dct.get('contextData')
+        session_additional_data: Optional[UserSessionAdditionalData] = None
+        session_additional_data_raw: Dict[str, Any] = json_dct.get('sessionAdditionalData')
+        if session_additional_data_raw:
+            session_additional_data = parse_session_additional_data(session_additional_data_raw)
         user: SapioUser = SapioUser(url=webservice_url, verify_ssl_cert=verify_ssl_cert,
                                     timeout_seconds=timeout_seconds, api_token=api_token,
-                                    username=username, guid=app_guid)
+                                    username=username, guid=app_guid, session_additional_data=session_additional_data)
         data_record: Optional[DataRecord] = None
         if json_dct.get('dataRecordPojo') is not None:
             data_record = DataRecord.from_json(json_dct.get('dataRecordPojo'))
         base_data_record: Optional[DataRecord] = None
         if json_dct.get('baseDataRecordPojo') is not None:
             base_data_record = DataRecord.from_json(json_dct.get('baseDataRecordPojo'))
         data_record_list: Optional[List[DataRecord]] = None
```

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookResult.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/pojo/webhook/WebhookResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/DataRecordUtil.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/DataRecordUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/DataTypeCacheManager.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/DataTypeCacheManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/FormBuilder.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/FormBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/FoundationAccessioning.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/FoundationAccessioning.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/MultiMap.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/MultiMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/ProtocolUtils.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/ProtocolUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/Protocols.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/Protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,21 @@
     def complete_step(self) -> None:
         pass
 
     @abstractmethod
     def unlock_step(self) -> None:
         pass
 
+    @abstractmethod
+    def is_available(self) -> bool:
+        """
+        Returns true if user can make edits to the step right now.
+        """
+        pass
+
     def __hash__(self):
         return hash(self.get_id())
 
     def __eq__(self, other):
         if other is None:
             return False
         if not isinstance(other, AbstractStep):
@@ -365,14 +372,36 @@
     def set_name(self, new_name: str) -> None:
         eln_manager = DataMgmtServer.get_eln_manager(self.user)
         entry_update_criteria = ExperimentEntryCriteriaUtil.create_empty_criteria(self.eln_entry)
         entry_update_criteria.entry_name = new_name
         eln_manager.update_experiment_entry(self.protocol.eln_experiment.notebook_experiment_id,
                                             self.eln_entry.entry_id, entry_update_criteria)
 
+    def is_available(self) -> bool:
+        # ELN Experiment must not be submitted yet.
+        if not self.protocol.is_available():
+            return False
+        # This entry must not be submitted yet.
+        status = self.eln_entry.entry_status
+        if status in self._LOCKED_STATUSES:
+            return False
+        # Either my current user is an author, or my current group is an author.
+        user_assignments = self.protocol.eln_experiment.user_roles
+        user_role = user_assignments.get(self.user.username)
+        if user_role is not None:
+            if user_role.is_author:
+                return True
+        current_group_id = self.user.session_additional_data.current_group_id
+        if current_group_id is not None:
+            group_assignments = self.protocol.eln_experiment.group_roles
+            group_role = group_assignments.get(current_group_id)
+            if group_role is not None:
+                return group_role.is_author
+        return False
+
 
 class ElnExperimentProtocol(AbstractProtocol[ElnEntryStep]):
     """
     This is an ELN-workflow implementation of the workflow protocol.
     """
     sorted_step_list: Optional[List[ElnEntryStep]]
     eln_experiment: ElnExperiment
```

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/SapioDateUtils.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/SapioDateUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/plates/PlatingUtils.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/plates/PlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py` & `sapiopylib-2023.5.5.135/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/LICENSE` & `sapiopylib-2023.5.5.135/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/README.md` & `sapiopylib-2023.5.5.135/README.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.5.5.134/pyproject.toml` & `sapiopylib-2023.5.5.135/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopylib"
-version='2023.05.05.134'
+version='2023.05.05.135'
 authors = [
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Informatics Platform Python API"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `sapiopylib-2023.5.5.134/PKG-INFO` & `sapiopylib-2023.5.5.135/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapiopylib
-Version: 2023.5.5.134
+Version: 2023.5.5.135
 Summary: Official Sapio Informatics Platform Python API
 Project-URL: Homepage, https://github.com/sapiosciences
 Project-URL: Bug Tracker, https://github.com/sapiosciences/sapio-py-tutorials/issues
 Author-email: Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
```

