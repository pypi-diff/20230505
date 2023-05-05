# Comparing `tmp/RSTAB-1.5.0.tar.gz` & `tmp/RSTAB-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RSTAB-1.5.0.tar", last modified: Mon Dec 12 14:41:25 2022, max compression
+gzip compressed data, was "RSTAB-1.6.0.tar", last modified: Fri May  5 08:23:37 2023, max compression
```

## Comparing `RSTAB-1.5.0.tar` & `RSTAB-1.6.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.089734 RSTAB-1.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.077734 RSTAB-1.5.0/Examples/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/Examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1072 2022-12-12 14:41:16.000000 RSTAB-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      109 2022-12-12 14:41:16.000000 RSTAB-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    10433 2022-12-12 14:41:25.089734 RSTAB-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     9988 2022-12-12 14:41:16.000000 RSTAB-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.077734 RSTAB-1.5.0/RSTAB/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.081734 RSTAB-1.5.0/RSTAB/BasicObjects/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/BasicObjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1911 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/BasicObjects/material.py
--rw-r--r--   0 runner    (1001) docker     (116)    89006 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/BasicObjects/member.py
--rw-r--r--   0 runner    (1001) docker     (116)     4804 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/BasicObjects/memberSet.py
--rw-r--r--   0 runner    (1001) docker     (116)    14609 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/BasicObjects/node.py
--rw-r--r--   0 runner    (1001) docker     (116)     2069 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/BasicObjects/section.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.081734 RSTAB-1.5.0/RSTAB/Calculate/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Calculate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1811 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Calculate/optimizationSettings.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.081734 RSTAB-1.5.0/RSTAB/ConcreteDesign/
--rw-r--r--   0 runner    (1001) docker     (116)     3190 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/ConcreteDesign/ConcreteServiceabilityConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (116)     3184 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/ConcreteDesign/ConcreteUltimateConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/ConcreteDesign/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.081734 RSTAB-1.5.0/RSTAB/DynamicLoads/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/DynamicLoads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6045 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/DynamicLoads/responseSpectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.081734 RSTAB-1.5.0/RSTAB/Imperfections/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Imperfections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    20527 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Imperfections/imperfectionCase.py
--rw-r--r--   0 runner    (1001) docker     (116)     9351 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Imperfections/memberImperfection.py
--rw-r--r--   0 runner    (1001) docker     (116)     9275 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Imperfections/membersetImperfection.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.081734 RSTAB-1.5.0/RSTAB/ImportExport/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/ImportExport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5650 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/ImportExport/exports.py
--rw-r--r--   0 runner    (1001) docker     (116)      983 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/ImportExport/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.081734 RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2025 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/designSituation.py
--rw-r--r--   0 runner    (1001) docker     (116)     6809 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/loadCase.py
--rw-r--r--   0 runner    (1001) docker     (116)   136427 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/loadCasesAndCombinations.py
--rw-r--r--   0 runner    (1001) docker     (116)     4494 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/loadCombination.py
--rw-r--r--   0 runner    (1001) docker     (116)    16758 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/modalAnalysisSettings.py
--rw-r--r--   0 runner    (1001) docker     (116)     1295 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/resultCombination.py
--rw-r--r--   0 runner    (1001) docker     (116)     4535 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/spectralAnalysisSettings.py
--rw-r--r--   0 runner    (1001) docker     (116)    23114 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/stabilityAnalysisSettings.py
--rw-r--r--   0 runner    (1001) docker     (116)    14594 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/staticAnalysisSettings.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.081734 RSTAB-1.5.0/RSTAB/Loads/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Loads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2351 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Loads/imposedNodalDeformation.py
--rw-r--r--   0 runner    (1001) docker     (116)   100867 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Loads/memberLoad.py
--rw-r--r--   0 runner    (1001) docker     (116)   115392 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Loads/membersetload.py
--rw-r--r--   0 runner    (1001) docker     (116)    23165 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Loads/nodalLoad.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.085734 RSTAB-1.5.0/RSTAB/Reports/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    32882 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Reports/favicon32.png
--rw-r--r--   0 runner    (1001) docker     (116)    10298 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Reports/html.py
--rw-r--r--   0 runner    (1001) docker     (116)     1579 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Reports/htmlScript.js
--rw-r--r--   0 runner    (1001) docker     (116)     1165 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Reports/htmlStyles.css
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Reports/partsList.py
--rw-r--r--   0 runner    (1001) docker     (116)     1289 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Reports/printoutReport.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.085734 RSTAB-1.5.0/RSTAB/Results/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      888 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Results/designOverview.py
--rw-r--r--   0 runner    (1001) docker     (116)   174365 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Results/resultTables.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.085734 RSTAB-1.5.0/RSTAB/SpecialObjects/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/SpecialObjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      248 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/SpecialObjects/nodalRelease.py
--rw-r--r--   0 runner    (1001) docker     (116)    16668 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/SpecialObjects/structureModification.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.085734 RSTAB-1.5.0/RSTAB/SteelDesign/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/SteelDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2430 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/SteelDesign/steelUltimateConfigurations.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.085734 RSTAB-1.5.0/RSTAB/TimberDesign/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TimberDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2466 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TimberDesign/timberServiceLimitStateConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (116)     2435 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TimberDesign/timberUltimateConfigurations.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.085734 RSTAB-1.5.0/RSTAB/Tools/
--rw-r--r--   0 runner    (1001) docker     (116)     1219 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Tools/GetObjectNumbersByType.py
--rw-r--r--   0 runner    (1001) docker     (116)     3767 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Tools/ModelCheck.py
--rw-r--r--   0 runner    (1001) docker     (116)      827 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Tools/PlausibilityCheck.py
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4720 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Tools/centreOfGravityAndObjectInfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     2206 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/Tools/sectionDialogue.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.085734 RSTAB-1.5.0/RSTAB/TypesForAluminumDesign/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForAluminumDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5052 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForAluminumDesign/aluminumEffectiveLengths.py
--rw-r--r--   0 runner    (1001) docker     (116)     5195 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForAluminumDesign/aluminumMemberLocalSectionReduction.py
--rw-r--r--   0 runner    (1001) docker     (116)     6912 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForAluminumDesign/aluminumMemberRotationalRestraints.py
--rw-r--r--   0 runner    (1001) docker     (116)     8967 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForAluminumDesign/aluminumMemberShearPanel.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.085734 RSTAB-1.5.0/RSTAB/TypesForMembers/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForMembers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4114 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForMembers/memberDefinableStiffness.py
--rw-r--r--   0 runner    (1001) docker     (116)     6505 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForMembers/memberEccentricity.py
--rw-r--r--   0 runner    (1001) docker     (116)    32540 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForMembers/memberHinge.py
--rw-r--r--   0 runner    (1001) docker     (116)     2716 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForMembers/memberNonlinearity.py
--rw-r--r--   0 runner    (1001) docker     (116)     2556 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForMembers/memberResultIntermediatePoints.py
--rw-r--r--   0 runner    (1001) docker     (116)     6297 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForMembers/memberStiffnessModification.py
--rw-r--r--   0 runner    (1001) docker     (116)     2935 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForMembers/memberSupport.py
--rw-r--r--   0 runner    (1001) docker     (116)     5582 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForMembers/memberTransverseStiffeners.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.085734 RSTAB-1.5.0/RSTAB/TypesForNodes/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForNodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4332 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForNodes/nodalSupport.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.085734 RSTAB-1.5.0/RSTAB/TypesForSpecialObjects/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForSpecialObjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      258 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForSpecialObjects/nodalReleaseType.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.089734 RSTAB-1.5.0/RSTAB/TypesForSteelDesign/
--rw-r--r--   0 runner    (1001) docker     (116)     5277 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForSteelDesign/SteelMemberLocalSectionReduction.py
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForSteelDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10286 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForSteelDesign/steelBoundaryConditions.py
--rw-r--r--   0 runner    (1001) docker     (116)    10541 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForSteelDesign/steelEffectiveLengths.py
--rw-r--r--   0 runner    (1001) docker     (116)     6974 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForSteelDesign/steelMemberRotationalRestraints.py
--rw-r--r--   0 runner    (1001) docker     (116)     8903 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForSteelDesign/steelMemberShearPanel.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.089734 RSTAB-1.5.0/RSTAB/TypesForTimberDesign/
--rw-r--r--   0 runner    (1001) docker     (116)        2 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForTimberDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7738 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForTimberDesign/timberEffectiveLengths.py
--rw-r--r--   0 runner    (1001) docker     (116)    11469 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForTimberDesign/timberMemberLocalSectionReduction.py
--rw-r--r--   0 runner    (1001) docker     (116)     3120 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForTimberDesign/timberMemberRotationalRestraint.py
--rw-r--r--   0 runner    (1001) docker     (116)     2925 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForTimberDesign/timberMemberShearPanel.py
--rw-r--r--   0 runner    (1001) docker     (116)     2213 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesForTimberDesign/timberServiceClass.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.089734 RSTAB-1.5.0/RSTAB/TypesforConcreteDesign/
--rw-r--r--   0 runner    (1001) docker     (116)     8964 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesforConcreteDesign/ConcreteDurability.py
--rw-r--r--   0 runner    (1001) docker     (116)     5170 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesforConcreteDesign/ConcreteEffectiveLength.py
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/TypesforConcreteDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2508 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/baseSettings.py
--rw-r--r--   0 runner    (1001) docker     (116)       42 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/dataTypes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1331 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (116)   117536 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/enums.py
--rw-r--r--   0 runner    (1001) docker     (116)     5007 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/formula.py
--rw-r--r--   0 runner    (1001) docker     (116)     4453 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/globalParameter.py
--rw-r--r--   0 runner    (1001) docker     (116)    19249 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/initModel.py
--rw-r--r--   0 runner    (1001) docker     (116)     2633 2022-12-12 14:41:16.000000 RSTAB-1.5.0/RSTAB/suds_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-12 14:41:25.081734 RSTAB-1.5.0/RSTAB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    10433 2022-12-12 14:41:24.000000 RSTAB-1.5.0/RSTAB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4254 2022-12-12 14:41:25.000000 RSTAB-1.5.0/RSTAB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:24.000000 RSTAB-1.5.0/RSTAB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-12 14:41:24.000000 RSTAB-1.5.0/RSTAB.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       55 2022-12-12 14:41:24.000000 RSTAB-1.5.0/RSTAB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2022-12-12 14:41:24.000000 RSTAB-1.5.0/RSTAB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-12-12 14:41:25.089734 RSTAB-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      905 2022-12-12 14:41:16.000000 RSTAB-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.913231 RSTAB-1.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.901231 RSTAB-1.6.0/Examples/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/Examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-05-05 08:23:29.000000 RSTAB-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-05 08:23:29.000000 RSTAB-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-05-05 08:23:37.913231 RSTAB-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9988 2023-05-05 08:23:29.000000 RSTAB-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB/BasicObjects/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/BasicObjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2247 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/BasicObjects/material.py
+-rw-r--r--   0 runner    (1001) docker     (122)    89338 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/BasicObjects/member.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5147 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/BasicObjects/memberSet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14897 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/BasicObjects/node.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/BasicObjects/section.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB/Calculate/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Calculate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1811 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Calculate/optimizationSettings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB/ConcreteDesign/
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/ConcreteDesign/ConcreteServiceabilityConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/ConcreteDesign/ConcreteUltimateConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/ConcreteDesign/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB/DynamicLoads/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/DynamicLoads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6336 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/DynamicLoads/responseSpectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB/Imperfections/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Imperfections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20742 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Imperfections/imperfectionCase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9351 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Imperfections/memberImperfection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9275 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Imperfections/membersetImperfection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB/ImportExport/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/ImportExport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5650 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/ImportExport/exports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1128 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/ImportExport/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8304 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/combinationWizard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/designSituation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9427 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/loadCase.py
+-rw-r--r--   0 runner    (1001) docker     (122)   136467 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/loadCasesAndCombinations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3957 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/loadCombination.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16722 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/modalAnalysisSettings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/resultCombination.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4535 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/spectralAnalysisSettings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23114 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/stabilityAnalysisSettings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14699 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/staticAnalysisSettings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/Loads/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Loads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Loads/imposedNodalDeformation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    99681 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Loads/memberLoad.py
+-rw-r--r--   0 runner    (1001) docker     (122)   113024 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Loads/membersetload.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22037 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Loads/nodalLoad.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/Reports/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32882 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Reports/favicon32.png
+-rw-r--r--   0 runner    (1001) docker     (122)    10352 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Reports/html.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Reports/htmlScript.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Reports/htmlStyles.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2158 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Reports/partsList.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Reports/printoutReport.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/Results/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Results/designOverview.py
+-rw-r--r--   0 runner    (1001) docker     (122)   174365 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Results/resultTables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/SpecialObjects/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/SpecialObjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/SpecialObjects/nodalRelease.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10945 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/SpecialObjects/structureModification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/SteelDesign/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/SteelDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/SteelDesign/steelServiceabilityConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/SteelDesign/steelUltimateConfigurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/TimberDesign/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TimberDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2448 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TimberDesign/timberServiceLimitStateConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TimberDesign/timberUltimateConfigurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/Tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Tools/GetObjectNumbersByType.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Tools/ModelCheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Tools/PlausibilityCheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Tools/centreOfGravityAndObjectInfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/Tools/sectionDialogue.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.909231 RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5052 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/aluminumEffectiveLengths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5314 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/aluminumMemberLocalSectionReduction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3837 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/aluminumMemberTransverseWelds.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.913231 RSTAB-1.6.0/RSTAB/TypesForMembers/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4114 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberDefinableStiffness.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6504 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberEccentricity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33161 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberHinge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2716 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberNonlinearity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2629 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberResultIntermediatePoints.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11825 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberRotationalRestraint.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18158 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberShearPanel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6297 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberStiffnessModification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4100 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberSupport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5685 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForMembers/memberTransverseStiffeners.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.913231 RSTAB-1.6.0/RSTAB/TypesForNodes/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForNodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4332 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForNodes/nodalSupport.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.913231 RSTAB-1.6.0/RSTAB/TypesForSpecialObjects/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForSpecialObjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44487 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForSpecialObjects/nodalReleaseType.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.913231 RSTAB-1.6.0/RSTAB/TypesForSteelDesign/
+-rw-r--r--   0 runner    (1001) docker     (122)     5381 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForSteelDesign/SteelMemberLocalSectionReduction.py
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForSteelDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10495 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForSteelDesign/steelBoundaryConditions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10742 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForSteelDesign/steelEffectiveLengths.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.913231 RSTAB-1.6.0/RSTAB/TypesForTimberDesign/
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForTimberDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7941 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForTimberDesign/timberEffectiveLengths.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11534 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForTimberDesign/timberMemberLocalSectionReduction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesForTimberDesign/timberServiceClass.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.913231 RSTAB-1.6.0/RSTAB/TypesforConcreteDesign/
+-rw-r--r--   0 runner    (1001) docker     (122)     8964 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesforConcreteDesign/ConcreteDurability.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5375 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesforConcreteDesign/ConcreteEffectiveLength.py
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/TypesforConcreteDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2943 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/baseData.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/baseSettings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/dataTypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)   124006 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5007 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4453 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/globalParameter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23148 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/initModel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-05-05 08:23:29.000000 RSTAB-1.6.0/RSTAB/suds_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 08:23:37.905231 RSTAB-1.6.0/RSTAB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-05-05 08:23:37.000000 RSTAB-1.6.0/RSTAB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4182 2023-05-05 08:23:37.000000 RSTAB-1.6.0/RSTAB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:37.000000 RSTAB-1.6.0/RSTAB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 08:23:37.000000 RSTAB-1.6.0/RSTAB.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-05 08:23:37.000000 RSTAB-1.6.0/RSTAB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-05 08:23:37.000000 RSTAB-1.6.0/RSTAB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-05 08:23:37.913231 RSTAB-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      905 2023-05-05 08:23:29.000000 RSTAB-1.6.0/setup.py
```

### Comparing `RSTAB-1.5.0/LICENSE` & `RSTAB-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/PKG-INFO` & `RSTAB-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RSTAB
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python Framework for RSTAB9 Web Services
 Home-page: https://github.com/Dlubal-Software/RSTAB_Python_Client
 Author: Dlubal Software
 Author-email: info@dlubal.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: RSTAB Version: 1.5.0 Summary: Python Framework for
+Metadata-Version: 2.1 Name: RSTAB Version: 1.6.0 Summary: Python Framework for
 RSTAB9 Web Services Home-page: https://github.com/Dlubal-Software/
 RSTAB_Python_Client Author: Dlubal Software Author-email: info@dlubal.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Description-Content-Type: text/markdown License-File: LICENSE
 ****** [Dlubal_Software] Dlubal Software GmbH [![image](https://img.shields.io/
 twitter/follow/dlubal_en?style=social)](https://twitter.com/dlubal_en "Twitter
```

### Comparing `RSTAB-1.5.0/README.md` & `RSTAB-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/BasicObjects/material.py` & `RSTAB-1.6.0/RSTAB/BasicObjects/material.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,7 +53,19 @@
             materials_no (str): Numbers of Materials to be deleted
             model (RSTAB Class, optional): Model to be edited
         '''
 
         # Delete from client model
         for material in ConvertStrToListOfInt(materials_no):
             model.clientModel.service.delete_object(ObjectTypes.E_OBJECT_TYPE_MATERIAL.name, material)
+
+    @staticmethod
+    def GetMaterial(object_index: int = 1, model = Model):
+
+        '''
+        Args:
+            obejct_index (int): Material Index
+            model (RSTAB Class, optional): Model to be edited
+        '''
+
+        # Get Material from client model
+        return model.clientModel.service.get_material(object_index)
```

### Comparing `RSTAB-1.5.0/RSTAB/BasicObjects/member.py` & `RSTAB-1.6.0/RSTAB/BasicObjects/member.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
                     rotation_parameters = [rotation_surface, rotation_surface_plane_type]
             start_section_no (int): Tag of Start Section
             end_section_no (int): End of End Section
             distribution_parameters (list): Distribution Parameters
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
                 params = {'member_hinge_start':, 'member_hinge_end': , 'member_eccentricity_start': ,
-                          'member_eccentricity_end': , 'support':, 'member_nonlinearity': ,
+                          'member_eccentricity_end': 0, 'support':0, 'member_nonlinearity': 0,
                           'end_modifications_member_start_extension': , 'end_modifications_member_start_slope_y': ,
                           'end_modifications_member_start_slope_z': , 'end_modifications_member_end_extension': ,
                           'end_modifications_member_end_slope_y': , 'end_modifications_member_end_slope_z': ,
                           'member_result_intermediate_point' : , 'is_deactivated_for_calculation' : }
             model (RSTAB Class, optional): Model to be edited
         """
 
@@ -1672,8 +1672,20 @@
         Args:
             members_no (str): Numbers of Members to be deleted
             model (RSTAB Class, optional): Model to be edited
         '''
 
         # Delete from client model
         for member in ConvertStrToListOfInt(members_no):
-            model.clientModel.service.delete_object(ObjectTypes.E_OBJECT_TYPE_MEMBER.name, member)
+            model.clientModel.service.delete_object(ObjectTypes.E_OBJECT_TYPE_MEMBER.name, member)
+
+    @staticmethod
+    def GetMember(object_index: int = 1, model = Model):
+
+        '''
+        Args:
+            obejct_index (int): Member Index
+            model (RSTAB Class, optional): Model to be edited
+        '''
+
+        # Get Member from client model
+        return model.clientModel.service.get_member(object_index)
```

### Comparing `RSTAB-1.5.0/RSTAB/BasicObjects/memberSet.py` & `RSTAB-1.6.0/RSTAB/BasicObjects/memberSet.py`

 * *Files 9% similar despite different names*

```diff
@@ -136,7 +136,19 @@
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
         # Add Member Set to client model
         model.clientModel.service.set_member_set(clientObject)
+
+    @staticmethod
+    def GetMemberSet(object_index: int = 1, model = Model):
+
+        '''
+        Args:
+            obejct_index (int): Member Set Index
+            model (RSTAB Class, optional): Model to be edited
+        '''
+
+        # Get Member Set from client model
+        return model.clientModel.service.get_member_set(object_index)
```

### Comparing `RSTAB-1.5.0/RSTAB/BasicObjects/node.py` & `RSTAB-1.6.0/RSTAB/BasicObjects/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         clientObject.type = NodeType.TYPE_STANDARD.name
 
         # Coordinates
 
         clientObject.coordinate_system_type = coordinate_system_type.name
 
         if len(coordinate_system) != 3:
-            raise Exception('WARNING: The coordinate system needs to be of length 3.')
+            raise ValueError('WARNING: The coordinate system needs to be of length 3.')
 
         if not all(isinstance(x, (int, float)) for x in coordinate_system):
             raise Exception ('WARNING: Coordinate system should be type "int" or "float".')
 
 
         if clientObject.coordinate_system_type == "COORDINATE_SYSTEM_CARTESIAN":
             clientObject.coordinate_1 = coordinate_system[0]
@@ -191,22 +191,20 @@
         # Start Node No.
         clientObject.between_two_nodes_start_node = start_node_no
 
         # End Node No.
         clientObject.between_two_nodes_end_node = end_node_no
 
          # Length between i and j
-
         clientObject.reference_type = node_reference.name
 
         clientObject.reference_object_projected_length = length_between_i_and_j
 
         # Distance between node k and start point
-
-        if parameters[0]: #if parameters[0]==True
+        if parameters[0]:
             clientObject.distance_from_start_relative = parameters[1]
         else:
             clientObject.distance_from_start_absolute = parameters[1]
 
         # Offset_local_y
         clientObject.offset_in_local_direction_y = offset_y
 
@@ -308,15 +306,15 @@
 
         if params:
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
-        
+
         # Add Node to client model
         model.clientModel.service.set_node(clientObject)
 
     @staticmethod
     def OnMember(
                  no: int = 1,
                  member_number: int = 1,
@@ -391,8 +389,20 @@
         Args:
             nodes_no (str): Numbers of Nodes to be deleted
             model (RSTAB Class, optional): Model to be edited
         '''
 
         # Delete from client model
         for node in ConvertStrToListOfInt(nodes_no):
-            model.clientModel.service.delete_object(ObjectTypes.E_OBJECT_TYPE_NODE.name, node)
+            model.clientModel.service.delete_object(ObjectTypes.E_OBJECT_TYPE_NODE.name, node)
+
+    @staticmethod
+    def GetNode(object_index: int = 1, model = Model):
+
+        '''
+        Args:
+            obejct_index (int): Node Index
+            model (RSTAB Class, optional): Model to be edited
+        '''
+
+        # Get Node from client model
+        return model.clientModel.service.get_node(object_index)
```

### Comparing `RSTAB-1.5.0/RSTAB/BasicObjects/section.py` & `RSTAB-1.6.0/RSTAB/BasicObjects/section.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,8 +56,20 @@
         Args:
             sections_no (str): Numbers of Sections to be deleted
             model (RSTAB Class, optional): Model to be edited
         '''
 
         # Delete from client model
         for section in ConvertStrToListOfInt(sections_no):
-            model.clientModel.service.delete_object(ObjectTypes.E_OBJECT_TYPE_SECTION.name, section)
+            model.clientModel.service.delete_object(ObjectTypes.E_OBJECT_TYPE_SECTION.name, section)
+
+    @staticmethod
+    def GetSection(object_index: int = 1, model = Model):
+
+        '''
+        Args:
+            obejct_index (int): Section Index
+            model (RSTAB Class, optional): Model to be edited
+        '''
+
+        # Get Section from client model
+        return model.clientModel.service.get_section(object_index)
```

### Comparing `RSTAB-1.5.0/RSTAB/Calculate/optimizationSettings.py` & `RSTAB-1.6.0/RSTAB/Calculate/optimizationSettings.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/ConcreteDesign/ConcreteServiceabilityConfigurations.py` & `RSTAB-1.6.0/RSTAB/SteelDesign/steelServiceabilityConfiguration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,67 @@
 from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
 
-
-class ConcreteServiceabilityConfiguration():
+class SteelDesignServiceabilityConfigurations():
 
     def __init__(self,
-                no: int = 1,
-                name: str = 'SLS',
-                members: str = 'All',
-                member_sets: str = 'All',
-                surfaces: str = 'All',
-                surface_sets: str = 'All',
-                nodes: str = '',
-                comment: str = '',
-                params: dict = None,
-                model = Model):
+                 no: int = 1,
+                 name: str = 'SLS1',
+                 members_no: str = 'All',
+                 member_sets_no: str = 'All',
+                 comment: str = '',
+                 params: dict = None,
+                 model = Model):
+
         """
         Args:
-            no (int): Configuration Tag
-            name (str): User Defined Name
-            members (str): Assigned Members
-            member_sets (str): Assigned Member Sets
-            surfaces (str): Assigned Surfaces
-            surface_sets (str): Assigned Surface Sets
-            nodes (str): Assigned Nodes
+            no (int): Steel Design Serviceability Configuration Tag
+            name (str): User Defined Configuration Name
+            members_no (str): Assign Configuration to Selected Members
+            member_sets_no (str): Assign Configuration to Selected Member Sets
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
-        # Client model | Concrete Durabilities
-        clientObject = model.clientModel.factory.create('ns0:concrete_design_sls_configuration')
+        # Client Model | Steel Design Serviceability Configurations
+        clientObject = model.clientModel.factory.create('ns0:steel_design_sls_configuration')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
-        # Concrete Durability No.
+        # ULS Configuration No.
         clientObject.no = no
 
         # User Defined Name
         if name:
             clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
         # Assigned Members
-        if members == 'All':
+        if members_no == 'All':
             clientObject.assigned_to_all_members = True
 
         else:
             clientObject.assigned_to_all_members = False
-            clientObject.assigned_to_members = ConvertToDlString(members)
+            clientObject.assigned_to_members = ConvertToDlString(members_no)
 
         # Assigned Member Sets
-        if member_sets == 'All':
+        if member_sets_no == 'All':
             clientObject.assigned_to_all_member_sets = True
 
         else:
             clientObject.assigned_to_all_member_sets = False
-            clientObject.assigned_to_member_sets = ConvertToDlString(member_sets)
-
-        # Assigned Surfaces
-        if surfaces == 'All':
-            clientObject.assigned_to_all_surfaces = True
-
-        else:
-            clientObject.assigned_to_all_surfaces = False
-            clientObject.assigned_to_surfaces = ConvertToDlString(surfaces)
-
-        # Assigned Surface Sets
-        if surface_sets == 'All':
-            clientObject.assigned_to_all_surface_sets = True
-
-        else:
-            clientObject.assigned_to_all_surface_sets = False
-            clientObject.assigned_to_surface_sets = ConvertToDlString(surface_sets)
-
-        #Assinged Nodes
-        clientObject.assigned_to_nodes = ConvertToDlString(nodes)
+            clientObject.assigned_to_member_sets = ConvertToDlString(member_sets_no)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
-        # Add Global Parameter to client model
-        model.clientModel.service.set_concrete_design_sls_configuration(clientObject)
+        # Add Global Parameters to Client Model
+        model.clientModel.service.set_steel_design_sls_configuration(clientObject)
```

### Comparing `RSTAB-1.5.0/RSTAB/ConcreteDesign/ConcreteUltimateConfigurations.py` & `RSTAB-1.6.0/RSTAB/TypesForMembers/memberResultIntermediatePoints.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,65 @@
-from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
-
-
-class ConcreteUltimateConfiguration():
+from RSTAB.initModel import Model, clearAttributes, ConvertToDlString, deleteEmptyAttributes
 
+class MemberResultIntermediatePoint():
     def __init__(self,
-                no: int = 1,
-                name: str = 'ULS',
-                members: str = 'All',
-                member_sets: str = 'All',
-                surfaces: str = 'All',
-                surface_sets: str = 'All',
-                nodes: str = '',
-                comment: str = '',
-                params: dict = None,
-                model = Model):
+                 no: int = 1,
+                 members: str = "",
+                 point_count: int = 2,
+                 uniform_distribution: bool = True,
+                 distances = None,
+                 comment: str = '',
+                 params: dict = None,
+                 model = Model):
         """
         Args:
-            no (int): Configuration Tag
-            name (str): User Defined Name
+            no (int): Member Result Intermediate Point Tag
             members (str): Assigned Members
-            member_sets (str): Assigned Member Sets
-            surfaces (str): Assigned Surfaces
-            surface_sets (str): Assigned Surface Sets
-            nodes (str): Assigned Nodes
+            point_count (int): Assigned Point Number
+            uniform_distribution (bool): Uniform Distrubition Option
+            distances (list of lists): Distances Table
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
-        # Client model | Concrete Durabilities
-        clientObject = model.clientModel.factory.create('ns0:concrete_design_uls_configuration')
+        # Client model | Member Result Intermediate Point
+        clientObject = model.clientModel.factory.create('ns0:member_result_intermediate_point')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
-        # Concrete Durability No.
+        # Member Result Intermediate Point No.
         clientObject.no = no
 
-        # User Defined Name
-        if name:
-            clientObject.user_defined_name_enabled = True
-            clientObject.name = name
-
         # Assigned Members
-        if members == 'All':
-            clientObject.assigned_to_all_members = True
-
-        else:
-            clientObject.assigned_to_all_members = False
-            clientObject.assigned_to_members = ConvertToDlString(members)
+        clientObject.members = ConvertToDlString(members)
 
-        # Assigned Member Sets
-        if member_sets == 'All':
-            clientObject.assigned_to_all_member_sets = True
+        # Point Count
+        clientObject.uniform_distribution = uniform_distribution
+        if uniform_distribution:
+            clientObject.point_count = point_count
 
         else:
-            clientObject.assigned_to_all_member_sets = False
-            clientObject.assigned_to_member_sets = ConvertToDlString(member_sets)
+            clientObject.distances = Model.clientModel.factory.create('ns0:member_result_intermediate_point.distances')
 
-        # Assigned Surfaces
-        if surfaces == 'All':
-            clientObject.assigned_to_all_surfaces = True
-
-        else:
-            clientObject.assigned_to_all_surfaces = False
-            clientObject.assigned_to_surfaces = ConvertToDlString(surfaces)
-
-        # Assigned Surface Sets
-        if surface_sets == 'All':
-            clientObject.assigned_to_all_surface_sets = True
-
-        else:
-            clientObject.assigned_to_all_surface_sets = False
-            clientObject.assigned_to_surface_sets = ConvertToDlString(surface_sets)
+            for i,j in enumerate(distances):
+                mlvlp = Model.clientModel.factory.create('ns0:member_result_intermediate_point_distances_row')
+                mlvlp.no = i+1
+                mlvlp.row = Model.clientModel.factory.create('ns0:member_result_intermediate_point_distances')
+                mlvlp.row.value = distances[i][0]
 
-        #Assinged Nodes
-        clientObject.assigned_to_nodes = ConvertToDlString(nodes)
+                clientObject.distances.member_result_intermediate_point_distances.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
-        # Add Global Parameter to client model
-        model.clientModel.service.set_concrete_design_uls_configuration(clientObject)
+        # Add Member Result Intermediate Point to client model
+        model.clientModel.service.set_member_result_intermediate_point(clientObject)
```

### Comparing `RSTAB-1.5.0/RSTAB/DynamicLoads/responseSpectrum.py` & `RSTAB-1.6.0/RSTAB/DynamicLoads/responseSpectrum.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,16 @@
                  model = Model):
         """
         Args:
             no (int): Response Spectrum Tag
             name (str): User Defined Name
             constant_period_step (float): Enables Constant Period Step
             sort_table (bool): Sort Table Option
-            user_defined_spectrum (list): User Defined Spectrum
-
+            user_defined_spectrum (list of lists): User Defined Spectrum
                 user_defined_spectrum = [[period, acceleration], [period, acceleration], ...]
-
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
         # client model | response spectrum
         clientObject = model.clientModel.factory.create('ns0:response_spectrum')
@@ -51,21 +49,23 @@
 
         # sort table option
         clientObject.user_defined_spectrum_sorted = sort_table
 
         # user defined spectrum
         clientObject.user_defined_response_spectrum = model.clientModel.factory.create('ns0:response_spectrum.user_defined_response_spectrum')
 
-        for i,j in enumerate(user_defined_spectrum):
-            rsp = model.clientModel.factory.create('ns0:response_spectrum_user_defined_response_spectrum_row')
-            rsp.no = i+1
-            rsp.row.period = user_defined_spectrum[i][0]
-            rsp.row.acceleration = user_defined_spectrum[i][1]
+        if user_defined_spectrum:
+            for i,j in enumerate(user_defined_spectrum):
+                rsp = model.clientModel.factory.create('ns0:response_spectrum_user_defined_response_spectrum_row')
+                rsp.no = i+1
+                rsp.row = model.clientModel.factory.create('ns0:response_spectrum_user_defined_response_spectrum')
+                rsp.row.period = user_defined_spectrum[i][0]
+                rsp.row.acceleration = user_defined_spectrum[i][1]
 
-            clientObject.user_defined_response_spectrum.response_spectrum_user_defined_response_spectrum.append(rsp)
+                clientObject.user_defined_response_spectrum.response_spectrum_user_defined_response_spectrum.append(rsp)
 
         # comment
         clientObject.comment = comment
 
         # adding optional parameters via dictionary
         if params:
             for key in params:
@@ -130,14 +130,15 @@
 
         # user defined spectrum
         clientObject.user_defined_response_spectrum = model.clientModel.factory.create('ns0:response_spectrum.user_defined_response_spectrum')
 
         for i,j in enumerate(user_defined_spectrum):
             rsp = model.clientModel.factory.create('ns0:response_spectrum_user_defined_response_spectrum_row')
             rsp.no = i+1
+            rsp.row = model.clientModel.factory.create('ns0:response_spectrum_user_defined_response_spectrum')
             rsp.row.period = user_defined_spectrum[i][0]
             rsp.row.acceleration = user_defined_spectrum[i][1]
 
             clientObject.user_defined_response_spectrum.response_spectrum_user_defined_response_spectrum.append(rsp)
 
         # comment
         clientObject.comment = comment
```

### Comparing `RSTAB-1.5.0/RSTAB/Imperfections/imperfectionCase.py` & `RSTAB-1.6.0/RSTAB/Imperfections/imperfectionCase.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,15 @@
 
         # Level Imperfections Table
         clientObject.level_imperfections = model.clientModel.factory.create('ns0:array_of_imperfection_case_level_imperfections')
 
         for i in level_imperfections:
             li_proto = model.clientModel.factory.create('ns0:imperfection_case_level_imperfections_row')
             li_proto.no = i['no']
+            li_proto.row = model.clientModel.factory.create('ns0:imperfection_case_level_imperfections')
             li_proto.row.level = i['level']
             li_proto.row.e_1 = i['e_1']
             li_proto.row.theta_1 = i['theta_1']
             li_proto.row.e_2 = i['e_2']
             li_proto.row.theta_2 = i['theta_2']
             li_proto.row.comment = i['comment']
 
@@ -456,14 +457,15 @@
 
         # Imperfection Case Items
         clientObject.imperfection_cases_items = model.clientModel.factory.create('ns0:array_of_imperfection_case_imperfection_cases_items')
 
         for i in imperfection_cases:
             li_proto = model.clientModel.factory.create('ns0:imperfection_case_imperfection_cases_items_row')
             li_proto.no = i['no']
+            li_proto.row = model.clientModel.factory.create('ns0:imperfection_case_imperfection_cases_items')
             li_proto.row.name = i['name']
             li_proto.row.factor = i['factor']
             li_proto.row.operator_type = i['operator_type']
             li_proto.row.comment = i['comment']
 
             clientObject.imperfection_cases_items.imperfection_case_imperfection_cases_items.append(li_proto)
```

### Comparing `RSTAB-1.5.0/RSTAB/Imperfections/memberImperfection.py` & `RSTAB-1.6.0/RSTAB/Imperfections/memberImperfection.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/Imperfections/membersetImperfection.py` & `RSTAB-1.6.0/RSTAB/Imperfections/membersetImperfection.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/ImportExport/exports.py` & `RSTAB-1.6.0/RSTAB/ImportExport/exports.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/ImportExport/imports.py` & `RSTAB-1.6.0/RSTAB/ImportExport/imports.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-from RSTAB.initModel import client
+import os
+from RSTAB.initModel import client, Model
 
 def importFrom(targetFilePath: str):
     '''
     Allowed file extensions are .xml, .saf and .xlsx.
 
     Args:
         targetFilePath (string): Destination path to the file
     '''
     client.service.import_from(targetFilePath)
+    head, tail = os.path.split(targetFilePath)
+    if '.' in tail:
+            tail = tail.split('.')[0]
+    Model(False, tail)
 
 def getConversionTables():
     '''
     Get conversion tables.
     '''
     return client.service.get_conversion_tables()
```

### Comparing `RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/designSituation.py` & `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/designSituation.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/loadCasesAndCombinations.py` & `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/loadCasesAndCombinations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from RSTAB.initModel import Model, clearAttributes
-from enum import Enum
 
 class LoadCasesAndCombinations():
 
     def __init__(self,
                  params: dict = {
                     "current_standard_for_combination_wizard": 6207,
                     "activate_combination_wizard_and_classification": True,
@@ -14,14 +13,15 @@
                     "combination_name_according_to_action_category": False
                  },
                  model= Model):
 
         """
         Args:
             params(dict, optional): Combination Wizard Parameters
+            model (RSTAB Class, optional): Model to be edited
 
                         National Annex                                      Codes
                        ----------------                                     -----
         NATIONAL_ANNEX_AND_EDITION_EN_1990_CEN_2010_04		                6207
         NATIONAL_ANNEX_AND_EDITION_EN_1990_BDS_2015_02		                6034
         NATIONAL_ANNEX_AND_EDITION_EN_1990_BS_2009_06		                6035
         NATIONAL_ANNEX_AND_EDITION_EN_1990_CSN_2015_05		                6036
```

### Comparing `RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/loadCombination.py` & `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/loadCombination.py`

 * *Files 17% similar despite different names*

```diff
@@ -82,39 +82,19 @@
 
         # Items
         clientObject.items = model.clientModel.factory.create('ns0:load_combination.items')
 
         for i,j in enumerate(combination_items):
             mlvlp = model.clientModel.factory.create('ns0:load_combination_items_row')
             mlvlp.no = i+1
+            mlvlp.row = model.clientModel.factory.create('ns0:load_combination_items')
             mlvlp.row.factor = combination_items[i][0]
             mlvlp.row.load_case = combination_items[i][1]
             mlvlp.row.action = combination_items[i][2]
             mlvlp.row.is_leading = combination_items[i][3]
-            mlvlp.row.gamma=0
-            mlvlp.row.psi=0
-            mlvlp.row.xi=0
-            mlvlp.row.k_fi=0
-            mlvlp.row.c_esl=0
-            mlvlp.row.k_def=0
-            mlvlp.row.psi_0=0
-            mlvlp.row.psi_1=0
-            mlvlp.row.psi_2=0
-            mlvlp.row.fi=0
-            mlvlp.row.gamma_0=0
-            mlvlp.row.alfa=0
-            mlvlp.row.k_f=0
-            mlvlp.row.phi=0
-            mlvlp.row.rho=0
-            mlvlp.row.omega_0=0
-            mlvlp.row.gamma_l_1=0
-            mlvlp.row.k_creep=0
-            mlvlp.row.shift=0
-            mlvlp.row.amplitude_function_type = "CONSTANT"
-
 
             clientObject.items.load_combination_items.append(mlvlp)
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
         # Add Load Combination to client model
```

### Comparing `RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/modalAnalysisSettings.py` & `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/modalAnalysisSettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class ModalAnalysisSettings():
 
     def __init__(self,
                  no: int = 1,
                  name: str = 'Modal Analysis Settings',
                  number_of_modes_method = ModalNumberOfModes.NUMBER_OF_MODES_METHOD_USER_DEFINED,
                  number_of_modes : int = 4,
-                 solution_method = ModalSolutionMethod.SOLUTION_METHOD_SHIFTED_INVERSE_POWER_METHOD,
+                 solution_method = ModalSolutionMethod.METHOD_SHIFTED_INVERSE_POWER_METHOD,
                  find_modes_beyond_frequency: bool = False,
                  frequency_f: float = 10,
                  maxmimum_natural_frequency: float = 1700,
                  effective_modal_mass_factor: float = 0.85,
                  mass_matrix_type = ModalMassMatrixType.MASS_MATRIX_TYPE_CONSISTENT,
                  mass_conversion_type = ModalMassConversionType.MASS_CONVERSION_TYPE_Z_COMPONENTS_OF_LOADS,
                  acting_masses: list = None,
@@ -109,15 +109,15 @@
         # Add Static Analysis Settings to client model
         model.clientModel.service.set_modal_analysis_settings(clientObject)
 
     @staticmethod
     def UserDefined(no: int = 1,
                     name: str = 'Modal Analysis User Defined',
                     number_of_modes : int = 4,
-                    solution_method = ModalSolutionMethod.SOLUTION_METHOD_SHIFTED_INVERSE_POWER_METHOD,
+                    solution_method = ModalSolutionMethod.METHOD_SHIFTED_INVERSE_POWER_METHOD,
                     find_modes_beyond_frequency: bool = False,
                     frequency_f: float = 10,
                     mass_matrix_type = ModalMassMatrixType.MASS_MATRIX_TYPE_CONSISTENT,
                     mass_conversion_type = ModalMassConversionType.MASS_CONVERSION_TYPE_Z_COMPONENTS_OF_LOADS,
                     acting_masses: list = None,
                     neglect_masses = ModalNeglectMasses.E_NEGLECT_MASSES_NO_NEGLECTION,
                     comment: str = '',
@@ -197,15 +197,15 @@
 
         # Add Static Analysis Settings to client model
         model.clientModel.service.set_modal_analysis_settings(clientObject)
 
     @staticmethod
     def EffectiveMass(no: int = 1,
                       name: str = 'Modal Analysis Effective Mass',
-                      solution_method = ModalSolutionMethod.SOLUTION_METHOD_SHIFTED_INVERSE_POWER_METHOD,
+                      solution_method = ModalSolutionMethod.METHOD_SHIFTED_INVERSE_POWER_METHOD,
                       effective_modal_mass_factor: float = 0.85,
                       mass_matrix_type = ModalMassMatrixType.MASS_MATRIX_TYPE_CONSISTENT,
                       mass_conversion_type = ModalMassConversionType.MASS_CONVERSION_TYPE_Z_COMPONENTS_OF_LOADS,
                       acting_masses: list = None,
                       neglect_masses = ModalNeglectMasses.E_NEGLECT_MASSES_NO_NEGLECTION,
                       comment: str = '',
                       params: dict = None,
@@ -279,15 +279,15 @@
 
         # Add Static Analysis Settings to client model
         model.clientModel.service.set_modal_analysis_settings(clientObject)
 
     @staticmethod
     def MaximumFrequency(no: int = 1,
                          name: str = 'Modal Analysis Maximum Freq',
-                         solution_method = ModalSolutionMethod.SOLUTION_METHOD_SHIFTED_INVERSE_POWER_METHOD,
+                         solution_method = ModalSolutionMethod.METHOD_SHIFTED_INVERSE_POWER_METHOD,
                          find_modes_beyond_frequency: bool = False,
                          frequency_f: float = 10,
                          maxmimum_natural_frequency: float = 1700,
                          mass_matrix_type = ModalMassMatrixType.MASS_MATRIX_TYPE_CONSISTENT,
                          mass_conversion_type = ModalMassConversionType.MASS_CONVERSION_TYPE_Z_COMPONENTS_OF_LOADS,
                          acting_masses: list = None,
                          neglect_masses = ModalNeglectMasses.E_NEGLECT_MASSES_NO_NEGLECTION,
```

### Comparing `RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/resultCombination.py` & `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/resultCombination.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/spectralAnalysisSettings.py` & `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/spectralAnalysisSettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
             damping_for_cqc_rule (enum): Cqs Damping Rule Enumeration
             constant_d_for_each_mode (float): Constant d for Each Mode
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         '''
         # Check if Spectral Add-on is active.
-        if not GetAddonStatus(Model.clientModel, AddOn.spectral_active):
-            SetAddonStatus(Model.clientModel, AddOn.spectral_active)
+        if not GetAddonStatus(model.clientModel, AddOn.spectral_active):
+            SetAddonStatus(model.clientModel, AddOn.spectral_active)
 
         # Client model | Surface
         clientObject = model.clientModel.factory.create('ns0:spectral_analysis_settings')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
```

### Comparing `RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/stabilityAnalysisSettings.py` & `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/stabilityAnalysisSettings.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/LoadCasesAndCombinations/staticAnalysisSettings.py` & `RSTAB-1.6.0/RSTAB/LoadCasesAndCombinations/staticAnalysisSettings.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,32 +50,32 @@
         # Add Static Analysis Settings to client model
         model.clientModel.service.set_static_analysis_settings(clientObject)
 
     @staticmethod
     def GeometricallyLinear(
                   no: int = 1,
                   name: str = None,
-                  load_modification = [False, 1, False],
+                  load_modification: list = [False, 1, False],
                   bourdon_effect: bool = False,
-                  mass_conversion = [False, 0, 0, 0],
+                  mass_conversion: list = [False, 0, 0, 0],
                   comment: str = '',
                   params: dict = None,
                   model = Model):
 
         """
         Args:
             no (int): Static Analysis Setting Tag
             name (str): Static Analysis Setting Name
             load_modification (list): Load Modification Parameters
                 load_modification = [loading_by_multiplier_factor, multiplier_factor, dividing_results]
             mass_conversion (list): Mass Conversion Parameters
                 mass_conversion = [mass_conversion_enabled, mass_conversion_factor_in_direction_x, mass_conversion_factor_in_direction_y, mass_conversion_factor_in_direction_z]
-            comment (str): Comments
-            params (dict): Any WS Parameter relevant to the object and its value in form of a dictionary
-            model (RSTAB Class): Model to be edited
+            comment (str, optional): Comments
+            params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
+            model (RSTAB Class, optional): Model to be edited
         """
 
         # Client model
         clientObject = model.clientModel.factory.create('ns0:static_analysis_settings')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
@@ -124,17 +124,17 @@
     def LargeDeformation(
                   no: int = 1,
                   name: str = None,
                   iterative_method = StaticAnalysisSettingsIterativeMethodForNonlinearAnalysis.NEWTON_RAPHSON,
                   precision_of_convergence_criteria_for_nonlinear_calculation: float = 0,
                   max_number_of_iterations: float = 100,
                   number_of_load_increments: float = 1,
-                  load_modification = [False, 1, False],
+                  load_modification: list = [False, 1, False],
                   bourdon_effect: bool = True,
-                  mass_conversion = [False, 0, 0, 1],
+                  mass_conversion: list = [False, 0, 0, 1],
                   comment: str = '',
                   params: dict = {'save_results_of_all_load_increments': False},
                   model = Model):
 
         """
         Args:
             no (int): Static Analysis Setting Tag
@@ -144,17 +144,17 @@
             max_number_of_iterations (float): Maximum Number of Iterations
             number_of_load_increments (float): Number of Load Increments
             load_modification (list): Load Modification Parameters
                 load_modification = [loading_by_multiplier_factor, multiplier_factor, dividing_results]
             bourdon_effect (bool): Bourdon Effect Boolean
             mass_conversion (list): Mass Conversion Parameters
                 mass_conversion = [mass_conversion_enabled, mass_conversion_factor_in_direction_x, mass_conversion_factor_in_direction_y, mass_conversion_factor_in_direction_z]
-            comment (str): Comments
-            params (dict): Any WS Parameter relevant to the object and its value in form of a dictionary
-            model (RSTAB Class): Model to be edited
+            comment (str, optional): Comments
+            params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
+            model (RSTAB Class, optional): Model to be edited
         """
 
         # Client model
         clientObject = model.clientModel.factory.create('ns0:static_analysis_settings')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
@@ -170,16 +170,15 @@
         # Static Analysis Type
         clientObject.analysis_type = StaticAnalysisType.LARGE_DEFORMATIONS.name
 
         # Bourdon Effect Displacement
         clientObject.displacements_due_to_bourdon_effect = bourdon_effect
 
         # Iterative Method
-        # TODO: bug 32711
-        #clientObject.iterative_method_for_nonlinear_analysis = iterative_method.name
+        clientObject.iterative_method_for_nonlinear_analysis = iterative_method.name
 
         clientObject.max_number_of_iterations = max_number_of_iterations
         clientObject.number_of_load_increments = number_of_load_increments
 
         # Conversion of Mass into Load
         clientObject.mass_conversion_enabled = mass_conversion[0]
         if mass_conversion[0]:
@@ -217,20 +216,20 @@
 
     @staticmethod
     def SecondOrderPDelta(
                   no: int = 1,
                   name: str = None,
                   max_number_of_iterations: int = 100,
                   number_of_load_increments: int = 1,
-                  load_modification = [False, 0, False],
+                  load_modification: list = [False, 0, False],
                   precision_of_convergence_criteria_for_nonlinear_calculation: float = 0,
                   favorable_effect_due_to_tension_in_members : bool = False,
                   bourdon_effect: bool = True,
-                  internal_forces_to_deformed_structure = [True, True, True, True],
-                  mass_conversion = [False, 0, 0, 1],
+                  internal_forces_to_deformed_structure: list = [True, True, True, True],
+                  mass_conversion: list = [False, 0, 0, 1],
                   comment: str = '',
                   params: dict = None,
                   model = Model):
         """
         Args:
             no (int): Static Analysis Setting Tag
             name (str):  Static Analysis Setting Name
@@ -241,17 +240,17 @@
             precision_of_convergence_criteria_for_nonlinear_calculation (float): Precision of Convergence defaults to 0
             favorable_effect_due_to_tension_in_members (bool): Favorable Effect due to Tension In Members Boolean
             bourdon_effect (bool): Bourdon Effect Boolean
             internal_forces_to_deformed_structure (list): Internal Forces to Deformed Structure List
                 internal_forces_to_deformed_structure = [refer_internal_forces_to_deformed_structure, internal_forces_to_deformed_structure_for_moments, internal_forces_to_deformed_structure_for_normal_forces, internal_forces_to_deformed_structure_for_shear_forces]
             mass_conversion (list): Mass Conversion Parameters
                 mass_conversion = [mass_conversion_enabled, mass_conversion_factor_in_direction_x, mass_conversion_factor_in_direction_y, mass_conversion_factor_in_direction_z]
-            comment (str): Comments
-            params (dict): Any WS Parameter relevant to the object and its value in form of a dictionary
-            model (RSTAB Class): Model to be edited
+            comment (str, optional): Comments
+            params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
+            model (RSTAB Class, optional): Model to be edited
         """
 
         # Client model
         clientObject = model.clientModel.factory.create('ns0:static_analysis_settings')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
```

### Comparing `RSTAB-1.5.0/RSTAB/Loads/imposedNodalDeformation.py` & `RSTAB-1.6.0/RSTAB/Loads/imposedNodalDeformation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes
+from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
 
 class ImposedNodalDeformation():
 
     def __init__(self,
                  no: int = 1,
                  load_case_no: int = 1,
                  node_no: str = '1',
@@ -31,16 +31,15 @@
         # Load No.
         clientObject.no = no
 
         # Load Case No.
         clientObject.load_case = load_case_no
 
         # Assigned Node No.
-        #clientObject.node_no = ConvertToDlString(node_no()
-        clientObject.nodes = node_no
+        clientObject.nodes = ConvertToDlString(node_no)
 
         # Load Parameter
         clientObject.imposed_displacement_x = load_parameter[0]
         clientObject.imposed_displacement_y = load_parameter[1]
         clientObject.imposed_displacement_z = load_parameter[2]
 
         clientObject.imposed_rotation_x = load_parameter[3]
```

### Comparing `RSTAB-1.5.0/RSTAB/Loads/memberLoad.py` & `RSTAB-1.6.0/RSTAB/Loads/memberLoad.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         # Member Load Distribution
         load_distribution = MemberLoadDistribution.LOAD_DISTRIBUTION_UNIFORM
         clientObject.load_distribution = load_distribution.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         clientObject.magnitude = magnitude
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -146,15 +146,15 @@
         # Member Load Type
         load_type = MemberLoadType.LOAD_TYPE_FORCE
         clientObject.load_type = load_type.name
 
         # Member Load Distribution
         clientObject.load_distribution= load_distribution.name
 
-        #Load Magnitude and Parameters
+        # Load Magnitude and Parameters
         if load_distribution.name == "LOAD_DISTRIBUTION_UNIFORM" or load_distribution.name == "LOAD_DISTRIBUTION_UNIFORM_TOTAL":
             clientObject.magnitude = load_parameter[0]
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_CONCENTRATED_1":
             clientObject.distance_a_is_defined_as_relative = load_parameter[0]
             if load_parameter[0] == False:
                 clientObject.magnitude = load_parameter[1]
@@ -220,21 +220,17 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
 
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
             clientObject.distance_a_is_defined_as_relative = load_parameter[0]
             clientObject.distance_b_is_defined_as_relative = load_parameter[1]
             clientObject.magnitude_1 = load_parameter[2]
@@ -274,48 +270,40 @@
         elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING":
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING_IN_Z":
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Reference to List of Members
+        # Reference to List of Members
         clientObject.reference_to_list_of_members = list_reference
 
-        #Force Eccentiricity
+        # Force Eccentiricity
         clientObject.has_force_eccentricity = force_eccentricity
 
         if force_eccentricity == True:
 
             params_ecc = {'eccentricity_horizontal_alignment': MemberLoadEccentricityHorizontalAlignment.ALIGN_NONE,
                            'eccentricity_vertical_alignment': MemberLoadEccentricityVerticalAlignment.ALIGN_NONE,
                            'eccentricity_section_middle': MemberLoadEccentricitySectionMiddle.LOAD_ECCENTRICITY_SECTION_MIDDLE_CENTER_OF_GRAVITY,
@@ -426,15 +414,15 @@
         # Member Load Type
         load_type = MemberLoadType.LOAD_TYPE_MOMENT
         clientObject.load_type = load_type.name
 
         # Member Load Distribution
         clientObject.load_distribution= load_distribution.name
 
-        #Load Magnitude and Parameters
+        # Load Magnitude and Parameters
         if load_distribution.name == "LOAD_DISTRIBUTION_UNIFORM":
             clientObject.magnitude = load_parameter[0]
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_CONCENTRATED_1":
             clientObject.distance_a_is_defined_as_relative = load_parameter[0]
             if load_parameter[0] == False:
                 clientObject.magnitude = load_parameter[1]
@@ -500,21 +488,17 @@
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
 
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
             clientObject.distance_a_is_defined_as_relative = load_parameter[0]
             clientObject.distance_b_is_defined_as_relative = load_parameter[1]
             clientObject.magnitude_1 = load_parameter[2]
@@ -554,28 +538,24 @@
         elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING":
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Reference to List of Members
+        # Reference to List of Members
         clientObject.reference_to_list_of_members = list_reference
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -722,15 +702,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = load_distribution.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         if load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_UNIFORM:
             clientObject.magnitude_t_b = load_parameter[0]
             clientObject.magnitude_t_t = load_parameter[1]
 
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             clientObject.magnitude_t_b_1 = load_parameter[0]
             clientObject.magnitude_t_b_2 = load_parameter[1]
@@ -788,17 +768,17 @@
         elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING":
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
-                mlvlp.row.note = None
                 mlvlp.row.magnitude_t_c = load_parameter[i][1]
                 mlvlp.row.magnitude_delta_t = load_parameter[i][2]
                 mlvlp.row.magnitude_t_t = load_parameter[i][1]
                 mlvlp.row.magnitude_t_b = load_parameter[i][2]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
@@ -882,15 +862,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = load_distribution.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         if load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_UNIFORM:
             clientObject.magnitude_delta_t = load_parameter[0]
             clientObject.magnitude_t_c = load_parameter[1]
 
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             clientObject.magnitude_delta_t_1 = load_parameter[0]
             clientObject.magnitude_delta_t_2 = load_parameter[1]
@@ -948,17 +928,17 @@
         elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING":
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
-                mlvlp.row.note = None
                 mlvlp.row.magnitude_t_c = load_parameter[i][1]
                 mlvlp.row.magnitude_delta_t = load_parameter[i][2]
                 mlvlp.row.magnitude_t_t = load_parameter[i][1]
                 mlvlp.row.magnitude_t_b = load_parameter[i][2]
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
@@ -1039,15 +1019,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = load_distribution.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         if load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_UNIFORM:
             clientObject.magnitude = load_parameter[0]
 
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             clientObject.magnitude_1 = load_parameter[0]
             clientObject.magnitude_2 = load_parameter[1]
 
@@ -1097,21 +1077,17 @@
         elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING":
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Reference to list of members
         clientObject.reference_to_list_of_members = list_reference
 
         # Comment
@@ -1172,15 +1148,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = MemberLoadDistribution.LOAD_DISTRIBUTION_UNIFORM.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         clientObject.magnitude = magnitude
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -1253,15 +1229,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = load_distribution.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         if load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_UNIFORM:
             clientObject.magnitude = load_parameter[0]
 
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             clientObject.magnitude_1 = load_parameter[0]
             clientObject.magnitude_2 = load_parameter[1]
 
@@ -1311,21 +1287,17 @@
         elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING":
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Reference to list of members
         clientObject.reference_to_list_of_members = list_reference
 
         # Comment
@@ -1386,15 +1358,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = MemberLoadDistribution.LOAD_DISTRIBUTION_UNIFORM.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         clientObject.magnitude = magnitude
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -1477,15 +1449,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = load_distribution.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         if load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_UNIFORM:
             clientObject.magnitude = load_parameter[0]
 
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_1:
             clientObject.magnitude = load_parameter[0]
             clientObject.distance_a_is_defined_as_relative = load_parameter[1]
             if load_parameter[1]:
@@ -1549,21 +1521,17 @@
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_VARYING:
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 3:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             clientObject.magnitude_1 = load_parameter[0]
             clientObject.magnitude_2 = load_parameter[1]
 
@@ -1610,21 +1578,17 @@
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_VARYING:
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Reference to list of members
         clientObject.reference_to_list_of_members = list_reference
 
         # Comment
@@ -1711,15 +1675,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = load_distribution.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         if load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_UNIFORM:
             clientObject.magnitude = load_parameter[0]
 
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_1:
             clientObject.magnitude = load_parameter[0]
             clientObject.distance_a_is_defined_as_relative = load_parameter[1]
             if load_parameter[1]:
@@ -1783,21 +1747,17 @@
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_VARYING:
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             clientObject.magnitude_1 = load_parameter[0]
             clientObject.magnitude_2 = load_parameter[1]
 
@@ -1844,21 +1804,17 @@
         elif load_distribution == MemberLoadDistribution.LOAD_DISTRIBUTION_VARYING:
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
                 if len(load_parameter[i]) != 2:
                     raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
                 mlvlp.row.magnitude = load_parameter[i][1]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
 
                 clientObject.varying_load_parameters.member_load_varying_load_parameters.append(mlvlp)
 
         # Reference to list of members
         clientObject.reference_to_list_of_members = list_reference
 
         # Comment
@@ -1919,18 +1875,18 @@
 
         # Member Load Distribution
         clientObject.load_distribution = MemberLoadDistribution.LOAD_DISTRIBUTION_UNIFORM.name
 
         # Member Load Direction
         clientObject.load_direction = MemberLoadDirection.LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W_TRUE.name
 
-        #Member Load Orientation
+        # Member Load Orientation
         clientObject.load_direction_orientation = load_direction_orientation.name
 
-        #Load Magnitude
+        # Load Magnitude
         clientObject.magnitude = specific_weight
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -1989,21 +1945,21 @@
 
         # Member Load Distribution
         clientObject.load_distribution = MemberLoadDistribution.LOAD_DISTRIBUTION_UNIFORM.name
 
         # Member Load Direction
         clientObject.load_direction = MemberLoadDirection.LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W_TRUE.name
 
-        #Member Load Orientation
+        # Member Load Orientation
         clientObject.load_direction_orientation = load_direction_orientation.name
 
-        #Load Magnitude
+        # Load Magnitude
         clientObject.magnitude = specific_weight
 
-        #Filling Height
+        # Filling Height
         clientObject.filling_height = filling_height
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -2058,15 +2014,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = MemberLoadDistribution.LOAD_DISTRIBUTION_UNIFORM.name
 
         # Member Load Direction
         clientObject.load_direction = MemberLoadDirection.LOAD_DIRECTION_LOCAL_X.name
 
-        #Load Magnitude
+        # Load Magnitude
         clientObject.magnitude = pressure
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -2127,24 +2083,24 @@
         # Members No. (e.g. '5 6 7 12')
         clientObject.members = ConvertToDlString(members_no)
 
         # Member Load Type
         load_type = MemberLoadType.LOAD_TYPE_ROTARY_MOTION
         clientObject.load_type = load_type.name
 
-        #Angular Acceleration
+        # Angular Acceleration
         clientObject.angular_acceleration = angular_acceleration
 
-        #Angular Velocity
+        # Angular Velocity
         clientObject.angular_velocity = angular_velocity
 
-        #Axis Definition Type
+        # Axis Definition Type
         clientObject.axis_definition_type = axis_definition_type.name
 
-        #Axis definition
+        # Axis definition
         if axis_definition_type == MemberLoadAxisDefinitionType.AXIS_DEFINITION_TWO_POINTS.name:
             clientObject.axis_definition_p1_x = axis_definition_p1[0]
             clientObject.axis_definition_p1_y = axis_definition_p1[1]
             clientObject.axis_definition_p1_z = axis_definition_p1[2]
 
             clientObject.axis_definition_p2_x = axis_definition_p2[0]
             clientObject.axis_definition_p2_y = axis_definition_p2[1]
```

### Comparing `RSTAB-1.5.0/RSTAB/Loads/membersetload.py` & `RSTAB-1.6.0/RSTAB/Loads/membersetload.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         # Member Load Distribution
         load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_UNIFORM
         clientObject.load_distribution = load_distribution.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         clientObject.magnitude = magnitude
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -98,25 +98,25 @@
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_N:
                     load_parameter = [relative_distance_a = False, relative_distance_b = False, magnitude, count_n, distance_a, distance_b]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_2x2:
                     load_parameter = [relative_distance_a = False, relative_distance_b = False, relative_distance_c = False, magnitude, distance_a, distance_b, distance_c]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_2:
                     load_parameter = [relative_distance_a = False, relative_distance_b = False, magnitude_1, magnitude_2, distance_a, distance_b]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_VARYING:
-                    load_parameter = [[distance, delta_distance, magnitude], ...]
+                    load_parameter = [[distance, magnitude], ...]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
                     load_parameter = [relative_distance_a = False, relative_distance_b = False,magnitude_1, magnitude_2, distance_a, distance_b]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_TAPERED:
                     load_parameter = [relative_distance_a = False, relative_distance_b = False,magnitude_1, magnitude_2, distance_a, distance_b]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_PARABOLIC:
                     load_parameter = [magnitude_1, magnitude_2, magnitude_3]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_VARYING:
-                    load_parameter = [[distance, delta_distance, magnitude], ...]
+                    load_parameter = [[distance, magnitude], ...]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_VARYING_IN_Z:
-                    load_parameter = [[distance, delta_distance, magnitude], ...]
+                    load_parameter = [[distance, magnitude], ...]
             force_eccentricity (bool): Force Eccentricity Option
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
                 for force_eccentricity == True:
                     params = {'eccentricity_horizontal_alignment': MemberSetLoadEccentricityHorizontalAlignment.ALIGN_NONE,
                     'eccentricity_vertical_alignment': MemberSetLoadEccentricityVerticalAlignment.ALIGN_NONE,
                     'eccentricity_section_middle': MemberSetLoadEccentricitySectionMiddle.LOAD_ECCENTRICITY_SECTION_MIDDLE_CENTER_OF_GRAVITY,
@@ -145,15 +145,15 @@
         # Member Load Type
         load_type = MemberSetLoadType.LOAD_TYPE_FORCE
         clientObject.load_type = load_type.name
 
         # Member Load Distribution
         clientObject.load_distribution= load_distribution.name
 
-        #Load Magnitude and Parameters
+        # Load Magnitude and Parameters
         if load_parameter == []:
             raise ValueError("WARNING: Load parameter cannot be empty. Kindly check list inputs completeness and correctness.")
         else:
             if load_distribution.name == "LOAD_DISTRIBUTION_UNIFORM" or load_distribution.name == "LOAD_DISTRIBUTION_UNIFORM_TOTAL":
                 if len(load_parameter) == 1:
                     clientObject.magnitude = load_parameter[0]
                 else:
@@ -232,26 +232,21 @@
                         clientObject.distance_b_relative = load_parameter[5]
                 else:
                     raise ValueError("WARNING: Load parameter array length should be 6 for LOAD_DISTRIBUTION_CONCENTRATED_2. Kindly check list inputs completeness and correctness.")
 
             elif load_distribution.name == "LOAD_DISTRIBUTION_CONCENTRATED_VARYING":
                 clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
                 for i,j in enumerate(load_parameter):
-                    if len(load_parameter[i]) != 3:
+                    if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                     mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                     mlvlp.no = i+1
+                    mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
                     mlvlp.row.distance = load_parameter[i][0]
-                    mlvlp.row.delta_distance = load_parameter[i][1]
-                    mlvlp.row.magnitude = load_parameter[i][2]
-                    mlvlp.row.note = None
-                    mlvlp.row.magnitude_t_c = 0.0
-                    mlvlp.row.magnitude_delta_t = 0.0
-                    mlvlp.row.magnitude_t_t = 0.0
-                    mlvlp.row.magnitude_t_b = 0.0
+                    mlvlp.row.magnitude = load_parameter[i][1]
 
                     clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
             elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
                 if len(load_parameter) == 6:
                     clientObject.distance_a_is_defined_as_relative = load_parameter[0]
                     clientObject.distance_b_is_defined_as_relative = load_parameter[1]
@@ -295,51 +290,41 @@
                     clientObject.magnitude_2 = load_parameter[1]
                     clientObject.magnitude_3 = load_parameter[2]
                 else:
                     raise ValueError("WARNING: Load parameter array length should be 3 for LOAD_DISTRIBUTION_PARABOLIC. Kindly check list inputs completeness and correctness.")
             elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING":
                 clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
                 for i,j in enumerate(load_parameter):
-                    if len(load_parameter[i]) != 3:
+                    if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                     mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                     mlvlp.no = i+1
+                    mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
                     mlvlp.row.distance = load_parameter[i][0]
-                    mlvlp.row.delta_distance = load_parameter[i][1]
-                    mlvlp.row.magnitude = load_parameter[i][2]
-                    mlvlp.row.note = None
-                    mlvlp.row.magnitude_t_c = 0.0
-                    mlvlp.row.magnitude_delta_t = 0.0
-                    mlvlp.row.magnitude_t_t = 0.0
-                    mlvlp.row.magnitude_t_b = 0.0
+                    mlvlp.row.magnitude = load_parameter[i][1]
 
                     clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
             elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING_IN_Z":
                 clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
                 for i,j in enumerate(load_parameter):
-                    if len(load_parameter[i]) != 3:
+                    if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                     mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                     mlvlp.no = i+1
+                    mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
                     mlvlp.row.distance = load_parameter[i][0]
-                    mlvlp.row.delta_distance = load_parameter[i][1]
-                    mlvlp.row.magnitude = load_parameter[i][2]
-                    mlvlp.row.note = None
-                    mlvlp.row.magnitude_t_c = 0.0
-                    mlvlp.row.magnitude_delta_t = 0.0
-                    mlvlp.row.magnitude_t_t = 0.0
-                    mlvlp.row.magnitude_t_b = 0.0
+                    mlvlp.row.magnitude = load_parameter[i][1]
 
                     clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Force Eccentiricity
+        # Force Eccentiricity
         clientObject.has_force_eccentricity = force_eccentricity
 
         if force_eccentricity == True:
             if 'eccentricity_horizontal_alignment' and 'eccentricity_vertical_alignment' and 'eccentricity_section_middle' \
                 'is_eccentricity_at_end_different_from_start' and 'eccentricity_y_at_end' and 'eccentricity_y_at_start' \
                 'eccentricity_z_at_end' and 'eccentricity_z_at_start' in params:
                 pass
@@ -419,23 +404,23 @@
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_N:
                     load_parameter = [relative_distance_a = False, relative_distance_b = False, magnitude, count_n, distance_a, distance_b]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_2x2:
                     load_parameter = [relative_distance_a = False, relative_distance_b = False, relative_distance_c = False, magnitude, distance_a, distance_b, distance_c]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_2:
                     load_parameter = [relative_distance_a = False, relative_distance_b = False, magnitude_1, magnitude_2, distance_a, distance_b]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_VARYING:
-                    load_parameter = [[distance, delta_distance, magnitude], ...]
+                    load_parameter = [[distance, magnitude], ...]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
                     load_parameter = [relative_distance_a = False, relative_distance_b = False,magnitude_1, magnitude_2, distance_a, distance_b]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_TAPERED:
                     load_parameter = [relative_distance_a = False, relative_distance_b = False,magnitude_1, magnitude_2, distance_a, distance_b]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_PARABOLIC:
                     load_parameter = [magnitude_1, magnitude_2, magnitude_3]
                 for load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_VARYING:
-                    load_parameter = [[distance, delta_distance, magnitude], ...]
+                    load_parameter = [[distance, magnitude], ...]
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
         # Client model | Member Load
         clientObject = model.clientModel.factory.create('ns0:member_set_load')
 
@@ -454,15 +439,15 @@
         # Member Load Type
         load_type = MemberSetLoadType.LOAD_TYPE_MOMENT
         clientObject.load_type = load_type.name
 
         # Member Load Distribution
         clientObject.load_distribution= load_distribution.name
 
-        #Load Magnitude and Parameters
+        # Load Magnitude and Parameters
         if load_distribution.name == "LOAD_DISTRIBUTION_UNIFORM":
             if len(load_parameter) != 1:
                 raise ValueError("WARNING: Load parameter array length should be 1 for LOAD_DISTRIBUTION_UNIFORM. Kindly check list inputs completeness and correctness.")
             clientObject.magnitude = load_parameter[0]
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_CONCENTRATED_1":
             if len(load_parameter) != 3:
@@ -535,26 +520,21 @@
                 clientObject.distance_b_absolute = load_parameter[5]
             else:
                 clientObject.distance_b_relative = load_parameter[5]
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_CONCENTRATED_VARYING":
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                if len(load_parameter[i]) != 3:
+                if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
-                mlvlp.row.delta_distance = load_parameter[i][1]
-                mlvlp.row.magnitude = load_parameter[i][2]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
+                mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_TRAPEZOIDAL":
             if len(load_parameter) != 6:
                 raise ValueError("WARNING: Load parameter array length should be 6 for LOAD_DISTRIBUTION_TRAPEZOIDAL. Kindly check list inputs completeness and correctness.")
             clientObject.distance_a_is_defined_as_relative = load_parameter[0]
@@ -570,15 +550,15 @@
             if load_parameter[1] == False:
                 clientObject.distance_b_absolute = load_parameter[5]
             else:
                 clientObject.distance_b_relative = load_parameter[5]
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_TAPERED":
             if len(load_parameter) != 6:
-                raise ValueError("WARNING: Load parameter array length should be 4 for LOAD_DISTRIBUTION_TAPERED. Kindly check list inputs completeness and correctness.")
+                raise ValueError("WARNING: Load parameter array length should be 6 for LOAD_DISTRIBUTION_TAPERED. Kindly check list inputs completeness and correctness.")
             clientObject.distance_a_is_defined_as_relative = load_parameter[0]
             clientObject.distance_b_is_defined_as_relative = load_parameter[1]
             clientObject.magnitude_1 = load_parameter[2]
             clientObject.magnitude_2 = load_parameter[3]
 
             if load_parameter[0] == False:
                 clientObject.distance_a_absolute = load_parameter[4]
@@ -596,26 +576,21 @@
             clientObject.magnitude_1 = load_parameter[0]
             clientObject.magnitude_2 = load_parameter[1]
             clientObject.magnitude_3 = load_parameter[2]
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING":
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                if len(load_parameter[i]) != 3:
+                if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
-                mlvlp.row.delta_distance = load_parameter[i][1]
-                mlvlp.row.magnitude = load_parameter[i][2]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
+                mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
         # Comment
@@ -729,15 +704,15 @@
                     for load_over_total_length: bool= True:
                         load_parameter = [tt1, tt2, tb1, tb2]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_TAPERED:
                     load_parameter = [tt1, tt2, tb1, tb2, distance_a_relative = False, distance_a_relative = False, a_distance, b_distance]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_PARABOLIC:
                     load_parameter = [tb1, tb2, tb3, tt1, tt2, tt3]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_VARYING:
-                    load_parameter = [[distance, delta_distance, magnitude], ...]
+                    load_parameter = [[distance, magnitude], ...]
             load_over_total_length (bool): Enable/Disable Load Over Total Length Option
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
         # Client model | Member Load
         clientObject = model.clientModel.factory.create('ns0:member_set_load')
@@ -760,17 +735,17 @@
 
         # Member Load Distribution
         clientObject.load_distribution = load_distribution.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         if load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_UNIFORM:
-            if len(load_parameter) !=2:
+            if len(load_parameter) != 2:
                 raise ValueError("WARNING: Load parameter array length should be 2 for LOAD_DISTRIBUTION_UNIFORM. Kindly check list inputs completeness and correctness.")
             clientObject.magnitude_t_b = load_parameter[0]
             clientObject.magnitude_t_t = load_parameter[1]
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             if len(load_parameter) != 8:
                 raise ValueError("WARNING: Load parameter array length should be 8 for LOAD_DISTRIBUTION_TRAPEZOIDAL. Kindly check list inputs completeness and correctness.")
@@ -837,26 +812,24 @@
             clientObject.magnitude_t_t_1 = load_parameter[3]
             clientObject.magnitude_t_t_2 = load_parameter[4]
             clientObject.magnitude_t_t_3 = load_parameter[5]
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING":
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                if len(load_parameter[i]) != 4:
+                if len(load_parameter[i]) != 3:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
-                mlvlp.row.delta_distance = load_parameter[i][1]
-                mlvlp.row.magnitude = load_parameter[i][2]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = load_parameter[i][2]
-                mlvlp.row.magnitude_delta_t = load_parameter[i][3]
-                mlvlp.row.magnitude_t_t = load_parameter[i][2]
-                mlvlp.row.magnitude_t_b = load_parameter[i][3]
+                mlvlp.row.magnitude = load_parameter[i][1]
+                mlvlp.row.magnitude_t_c = load_parameter[i][1]
+                mlvlp.row.magnitude_t_t = load_parameter[i][1]
+                mlvlp.row.magnitude_t_b = load_parameter[i][2]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
@@ -898,15 +871,15 @@
                     for load_over_total_length: bool= True:
                         load_parameter = [delta_t_1, delta_t_2, t_c_1, t_c_2]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_TAPERED:
                     load_parameter = [delta_t_1, delta_t_2, t_c_1, t_c_2, distance_a_relative = False, distance_a_relative = False, a_distance, b_distance]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_PARABOLIC:
                     load_parameter = [delta_t_1, delta_t_2, delta_t_3, t_c_1, t_c_2, t_c_3]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_VARYING:
-                    load_parameter = [[distance, delta_distance, magnitude], ...]
+                    load_parameter = [[distance, magnitude], ...]
             load_over_total_length (bool): Load Over Total Length Option
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
         # Client model | Member Load
         clientObject = model.clientModel.factory.create('ns0:member_set_load')
@@ -929,17 +902,17 @@
 
         # Member Load Distribution
         clientObject.load_distribution = load_distribution.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         if load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_UNIFORM:
-            if len(load_parameter) !=2:
+            if len(load_parameter) != 2:
                 raise ValueError("WARNING: Load parameter array length should be 2 for LOAD_DISTRIBUTION_UNIFORM. Kindly check list inputs completeness and correctness.")
             clientObject.magnitude_delta_t = load_parameter[0]
             clientObject.magnitude_t_c = load_parameter[1]
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             if len(load_parameter) != 8:
                 raise ValueError("WARNING: Load parameter array length should be 8 for LOAD_DISTRIBUTION_TRAPEZOIDAL. Kindly check list inputs completeness and correctness.")
@@ -1000,26 +973,24 @@
             clientObject.magnitude_t_c_1 = load_parameter[3]
             clientObject.magnitude_t_c_2 = load_parameter[4]
             clientObject.magnitude_t_c_3 = load_parameter[5]
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING":
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                if len(load_parameter[i]) != 4:
+                if len(load_parameter[i]) != 3:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
-                mlvlp.row.delta_distance = load_parameter[i][1]
-                mlvlp.row.magnitude = load_parameter[i][2]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = load_parameter[i][2]
-                mlvlp.row.magnitude_delta_t = load_parameter[i][3]
-                mlvlp.row.magnitude_t_t = load_parameter[i][2]
-                mlvlp.row.magnitude_t_b = load_parameter[i][3]
+                mlvlp.row.magnitude = load_parameter[i][1]
+                mlvlp.row.magnitude_t_c = load_parameter[i][1]
+                mlvlp.row.magnitude_t_t = load_parameter[i][1]
+                mlvlp.row.magnitude_t_b = load_parameter[i][2]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
@@ -1061,15 +1032,15 @@
                     for load_over_total_length: bool= True:
                         load_parameter = [epsilon1, epsilon2]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_TAPERED:
                     load_parameter = [epsilon1, epsilon2, distance_a_relative = False, distance_a_relative = False, a_distance, b_distance]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_TAPERED:
                     load_parameter = [epsilon1, epsilon2, epsilon3]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_VARYING:
-                    load_parameter = [[distance, delta_distance, magnitude], ...]
+                    load_parameter = [[distance, magnitude], ...]
             load_over_total_length (bool): Load Over Total Length Option
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
         # Client model | Member Load
         clientObject = model.clientModel.factory.create('ns0:member_set_load')
@@ -1092,15 +1063,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = load_distribution.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         if load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_UNIFORM:
             if len(load_parameter) != 1:
                 raise ValueError("WARNING: Load parameter array length should be 1 for LOAD_DISTRIBUTION_UNIFORM. Kindly check list inputs completeness and correctness.")
             clientObject.magnitude = load_parameter[0]
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             if len(load_parameter) != 6:
@@ -1155,26 +1126,21 @@
             clientObject.magnitude_1 = load_parameter[0]
             clientObject.magnitude_2 = load_parameter[1]
             clientObject.magnitude_3 = load_parameter[2]
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING":
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                if len(load_parameter[i]) != 4:
+                if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
-                mlvlp.row.delta_distance = load_parameter[i][1]
-                mlvlp.row.magnitude = load_parameter[i][2]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
+                mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
@@ -1230,15 +1196,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_UNIFORM.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         clientObject.magnitude = magnitude
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -1279,15 +1245,15 @@
                     for load_over_total_length: bool= True:
                         load_parameter = [magnitude_1, magnitude_2]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_TAPERED:
                     load_parameter = [magnitude_1, magnitude_2, distance_a_relative = False, distance_a_relative = False, a_distance, b_distance]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_PARABOLIC:
                     load_parameter = [magnitude_1, magnitude_2, magnitude_3]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_VARYING:
-                    load_parameter = [[distance, delta_distance, magnitude], ...]
+                    load_parameter = [[distance, magnitude], ...]
             load_over_total_length (bool): Load Over Total Lenth Option
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
         # Client model | Member Load
         clientObject = model.clientModel.factory.create('ns0:member_set_load')
@@ -1310,15 +1276,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = load_distribution.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         if load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_UNIFORM:
             if len(load_parameter) != 1:
                 raise ValueError("WARNING: Load parameter array length should be 1 for LOAD_DISTRIBUTION_UNIFORM. Kindly check list inputs completeness and correctness.")
             clientObject.magnitude = load_parameter[0]
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             if len(load_parameter) != 6:
@@ -1374,26 +1340,21 @@
             clientObject.magnitude_1 = load_parameter[0]
             clientObject.magnitude_2 = load_parameter[1]
             clientObject.magnitude_3 = load_parameter[2]
 
         elif load_distribution.name == "LOAD_DISTRIBUTION_VARYING":
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                if len(load_parameter[i]) != 3:
+                if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
-                mlvlp.row.delta_distance = load_parameter[i][1]
-                mlvlp.row.magnitude = load_parameter[i][2]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
+                mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
@@ -1449,15 +1410,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_UNIFORM.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         clientObject.magnitude = magnitude
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -1497,23 +1458,23 @@
                 for load_distrubition = MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_N:
                     load_parameter = [magnitude, distance_a_is_defined_as_relative = False, distance_b_is_defined_as_relative = False, distance_a, distance_b]
                 for load_distrubition = MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_2x2:
                     load_parameter = [magnitude, distance_a_is_defined_as_relative = False, distance_b_is_defined_as_relative = False, distance_c_is_defined_as_relative = False, distance_a, distance_b, distance_c]
                 for load_distrubition = MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_2:
                     load_parameter = [magnitude_1, magnitude_2, distance_a_is_defined_as_relative = False, distance_b_is_defined_as_relative = False, distance_a, distance_b]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_VARYING:
-                    load_parameter = [[distance, delta_distance, magnitude], ...]
+                    load_parameter = [[distance, magnitude], ...]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_TRAPEZIODAL:
                     load_parameter = [magnitude_1, magnitude_2, distance_a_relative = False, distance_a_relative = False, a_distance, b_distance]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_TAPERED:
                     load_parameter = [magnitude_1, magnitude_2, distance_a_relative = False, distance_a_relative = False, a_distance, b_distance]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_PARABOLIC:
                     load_parameter = [magnitude_1, magnitude_2, magnitude_3]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_VARYING:
-                    load_parameter = [[distance, delta_distance, magnitude], ...]
+                    load_parameter = [[distance, magnitude], ...]
             load_over_total_length (bool): Load Over Total Length Option
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
         # Client model | Member Load
         clientObject = model.clientModel.factory.create('ns0:member_set_load')
@@ -1536,15 +1497,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = load_distribution.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         if load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_UNIFORM:
             if len(load_parameter) != 1:
                 raise ValueError("WARNING: Load parameter array length should be 1 for LOAD_DISTRIBUTION_UNIFORM. Kindly check list inputs completeness and correctness.")
             clientObject.magnitude = load_parameter[0]
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_1:
             if len(load_parameter) != 3:
@@ -1614,26 +1575,21 @@
                 clientObject.distance_b_relative = load_parameter[5]
             else:
                 clientObject.distance_b_absolute = load_parameter[5]
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_VARYING:
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                if len(load_parameter[i]) != 3:
+                if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
-                mlvlp.row.delta_distance = load_parameter[i][1]
-                mlvlp.row.magnitude = load_parameter[i][2]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
+                mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             if len(load_parameter) != 6:
                 raise ValueError("WARNING: Load parameter array length should be 6 for LOAD_DISTRIBUTION_TRAPEZOIDAL. Kindly check list inputs completeness and correctness.")
             clientObject.magnitude_1 = load_parameter[0]
@@ -1677,34 +1633,29 @@
             if load_parameter[3]:
                 clientObject.distance_b_relative = load_parameter[5]
             else:
                 clientObject.distance_b_absolute = load_parameter[5]
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_PARABOLIC:
             if len(load_parameter) != 3:
-                raise ValueError("WARNING: Load parameter array length should be 6 for LOAD_DISTRIBUTION_PARABOLIC. Kindly check list inputs completeness and correctness.")
+                raise ValueError("WARNING: Load parameter array length should be 3 for LOAD_DISTRIBUTION_PARABOLIC. Kindly check list inputs completeness and correctness.")
             clientObject.magnitude_1 = load_parameter[0]
             clientObject.magnitude_2 = load_parameter[1]
             clientObject.magnitude_3 = load_parameter[2]
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_VARYING:
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                if len(load_parameter[i]) != 3:
+                if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
-                mlvlp.row.delta_distance = load_parameter[i][1]
-                mlvlp.row.magnitude = load_parameter[i][2]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
+                mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
@@ -1745,23 +1696,23 @@
                 for load_distrubition = MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_N:
                     load_parameter = [magnitude, distance_a_is_defined_as_relative = False, distance_b_is_defined_as_relative = False, distance_a, distance_b]
                 for load_distrubition = MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_2x2:
                     load_parameter = [magnitude, distance_a_is_defined_as_relative = False, distance_b_is_defined_as_relative = False, distance_c_is_defined_as_relative = False, distance_a, distance_b, distance_c]
                 for load_distrubition = MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_2:
                     load_parameter = [magnitude_1, magnitude_2, distance_a_is_defined_as_relative = False, distance_b_is_defined_as_relative = False, distance_a, distance_b]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_VARYING:
-                    load_parameter = [[distance, delta_distance, magnitude], ...]
+                    load_parameter = [[distance, magnitude], ...]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_TRAPEZIODAL:
                     load_parameter = [magnitude_1, magnitude_2, distance_a_relative = False, distance_a_relative = False, a_distance, b_distance]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_TAPERED:
                     load_parameter = [magnitude_1, magnitude_2, distance_a_relative = False, distance_a_relative = False, a_distance, b_distance]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_PARABOLIC:
                     load_parameter = [magnitude_1, magnitude_2, magnitude_3]
                 for load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_VARYING:
-                    load_parameter = [[distance, delta_distance, magnitude], ...]
+                    load_parameter = [[distance, magnitude], ...]
             load_over_total_length (bool): Load Over Total Length
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
         # Client model | Member Load
         clientObject = model.clientModel.factory.create('ns0:member_set_load')
@@ -1784,15 +1735,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = load_distribution.name
 
         # Member Load Direction
         clientObject.load_direction = load_direction.name
 
-        #Load Magnitude
+        # Load Magnitude
         if load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_UNIFORM:
             if len(load_parameter) != 1:
                 raise ValueError("WARNING: Load parameter array length should be 1 for LOAD_DISTRIBUTION_UNIFORM. Kindly check list inputs completeness and correctness.")
             clientObject.magnitude = load_parameter[0]
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_1:
             if len(load_parameter) != 3:
@@ -1862,26 +1813,21 @@
                 clientObject.distance_b_relative = load_parameter[5]
             else:
                 clientObject.distance_b_absolute = load_parameter[5]
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_CONCENTRATED_VARYING:
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                if len(load_parameter[i]) != 3:
+                if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
-                mlvlp.row.delta_distance = load_parameter[i][1]
-                mlvlp.row.magnitude = load_parameter[i][2]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
+                mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_TRAPEZOIDAL:
             if len(load_parameter) != 6:
                 raise ValueError("WARNING: Load parameter array length should be 6 for LOAD_DISTRIBUTION_TRAPEZOIDAL. Kindly check list inputs completeness and correctness.")
             clientObject.magnitude_1 = load_parameter[0]
@@ -1933,26 +1879,21 @@
             clientObject.magnitude_1 = load_parameter[0]
             clientObject.magnitude_2 = load_parameter[1]
             clientObject.magnitude_3 = load_parameter[2]
 
         elif load_distribution == MemberSetLoadDistribution.LOAD_DISTRIBUTION_VARYING:
             clientObject.varying_load_parameters = model.clientModel.factory.create('ns0:member_set_load.varying_load_parameters')
             for i,j in enumerate(load_parameter):
-                if len(load_parameter[i]) != 3:
+                if len(load_parameter[i]) != 2:
                         raise ValueError("WARNING: MemberLoad no: %x, load case: %x - Wrong data input." % (no, load_case_no))
                 mlvlp = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters_row')
                 mlvlp.no = i+1
+                mlvlp.row = model.clientModel.factory.create('ns0:member_set_load_varying_load_parameters')
                 mlvlp.row.distance = load_parameter[i][0]
-                mlvlp.row.delta_distance = load_parameter[i][1]
-                mlvlp.row.magnitude = load_parameter[i][2]
-                mlvlp.row.note = None
-                mlvlp.row.magnitude_t_c = 0.0
-                mlvlp.row.magnitude_delta_t = 0.0
-                mlvlp.row.magnitude_t_t = 0.0
-                mlvlp.row.magnitude_t_b = 0.0
+                mlvlp.row.magnitude = load_parameter[i][1]
 
                 clientObject.varying_load_parameters.member_set_load_varying_load_parameters.append(mlvlp)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
@@ -2008,18 +1949,18 @@
 
         # Member Load Distribution
         clientObject.load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_UNIFORM.name
 
         # Member Load Direction
         clientObject.load_direction = MemberSetLoadDirection.LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W_TRUE.name
 
-        #Member Load Orientation
+        # Member Load Orientation
         clientObject.load_direction_orientation = load_direction_orientation.name
 
-        #Load Magnitude
+        # Load Magnitude
         clientObject.magnitude = specific_weight
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -2076,21 +2017,21 @@
 
         # Member Load Distribution
         clientObject.load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_UNIFORM.name
 
         # Member Load Direction
         clientObject.load_direction = MemberSetLoadDirection.LOAD_DIRECTION_GLOBAL_Z_OR_USER_DEFINED_W_TRUE.name
 
-        #Member Load Orientation
+        # Member Load Orientation
         clientObject.load_direction_orientation = load_direction_orientation.name
 
-        #Load Magnitude
+        # Load Magnitude
         clientObject.magnitude = specific_weight
 
-        #Filling Height
+        # Filling Height
         clientObject.filling_height = filling_height
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -2143,15 +2084,15 @@
 
         # Member Load Distribution
         clientObject.load_distribution = MemberSetLoadDistribution.LOAD_DISTRIBUTION_UNIFORM.name
 
         # Member Load Direction
         clientObject.load_direction = MemberSetLoadDirection.LOAD_DIRECTION_LOCAL_X.name
 
-        #Load Magnitude
+        # Load Magnitude
         clientObject.magnitude = pressure
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -2210,24 +2151,24 @@
         # Members No. (e.g. '5 6 7 12')
         clientObject.member_sets = ConvertToDlString(member_sets)
 
         # Member Load Type
         load_type = MemberSetLoadType.LOAD_TYPE_ROTARY_MOTION
         clientObject.load_type = load_type.name
 
-        #Angular Acceleration
+        # Angular Acceleration
         clientObject.angular_acceleration = angular_acceleration
 
-        #Angular Velocity
+        # Angular Velocity
         clientObject.angular_velocity = angular_velocity
 
-        #Axis Definition Type
+        # Axis Definition Type
         clientObject.axis_definition_type = axis_definition_type.name
 
-        #Axis definition
+        # Axis definition
         if clientObject.axis_definition_type == "AXIS_DEFINITION_TWO_POINTS":
             clientObject.axis_definition_p1_x = axis_definition_p1[0]
             clientObject.axis_definition_p1_y = axis_definition_p1[1]
             clientObject.axis_definition_p1_z = axis_definition_p1[2]
 
             clientObject.axis_definition_p2_x = axis_definition_p2[0]
             clientObject.axis_definition_p2_y = axis_definition_p2[1]
```

### Comparing `RSTAB-1.5.0/RSTAB/Loads/nodalLoad.py` & `RSTAB-1.6.0/RSTAB/Loads/nodalLoad.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,16 +89,14 @@
             params (dict, optional):
                 For specific_direction type DIRECTION_TYPE_ROTATED_VIA_3_ANGLES;
                     params={'specific_direction' : [NodalLoadSpecificDirectionType.DIRECTION_TYPE_ROTATED_VIA_3_ANGLES, NodalLoadAxesSequence, angle_1, angle_2, angle_3, angle_x, angle_y, angle_z]}
                 For specific_direction type DIRECTION_TYPE_DIRECTED_TO_NODE;
                     params={'specific_direction' : [NodalLoadSpecificDirectionType.DIRECTION_TYPE_DIRECTED_TO_NODE, nodes_no]}
                 For specific_direction type DIRECTION_TYPE_PARALLEL_TO_TWO_NODES;
                     params={'specific_direction' : [NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_TWO_NODES, nodes_no]}
-                For specific_direction type DIRECTION_TYPE_PARALLEL_TO_CS_OF_LINE;
-                    params={'specific_direction' : [NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_CS_OF_LINE, line_no]}
                 For specific_direction type DIRECTION_TYPE_PARALLEL_TO_CS_OF_MEMBER;
                     params={'specific_direction' : [NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_CS_OF_MEMBER, member_no]}
                 For force_eccentricity;
                     params={'force_eccentricity' : [ex, ey, ez]}
                 For shifted_display;
                     params={'shifted_display' : [offset_x, offset_y, offset_y, distance]}
             model (RSTAB Class, optional): Model to be edited
@@ -121,18 +119,18 @@
         # Force Direction
         clientObject.load_direction = load_direction.name
 
         # Load Type
         load_type = NodalLoadType.LOAD_TYPE_FORCE
         clientObject.load_type = load_type.name
 
-        ## Force Magnitude
+        # Force Magnitude
         clientObject.force_magnitude = magnitude
 
-        #Option Check
+        # Option Check
         if force_eccentricity and shifted_display:
             raise ValueError("Only one of force_eccentiricity and shifted_display could be TRUE")
 
         # Specific Direction
         if specific_direction:
 
             if 'specific_direction' not in list(params.keys()):
@@ -155,35 +153,32 @@
             elif params_s[0] == NodalLoadSpecificDirectionType.DIRECTION_TYPE_DIRECTED_TO_NODE:
                 clientObject.directed_to_node_direction_node = params_s[1]
 
             elif params_s[0] == NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_TWO_NODES:
                 clientObject.parallel_to_two_nodes_first_node = params_s[1]
                 clientObject.parallel_to_two_nodes_second_node = params_s[2]
 
-            elif params_s[0] == NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_CS_OF_LINE:
-                clientObject.parallel_to_line = params_s[1]
-
             elif params_s[0] == NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_CS_OF_MEMBER:
                 clientObject.parallel_to_member = params_s[1]
 
-        #Force Eccentiricity
+        # Force Eccentiricity
         if force_eccentricity:
 
             if 'force_eccentricity' not in list(params.keys()):
                 raise ValueError("Required key is missing")
 
             params_e = params['force_eccentricity']
 
             clientObject.has_force_eccentricity = True
 
             clientObject.force_eccentricity_x = params_e[0]
             clientObject.force_eccentricity_y = params_e[1]
             clientObject.force_eccentricity_z = params_e[2]
 
-        #Shifted Display
+        # Shifted Display
         if shifted_display:
 
             if 'shifted_display' not in list(params.keys()):
                 raise ValueError("Required key is missing")
 
             params_d = params['shifted_display']
 
@@ -235,16 +230,14 @@
             params (dict, optional):
                 For specific_direction type DIRECTION_TYPE_ROTATED_VIA_3_ANGLES;
                     params={'specific_direction' : [NodalLoadSpecificDirectionType.DIRECTION_TYPE_ROTATED_VIA_3_ANGLES, NodalLoadAxesSequence, angle_1, angle_2, angle_3, angle_x, angle_y, angle_z]}
                 For specific_direction type DIRECTION_TYPE_DIRECTED_TO_NODE;
                     params={'specific_direction' : [NodalLoadSpecificDirectionType.DIRECTION_TYPE_DIRECTED_TO_NODE, nodes_no]}
                 For specific_direction type DIRECTION_TYPE_PARALLEL_TO_TWO_NODES;
                     params={'specific_direction' : [NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_TWO_NODES, nodes_no]}
-                For specific_direction type DIRECTION_TYPE_PARALLEL_TO_CS_OF_LINE;
-                    params={'specific_direction' : [NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_CS_OF_LINE, line_no]}
                 For specific_direction type DIRECTION_TYPE_PARALLEL_TO_CS_OF_MEMBER;
                     params={'specific_direction' : [NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_CS_OF_MEMBER, member_no]}
                 For shifted_display;
                     params={'shifted_display' : [offset_x, offset_y, offset_y, distance]}
             model (RSTAB Class, optional): Model to be edited
         """
         # Client model | Nodal Force
@@ -265,15 +258,15 @@
         # Force Direction
         clientObject.load_direction = load_direction.name
 
         # Load Type
         load_type = NodalLoadType.LOAD_TYPE_MOMENT
         clientObject.load_type = load_type.name
 
-        ## Force Magnitude
+        # Force Magnitude
         clientObject.moment_magnitude = moment_magnitude
 
         # Specific Direction
         if specific_direction:
 
             if 'specific_direction' not in list(params.keys()):
                 raise ValueError("Required key is missing")
@@ -295,21 +288,18 @@
             elif params_s[0] == NodalLoadSpecificDirectionType.DIRECTION_TYPE_DIRECTED_TO_NODE:
                 clientObject.directed_to_node_direction_node = params_s[1]
 
             elif params_s[0] == NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_TWO_NODES:
                 clientObject.parallel_to_two_nodes_first_node = params_s[1]
                 clientObject.parallel_to_two_nodes_second_node = params_s[2]
 
-            elif params_s[0] == NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_CS_OF_LINE:
-                clientObject.parallel_to_line = params_s[1]
-
             elif params_s[0] == NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_CS_OF_MEMBER:
                 clientObject.parallel_to_member = params_s[1]
 
-        #Shifted Display
+        # Shifted Display
         if shifted_display:
 
             if 'shifted_display' not in list(params.keys()):
                 raise ValueError("Required key is missing")
 
             params_d = params['shifted_display']
 
@@ -357,16 +347,14 @@
             specific_direction (bool): Enable/Disable Specific Direction Option
             force_eccentricity(bool): Enable/Disable Force Direction Option
             shifted_display(bool): Enable/Disable Shifted Display Option
             comment (str, optional): Comments
             params (dict, optional):
                 For specific_direction type DIRECTION_TYPE_ROTATED_VIA_3_ANGLES;
                     params={'specific_direction' : [NodalLoadSpecificDirectionType.DIRECTION_TYPE_ROTATED_VIA_3_ANGLES, NodalLoadAxesSequence, angle_1, angle_2, angle_3, angle_x, angle_y, angle_z]}
-                For specific_direction type DIRECTION_TYPE_PARALLEL_TO_CS_OF_LINE;
-                    params={'specific_direction' : [NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_CS_OF_LINE, line_no]}
                 For specific_direction type DIRECTION_TYPE_PARALLEL_TO_CS_OF_MEMBER;
                     params={'specific_direction' : [NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_CS_OF_MEMBER, member_no]}
                 For force_eccentricity;
                     params={'force_eccentricity' : [ex, ey, ez]}
 
                 For shifted_display;
                     params={'shifted_display' : [offset_x, offset_y, offset_y, distance]}
@@ -387,27 +375,27 @@
         # Nodes No. (e.g. '5 6 7 12')
         clientObject.nodes = ConvertToDlString(nodes_no)
 
         # Load Type
         load_type = NodalLoadType.LOAD_TYPE_COMPONENTS
         clientObject.load_type = load_type.name
 
-        #Load Magnitudes
+        # Load Magnitudes
         if len(components) == 6:
             clientObject.components_force_x = components[0]
             clientObject.components_force_y = components[1]
             clientObject.components_force_z = components[2]
 
             clientObject.components_moment_x = components[3]
             clientObject.components_moment_y = components[4]
             clientObject.components_moment_z = components[5]
         else:
             raise ValueError("WARNING: The components must contain 6 elements. Kindly check list inputs for completeness and correctness.")
 
-        #Option Check
+        # Option Check
         if force_eccentricity and shifted_display:
             raise ValueError("WARNING: Only one of force_eccentiricity and shifted_display could be TRUE")
 
         # Specific Direction
         if specific_direction:
 
             if 'specific_direction' not in list(params.keys()):
@@ -423,35 +411,32 @@
                 clientObject.rotated_about_angle_1 = params_s[2]
                 clientObject.rotated_about_angle_2 = params_s[3]
                 clientObject.rotated_about_angle_3 = params_s[4]
                 clientObject.rotated_about_angle_x = params_s[5]
                 clientObject.rotated_about_angle_y = params_s[6]
                 clientObject.rotated_about_angle_z = params_s[7]
 
-            elif params_s[0] == NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_CS_OF_LINE:
-                clientObject.parallel_to_line = params_s[1]
-
             elif params_s[0] == NodalLoadSpecificDirectionType.DIRECTION_TYPE_PARALLEL_TO_CS_OF_MEMBER:
                 clientObject.parallel_to_member = params_s[1]
 
-        #Force Eccentiricity
+        # Force Eccentiricity
         if force_eccentricity:
 
             if 'force_eccentricity' not in list(params.keys()):
                 raise ValueError("Required key is missing")
 
             params_e = params['force_eccentricity']
 
             clientObject.has_force_eccentricity = force_eccentricity
 
             clientObject.force_eccentricity_x = params_e[0]
             clientObject.force_eccentricity_y = params_e[1]
             clientObject.force_eccentricity_z = params_e[2]
 
-        #Shifted Display
+        # Shifted Display
         if shifted_display:
 
             if 'shifted_display' not in list(params.keys()):
                 raise ValueError("Required key is missing")
 
             params_d = params['shifted_display']
```

### Comparing `RSTAB-1.5.0/RSTAB/Reports/favicon32.png` & `RSTAB-1.6.0/RSTAB/Reports/favicon32.png`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/Reports/html.py` & `RSTAB-1.6.0/RSTAB/Reports/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,15 @@
                 if endBySpace == -1:
                     line = line[:beginId]+'<sup>'+line[beginId+1:endByArrow]+'</sup>'+line[endByArrow:]
                 else:
                     endId = min(endBySpace + beginId, endByArrow)
                     line = line[:beginId]+'<sup>'+line[beginId+1:endId]+'</sup>'+line[endId:]
             f.write(line+'\n')
 
-def ExportResultTablesToHtml(TargetFolderPath: str):
+def ExportResultTablesToHtml(TargetFolderPath: str, OpenBrowser: bool = True):
     '''
     This feature allows the user to create an output HTML file with the results.
     The results are in the same form as result tables in RSTAB.
     The output file is written in HTML and consists of embedded tabular data.
     It will also include dropdown menu with all tables/files.
     Result files are language dependent, so parsing based on strings is impossible.
 
@@ -276,9 +276,10 @@
     copy(os.path.join(dirname, 'htmlScript.js'), TargetFolderPath)
     copy(os.path.join(dirname, 'favicon32.png'), TargetFolderPath)
 
     with open(os.path.join(TargetFolderPath,'index.html'), "w", encoding="utf-8") as f:
         for line in indexOutput:
             f.write(line+'\n')
 
-    # Open result html page
-    os.system(f"start {os.path.join(TargetFolderPath, 'index.html')}")
+    if OpenBrowser:
+        # Open result html page
+        os.system(f"start {os.path.join(TargetFolderPath, 'index.html')}")
```

### Comparing `RSTAB-1.5.0/RSTAB/Reports/htmlScript.js` & `RSTAB-1.6.0/RSTAB/Reports/htmlScript.js`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/Reports/htmlStyles.css` & `RSTAB-1.6.0/RSTAB/Reports/htmlStyles.css`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/Reports/partsList.py` & `RSTAB-1.6.0/RSTAB/Reports/partsList.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/Reports/printoutReport.py` & `RSTAB-1.6.0/RSTAB/Reports/printoutReport.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/Results/designOverview.py` & `RSTAB-1.6.0/RSTAB/Results/designOverview.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/Results/resultTables.py` & `RSTAB-1.6.0/RSTAB/Results/resultTables.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/SpecialObjects/structureModification.py` & `RSTAB-1.6.0/RSTAB/SpecialObjects/structureModification.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,58 @@
 from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes
 
 class StructureModification():
     material_item = {'no': 1, 'material_name': 1, 'modification_type': 'DIVISION_FACTOR', 'E_and_G': 1.5, 'comment': 'comment'}
     section_item = {'no': 1, 'section_name': 'IPN 300', 'A': 1.0, 'A_y':1.0, 'A_z': 1.0, 'J': 1.0, 'I_y': 1.0, 'I_z': 1.0}
     member_item = {'no': 2, 'member_modification': 1, 'members':'11', 'comment': ''}
-    surface_item = {'no': 1, 'surface_modification': 1, 'surfaces':'2', 'comment': ''}
     member_hinge_item = {'no': 1, 'member_side': 'Start', 'C_u_x': 1, 'C_u_y': 0, 'C_u_z': 0, 'C_phi_x': 0, 'C_phi_y': 0, 'C_phi_z': 0}
-    line_hinge_item = {'no': 1, 'C_u_x': 1, 'C_u_y': 0, 'C_u_z': 0, 'C_phi_x': 0, 'C_phi_y': 0, 'C_phi_z': 0}
     nodal_support_item = {'C_u_X': 1, 'C_u_Y': 0, 'C_u_Z': 0, 'C_phi_X': 0, 'C_phi_Y': 0, 'C_phi_Z': 0}
-    line_support_item = {'C_u_X': 1, 'C_u_Y': 0, 'C_u_Z': 0, 'C_phi_X': 0, 'C_phi_Y': 0, 'C_phi_Z': 0}
     member_support_item = {'C_u_x': 1, 'C_u_y': 0, 'C_u_z': 0, 'C_s_x': 0, 'C_s_y': 0, 'C_s_z': 0, 'C_phi_x': 0}
-    surface_support_item = {'C_u_X': 1, 'C_u_Y': 0, 'C_u_Z': 0, 'C_v_xz': 0, 'C_v_yz': 0}
     modify_stiffness = {'modify_stiffnesses_gamma_m': False,
                         'modify_stiffnesses_materials': False,
                         'modify_stiffnesses_sections': False,
                         'modify_stiffnesses_members': False,
-                        'modify_stiffnesses_surfaces': False,
                         'modify_stiffnesses_member_hinges': False,
-                        'modify_stiffnesses_line_hinges': False,
                         'modify_stiffnesses_nodal_supports': False,
-                        'modify_stiffnesses_line_supports': False,
                         'modify_stiffnesses_member_supports': False,
-                        'modify_stiffnesses_surface_supports': False,
-                        'modify_stiffness_member_reinforcement': False,
-                        'modify_stiffness_surface_reinforcement': False,
                         'modify_stiffness_timber_members_due_moisture_class': False,
                         'nonlinearities_disabled_material_nonlinearity_models': False,
                         'nonlinearities_disabled_material_temperature_nonlinearities': False,
-                        'nonlinearities_disabled_line_hinges': False,
                         'nonlinearities_disabled_member_types': False,
                         'nonlinearities_disabled_member_nonlinearities': False,
-                        'nonlinearities_disabled_solid_types_contact_or_surfaces_contact': False,
                         'nonlinearities_disabled_member_hinges': False,
                         'nonlinearities_disabled_nodal_supports': False,
-                        'nonlinearities_disabled_line_supports': False,
                         'nonlinearities_disabled_member_supports': False,
-                        'nonlinearities_disabled_surface_supports': False,
                         'deactivate_members_enabled': False}
 
     def __init__(self,
                  no: int = 1,
                  modify_stiffnesses: dict = modify_stiffness,
                  modify_stiffnesses_materials_list: list = None,
                  modify_stiffnesses_sections_list: list = None,
                  modify_stiffnesses_members_list: list = None,
-                 modify_stiffnesses_surfaces_list: list = None,
                  modify_stiffnesses_member_hinges_list: list = None,
-                 modify_stiffnesses_line_hinges_list: list = None,
                  modify_stiffnesses_nodal_supports_list: list = None,
-                 modify_stiffnesses_line_supports_list: list = None,
                  modify_stiffnesses_member_supports_list: list = None,
-                 modify_stiffnesses_surface_supports_list: list = None,
                  comment: str = '',
                  params: dict = None,
                  model = Model):
         """
         Structural Modification
         Modify only objects allready existing and used/assigned in the model.
 
         Args:
             no (int, optional): Structure Modification Tag
             modify_stiffnesses (dict, optional): Modify Stiffnesses
             modify_stiffnesses_materials_list (list, optional): Modify Stiffnesses Materials List
             modify_stiffnesses_sections_list (list, optional): Modify Stiffnesses Sections List
             modify_stiffnesses_members_list (list, optional): Modify Stiffnesses Members List
-            modify_stiffnesses_surfaces_list (list, optional): Modify Stiffnesses Surfaces List
             modify_stiffnesses_member_hinges_list (list, optional): Modify Stiffnesses Member Hinges List
-            modify_stiffnesses_line_hinges_list (list, optional): Modify Stiffnesses Line Hinges List
             modify_stiffnesses_nodal_supports_list (list, optional): Modify Stiffnesses Nodal Supports List
-            modify_stiffnesses_line_supports_list (list, optional): Modify Stiffnesses Line Support List
             modify_stiffnesses_member_supports_list (list, optional): Modify Stiffnesses Member Suppoorts List
-            modify_stiffnesses_surface_supports_list (list, optional): Modify Stiffnesses Surface Supports List
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
         # Client model | Structure Modification
         clientObject = None
@@ -90,35 +68,25 @@
             clientObject.no = no
 
             # Modify Stiffneesses
             clientObject.modify_stiffnesses_gamma_m = modify_stiffnesses['modify_stiffnesses_gamma_m']
             clientObject.modify_stiffnesses_materials = modify_stiffnesses['modify_stiffnesses_materials']
             clientObject.modify_stiffnesses_sections = modify_stiffnesses['modify_stiffnesses_sections']
             clientObject.modify_stiffnesses_members = modify_stiffnesses['modify_stiffnesses_members']
-            clientObject.modify_stiffnesses_surfaces = modify_stiffnesses['modify_stiffnesses_surfaces']
             clientObject.modify_stiffnesses_member_hinges = modify_stiffnesses['modify_stiffnesses_member_hinges']
-            clientObject.modify_stiffnesses_line_hinges = modify_stiffnesses['modify_stiffnesses_line_hinges']
             clientObject.modify_stiffnesses_nodal_supports = modify_stiffnesses['modify_stiffnesses_nodal_supports']
-            clientObject.modify_stiffnesses_line_supports = modify_stiffnesses['modify_stiffnesses_line_supports']
             clientObject.modify_stiffnesses_member_supports = modify_stiffnesses['modify_stiffnesses_member_supports']
-            clientObject.modify_stiffnesses_surface_supports = modify_stiffnesses['modify_stiffnesses_surface_supports']
-            clientObject.modify_stiffness_member_reinforcement = modify_stiffnesses['modify_stiffness_member_reinforcement']
-            clientObject.modify_stiffness_surface_reinforcement = modify_stiffnesses['modify_stiffness_surface_reinforcement']
             clientObject.modify_stiffness_timber_members_due_moisture_class = modify_stiffnesses['modify_stiffness_timber_members_due_moisture_class']
             clientObject.nonlinearities_disabled_material_nonlinearity_models = modify_stiffnesses['nonlinearities_disabled_material_nonlinearity_models']
             clientObject.nonlinearities_disabled_material_temperature_nonlinearities = modify_stiffnesses['nonlinearities_disabled_material_temperature_nonlinearities']
-            clientObject.nonlinearities_disabled_line_hinges = modify_stiffnesses['nonlinearities_disabled_line_hinges']
             clientObject.nonlinearities_disabled_member_types = modify_stiffnesses['nonlinearities_disabled_member_types']
             clientObject.nonlinearities_disabled_member_nonlinearities = modify_stiffnesses['nonlinearities_disabled_member_nonlinearities']
-            clientObject.nonlinearities_disabled_solid_types_contact_or_surfaces_contact = modify_stiffnesses['nonlinearities_disabled_solid_types_contact_or_surfaces_contact']
             clientObject.nonlinearities_disabled_member_hinges = modify_stiffnesses['nonlinearities_disabled_member_hinges']
             clientObject.nonlinearities_disabled_nodal_supports = modify_stiffnesses['nonlinearities_disabled_nodal_supports']
-            clientObject.nonlinearities_disabled_line_supports = modify_stiffnesses['nonlinearities_disabled_line_supports']
             clientObject.nonlinearities_disabled_member_supports = modify_stiffnesses['nonlinearities_disabled_member_supports']
-            clientObject.nonlinearities_disabled_surface_supports = modify_stiffnesses['nonlinearities_disabled_surface_supports']
             clientObject.deactivate_members_enabled = modify_stiffnesses['deactivate_members_enabled']
 
             model.clientModel.service.set_structure_modification(clientObject)
             clientObject = model.clientModel.service.get_structure_modification(no)
 
         # Modify Stiffneesses Tables
         if modify_stiffnesses['modify_stiffnesses_materials']:
@@ -138,75 +106,43 @@
                 clientObject.modify_stiffnesses_sections_table[0][idx].row.I_z = i['I_z']
         if modify_stiffnesses['modify_stiffnesses_members']:
             for i in modify_stiffnesses_members_list:
                 idx = i['no']-1
                 clientObject.modify_stiffnesses_members_table[0][idx].row.member_modification = i['member_modification']
                 clientObject.modify_stiffnesses_members_table[0][idx].row.members = i['members']
                 clientObject.modify_stiffnesses_members_table[0][idx].row.comment = i['comment']
-        if modify_stiffnesses['modify_stiffnesses_surfaces']:
-            for i in modify_stiffnesses_surfaces_list:
-                idx = i['no']-1
-                clientObject.modify_stiffnesses_surfaces_table[0][idx].row.surface_modification = i['surface_modification']
-                clientObject.modify_stiffnesses_surfaces_table[0][idx].row.surfaces = i['surfaces']
-                clientObject.modify_stiffnesses_surfaces_table[0][idx].row.comment = i['comment']
         if modify_stiffnesses['modify_stiffnesses_member_hinges']:
             for i in modify_stiffnesses_member_hinges_list:
                 idx = i['no']-1
                 clientObject.modify_stiffnesses_member_hinges_table[0][idx].row.member_side = i['member_side']
                 clientObject.modify_stiffnesses_member_hinges_table[0][idx].row.C_u_x = i['C_u_x']
                 clientObject.modify_stiffnesses_member_hinges_table[0][idx].row.C_u_y = i['C_u_y']
                 clientObject.modify_stiffnesses_member_hinges_table[0][idx].row.C_u_z = i['C_u_z']
                 clientObject.modify_stiffnesses_member_hinges_table[0][idx].row.C_phi_x = i['C_phi_x']
                 clientObject.modify_stiffnesses_member_hinges_table[0][idx].row.C_phi_y = i['C_phi_y']
                 clientObject.modify_stiffnesses_member_hinges_table[0][idx].row.C_phi_z = i['C_phi_z']
-        if modify_stiffnesses['modify_stiffnesses_line_hinges']:
-            for i in modify_stiffnesses_line_hinges_list:
-                idx = i['no']-1
-                clientObject.modify_stiffnesses_line_hinges_table[0][idx].row.C_u_x = i['C_u_x']
-                clientObject.modify_stiffnesses_line_hinges_table[0][idx].row.C_u_y = i['C_u_y']
-                clientObject.modify_stiffnesses_line_hinges_table[0][idx].row.C_u_z = i['C_u_z']
-                clientObject.modify_stiffnesses_line_hinges_table[0][idx].row.C_phi_x = i['C_phi_x']
-                clientObject.modify_stiffnesses_line_hinges_table[0][idx].row.C_phi_y = i['C_phi_y']
-                clientObject.modify_stiffnesses_line_hinges_table[0][idx].row.C_phi_z = i['C_phi_z']
         if modify_stiffnesses['modify_stiffnesses_nodal_supports']:
             for i in modify_stiffnesses_nodal_supports_list:
                 idx = i['no']-1
                 clientObject.modify_stiffnesses_nodal_supports_table[0][idx].row.C_u_x = i['C_u_x']
                 clientObject.modify_stiffnesses_nodal_supports_table[0][idx].row.C_u_y = i['C_u_y']
                 clientObject.modify_stiffnesses_nodal_supports_table[0][idx].row.C_u_z = i['C_u_z']
                 clientObject.modify_stiffnesses_nodal_supports_table[0][idx].row.C_phi_x = i['C_phi_x']
                 clientObject.modify_stiffnesses_nodal_supports_table[0][idx].row.C_phi_y = i['C_phi_y']
                 clientObject.modify_stiffnesses_nodal_supports_table[0][idx].row.C_phi_z = i['C_phi_z']
-        if modify_stiffnesses['modify_stiffnesses_line_supports']:
-            for i in modify_stiffnesses_line_supports_list:
-                idx = i['no']-1
-                clientObject.modify_stiffnesses_line_supports_table[0][idx].row.C_u_X = i['C_u_X']
-                clientObject.modify_stiffnesses_line_supports_table[0][idx].row.C_u_Y = i['C_u_Y']
-                clientObject.modify_stiffnesses_line_supports_table[0][idx].row.C_u_Z = i['C_u_Z']
-                clientObject.modify_stiffnesses_line_supports_table[0][idx].row.C_phi_X = i['C_phi_X']
-                clientObject.modify_stiffnesses_line_supports_table[0][idx].row.C_phi_Y = i['C_phi_Y']
-                clientObject.modify_stiffnesses_line_supports_table[0][idx].row.C_phi_Z = i['C_phi_Z']
         if modify_stiffnesses['modify_stiffnesses_member_supports']:
             for i in modify_stiffnesses_member_supports_list:
                 idx = i['no']-1
                 clientObject.modify_stiffnesses_member_supports_table[0][idx].row.C_u_x = i['C_u_x']
                 clientObject.modify_stiffnesses_member_supports_table[0][idx].row.C_u_y = i['C_u_y']
                 clientObject.modify_stiffnesses_member_supports_table[0][idx].row.C_u_z = i['C_u_z']
                 clientObject.modify_stiffnesses_member_supports_table[0][idx].row.C_s_x = i['C_s_x']
                 clientObject.modify_stiffnesses_member_supports_table[0][idx].row.C_s_y = i['C_s_y']
                 clientObject.modify_stiffnesses_member_supports_table[0][idx].row.C_s_z = i['C_s_z']
                 clientObject.modify_stiffnesses_member_supports_table[0][idx].row.C_phi_x = i['C_phi_x']
-        if modify_stiffnesses['modify_stiffnesses_surface_supports']:
-            for i in modify_stiffnesses_surface_supports_list:
-                idx = i['no']-1
-                clientObject.modify_stiffnesses_surface_supports_table[0][idx].row.C_u_X = i['C_u_X']
-                clientObject.modify_stiffnesses_surface_supports_table[0][idx].row.C_u_Y = i['C_u_Y']
-                clientObject.modify_stiffnesses_surface_supports_table[0][idx].row.C_u_Z = i['C_u_Z']
-                clientObject.modify_stiffnesses_surface_supports_table[0][idx].row.C_v_xz = i['C_v_xz']
-                clientObject.modify_stiffnesses_surface_supports_table[0][idx].row.C_v_yz = i['C_v_yz']
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
```

### Comparing `RSTAB-1.5.0/RSTAB/SteelDesign/steelUltimateConfigurations.py` & `RSTAB-1.6.0/RSTAB/SteelDesign/steelUltimateConfigurations.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                  member_sets_no: str = 'All',
                  comment: str = '',
                  params: dict = None,
                  model = Model):
         """
         Args:
             no (int): Steel Design Ultimate Configuration Tag
-            user_defined_name (list): User Defined Name Configuration Name
+            name (str): User Defined Configuration Name
             members_no (str): Assign Configuration to Selected Members
             member_sets_no (str): Assign Configuration to Selected Member Sets
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
@@ -39,15 +39,15 @@
         if members_no == 'All':
             clientObject.assigned_to_all_members = True
 
         else:
             clientObject.assigned_to_all_members = False
             clientObject.assigned_to_members = ConvertToDlString(members_no)
 
-        #Assigned Member Sets
+        # Assigned Member Sets
         if member_sets_no == 'All':
             clientObject.assigned_to_all_member_sets = True
 
         else:
             clientObject.assigned_to_all_member_sets = False
             clientObject.assigned_to_member_sets = ConvertToDlString(member_sets_no)
```

### Comparing `RSTAB-1.5.0/RSTAB/TimberDesign/timberServiceLimitStateConfigurations.py` & `RSTAB-1.6.0/RSTAB/TimberDesign/timberServiceLimitStateConfigurations.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                  member_sets_no: str = 'All',
                  comment: str = '',
                  params: dict = None,
                  model = Model):
         """
         Args:
             no (int): Timber Design Service Limit State Configuration Tag
-            user_defined_name (list): User Defined Name Configuration Name
+            name (str): User Defined Configuration Name
             members_no (str): Assign Configuration to Selected Members
             member_sets_no (str): Assign Configuration to Selected Member Sets
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
@@ -39,15 +39,15 @@
         if members_no == 'All':
             clientObject.assigned_to_all_members = True
 
         else:
             clientObject.assigned_to_all_members = False
             clientObject.assigned_to_members = ConvertToDlString(members_no)
 
-        #Assigned Member Sets
+        # Assigned Member Sets
         if member_sets_no == 'All':
             clientObject.assigned_to_all_member_sets = True
 
         else:
             clientObject.assigned_to_all_member_sets = False
             clientObject.assigned_to_member_sets = ConvertToDlString(member_sets_no)
```

### Comparing `RSTAB-1.5.0/RSTAB/TimberDesign/timberUltimateConfigurations.py` & `RSTAB-1.6.0/RSTAB/TimberDesign/timberUltimateConfigurations.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                  member_sets_no: str = 'All',
                  comment: str = '',
                  params: dict = None,
                  model = Model):
         """
         Args:
             no (int): Timber Design Ultimate Configuration Tag
-            user_defined_name (list): User Defined Name Configuration Name
+            name (str): User Defined Configuration Name
             members_no (str): Assign Configuration to Selected Members
             member_sets_no (str): Assign Configuration to Selected Member Sets
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
@@ -39,15 +39,15 @@
         if members_no == 'All':
             clientObject.assigned_to_all_members = True
 
         else:
             clientObject.assigned_to_all_members = False
             clientObject.assigned_to_members = ConvertToDlString(members_no)
 
-        #Assigned Member Sets
+        # Assigned Member Sets
         if member_sets_no == 'All':
             clientObject.assigned_to_all_member_sets = True
 
         else:
             clientObject.assigned_to_all_member_sets = False
             clientObject.assigned_to_member_sets = ConvertToDlString(member_sets_no)
```

### Comparing `RSTAB-1.5.0/RSTAB/Tools/GetObjectNumbersByType.py` & `RSTAB-1.6.0/RSTAB/Tools/GetObjectNumbersByType.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/Tools/ModelCheck.py` & `RSTAB-1.6.0/RSTAB/Tools/ModelCheck.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/Tools/PlausibilityCheck.py` & `RSTAB-1.6.0/RSTAB/Tools/PlausibilityCheck.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/Tools/centreOfGravityAndObjectInfo.py` & `RSTAB-1.6.0/RSTAB/Tools/centreOfGravityAndObjectInfo.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/Tools/sectionDialogue.py` & `RSTAB-1.6.0/RSTAB/Tools/sectionDialogue.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/TypesForAluminumDesign/aluminumEffectiveLengths.py` & `RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/aluminumEffectiveLengths.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from RSTAB.initModel import Model, clearAttributes, ConvertToDlString, deleteEmptyAttributes
+from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
 from RSTAB.enums import AluminumEffectiveLengthsDeterminationMcrEurope
 
 class AluminumEffectiveLengths():
     def __init__(self,
                  no: int = 1,
                  members: str = '1',
                  member_sets: str = '',
```

### Comparing `RSTAB-1.5.0/RSTAB/TypesForAluminumDesign/aluminumMemberLocalSectionReduction.py` & `RSTAB-1.6.0/RSTAB/TypesForAluminumDesign/aluminumMemberLocalSectionReduction.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,36 +45,36 @@
 
         # Client Model | Types For Aluminum Member Local Section Reduction
         clientObject = model.clientModel.factory.create('ns0:aluminum_member_local_section_reduction')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
-        #Local Section Reduction No.
+        # Local Section Reduction No.
         clientObject.no = no
 
-        #Local Section Reduction Assigned Members
+        # Local Section Reduction Assigned Members
         clientObject.members = ConvertToDlString(members)
 
-        #Local Section Reduction Assigned Member Sets
+        # Local Section Reduction Assigned Member Sets
         clientObject.member_sets = ConvertToDlString(member_sets)
 
-        #Local Section Reduction User defined Name
+        # Local Section Reduction User defined Name
         if name:
             clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
-        #Local Section Reduction Components
+        # Local Section Reduction Components
         clientObject.components = model.clientModel.factory.create('ns0:array_of_aluminum_member_local_section_reduction_components')
 
         for i,j in enumerate(components):
             smlsr = model.clientModel.factory.create('ns0:aluminum_member_local_section_reduction_components_row')
-            clearAttributes(smlsr.row)
-
             smlsr.no = i+1
+            smlsr.row = model.clientModel.factory.create('ns0:aluminum_member_local_section_reduction_components')
+            clearAttributes(smlsr.row)
             smlsr.row.reduction_type = components[i][0].name
             smlsr.row.position = components[i][1]
             smlsr.row.multiple = components[i][2]
             smlsr.row.fastener_definition_type = components[i][3].name
             if smlsr.row.fastener_definition_type == "DEFINITION_TYPE_ABSOLUTE":
                 smlsr.row.reduction_area = components[i][4]
             elif smlsr.row.fastener_definition_type == "DEFINITION_TYPE_RELATIVE":
```

### Comparing `RSTAB-1.5.0/RSTAB/TypesForMembers/memberDefinableStiffness.py` & `RSTAB-1.6.0/RSTAB/TypesForMembers/memberDefinableStiffness.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/TypesForMembers/memberEccentricity.py` & `RSTAB-1.6.0/RSTAB/TypesForMembers/memberEccentricity.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                  hinge_location_at_node: bool = False,
                  comment: str = '',
                  params: dict = None,
                  model = Model):
         """
         Args:
             no (int): Eccentricity Tag
-            name (list): User Defined Name
+            name (str): User Defined Name
             eccentricity_type (enum): Member Eccentricity Specification Type Enumeration
             eccentricity_parameters (list): Eccentricity Parameters List
                 for eccentricity_type == MemberEccentricitySpecificationType.TYPE_RELATIVE:
                     eccentricity_parameters = [horizontal_section_alignment, vertical_section_alignment]
                 for eccentricity_type == MemberEccentricitySpecificationType.TYPE_ABSOLUTE:
                     eccentricity_parameters = [coordinate_system, offset_x, offset_y, offset_z]
                 for eccentricity_type == MemberEccentricitySpecificationType.TYPE_RELATIVE_AND_ABSOLUTE:
```

### Comparing `RSTAB-1.5.0/RSTAB/TypesForMembers/memberHinge.py` & `RSTAB-1.6.0/RSTAB/TypesForMembers/memberHinge.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,15 @@
             clientObject.diagram_along_x_end = translational_release_n_nonlinearity[1][1].name
 
             clientObject.diagram_along_x_table = Model.clientModel.factory.create('ns0:member_hinge.diagram_along_x_table')
 
             for i,j in enumerate(translational_release_n_nonlinearity[1][2]):
                 mlvlp = Model.clientModel.factory.create('ns0:member_hinge_diagram_along_x_table_row')
                 mlvlp.no = i+1
+                mlvlp.row = Model.clientModel.factory.create('ns0:member_hinge_diagram_along_x_table')
                 mlvlp.row.displacement = translational_release_n_nonlinearity[1][2][i][0]
                 mlvlp.row.force = translational_release_n_nonlinearity[1][2][i][1]
                 mlvlp.row.spring = translational_release_n_nonlinearity[1][2][i][2]
 
                 clientObject.diagram_along_x_table.member_hinge_diagram_along_x_table.append(mlvlp)
 
         elif translational_release_n_nonlinearity[0].name == "NONLINEARITY_TYPE_FRICTION_DIRECTION_1" \
@@ -200,14 +201,15 @@
             clientObject.diagram_along_y_end = translational_release_vy_nonlinearity[1][1].name
 
             clientObject.diagram_along_y_table = Model.clientModel.factory.create('ns0:member_hinge.diagram_along_y_table')
 
             for i,j in enumerate(translational_release_vy_nonlinearity[1][2]):
                 mlvlp = Model.clientModel.factory.create('ns0:member_hinge_diagram_along_y_table_row')
                 mlvlp.no = i+1
+                mlvlp.row = Model.clientModel.factory.create('ns0:member_hinge_diagram_along_y_table')
                 mlvlp.row.displacement = translational_release_vy_nonlinearity[1][2][i][0]
                 mlvlp.row.force = translational_release_vy_nonlinearity[1][2][i][1]
                 mlvlp.row.spring = translational_release_vy_nonlinearity[1][2][i][2]
 
                 clientObject.diagram_along_y_table.member_hinge_diagram_along_y_table.append(mlvlp)
 
         elif translational_release_vy_nonlinearity[0].name == "NONLINEARITY_TYPE_FRICTION_DIRECTION_1" \
@@ -271,14 +273,15 @@
             clientObject.diagram_along_z_end = translational_release_vz_nonlinearity[1][1].name
 
             clientObject.diagram_along_z_table = Model.clientModel.factory.create('ns0:member_hinge.diagram_along_z_table')
 
             for i,j in enumerate(translational_release_vz_nonlinearity[1][2]):
                 mlvlp = Model.clientModel.factory.create('ns0:member_hinge_diagram_along_z_table_row')
                 mlvlp.no = i+1
+                mlvlp.row = Model.clientModel.factory.create('ns0:member_hinge_diagram_along_z_table')
                 mlvlp.row.displacement = translational_release_vz_nonlinearity[1][2][i][0]
                 mlvlp.row.force = translational_release_vz_nonlinearity[1][2][i][1]
                 mlvlp.row.spring = translational_release_vz_nonlinearity[1][2][i][2]
 
                 clientObject.diagram_along_z_table.member_hinge_diagram_along_z_table.append(mlvlp)
 
         elif translational_release_vz_nonlinearity[0].name == "NONLINEARITY_TYPE_FRICTION_DIRECTION_1" \
@@ -342,14 +345,15 @@
             clientObject.diagram_around_x_end = rotational_release_mt_nonlinearity[1][1].name
 
             clientObject.diagram_around_x_table = Model.clientModel.factory.create('ns0:member_hinge.diagram_around_x_table')
 
             for i,j in enumerate(rotational_release_mt_nonlinearity[1][2]):
                 mlvlp = Model.clientModel.factory.create('ns0:member_hinge_diagram_around_x_table_row')
                 mlvlp.no = i+1
+                mlvlp.row = Model.clientModel.factory.create('ns0:member_hinge_diagram_around_x_table')
                 mlvlp.row.rotation = rotational_release_mt_nonlinearity[1][2][i][0]
                 mlvlp.row.moment = rotational_release_mt_nonlinearity[1][2][i][1]
                 mlvlp.row.spring = rotational_release_mt_nonlinearity[1][2][i][2]
 
                 clientObject.diagram_around_x_table.member_hinge_diagram_around_x_table.append(mlvlp)
 
         # Rotational Release My Nonlinearity
@@ -402,14 +406,15 @@
             clientObject.diagram_around_y_end = rotational_release_my_nonlinearity[1][1].name
 
             clientObject.diagram_around_y_table = Model.clientModel.factory.create('ns0:member_hinge.diagram_around_y_table')
 
             for i,j in enumerate(rotational_release_my_nonlinearity[1][2]):
                 mlvlp = Model.clientModel.factory.create('ns0:member_hinge_diagram_around_y_table_row')
                 mlvlp.no = i+1
+                mlvlp.row = Model.clientModel.factory.create('ns0:member_hinge_diagram_around_y_table')
                 mlvlp.row.rotation = rotational_release_my_nonlinearity[1][2][i][0]
                 mlvlp.row.moment = rotational_release_my_nonlinearity[1][2][i][1]
                 mlvlp.row.spring = rotational_release_my_nonlinearity[1][2][i][2]
 
                 clientObject.diagram_around_y_table.member_hinge_diagram_around_y_table.append(mlvlp)
 
         # Rotational Release Mz Nonlinearity
@@ -462,14 +467,15 @@
             clientObject.diagram_around_z_end = rotational_release_mz_nonlinearity[1][1].name
 
             clientObject.diagram_around_z_table = Model.clientModel.factory.create('ns0:member_hinge.diagram_around_z_table')
 
             for i,j in enumerate(rotational_release_mz_nonlinearity[1][2]):
                 mlvlp = Model.clientModel.factory.create('ns0:member_hinge_diagram_around_z_table_row')
                 mlvlp.no = i+1
+                mlvlp.row = Model.clientModel.factory.create('ns0:member_hinge_diagram_around_z_table')
                 mlvlp.row.rotation = rotational_release_mz_nonlinearity[1][2][i][0]
                 mlvlp.row.moment = rotational_release_mz_nonlinearity[1][2][i][1]
                 mlvlp.row.spring = rotational_release_mz_nonlinearity[1][2][i][2]
 
                 clientObject.diagram_around_z_table.member_hinge_diagram_around_z_table.append(mlvlp)
 
         # Comment
```

### Comparing `RSTAB-1.5.0/RSTAB/TypesForMembers/memberNonlinearity.py` & `RSTAB-1.6.0/RSTAB/TypesForMembers/memberNonlinearity.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/TypesForMembers/memberResultIntermediatePoints.py` & `RSTAB-1.6.0/RSTAB/TypesForTimberDesign/timberServiceClass.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,59 @@
-from RSTAB.initModel import Model, clearAttributes, ConvertToDlString, deleteEmptyAttributes
+from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
+from RSTAB.enums import TimberServiceClassServiceClass
 
-class MemberResultIntermediatePoint():
+class TimberServiceClass():
     def __init__(self,
-                 no: int = 1,
-                 members: str = "",
-                 point_count: int = 2,
-                 uniform_distribution: bool = True,
-                 distances = None,
-                 comment: str = '',
-                 params: dict = None,
-                 model = Model):
+                no: int = 1,
+                name: str = '',
+                members: str = '',
+                member_sets: str = '',
+                service_class = TimberServiceClassServiceClass.TIMBER_SERVICE_CLASS_TYPE_1,
+                comment: str = '',
+                params: dict = None):
         """
         Args:
-            no (int): Member Result Intermediate Point Tag
+            no (int): Timber Service Class Tag
+            name (str): User Defined Timber Service Class Name
             members (str): Assigned Members
-            point_count (int): Assigned Point Number
-            uniform_distribution (bool): Uniform Distrubition Option
-            distances (list of lists): Distances Table
+            member_sets (str): Assigned Member Sets
+            service_class (enum): Timber Service Class Service Class
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
-            model (RSTAB Class, optional): Model to be edited
         """
 
-        # Client model | Member Result Intermediate Point
-        clientObject = model.clientModel.factory.create('ns0:member_result_intermediate_point')
+         # Client Model | Types For Timber Design Service Class
+        clientObject = Model.clientModel.factory.create('ns0:timber_service_class')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
-        # Member Result Intermediate Point No.
+        # Member Service Class
         clientObject.no = no
 
         # Assigned Members
-        clientObject.members = ConvertToDlString(members)
+        clientObject.member = ConvertToDlString(members)
 
-        # Point Count
-        clientObject.uniform_distribution = uniform_distribution
-        if uniform_distribution:
-            clientObject.point_count = point_count
-
-        else:
-            clientObject.distances = Model.clientModel.factory.create('ns0:member_result_intermediate_point.distances')
-
-            for i,j in enumerate(distances):
-                mlvlp = Model.clientModel.factory.create('ns0:member_result_intermediate_point_distances_row')
-                mlvlp.no = i+1
-                mlvlp.row.value = distances[i][0]
-                mlvlp.row.note = None
+        # Assigned Member Sets
+        clientObject.member_sets = ConvertToDlString(member_sets)
 
-                clientObject.distances.member_result_intermediate_point_distances.append(mlvlp)
+        # Service Class
+        clientObject.service_class = service_class.name
+
+        # User Defined Name
+        if name:
+            clientObject.user_defined_name_enabled = True
+            clientObject.name = name
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
-        # Add Member Result Intermediate Point to client model
-        model.clientModel.service.set_member_result_intermediate_point(clientObject)
+        # Add Service Class to client model
+        Model.clientModel.service.set_timber_service_class(clientObject)
```

### Comparing `RSTAB-1.5.0/RSTAB/TypesForMembers/memberStiffnessModification.py` & `RSTAB-1.6.0/RSTAB/TypesForMembers/memberStiffnessModification.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/TypesForMembers/memberSupport.py` & `RSTAB-1.6.0/RSTAB/TypesForMembers/memberSupport.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,28 +9,37 @@
                  spring_translation_x: float = 0.0,
                  spring_translation_y: float = 0.0,
                  spring_translation_z: list = [inf, MemberSupportNonlinearity.NONLINEARITY_NONE],
                  spring_rotation: float = 0.0,
                  spring_shear_x: float = 0.0,
                  spring_shear_y: float = 0.0,
                  spring_shear_z: float = 0.0,
+                 member_shear_panel: list = [False],
+                 member_rotational_restraint: list = [False],
                  comment: str = '',
                  params: dict = None,
                  model = Model):
         """
         Args:
             no (int): Member Support Tag
             members (str): Assigned Members
             spring_translation_x (float): Translational X Spring Constant
             spring_translation_y (float): Translational Y Spring Constant
             spring_translation_z (list): [Translational Z Spring Constant, Nonlinearity Type]
             spring_rotation (float): Rotational Spring Constant
             spring_shear_x (float): Shear X Spring Constant
             spring_shear_y (float): Shear Y Spring Constant
             spring_shear_z (float): Shear Z Spring Constant
+            member_shear_panel (list): Member Shear Panel Option
+                if member_shear_panel[0] == True:
+                    member_shear_panel[1] = Member Shear Panel Number
+            member_rotational_restraint (list): Member Rotational Restraint Option
+                if member_rotational_restraint[0] == True:
+                    member_rotational_restraint[1] = Member Rotational Restraint Number
+                    member_rotational_restraint[2] = load_introduced_from_sheeting_to_beam
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
         # Client model | Member Support
         clientObject = model.clientModel.factory.create('ns0:member_support')
@@ -52,14 +61,25 @@
         clientObject.nonlinearity = spring_translation_z[1].name
 
         # Spring Shear
         clientObject.spring_shear_x = spring_shear_x
         clientObject.spring_shear_y = spring_shear_y
         clientObject.spring_shear_z = spring_shear_z
 
+        # Member Shear Panel
+        clientObject.shear_panel_enabled = member_shear_panel[0]
+        if member_shear_panel[0]:
+            clientObject.member_shear_panel = member_shear_panel[1]
+
+        # Member Rotational Restraint
+        clientObject.rotational_restraint_enabled = member_rotational_restraint[0]
+        if member_rotational_restraint[0]:
+            clientObject.member_rotational_restraint = member_rotational_restraint[1]
+            clientObject.load_introduced_from_sheeting_to_beam = member_rotational_restraint[2]
+
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
```

### Comparing `RSTAB-1.5.0/RSTAB/TypesForMembers/memberTransverseStiffeners.py` & `RSTAB-1.6.0/RSTAB/TypesForMembers/memberTransverseStiffeners.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 
         # Member Transverse Components
         clientObject.components = Model.clientModel.factory.create('ns0:member_transverse_stiffener.components')
 
         for i in components:
             mlvlp = Model.clientModel.factory.create('ns0:member_transverse_stiffener_components_row')
             mlvlp.no = i['no']
+            mlvlp.row = Model.clientModel.factory.create('ns0:member_transverse_stiffener_components')
             mlvlp.row.stiffener_type = i['stiffener_type'].name
             mlvlp.row.position = i['position']
             mlvlp.row.position_type = i['position_type'].name
             mlvlp.row.multiple = i['multiple']
             mlvlp.row.multiple_number = i['multiple_number']
             mlvlp.row.multiple_offset_definition_type = i['multiple_offset_definition_type'].name
             mlvlp.row.multiple_offset = i['multiple_offset']
```

### Comparing `RSTAB-1.5.0/RSTAB/TypesForNodes/nodalSupport.py` & `RSTAB-1.6.0/RSTAB/TypesForNodes/nodalSupport.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/TypesForSteelDesign/SteelMemberLocalSectionReduction.py` & `RSTAB-1.6.0/RSTAB/TypesForSteelDesign/SteelMemberLocalSectionReduction.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,47 +33,48 @@
                 if components[i][2] == True
                     components[i][5] (int): Multiple Number
                     components[i][6] (enum): Multiple Offset Definition Type Enumeration
                     for components[i][6] == MultipleOffsetDefinitionType.OFFSET_DEFINITION_TYPE_ABSOLUTE;
                         components[i][7] (float): Multiple Offset Value
                     for components[i][6] == MultipleOffsetDefinitionType.OFFSET_DEFINITION_TYPE_RELATIVE;
                         components[i][7] (float): Multiple Offset Value (value must be between 0.0 and 1.0)
-            user_defined_name (str): User Defined  Member Local Section Reduction Name
+            name (str): User Defined  Member Local Section Reduction Name
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
         # Client Model | Types For Steel Member Local Section Reduction
         clientObject = model.clientModel.factory.create('ns0:steel_member_local_section_reduction')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
-        #Local Section Reduction No.
+        # Local Section Reduction No.
         clientObject.no = no
 
-        #Local Section Reduction Assigned Members
+        # Local Section Reduction Assigned Members
         clientObject.members = ConvertToDlString(members)
 
-        #Local Section Reduction Assigned Member Sets
+        # Local Section Reduction Assigned Member Sets
         clientObject.member_sets = ConvertToDlString(member_sets)
 
-        #Local Section Reduction User defined Name
+        # Local Section Reduction User defined Name
         if user_defined_name:
             clientObject.user_defined_name_enabled = True
             clientObject.name = user_defined_name
 
-        #Local Section Reduction Components
+        # Local Section Reduction Components
         clientObject.components = model.clientModel.factory.create('ns0:array_of_steel_member_local_section_reduction_components')
 
         for i,j in enumerate(components):
             smlsr = model.clientModel.factory.create('ns0:steel_member_local_section_reduction_components_row')
-            clearAttributes(smlsr.row)
             smlsr.no = i+1
+            smlsr.row = model.clientModel.factory.create('ns0:steel_member_local_section_reduction_components')
+            clearAttributes(smlsr.row)
             smlsr.row.reduction_type = components[i][0].name
             smlsr.row.position = components[i][1]
             smlsr.row.multiple = components[i][2]
             smlsr.row.fastener_definition_type = components[i][3].name
             if smlsr.row.fastener_definition_type == "DEFINITION_TYPE_ABSOLUTE":
                 smlsr.row.reduction_area = components[i][4]
             elif smlsr.row.fastener_definition_type == "DEFINITION_TYPE_RELATIVE":
```

### Comparing `RSTAB-1.5.0/RSTAB/TypesForSteelDesign/steelBoundaryConditions.py` & `RSTAB-1.6.0/RSTAB/TypesForSteelDesign/steelBoundaryConditions.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 
         # Boundary Conditions Nodal Supports
         clientObject.nodal_supports = model.clientModel.factory.create('ns0:steel_boundary_conditions.nodal_supports')
 
         for i,j in enumerate(nodal_supports):
             mlvlp = model.clientModel.factory.create('ns0:steel_boundary_conditions_nodal_supports_row')
             mlvlp.no = i+1
+            mlvlp.row = model.clientModel.factory.create('ns0:steel_boundary_conditions_nodal_supports')
             mlvlp.row.node_seq_no = nodal_supports[i][0]
             mlvlp.row.support_type = nodal_supports[i][1].name
             mlvlp.row.support_in_x = nodal_supports[i][2]
             mlvlp.row.support_in_y = nodal_supports[i][3]
             mlvlp.row.support_in_z = nodal_supports[i][4]
             mlvlp.row.restraint_about_x = nodal_supports[i][5]
             mlvlp.row.restraint_about_y = nodal_supports[i][6]
@@ -140,14 +141,15 @@
 
         # Boundary Conditions Member Hinges
         clientObject.member_hinges = model.clientModel.factory.create('ns0:steel_boundary_conditions.member_hinges')
 
         for i,j in enumerate(member_hinges):
             mlvlp = model.clientModel.factory.create('ns0:steel_boundary_conditions_member_hinges_row')
             mlvlp.no = i+1
+            mlvlp.row = model.clientModel.factory.create('ns0:steel_boundary_conditions_member_hinges')
             mlvlp.row.node_seq_no = member_hinges[i][0]
             mlvlp.row.release_in_x = member_hinges[i][1]
             mlvlp.row.release_in_y = member_hinges[i][2]
             mlvlp.row.release_in_z = member_hinges[i][3]
             mlvlp.row.release_about_x = member_hinges[i][4]
             mlvlp.row.release_about_y = member_hinges[i][5]
             mlvlp.row.release_about_z = member_hinges[i][6]
```

### Comparing `RSTAB-1.5.0/RSTAB/TypesForSteelDesign/steelEffectiveLengths.py` & `RSTAB-1.6.0/RSTAB/TypesForSteelDesign/steelEffectiveLengths.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,15 @@
 
         # Effective Lengths Nodal Supports
         clientObject.nodal_supports = model.clientModel.factory.create('ns0:array_of_steel_effective_lengths_nodal_supports')
 
         for i,j in enumerate(nodal_supports):
             mlvlp = model.clientModel.factory.create('ns0:steel_effective_lengths_nodal_supports_row')
             mlvlp.no = i+1
+            mlvlp.row = model.clientModel.factory.create('ns0:steel_effective_lengths_nodal_supports')
             mlvlp.row.support_type = nodal_supports[i][0].name
             mlvlp.row.support_in_z = nodal_supports[i][1]
             mlvlp.row.support_spring_in_y = nodal_supports[i][2]
             mlvlp.row.eccentricity_type = nodal_supports[i][3].name
             mlvlp.row.eccentricity_ez = nodal_supports[i][4]
             mlvlp.row.restraint_spring_about_x = nodal_supports[i][5]
             mlvlp.row.restraint_spring_about_z = nodal_supports[i][6]
@@ -142,14 +143,15 @@
 
         # Effective Lengths Factors
         clientObject.factors = model.clientModel.factory.create('ns0:array_of_steel_effective_lengths_factors')
 
         for i,j in enumerate(factors):
             mlvlp_f = model.clientModel.factory.create('ns0:steel_effective_lengths_factors_row')
             mlvlp_f.no = i+1
+            mlvlp_f.row = model.clientModel.factory.create('ns0:steel_effective_lengths_factors')
             mlvlp_f.row.flexural_buckling_u = factors[i][0]
             mlvlp_f.row.flexural_buckling_v = factors[i][1]
             mlvlp_f.row.flexural_buckling_y = factors[i][2]
             mlvlp_f.row.flexural_buckling_z = factors[i][3]
             mlvlp_f.row.torsional_buckling = factors[i][4]
             mlvlp_f.row.lateral_torsional_buckling = factors[i][5]
             mlvlp_f.row.lateral_torsional_buckling_top = factors[i][6]
```

### Comparing `RSTAB-1.5.0/RSTAB/TypesForTimberDesign/timberEffectiveLengths.py` & `RSTAB-1.6.0/RSTAB/TypesForTimberDesign/timberEffectiveLengths.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 
         # Effective Lengths Nodal Supports
         clientObject.nodal_supports = model.clientModel.factory.create('ns0:array_of_timber_effective_lengths_nodal_supports')
 
         for i,j in enumerate(nodal_supports):
             mlvlp = model.clientModel.factory.create('ns0:timber_effective_lengths_nodal_supports_row')
             mlvlp.no = i+1
+            mlvlp.row = model.clientModel.factory.create('ns0:timber_effective_lengths_nodal_supports')
             mlvlp.row.support_type = nodal_supports[i][0].name
             mlvlp.row.support_in_z = nodal_supports[i][1]
             mlvlp.row.eccentricity_type = nodal_supports[i][2].name
             mlvlp.row.support_in_y_type = nodal_supports[i][3].name
             mlvlp.row.restraint_about_x_type = nodal_supports[i][4].name
             mlvlp.row.nodes = ConvertToDlString(nodal_supports[i][5])
 
@@ -115,14 +116,15 @@
 
         # Effective Lengths Factors
         clientObject.factors = model.clientModel.factory.create('ns0:array_of_timber_effective_lengths_factors')
 
         for i,j in enumerate(factors):
             mlvlp_f = model.clientModel.factory.create('ns0:timber_effective_lengths_factors_row')
             mlvlp_f.no = i+1
+            mlvlp_f.row = model.clientModel.factory.create('ns0:timber_effective_lengths_factors')
             mlvlp_f.row.flexural_buckling_u = factors[i][0]
             mlvlp_f.row.flexural_buckling_v = factors[i][1]
             mlvlp_f.row.lateral_torsional_buckling = factors[i][2]
 
             clientObject.factors.timber_effective_lengths_factors.append(mlvlp_f)
 
         # Effective Lengths Fire Design
```

### Comparing `RSTAB-1.5.0/RSTAB/TypesForTimberDesign/timberMemberLocalSectionReduction.py` & `RSTAB-1.6.0/RSTAB/TypesForTimberDesign/timberMemberLocalSectionReduction.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,58 +76,58 @@
 
 class TimberMemberLocalSectionReduction():
     def __init__(self,
                  no: int = 1,
                  members: str = '1',
                  member_sets: str = '',
                  components: list = None,
-                 user_defined_name: str = '',
+                 name: str = '',
                  comment: str = '',
                  params: dict = None,
                  model = Model):
         """
         Args:
             no (int): Member Local Section Reduction Tag
             members (str): Assigned Members
             member_sets (str): Assigned Member Sets
             components (list): List of Component classes
-            user_defined_name (str): User Defined  Member Local Section Reduction Name
+            name (str): User Defined  Member Local Section Reduction Name
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
         # Client Model | Types For Timber Member Local Section Reduction
         clientObject = model.clientModel.factory.create('ns0:timber_member_local_section_reduction')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
-        #Local Section Reduction No.
+        # Local Section Reduction No.
         clientObject.no = no
 
-        #Local Section Reduction Assigned Members
+        # Local Section Reduction Assigned Members
         clientObject.members = ConvertToDlString(members)
 
-        #Local Section Reduction Assigned Member Sets
+        # Local Section Reduction Assigned Member Sets
         clientObject.member_sets = ConvertToDlString(member_sets)
 
-        #Local Section Reduction User defined Name
-        if user_defined_name:
+        # Local Section Reduction User defined Name
+        if name:
             clientObject.user_defined_name_enabled = True
-            clientObject.name = user_defined_name
+            clientObject.name = name
 
-        #Local Section Reduction Components
+        # Local Section Reduction Components
         clientObject.components = model.clientModel.factory.create('ns0:array_of_timber_member_local_section_reduction_components')
 
         for i,j in enumerate(components):
             smlsr = model.clientModel.factory.create('ns0:timber_member_local_section_reduction_components_row')
-            clearAttributes(smlsr.row)
-
             smlsr.no = i+1
+            smlsr.row = model.clientModel.factory.create('ns0:timber_member_local_section_reduction_components')
+            clearAttributes(smlsr.row)
             smlsr.row.reduction_type = components[i].reduction_type
             if smlsr.row.reduction_type == 'REDUCTION_COMPONENT_TYPE_RECTANGLE_OPENING':
                 smlsr.row.position = components[i].position
                 smlsr.row.width = components[i].width
                 smlsr.row.height = components[i].height
                 smlsr.row.z_axis_reference_type = components[i].z_axis_reference_type
                 smlsr.row.distance = components[i].distance
```

### Comparing `RSTAB-1.5.0/RSTAB/TypesForTimberDesign/timberMemberRotationalRestraint.py` & `RSTAB-1.6.0/RSTAB/ConcreteDesign/ConcreteServiceabilityConfigurations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,67 @@
-from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString, GetAddonStatus, SetAddonStatus
-from RSTAB.enums import AddOn
+from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
+
+
+class ConcreteServiceabilityConfiguration():
 
-class TimberMemberRotationalRestraint():
     def __init__(self,
                 no: int = 1,
-                name: str = '',
-                members: str = "",
-                member_sets: str = "",
-                spring_stiffness: float = 20000,
+                name: str = 'SLS',
+                members: str = 'All',
+                member_sets: str = 'All',
                 comment: str = '',
                 params: dict = None,
                 model = Model):
         """
         Args:
-            no (int): Timber Member Rotational Restraint Tag
-            name (str): User Defined Member Rotational Restraint Name
+            no (int): Configuration Tag
+            name (str): User Defined Name
             members (str): Assigned Members
             member_sets (str): Assigned Member Sets
-            spring_stiffness (float): Total Rotational Spring Stiffness
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
-        # Deducing RSTAB Language from timber_design_addon String:
-        modelInfo = Model.clientModel.service.get_model_info()
-        if modelInfo.property_addon_timber_design.split()[0] != 'Timber':
-            raise ValueError("WARNING: The TimberMemberRotationalRestraints operates with the RSTAB Application set to English. Kindly switch RSTAB to English such that Database searches can completed successfully.")
-
-        # Check if Timber Design Add-on is ON.
-        if not GetAddonStatus(model.clientModel, AddOn.timber_design_active):
-            SetAddonStatus(model.clientModel, AddOn.timber_design_active, True)
-
-        # Client Model / Types For Timber Design Member Rotational Restraints
-        clientObject = model.clientModel.factory.create('ns0:timber_member_rotational_restraint')
+        # Client model | Concrete Durabilities
+        clientObject = model.clientModel.factory.create('ns0:concrete_design_sls_configuration')
 
-        # Clears Object Attributes / Sets all the attributes to None
+        # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
-        # Member Rotational Restraint No.
+        # Concrete Durability No.
         clientObject.no = no
 
-        # Member Rotational Restraint Assigned Members
-        clientObject.members = ConvertToDlString(members)
-
-        # Member Rotational Restraint Assigned Member Sets
-        clientObject.member_sets = ConvertToDlString(member_sets)
-
-        # Member Rotational Restraint Name
+        # User Defined Name
         if name:
             clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
-        # Member Rotational Restraint Type
-        clientObject.type = 'TYPE_MANUALLY'
-
-        # Member Rotational Spring Stiffness
-        clientObject.total_rotational_spring_stiffness = spring_stiffness
+        # Assigned Members
+        if members == 'All':
+            clientObject.assigned_to_all_members = True
+
+        else:
+            clientObject.assigned_to_all_members = False
+            clientObject.assigned_to_members = ConvertToDlString(members)
+
+        # Assigned Member Sets
+        if member_sets == 'All':
+            clientObject.assigned_to_all_member_sets = True
+
+        else:
+            clientObject.assigned_to_all_member_sets = False
+            clientObject.assigned_to_member_sets = ConvertToDlString(member_sets)
 
-        #Comment
+        # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
-        # Add Timber Member Rotational Restraint to Client Model
-        model.clientModel.service.set_timber_member_rotational_restraint(clientObject)
+        # Add Global Parameter to client model
+        model.clientModel.service.set_concrete_design_sls_configuration(clientObject)
```

### Comparing `RSTAB-1.5.0/RSTAB/TypesForTimberDesign/timberServiceClass.py` & `RSTAB-1.6.0/RSTAB/ConcreteDesign/ConcreteUltimateConfigurations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,67 @@
 from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
-from RSTAB.enums import TimberServiceClassServiceClass
 
-class TimberServiceClass():
+
+class ConcreteUltimateConfiguration():
+
     def __init__(self,
                 no: int = 1,
-                name: str = '',
-                members: str = '',
-                member_sets: str = '',
-                service_class = TimberServiceClassServiceClass.TIMBER_SERVICE_CLASS_TYPE_1,
+                name: str = 'ULS',
+                members: str = 'All',
+                member_sets: str = 'All',
                 comment: str = '',
-                params: dict = None):
+                params: dict = None,
+                model = Model):
         """
         Args:
-            no (int): Timber Member Shear Panel Tag
-            name (str): User Defined Member Shear Panel Name
-            definition_type (enum): Timber Member Shear Panel Definition Type Enumeration
+            no (int): Configuration Tag
+            name (str): User Defined Name
             members (str): Assigned Members
             member_sets (str): Assigned Member Sets
-            service_class (enum): Timber Service Class Service Class
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
+            model (RSTAB Class, optional): Model to be edited
         """
 
-         # Client Model | Types For Timber Design Service Class
-        clientObject = Model.clientModel.factory.create('ns0:timber_service_class')
+        # Client model | Concrete Durabilities
+        clientObject = model.clientModel.factory.create('ns0:concrete_design_uls_configuration')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
-        # Member Service Class
+        # Concrete Durability No.
         clientObject.no = no
 
-        # Assigned Members
-        clientObject.member = ConvertToDlString(members)
-
-        # Assigned Member Sets
-        clientObject.member_sets = ConvertToDlString(member_sets)
-
-        # Service Class
-        clientObject.service_class = service_class.name
-
         # User Defined Name
         if name:
             clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
+        # Assigned Members
+        if members == 'All':
+            clientObject.assigned_to_all_members = True
+
+        else:
+            clientObject.assigned_to_all_members = False
+            clientObject.assigned_to_members = ConvertToDlString(members)
+
+        # Assigned Member Sets
+        if member_sets == 'All':
+            clientObject.assigned_to_all_member_sets = True
+
+        else:
+            clientObject.assigned_to_all_member_sets = False
+            clientObject.assigned_to_member_sets = ConvertToDlString(member_sets)
+
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
-        # Add Service Class to client model
-        Model.clientModel.service.set_timber_service_class(clientObject)
+        # Add Global Parameter to client model
+        model.clientModel.service.set_concrete_design_uls_configuration(clientObject)
```

### Comparing `RSTAB-1.5.0/RSTAB/TypesforConcreteDesign/ConcreteDurability.py` & `RSTAB-1.6.0/RSTAB/TypesforConcreteDesign/ConcreteDurability.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/TypesforConcreteDesign/ConcreteEffectiveLength.py` & `RSTAB-1.6.0/RSTAB/TypesforConcreteDesign/ConcreteEffectiveLength.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,24 +65,26 @@
         clientObject.structure_type_about_axis_z = flexural_buckling_about_z[1].name
 
         # Factors
         clientObject.factors = model.clientModel.factory.create('ns0:array_of_concrete_effective_lengths_factors')
         for i in range(len(factors)):
             mlvlp = model.clientModel.factory.create('ns0:concrete_effective_lengths_factors_row')
             mlvlp.no = i+1
+            mlvlp.row = model.clientModel.factory.create('ns0:concrete_effective_lengths_factors')
             mlvlp.row.flexural_buckling_y = factors[i][0]
             mlvlp.row.flexural_buckling_z = factors[i][1]
 
             clientObject.factors.concrete_effective_lengths_factors.append(mlvlp)
 
         # Nodal Supports
         clientObject.nodal_supports = model.clientModel.factory.create('ns0:array_of_concrete_effective_lengths_nodal_supports')
         for i in range(len(nodal_supports)):
             mlvlp = model.clientModel.factory.create('ns0:concrete_effective_lengths_nodal_supports_row')
             mlvlp.no = i+1
+            mlvlp.row = model.clientModel.factory.create('ns0:concrete_effective_lengths_nodal_supports')
             mlvlp.row.support_type = nodal_supports[i][0].name
             mlvlp.row.support_in_z = nodal_supports[i][1]
             mlvlp.row.eccentricity_type = nodal_supports[i][2].name
             mlvlp.row.support_in_y_type = nodal_supports[i][3].name
             mlvlp.row.restraint_about_x_type = nodal_supports[i][4].name
             mlvlp.row.restraint_about_z_type = nodal_supports[i][5].name
             mlvlp.row.restraint_warping_type = nodal_supports[i][6].name
```

### Comparing `RSTAB-1.5.0/RSTAB/baseSettings.py` & `RSTAB-1.6.0/RSTAB/baseSettings.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/dependencies.py` & `RSTAB-1.6.0/RSTAB/dependencies.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/enums.py` & `RSTAB-1.6.0/RSTAB/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,28 @@
     Welded Type | Enum
     """
     WELD_BEVEL_AND_FILLET, WELD_DOUBLE_BEVEL, WELD_DOUBLE_FILLET, WELD_DOUBLE_J,\
     WELD_DOUBLE_SQUARE, WELD_DOUBLE_U, WELD_DOUBLE_V, WELD_J_AND_FILLET, WELD_SINGLE_BEVEL,\
     WELD_SINGLE_FILLET, WELD_SINGLE_J, WELD_SINGLE_SQUARE, WELD_SINGLE_U, WELD_SINGLE_V, WELD_V_AND_FILLET = range(15)
 
 
+class WeldComponentType(Enum):
+    '''
+    Aluminum Member Transverse Weld Component | Enum
+    '''
+    WELD_COMPONENT_TYPE_BUTT, WELD_COMPONENT_TYPE_FILLET = range(2)
+
+
+class WeldingMethod(Enum):
+    '''
+    Aluminum Member Transverse Weld Welding Method | Enum
+    '''
+    WELDING_METHOD_TIG, WELDING_METHOD_MIG = range(2)
+
+
 class WeldLongitudalArrangement(Enum):
     """
     Weld Longitudat Arrangement Type | Enum
     """
     CHAIN_INTERMITTENT, CONTINUOUS, STAGGERED_INTERMITTENT = range(3)
 
 
@@ -235,15 +249,15 @@
     LOAD_TYPE_COMPONENTS, LOAD_TYPE_FORCE, LOAD_TYPE_MASS, LOAD_TYPE_MOMENT = range(4)
 
 
 class NodalLoadSpecificDirectionType(Enum):
     '''
     Nodal Load Specific Direction Type
     '''
-    DIRECTION_TYPE_DIRECTED_TO_NODE, DIRECTION_TYPE_PARALLEL_TO_CS_OF_LINE, DIRECTION_TYPE_PARALLEL_TO_CS_OF_MEMBER, DIRECTION_TYPE_PARALLEL_TO_TWO_NODES, DIRECTION_TYPE_ROTATED_VIA_3_ANGLES = range(5)
+    DIRECTION_TYPE_DIRECTED_TO_NODE, DIRECTION_TYPE_PARALLEL_TO_CS_OF_MEMBER, DIRECTION_TYPE_PARALLEL_TO_TWO_NODES, DIRECTION_TYPE_ROTATED_VIA_3_ANGLES = range(4)
 
 
 class NodalLoadAxesSequence(Enum):
     '''
     Nodal Load Axes Sequence
     '''
     SEQUENCE_XYZ, SEQUENCE_XZY, SEQUENCE_YXZ, SEQUENCE_YZX, SEQUENCE_ZXY, SEQUENCE_ZYX = range(6)
@@ -828,15 +842,16 @@
     EIGENVALUE_METHOD, INCREMENTALY_METHOD_WITHOUT_EIGENVALUE, INCREMENTALY_METHOD_WITH_EIGENVALUE = range(3)
 
 
 class StabilityAnalysisSettingsEigenvalueMethod(Enum):
     '''
     Stability Analysis Settings Eigenvalue Method | Enum
     '''
-    EIGENVALUE_METHOD_SUBSPACE_ITERATION, E_EIGENVALUE_METHOD_SHIFTED_INVERSE_POWER_METHOD = range(2)
+    EIGENVALUE_METHOD_ICG_ITERATION, EIGENVALUE_METHOD_LANCZOS, EIGENVALUE_METHOD_ROOTS_OF_CHARACTERISTIC_POLYNOMIAL, \
+    EIGENVALUE_METHOD_SUBSPACE_ITERATION, EIGENVALUE_METHOD_SHIFTED_INVERSE_POWER_METHOD = range(5)
 
 
 class StabilityAnalysisSettingsMatrixType(Enum):
     '''
     Stability Analysis Settings Matrix Type | Enum
     '''
     MATRIX_TYPE_STANDARD, MATRIX_TYPE_UNIT = range(2)
@@ -858,37 +873,36 @@
     TYPE_ARC, TYPE_CIRCLE, TYPE_CUT_VIA_SECTION, TYPE_CUT_VIA_TWO_LINES, TYPE_ELLIPTICAL_ARC, TYPE_ELLIPSE, TYPE_NURBS, TYPE_PARABOLA, TYPE_POLYLINE, TYPE_SPLINE = range(10)
 
 
 class ObjectTypes(Enum):
     '''
     Object Types
     '''
-    E_OBJECT_TYPE_ACTION, E_OBJECT_TYPE_ACTION_COMBINATION, E_OBJECT_TYPE_ALUMINUM_EFFECTIVE_LENGTHS, E_OBJECT_TYPE_ALUMINUM_MEMBER_LOCAL_SECTION_REDUCTION, \
-    E_OBJECT_TYPE_ALUMINUM_MEMBER_ROTATIONAL_RESTRAINT, E_OBJECT_TYPE_ALUMINUM_MEMBER_SHEAR_PANEL, E_OBJECT_TYPE_ALUMINUM_MEMBER_TRANSVERSE_WELD, E_OBJECT_TYPE_BOREHOLE, \
+    E_OBJECT_TYPE_ACTION, E_OBJECT_TYPE_ACTION_COMBINATION, E_OBJECT_TYPE_ALUMINUM_EFFECTIVE_LENGTHS, E_OBJECT_TYPE_ALUMINUM_MEMBER_LOCAL_SECTION_REDUCTION, E_OBJECT_TYPE_ALUMINUM_MEMBER_TRANSVERSE_WELD, E_OBJECT_TYPE_BOREHOLE, \
     E_OBJECT_TYPE_BUILDING_STORY, E_OBJECT_TYPE_CLIPPING_BOX, E_OBJECT_TYPE_CLIPPING_PLANE, E_OBJECT_TYPE_COMBINATION_WIZARD, E_OBJECT_TYPE_CONSTRUCTION_STAGE,  \
     E_OBJECT_TYPE_COORDINATE_SYSTEM, E_OBJECT_TYPE_DESIGN_SITUATION, E_OBJECT_TYPE_DESIGN_SUPPORT, E_OBJECT_TYPE_DIMENSION, E_OBJECT_TYPE_DXF_FILE_MODEL_OBJECT,  \
     E_OBJECT_TYPE_DXF_MODEL_OBJECT, E_OBJECT_TYPE_FREE_CIRCULAR_LOAD, E_OBJECT_TYPE_FREE_CONCENTRATED_LOAD, E_OBJECT_TYPE_FREE_LINE_LOAD, E_OBJECT_TYPE_FREE_POLYGON_LOAD,  \
     E_OBJECT_TYPE_FREE_RECTANGULAR_LOAD, E_OBJECT_TYPE_GLOBAL_PARAMETER, E_OBJECT_TYPE_IMPERFECTION_CASE, E_OBJECT_TYPE_IMPOSED_LINE_DEFORMATION, E_OBJECT_TYPE_IMPOSED_NODAL_DEFORMATION, \
     E_OBJECT_TYPE_INTERSECTION, E_OBJECT_TYPE_LINE, E_OBJECT_TYPE_LINE_GRID, E_OBJECT_TYPE_LINE_HINGE, E_OBJECT_TYPE_LINE_LOAD, E_OBJECT_TYPE_LINE_MESH_REFINEMENT, E_OBJECT_TYPE_LINE_SET, \
     E_OBJECT_TYPE_LINE_SET_LOAD, E_OBJECT_TYPE_LINE_SUPPORT, E_OBJECT_TYPE_LINE_WELDED_JOINT, E_OBJECT_TYPE_LOAD_CASE, E_OBJECT_TYPE_LOAD_COMBINATION, E_OBJECT_TYPE_MATERIAL, \
     E_OBJECT_TYPE_MEMBER, E_OBJECT_TYPE_MEMBER_DEFINABLE_STIFFNESS, E_OBJECT_TYPE_MEMBER_ECCENTRICITY, E_OBJECT_TYPE_MEMBER_HINGE, E_OBJECT_TYPE_MEMBER_IMPERFECTION, E_OBJECT_TYPE_MEMBER_LOAD, \
     E_OBJECT_TYPE_MEMBER_NONLINEARITY, E_OBJECT_TYPE_MEMBER_REPRESENTATIVE, E_OBJECT_TYPE_MEMBER_RESULT_INTERMEDIATE_POINT, E_OBJECT_TYPE_MEMBER_SET, E_OBJECT_TYPE_MEMBER_SET_IMPERFECTION, \
     E_OBJECT_TYPE_MEMBER_SET_LOAD, E_OBJECT_TYPE_MEMBER_SET_REPRESENTATIVE, E_OBJECT_TYPE_MEMBER_STIFFNESS_MODIFICATION, E_OBJECT_TYPE_MEMBER_SUPPORT, E_OBJECT_TYPE_MEMBER_TRANSVERSE_STIFFENER, \
     E_OBJECT_TYPE_MODAL_ANALYSIS_SETTINGS, E_OBJECT_TYPE_NODAL_LOAD, E_OBJECT_TYPE_NODAL_MESH_REFINEMENT, E_OBJECT_TYPE_NODAL_SUPPORT, E_OBJECT_TYPE_NODE, E_OBJECT_TYPE_NOTE, \
     E_OBJECT_TYPE_OBJECT_SNAP, E_OBJECT_TYPE_OPENING, E_OBJECT_TYPE_OPENING_LOAD, E_OBJECT_TYPE_PUNCHING_REINFORCEMENT, E_OBJECT_TYPE_RELATIONSHIP_BETWEEN_LOAD_CASES, \
     E_OBJECT_TYPE_RESULT_COMBINATION, E_OBJECT_TYPE_RESULT_SECTION, E_OBJECT_TYPE_RIGID_LINK, E_OBJECT_TYPE_SECTION, E_OBJECT_TYPE_SOIL_MASSIF, E_OBJECT_TYPE_SOLID, E_OBJECT_TYPE_SOLID_CONTACTS, \
     E_OBJECT_TYPE_SOLID_GAS, E_OBJECT_TYPE_SOLID_LOAD, E_OBJECT_TYPE_SOLID_MESH_REFINEMENT, E_OBJECT_TYPE_SOLID_SET, E_OBJECT_TYPE_SOLID_SET_LOAD, E_OBJECT_TYPE_SPECTRAL_ANALYSIS_SETTINGS, \
     E_OBJECT_TYPE_STABILITY_ANALYSIS_SETTINGS, E_OBJECT_TYPE_STATIC_ANALYSIS_SETTINGS, E_OBJECT_TYPE_STEEL_BOUNDARY_CONDITIONS, E_OBJECT_TYPE_STEEL_EFFECTIVE_LENGTHS, \
-    E_OBJECT_TYPE_STEEL_MEMBER_LOCAL_SECTION_REDUCTION, E_OBJECT_TYPE_STEEL_MEMBER_ROTATIONAL_RESTRAINT, E_OBJECT_TYPE_STEEL_MEMBER_SHEAR_PANEL, E_OBJECT_TYPE_STRUCTURE_MODIFICATION, \
+    E_OBJECT_TYPE_STEEL_MEMBER_LOCAL_SECTION_REDUCTION, E_OBJECT_TYPE_STRUCTURE_MODIFICATION, \
     E_OBJECT_TYPE_SURFACE, E_OBJECT_TYPE_SURFACES_CONTACT, E_OBJECT_TYPE_SURFACES_CONTACT_TYPE, E_OBJECT_TYPE_SURFACE_ECCENTRICITY, E_OBJECT_TYPE_SURFACE_IMPERFECTION, E_OBJECT_TYPE_SURFACE_LOAD, \
     E_OBJECT_TYPE_SURFACE_MESH_REFINEMENT, E_OBJECT_TYPE_SURFACE_RESULTS_ADJUSTMENT, E_OBJECT_TYPE_SURFACE_SET, E_OBJECT_TYPE_SURFACE_SET_IMPERFECTION, E_OBJECT_TYPE_SURFACE_SET_LOAD, \
     E_OBJECT_TYPE_SURFACE_STIFFNESS_MODIFICATION, E_OBJECT_TYPE_SURFACE_SUPPORT, E_OBJECT_TYPE_TERRAIN, E_OBJECT_TYPE_THICKNESS, E_OBJECT_TYPE_TIMBER_EFFECTIVE_LENGTHS, \
-    E_OBJECT_TYPE_TIMBER_MEMBER_LOCAL_SECTION_REDUCTION, E_OBJECT_TYPE_TIMBER_MEMBER_ROTATIONAL_RESTRAINT, E_OBJECT_TYPE_TIMBER_MEMBER_SHEAR_PANEL, E_OBJECT_TYPE_TIMBER_MOISTURE_CLASS, \
-    E_OBJECT_TYPE_TIMBER_SERVICE_CLASS, E_OBJECT_TYPE_TIMBER_SERVICE_CONDITIONS, E_OBJECT_TYPE_VISUAL_OBJECT, E_OBJECT_TYPE_WIND_PROFILE, E_OBJECT_TYPE_WIND_SIMULATION, E_OBJECT_TYPE_WIND_SIMULATION_ANALYSIS_SETTINGS = range(115)
-
+    E_OBJECT_TYPE_TIMBER_MEMBER_LOCAL_SECTION_REDUCTION, E_OBJECT_TYPE_TIMBER_MOISTURE_CLASS, \
+    E_OBJECT_TYPE_TIMBER_SERVICE_CLASS, E_OBJECT_TYPE_TIMBER_SERVICE_CONDITIONS, E_OBJECT_TYPE_VISUAL_OBJECT, E_OBJECT_TYPE_WIND_PROFILE, E_OBJECT_TYPE_WIND_SIMULATION, E_OBJECT_TYPE_WIND_SIMULATION_ANALYSIS_SETTINGS,\
+    E_OBJECT_TYPE_RESPONSE_SPECTRUM, E_OBJECT_TYPE_MEMBER_ROTATIONAL_RESTRAINT, E_OBJECT_TYPE_MEMBER_SHEAR_PANEL = range(112)
 
 class export_to_ifc_axis_rotation_sequence_type(Enum):
     '''
     Export to IFC Axis Rotation Sequence Type
     '''
     XYZ, XZY, YXZ, YZX, ZXY, ZYX = range(6)
 
@@ -1121,15 +1135,15 @@
     NUMBER_OF_MODES_METHOD_USER_DEFINED, NUMBER_OF_MODES_METHOD_EFFECTIVE_MASS_FACTORS, NUMBER_OF_MODES_METHOD_MAXIMUM_FREQUENCY = range(3)
 
 
 class ModalSolutionMethod(Enum):
     '''
     Modal Analysis Settings Solution Method
     '''
-    METHOD_ICG_ITERATION, METHOD_LANCZOS, METHOD_ROOT_OF_CHARACTERISTIC_POLYNOMIAL, METHOD_SUBSPACE_ITERATION, SOLUTION_METHOD_SHIFTED_INVERSE_POWER_METHOD = range(5)
+    METHOD_LANCZOS, METHOD_ROOT_OF_CHARACTERISTIC_POLYNOMIAL, METHOD_SHIFTED_INVERSE_POWER_METHOD, METHOD_SUBSPACE_ITERATION = range(4)
 
 
 class ModalMassConversionType(Enum):
     '''
     Modal Analysis Settings Mass Conversion Type
     '''
     MASS_CONVERSION_TYPE_FULL_LOADS_AS_MASS, MASS_CONVERSION_TYPE_Z_COMPONENTS_OF_LOADS, MASS_CONVERSION_TYPE_Z_COMPONENTS_OF_LOADS_IN_DIRECTION_OF_GRAVITY = range(3)
@@ -1520,17 +1534,17 @@
 class AddOn(Enum):
     '''
     AddOn types
     '''
     stress_analysis_active, concrete_design_active, steel_design_active, timber_design_active, aluminum_design_active, \
     steel_joints_active, timber_joints_active, craneway_design_active, masonry_design_active, multilayer_surfaces_design_active, \
     material_nonlinear_analysis_active, structure_stability_active, construction_stages_active, time_dependent_active, \
-    form_finding_active, cutting_patterns_active, torsional_warping_active, cost_estimation_active, modal_active, spectral_active, \
-    time_history_active, pushover_active, harmonic_response_active, building_model_active, wind_simulation_active, \
-    geotechnical_analysis_active = range(26)
+    influence_lines_areas_active, form_finding_active, cutting_patterns_active, torsional_warping_active, cost_estimation_active, modal_active, equivalent_lateral_forces_active, spectral_active, \
+    time_history_active, pushover_active, harmonic_response_active, building_model_active, wind_simulation_active, tower_wizard_active, tower_equipment_wizard_active, piping_active, air_cushions_active,\
+    geotechnical_analysis_active = range(32)
 
 
 class IFCExportType(Enum):
     '''
     IFC Export Type
     '''
     E_EXPORT_IFC4_REFERENCE_VIEW, E_EXPORT_IFC4_STRUCTURAL_ANALYSIS_VIEW = range(2)
@@ -1664,56 +1678,14 @@
 
 class AluminumEffectiveLengthsDeterminationMcrEurope(Enum):
     '''
     Aluminum Effective Lengths Determination MCR Europe
     '''
     DETERMINATION_EUROPE_EIGENVALUE, DETERMINATION_EUROPE_USER_DEFINED = range(2)
 
-class AluminumMemberRotationalRestraintType(Enum):
-    '''
-    Aluminum Member Rotational Restraint Type
-    '''
-    TYPE_CONTINUOUS, TYPE_DISCRETE, TYPE_MANUALLY = range(3)
-
-class AluminumMemberRotationalRestraintContinuousBeamEffect(Enum):
-    '''
-    Aluminum Member Rotational Restraint Continuous Beam Effect
-    '''
-    CONTINUOUS_BEAM_EFFECT_END_PANEL, CONTINUOUS_BEAM_EFFECT_INTERNAL_PANEL = range(2)
-
-class AluminumMemberRotationalRestraintPositionofSheeting(Enum):
-    '''
-    Aluminum Member Rotational Restraint Position of Sheeting
-    '''
-    SHEETING_POSITION_NEGATIVE, SHEETING_POSITION_POSITIVE = range(2)
-
-class AluminumMemberRotationalRestraintRotationalStiffness(Enum):
-    '''
-    Steel Member Rotational Restraint Rotational Stiffness
-    '''
-    ROTATIONAL_STIFFNESS_INFINITELY, ROTATIONAL_STIFFNESS_MANUALLY = range(2)
-
-class AluminumMemberShearPanelDefinitionType(Enum):
-    '''
-    Aluminum Member Shear Panel Definition Type
-    '''
-    DEFINITION_TYPE_BRACING, DEFINITION_TYPE_DEFINE_S_PROV, DEFINITION_TYPE_TRAPEZOIDAL_SHEETING, DEFINITION_TYPE_TRAPEZOIDAL_SHEETING_AND_BRACING = range(4)
-
-class AluminumMemberShearPanelPositionOnSection(Enum):
-    '''
-    Aluminum Member Shear Panel Position On Section
-    '''
-    POSITION_DEFINE, POSITION_IN_CENTROID, POSITION_ON_LOWER_FLANGE, POSITION_ON_UPPER_FLANGE = range(4)
-
-class AluminumMemberShearPanelFasteningArrangement(Enum):
-    '''
-    Aluminum Member Shear Panel Fastening Arrangement
-    '''
-    FASTENING_ARRANGEMENT_EVERY_RIB, FASTENING_ARRANGEMENT_EVERY_SECOND_RIB = range(2)
-
 class SteelEffectiveLengthsDeterminationMcrIs800(Enum):
     '''
     Steel Effective Lengths Determination MCR IS 800
     '''
     DETERMINATION_IS800_EIGENVALUE, DETERMINATION_IS800_USER_DEFINED = range(2)
 
 
@@ -1811,56 +1783,14 @@
 
 class SteelEffectiveLengthsMemberTypeZZ(Enum):
     '''
     Steel Effective Lengths Member Type ZZ
     '''
     MEMBER_TYPE_BEAM, MEMBER_TYPE_CANTILEVER = range(2)
 
-class SteelMemberShearPanelDefinitionType(Enum):
-    '''
-    Steel Member Shear Panel Definition Type
-    '''
-    DEFINITION_TYPE_BRACING, DEFINITION_TYPE_DEFINE_S_PROV, DEFINITION_TYPE_TRAPEZOIDAL_SHEETING, DEFINITION_TYPE_TRAPEZOIDAL_SHEETING_AND_BRACING = range(4)
-
-class SteelMemberShearPanelPositionOnSection(Enum):
-    '''
-    Steel Member Shear Panel Position On Section
-    '''
-    POSITION_DEFINE, POSITION_IN_CENTROID, POSITION_ON_LOWER_FLANGE, POSITION_ON_UPPER_FLANGE = range(4)
-
-class SteelMemberShearPanelFasteningArrangement(Enum):
-    '''
-    Steel Member Shear Panel Fastening Arrangement
-    '''
-    FASTENING_ARRANGEMENT_EVERY_RIB, FASTENING_ARRANGEMENT_EVERY_SECOND_RIB = range(2)
-
-class SteelMemberRotationalRestraintType(Enum):
-    '''
-    Steel Member Rotational Restraint Type
-    '''
-    TYPE_CONTINUOUS, TYPE_DISCRETE, TYPE_MANUALLY = range(3)
-
-class SteelMemberRotationalRestraintContinuousBeamEffect(Enum):
-    '''
-    Steel Member Rotational Restraint Continuous Beam Effect
-    '''
-    CONTINUOUS_BEAM_EFFECT_END_PANEL, CONTINUOUS_BEAM_EFFECT_INTERNAL_PANEL = range(2)
-
-class SteelMemberRotationalRestraintPositionofSheeting(Enum):
-    '''
-    Steel Member Rotational Restraint Position of Sheeting
-    '''
-    SHEETING_POSITION_NEGATIVE, SHEETING_POSITION_POSITIVE = range(2)
-
-class SteelMemberRotationalRestraintRotationalStiffness(Enum):
-    '''
-    Steel Member Rotational Restraint Rotational Stiffness
-    '''
-    ROTATIONAL_STIFFNESS_INFINITELY, ROTATIONAL_STIFFNESS_MANUALLY = range(2)
-
 class SteelBoundaryConditionsSupportType(Enum):
     '''
     Steel Boundary Conditions Support Type
     '''
     SUPPORT_TYPE_FIXED_ALL, SUPPORT_TYPE_FIXED_IN_Y, SUPPORT_TYPE_FIXED_IN_Y_AND_TORSION, SUPPORT_TYPE_FIXED_IN_Y_AND_TORSION_AND_WARPING, \
     SUPPORT_TYPE_FIXED_IN_Y_AND_WARPING, SUPPORT_TYPE_INDIVIDUALLY, SUPPORT_TYPE_NONE, SUPPORT_TYPE_TORSION, SUPPORT_TYPE_TORSION_AND_WARPING = range(9)
 
@@ -2293,8 +2223,249 @@
     '''
     ALL, FORMULA, IS_VALID, CALCULATED_VALUE = range(4)
 
 class ResponseSpectrumDefinitionType(Enum):
     '''
     Response Spectrum Definition Type
     '''
-    ACCORDING_TO_STANDARD, GENERATED_FROM_ACCELEROGRAM, USER_DEFINED, USER_DEFINED_IN_G_FACTOR = range(4)
+    ACCORDING_TO_STANDARD, GENERATED_FROM_ACCELEROGRAM, USER_DEFINED, USER_DEFINED_IN_G_FACTOR = range(4)
+
+class WindSimulationAnalysisSettingsSimulationType(Enum):
+    '''
+    Wind Simulation Analysis Settings Simulation Type
+    '''
+    STEADY_FLOW, TRANSIENT_FLOW = range(2)
+
+class WindSimulationAnalysisSettingsMemberLoadDistribution(Enum):
+    '''
+    Wind Simulation Analysis Settings Member Load Distribution
+    '''
+    CONCENTRATED, TRAPEZODIAL, UNIFORM = range(3)
+
+class WindSimulationAnalysisSettingsMeshRefinementType(Enum):
+    '''
+    Wind Simulation Analysis Settings Mesh Refinement Type
+    '''
+    DISTANCE_FROM_SURFACE, SURFACE_CURVATURE = range(2)
+
+class WindSimulationAnalysisSettingsNumericalSolver(Enum):
+    '''
+    Wind Simulation Analysis Settings Numerical Solver
+    '''
+    OPEN_FOAM = range(1)
+
+class WindSimulationAnalysisSettingsTurbulenceModelType(Enum):
+    '''
+    Wind Simulation Analysis Settings Turbulence Model Type
+    '''
+    TURBULENCE_TYPE_EPSILON, TURBULENCE_TYPE_LES, TURBULENCE_TYPE_OMEGA = range(3)
+
+class TranslationalReleaseNonlinearity(Enum):
+    '''
+    Translational Release Nonlinearity Enumeration
+    '''
+    NONLINEARITY_TYPE_NONE, NONLINEARITY_TYPE_FAILURE_IF_NEGATIVE, NONLINEARITY_TYPE_FAILURE_IF_POSITIVE, \
+    NONLINEARITY_TYPE_DIAGRAM, NONLINEARITY_TYPE_PARTIAL_ACTIVITY = range(5)
+
+class RotationalReleaseNonlinearity(Enum):
+    '''
+    Rotational Release Nonlinearity Enumeration
+    '''
+    NONLINEARITY_TYPE_NONE, NONLINEARITY_TYPE_FAILURE_IF_NEGATIVE, NONLINEARITY_TYPE_FAILURE_IF_POSITIVE, \
+    NONLINEARITY_TYPE_DIAGRAM, NONLINEARITY_TYPE_PARTIAL_ACTIVITY, NONLINEARITY_TYPE_FORCE_MOMENT_DIAGRAM = range(6)
+
+class LineReleaseLocalAxisSystem(Enum):
+    '''
+    Line Release Local Axis System Enumeration
+    '''
+    LOCAL_AXIS_SYSTEM_TYPE_ORIGINAL_LINE, LOCAL_AXIS_SYSTEM_TYPE_MEMBER_ON_ORIGINAL_LINE, \
+    LOCAL_AXIS_SYSTEM_TYPE_Z_AXIS_PERPENDICULAR_TO_SURFACE, E_LOCAL_AXIS_SYSTEM_TYPE_HELP_NODE= range(4)
+
+class LocalAxisSystemObjectInPlane(Enum):
+    '''
+    Line Release Local Axis System Object In Plane Enumeration
+    '''
+    LOCAL_AXIS_SYSTEM_IN_PLANE_XY, LOCAL_AXIS_SYSTEM_IN_PLANE_XZ = range(2)
+
+class PartialActivityAlongType(Enum):
+    '''
+    Partial Activity Along Type Enumeration
+    '''
+    PARTIAL_ACTIVITY_TYPE_COMPLETE, PARTIAL_ACTIVITY_TYPE_FIXED, PARTIAL_ACTIVITY_TYPE_FAILURE_FROM_FORCE, \
+    PARTIAL_ACTIVITY_TYPE_YIELDING_FROM_FORCE, PARTIAL_ACTIVITY_TYPE_INEFFECTIVNESS = range(5)
+
+class PartialActivityAroundType(Enum):
+    '''
+    Partial Activity Around Type Enumeration
+    '''
+    PARTIAL_ACTIVITY_TYPE_COMPLETE, PARTIAL_ACTIVITY_TYPE_FIXED, PARTIAL_ACTIVITY_TYPE_FAILURE_FROM_MOMENT, \
+    PARTIAL_ACTIVITY_TYPE_YIELDING_FROM_MOMENT, PARTIAL_ACTIVITY_TYPE_INEFFECTIVNESS = range(5)
+
+class LineReleaseDiagram(Enum):
+    '''
+    Line Release Diagram Type Enumeration
+    '''
+    DIAGRAM_ENDING_TYPE_CONTINUOUS, DIAGRAM_ENDING_TYPE_FAILURE, DIAGRAM_ENDING_TYPE_STOP, DIAGRAM_ENDING_TYPE_YIELDING = range(4)
+
+class LineReleaseForceMomentDiagram(Enum):
+    '''
+    Line Release Force Moment Diagram Enumeration
+    '''
+    FORCE_MOMENT_DIAGRAM_ENDING_TYPE_CONTINUOUS, FORCE_MOMENT_DIAGRAM_ENDING_TYPE_FAILURE, FORCE_MOMENT_DIAGRAM_ENDING_TYPE_YIELDING = range(3)
+
+class LineReleaseForceMomentDepend(Enum):
+    '''
+    Line Release Force Moment Depend Enumeration
+    '''
+    FORCE_MOMENT_DIAGRAM_DEPENDS_ON_N, FORCE_MOMENT_DIAGRAM_DEPENDS_ON_VY, FORCE_MOMENT_DIAGRAM_DEPENDS_ON_VZ = range(3)
+
+class LineReleaseReleaseLocation(Enum):
+    '''
+    Line Release Release Location Enumeration
+    '''
+    RELEASE_LOCATION_ORIGIN, RELEASE_LOCATION_RELEASED = range(2)
+
+class LoadWizardType(Enum):
+    ''''
+    Types of Loading Wizards
+    '''
+    GENERATE_LOAD_COMBINATIONS, GENERATE_RESULT_COMBINATIONS = range(2)
+
+class InitialStateDefintionType(Enum):
+    '''
+    Types of Initial States
+    '''
+    DEFINITION_TYPE_FINAL_STATE, DEFINITION_TYPE_STIFFNESS, DEFINITION_TYPE_STRAINS, DEFINITION_TYPE_STRAINS_WITH_USER_DEFINED_FACTORS = range(4)
+
+class NodalReleaseReleaseLocation(Enum):
+    '''
+    Nodal Release Release Location
+    '''
+    RELEASE_LOCATION_ORIGIN, RELEASE_LOCATION_RELEASED = range(2)
+
+class NodalReleaseTypeReleaseNonlinearity(Enum):
+    '''
+    Nodal Release Type Release Nonlinearity
+    '''
+    NONLINEARITY_TYPE_DIAGRAM, NONLINEARITY_TYPE_FAILURE_ALL_IF_NEGATIVE, NONLINEARITY_TYPE_FAILURE_ALL_IF_POSITIVE, \
+    NONLINEARITY_TYPE_FAILURE_IF_NEGATIVE, NONLINEARITY_TYPE_FAILURE_IF_POSITIVE, NONLINEARITY_TYPE_FORCE_MOMENT_DIAGRAM, \
+    NONLINEARITY_TYPE_FRICTION_DIRECTION_1, NONLINEARITY_TYPE_FRICTION_DIRECTION_1_2, NONLINEARITY_TYPE_FRICTION_DIRECTION_1_PLUS_2,\
+    NONLINEARITY_TYPE_FRICTION_DIRECTION_2, NONLINEARITY_TYPE_NONE, NONLINEARITY_TYPE_PARTIAL_ACTIVITY,\
+    NONLINEARITY_TYPE_STIFFNESS_DIAGRAM = range(13)
+
+class NodalReleaseTypeDiagram(Enum):
+    '''
+    Nodal Release Type Diagram
+    '''
+    DIAGRAM_ENDING_TYPE_CONTINUOUS, DIAGRAM_ENDING_TYPE_FAILURE, DIAGRAM_ENDING_TYPE_STOP, \
+    DIAGRAM_ENDING_TYPE_YIELDING = range(4)
+
+class NodalReleaseTypePartialActivityAlong(Enum):
+    '''
+    Nodal Release Type Partial Activity Along
+    '''
+    PARTIAL_ACTIVITY_TYPE_COMPLETE, PARTIAL_ACTIVITY_TYPE_FAILURE_FROM_FORCE, PARTIAL_ACTIVITY_TYPE_FIXED, \
+    PARTIAL_ACTIVITY_TYPE_INEFFECTIVNESS, PARTIAL_ACTIVITY_TYPE_YIELDING_FROM_FORCE = range(5)
+
+class NodalReleaseTypePartialActivityAround(Enum):
+    '''
+    Nodal Release Type Partial Activity Around
+    '''
+    PARTIAL_ACTIVITY_TYPE_COMPLETE, PARTIAL_ACTIVITY_TYPE_FAILURE_FROM_MOMENT, PARTIAL_ACTIVITY_TYPE_FIXED, \
+    PARTIAL_ACTIVITY_TYPE_INEFFECTIVNESS, PARTIAL_ACTIVITY_TYPE_YIELDING_FROM_MOMENT = range(5)
+
+class NodalReleaseTypeLocalAxisSystemObjectType(Enum):
+    '''
+    Nodal Release Type Local Axis System Object Type
+    '''
+    LOCAL_AXIS_SYSTEM_OBJECT_TYPE_LINE, LOCAL_AXIS_SYSTEM_OBJECT_TYPE_MEMBER = range(2)
+
+class MaterialModel(Enum):
+    '''
+    Types of Material Models
+    '''
+    MODEL_ISOTROPIC_DAMAGE_2D_3D, MODEL_ISOTROPIC_LINEAR_ELASTIC, MODEL_ISOTROPIC_MASONRY_PLASTIC_2D,MODEL_ISOTROPIC_NONLINEAR_ELASTIC_1D, MODEL_ISOTROPIC_NONLINEAR_ELASTIC_2D_3D, MODEL_ISOTROPIC_PLASTIC_1D, MODEL_ISOTROPIC_PLASTIC_2D_3D,MODEL_ISOTROPIC_SOIL_NONLINEAR_ELASTIC_3D,  MODEL_ISOTROPIC_SOIL_PLASTIC_3D, \
+    MODEL_ISOTROPIC_TIMBER_LINEAR_ELASTIC_MEMBERS, MODEL_ORTHOTROPIC_2D, MODEL_ORTHOTROPIC_3D, MODEL_ORTHOTROPIC_MASONRY_PLASTIC_2D,MODEL_ORTHOTROPIC_PLASTIC_2D, MODEL_ORTHOTROPIC_PLASTIC_3D, MODEL_ORTHOTROPIC_TIMBER_LINEAR_ELASTIC_SURFACES = range(16)
+
+class ThicknessIntegrationMethod(Enum):
+    '''
+    Types of Integration Methods
+    '''
+    INTEGRATION_METHOD_TYPE_GAUSS_LOBATTO_QUADRATURE, INTEGRATION_METHOD_TYPE_SIMPSONS_RULE, INTEGRATION_METHOD_TYPE_TRAPEZOIDAL_RULE = range(3)
+
+class MemberShearPanelDefinitionType(Enum):
+    '''
+    Member Shear Panel Definition Type
+    '''
+    DEFINITION_TYPE_BRACING, DEFINITION_TYPE_DEFINE_S_PROV, DEFINITION_TYPE_TRAPEZOIDAL_SHEETING, DEFINITION_TYPE_TRAPEZOIDAL_SHEETING_AND_BRACING = range(4)
+
+class MemberShearPanelFasteningArrangement(Enum):
+    '''
+    Member Shear Panel Fastening Arrangement
+    '''
+    FASTENING_ARRANGEMENT_EVERY_RIB, FASTENING_ARRANGEMENT_EVERY_SECOND_RIB = range(2)
+
+class MemberShearPanelPositionOnSection(Enum):
+    '''
+    Member Shear Panel Position On Section
+    '''
+    POSITION_DEFINE, POSITION_IN_CENTROID, POSITION_ON_LOWER_FLANGE, POSITION_ON_UPPER_FLANGE = range(4)
+
+class MemberRotationalRestraintSheetingPosition(Enum):
+    '''
+    Member Rotational Restraint Position of Sheeting
+    '''
+    SHEETING_POSITION_NEGATIVE, SHEETING_POSITION_POSITIVE = range(2)
+
+class MemberRotationalRestraintRotationalStiffness(Enum):
+    '''
+    Member Rotational Restraint Rotational Stiffness
+    '''
+    ROTATIONAL_STIFFNESS_INFINITELY, ROTATIONAL_STIFFNESS_MANUALLY = range(2)
+
+class MemberRotationalRestraintType(Enum):
+    '''
+    Member Rotational Restraint Type
+    '''
+    TYPE_CONTINUOUS, TYPE_DISCRETE, TYPE_MANUALLY = range(3)
+
+class MemberRotationalRestraintContinousBeamEffect(Enum):
+    '''
+    Member Rotational Restraint Continous Beam Effect
+    '''
+    CONTINUOUS_BEAM_EFFECT_END_PANEL, CONTINUOUS_BEAM_EFFECT_INTERNAL_PANEL = range(2)
+
+class ModelHistoryStatusType(Enum):
+    '''
+    Model History Status Type Enumeration
+    '''
+    E_HISTORY_RECORD_STATUS_CREATED, E_HISTORY_RECORD_STATUS_MODIFIED, E_HISTORY_RECORD_STATUS_VERSIONED = range(3)
+
+class ModelLocationRowType(Enum):
+    '''
+    Model Location Row Type Enumeration
+    '''
+    E_ROW_ALTITUDE, E_ROW_CITY, E_ROW_COUNTRY_ISO, E_ROW_LATITUDE, E_ROW_LONGITUDE, E_ROW_STATE, E_ROW_STREET, E_ROW_ZIP = range(8)
+
+class NoteType(Enum):
+    '''
+    Note Type Enumeration
+    '''
+    NOTE_TYPE_MEMBER, NOTE_TYPE_NODE, NOTE_TYPE_POINT = range(3)
+
+class NoteOffsetType(Enum):
+    '''
+    Note Offset Type Enumeration
+    '''
+    OFFSET_TYPE_XY, OFFSET_TYPE_XYZ, OFFSET_TYPE_XZ, OFFSET_TYPE_YZ = range(4)
+
+class NoteMemberReferenceType(Enum):
+    '''
+    Note Member Reference Type Enumeration
+    '''
+    REFERENCE_TYPE_L, REFERENCE_TYPE_XY, REFERENCE_TYPE_XZ, REFERENCE_TYPE_YZ = range(4)
+
+class NoteSurfaceReferenceType(Enum):
+    '''
+    Note Surface Reference Type Enumeration
+    '''
+    OFFSET_TYPE_XY, OFFSET_TYPE_XZ, OFFSET_TYPE_YZ = range(3)
```

### Comparing `RSTAB-1.5.0/RSTAB/formula.py` & `RSTAB-1.6.0/RSTAB/formula.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/globalParameter.py` & `RSTAB-1.6.0/RSTAB/globalParameter.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB/initModel.py` & `RSTAB-1.6.0/RSTAB/initModel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import sys
-import RSTAB.dependencies
+import RSTAB.dependencies # dependency check ahead of imports
 import socket
 import requests
 from suds.client import Client
 from RSTAB.enums import ObjectTypes, ModelType, AddOn
 from RSTAB.suds_requests import RequestsTransport
+from suds.cache import DocumentCache
+from tempfile import gettempdir
 
 # Connect to server
 # Check server port range set in "Program Options & Settings"
 # By default range is set between 8081 ... 8089
 print('Connecting to server...')
 
 # local machine url format: 'http://127.0.0.1'
@@ -31,15 +33,16 @@
     print('Please check:')
     print('- If you have started RSTAB application at the remote destination correctly.')
     a_socket.close()
     sys.exit()
 
 # Check for issues locally and remotely
 try:
-    client = Client(urlAndPort+'/wsdl', location = urlAndPort)
+    ca = DocumentCache(location=os.path.join(gettempdir(), 'WSDL'))
+    client = Client(urlAndPort+'/wsdl', location = urlAndPort, cache=ca)
 except:
     print('Error: Connection to server failed!')
     print('Please check:')
     print('- If you have started RSTAB application')
     print('- If all RSTAB dialogs are closed')
     print('- If server port range is set correctly')
     print('- If you have a valid Web Services license')
@@ -52,22 +55,18 @@
     modelLst = client.service.get_model_list()
 except:
     print('Error: Please check if all RSTAB dialogs are closed.')
     input('Press Enter to exit...')
     sys.exit()
 
 # Persistent connection
-# Next 4 lines enables Client to work within 1 session which is much faster to execute.
+# 'session' and 'trans'(port) enable Client to work within 1 session which is much faster to execute.
 # Without it the session lasts only one request which results in poor performance.
 # Assigning session to application Client (here client) instead of model Client
 # results also in poor performance.
-session = requests.Session()
-adapter = requests.adapters.HTTPAdapter(pool_connections=1, pool_maxsize=1)
-session.mount('http://', adapter)
-trans = RequestsTransport(session)
 
 class Model():
     clientModel = None
     clientModelDct = {}
 
     def __init__(self,
                  new_model: bool=True,
@@ -90,63 +89,79 @@
         modelLst = []
         modelVct = client.service.get_model_list()
         if modelVct:
             modelLst = modelVct.name
 
         # The model suffix is omitted in modelLs, so it must be omitted in model_name to match exactly
         original_model_name = model_name
-        if '.rs9' in model_name:
-            model_name = model_name[:-4]
+        if '.' in model_name:
+            model_name = model_name.split('.')[0]
 
         if new_model:
             # Requested new model but the model with given name was already connected
             if model_name in self.clientModelDct:
                 cModel = self.clientModelDct[model_name]
                 cModel.service.delete_all_results()
                 cModel.service.delete_all()
 
             # Requested new model, model with given name DOESN'T exist yet
             else:
                 modelPath = ''
                 # Requested new model, model with given name was NOT connected yet but file with the same name was opened
                 if model_name in modelLst:
-                    id = 0
-                    for i,j in enumerate(modelLst):
-                        if modelLst[i] == model_name:
-                            id = i
+                    id = modelLst.index(model_name)
                     modelPath =  client.service.get_model(id)
                 else:
                     modelPath =  client.service.new_model(original_model_name)
                 modelPort = modelPath[-5:-1]
                 modelUrlPort = url+':'+modelPort
                 modelCompletePath = modelUrlPort+'/wsdl'
 
                 if self.clientModelDct:
-                    cModel = Client(modelCompletePath, location = modelUrlPort)
+                    cModel = Client(modelCompletePath, location = modelUrlPort, cache=ca)
                 else:
-                    cModel = Client(modelCompletePath, transport=trans, location = modelUrlPort)
+                    session = requests.Session()
+                    adapter = requests.adapters.HTTPAdapter(pool_connections=1, pool_maxsize=1)
+                    session.mount('http://', adapter)
+                    trans = RequestsTransport(session)
+
+                    cModel = Client(modelCompletePath, transport=trans, location = modelUrlPort, cache=ca)
+
                 self.clientModelDct[model_name] = cModel
 
         else:
             # Requested model which was already connected
             assert model_name in self.clientModelDct or model_name in modelLst, 'WARNING: '+model_name +'is not connected neither opened in RSTAB.'
 
             if model_name in self.clientModelDct:
                 cModel = self.clientModelDct[model_name]
-            else:
+            elif model_name in modelLst:
                 id = 0
                 for i,j in enumerate(modelLst):
                     if modelLst[i] == model_name:
                         id = i
                 modelPath =  client.service.get_model(id)
                 modelPort = modelPath[-5:-1]
                 modelUrlPort = url+':'+modelPort
                 modelCompletePath = modelUrlPort+'/wsdl'
-                cModel = Client(modelCompletePath, location = modelUrlPort)
+
+                if self.clientModelDct:
+                    cModel = Client(modelCompletePath, location = modelUrlPort, cache=ca)
+                else:
+                    session = requests.Session()
+                    adapter = requests.adapters.HTTPAdapter(pool_connections=1, pool_maxsize=1)
+                    session.mount('http://', adapter)
+                    trans = RequestsTransport(session)
+
+                    cModel = Client(modelCompletePath, transport=trans, location = modelUrlPort, cache=ca)
+
                 self.clientModelDct[model_name] = cModel
+            else:
+                print('Model name "'+model_name+'" is not created in RSTAB. Consider changing new_model parameter in Model class from False to True.')
+                sys.exit()
 
             if delete:
                 print('Deleting results...')
                 cModel.service.delete_all_results()
             if delete_all:
                 print('Delete all...')
                 cModel.service.delete_all()
@@ -156,36 +171,37 @@
         # when using only one instance/model
         Model.clientModel = cModel
 
     def __delete__(self, index_or_name):
         '''
         Purpose of this function is to facilitate removing client instances
         from clientModelDct dictionary, which is held in Model for the purpose of
-        working with mustiple models either created directly in RSTAB or opened from file.
+        working with multiple models either created directly in RSTAB or opened from file.
 
         Args:
             index_or_name (str or int): Name of the index of model
         '''
         if isinstance(index_or_name, str):
             self.clientModelDct.pop(index_or_name)
             if len(self.clientModelDct) > 0:
                 model_key = list(self.clientModelDct)[-1]
                 self.clientModel = self.clientModelDct[model_key]
             else:
                 self.clientModel = None
         if isinstance(index_or_name, int):
             assert index_or_name <= len(self.clientModelDct)
             modelLs = client.service.get_model_list()
-            self.clientModelDct.pop(modelLs.name[index_or_name])
-            if len(self.clientModelDct) > 0:
-                model_key = list(self.clientModelDct)[-1]
-                self.clientModel = self.clientModelDct[model_key]
 
-            else:
-                self.clientModel = None
+            if modelLs:
+                self.clientModelDct.pop(modelLs.name[index_or_name])
+                if len(self.clientModelDct) > 0:
+                    model_key = list(self.clientModelDct)[-1]
+                    self.clientModel = self.clientModelDct[model_key]
+                else:
+                    self.clientModel = None
 
 def clearAttributes(obj):
     '''
     Clears object attributes.
     Sets all attributes to None.
 
     Args:
@@ -247,22 +263,31 @@
         client.service.close_model(index_or_name, save_changes)
 
     elif isinstance(index_or_name, str):
         if '.rs9' in index_or_name:
             index_or_name = index_or_name[:-4]
 
         modelLs = client.service.get_model_list()
-        for i,j in enumerate(modelLs.name):
-            if modelLs.name[i] == index_or_name:
-                Model.__delete__(Model, index_or_name)
-                client.service.close_model(i, save_changes)
-                continue
+        Model.__delete__(Model, index_or_name)
+        client.service.close_model(modelLs.name.index(index_or_name), save_changes)
     else:
         assert False, 'Parameter index_or_name must be int or string.'
 
+def closeAllModels(save_changes = False):
+    '''
+    Function that closes all opened models in reverse order.
+
+    Args:
+        save_changes (bool): Enable/Disable Save Changes Option
+    '''
+    modelLs = client.service.get_model_list()
+    if modelLs:
+        for j in reversed(modelLs.name):
+            closeModel(j, save_changes)
+
 def saveFile(model_path):
     '''
     This function saves a model in a .rs9 file.
 
     Args:
         index_or_name : Model Index or Name to be Close
         model_path: Path to RSTAB9 model.
@@ -286,15 +311,16 @@
     It works when executing tests individually but when running all of them
     it causes RSTAB to stuck and generates failures, which are hard to investigate.
 
     Args:
         generateXmlSolverInput (bool): Generate XML Solver Input
         model (RSTAB Class, optional): Model to be edited
     '''
-    model.clientModel.service.calculate_all(generateXmlSolverInput)
+    calculationMessages = model.clientModel.service.calculate_all(generateXmlSolverInput)
+    return calculationMessages
 
 def ConvertToDlString(s):
     '''
     The function converts strings commonly used in RSTAB so that they
     can be used In WebServices. It solved issue #4.
     Examples:
     '1,3'       -> '1 3'
@@ -329,16 +355,15 @@
                 inLst.append(str(i))
 
             inS = ' '.join(inLst)
             new_lst.append(inS)
         else:
             new_lst.append(element)
 
-    s = ' '.join(new_lst)
-    return s
+    return ' '.join(new_lst)
 
 def ConvertStrToListOfInt(st):
     """
     This function coverts string to list of integers.
     Args:
         st (str): RSTAB Common String
     """
@@ -429,14 +454,15 @@
         status (bool): in/active
 
     Analysis addOns list:
         material_nonlinear_analysis_active
         structure_stability_active
         construction_stages_active
         time_dependent_active
+        influence_lines_areas_active
         form_finding_active
         cutting_patterns_active
         torsional_warping_active
         cost_estimation_active
 
     Design addOns list:
         stress_analysis_active
@@ -446,22 +472,27 @@
         aluminum_design_active
         steel_joints_active
         timber_joints_active
         craneway_design_active
 
     Dynamic addOns list:
         modal_active
+        equivalent_lateral_forces_active
         spectral_active
         time_history_active
         pushover_active
         harmonic_response_active
 
     Special aadOns list:
         building_model_active
         wind_simulation_active
+        tower_wizard_active
+        tower_equipment_wizard_active
+        piping_active
+        air_cushions_active
         geotechnical_analysis_active
     """
 
     # this will also provide sanity check
     currentStatus = GetAddonStatus(modelClient, addOn)
     if currentStatus != status:
         addonLst = modelClient.service.get_addon_statuses()
@@ -470,50 +501,52 @@
         else:
             for listType in addonLst['__keylist__']:
                 if not isinstance(addonLst[listType], bool) and addOn.name in addonLst[listType]:
                     addonLst[listType][addOn.name] = status
 
         modelClient.service.set_addon_statuses(addonLst)
 
-def CalculateSelectedCases(loadCases: list = None, designSituations: list = None, loadCombinations: list = None, model = Model):
+def CalculateSelectedCases(loadCases: list = None, designSituations: list = None, loadCombinations: list = None,skipWarnings = True, model = Model):
     '''
     This method calculate just selected objects - load cases, designSituations, loadCombinations
 
     Args:
         loadCases (list, optional): Load Case List
         designSituations (list, optional): Design Situations List
         loadCombinations (list, optional): Load Combinations List
         model (RSTAB Class, optional): Model to be edited
     '''
-    specificObjectsToCalculate = model.clientModel.factory.create('ns0:array_of_calculate_specific_objects_elements')
+    specificObjectsToCalculate = model.clientModel.factory.create('ns0:calculate_specific_loadings')
     if loadCases:
         for loadCase in loadCases:
-            specificObjectsToCalculateLC = model.clientModel.factory.create('ns0:array_of_calculate_specific_objects_elements.element')
-            specificObjectsToCalculateLC.no = loadCase
-            specificObjectsToCalculateLC.parent_no = 0
-            specificObjectsToCalculateLC.type = ObjectTypes.E_OBJECT_TYPE_LOAD_CASE.name
-            specificObjectsToCalculate.element.append(specificObjectsToCalculateLC)
+            specificObjectsToCalculateLS = model.clientModel.factory.create('ns0:calculate_specific_loadings.loading')
+            specificObjectsToCalculateLS.no = loadCase
+            specificObjectsToCalculateLS.type = ObjectTypes.E_OBJECT_TYPE_LOAD_CASE.name
+            specificObjectsToCalculate.loading.append(specificObjectsToCalculateLS)
 
     if designSituations:
         for designSituation in designSituations:
-            specificObjectsToCalculateDS = model.clientModel.factory.create('ns0:array_of_calculate_specific_objects_elements.element')
+            specificObjectsToCalculateDS = model.clientModel.factory.create('ns0:calculate_specific_loadings.loading')
             specificObjectsToCalculateDS.no = designSituation
-            specificObjectsToCalculateDS.parent_no = 0
             specificObjectsToCalculateDS.type = ObjectTypes.E_OBJECT_TYPE_DESIGN_SITUATION.name
-            specificObjectsToCalculate.element.append(specificObjectsToCalculateDS)
+            specificObjectsToCalculate.loading.append(specificObjectsToCalculateDS)
+
 
     if loadCombinations:
         for loadCombination in loadCombinations:
-            specificObjectsToCalculateLC = model.clientModel.factory.create('ns0:array_of_calculate_specific_objects_elements.element')
-            specificObjectsToCalculateLC.no = loadCombination
-            specificObjectsToCalculateLC.parent_no = 0
-            specificObjectsToCalculateLC.type = ObjectTypes.E_OBJECT_TYPE_LOAD_CASE.name
-            specificObjectsToCalculate.element.append(specificObjectsToCalculateLC)
+            specificObjectsToCalculateCC = model.clientModel.factory.create('ns0:calculate_specific_loadings.loading')
+            specificObjectsToCalculateCC.no = loadCombination
+            specificObjectsToCalculateCC.type = ObjectTypes.E_OBJECT_TYPE_LOAD_COMBINATION.name
+            specificObjectsToCalculate.loading.append(specificObjectsToCalculateCC)
+    try:
+        calculationMessages = model.clientModel.service.calculate_specific(specificObjectsToCalculate, skipWarnings)
+    except Exception as inst:
+        calculationMessages = "Calculation was unsuccessful: " + inst.fault.faultstring
 
-    model.clientModel.service.calculate_specific_objects(specificObjectsToCalculate)
+    return calculationMessages
 
 def FirstFreeIdNumber(memType = ObjectTypes.E_OBJECT_TYPE_MEMBER, parent_no: int = 0, model = Model):
     '''
     This method returns the next available Id Number for the selected object type
 
     Args:
         memType (enum): Object Type Enumeration
@@ -550,7 +583,108 @@
     The method returns a string of the current model type.
 
     Args:
         model (RSTAB Class): Model Instance
     '''
 
     return model.clientModel.service.get_model_type()
+
+def NewModelAsCopy(old_model_name: str = '',
+                   old_model_folder: str = ''):
+    '''
+    The method creates a new model as copy from an existing model
+
+    Args:
+        old_model_name (str): Old Model Name
+        old_model_folder (str): Old Model Folder
+    '''
+
+    # Old Model Name
+    new_model_name = ''
+    if '.rf6' in old_model_name:
+        new_model_name = old_model_name[:-4] + '_copy'
+
+    else:
+         assert TypeError('Model ' + old_model_name +  ' does not exist')
+
+    old_model_path = os.path.join(old_model_folder, old_model_name)
+
+    # New Model Name
+    newModelAsCopy = client.service.new_model_as_copy(new_model_name, old_model_path)
+
+    return newModelAsCopy
+
+def GetModelMainParameters(model = Model):
+    '''
+    The method returns the main parameters of the current model.
+
+    Args:
+        model (RSTAB Class, optional): Model to be edited
+    '''
+
+    # Client Model | Get Model Main Parameters
+    return model.clientModel.service.get_model_main_parameters()
+
+def GetModelId(model = Model):
+    '''
+    This method returns model id as a string.
+
+    Args:
+        model (RSTAB Class, optional): Model to be edited
+    '''
+
+    # Client Model | Get Model ID
+    return model.clientModel.service.get_model_main_parameters().model_id
+
+def GetModelParameters(model = Model):
+    '''
+    This method retuns the parameters of the current model.
+
+    Args:
+        model (RSTAB Class, optional): Model to be edited
+    '''
+
+    # Client Model | Get Model Parameters
+    return model.clientModel.service.get_model_parameters()
+
+def GetModelSessionId(model = Model):
+    '''
+    This method returns model session id as a string.
+
+    Args:
+        model (RSTAB Class, optional): Model to be edited
+    '''
+
+    # Client Model | Get Session Id
+    return model.clientModel.service.get_session_id()
+
+def GetName():
+    '''
+    This method returns app name as a string.
+    '''
+
+    # Client Application | Get Information
+    return client.service.get_information().name
+
+def GetVersion():
+    '''
+    This method returns version as a string.
+    '''
+
+    # Client Application | Get Information
+    return client.service.get_information().version
+
+def GetLanguage():
+    '''
+    This method returns language as a string.
+    '''
+
+    # Client Application | Get Information
+    return client.service.get_information().language_name
+
+def GetAppSessionId():
+    '''
+    This method returns session id as a string.
+    '''
+
+    # Client Application | Get Session ID
+    return client.service.get_session_id()
```

### Comparing `RSTAB-1.5.0/RSTAB/suds_requests.py` & `RSTAB-1.6.0/RSTAB/suds_requests.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.5.0/RSTAB.egg-info/PKG-INFO` & `RSTAB-1.6.0/RSTAB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RSTAB
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python Framework for RSTAB9 Web Services
 Home-page: https://github.com/Dlubal-Software/RSTAB_Python_Client
 Author: Dlubal Software
 Author-email: info@dlubal.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: RSTAB Version: 1.5.0 Summary: Python Framework for
+Metadata-Version: 2.1 Name: RSTAB Version: 1.6.0 Summary: Python Framework for
 RSTAB9 Web Services Home-page: https://github.com/Dlubal-Software/
 RSTAB_Python_Client Author: Dlubal Software Author-email: info@dlubal.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Description-Content-Type: text/markdown License-File: LICENSE
 ****** [Dlubal_Software] Dlubal Software GmbH [![image](https://img.shields.io/
 twitter/follow/dlubal_en?style=social)](https://twitter.com/dlubal_en "Twitter
```

### Comparing `RSTAB-1.5.0/RSTAB.egg-info/SOURCES.txt` & `RSTAB-1.6.0/RSTAB.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 Examples/__init__.py
 RSTAB/__init__.py
+RSTAB/baseData.py
 RSTAB/baseSettings.py
 RSTAB/dataTypes.py
 RSTAB/dependencies.py
 RSTAB/enums.py
 RSTAB/formula.py
 RSTAB/globalParameter.py
 RSTAB/initModel.py
@@ -35,14 +36,15 @@
 RSTAB/Imperfections/imperfectionCase.py
 RSTAB/Imperfections/memberImperfection.py
 RSTAB/Imperfections/membersetImperfection.py
 RSTAB/ImportExport/__init__.py
 RSTAB/ImportExport/exports.py
 RSTAB/ImportExport/imports.py
 RSTAB/LoadCasesAndCombinations/__init__.py
+RSTAB/LoadCasesAndCombinations/combinationWizard.py
 RSTAB/LoadCasesAndCombinations/designSituation.py
 RSTAB/LoadCasesAndCombinations/loadCase.py
 RSTAB/LoadCasesAndCombinations/loadCasesAndCombinations.py
 RSTAB/LoadCasesAndCombinations/loadCombination.py
 RSTAB/LoadCasesAndCombinations/modalAnalysisSettings.py
 RSTAB/LoadCasesAndCombinations/resultCombination.py
 RSTAB/LoadCasesAndCombinations/spectralAnalysisSettings.py
@@ -63,50 +65,48 @@
 RSTAB/Results/__init__.py
 RSTAB/Results/designOverview.py
 RSTAB/Results/resultTables.py
 RSTAB/SpecialObjects/__init__.py
 RSTAB/SpecialObjects/nodalRelease.py
 RSTAB/SpecialObjects/structureModification.py
 RSTAB/SteelDesign/__init__.py
+RSTAB/SteelDesign/steelServiceabilityConfiguration.py
 RSTAB/SteelDesign/steelUltimateConfigurations.py
 RSTAB/TimberDesign/__init__.py
 RSTAB/TimberDesign/timberServiceLimitStateConfigurations.py
 RSTAB/TimberDesign/timberUltimateConfigurations.py
 RSTAB/Tools/GetObjectNumbersByType.py
 RSTAB/Tools/ModelCheck.py
 RSTAB/Tools/PlausibilityCheck.py
 RSTAB/Tools/__init__.py
 RSTAB/Tools/centreOfGravityAndObjectInfo.py
 RSTAB/Tools/sectionDialogue.py
 RSTAB/TypesForAluminumDesign/__init__.py
 RSTAB/TypesForAluminumDesign/aluminumEffectiveLengths.py
 RSTAB/TypesForAluminumDesign/aluminumMemberLocalSectionReduction.py
-RSTAB/TypesForAluminumDesign/aluminumMemberRotationalRestraints.py
-RSTAB/TypesForAluminumDesign/aluminumMemberShearPanel.py
+RSTAB/TypesForAluminumDesign/aluminumMemberTransverseWelds.py
 RSTAB/TypesForMembers/__init__.py
 RSTAB/TypesForMembers/memberDefinableStiffness.py
 RSTAB/TypesForMembers/memberEccentricity.py
 RSTAB/TypesForMembers/memberHinge.py
 RSTAB/TypesForMembers/memberNonlinearity.py
 RSTAB/TypesForMembers/memberResultIntermediatePoints.py
+RSTAB/TypesForMembers/memberRotationalRestraint.py
+RSTAB/TypesForMembers/memberShearPanel.py
 RSTAB/TypesForMembers/memberStiffnessModification.py
 RSTAB/TypesForMembers/memberSupport.py
 RSTAB/TypesForMembers/memberTransverseStiffeners.py
 RSTAB/TypesForNodes/__init__.py
 RSTAB/TypesForNodes/nodalSupport.py
 RSTAB/TypesForSpecialObjects/__init__.py
 RSTAB/TypesForSpecialObjects/nodalReleaseType.py
 RSTAB/TypesForSteelDesign/SteelMemberLocalSectionReduction.py
 RSTAB/TypesForSteelDesign/__init__.py
 RSTAB/TypesForSteelDesign/steelBoundaryConditions.py
 RSTAB/TypesForSteelDesign/steelEffectiveLengths.py
-RSTAB/TypesForSteelDesign/steelMemberRotationalRestraints.py
-RSTAB/TypesForSteelDesign/steelMemberShearPanel.py
 RSTAB/TypesForTimberDesign/__init__.py
 RSTAB/TypesForTimberDesign/timberEffectiveLengths.py
 RSTAB/TypesForTimberDesign/timberMemberLocalSectionReduction.py
-RSTAB/TypesForTimberDesign/timberMemberRotationalRestraint.py
-RSTAB/TypesForTimberDesign/timberMemberShearPanel.py
 RSTAB/TypesForTimberDesign/timberServiceClass.py
 RSTAB/TypesforConcreteDesign/ConcreteDurability.py
 RSTAB/TypesforConcreteDesign/ConcreteEffectiveLength.py
 RSTAB/TypesforConcreteDesign/__init__.py
```

### Comparing `RSTAB-1.5.0/setup.py` & `RSTAB-1.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent
 readme = (here/"README.md").read_text(encoding="utf-8")
 
 setup(
     name='RSTAB',
-    version='1.05.0',
+    version='1.06.0',
     description='Python Framework for RSTAB9 Web Services',
     long_description=readme,
     long_description_content_type = "text/markdown",
     url="https://github.com/Dlubal-Software/RSTAB_Python_Client",
     author="Dlubal Software",
     author_email="info@dlubal.com",
     license="MIT",
```

