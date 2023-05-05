# Comparing `tmp/pyaedt-0.6.73.tar.gz` & `tmp/pyaedt-0.6.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.6.73.tar", last modified: Fri Apr 28 12:20:16 2023, max compression
+gzip compressed data, was "pyaedt-0.6.74.tar", last modified: Fri May  5 15:05:33 2023, max compression
```

## Comparing `pyaedt-0.6.73.tar` & `pyaedt-0.6.74.tar`

### file list

```diff
@@ -1,251 +1,251 @@
--rw-r--r--   0        0        0     1111 2023-04-27 10:48:38.937375 pyaedt-0.6.73/LICENSE
--rw-r--r--   0        0        0    10041 2023-04-27 10:48:38.937375 pyaedt-0.6.73/README.rst
--rw-r--r--   0        0        0     2503 2023-04-28 12:05:25.194514 pyaedt-0.6.73/pyaedt/__init__.py
--rw-r--r--   0        0        0    26253 2023-04-27 10:48:40.495559 pyaedt-0.6.73/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6965 2023-04-27 10:48:40.495559 pyaedt-0.6.73/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    88739 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    41260 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    17009 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3088 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    19795 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4374 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4539 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   127521 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6115 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    75493 2023-04-27 13:08:15.716301 pyaedt-0.6.73/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12433 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    37014 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    57605 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/circuit.py
--rw-r--r--   0        0        0    10034 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    57382 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/desktop.py
--rw-r--r--   0        0        0    15104 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/dlls/PDFReport/AnsysReport.deps.json
--rw-r--r--   0        0        0    23552 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/dlls/PDFReport/AnsysReport.dll
--rw-r--r--   0        0        0     1092 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/dlls/PDFReport/AnsysTemplate.json
--rw-r--r--   0        0        0   204800 2023-04-27 10:48:40.511198 pyaedt-0.6.73/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
--rw-r--r--   0        0        0   577445 2023-04-27 10:48:40.526826 pyaedt-0.6.73/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
--rw-r--r--   0        0        0     9836 2023-04-27 10:48:40.526826 pyaedt-0.6.73/pyaedt/dlls/PDFReport/Images/Ansys.png
--rw-r--r--   0        0        0   238592 2023-04-27 10:48:40.526826 pyaedt-0.6.73/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
--rw-r--r--   0        0        0   115712 2023-04-27 10:48:40.526826 pyaedt-0.6.73/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
--rw-r--r--   0        0        0   705296 2023-04-27 10:48:40.526826 pyaedt-0.6.73/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
--rw-r--r--   0        0        0   712253 2023-04-27 10:48:40.542451 pyaedt-0.6.73/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
--rw-r--r--   0        0        0    80384 2023-04-27 10:48:40.542451 pyaedt-0.6.73/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
--rw-r--r--   0        0        0   546816 2023-04-27 10:48:40.542451 pyaedt-0.6.73/pyaedt/dlls/PDFReport/PdfSharpCore.dll
--rw-r--r--   0        0        0   367616 2023-04-27 10:48:40.542451 pyaedt-0.6.73/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
--rw-r--r--   0        0        0   536367 2023-04-27 10:48:40.558076 pyaedt-0.6.73/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
--rw-r--r--   0        0        0  1229824 2023-04-27 10:48:40.558076 pyaedt-0.6.73/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
--rw-r--r--   0        0        0  3285773 2023-04-27 10:48:40.589270 pyaedt-0.6.73/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
--rw-r--r--   0        0        0   120664 2023-04-27 10:48:40.589270 pyaedt-0.6.73/pyaedt/dlls/PDFReport/System.Runtime.dll
--rw-r--r--   0        0        0  1505294 2023-04-27 10:48:40.589270 pyaedt-0.6.73/pyaedt/dlls/PDFReport/System.Runtime.xml
--rw-r--r--   0        0        0     5632 2023-04-27 10:48:40.589270 pyaedt-0.6.73/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
--rw-r--r--   0        0        0   160754 2023-04-27 10:48:40.589270 pyaedt-0.6.73/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
--rw-r--r--   0        0        0    23386 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/downloads.py
--rw-r--r--   0        0        0   132412 2023-04-28 08:23:04.967029 pyaedt-0.6.73/pyaedt/edb.py
--rw-r--r--   0        0        0      333 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/__init__.py
--rw-r--r--   0        0        0    87982 2023-04-28 08:59:15.508478 pyaedt-0.6.73/pyaedt/edb_core/components.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    32856 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0      937 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0      324 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/edb_builder.py
--rw-r--r--   0        0        0     1166 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    12081 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/hfss_extent_info.py
--rw-r--r--   0        0        0    65580 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    20305 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     4724 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    61111 2023-04-27 15:58:46.158994 pyaedt-0.6.73/pyaedt/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0    32298 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0    99826 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    36282 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    31276 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0     4147 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     2425 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     3258 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/general.py
--rw-r--r--   0        0        0    60863 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/hfss.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.604919 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0      673 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     1283 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     2213 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0      524 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/__init__.py
--rw-r--r--   0        0        0      768 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/color.py
--rw-r--r--   0        0        0     2118 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/content.py
--rw-r--r--   0        0        0      938 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0      921 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     1029 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0      416 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0      548 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0      523 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/fill.py
--rw-r--r--   0        0        0      284 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     2844 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     1183 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     1319 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     1516 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0      960 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     1964 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     1158 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     7706 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0      921 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     1079 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     4646 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     1440 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0      875 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     2775 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0      887 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     4104 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     2567 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     1002 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8010 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0      663 2023-04-27 10:48:40.620538 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     1162 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     1626 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0      838 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    11163 2023-04-28 08:59:15.508478 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     1033 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0      683 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     2008 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     1624 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/history_record.py
--rw-r--r--   0        0        0    21750 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ipc2581.py
--rw-r--r--   0        0        0      966 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/edb_core/ipc2581/logistic_header.py
--rw-r--r--   0        0        0    47799 2023-04-27 15:58:46.158994 pyaedt-0.6.73/pyaedt/edb_core/layout.py
--rw-r--r--   0        0        0    33242 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/edb_core/materials.py
--rw-r--r--   0        0        0    43680 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/edb_core/nets.py
--rw-r--r--   0        0        0    45432 2023-04-28 08:59:15.508478 pyaedt-0.6.73/pyaedt/edb_core/padstack.py
--rw-r--r--   0        0        0    57133 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/edb_core/siwave.py
--rw-r--r--   0        0        0   108893 2023-04-28 08:23:04.982656 pyaedt-0.6.73/pyaedt/edb_core/stackup.py
--rw-r--r--   0        0        0    11275 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/emit.py
--rw-r--r--   0        0        0     3555 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     3291 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/emit_core/EmitConstants.py
--rw-r--r--   0        0        0      791 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0        2 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7546 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    11682 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0    14317 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    11758 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.636162 pyaedt-0.6.73/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     3257 2023-04-28 11:15:19.829287 pyaedt-0.6.73/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    83387 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28645 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    19616 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0     3416 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    63135 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0    25808 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     6989 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0     9795 2023-04-28 11:15:19.829287 pyaedt-0.6.73/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    62296 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    11301 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/generic/process.py
--rw-r--r--   0        0        0    19736 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3466 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    60355 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/generic/toolkit.py
--rw-r--r--   0        0        0    17095 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0      438 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/generic/wpf_template.xaml
--rw-r--r--   0        0        0   252855 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/hfss.py
--rw-r--r--   0        0        0    82916 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   154882 2023-04-28 11:15:19.829287 pyaedt-0.6.73/pyaedt/icepak.py
--rw-r--r--   0        0        0   118433 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7803 2023-04-27 10:48:40.651785 pyaedt-0.6.73/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24259 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3035 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     3695 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     2380 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0       53 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    10210 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     3731 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     3829 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0      678 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-04-27 10:48:40.667417 pyaedt-0.6.73/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      953 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0      868 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14076 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    19994 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18513 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16809 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   120831 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0   194519 2023-04-28 11:15:19.844857 pyaedt-0.6.73/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   115253 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    11332 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   119788 2023-04-27 12:53:11.246332 pyaedt-0.6.73/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    29079 2023-04-27 10:48:40.683090 pyaedt-0.6.73/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49002 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59350 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53084 2023-04-28 11:15:19.844857 pyaedt-0.6.73/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12588 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    42270 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    32270 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8157 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    63043 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15094 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    31983 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    67799 2023-04-28 11:15:19.844857 pyaedt-0.6.73/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6897 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    52430 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    31270 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    49837 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    65608 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    21640 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    30094 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   113864 2023-04-27 10:48:40.698662 pyaedt-0.6.73/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71549 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    51910 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    40297 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0    82846 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    28306 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53168 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11919 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    26048 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   172808 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    64104 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   119128 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    33226 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    28652 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   103276 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   125048 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    95482 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/q3d.py
--rw-r--r--   0        0        0    10556 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.714291 pyaedt-0.6.73/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    40721 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9425 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7601 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    10373 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/siwave.py
--rw-r--r--   0        0        0    10527 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     4063 2023-04-27 10:48:40.729916 pyaedt-0.6.73/pyproject.toml
--rw-r--r--   0        0        0    15020 1970-01-01 00:00:00.000000 pyaedt-0.6.73/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-04-27 10:48:38.937375 pyaedt-0.6.74/LICENSE
+-rw-r--r--   0        0        0     9947 2023-05-04 17:35:03.992963 pyaedt-0.6.74/README.md
+-rw-r--r--   0        0        0     2634 2023-05-05 14:48:17.527685 pyaedt-0.6.74/pyaedt/__init__.py
+-rw-r--r--   0        0        0    26253 2023-04-27 10:48:40.495559 pyaedt-0.6.74/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6965 2023-04-27 10:48:40.495559 pyaedt-0.6.74/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    89212 2023-05-03 07:06:47.305842 pyaedt-0.6.74/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    41260 2023-05-04 22:05:14.854681 pyaedt-0.6.74/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    17009 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3088 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    19795 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4374 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4539 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   127521 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6115 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    75493 2023-04-27 13:08:15.716301 pyaedt-0.6.74/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12433 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    37014 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    57605 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10034 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    57391 2023-05-04 12:03:46.353459 pyaedt-0.6.74/pyaedt/desktop.py
+-rw-r--r--   0        0        0    15104 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/dlls/PDFReport/AnsysReport.deps.json
+-rw-r--r--   0        0        0    23552 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/dlls/PDFReport/AnsysReport.dll
+-rw-r--r--   0        0        0     1092 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/dlls/PDFReport/AnsysTemplate.json
+-rw-r--r--   0        0        0   204800 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
+-rw-r--r--   0        0        0   577445 2023-04-27 10:48:40.526826 pyaedt-0.6.74/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
+-rw-r--r--   0        0        0     9836 2023-04-27 10:48:40.526826 pyaedt-0.6.74/pyaedt/dlls/PDFReport/Images/Ansys.png
+-rw-r--r--   0        0        0   238592 2023-04-27 10:48:40.526826 pyaedt-0.6.74/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
+-rw-r--r--   0        0        0   115712 2023-04-27 10:48:40.526826 pyaedt-0.6.74/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
+-rw-r--r--   0        0        0   705296 2023-04-27 10:48:40.526826 pyaedt-0.6.74/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
+-rw-r--r--   0        0        0   712253 2023-04-27 10:48:40.542451 pyaedt-0.6.74/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
+-rw-r--r--   0        0        0    80384 2023-04-27 10:48:40.542451 pyaedt-0.6.74/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
+-rw-r--r--   0        0        0   546816 2023-04-27 10:48:40.542451 pyaedt-0.6.74/pyaedt/dlls/PDFReport/PdfSharpCore.dll
+-rw-r--r--   0        0        0   367616 2023-04-27 10:48:40.542451 pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
+-rw-r--r--   0        0        0   536367 2023-04-27 10:48:40.558076 pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
+-rw-r--r--   0        0        0  1229824 2023-04-27 10:48:40.558076 pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
+-rw-r--r--   0        0        0  3285773 2023-04-27 10:48:40.589270 pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
+-rw-r--r--   0        0        0   120664 2023-04-27 10:48:40.589270 pyaedt-0.6.74/pyaedt/dlls/PDFReport/System.Runtime.dll
+-rw-r--r--   0        0        0  1505294 2023-04-27 10:48:40.589270 pyaedt-0.6.74/pyaedt/dlls/PDFReport/System.Runtime.xml
+-rw-r--r--   0        0        0     5632 2023-04-27 10:48:40.589270 pyaedt-0.6.74/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
+-rw-r--r--   0        0        0   160754 2023-04-27 10:48:40.589270 pyaedt-0.6.74/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
+-rw-r--r--   0        0        0    23386 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/downloads.py
+-rw-r--r--   0        0        0   132412 2023-04-28 08:23:04.967029 pyaedt-0.6.74/pyaedt/edb.py
+-rw-r--r--   0        0        0      333 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/__init__.py
+-rw-r--r--   0        0        0    92729 2023-05-04 13:41:54.201025 pyaedt-0.6.74/pyaedt/edb_core/components.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    32856 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0      937 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0      324 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/edb_builder.py
+-rw-r--r--   0        0        0     1166 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    12141 2023-04-28 22:06:54.714447 pyaedt-0.6.74/pyaedt/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    65580 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    20305 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     4724 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    61111 2023-04-27 15:58:46.158994 pyaedt-0.6.74/pyaedt/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0    32298 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0    99826 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    36282 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    31276 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0     4147 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     2425 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     3258 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/general.py
+-rw-r--r--   0        0        0    60863 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/hfss.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0      673 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     1283 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     2213 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0      524 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0      768 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/color.py
+-rw-r--r--   0        0        0     2118 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/content.py
+-rw-r--r--   0        0        0      938 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0      921 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     1029 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0      416 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0      548 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0      523 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/fill.py
+-rw-r--r--   0        0        0      284 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     2844 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     1183 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     1319 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     1516 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0      960 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     1964 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     1158 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     7706 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0      921 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     1079 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     4646 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     1440 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0      875 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     2775 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0      887 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     4104 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     2567 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     1002 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8010 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0      663 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     1162 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     1626 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0      838 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    11333 2023-05-02 12:25:34.524335 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     1033 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0      683 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     2008 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     1624 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/history_record.py
+-rw-r--r--   0        0        0    21750 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0      966 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0    49064 2023-05-02 10:24:55.037694 pyaedt-0.6.74/pyaedt/edb_core/layout.py
+-rw-r--r--   0        0        0    33242 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/materials.py
+-rw-r--r--   0        0        0    43680 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/nets.py
+-rw-r--r--   0        0        0    46611 2023-05-02 13:33:56.688526 pyaedt-0.6.74/pyaedt/edb_core/padstack.py
+-rw-r--r--   0        0        0    57133 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/siwave.py
+-rw-r--r--   0        0        0   108893 2023-04-28 08:23:04.982656 pyaedt-0.6.74/pyaedt/edb_core/stackup.py
+-rw-r--r--   0        0        0    11275 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/emit.py
+-rw-r--r--   0        0        0     3555 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     3291 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/emit_core/EmitConstants.py
+-rw-r--r--   0        0        0     1074 2023-05-03 22:08:43.552442 pyaedt-0.6.74/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0        2 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7406 2023-05-03 22:08:43.552442 pyaedt-0.6.74/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    11154 2023-05-03 22:08:43.552442 pyaedt-0.6.74/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0    14317 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    11758 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     3257 2023-04-28 11:15:19.829287 pyaedt-0.6.74/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    83387 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28645 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    19616 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0     3416 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    67564 2023-05-05 10:19:45.526526 pyaedt-0.6.74/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0    25808 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     6989 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0     9795 2023-04-28 11:15:19.829287 pyaedt-0.6.74/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    62296 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    11301 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/process.py
+-rw-r--r--   0        0        0    19736 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3466 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    60355 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/toolkit.py
+-rw-r--r--   0        0        0    17095 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0      438 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/wpf_template.xaml
+-rw-r--r--   0        0        0   252855 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/hfss.py
+-rw-r--r--   0        0        0    82916 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   154940 2023-05-04 12:57:05.488766 pyaedt-0.6.74/pyaedt/icepak.py
+-rw-r--r--   0        0        0   118433 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7803 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24259 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3035 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     3695 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     2380 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0       53 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10210 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     3731 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     3829 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0      678 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      953 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0      868 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14076 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    19994 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16809 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   120831 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0   194513 2023-04-28 22:06:54.714447 pyaedt-0.6.74/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   115253 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    11332 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   127838 2023-05-05 12:50:06.063040 pyaedt-0.6.74/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    31549 2023-05-05 11:21:28.656568 pyaedt-0.6.74/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49002 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59516 2023-05-04 12:57:05.488766 pyaedt-0.6.74/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53100 2023-04-28 22:06:54.714447 pyaedt-0.6.74/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12588 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    42270 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    32270 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8157 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    63043 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15094 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    31983 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    68020 2023-04-28 22:06:54.714447 pyaedt-0.6.74/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6897 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    52430 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    31270 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    49837 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    65608 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    21640 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    30094 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   114236 2023-05-04 10:13:14.811305 pyaedt-0.6.74/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71549 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    51910 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40297 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0    82846 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    28306 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53168 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11919 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    26048 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   172808 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    64104 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   119621 2023-05-04 08:14:06.606295 pyaedt-0.6.74/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    33226 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    28652 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   103276 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   125048 2023-05-04 22:05:14.870254 pyaedt-0.6.74/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    95482 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10556 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    40721 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9425 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7601 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    10373 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/siwave.py
+-rw-r--r--   0        0        0    10527 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     4134 2023-05-05 10:19:45.542100 pyaedt-0.6.74/pyproject.toml
+-rw-r--r--   0        0        0    15129 1970-01-01 00:00:00.000000 pyaedt-0.6.74/PKG-INFO
```

### Comparing `pyaedt-0.6.73/LICENSE` & `pyaedt-0.6.74/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/README.rst` & `pyaedt-0.6.74/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,628 +1,622 @@
-00000000: 5079 4145 4454 0d0a 3d3d 3d3d 3d3d 0d0a  PyAEDT..======..
-00000010: 0d0a 7c70 7961 6e73 7973 7c20 7c70 7970  ..|pyansys| |pyp
-00000020: 697c 207c 5079 5049 6163 747c 207c 5079  i| |PyPIact| |Py
-00000030: 7468 6f6e 5665 7273 696f 6e7c 207c 4748  thonVersion| |GH
-00000040: 2d43 497c 207c 636f 6465 636f 767c 207c  -CI| |codecov| |
-00000050: 4d49 547c 207c 626c 6163 6b7c 207c 416e  MIT| |black| |An
-00000060: 6163 6f6e 6461 7c20 7c70 7265 2d63 6f6d  aconda| |pre-com
-00000070: 6d69 747c 0d0a 0d0a 2e2e 207c 7079 616e  mit|...... |pyan
-00000080: 7379 737c 2069 6d61 6765 3a3a 2068 7474  sys| image:: htt
-00000090: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000000a0: 2e69 6f2f 6261 6467 652f 5079 2d41 6e73  .io/badge/Py-Ans
-000000b0: 7973 2d66 6663 3130 372e 7376 673f 6c6f  ys-ffc107.svg?lo
-000000c0: 676f 3d64 6174 613a 696d 6167 652f 706e  go=data:image/pn
-000000d0: 673b 6261 7365 3634 2c69 5642 4f52 7730  g;base64,iVBORw0
-000000e0: 4b47 676f 4141 4141 4e53 5568 4555 6741  KGgoAAAANSUhEUgA
-000000f0: 4141 4241 4141 4141 5143 4149 4141 4143  AABAAAAAQCAIAAAC
-00000100: 516b 5767 3241 4141 4244 6b6c 4551 5651  QkWg2AAABDklEQVQ
-00000110: 346a 574e 676f 4466 6735 6d44 3876 4537  4jWNgoDfg5mD8vE7
-00000120: 712f 3362 7056 7973 6b62 5730 734d 5255  q/3bpVyskbW0sMRU
-00000130: 776f 6648 4437 4468 354f 426b 5a47 4267  wofHD7Dh5OBkZGBg
-00000140: 5737 2f33 5732 745a 7061 3274 4c51 454f  W7/3W2tZpa2tLQEO
-00000150: 794f 7a65 4573 6675 6d6c 4b32 7462 5670  yOzeEsfumlK2tbVp
-00000160: 6147 6a34 4e36 6a49 7331 6c70 7344 4177  aGj4N6jIs1lpsDAw
-00000170: 4d4a 3237 3873 7665 4d59 3242 6743 4130  MJ278sveMY2BgCA0
-00000180: 4e46 5249 5377 716b 6879 5131 712f 4e79  NFRISwqkhyQ1q/Ny
-00000190: 6433 7a67 344f 4267 5947 4e6a 5a32 6550  d3zg4OBgYGNjZ2eP
-000001a0: 6934 7242 356c 6f47 4268 5a6e 6878 544c  i4rB5loGBhZnhxTL
-000001b0: 4a2f 3975 6c76 3236 5134 7556 6b31 4e58  J/9ulv26Q4uVk1NX
-000001c0: 562f 662f 2f2f 2f2f 2f2f 3639 6475 345a  V/f///////69du4Z
-000001d0: 6467 3738 6c78 2f2f 7430 762b 3353 3838  dg78lx//t0v+3S88
-000001e0: 7246 4953 496e 4435 3947 7149 4832 6573  rFISInD59GqIH2es
-000001f0: 494a 3847 394f 322f 5856 7768 6a7a 7077  IJ8G9O2/XVwhjzpw
-00000200: 3545 4161 6d31 786b 6b42 4a6e 2f62 4a58  5EAam1xkkBJn/bJX
-00000210: 2b76 3133 3635 6878 7875 4341 6648 392b  +v1365hxxuCAfH9+
-00000220: 3362 392f 2b2f 2f2f 2f34 3863 5075 4e65  3b9/+////48cPuNe
-00000230: 684e 7353 3763 4445 7a4d 5441 774d 4d7a  hNsS7cDEzMTAwMMz
-00000240: 622b 5132 7534 644f 6e54 3276 5772 4d48  b+Q2u4dOnT2vWrMH
-00000250: 7539 5a74 7a78 5039 766c 2f36 3952 5670  u9ZtzxP9vl/69RVp
-00000260: 436b 426c 5a33 4e37 656e 6f44 5842 7745  CkBlZ3N7enoDXBwE
-00000270: 4141 412b 5959 6974 4f69 6c4d 5641 4141  AAA+YYitOilMVAAA
-00000280: 4141 456c 4654 6b53 7551 6d43 430d 0a20  AAElFTkSuQmCC.. 
-00000290: 2020 3a74 6172 6765 743a 2068 7474 7073    :target: https
-000002a0: 3a2f 2f64 6f63 732e 7079 616e 7379 732e  ://docs.pyansys.
-000002b0: 636f 6d2f 0d0a 2020 203a 616c 743a 2050  com/..   :alt: P
-000002c0: 7941 6e73 7973 0d0a 0d0a 2e2e 207c 7079  yAnsys...... |py
-000002d0: 7069 7c20 696d 6167 653a 3a20 6874 7470  pi| image:: http
-000002e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000002f0: 696f 2f70 7970 692f 762f 7079 6165 6474  io/pypi/v/pyaedt
-00000300: 2e73 7667 3f6c 6f67 6f3d 7079 7468 6f6e  .svg?logo=python
-00000310: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
-00000320: 0d0a 2020 203a 7461 7267 6574 3a20 6874  ..   :target: ht
-00000330: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000340: 726f 6a65 6374 2f70 7961 6564 742f 0d0a  roject/pyaedt/..
-00000350: 0d0a 2e2e 207c 5079 5049 6163 747c 2020  .... |PyPIact|  
-00000360: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
-00000370: 7065 7079 2e74 6563 682f 6261 6467 652f  pepy.tech/badge/
-00000380: 7079 6165 6474 2f6d 6f6e 7468 0d0a 2020  pyaedt/month..  
-00000390: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
-000003a0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-000003b0: 6374 2f70 7961 6564 742f 0d0a 0d0a 2e2e  ct/pyaedt/......
-000003c0: 207c 5079 7468 6f6e 5665 7273 696f 6e7c   |PythonVersion|
-000003d0: 2069 6d61 6765 3a3a 2068 7474 7073 3a2f   image:: https:/
-000003e0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000003f0: 6261 6467 652f 7079 7468 6f6e 2d33 2e37  badge/python-3.7
-00000400: 2b2d 626c 7565 2e73 7667 0d0a 2020 203a  +-blue.svg..   :
-00000410: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
-00000420: 7777 772e 7079 7468 6f6e 2e6f 7267 2f64  www.python.org/d
-00000430: 6f77 6e6c 6f61 6473 2f0d 0a0d 0a2e 2e20  ownloads/...... 
-00000440: 7c47 482d 4349 7c20 696d 6167 653a 3a20  |GH-CI| image:: 
-00000450: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000460: 6f6d 2f70 7961 6e73 7973 2f70 7961 6564  om/pyansys/pyaed
-00000470: 742f 6163 7469 6f6e 732f 776f 726b 666c  t/actions/workfl
-00000480: 6f77 732f 756e 6974 5f74 6573 7473 2e79  ows/unit_tests.y
-00000490: 6d6c 2f62 6164 6765 2e73 7667 0d0a 2020  ml/badge.svg..  
-000004a0: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
-000004b0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7961  //github.com/pya
-000004c0: 6e73 7973 2f70 7961 6564 742f 6163 7469  nsys/pyaedt/acti
-000004d0: 6f6e 732f 776f 726b 666c 6f77 732f 756e  ons/workflows/un
-000004e0: 6974 5f74 6573 7473 2e79 6d6c 0d0a 0d0a  it_tests.yml....
-000004f0: 2e2e 207c 636f 6465 636f 767c 2069 6d61  .. |codecov| ima
-00000500: 6765 3a3a 2068 7474 7073 3a2f 2f63 6f64  ge:: https://cod
-00000510: 6563 6f76 2e69 6f2f 6768 2f70 7961 6e73  ecov.io/gh/pyans
-00000520: 7973 2f70 7961 6564 742f 6272 616e 6368  ys/pyaedt/branch
-00000530: 2f6d 6169 6e2f 6772 6170 682f 6261 6467  /main/graph/badg
-00000540: 652e 7376 670d 0a20 2020 3a74 6172 6765  e.svg..   :targe
-00000550: 743a 2068 7474 7073 3a2f 2f63 6f64 6563  t: https://codec
-00000560: 6f76 2e69 6f2f 6768 2f70 7961 6e73 7973  ov.io/gh/pyansys
-00000570: 2f70 7961 6564 740d 0a0d 0a2e 2e20 7c4d  /pyaedt...... |M
-00000580: 4954 7c20 696d 6167 653a 3a20 6874 7470  IT| image:: http
-00000590: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000005a0: 696f 2f62 6164 6765 2f4c 6963 656e 7365  io/badge/License
-000005b0: 2d4d 4954 2d79 656c 6c6f 772e 7376 670d  -MIT-yellow.svg.
-000005c0: 0a20 2020 3a74 6172 6765 743a 2068 7474  .   :target: htt
-000005d0: 7073 3a2f 2f6f 7065 6e73 6f75 7263 652e  ps://opensource.
-000005e0: 6f72 672f 6c69 6365 6e73 6573 2f4d 4954  org/licenses/MIT
-000005f0: 0d0a 0d0a 2e2e 207c 626c 6163 6b7c 2069  ...... |black| i
-00000600: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f69  mage:: https://i
-00000610: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000620: 6467 652f 636f 6465 2532 3073 7479 6c65  dge/code%20style
-00000630: 2d62 6c61 636b 2d30 3030 3030 302e 7376  -black-000000.sv
-00000640: 673f 7374 796c 653d 666c 6174 0d0a 2020  g?style=flat..  
-00000650: 3a74 6172 6765 743a 2068 7474 7073 3a2f  :target: https:/
-00000660: 2f67 6974 6875 622e 636f 6d2f 7073 662f  /github.com/psf/
-00000670: 626c 6163 6b0d 0a20 203a 616c 743a 2062  black..  :alt: b
-00000680: 6c61 636b 0d0a 0d0a 2e2e 207c 416e 6163  lack...... |Anac
-00000690: 6f6e 6461 7c20 696d 6167 653a 3a20 6874  onda| image:: ht
-000006a0: 7470 733a 2f2f 616e 6163 6f6e 6461 2e6f  tps://anaconda.o
-000006b0: 7267 2f63 6f6e 6461 2d66 6f72 6765 2f70  rg/conda-forge/p
-000006c0: 7961 6564 742f 6261 6467 6573 2f76 6572  yaedt/badges/ver
-000006d0: 7369 6f6e 2e73 7667 0d0a 2020 3a74 6172  sion.svg..  :tar
-000006e0: 6765 743a 2068 7474 7073 3a2f 2f61 6e61  get: https://ana
-000006f0: 636f 6e64 612e 6f72 672f 636f 6e64 612d  conda.org/conda-
-00000700: 666f 7267 652f 7079 6165 6474 0d0a 0d0a  forge/pyaedt....
-00000710: 2e2e 207c 7072 652d 636f 6d6d 6974 7c20  .. |pre-commit| 
-00000720: 696d 6167 653a 3a20 6874 7470 733a 2f2f  image:: https://
-00000730: 7265 7375 6c74 732e 7072 652d 636f 6d6d  results.pre-comm
-00000740: 6974 2e63 692f 6261 6467 652f 6769 7468  it.ci/badge/gith
-00000750: 7562 2f70 7961 6e73 7973 2f70 7961 6564  ub/pyansys/pyaed
-00000760: 742f 6d61 696e 2e73 7667 0d0a 2020 203a  t/main.svg..   :
-00000770: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
-00000780: 7265 7375 6c74 732e 7072 652d 636f 6d6d  results.pre-comm
-00000790: 6974 2e63 692f 6c61 7465 7374 2f67 6974  it.ci/latest/git
-000007a0: 6875 622f 7079 616e 7379 732f 7079 6165  hub/pyansys/pyae
-000007b0: 6474 2f6d 6169 6e0d 0a20 2020 3a61 6c74  dt/main..   :alt
-000007c0: 3a20 7072 652d 636f 6d6d 6974 2e63 6920  : pre-commit.ci 
-000007d0: 7374 6174 7573 0d0a 0d0a 0d0a 5768 6174  status......What
-000007e0: 2069 7320 5079 4145 4454 3f0d 0a2d 2d2d   is PyAEDT?..---
-000007f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 5079  ------------..Py
-00000800: 4145 4454 2069 7320 6120 5079 7468 6f6e  AEDT is a Python
-00000810: 206c 6962 7261 7279 2074 6861 7420 696e   library that in
-00000820: 7465 7261 6374 7320 6469 7265 6374 6c79  teracts directly
-00000830: 2077 6974 6820 7468 6520 4150 4920 666f   with the API fo
-00000840: 720d 0a41 6e73 7973 2045 6c65 6374 726f  r..Ansys Electro
-00000850: 6e69 6373 2044 6573 6b74 6f70 2028 4145  nics Desktop (AE
-00000860: 4454 2920 746f 206d 616b 6520 7363 7269  DT) to make scri
-00000870: 7074 696e 6720 7369 6d70 6c65 722e 2054  pting simpler. T
-00000880: 6865 2061 7263 6869 7465 6374 7572 650d  he architecture.
-00000890: 0a66 6f72 2050 7941 4544 5420 6361 6e20  .for PyAEDT can 
-000008a0: 6265 2072 6575 7365 6420 666f 7220 616c  be reused for al
-000008b0: 6c20 4145 4454 2033 4420 7072 6f64 7563  l AEDT 3D produc
-000008c0: 7473 2028 4846 5353 2c20 4963 6570 616b  ts (HFSS, Icepak
-000008d0: 2c20 4d61 7877 656c 6c20 3344 2c0d 0a61  , Maxwell 3D,..a
-000008e0: 6e64 2051 3344 2045 7874 7261 6374 6f72  nd Q3D Extractor
-000008f0: 292c 2032 4420 746f 6f6c 732c 2061 6e64  ), 2D tools, and
-00000900: 2041 6e73 7973 204d 6563 6861 6e69 6361   Ansys Mechanica
-00000910: 6c2e 2050 7941 4544 5420 616c 736f 2070  l. PyAEDT also p
-00000920: 726f 7669 6465 730d 0a73 7570 706f 7274  rovides..support
-00000930: 2066 6f72 2063 6972 6375 6974 2074 6f6f   for circuit too
-00000940: 6c73 206c 696b 6520 4e65 7878 696d 2061  ls like Nexxim a
-00000950: 6e64 2073 7973 7465 6d20 7369 6d75 6c61  nd system simula
-00000960: 7469 6f6e 2074 6f6f 6c73 206c 696b 650d  tion tools like.
-00000970: 0a54 7769 6e20 4275 696c 6465 722e 2046  .Twin Builder. F
-00000980: 696e 616c 6c79 2c20 5079 4145 4454 2070  inally, PyAEDT p
-00000990: 726f 7669 6465 7320 7363 7269 7074 696e  rovides scriptin
-000009a0: 6720 6361 7061 6269 6c69 7469 6573 2069  g capabilities i
-000009b0: 6e20 416e 7379 7320 6c61 796f 7574 0d0a  n Ansys layout..
-000009c0: 746f 6f6c 7320 6c69 6b65 2048 4653 5320  tools like HFSS 
-000009d0: 3344 204c 6179 6f75 7420 616e 6420 4544  3D Layout and ED
-000009e0: 422e 2054 6865 2050 7941 4544 5420 636c  B. The PyAEDT cl
-000009f0: 6173 7320 616e 6420 6d65 7468 6f64 2073  ass and method s
-00000a00: 7472 7563 7475 7265 730d 0a73 696d 706c  tructures..simpl
-00000a10: 6966 7920 6f70 6572 6174 696f 6e20 7768  ify operation wh
-00000a20: 696c 6520 7265 7573 696e 6720 696e 666f  ile reusing info
-00000a30: 726d 6174 696f 6e20 6173 206d 7563 6820  rmation as much 
-00000a40: 6173 2070 6f73 7369 626c 6520 6163 726f  as possible acro
-00000a50: 7373 0d0a 7468 6520 4150 492e 0d0a 0d0a  ss..the API.....
-00000a60: 496e 7374 616c 6c20 6f6e 2043 5079 7468  Install on CPyth
-00000a70: 6f6e 2066 726f 6d20 5079 5049 0d0a 2d2d  on from PyPI..--
-00000a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000a90: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 596f 7520  ----------..You 
-00000aa0: 6361 6e20 696e 7374 616c 6c20 5079 4145  can install PyAE
-00000ab0: 4454 206f 6e20 4350 7974 686f 6e20 332e  DT on CPython 3.
-00000ac0: 3720 7468 726f 7567 6820 332e 3130 2066  7 through 3.10 f
-00000ad0: 726f 6d20 5079 5049 2077 6974 6820 7468  rom PyPI with th
-00000ae0: 6973 2063 6f6d 6d61 6e64 3a0d 0a0d 0a2e  is command:.....
-00000af0: 2e20 636f 6465 3a3a 2070 7974 686f 6e0d  . code:: python.
-00000b00: 0a0d 0a20 2020 2070 6970 2069 6e73 7461  ...    pip insta
-00000b10: 6c6c 2070 7961 6564 740d 0a0d 0a54 6f20  ll pyaedt....To 
-00000b20: 696e 7374 616c 6c20 5079 4145 4454 2077  install PyAEDT w
-00000b30: 6974 6820 616c 6c20 6578 7472 6120 7061  ith all extra pa
-00000b40: 636b 6167 6573 2028 4d61 7470 6c6f 746c  ckages (Matplotl
-00000b50: 6962 2c20 4e75 6d50 792c 2050 616e 6461  ib, NumPy, Panda
-00000b60: 732c 2061 6e64 2050 7956 6973 7461 292c  s, and PyVista),
-00000b70: 0d0a 7573 6520 7468 6973 2063 6f6d 6d61  ..use this comma
-00000b80: 6e64 3a0d 0a0d 0a2e 2e20 636f 6465 3a3a  nd:...... code::
-00000b90: 2070 7974 686f 6e0d 0a0d 0a20 2020 2070   python....    p
-00000ba0: 6970 2069 6e73 7461 6c6c 2070 7961 6564  ip install pyaed
-00000bb0: 745b 6675 6c6c 5d0d 0a0d 0a59 6f75 2063  t[full]....You c
-00000bc0: 616e 2061 6c73 6f20 696e 7374 616c 6c20  an also install 
-00000bd0: 5079 4145 4454 2066 726f 6d20 436f 6e64  PyAEDT from Cond
-00000be0: 612d 466f 7267 6520 7769 7468 2074 6869  a-Forge with thi
-00000bf0: 7320 636f 6d6d 616e 643a 0d0a 0d0a 2e2e  s command:......
-00000c00: 2063 6f64 653a 3a20 7079 7468 6f6e 0d0a   code:: python..
-00000c10: 0d0a 2020 2020 636f 6e64 6120 696e 7374  ..    conda inst
-00000c20: 616c 6c20 2d63 2063 6f6e 6461 2d66 6f72  all -c conda-for
-00000c30: 6765 2070 7961 6564 740d 0a0d 0a50 7941  ge pyaedt....PyA
-00000c40: 4544 5420 7265 6d61 696e 7320 636f 6d70  EDT remains comp
-00000c50: 6174 6962 6c65 2077 6974 6820 4972 6f6e  atible with Iron
-00000c60: 5079 7468 6f6e 2061 6e64 2063 616e 2062  Python and can b
-00000c70: 6520 7374 696c 6c20 7573 6564 2069 6e20  e still used in 
-00000c80: 7468 6520 4145 4454 2046 7261 6d65 776f  the AEDT Framewo
-00000c90: 726b 2e0d 0a0d 0a41 626f 7574 2050 7941  rk.....About PyA
-00000ca0: 6e73 7973 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d  nsys..----------
-00000cb0: 2d2d 2d0d 0a0d 0a50 7941 4544 5420 6973  ---....PyAEDT is
-00000cc0: 2070 6172 7420 6f66 2074 6865 206c 6172   part of the lar
-00000cd0: 6765 7220 6050 7941 6e73 7973 203c 6874  ger `PyAnsys <ht
-00000ce0: 7470 733a 2f2f 646f 6373 2e70 7961 6e73  tps://docs.pyans
-00000cf0: 7973 2e63 6f6d 3e60 5f0d 0a65 6666 6f72  ys.com>`_..effor
-00000d00: 7420 746f 2066 6163 696c 6974 6174 6520  t to facilitate 
-00000d10: 7468 6520 7573 6520 6f66 2041 6e73 7973  the use of Ansys
-00000d20: 2074 6563 686e 6f6c 6f67 6965 7320 6469   technologies di
-00000d30: 7265 6374 6c79 2066 726f 6d20 5079 7468  rectly from Pyth
-00000d40: 6f6e 2e0d 0a0d 0a50 7941 4544 5420 6973  on.....PyAEDT is
-00000d50: 2069 6e74 656e 6465 6420 746f 2063 6f6e   intended to con
-00000d60: 736f 6c69 6461 7465 2061 6e64 2065 7874  solidate and ext
-00000d70: 656e 6420 616c 6c20 6578 6973 7469 6e67  end all existing
-00000d80: 0d0a 6675 6e63 7469 6f6e 616c 6974 6965  ..functionalitie
-00000d90: 7320 6172 6f75 6e64 2073 6372 6970 7469  s around scripti
-00000da0: 6e67 2066 6f72 2041 4544 5420 746f 2061  ng for AEDT to a
-00000db0: 6c6c 6f77 2072 6575 7365 206f 6620 6578  llow reuse of ex
-00000dc0: 6973 7469 6e67 2063 6f64 652c 0d0a 7368  isting code,..sh
-00000dd0: 6172 696e 6720 6f66 2062 6573 7420 7072  aring of best pr
-00000de0: 6163 7469 6365 732c 2061 6e64 2069 6e63  actices, and inc
-00000df0: 7265 6173 6564 2063 6f6c 6c61 626f 7261  reased collabora
-00000e00: 7469 6f6e 2e0d 0a0d 0a0d 0a41 626f 7574  tion.......About
-00000e10: 2041 4544 540d 0a2d 2d2d 2d2d 2d2d 2d2d   AEDT..---------
-00000e20: 2d0d 0a0d 0a60 4145 4454 203c 6874 7470  -....`AEDT <http
-00000e30: 733a 2f2f 7777 772e 616e 7379 732e 636f  s://www.ansys.co
-00000e40: 6d2f 7072 6f64 7563 7473 2f65 6c65 6374  m/products/elect
-00000e50: 726f 6e69 6373 3e60 5f20 6973 2061 2070  ronics>`_ is a p
-00000e60: 6c61 7466 6f72 6d20 7468 6174 2065 6e61  latform that ena
-00000e70: 626c 6573 2074 7275 650d 0a65 6c65 6374  bles true..elect
-00000e80: 726f 6e69 6373 2073 7973 7465 6d20 6465  ronics system de
-00000e90: 7369 676e 2e20 4145 4454 2070 726f 7669  sign. AEDT provi
-00000ea0: 6465 7320 6163 6365 7373 2074 6f20 7468  des access to th
-00000eb0: 6520 416e 7379 7320 676f 6c64 2d73 7461  e Ansys gold-sta
-00000ec0: 6e64 6172 640d 0a65 6c65 6374 726f 2d6d  ndard..electro-m
-00000ed0: 6167 6e65 7469 6373 2073 696d 756c 6174  agnetics simulat
-00000ee0: 696f 6e20 736f 6c75 7469 6f6e 732c 2073  ion solutions, s
-00000ef0: 7563 6820 6173 2041 6e73 7973 2048 4653  uch as Ansys HFS
-00000f00: 532c 2041 6e73 7973 204d 6178 7765 6c6c  S, Ansys Maxwell
-00000f10: 2c0d 0a41 6e73 7973 2051 3344 2045 7874  ,..Ansys Q3D Ext
-00000f20: 7261 6374 6f72 2c20 416e 7379 7320 5369  ractor, Ansys Si
-00000f30: 7761 7665 2c20 616e 6420 416e 7379 7320  wave, and Ansys 
-00000f40: 4963 6570 616b 2075 7369 6e67 2065 6c65  Icepak using ele
-00000f50: 6374 7269 6361 6c20 4341 4420 2845 4341  ctrical CAD (ECA
-00000f60: 4429 2061 6e64 0d0a 4d65 6368 616e 6963  D) and..Mechanic
-00000f70: 616c 2043 4144 2028 4d43 4144 2920 776f  al CAD (MCAD) wo
-00000f80: 726b 666c 6f77 732e 0d0a 0d0a 496e 2061  rkflows.....In a
-00000f90: 6464 6974 696f 6e2c 2041 4544 5420 696e  ddition, AEDT in
-00000fa0: 636c 7564 6573 2064 6972 6563 7420 6c69  cludes direct li
-00000fb0: 6e6b 7320 746f 2074 6865 2063 6f6d 706c  nks to the compl
-00000fc0: 6574 6520 416e 7379 7320 706f 7274 666f  ete Ansys portfo
-00000fd0: 6c69 6f20 6f66 2074 6865 726d 616c 2c20  lio of thermal, 
-00000fe0: 666c 7569 642c 0d0a 616e 6420 6d65 6368  fluid,..and mech
-00000ff0: 616e 6963 616c 2073 6f6c 7665 7273 2066  anical solvers f
-00001000: 6f72 2063 6f6d 7072 6568 656e 7369 7665  or comprehensive
-00001010: 206d 756c 7469 7068 7973 6963 7320 616e   multiphysics an
-00001020: 616c 7973 6973 2e0d 0a54 6967 6874 2069  alysis...Tight i
-00001030: 6e74 6567 7261 7469 6f6e 2061 6d6f 6e67  ntegration among
-00001040: 2074 6865 7365 2073 6f6c 7574 696f 6e73   these solutions
-00001050: 2070 726f 7669 6465 7320 756e 7072 6563   provides unprec
-00001060: 6564 656e 7465 6420 6561 7365 206f 6620  edented ease of 
-00001070: 7573 6520 666f 7220 7365 7475 7020 616e  use for setup an
-00001080: 640d 0a66 6173 7465 7220 7265 736f 6c75  d..faster resolu
-00001090: 7469 6f6e 206f 6620 636f 6d70 6c65 7820  tion of complex 
-000010a0: 7369 6d75 6c61 7469 6f6e 7320 666f 7220  simulations for 
-000010b0: 6465 7369 676e 2061 6e64 206f 7074 696d  design and optim
-000010c0: 697a 6174 696f 6e2e 0d0a 0d0a 2e2e 2069  ization....... i
-000010d0: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f69  mage:: https://i
-000010e0: 6d61 6765 732e 616e 7379 732e 636f 6d2f  mages.ansys.com/
-000010f0: 6973 2f69 6d61 6765 2f61 6e73 7973 2f61  is/image/ansys/a
-00001100: 6e73 7973 2d65 6c65 6374 726f 6e69 6373  nsys-electronics
-00001110: 2d74 6563 686e 6f6c 6f67 792d 636f 6c6c  -technology-coll
-00001120: 6167 653f 7769 643d 3934 3126 6f70 5f75  age?wid=941&op_u
-00001130: 736d 3d30 2e39 2c31 2e30 2c32 302c 3026  sm=0.9,1.0,20,0&
-00001140: 6669 743d 636f 6e73 7472 6169 6e2c 300d  fit=constrain,0.
-00001150: 0a20 203a 7769 6474 683a 2038 3030 0d0a  .  :width: 800..
-00001160: 2020 3a61 6c74 3a20 4145 4454 2041 7070    :alt: AEDT App
-00001170: 6c69 6361 7469 6f6e 730d 0a20 203a 7461  lications..  :ta
-00001180: 7267 6574 3a20 6874 7470 733a 2f2f 7777  rget: https://ww
-00001190: 772e 616e 7379 732e 636f 6d2f 7072 6f64  w.ansys.com/prod
-000011a0: 7563 7473 2f65 6c65 6374 726f 6e69 6373  ucts/electronics
-000011b0: 0d0a 0d0a 0d0a 5079 4145 4454 2069 7320  ......PyAEDT is 
-000011c0: 6c69 6365 6e73 6564 2075 6e64 6572 2074  licensed under t
-000011d0: 6865 2060 4d49 5420 4c69 6365 6e73 650d  he `MIT License.
-000011e0: 0a3c 6874 7470 733a 2f2f 6769 7468 7562  .<https://github
-000011f0: 2e63 6f6d 2f70 7961 6e73 7973 2f50 7941  .com/pyansys/PyA
-00001200: 4544 542f 626c 6f62 2f6d 6169 6e2f 4c49  EDT/blob/main/LI
-00001210: 4345 4e53 453e 605f 2e0d 0a0d 0a50 7941  CENSE>`_.....PyA
-00001220: 4544 5420 696e 636c 7564 6573 2066 756e  EDT includes fun
-00001230: 6374 696f 6e61 6c69 7479 2066 6f72 2069  ctionality for i
-00001240: 6e74 6572 6163 7469 6e67 2077 6974 6820  nteracting with 
-00001250: 7468 6520 666f 6c6c 6f77 696e 6720 4145  the following AE
-00001260: 4454 2074 6f6f 6c73 2061 6e64 2041 6e73  DT tools and Ans
-00001270: 7973 2070 726f 6475 6374 733a 0d0a 0d0a  ys products:....
-00001280: 2d20 4846 5353 2061 6e64 2048 4653 5320  - HFSS and HFSS 
-00001290: 3344 204c 6179 6f75 740d 0a2d 2049 6365  3D Layout..- Ice
-000012a0: 7061 6b0d 0a2d 204d 6178 7765 6c6c 2032  pak..- Maxwell 2
-000012b0: 442c 204d 6178 7765 6c6c 2033 442c 2061  D, Maxwell 3D, a
-000012c0: 6e64 2052 4d58 7072 740d 0a2d 2032 4420  nd RMXprt..- 2D 
-000012d0: 4578 7472 6163 746f 7220 616e 6420 5133  Extractor and Q3
-000012e0: 4420 4578 7472 6163 746f 720d 0a2d 204d  D Extractor..- M
-000012f0: 6563 6861 6e69 6361 6c0d 0a2d 204e 6578  echanical..- Nex
-00001300: 7869 6d0d 0a2d 2045 4442 0d0a 2d20 5477  xim..- EDB..- Tw
-00001310: 696e 2042 7569 6c64 6572 0d0a 0d0a 0d0a  in Builder......
-00001320: 446f 6375 6d65 6e74 6174 696f 6e20 616e  Documentation an
-00001330: 6420 6973 7375 6573 0d0a 2d2d 2d2d 2d2d  d issues..------
-00001340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001350: 2d2d 0d0a 446f 6375 6d65 6e74 6174 696f  --..Documentatio
-00001360: 6e20 666f 7220 7468 6520 6c61 7465 7374  n for the latest
-00001370: 2073 7461 626c 6520 7265 6c65 6173 6520   stable release 
-00001380: 6f66 2050 7941 4544 5420 6973 2068 6f73  of PyAEDT is hos
-00001390: 7465 6420 6174 0d0a 6050 7941 4544 5420  ted at..`PyAEDT 
-000013a0: 446f 6375 6d65 6e74 6174 696f 6e20 3c68  Documentation <h
-000013b0: 7474 7073 3a2f 2f61 6564 742e 646f 6373  ttps://aedt.docs
-000013c0: 2e70 7961 6e73 7973 2e63 6f6d 2f76 6572  .pyansys.com/ver
-000013d0: 7369 6f6e 2f73 7461 626c 652f 3e60 5f2e  sion/stable/>`_.
-000013e0: 0d0a 0d0a 496e 2074 6865 2075 7070 6572  ....In the upper
-000013f0: 2072 6967 6874 2063 6f72 6e65 7220 6f66   right corner of
-00001400: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
-00001410: 6f6e 2773 2074 6974 6c65 2062 6172 2c20  on's title bar, 
-00001420: 7468 6572 6520 6973 2061 6e20 6f70 7469  there is an opti
-00001430: 6f6e 0d0a 666f 7220 7377 6974 6368 696e  on..for switchin
-00001440: 6720 6672 6f6d 2076 6965 7769 6e67 2074  g from viewing t
-00001450: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
-00001460: 2066 6f72 2074 6865 206c 6174 6573 7420   for the latest 
-00001470: 7374 6162 6c65 2072 656c 6561 7365 0d0a  stable release..
-00001480: 746f 2076 6965 7769 6e67 2074 6865 2064  to viewing the d
-00001490: 6f63 756d 656e 7461 7469 6f6e 2066 6f72  ocumentation for
-000014a0: 2074 6865 2064 6576 656c 6f70 6d65 6e74   the development
-000014b0: 2076 6572 7369 6f6e 206f 7220 7072 6576   version or prev
-000014c0: 696f 7573 6c79 0d0a 7265 6c65 6173 6564  iously..released
-000014d0: 2076 6572 7369 6f6e 732e 0d0a 0d0a 4f6e   versions.....On
-000014e0: 2074 6865 2060 5079 4145 4454 2049 7373   the `PyAEDT Iss
-000014f0: 7565 7320 3c68 7474 7073 3a2f 2f67 6974  ues <https://git
-00001500: 6875 622e 636f 6d2f 7079 616e 7379 732f  hub.com/pyansys/
-00001510: 5079 4145 4454 2f69 7373 7565 733e 605f  PyAEDT/issues>`_
-00001520: 2070 6167 652c 2079 6f75 2063 616e 0d0a   page, you can..
-00001530: 6372 6561 7465 2069 7373 7565 7320 746f  create issues to
-00001540: 2073 7562 6d69 7420 7175 6573 7469 6f6e   submit question
-00001550: 732c 2072 6570 6f72 7420 6275 6773 2c20  s, report bugs, 
-00001560: 616e 6420 7265 7175 6573 7420 6e65 7720  and request new 
-00001570: 6665 6174 7572 6573 2e0d 0a0d 0a54 6f20  features.....To 
-00001580: 7265 6163 6820 7468 6520 7072 6f6a 6563  reach the projec
-00001590: 7420 7375 7070 6f72 7420 7465 616d 2c20  t support team, 
-000015a0: 656d 6169 6c20 6070 7961 6e73 7973 2e63  email `pyansys.c
-000015b0: 6f72 6540 616e 7379 732e 636f 6d20 3c70  ore@ansys.com <p
-000015c0: 7961 6e73 7973 2e63 6f72 6540 616e 7379  yansys.core@ansy
-000015d0: 732e 636f 6d3e 605f 2e0d 0a0d 0a44 6570  s.com>`_.....Dep
-000015e0: 656e 6465 6e63 6965 730d 0a2d 2d2d 2d2d  endencies..-----
-000015f0: 2d2d 2d2d 2d2d 2d0d 0a54 6f20 7275 6e20  -------..To run 
-00001600: 5079 4145 4454 2c20 796f 7520 6d75 7374  PyAEDT, you must
-00001610: 2068 6176 6520 6120 6c6f 6361 6c20 6c69   have a local li
-00001620: 6365 6e73 6564 2063 6f70 7920 6f66 2041  censed copy of A
-00001630: 4544 542e 0d0a 5079 4145 4454 2073 7570  EDT...PyAEDT sup
-00001640: 706f 7274 7320 4145 4454 2076 6572 7369  ports AEDT versi
-00001650: 6f6e 7320 3230 3232 2052 3120 616e 6420  ons 2022 R1 and 
-00001660: 6c61 7465 722e 0d0a 0d0a 5374 7564 656e  later.....Studen
-00001670: 7420 7665 7273 696f 6e0d 0a2d 2d2d 2d2d  t version..-----
-00001680: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a 5079  ----------....Py
-00001690: 4145 4454 2073 7570 706f 7274 7320 4145  AEDT supports AE
-000016a0: 4454 2053 7475 6465 6e74 2076 6572 7369  DT Student versi
-000016b0: 6f6e 7320 3230 3232 2052 3120 616e 6420  ons 2022 R1 and 
-000016c0: 6c61 7465 722e 2046 6f72 206d 6f72 6520  later. For more 
-000016d0: 696e 666f 726d 6174 696f 6e2c 2073 6565  information, see
-000016e0: 0d0a 6041 6e73 7973 2045 6c65 6374 726f  ..`Ansys Electro
-000016f0: 6e69 6373 2044 6573 6b74 6f70 2053 7475  nics Desktop Stu
-00001700: 6465 6e74 2020 2d20 4672 6565 2053 6f66  dent  - Free Sof
-00001710: 7477 6172 6520 446f 776e 6c6f 6164 203c  tware Download <
-00001720: 6874 7470 733a 2f2f 7777 772e 616e 7379  https://www.ansy
-00001730: 732e 636f 6d2f 6163 6164 656d 6963 2f73  s.com/academic/s
-00001740: 7475 6465 6e74 732f 616e 7379 732d 650d  tudents/ansys-e.
-00001750: 0a6c 6563 7472 6f6e 6963 732d 6465 736b  .lectronics-desk
-00001760: 746f 702d 7374 7564 656e 743e 605f 206f  top-student>`_ o
-00001770: 6e20 7468 6520 416e 7379 7320 7765 6273  n the Ansys webs
-00001780: 6974 652e 0d0a 0d0a 0d0a 5768 7920 5079  ite.......Why Py
-00001790: 4145 4454 3f0d 0a2d 2d2d 2d2d 2d2d 2d2d  AEDT?..---------
-000017a0: 2d2d 0d0a 4120 7175 6963 6b20 616e 6420  --..A quick and 
-000017b0: 6561 7379 2061 7070 726f 6163 6820 666f  easy approach fo
-000017c0: 7220 6175 746f 6d61 7469 6e67 2061 2073  r automating a s
-000017d0: 696d 706c 6520 6f70 6572 6174 696f 6e20  imple operation 
-000017e0: 696e 2074 6865 200d 0a41 4544 5420 5549  in the ..AEDT UI
-000017f0: 2069 7320 746f 2072 6563 6f72 6420 616e   is to record an
-00001800: 6420 7265 7573 6520 6120 7363 7269 7074  d reuse a script
-00001810: 2e20 486f 7765 7665 722c 2068 6572 6520  . However, here 
-00001820: 6172 6520 736f 6d65 2064 6973 6164 7661  are some disadva
-00001830: 6e74 6167 6573 206f 6620 0d0a 7468 6973  ntages of ..this
-00001840: 2061 7070 726f 6163 683a 0d0a 0d0a 2d20   approach:....- 
-00001850: 5265 636f 7264 6564 2063 6f64 6520 6973  Recorded code is
-00001860: 2064 6972 7479 2061 6e64 2064 6966 6669   dirty and diffi
-00001870: 6375 6c74 2074 6f20 7265 6164 2061 6e64  cult to read and
-00001880: 2075 6e64 6572 7374 616e 642e 0d0a 2d20   understand...- 
-00001890: 5265 636f 7264 6564 2073 6372 6970 7473  Recorded scripts
-000018a0: 2061 7265 2064 6966 6669 6375 6c74 2074   are difficult t
-000018b0: 6f20 7265 7573 6520 616e 6420 6164 6170  o reuse and adap
-000018c0: 742e 0d0a 2d20 436f 6d70 6c65 7820 636f  t...- Complex co
-000018d0: 6469 6e67 2069 7320 7265 7175 6972 6564  ding is required
-000018e0: 2062 7920 6d61 6e79 2067 6c6f 6261 6c20   by many global 
-000018f0: 7573 6572 7320 6f66 2041 4544 542e 0d0a  users of AEDT...
-00001900: 0d0a 4865 7265 2061 7265 2074 6865 206d  ..Here are the m
-00001910: 6169 6e20 6164 7661 6e74 6167 6573 2074  ain advantages t
-00001920: 6861 7420 5079 4145 4454 2070 726f 7669  hat PyAEDT provi
-00001930: 6465 733a 0d0a 0d0a 2d20 4175 746f 6d61  des:....- Automa
-00001940: 7469 6320 696e 6974 6961 6c69 7a61 7469  tic initializati
-00001950: 6f6e 206f 6620 616c 6c20 4145 4454 206f  on of all AEDT o
-00001960: 626a 6563 7473 2c20 7375 6368 2061 7320  bjects, such as 
-00001970: 6465 736b 746f 700d 0a20 206f 626a 6563  desktop..  objec
-00001980: 7473 206c 696b 6520 7468 6520 6564 6974  ts like the edit
-00001990: 6f72 2c20 626f 756e 6461 7269 6573 2c20  or, boundaries, 
-000019a0: 616e 6420 6d6f 7265 0d0a 2d20 4572 726f  and more..- Erro
-000019b0: 7220 6d61 6e61 6765 6d65 6e74 0d0a 2d20  r management..- 
-000019c0: 4c6f 6720 6d61 6e61 6765 6d65 6e74 0d0a  Log management..
-000019d0: 2d20 5661 7269 6162 6c65 206d 616e 6167  - Variable manag
-000019e0: 656d 656e 740d 0a2d 2043 6f6d 7061 7469  ement..- Compati
-000019f0: 6269 6c69 7479 2077 6974 6820 4972 6f6e  bility with Iron
-00001a00: 5079 7468 6f6e 2061 6e64 2043 5079 7468  Python and CPyth
-00001a10: 6f6e 0d0a 2d20 5369 6d70 6c69 6669 6361  on..- Simplifica
-00001a20: 7469 6f6e 206f 6620 636f 6d70 6c65 7820  tion of complex 
-00001a30: 4150 4920 7379 6e74 6178 2075 7369 6e67  API syntax using
-00001a40: 2064 6174 6120 6f62 6a65 6374 7320 7768   data objects wh
-00001a50: 696c 650d 0a20 206d 6169 6e74 6169 6e69  ile..  maintaini
-00001a60: 6e67 2050 4550 3820 636f 6d70 6c69 616e  ng PEP8 complian
-00001a70: 6365 2e0d 0a2d 2043 6f64 6520 7265 7573  ce...- Code reus
-00001a80: 6162 696c 6974 7920 6163 726f 7373 2064  ability across d
-00001a90: 6966 6665 7265 6e74 2073 6f6c 7665 7273  ifferent solvers
-00001aa0: 0d0a 2d20 436c 6561 7220 646f 6375 6d65  ..- Clear docume
-00001ab0: 6e74 6174 696f 6e20 6f6e 2066 756e 6374  ntation on funct
-00001ac0: 696f 6e73 2061 6e64 2041 5049 0d0a 2d20  ions and API..- 
-00001ad0: 556e 6974 2074 6573 7473 206f 6620 636f  Unit tests of co
-00001ae0: 6465 2074 6f20 696e 6372 6561 7365 2071  de to increase q
-00001af0: 7561 6c69 7479 2061 6372 6f73 7320 6469  uality across di
-00001b00: 6666 6572 656e 7420 4145 4454 2076 6572  fferent AEDT ver
-00001b10: 7369 6f6e 730d 0a0d 0a0d 0a45 7861 6d70  sions......Examp
-00001b20: 6c65 2077 6f72 6b66 6c6f 770d 0a2d 2d2d  le workflow..---
-00001b30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  --------------..
-00001b40: 312e 2049 6e69 7469 616c 697a 6520 7468  1. Initialize th
-00001b50: 6520 6060 4465 736b 746f 7060 6020 636c  e ``Desktop`` cl
-00001b60: 6173 7320 7769 7468 2074 6865 2076 6572  ass with the ver
-00001b70: 7369 6f6e 206f 6620 4145 4454 2074 6f20  sion of AEDT to 
-00001b80: 7573 652e 0d0a 322e 2049 6e69 7469 616c  use...2. Initial
-00001b90: 697a 6520 7468 6520 6170 706c 6963 6174  ize the applicat
-00001ba0: 696f 6e20 746f 2075 7365 2077 6974 6869  ion to use withi
-00001bb0: 6e20 4145 4454 2e0d 0a0d 0a0d 0a43 6f6e  n AEDT.......Con
-00001bc0: 6e65 6374 2074 6f20 4145 4454 2066 726f  nect to AEDT fro
-00001bd0: 6d20 6120 5079 7468 6f6e 2049 4445 0d0a  m a Python IDE..
-00001be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001c00: 2d0d 0a50 7941 4544 5420 776f 726b 7320  -..PyAEDT works 
-00001c10: 626f 7468 2069 6e73 6964 6520 4145 4454  both inside AEDT
-00001c20: 2061 6e64 2061 7320 6120 7374 616e 6461   and as a standa
-00001c30: 6c6f 6e65 2061 7070 2e0d 0a54 6869 7320  lone app...This 
-00001c40: 5079 7468 6f6e 206c 6962 7261 7279 2061  Python library a
-00001c50: 7574 6f6d 6174 6963 616c 6c79 2064 6574  utomatically det
-00001c60: 6563 7473 2077 6865 7468 6572 2069 7420  ects whether it 
-00001c70: 6973 2072 756e 6e69 6e67 0d0a 696e 2061  is running..in a
-00001c80: 6e20 4972 6f6e 5079 7468 6f6e 206f 7220  n IronPython or 
-00001c90: 4350 7974 686f 6e20 656e 7669 726f 6e6d  CPython environm
-00001ca0: 656e 7420 616e 6420 696e 6974 6961 6c69  ent and initiali
-00001cb0: 7a65 7320 4145 4454 2061 6363 6f72 6469  zes AEDT accordi
-00001cc0: 6e67 6c79 2e0d 0a50 7941 4544 5420 616c  ngly...PyAEDT al
-00001cd0: 736f 2070 726f 7669 6465 7320 6164 7661  so provides adva
-00001ce0: 6e63 6564 2065 7272 6f72 206d 616e 6167  nced error manag
-00001cf0: 656d 656e 742e 2055 7361 6765 2065 7861  ement. Usage exa
-00001d00: 6d70 6c65 7320 666f 6c6c 6f77 2e0d 0a0d  mples follow....
-00001d10: 0a45 7870 6c69 6369 7420 4145 4454 2064  .Explicit AEDT d
-00001d20: 6563 6c61 7261 7469 6f6e 2061 6e64 2065  eclaration and e
-00001d30: 7272 6f72 206d 616e 6167 656d 656e 740d  rror management.
-00001d40: 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  .~~~~~~~~~~~~~~~
-00001d50: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001d60: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0d  ~~~~~~~~~~~~~~~.
-00001d70: 0a0d 0a2e 2e20 636f 6465 3a3a 2070 7974  ..... code:: pyt
-00001d80: 686f 6e0d 0a0d 0a20 2020 2023 204c 6175  hon....    # Lau
-00001d90: 6e63 6820 4145 4454 2032 3032 3320 5231  nch AEDT 2023 R1
-00001da0: 2069 6e20 6e6f 6e2d 6772 6170 6869 6361   in non-graphica
-00001db0: 6c20 6d6f 6465 0d0a 0d0a 2020 2020 6672  l mode....    fr
-00001dc0: 6f6d 2070 7961 6564 7420 696d 706f 7274  om pyaedt import
-00001dd0: 2044 6573 6b74 6f70 2c20 4369 7263 7569   Desktop, Circui
-00001de0: 740d 0a20 2020 2077 6974 6820 4465 736b  t..    with Desk
-00001df0: 746f 7028 7370 6563 6966 6965 645f 7665  top(specified_ve
-00001e00: 7273 696f 6e3d 2232 3032 332e 3122 2c0d  rsion="2023.1",.
-00001e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001e20: 2020 6e6f 6e5f 6772 6170 6869 6361 6c3d    non_graphical=
-00001e30: 4661 6c73 652c 206e 6577 5f64 6573 6b74  False, new_deskt
-00001e40: 6f70 5f73 6573 7369 6f6e 3d54 7275 652c  op_session=True,
-00001e50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001e60: 2020 2063 6c6f 7365 5f6f 6e5f 6578 6974     close_on_exit
-00001e70: 3d54 7275 652c 2073 7475 6465 6e74 5f76  =True, student_v
-00001e80: 6572 7369 6f6e 3d46 616c 7365 293a 0d0a  ersion=False):..
-00001e90: 2020 2020 2020 2020 6369 7263 7569 7420          circuit 
-00001ea0: 3d20 4369 7263 7569 7428 290d 0a20 2020  = Circuit()..   
-00001eb0: 2020 2020 202e 2e2e 0d0a 2020 2020 2020       .....      
-00001ec0: 2020 2320 416e 7920 6572 726f 7220 6865    # Any error he
-00001ed0: 7265 2077 696c 6c20 6265 2063 6175 6768  re will be caugh
-00001ee0: 7420 6279 2044 6573 6b74 6f70 2e0d 0a20  t by Desktop... 
-00001ef0: 2020 2020 2020 202e 2e2e 0d0a 0d0a 2020         .......  
-00001f00: 2020 2320 4465 736b 746f 7020 6973 2061    # Desktop is a
-00001f10: 7574 6f6d 6174 6963 616c 6c79 2072 656c  utomatically rel
-00001f20: 6561 7365 6420 6865 7265 2e0d 0a0d 0a0d  eased here......
-00001f30: 0a49 6d70 6c69 6369 7420 4145 4454 2064  .Implicit AEDT d
-00001f40: 6563 6c61 7261 7469 6f6e 2061 6e64 2065  eclaration and e
-00001f50: 7272 6f72 206d 616e 6167 656d 656e 740d  rror management.
-00001f60: 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  .~~~~~~~~~~~~~~~
-00001f70: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00001f80: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0d  ~~~~~~~~~~~~~~~.
-00001f90: 0a0d 0a2e 2e20 636f 6465 3a3a 2070 7974  ..... code:: pyt
-00001fa0: 686f 6e0d 0a0d 0a20 2020 2023 204c 6175  hon....    # Lau
-00001fb0: 6e63 6820 7468 6520 6c61 7465 7374 2069  nch the latest i
-00001fc0: 6e73 7461 6c6c 6564 2076 6572 7369 6f6e  nstalled version
-00001fd0: 206f 6620 4145 4454 2069 6e20 6772 6170   of AEDT in grap
-00001fe0: 6869 6361 6c20 6d6f 6465 0d0a 0d0a 2020  hical mode....  
-00001ff0: 2020 6672 6f6d 2070 7961 6564 7420 696d    from pyaedt im
-00002000: 706f 7274 2043 6972 6375 6974 0d0a 2020  port Circuit..  
-00002010: 2020 7769 7468 2043 6972 6375 6974 2873    with Circuit(s
-00002020: 7065 6369 6669 6564 5f76 6572 7369 6f6e  pecified_version
-00002030: 3d22 3230 3233 2e31 222c 0d0a 2020 2020  ="2023.1",..    
-00002040: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00002050: 5f67 7261 7068 6963 616c 3d46 616c 7365  _graphical=False
-00002060: 2920 6173 2063 6972 6375 6974 3a0d 0a20  ) as circuit:.. 
-00002070: 2020 2020 2020 202e 2e2e 0d0a 2020 2020         .....    
-00002080: 2020 2020 2320 416e 7920 6572 726f 7220      # Any error 
-00002090: 6865 7265 2077 696c 6c20 6265 2063 6175  here will be cau
-000020a0: 6768 7420 6279 2044 6573 6b74 6f70 2e0d  ght by Desktop..
-000020b0: 0a20 2020 2020 2020 202e 2e2e 0d0a 0d0a  .        .......
-000020c0: 2020 2020 2320 4465 736b 746f 7020 6973      # Desktop is
-000020d0: 2061 7574 6f6d 6174 6963 616c 6c79 2072   automatically r
-000020e0: 656c 6561 7365 6420 6865 7265 2e0d 0a0d  eleased here....
-000020f0: 0a0d 0a52 656d 6f74 6520 6170 706c 6963  ...Remote applic
-00002100: 6174 696f 6e20 6361 6c6c 0d0a 7e7e 7e7e  ation call..~~~~
-00002110: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00002120: 7e7e 7e0d 0a59 6f75 2063 616e 206d 616b  ~~~..You can mak
-00002130: 6520 6120 7265 6d6f 7465 2061 7070 6c69  e a remote appli
-00002140: 6361 7469 6f6e 2063 616c 6c20 6f6e 2061  cation call on a
-00002150: 2043 5079 7468 6f6e 2073 6572 7665 720d   CPython server.
-00002160: 0a6f 7220 616e 7920 5769 6e64 6f77 7320  .or any Windows 
-00002170: 636c 6965 6e74 206d 6163 6869 6e65 2e0d  client machine..
-00002180: 0a0d 0a4f 6e20 6120 4350 7974 686f 6e20  ...On a CPython 
-00002190: 7365 7276 6572 3a0d 0a0d 0a2e 2e20 636f  server:...... co
-000021a0: 6465 3a3a 2070 7974 686f 6e0d 0a0d 0a20  de:: python.... 
-000021b0: 2020 2023 204c 6175 6e63 6820 5079 4145     # Launch PyAE
-000021c0: 4454 2072 656d 6f74 6520 7365 7276 6572  DT remote server
-000021d0: 206f 6e20 4350 7974 686f 6e0d 0a0d 0a20   on CPython.... 
-000021e0: 2020 2066 726f 6d20 7079 6165 6474 2e63     from pyaedt.c
-000021f0: 6f6d 6d6f 6e5f 7270 6320 696d 706f 7274  ommon_rpc import
-00002200: 2070 7961 6564 745f 7365 7276 6963 655f   pyaedt_service_
-00002210: 6d61 6e61 6765 720d 0a20 2020 2070 7961  manager..    pya
-00002220: 6564 745f 7365 7276 6963 655f 6d61 6e61  edt_service_mana
-00002230: 6765 7228 290d 0a0d 0a0d 0a4f 6e20 616e  ger()......On an
-00002240: 7920 5769 6e64 6f77 7320 636c 6965 6e74  y Windows client
-00002250: 206d 6163 6869 6e65 3a0d 0a0d 0a2e 2e20   machine:...... 
-00002260: 636f 6465 3a3a 2070 7974 686f 6e0d 0a0d  code:: python...
-00002270: 0a20 2020 2066 726f 6d20 7079 6165 6474  .    from pyaedt
-00002280: 2e63 6f6d 6d6f 6e5f 7270 6320 696d 706f  .common_rpc impo
-00002290: 7274 2063 7265 6174 655f 7365 7373 696f  rt create_sessio
-000022a0: 6e0d 0a20 2020 2063 6c31 203d 2063 7265  n..    cl1 = cre
-000022b0: 6174 655f 7365 7373 696f 6e28 2273 6572  ate_session("ser
-000022c0: 7665 725f 6e61 6d65 2229 0d0a 2020 2020  ver_name")..    
-000022d0: 636c 312e 6165 6474 2870 6f72 743d 3530  cl1.aedt(port=50
-000022e0: 3030 302c 206e 6f6e 5f67 7261 7068 6963  000, non_graphic
-000022f0: 616c 3d46 616c 7365 290d 0a20 2020 2068  al=False)..    h
-00002300: 6673 7320 3d20 4866 7373 286d 6163 6869  fss = Hfss(machi
-00002310: 6e65 3d22 7365 7276 6572 5f6e 616d 6522  ne="server_name"
-00002320: 2c20 706f 7274 3d35 3030 3030 290d 0a20  , port=50000).. 
-00002330: 2020 2023 2079 6f75 7220 636f 6465 2068     # your code h
-00002340: 6572 650d 0a0d 0a56 6172 6961 626c 6573  ere....Variables
-00002350: 0d0a 7e7e 7e7e 7e7e 7e7e 7e0d 0a0d 0a2e  ..~~~~~~~~~.....
-00002360: 2e20 636f 6465 3a3a 2070 7974 686f 6e0d  . code:: python.
-00002370: 0a0d 0a20 2020 2066 726f 6d20 7079 6165  ...    from pyae
-00002380: 6474 2e48 4653 5320 696d 706f 7274 2048  dt.HFSS import H
-00002390: 4653 530d 0a20 2020 2077 6974 6820 4846  FSS..    with HF
-000023a0: 5353 2061 7320 6866 7373 3a0d 0a20 2020  SS as hfss:..   
-000023b0: 2020 2020 2020 6866 7373 5b22 6469 6d22        hfss["dim"
-000023c0: 5d20 3d20 2231 6d6d 2220 2020 2320 6465  ] = "1mm"   # de
-000023d0: 7369 676e 2076 6172 6961 626c 650d 0a20  sign variable.. 
-000023e0: 2020 2020 2020 2020 6866 7373 5b22 2464          hfss["$d
-000023f0: 696d 225d 203d 2022 316d 6d22 2020 2320  im"] = "1mm"  # 
-00002400: 7072 6f6a 6563 7420 7661 7269 6162 6c65  project variable
-00002410: 0d0a 0d0a 0d0a 4d6f 6465 6c65 720d 0a7e  ......Modeler..~
-00002420: 7e7e 7e7e 7e7e 0d0a 0d0a 2e2e 2063 6f64  ~~~~~~...... cod
-00002430: 653a 3a20 7079 7468 6f6e 0d0a 0d0a 2020  e:: python....  
-00002440: 2020 2320 4372 6561 7465 2061 2062 6f78    # Create a box
-00002450: 2c20 6173 7369 676e 2076 6172 6961 626c  , assign variabl
-00002460: 6573 2c20 616e 6420 6173 7369 676e 206d  es, and assign m
-00002470: 6174 6572 6961 6c73 2e0d 0a0d 0a20 2020  aterials.....   
-00002480: 2066 726f 6d20 7079 6165 6474 2e68 6673   from pyaedt.hfs
-00002490: 7320 696d 706f 7274 2048 6673 730d 0a20  s import Hfss.. 
-000024a0: 2020 2077 6974 6820 4866 7373 2061 7320     with Hfss as 
-000024b0: 6866 7373 3a0d 0a20 2020 2020 2020 2020  hfss:..         
-000024c0: 6866 7373 2e6d 6f64 656c 6572 2e63 7265  hfss.modeler.cre
-000024d0: 6174 655f 626f 7828 5b30 2c20 302c 2030  ate_box([0, 0, 0
-000024e0: 5d2c 205b 3130 2c20 2264 696d 222c 2031  ], [10, "dim", 1
-000024f0: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
-00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002510: 2020 2020 2020 226d 7962 6f78 222c 2022        "mybox", "
-00002520: 616c 756d 696e 756d 2229 0d0a 0d0a 4c69  aluminum")....Li
-00002530: 6365 6e73 650d 0a2d 2d2d 2d2d 2d2d 0d0a  cense..-------..
-00002540: 5079 4145 4454 2069 7320 6c69 6365 6e73  PyAEDT is licens
-00002550: 6564 2075 6e64 6572 2074 6865 204d 4954  ed under the MIT
-00002560: 206c 6963 656e 7365 2e0d 0a0d 0a54 6869   license.....Thi
-00002570: 7320 6d6f 6475 6c65 206d 616b 6573 206e  s module makes n
-00002580: 6f20 636f 6d6d 6572 6369 616c 2063 6c61  o commercial cla
-00002590: 696d 206f 7665 7220 416e 7379 7320 7768  im over Ansys wh
-000025a0: 6174 736f 6576 6572 2e0d 0a50 7941 4544  atsoever...PyAED
-000025b0: 5420 6578 7465 6e64 7320 7468 6520 6675  T extends the fu
-000025c0: 6e63 7469 6f6e 616c 6974 7920 6f66 2041  nctionality of A
-000025d0: 4544 5420 6279 2061 6464 696e 670d 0a61  EDT by adding..a
-000025e0: 6e20 6164 6469 7469 6f6e 616c 2050 7974  n additional Pyt
-000025f0: 686f 6e20 696e 7465 7266 6163 6520 746f  hon interface to
-00002600: 2041 4544 5420 7769 7468 6f75 7420 6368   AEDT without ch
-00002610: 616e 6769 6e67 2074 6865 2063 6f72 650d  anging the core.
-00002620: 0a62 6568 6176 696f 7220 6f72 206c 6963  .behavior or lic
-00002630: 656e 7365 206f 6620 7468 6520 6f72 6967  ense of the orig
-00002640: 696e 616c 2073 6f66 7477 6172 652e 2054  inal software. T
-00002650: 6865 2075 7365 206f 6620 7468 650d 0a69  he use of the..i
-00002660: 6e74 6572 6163 7469 7665 2063 6f6e 7472  nteractive contr
-00002670: 6f6c 206f 6620 5079 4145 4454 2072 6571  ol of PyAEDT req
-00002680: 7569 7265 7320 6120 6c65 6761 6c6c 7920  uires a legally 
-00002690: 6c69 6365 6e73 6564 0d0a 6c6f 6361 6c20  licensed..local 
-000026a0: 636f 7079 206f 6620 4145 4454 2e20 466f  copy of AEDT. Fo
-000026b0: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
-000026c0: 6f6e 2061 626f 7574 2041 4544 542c 200d  on about AEDT, .
-000026d0: 0a73 6565 2074 6865 2060 416e 7379 7320  .see the `Ansys 
-000026e0: 456c 6563 7472 6f6e 6963 7320 3c68 7474  Electronics <htt
-000026f0: 7073 3a2f 2f77 7777 2e61 6e73 7973 2e63  ps://www.ansys.c
-00002700: 6f6d 2f70 726f 6475 6374 732f 656c 6563  om/products/elec
-00002710: 7472 6f6e 6963 733e 605f 200d 0a70 6167  tronics>`_ ..pag
-00002720: 6520 6f6e 2074 6865 2041 6e73 7973 2077  e on the Ansys w
-00002730: 6562 7369 7465 2e0d 0a                   ebsite...
+00000000: 3c21 2d2d 202d 2d3e 0d0a 3c61 206e 616d  <!-- -->..<a nam
+00000010: 653d 2272 6561 646d 652d 746f 7022 3e3c  e="readme-top"><
+00000020: 2f61 3e0d 0a3c 212d 2d0d 0a2a 2a2a 2050  /a>..<!--..*** P
+00000030: 7941 4544 5420 5245 4144 4d45 0d0a 2d2d  yAEDT README..--
+00000040: 3e0d 0a0d 0a0d 0a23 2050 7941 4544 540d  >......# PyAEDT.
+00000050: 0a0d 0a3c 7020 7374 796c 653d 2274 6578  ...<p style="tex
+00000060: 742d 616c 6967 6e3a 2063 656e 7465 723b  t-align: center;
+00000070: 223e 0d0a 2020 2020 3c62 723e 2045 6e67  ">..    <br> Eng
+00000080: 6c69 7368 207c 203c 6120 6872 6566 3d22  lish | <a href="
+00000090: 5245 4144 4d45 5f43 4e2e 6d64 223e e4b8  README_CN.md">..
+000000a0: ade6 9687 3c2f 613e 0d0a 3c2f 703e 0d0a  ....</a>..</p>..
+000000b0: 0d0a 5b21 5b50 7941 6e73 7973 5d28 6874  ..[![PyAnsys](ht
+000000c0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000000d0: 732e 696f 2f62 6164 6765 2f50 792d 416e  s.io/badge/Py-An
+000000e0: 7379 732d 6666 6331 3037 2e73 7667 3f6c  sys-ffc107.svg?l
+000000f0: 6f67 6f3d 6461 7461 3a69 6d61 6765 2f70  ogo=data:image/p
+00000100: 6e67 3b62 6173 6536 342c 6956 424f 5277  ng;base64,iVBORw
+00000110: 304b 4767 6f41 4141 414e 5355 6845 5567  0KGgoAAAANSUhEUg
+00000120: 4141 4142 4141 4141 4151 4341 4941 4141  AAABAAAAAQCAIAAA
+00000130: 4351 6b57 6732 4141 4142 446b 6c45 5156  CQkWg2AAABDklEQV
+00000140: 5134 6a57 4e67 6f44 6667 356d 4438 7645  Q4jWNgoDfg5mD8vE
+00000150: 3771 2f33 6270 5679 736b 6257 3073 4d52  7q/3bpVyskbW0sMR
+00000160: 5577 6f66 4844 3744 6835 4f42 6b5a 4742  UwofHD7Dh5OBkZGB
+00000170: 6757 372f 3357 3274 5a70 6132 744c 5145  gW7/3W2tZpa2tLQE
+00000180: 4f79 4f7a 6545 7366 756d 6c4b 3274 6256  OyOzeEsfumlK2tbV
+00000190: 7061 476a 344e 366a 4973 316c 7073 4441  paGj4N6jIs1lpsDA
+000001a0: 774d 4a32 3738 7376 654d 5932 4267 4341  wMJ278sveMY2BgCA
+000001b0: 304e 4652 4953 7771 6b68 7951 3171 2f4e  0NFRISwqkhyQ1q/N
+000001c0: 7964 337a 6734 4f42 6759 474e 6a5a 3265  yd3zg4OBgYGNjZ2e
+000001d0: 5069 3472 4235 6c6f 4742 685a 6e68 7854  Pi4rB5loGBhZnhxT
+000001e0: 4c4a 2f39 756c 7632 3651 3475 566b 314e  LJ/9ulv26Q4uVk1N
+000001f0: 5856 2f66 2f2f 2f2f 2f2f 2f36 3964 7534  XV/f///////69du4
+00000200: 5a64 6737 386c 782f 2f74 3076 2b33 5338  Zdg78lx//t0v+3S8
+00000210: 3872 4649 5349 6e44 3539 4771 4948 3265  8rFISInD59GqIH2e
+00000220: 7349 4a38 4739 4f32 2f58 5677 686a 7a70  sIJ8G9O2/XVwhjzp
+00000230: 7735 4541 616d 3178 6b6b 424a 6e2f 624a  w5EAam1xkkBJn/bJ
+00000240: 582b 7631 3336 3568 7878 7543 4166 4839  X+v1365hxxuCAfH9
+00000250: 2b33 6239 2f2b 2f2f 2f2f 3438 6350 754e  +3b9/+////48cPuN
+00000260: 6568 4e73 5337 6344 457a 4d54 4177 4d4d  ehNsS7cDEzMTAwMM
+00000270: 7a62 2b51 3275 3464 4f6e 5432 7657 724d  zb+Q2u4dOnT2vWrM
+00000280: 4875 395a 747a 7850 3976 6c2f 3639 5256  Hu9ZtzxP9vl/69RV
+00000290: 7043 6b42 6c5a 334e 3765 6e6f 4458 4277  pCkBlZ3N7enoDXBw
+000002a0: 4541 4141 2b59 5969 744f 696c 4d56 4141  EAAA+YYitOilMVAA
+000002b0: 4141 4145 6c46 546b 5375 516d 4343 295d  AAAElFTkSuQmCC)]
+000002c0: 2868 7474 7073 3a2f 2f64 6f63 732e 7079  (https://docs.py
+000002d0: 616e 7379 732e 636f 6d2f 295b 215b 7079  ansys.com/)[![py
+000002e0: 7069 5d28 6874 7470 733a 2f2f 696d 672e  pi](https://img.
+000002f0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000300: 762f 7079 6165 6474 2e73 7667 3f6c 6f67  v/pyaedt.svg?log
+00000310: 6f3d 7079 7468 6f6e 266c 6f67 6f43 6f6c  o=python&logoCol
+00000320: 6f72 3d77 6869 7465 295d 2868 7474 7073  or=white)](https
+00000330: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000340: 6563 742f 7079 6165 6474 2f29 5b21 5b50  ect/pyaedt/)[![P
+00000350: 7950 4961 6374 5d28 6874 7470 733a 2f2f  yPIact](https://
+00000360: 7065 7079 2e74 6563 682f 6261 6467 652f  pepy.tech/badge/
+00000370: 7079 6165 6474 2f6d 6f6e 7468 295d 2868  pyaedt/month)](h
+00000380: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00000390: 7072 6f6a 6563 742f 7079 6165 6474 2f29  project/pyaedt/)
+000003a0: 5b21 5b50 7974 686f 6e56 6572 7369 6f6e  [![PythonVersion
+000003b0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+000003c0: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
+000003d0: 7974 686f 6e2d 332e 372b 2d62 6c75 652e  ython-3.7+-blue.
+000003e0: 7376 6729 5d28 6874 7470 733a 2f2f 7777  svg)](https://ww
+000003f0: 772e 7079 7468 6f6e 2e6f 7267 2f64 6f77  w.python.org/dow
+00000400: 6e6c 6f61 6473 2f29 5b21 5b47 482d 4349  nloads/)[![GH-CI
+00000410: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000420: 2e63 6f6d 2f70 7961 6e73 7973 2f70 7961  .com/pyansys/pya
+00000430: 6564 742f 6163 7469 6f6e 732f 776f 726b  edt/actions/work
+00000440: 666c 6f77 732f 756e 6974 5f74 6573 7473  flows/unit_tests
+00000450: 2e79 6d6c 2f62 6164 6765 2e73 7667 295d  .yml/badge.svg)]
+00000460: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000470: 636f 6d2f 7079 616e 7379 732f 7079 6165  com/pyansys/pyae
+00000480: 6474 2f61 6374 696f 6e73 2f77 6f72 6b66  dt/actions/workf
+00000490: 6c6f 7773 2f75 6e69 745f 7465 7374 732e  lows/unit_tests.
+000004a0: 796d 6c29 5b21 5b63 6f64 6563 6f76 5d28  yml)[![codecov](
+000004b0: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+000004c0: 696f 2f67 682f 7079 616e 7379 732f 7079  io/gh/pyansys/py
+000004d0: 6165 6474 2f62 7261 6e63 682f 6d61 696e  aedt/branch/main
+000004e0: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
+000004f0: 295d 2868 7474 7073 3a2f 2f63 6f64 6563  )](https://codec
+00000500: 6f76 2e69 6f2f 6768 2f70 7961 6e73 7973  ov.io/gh/pyansys
+00000510: 2f70 7961 6564 7429 5b21 5b4d 4954 5d28  /pyaedt)[![MIT](
+00000520: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000530: 6c64 732e 696f 2f62 6164 6765 2f4c 6963  lds.io/badge/Lic
+00000540: 656e 7365 2d4d 4954 2d79 656c 6c6f 772e  ense-MIT-yellow.
+00000550: 7376 6729 5d28 6874 7470 733a 2f2f 6f70  svg)](https://op
+00000560: 656e 736f 7572 6365 2e6f 7267 2f6c 6963  ensource.org/lic
+00000570: 656e 7365 732f 4d49 5429 5b21 5b62 6c61  enses/MIT)[![bla
+00000580: 636b 5d28 6874 7470 733a 2f2f 696d 672e  ck](https://img.
+00000590: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000005a0: 2f63 6f64 6525 3230 7374 796c 652d 626c  /code%20style-bl
+000005b0: 6163 6b2d 3030 3030 3030 2e73 7667 3f73  ack-000000.svg?s
+000005c0: 7479 6c65 3d66 6c61 7429 5d28 6874 7470  tyle=flat)](http
+000005d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+000005e0: 7366 2f62 6c61 636b 295b 215b 416e 6163  sf/black)[![Anac
+000005f0: 6f6e 6461 5d28 6874 7470 733a 2f2f 616e  onda](https://an
+00000600: 6163 6f6e 6461 2e6f 7267 2f63 6f6e 6461  aconda.org/conda
+00000610: 2d66 6f72 6765 2f70 7961 6564 742f 6261  -forge/pyaedt/ba
+00000620: 6467 6573 2f76 6572 7369 6f6e 2e73 7667  dges/version.svg
+00000630: 295d 2868 7474 7073 3a2f 2f61 6e61 636f  )](https://anaco
+00000640: 6e64 612e 6f72 672f 636f 6e64 612d 666f  nda.org/conda-fo
+00000650: 7267 652f 7079 6165 6474 295b 215b 7072  rge/pyaedt)[![pr
+00000660: 652d 636f 6d6d 6974 5d28 6874 7470 733a  e-commit](https:
+00000670: 2f2f 7265 7375 6c74 732e 7072 652d 636f  //results.pre-co
+00000680: 6d6d 6974 2e63 692f 6261 6467 652f 6769  mmit.ci/badge/gi
+00000690: 7468 7562 2f70 7961 6e73 7973 2f70 7961  thub/pyansys/pya
+000006a0: 6564 742f 6d61 696e 2e73 7667 295d 2868  edt/main.svg)](h
+000006b0: 7474 7073 3a2f 2f72 6573 756c 7473 2e70  ttps://results.p
+000006c0: 7265 2d63 6f6d 6d69 742e 6369 2f6c 6174  re-commit.ci/lat
+000006d0: 6573 742f 6769 7468 7562 2f70 7961 6e73  est/github/pyans
+000006e0: 7973 2f70 7961 6564 742f 6d61 696e 290d  ys/pyaedt/main).
+000006f0: 0a0d 0a23 2320 5768 6174 2069 7320 5079  ...## What is Py
+00000700: 4145 4454 3f0d 0a0d 0a60 5079 4145 4454  AEDT?....`PyAEDT
+00000710: 6020 6973 2061 2050 7974 686f 6e20 6c69  ` is a Python li
+00000720: 6272 6172 7920 7468 6174 2069 6e74 6572  brary that inter
+00000730: 6163 7473 2064 6972 6563 746c 7920 7769  acts directly wi
+00000740: 7468 2074 6865 2041 5049 2066 6f72 0d0a  th the API for..
+00000750: 416e 7379 7320 456c 6563 7472 6f6e 6963  Ansys Electronic
+00000760: 7320 4465 736b 746f 7020 2841 4544 5429  s Desktop (AEDT)
+00000770: 2074 6f20 6d61 6b65 2073 6372 6970 7469   to make scripti
+00000780: 6e67 2073 696d 706c 6572 2e20 5468 6520  ng simpler. The 
+00000790: 6172 6368 6974 6563 7475 7265 0d0a 666f  architecture..fo
+000007a0: 7220 5079 4145 4454 2063 616e 2062 6520  r PyAEDT can be 
+000007b0: 7265 7573 6564 2066 6f72 2061 6c6c 2041  reused for all A
+000007c0: 4544 5420 3344 2070 726f 6475 6374 7320  EDT 3D products 
+000007d0: 2848 4653 532c 2049 6365 7061 6b2c 204d  (HFSS, Icepak, M
+000007e0: 6178 7765 6c6c 2033 442c 0d0a 616e 6420  axwell 3D,..and 
+000007f0: 5133 4420 4578 7472 6163 746f 7229 2c20  Q3D Extractor), 
+00000800: 3244 2074 6f6f 6c73 2c20 616e 6420 416e  2D tools, and An
+00000810: 7379 7320 4d65 6368 616e 6963 616c 2e20  sys Mechanical. 
+00000820: 5079 4145 4454 2061 6c73 6f20 7072 6f76  PyAEDT also prov
+00000830: 6964 6573 0d0a 7375 7070 6f72 7420 666f  ides..support fo
+00000840: 7220 6369 7263 7569 7420 746f 6f6c 7320  r circuit tools 
+00000850: 6c69 6b65 204e 6578 7869 6d20 616e 6420  like Nexxim and 
+00000860: 7379 7374 656d 2073 696d 756c 6174 696f  system simulatio
+00000870: 6e20 746f 6f6c 7320 6c69 6b65 0d0a 5477  n tools like..Tw
+00000880: 696e 2042 7569 6c64 6572 2e20 4669 6e61  in Builder. Fina
+00000890: 6c6c 792c 2050 7941 4544 5420 7072 6f76  lly, PyAEDT prov
+000008a0: 6964 6573 2073 6372 6970 7469 6e67 2063  ides scripting c
+000008b0: 6170 6162 696c 6974 6965 7320 696e 2041  apabilities in A
+000008c0: 6e73 7973 206c 6179 6f75 740d 0a74 6f6f  nsys layout..too
+000008d0: 6c73 206c 696b 6520 4846 5353 2033 4420  ls like HFSS 3D 
+000008e0: 4c61 796f 7574 2061 6e64 2045 4442 2e20  Layout and EDB. 
+000008f0: 5468 6520 5079 4145 4454 2063 6c61 7373  The PyAEDT class
+00000900: 2061 6e64 206d 6574 686f 6420 7374 7275   and method stru
+00000910: 6374 7572 6573 0d0a 7369 6d70 6c69 6679  ctures..simplify
+00000920: 206f 7065 7261 7469 6f6e 2077 6869 6c65   operation while
+00000930: 2072 6575 7369 6e67 2069 6e66 6f72 6d61   reusing informa
+00000940: 7469 6f6e 2061 7320 6d75 6368 2061 7320  tion as much as 
+00000950: 706f 7373 6962 6c65 2061 6372 6f73 730d  possible across.
+00000960: 0a74 6865 2041 5049 2e0d 0a0d 0a23 2320  .the API.....## 
+00000970: 496e 7374 616c 6c20 6f6e 2043 5079 7468  Install on CPyth
+00000980: 6f6e 2066 726f 6d20 5079 5049 0d0a 0d0a  on from PyPI....
+00000990: 596f 7520 6361 6e20 696e 7374 616c 6c20  You can install 
+000009a0: 5079 4145 4454 206f 6e20 4350 7974 686f  PyAEDT on CPytho
+000009b0: 6e20 332e 3720 7468 726f 7567 6820 332e  n 3.7 through 3.
+000009c0: 3130 2066 726f 6d20 5079 5049 2077 6974  10 from PyPI wit
+000009d0: 6820 7468 6973 2063 6f6d 6d61 6e64 3a0d  h this command:.
+000009e0: 0a0d 0a60 6060 7368 0d0a 2020 7069 7020  ...```sh..  pip 
+000009f0: 696e 7374 616c 6c20 7079 6165 6474 0d0a  install pyaedt..
+00000a00: 6060 600d 0a0d 0a49 6e73 7461 6c6c 2060  ```....Install `
+00000a10: 5079 4145 4454 6020 7769 7468 2061 6c6c  PyAEDT` with all
+00000a20: 2065 7874 7261 2070 6163 6b61 6765 7320   extra packages 
+00000a30: 286d 6174 706c 6f74 6c69 622c 206e 756d  (matplotlib, num
+00000a40: 7079 2c20 7061 6e64 6173 2c20 7079 7669  py, pandas, pyvi
+00000a50: 7374 6129 3a0d 0a0d 0a60 6060 7368 0d0a  sta):....```sh..
+00000a60: 2020 7069 7020 696e 7374 616c 6c20 7079    pip install py
+00000a70: 6165 6474 5b66 756c 6c5d 0d0a 6060 600d  aedt[full]..```.
+00000a80: 0a0d 0a59 6f75 2063 616e 2061 6c73 6f20  ...You can also 
+00000a90: 696e 7374 616c 6c20 5079 4145 4454 2066  install PyAEDT f
+00000aa0: 726f 6d20 436f 6e64 612d 466f 7267 6520  rom Conda-Forge 
+00000ab0: 7769 7468 2074 6869 7320 636f 6d6d 616e  with this comman
+00000ac0: 643a 0d0a 0d0a 6060 6073 680d 0a20 2063  d:....```sh..  c
+00000ad0: 6f6e 6461 2069 6e73 7461 6c6c 202d 6320  onda install -c 
+00000ae0: 636f 6e64 612d 666f 7267 6520 7079 6165  conda-forge pyae
+00000af0: 6474 0d0a 6060 600d 0a50 7941 4544 5420  dt..```..PyAEDT 
+00000b00: 7265 6d61 696e 7320 636f 6d70 6174 6962  remains compatib
+00000b10: 6c65 2077 6974 6820 4972 6f6e 5079 7468  le with IronPyth
+00000b20: 6f6e 2061 6e64 2063 616e 2062 6520 7374  on and can be st
+00000b30: 696c 6c20 7573 6564 2069 6e20 7468 6520  ill used in the 
+00000b40: 4145 4454 2046 7261 6d65 776f 726b 2e0d  AEDT Framework..
+00000b50: 0a0d 0a23 2320 4162 6f75 7420 5079 416e  ...## About PyAn
+00000b60: 7379 730d 0a0d 0a60 5079 4145 4454 6020  sys....`PyAEDT` 
+00000b70: 6973 2070 6172 7420 6f66 2074 6865 206c  is part of the l
+00000b80: 6172 6765 7220 5b50 7941 6e73 7973 5d28  arger [PyAnsys](
+00000b90: 6874 7470 733a 2f2f 646f 6373 2e70 7961  https://docs.pya
+00000ba0: 6e73 7973 2e63 6f6d 2022 5079 416e 7379  nsys.com "PyAnsy
+00000bb0: 7322 2920 6566 666f 7274 2074 6f20 6661  s") effort to fa
+00000bc0: 6369 6c69 7461 7465 2074 6865 2075 7365  cilitate the use
+00000bd0: 206f 6620 416e 7379 7320 7465 6368 6e6f   of Ansys techno
+00000be0: 6c6f 6769 6573 2064 6972 6563 746c 7920  logies directly 
+00000bf0: 6672 6f6d 2050 7974 686f 6e2e 0d0a 0d0a  from Python.....
+00000c00: 5079 4145 4454 2069 7320 696e 7465 6e64  PyAEDT is intend
+00000c10: 6564 2074 6f20 636f 6e73 6f6c 6964 6174  ed to consolidat
+00000c20: 6520 616e 6420 6578 7465 6e64 2061 6c6c  e and extend all
+00000c30: 2065 7869 7374 696e 670d 0a66 756e 6374   existing..funct
+00000c40: 696f 6e61 6c69 7469 6573 2061 726f 756e  ionalities aroun
+00000c50: 6420 7363 7269 7074 696e 6720 666f 7220  d scripting for 
+00000c60: 4145 4454 2074 6f20 616c 6c6f 7720 7265  AEDT to allow re
+00000c70: 7573 6520 6f66 2065 7869 7374 696e 6720  use of existing 
+00000c80: 636f 6465 2c0d 0a73 6861 7269 6e67 206f  code,..sharing o
+00000c90: 6620 6265 7374 2070 7261 6374 6963 6573  f best practices
+00000ca0: 2c20 616e 6420 696e 6372 6561 7365 6420  , and increased 
+00000cb0: 636f 6c6c 6162 6f72 6174 696f 6e2e 0d0a  collaboration...
+00000cc0: 0d0a 2323 2041 626f 7574 2041 4544 540d  ..## About AEDT.
+00000cd0: 0a0d 0a5b 4145 4454 5d28 6874 7470 733a  ...[AEDT](https:
+00000ce0: 2f2f 7777 772e 616e 7379 732e 636f 6d2f  //www.ansys.com/
+00000cf0: 7072 6f64 7563 7473 2f65 6c65 6374 726f  products/electro
+00000d00: 6e69 6373 2920 6973 2061 2070 6c61 7466  nics) is a platf
+00000d10: 6f72 6d20 7468 6174 2065 6e61 626c 6573  orm that enables
+00000d20: 2074 7275 650d 0a65 6c65 6374 726f 6e69   true..electroni
+00000d30: 6373 2073 7973 7465 6d20 6465 7369 676e  cs system design
+00000d40: 2e20 4145 4454 2070 726f 7669 6465 7320  . AEDT provides 
+00000d50: 6163 6365 7373 2074 6f20 7468 6520 416e  access to the An
+00000d60: 7379 7320 676f 6c64 2d73 7461 6e64 6172  sys gold-standar
+00000d70: 640d 0a65 6c65 6374 726f 2d6d 6167 6e65  d..electro-magne
+00000d80: 7469 6373 2073 696d 756c 6174 696f 6e20  tics simulation 
+00000d90: 736f 6c75 7469 6f6e 732c 2073 7563 6820  solutions, such 
+00000da0: 6173 2041 6e73 7973 2048 4653 532c 2041  as Ansys HFSS, A
+00000db0: 6e73 7973 204d 6178 7765 6c6c 2c0d 0a41  nsys Maxwell,..A
+00000dc0: 6e73 7973 2051 3344 2045 7874 7261 6374  nsys Q3D Extract
+00000dd0: 6f72 2c20 416e 7379 7320 5369 7761 7665  or, Ansys Siwave
+00000de0: 2c20 616e 6420 416e 7379 7320 4963 6570  , and Ansys Icep
+00000df0: 616b 2075 7369 6e67 2065 6c65 6374 7269  ak using electri
+00000e00: 6361 6c20 4341 4420 2845 4341 4429 2061  cal CAD (ECAD) a
+00000e10: 6e64 0d0a 4d65 6368 616e 6963 616c 2043  nd..Mechanical C
+00000e20: 4144 2028 4d43 4144 2920 776f 726b 666c  AD (MCAD) workfl
+00000e30: 6f77 732e 0d0a 0d0a 496e 2061 6464 6974  ows.....In addit
+00000e40: 696f 6e2c 2041 4544 5420 696e 636c 7564  ion, AEDT includ
+00000e50: 6573 2064 6972 6563 7420 6c69 6e6b 7320  es direct links 
+00000e60: 746f 2074 6865 2063 6f6d 706c 6574 6520  to the complete 
+00000e70: 416e 7379 7320 706f 7274 666f 6c69 6f20  Ansys portfolio 
+00000e80: 6f66 2074 6865 726d 616c 2c20 666c 7569  of thermal, flui
+00000e90: 642c 0d0a 616e 6420 6d65 6368 616e 6963  d,..and mechanic
+00000ea0: 616c 2073 6f6c 7665 7273 2066 6f72 2063  al solvers for c
+00000eb0: 6f6d 7072 6568 656e 7369 7665 206d 756c  omprehensive mul
+00000ec0: 7469 7068 7973 6963 7320 616e 616c 7973  tiphysics analys
+00000ed0: 6973 2e0d 0a54 6967 6874 2069 6e74 6567  is...Tight integ
+00000ee0: 7261 7469 6f6e 2061 6d6f 6e67 2074 6865  ration among the
+00000ef0: 7365 2073 6f6c 7574 696f 6e73 2070 726f  se solutions pro
+00000f00: 7669 6465 7320 756e 7072 6563 6564 656e  vides unpreceden
+00000f10: 7465 6420 6561 7365 206f 6620 7573 6520  ted ease of use 
+00000f20: 666f 7220 7365 7475 7020 616e 640d 0a66  for setup and..f
+00000f30: 6173 7465 7220 7265 736f 6c75 7469 6f6e  aster resolution
+00000f40: 206f 6620 636f 6d70 6c65 7820 7369 6d75   of complex simu
+00000f50: 6c61 7469 6f6e 7320 666f 7220 6465 7369  lations for desi
+00000f60: 676e 2061 6e64 206f 7074 696d 697a 6174  gn and optimizat
+00000f70: 696f 6e2e 0d0a 0d0a 3c70 2061 6c69 676e  ion.....<p align
+00000f80: 3d22 6365 6e74 6572 223e 0d0a 2020 3c69  ="center">..  <i
+00000f90: 6d67 2077 6964 7468 3d22 3130 3025 2220  mg width="100%" 
+00000fa0: 7372 633d 2268 7474 7073 3a2f 2f69 6d61  src="https://ima
+00000fb0: 6765 732e 616e 7379 732e 636f 6d2f 6973  ges.ansys.com/is
+00000fc0: 2f69 6d61 6765 2f61 6e73 7973 2f61 6e73  /image/ansys/ans
+00000fd0: 7973 2d65 6c65 6374 726f 6e69 6373 2d74  ys-electronics-t
+00000fe0: 6563 686e 6f6c 6f67 792d 636f 6c6c 6167  echnology-collag
+00000ff0: 653f 7769 643d 3934 3126 6f70 5f75 736d  e?wid=941&op_usm
+00001000: 3d30 2e39 2c31 2e30 2c32 302c 3026 6669  =0.9,1.0,20,0&fi
+00001010: 743d 636f 6e73 7472 6169 6e2c 3022 2074  t=constrain,0" t
+00001020: 6974 6c65 3d22 4145 4454 2041 7070 6c69  itle="AEDT Appli
+00001030: 6361 7469 6f6e 7322 2068 6572 663d 2268  cations" herf="h
+00001040: 7474 7073 3a2f 2f77 7777 2e61 6e73 7973  ttps://www.ansys
+00001050: 2e63 6f6d 2f70 726f 6475 6374 732f 656c  .com/products/el
+00001060: 6563 7472 6f6e 6963 7322 0d0a 2020 2f3e  ectronics"..  />
+00001070: 0d0a 3c2f 703e 0d0a 0d0a 6050 7941 4544  ..</p>....`PyAED
+00001080: 5460 2069 7320 6c69 6365 6e73 6564 2075  T` is licensed u
+00001090: 6e64 6572 2074 6865 205b 4d49 5420 4c69  nder the [MIT Li
+000010a0: 6365 6e73 655d 2868 7474 7073 3a2f 2f67  cense](https://g
+000010b0: 6974 6875 622e 636f 6d2f 7079 616e 7379  ithub.com/pyansy
+000010c0: 732f 5079 4145 4454 2f62 6c6f 622f 6d61  s/PyAEDT/blob/ma
+000010d0: 696e 2f4c 4943 454e 5345 290d 0a0d 0a60  in/LICENSE)....`
+000010e0: 5079 4145 4454 6020 696e 636c 7564 6573  PyAEDT` includes
+000010f0: 2066 756e 6374 696f 6e61 6c69 7479 2066   functionality f
+00001100: 6f72 2069 6e74 6572 6163 7469 6e67 2077  or interacting w
+00001110: 6974 6820 7468 6520 666f 6c6c 6f77 696e  ith the followin
+00001120: 6720 6041 4544 5420 746f 6f6c 7360 2061  g `AEDT tools` a
+00001130: 6e64 2060 416e 7379 7320 7072 6f64 7563  nd `Ansys produc
+00001140: 7473 603a 0d0a 0d0a 2020 2d20 4846 5353  ts`:....  - HFSS
+00001150: 2061 6e64 2048 4653 5320 3344 204c 6179   and HFSS 3D Lay
+00001160: 6f75 740d 0a20 202d 2049 6365 7061 6b0d  out..  - Icepak.
+00001170: 0a20 202d 204d 6178 7765 6c6c 2032 442c  .  - Maxwell 2D,
+00001180: 204d 6178 7765 6c6c 2033 442c 2061 6e64   Maxwell 3D, and
+00001190: 2052 4d58 7072 740d 0a20 202d 2032 4420   RMXprt..  - 2D 
+000011a0: 4578 7472 6163 746f 7220 616e 6420 5133  Extractor and Q3
+000011b0: 4420 4578 7472 6163 746f 720d 0a20 202d  D Extractor..  -
+000011c0: 204d 6563 6861 6e69 6361 6c0d 0a20 202d   Mechanical..  -
+000011d0: 204e 6578 7869 6d0d 0a20 202d 2045 4442   Nexxim..  - EDB
+000011e0: 0d0a 2020 2d20 5477 696e 2042 7569 6c64  ..  - Twin Build
+000011f0: 6572 0d0a 0d0a 2323 2044 6f63 756d 656e  er....## Documen
+00001200: 7461 7469 6f6e 2061 6e64 2069 7373 7565  tation and issue
+00001210: 730d 0a0d 0a49 6e20 6164 6469 7469 6f6e  s....In addition
+00001220: 2074 6f20 696e 7374 616c 6c61 7469 6f6e   to installation
+00001230: 2061 6e64 2075 7361 6765 2069 6e66 6f72   and usage infor
+00001240: 6d61 7469 6f6e 2c20 7468 6520 6050 7941  mation, the `PyA
+00001250: 4544 5460 2064 6f63 756d 656e 7461 7469  EDT` documentati
+00001260: 6f6e 2070 726f 7669 6465 7320 5b41 5049  on provides [API
+00001270: 2072 6566 6572 656e 6365 5d28 6874 7470   reference](http
+00001280: 733a 2f2f 6165 6474 2e64 6f63 732e 7079  s://aedt.docs.py
+00001290: 616e 7379 732e 636f 6d2f 7665 7273 696f  ansys.com/versio
+000012a0: 6e2f 7374 6162 6c65 292c 205b 4578 616d  n/stable), [Exam
+000012b0: 706c 6573 5d28 6874 7470 733a 2f2f 6165  ples](https://ae
+000012c0: 6474 2e64 6f63 732e 7079 616e 7379 732e  dt.docs.pyansys.
+000012d0: 636f 6d2f 7665 7273 696f 6e2f 7374 6162  com/version/stab
+000012e0: 6c65 2f65 7861 6d70 6c65 732f 696e 6465  le/examples/inde
+000012f0: 782e 6874 6d6c 292c 2061 6e64 205b 436f  x.html), and [Co
+00001300: 6e74 7269 6275 7465 5d28 6874 7470 733a  ntribute](https:
+00001310: 2f2f 6165 6474 2e64 6f63 732e 7079 616e  //aedt.docs.pyan
+00001320: 7379 732e 636f 6d2f 7665 7273 696f 6e2f  sys.com/version/
+00001330: 7374 6162 6c65 2f43 6f6e 7472 6962 7574  stable/Contribut
+00001340: 696e 672e 6874 6d6c 2920 7365 6374 696f  ing.html) sectio
+00001350: 6e73 2e0d 0a0d 0a49 6e20 7468 6520 7570  ns.....In the up
+00001360: 7065 7220 7269 6768 7420 636f 726e 6572  per right corner
+00001370: 206f 6620 7468 6520 646f 6375 6d65 6e74   of the document
+00001380: 6174 696f 6e27 7320 7469 746c 6520 6261  ation's title ba
+00001390: 722c 2074 6865 7265 2069 7320 616e 206f  r, there is an o
+000013a0: 7074 696f 6e0d 0a66 6f72 2073 7769 7463  ption..for switc
+000013b0: 6869 6e67 2066 726f 6d20 7669 6577 696e  hing from viewin
+000013c0: 6720 7468 6520 646f 6375 6d65 6e74 6174  g the documentat
+000013d0: 696f 6e20 666f 7220 7468 6520 6c61 7465  ion for the late
+000013e0: 7374 2073 7461 626c 6520 7265 6c65 6173  st stable releas
+000013f0: 650d 0a74 6f20 7669 6577 696e 6720 7468  e..to viewing th
+00001400: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
+00001410: 666f 7220 7468 6520 6465 7665 6c6f 706d  for the developm
+00001420: 656e 7420 7665 7273 696f 6e20 6f72 2070  ent version or p
+00001430: 7265 7669 6f75 736c 790d 0a72 656c 6561  reviously..relea
+00001440: 7365 6420 7665 7273 696f 6e73 2e0d 0a0d  sed versions....
+00001450: 0a4f 6e20 7468 6520 5b50 7941 4544 5420  .On the [PyAEDT 
+00001460: 4973 7375 6573 5d28 6874 7470 733a 2f2f  Issues](https://
+00001470: 6769 7468 7562 2e63 6f6d 2f70 7961 6e73  github.com/pyans
+00001480: 7973 2f50 7941 4544 542f 6973 7375 6573  ys/PyAEDT/issues
+00001490: 2920 7061 6765 2c20 796f 7520 6361 6e0d  ) page, you can.
+000014a0: 0a63 7265 6174 6520 6973 7375 6573 2074  .create issues t
+000014b0: 6f20 7375 626d 6974 2071 7565 7374 696f  o submit questio
+000014c0: 6e73 2c20 7265 706f 7274 2062 7567 732c  ns, report bugs,
+000014d0: 2061 6e64 2072 6571 7565 7374 206e 6577   and request new
+000014e0: 2066 6561 7475 7265 732e 0d0a 0d0a 546f   features.....To
+000014f0: 2072 6561 6368 2074 6865 2070 726f 6a65   reach the proje
+00001500: 6374 2073 7570 706f 7274 2074 6561 6d2c  ct support team,
+00001510: 2065 6d61 696c 2060 7079 616e 7379 732e   email `pyansys.
+00001520: 636f 7265 4061 6e73 7973 2e63 6f6d 203c  core@ansys.com <
+00001530: 7079 616e 7379 732e 636f 7265 4061 6e73  pyansys.core@ans
+00001540: 7973 2e63 6f6d 3e60 5f2e 0d0a 0d0a 2323  ys.com>`_.....##
+00001550: 2044 6570 656e 6465 6e63 6965 730d 0a0d   Dependencies...
+00001560: 0a54 6f20 7275 6e20 6050 7941 4544 5460  .To run `PyAEDT`
+00001570: 2c20 796f 7520 6d75 7374 2068 6176 6520  , you must have 
+00001580: 6120 6c6f 6361 6c20 6c69 6365 6e63 6564  a local licenced
+00001590: 2063 6f70 7920 6f66 2041 4544 542e 0d0a   copy of AEDT...
+000015a0: 6050 7941 4544 5460 2073 7570 706f 7274  `PyAEDT` support
+000015b0: 7320 4145 4454 2076 6572 7369 6f6e 7320  s AEDT versions 
+000015c0: 3230 3232 2052 3120 6f72 206e 6577 6572  2022 R1 or newer
+000015d0: 2e0d 0a0d 0a23 2320 5374 7564 656e 7420  .....## Student 
+000015e0: 7665 7273 696f 6e0d 0a0d 0a60 5079 4145  version....`PyAE
+000015f0: 4454 6020 7375 7070 6f72 7473 2060 4145  DT` supports `AE
+00001600: 4454 2053 7475 6465 6e74 2076 6572 7369  DT Student versi
+00001610: 6f6e 2032 3032 3220 5231 6020 616e 6420  on 2022 R1` and 
+00001620: 6c61 7465 722e 2046 6f72 206d 6f72 6520  later. For more 
+00001630: 696e 666f 726d 6174 696f 6e2c 2073 6565  information, see
+00001640: 205b 5374 7564 656e 7420 5665 7273 696f   [Student Versio
+00001650: 6e20 7061 6765 5d28 6874 7470 733a 2f2f  n page](https://
+00001660: 7777 772e 616e 7379 732e 636f 6d2f 6163  www.ansys.com/ac
+00001670: 6164 656d 6963 2f73 7475 6465 6e74 732f  ademic/students/
+00001680: 616e 7379 732d 656c 6563 7472 6f6e 6963  ansys-electronic
+00001690: 732d 6465 736b 746f 702d 7374 7564 656e  s-desktop-studen
+000016a0: 7429 2e0d 0a0d 0a23 2320 5768 7920 5079  t).....## Why Py
+000016b0: 4145 4454 3f0d 0a0d 0a41 2071 7569 636b  AEDT?....A quick
+000016c0: 2061 6e64 2065 6173 7920 6170 7072 6f61   and easy approa
+000016d0: 6368 2066 6f72 2061 7574 6f6d 6174 696e  ch for automatin
+000016e0: 6720 6120 7369 6d70 6c65 206f 7065 7261  g a simple opera
+000016f0: 7469 6f6e 2069 6e20 7468 6520 4145 4454  tion in the AEDT
+00001700: 2055 4920 6973 2074 6f20 7265 636f 7264   UI is to record
+00001710: 2061 6e64 2072 6575 7365 2061 2073 6372   and reuse a scr
+00001720: 6970 742e 2048 6f77 6576 6572 2c20 6469  ipt. However, di
+00001730: 7361 6476 616e 7461 6765 7320 6f66 2074  sadvantages of t
+00001740: 6869 7320 6170 7072 6f61 6368 2061 7265  his approach are
+00001750: 3a0d 0a0d 0a20 202d 2052 6563 6f72 6465  :....  - Recorde
+00001760: 6420 636f 6465 2069 7320 6469 7274 7920  d code is dirty 
+00001770: 616e 6420 6469 6666 6963 756c 7420 746f  and difficult to
+00001780: 2072 6561 6420 616e 6420 756e 6465 7273   read and unders
+00001790: 7461 6e64 2e0d 0a20 202d 2052 6563 6f72  tand...  - Recor
+000017a0: 6465 6420 7363 7269 7074 7320 6172 6520  ded scripts are 
+000017b0: 6469 6666 6963 756c 7420 746f 2072 6575  difficult to reu
+000017c0: 7365 2061 6e64 2061 6461 7074 2e0d 0a20  se and adapt... 
+000017d0: 202d 2043 6f6d 706c 6578 2063 6f64 696e   - Complex codin
+000017e0: 6720 6973 2072 6571 7569 7265 6420 6279  g is required by
+000017f0: 206d 616e 7920 676c 6f62 616c 2075 7365   many global use
+00001800: 7273 206f 6620 6041 4544 5460 2e0d 0a0d  rs of `AEDT`....
+00001810: 0a54 6865 206d 6169 6e20 6164 7661 6e74  .The main advant
+00001820: 6167 6573 206f 6620 6050 7941 4544 5460  ages of `PyAEDT`
+00001830: 2061 7265 3a0d 0a0d 0a20 202d 2041 7574   are:....  - Aut
+00001840: 6f6d 6174 6963 2069 6e69 7469 616c 697a  omatic initializ
+00001850: 6174 696f 6e20 6f66 2061 6c6c 2060 4145  ation of all `AE
+00001860: 4454 6020 6f62 6a65 6374 732c 2073 7563  DT` objects, suc
+00001870: 6820 6173 2064 6573 6b74 6f70 206f 626a  h as desktop obj
+00001880: 6563 7473 206c 696b 6520 7468 6520 6564  ects like the ed
+00001890: 6974 6f72 2c20 626f 756e 6461 7269 6573  itor, boundaries
+000018a0: 2c20 616e 6420 736f 206f 6e0d 0a20 202d  , and so on..  -
+000018b0: 2045 7272 6f72 206d 616e 6167 656d 656e   Error managemen
+000018c0: 740d 0a20 202d 204c 6f67 206d 616e 6167  t..  - Log manag
+000018d0: 656d 656e 740d 0a20 202d 2056 6172 6961  ement..  - Varia
+000018e0: 626c 6520 6d61 6e61 6765 6d65 6e74 0d0a  ble management..
+000018f0: 2020 2d20 436f 6d70 6174 6962 696c 6974    - Compatibilit
+00001900: 7920 7769 7468 2049 726f 6e50 7974 686f  y with IronPytho
+00001910: 6e20 616e 6420 4350 7974 686f 6e0d 0a20  n and CPython.. 
+00001920: 202d 2053 696d 706c 6966 6963 6174 696f   - Simplificatio
+00001930: 6e20 6f66 2063 6f6d 706c 6578 2041 5049  n of complex API
+00001940: 2073 796e 7461 7820 7573 696e 6720 6461   syntax using da
+00001950: 7461 206f 626a 6563 7473 2077 6869 6c65  ta objects while
+00001960: 206d 6169 6e74 6169 6e69 6e67 2050 4550   maintaining PEP
+00001970: 3820 636f 6d70 6c69 616e 6365 2e0d 0a20  8 compliance... 
+00001980: 202d 2043 6f64 6520 7265 7573 6162 696c   - Code reusabil
+00001990: 6974 7920 6163 726f 7373 2064 6966 6665  ity across diffe
+000019a0: 7265 6e74 2073 6f6c 7665 7273 0d0a 2020  rent solvers..  
+000019b0: 2d20 436c 6561 7220 646f 6375 6d65 6e74  - Clear document
+000019c0: 6174 696f 6e20 6f6e 2066 756e 6374 696f  ation on functio
+000019d0: 6e73 2061 6e64 2041 5049 0d0a 2020 2d20  ns and API..  - 
+000019e0: 556e 6974 2074 6573 7473 206f 6620 636f  Unit tests of co
+000019f0: 6465 2074 6f20 696e 6372 6561 7365 2071  de to increase q
+00001a00: 7561 6c69 7479 2061 6372 6f73 7320 6469  uality across di
+00001a10: 6666 6572 656e 7420 4145 4454 2076 6572  fferent AEDT ver
+00001a20: 7369 6f6e 730d 0a0d 0a23 2320 4578 616d  sions....## Exam
+00001a30: 706c 6520 776f 726b 666c 6f77 0d0a 0d0a  ple workflow....
+00001a40: 2031 2e20 496e 6974 6961 6c69 7a65 2074   1. Initialize t
+00001a50: 6865 2060 6044 6573 6b74 6f70 6060 2063  he ``Desktop`` c
+00001a60: 6c61 7373 2077 6974 6820 7468 6520 7665  lass with the ve
+00001a70: 7273 696f 6e20 6f66 2060 4145 4454 6020  rsion of `AEDT` 
+00001a80: 746f 2075 7365 2e0d 0a20 322e 2049 6e69  to use... 2. Ini
+00001a90: 7469 616c 697a 6520 7468 6520 6170 706c  tialize the appl
+00001aa0: 6963 6174 696f 6e20 746f 2075 7365 2077  ication to use w
+00001ab0: 6974 6869 6e20 6041 4544 5460 2e0d 0a0d  ithin `AEDT`....
+00001ac0: 0a23 2320 436f 6e6e 6563 7420 746f 2041  .## Connect to A
+00001ad0: 4544 5420 6672 6f6d 2050 7974 686f 6e20  EDT from Python 
+00001ae0: 4944 450d 0a0d 0a60 6050 7941 4544 5460  IDE....``PyAEDT`
+00001af0: 6020 776f 726b 7320 626f 7468 2069 6e73  ` works both ins
+00001b00: 6964 6520 4145 4454 2061 6e64 2061 7320  ide AEDT and as 
+00001b10: 6120 7374 616e 6461 6c6f 6e65 2061 7070  a standalone app
+00001b20: 6c69 6361 7469 6f6e 2e20 5468 6973 2050  lication. This P
+00001b30: 7974 686f 6e20 6c69 6272 6172 7920 6175  ython library au
+00001b40: 746f 6d61 7469 6361 6c6c 7920 6465 7465  tomatically dete
+00001b50: 6374 7320 7768 6574 6865 7220 6974 2069  cts whether it i
+00001b60: 7320 7275 6e6e 696e 6720 696e 2061 6e20  s running in an 
+00001b70: 4972 6f6e 5079 7468 6f6e 206f 7220 4350  IronPython or CP
+00001b80: 7974 686f 6e20 656e 7669 726f 6e6d 656e  ython environmen
+00001b90: 7420 616e 6420 696e 6974 6961 6c69 7a65  t and initialize
+00001ba0: 7320 4145 4454 2061 6363 6f72 6469 6e67  s AEDT according
+00001bb0: 6c79 2e0d 0a60 6050 7941 4544 5460 6020  ly...``PyAEDT`` 
+00001bc0: 616c 736f 2070 726f 7669 6465 7320 6164  also provides ad
+00001bd0: 7661 6e63 6564 2065 7272 6f72 206d 616e  vanced error man
+00001be0: 6167 656d 656e 742e 2055 7361 6765 2065  agement. Usage e
+00001bf0: 7861 6d70 6c65 7320 666f 6c6c 6f77 2e0d  xamples follow..
+00001c00: 0a0d 0a23 2320 4578 706c 6963 6974 2041  ...## Explicit A
+00001c10: 4544 5420 6465 636c 6172 6174 696f 6e20  EDT declaration 
+00001c20: 616e 6420 6572 726f 7220 6d61 6e61 6765  and error manage
+00001c30: 6d65 6e74 0d0a 0d0a 6060 6020 7079 7468  ment....``` pyth
+00001c40: 6f6e 0d0a 2020 2020 2320 4c61 756e 6368  on..    # Launch
+00001c50: 2041 4544 5420 3230 3232 2052 3220 696e   AEDT 2022 R2 in
+00001c60: 206e 6f6e 2d67 7261 7068 6963 616c 206d   non-graphical m
+00001c70: 6f64 650d 0a0d 0a20 2020 2066 726f 6d20  ode....    from 
+00001c80: 7079 6165 6474 2069 6d70 6f72 7420 4465  pyaedt import De
+00001c90: 736b 746f 702c 2043 6972 6375 6974 0d0a  sktop, Circuit..
+00001ca0: 2020 2020 7769 7468 2044 6573 6b74 6f70      with Desktop
+00001cb0: 2873 7065 6369 6669 6564 5f76 6572 7369  (specified_versi
+00001cc0: 6f6e 3d22 3230 3232 2e32 222c 0d0a 2020  on="2022.2",..  
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00001ce0: 6f6e 5f67 7261 7068 6963 616c 3d46 616c  on_graphical=Fal
+00001cf0: 7365 2c20 6e65 775f 6465 736b 746f 705f  se, new_desktop_
+00001d00: 7365 7373 696f 6e3d 5472 7565 2c0d 0a20  session=True,.. 
+00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d20: 636c 6f73 655f 6f6e 5f65 7869 743d 5472  close_on_exit=Tr
+00001d30: 7565 2c20 7374 7564 656e 745f 7665 7273  ue, student_vers
+00001d40: 696f 6e3d 4661 6c73 6529 3a0d 0a20 2020  ion=False):..   
+00001d50: 2020 2020 2063 6972 6375 6974 203d 2043       circuit = C
+00001d60: 6972 6375 6974 2829 0d0a 2020 2020 2020  ircuit()..      
+00001d70: 2020 2e2e 2e0d 0a20 2020 2020 2020 2023    .....        #
+00001d80: 2041 6e79 2065 7272 6f72 2068 6572 6520   Any error here 
+00001d90: 7769 6c6c 2062 6520 6361 7567 6874 2062  will be caught b
+00001da0: 7920 4465 736b 746f 702e 0d0a 2020 2020  y Desktop...    
+00001db0: 2020 2020 2e2e 2e0d 0a0d 0a20 2020 2023      .......    #
+00001dc0: 2044 6573 6b74 6f70 2069 7320 6175 746f   Desktop is auto
+00001dd0: 6d61 7469 6361 6c6c 7920 7265 6c65 6173  matically releas
+00001de0: 6564 2068 6572 652e 0d0a 6060 600d 0a0d  ed here...```...
+00001df0: 0a23 2320 496d 706c 6963 6974 2041 4544  .## Implicit AED
+00001e00: 5420 6465 636c 6172 6174 696f 6e20 616e  T declaration an
+00001e10: 6420 6572 726f 7220 6d61 6e61 6765 6d65  d error manageme
+00001e20: 6e74 0d0a 0d0a 6060 6020 7079 7468 6f6e  nt....``` python
+00001e30: 0d0a 2020 2020 2320 4c61 756e 6368 2074  ..    # Launch t
+00001e40: 6865 206c 6174 6573 7420 696e 7374 616c  he latest instal
+00001e50: 6c65 6420 7665 7273 696f 6e20 6f66 2041  led version of A
+00001e60: 4544 5420 696e 2067 7261 7068 6963 616c  EDT in graphical
+00001e70: 206d 6f64 650d 0a0d 0a20 2020 2066 726f   mode....    fro
+00001e80: 6d20 7079 6165 6474 2069 6d70 6f72 7420  m pyaedt import 
+00001e90: 4369 7263 7569 740d 0a20 2020 2077 6974  Circuit..    wit
+00001ea0: 6820 4369 7263 7569 7428 7370 6563 6966  h Circuit(specif
+00001eb0: 6965 645f 7665 7273 696f 6e3d 2232 3032  ied_version="202
+00001ec0: 322e 3222 2c0d 0a20 2020 2020 2020 2020  2.2",..         
+00001ed0: 2020 2020 2020 2020 6e6f 6e5f 6772 6170          non_grap
+00001ee0: 6869 6361 6c3d 4661 6c73 6529 2061 7320  hical=False) as 
+00001ef0: 6369 7263 7569 743a 0d0a 2020 2020 2020  circuit:..      
+00001f00: 2020 2e2e 2e0d 0a20 2020 2020 2020 2023    .....        #
+00001f10: 2041 6e79 2065 7272 6f72 2068 6572 6520   Any error here 
+00001f20: 7769 6c6c 2062 6520 6361 7567 6874 2062  will be caught b
+00001f30: 7920 4465 736b 746f 702e 0d0a 2020 2020  y Desktop...    
+00001f40: 2020 2020 2e2e 2e0d 0a0d 0a20 2020 2023      .......    #
+00001f50: 2044 6573 6b74 6f70 2069 7320 6175 746f   Desktop is auto
+00001f60: 6d61 7469 6361 6c6c 7920 7265 6c65 6173  matically releas
+00001f70: 6564 2068 6572 652e 0d0a 6060 600d 0a0d  ed here...```...
+00001f80: 0a23 2320 5265 6d6f 7465 2061 7070 6c69  .## Remote appli
+00001f90: 6361 7469 6f6e 2063 616c 6c0d 0a0d 0a59  cation call....Y
+00001fa0: 6f75 2063 616e 206d 616b 6520 6120 7265  ou can make a re
+00001fb0: 6d6f 7465 2061 7070 6c69 6361 7469 6f6e  mote application
+00001fc0: 2063 616c 6c20 6f6e 2061 2043 5079 7468   call on a CPyth
+00001fd0: 6f6e 2073 6572 7665 720d 0a6f 7220 616e  on server..or an
+00001fe0: 7920 5769 6e64 6f77 7320 636c 6965 6e74  y Windows client
+00001ff0: 206d 6163 6869 6e65 2e0d 0a0d 0a4f 6e20   machine.....On 
+00002000: 6120 4350 7974 686f 6e20 5365 7276 6572  a CPython Server
+00002010: 3a0d 0a0d 0a60 6060 2070 7974 686f 6e0d  :....``` python.
+00002020: 0a20 2020 2023 204c 6175 6e63 6820 5079  .    # Launch Py
+00002030: 4145 4454 2072 656d 6f74 6520 7365 7276  AEDT remote serv
+00002040: 6572 206f 6e20 4350 7974 686f 6e0d 0a0d  er on CPython...
+00002050: 0a20 2020 2066 726f 6d20 7079 6165 6474  .    from pyaedt
+00002060: 2e63 6f6d 6d6f 6e5f 7270 6320 696d 706f  .common_rpc impo
+00002070: 7274 2070 7961 6564 745f 7365 7276 6963  rt pyaedt_servic
+00002080: 655f 6d61 6e61 6765 720d 0a20 2020 2070  e_manager..    p
+00002090: 7961 6564 745f 7365 7276 6963 655f 6d61  yaedt_service_ma
+000020a0: 6e61 6765 7228 290d 0a60 6060 0d0a 0d0a  nager()..```....
+000020b0: 4f6e 2061 6e79 2057 696e 646f 7773 2063  On any Windows c
+000020c0: 6c69 656e 7420 6d61 6368 696e 653a 0d0a  lient machine:..
+000020d0: 0d0a 6060 6020 7079 7468 6f6e 0d0a 2020  ..``` python..  
+000020e0: 2020 6672 6f6d 2070 7961 6564 742e 636f    from pyaedt.co
+000020f0: 6d6d 6f6e 5f72 7063 2069 6d70 6f72 7420  mmon_rpc import 
+00002100: 6372 6561 7465 5f73 6573 7369 6f6e 0d0a  create_session..
+00002110: 2020 2020 636c 3120 3d20 6372 6561 7465      cl1 = create
+00002120: 5f73 6573 7369 6f6e 2822 7365 7276 6572  _session("server
+00002130: 5f6e 616d 6522 290d 0a20 2020 2063 6c31  _name")..    cl1
+00002140: 2e61 6564 7428 706f 7274 3d35 3030 3030  .aedt(port=50000
+00002150: 2c20 6e6f 6e5f 6772 6170 6869 6361 6c3d  , non_graphical=
+00002160: 4661 6c73 6529 0d0a 2020 2020 6866 7373  False)..    hfss
+00002170: 203d 2048 6673 7328 6d61 6368 696e 653d   = Hfss(machine=
+00002180: 2273 6572 7665 725f 6e61 6d65 222c 2070  "server_name", p
+00002190: 6f72 743d 3530 3030 3029 0d0a 2020 2020  ort=50000)..    
+000021a0: 2320 796f 7572 2063 6f64 6520 6865 7265  # your code here
+000021b0: 0d0a 6060 600d 0a0d 0a23 2320 5661 7269  ..```....## Vari
+000021c0: 6162 6c65 730d 0a0d 0a60 6060 2070 7974  ables....``` pyt
+000021d0: 686f 6e0d 0a20 2020 2066 726f 6d20 7079  hon..    from py
+000021e0: 6165 6474 2e48 4653 5320 696d 706f 7274  aedt.HFSS import
+000021f0: 2048 4653 530d 0a20 2020 2077 6974 6820   HFSS..    with 
+00002200: 4846 5353 2061 7320 6866 7373 3a0d 0a20  HFSS as hfss:.. 
+00002210: 2020 2020 2020 2020 6866 7373 5b22 6469          hfss["di
+00002220: 6d22 5d20 3d20 2231 6d6d 2220 2020 2320  m"] = "1mm"   # 
+00002230: 6465 7369 676e 2076 6172 6961 626c 650d  design variable.
+00002240: 0a20 2020 2020 2020 2020 6866 7373 5b22  .         hfss["
+00002250: 2464 696d 225d 203d 2022 316d 6d22 2020  $dim"] = "1mm"  
+00002260: 2320 7072 6f6a 6563 7420 7661 7269 6162  # project variab
+00002270: 6c65 0d0a 6060 600d 0a0d 0a23 2320 4d6f  le..```....## Mo
+00002280: 6465 6c65 720d 0a0d 0a60 6060 2070 7974  deler....``` pyt
+00002290: 686f 6e0d 0a20 2020 2023 2043 7265 6174  hon..    # Creat
+000022a0: 6520 6120 626f 782c 2061 7373 6967 6e20  e a box, assign 
+000022b0: 7661 7269 6162 6c65 732c 2061 6e64 2061  variables, and a
+000022c0: 7373 6967 6e20 6d61 7465 7269 616c 732e  ssign materials.
+000022d0: 0d0a 0d0a 2020 2020 6672 6f6d 2070 7961  ....    from pya
+000022e0: 6564 742e 6866 7373 2069 6d70 6f72 7420  edt.hfss import 
+000022f0: 4866 7373 0d0a 2020 2020 7769 7468 2048  Hfss..    with H
+00002300: 6673 7320 6173 2068 6673 733a 0d0a 2020  fss as hfss:..  
+00002310: 2020 2020 2020 2068 6673 732e 6d6f 6465         hfss.mode
+00002320: 6c65 722e 6372 6561 7465 5f62 6f78 285b  ler.create_box([
+00002330: 302c 2030 2c20 305d 2c20 5b31 302c 2022  0, 0, 0], [10, "
+00002340: 6469 6d22 2c20 3130 5d2c 0d0a 2020 2020  dim", 10],..    
+00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002360: 2020 2020 2020 2020 2020 2020 2022 6d79               "my
+00002370: 626f 7822 2c20 2261 6c75 6d69 6e75 6d22  box", "aluminum"
+00002380: 290d 0a60 6060 0d0a 0d0a 2323 204c 6963  )..```....## Lic
+00002390: 656e 7365 0d0a 0d0a 6050 7941 4544 5460  ense....`PyAEDT`
+000023a0: 2069 7320 6c69 6365 6e73 6564 2075 6e64   is licensed und
+000023b0: 6572 2074 6865 2060 4d49 5460 206c 6963  er the `MIT` lic
+000023c0: 656e 7365 2e0d 0a0d 0a54 6869 7320 6d6f  ense.....This mo
+000023d0: 6475 6c65 206d 616b 6573 206e 6f20 636f  dule makes no co
+000023e0: 6d6d 6572 6369 616c 2063 6c61 696d 206f  mmercial claim o
+000023f0: 7665 7220 416e 7379 7320 7768 6174 736f  ver Ansys whatso
+00002400: 6576 6572 2e20 6050 7941 4544 5460 2065  ever. `PyAEDT` e
+00002410: 7874 656e 6473 2074 6865 2066 756e 6374  xtends the funct
+00002420: 696f 6e61 6c69 7479 206f 6620 6041 4544  ionality of `AED
+00002430: 5460 2062 7920 6164 6469 6e67 2061 6e20  T` by adding an 
+00002440: 6164 6469 7469 6f6e 616c 2050 7974 686f  additional Pytho
+00002450: 6e20 696e 7465 7266 6163 6520 746f 2060  n interface to `
+00002460: 4145 4454 6020 7769 7468 6f75 7420 6368  AEDT` without ch
+00002470: 616e 6769 6e67 2074 6865 2063 6f72 6520  anging the core 
+00002480: 6265 6861 7669 6f72 206f 7220 6c69 6365  behavior or lice
+00002490: 6e73 6520 6f66 2074 6865 206f 7269 6769  nse of the origi
+000024a0: 6e61 6c20 736f 6674 7761 7265 2e20 5468  nal software. Th
+000024b0: 6520 7573 6520 6f66 2074 6865 2069 6e74  e use of the int
+000024c0: 6572 6163 7469 7665 2063 6f6e 7472 6f6c  eractive control
+000024d0: 206f 6620 6050 7941 4544 5460 2072 6571   of `PyAEDT` req
+000024e0: 7569 7265 7320 6120 6c65 6761 6c6c 7920  uires a legally 
+000024f0: 6c69 6365 6e73 6564 206c 6f63 616c 2063  licensed local c
+00002500: 6f70 7920 6f66 2060 4145 4454 602e 2046  opy of `AEDT`. F
+00002510: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+00002520: 696f 6e20 6162 6f75 7420 6041 4544 5460  ion about `AEDT`
+00002530: 2c20 7669 7369 7420 7468 6520 5b41 4544  , visit the [AED
+00002540: 5420 7061 6765 5d28 6874 7470 733a 2f2f  T page](https://
+00002550: 7777 772e 616e 7379 732e 636f 6d2f 7072  www.ansys.com/pr
+00002560: 6f64 7563 7473 2f65 6c65 6374 726f 6e69  oducts/electroni
+00002570: 6373 2920 6f6e 2074 6865 2060 416e 7379  cs) on the `Ansy
+00002580: 7360 2077 6562 7369 7465 2e0d 0a0d 0a3c  s` website.....<
+00002590: 7020 7374 796c 653d 2274 6578 742d 616c  p style="text-al
+000025a0: 6967 6e3a 2072 6967 6874 3b22 3e20 3c61  ign: right;"> <a
+000025b0: 2068 7265 663d 2223 7265 6164 6d65 2d74   href="#readme-t
+000025c0: 6f70 223e 6261 636b 2074 6f20 746f 703c  op">back to top<
+000025d0: 2f61 3e20 3c2f 703e 0d0a 0d0a 2323 2049  /a> </p>....## I
+000025e0: 6e64 6963 6573 2061 6e64 2074 6162 6c65  ndices and table
+000025f0: 730d 0a0d 0a2d 2020 5b49 6e64 6578 5d28  s....-  [Index](
+00002600: 6874 7470 733a 2f2f 6165 6474 2e64 6f63  https://aedt.doc
+00002610: 732e 7079 616e 7379 732e 636f 6d2f 7665  s.pyansys.com/ve
+00002620: 7273 696f 6e2f 7374 6162 6c65 2f67 656e  rsion/stable/gen
+00002630: 696e 6465 782e 6874 6d6c 290d 0a2d 2020  index.html)..-  
+00002640: 5b4d 6f64 756c 6520 496e 6465 785d 2868  [Module Index](h
+00002650: 7474 7073 3a2f 2f61 6564 742e 646f 6373  ttps://aedt.docs
+00002660: 2e70 7961 6e73 7973 2e63 6f6d 2f76 6572  .pyansys.com/ver
+00002670: 7369 6f6e 2f73 7461 626c 652f 7079 2d6d  sion/stable/py-m
+00002680: 6f64 696e 6465 782e 6874 6d6c 290d 0a2d  odindex.html)..-
+00002690: 2020 5b53 6561 7263 6820 5061 6765 5d28    [Search Page](
+000026a0: 6874 7470 733a 2f2f 6165 6474 2e64 6f63  https://aedt.doc
+000026b0: 732e 7079 616e 7379 732e 636f 6d2f 7665  s.pyansys.com/ve
+000026c0: 7273 696f 6e2f 7374 6162 6c65 2f73 6561  rsion/stable/sea
+000026d0: 7263 682e 6874 6d6c 290d 0a              rch.html)..
```

### Comparing `pyaedt-0.6.73/pyaedt/__init__.py` & `pyaedt-0.6.74/pyaedt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 if os.name == "nt":
     os.environ["PYTHONMALLOC"] = "malloc"
 os.environ["ANS_MESHER_PROC_DUMP_PREPOST_BEND_SM3"] = "1"
 os.environ["ANSYSEM_FEATURE_SF6694_NON_GRAPHICAL_COMMAND_EXECUTION_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE"] = "1"
+os.environ["ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE"] = "1"
 
 pyaedt_path = os.path.dirname(__file__)
 
-__version__ = "0.6.73"
+__version__ = "0.6.74"
 
 version = __version__
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
 import pyaedt.generic.general_methods as general_methods
 from pyaedt.generic.general_methods import _pythonver
@@ -23,14 +24,15 @@
 from pyaedt.generic.general_methods import generate_unique_folder_name
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import generate_unique_project_name
 from pyaedt.generic.general_methods import inside_desktop
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
 from pyaedt.generic.general_methods import is_windows
+from pyaedt.generic.general_methods import online_help
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import settings
 
 from pyaedt.aedt_logger import pyaedt_logger  # isort:skip
 
 try:
     from pyaedt.generic.design_types import Hfss3dLayout
```

### Comparing `pyaedt-0.6.73/pyaedt/aedt_logger.py` & `pyaedt-0.6.74/pyaedt/aedt_logger.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.6.74/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/application/Analysis.py` & `pyaedt-0.6.74/pyaedt/application/Analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1654,15 +1654,26 @@
                 target_name = os.path.join(tempfile.gettempdir(), generate_unique_name("config") + ".acf")
             else:
                 target_name = (
                     os.path.join(self.working_directory, config_name + ".acf").replace("\\", "/")
                     if self.working_directory[0] != "\\"
                     else os.path.join(self.working_directory, config_name + ".acf")
                 )
-            shutil.copy2(source_name, target_name)
+            try:
+                shutil.copy2(source_name, target_name)
+
+            # If source and destination are same
+            except shutil.SameFileError:
+                self.logger.warning("Source and destination represents the same file.")
+            # If there is any permission issue
+            except PermissionError:
+                self.logger.error("Permission denied.")
+            # For other errors
+            except:
+                self.logger.error("Error occurred while copying file.")
 
             if num_cores:
                 update_hpc_option(target_name, "NumCores", num_cores, False)
             if num_gpu:
                 update_hpc_option(target_name, "NumGPUs", num_gpu, False)
             if num_tasks:
                 update_hpc_option(target_name, "NumEngines", num_tasks, False)
```

### Comparing `pyaedt-0.6.73/pyaedt/application/Analysis3D.py` & `pyaedt-0.6.74/pyaedt/application/Analysis3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.6.74/pyaedt/application/Analysis3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.6.74/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.6.74/pyaedt/application/AnalysisNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.6.74/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.6.74/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/application/Design.py` & `pyaedt-0.6.74/pyaedt/application/Design.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/application/JobManager.py` & `pyaedt-0.6.74/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/application/Variables.py` & `pyaedt-0.6.74/pyaedt/application/Variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/application/aedt_objects.py` & `pyaedt-0.6.74/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/application/design_solutions.py` & `pyaedt-0.6.74/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/circuit.py` & `pyaedt-0.6.74/pyaedt/circuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/common_rpc.py` & `pyaedt-0.6.74/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/desktop.py` & `pyaedt-0.6.74/pyaedt/desktop.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,15 @@
                         elif session[0] == aedt_process_id:
                             settings.use_grpc_api = False
                             break
 
             if version_key < "2022.2":
                 settings.use_grpc_api = False
             elif (
-                version_key == "2022.2"
+                version_key.startswith("2022.2")
                 and not self.port
                 and not self.machine
                 and settings.use_grpc_api is None
                 and _com != "gprc_v3"
             ):
                 settings.use_grpc_api = False
             elif settings.use_grpc_api is None or _com == "gprc_v3":
```

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/AnsysReport.deps.json` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/AnsysReport.deps.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/AnsysReport.dll` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/AnsysReport.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/AnsysTemplate.json` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/Images/Ansys.png` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/Images/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/PdfSharpCore.dll` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/PdfSharpCore.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/System.Runtime.dll` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/System.Runtime.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/System.Runtime.xml` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/System.Runtime.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml` & `pyaedt-0.6.74/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/downloads.py` & `pyaedt-0.6.74/pyaedt/downloads.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb.py` & `pyaedt-0.6.74/pyaedt/edb.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/components.py` & `pyaedt-0.6.74/pyaedt/edb_core/components.py`

 * *Files 3% similar despite different names*

```diff
@@ -727,14 +727,94 @@
                     r_value=source.r_value,
                     l_value=source.l_value,
                     c_value=source.c_value,
                 )
         return True
 
     @pyaedt_function_handler()
+    def create_port_on_pins(self, refdes, pins, reference_pins, impedance=50.0):
+        """Create circuit port between pins and reference ones.
+
+        Parameters
+        ----------
+        refdes : Component reference designator
+            str or EDBComponent object.
+        pins : pin name where the terminal has to be created. Single pin or several ones can be provided.If several
+        pins are provided a pin group will is created. Pin names can be the EDB name or the EDBPadstackInstance one.
+        For instance the pin called ``Pin1`` located on component ``U1``, ``U1-Pin1`` or ``Pin1`` can be provided and
+        will be handled.
+            str, [str], EDBPadstackInstance, [EDBPadstackInstance]
+        reference_pins : reference pin name used for terminal reference. Single pin or several ones can be provided.
+        If several pins are provided a pin group will is created. Pin names can be the EDB name or the
+        EDBPadstackInstance one. For instance the pin called ``Pin1`` located on component ``U1``, ``U1-Pin1``
+        or ``Pin1`` can be provided and will be handled.
+            str, [str], EDBPadstackInstance, [EDBPadstackInstance]
+        impedance : Port impedance
+            str, float
+
+        Returns
+        -------
+        EDB terminal created, or False if failed to create.
+
+        Example:
+        >>> from pyaedt import Edb
+        >>> edb = Edb(path_to_edb_file)
+        >>> pin = "AJ6"
+        >>> ref_pins = ["AM7", "AM4"]
+        Or to take all reference pins
+        >>> ref_pins = [pin for pin in list(edb.components["U2A5"].pins.values()) if pin.net_name == "GND"]
+        >>> edb.components.create_port_on_pins(refdes="U2A5", pins=pin, reference_pins=ref_pins)
+        >>> edb.save_edb()
+        >>> edb.close_edb()
+        """
+
+        if isinstance(pins, str) or isinstance(pins, EDBPadstackInstance):
+            pins = [pins]
+        if isinstance(reference_pins, str):
+            reference_pins = [reference_pins]
+        if isinstance(refdes, str) or isinstance(refdes, EDBComponent):
+            refdes = self.instances[refdes]
+        if len([pin for pin in pins if isinstance(pin, str)]) == len(pins):
+            cmp_pins = []
+            for pin_name in pins:
+                cmp_pin = [pin for pin in list(refdes.pins.values()) if pin_name in pin.name]
+                if cmp_pin:
+                    cmp_pins.append(cmp_pin[0])
+            if not cmp_pins:
+                return
+            pins = cmp_pins
+        if not len([pin for pin in pins if isinstance(pin, EDBPadstackInstance)]) == len(pins):
+            self._logger.error("Pin list must contain only pins instances")
+            return
+        if len([pin for pin in reference_pins if isinstance(pin, str)]) == len(reference_pins):
+            ref_cmp_pins = []
+            for ref_pin_name in reference_pins:
+                cmp_ref_pin = [pin for pin in list(refdes.pins.values()) if ref_pin_name in pin.name]
+                if cmp_ref_pin:
+                    ref_cmp_pins.append(cmp_ref_pin[0])
+            if not ref_cmp_pins:
+                return
+            reference_pins = ref_cmp_pins
+        if not len([pin for pin in reference_pins if isinstance(pin, EDBPadstackInstance)]) == len(reference_pins):
+            return
+        group_name = "group_{}_{}".format(pins[0].net_name, pins[0].name)
+        ref_group_name = "group_{}_{}_ref".format(pins[0].net_name, pins[0].name)
+        pin_group = self.create_pingroup_from_pins(pins, group_name)
+        ref_pin_group = self.create_pingroup_from_pins(reference_pins, ref_group_name)
+        term = self._create_pin_group_terminal(pingroup=pin_group, component=refdes.refdes)
+        term.SetIsCircuitPort(True)
+        ref_term = self._create_pin_group_terminal(pingroup=ref_pin_group, component=refdes.refdes)
+        ref_term.SetIsCircuitPort(True)
+        term.SetImpedance(self._edb.Utility.Value(impedance))
+        term.SetReferenceTerminal(ref_term)
+        if term:
+            return term
+        return False
+
+    @pyaedt_function_handler()
     def create_port_on_component(
         self,
         component,
         net_list,
         port_type=SourceType.CoaxPort,
         do_pingroup=True,
         reference_net="gnd",
@@ -796,16 +876,21 @@
             self._logger.info(
                 "No pins found on component {}, searching padstack instances instead".format(component.GetName())
             )
             return False
         pin_layers = cmp_pins[0].GetPadstackDef().GetData().GetLayerNames()
         if port_type == SourceType.CoaxPort:
             pad_params = self._padstack.get_pad_parameters(pin=cmp_pins[0], layername=pin_layers[0], pad_type=0)
-            sball_diam = min([self._pedb.edb_value(val).ToDouble() for val in pad_params[1]])
-            solder_ball_height = sball_diam
+            if not pad_params[0] == 7:
+                sball_diam = min([self._pedb.edb_value(val).ToDouble() for val in pad_params[1]])
+                solder_ball_height = sball_diam / 2
+            else:
+                bbox = pad_params[1]
+                sball_diam = min([abs(bbox[2] - bbox[0]), abs(bbox[3] - bbox[1])]) * 0.8
+                solder_ball_height = sball_diam / 2
             self.set_solder_ball(component, solder_ball_height, sball_diam)
             for pin in cmp_pins:
                 self._padstack.create_coax_port(pin)
 
         elif port_type == SourceType.CircPort:  # pragma no cover
             ref_pins = [
                 p
@@ -1386,15 +1471,15 @@
     @pyaedt_function_handler()
     def create_pingroup_from_pins(self, pins, group_name=None):
         """Create a pin group on a component.
 
         Parameters
         ----------
         pins : list
-            List of EDB core pins.
+            List of EDB pins.
         group_name : str, optional
             Name for the group. The default is ``None``, in which case
             a default name is assigned as follows: ``[component Name] [NetName]``.
 
         Returns
         -------
         tuple
@@ -1406,16 +1491,24 @@
         >>> edbapp = Edb("myaedbfolder")
         >>> edbapp.components.create_pingroup_from_pins(gndpinlist, "MyGNDPingroup")
 
         """
         if len(pins) < 1:
             self._logger.error("No pins specified for pin group %s", group_name)
             return (False, None)
+        if len([pin for pin in pins if isinstance(pin, EDBPadstackInstance)]):
+            _pins = [pin._edb_padstackinstance for pin in pins]
+            if _pins:
+                pins = _pins
         if group_name is None:
             group_name = self._edb.Cell.Hierarchy.PinGroup.GetUniqueName(self._active_layout)
+        for pin in pins:
+            pin.SetIsLayoutPin(True)
+        forbiden_car = "-><"
+        group_name = group_name.translate({ord(i): "_" for i in forbiden_car})
         pingroup = _retry_ntimes(
             10,
             self._edb.Cell.Hierarchy.PinGroup.Create,
             self._active_layout,
             group_name,
             convert_py_list_to_net_list(pins),
         )
```

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/edb_data/components_data.py` & `pyaedt-0.6.74/pyaedt/edb_core/edb_data/components_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/edb_data/design_options.py` & `pyaedt-0.6.74/pyaedt/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/edb_data/edbvalue.py` & `pyaedt-0.6.74/pyaedt/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/edb_data/hfss_extent_info.py` & `pyaedt-0.6.74/pyaedt/edb_core/edb_data/hfss_extent_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     @property
     def air_box_positive_vertical_extent(self):
         """Negative vertical extent for the air box."""
         return self._edb_hfss_extent_info.AirBoxPositiveVerticalExtent.Item1
 
     @air_box_positive_vertical_extent.setter
     def air_box_positive_vertical_extent(self, value):
+        value = float(value)
         info = self._edb_hfss_extent_info
         info.AirBoxPositiveVerticalExtent = convert_pytuple_to_nettuple(
             (value, self.air_box_positive_vertical_extent_enabled)
         )
         self._update_hfss_extent_info(info)
 
     @property
@@ -104,14 +105,15 @@
     @property
     def air_box_negative_vertical_extent(self):
         """Negative vertical extent for the airbox."""
         return self._edb_hfss_extent_info.AirBoxNegativeVerticalExtent.Item1
 
     @air_box_negative_vertical_extent.setter
     def air_box_negative_vertical_extent(self, value):
+        value = float(value)
         info = self._edb_hfss_extent_info
         info.AirBoxNegativeVerticalExtent = convert_pytuple_to_nettuple(
             (value, self.air_box_negative_vertical_extent_enabled)
         )
         self._update_hfss_extent_info(info)
 
     @property
```

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyaedt-0.6.74/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/edb_data/layer_data.py` & `pyaedt-0.6.74/pyaedt/edb_core/edb_data/layer_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/edb_data/nets_data.py` & `pyaedt-0.6.74/pyaedt/edb_core/edb_data/nets_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/edb_data/padstacks_data.py` & `pyaedt-0.6.74/pyaedt/edb_core/edb_data/padstacks_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/edb_data/primitives_data.py` & `pyaedt-0.6.74/pyaedt/edb_core/edb_data/primitives_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/edb_data/simulation_configuration.py` & `pyaedt-0.6.74/pyaedt/edb_core/edb_data/simulation_configuration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyaedt-0.6.74/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/edb_data/sources.py` & `pyaedt-0.6.74/pyaedt/edb_core/edb_data/sources.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/edb_data/utilities.py` & `pyaedt-0.6.74/pyaedt/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/edb_data/variables.py` & `pyaedt-0.6.74/pyaedt/edb_core/edb_data/variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/general.py` & `pyaedt-0.6.74/pyaedt/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/hfss.py` & `pyaedt-0.6.74/pyaedt/edb_core/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/bom/bom.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/bom/bom_item.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/bom/characteristics.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/bom/refdes.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/color.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/content.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/dictionary_color.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/dictionary_fill.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/dictionary_line.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/entry_line.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/fill.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,32 +124,34 @@
                 package.height = ""
                 package.type = component.type
                 pin_number = 0
                 for _, pin in component.pins.items():
                     geometry_type, pad_parameters, pos_x, pos_y, rot = self._pedb.padstacks.get_pad_parameters(
                         pin._edb_padstackinstance, component.placement_layer, 0
                     )
-                    position = pin._position if pin._position else pin.position
-
-                    pin_pos_x = self._ipc.from_meter_to_units(position[0], self.units)
-                    pin_pos_y = self._ipc.from_meter_to_units(position[1], self.units)
-                    primitive_ref = ""
-                    if geometry_type == 1:
-                        primitive_ref = "CIRC_{}".format(pad_parameters[0])
-                    elif geometry_type == 2:
-                        primitive_ref = "RECT_{}_{}".format(pad_parameters[0], pad_parameters[0])
-                    elif geometry_type == 3:
-                        primitive_ref = "RECT_{}_{}".format(pad_parameters[0], pad_parameters[1])
-                    elif geometry_type == 4:
-                        primitive_ref = "OVAL_{}_{}_{}".format(pad_parameters[0], pad_parameters[1], pad_parameters[2])
-                    if primitive_ref:
-                        package.add_pin(
-                            number=pin_number, x=pin_pos_x, y=pin_pos_y, rotation=rot, primitive_ref=primitive_ref
-                        )
-                    pin_number += 1
+                    if pad_parameters:
+                        position = pin._position if pin._position else pin.position
+                        pin_pos_x = self._ipc.from_meter_to_units(position[0], self.units)
+                        pin_pos_y = self._ipc.from_meter_to_units(position[1], self.units)
+                        primitive_ref = ""
+                        if geometry_type == 1:
+                            primitive_ref = "CIRC_{}".format(pad_parameters[0])
+                        elif geometry_type == 2:
+                            primitive_ref = "RECT_{}_{}".format(pad_parameters[0], pad_parameters[0])
+                        elif geometry_type == 3:
+                            primitive_ref = "RECT_{}_{}".format(pad_parameters[0], pad_parameters[1])
+                        elif geometry_type == 4:
+                            primitive_ref = "OVAL_{}_{}_{}".format(
+                                pad_parameters[0], pad_parameters[1], pad_parameters[2]
+                            )
+                        if primitive_ref:
+                            package.add_pin(
+                                number=pin_number, x=pin_pos_x, y=pin_pos_y, rotation=rot, primitive_ref=primitive_ref
+                            )
+                        pin_number += 1
                 self.packages[package.name] = package
             ipc_component = Component()
             ipc_component.type = component.type
             try:
                 ipc_component.value = component.value
             except:
                 pass
```

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/cad_header.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/ecad.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ecad/spec.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/history_record.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/ipc2581.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/ipc2581/logistic_header.py` & `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/layout.py` & `pyaedt-0.6.74/pyaedt/edb_core/layout.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module contains these classes: `EdbLayout` and `Shape`.
 """
 import math
+import warnings
 
 from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
 from pyaedt.edb_core.edb_data.utilities import EDBStatistics
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.clr_module import Tuple
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
@@ -504,15 +505,19 @@
     @pyaedt_function_handler()
     def create_polygon(self, main_shape, layer_name, voids=[], net_name=""):
         """Create a polygon based on a list of points and voids.
 
         Parameters
         ----------
         main_shape : list of points or PolygonData or ``modeler.Shape``
-            Shape or point lists of the main object.
+            Shape or point lists of the main object. Point list can be in the format of `[[x1,y1], [x2,y2],..,[xn,yn]]`.
+            Each point can be:
+            - [x, y] coordinate
+            - [x, y, height] for an arc with specific height (between previous point and actual point)
+            - [x, y, rotation, xc, yc] for an arc given a point, rotation and center.
         layer_name : str
             Name of the layer on which to create the polygon.
         voids : list, optional
             List of shape objects for voids or points that creates the shapes. The default is``[]``.
         net_name : str, optional
             Name of the net. The default is ``""``.
 
@@ -551,39 +556,38 @@
         else:
             return EDBPrimitives(polygon, self._pedb)
 
     @pyaedt_function_handler()
     def create_polygon_from_points(self, point_list, layer_name, net_name=""):
         """Create a new polygon from a point list.
 
+        .. deprecated:: 0.6.73
+        Use :func:`create_polygon` method instead. It now supports point lists as arguments.
+
         Parameters
         ----------
         point_list : list
             Point list in the format of `[[x1,y1], [x2,y2],..,[xn,yn]]`.
+            Each point can be:
+            - [x,y] coordinate
+            - [x,y, height] for an arc with specific height (between previous point and actual point)
+            - [x,y, rotation, xc,yc] for an arc given a point, rotation and center.
         layer_name : str
             Name of layer on which create the polygon.
         net_name : str, optional
             Name of the net on which create the polygon.
 
         Returns
         -------
         :class:`pyaedt.edb_core.edb_data.primitives_data.EDBPrimitives`
         """
-        net = self._pedb.nets.find_or_create_net(net_name)
-        plane = self.Shape("polygon", points=point_list)
-        _poly = self.shape_to_polygon_data(plane)
-        if _poly is None or _poly.IsNull() or _poly is False:
-            self._logger.error("Failed to create main shape polygon data")
-            return False
-        polygon = self._edb.Cell.Primitive.Polygon.Create(self._active_layout, layer_name, net, _poly)
-        if polygon.IsNull():
-            self._logger.error("Null polygon created")
-            return False
-        else:
-            return EDBPrimitives(polygon, self._pedb)
+        warnings.warn(
+            "Use :func:`create_polygon` method instead. It now supports point lists as arguments.", DeprecationWarning
+        )
+        return self.create_polygon(point_list, layer_name, net_name=net_name)
 
     @pyaedt_function_handler()
     def create_rectangle(
         self,
         layer_name,
         net_name="",
         lower_left_point="",
@@ -866,14 +870,29 @@
                     or endPoint[1].IsParametric()
                 )
                 arc = self._edb.Geometry.ArcData(
                     self._pedb.point_data(startPoint[0], startPoint[1]),
                     self._pedb.point_data(endPoint[0], endPoint[1]),
                 )
                 arcs.append(arc)
+            elif len(endPoint) == 3:
+                is_parametric = (
+                    is_parametric
+                    or startPoint[0].IsParametric()
+                    or startPoint[1].IsParametric()
+                    or endPoint[0].IsParametric()
+                    or endPoint[1].IsParametric()
+                    or endPoint[2].IsParametric()
+                )
+                arc = self._edb.Geometry.ArcData(
+                    self._pedb.point_data(startPoint[0], startPoint[1]),
+                    self._pedb.point_data(endPoint[0], endPoint[1]),
+                    endPoint[2].ToDouble(),
+                )
+                arcs.append(arc)
             elif len(endPoint) == 5:
                 is_parametric = (
                     is_parametric
                     or startPoint[0].IsParametric()
                     or startPoint[1].IsParametric()
                     or endPoint[0].IsParametric()
                     or endPoint[1].IsParametric()
@@ -885,27 +904,18 @@
                     rotationDirection = self._edb.Geometry.RotationDirection.CW
                 elif endPoint[2].ToString() == "ccw":
                     rotationDirection = self._edb.Geometry.RotationDirection.CCW
                 else:
                     self._logger.error("Invalid rotation direction %s is specified.", endPoint[2])
                     return None
                 arc = self._edb.Geometry.ArcData(
-                    self._edb.Geometry.PointData(
-                        self._get_edb_value(startPoint[0].ToDouble()),
-                        self._get_edb_value(startPoint[1].ToDouble()),
-                    ),
-                    self._edb.Geometry.PointData(
-                        self._get_edb_value(endPoint[0].ToDouble()),
-                        self._get_edb_value(endPoint[1].ToDouble()),
-                    ),
+                    self._pedb.point_data(startPoint[0], startPoint[1]),
+                    self._pedb.point_data(endPoint[0], endPoint[1]),
                     rotationDirection,
-                    self._edb.Geometry.PointData(
-                        self._get_edb_value(endPoint[3].ToDouble()),
-                        self._get_edb_value(endPoint[4].ToDouble()),
-                    ),
+                    self._pedb.point_data(endPoint[3], endPoint[4]),
                 )
                 arcs.append(arc)
         polygon = self._edb.Geometry.PolygonData.CreateFromArcs(convert_py_list_to_net_list(arcs), True)
         if not is_parametric:
             return polygon
         else:
             k = 0
@@ -924,14 +934,28 @@
             if not isinstance(point[0], (int, float, str)):
                 self._logger.error("Point X value must be a number.")
                 return False
             if not isinstance(point[1], (int, float, str)):
                 self._logger.error("Point Y value must be a number.")
                 return False
             return True
+        elif len(point) == 3:
+            if not allowArcs:
+                self._logger.error("Arc found but arcs are not allowed in _validatePoint.")
+                return False
+            if not isinstance(point[0], (int, float, str)):
+                self._logger.error("Point X value must be a number.")
+                return False
+            if not isinstance(point[1], (int, float, str)):
+                self._logger.error("Point Y value must be a number.")
+                return False
+            if not isinstance(point[1], (int, float, str)):
+                self._logger.error("Invalid point height.")
+                return False
+            return True
         elif len(point) == 5:
             if not allowArcs:
                 self._logger.error("Arc found but arcs are not allowed in _validatePoint.")
                 return False
             if not isinstance(point[0], (int, float, str)):
                 self._logger.error("Point X value must be a number.")
                 return False
```

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/materials.py` & `pyaedt-0.6.74/pyaedt/edb_core/materials.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/nets.py` & `pyaedt-0.6.74/pyaedt/edb_core/nets.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/padstack.py` & `pyaedt-0.6.74/pyaedt/edb_core/padstack.py`

 * *Files 2% similar despite different names*

```diff
@@ -567,20 +567,44 @@
 
         if "PadstackDef" in str(type(pin)):
             padparams = pin.GetData().GetPadParametersValue(layername, self.int_to_pad_type(pad_type))
         else:
             padparams = self._edb.Definition.PadstackDefData(pin.GetPadstackDef().GetData()).GetPadParametersValue(
                 layername, self.int_to_pad_type(pad_type)
             )
-        geom_type = int(padparams[1])
-        parameters = [i.ToString() for i in padparams[2]]
-        offset_x = padparams[3].ToDouble()
-        offset_y = padparams[4].ToDouble()
-        rot = padparams[5].ToDouble()
-        return geom_type, parameters, offset_x, offset_y, rot
+        if padparams[2]:
+            geometry_type = int(padparams[1])
+            parameters = [i.ToString() for i in padparams[2]]
+            offset_x = padparams[3].ToDouble()
+            offset_y = padparams[4].ToDouble()
+            rotation = padparams[5].ToDouble()
+            return geometry_type, parameters, offset_x, offset_y, rotation
+        else:
+            if isinstance(pin, self._edb.Definition.PadstackDef):
+                padparams = self._edb.Definition.PadstackDefData(pin.GetData()).GetPolygonalPadParameters(
+                    layername, self.int_to_pad_type(pad_type)
+                )
+            else:
+                padparams = self._edb.Definition.PadstackDefData(
+                    pin.GetPadstackDef().GetData()
+                ).GetPolygonalPadParameters(layername, self.int_to_pad_type(pad_type))
+
+            if padparams[0]:
+                parameters = [
+                    padparams[1].GetBBox().Item1.X.ToDouble(),
+                    padparams[1].GetBBox().Item1.Y.ToDouble(),
+                    padparams[1].GetBBox().Item2.X.ToDouble(),
+                    padparams[1].GetBBox().Item2.Y.ToDouble(),
+                ]
+                offset_x = padparams[2]
+                offset_y = padparams[3]
+                rotation = padparams[4]
+                geometry_type = 7
+                return geometry_type, parameters, offset_x, offset_y, rotation
+            return 0, [0], 0, 0, 0
 
     @pyaedt_function_handler
     def set_all_antipad_value(self, value):
         """Set all anti-pads from all pad-stack definition to the given value.
 
         Parameters
         ----------
```

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/siwave.py` & `pyaedt-0.6.74/pyaedt/edb_core/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/edb_core/stackup.py` & `pyaedt-0.6.74/pyaedt/edb_core/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/emit.py` & `pyaedt-0.6.74/pyaedt/emit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/emit_core/Couplings.py` & `pyaedt-0.6.74/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/emit_core/EmitConstants.py` & `pyaedt-0.6.74/pyaedt/emit_core/EmitConstants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/emit_core/__init__.py` & `pyaedt-0.6.74/pyaedt/emit_core/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import imp
 from importlib import import_module
 import os
 import sys
 
+from pyaedt import pyaedt_logger as logger
+
 EMIT_API_PYTHON = None
 
 delcross_python_path = os.environ.get("ANSYS_DELCROSS_PYTHON_PATH")
 if delcross_python_path:
     sys.path.append(delcross_python_path)
 
 
@@ -20,10 +23,13 @@
 # need this as a function so that it can be set
 # for the correct aedt version that the user is running
 def _set_api(aedt_version):
     numeric_version = int(aedt_version[-3:])
     desktop_path = os.environ.get(aedt_version)
     if desktop_path and numeric_version > 231:
         path = os.path.join(desktop_path, "Delcross")
-        sys.path.append(path)
+        sys.path.insert(0, path)
+        module_path = imp.find_module("EmitApiPython")[1]
+        logger.info("Importing EmitApiPython from: {}".format(module_path))
         global EMIT_API_PYTHON
         EMIT_API_PYTHON = import_module("EmitApiPython")
+        logger.info("Loaded {}".format(EMIT_API_PYTHON.EmitApi().get_version(True)))
```

### Comparing `pyaedt-0.6.73/pyaedt/emit_core/results/results.py` & `pyaedt-0.6.74/pyaedt/emit_core/results/results.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,35 +34,31 @@
         """List of all result revisions. Only one loaded at a time"""
 
         self.design = emit_obj.odesktop.GetActiveProject().GetActiveDesign()
         """Active design for the Emit project."""
 
     @pyaedt_function_handler()
     def _add_revision(self, name=None):
-        """Add a new revision.
+        """Add a new revision or get the current revision if it already exists.
 
         Parameters
         ----------
         name : str, optional
-            Name for the new revision. If None, it will
-            be named the current design revision.
+            Name for the new revision, if created. The default is ``None``, in which
+            case the name of the current design revision is used.
+
+        Raises
+        ------
+        RuntimeError if the name given is not the name of an existing result set and a current result set already
+        exists.
 
         Returns
         -------
         ``Revision`` object that was created.
         """
-        if name == None:
-            # check for a Current Revision that just hasn't been
-            # loaded by pyaedt
-            if self.design.GetCurrentResult() == "":
-                self.design.AddResult()
-                rev_num = self.design.GetRevision()
-                name = "Revision {}".format(rev_num)
-            else:
-                name = self.design.GetCurrentResult()
         revision = Revision(self, self.emit_project, name)
         self.revisions.append(revision)
         return revision
 
     @pyaedt_function_handler()
     def delete_revision(self, revision_name):
         """Delete the specified revision from the results.
```

### Comparing `pyaedt-0.6.73/pyaedt/emit_core/results/revision.py` & `pyaedt-0.6.74/pyaedt/emit_core/results/revision.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import warnings
 
 import pyaedt.emit_core.EmitConstants as emitConsts
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class Revision:
@@ -12,66 +11,59 @@
     Parameters
     ----------
     parent_results :
         ``Results`` object that this revision is associated with.
     emit_obj :
          ``Emit`` object that this revision is associated with.
     name : str, optional
-        Name of the revision to create. The default is ``None``, in which case a
-        default name is given.
+        Name of the revision to create. The default is ``None``, in which
+        case the name of the current design revision is used.
+
+    Raises
+    ------
+    RuntimeError if the name given is not the name of an existing result set and a current result set already exists.
 
     Examples
     --------
     Create a ``Revision`` instance.
 
     >>> aedtapp = Emit()
     >>> rev = Revision(results, aedtapp, "Revision 1")
     >>> domain = aedtapp.interaction_domain()
     >>> rev.run(domain)
     """
 
-    def __init__(self, parent_results, emit_obj, name=""):
-        design = emit_obj.odesktop.GetActiveProject().GetActiveDesign()
-        subfolder = ""
-        proj_name = emit_obj.oproject.GetName()
-        for f in os.scandir(emit_obj.oproject.GetPath()):
-            if os.path.splitext(f.name)[0] == proj_name and os.path.splitext(f.name)[1].lower() == ".aedtresults":
-                subfolder = os.path.join(f.path, "EmitDesign1")
-        default_behaviour = not os.path.exists(os.path.join(subfolder, "{}.emit".format(name)))
-        if default_behaviour:
-            print("The most recently generated revision will be used because the revision specified does not exist.")
-        if name == "" or default_behaviour:
-            # if there are no results yet, add a new Result
-            result_files = os.listdir(subfolder)
-            if len(result_files) == 0:
-                name = design.AddResult()
-                full = subfolder + "/{}.emit".format(name)
-            else:
-                file = max([f for f in os.scandir(subfolder)], key=lambda x: x.stat().st_mtime)
-                full = file.path
-                name = file.name
+    def __init__(self, parent_results, emit_obj, name=None):
+        if not name:
+            name = emit_obj.odesign.GetCurrentResult()
+            if not name:
+                name = emit_obj.odesign.AddResult("")
         else:
-            full = subfolder + "/{}.emit".format(name)
+            if name not in emit_obj.odesign.GetResultList():
+                name = emit_obj.odesign.AddResult(name)
+        full = emit_obj.odesign.GetResultDirectory(name)
+
         self.name = name
         """Name of the revision."""
 
         self.path = full
         """Full path of the revision."""
 
         self.emit_project = emit_obj
         """Emit project."""
 
-        result_props = design.GetResultProperties(name)
-        # Strip off the Revision #
-        self.revision_number = result_props[0][9:]
+        raw_props = emit_obj.odesign.GetResultProperties(name)
+        key = lambda s: s.split("=", 1)[0]
+        val = lambda s: s.split("=", 1)[1]
+        props = {key(s): val(s) for s in raw_props}
+
+        self.revision_number = int(props["Revision"])
         """Unique revision number from the Emit design"""
 
-        result_props = design.GetResultProperties(name)
-        # Strip off the 'Timestamp='
-        self.timestamp = result_props[1][10:]
+        self.timestamp = props["Timestamp"]
         """Unique timestamp for the revision"""
 
         self.parent_results = parent_results
         """Parent Results object"""
 
         # load the revision after creating it
         self.revision_loaded = False
@@ -122,14 +114,16 @@
         ----------
         >>> domain = aedtapp.results.interaction_domain()
         >>> rev.run(domain)
 
         """
         self._load_revision()
         engine = self.emit_project._emit_api.get_engine()
+        if domain.interferer_names and engine.max_simultaneous_interferers != len(domain.interferer_names):
+            raise ValueError("The max_simultaneous_interferers must equal the number of interferers in the domain.")
         interaction = engine.run(domain)
         # save the revision
         self.emit_project._emit_api.save_project()
         return interaction
 
     @pyaedt_function_handler()
     def is_domain_valid(self, domain):
@@ -321,15 +315,14 @@
 
         Examples
         ----------
         >>> aedtapp.results.current_revision.notes = "Added a filter to the WiFi Radio."
         >>> aedtapp.results.current_revision.notes
         'Added a filter to the WiFi Radio.'
         """
-        design = self.emit_project.odesktop.GetActiveProject().GetActiveDesign()
+        design = self.emit_project.odesign
         return design.GetResultNotes(self.name)
 
     @notes.setter
     def notes(self, notes):
-        design = self.emit_project.odesktop.GetActiveProject().GetActiveDesign()
-        design.SetResultNotes(self.name, notes)
+        self.emit_project.odesign.SetResultNotes(self.name, notes)
         self.emit_project._emit_api.save_project()
```

### Comparing `pyaedt-0.6.73/pyaedt/generic/DataHandlers.py` & `pyaedt-0.6.74/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.6.74/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/clr_module.py` & `pyaedt-0.6.74/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/configurations.py` & `pyaedt-0.6.74/pyaedt/generic/configurations.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/constants.py` & `pyaedt-0.6.74/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/design_types.py` & `pyaedt-0.6.74/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/filesystem.py` & `pyaedt-0.6.74/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/general_methods.py` & `pyaedt-0.6.74/pyaedt/generic/general_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1570,14 +1570,134 @@
                 if install_version == long_version:
                     return True
         except:
             pass
     return False
 
 
+def install_with_pip(package_name, package_path=None, upgrade=False, uninstall=False):  # pragma: no cover
+    """Install a new package using pip.
+    This method is useful for installing a package from the AEDT Console without launching the Python environment.
+
+    Parameters
+    ----------
+    package_name : str
+        Name of the package to install.
+    package_path : str, optional
+        Path for the GitHub package to download and install. For example, ``git+https://.....``.
+    upgrade : bool, optional
+        Whether to upgrade the package. The default is ``False``.
+    uninstall : bool, optional
+        Whether to install the package or uninstall the package.
+    """
+    if is_linux and is_ironpython:
+        import subprocessdotnet as subprocess
+    else:
+        import subprocess
+    executable = '"{}"'.format(sys.executable) if is_windows else sys.executable
+
+    commands = []
+    if uninstall:
+        commands.append([executable, "-m", "pip", "uninstall", "--yes", package_name])
+    else:
+        if package_path and upgrade:
+            commands.append([executable, "-m", "pip", "uninstall", "--yes", package_name])
+            command = [executable, "-m", "pip", "install", package_path]
+        else:
+            command = [executable, "-m", "pip", "install", package_name]
+        if upgrade:
+            command.append("-U")
+
+        commands.append(command)
+    for command in commands:
+        if is_linux:
+            p = subprocess.Popen(command)
+        else:
+            p = subprocess.Popen(" ".join(command))
+        p.wait()
+
+
+class Help:  # pragma: no cover
+    def __init__(self):
+        self._base_path = "https://aedt.docs.pyansys.com/version/stable"
+        self.browser = "default"
+
+    def _launch_ur(self, url):
+        import webbrowser
+
+        if self.browser != "default":
+            webbrowser.get(self.browser).open_new_tab(url)
+        else:
+            webbrowser.open_new_tab(url)
+
+    def search(self, keywords, app_name=None, search_in_examples_only=False):
+        """Search for one or more keywords.
+
+        Parameters
+        ----------
+        keywords : str or list
+        app_name : str, optional
+            Name of a PyAEDT app. For example, ``"Hfss"``, ``"Circuit"``, ``"Icepak"``, or any other available app.
+        search_in_examples_only : bool, optional
+            Whether to search for the one or more keywords only in the PyAEDT examples.
+            The default is ``False``.
+        """
+        if isinstance(keywords, str):
+            keywords = [keywords]
+        if search_in_examples_only:
+            keywords.append("This example")
+        if app_name:
+            keywords.append(app_name)
+        url = self._base_path + "/search.html?q={}".format("+".join(keywords))
+        self._launch_ur(url)
+
+    def getting_started(self):
+        """Open the PyAEDT User guide page."""
+        url = self._base_path + "/User_guide/index.html"
+        self._launch_ur(url)
+
+    def examples(self):
+        """Open the PyAEDT Examples page."""
+        url = self._base_path + "/examples/index.html"
+        self._launch_ur(url)
+
+    def github(self):
+        """Open the PyAEDT GitHub page."""
+        url = "https://github.com/pyansys/pyaedt"
+        self._launch_ur(url)
+
+    def changelog(self, release=None):
+        """Open the PyAEDT GitHub Changelog for a given release.
+
+        Parameters
+        ----------
+        release : str, optional
+            Release to get the changelog for. For example, ``"0.6.70"``.
+        """
+        if release is None:
+            from pyaedt import __version__ as release
+        url = "https://github.com/pyansys/pyaedt/releases/tag/v" + release
+        self._launch_ur(url)
+
+    def issues(self):
+        """Open the PyAEDT GitHub Issues page."""
+        url = "https://github.com/pyansys/pyaedt/issues"
+        self._launch_ur(url)
+
+    def ansys_forum(self):
+        """Open the PyAEDT GitHub Issues page."""
+        url = "https://discuss.ansys.com/discussions/tagged/pyaedt"
+        self._launch_ur(url)
+
+    def developer_forum(self):
+        """Open the Discussions page on the Ansys Developer site."""
+        url = "https://developer.ansys.com/"
+        self._launch_ur(url)
+
+
 class Settings(object):
     """Manages all PyAEDT environment variables and global settings."""
 
     def __init__(self):
         self._enable_logger = True
         self._enable_desktop_logs = True
         self._enable_screen_logs = True
@@ -1621,14 +1741,15 @@
         self._lsf_queue = None
         self._aedt_environment_variables = {
             "ANS_MESHER_PROC_DUMP_PREPOST_BEND_SM3": "1",
             "ANSYSEM_FEATURE_SF6694_NON_GRAPHICAL_COMMAND_EXECUTION_ENABLE": "1",
             "ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE": "1",
             "ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE": "1",
             "ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE": "1",
+            "ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE": "1",
         }
         if is_linux:
             self._aedt_environment_variables["ANS_NODEPCHECK"] = "1"
         self._desktop_launch_timeout = 90
 
     @property
     def desktop_launch_timeout(self):
@@ -2017,7 +2138,8 @@
 
     @enable_debug_logger.setter
     def enable_debug_logger(self, val):
         self._enable_debug_logger = val
 
 
 settings = Settings()
+online_help = Help()
```

### Comparing `pyaedt-0.6.73/pyaedt/generic/ibis_reader.py` & `pyaedt-0.6.74/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/near_field_import.py` & `pyaedt-0.6.74/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/pdf.py` & `pyaedt-0.6.74/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/plot.py` & `pyaedt-0.6.74/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/process.py` & `pyaedt-0.6.74/pyaedt/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/python_optimizers.py` & `pyaedt-0.6.74/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/report_file_parser.py` & `pyaedt-0.6.74/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/toolkit.py` & `pyaedt-0.6.74/pyaedt/generic/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.6.74/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/hfss.py` & `pyaedt-0.6.74/pyaedt/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/hfss3dlayout.py` & `pyaedt-0.6.74/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/icepak.py` & `pyaedt-0.6.74/pyaedt/icepak.py`

 * *Files 1% similar despite different names*

```diff
@@ -1844,15 +1844,14 @@
 
         Returns
         -------
         list
             List containing the requested link data.
 
         """
-
         if "linkData" in kwargs:
             warnings.warn(
                 "The ``linkData`` parameter was deprecated in 0.6.43. Use the ``links_data`` parameter instead.",
                 DeprecationWarning,
             )
             links_data = kwargs["linkData"]
 
@@ -2073,15 +2072,14 @@
             NativeComponentObject object.
 
         References
         ----------
 
         >>> oModule.InsertNativeComponent
         """
-
         if "extenttype" in kwargs:
             warnings.warn(
                 "The ``extenttype`` parameter was deprecated in 0.6.43. Use the ``extent_type`` parameter instead.",
                 DeprecationWarning,
             )
             extent_type = kwargs["extenttype"]
 
@@ -2180,39 +2178,38 @@
             Name of the new PCB component to create in Icepak.
         project_name : str
             Name of the project or the full path to the project.
         design_name : str
             Name of the design.
         resolution : int, optional
             Resolution of the mapping. The default is ``2``.
-        extent_type :
+        extent_type : str, optional
             Type of the extent. Options are ``"Polygon"`` and ``"Bounding Box"``. The default
             is ``"Bounding Box"``.
         outline_polygon : str, optional
             Name of the outline polygon if ``extent_type="Polygon"``. The default is ``""``.
         close_linked_project_after_import : bool, optional
             Whether to close the linked AEDT project after the import. The default is ``True``.
-        custom_x_resolution :
+        custom_x_resolution : int, optional
             The default is ``None``.
-        custom_y_resolution :
+        custom_y_resolution : int, optional
             The default is ``None``.
         power_in : float, optional
             Power in in Watt.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.InsertNativeComponent
         """
-
         if "extenttype" in kwargs:
             warnings.warn(
                 "``extenttype`` was deprecated in 0.6.43. Use ``extent_type`` instead.",
                 DeprecationWarning,
             )
             extent_type = kwargs["extenttype"]
 
@@ -2266,15 +2263,14 @@
 
         References
         ----------
 
         >>> oEditor.Copy
         >>> oeditor.Paste
         """
-
         if "groupName" in kwargs:
             warnings.warn(
                 "The ``groupName`` parameter was deprecated in 0.6.43. Use the ``group_name`` parameter instead.",
                 DeprecationWarning,
             )
             group_name = kwargs["groupName"]
 
@@ -2356,15 +2352,14 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.EditGlobalMeshRegion
         """
-
         bounding_box = self.modeler.oeditor.GetModelBoundingBox()
         xsize = abs(float(bounding_box[0]) - float(bounding_box[3])) / (15 * meshtype * meshtype)
         ysize = abs(float(bounding_box[1]) - float(bounding_box[4])) / (15 * meshtype * meshtype)
         zsize = abs(float(bounding_box[2]) - float(bounding_box[5])) / (10 * meshtype)
         MaxSizeRatio = 1 + (meshtype / 2)
 
         self.omeshmodule.EditGlobalMeshRegion(
@@ -2684,30 +2679,29 @@
         gravityDir : int, optional
             Gravity direction index in the range ``[0, 5]``. The default is ``5``.
         perform_minimal_val : bool, optional
             Whether to perform minimal validation. The default is ``True``.
             If ``False``, full validation is performed.
         default_fluid : str, optional
             Type of fluid. The default is ``"Air"``.
-        default_solid :
+        default_solid : str, optional
             Type of solid. The default is ``"Al-Extruded"``.
-        default_surface :
+        default_surface : str, optional
             Type of surface. The default is ``"Steel-oxidised-surface"``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oDesign.SetDesignSettings
         """
-
         ambient_temperature = self.modeler._arg_with_dim(ambienttemp, "cel")
 
         axes = ["X", "Y", "Z"]
         GVPos = False
         if int(gravityDir) > 2:
             GVPos = True
         gravity_axis = axes[int(gravityDir) - 3]
```

### Comparing `pyaedt-0.6.73/pyaedt/maxwell.py` & `pyaedt-0.6.74/pyaedt/maxwell.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/maxwellcircuit.py` & `pyaedt-0.6.74/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/mechanical.py` & `pyaedt-0.6.74/pyaedt/mechanical.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/Console.py_build` & `pyaedt-0.6.74/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.6.74/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.6.74/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.6.74/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.6.74/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.6.74/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/amat.xml` & `pyaedt-0.6.74/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/console_setup.py` & `pyaedt-0.6.74/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.6.74/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.6.74/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.6.74/pyaedt/misc/install_extra_toolkits.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.6.74/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/misc.py` & `pyaedt-0.6.74/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.6.74/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.6.74/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.6.74/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.6.74/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.6.74/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.6.74/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/misc/template.acf` & `pyaedt-0.6.74/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.6.74/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.6.74/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.6.74/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.6.74/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.6.74/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.6.74/pyaedt/modeler/cad/Modeler.py`

 * *Files 0% similar despite different names*

```diff
@@ -2635,15 +2635,14 @@
 
         References
         ----------
 
         >>> oEditor.Mirror
         >>> oEditor.DuplicateMirror
         """
-
         selections = self.convert_to_selections(objid)
         Xpos, Ypos, Zpos = self._pos_with_arg(position)
         Xnorm, Ynorm, Znorm = self._pos_with_arg(vector)
         if duplicate:
             vArg1 = ["NAME:Selections", "Selections:=", selections, "NewPartsModelFlag:=", "Model"]
             vArg2 = ["NAME:DuplicateToMirrorParameters"]
             vArg2.append("DuplicateMirrorBaseX:="), vArg2.append(Xpos)
@@ -4978,15 +4977,14 @@
 
         References
         ----------
 
         >>> oEditor.MoveFaces
 
         """
-
         face_selection = self.convert_to_selections(faces, True)
         selection = {}
         for f in face_selection:
             if self.oeditor.GetObjectNameByFaceID(f) in selection:
                 selection[self.oeditor.GetObjectNameByFaceID(f)].append(f)
             else:
                 selection[self.oeditor.GetObjectNameByFaceID(f)] = [f]
@@ -5040,15 +5038,14 @@
 
         References
         ----------
 
         >>> oEditor.MoveEdges
 
         """
-
         edge_selection = self.convert_to_selections(edges, True)
         selection = {}
         for f in edge_selection:
             if self.oeditor.GetObjectNameByEdgeID(f) in selection:
                 selection[self.oeditor.GetObjectNameByEdgeID(f)].append(f)
             else:
                 selection[self.oeditor.GetObjectNameByEdgeID(f)] = [f]
```

### Comparing `pyaedt-0.6.73/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.6.74/pyaedt/modeler/cad/Primitives.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.6.74/pyaedt/modeler/cad/Primitives2D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.6.74/pyaedt/modeler/cad/Primitives3D.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from math import pi
 from math import radians
 from math import sin
 from math import sqrt
 from math import tan
 import os
 
+from pyaedt import Edb
 from pyaedt import Icepak
 from pyaedt.generic import LoadAEDTFile
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.advanced_cad.actors import Bird
@@ -1423,14 +1424,249 @@
                 udm_obj.name = name
             os.remove(temp_proj)
             return udm_obj, mapping_dict, aux_dict
         else:
             return udm_obj
 
     @pyaedt_function_handler()
+    def insert_layout_component(
+        self,
+        comp_file,
+        coordinate_system="Global",
+        name=None,
+        parameter_mapping=False,
+    ):
+        """Insert a new layout component.
+
+        Parameters
+        ----------
+        comp_file : str
+            Path of the component file. Either ``".aedb"`` and ``".aedbcomp"`` are allowed.
+        coordinate_system : str, optional
+            Target coordinate system. The default is ``"Global"``.
+        name : str, optional
+            3D component name. The default is ``None``.
+        parameter_mapping : bool, optional
+            Map the layout parameters in the target HFSS design. The default is ``False``.
+
+        Returns
+        -------
+        :class:`pyaedt.modeler.components_3d.UserDefinedComponent`
+            User defined component object.
+
+        References
+        ----------
+
+        >>> oEditor.InsertNativeComponent
+
+        Examples
+        --------
+        >>> from pyaedt import Hfss
+        >>> app = Hfss()
+        >>> layout_component = "path/to/layout_component/component.aedbcomp"
+        >>> comp = app.modeler.insert_layout_component(layout_component)
+
+        """
+        if self._app.solution_type != "Terminal" and self._app.solution_type != "TransientAPhiFormulation":
+            self.logger.warning("Solution type must be terminal in HFSS or APhi in Maxwell")
+            return False
+
+        component_name = os.path.splitext(os.path.basename(comp_file))[0]
+        aedt_component_name = component_name
+        if component_name not in self._app.o_component_manager.GetNames():
+            compInfo = ["NAME:" + str(component_name), "Info:=", []]
+
+            compInfo.extend(
+                [
+                    "CircuitEnv:=",
+                    0,
+                    "Refbase:=",
+                    "U",
+                    "NumParts:=",
+                    1,
+                    "ModSinceLib:=",
+                    True,
+                    "Terminal:=",
+                    [],
+                    "CompExtID:=",
+                    9,
+                    "ModelEDBFilePath:=",
+                    comp_file,
+                    "EDBCompPassword:=",
+                    "",
+                ]
+            )
+
+            aedt_component_name = self._app.o_component_manager.Add(compInfo)
+
+        if not name or name in self.modeler.user_defined_component_names:
+            name = generate_unique_name("LC")
+
+        # Open Layout component and get information
+        aedb_component_path = comp_file
+        if os.path.splitext(os.path.basename(comp_file))[1] == ".aedbcomp":
+            aedb_project_path = os.path.join(self._app.project_path, self._app.project_name + ".aedb")
+            aedb_component_path = os.path.join(
+                aedb_project_path, "LayoutComponents", aedt_component_name, aedt_component_name + ".aedb"
+            )
+            aedb_component_path = aedb_component_path.replace("/", "\\")
+
+        component_obj = Edb(
+            edbpath=aedb_component_path,
+            isreadonly=True,
+            edbversion=self._app._aedt_version,
+            student_version=self._app.student_version,
+        )
+
+        # Extract and map parameters
+        parameters = {}
+        for param in component_obj.design_variables:
+            parameters[param] = [param + "_" + name, component_obj.design_variables[param].value_string]
+            if parameter_mapping:
+                self._app[param + "_" + name] = component_obj.design_variables[param].value_string
+
+        # Get coordinate systems
+        component_cs = list(component_obj.components.components.keys())
+        component_obj.close_edb()
+
+        vArg1 = ["NAME:InsertNativeComponentData"]
+        vArg1.append("TargetCS:=")
+        vArg1.append(coordinate_system)
+        vArg1.append("SubmodelDefinitionName:=")
+        vArg1.append("LC")
+        varg2 = ["NAME:ComponentPriorityLists"]
+        vArg1.append(varg2)
+        vArg1.append("NextUniqueID:=")
+        vArg1.append(0)
+        vArg1.append("MoveBackwards:=")
+        vArg1.append(False)
+        vArg1.append("DatasetType:=")
+        vArg1.append("ComponentDatasetType")
+        varg3 = ["NAME:DatasetDefinitions"]
+        vArg1.append(varg3)
+        varg4 = [
+            "NAME:BasicComponentInfo",
+            "ComponentName:=",
+            "LC",
+            "Company:=",
+            "",
+            "Company URL:=",
+            "",
+            "Model Number:=",
+            "",
+            "Help URL:=",
+            "",
+            "Version:=",
+            "1.0",
+            "Notes:=",
+            "",
+            "IconTypeL:=",
+            "Layout Component",
+        ]
+        vArg1.append(varg4)
+        varg5 = [
+            "NAME:GeometryDefinitionParameters",
+        ]
+        if parameters and parameter_mapping:
+            for param in parameters:
+                varg5.append("VariableProp:=")
+                varg5.append([parameters[param][0], "D", "", parameters[param][1]])
+
+        varg5.append(["NAME:VariableOrders"])
+        vArg1.append(varg5)
+
+        varg6 = ["NAME:DesignDefinitionParameters", ["NAME:VariableOrders"]]
+        vArg1.append(varg6)
+
+        varg7 = ["NAME:MaterialDefinitionParameters", ["NAME:VariableOrders"]]
+        vArg1.append(varg7)
+
+        vArg1.append("DefReferenceCSID:=")
+        vArg1.append(1)
+        vArg1.append("MapInstanceParameters:=")
+        vArg1.append("DesignVariable")
+        vArg1.append("UniqueDefinitionIdentifier:=")
+        vArg1.append("")
+        vArg1.append("OriginFilePath:=")
+        vArg1.append("")
+        vArg1.append("IsLocal:=")
+        vArg1.append(False)
+        vArg1.append("ChecksumString:=")
+        vArg1.append("")
+        vArg1.append("ChecksumHistory:=")
+        vArg1.append([])
+        vArg1.append("VersionHistory:=")
+        vArg1.append([])
+
+        varg8 = ["NAME:VariableMap"]
+
+        for param in parameters:
+            varg8.append(param + ":=")
+            if parameter_mapping:
+                varg8.append(parameters[param][0])
+            else:
+                varg8.append(parameters[param][1])
+
+        varg9 = [
+            "NAME:NativeComponentDefinitionProvider",
+            "Type:=",
+            "Layout Component",
+            "Unit:=",
+            "mm",
+            "Version:=",
+            1.1,
+            "EDBDefinition:=",
+            aedt_component_name,
+            varg8,
+            "ReferenceCS:=",
+            "Global",
+            "CSToImport:=",
+        ]
+
+        if component_cs:
+            varg10 = component_cs
+            varg10.append("Global")
+        else:
+            varg10 = ["Global"]
+        varg9.append(varg10)
+        vArg1.append(varg9)
+
+        varg11 = ["NAME:InstanceParameters"]
+        varg11.append("GeometryParameters:=")
+
+        if parameters and parameter_mapping:
+            varg12 = ""
+            for param in parameters:
+                varg12 += " {0}='{1}'".format(parameters[param][0], parameters[param][0])
+        else:
+            varg12 = ""
+        varg11.append(varg12[1:])
+
+        varg11.append("MaterialParameters:=")
+        varg11.append("")
+        varg11.append("DesignParameters:=")
+        varg11.append("")
+        vArg1.append(varg11)
+
+        try:
+            new_object_name = self.oeditor.InsertNativeComponent(vArg1)
+            udm_obj = False
+            if new_object_name:
+                obj_list = list(self.oeditor.Get3DComponentPartNames(new_object_name))
+                for new_name in obj_list:
+                    self._create_object(new_name)
+
+                udm_obj = self._create_user_defined_component(new_object_name)
+                if name:
+                    udm_obj.name = name
+        except Exception:  # pragma: no cover
+            udm_obj = False
+        return udm_obj
+
+    @pyaedt_function_handler()
     def get_3d_component_object_list(self, componentname):
         """Retrieve all objects belonging to a 3D component.
 
         Parameters
         ----------
         componentname : str
             Name of the 3D component.
```

### Comparing `pyaedt-0.6.73/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.6.74/pyaedt/modeler/cad/components_3d.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,14 +98,16 @@
             "Date",
             "Purpose",
             "Version",
         ]
         self._group_name = None
         self._is3dcomponent = None
         self._mesh_assembly = None
+        self._show_layout = None
+        self._fast_transformation = None
         if name:
             self._m_name = name
         else:
             self._m_name = _uname()
         self._parameters = {}
         self._parts = None
         self._primitives = primitives
@@ -119,23 +121,23 @@
         if component_type:
             self.auto_update = False
             self._props = UserDefinedComponentProps(
                 self,
                 OrderedDict(
                     {
                         "TargetCS": self._target_coordinate_system,
-                        "SubmodelDefinitionName": component,
+                        "SubmodelDefinitionName": self.definition_name,
                         "ComponentPriorityLists": OrderedDict({}),
                         "NextUniqueID": 0,
                         "MoveBackwards": False,
                         "DatasetType": "ComponentDatasetType",
                         "DatasetDefinitions": OrderedDict({}),
                         "BasicComponentInfo": OrderedDict(
                             {
-                                "ComponentName": component,
+                                "ComponentName": self.definition_name,
                                 "Company": "",
                                 "Company URL": "",
                                 "Model Number": "",
                                 "Help URL": "",
                                 "Version": "1.0",
                                 "Notes": "",
                                 "IconType": "",
@@ -297,14 +299,74 @@
             and isinstance(ma, bool)
             and key in self._primitives.oeditor.GetChildObject(self.name).GetPropNames()
         ):
             self._primitives.oeditor.GetChildObject(self.name).SetPropValue(key, ma)
             self._mesh_assembly = ma
 
     @property
+    def show_layout(self):
+        """Show layout flag.
+
+        Returns
+        -------
+        bool
+           ``True`` if show layout is checked and if the component is a Layout Component,
+           ``None`` if other cases.
+
+        """
+        key = "Show Layout"
+        if self.is3dcomponent and key in self._primitives.oeditor.GetChildObject(self.name).GetPropNames():
+            show_layout = self._primitives.oeditor.GetChildObject(self.name).GetPropValue(key)
+            self._show_layout = show_layout
+            return show_layout
+        else:
+            return None
+
+    @show_layout.setter
+    def show_layout(self, show_layout):
+        key = "Show Layout"
+        if (
+            self.is3dcomponent
+            and isinstance(show_layout, bool)
+            and key in self._primitives.oeditor.GetChildObject(self.name).GetPropNames()
+        ):
+            self._primitives.oeditor.GetChildObject(self.name).SetPropValue(key, show_layout)
+            self._show_layout = show_layout
+
+    @property
+    def fast_transformation(self):
+        """Show layout flag.
+
+        Returns
+        -------
+        bool
+           ``True`` if fast transformation is checked and if the component is a Layout Component,
+           ``None`` if other cases.
+
+        """
+        key = "Fast Transformation"
+        if self.is3dcomponent and key in self._primitives.oeditor.GetChildObject(self.name).GetPropNames():
+            fast_transformation = self._primitives.oeditor.GetChildObject(self.name).GetPropValue(key)
+            self._fast_transformation = fast_transformation
+            return fast_transformation
+        else:
+            return None
+
+    @fast_transformation.setter
+    def fast_transformation(self, fast_transformation):
+        key = "Fast Transformation"
+        if (
+            self.is3dcomponent
+            and isinstance(fast_transformation, bool)
+            and key in self._primitives.oeditor.GetChildObject(self.name).GetPropNames()
+        ):
+            self._primitives.oeditor.GetChildObject(self.name).SetPropValue(key, fast_transformation)
+            self._fast_transformation = fast_transformation
+
+    @property
     def name(self):
         """Name of the object.
 
         Returns
         -------
         str
            Name of the object.
@@ -374,15 +436,19 @@
 
         Returns
         -------
         dict
            :class:`pyaedt.modeler.Object3d`
 
         """
-        component_parts = list(self._primitives.oeditor.GetChildObject(self.name).GetChildNames())
+        if self.is3dcomponent:
+            component_parts = list(self._primitives.oeditor.Get3DComponentPartNames(self.name))
+        else:
+            component_parts = list(self._primitives.oeditor.GetChildObject(self.name).GetChildNames())
+
         parts_id = [
             self._primitives._object_names_to_ids[part]
             for part in self._primitives._object_names_to_ids
             if part in component_parts
         ]
         parts_dict = {part_id: self._primitives.objects[part_id] for part_id in parts_id}
         return parts_dict
```

### Comparing `pyaedt-0.6.73/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.6.74/pyaedt/modeler/cad/elements3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.6.74/pyaedt/modeler/cad/object3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -888,20 +888,25 @@
                 self._material_name = mat.strip('"').lower()
             return self._material_name
         return ""
 
     @material_name.setter
     def material_name(self, mat):
         matobj = self._primitives._materials.checkifmaterialexists(mat)
+        mat_value = None
         if matobj:
+            mat_value = chr(34) + matobj.name + chr(34)
+        elif "[" in mat or "(" in mat:
+            mat_value = mat
+        if mat_value is not None:
             if not self.model:
                 self.model = True
-            vMaterial = ["NAME:Material", "Value:=", chr(34) + matobj.name + chr(34)]
+            vMaterial = ["NAME:Material", "Value:=", mat_value]
             self._change_property(vMaterial)
-            self._material_name = matobj.name.lower()
+            self._material_name = mat_value.strip('"')
             self._solve_inside = None
         else:
             self.logger.warning("Material %s does not exist.", mat)
 
     @surface_material_name.setter
     def surface_material_name(self, mat):
         try:
```

### Comparing `pyaedt-0.6.73/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.6.74/pyaedt/modeler/cad/polylines.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,16 @@
 
     def _update_segments_and_points(self):
         """Updates the self._segment_types and the self._positions from the history.
         This internal method is called by properties ``points`` and ``segment_types``.
         It will be called only once after opening a new project, then the internal
         variables are maintained updated.
         It is a single update call for both properties because they are very similar,
-        and we can access to the history only once."""
+        and we can access to the history only once.
+        """
 
         def _convert_points(p_in, dest_unit):
             p_out = []
             for ip in p_in:
                 v, u = decompose_variable_value(ip)
                 if u == "":
                     p_out.append(v)
@@ -437,15 +438,14 @@
         # if succeeded save the result
         self._segment_types = segments
         self._positions = points
 
     @property
     def points(self):
         """Polyline Points."""
-
         if self._positions:
             return self._positions
         else:
             self._update_segments_and_points()
             return self._positions
 
     @property
@@ -569,15 +569,15 @@
         # Poly Line Cross Section
         varg1.append(self._xsection)
 
         return varg1
 
     @pyaedt_function_handler()
     def _evaluate_arc_angle_extra_points(self, segment, start_point):
-        """Evaluates the extra points for the ArcAngle segment type.
+        """Evaluate the extra points for the ArcAngle segment type.
         It also auto evaluates the arc_plane if it was not specified by the user.
         segment.extra_points[0] contains the arc mid point (on the arc).
         segment.extra_points[1] contains the arc end point.
         Both are function of the arc center, arc angle and arc plane.
         """
         # from start-point and angle, calculate the mid-point and end-points
         # Also identify the plane of the arc ("YZ", "ZX", "XY")
@@ -628,30 +628,30 @@
         return True
 
     @pyaedt_function_handler()
     def _segment_array(self, segment_data, start_index=0, start_point=None):
         """Retrieve a property array for a polyline segment for use in the
         :class:`pyaedt.modeler.Primitives.Polyline` constructor.
 
-         Parameters
-         ----------
-         segment_data : :class:`pyaedt.modeler.Primitives.PolylineSegment` or str
-             Pointer to the calling object that provides additional functionality
-             or a string with the segment type ``Line`` or ``Arc``.
-         start_index : int, string
-             Starting vertex index of the segment within a compound polyline. The
-             default is ``0``.
-         start_point : list, optional
-             Position of the first point for type ``AngularArc``. The default is
-             ``None``. Float values are considered in model units.
-
-         Returns
-         ------
-         list
-             List of properties defining a polyline segment.
+        Parameters
+        ----------
+        segment_data : :class:`pyaedt.modeler.Primitives.PolylineSegment` or str
+            Pointer to the calling object that provides additional functionality
+            or a string with the segment type ``Line`` or ``Arc``.
+        start_index : int, string
+            Starting vertex index of the segment within a compound polyline. The
+            default is ``0``.
+        start_point : list, optional
+            Position of the first point for type ``AngularArc``. The default is
+            ``None``. Float values are considered in model units.
+
+        Returns
+        -------
+        list
+            List of properties defining a polyline segment.
 
         """
         if isinstance(segment_data, str):
             segment_data = PolylineSegment(segment_data)
 
         seg = [
             "NAME:PLSegment",
@@ -1029,15 +1029,15 @@
             If set to ``False`` only points that are at the extremities of the segments are considered.
             If pn is in the middle of a segment, the function returns False.
             If set to ``True`` also points in the middle of the segments are considered.
 
         Returns
         -------
         int, bool
-            segment id when successful. ``False`` when failed.
+            Segment id when successful. ``False`` when failed.
         """
         n_points = 0
         for i, s in enumerate(self.segment_types):
             if n_points == pn and at_start:
                 return i
             n_points_imu = n_points
             if s.type == "Line":
@@ -1064,28 +1064,27 @@
             List of positions of the points that define the segment to insert.
             Either the starting point or ending point of the segment list must
             match one of the vertices of the existing polyline.
         segment : str or :class:`pyaedt.modeler.Primitives.PolylineSegment`, optional
             Definition of the segment to insert. For the types ``"Line"`` and ``"Arc"``,
             use their string values ``"Line"`` and ``"Arc"``. For the types ``"AngularArc"``
             and ``"Spline"``, use the :class:`pyaedt.modeler.Primitives.PolylineSegment`
-            object to define the segment precisely.
+            object to define the segment precisely. The default is ``None``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.InsertPolylineSegment
 
         """
-
         # Check for a valid number of points
         num_points = len(position_list)
 
         # define the segment type from the number of points given
         if not segment:
             if num_points < 2:
                 raise ValueError("num_points must contain at least 2 points to auto-define a segment.")
```

### Comparing `pyaedt-0.6.73/pyaedt/modeler/calculators.py` & `pyaedt-0.6.74/pyaedt/modeler/calculators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.6.74/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.6.74/pyaedt/modeler/geometry_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,21 @@
     @pyaedt_function_handler()
     def parse_dim_arg(string, scale_to_unit=None, variable_manager=None):
         """Convert a number and unit to a float.
         Angles are converted in radians.
 
         Parameters
         ----------
-        string : str
-            String to convert. For example, ``"2mm"``.
-        scale_to_unit : str
+        string : str, optional
+            String to convert. For example, ``"2mm"``. The default is ``None``.
+        scale_to_unit : str, optional
             Units for the value to convert. For example, ``"mm"``.
         variable_manager : :class:`pyaedt.application.Variables.VariableManager`, optional
             Try to parse formula and returns numeric value.
+            The default is ``None``.
 
         Returns
         -------
         float
             Value for the converted value and units. For example, ``0.002``.
 
         Examples
@@ -69,15 +70,14 @@
 
         Use the optional argument ``scale_to_unit`` to specify the destination unit.
 
         >>> go.parse_dim_arg('2mm', scale_to_unit='mm')
         >>> 2.0
 
         """
-
         if type(string) is not str:
             try:
                 return float(string)
             except ValueError:  # pragma: no cover
                 raise TypeError("Input argument is not string nor number")
         sunit = 1.0
         if scale_to_unit:
@@ -111,16 +111,16 @@
     @staticmethod
     @pyaedt_function_handler()
     def cs_plane_to_axis_str(val):
         """Retrieve a string for a coordinate system plane.
 
         Parameters
         ----------
-        val :
-
+        val : int
+            ``PLANE`` enum vélo.
 
         Returns
         -------
         str
            String for the coordinate system plane.
 
         """
@@ -157,15 +157,16 @@
     @staticmethod
     @pyaedt_function_handler()
     def cs_axis_str(val):
         """Retrieve a string for a coordinate system axis.
 
         Parameters
         ----------
-        val :
+        val : int
+            ``AXIS`` enum value.
 
 
         Returns
         -------
         str
             String for the coordinate system axis.
 
@@ -180,16 +181,16 @@
     @staticmethod
     @pyaedt_function_handler()
     def draft_type_str(val):
         """Retrieve the draft type.
 
         Parameters
         ----------
-        val :
-
+        val : int
+            ``SWEEPDRAFT`` enum value.
 
         Returns
         -------
         str
            Type of the draft.
 
         """
@@ -263,15 +264,14 @@
             List of ``[x, y, z]`` coordinates for the second vector.
 
         Returns
         -------
         List
             List of ``[x, y, z]`` coordinates for the result vector.
         """
-
         c = [a[1] * b[2] - a[2] * b[1], a[2] * b[0] - a[0] * b[2], a[0] * b[1] - a[1] * b[0]]
         return c
 
     @staticmethod
     @pyaedt_function_handler()
     def _v_dot(a, b):
         """Evaluate the dot product between two geometry vectors.
@@ -427,16 +427,16 @@
     @staticmethod
     @pyaedt_function_handler()
     def v_norm(a):
         """Evaluate the Euclidean norm of a geometry vector.
 
         Parameters
         ----------
-         a : List
-            List of ``[x, y, z]`` coordinates for the vector.
+        a : List
+        List of ``[x, y, z]`` coordinates for the vector.
 
         Returns
         -------
         float
             Evaluated norm in the same unit as the coordinates for the input vector.
 
         """
@@ -525,15 +525,14 @@
              The default is ``0``.
 
         Returns
         -------
         List
 
         """
-
         if direction <= 2:
             point = 1e6
             for p in pointlists:
                 if p[direction] < point:
                     point = p[direction]
         else:
             point = -1e6
@@ -724,15 +723,15 @@
         if not GeometryOperators.is_between_points(a2n, b1, b2):
             return False
         return True
 
     @staticmethod
     @pyaedt_function_handler()
     def arrays_positions_sum(vertlist1, vertlist2):
-        """ADD DESCRIPTION.
+        """Return the sum of two vertices lists.
 
         Parameters
         ----------
         vertlist1 : List
 
         vertlist2 : List
 
@@ -788,15 +787,14 @@
             List of ``[x, y, z]`` coordinates for the Y pointing axis.
 
         Returns
         -------
         tuple
             ``[Xx, Xy, Xz], [Yx, Yy, Yz], [Zx, Zy, Zz]`` of the three axes (normalized).
         """
-
         zpt = GeometryOperators.v_cross(x_pointing, y_pointing)
         ypt = GeometryOperators.v_cross(zpt, x_pointing)
 
         xp = GeometryOperators.normalize_vector(x_pointing)
         zp = GeometryOperators.normalize_vector(zpt)
         yp = GeometryOperators.normalize_vector(ypt)
 
@@ -1360,24 +1358,24 @@
             return 0.0
         else:
             return float(s)
 
     @staticmethod
     @pyaedt_function_handler()
     def is_small(s):
-        """
-        Return True if the number represented by s is zero (i.e very small).
+        """Return ``True`` if the number represented by s is zero (i.e very small).
 
         Parameters
         ----------
-        s, numeric or str
+        s : numeric or str
             Variable value.
 
         Returns
         -------
+            bool
 
         """
         n = GeometryOperators.get_numeric(s)
         return True if math.fabs(n) < 2.0 * abs(sys.float_info.epsilon) else False
 
     @staticmethod
     @pyaedt_function_handler()
```

### Comparing `pyaedt-0.6.73/pyaedt/modeler/modeler2d.py` & `pyaedt-0.6.74/pyaedt/modeler/modeler2d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/modeler3d.py` & `pyaedt-0.6.74/pyaedt/modeler/modeler3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.6.74/pyaedt/modeler/modelerpcb.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.6.74/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.6.74/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modeler/schematic.py` & `pyaedt-0.6.74/pyaedt/modeler/schematic.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.6.74/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/Boundary.py` & `pyaedt-0.6.74/pyaedt/modules/Boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1599,16 +1599,20 @@
     @property
     def name(self):
         """Boundary Name."""
         return self._name
 
     @name.setter
     def name(self, value):
-        self._name = value
+        if "Port" in self.props:
+            self.auto_update = False
+            self.props["Port"] = value
+            self.auto_update = True
         self.update()
+        self._name = value
 
     @pyaedt_function_handler()
     def _get_args(self, props=None):
         """Retrieve arguments.
 
         Parameters
         ----------
@@ -1644,15 +1648,18 @@
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
         updated = False
         for el in list(self.props.keys()):
-            if el in self._app.oeditor.GetProperties("EM Design", "Excitations:{}".format(self.name)) and self.props[
+            if el == "Port" and self._name != self.props[el]:
+                self._app.oeditor.SetPropertyValue("EM Design", "Excitations:" + self.name, el, self.props[el])
+                self._name = self.props[el]
+            elif el in self._app.oeditor.GetProperties("EM Design", "Excitations:{}".format(self.name)) and self.props[
                 el
             ] != self._app.oeditor.GetPropertyValue("EM Design", "Excitations:" + self.name, el):
                 self._app.oeditor.SetPropertyValue("EM Design", "Excitations:" + self.name, el, self.props[el])
                 updated = True
 
         if updated:
             self._refresh_properties()
```

### Comparing `pyaedt-0.6.73/pyaedt/modules/CableModeling.py` & `pyaedt-0.6.74/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.6.74/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.6.74/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/LayerStackup.py` & `pyaedt-0.6.74/pyaedt/modules/LayerStackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/Material.py` & `pyaedt-0.6.74/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/MaterialLib.py` & `pyaedt-0.6.74/pyaedt/modules/MaterialLib.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/Mesh.py` & `pyaedt-0.6.74/pyaedt/modules/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.6.74/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.6.74/pyaedt/modules/MeshIcepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.6.74/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/PostProcessor.py` & `pyaedt-0.6.74/pyaedt/modules/PostProcessor.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.6.74/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/SolveSetup.py` & `pyaedt-0.6.74/pyaedt/modules/SolveSetup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3073,14 +3073,32 @@
 
     @dc_enabled.setter
     def dc_enabled(self, value):
         if value or (self._ac_rl_enbled or self._capacitance_enabled):
             self._dc_enabled = value
             self.update()
 
+    @property
+    def dc_resistance_only(self):
+        """Get/Set the DC Resistance Only or Resistance/Inductance calculatio in active Q3D setup.
+
+        Returns
+        -------
+        bool
+        """
+        try:
+            return self.props["DC"]["SolveResOnly"]
+        except KeyError:
+            return False
+
+    @dc_resistance_only.setter
+    def dc_resistance_only(self, value):
+        if self.dc_enabled:
+            self.props["DC"]["SolveResOnly"] = value
+
     @pyaedt_function_handler()
     def update(self, update_dictionary=None):
         """Update the setup based on either the class argument or a dictionary.
 
         Parameters
         ----------
         update_dictionary : optional
```

### Comparing `pyaedt-0.6.73/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.6.74/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.6.74/pyaedt/modules/monitor_icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/report_templates.py` & `pyaedt-0.6.74/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/modules/solutions.py` & `pyaedt-0.6.74/pyaedt/modules/solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/q3d.py` & `pyaedt-0.6.74/pyaedt/q3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/rmxprt.py` & `pyaedt-0.6.74/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.6.74/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.6.74/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.6.74/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.6.74/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.6.74/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.6.74/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.6.74/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.6.74/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.6.74/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.6.74/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.6.74/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.6.74/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.6.74/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.6.74/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/sbrplus/plot.py` & `pyaedt-0.6.74/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/siwave.py` & `pyaedt-0.6.74/pyaedt/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyaedt/twinbuilder.py` & `pyaedt-0.6.74/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.73/pyproject.toml` & `pyaedt-0.6.74/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 
 [project]
 name = "pyaedt"
 dynamic = ["version"]
 description = "Higher-Level Pythonic Ansys Electronics Desktop Framework"
-readme = "README.rst"
+readme = "README.md"
 requires-python = ">=3.7,<4"
 license = {file = "LICENSE"}
 authors = [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 maintainers = [{name = "PyAEDT developers", email = "massimo.capodiferro@ansys.com"}]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
@@ -31,87 +31,90 @@
     "rpyc==5.3.1",
     "psutil",
     "dotnetcore2 ==3.1.23;platform_system=='Linux'",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "ipython==8.12.0",
+    "ipython==8.13.0",
+    "imageio==2.28.0",
     "joblib==1.2.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "openpyxl==3.1.2",
     "osmnx",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.1; python_version > '3.7'",
     "pytest==7.3.1",
     "pytest-cov==4.0.0",
     "pytest-xdist==3.2.1",
-    "pyvista==0.38.5",
+    "pyvista==0.38.6",
     "scikit-learn==1.2.2",
     "SRTM.py",
     "utm",
     "scikit-rf",
 
 ]
 doc = [
     "ansys-sphinx-theme==0.9.8",
     "imageio==2.28.0",
     "imageio-ffmpeg==0.4.8",
-    "ipython==8.12.0",
+    "ipython==8.13.0",
     "ipywidgets==8.0.6",
     "joblib==1.2.0",
     "jupyterlab==3.6.3",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "nbsphinx==0.9.1",
     "numpydoc==1.5.0",
     "osmnx",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
-    "pyvista==0.38.5",
+    "pyvista==0.38.6",
     "recommonmark==0.7.1",
     "scikit-learn==1.2.2",
-    "Sphinx==6.2.1",
+    "Sphinx==7.0.0",
     "sphinx-autobuild==2021.3.14",
     "sphinx-autodoc-typehints==1.23.0",
     "sphinx-copybutton==0.5.2",
     "sphinx-gallery==0.13.0",
     "sphinx-notfound-page==0.8.3",
     "sphinxcontrib-websupport==1.2.4",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 full = [
+    "imageio==2.28.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.1; python_version > '3.7'",
     "osmnx",
-    "pyvista==0.38.5",
+    "pyvista==0.38.6",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 all = [
+    "imageio==2.28.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.1; python_version > '3.7'",
     "osmnx",
-    "pyvista==0.38.5",
+    "pyvista==0.38.6",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 
 [tool.flit.module]
```

### Comparing `pyaedt-0.6.73/PKG-INFO` & `pyaedt-0.6.74/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.6.73
+Version: 0.6.74
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -17,368 +17,318 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: cffi == 1.15.1;platform_system=='Linux'
 Requires-Dist: pywin32 >= 303;platform_system=='Windows'
 Requires-Dist: pythonnet == 3.0.1
 Requires-Dist: rpyc==5.3.1
 Requires-Dist: psutil
 Requires-Dist: dotnetcore2 ==3.1.23;platform_system=='Linux'
+Requires-Dist: imageio==2.28.0 ; extra == "all"
 Requires-Dist: matplotlib==3.5.3 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: pandas==1.3.5 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "all"
-Requires-Dist: pyvista==0.38.5 ; extra == "all"
+Requires-Dist: pyvista==0.38.6 ; extra == "all"
 Requires-Dist: SRTM.py ; extra == "all"
 Requires-Dist: utm ; extra == "all"
 Requires-Dist: scikit-rf ; extra == "all"
 Requires-Dist: openpyxl==3.1.2 ; extra == "all"
 Requires-Dist: ansys-sphinx-theme==0.9.8 ; extra == "doc"
 Requires-Dist: imageio==2.28.0 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
-Requires-Dist: ipython==8.12.0 ; extra == "doc"
+Requires-Dist: ipython==8.13.0 ; extra == "doc"
 Requires-Dist: ipywidgets==8.0.6 ; extra == "doc"
 Requires-Dist: joblib==1.2.0 ; extra == "doc"
 Requires-Dist: jupyterlab==3.6.3 ; extra == "doc"
 Requires-Dist: matplotlib==3.5.3 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: nbsphinx==0.9.1 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: osmnx ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
-Requires-Dist: pyvista==0.38.5 ; extra == "doc"
+Requires-Dist: pyvista==0.38.6 ; extra == "doc"
 Requires-Dist: recommonmark==0.7.1 ; extra == "doc"
 Requires-Dist: scikit-learn==1.2.2 ; extra == "doc"
-Requires-Dist: Sphinx==6.2.1 ; extra == "doc"
+Requires-Dist: Sphinx==7.0.0 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.23.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: SRTM.py ; extra == "doc"
 Requires-Dist: utm ; extra == "doc"
 Requires-Dist: scikit-rf ; extra == "doc"
 Requires-Dist: openpyxl==3.1.2 ; extra == "doc"
+Requires-Dist: imageio==2.28.0 ; extra == "full"
 Requires-Dist: matplotlib==3.5.3 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: pandas==1.3.5 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "full"
-Requires-Dist: pyvista==0.38.5 ; extra == "full"
+Requires-Dist: pyvista==0.38.6 ; extra == "full"
 Requires-Dist: SRTM.py ; extra == "full"
 Requires-Dist: utm ; extra == "full"
 Requires-Dist: scikit-rf ; extra == "full"
 Requires-Dist: openpyxl==3.1.2 ; extra == "full"
-Requires-Dist: ipython==8.12.0 ; extra == "tests"
+Requires-Dist: ipython==8.13.0 ; extra == "tests"
+Requires-Dist: imageio==2.28.0 ; extra == "tests"
 Requires-Dist: joblib==1.2.0 ; extra == "tests"
 Requires-Dist: matplotlib==3.5.3 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: openpyxl==3.1.2 ; extra == "tests"
 Requires-Dist: osmnx ; extra == "tests"
 Requires-Dist: pandas==1.3.5 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pytest==7.3.1 ; extra == "tests"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
 Requires-Dist: pytest-xdist==3.2.1 ; extra == "tests"
-Requires-Dist: pyvista==0.38.5 ; extra == "tests"
+Requires-Dist: pyvista==0.38.6 ; extra == "tests"
 Requires-Dist: scikit-learn==1.2.2 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
 Requires-Dist: utm ; extra == "tests"
 Requires-Dist: scikit-rf ; extra == "tests"
 Project-URL: Bug Tracker, https://github.com/pyansys/pyaedt/issues
 Project-URL: Documentation, https://aedt.docs.pyansys.com
 Project-URL: Source Code, https://github.com/pyansys/pyaedt
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: full
 Provides-Extra: tests
 
-PyAEDT
-======
+<!-- -->
+<a name="readme-top"></a>
+<!--
+*** PyAEDT README
+-->
 
-|pyansys| |pypi| |PyPIact| |PythonVersion| |GH-CI| |codecov| |MIT| |black| |Anaconda| |pre-commit|
 
-.. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
-   :target: https://docs.pyansys.com/
-   :alt: PyAnsys
+# PyAEDT
 
-.. |pypi| image:: https://img.shields.io/pypi/v/pyaedt.svg?logo=python&logoColor=white
-   :target: https://pypi.org/project/pyaedt/
+<p style="text-align: center;">
+    <br> English | <a href="README_CN.md">中文</a>
+</p>
 
-.. |PyPIact|  image:: https://pepy.tech/badge/pyaedt/month
-   :target: https://pypi.org/project/pyaedt/
+[![PyAnsys](https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC)](https://docs.pyansys.com/)[![pypi](https://img.shields.io/pypi/v/pyaedt.svg?logo=python&logoColor=white)](https://pypi.org/project/pyaedt/)[![PyPIact](https://pepy.tech/badge/pyaedt/month)](https://pypi.org/project/pyaedt/)[![PythonVersion](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)[![GH-CI](https://github.com/pyansys/pyaedt/actions/workflows/unit_tests.yml/badge.svg)](https://github.com/pyansys/pyaedt/actions/workflows/unit_tests.yml)[![codecov](https://codecov.io/gh/pyansys/pyaedt/branch/main/graph/badge.svg)](https://codecov.io/gh/pyansys/pyaedt)[![MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black)[![Anaconda](https://anaconda.org/conda-forge/pyaedt/badges/version.svg)](https://anaconda.org/conda-forge/pyaedt)[![pre-commit](https://results.pre-commit.ci/badge/github/pyansys/pyaedt/main.svg)](https://results.pre-commit.ci/latest/github/pyansys/pyaedt/main)
 
-.. |PythonVersion| image:: https://img.shields.io/badge/python-3.7+-blue.svg
-   :target: https://www.python.org/downloads/
+## What is PyAEDT?
 
-.. |GH-CI| image:: https://github.com/pyansys/pyaedt/actions/workflows/unit_tests.yml/badge.svg
-   :target: https://github.com/pyansys/pyaedt/actions/workflows/unit_tests.yml
-
-.. |codecov| image:: https://codecov.io/gh/pyansys/pyaedt/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/pyansys/pyaedt
-
-.. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
-   :target: https://opensource.org/licenses/MIT
-
-.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
-  :target: https://github.com/psf/black
-  :alt: black
-
-.. |Anaconda| image:: https://anaconda.org/conda-forge/pyaedt/badges/version.svg
-  :target: https://anaconda.org/conda-forge/pyaedt
-
-.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/pyansys/pyaedt/main.svg
-   :target: https://results.pre-commit.ci/latest/github/pyansys/pyaedt/main
-   :alt: pre-commit.ci status
-
-
-What is PyAEDT?
----------------
-PyAEDT is a Python library that interacts directly with the API for
+`PyAEDT` is a Python library that interacts directly with the API for
 Ansys Electronics Desktop (AEDT) to make scripting simpler. The architecture
 for PyAEDT can be reused for all AEDT 3D products (HFSS, Icepak, Maxwell 3D,
 and Q3D Extractor), 2D tools, and Ansys Mechanical. PyAEDT also provides
 support for circuit tools like Nexxim and system simulation tools like
 Twin Builder. Finally, PyAEDT provides scripting capabilities in Ansys layout
 tools like HFSS 3D Layout and EDB. The PyAEDT class and method structures
 simplify operation while reusing information as much as possible across
 the API.
 
-Install on CPython from PyPI
-----------------------------
-You can install PyAEDT on CPython 3.7 through 3.10 from PyPI with this command:
-
-.. code:: python
-
-    pip install pyaedt
-
-To install PyAEDT with all extra packages (Matplotlib, NumPy, Pandas, and PyVista),
-use this command:
+## Install on CPython from PyPI
 
-.. code:: python
+You can install PyAEDT on CPython 3.7 through 3.10 from PyPI with this command:
 
-    pip install pyaedt[full]
+```sh
+  pip install pyaedt
+```
+
+Install `PyAEDT` with all extra packages (matplotlib, numpy, pandas, pyvista):
+
+```sh
+  pip install pyaedt[full]
+```
 
 You can also install PyAEDT from Conda-Forge with this command:
 
-.. code:: python
-
-    conda install -c conda-forge pyaedt
-
+```sh
+  conda install -c conda-forge pyaedt
+```
 PyAEDT remains compatible with IronPython and can be still used in the AEDT Framework.
 
-About PyAnsys
--------------
+## About PyAnsys
 
-PyAEDT is part of the larger `PyAnsys <https://docs.pyansys.com>`_
-effort to facilitate the use of Ansys technologies directly from Python.
+`PyAEDT` is part of the larger [PyAnsys](https://docs.pyansys.com "PyAnsys") effort to facilitate the use of Ansys technologies directly from Python.
 
 PyAEDT is intended to consolidate and extend all existing
 functionalities around scripting for AEDT to allow reuse of existing code,
 sharing of best practices, and increased collaboration.
 
+## About AEDT
 
-About AEDT
-----------
-
-`AEDT <https://www.ansys.com/products/electronics>`_ is a platform that enables true
+[AEDT](https://www.ansys.com/products/electronics) is a platform that enables true
 electronics system design. AEDT provides access to the Ansys gold-standard
 electro-magnetics simulation solutions, such as Ansys HFSS, Ansys Maxwell,
 Ansys Q3D Extractor, Ansys Siwave, and Ansys Icepak using electrical CAD (ECAD) and
 Mechanical CAD (MCAD) workflows.
 
 In addition, AEDT includes direct links to the complete Ansys portfolio of thermal, fluid,
 and mechanical solvers for comprehensive multiphysics analysis.
 Tight integration among these solutions provides unprecedented ease of use for setup and
 faster resolution of complex simulations for design and optimization.
 
-.. image:: https://images.ansys.com/is/image/ansys/ansys-electronics-technology-collage?wid=941&op_usm=0.9,1.0,20,0&fit=constrain,0
-  :width: 800
-  :alt: AEDT Applications
-  :target: https://www.ansys.com/products/electronics
-
-
-PyAEDT is licensed under the `MIT License
-<https://github.com/pyansys/PyAEDT/blob/main/LICENSE>`_.
-
-PyAEDT includes functionality for interacting with the following AEDT tools and Ansys products:
-
-- HFSS and HFSS 3D Layout
-- Icepak
-- Maxwell 2D, Maxwell 3D, and RMXprt
-- 2D Extractor and Q3D Extractor
-- Mechanical
-- Nexxim
-- EDB
-- Twin Builder
-
-
-Documentation and issues
-------------------------
-Documentation for the latest stable release of PyAEDT is hosted at
-`PyAEDT Documentation <https://aedt.docs.pyansys.com/version/stable/>`_.
+<p align="center">
+  <img width="100%" src="https://images.ansys.com/is/image/ansys/ansys-electronics-technology-collage?wid=941&op_usm=0.9,1.0,20,0&fit=constrain,0" title="AEDT Applications" herf="https://www.ansys.com/products/electronics"
+  />
+</p>
+
+`PyAEDT` is licensed under the [MIT License](https://github.com/pyansys/PyAEDT/blob/main/LICENSE)
+
+`PyAEDT` includes functionality for interacting with the following `AEDT tools` and `Ansys products`:
+
+  - HFSS and HFSS 3D Layout
+  - Icepak
+  - Maxwell 2D, Maxwell 3D, and RMXprt
+  - 2D Extractor and Q3D Extractor
+  - Mechanical
+  - Nexxim
+  - EDB
+  - Twin Builder
+
+## Documentation and issues
+
+In addition to installation and usage information, the `PyAEDT` documentation provides [API reference](https://aedt.docs.pyansys.com/version/stable), [Examples](https://aedt.docs.pyansys.com/version/stable/examples/index.html), and [Contribute](https://aedt.docs.pyansys.com/version/stable/Contributing.html) sections.
 
 In the upper right corner of the documentation's title bar, there is an option
 for switching from viewing the documentation for the latest stable release
 to viewing the documentation for the development version or previously
 released versions.
 
-On the `PyAEDT Issues <https://github.com/pyansys/PyAEDT/issues>`_ page, you can
+On the [PyAEDT Issues](https://github.com/pyansys/PyAEDT/issues) page, you can
 create issues to submit questions, report bugs, and request new features.
 
 To reach the project support team, email `pyansys.core@ansys.com <pyansys.core@ansys.com>`_.
 
-Dependencies
-------------
-To run PyAEDT, you must have a local licensed copy of AEDT.
-PyAEDT supports AEDT versions 2022 R1 and later.
-
-Student version
----------------
-
-PyAEDT supports AEDT Student versions 2022 R1 and later. For more information, see
-`Ansys Electronics Desktop Student  - Free Software Download <https://www.ansys.com/academic/students/ansys-e
-lectronics-desktop-student>`_ on the Ansys website.
-
-
-Why PyAEDT?
------------
-A quick and easy approach for automating a simple operation in the 
-AEDT UI is to record and reuse a script. However, here are some disadvantages of 
-this approach:
-
-- Recorded code is dirty and difficult to read and understand.
-- Recorded scripts are difficult to reuse and adapt.
-- Complex coding is required by many global users of AEDT.
-
-Here are the main advantages that PyAEDT provides:
-
-- Automatic initialization of all AEDT objects, such as desktop
-  objects like the editor, boundaries, and more
-- Error management
-- Log management
-- Variable management
-- Compatibility with IronPython and CPython
-- Simplification of complex API syntax using data objects while
-  maintaining PEP8 compliance.
-- Code reusability across different solvers
-- Clear documentation on functions and API
-- Unit tests of code to increase quality across different AEDT versions
-
-
-Example workflow
------------------
-1. Initialize the ``Desktop`` class with the version of AEDT to use.
-2. Initialize the application to use within AEDT.
-
-
-Connect to AEDT from a Python IDE
----------------------------------
-PyAEDT works both inside AEDT and as a standalone app.
-This Python library automatically detects whether it is running
-in an IronPython or CPython environment and initializes AEDT accordingly.
-PyAEDT also provides advanced error management. Usage examples follow.
+## Dependencies
+
+To run `PyAEDT`, you must have a local licenced copy of AEDT.
+`PyAEDT` supports AEDT versions 2022 R1 or newer.
+
+## Student version
+
+`PyAEDT` supports `AEDT Student version 2022 R1` and later. For more information, see [Student Version page](https://www.ansys.com/academic/students/ansys-electronics-desktop-student).
+
+## Why PyAEDT?
 
-Explicit AEDT declaration and error management
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+A quick and easy approach for automating a simple operation in the AEDT UI is to record and reuse a script. However, disadvantages of this approach are:
 
-.. code:: python
+  - Recorded code is dirty and difficult to read and understand.
+  - Recorded scripts are difficult to reuse and adapt.
+  - Complex coding is required by many global users of `AEDT`.
 
-    # Launch AEDT 2023 R1 in non-graphical mode
+The main advantages of `PyAEDT` are:
+
+  - Automatic initialization of all `AEDT` objects, such as desktop objects like the editor, boundaries, and so on
+  - Error management
+  - Log management
+  - Variable management
+  - Compatibility with IronPython and CPython
+  - Simplification of complex API syntax using data objects while maintaining PEP8 compliance.
+  - Code reusability across different solvers
+  - Clear documentation on functions and API
+  - Unit tests of code to increase quality across different AEDT versions
+
+## Example workflow
+
+ 1. Initialize the ``Desktop`` class with the version of `AEDT` to use.
+ 2. Initialize the application to use within `AEDT`.
+
+## Connect to AEDT from Python IDE
+
+``PyAEDT`` works both inside AEDT and as a standalone application. This Python library automatically detects whether it is running in an IronPython or CPython environment and initializes AEDT accordingly.
+``PyAEDT`` also provides advanced error management. Usage examples follow.
+
+## Explicit AEDT declaration and error management
+
+``` python
+    # Launch AEDT 2022 R2 in non-graphical mode
 
     from pyaedt import Desktop, Circuit
-    with Desktop(specified_version="2023.1",
+    with Desktop(specified_version="2022.2",
                  non_graphical=False, new_desktop_session=True,
                  close_on_exit=True, student_version=False):
         circuit = Circuit()
         ...
         # Any error here will be caught by Desktop.
         ...
 
     # Desktop is automatically released here.
+```
 
+## Implicit AEDT declaration and error management
 
-Implicit AEDT declaration and error management
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-.. code:: python
-
+``` python
     # Launch the latest installed version of AEDT in graphical mode
 
     from pyaedt import Circuit
-    with Circuit(specified_version="2023.1",
+    with Circuit(specified_version="2022.2",
                  non_graphical=False) as circuit:
         ...
         # Any error here will be caught by Desktop.
         ...
 
     # Desktop is automatically released here.
+```
 
+## Remote application call
 
-Remote application call
-~~~~~~~~~~~~~~~~~~~~~~~
 You can make a remote application call on a CPython server
 or any Windows client machine.
 
-On a CPython server:
-
-.. code:: python
+On a CPython Server:
 
+``` python
     # Launch PyAEDT remote server on CPython
 
     from pyaedt.common_rpc import pyaedt_service_manager
     pyaedt_service_manager()
-
+```
 
 On any Windows client machine:
 
-.. code:: python
-
+``` python
     from pyaedt.common_rpc import create_session
     cl1 = create_session("server_name")
     cl1.aedt(port=50000, non_graphical=False)
     hfss = Hfss(machine="server_name", port=50000)
     # your code here
+```
 
-Variables
-~~~~~~~~~
-
-.. code:: python
+## Variables
 
+``` python
     from pyaedt.HFSS import HFSS
     with HFSS as hfss:
          hfss["dim"] = "1mm"   # design variable
          hfss["$dim"] = "1mm"  # project variable
+```
 
+## Modeler
 
-Modeler
-~~~~~~~
-
-.. code:: python
-
+``` python
     # Create a box, assign variables, and assign materials.
 
     from pyaedt.hfss import Hfss
     with Hfss as hfss:
          hfss.modeler.create_box([0, 0, 0], [10, "dim", 10],
                                  "mybox", "aluminum")
+```
+
+## License
+
+`PyAEDT` is licensed under the `MIT` license.
+
+This module makes no commercial claim over Ansys whatsoever. `PyAEDT` extends the functionality of `AEDT` by adding an additional Python interface to `AEDT` without changing the core behavior or license of the original software. The use of the interactive control of `PyAEDT` requires a legally licensed local copy of `AEDT`. For more information about `AEDT`, visit the [AEDT page](https://www.ansys.com/products/electronics) on the `Ansys` website.
+
+<p style="text-align: right;"> <a href="#readme-top">back to top</a> </p>
+
+## Indices and tables
 
-License
--------
-PyAEDT is licensed under the MIT license.
-
-This module makes no commercial claim over Ansys whatsoever.
-PyAEDT extends the functionality of AEDT by adding
-an additional Python interface to AEDT without changing the core
-behavior or license of the original software. The use of the
-interactive control of PyAEDT requires a legally licensed
-local copy of AEDT. For more information about AEDT, 
-see the `Ansys Electronics <https://www.ansys.com/products/electronics>`_ 
-page on the Ansys website.
+-  [Index](https://aedt.docs.pyansys.com/version/stable/genindex.html)
+-  [Module Index](https://aedt.docs.pyansys.com/version/stable/py-modindex.html)
+-  [Search Page](https://aedt.docs.pyansys.com/version/stable/search.html)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

