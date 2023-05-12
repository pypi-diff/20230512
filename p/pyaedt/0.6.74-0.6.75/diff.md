# Comparing `tmp/pyaedt-0.6.74.tar.gz` & `tmp/pyaedt-0.6.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.6.74.tar", last modified: Fri May  5 15:05:33 2023, max compression
+gzip compressed data, was "pyaedt-0.6.75.tar", last modified: Fri May 12 16:29:05 2023, max compression
```

## Comparing `pyaedt-0.6.74.tar` & `pyaedt-0.6.75.tar`

### file list

```diff
@@ -1,251 +1,252 @@
--rw-r--r--   0        0        0     1111 2023-04-27 10:48:38.937375 pyaedt-0.6.74/LICENSE
--rw-r--r--   0        0        0     9947 2023-05-04 17:35:03.992963 pyaedt-0.6.74/README.md
--rw-r--r--   0        0        0     2634 2023-05-05 14:48:17.527685 pyaedt-0.6.74/pyaedt/__init__.py
--rw-r--r--   0        0        0    26253 2023-04-27 10:48:40.495559 pyaedt-0.6.74/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6965 2023-04-27 10:48:40.495559 pyaedt-0.6.74/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    89212 2023-05-03 07:06:47.305842 pyaedt-0.6.74/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    41260 2023-05-04 22:05:14.854681 pyaedt-0.6.74/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    17009 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3088 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    19795 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4374 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4539 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   127521 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6115 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    75493 2023-04-27 13:08:15.716301 pyaedt-0.6.74/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12433 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    37014 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    57605 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/circuit.py
--rw-r--r--   0        0        0    10034 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    57391 2023-05-04 12:03:46.353459 pyaedt-0.6.74/pyaedt/desktop.py
--rw-r--r--   0        0        0    15104 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/dlls/PDFReport/AnsysReport.deps.json
--rw-r--r--   0        0        0    23552 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/dlls/PDFReport/AnsysReport.dll
--rw-r--r--   0        0        0     1092 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/dlls/PDFReport/AnsysTemplate.json
--rw-r--r--   0        0        0   204800 2023-04-27 10:48:40.511198 pyaedt-0.6.74/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
--rw-r--r--   0        0        0   577445 2023-04-27 10:48:40.526826 pyaedt-0.6.74/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
--rw-r--r--   0        0        0     9836 2023-04-27 10:48:40.526826 pyaedt-0.6.74/pyaedt/dlls/PDFReport/Images/Ansys.png
--rw-r--r--   0        0        0   238592 2023-04-27 10:48:40.526826 pyaedt-0.6.74/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
--rw-r--r--   0        0        0   115712 2023-04-27 10:48:40.526826 pyaedt-0.6.74/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
--rw-r--r--   0        0        0   705296 2023-04-27 10:48:40.526826 pyaedt-0.6.74/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
--rw-r--r--   0        0        0   712253 2023-04-27 10:48:40.542451 pyaedt-0.6.74/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
--rw-r--r--   0        0        0    80384 2023-04-27 10:48:40.542451 pyaedt-0.6.74/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
--rw-r--r--   0        0        0   546816 2023-04-27 10:48:40.542451 pyaedt-0.6.74/pyaedt/dlls/PDFReport/PdfSharpCore.dll
--rw-r--r--   0        0        0   367616 2023-04-27 10:48:40.542451 pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
--rw-r--r--   0        0        0   536367 2023-04-27 10:48:40.558076 pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
--rw-r--r--   0        0        0  1229824 2023-04-27 10:48:40.558076 pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
--rw-r--r--   0        0        0  3285773 2023-04-27 10:48:40.589270 pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
--rw-r--r--   0        0        0   120664 2023-04-27 10:48:40.589270 pyaedt-0.6.74/pyaedt/dlls/PDFReport/System.Runtime.dll
--rw-r--r--   0        0        0  1505294 2023-04-27 10:48:40.589270 pyaedt-0.6.74/pyaedt/dlls/PDFReport/System.Runtime.xml
--rw-r--r--   0        0        0     5632 2023-04-27 10:48:40.589270 pyaedt-0.6.74/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
--rw-r--r--   0        0        0   160754 2023-04-27 10:48:40.589270 pyaedt-0.6.74/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
--rw-r--r--   0        0        0    23386 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/downloads.py
--rw-r--r--   0        0        0   132412 2023-04-28 08:23:04.967029 pyaedt-0.6.74/pyaedt/edb.py
--rw-r--r--   0        0        0      333 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/__init__.py
--rw-r--r--   0        0        0    92729 2023-05-04 13:41:54.201025 pyaedt-0.6.74/pyaedt/edb_core/components.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    32856 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0      937 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0      324 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/edb_builder.py
--rw-r--r--   0        0        0     1166 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    12141 2023-04-28 22:06:54.714447 pyaedt-0.6.74/pyaedt/edb_core/edb_data/hfss_extent_info.py
--rw-r--r--   0        0        0    65580 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    20305 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     4724 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    61111 2023-04-27 15:58:46.158994 pyaedt-0.6.74/pyaedt/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0    32298 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0    99826 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    36282 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    31276 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0     4147 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     2425 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     3258 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/general.py
--rw-r--r--   0        0        0    60863 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/hfss.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.604919 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0      673 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     1283 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     2213 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0      524 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/__init__.py
--rw-r--r--   0        0        0      768 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/color.py
--rw-r--r--   0        0        0     2118 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/content.py
--rw-r--r--   0        0        0      938 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0      921 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     1029 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0      416 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0      548 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0      523 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/fill.py
--rw-r--r--   0        0        0      284 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     2844 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     1183 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     1319 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     1516 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0      960 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     1964 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     1158 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     7706 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0      921 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     1079 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     4646 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     1440 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0      875 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     2775 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0      887 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     4104 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     2567 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     1002 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8010 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0      663 2023-04-27 10:48:40.620538 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     1162 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     1626 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0      838 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    11333 2023-05-02 12:25:34.524335 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     1033 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0      683 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     2008 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     1624 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/history_record.py
--rw-r--r--   0        0        0    21750 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ipc2581.py
--rw-r--r--   0        0        0      966 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/ipc2581/logistic_header.py
--rw-r--r--   0        0        0    49064 2023-05-02 10:24:55.037694 pyaedt-0.6.74/pyaedt/edb_core/layout.py
--rw-r--r--   0        0        0    33242 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/materials.py
--rw-r--r--   0        0        0    43680 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/nets.py
--rw-r--r--   0        0        0    46611 2023-05-02 13:33:56.688526 pyaedt-0.6.74/pyaedt/edb_core/padstack.py
--rw-r--r--   0        0        0    57133 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/edb_core/siwave.py
--rw-r--r--   0        0        0   108893 2023-04-28 08:23:04.982656 pyaedt-0.6.74/pyaedt/edb_core/stackup.py
--rw-r--r--   0        0        0    11275 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/emit.py
--rw-r--r--   0        0        0     3555 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     3291 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/emit_core/EmitConstants.py
--rw-r--r--   0        0        0     1074 2023-05-03 22:08:43.552442 pyaedt-0.6.74/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0        2 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7406 2023-05-03 22:08:43.552442 pyaedt-0.6.74/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    11154 2023-05-03 22:08:43.552442 pyaedt-0.6.74/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0    14317 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    11758 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.636162 pyaedt-0.6.74/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     3257 2023-04-28 11:15:19.829287 pyaedt-0.6.74/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    83387 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28645 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    19616 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0     3416 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    67564 2023-05-05 10:19:45.526526 pyaedt-0.6.74/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0    25808 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     6989 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0     9795 2023-04-28 11:15:19.829287 pyaedt-0.6.74/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    62296 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    11301 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/process.py
--rw-r--r--   0        0        0    19736 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3466 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    60355 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/toolkit.py
--rw-r--r--   0        0        0    17095 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0      438 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/generic/wpf_template.xaml
--rw-r--r--   0        0        0   252855 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/hfss.py
--rw-r--r--   0        0        0    82916 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   154940 2023-05-04 12:57:05.488766 pyaedt-0.6.74/pyaedt/icepak.py
--rw-r--r--   0        0        0   118433 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7803 2023-04-27 10:48:40.651785 pyaedt-0.6.74/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24259 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3035 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     3695 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     2380 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0       53 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    10210 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     3731 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     3829 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0      678 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-04-27 10:48:40.667417 pyaedt-0.6.74/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      953 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0      868 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14076 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    19994 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18513 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16809 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   120831 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0   194513 2023-04-28 22:06:54.714447 pyaedt-0.6.74/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   115253 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    11332 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   127838 2023-05-05 12:50:06.063040 pyaedt-0.6.74/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.683090 pyaedt-0.6.74/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    31549 2023-05-05 11:21:28.656568 pyaedt-0.6.74/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49002 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59516 2023-05-04 12:57:05.488766 pyaedt-0.6.74/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53100 2023-04-28 22:06:54.714447 pyaedt-0.6.74/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12588 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    42270 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    32270 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8157 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    63043 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15094 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    31983 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    68020 2023-04-28 22:06:54.714447 pyaedt-0.6.74/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6897 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    52430 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    31270 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    49837 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    65608 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    21640 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    30094 2023-04-27 10:48:40.698662 pyaedt-0.6.74/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   114236 2023-05-04 10:13:14.811305 pyaedt-0.6.74/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71549 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    51910 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    40297 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0    82846 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    28306 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53168 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11919 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    26048 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   172808 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    64104 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   119621 2023-05-04 08:14:06.606295 pyaedt-0.6.74/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    33226 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    28652 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   103276 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   125048 2023-05-04 22:05:14.870254 pyaedt-0.6.74/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    95482 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/q3d.py
--rw-r--r--   0        0        0    10556 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.714291 pyaedt-0.6.74/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    40721 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9425 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7601 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    10373 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/siwave.py
--rw-r--r--   0        0        0    10527 2023-04-27 10:48:40.729916 pyaedt-0.6.74/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     4134 2023-05-05 10:19:45.542100 pyaedt-0.6.74/pyproject.toml
--rw-r--r--   0        0        0    15129 1970-01-01 00:00:00.000000 pyaedt-0.6.74/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-03-24 16:10:16.742763 pyaedt-0.6.75/LICENSE
+-rw-r--r--   0        0        0     9947 2023-05-04 14:08:42.179957 pyaedt-0.6.75/README.md
+-rw-r--r--   0        0        0     2634 2023-05-12 15:52:06.115764 pyaedt-0.6.75/pyaedt/__init__.py
+-rw-r--r--   0        0        0    26253 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6965 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    89244 2023-05-12 14:39:14.493618 pyaedt-0.6.75/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    41260 2023-05-04 22:05:09.593531 pyaedt-0.6.75/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    17009 2023-04-06 11:56:42.332868 pyaedt-0.6.75/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3088 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    19795 2023-04-06 11:56:42.332868 pyaedt-0.6.75/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4374 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4539 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   127521 2023-04-27 08:03:43.579230 pyaedt-0.6.75/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6115 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    75493 2023-04-27 13:10:02.023398 pyaedt-0.6.75/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12433 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    37014 2023-03-24 16:10:18.742581 pyaedt-0.6.75/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    57603 2023-05-11 09:46:53.726038 pyaedt-0.6.75/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10034 2023-03-24 16:10:18.758234 pyaedt-0.6.75/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    57391 2023-05-04 10:56:05.337017 pyaedt-0.6.75/pyaedt/desktop.py
+-rw-r--r--   0        0        0    15104 2023-04-27 07:01:19.524177 pyaedt-0.6.75/pyaedt/dlls/PDFReport/AnsysReport.deps.json
+-rw-r--r--   0        0        0    23552 2023-04-27 07:01:19.524177 pyaedt-0.6.75/pyaedt/dlls/PDFReport/AnsysReport.dll
+-rw-r--r--   0        0        0     1092 2023-04-27 07:01:19.524177 pyaedt-0.6.75/pyaedt/dlls/PDFReport/AnsysTemplate.json
+-rw-r--r--   0        0        0   204800 2023-04-27 07:01:19.539803 pyaedt-0.6.75/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
+-rw-r--r--   0        0        0   577445 2023-04-27 07:01:19.539803 pyaedt-0.6.75/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
+-rw-r--r--   0        0        0     9836 2023-04-27 07:01:19.539803 pyaedt-0.6.75/pyaedt/dlls/PDFReport/Images/Ansys.png
+-rw-r--r--   0        0        0   238592 2023-04-27 07:01:19.539803 pyaedt-0.6.75/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
+-rw-r--r--   0        0        0   115712 2023-04-27 07:01:19.539803 pyaedt-0.6.75/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
+-rw-r--r--   0        0        0   705296 2023-04-27 07:01:19.555426 pyaedt-0.6.75/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
+-rw-r--r--   0        0        0   712253 2023-04-27 07:01:19.555426 pyaedt-0.6.75/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
+-rw-r--r--   0        0        0    80384 2023-04-27 07:01:19.555426 pyaedt-0.6.75/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
+-rw-r--r--   0        0        0   546816 2023-04-27 07:01:19.571050 pyaedt-0.6.75/pyaedt/dlls/PDFReport/PdfSharpCore.dll
+-rw-r--r--   0        0        0   367616 2023-04-27 07:01:19.571050 pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
+-rw-r--r--   0        0        0   536367 2023-04-27 07:01:19.571050 pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
+-rw-r--r--   0        0        0  1229824 2023-04-27 07:01:19.586676 pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
+-rw-r--r--   0        0        0  3285773 2023-04-27 07:01:19.602300 pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
+-rw-r--r--   0        0        0   120664 2023-04-27 07:01:19.602300 pyaedt-0.6.75/pyaedt/dlls/PDFReport/System.Runtime.dll
+-rw-r--r--   0        0        0  1505294 2023-04-27 07:01:19.617927 pyaedt-0.6.75/pyaedt/dlls/PDFReport/System.Runtime.xml
+-rw-r--r--   0        0        0     5632 2023-04-27 07:01:19.617927 pyaedt-0.6.75/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
+-rw-r--r--   0        0        0   160754 2023-04-27 07:01:19.617927 pyaedt-0.6.75/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
+-rw-r--r--   0        0        0    23386 2023-04-18 21:46:42.426459 pyaedt-0.6.75/pyaedt/downloads.py
+-rw-r--r--   0        0        0   134259 2023-05-12 14:39:14.493618 pyaedt-0.6.75/pyaedt/edb.py
+-rw-r--r--   0        0        0      333 2023-04-06 16:51:57.478550 pyaedt-0.6.75/pyaedt/edb_core/__init__.py
+-rw-r--r--   0        0        0    92731 2023-05-12 14:39:14.493618 pyaedt-0.6.75/pyaedt/edb_core/components.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.820698 pyaedt-0.6.75/pyaedt/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    32856 2023-04-06 17:43:43.595268 pyaedt-0.6.75/pyaedt/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0    40043 2023-05-12 14:39:14.493618 pyaedt-0.6.75/pyaedt/edb_core/edb_data/control_file.py
+-rw-r--r--   0        0        0      937 2023-03-24 16:10:18.820698 pyaedt-0.6.75/pyaedt/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0      324 2023-03-24 16:10:18.820698 pyaedt-0.6.75/pyaedt/edb_core/edb_data/edb_builder.py
+-rw-r--r--   0        0        0     1166 2023-03-24 16:10:18.820698 pyaedt-0.6.75/pyaedt/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    12141 2023-04-28 15:10:16.972093 pyaedt-0.6.75/pyaedt/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    65580 2023-04-13 10:23:17.415379 pyaedt-0.6.75/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    20305 2023-04-06 16:51:57.478550 pyaedt-0.6.75/pyaedt/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     4724 2023-04-17 09:21:51.433903 pyaedt-0.6.75/pyaedt/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    61111 2023-04-27 17:41:51.680530 pyaedt-0.6.75/pyaedt/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0    32298 2023-04-06 16:51:57.478550 pyaedt-0.6.75/pyaedt/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0    99826 2023-04-25 22:05:43.936271 pyaedt-0.6.75/pyaedt/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    36282 2023-04-25 22:05:43.936271 pyaedt-0.6.75/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    33728 2023-05-09 13:57:21.715124 pyaedt-0.6.75/pyaedt/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0     4147 2023-03-24 16:10:18.820698 pyaedt-0.6.75/pyaedt/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     2425 2023-03-27 19:28:28.383108 pyaedt-0.6.75/pyaedt/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     3258 2023-04-25 22:05:43.936271 pyaedt-0.6.75/pyaedt/edb_core/general.py
+-rw-r--r--   0        0        0    60863 2023-04-25 22:05:43.936271 pyaedt-0.6.75/pyaedt/edb_core/hfss.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0      673 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     1283 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     2213 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0      524 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0      768 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/color.py
+-rw-r--r--   0        0        0     2118 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/content.py
+-rw-r--r--   0        0        0      938 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0      921 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     1029 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0      416 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0      548 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0      523 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/fill.py
+-rw-r--r--   0        0        0      284 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     2844 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     1183 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     1319 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     1516 2023-03-24 16:10:18.836323 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0      960 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     1964 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     1158 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     7706 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0      921 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     1079 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     4646 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     1440 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0      875 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     2775 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0      887 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     4104 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     2567 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     1002 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8010 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0      663 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     1162 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     1626 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0      838 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    11333 2023-05-02 12:13:55.192015 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     1033 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0      683 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     2008 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     1624 2023-03-24 16:10:18.851970 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/history_record.py
+-rw-r--r--   0        0        0    21750 2023-04-03 14:45:49.232236 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0      966 2023-03-24 16:10:18.867622 pyaedt-0.6.75/pyaedt/edb_core/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0    49064 2023-05-02 12:59:04.166088 pyaedt-0.6.75/pyaedt/edb_core/layout.py
+-rw-r--r--   0        0        0    33242 2023-04-07 10:17:20.946469 pyaedt-0.6.75/pyaedt/edb_core/materials.py
+-rw-r--r--   0        0        0    43680 2023-04-06 17:49:40.538145 pyaedt-0.6.75/pyaedt/edb_core/nets.py
+-rw-r--r--   0        0        0    46611 2023-05-09 09:08:50.766572 pyaedt-0.6.75/pyaedt/edb_core/padstack.py
+-rw-r--r--   0        0        0    57133 2023-04-06 16:51:57.478550 pyaedt-0.6.75/pyaedt/edb_core/siwave.py
+-rw-r--r--   0        0        0   108893 2023-04-28 11:15:40.689926 pyaedt-0.6.75/pyaedt/edb_core/stackup.py
+-rw-r--r--   0        0        0    11275 2023-04-26 16:24:45.451996 pyaedt-0.6.75/pyaedt/emit.py
+-rw-r--r--   0        0        0     3555 2023-03-24 16:10:18.867622 pyaedt-0.6.75/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     3291 2023-04-25 22:05:43.951906 pyaedt-0.6.75/pyaedt/emit_core/EmitConstants.py
+-rw-r--r--   0        0        0     1074 2023-05-03 22:08:50.820887 pyaedt-0.6.75/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0        2 2023-03-24 16:10:18.867622 pyaedt-0.6.75/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7406 2023-05-03 22:08:50.820887 pyaedt-0.6.75/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    12191 2023-05-12 15:07:06.269545 pyaedt-0.6.75/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0    14317 2023-03-27 12:10:05.425190 pyaedt-0.6.75/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    11758 2023-03-24 16:10:18.867622 pyaedt-0.6.75/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.867622 pyaedt-0.6.75/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     3257 2023-04-28 11:15:40.689926 pyaedt-0.6.75/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    83387 2023-04-26 10:50:39.177934 pyaedt-0.6.75/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28645 2023-04-07 12:58:03.133395 pyaedt-0.6.75/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    21891 2023-05-12 14:39:14.493618 pyaedt-0.6.75/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0     3416 2023-03-30 13:11:17.942263 pyaedt-0.6.75/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    67958 2023-05-10 08:50:46.369435 pyaedt-0.6.75/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0    25808 2023-03-24 16:10:18.883250 pyaedt-0.6.75/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     6989 2023-03-24 16:10:18.883250 pyaedt-0.6.75/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0     9795 2023-04-28 11:15:40.689926 pyaedt-0.6.75/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    62296 2023-04-07 12:58:03.133395 pyaedt-0.6.75/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    11301 2023-03-24 16:10:18.883250 pyaedt-0.6.75/pyaedt/generic/process.py
+-rw-r--r--   0        0        0    20326 2023-05-12 14:39:14.493618 pyaedt-0.6.75/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3466 2023-03-24 16:10:18.883250 pyaedt-0.6.75/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    60355 2023-03-24 16:10:18.898857 pyaedt-0.6.75/pyaedt/generic/toolkit.py
+-rw-r--r--   0        0        0    17095 2023-04-25 22:05:43.951906 pyaedt-0.6.75/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0      438 2023-03-24 16:10:18.898857 pyaedt-0.6.75/pyaedt/generic/wpf_template.xaml
+-rw-r--r--   0        0        0   252855 2023-04-25 22:05:43.951906 pyaedt-0.6.75/pyaedt/hfss.py
+-rw-r--r--   0        0        0    82916 2023-04-06 11:56:42.332868 pyaedt-0.6.75/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   154940 2023-05-04 12:30:42.836343 pyaedt-0.6.75/pyaedt/icepak.py
+-rw-r--r--   0        0        0   118454 2023-05-10 06:31:48.338096 pyaedt-0.6.75/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7803 2023-04-25 22:05:43.951906 pyaedt-0.6.75/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24259 2023-04-25 22:05:43.951906 pyaedt-0.6.75/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-04-03 09:31:32.851623 pyaedt-0.6.75/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-03-24 16:10:18.907751 pyaedt-0.6.75/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3035 2023-04-03 09:31:32.851623 pyaedt-0.6.75/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     3695 2023-03-30 19:37:04.658681 pyaedt-0.6.75/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     2380 2023-03-30 19:37:04.658681 pyaedt-0.6.75/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0       53 2023-03-24 16:10:18.907751 pyaedt-0.6.75/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10210 2023-04-18 21:46:42.442098 pyaedt-0.6.75/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-03-24 16:10:18.907751 pyaedt-0.6.75/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     3731 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     3829 2023-04-25 22:05:43.951906 pyaedt-0.6.75/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0      678 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-03-24 16:10:18.914516 pyaedt-0.6.75/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      953 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0      868 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14076 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    19994 2023-03-24 16:10:18.930163 pyaedt-0.6.75/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-04-18 21:46:42.442098 pyaedt-0.6.75/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16809 2023-04-07 12:58:03.149048 pyaedt-0.6.75/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   120831 2023-04-05 05:51:09.186354 pyaedt-0.6.75/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0   194513 2023-04-28 15:10:16.972093 pyaedt-0.6.75/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   115362 2023-05-10 15:44:48.349712 pyaedt-0.6.75/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    11332 2023-03-24 16:10:18.945688 pyaedt-0.6.75/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   127894 2023-05-10 08:50:46.369435 pyaedt-0.6.75/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.945688 pyaedt-0.6.75/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    31549 2023-05-05 11:21:23.857681 pyaedt-0.6.75/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49002 2023-04-06 10:00:10.649919 pyaedt-0.6.75/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59516 2023-05-04 12:57:11.212325 pyaedt-0.6.75/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53100 2023-04-28 15:10:16.972093 pyaedt-0.6.75/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12588 2023-04-13 16:03:19.110009 pyaedt-0.6.75/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    42270 2023-04-25 22:05:43.967519 pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    32723 2023-05-08 20:33:32.647460 pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8157 2023-03-24 16:10:18.945688 pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    63043 2023-04-13 10:51:44.555559 pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15094 2023-03-24 16:10:18.945688 pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.945688 pyaedt-0.6.75/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    31983 2023-04-13 10:51:44.555559 pyaedt-0.6.75/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    68020 2023-04-28 15:10:16.972093 pyaedt-0.6.75/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6897 2023-04-25 22:05:43.967519 pyaedt-0.6.75/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    52442 2023-05-12 11:17:44.639145 pyaedt-0.6.75/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    31270 2023-04-13 15:33:56.717485 pyaedt-0.6.75/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    49837 2023-04-25 22:05:43.967519 pyaedt-0.6.75/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.961334 pyaedt-0.6.75/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    65608 2023-04-25 22:05:43.967519 pyaedt-0.6.75/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    21640 2023-04-25 22:05:43.983120 pyaedt-0.6.75/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    30094 2023-04-27 07:01:19.617927 pyaedt-0.6.75/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   114236 2023-05-04 09:41:18.539853 pyaedt-0.6.75/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71549 2023-03-24 16:10:18.961334 pyaedt-0.6.75/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-05-11 09:46:53.726038 pyaedt-0.6.75/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    51910 2023-03-24 16:10:18.961334 pyaedt-0.6.75/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40297 2023-04-25 22:05:43.983120 pyaedt-0.6.75/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0    82846 2023-03-24 16:10:18.961334 pyaedt-0.6.75/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    28306 2023-03-24 16:43:00.406402 pyaedt-0.6.75/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53168 2023-04-07 14:18:16.263614 pyaedt-0.6.75/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11919 2023-03-24 16:10:18.961334 pyaedt-0.6.75/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    26048 2023-03-31 15:10:27.419349 pyaedt-0.6.75/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   172944 2023-05-10 12:27:31.281987 pyaedt-0.6.75/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    64104 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   119693 2023-05-10 15:44:48.349712 pyaedt-0.6.75/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    33226 2023-04-07 14:18:16.263614 pyaedt-0.6.75/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    28652 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   103276 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   125048 2023-05-04 22:05:09.593531 pyaedt-0.6.75/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    95851 2023-05-10 17:22:00.121611 pyaedt-0.6.75/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10556 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    40721 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-03-24 16:10:18.976973 pyaedt-0.6.75/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9425 2023-04-18 21:46:42.457739 pyaedt-0.6.75/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-03-28 22:11:07.622485 pyaedt-0.6.75/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7601 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    10373 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/siwave.py
+-rw-r--r--   0        0        0    10527 2023-03-24 16:10:18.992592 pyaedt-0.6.75/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     4134 2023-05-09 19:48:15.535200 pyaedt-0.6.75/pyproject.toml
+-rw-r--r--   0        0        0    15129 1970-01-01 00:00:00.000000 pyaedt-0.6.75/PKG-INFO
```

### Comparing `pyaedt-0.6.74/LICENSE` & `pyaedt-0.6.75/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/README.md` & `pyaedt-0.6.75/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/__init__.py` & `pyaedt-0.6.75/pyaedt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 os.environ["ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE"] = "1"
 
 pyaedt_path = os.path.dirname(__file__)
 
-__version__ = "0.6.74"
+__version__ = "0.6.75"
 
 version = __version__
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
 import pyaedt.generic.general_methods as general_methods
 from pyaedt.generic.general_methods import _pythonver
```

### Comparing `pyaedt-0.6.74/pyaedt/aedt_logger.py` & `pyaedt-0.6.75/pyaedt/aedt_logger.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.6.75/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/application/Analysis.py` & `pyaedt-0.6.75/pyaedt/application/Analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1505,14 +1505,15 @@
 
         >>> oDesign.Analyze
         """
         warnings.warn("`analyze_nominal` is deprecated. Use `analyze` method instead.", DeprecationWarning)
 
         return self.analyze(self.active_setup, num_cores, num_tasks, num_gpu, acf_file, use_auto_settings)
 
+    @pyaedt_function_handler()
     def analyze(
         self,
         setup_name=None,
         num_cores=1,
         num_tasks=1,
         num_gpu=1,
         acf_file=None,
```

### Comparing `pyaedt-0.6.74/pyaedt/application/Analysis3D.py` & `pyaedt-0.6.75/pyaedt/application/Analysis3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.6.75/pyaedt/application/Analysis3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.6.75/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.6.75/pyaedt/application/AnalysisNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.6.75/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.6.75/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/application/Design.py` & `pyaedt-0.6.75/pyaedt/application/Design.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/application/JobManager.py` & `pyaedt-0.6.75/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/application/Variables.py` & `pyaedt-0.6.75/pyaedt/application/Variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/application/aedt_objects.py` & `pyaedt-0.6.75/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/application/design_solutions.py` & `pyaedt-0.6.75/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/circuit.py` & `pyaedt-0.6.75/pyaedt/circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1264,15 +1264,15 @@
             Circuit Source Object.
 
         References
         ----------
 
         >>> oDesign.UpdateSources
         """
-        source_p = self.create_source(source_type="CurrentSin")
+        source_p = self.create_source(source_type="PowerSin")
         for port in ports:
             self.excitations[port].enabled_sources.append(source_p.name)
             self.excitations[port].update()
         return source_p
 
     @pyaedt_function_handler()
     def assign_voltage_frequency_dependent_excitation_to_ports(self, ports, filepath):
```

### Comparing `pyaedt-0.6.74/pyaedt/common_rpc.py` & `pyaedt-0.6.75/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/desktop.py` & `pyaedt-0.6.75/pyaedt/desktop.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/AnsysReport.deps.json` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/AnsysReport.deps.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/AnsysReport.dll` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/AnsysReport.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/AnsysTemplate.json` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/Images/Ansys.png` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/Images/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/PdfSharpCore.dll` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/PdfSharpCore.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/System.Runtime.dll` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/System.Runtime.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/System.Runtime.xml` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/System.Runtime.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml` & `pyaedt-0.6.75/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/downloads.py` & `pyaedt-0.6.75/pyaedt/downloads.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb.py` & `pyaedt-0.6.75/pyaedt/edb.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 This module is implicitily loaded in HFSS 3D Layout when launched.
 
 """
 import os
 import re
 import shutil
 import sys
+import tempfile
 import time
 import traceback
 import warnings
 
 from pyaedt import __version__
 from pyaedt import pyaedt_logger
 from pyaedt import settings
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.edb_core import Components
 from pyaedt.edb_core import EdbHfss
 from pyaedt.edb_core import EdbLayout
 from pyaedt.edb_core import EdbNets
 from pyaedt.edb_core import EdbSiwave
+from pyaedt.edb_core.edb_data.control_file import ControlFile
+from pyaedt.edb_core.edb_data.control_file import convert_technology_file
 from pyaedt.edb_core.edb_data.design_options import EdbDesignOptions
 from pyaedt.edb_core.edb_data.edb_builder import EdbBuilder
 from pyaedt.edb_core.edb_data.edbvalue import EdbValue
 from pyaedt.edb_core.edb_data.hfss_simulation_setup_data import HfssSimulationSetup
 from pyaedt.edb_core.edb_data.simulation_configuration import SimulationConfiguration
 from pyaedt.edb_core.edb_data.siwave_simulation_setup_data import SiwaveDCSimulationSetup
 from pyaedt.edb_core.edb_data.siwave_simulation_setup_data import SiwaveSYZSimulationSetup
@@ -87,14 +90,16 @@
     isaedtowned : bool, optional
         Whether to launch EDB from HFSS 3D Layout. The
         default is ``False``.
     oproject : optional
         Reference to the AEDT project object.
     student_version : bool, optional
         Whether to open the AEDT student version. The default is ``False.``
+    technology_file : str, optional
+        Full path to technology file to be converted to xml before importing or xml. Supported by GDS format only.
 
     Examples
     --------
     Create an ``Edb`` object and a new EDB cell.
 
     >>> from pyaedt import Edb
     >>> app = Edb()
@@ -133,14 +138,15 @@
         cellname=None,
         isreadonly=False,
         edbversion=None,
         isaedtowned=False,
         oproject=None,
         student_version=False,
         use_ppe=False,
+        technology_file=None,
     ):
         self._clean_variables()
         if inside_desktop:
             self.standalone = False
         else:
             self.standalone = True
         if edb_initialized:
@@ -184,15 +190,21 @@
                 )
 
             if isaedtowned and (inside_desktop or settings.remote_api):
                 self.open_edb_inside_aedt()
             elif edbpath[-3:] in ["brd", "gds", "xml", "dxf", "tgz"]:
                 self.edbpath = edbpath[:-4] + ".aedb"
                 working_dir = os.path.dirname(edbpath)
-                self.import_layout_pcb(edbpath, working_dir, use_ppe=use_ppe)
+                control_file = None
+                if technology_file:
+                    if os.path.splitext(technology_file)[1] == ".xml":
+                        control_file = technology_file
+                    else:
+                        control_file = convert_technology_file(technology_file, edbversion=edbversion)
+                self.import_layout_pcb(edbpath, working_dir, use_ppe=use_ppe, control_file=control_file)
                 if settings.enable_local_log_file and self.log_name:
                     self._logger = self._global_logger.add_file_logger(self.log_name, "Edb")
                 self.logger.info("EDB %s was created correctly from %s file.", self.edbpath, edbpath[-2:])
             elif edbpath.endswith("edb.def"):
                 self.edbpath = os.path.dirname(edbpath)
                 if settings.enable_local_log_file and self.log_name:
                     self._logger = self._global_logger.add_file_logger(self.log_name, "Edb")
@@ -456,35 +468,35 @@
 
         Returns
         -------
 
         """
         if init_dlls:
             self._init_dlls()
-        self.logger.info("EDB Path is %s", self.edbpath)
-        self.logger.info("EDB Version is %s", self.edbversion)
+        # self.logger.info("EDB Path is %s", self.edbpath)
+        # self.logger.info("EDB Version is %s", self.edbversion)
         # if self.edbversion > "2023.1":
         #     self.standalone = False
 
         self.edb.Database.SetRunAsStandAlone(self.standalone)
 
-        self.logger.info("EDB Standalone %s", self.standalone)
+        # self.logger.info("EDB Standalone %s", self.standalone)
         try:
             db = self.edb.Database.Open(self.edbpath, self.isreadonly)
         except Exception as e:
             db = None
             self.logger.error("Builder is not Initialized.")
         if not db:
             self.logger.warning("Error Opening db")
             self._db = None
             self._active_cell = None
             self.builder = None
             return None
         self._db = db
-        self.logger.info("Database Opened")
+        self.logger.info("Database {} Opened in {}".format(os.path.split(self.edbpath)[-1], self.edbversion))
 
         self._active_cell = None
         if self.cellname:
             for cell in list(self._db.TopCircuitCells):
                 if cell.GetName() == self.cellname:
                     self._active_cell = cell
         # if self._active_cell is still None, set it to default cell
@@ -643,21 +655,26 @@
         if not use_ppe:
             cmd_translator.append("-ppe=false")
         if control_file and input_file[-3:] not in ["brd"]:
             if is_linux:
                 cmd_translator.append("-c={}".format(control_file))
             else:
                 cmd_translator.append('-c="{}"'.format(control_file))
-        p = subprocess.Popen(cmd_translator)
+        if is_linux:
+            p = subprocess.Popen(cmd_translator)
+        else:
+            p = subprocess.Popen(" ".join(cmd_translator))
         p.wait()
         if not os.path.exists(os.path.join(working_dir, aedb_name)):
             self.logger.error("Translator failed to translate.")
             return False
+        else:
+            self.logger.info("Translation correctly completed")
         self.edbpath = os.path.join(working_dir, aedb_name)
-        self.open_edb()
+        return self.open_edb()
 
     @pyaedt_function_handler()
     def export_to_ipc2581(self, ipc_path=None, units="MILLIMETER"):
         """Create an XML IPC2581 file from the active EDB.
 
         .. note::
            The method works only in CPython because of some limitations on Ironpython in XML parsing and
@@ -1318,17 +1335,29 @@
             inputBrd, working_dir=WorkDir, anstranslator_full_path=anstranslator_full_path, use_ppe=use_ppe
         ):
             return True
         else:
             return False
 
     @pyaedt_function_handler()
-    def import_gds_file(self, inputGDS, WorkDir=None, anstranslator_full_path="", use_ppe=False, control_file=None):
+    def import_gds_file(
+        self,
+        inputGDS,
+        WorkDir=None,
+        anstranslator_full_path="",
+        use_ppe=False,
+        control_file=None,
+        tech_file=None,
+        map_file=None,
+    ):
         """Import a GDS file and generate an ``edb.def`` file in the working directory.
 
+        ..note::
+            `ANSYSLMD_LICENSE_FILE` is needed to run the translator.
+
         Parameters
         ----------
         inputGDS : str
             Full path to the GDS file.
         WorkDir : str, optional
             Directory in which to create the ``aedb`` folder. The default value is ``None``,
             in which case the AEDB file is given the same name as the GDS file. Only the extension
@@ -1337,21 +1366,33 @@
             Full path to the Ansys translator.
         use_ppe : bool, optional
             Whether to use the PPE License. The default is ``False``.
         control_file : str, optional
             Path to the XML file. The default is ``None``, in which case an attempt is made to find
             the XML file in the same directory as the GDS file. To succeed, the XML file and GDS file must
             have the same name. Only the extension differs.
+        tech_file : str, optional
+            Technology file. It uses Helic to convert tech file to xml and then imports the gds. Works on Linux only.
+        map_file : str, optional
+            Layer map file.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
+        if tech_file or map_file:
+            control_file_temp = os.path.join(tempfile.gettempdir(), os.path.split(inputGDS)[-1][:-3] + "xml")
+            control_file = ControlFile(xml_input=control_file, tecnhology=tech_file, layer_map=map_file).write_xml(
+                control_file_temp
+            )
+        elif tech_file:
+            self.logger.error("Technology files are supported only in Linux. Use control file instead.")
+            return False
         if self.import_layout_pcb(
             inputGDS,
             working_dir=WorkDir,
             anstranslator_full_path=anstranslator_full_path,
             use_ppe=use_ppe,
             control_file=control_file,
         ):
```

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/components.py` & `pyaedt-0.6.75/pyaedt/edb_core/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
         with codecs.open(file_path, "w", encoding="utf-8") as f:
             json.dump(data, f, ensure_ascii=False, indent=4)
         return file_path
 
     @pyaedt_function_handler()
     def refresh_components(self):
         """Refresh the component dictionary."""
-        self._logger.info("Refreshing the Components dictionary.")
+        # self._logger.info("Refreshing the Components dictionary.")
         self._cmp = {
             l.GetName(): EDBComponent(self, l)
             for l in self._active_layout.Groups
             if l.ToString() == "Ansys.Ansoft.Edb.Cell.Hierarchy.Component"
         }
         return True
```

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/edb_data/components_data.py` & `pyaedt-0.6.75/pyaedt/edb_core/edb_data/components_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/edb_data/design_options.py` & `pyaedt-0.6.75/pyaedt/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/edb_data/edbvalue.py` & `pyaedt-0.6.75/pyaedt/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/edb_data/hfss_extent_info.py` & `pyaedt-0.6.75/pyaedt/edb_core/edb_data/hfss_extent_info.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyaedt-0.6.75/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/edb_data/layer_data.py` & `pyaedt-0.6.75/pyaedt/edb_core/edb_data/layer_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/edb_data/nets_data.py` & `pyaedt-0.6.75/pyaedt/edb_core/edb_data/nets_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/edb_data/padstacks_data.py` & `pyaedt-0.6.75/pyaedt/edb_core/edb_data/padstacks_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/edb_data/primitives_data.py` & `pyaedt-0.6.75/pyaedt/edb_core/edb_data/primitives_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/edb_data/simulation_configuration.py` & `pyaedt-0.6.75/pyaedt/edb_core/edb_data/simulation_configuration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyaedt-0.6.75/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/edb_data/sources.py` & `pyaedt-0.6.75/pyaedt/edb_core/edb_data/sources.py`

 * *Files 3% similar despite different names*

```diff
@@ -777,43 +777,105 @@
         CommonExcitation.__init__(self, pedb, edb_terminal)
 
     @property
     def _edb_properties(self):
         p = self._edb_terminal.GetProductSolverOption(self._edb.ProductId.Designer, "HFSS")
         return p
 
+    @_edb_properties.setter
+    def _edb_properties(self, value):
+        self._edb_terminal.SetProductSolverOption(self._edb.ProductId.Designer, "HFSS", value)
+
     @property
     def hfss_type(self):
         """HFSS port type."""
-        txt = re.search(r"'HFSS Type'='.*?'", self._edb_properties).group()
-        return txt.split("=")[1].replace("'", "")
+        temp = re.search(r"'HFSS Type'='.*?'", self._edb_properties)
+        if temp:
+            txt = temp.group()
+            return txt.split("=")[1].replace("'", "")
+        else:  # pragma: no cover
+            return None
 
     @property
     def horizontal_extent_factor(self):
         """Horizontal extent factor."""
-        txt = re.search(r"'Horizontal Extent Factor'='.*?'", self._edb_properties).group()
-        return float(txt.split("=")[1].replace("'", ""))
+        temp = re.search(r"'Horizontal Extent Factor'='.*?'", self._edb_properties)
+        if temp:
+            txt = temp.group()
+            return float(txt.split("=")[1].replace("'", ""))
+        else:  # pragma: no cover
+            return None
+
+    @horizontal_extent_factor.setter
+    def horizontal_extent_factor(self, value):
+        new_arg = r"'Horizontal Extent Factor'='{}'".format(value)
+        if self.horizontal_extent_factor:
+            p = re.sub(r"'Horizontal Extent Factor'='.*?'", new_arg, self._edb_properties)
+        else:
+            match = re.search(r"(.*\))$", self._edb_properties)
+            p = match.group(1)[:-1] + ", " + new_arg + ")"
+        self._edb_properties = p
 
     @property
     def vertical_extent_factor(self):
-        """Vvertical extent factor."""
-        txt = re.search(r"'Vertical Extent Factor'='.*?'", self._edb_properties).group()
-        return float(txt.split("=")[1].replace("'", ""))
+        """Vertical extent factor."""
+        temp = re.search(r"'Vertical Extent Factor'='.*?'", self._edb_properties)
+        if temp:
+            txt = temp.group()
+            return float(txt.split("=")[1].replace("'", ""))
+        return None  # pragma: no cover
+
+    @vertical_extent_factor.setter
+    def vertical_extent_factor(self, value):
+        new_arg = r"'Vertical Extent Factor'='{}'".format(value)
+        if self.vertical_extent_factor:
+            p = re.sub(r"'Vertical Extent Factor'='.*?'", new_arg, self._edb_properties)
+        else:
+            match = re.search(r"(.*\))$", self._edb_properties)
+            p = match.group(1)[:-1] + ", " + new_arg + ")"
+        self._edb_properties = p
 
     @property
     def radial_extent_factor(self):
         """Radial extent factor."""
-        txt = re.search(r"'Radial Extent Factor'='.*?'", self._edb_properties).group()
-        return float(txt.split("=")[1].replace("'", ""))
+        temp = re.search(r"'Radial Extent Factor'='.*?'", self._edb_properties)
+        if temp:
+            txt = temp.group()
+            return float(txt.split("=")[1].replace("'", ""))
+        return None  # pragma: no cover
+
+    @radial_extent_factor.setter
+    def radial_extent_factor(self, value):
+        new_arg = r"'Radial Extent Factor'='{}'".format(value)
+        if self.radial_extent_factor:
+            p = re.sub(r"'Radial Extent Factor'='.*?'", new_arg, self._edb_properties)
+        else:
+            match = re.search(r"(.*\))$", self._edb_properties)
+            p = match.group(1)[:-1] + ", " + new_arg + ")"
+        self._edb_properties = p
 
     @property
     def pec_launch_width(self):
         """Launch width for the printed electronic component (PEC)."""
-        txt = re.search(r"'PEC Launch Width'='.*?'", self._edb_properties).group()
-        return txt.split("=")[1].replace("'", "")
+        temp = re.search(r"'PEC Launch Width'='.*?'", self._edb_properties)
+        if temp:
+            txt = temp.group()
+            return txt.split("=")[1].replace("'", "")
+        else:  # pragma: no cover
+            return None
+
+    @pec_launch_width.setter
+    def pec_launch_width(self, value):
+        new_arg = r"'PEC Launch Width'='{}'".format(value)
+        if self.pec_launch_width:
+            p = re.sub(r"'PEC Launch Width'='.*?'", new_arg, self._edb_properties)
+        else:
+            match = re.search(r"(.*\))$", self._edb_properties)
+            p = match.group(1)[:-1] + ", " + new_arg + ")"
+        self._edb_properties = p
 
     @property
     def impedance(self):
         """Impedance of the port."""
         return self._edb_terminal.GetImpedance().ToDouble()
 
     @property
```

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/edb_data/utilities.py` & `pyaedt-0.6.75/pyaedt/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/edb_data/variables.py` & `pyaedt-0.6.75/pyaedt/edb_core/edb_data/variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/general.py` & `pyaedt-0.6.75/pyaedt/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/hfss.py` & `pyaedt-0.6.75/pyaedt/edb_core/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/bom.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/bom_item.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/characteristics.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/bom/refdes.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/color.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/content.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/dictionary_color.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/dictionary_fill.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/dictionary_line.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/entry_line.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/fill.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/cad_header.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/ecad.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ecad/spec.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/history_record.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/ipc2581.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/ipc2581/logistic_header.py` & `pyaedt-0.6.75/pyaedt/edb_core/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/layout.py` & `pyaedt-0.6.75/pyaedt/edb_core/layout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/materials.py` & `pyaedt-0.6.75/pyaedt/edb_core/materials.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/nets.py` & `pyaedt-0.6.75/pyaedt/edb_core/nets.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/padstack.py` & `pyaedt-0.6.75/pyaedt/edb_core/padstack.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/siwave.py` & `pyaedt-0.6.75/pyaedt/edb_core/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/edb_core/stackup.py` & `pyaedt-0.6.75/pyaedt/edb_core/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/emit.py` & `pyaedt-0.6.75/pyaedt/emit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/emit_core/Couplings.py` & `pyaedt-0.6.75/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/emit_core/EmitConstants.py` & `pyaedt-0.6.75/pyaedt/emit_core/EmitConstants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/emit_core/__init__.py` & `pyaedt-0.6.75/pyaedt/emit_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/emit_core/results/results.py` & `pyaedt-0.6.75/pyaedt/emit_core/results/results.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/emit_core/results/revision.py` & `pyaedt-0.6.75/pyaedt/emit_core/results/revision.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,42 @@
 
         Returns
         -------
         """
         print("This function is inaccessible when the revision is not loaded.")
 
     @pyaedt_function_handler()
+    def get_interaction(self, domain):
+        """
+        Creates a new interaction for a domain.
+
+        Parameters
+        ----------
+        domain : class:`Emit.InteractionDomain`
+            ``InteractionDomain`` object for constraining the analysis parameters.
+
+        Returns
+        -------
+        interaction:class: `Interaction`
+            Interaction object.
+
+        Examples
+        ----------
+        >>> domain = aedtapp.results.interaction_domain()
+        >>> rev.get_interaction(domain)
+
+        """
+        self._load_revision()
+        engine = self.emit_project._emit_api.get_engine()
+        if domain.interferer_names and engine.max_simultaneous_interferers != len(domain.interferer_names):
+            raise ValueError("The max_simultaneous_interferers must equal the number of interferers in the domain.")
+        interaction = engine.get_interaction(domain)
+        return interaction
+
+    @pyaedt_function_handler()
     def run(self, domain):
         """
         Load the revision and then analyze along the given domain.
 
         Parameters
         ----------
         domain :
@@ -268,25 +296,25 @@
             bands = self.emit_project._emit_api.get_band_names(radio_name, tx_rx_mode)
         else:
             bands = None
             self.result_mode_error()
         return bands
 
     @pyaedt_function_handler()
-    def get_active_frequencies(self, radio_name, band_name, tx_rx_mode=None, units=""):
+    def get_active_frequencies(self, radio_name, band_name, tx_rx_mode, units=""):
         """
         Get a list of active frequencies for a ``tx`` or ``rx`` band in a radio/emitter.
 
         Parameters
         ----------
         radio_name : str
             Name of the radio/emitter.
         band_name : str
            Name of the band.
-        tx_rx : :class:`EmitConstants.tx_rx_mode`, optional
+        tx_rx : :class:`EmitConstants.tx_rx_mode`
             Specifies whether to get ``tx`` or ``rx`` radio freqs. The default
             is ``None``, in which case both ``tx`` and ``rx`` freqs are returned.
         units : str, optional
             Units for the frequencies. The default is ``None`` which uses the units
             specified globally for the project.
 
         Returns
@@ -295,16 +323,16 @@
             List of ``tx`` or ``rx`` radio/emitter frequencies.
 
         Examples
         ----------
         >>> freqs = aedtapp.results.current_revision.get_active_frequencies(
                 'Bluetooth', 'Rx - Base Data Rate', Emit.tx_rx_mode.rx)
         """
-        if tx_rx_mode is None:
-            tx_rx_mode = emitConsts.tx_rx_mode().both
+        if tx_rx_mode is None or tx_rx_mode == emitConsts.tx_rx_mode().both:
+            raise ValueError("The mode type must be specified as either Tx or Rx.")
         if self.revision_loaded:
             freqs = self.emit_project._emit_api.get_active_frequencies(radio_name, band_name, tx_rx_mode, units)
         else:
             freqs = None
             self.result_mode_error()
         return freqs
```

### Comparing `pyaedt-0.6.74/pyaedt/generic/DataHandlers.py` & `pyaedt-0.6.75/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.6.75/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/generic/clr_module.py` & `pyaedt-0.6.75/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/generic/configurations.py` & `pyaedt-0.6.75/pyaedt/generic/configurations.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/generic/constants.py` & `pyaedt-0.6.75/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/generic/design_types.py` & `pyaedt-0.6.75/pyaedt/generic/design_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -636,27 +636,95 @@
     cellname=None,
     isreadonly=False,
     edbversion=None,
     isaedtowned=False,
     oproject=None,
     student_version=False,
     use_ppe=False,
+    technology_file=None,
 ):
-    """Edb Class."""
+    """Provides the EDB application interface.
+
+    This module inherits all objects that belong to EDB.
+
+    Parameters
+    ----------
+    edbpath : str, optional
+        Full path to the ``aedb`` folder. The variable can also contain
+        the path to a layout to import. Allowed formats are BRD,
+        XML (IPC2581), GDS, and DXF. The default is ``None``.
+        For GDS import, the Ansys control file (also XML) should have the same
+        name as the GDS file. Only the file extension differs.
+    cellname : str, optional
+        Name of the cell to select. The default is ``None``.
+    isreadonly : bool, optional
+        Whether to open EBD in read-only mode when it is
+        owned by HFSS 3D Layout. The default is ``False``.
+    edbversion : str, optional
+        Version of EDB to use. The default is ``"2021.2"``.
+    isaedtowned : bool, optional
+        Whether to launch EDB from HFSS 3D Layout. The
+        default is ``False``.
+    oproject : optional
+        Reference to the AEDT project object.
+    student_version : bool, optional
+        Whether to open the AEDT student version. The default is ``False.``
+    technology_file : str, optional
+        Full path to technology file to be converted to xml before importing or xml. Supported by GDS format only.
+
+    Returns
+    -------
+    :class:`pyaedt.edb.Edb`
+
+    Examples
+    --------
+    Create an ``Edb`` object and a new EDB cell.
+
+    >>> from pyaedt import Edb
+    >>> app = Edb()
+
+    Add a new variable named "s1" to the ``Edb`` instance.
+
+    >>> app['s1'] = "0.25 mm"
+    >>> app['s1'].tofloat
+    >>> 0.00025
+    >>> app['s1'].tostring
+    >>> "0.25mm"
+
+    or add a new parameter with description:
+
+    >>> app['s2'] = ["20um", "Spacing between traces"]
+    >>> app['s2'].value
+    >>> 1.9999999999999998e-05
+    >>> app['s2'].description
+    >>> 'Spacing between traces'
+
+
+    Create an ``Edb`` object and open the specified project.
+
+    >>> app = Edb("myfile.aedb")
+
+    Create an ``Edb`` object from GDS and control files.
+    The XML control file resides in the same directory as the GDS file: (myfile.xml).
+
+    >>> app = Edb("/path/to/file/myfile.gds")
+
+    """
     from pyaedt.edb import Edb as app
 
     return app(
         edbpath=edbpath,
         cellname=cellname,
         isreadonly=isreadonly,
         edbversion=edbversion,
         isaedtowned=isaedtowned,
         oproject=oproject,
         student_version=student_version,
         use_ppe=use_ppe,
+        technology_file=technology_file,
     )
 
 
 def Siwave(
     specified_version=None,
 ):
     """Siwave Class."""
```

### Comparing `pyaedt-0.6.74/pyaedt/generic/filesystem.py` & `pyaedt-0.6.75/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/generic/general_methods.py` & `pyaedt-0.6.75/pyaedt/generic/general_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,34 @@
     _write_mes(
         "Check Online documentation on: https://aedt.docs.pyansys.com/version/stable/search.html?q={}".format(
             "+".join(args)
         )
     )
 
 
+def normalize_path(path_in, sep=None):
+    """Normalize path separators.
+
+    Parameters
+    ----------
+    path_in : str
+        Path to normalize.
+    sep : str, optional
+        Separator.
+
+    Returns
+    -------
+    str
+        Path normalized to new separator.
+    """
+    if sep is None:
+        sep = os.sep
+    return path_in.replace("\\", sep).replace("/", sep)
+
+
 def _check_types(arg):
     if "netref.builtins.list" in str(type(arg)):
         return "list"
     elif "netref.builtins.dict" in str(type(arg)):
         return "dict"
     elif "netref.__builtin__.list" in str(type(arg)):
         return "list"
```

### Comparing `pyaedt-0.6.74/pyaedt/generic/ibis_reader.py` & `pyaedt-0.6.75/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/generic/near_field_import.py` & `pyaedt-0.6.75/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/generic/pdf.py` & `pyaedt-0.6.75/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/generic/plot.py` & `pyaedt-0.6.75/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/generic/process.py` & `pyaedt-0.6.75/pyaedt/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/generic/python_optimizers.py` & `pyaedt-0.6.75/pyaedt/generic/python_optimizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,39 +264,47 @@
             for i in self.reals[0]:
                 var[i] = self.var_bound[i][0] + np.random.random() * (self.var_bound[i][1] - self.var_bound[i][0])
                 solo[i] = var[i].copy()
 
             obj = self.sim(var)
             solo[self.dim] = obj
             pop[p] = solo.copy()
+            if self.population_file:
+                # Save Population in CSV
+                np.savetxt(self.population_file, pop, delimiter=",")
 
         # Sort
         pop = pop[pop[:, self.dim].argsort()]
         self.best_function = pop[0, self.dim].copy()
         self.best_variable = pop[0, : self.dim].copy()
 
         t = 1
         counter = 0
         while t <= self.iterate:
-            if self.population_file:
-                # Save Population in CSV
-                np.savetxt(self.population_file, pop, delimiter=",")
+            # if self.population_file:
+            #     # Save Population in CSV
+            #     np.savetxt(self.population_file, pop, delimiter=",")
 
             if self.progress_bar:
                 self.progress(t, self.iterate, status="GA is running...")
             # Sort
             pop = pop[pop[:, self.dim].argsort()]
 
             if pop[0, self.dim] < self.best_function:
                 self.best_function = pop[0, self.dim].copy()
                 self.best_variable = pop[0, : self.dim].copy()
                 if pop[0, self.dim] > self.goal:
                     counter = 0
             else:
                 counter += 1
+            if self.best_function < self.goal:
+                break
+            print("\nInfo: Iteration {}".format(t))
+            print("\nInfo: Best Function {}".format(self.best_function))
+            print("\nInfo: Best Variable {}".format(self.best_variable))
 
             # Report
             self.report.append(pop[0, self.dim])
 
             # Normalizing objective function
             # normobj = np.zeros(self.population_size)
             minobj = pop[0, self.dim]
@@ -377,14 +385,17 @@
                 obj = self.sim(ch1)
                 solo[self.dim] = obj
                 pop[k] = solo.copy()
                 solo[: self.dim] = ch2.copy()
                 obj = self.sim(ch2)
                 solo[self.dim] = obj
                 pop[k + 1] = solo.copy()
+                if self.population_file:
+                    # Save Population in CSV
+                    np.savetxt(self.population_file, pop, delimiter=",")
 
             t += 1
             if counter > self.stop_iterations or self.best_function == 0:
                 pop = pop[pop[:, self.dim].argsort()]
                 text = str(t - 1)
                 print("\nInfo: GA is terminated after " + text + " iterations")
                 break
```

### Comparing `pyaedt-0.6.74/pyaedt/generic/report_file_parser.py` & `pyaedt-0.6.75/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/generic/toolkit.py` & `pyaedt-0.6.75/pyaedt/generic/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.6.75/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/hfss.py` & `pyaedt-0.6.75/pyaedt/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/hfss3dlayout.py` & `pyaedt-0.6.75/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/icepak.py` & `pyaedt-0.6.75/pyaedt/icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/maxwell.py` & `pyaedt-0.6.75/pyaedt/maxwell.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             {"ComputeTransientInductance": compute_transient_inductance, "ComputeIncrementalMatrix": incremental_matrix}
         )
 
     @pyaedt_function_handler()
     def set_core_losses(self, objects, value=True):
         """Whether to enable core losses for a set of objects.
 
-        For``EddyCurrent`` and ``Transient`` solver design, core losses calulcations
+        For ``EddyCurrent`` and ``Transient`` solver designs, core losses calulcations
         may be included in the simulation on any object that has a corresponding
         core loss definition (with core loss coefficient settings) in the material library.
 
         Parameters
         ----------
         objects : list, str
             List of object to apply core losses to.
@@ -1516,15 +1516,15 @@
         objects,
         force_type=0,
         window_function="Rectangular",
         use_number_of_last_cycles=True,
         last_cycles_number=1,
         calculate_force="Harmonic",
     ):
-        """Set the Harmonic Force for Transient Analysis.
+        """Enable the harmonic force calculation for the transient analysis.
 
         Parameters
         ----------
         objects : list
             List of object names for force calculations.
         force_type : int, optional
             Force Type. ``0`` for Objects, ``1`` for Surface, ``2`` for volumetric.
```

### Comparing `pyaedt-0.6.74/pyaedt/maxwellcircuit.py` & `pyaedt-0.6.75/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/mechanical.py` & `pyaedt-0.6.75/pyaedt/mechanical.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/Console.py_build` & `pyaedt-0.6.75/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.6.75/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.6.75/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.6.75/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.6.75/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.6.75/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/amat.xml` & `pyaedt-0.6.75/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/console_setup.py` & `pyaedt-0.6.75/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.6.75/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.6.75/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.6.75/pyaedt/misc/install_extra_toolkits.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.6.75/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/misc.py` & `pyaedt-0.6.75/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.6.75/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.6.75/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.6.75/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.6.75/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.6.75/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.6.75/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/misc/template.acf` & `pyaedt-0.6.75/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.6.75/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.6.75/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.6.75/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.6.75/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.6.75/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.6.75/pyaedt/modeler/cad/Modeler.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.6.75/pyaedt/modeler/cad/Primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -1515,15 +1515,19 @@
         References
         ----------
 
         >>> oEditor.GetObjectsByMaterial
 
         """
         if materialname is not None:
-            obj_lst = [x for x in self.object_list if x.material_name == materialname]
+            obj_lst = [
+                x
+                for x in self.object_list
+                if x.material_name == materialname or x.material_name == materialname.lower()
+            ]
         else:
             obj_lst = [
                 self._get_object_dict_by_material(self.materials.conductors),
                 self._get_object_dict_by_material(self.materials.dielectrics),
                 self._get_object_dict_by_material(self.materials.gases),
                 self._get_object_dict_by_material(self.materials.liquids),
             ]
```

### Comparing `pyaedt-0.6.74/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.6.75/pyaedt/modeler/cad/Primitives2D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.6.75/pyaedt/modeler/cad/Primitives3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import os
 
 from pyaedt import Edb
 from pyaedt import Icepak
 from pyaedt.generic import LoadAEDTFile
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import normalize_path
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.advanced_cad.actors import Bird
 from pyaedt.modeler.advanced_cad.actors import Person
 from pyaedt.modeler.advanced_cad.actors import Vehicle
 from pyaedt.modeler.advanced_cad.multiparts import Environment
 from pyaedt.modeler.advanced_cad.multiparts import MultiPartComponent
@@ -1504,15 +1505,15 @@
         # Open Layout component and get information
         aedb_component_path = comp_file
         if os.path.splitext(os.path.basename(comp_file))[1] == ".aedbcomp":
             aedb_project_path = os.path.join(self._app.project_path, self._app.project_name + ".aedb")
             aedb_component_path = os.path.join(
                 aedb_project_path, "LayoutComponents", aedt_component_name, aedt_component_name + ".aedb"
             )
-            aedb_component_path = aedb_component_path.replace("/", "\\")
+            aedb_component_path = normalize_path(aedb_component_path)
 
         component_obj = Edb(
             edbpath=aedb_component_path,
             isreadonly=True,
             edbversion=self._app._aedt_version,
             student_version=self._app.student_version,
         )
```

### Comparing `pyaedt-0.6.74/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.6.75/pyaedt/modeler/cad/components_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.6.75/pyaedt/modeler/cad/elements3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.6.75/pyaedt/modeler/cad/object3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.6.75/pyaedt/modeler/cad/polylines.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/calculators.py` & `pyaedt-0.6.75/pyaedt/modeler/calculators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
         -------
         EmitComponent
             An instance of the new component.
         """
         nodes = components.odesign.GetComponentNodeNames(component_name)
         root_node = nodes[0]
         prop_list = components.odesign.GetComponentNodeProperties(component_name, root_node)
-        props = dict(p.split("=") for p in prop_list)
+        props = dict(p.split("=", 1) for p in prop_list)
         root_node_type = props["Type"]
         if root_node_type.endswith("Node"):
             root_node_type = root_node_type[: -len("Node")]
         if root_node_type not in cls.subclasses:
             return EmitComponent(components, component_name)
         return cls.subclasses[root_node_type](components, component_name)
 
@@ -457,15 +457,15 @@
         """
         nodes = sorted(self.odesign.GetComponentNodeNames(self.name))
         root_node = nodes[0]
         node_name = root_node
         if node is not None:
             node_name = root_node + "-*-" + "-*-".join(node.split("/")[1:])
         props_list = self.odesign.GetComponentNodeProperties(self.name, node_name)
-        props = dict(p.split("=") for p in props_list)
+        props = dict(p.split("=", 1) for p in props_list)
         return props
 
     @pyaedt_function_handler()
     def set_property(self, property_name, property_value):
         """Set part property
 
         Parameters
@@ -708,14 +708,30 @@
         Returns
         -------
         List
             List of the band nodes in the radio."""
         band_nodes = self.get_prop_nodes({"Type": "Band"})
         return band_nodes
 
+    def band_node(self, band_name):
+        """Get the specified band node from this radio.
+
+        Parameters
+        ----------
+        band_name : name of the desired band node.
+
+        Returns
+        -------
+        band_node : Instance of the band node."""
+        band_nodes = self.bands()
+        for node in band_nodes:
+            if band_name == node.props["Name"]:
+                return node
+        return None
+
     def band_start_frequency(self, band_node, units=""):
         """Get the start frequency of the band node.
 
         Parameters
         ----------
         band_node : Instance of the band node.
         units : str, optional
@@ -841,15 +857,15 @@
         None
 
         Returns
         -------
         Dict
             Dictionary of all the properties for this node."""
         prop_list = self.odesign.GetComponentNodeProperties(self.parent_component.name, self.node_name)
-        props = dict(p.split("=") for p in prop_list)
+        props = dict(p.split("=", 1) for p in prop_list)
         return props
 
     @property
     def enabled(self):
         """Returns ''True'' if the node is enabled and
         ''False'' if the node is disabled.
```

### Comparing `pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.6.75/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.6.75/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.6.75/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/modeler2d.py` & `pyaedt-0.6.75/pyaedt/modeler/modeler2d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/modeler3d.py` & `pyaedt-0.6.75/pyaedt/modeler/modeler3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
             try:
                 meshregions.remove("Global")
             except:
                 pass
             if meshregions:
                 arg2.append("MeshRegions:="), arg2.append(meshregions)
         else:
-            if excitation_list:
+            if excitation_list is not None:
                 excitations = excitation_list
             else:
                 excitations = self._app.excitations
                 if self._app.design_type == "HFSS":
                     exc = self._app.get_oo_name(self._app.odesign, "Excitations")
                     if exc and exc[0] not in self._app.excitations:
                         excitations.extend(exc)
```

### Comparing `pyaedt-0.6.74/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.6.75/pyaedt/modeler/modelerpcb.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.6.75/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.6.75/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modeler/schematic.py` & `pyaedt-0.6.75/pyaedt/modeler/schematic.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.6.75/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/Boundary.py` & `pyaedt-0.6.75/pyaedt/modules/Boundary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/CableModeling.py` & `pyaedt-0.6.75/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.6.75/pyaedt/modules/CircuitTemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 VoltageSinusoidal = [
     "NAME:Name",
     "DataId:=",
     "",
     "Type:=",
     1,
     "Output:=",
-    2,
+    0,
     "NumPins:=",
     2,
     "Netlist:=",
     "",
     "CompName:=",
     "Nexxim Circuit Elements\\Independent Sources:V_SIN",
     "FDSFileName:=",
@@ -170,15 +170,15 @@
 CurrentSinusoidal = [
     "NAME:Name",
     "DataId:=",
     "",
     "Type:=",
     1,
     "Output:=",
-    2,
+    1,
     "NumPins:=",
     2,
     "Netlist:=",
     "",
     "CompName:=",
     "Nexxim Circuit Elements\\Independent Sources:I_SIN",
     "FDSFileName:=",
@@ -486,17 +486,17 @@
 
 # Voltage DC
 VoltageDC = [
     "NAME:Name",
     "DataId:=",
     "",
     "Type:=",
-    1,
+    0,
     "Output:=",
-    2,
+    0,
     "NumPins:=",
     2,
     "Netlist:=",
     "",
     "CompName:=",
     "Nexxim Circuit Elements\\Independent Sources:V_DC",
     "FDSFileName:=",
```

### Comparing `pyaedt-0.6.74/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.6.75/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/LayerStackup.py` & `pyaedt-0.6.75/pyaedt/modules/LayerStackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/Material.py` & `pyaedt-0.6.75/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/MaterialLib.py` & `pyaedt-0.6.75/pyaedt/modules/MaterialLib.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/Mesh.py` & `pyaedt-0.6.75/pyaedt/modules/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.6.75/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.6.75/pyaedt/modules/MeshIcepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.6.75/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/PostProcessor.py` & `pyaedt-0.6.75/pyaedt/modules/PostProcessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1745,15 +1745,19 @@
         elif context and isinstance(context, dict):
             for attribute in context:
                 if hasattr(report, attribute):
                     report.__setattr__(attribute, context[attribute])
                 else:
                     self.logger.warning("Parameter " + attribute + " is not available, check syntax.")
         elif context:
-            if hasattr(self.modeler, "line_names") and context in self.modeler.line_names:
+            if (
+                hasattr(self.modeler, "line_names")
+                and hasattr(self.modeler, "point_names")
+                and context in self.modeler.point_names + self.modeler.line_names
+            ):
                 report.polyline = context
             elif context in [
                 "RL",
                 "Sources",
                 "Vias",
                 "Bondwires",
                 "Probes",
```

### Comparing `pyaedt-0.6.74/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.6.75/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/SolveSetup.py` & `pyaedt-0.6.75/pyaedt/modules/SolveSetup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1423,20 +1423,20 @@
                             for pad_obj in pad_objs:
                                 if pad_obj in metal_object:
                                     pad_ind = aedtapp.modeler._object_names_to_ids[pad_obj]
                                     if pad_ind not in obj_dict:
                                         obj_dict[pad_ind] = aedtapp.modeler.objects[pad_ind]
             obj_list = list(obj_dict.values())
             if len(obj_list) == 1:
-                obj_list[0].name = net
+                obj_list[0].name = net.replace(".", "_").replace("/", "_")
                 obj_list[0].color = [randrange(255), randrange(255), randrange(255)]
             elif len(obj_list) > 1:
                 united_object = aedtapp.modeler.unite(obj_list, purge=True)
                 obj_ind = aedtapp.modeler._object_names_to_ids[united_object]
-                aedtapp.modeler.objects[obj_ind].name = net
+                aedtapp.modeler.objects[obj_ind].name = net.replace(".", "_").replace("/", "_")
                 aedtapp.modeler.objects[obj_ind].color = [randrange(255), randrange(255), randrange(255)]
         if aedtapp.design_type == "Q3D Extractor":
             aedtapp.auto_identify_nets()
         aedtapp.close_project(save_project=True)
 
     @pyaedt_function_handler()
     def _get_primitives_points_per_net(self):
```

### Comparing `pyaedt-0.6.74/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.6.75/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.6.75/pyaedt/modules/monitor_icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/report_templates.py` & `pyaedt-0.6.75/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/modules/solutions.py` & `pyaedt-0.6.75/pyaedt/modules/solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/q3d.py` & `pyaedt-0.6.75/pyaedt/q3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1311,23 +1311,33 @@
         net_names = []
         for i in nets_data:
             if isinstance(i, (list, tuple)):
                 net_names.append(i[0].split(":")[1])
         return net_names
 
     @pyaedt_function_handler()
+    def delete_all_nets(self):
+        """Delete all nets in the design."""
+        net_names = self.nets[::]
+        for i in self.boundaries[::]:
+            if i.name in net_names:
+                i.delete()
+        return True
+
+    @pyaedt_function_handler()
     def objects_from_nets(self, nets, materials=None):
-        """Find the objects that belongs to a net. Material can be applied as filter.
+        """Find the objects that belong to one or more nets. You can filter by materials.
 
         Parameters
         ----------
         nets : str, list
-            Nets to search for. Case insensitive.
+            One or more nets to search for. The search is case-insensitive.
         materials : str, list, optional
-            Materials to filter the nets objects. Case insensitive.
+            One or more materials for filtering the net objects. The default
+            is ``None``. The search is case insensitive.
 
         Returns
         -------
         dict
             Dictionary of net name and objects that belongs to it.
         """
         if isinstance(nets, str):
```

### Comparing `pyaedt-0.6.74/pyaedt/rmxprt.py` & `pyaedt-0.6.75/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.6.75/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.6.75/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.6.75/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.6.75/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.6.75/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.6.75/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.6.75/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.6.75/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.6.75/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.6.75/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.6.75/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.6.75/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.6.75/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.6.75/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/sbrplus/plot.py` & `pyaedt-0.6.75/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/siwave.py` & `pyaedt-0.6.75/pyaedt/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyaedt/twinbuilder.py` & `pyaedt-0.6.75/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.74/pyproject.toml` & `pyaedt-0.6.75/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     "scikit-learn==1.2.2",
     "SRTM.py",
     "utm",
     "scikit-rf",
 
 ]
 doc = [
-    "ansys-sphinx-theme==0.9.8",
+    "ansys-sphinx-theme==0.9.9",
     "imageio==2.28.0",
     "imageio-ffmpeg==0.4.8",
     "ipython==8.13.0",
     "ipywidgets==8.0.6",
     "joblib==1.2.0",
     "jupyterlab==3.6.3",
     "matplotlib==3.5.3; python_version <= '3.7'",
```

### Comparing `pyaedt-0.6.74/PKG-INFO` & `pyaedt-0.6.75/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.6.74
+Version: 0.6.75
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -30,15 +30,15 @@
 Requires-Dist: pandas==2.0.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "all"
 Requires-Dist: pyvista==0.38.6 ; extra == "all"
 Requires-Dist: SRTM.py ; extra == "all"
 Requires-Dist: utm ; extra == "all"
 Requires-Dist: scikit-rf ; extra == "all"
 Requires-Dist: openpyxl==3.1.2 ; extra == "all"
-Requires-Dist: ansys-sphinx-theme==0.9.8 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: imageio==2.28.0 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
 Requires-Dist: ipython==8.13.0 ; extra == "doc"
 Requires-Dist: ipywidgets==8.0.6 ; extra == "doc"
 Requires-Dist: joblib==1.2.0 ; extra == "doc"
 Requires-Dist: jupyterlab==3.6.3 ; extra == "doc"
 Requires-Dist: matplotlib==3.5.3 ; extra == "doc" and ( python_version <= '3.7')
```

