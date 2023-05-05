# Comparing `tmp/sapiopylib-2023.4.26.133.tar.gz` & `tmp/sapiopylib-2023.5.5.134.tar.gz`

## Comparing `sapiopylib-2023.4.26.133.tar` & `sapiopylib-2023.5.5.134.tar`

### file list

```diff
@@ -1,93 +1,96 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/INSTALL.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/sapio_input_config.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/sapio_input_data.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/sapio_native_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/csp/__init__.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/PyCspFieldMap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/__init__.py
--rw-r--r--   0        0        0    36940 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/plotly/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/jarvis/QQPlotComputer.py
--rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/AccessionService.py
--rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/CustomReportService.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/DashboardManager.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/DataMgmtService.py
--rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/DataRecordManagerService.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/DataTypeService.py
--rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/ELNService.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/PicklistService.py
--rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/User.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/WebhookService.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/__init__.py
--rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/CustomReport.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecord.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecordPaging.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DateRange.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/Picklist.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/SapioAccessType.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/Sort.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/TableColumn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/__init__.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/ChartData.py
--rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
--rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/__init__.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataType.py
--rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
--rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/__init__.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
--rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
--rw-r--r--   0        0        0    21385 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/__init__.py
--rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
--rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
--rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/__init__.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/DataRecordUtil.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/DataTypeCacheManager.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/FormBuilder.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/FoundationAccessioning.py
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/MultiMap.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/ProtocolUtils.py
--rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/Protocols.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/SapioDateUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/__init__.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/plates/PlatingUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/plates/__init__.py
--rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
--rw-r--r--   0        0        0    45312 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
--rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/tests/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/LICENSE
--rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/README.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/pyproject.toml
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 sapiopylib-2023.4.26.133/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/INSTALL.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/sapio_input_config.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/sapio_input_data.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/sapio_native_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/csp/__init__.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/PyCspFieldMap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/__init__.py
+-rw-r--r--   0        0        0    36940 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/plotly/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/jarvis/QQPlotComputer.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/AccessionService.py
+-rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/CustomReportService.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/DashboardManager.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/DataMgmtService.py
+-rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/DataRecordManagerService.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/DataTypeService.py
+-rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/ELNService.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/GroupManagerService.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/PicklistService.py
+-rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/User.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/UserManagerService.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/WebhookService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/__init__.py
+-rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/CustomReport.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecord.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecordPaging.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DateRange.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/Picklist.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/SapioAccessType.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/Sort.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/TableColumn.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/UserInfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/__init__.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/ChartData.py
+-rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
+-rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/__init__.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataType.py
+-rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
+-rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/__init__.py
+-rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
+-rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
+-rw-r--r--   0        0        0    21385 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/__init__.py
+-rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
+-rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
+-rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/__init__.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/DataRecordUtil.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/DataTypeCacheManager.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/FormBuilder.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/FoundationAccessioning.py
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/MultiMap.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/ProtocolUtils.py
+-rw-r--r--   0        0        0    18079 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/Protocols.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/SapioDateUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/__init__.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/plates/PlatingUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/plates/__init__.py
+-rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
+-rw-r--r--   0        0        0    46781 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
+-rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/tests/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/LICENSE
+-rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/README.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/pyproject.toml
+-rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 sapiopylib-2023.5.5.134/PKG-INFO
```

### Comparing `sapiopylib-2023.4.26.133/INSTALL.md` & `sapiopylib-2023.5.5.134/INSTALL.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/sapio_input_data.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/sapio_input_data.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/sapio_native_tools.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/sapio_native_tools.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/PyCspFieldMap.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/PyCspFieldMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/plotly/PlotlyCspData.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/plotly/PlotlyCspData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/jarvis/QQPlotComputer.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/jarvis/QQPlotComputer.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/AccessionService.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/AccessionService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/CustomReportService.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/CustomReportService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/DashboardManager.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/DashboardManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/DataMgmtService.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/DataMgmtService.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from sapiopylib.rest.DashboardManager import DashboardManager
 from sapiopylib.rest.DataTypeService import DataTypeManager
 
 from sapiopylib.rest.AccessionService import AccessionManager
 from sapiopylib.rest.CustomReportService import CustomReportManager
 from sapiopylib.rest.DataRecordManagerService import DataRecordManager
 from sapiopylib.rest.ELNService import ElnManager
+from sapiopylib.rest.GroupManagerService import VeloxGroupManager
 from sapiopylib.rest.PicklistService import PicklistManager
 from sapiopylib.rest.User import SapioUser
+from sapiopylib.rest.UserManagerService import VeloxUserManager
 
 
 class DataMgmtServer:
     """
     Contains all service points for the current API.
     """
 
@@ -65,7 +67,21 @@
     @staticmethod
     def get_data_type_manager(user: SapioUser) -> DataTypeManager:
         """
         Get the data type manager for the current context.
         :param user: The user auth context.
         """
         return DataTypeManager(user)
+
+    @staticmethod
+    def get_user_manager(user: SapioUser) -> VeloxUserManager:
+        """
+        Get the user manager that contains info about users in the system.
+        """
+        return VeloxUserManager(user)
+
+    @staticmethod
+    def get_group_manager(user: SapioUser) -> VeloxGroupManager:
+        """
+        Get the group manager that contains info about groups and user memberships into groups.
+        """
+        return VeloxGroupManager(user)
```

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/DataRecordManagerService.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/DataRecordManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/DataTypeService.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/DataTypeService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/ELNService.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/ELNService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/PicklistService.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/PicklistService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/User.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/User.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/WebhookService.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/WebhookService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/CustomReport.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/CustomReport.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecord.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecord.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecordPaging.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecordPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/DateRange.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/DateRange.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/Picklist.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/Picklist.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/Sort.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/Sort.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/TableColumn.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/TableColumn.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/ChartData.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/ChartData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataType.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ElnExperiment.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ElnExperiment.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/VeloxRules.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/VeloxRules.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookContext.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/pojo/webhook/WebhookResult.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/pojo/webhook/WebhookResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/DataRecordUtil.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/DataRecordUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/DataTypeCacheManager.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/DataTypeCacheManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/FormBuilder.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/FormBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/FoundationAccessioning.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/FoundationAccessioning.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/MultiMap.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/MultiMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/ProtocolUtils.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/ProtocolUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/Protocols.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/Protocols.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     The protocol/step interface provides natural workflow abstraction for Sapio workflows.
     A protocol is consisted of multiple steps, in a sequential order.
     It is also a single process step for process tracking.
     A step holds the data and presentation config for a part of workflow.
     A step may be completed, active or unlocked.
     The data records that are part of the step are said to be attached to the step.
     """
+
     @abstractmethod
     def get_id(self) -> int:
         pass
 
     @abstractmethod
     def get_name(self) -> str:
         pass
@@ -91,14 +92,30 @@
     The protocol/step interface provides natural workflow abstraction for Sapio workflows.
     A protocol is consisted of multiple steps, in a sequential order.
     It is also a single process step for process tracking.
     A protocol may be completed, cancelled, or in progress.
     A step holds the data and presentation config for a part of workflow.
     The data records that are part of the step are said to be attached to the step.
     """
+
+    @abstractmethod
+    def is_available(self) -> bool:
+        """
+        Returns true if the protocol can still be edited (not submitted or cancelled).
+        """
+        pass
+
+    @abstractmethod
+    def get_record(self) -> Optional[DataRecord]:
+        """
+        Get the data record that stores data of the active protocol, if there are any.
+        For ELN protocols, this is guaranteed to be non-trivial.
+        """
+        pass
+
     @abstractmethod
     def complete_protocol(self) -> None:
         """
         Completing the protocol will complete the current ELN workflow.
         If there are any process-tracking enabled records, these records will advance into the next process step.
         """
         pass
@@ -151,15 +168,15 @@
     def get_options(self) -> Dict[str, str]:
         """
         Get the user-invisible options for the protocol. These can be used for certain plugins.
         """
         pass
 
     @abstractmethod
-    def set_options(self, new_options:  Dict[str, str]) -> None:
+    def set_options(self, new_options: Dict[str, str]) -> None:
         """
         Set the user-invisible options for the protocol. These can be used for certain plugins.
         """
         pass
 
     @abstractmethod
     def invalidate(self) -> None:
@@ -272,14 +289,18 @@
     """
     This is the ELN step implementation ELN-workflow.
     """
     eln_entry: ExperimentEntry
     protocol: ElnExperimentProtocol
     user: SapioUser
 
+    _LOCKED_STATUSES = [ExperimentEntryStatus.Completed, ExperimentEntryStatus.CompletedApproved,
+                        ExperimentEntryStatus.Disabled, ExperimentEntryStatus.LockedAwaitingApproval,
+                        ExperimentEntryStatus.LockedRejected]
+
     def get_name(self) -> str:
         return self.eln_entry.entry_name
 
     def __init__(self, protocol: ElnExperimentProtocol,
                  eln_entry: ExperimentEntry):
         self.protocol = protocol
         self.user = protocol.user
@@ -354,19 +375,34 @@
     This is an ELN-workflow implementation of the workflow protocol.
     """
     sorted_step_list: Optional[List[ElnEntryStep]]
     eln_experiment: ElnExperiment
     user: SapioUser
     lock: threading.RLock
 
+    _protocol_record_cache: Optional[DataRecord]
+    _LOCKED_STATUSES = [ElnExperimentStatus.Completed, ElnExperimentStatus.CompletedApproved,
+                        ElnExperimentStatus.LockedRejected, ElnExperimentStatus.LockedAwaitingApproval,
+                        ElnExperimentStatus.Canceled]
+
+    def get_record(self) -> Optional[DataRecord]:
+        # Keep a cache so continued retrieval over and over again will not cause re-query of DB.
+        if self._protocol_record_cache is not None:
+            return self._protocol_record_cache
+        record_id = self.eln_experiment.experiment_record_id
+        self._protocol_record_cache = DataMgmtServer.get_data_record_manager(self.user).query_system_for_record(
+            ElnBaseDataType.EXPERIMENT.data_type_name, record_id)
+        return self._protocol_record_cache
+
     def __init__(self, eln_experiment: ElnExperiment, user: SapioUser):
         self.lock = threading.RLock()
         self.eln_experiment = eln_experiment
         self.user = user
         self.sorted_step_list = None
+        self._protocol_record_cache = None
 
     def invalidate(self) -> None:
         with self.lock:
             self.sorted_step_list = None
 
     def get_data_type_name(self) -> str:
         return self.eln_experiment.experiment_data_type_name
@@ -382,15 +418,15 @@
     def get_id(self) -> int:
         return self.eln_experiment.notebook_experiment_id
 
     def get_options(self) -> Dict[str, str]:
         eln_manager = DataMgmtServer.get_eln_manager(self.user)
         return eln_manager.get_notebook_experiment_options(self.eln_experiment.notebook_experiment_id)
 
-    def set_options(self, new_options:  Dict[str, str]) -> None:
+    def set_options(self, new_options: Dict[str, str]) -> None:
         eln_manager = DataMgmtServer.get_eln_manager(self.user)
         update_criteria: ElnExperimentUpdateCriteria = ElnExperimentUpdateCriteria(experiment_option_map=new_options)
         eln_manager.update_notebook_experiment(self.eln_experiment.notebook_experiment_id, update_criteria)
 
     def get_sorted_step_list(self) -> List[ElnEntryStep]:
         with self.lock:
             if self.sorted_step_list is not None:
@@ -413,7 +449,11 @@
         eln_manager.update_notebook_experiment(self.eln_experiment.notebook_experiment_id, update_criteria)
 
     def cancel_protocol(self) -> None:
         eln_manager = DataMgmtServer.get_eln_manager(self.user)
         update_criteria: ElnExperimentUpdateCriteria = ElnExperimentUpdateCriteria(
             new_experiment_status=ElnExperimentStatus.Canceled)
         eln_manager.update_notebook_experiment(self.eln_experiment.notebook_experiment_id, update_criteria)
+
+    def is_available(self) -> bool:
+        status: ElnExperimentStatus = self.eln_experiment.notebook_experiment_status
+        return status not in self._LOCKED_STATUSES
```

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/SapioDateUtils.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/SapioDateUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/plates/PlatingUtils.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/plates/PlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,32 +397,32 @@
         if self.__initialized:
             return
         self._record_model_manager = record_model_manager
         self.__side_link_handler = _RelationshipSideLinkHandler(self)
         self._record_model_manager.event_bus.subscribe_side_link_changed_event(self.__side_link_handler)
         self.__initialized = True
 
-    def load_forward_side_links_of_type(self, records: List[WrappedRecordModel], field_name: str):
+    def load_forward_side_links_of_type(self, wrapped_records: List[WrappedRecordModel], field_name: str):
         """
         Load forward side links from these records. This is the wrapper version.
-        :param records: The records to be loaded.
+        :param wrapped_records: The wrapped records to be loaded.
         :param field_name: The field name to be loaded for these records.
         """
-        self.load_forward_side_links(RecordModelWrapperUtil.unwrap_list(records), field_name)
+        self.load_forward_side_links(RecordModelWrapperUtil.unwrap_list(wrapped_records), field_name)
 
-    def load_forward_side_links(self, records: List[PyRecordModel], field_name: str) -> None:
+    def load_forward_side_links(self, root_records: List[PyRecordModel], field_name: str) -> None:
         """
         Load forward side links from these records.
-        :param records: The records to be loaded.
+        :param root_records: The root records to be loaded.
         :param field_name: The field name to be loaded for these records.
         """
-        if not records:
+        if not root_records:
             return
         records_by_dt_name: SetMultimap[str, PyRecordModel] = \
-            RecordModelUtil.multi_map_models_by_data_type_name(records)
+            RecordModelUtil.multi_map_models_by_data_type_name(root_records)
         for dt_name in records_by_dt_name:
             models_to_load: List[PyRecordModel] = list()
             models_of_type = records_by_dt_name.get(dt_name)
             for model in models_of_type:
                 if model.is_deleted:
                     continue
                 if model.is_forward_side_link_loaded(field_name):
@@ -455,44 +455,44 @@
                     link = inst_man._get_or_add_record(link_rec)
                     # noinspection PyProtectedMember
                     source_model._mark_forward_side_link_loaded(field_name, link.record_id)
                 else:
                     # noinspection PyProtectedMember
                     source_model._mark_forward_side_link_loaded(field_name, None)
 
-    def load_reverse_side_links_of_type(self, records: List[WrappedRecordModel],
+    def load_reverse_side_links_of_type(self, wrapped_records: List[WrappedRecordModel],
                                         reverse_link_type: Type[WrappedRecordModel],
                                         reverse_link_field_name: str) -> None:
         """
         Load the reverse side links of provided records (wrapped records version)
-        :param records: The records to be loaded
+        :param wrapped_records: The wrapped records to be loaded
         :param reverse_link_type: The reverse side link data type name of records that will point to these records.
         :param reverse_link_field_name: The field name on the reverse side link data type that will point
         to these records.
         :return: The records that will be linked to at least one of the records provided as input.
         """
-        self.load_reverse_side_links(RecordModelWrapperUtil.unwrap_list(records),
+        self.load_reverse_side_links(RecordModelWrapperUtil.unwrap_list(wrapped_records),
                                      reverse_link_dt_name=reverse_link_type.get_wrapper_data_type_name(),
                                      reverse_link_field_name=reverse_link_field_name)
 
-    def load_reverse_side_links(self, records: List[PyRecordModel], reverse_link_dt_name: str,
+    def load_reverse_side_links(self, root_records: List[PyRecordModel], reverse_link_dt_name: str,
                                 reverse_link_field_name: str) -> None:
         """
         Load the reverse side links of provided records
-        :param records: The records to be loaded
+        :param root_records: The root records to be loaded
         :param reverse_link_dt_name: The reverse side link data type name of records that will point to these records.
         :param reverse_link_field_name: The field name on the reverse side link data type that will point
         to these records.
         :return: The records that will be linked to at least one of the records provided as input.
         """
-        if not records:
+        if not root_records:
             return
         cache_key = RecordModelReverseSideLinkCacheKey(reverse_link_dt_name, reverse_link_field_name)
         models_to_load: List[PyRecordModel] = list()
-        for record in records:
+        for record in root_records:
             if record.is_deleted:
                 continue
             if record.is_reverse_side_link_loaded_key(cache_key):
                 continue
             models_to_load.append(record)
         if not models_to_load:
             return
@@ -519,34 +519,39 @@
             # noinspection PyProtectedMember
             link_models = [inst_man._get_or_add_record(x) for x in links]
             # noinspection PyProtectedMember
             target_model._mark_reverse_side_link_loaded(back_side_link_dt_name=reverse_link_dt_name,
                                                         back_side_link_field_name=reverse_link_field_name,
                                                         loaded_side_links=link_models)
 
-    def load_children_of_type(self, records: List[WrappedRecordModel], child_wrapped_type: Type[WrappedRecordModel]) \
+    def load_children_of_type(self, wrapped_records: List[WrappedRecordModel], child_wrapped_type: Type[WrappedRecordModel]) \
             -> None:
         """
         Load children that we have not traversed yet.
 
         This call will not do anything to models that are deleted, models that are new,
         or models with children loaded already.
+        :param wrapped_records wrapped records of record model list
+        :param child_wrapped_type the wrapped child class type to load for these records.
         """
         child_type_name: str = child_wrapped_type.get_wrapper_data_type_name()
-        return self.load_children(RecordModelWrapperUtil.unwrap_list(records), child_type_name)
+        return self.load_children(RecordModelWrapperUtil.unwrap_list(wrapped_records), child_type_name)
 
-    def load_children(self, records: List[PyRecordModel], child_type_name: str) -> None:
+    def load_children(self, root_records: List[PyRecordModel], child_type_name: str) -> None:
         """
         Load children that we have not traversed yet.
 
         This call will not do anything to models that are deleted, models that are new,
         or models with children loaded already.
+
+        :param root_records root records of record model list.
+        :param child_type_name the child data type name to load for these records.
         """
         models_to_load: Set[PyRecordModel] = set()
-        for record in records:
+        for record in root_records:
             if record.is_children_loaded(child_type_name):
                 continue
             models_to_load.add(record)
 
         if not models_to_load:
             return
 
@@ -567,34 +572,38 @@
         inst_man = self._record_model_manager.instance_manager
         for source_record_id, children_record_list in result_map.items():
             source_model: PyRecordModel = inst_man.get_known_record_with_record_id(source_record_id)
             children_model_list: List[PyRecordModel] = inst_man.add_existing_records(children_record_list)
             # noinspection PyProtectedMember
             source_model._mark_children_loaded(child_type_name, children_model_list)
 
-    def load_parents_of_type(self, records: List[WrappedRecordModel], parent_wrapper_type: Type[WrappedRecordModel]) \
+    def load_parents_of_type(self, wrapped_records: List[WrappedRecordModel], parent_wrapper_type: Type[WrappedRecordModel]) \
             -> None:
         """
         Load parents that we have not traversed yet.
 
         This call will not do anything to models that are deleted, models that are new,
         or models with parents loaded already.
+        :param wrapped_records wrapped record list of record models.
+        :param parent_wrapper_type the parent wrapper class type to retrieve parent records for.
         """
-        return self.load_parents(RecordModelWrapperUtil.unwrap_list(records),
+        return self.load_parents(RecordModelWrapperUtil.unwrap_list(wrapped_records),
                                  parent_wrapper_type.get_wrapper_data_type_name())
 
-    def load_parents(self, records: List[PyRecordModel], parent_type_name: str) -> None:
+    def load_parents(self, root_records: List[PyRecordModel], parent_type_name: str) -> None:
         """
         Load parents that we have not traversed yet.
 
         This call will not do anything to models that are deleted, models that are new,
         or models with parents loaded already.
+        :param root_records root record list of record models.
+        :param parent_type_name the parent data type name to load.
         """
         models_to_load: Set[PyRecordModel] = set()
-        for record in records:
+        for record in root_records:
             if record.is_parents_loaded(parent_type_name):
                 continue
             models_to_load.add(record)
 
         if not models_to_load:
             return
 
@@ -615,21 +624,33 @@
         inst_man = self._record_model_manager.instance_manager
         for source_record_id, parent_record_list in result_map.items():
             source_model: PyRecordModel = inst_man.get_known_record_with_record_id(source_record_id)
             parent_model_list: List[PyRecordModel] = inst_man.add_existing_records(parent_record_list)
             # noinspection PyProtectedMember
             source_model._mark_parents_loaded(parent_type_name, parent_model_list)
 
-    def load_path(self, records: List[PyRecordModel], rel_path: RelationshipPath):
+    def load_path_of_type(self, wrapped_records: List[WrappedRecordModel], rel_path: RelationshipPath) -> None:
+        """
+        Load an entire path of records that we need to load along this path.
+        If any parents or children for any records along this way are already loaded, it will not attempt to reload.
+        :param wrapped_records: wrapped records list.
+        :param rel_path: the relationship path to load.
+        """
+        unwrapped_records = RecordModelWrapperUtil.unwrap_list(wrapped_records)
+        return self.load_path(unwrapped_records, rel_path)
+
+    def load_path(self, root_records: List[PyRecordModel], rel_path: RelationshipPath) -> None:
         """
         Load an entire path of records that we need to load along this path.
         If any parents or children for any records along this way are already loaded, it will not attempt to reload.
+        :param root_records: root records list.
+        :param rel_path: the relationship path to load.
         """
         path: List[Tuple[RelationshipPathDir, str]] = rel_path.path
-        cur_records: List[PyRecordModel] = records
+        cur_records: List[PyRecordModel] = root_records
         for direction, dt_name in path:
             next_records: List[PyRecordModel] = []
             if direction == RelationshipPathDir.PARENT:
                 self.load_parents(cur_records, dt_name)
                 for record in cur_records:
                     parents = record.get_parents_of_type(dt_name)
                     for parent in parents:
```

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py` & `sapiopylib-2023.5.5.134/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/LICENSE` & `sapiopylib-2023.5.5.134/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/README.md` & `sapiopylib-2023.5.5.134/README.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.26.133/pyproject.toml` & `sapiopylib-2023.5.5.134/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopylib"
-version='2023.04.26.133'
+version='2023.05.05.134'
 authors = [
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Informatics Platform Python API"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `sapiopylib-2023.4.26.133/PKG-INFO` & `sapiopylib-2023.5.5.134/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapiopylib
-Version: 2023.4.26.133
+Version: 2023.5.5.134
 Summary: Official Sapio Informatics Platform Python API
 Project-URL: Homepage, https://github.com/sapiosciences
 Project-URL: Bug Tracker, https://github.com/sapiosciences/sapio-py-tutorials/issues
 Author-email: Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
```

