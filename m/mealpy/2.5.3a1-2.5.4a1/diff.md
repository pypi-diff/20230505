# Comparing `tmp/mealpy-2.5.3a1.tar.gz` & `tmp/mealpy-2.5.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mealpy-2.5.3a1.tar", last modified: Tue Mar 21 15:12:13 2023, max compression
+gzip compressed data, was "mealpy-2.5.4a1.tar", last modified: Fri May  5 08:41:36 2023, max compression
```

## Comparing `mealpy-2.5.3a1.tar` & `mealpy-2.5.4a1.tar`

### file list

```diff
@@ -1,175 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:12:13.465481 mealpy-2.5.3a1/
--rw-r--r--   0 runner    (1001) docker     (123)    57487 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    90293 2023-03-21 15:12:13.465481 mealpy-2.5.3a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    87752 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:12:13.433481 mealpy-2.5.3a1/mealpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:12:13.437481 mealpy-2.5.3a1/mealpy/bio_based/
--rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/bio_based/BBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/bio_based/BBOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/bio_based/BMO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/bio_based/EOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/bio_based/IWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/bio_based/SBO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/bio_based/SMA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/bio_based/SOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/bio_based/SOS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/bio_based/TPO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/bio_based/TSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    11744 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/bio_based/VCS.py
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/bio_based/WHO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/bio_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:12:13.437481 mealpy-2.5.3a1/mealpy/evolutionary_based/
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/evolutionary_based/CRO.py
--rw-r--r--   0 runner    (1001) docker     (123)    40520 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/evolutionary_based/DE.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/evolutionary_based/EP.py
--rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/evolutionary_based/ES.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/evolutionary_based/FPA.py
--rw-r--r--   0 runner    (1001) docker     (123)    38686 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/evolutionary_based/GA.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/evolutionary_based/MA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/evolutionary_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:12:13.441481 mealpy-2.5.3a1/mealpy/human_based/
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/BRO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/BSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/CA.py
--rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/CHIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/FBIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/GSKA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/HBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/HCO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/ICA.py
--rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/LCO.py
--rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/QSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/SARO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/SPBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/SSDO.py
--rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/TLO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/TOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/WarSO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/human_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:12:13.445481 mealpy-2.5.3a1/mealpy/math_based/
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/math_based/AOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/math_based/CEM.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/math_based/CGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/math_based/CircleSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/math_based/GBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/math_based/HC.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/math_based/INFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/math_based/PSS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/math_based/RUN.py
--rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/math_based/SCA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/math_based/SHIO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/math_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/multitask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:12:13.445481 mealpy-2.5.3a1/mealpy/music_based/
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/music_based/HS.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/music_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32769 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:12:13.445481 mealpy-2.5.3a1/mealpy/physics_based/
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/ASO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/ArchOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/CDO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/EFO.py
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/EO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/EVO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/FLA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/HGSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/MVO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/NRO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/RIME.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/SA.py
--rw-r--r--   0 runner    (1001) docker     (123)    20823 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/TWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/WDO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/physics_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:12:13.461481 mealpy-2.5.3a1/mealpy/swarm_based/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/ABC.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/ACOR.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/AGTO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/ALO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/AO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/ARO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/AVOA.py
--rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/BA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/BES.py
--rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/BFO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/BSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    17152 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/BeesA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/COA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/CSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/CSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/CoatiOA.py
--rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/DMOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/DO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/EHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/ESOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/FA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/FFA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/FFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/FOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/FOX.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/GJO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/GOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/GTO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/GWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/HBA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/HGS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/HHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/JA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/MFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/MGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/MPA.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/MRFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/MSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/NGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/NMRA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/OOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/PFA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/POA.py
--rw-r--r--   0 runner    (1001) docker     (123)    27340 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/PSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/SCSO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/SFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/SHO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/SLO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/SRSR.py
--rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/SSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/SSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/SSpiderA.py
--rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/SSpiderO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/STO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/SeaHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/ServalOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/TDO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/TSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/WOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/WaOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/ZOA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/swarm_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:12:13.461481 mealpy-2.5.3a1/mealpy/system_based/
--rw-r--r--   0 runner    (1001) docker     (123)    28103 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/system_based/AEO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/system_based/GCO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/system_based/WCA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/system_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13359 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:12:13.461481 mealpy-2.5.3a1/mealpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/utils/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/utils/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/utils/termination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:12:13.465481 mealpy-2.5.3a1/mealpy/utils/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/utils/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/mealpy/utils/visualize/linechart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:12:13.433481 mealpy-2.5.3a1/mealpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    90293 2023-03-21 15:12:13.000000 mealpy-2.5.3a1/mealpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-03-21 15:12:13.000000 mealpy-2.5.3a1/mealpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:12:13.000000 mealpy-2.5.3a1/mealpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-21 15:12:13.000000 mealpy-2.5.3a1/mealpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-21 15:12:13.000000 mealpy-2.5.3a1/mealpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 15:12:13.465481 mealpy-2.5.3a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:12:13.465481 mealpy-2.5.3a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-03-21 15:09:26.000000 mealpy-2.5.3a1/tests/test_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.563960 mealpy-2.5.4a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    57633 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    90608 2023-05-05 08:41:36.563960 mealpy-2.5.4a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    88069 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.543960 mealpy-2.5.4a1/mealpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.543960 mealpy-2.5.4a1/mealpy/bio_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/BBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/BBOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/BMO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/EOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/IWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/SBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/SMA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/SOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/SOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/TPO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/TSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11744 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/VCS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/WHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.547960 mealpy-2.5.4a1/mealpy/evolutionary_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/CRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40520 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/DE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/EP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/ES.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/FPA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38686 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/GA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/MA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.547960 mealpy-2.5.4a1/mealpy/human_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/BRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/BSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/CA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/CHIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/FBIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/GSKA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/HBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/HCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/ICA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/ILA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/LCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/QSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/SARO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/SPBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/SSDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/TLO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/TOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/WarSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.551960 mealpy-2.5.4a1/mealpy/math_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/AOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/CEM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/CGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/CircleSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/GBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/HC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/INFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/PSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/RUN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/SCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/SHIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/multitask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.551960 mealpy-2.5.4a1/mealpy/music_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/music_based/HS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/music_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32769 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.551960 mealpy-2.5.4a1/mealpy/physics_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/ASO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/ArchOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/CDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/EFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/EO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/EVO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/FLA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/HGSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/MVO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/NRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/RIME.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/SA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20823 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/TWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/WDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.559960 mealpy-2.5.4a1/mealpy/swarm_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/ABC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/ACOR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/AGTO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/ALO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/AO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/ARO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/AVOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/BA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/BES.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/BFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/BSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17152 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/BeesA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/COA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/CSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/CSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/CoatiOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/DMOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/DO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/EHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/ESOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/FA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/FFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/FFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/FOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/FOX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/GJO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/GOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19661 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/GTO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/GWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/HBA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/HGS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/HHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/JA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/MFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/MGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/MPA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/MRFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/MSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/NGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/NMRA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/OOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/PFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/POA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27340 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/PSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SCSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14771 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SLO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SRSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SSpiderA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SSpiderO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/STO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SeaHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/ServalOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/TDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/TSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/WOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/WaOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/ZOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.559960 mealpy-2.5.4a1/mealpy/system_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    28103 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/system_based/AEO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/system_based/GCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/system_based/WCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/system_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.563960 mealpy-2.5.4a1/mealpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/termination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.563960 mealpy-2.5.4a1/mealpy/utils/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/visualize/linechart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.543960 mealpy-2.5.4a1/mealpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    90608 2023-05-05 08:41:36.000000 mealpy-2.5.4a1/mealpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-05 08:41:36.000000 mealpy-2.5.4a1/mealpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:41:36.000000 mealpy-2.5.4a1/mealpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 08:41:36.000000 mealpy-2.5.4a1/mealpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 08:41:36.000000 mealpy-2.5.4a1/mealpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:41:36.563960 mealpy-2.5.4a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.563960 mealpy-2.5.4a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/tests/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/tests/test_tuner.py
```

### Comparing `mealpy-2.5.3a1/ChangeLog.md` & `mealpy-2.5.4a1/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,39 @@
   * 2.0.0 <= mealpy <= 2.1.2
   * mealpy == 2.2.0 
   * mealpy == 2.3.0 
   * 2.4.0 <= mealpy <= 2.4.2 (From this version, algorithms can solve discrete problem)
   * mealpy >= 2.5.1 (Define model 1 time, solve multiple problems)
 
 
+# Version 2.5.4
+
+### Update
++ Update the parameter's order in Tuner class  
++ Update the saving's bug when using Termination in Multitask
+
+
+
+
+# Version 2.5.3
+
+### Update 
++ Fix bug in roulette-wheel-selection in Optimizer
++ Update multitask with input modes and terminations
++ Update Tuner with more input parameters
++ Add Lévy flight, and the selective opposition version of the artificial rabbit algorithm (LARO)
++ Add Modified Gorilla Troops Optimization (MGTO)
++ Update Giant Trevally Optimizer as requested by the authors
+  + Matlab101GTO: This version was used to produce the results presented in the paper.
+  + Matlab102GTO: This is a new version provided by the authors (Matlab link), which has been updated recently to 
+    reduce computation time.
+  + OriginalGTO: This version is implemented exactly as described in the paper.
+
+
+
 
 
 # Version 2.5.2
 
 ### Update
 
 + Fixed bug all fitness values are equals in function "get index roulette wheel selection" in Optimizer class
@@ -66,15 +91,15 @@
   + Add Golden jackal optimization (GJO)
     + Ref: Golden jackal optimization: A novel nature-inspired optimizer for engineering applications
   + Add Fox Optimizer (FOX)
     + Ref: FOX: a FOX-inspired optimization algorithm
   + Add Giant Trevally Optimizer (GTO)
     + Ref: Giant Trevally Optimizer (GTO): A Novel Metaheuristic Algorithm for Global Optimization and Challenging Engineering Problems
     
-+ **Warning**: The list of all algorithms below we should avoid to use it
++ **Warning**: Please check the original paper before you want to use these algorithms.
   + Add Zebra Optimization Algorithm (ZOA)
     + Ref: Zebra Optimization Algorithm: A New Bio-Inspired Optimization Algorithm for Solving Optimization Algorithm
   + Add Osprey Optimization Algorithm (OOA)
     + Ref: Osprey optimization algorithm: A new bio-inspired metaheuristic algorithm for solving engineering optimization problems
   + Add Coati Optimization Algorithm (CoatiOA)
     + Ref: Coati Optimization Algorithm: A New Bio-Inspired Metaheuristic Algorithm for Solving Optimization Problems
   + Add Pelican Optimization Algorithm (POA)
@@ -90,20 +115,15 @@
   + Add Tasmanian Devil Optimization (TDO)
     + Ref: Tasmanian devil optimization: a new bio-inspired optimization algorithm for solving optimization algorithm
   + Add Fennec Fox Optimization (FFO)
     + Ref: Fennec Fox Optimization: A New Nature-Inspired Optimization Algorithm
   + Add Teamwork Optimization Algorithm (TOA)
     + Ref: Teamwork Optimization Algorithm: A New Optimization Approach for Function Minimization/Maximization
 
-+ **Notes on plagiarism and fake algorithm:**
-    + OOA and STO with the same exact code 
-    + POA ServalOA, NGO, WaOA, and TDO with almost the same exact code 
-    + ZOA and CoatiOA with almost the same exact code 
-    + FFO is swap two phases of POA
-    + TOA is kinda same as OOA and POA 
+
 
 
 ---------------------------------------------------------------------
 
 
 # Version 2.5.1
 
@@ -625,51 +645,42 @@
         + Check bound and update fitness after each individual move instead of after the whole population move in the original version
         + My version not only faster but also better
         
 + Added Spotted Hyena Optimizer (SHO) to swarm_based group:
     + OriginalSHO: my modified version
 
        
-+ Add category for fake algorithms (papers) and proofs: 
++ Add category for questionable algorithm or papers (called fake): 
     + Butterfly Optimization Algorithm (BOA) to swarm_based group:
-        + OriginalBOA: this is fake algorithm 
+        + OriginalBOA: this algorithm is made up one 
         + AdaptiveBOA:
         + BaseBOA:
-            + Look at this guy (the author of this algorithm):
+            + Look at the author of this algorithm
             + https://scholar.google.co.in/citations?hl=en&user=KvcHovcAAAAJ&view_op=list_works&sortby=pubdate
-            + He invent BOA algorithm and public it in 2019, but so many variant version of BOA has been created since 2015.
-            + How the hell that happened?
-            + This is a plagiarism? I think this is one of the most biggest reason why mathematician researchers
-             calling out meta-heuristics community is completely bullshit and unethical.
-            + Just for producing more trash paper without any knowledge in it? This is why I listed BOA as the totally
-             trash and fake
+            + It is interesting to note that there have been many variant versions of BOA created since 2015, even though the inventor of BOA only published it in 2019. This raises some questions about the origins of these variant algorithms and how they came to be.
              
     + Sandpiper Optimization Algorithm (SOA) to swarm_based group:
-        + OriginalSOA: the original version is fake
-            + This algorithm is trash, unethical when summit a paper to 2 journals.
-            + Can't even update its position.
+        + OriginalSOA: the original version is made up one
+            + This algorithm suffers from local optimal and lower convergence rate. 
+            + It cannot update the position, so how to converge without update position?
+            + I am curious about the algorithm's publication history, as I have found it submitted to multiple journals.
             + A detailed explain in this comment section 
             (https://www.researchgate.net/publication/334897831_Sandpiper_optimization_algorithm_a_novel_approach_for_solving_real-life_engineering_problems/comments)
         + BaseSOA: my modified version which changed some equations and flow.
         
     + Sooty Tern Optimization Algorithm (STOA) is another name of Sandpiper Optimization Algorithm (SOA) 
-        + Amandeep Kaur, Sushma Jain, Shivani Goel,  Gaurav Dhiman. What they are doing are plagiarism, uneducated
-         and unethical to meta-heuristics community.
+        + If you read the paper, you will see the similarity between these two 
     
     + Blue Monkey Optimization (BMO) to swarm_based group:
-        + OriginalBMO: the original version is fake 
-            + The idea look like "Chicken Swarm Optimization"
-            + The pseudo-code totally bullshit in my opinion, just read the paper you will understand.
-            + The unclear point here is the "Rate equation": really confuse because It's contain the position. As you know,
-                The position is the vector, but finally, the author conclude that Rate is random number in range [0, 1]
-                Luckily, using number we can plus/add number and vector or vector and vector.
-                So at first, Rate is random number then after the 1st loop, its become vector. 
-            + Morever, both equtions movement of blue monkey and children is the same.
-            + In addition, they don't check the bound after update position.
-            + Keep going, they don't tell you the how to find the global best (I mean from blue monkey group or child group)
+        + OriginalBMO: 
+            + It is a made-up algorithm with a similar idea to "Chicken Swarm Optimization," which raises questions about its originality.
+            + The pseudo-code is confusing, particularly the "Rate equation," which starts as a random number and then becomes a vector after the first loop. 
+            + The movement of the blue monkey and children is the same equations???
+            + The algorithm does not check the bound after updating the position, which can cause issues with the search space.
+            + The algorithm does not provide guidance on how to find the global best from the blue monkey group or child group.
         + BaseBMO: my modified version which used my knowledge about meta-heuristics to do it. 
 
 
 ### Change others
 + models_history.csv: Update history of meta-heuristic algorithms        
 + examples: 
     + Update and Add examples for all algorithms
@@ -729,17 +740,17 @@
         + Remove all third loop, n-times faster than original
         + No need equation (1, 2) in the paper, calculate the probability by roulette-wheel. Also can handle negative values
         + Apply batch-size idea
     + BaseBWO (BWO): This is my changed version and worked. 
         + Using k-way tournament selection to select parent instead of randomizing
         + Repeat cross-over population_size / 2 instead of n_var/2
         + Mutation 50% of position instead of swap only 2 variable in a single position
-        + OriginalBWO: is fake and just a variant of Genetic Algorithm
+        + OriginalBWO: is made up algorithm and just a variant of Genetic Algorithm
     + BaseAAA (AAA): This is my changed version but still not working
-        + OriginalAAA: is fake taken from DE and CRO 
+        + OriginalAAA: is made up algorithm taken from DE and CRO 
         + I realize in the original paper, parameters, and equations not clear.
         + In the Adaptation phase, what is the point of saving starving value when it doesn't affect the solution at all?
         + The size of the solution always = 2/3, so the friction surface will always stay at the same value.
         + The idea of the equation seems like taken from DE, the adaptation and reproduction process seem like taken from CRO.
         + Appearance from 2015, but still now 2020 none of Matlab code or python code about this algorithm.
     + EOA: 
         + OriginalEOA: My modified version from original Matlab version
@@ -844,15 +855,15 @@
     + FA:
         + OriginalFA: is the original version, running slow even the all third loop already removed
     + BA:
         + OriginalBA: is the original version 
         + BasicBA: is also the original version with improved parameters
         + AdaptiveBA: my modified version without A parameter
     + PIO: 
-        + This is fake algorithm, after changing almost everything, the algorithm works
+        + This is made up algorithm, after changing almost everything, the algorithm works
         + BasePIO: My base version
         + LevyPIO: My version based on levy-flight for large-scale dimensions
     + GWO:
         + OriginalGWO: is the original version
     + ALO:
         + OriginalALO: is the original version, slow and less efficient
         + BaseALO: my modified version which using matrix multiplication for faster 
@@ -919,15 +930,15 @@
             + Reform Energy equation,
             + No need parameter A and epxilon
             + Based on idea of Opposition-based Learning
     + SLO:
         + OriginalSLO: is the changed version from my student
         + ImprovedSLO: is the improved version 
     + SpaSA:
-        + BaseSpaSA: is my modified version, the original paper is fake, tons of unclear like parameters or equations
+        + BaseSpaSA: is my modified version, the original paper has several unclear parameters and equations
     + MRFO:
         + OriginalMRFO: is the original version
         + LevyMRFO: is my modified version based on levy-flight
     + HHO:
         + OriginalHHO: is the original version 
     + SSA:
         + OriginalSSA: is the original version
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mealpy-2.5.3a1/LICENSE` & `mealpy-2.5.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/PKG-INFO` & `mealpy-2.5.4a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mealpy
-Version: 2.5.3a1
-Summary: MEALPY: A Framework Of The State-Of-The-Art Meta-Heuristic Algorithms In Python
+Version: 2.5.4a1
+Summary: MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python
 Home-page: https://github.com/thieu1995/mealpy
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mealpy.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mealpy
 Project-URL: Bug Tracker, https://github.com/thieu1995/mealpy/issues
@@ -38,20 +38,24 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-<p align="center"><img src="https://thieu1995.github.io/post/2022-04/19-mealpy-tutorials/mealpy1.png" alt="MEALPY"/></p>
+<p align="center">
+<img style="height:400px;" 
+src="https://thieu1995.github.io/post/2022-04/19-mealpy-tutorials/mealpy5-nobg.png" 
+alt="MEALPY"/>
+</p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-2.5.2-yellow.svg)](https://github.com/thieu1995/mealpy/releases)
+[![GitHub release](https://img.shields.io/badge/release-2.5.3-yellow.svg)](https://github.com/thieu1995/mealpy/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mealpy) 
 [![PyPI version](https://badge.fury.io/py/mealpy.svg)](https://badge.fury.io/py/mealpy)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mealpy.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mealpy.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mealpy.svg)
 [![Downloads](https://pepy.tech/badge/mealpy)](https://pepy.tech/project/mealpy)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mealpy/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mealpy/actions/workflows/publish-package.yaml)
@@ -66,15 +70,15 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 MEALPY is the largest python library for most of the cutting-edge nature-inspired meta-heuristic algorithms (population-based). Population meta-heuristic algorithms (PMA) are the most popular algorithms in the field of 
 approximate optimization.
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Total algorithms**: 172 (102 original, 45 official variants, 25 developed variants)
+* **Total algorithms**: 174 (102 original, 45 official variants, 27 developed variants)
 * **Documentation:** https://mealpy.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
 * **Dependencies:** numpy, scipy, pandas, matplotlib
 
 
 # Goals
 
@@ -90,15 +94,15 @@
 
 
 # Installation
 
 ### Install with pip
 Install the [current PyPI release](https://pypi.python.org/pypi/mealpy):
 ```sh 
-$ pip install mealpy==2.5.2
+$ pip install mealpy==2.5.3
 ```
 
 ### Install from source
 In case you want to install directly from the source code, use:
 ```sh 
 $ git clone https://github.com/thieu1995/mealpy.git
 $ cd mealpy
@@ -223,19 +227,25 @@
 paras_bbo_grid = {
     "epoch": [100],
     "pop_size": [50],
     "elites": [2, 3, 4, 5],
     "p_m": [0.01, 0.02, 0.05, 0.1, 0.15, 0.2]
 }
 
+term = {
+  "max_fe": 10000
+}
+
 if __name__ == "__main__":
     model = BBO.BaseBBO()
 
     tuner = Tuner(model, paras_bbo_grid)
-    tuner.execute(problem=problem, n_trials=10, mode="parallel", n_workers=4)
+    tuner.execute(problem=problem, termination=term, n_trials=5, n_jobs=5, mode="thread", n_workers=4, verbose=True)
+    ## Solve this problem 5 times (n_trials) using 5 processes (n_jobs), each process will handle 1 trial. 
+    ## The mode to run the solver is thread (mode), we will calculate the fitness of 4 solutions (n_workers) at the same time 
 
     print(tuner.best_score)
     print(tuner.best_params)
     print(tuner.best_algorithm)
     print(tuner.best_algorithm.get_name())
     
     ## Save results to csv file 
@@ -306,20 +316,24 @@
 
 ## Define models
 
 model1 = BBO.BaseBBO(epoch=10, pop_size=50)
 model2 = BBO.OriginalBBO(epoch=10, pop_size=50)
 model3 = DE.BaseDE(epoch=10, pop_size=50)
 
+## Define termination if needed
+term = {
+    "max_fe": 10000
+}
 
 ## Define and run Multitask
-
 if __name__ == "__main__":
-    multitask = Multitask(algorithms=(model1, model2, model3), problems=(p1, p2, p3))
-    multitask.execute(n_trials=3, mode="parallel", n_workers=6, save_path="history", save_as="csv", save_convergence=True, verbose=True)
+    multitask = Multitask(algorithms=(model1, model2, model3), problems=(p1, p2, p3), terminations=(term, ), modes=("thread", ))
+    # default modes = "single", default termination = epoch (as defined in problem dictionary)
+    multitask.execute(n_trials=5, n_jobs=5, save_path="history", save_as="csv", save_convergence=False, verbose=False)
     
     ## Check the directory: history/, you will see list of .csv result files
 ```
 
 For more usage examples please look at [examples](/examples) folder.
 
 More advanced examples can also be found in the [Mealpy-examples repository](https://github.com/thieu1995/mealpy_examples).
@@ -398,23 +412,20 @@
 We share lots of information, questions, and answers there. You will get more support and knowledge there.
 
 ### Cite Us
 
 If you are using mealpy in your project, we would appreciate citations:
 
 ```bibtex 
-@software{nguyen_van_thieu_2022_6684223,
-  author       = {Nguyen Van Thieu and Seyedali Mirjalili},
-  title        = {{MEALPY: a Framework of The State-of-The-Art Meta-Heuristic Algorithms in Python}},
-  month        = jun,
-  year         = 2022,
-  publisher    = {Zenodo},
-  version      = {v2.4.2},
-  doi          = {10.5281/zenodo.6684223},
-  url          = {https://doi.org/10.5281/zenodo.6684223}
+@article{van2023mealpy,
+  title={MEALPY: An open-source library for latest meta-heuristic algorithms in Python},
+  author={Van Thieu, Nguyen and Mirjalili, Seyedali},
+  journal={Journal of Systems Architecture},
+  year={2023},
+  publisher={Elsevier}
 }
 
 @article{van2023groundwater,
   title={Groundwater level modeling using Augmented Artificial Ecosystem Optimization},
   author={Van Thieu, Nguyen and Barma, Surajit Deb and Van Lam, To and Kisi, Ozgur and Mahesha, Amai},
   journal={Journal of Hydrology},
   volume={617},
@@ -495,15 +506,15 @@
     + Physics-based: Idea from physics law such as Newton's law of universal gravitation, black hole, multiverse 
     + Human-based: Idea from human interaction such as queuing search, teaching learning, ... 
     + Biology-based: Idea from biology creature (or microorganism),...
     + System-based: Idea from eco-system, immune-system, network-system, ...
     + Math-based: Idea from mathematical form or mathematical law such as sin-cosin 
     + Music-based: Idea from music instrument
 
-* Difficulty - Difficulty Level (Personal Opinion): Objective observation from author. Depend on the number of 
+* Difficulty - Difficulty Level (Personal Opinion): **Objective observation from author**. Depend on the number of 
   parameters, number of equations, the original ideas, time spend for coding, source lines of code (SLOC).
     + Easy: A few paras, few equations, SLOC very short
     + Medium: more equations than Easy level, SLOC longer than Easy level
     + Hard: Lots of equations, SLOC longer than Medium level, the paper hard to read.
     + Hard* - Very hard: Lots of equations, SLOC too long, the paper is very hard to read.
     
 ** For newbie, we recommend to read the paper of algorithms which difficulty is "easy" or "medium" difficulty level.
@@ -1122,15 +1133,15 @@
   * **OriginalWOA**: Mirjalili, S., & Lewis, A. (2016). The whale optimization algorithm. Advances in engineering software, 95, 51-67.
   * **HI_WOA**: Tang, C., Sun, W., Wu, W., & Xue, M. (2019, July). A hybrid improved whale optimization algorithm. In 2019 IEEE 15th International Conference on Control and Automation (ICCA) (pp. 362-367). IEEE.
 
 * **WHO - Wildebeest Herd Optimization** 
   * **OriginalWHO**: Amali, D., & Dinakaran, M. (2019). Wildebeest herd optimization: A new global optimization algorithm inspired by wildebeest herding behaviour. Journal of Intelligent & Fuzzy Systems, (Preprint), 1-14.
 
 * **WDO - Wind Driven Optimization** 
-  * **OriginalWDO**: Bayraktar, Z., Komurcu, M., & Werner, D. H. (2010, July). Wind Driven Optimization (WDO): A novel nature-inspired optimization algorithm and its application to electromagnetics. In 2010 IEEE antennas and propagation society international symposium (pp. 1-4). IEEE.
+  * **OriginalWDO**: Bayraktar, Z., Komurcu, M., Bossard, J.A. and Werner, D.H., 2013. The wind driven optimization technique and its application in electromagnetics. IEEE transactions on antennas and propagation, 61(5), pp.2745-2757.
 
 
 ### X
 
 ### Y
 
 ### Z
```

### Comparing `mealpy-2.5.3a1/README.md` & `mealpy-2.5.4a1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 
-<p align="center"><img src="https://thieu1995.github.io/post/2022-04/19-mealpy-tutorials/mealpy1.png" alt="MEALPY"/></p>
+<p align="center">
+<img style="height:400px;" 
+src="https://thieu1995.github.io/post/2022-04/19-mealpy-tutorials/mealpy5-nobg.png" 
+alt="MEALPY"/>
+</p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-2.5.2-yellow.svg)](https://github.com/thieu1995/mealpy/releases)
+[![GitHub release](https://img.shields.io/badge/release-2.5.3-yellow.svg)](https://github.com/thieu1995/mealpy/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mealpy) 
 [![PyPI version](https://badge.fury.io/py/mealpy.svg)](https://badge.fury.io/py/mealpy)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mealpy.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mealpy.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mealpy.svg)
 [![Downloads](https://pepy.tech/badge/mealpy)](https://pepy.tech/project/mealpy)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mealpy/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mealpy/actions/workflows/publish-package.yaml)
@@ -23,15 +27,15 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 MEALPY is the largest python library for most of the cutting-edge nature-inspired meta-heuristic algorithms (population-based). Population meta-heuristic algorithms (PMA) are the most popular algorithms in the field of 
 approximate optimization.
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Total algorithms**: 172 (102 original, 45 official variants, 25 developed variants)
+* **Total algorithms**: 174 (102 original, 45 official variants, 27 developed variants)
 * **Documentation:** https://mealpy.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
 * **Dependencies:** numpy, scipy, pandas, matplotlib
 
 
 # Goals
 
@@ -47,15 +51,15 @@
 
 
 # Installation
 
 ### Install with pip
 Install the [current PyPI release](https://pypi.python.org/pypi/mealpy):
 ```sh 
-$ pip install mealpy==2.5.2
+$ pip install mealpy==2.5.3
 ```
 
 ### Install from source
 In case you want to install directly from the source code, use:
 ```sh 
 $ git clone https://github.com/thieu1995/mealpy.git
 $ cd mealpy
@@ -180,19 +184,25 @@
 paras_bbo_grid = {
     "epoch": [100],
     "pop_size": [50],
     "elites": [2, 3, 4, 5],
     "p_m": [0.01, 0.02, 0.05, 0.1, 0.15, 0.2]
 }
 
+term = {
+  "max_fe": 10000
+}
+
 if __name__ == "__main__":
     model = BBO.BaseBBO()
 
     tuner = Tuner(model, paras_bbo_grid)
-    tuner.execute(problem=problem, n_trials=10, mode="parallel", n_workers=4)
+    tuner.execute(problem=problem, termination=term, n_trials=5, n_jobs=5, mode="thread", n_workers=4, verbose=True)
+    ## Solve this problem 5 times (n_trials) using 5 processes (n_jobs), each process will handle 1 trial. 
+    ## The mode to run the solver is thread (mode), we will calculate the fitness of 4 solutions (n_workers) at the same time 
 
     print(tuner.best_score)
     print(tuner.best_params)
     print(tuner.best_algorithm)
     print(tuner.best_algorithm.get_name())
     
     ## Save results to csv file 
@@ -263,20 +273,24 @@
 
 ## Define models
 
 model1 = BBO.BaseBBO(epoch=10, pop_size=50)
 model2 = BBO.OriginalBBO(epoch=10, pop_size=50)
 model3 = DE.BaseDE(epoch=10, pop_size=50)
 
+## Define termination if needed
+term = {
+    "max_fe": 10000
+}
 
 ## Define and run Multitask
-
 if __name__ == "__main__":
-    multitask = Multitask(algorithms=(model1, model2, model3), problems=(p1, p2, p3))
-    multitask.execute(n_trials=3, mode="parallel", n_workers=6, save_path="history", save_as="csv", save_convergence=True, verbose=True)
+    multitask = Multitask(algorithms=(model1, model2, model3), problems=(p1, p2, p3), terminations=(term, ), modes=("thread", ))
+    # default modes = "single", default termination = epoch (as defined in problem dictionary)
+    multitask.execute(n_trials=5, n_jobs=5, save_path="history", save_as="csv", save_convergence=False, verbose=False)
     
     ## Check the directory: history/, you will see list of .csv result files
 ```
 
 For more usage examples please look at [examples](/examples) folder.
 
 More advanced examples can also be found in the [Mealpy-examples repository](https://github.com/thieu1995/mealpy_examples).
@@ -355,23 +369,20 @@
 We share lots of information, questions, and answers there. You will get more support and knowledge there.
 
 ### Cite Us
 
 If you are using mealpy in your project, we would appreciate citations:
 
 ```bibtex 
-@software{nguyen_van_thieu_2022_6684223,
-  author       = {Nguyen Van Thieu and Seyedali Mirjalili},
-  title        = {{MEALPY: a Framework of The State-of-The-Art Meta-Heuristic Algorithms in Python}},
-  month        = jun,
-  year         = 2022,
-  publisher    = {Zenodo},
-  version      = {v2.4.2},
-  doi          = {10.5281/zenodo.6684223},
-  url          = {https://doi.org/10.5281/zenodo.6684223}
+@article{van2023mealpy,
+  title={MEALPY: An open-source library for latest meta-heuristic algorithms in Python},
+  author={Van Thieu, Nguyen and Mirjalili, Seyedali},
+  journal={Journal of Systems Architecture},
+  year={2023},
+  publisher={Elsevier}
 }
 
 @article{van2023groundwater,
   title={Groundwater level modeling using Augmented Artificial Ecosystem Optimization},
   author={Van Thieu, Nguyen and Barma, Surajit Deb and Van Lam, To and Kisi, Ozgur and Mahesha, Amai},
   journal={Journal of Hydrology},
   volume={617},
@@ -452,15 +463,15 @@
     + Physics-based: Idea from physics law such as Newton's law of universal gravitation, black hole, multiverse 
     + Human-based: Idea from human interaction such as queuing search, teaching learning, ... 
     + Biology-based: Idea from biology creature (or microorganism),...
     + System-based: Idea from eco-system, immune-system, network-system, ...
     + Math-based: Idea from mathematical form or mathematical law such as sin-cosin 
     + Music-based: Idea from music instrument
 
-* Difficulty - Difficulty Level (Personal Opinion): Objective observation from author. Depend on the number of 
+* Difficulty - Difficulty Level (Personal Opinion): **Objective observation from author**. Depend on the number of 
   parameters, number of equations, the original ideas, time spend for coding, source lines of code (SLOC).
     + Easy: A few paras, few equations, SLOC very short
     + Medium: more equations than Easy level, SLOC longer than Easy level
     + Hard: Lots of equations, SLOC longer than Medium level, the paper hard to read.
     + Hard* - Very hard: Lots of equations, SLOC too long, the paper is very hard to read.
     
 ** For newbie, we recommend to read the paper of algorithms which difficulty is "easy" or "medium" difficulty level.
@@ -1079,15 +1090,15 @@
   * **OriginalWOA**: Mirjalili, S., & Lewis, A. (2016). The whale optimization algorithm. Advances in engineering software, 95, 51-67.
   * **HI_WOA**: Tang, C., Sun, W., Wu, W., & Xue, M. (2019, July). A hybrid improved whale optimization algorithm. In 2019 IEEE 15th International Conference on Control and Automation (ICCA) (pp. 362-367). IEEE.
 
 * **WHO - Wildebeest Herd Optimization** 
   * **OriginalWHO**: Amali, D., & Dinakaran, M. (2019). Wildebeest herd optimization: A new global optimization algorithm inspired by wildebeest herding behaviour. Journal of Intelligent & Fuzzy Systems, (Preprint), 1-14.
 
 * **WDO - Wind Driven Optimization** 
-  * **OriginalWDO**: Bayraktar, Z., Komurcu, M., & Werner, D. H. (2010, July). Wind Driven Optimization (WDO): A novel nature-inspired optimization algorithm and its application to electromagnetics. In 2010 IEEE antennas and propagation society international symposium (pp. 1-4). IEEE.
+  * **OriginalWDO**: Bayraktar, Z., Komurcu, M., Bossard, J.A. and Werner, D.H., 2013. The wind driven optimization technique and its application in electromagnetics. IEEE transactions on antennas and propagation, 61(5), pp.2745-2757.
 
 
 ### X
 
 ### Y
 
 ### Z
```

### Comparing `mealpy-2.5.3a1/mealpy/__init__.py` & `mealpy-2.5.4a1/mealpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # >>>
 # >>> ## Run the algorithm
 # >>> model = PSO.C_PSO(epoch=5, pop_size=50, name="C-PSO")
 # >>> best_position, best_fitness = model.solve(problem)
 # >>> print(f"Best solution: {best_position}, Best fitness: {best_fitness}")
 
 
-__version__ = "2.5.3-alpha.1"
+__version__ = "2.5.4-alpha.1"
 
 from .bio_based import (BBO, BBOA, BMO, EOA, IWO, SBO, SMA, SOA, SOS, TPO, TSA, VCS, WHO)
 from .evolutionary_based import (CRO, DE, EP, ES, FPA, GA, MA)
 from .human_based import (BRO, BSO, CA, CHIO, FBIO, GSKA, HBO, HCO, ICA, LCO, QSA, SARO, SPBO, SSDO, TLO, TOA, WarSO)
 from .math_based import (AOA, CEM, CGO, CircleSA, GBO, HC, INFO, PSS, RUN, SCA, SHIO)
 from .physics_based import (ArchOA, ASO, CDO, EFO, EO, EVO, FLA, HGSO, MVO, NRO, RIME, SA, TWO, WDO)
 from .swarm_based import (ABC, ACOR, AGTO, ALO, AO, ARO, AVOA, BA, BeesA, BES, BFO, BSA, COA, CoatiOA, CSA, CSO,
```

### Comparing `mealpy-2.5.3a1/mealpy/bio_based/BBO.py` & `mealpy-2.5.4a1/mealpy/bio_based/BBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/bio_based/BBOA.py` & `mealpy-2.5.4a1/mealpy/bio_based/BBOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/bio_based/BMO.py` & `mealpy-2.5.4a1/mealpy/bio_based/BMO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/bio_based/EOA.py` & `mealpy-2.5.4a1/mealpy/bio_based/EOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/bio_based/IWO.py` & `mealpy-2.5.4a1/mealpy/bio_based/IWO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/bio_based/SBO.py` & `mealpy-2.5.4a1/mealpy/bio_based/SBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/bio_based/SMA.py` & `mealpy-2.5.4a1/mealpy/bio_based/SMA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/bio_based/SOA.py` & `mealpy-2.5.4a1/mealpy/bio_based/SOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/bio_based/SOS.py` & `mealpy-2.5.4a1/mealpy/bio_based/SOS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/bio_based/TPO.py` & `mealpy-2.5.4a1/mealpy/bio_based/TPO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/bio_based/TSA.py` & `mealpy-2.5.4a1/mealpy/bio_based/TSA.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,18 @@
     The original version: Tunicate Swarm Algorithm (TSA)
 
     Links:
         1. https://www.sciencedirect.com/science/article/abs/pii/S0952197620300385?via%3Dihub
         2. https://www.mathworks.com/matlabcentral/fileexchange/75182-tunicate-swarm-algorithm-tsa
 
     Notes:
-        1. Weakest algorithm in the list
-        2. The paper has so many wrong equations in algorithm
-        3. Matlab code different to the paper
-        4. This algorithm is typical similar to Barnacles Mating Optimizer (BMO)
+        1. This algorithm has some limitations
+        2. The paper has several wrong equations in algorithm
+        3. The implementation in Matlab code has some difference to the paper
+        4. This algorithm shares some similarities with the Barnacles Mating Optimizer (BMO)
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.bio_based.TSA import OriginalTSA
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/bio_based/VCS.py` & `mealpy-2.5.4a1/mealpy/bio_based/VCS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/bio_based/WHO.py` & `mealpy-2.5.4a1/mealpy/bio_based/WHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/evolutionary_based/CRO.py` & `mealpy-2.5.4a1/mealpy/evolutionary_based/CRO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/evolutionary_based/DE.py` & `mealpy-2.5.4a1/mealpy/evolutionary_based/DE.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/evolutionary_based/EP.py` & `mealpy-2.5.4a1/mealpy/evolutionary_based/EP.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/evolutionary_based/ES.py` & `mealpy-2.5.4a1/mealpy/evolutionary_based/ES.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/evolutionary_based/FPA.py` & `mealpy-2.5.4a1/mealpy/evolutionary_based/FPA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/evolutionary_based/GA.py` & `mealpy-2.5.4a1/mealpy/evolutionary_based/GA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/evolutionary_based/MA.py` & `mealpy-2.5.4a1/mealpy/evolutionary_based/MA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/human_based/BRO.py` & `mealpy-2.5.4a1/mealpy/human_based/BRO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/human_based/BSO.py` & `mealpy-2.5.4a1/mealpy/human_based/BSO.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 class ImprovedBSO(Optimizer):
     """
     The improved version: Brain Storm Optimization (BSO)
 
     Notes
     ~~~~~
-    + Remove some probability parameters, and some useless equations.
-    + Levy-flight technique is used for robustness
+    + Remove some probability parameters, and some unnecessary equations.
+    + The Levy-flight technique is employed to enhance the algorithm's robustness and resilience in challenging environments.
 
     Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
         + m_clusters (int): [3, 10], number of clusters (m in the paper)
         + p1 (float): 25% percent
         + p2 (float): 50% percent changed by its own (local search), 50% percent changed by outside (global search)
         + p3 (float): 75% percent develop the old idea, 25% invented new idea based on levy-flight
         + p4 (float): [0.4, 0.6], Need more weights on the centers instead of the random position
```

### Comparing `mealpy-2.5.3a1/mealpy/human_based/CA.py` & `mealpy-2.5.4a1/mealpy/human_based/CA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/human_based/CHIO.py` & `mealpy-2.5.4a1/mealpy/human_based/CHIO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/human_based/FBIO.py` & `mealpy-2.5.4a1/mealpy/human_based/FBIO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/human_based/GSKA.py` & `mealpy-2.5.4a1/mealpy/human_based/GSKA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/human_based/HBO.py` & `mealpy-2.5.4a1/mealpy/human_based/HBO.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     The original version of: Heap-based optimizer (HBO)
 
     Links:
         1. https://www.sciencedirect.com/science/article/abs/pii/S0957417420305261#!
         2. https://github.com/qamar-askari/HBO/blob/master/HBO.m
 
     Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
-            + degree (int): [2, 4], the degree level in Corporate Rank Hierarchy (CRH), default=2
+        + degree (int): [2, 4], the degree level in Corporate Rank Hierarchy (CRH), default=2
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.human_based.HBO import OriginalHBO
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/human_based/HCO.py` & `mealpy-2.5.4a1/mealpy/human_based/HCO.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     The original version of: Human Conception Optimizer (HCO)
 
     Links:
         1. https://www.mathworks.com/matlabcentral/fileexchange/124200-human-conception-optimizer-hco
         2. https://www.nature.com/articles/s41598-022-25031-6
 
     Notes:
-        1. Kinda similar to PSO algorithm. Just the concepts of nature-inspired animals are difference
-        2. Matlab code different to the paper
+        1. This algorithm shares some similarities with the PSO algorithm (equations)
+        2. The implementation of Matlab code is kinda different to the paper
 
     Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
         + w (float): (0, 1.) - weight factor for probability of fitness selection, default=0.65
         + w1 (float): (0, 1.0) - weight factor for velocity update stage, default=0.05
         + c1 (float): (0., 3.0) - acceleration coefficient, same as PSO, default=1.4
         + c2 (float): (0., 3.0) - acceleration coefficient, same as PSO, default=1.4
```

### Comparing `mealpy-2.5.3a1/mealpy/human_based/ICA.py` & `mealpy-2.5.4a1/mealpy/human_based/ICA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/human_based/LCO.py` & `mealpy-2.5.4a1/mealpy/human_based/LCO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/human_based/QSA.py` & `mealpy-2.5.4a1/mealpy/human_based/QSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/human_based/SARO.py` & `mealpy-2.5.4a1/mealpy/human_based/SARO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/human_based/SPBO.py` & `mealpy-2.5.4a1/mealpy/human_based/SPBO.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 
 class OriginalSPBO(Optimizer):
     """
     The original version of: Student Psychology Based Optimization (SPBO)
 
     Notes:
-        1. Weak algorithm
-        2. Consume too much time because of ndim * pop_size updating times.
+        1. This algorithm is a weak algorithm in solving several problems
+        2. It also consumes too much time because of ndim * pop_size updating times.
 
     Links:
        1. https://www.sciencedirect.com/science/article/abs/pii/S0965997820301484
        2. https://www.mathworks.com/matlabcentral/fileexchange/80991-student-psycology-based-optimization-spbo-algorithm
 
     Examples
     ~~~~~~~~
```

### Comparing `mealpy-2.5.3a1/mealpy/human_based/SSDO.py` & `mealpy-2.5.4a1/mealpy/human_based/SSDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/human_based/TLO.py` & `mealpy-2.5.4a1/mealpy/human_based/TLO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/human_based/TOA.py` & `mealpy-2.5.4a1/mealpy/human_based/TOA.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,26 @@
 class OriginalTOA(Optimizer):
     """
     The original version of: Teamwork Optimization Algorithm (TOA)
 
     Links:
         1. https://www.mdpi.com/1424-8220/21/13/4567
 
-    Notes (Plagiarism):
-        1. Algorithm design is very similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Coati Optimization Algorithm (CoatiOA),
+    Notes:
+        1. Algorithm design is similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Coati Optimization Algorithm (CoatiOA),
         Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA),
         Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Pelican Optimization Algorithm (POA), Northern goshawk optimization (NGO),
         Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
-        2. Check the matlab code of all above algorithms
-        2. Same authors, self-plagiarized article with kinda same algorithm with different meta-metaphors
-        4. Check the results of benchmark functions in the papers, they are mostly make up results
+
+        2. It may be useful to compare the Matlab code of this algorithm with those of the similar algorithms to ensure its accuracy and completeness.
+
+        3. While this article may share some similarities with previous work by the same authors, it is important to recognize the potential value in exploring
+        different meta-metaphors and concepts to drive innovation and progress in optimization research.
+
+        4. Further investigation may be warranted to verify the benchmark results reported in the papers and ensure their reliability and accuracy.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.human_based.TOA import OriginalTOA
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/human_based/WarSO.py` & `mealpy-2.5.4a1/mealpy/human_based/WarSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/math_based/AOA.py` & `mealpy-2.5.4a1/mealpy/math_based/AOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/math_based/CEM.py` & `mealpy-2.5.4a1/mealpy/math_based/CEM.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/math_based/CGO.py` & `mealpy-2.5.4a1/mealpy/math_based/CGO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/math_based/CircleSA.py` & `mealpy-2.5.4a1/mealpy/math_based/CircleSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/math_based/GBO.py` & `mealpy-2.5.4a1/mealpy/math_based/GBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/math_based/HC.py` & `mealpy-2.5.4a1/mealpy/math_based/HC.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/math_based/INFO.py` & `mealpy-2.5.4a1/mealpy/math_based/INFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/math_based/PSS.py` & `mealpy-2.5.4a1/mealpy/math_based/PSS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/math_based/RUN.py` & `mealpy-2.5.4a1/mealpy/math_based/RUN.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/math_based/SCA.py` & `mealpy-2.5.4a1/mealpy/math_based/SCA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/math_based/SHIO.py` & `mealpy-2.5.4a1/mealpy/math_based/SHIO.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,18 +13,17 @@
     The original version of: Success History Intelligent Optimizer (SHIO)
 
     Links:
         1. https://link.springer.com/article/10.1007/s11227-021-04093-9
         2. https://www.mathworks.com/matlabcentral/fileexchange/122157-success-history-intelligent-optimizer-shio
 
     Notes:
-        1. The algorithm is very easy with no special operators.
-        2. This is a weak algorithm and should not be used in research or practical problems.
-        3. There is slow convergence in the algorithm. If we look at the Matlab code, we can see that a student
-        is trying to implement it with many errors and unnecessary things. Not sure why it got accepted in that journal
+        1. The algorithm is designed with simplicity and ease of implementation in mind, utilizing basic operators.
+        2. This algorithm has several limitations and weak when dealing with several problems
+        3. The algorithm's convergence is slow. The Matlab code has many errors and unnecessary things.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.math_based.SHIO import OriginalSHIO
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/multitask.py` & `mealpy-2.5.4a1/mealpy/multitask.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,14 +23,64 @@
     Additionally, it allows for exporting results in various formats such as Pandas DataFrame, JSON, and CSV.
 
     Args:
         algorithms (list, tuple): List of algorithms to run
         problems (list, tuple): List of problems to run
         terminations (list, tuple): List of terminations to apply on algorithm/problem
         modes (list, tuple): List of modes to apply on algorithm/problem
+
+    Examples
+    --------
+    >>> from opfunu.cec_based.cec2017 import F52017, F102017, F292017
+    >>> from mealpy.bio_based import BBO
+    >>> from mealpy.evolutionary_based import DE
+    >>> from mealpy.multitask import Multitask
+    >>> ## Define your own problems
+    >>> f1 = F52017(30, f_bias=0)
+    >>> f2 = F102017(30, f_bias=0)
+    >>> f3 = F292017(30, f_bias=0)
+    >>> p1 = {
+    >>>     "lb": f1.lb,
+    >>>     "ub": f1.ub,
+    >>>     "minmax": "min",
+    >>>     "fit_func": f1.evaluate,
+    >>>     "name": "F5",
+    >>>     "log_to": None,
+    >>> }
+    >>> p2 = {
+    >>>     "lb": f2.lb,
+    >>>     "ub": f2.ub,
+    >>>     "minmax": "min",
+    >>>     "fit_func": f2.evaluate,
+    >>>     "name": "F10",
+    >>>     "log_to": None,
+    >>> }
+    >>> p3 = {
+    >>>     "lb": f3.lb,
+    >>>     "ub": f3.ub,
+    >>>     "minmax": "min",
+    >>>     "fit_func": f3.evaluate,
+    >>>     "name": "F29",
+    >>>     "log_to": None,
+    >>> }
+    >>> ## Define models
+    >>> model1 = BBO.BaseBBO(epoch=10000, pop_size=50)
+    >>> model2 = BBO.OriginalBBO(epoch=10000, pop_size=50)
+    >>> model3 = DE.BaseDE(epoch=10000, pop_size=50)
+    >>> model4 = DE.SAP_DE(epoch=10000, pop_size=50)
+    >>> ## Define termination if needed
+    >>> term = {
+    >>>     "max_fe": 30000
+    >>> }
+    >>> ## Define and run Multitask
+    >>> if __name__ == "__main__":
+    >>>     multitask = Multitask(algorithms=(model1, model2, model3, model4), problems=(p1, p2, p3), terminations=(term, ), modes=("thread", ))
+    >>>     # default modes = "single", default termination = epoch (as defined in problem dictionary)
+    >>>     multitask.execute(n_trials=5, n_jobs=5, save_path="history", save_as="csv", save_convergence=True, verbose=False)
+    >>>     # multitask.execute(n_trials=5, save_path="history", save_as="csv", save_convergence=True, verbose=False)
     """
     def __init__(self, algorithms=(), problems=(), terminations=None, modes=None, **kwargs):
         self.__set_keyword_arguments(kwargs)
         self.validator = Validator(log_to="console", log_file=None)
         self.algorithms = self.validator.check_list_tuple("algorithms", algorithms, "Optimizer")
         self.problems = self.validator.check_list_tuple("problems", problems, "Problem")
         self.n_algorithms = len(self.algorithms)
@@ -76,36 +126,34 @@
         _, best_fitness = model.solve(problem, mode=mode, termination=termination)
         return {
             "id_trial": id_trial,
             "best_fitness": best_fitness,
             "convergence": model.history.list_global_best_fit
         }
 
-    def execute(self, n_trials=2, mode="sequential", n_workers=2, save_path="history", save_as="csv", save_convergence=False, verbose=False):
+    def execute(self, n_trials=2, n_jobs=None, save_path="history", save_as="csv", save_convergence=False, verbose=False):
         """Execute multitask utility.
 
         Args:
             n_trials (int): Number of repetitions
-            mode (str): Execute problem using "sequential" or "parallel" mode, default = "sequential"
-            n_workers (int): Number of processes if mode is "parallel"
+            n_jobs (int, None): Number of processes will be used to speed up the computation (<=1 or None: sequential, >=2: parallel)
             save_path (str): The path to the folder that hold results
             save_as (str): Saved file type (e.g. dataframe, json, csv) (default: "csv")
             save_convergence (bool): Save the error (convergence/fitness) during generations (default: False)
             verbose (bool): Switch for verbose logging (default: False)
 
         Raises:
             TypeError: Raises TypeError if export type is not supported
 
         """
         n_trials = self.validator.check_int("n_trials", n_trials, [1, 100000])
-        mode = self.validator.check_str("mode", mode, ["parallel", "sequential"])
-        if mode == "parallel":
-            n_workers = self.validator.check_int("n_workers", n_workers, [2, min(61, os.cpu_count() - 1)])
-        else:
-            n_workers = None
+        n_workers = None
+        if (n_jobs is not None) and (n_jobs >= 1):
+            n_workers = self.validator.check_int("n_jobs", n_jobs, [2, min(61, os.cpu_count() - 1)])
+
         ## Get export function
         save_as = self.validator.check_str("save_as", save_as, ["csv", "json", "dataframe"])
         export_function = getattr(self, f"export_to_{save_as}")
 
         for id_model, model in enumerate(self.algorithms):
             if not isinstance(model, Optimizer):
                 print(f"Model: {id_model+1} is not an instance of Optimizer class.")
@@ -144,15 +192,15 @@
                         print(f"Mode: {id_prob + 1} is fall back on 'single'")
 
                 convergence_trials = {}
                 best_fit_trials = []
 
                 trial_list = list(range(1, n_trials+1))
 
-                if mode == "parallel":
+                if n_workers is not None:
                     with parallel.ProcessPoolExecutor(n_workers) as executor:
                         list_results = executor.map(partial(self.__run__, model=model, problem=problem, termination=term, mode=mode), trial_list)
                         for result in list_results:
                             convergence_trials[f"trial_{result['id_trial']}"] = result['convergence']
                             best_fit_trials.append(result['best_fitness'])
                             if verbose:
                                 print(f"Solving problem: {problem.get_name()} using algorithm: {model.get_name()}, on the: {result['id_trial']} trial")
@@ -162,12 +210,15 @@
                         convergence_trials[f"trial_{result['id_trial']}"] = result['convergence']
                         best_fit_trials.append(result['best_fitness'])
                         if verbose:
                             print(f"Solving problem: {problem.get_name()} using algorithm: {model.get_name()}, on the: {result['id_trial']} trial")
 
                 best_fit_model_results[problem.get_name()] = best_fit_trials
                 if save_convergence:
+                    max_length = max([len(col) for col in convergence_trials.values()])
+                    for kk, vv in convergence_trials.items():
+                        convergence_trials[kk] = list(vv) + [float('nan')] * (max_length - len(vv))
                     df1 = pd.DataFrame(convergence_trials)
                     export_function(df1, f"{path_convergence}/{problem.get_name()}_convergence")
 
             df2 = pd.DataFrame(best_fit_model_results)
             export_function(df2, f"{path_best_fit}/{model.get_name()}_best_fit")
```

### Comparing `mealpy-2.5.3a1/mealpy/music_based/HS.py` & `mealpy-2.5.4a1/mealpy/music_based/HS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/optimizer.py` & `mealpy-2.5.4a1/mealpy/optimizer.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/physics_based/ASO.py` & `mealpy-2.5.4a1/mealpy/physics_based/ASO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/physics_based/ArchOA.py` & `mealpy-2.5.4a1/mealpy/physics_based/ArchOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/physics_based/CDO.py` & `mealpy-2.5.4a1/mealpy/physics_based/CDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/physics_based/EFO.py` & `mealpy-2.5.4a1/mealpy/physics_based/EFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/physics_based/EO.py` & `mealpy-2.5.4a1/mealpy/physics_based/EO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/physics_based/EVO.py` & `mealpy-2.5.4a1/mealpy/physics_based/EVO.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     """
     The original version of: Energy Valley Optimizer (EVO)
 
     Links:
         1. https://www.nature.com/articles/s41598-022-27344-y
         2. https://www.mathworks.com/matlabcentral/fileexchange/123130-energy-valley-optimizer-a-novel-metaheuristic-algorithm
 
-    Notes (parameters):
-        1. The algorithm is very easy, and there is nothing special about this one.
-        2. This is a very weak algorithm with slow convergence because there is no good strategy, and no special operations are performed.
+    Notes:
+        1. The algorithm is straightforward and does not require any specialized knowledge or techniques.
+        2. The algorithm may not perform optimally due to slow convergence and no good operations, which could be improved by implementing better strategies and operations.
         3. The problem is that it is stuck at a local optimal around 1/2 of the max generations because fitness distance is being used as a factor in the equations.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.physics_based.EVO import OriginalEVO
     >>>
```

### Comparing `mealpy-2.5.3a1/mealpy/physics_based/FLA.py` & `mealpy-2.5.4a1/mealpy/physics_based/FLA.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,17 @@
         + C2 (float): factor C2, default=2.0
         + C3 (float): factor C3, default=0.1
         + C4 (float): factor C4, default=0.2
         + C5 (float): factor C5, default=2.0
         + DD (float): factor D in the paper, default=0.01
 
     Notes:
-        1. Too many parameters, and they are unnecessary
-        2. The algorithms are complex, but they are weak, making it easy to get stuck in local optima.
-        3. Overflow problems will occur due to the division by the fitness value.
+        1. The algorithm contains a high number of parameters, some of which may be unnecessary.
+        2. Despite the complexity of the algorithms, they may not perform optimally and could potentially become trapped in local optima.
+        3. Division by the fitness value may cause overflow issues to arise.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.physics_based.FLA import OriginalFLA
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/physics_based/HGSO.py` & `mealpy-2.5.4a1/mealpy/physics_based/HGSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/physics_based/MVO.py` & `mealpy-2.5.4a1/mealpy/physics_based/MVO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/physics_based/NRO.py` & `mealpy-2.5.4a1/mealpy/physics_based/NRO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/physics_based/RIME.py` & `mealpy-2.5.4a1/mealpy/physics_based/RIME.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 import numpy as np
 from mealpy.optimizer import Optimizer
 
 
 class OriginalRIME(Optimizer):
     """
-    The original version of: Artificial Gorilla Troops Optimization (RIME)
+    The original version of: physical phenomenon of RIME-ice  (RIME)
 
     Links:
         1. https://doi.org/10.1016/j.neucom.2023.02.010
         2. https://www.mathworks.com/matlabcentral/fileexchange/124610-rime-a-physics-based-optimization
 
     Notes (parameters):
         1. w (float): Soft-rime parameters, default=5.0
-        2. The algorithm is very easy and there is nothing special about this one.
-        3. This is very weak algorithm, slow convergence.
+        2. The algorithm is straightforward and does not require any specialized knowledge or techniques.
+        3. The algorithm may exhibit slow convergence and may not perform optimally.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.physics_based.RIME import OriginalRIME
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/physics_based/SA.py` & `mealpy-2.5.4a1/mealpy/physics_based/SA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/physics_based/TWO.py` & `mealpy-2.5.4a1/mealpy/physics_based/TWO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/physics_based/WDO.py` & `mealpy-2.5.4a1/mealpy/physics_based/WDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/ABC.py` & `mealpy-2.5.4a1/mealpy/swarm_based/ABC.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/ACOR.py` & `mealpy-2.5.4a1/mealpy/swarm_based/ACOR.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class OriginalACOR(Optimizer):
     """
     The original version of: Ant Colony Optimization Continuous (ACOR)
 
     Notes
     ~~~~~
-    + Use Gaussian Distribution instead of random number (np.random.normal() function)
+    + Use Gaussian Distribution (np.random.normal() function) instead of random number (np.random.rand())
     + Amend solution when they went out of space
 
     Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
         + sample_count (int): [2, 10000], Number of Newly Generated Samples, default = 25
         + intent_factor (float): [0.2, 1.0], Intensification Factor (Selection Pressure), (q in the paper), default = 0.5
         + zeta (float): [1, 2, 3], Deviation-Distance Ratio, default = 1
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/AGTO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/TDO.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,118 +4,101 @@
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from mealpy.optimizer import Optimizer
 
 
-class OriginalAGTO(Optimizer):
+class OriginalTDO(Optimizer):
     """
-    The original version of: Artificial Gorilla Troops Optimization (AGTO)
+    The original version of: Tasmanian Devil Optimization (TDO)
 
     Links:
-        1. https://doi.org/10.1002/int.22535
-        2. https://www.mathworks.com/matlabcentral/fileexchange/95953-artificial-gorilla-troops-optimizer
+        1. https://www.mathworks.com/matlabcentral/fileexchange/111380-tasmanian-devil-optimization-tdo
+        2. https://ieeexplore.ieee.org/abstract/document/9714388
 
-    Notes (parameters):
-        1. p1 (float): the probability of transition in exploration phase (p in the paper), default = 0.03
-        2. p2 (float): the probability of transition in exploitation phase (w in the paper), default = 0.8
-        3. beta (float): coefficient in updating equation, should be in [-5.0, 5.0], default = 3.0
+    Notes:
+        1. This is somewhat concerning, as there appears to be a high degree of similarity between the source code for this algorithm and the Osprey Optimization Algorithm (OOA)
+        2. Algorithm design is similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Pelican optimization algorithm (POA), Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA), Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Northern goshawk optimization (NGO), Osprey Optimization Algorithm (OOA), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
+        3. It may be useful to compare the Matlab code of this algorithm with those of the similar algorithms to ensure its accuracy and completeness.
+        4. The article may share some similarities with previous work by the same authors, further investigation may be warranted to verify the benchmark results reported in the papers and ensure their reliability and accuracy.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.swarm_based.AGTO import OriginalAGTO
+    >>> from mealpy.swarm_based.TDO import OriginalTDO
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
     >>> problem_dict1 = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
     >>> }
     >>>
     >>> epoch = 1000
     >>> pop_size = 50
-    >>> model = OriginalAGTO(epoch, pop_size)
+    >>> model = OriginalTDO(epoch, pop_size)
     >>> best_position, best_fitness = model.solve(problem_dict1)
     >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
 
     References
     ~~~~~~~~~~
-    [1] Abdollahzadeh, B., Soleimanian Gharehchopogh, F., & Mirjalili, S. (2021). Artificial gorilla troops optimizer: a new
-    nature‐inspired metaheuristic algorithm for global optimization problems. International Journal of Intelligent Systems, 36(10), 5887-5958.
+    [1] Dehghani, M., Hubálovský, Š., & Trojovský, P. (2022). Tasmanian devil optimization: a new bio-inspired
+    optimization algorithm for solving optimization algorithm. IEEE Access, 10, 19599-19620.
     """
-    def __init__(self, epoch=10000, pop_size=100, p1=0.03, p2=0.8, beta=3.0, **kwargs):
+    def __init__(self, epoch=10000, pop_size=100, **kwargs):
         """
         Args:
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
         """
         super().__init__(**kwargs)
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
-        self.p1 = self.validator.check_float("p1", p1, (0, 1))      # p in the paper
-        self.p2 = self.validator.check_float("p2", p2, (0, 1))      # w in the paper
-        self.beta = self.validator.check_float("beta", beta, [-10.0, 10.0])
-        self.set_parameters(["epoch", "pop_size", "p1", "p2", "beta"])
+        self.set_parameters(["epoch", "pop_size"])
+        self.support_parallel_modes = False
         self.sort_flag = False
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        a = (np.cos(2*np.random.rand())+1) * (1 - (epoch+1)/self.epoch)
-        c = a * (2 * np.random.rand() - 1)
-
-        ## Exploration
-        pop_new = []
         for idx in range(0, self.pop_size):
-            if np.random.rand() < self.p1:
-                pos_new = self.generate_position(self.problem.lb, self.problem.ub)
-            else:
-                if np.random.rand() >= 0.5:
-                    z = np.random.uniform(-a, a, self.problem.n_dims)
-                    rand_idx = np.random.randint(0, self.pop_size)
-                    pos_new = (np.random.rand() - a) * self.pop[rand_idx][self.ID_POS] + c * z * self.pop[idx][self.ID_POS]
+            # PHASE1: Hunting Feeding
+            if np.random.rand() > 0.5:
+                # STRATEGY 1: FEEDING BY EATING CARRION (EXPLORATION PHASE)
+                # CARRION selection using (3)
+                kk = np.random.choice(list(set(range(0, self.pop_size)) - {idx}))
+                if self.compare_agent(self.pop[kk], self.pop[idx]):
+                    pos_new = self.pop[idx][self.ID_POS] + np.random.rand(self.problem.n_dims) * (self.pop[kk][self.ID_POS] - np.random.randint(1, 3)*self.pop[idx][self.ID_POS])
                 else:
-                    id1, id2 = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 2, replace=False)
-                    pos_new = self.pop[idx][self.ID_POS] - c*(c*self.pop[idx][self.ID_POS] - self.pop[id1][self.ID_POS]) + \
-                        np.random.rand() * (self.pop[idx][self.ID_POS] - self.pop[id2][self.ID_POS])
-            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-            pop_new.append([pos_new, None])
-            if self.mode not in self.AVAILABLE_MODES:
-                target = self.get_target_wrapper(pos_new)
-                self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
-        if self.mode in self.AVAILABLE_MODES:
-            pop_new = self.update_target_wrapper_population(pop_new)
-            self.pop = self.greedy_selection_population(self.pop, pop_new)
-        _, self.g_best = self.update_global_best_solution(self.pop, save=False)
-
-        pos_list = np.array([agent[self.ID_POS] for agent in self.pop])
-        ## Exploitation
-        pop_new = []
-        for idx in range(0, self.pop_size):
-            if a >= self.p2:
-                g = 2 ** c
-                delta = (np.abs(np.mean(pos_list, axis=0)) ** g) ** (1.0 / g)
-                pos_new = c*delta*(self.pop[idx][self.ID_POS] - self.g_best[self.ID_POS]) + self.pop[idx][self.ID_POS]
+                    pos_new = self.pop[idx][self.ID_POS] + np.random.rand(self.problem.n_dims) * (self.pop[idx][self.ID_POS] - self.pop[kk][self.ID_POS])
+                pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+                tar_new = self.get_target_wrapper(pos_new)
+                if self.compare_agent([pos_new, tar_new], self.pop[idx]):
+                    self.pop[idx] = [pos_new, tar_new]
             else:
-                if np.random.rand() >= 0.5:
-                    h = np.random.normal(0, 1, self.problem.n_dims)
+            # STRATEGY 2: FEEDING BY EATING PREY (EXPLOITATION PHASE)
+            # stage1: prey selection and attack it
+                kk = np.random.choice(list(set(range(0, self.pop_size)) - {idx}))
+                if self.compare_agent(self.pop[kk], self.pop[idx]):
+                    pos_new = self.pop[idx][self.ID_POS] + np.random.rand(self.problem.n_dims) * (self.pop[kk][self.ID_POS] - np.random.randint(1, 3) * self.pop[idx][self.ID_POS])
                 else:
-                    h = np.random.normal(0, 1)
-                r1 = np.random.rand()
-                pos_new = self.g_best[self.ID_POS] - (2*r1-1)*(self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS]) * (self.beta * h)
+                    pos_new = self.pop[idx][self.ID_POS] + np.random.rand(self.problem.n_dims) * (self.pop[idx][self.ID_POS] - self.pop[kk][self.ID_POS])
+                pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+                tar_new = self.get_target_wrapper(pos_new)
+                if self.compare_agent([pos_new, tar_new], self.pop[idx]):
+                    self.pop[idx] = [pos_new, tar_new]
+
+            # stage2: prey chasing
+            rr = 0.01 * (1 - (epoch+1)/self.epoch)      # Calculating the neighborhood radius using(9)
+            pos_new = self.pop[idx][self.ID_POS] + (-rr + 2 * rr * np.random.rand(self.problem.n_dims)) * self.pop[idx][self.ID_POS]
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-            pop_new.append([pos_new, None])
-            if self.mode not in self.AVAILABLE_MODES:
-                target = self.get_target_wrapper(pos_new)
-                self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
-        if self.mode in self.AVAILABLE_MODES:
-            pop_new = self.update_target_wrapper_population(pop_new)
-            self.pop = self.greedy_selection_population(self.pop, pop_new)
+            tar_new = self.get_target_wrapper(pos_new)
+            if self.compare_agent([pos_new, tar_new], self.pop[idx]):
+                self.pop[idx] = [pos_new, tar_new]
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/ALO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/ALO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/AO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/AO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/ARO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/PFA.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,96 @@
 #!/usr/bin/env python
-# Created by "Thieu" at 22:46, 26/10/2022 ----------%                                                                               
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
+# Created by "Thieu" at 14:51, 17/03/2020 ----------%
+#       Email: nguyenthieu2102@gmail.com            %
+#       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
+from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
-class OriginalARO(Optimizer):
+class OriginalPFA(Optimizer):
     """
-    The original version of: Artificial Rabbits Optimization (ARO)
+    The original version of: Pathfinder Algorithm (PFA)
 
     Links:
-        1. https://doi.org/10.1016/j.engappai.2022.105082
-        2. https://www.mathworks.com/matlabcentral/fileexchange/110250-artificial-rabbits-optimization-aro
+        1. https://doi.org/10.1016/j.asoc.2019.03.012
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.swarm_based.ARO import OriginalARO
+    >>> from mealpy.swarm_based.PFA import OriginalPFA
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
     >>> problem_dict1 = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
     >>> }
     >>>
     >>> epoch = 1000
     >>> pop_size = 50
-    >>> model = OriginalARO(epoch, pop_size)
+    >>> model = OriginalPFA(epoch, pop_size)
     >>> best_position, best_fitness = model.solve(problem_dict1)
     >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
 
     References
     ~~~~~~~~~~
-    [1] Wang, L., Cao, Q., Zhang, Z., Mirjalili, S., & Zhao, W. (2022). Artificial rabbits optimization: A new bio-inspired
-    meta-heuristic algorithm for solving engineering optimization problems. Engineering Applications of Artificial Intelligence, 114, 105082.
+    [1] Yapici, H. and Cetinkaya, N., 2019. A new meta-heuristic optimizer: Pathfinder algorithm.
+    Applied soft computing, 78, pp.545-568.
     """
 
     def __init__(self, epoch=10000, pop_size=100, **kwargs):
         """
         Args:
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
         """
         super().__init__(**kwargs)
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
         self.set_parameters(["epoch", "pop_size"])
-        self.sort_flag = False
+        self.sort_flag = True
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        theta = 2 * (1 - (epoch+1)/self.epoch)
-        pop_new = []
-        for idx in range(0, self.pop_size):
-            L = (np.exp(1) - np.exp((epoch / self.epoch)**2)) * (np.sin(2*np.pi*np.random.rand()))
-            temp = np.zeros(self.problem.n_dims)
-            rd_index = np.random.choice(np.arange(0, self.problem.n_dims), int(np.ceil(np.random.rand()*self.problem.n_dims)), replace=False)
-            temp[rd_index] = 1
-            R = L * temp        # Eq 2
-            A = 2 * np.log(1.0 / np.random.rand()) * theta      # Eq. 15
-            if A > 1:
-                rand_idx = np.random.randint(0, self.pop_size)
-                pos_new = self.pop[rand_idx][self.ID_POS] + R * (self.pop[idx][self.ID_POS] - self.pop[rand_idx][self.ID_POS]) + \
-                    np.round(0.5 * (0.05 + np.random.rand())) * np.random.normal(0, 1)      # Eq. 1
-            else:
-                gr = np.zeros(self.problem.n_dims)
-                rd_index = np.random.choice(np.arange(0, self.problem.n_dims), int(np.ceil(np.random.rand() * self.problem.n_dims)), replace=False)
-                gr[rd_index] = 1        # Eq. 12
-                H = np.random.normal(0, 1) * (epoch / self.epoch)       # Eq. 8
-                b = self.pop[idx][self.ID_POS] + H * gr * self.pop[idx][self.ID_POS]        # Eq. 13
-                pos_new = self.pop[idx][self.ID_POS] + R * (np.random.rand() * b - self.pop[idx][self.ID_POS])      # Eq. 11
+        alpha, beta = np.random.uniform(1, 2, 2)
+        A = np.random.uniform(self.problem.lb, self.problem.ub) * np.exp(-2 * (epoch + 1) / self.epoch)
+        t = 1 - (epoch + 1) * 1.0 / self.epoch
+        space = self.problem.ub - self.problem.lb
+
+        ## Update the position of pathfinder and check the bound
+        pos_new = self.pop[0][self.ID_POS] + 2 * np.random.uniform() * (self.g_best[self.ID_POS] - self.pop[0][self.ID_POS]) + A
+        pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+        target = self.get_target_wrapper(pos_new)
+        pop_new = [[pos_new, target], ]
+
+        ## Update positions of members, check the bound and calculate new fitness
+        for idx in range(1, self.pop_size):
+            agent = deepcopy(self.pop[idx])
+            pos_new = deepcopy(self.pop[idx][self.ID_POS]).astype(float)
+            for k in range(1, self.pop_size):
+                dist = np.sqrt(np.sum((self.pop[k][self.ID_POS] - self.pop[idx][self.ID_POS]) ** 2)) / self.problem.n_dims
+                t2 = alpha * np.random.uniform() * (self.pop[k][self.ID_POS] - self.pop[idx][self.ID_POS])
+                ## First stabilize the distance
+                t3 = np.random.uniform() * t * (dist / space)
+                pos_new += t2 + t3
+            ## Second stabilize the population size
+            t1 = beta * np.random.uniform() * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
+            pos_new = (pos_new + t1) / self.pop_size
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-            pop_new.append([pos_new, None])
+            agent[self.ID_POS] = pos_new
+            pop_new.append(agent)
             if self.mode not in self.AVAILABLE_MODES:
-                target = self.get_target_wrapper(pos_new)
-                self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
+                pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
-            self.pop = self.greedy_selection_population(self.pop, pop_new)
+        self.pop = self.greedy_selection_population(self.pop, pop_new)
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/AVOA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/AVOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/BA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/BA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/BES.py` & `mealpy-2.5.4a1/mealpy/swarm_based/BES.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/BFO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/BFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/BSA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/BSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/BeesA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/BeesA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/COA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/COA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/CSA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/CSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/CSO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/CSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/CoatiOA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/CoatiOA.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,22 +12,18 @@
     """
     The original version of: Coati Optimization Algorithm (CoatiOA)
 
     Links:
         1. https://www.sciencedirect.com/science/article/pii/S0950705122011042
         2. https://www.mathworks.com/matlabcentral/fileexchange/116965-coa-coati-optimization-algorithm
 
-    Notes (Plagiarism):
-        1. Algorithm design is very similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Pelican optimization algorithm (POA),
-        Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA),
-        Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Northern goshawk optimization (NGO),
-        Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
-        2. Check the matlab code of all above algorithms
-        2. Same authors, self-plagiarized article with kinda same algorithm with different meta-metaphors
-        4. Check the results of benchmark functions in the papers, they are mostly make up results
+    Notes:
+        1. Algorithm design is similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Pelican optimization algorithm (POA), Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA), Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Northern goshawk optimization (NGO), Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
+        2. It may be useful to compare the Matlab code of this algorithm with those of the similar algorithms to ensure its accuracy and completeness.
+        3. The article may share some similarities with previous work by the same authors, further investigation may be warranted to verify the benchmark results reported in the papers and ensure their reliability and accuracy.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.swarm_based.CoatiOA import OriginalCoatiOA
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/DMOA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/DMOA.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     The original version of: Dwarf Mongoose Optimization Algorithm (DMOA)
 
     Links:
         1. https://doi.org/10.1016/j.cma.2022.114570
         2. https://www.mathworks.com/matlabcentral/fileexchange/105125-dwarf-mongoose-optimization-algorithm
 
     Notes:
-        1. Matlab code is litle bit difference than original paper
-        2. There are some meaningless parameters and equations in the matlab code
-        3. Weak algorithm
+        1. The Matlab code differs slightly from the original paper
+        2. There are some parameters and equations in the Matlab code that don't seem to have any meaningful purpose.
+        3. The algorithm seems to be weak on solving several problems.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.swarm_based.DMOA import OriginalDMOA
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/DO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/DO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/EHO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/EHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/ESOA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/ESOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/FA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/FA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/FFA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/FFA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/FFO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/FFO.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,23 +11,19 @@
 class OriginalFFO(Optimizer):
     """
     The original version of: Fennec Fox Optimization (FFO)
 
     Links:
         1. https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9853509
 
-    Notes (Plagiarism):
-        0. This is really disgusting, because the source code for this algorithm is almost exactly the same as the source code for Pelican Optimization Algorithm (POA)
-        1. Algorithm design is very similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Coati Optimization Algorithm (CoatiOA),
-        Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA),
-        Pelican Optimization Algorithm (POA), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Northern goshawk optimization (NGO),
-        Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
-        2. Check the matlab code of all above algorithms
-        2. Same authors, self-plagiarized article with kinda same algorithm with different meta-metaphors
-        4. Check the results of benchmark functions in the papers, they are mostly make up results
+    Notes:
+        1. This is somewhat concerning, as there appears to be a high degree of similarity between the source code for this algorithm and the Pelican Optimization Algorithm (POA).
+        2. Algorithm design is similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Coati Optimization Algorithm (CoatiOA), Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA), Pelican Optimization Algorithm (POA), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Northern goshawk optimization (NGO), Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
+        3. It may be useful to compare the Matlab code of this algorithm with those of the similar algorithms to ensure its accuracy and completeness.
+        4. The article may share some similarities with previous work by the same authors, further investigation may be warranted to verify the benchmark results reported in the papers and ensure their reliability and accuracy.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.swarm_based.FFO import OriginalFFO
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/FOA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/FOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/FOX.py` & `mealpy-2.5.4a1/mealpy/swarm_based/FOX.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,19 +16,17 @@
         1. https://link.springer.com/article/10.1007/s10489-022-03533-0
         2. https://www.mathworks.com/matlabcentral/fileexchange/121592-fox-a-fox-inspired-optimization-algorithm
 
     Notes (parameters):
         1. c1 (float): the probability of jumping (c1 in the paper), default = 0.18
         2. c2 (float): the probability of jumping (c2 in the paper), default = 0.82
 
-    Notes (Algorithm's design):
-        1. I don't know how this algorithm get accepted in Applied Intelligence journal
-        2. The equation to calculate distance_S_travel value in matlab code is meaningless
-        3. The whole point of if else conditions with p > 0.18 is meaningless. The authors just choice the best value
-        based on his experiment without explaining it.
+    Notes:
+        1. The equation used to calculate the distance_S_travel value in the Matlab code seems to be lacking in meaning.
+        2. The if-else conditions used with p > 0.18 seem to lack a clear justification. The authors seem to have simply chosen the best value based on their experiments without explaining the rationale behind it.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.swarm_based.FOX import OriginalFOX
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/GJO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/GJO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/GOA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/GOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/GTO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/HHO.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,136 +1,126 @@
 #!/usr/bin/env python
-# Created by "Thieu" at 21:58, 16/03/2023 ----------%                                                                               
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
+# Created by "Thieu" at 14:51, 17/03/2020 ----------%
+#       Email: nguyenthieu2102@gmail.com            %
+#       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
-from math import gamma
 import numpy as np
+from math import gamma
+from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
-class OriginalGTO(Optimizer):
+class OriginalHHO(Optimizer):
     """
-    The original version of: Giant Trevally Optimizer (GTO)
+    The original version of: Harris Hawks Optimization (HHO)
 
     Links:
-        1. https://www.mathworks.com/matlabcentral/fileexchange/121358-giant-trevally-optimizer-gto
-        2. https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9955508
-
-    Notes:
-        1. This algorithm costs a huge amount of computational resources in each epoch.
-        Therefore, be careful when using the maximum number of generations as a stopping condition.
-        2. Other algorithms update around K*pop_size times in each epoch, this algorithm updates around 2*pop_size^2 + pop_size times
+        1. https://doi.org/10.1016/j.future.2019.02.028
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.swarm_based.GTO import OriginalGTO
+    >>> from mealpy.swarm_based.HHO import OriginalHHO
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
     >>> problem_dict1 = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
     >>> }
     >>>
     >>> epoch = 1000
     >>> pop_size = 50
-    >>> model = OriginalGTO(epoch, pop_size)
+    >>> model = OriginalHHO(epoch, pop_size)
     >>> best_position, best_fitness = model.solve(problem_dict1)
     >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
 
     References
     ~~~~~~~~~~
-    [1] Sadeeq, H. T., & Abdulazeez, A. M. (2022). Giant Trevally Optimizer (GTO): A Novel Metaheuristic
-    Algorithm for Global Optimization and Challenging Engineering Problems. IEEE Access, 10, 121615-121640.
+    [1] Heidari, A.A., Mirjalili, S., Faris, H., Aljarah, I., Mafarja, M. and Chen, H., 2019.
+    Harris hawks optimization: Algorithm and applications. Future generation computer systems, 97, pp.849-872.
     """
-    def __init__(self, epoch=10000, pop_size=100, p1=0.03, p2=0.8, beta=3.0, **kwargs):
+
+    def __init__(self, epoch=10000, pop_size=100, **kwargs):
         """
         Args:
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
         """
         super().__init__(**kwargs)
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
         self.set_parameters(["epoch", "pop_size"])
-        self.sort_flag = True
-
-    def levy__(self, beta=1.0, size=None, step=0.01):
-        num = gamma(1 + beta) * np.sin(np.pi * beta/2)
-        den = gamma((1+beta)/2) * beta * 2**((beta-1)/2)
-        sigma_u = (num/den)**(1.0/beta)
-        u = np.random.normal(0, sigma_u, size=size)
-        v = np.random.normal(0, 1, size=size)
-        return u/(np.abs(v)**(1.0/beta)) * step
+        self.sort_flag = False
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        # Step 1: Extensive Search
-        for idx in range(0, self.pop_size):
-            pop_new = []
-            for jdx in range(0, self.pop_size):
-                if idx == jdx:
-                    continue
-                # foraging movement patterns of giant trevallies are simulated using Eq.(4)
-                pos_new = self.g_best[self.ID_POS] * np.random.rand() + ((self.problem.ub - self.problem.lb) * np.random.rand() + self.problem.lb) * \
-                          self.levy__(beta=1.5, size=self.problem.n_dims)
-                pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-                pop_new.append([pos_new, None])
-                if self.mode not in self.AVAILABLE_MODES:
-                    pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
-            pop_new = self.update_target_wrapper_population(pop_new)
-            _, self.pop[idx] = self.get_global_best_solution(pop_new + [self.pop[idx]])
-        _, self.g_best = self.update_global_best_solution(self.pop, save=False)
-
-        # Step 2: Choosing Area
-        pos_list = np.array([agent[self.ID_POS] for agent in self.pop])
-        pos_m = np.mean(pos_list, axis=0)
-        A = 0.4
         pop_new = []
         for idx in range(0, self.pop_size):
-            # In the choosing area step, giant trevallies identify and select the best area in terms of
-            # the amount of food (seabirds) within the selected search space where they can hunt for prey.
-            r3 = np.random.rand()
-            pos_new = self.g_best[self.ID_POS] * A * r3 + pos_m - self.pop[idx][self.ID_POS] * r3        # Eq. 7
-            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-            pop_new.append([pos_new, None])
-            if self.mode not in self.AVAILABLE_MODES:
-                target = self.get_target_wrapper(pos_new)
-                self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
-        if self.mode in self.AVAILABLE_MODES:
-            pop_new = self.update_target_wrapper_population(pop_new)
-            self.pop = self.greedy_selection_population(self.pop, pop_new)
-        _, self.g_best = self.update_global_best_solution(self.pop, save=False)
-
-        # Step 3: Attacking
-        H = np.random.rand() * (2.0 - (epoch+1) * 2.0 / self.epoch)     #  Eq.(15)
-        for idx in range(0, self.pop_size):
-            pop_new = []
-            for jdx in range(0, self.pop_size):
-                if idx == jdx:
-                    continue
-                # the distance between the prey and the attacker, and can be calculated using (12):
-                dist = np.sum(np.abs(self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS]))
-                theta2 = (360 - 0) * np.random.rand() + 0
-                theta1 = 1.3296 * np.sin(np.radians(theta2))        # calculate theta_1 using (10)
-                # visual distortion indicates the apparent height of the bird, which is always seen
-                # to be higher than its actual height due to the refraction of the light.
-                VD = np.sin(np.radians(theta1)) * dist      # Eq. 11
-                # the behavior of giant trevally when chasing and jumping out of the water is mathematically simulated using (13)
-                pos_new = self.pop[idx][self.ID_POS] * np.sin(np.radians(theta2)) * self.pop[idx][self.ID_TAR][self.ID_FIT] + VD + H
+            # -1 < E0 < 1
+            E0 = 2 * np.random.uniform() - 1
+            # factor to show the decreasing energy of rabbit
+            E = 2 * E0 * (1 - (epoch + 1) * 1.0 / self.epoch)
+            J = 2 * (1 - np.random.uniform())
+
+            # -------- Exploration phase Eq. (1) in paper -------------------
+            if np.abs(E) >= 1:
+                # Harris' hawks perch randomly based on 2 strategy:
+                if np.random.rand() >= 0.5:  # perch based on other family members
+                    X_rand = deepcopy(self.pop[np.random.randint(0, self.pop_size)][self.ID_POS])
+                    pos_new = X_rand - np.random.uniform() * np.abs(X_rand - 2 * np.random.uniform() * self.pop[idx][self.ID_POS])
+
+                else:  # perch on a random tall tree (random site inside group's home range)
+                    X_m = np.mean([x[self.ID_POS] for x in self.pop])
+                    pos_new = (self.g_best[self.ID_POS] - X_m) - np.random.uniform() * \
+                              (self.problem.lb + np.random.uniform() * (self.problem.ub - self.problem.lb))
                 pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
                 pop_new.append([pos_new, None])
-                if self.mode not in self.AVAILABLE_MODES:
-                    pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
+            # -------- Exploitation phase -------------------
+            else:
+                # Attacking the rabbit using 4 strategies regarding the behavior of the rabbit
+                # phase 1: ----- surprise pounce (seven kills) ----------
+                # surprise pounce (seven kills): multiple, short rapid dives by different hawks
+                if (np.random.rand() >= 0.5):
+                    delta_X = self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS]
+                    if np.abs(E) >= 0.5:  # Hard besiege Eq. (6) in paper
+                        pos_new = delta_X - E * np.abs(J * self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
+                    else:  # Soft besiege Eq. (4) in paper
+                        pos_new = self.g_best[self.ID_POS] - E * np.abs(delta_X)
+                    pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+                    pop_new.append([pos_new, None])
+                else:
+                    xichma = np.power((gamma(1 + 1.5) * np.sin(np.pi * 1.5 / 2.0)) /
+                                      (gamma((1 + 1.5) * 1.5 * np.power(2, (1.5 - 1) / 2)) / 2.0), 1.0 / 1.5)
+                    LF_D = 0.01 * np.random.uniform() * xichma / np.power(np.abs(np.random.uniform()), 1.0 / 1.5)
+                    if np.abs(E) >= 0.5:  # Soft besiege Eq. (10) in paper
+                        Y = self.g_best[self.ID_POS] - E * np.abs(J * self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
+                    else:  # Hard besiege Eq. (11) in paper
+                        X_m = np.mean([x[self.ID_POS] for x in self.pop])
+                        Y = self.g_best[self.ID_POS] - E * np.abs(J * self.g_best[self.ID_POS] - X_m)
+                    pos_Y = self.amend_position(Y, self.problem.lb, self.problem.ub)
+                    target_Y = self.get_target_wrapper(pos_Y)
+                    Z = Y + np.random.uniform(self.problem.lb, self.problem.ub) * LF_D
+                    pos_Z = self.amend_position(Z, self.problem.lb, self.problem.ub)
+                    target_Z = self.get_target_wrapper(pos_Z)
+                    if self.compare_agent([pos_Y, target_Y], self.pop[idx]):
+                        pop_new.append([pos_Y, target_Y])
+                        continue
+                    if self.compare_agent([pos_Z, target_Z], self.pop[idx]):
+                        pop_new.append([pos_Z, target_Z])
+                        continue
+                    pop_new.append(deepcopy(self.pop[idx]))
+        if self.mode not in self.AVAILABLE_MODES:
+            for idx, agent in enumerate(pop_new):
+                pop_new[idx][self.ID_TAR] = self.get_target_wrapper(agent[self.ID_POS])
+        else:
             pop_new = self.update_target_wrapper_population(pop_new)
-            _, self.pop[idx] = self.get_global_best_solution(pop_new + [self.pop[idx]])
+        self.pop = self.greedy_selection_population(self.pop, pop_new)
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/GWO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/GWO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/HBA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/HBA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/HGS.py` & `mealpy-2.5.4a1/mealpy/swarm_based/HGS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/HHO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/MSA.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,127 @@
 #!/usr/bin/env python
-# Created by "Thieu" at 14:51, 17/03/2020 ----------%
+# Created by "Thieu" at 14:52, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
 from math import gamma
 from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
-class OriginalHHO(Optimizer):
+class OriginalMSA(Optimizer):
     """
-    The original version of: Harris Hawks Optimization (HHO)
+    The original version: Moth Search Algorithm (MSA)
 
     Links:
-        1. https://doi.org/10.1016/j.future.2019.02.028
+        1. https://www.mathworks.com/matlabcentral/fileexchange/59010-moth-search-ms-algorithm
+        2. https://doi.org/10.1007/s12293-016-0212-3
+
+    Notes
+        + The matlab version of original paper is not good (especially convergence chart)
+        + The random number (gaussian distribution) is added in each updating equation
+
+    Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
+        + n_best (int): [3, 10], how many of the best moths to keep from one generation to the next, default=5
+        + partition (float): [0.3, 0.8], The proportional of first partition, default=0.5
+        + max_step_size (float): [0.5, 2.0], Max step size used in Levy-flight technique, default=1.0
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.swarm_based.HHO import OriginalHHO
+    >>> from mealpy.swarm_based.MSA import OriginalMSA
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
     >>> problem_dict1 = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
     >>> }
     >>>
     >>> epoch = 1000
     >>> pop_size = 50
-    >>> model = OriginalHHO(epoch, pop_size)
+    >>> n_best = 5
+    >>> partition = 0.5
+    >>> max_step_size = 1.0
+    >>> model = OriginalMSA(epoch, pop_size, n_best, partition, max_step_size)
     >>> best_position, best_fitness = model.solve(problem_dict1)
     >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
 
     References
     ~~~~~~~~~~
-    [1] Heidari, A.A., Mirjalili, S., Faris, H., Aljarah, I., Mafarja, M. and Chen, H., 2019.
-    Harris hawks optimization: Algorithm and applications. Future generation computer systems, 97, pp.849-872.
+    [1] Wang, G.G., 2018. Moth search algorithm: a bio-inspired metaheuristic algorithm for
+    global optimization problems. Memetic Computing, 10(2), pp.151-164.
     """
 
-    def __init__(self, epoch=10000, pop_size=100, **kwargs):
+    def __init__(self, epoch=10000, pop_size=100, n_best=5, partition=0.5, max_step_size=1.0, **kwargs):
         """
         Args:
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
+            n_best (int): how many of the best moths to keep from one generation to the next, default=5
+            partition (float): The proportional of first partition, default=0.5
+            max_step_size (float): Max step size used in Levy-flight technique, default=1.0
         """
         super().__init__(**kwargs)
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
-        self.set_parameters(["epoch", "pop_size"])
-        self.sort_flag = False
+        self.n_best = self.validator.check_int("n_best", n_best, [2, int(self.pop_size/2)])
+        self.partition = self.validator.check_float("partition", partition, (0, 1.0))
+        self.max_step_size = self.validator.check_float("max_step_size", max_step_size, (0, 5.0))
+        self.set_parameters(["epoch", "pop_size", "n_best", "partition", "max_step_size"])
+        self.sort_flag = True
+        # np1 in paper
+        self.n_moth1 = int(np.ceil(self.partition * self.pop_size))
+        # np2 in paper, we actually don't need this variable
+        self.n_moth2 = self.pop_size - self.n_moth1
+        # you can change this ratio so as to get much better performance
+        self.golden_ratio = (np.sqrt(5) - 1) / 2.0
+
+    def _levy_walk(self, iteration):
+        beta = 1.5  # Eq. 2.23
+        sigma = (gamma(1 + beta) * np.sin(np.pi * (beta - 1) / 2) / (gamma(beta / 2) * (beta - 1) * 2 ** ((beta - 2) / 2))) ** (1 / (beta - 1))
+        u = np.random.uniform(self.problem.lb, self.problem.ub) * sigma
+        v = np.random.uniform(self.problem.lb, self.problem.ub)
+        step = u / np.abs(v) ** (1.0 / (beta - 1))  # Eq. 2.21
+        scale = self.max_step_size / (iteration + 1)
+        delta_x = scale * step
+        return delta_x
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
+        pop_best = deepcopy(self.pop[:self.n_best])
+
         pop_new = []
         for idx in range(0, self.pop_size):
-            # -1 < E0 < 1
-            E0 = 2 * np.random.uniform() - 1
-            # factor to show the decreasing energy of rabbit
-            E = 2 * E0 * (1 - (epoch + 1) * 1.0 / self.epoch)
-            J = 2 * (1 - np.random.uniform())
-
-            # -------- Exploration phase Eq. (1) in paper -------------------
-            if np.abs(E) >= 1:
-                # Harris' hawks perch randomly based on 2 strategy:
-                if np.random.rand() >= 0.5:  # perch based on other family members
-                    X_rand = deepcopy(self.pop[np.random.randint(0, self.pop_size)][self.ID_POS])
-                    pos_new = X_rand - np.random.uniform() * np.abs(X_rand - 2 * np.random.uniform() * self.pop[idx][self.ID_POS])
-
-                else:  # perch on a random tall tree (random site inside group's home range)
-                    X_m = np.mean([x[self.ID_POS] for x in self.pop])
-                    pos_new = (self.g_best[self.ID_POS] - X_m) - np.random.uniform() * \
-                              (self.problem.lb + np.random.uniform() * (self.problem.ub - self.problem.lb))
-                pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-                pop_new.append([pos_new, None])
-            # -------- Exploitation phase -------------------
+            # Migration operator
+            if idx < self.n_moth1:
+                # scale = self.max_step_size / (epoch+1)       # Smaller step for local walk
+                pos_new = self.pop[idx][self.ID_POS] + np.random.normal() * self._levy_walk(epoch)
             else:
-                # Attacking the rabbit using 4 strategies regarding the behavior of the rabbit
-                # phase 1: ----- surprise pounce (seven kills) ----------
-                # surprise pounce (seven kills): multiple, short rapid dives by different hawks
-                if (np.random.rand() >= 0.5):
-                    delta_X = self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS]
-                    if np.abs(E) >= 0.5:  # Hard besiege Eq. (6) in paper
-                        pos_new = delta_X - E * np.abs(J * self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
-                    else:  # Soft besiege Eq. (4) in paper
-                        pos_new = self.g_best[self.ID_POS] - E * np.abs(delta_X)
-                    pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-                    pop_new.append([pos_new, None])
-                else:
-                    xichma = np.power((gamma(1 + 1.5) * np.sin(np.pi * 1.5 / 2.0)) /
-                                      (gamma((1 + 1.5) * 1.5 * np.power(2, (1.5 - 1) / 2)) / 2.0), 1.0 / 1.5)
-                    LF_D = 0.01 * np.random.uniform() * xichma / np.power(np.abs(np.random.uniform()), 1.0 / 1.5)
-                    if np.abs(E) >= 0.5:  # Soft besiege Eq. (10) in paper
-                        Y = self.g_best[self.ID_POS] - E * np.abs(J * self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
-                    else:  # Hard besiege Eq. (11) in paper
-                        X_m = np.mean([x[self.ID_POS] for x in self.pop])
-                        Y = self.g_best[self.ID_POS] - E * np.abs(J * self.g_best[self.ID_POS] - X_m)
-                    pos_Y = self.amend_position(Y, self.problem.lb, self.problem.ub)
-                    target_Y = self.get_target_wrapper(pos_Y)
-                    Z = Y + np.random.uniform(self.problem.lb, self.problem.ub) * LF_D
-                    pos_Z = self.amend_position(Z, self.problem.lb, self.problem.ub)
-                    target_Z = self.get_target_wrapper(pos_Z)
-                    if self.compare_agent([pos_Y, target_Y], self.pop[idx]):
-                        pop_new.append([pos_Y, target_Y])
-                        continue
-                    if self.compare_agent([pos_Z, target_Z], self.pop[idx]):
-                        pop_new.append([pos_Z, target_Z])
-                        continue
-                    pop_new.append(deepcopy(self.pop[idx]))
-        if self.mode not in self.AVAILABLE_MODES:
-            for idx, agent in enumerate(pop_new):
-                pop_new[idx][self.ID_TAR] = self.get_target_wrapper(agent[self.ID_POS])
-        else:
+                # Flying in a straight line
+                temp_case1 = self.pop[idx][self.ID_POS] + np.random.normal() * \
+                             self.golden_ratio * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
+                temp_case2 = self.pop[idx][self.ID_POS] + np.random.normal() * \
+                             (1.0 / self.golden_ratio) * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
+                pos_new = np.where(np.random.uniform(self.problem.n_dims) < 0.5, temp_case2, temp_case1)
+            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+            pop_new.append([pos_new, None])
+            if self.mode not in self.AVAILABLE_MODES:
+                target = self.get_target_wrapper(pos_new)
+                self.pop[idx] = self.get_better_solution(self.pop[idx], [pos_new, target])
+        if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
-        self.pop = self.greedy_selection_population(self.pop, pop_new)
+            self.pop = self.greedy_selection_population(self.pop, pop_new)
+        self.pop, _ = self.get_global_best_solution(self.pop)
+        # Replace the worst with the previous generation's elites.
+        for i in range(0, self.n_best):
+            self.pop[-1 - i] = deepcopy(pop_best[i])
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/JA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/JA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/MFO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/MFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/MGO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/MGO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/MPA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/MPA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/MRFO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/MRFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/MSA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/SSpiderA.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,128 +1,150 @@
 #!/usr/bin/env python
-# Created by "Thieu" at 14:52, 17/03/2020 ----------%
+# Created by "Thieu" at 11:59, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from math import gamma
 from copy import deepcopy
+from scipy.spatial.distance import cdist
 from mealpy.optimizer import Optimizer
 
 
-class OriginalMSA(Optimizer):
+class OriginalSSpiderA(Optimizer):
     """
-    The original version: Moth Search Algorithm (MSA)
+    The developed version of: Social Spider Algorithm (OriginalSSpiderA)
 
     Links:
-        1. https://www.mathworks.com/matlabcentral/fileexchange/59010-moth-search-ms-algorithm
-        2. https://doi.org/10.1007/s12293-016-0212-3
+        1. https://doi.org/10.1016/j.asoc.2015.02.014
+        2. https://github.com/James-Yu/SocialSpiderAlgorithm  (Modified this version)
 
-    Notes
-    ~~~~~
-    + The matlab version of original paper is not good (especially convergence chart)
-    + The random number (gaussian distribution) is added in each updating equation
+    Notes:
+        + The version of the algorithm available on the GitHub repository has a slow convergence rate.
+        + Changes the idea of intensity, which one has better intensity, others will move toward to it
 
     Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
-        + n_best (int): [3, 10], how many of the best moths to keep from one generation to the next, default=5
-        + partition (float): [0.3, 0.8], The proportional of first partition, default=0.5
-        + max_step_size (float): [0.5, 2.0], Max step size used in Levy-flight technique, default=1.0
+        + r_a (float): the rate of vibration attenuation when propagating over the spider web, default=1.0
+        + p_c (float): controls the probability of the spiders changing their dimension mask in the random walk step, default=0.7
+        + p_m (float): the probability of each value in a dimension mask to be one, default=0.1
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.swarm_based.MSA import OriginalMSA
+    >>> from mealpy.swarm_based.SSpiderA import OriginalSSpiderA
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
     >>> problem_dict1 = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
     >>> }
     >>>
     >>> epoch = 1000
     >>> pop_size = 50
-    >>> n_best = 5
-    >>> partition = 0.5
-    >>> max_step_size = 1.0
-    >>> model = OriginalMSA(epoch, pop_size, n_best, partition, max_step_size)
+    >>> r_a = 1.0
+    >>> p_c = 0.7
+    >>> p_m = 0.1
+    >>> model = OriginalSSpiderA(epoch, pop_size, r_a, p_c, p_m)
     >>> best_position, best_fitness = model.solve(problem_dict1)
     >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
 
     References
     ~~~~~~~~~~
-    [1] Wang, G.G., 2018. Moth search algorithm: a bio-inspired metaheuristic algorithm for
-    global optimization problems. Memetic Computing, 10(2), pp.151-164.
+    [1] James, J.Q. and Li, V.O., 2015. A social spider algorithm for global optimization.
+    Applied soft computing, 30, pp.614-627.
     """
 
-    def __init__(self, epoch=10000, pop_size=100, n_best=5, partition=0.5, max_step_size=1.0, **kwargs):
+    ID_POS = 0
+    ID_TAR = 1
+    ID_INT = 2
+    ID_TARGET_POS = 3
+    ID_PREV_MOVE_VEC = 4
+    ID_MASK = 5
+
+    def __init__(self, epoch=10000, pop_size=100, r_a=1.0, p_c=0.7, p_m=0.1, **kwargs):
         """
         Args:
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
-            n_best (int): how many of the best moths to keep from one generation to the next, default=5
-            partition (float): The proportional of first partition, default=0.5
-            max_step_size (float): Max step size used in Levy-flight technique, default=1.0
+            r_a (float): the rate of vibration attenuation when propagating over the spider web, default=1.0
+            p_c (float): controls the probability of the spiders changing their dimension mask in the random walk step, default=0.7
+            p_m (float): the probability of each value in a dimension mask to be one, default=0.1
         """
         super().__init__(**kwargs)
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
-        self.n_best = self.validator.check_int("n_best", n_best, [2, int(self.pop_size/2)])
-        self.partition = self.validator.check_float("partition", partition, (0, 1.0))
-        self.max_step_size = self.validator.check_float("max_step_size", max_step_size, (0, 5.0))
-        self.set_parameters(["epoch", "pop_size", "n_best", "partition", "max_step_size"])
-        self.sort_flag = True
-        # np1 in paper
-        self.n_moth1 = int(np.ceil(self.partition * self.pop_size))
-        # np2 in paper, we actually don't need this variable
-        self.n_moth2 = self.pop_size - self.n_moth1
-        # you can change this ratio so as to get much better performance
-        self.golden_ratio = (np.sqrt(5) - 1) / 2.0
-
-    def _levy_walk(self, iteration):
-        beta = 1.5  # Eq. 2.23
-        sigma = (gamma(1 + beta) * np.sin(np.pi * (beta - 1) / 2) / (gamma(beta / 2) * (beta - 1) * 2 ** ((beta - 2) / 2))) ** (1 / (beta - 1))
-        u = np.random.uniform(self.problem.lb, self.problem.ub) * sigma
-        v = np.random.uniform(self.problem.lb, self.problem.ub)
-        step = u / np.abs(v) ** (1.0 / (beta - 1))  # Eq. 2.21
-        scale = self.max_step_size / (iteration + 1)
-        delta_x = scale * step
-        return delta_x
+        self.r_a = self.validator.check_float("r_a", r_a, (0, 5.0))
+        self.p_c = self.validator.check_float("p_c", p_c, (0, 1.0))
+        self.p_m = self.validator.check_float("p_m", p_m, (0, 1.0))
+        self.set_parameters(["epoch", "pop_size", "r_a", "p_c", "p_m"])
+        self.sort_flag = False
+
+    def create_solution(self, lb=None, ub=None, pos=None):
+        """
+        Overriding method in Optimizer class
+        + x: The position of s on the web.
+        + train: The fitness of the current position of s
+        + target_vibration: The target vibration of s in the previous iteration.
+        + intensity_vibration: intensity of vibration
+        + movement_vector: The movement that s performed in the previous iteration
+        + dimension_mask: The dimension mask 1 that s employed to guide movement in the previous iteration
+        + The dimension mask is a 0-1 binary vector of length problem size
+        + n_changed: The number of iterations since s has last changed its target vibration. (No need)
+
+        Returns:
+            list: wrapper of solution with format [position, target, intensity, target_position, previous_movement_vector, dimension_mask]
+        """
+        if pos is None:
+            pos = self.generate_position(lb, ub)
+        position = self.amend_position(pos, lb, ub)
+        target = self.get_target_wrapper(position)
+        intensity = np.log(1. / (abs(target[self.ID_FIT]) + self.EPSILON) + 1)
+        target_position = deepcopy(position)
+        previous_movement_vector = np.zeros(self.problem.n_dims)
+        dimension_mask = np.zeros(self.problem.n_dims)
+        return [position, target, intensity, target_position, previous_movement_vector, dimension_mask]
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        pop_best = deepcopy(self.pop[:self.n_best])
+        all_pos = np.array([it[self.ID_POS] for it in self.pop])  ## Matrix (pop_size, problem_size)
+        base_distance = np.mean(np.std(all_pos, axis=0))  ## Number
+        dist = cdist(all_pos, all_pos, 'euclidean')
+
+        intensity_source = np.array([it[self.ID_INT] for it in self.pop])
+        intensity_attenuation = np.exp(-dist / (base_distance * self.r_a))  ## vector (pop_size)
+        intensity_receive = np.dot(np.reshape(intensity_source, (1, self.pop_size)), intensity_attenuation)  ## vector (1, pop_size)
+        id_best_intennsity = np.argmax(intensity_receive)
 
         pop_new = []
         for idx in range(0, self.pop_size):
-            # Migration operator
-            if idx < self.n_moth1:
-                # scale = self.max_step_size / (epoch+1)       # Smaller step for local walk
-                pos_new = self.pop[idx][self.ID_POS] + np.random.normal() * self._levy_walk(epoch)
-            else:
-                # Flying in a straight line
-                temp_case1 = self.pop[idx][self.ID_POS] + np.random.normal() * \
-                             self.golden_ratio * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
-                temp_case2 = self.pop[idx][self.ID_POS] + np.random.normal() * \
-                             (1.0 / self.golden_ratio) * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
-                pos_new = np.where(np.random.uniform(self.problem.n_dims) < 0.5, temp_case2, temp_case1)
-            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-            pop_new.append([pos_new, None])
+            agent = deepcopy(self.pop[idx])
+            if self.pop[id_best_intennsity][self.ID_INT] > self.pop[idx][self.ID_INT]:
+                agent[self.ID_TARGET_POS] = self.pop[id_best_intennsity][self.ID_TARGET_POS]
+            if np.random.uniform() > self.p_c:  ## changing mask
+                agent[self.ID_MASK] = np.where(np.random.uniform(0, 1, self.problem.n_dims) < self.p_m, 0, 1)
+            pos_new = np.where(self.pop[idx][self.ID_MASK] == 0, self.pop[idx][self.ID_TARGET_POS],
+                               self.pop[np.random.randint(0, self.pop_size)][self.ID_POS])
+            ## Perform random walk
+            pos_new = self.pop[idx][self.ID_POS] + np.random.normal() * \
+                      (self.pop[idx][self.ID_POS] - self.pop[idx][self.ID_PREV_MOVE_VEC]) + \
+                      (pos_new - self.pop[idx][self.ID_POS]) * np.random.normal()
+            agent[self.ID_POS] = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             if self.mode not in self.AVAILABLE_MODES:
-                target = self.get_target_wrapper(pos_new)
-                self.pop[idx] = self.get_better_solution(self.pop[idx], [pos_new, target])
-        if self.mode in self.AVAILABLE_MODES:
-            pop_new = self.update_target_wrapper_population(pop_new)
-            self.pop = self.greedy_selection_population(self.pop, pop_new)
-        self.pop, _ = self.get_global_best_solution(self.pop)
-        # Replace the worst with the previous generation's elites.
-        for i in range(0, self.n_best):
-            self.pop[-1 - i] = deepcopy(pop_best[i])
+                agent[self.ID_TAR] = self.get_target_wrapper(agent[self.ID_POS])
+                pop_new.append(agent)
+        pop_new = self.update_target_wrapper_population(pop_new)
+
+        for idx in range(0, self.pop_size):
+            if self.compare_agent(pop_new[idx], self.pop[idx]):
+                self.pop[idx][self.ID_PREV_MOVE_VEC] = pop_new[idx][self.ID_POS] - self.pop[idx][self.ID_POS]
+                self.pop[idx][self.ID_INT] = np.log(1. / (abs(pop_new[idx][self.ID_TAR][self.ID_FIT]) + self.EPSILON) + 1)
+                self.pop[idx][self.ID_POS] = pop_new[idx][self.ID_POS]
+                self.pop[idx][self.ID_TAR] = pop_new[idx][self.ID_TAR]
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/NGO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/NGO.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,19 @@
     """
     The original version of: Northern Goshawk Optimization (NGO)
 
     Links:
         1. https://ieeexplore.ieee.org/abstract/document/9638618
         2. https://www.mathworks.com/matlabcentral/fileexchange/106665-northern-goshawk-optimization-a-new-swarm-based-algorithm
 
-    Notes (Plagiarism):
-        0. This is really disgusting, because the source code for this algorithm is exactly the same as the source code for Pelican Optimization Algorithm (POA).
-        1. Algorithm design is very similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Coati Optimization Algorithm (CoatiOA),
-        Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA),
-        Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Pelican Optimization Algorithm (POA),
-        Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
-        2. Check the matlab code of all above algorithms
-        2. Same authors, self-plagiarized article with kinda same algorithm with different meta-metaphors
-        4. Check the results of benchmark functions in the papers, they are mostly make up results
+    Notes:
+        1. This is somewhat concerning, as there appears to be a high degree of similarity between the source code for this algorithm and the Pelican Optimization Algorithm (POA).
+        2. Algorithm design is similar similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Coati Optimization Algorithm (CoatiOA), Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA), Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Pelican Optimization Algorithm (POA), Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
+        3. It may be useful to compare the Matlab code of this algorithm with those of the similar algorithms to ensure its accuracy and completeness.
+        4. The article may share some similarities with previous work by the same authors, further investigation may be warranted to verify the benchmark results reported in the papers and ensure their reliability and accuracy.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.swarm_based.NGO import OriginalNGO
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/NMRA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/NMRA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/OOA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/OOA.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,18 @@
     """
     The original version of: Osprey Optimization Algorithm (OOA)
 
     Links:
         1. https://www.frontiersin.org/articles/10.3389/fmech.2022.1126450/full
         2. https://www.mathworks.com/matlabcentral/fileexchange/124555-osprey-optimization-algorithm
 
-    Notes (Plagiarism):
-        1. Algorithm design is very similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Pelican optimization algorithm (POA),
-        Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA),
-        Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Northern goshawk optimization (NGO),
-        Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
-        2. Check the matlab code of all above algorithms
-        2. Same authors, self-plagiarized article with kinda same algorithm with different meta-metaphors
-        4. Check the results of benchmark functions in the papers, they are mostly make up results
+    Notes:
+        1. Algorithm design is similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Pelican optimization algorithm (POA), Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA), Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Northern goshawk optimization (NGO), Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
+        2. It may be useful to compare the Matlab code of this algorithm with those of the similar algorithms to ensure its accuracy and completeness.
+        3. The article may share some similarities with previous work by the same authors, further investigation may be warranted to verify the benchmark results reported in the papers and ensure their reliability and accuracy.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.swarm_based.OOA import OriginalOOA
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/PFA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/SSO.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 #!/usr/bin/env python
-# Created by "Thieu" at 14:51, 17/03/2020 ----------%
+# Created by "Thieu" at 11:38, 02/03/2021 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
-class OriginalPFA(Optimizer):
+class OriginalSSO(Optimizer):
     """
-    The original version of: Pathfinder Algorithm (PFA)
+    The original version of: Salp Swarm Optimization (SSO)
 
     Links:
-        1. https://doi.org/10.1016/j.asoc.2019.03.012
+        1. https://doi.org/10.1016/j.advengsoft.2017.07.002
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.swarm_based.PFA import OriginalPFA
+    >>> from mealpy.swarm_based.SSO import OriginalSSO
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
     >>> problem_dict1 = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
     >>> }
     >>>
     >>> epoch = 1000
     >>> pop_size = 50
-    >>> model = OriginalPFA(epoch, pop_size)
+    >>> model = OriginalSSO(epoch, pop_size)
     >>> best_position, best_fitness = model.solve(problem_dict1)
     >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
 
     References
     ~~~~~~~~~~
-    [1] Yapici, H. and Cetinkaya, N., 2019. A new meta-heuristic optimizer: Pathfinder algorithm.
-    Applied soft computing, 78, pp.545-568.
+    [1] Mirjalili, S., Gandomi, A.H., Mirjalili, S.Z., Saremi, S., Faris, H. and Mirjalili, S.M., 2017.
+    Salp Swarm Algorithm: A bio-inspired optimizer for engineering design problems. Advances in
+    Engineering Software, 114, pp.163-191.
     """
 
     def __init__(self, epoch=10000, pop_size=100, **kwargs):
         """
         Args:
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
@@ -58,39 +58,30 @@
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        alpha, beta = np.random.uniform(1, 2, 2)
-        A = np.random.uniform(self.problem.lb, self.problem.ub) * np.exp(-2 * (epoch + 1) / self.epoch)
-        t = 1 - (epoch + 1) * 1.0 / self.epoch
-        space = self.problem.ub - self.problem.lb
-
-        ## Update the position of pathfinder and check the bound
-        pos_new = self.pop[0][self.ID_POS] + 2 * np.random.uniform() * (self.g_best[self.ID_POS] - self.pop[0][self.ID_POS]) + A
-        pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-        target = self.get_target_wrapper(pos_new)
-        pop_new = [[pos_new, target], ]
-
-        ## Update positions of members, check the bound and calculate new fitness
-        for idx in range(1, self.pop_size):
-            agent = deepcopy(self.pop[idx])
-            pos_new = deepcopy(self.pop[idx][self.ID_POS]).astype(float)
-            for k in range(1, self.pop_size):
-                dist = np.sqrt(np.sum((self.pop[k][self.ID_POS] - self.pop[idx][self.ID_POS]) ** 2)) / self.problem.n_dims
-                t2 = alpha * np.random.uniform() * (self.pop[k][self.ID_POS] - self.pop[idx][self.ID_POS])
-                ## First stabilize the distance
-                t3 = np.random.uniform() * t * (dist / space)
-                pos_new += t2 + t3
-            ## Second stabilize the population size
-            t1 = beta * np.random.uniform() * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
-            pos_new = (pos_new + t1) / self.pop_size
+        ## Eq. (3.2) in the paper
+        c1 = 2 * np.exp(-((4 * (epoch + 1) / self.epoch) ** 2))
+        pop_new = []
+        for idx in range(0, self.pop_size):
+            if idx < self.pop_size / 2:
+                c2_list = np.random.random(self.problem.n_dims)
+                c3_list = np.random.random(self.problem.n_dims)
+                pos_new_1 = self.g_best[self.ID_POS] + c1 * ((self.problem.ub - self.problem.lb) * c2_list + self.problem.lb)
+                pos_new_2 = self.g_best[self.ID_POS] - c1 * ((self.problem.ub - self.problem.lb) * c2_list + self.problem.lb)
+                pos_new = np.where(c3_list < 0.5, pos_new_1, pos_new_2)
+            else:
+                # Eq. (3.4) in the paper
+                pos_new = (self.pop[idx][self.ID_POS] + self.pop[idx - 1][self.ID_POS]) / 2
+
+            # Check if salps go out of the search space and bring it back then re-calculate its fitness value
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-            agent[self.ID_POS] = pos_new
-            pop_new.append(agent)
+            pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
-                pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
+                target = self.get_target_wrapper(pos_new)
+                self.pop[idx] = self.get_better_solution(self.pop[idx], [pos_new, target])
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
-        self.pop = self.greedy_selection_population(self.pop, pop_new)
+            self.pop = self.greedy_selection_population(self.pop, pop_new)
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/POA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/POA.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,23 +12,19 @@
     """
     The original version of: Pelican Optimization Algorithm (POA)
 
     Links:
         1. https://www.mdpi.com/1424-8220/22/3/855
         2. https://www.mathworks.com/matlabcentral/fileexchange/106680-pelican-optimization-algorithm-a-novel-nature-inspired
 
-    Notes (Plagiarism):
-        0. This is really disgusting, because the source code for this algorithm is exactly the same as the source code for Northern Goshawk Optimization (NGO)
-        1. Algorithm design is very similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Coati Optimization Algorithm (CoatiOA),
-        Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA),
-        Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Northern goshawk optimization (NGO),
-        Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
-        2. Check the matlab code of all above algorithms
-        2. Same authors, self-plagiarized article with kinda same algorithm with different meta-metaphors
-        4. Check the results of benchmark functions in the papers, they are mostly make up results
+    Notes:
+        1. This is somewhat concerning, as there appears to be a high degree of similarity between the source code for this algorithm and the Northern Goshawk Optimization (NGO)
+        2. Algorithm design is similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Coati Optimization Algorithm (CoatiOA), Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA), Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Northern goshawk optimization (NGO), Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
+        3. It may be useful to compare the Matlab code of this algorithm with those of the similar algorithms to ensure its accuracy and completeness.
+        4. The article may share some similarities with previous work by the same authors, further investigation may be warranted to verify the benchmark results reported in the papers and ensure their reliability and accuracy.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.swarm_based.POA import OriginalPOA
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/PSO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/PSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/SCSO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/SCSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/SFO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/SFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/SHO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/SHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/SLO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/SLO.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,16 @@
     """
     The original version of: Sea Lion Optimization Algorithm (SLO)
 
     Links:
         1. https://www.researchgate.net/publication/333516932_Sea_Lion_Optimization_Algorithm
         2. https://doi.org/10.14569/IJACSA.2019.0100548
 
-    Notes
-    ~~~~~
-    + There are some unclear equations and parameters in the original paper 
+    Notes:
+        + There are some unclear equations and parameters in the original paper
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.swarm_based.SLO import OriginalSLO
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/SRSR.py` & `mealpy-2.5.4a1/mealpy/swarm_based/SRSR.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/SSA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/SSA.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 from mealpy.optimizer import Optimizer
 
 
 class BaseSSA(Optimizer):
     """
     The developed version: Sparrow Search Algorithm (SSA)
 
-    Notes
-    ~~~~~
-    + First, the population is sorted to find g-best and g-worst
-    + In Eq. 4, the np.random.normal() gaussian distribution is used instead of A+ and L
+    Notes:
+        + First, the population is sorted to find g-best and g-worst
+        + In Eq. 4, the np.random.normal() gaussian distribution is used instead of A+ and L
 
     Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
         + ST (float): ST in [0.5, 1.0], safety threshold value, default = 0.8
         + PD (float): number of producers (percentage), default = 0.2
         + SD (float): number of sparrows who perceive the danger, default = 0.1
 
     Examples
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/SSpiderA.py` & `mealpy-2.5.4a1/mealpy/system_based/GCO.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,151 +1,194 @@
 #!/usr/bin/env python
-# Created by "Thieu" at 11:59, 17/03/2020 ----------%
+# Created by "Thieu" at 16:44, 18/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
 from copy import deepcopy
-from scipy.spatial.distance import cdist
 from mealpy.optimizer import Optimizer
 
 
-class OriginalSSpiderA(Optimizer):
+class BaseGCO(Optimizer):
     """
-    The developed version of: Social Spider Algorithm (OriginalSSpiderA)
-
-    Links:
-        1. https://doi.org/10.1016/j.asoc.2015.02.014
-        2. https://github.com/James-Yu/SocialSpiderAlgorithm  (Modified this version)
+    The developed version: Germinal Center Optimization (GCO)
 
     Notes
     ~~~~~
-    + The version on above github is very slow convergence
-    + Changes the idea of intensity, which one has better intensity, others will move toward to it
+    + The global best solution and 2 random solutions are used instead of randomizing 3 solutions
 
     Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
-        + r_a (float): the rate of vibration attenuation when propagating over the spider web, default=1.0
-        + p_c (float): controls the probability of the spiders changing their dimension mask in the random walk step, default=0.7
-        + p_m (float): the probability of each value in a dimension mask to be one, default=0.1
+        + cr (float): [0.5, 0.95], crossover rate, default = 0.7 (Same as DE algorithm)
+        + wf (float): [1.0, 2.0], weighting factor (f in the paper), default = 1.25 (Same as DE algorithm)
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.swarm_based.SSpiderA import OriginalSSpiderA
+    >>> from mealpy.system_based.GCO import BaseGCO
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
     >>> problem_dict1 = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
     >>> }
     >>>
     >>> epoch = 1000
     >>> pop_size = 50
-    >>> r_a = 1.0
-    >>> p_c = 0.7
-    >>> p_m = 0.1
-    >>> model = OriginalSSpiderA(epoch, pop_size, r_a, p_c, p_m)
+    >>> cr = 0.7
+    >>> wf = 1.25
+    >>> model = BaseGCO(epoch, pop_size, cr, wf)
     >>> best_position, best_fitness = model.solve(problem_dict1)
     >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
-
-    References
-    ~~~~~~~~~~
-    [1] James, J.Q. and Li, V.O., 2015. A social spider algorithm for global optimization.
-    Applied soft computing, 30, pp.614-627.
     """
 
-    ID_POS = 0
-    ID_TAR = 1
-    ID_INT = 2
-    ID_TARGET_POS = 3
-    ID_PREV_MOVE_VEC = 4
-    ID_MASK = 5
-
-    def __init__(self, epoch=10000, pop_size=100, r_a=1.0, p_c=0.7, p_m=0.1, **kwargs):
+    def __init__(self, epoch=10000, pop_size=100, cr=0.7, wf=1.25, **kwargs):
         """
         Args:
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
-            r_a (float): the rate of vibration attenuation when propagating over the spider web, default=1.0
-            p_c (float): controls the probability of the spiders changing their dimension mask in the random walk step, default=0.7
-            p_m (float): the probability of each value in a dimension mask to be one, default=0.1
+            cr (float): crossover rate, default = 0.7 (Same as DE algorithm)
+            wf (float): weighting factor (f in the paper), default = 1.25 (Same as DE algorithm)
         """
         super().__init__(**kwargs)
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
-        self.r_a = self.validator.check_float("r_a", r_a, (0, 5.0))
-        self.p_c = self.validator.check_float("p_c", p_c, (0, 1.0))
-        self.p_m = self.validator.check_float("p_m", p_m, (0, 1.0))
-        self.set_parameters(["epoch", "pop_size", "r_a", "p_c", "p_m"])
+        self.cr = self.validator.check_float("cr", cr, (0, 1.0))
+        self.wf = self.validator.check_float("wf", wf, (0, 3.0))
+        self.set_parameters(["epoch", "pop_size", "cr", "wf"])
         self.sort_flag = False
 
-    def create_solution(self, lb=None, ub=None, pos=None):
-        """
-        Overriding method in Optimizer class
-        + x: The position of s on the web.
-        + train: The fitness of the current position of s
-        + target_vibration: The target vibration of s in the previous iteration.
-        + intensity_vibration: intensity of vibration
-        + movement_vector: The movement that s performed in the previous iteration
-        + dimension_mask: The dimension mask 1 that s employed to guide movement in the previous iteration
-        + The dimension mask is a 0-1 binary vector of length problem size
-        + n_changed: The number of iterations since s has last changed its target vibration. (No need)
-
-        Returns:
-            list: wrapper of solution with format [position, target, intensity, target_position, previous_movement_vector, dimension_mask]
-        """
-        if pos is None:
-            pos = self.generate_position(lb, ub)
-        position = self.amend_position(pos, lb, ub)
-        target = self.get_target_wrapper(position)
-        intensity = np.log(1. / (abs(target[self.ID_FIT]) + self.EPSILON) + 1)
-        target_position = deepcopy(position)
-        previous_movement_vector = np.zeros(self.problem.n_dims)
-        dimension_mask = np.zeros(self.problem.n_dims)
-        return [position, target, intensity, target_position, previous_movement_vector, dimension_mask]
+    def initialize_variables(self):
+        self.dyn_list_cell_counter = np.ones(self.pop_size)  # CEll Counter
+        self.dyn_list_life_signal = 70 * np.ones(self.pop_size)  # 70% to duplicate, and 30% to die  # LIfe-Signal
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        all_pos = np.array([it[self.ID_POS] for it in self.pop])  ## Matrix (pop_size, problem_size)
-        base_distance = np.mean(np.std(all_pos, axis=0))  ## Number
-        dist = cdist(all_pos, all_pos, 'euclidean')
-
-        intensity_source = np.array([it[self.ID_INT] for it in self.pop])
-        intensity_attenuation = np.exp(-dist / (base_distance * self.r_a))  ## vector (pop_size)
-        intensity_receive = np.dot(np.reshape(intensity_source, (1, self.pop_size)), intensity_attenuation)  ## vector (1, pop_size)
-        id_best_intennsity = np.argmax(intensity_receive)
-
+        ## Dark-zone process    (can be parallelization)
         pop_new = []
         for idx in range(0, self.pop_size):
-            agent = deepcopy(self.pop[idx])
-            if self.pop[id_best_intennsity][self.ID_INT] > self.pop[idx][self.ID_INT]:
-                agent[self.ID_TARGET_POS] = self.pop[id_best_intennsity][self.ID_TARGET_POS]
-            if np.random.uniform() > self.p_c:  ## changing mask
-                agent[self.ID_MASK] = np.where(np.random.uniform(0, 1, self.problem.n_dims) < self.p_m, 0, 1)
-            pos_new = np.where(self.pop[idx][self.ID_MASK] == 0, self.pop[idx][self.ID_TARGET_POS],
-                               self.pop[np.random.randint(0, self.pop_size)][self.ID_POS])
-            ## Perform random walk
-            pos_new = self.pop[idx][self.ID_POS] + np.random.normal() * \
-                      (self.pop[idx][self.ID_POS] - self.pop[idx][self.ID_PREV_MOVE_VEC]) + \
-                      (pos_new - self.pop[idx][self.ID_POS]) * np.random.normal()
-            agent[self.ID_POS] = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+            if np.random.uniform(0, 100) < self.dyn_list_life_signal[idx]:
+                self.dyn_list_cell_counter[idx] += 1
+            else:
+                self.dyn_list_cell_counter[idx] = 1
+
+            # Mutate process
+            r1, r2 = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 2, replace=False)
+            pos_new = self.g_best[self.ID_POS] + self.wf * (self.pop[r2][self.ID_POS] - self.pop[r1][self.ID_POS])
+            condition = np.random.random(self.problem.n_dims) < self.cr
+            pos_new = np.where(condition, pos_new, self.pop[idx][self.ID_POS])
+            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+            pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
-                agent[self.ID_TAR] = self.get_target_wrapper(agent[self.ID_POS])
-                pop_new.append(agent)
+                pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_new = self.update_target_wrapper_population(pop_new)
-
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], self.pop[idx]):
-                self.pop[idx][self.ID_PREV_MOVE_VEC] = pop_new[idx][self.ID_POS] - self.pop[idx][self.ID_POS]
-                self.pop[idx][self.ID_INT] = np.log(1. / (abs(pop_new[idx][self.ID_TAR][self.ID_FIT]) + self.EPSILON) + 1)
-                self.pop[idx][self.ID_POS] = pop_new[idx][self.ID_POS]
-                self.pop[idx][self.ID_TAR] = pop_new[idx][self.ID_TAR]
+                self.dyn_list_cell_counter[idx] += 10
+                self.pop[idx] = deepcopy(pop_new[idx])
+
+        ## Light-zone process   (no needs parallelization)
+        for i in range(0, self.pop_size):
+            self.dyn_list_cell_counter[i] = 10
+            fit_list = np.array([item[self.ID_TAR][self.ID_FIT] for item in self.pop])
+            fit_max = max(fit_list)
+            fit_min = min(fit_list)
+            self.dyn_list_cell_counter[i] += 10 * (self.pop[i][self.ID_TAR][self.ID_FIT] - fit_max) / (fit_min - fit_max + self.EPSILON)
+
+
+class OriginalGCO(BaseGCO):
+    """
+    The original version of: Germinal Center Optimization (GCO)
+
+    Links:
+        1. https://doi.org/10.2991/ijcis.2018.25905179
+        2. https://www.atlantis-press.com/journals/ijcis/25905179/view
+
+    Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
+        + cr (float): [0.5, 0.95], crossover rate, default = 0.7 (Same as DE algorithm)
+        + wf (float): [1.0, 2.0], weighting factor (f in the paper), default = 1.25 (Same as DE algorithm)
+
+    Examples
+    ~~~~~~~~
+    >>> import numpy as np
+    >>> from mealpy.system_based.GCO import OriginalGCO
+    >>>
+    >>> def fitness_function(solution):
+    >>>     return np.sum(solution**2)
+    >>>
+    >>> problem_dict1 = {
+    >>>     "fit_func": fitness_function,
+    >>>     "lb": [-10, -15, -4, -2, -8],
+    >>>     "ub": [10, 15, 12, 8, 20],
+    >>>     "minmax": "min",
+    >>> }
+    >>>
+    >>> epoch = 1000
+    >>> pop_size = 50
+    >>> cr = 0.7
+    >>> wf = 1.25
+    >>> model = OriginalGCO(epoch, pop_size, cr, wf)
+    >>> best_position, best_fitness = model.solve(problem_dict1)
+    >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
+
+    References
+    ~~~~~~~~~~
+    [1] Villaseñor, C., Arana-Daniel, N., Alanis, A.Y., López-Franco, C. and Hernandez-Vargas, E.A., 2018.
+    Germinal center optimization algorithm. International Journal of Computational Intelligence Systems, 12(1), p.13.
+    """
+
+    def __init__(self, epoch=10000, pop_size=100, cr=0.7, wf=1.25, **kwargs):
+        """
+        Args:
+            epoch (int): maximum number of iterations, default = 10000
+            pop_size (int): number of population size, default = 100
+            cr (float): crossover rate, default = 0.7 (Same as DE algorithm)
+            wf (float): weighting factor (f in the paper), default = 1.25 (Same as DE algorithm)
+        """
+        super().__init__(epoch, pop_size, cr, wf, **kwargs)
+        self.support_parallel_modes = False
+
+    def evolve(self, epoch):
+        """
+        The main operations (equations) of algorithm. Inherit from Optimizer class
+
+        Args:
+            epoch (int): The current iteration
+        """
+        ## Dark-zone process    (can be parallelization)
+        for idx in range(0, self.pop_size):
+            if np.random.uniform(0, 100) < self.dyn_list_life_signal[idx]:
+                self.dyn_list_cell_counter[idx] += 1
+            elif self.dyn_list_cell_counter[idx] > 1:
+                self.dyn_list_cell_counter[idx] -= 1
+
+            # Mutate process
+            p = self.dyn_list_cell_counter / np.sum(self.dyn_list_cell_counter)
+            r1, r2, r3 = np.random.choice(list(set(range(0, self.pop_size))), 3, replace=False, p=p)
+            pos_new = self.pop[r1][self.ID_POS] + self.wf * (self.pop[r2][self.ID_POS] - self.pop[r3][self.ID_POS])
+            condition = np.random.random(self.problem.n_dims) < self.cr
+            pos_new = np.where(condition, pos_new, self.pop[idx][self.ID_POS])
+            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+            # for each pos_new, generate the fitness
+            target = self.get_target_wrapper(pos_new)
+            if self.compare_agent([pos_new, target], self.pop[idx]):
+                self.pop[idx] = [pos_new, target]
+                self.dyn_list_life_signal[idx] += 10
+
+        ## Light-zone process   (no needs parallelization)
+        self.dyn_list_life_signal -= 10
+        fit_list = np.array([item[self.ID_TAR][self.ID_FIT] for item in self.pop])
+        fit_max = np.max(fit_list)
+        fit_min = np.min(fit_list)
+        fit = (fit_list - fit_max) / (fit_min - fit_max)
+        if self.problem.minmax != 'min':
+            fit = 1 - fit
+        self.dyn_list_life_signal += 10 * fit
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/SSpiderO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/SSpiderO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/STO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/STO.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,23 +12,19 @@
     """
     The original version of: Siberian Tiger Optimization (STO)
 
     Links:
         1. https://ieeexplore.ieee.org/abstract/document/9989374
         2. https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9989374
 
-    Notes (Plagiarism):
-        0. This is really disgusting, because the source code for this algorithm is exact the same as the source code for Osprey Optimization Algorithm (OOA)
-        1. Algorithm design is very similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Coati Optimization Algorithm (CoatiOA),
-        Northern Goshawk Optimization (NGO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA),
-        Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Pelican Optimization Algorithm (POA),
-        Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
-        2. Check the matlab code of all above algorithms
-        2. Same authors, self-plagiarized article with kinda same algorithm with different meta-metaphors
-        4. Check the results of benchmark functions in the papers, they are mostly make up results
+    Notes:
+        1. This is somewhat concerning, as there appears to be a high degree of similarity between the source code for this algorithm and the Osprey Optimization Algorithm (OOA)
+        2. Algorithm design is similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Coati Optimization Algorithm (CoatiOA), Northern Goshawk Optimization (NGO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA), Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Pelican Optimization Algorithm (POA), Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
+        3. It may be useful to compare the Matlab code of this algorithm with those of the similar algorithms to ensure its accuracy and completeness.
+        4. The article may share some similarities with previous work by the same authors, further investigation may be warranted to verify the benchmark results reported in the papers and ensure their reliability and accuracy.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.swarm_based.STO import OriginalSTO
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/SeaHO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/SeaHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/ServalOA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/ServalOA.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,19 @@
 class OriginalServalOA(Optimizer):
     """
     The original version of: Serval Optimization Algorithm (ServalOA)
 
     Links:
         1. https://www.mdpi.com/2313-7673/7/4/204
 
-    Notes (Plagiarism):
-        0. It's really horrible, it's like he's copying and pasting all the garbage algorithms that he invented. They are almost the same.
-        1. Algorithm design is very similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Coati Optimization Algorithm (CoatiOA),
-        Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Pelican Optimization Algorithm (POA), Walrus Optimization Algorithm (WOA),
-        Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Northern goshawk optimization (NGO),
-        Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
-        2. Check the matlab code of all above algorithms
-        2. Same authors, self-plagiarized article with kinda same algorithm with different meta-metaphors
-        4. Check the results of benchmark functions in the papers, they are mostly make up results
+    Notes:
+        0. It's concerning that the author seems to be reusing the same algorithms with minor variations.
+        1. Algorithm design is similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Coati Optimization Algorithm (CoatiOA), Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Pelican Optimization Algorithm (POA), Walrus Optimization Algorithm (WOA), Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Northern goshawk optimization (NGO), Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
+        3. It may be useful to compare the Matlab code of this algorithm with those of the similar algorithms to ensure its accuracy and completeness.
+        4. The article may share some similarities with previous work by the same authors, further investigation may be warranted to verify the benchmark results reported in the papers and ensure their reliability and accuracy.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.swarm_based.ServalOA import OriginalServalOA
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/TDO.py` & `mealpy-2.5.4a1/mealpy/swarm_based/TSO.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,108 +1,129 @@
 #!/usr/bin/env python
-# Created by "Thieu" at 00:08, 27/10/2022 ----------%                                                                               
+# Created by "Thieu" at 17:52, 21/05/2022 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from mealpy.optimizer import Optimizer
 
 
-class OriginalTDO(Optimizer):
+class OriginalTSO(Optimizer):
     """
-    The original version of: Tasmanian Devil Optimization (TDO)
+    The original version of: Tuna Swarm Optimization (TSO)
 
     Links:
-        1. https://www.mathworks.com/matlabcentral/fileexchange/111380-tasmanian-devil-optimization-tdo
-        2. https://ieeexplore.ieee.org/abstract/document/9714388
+        1. https://www.hindawi.com/journals/cin/2021/9210050/
+        2. https://www.mathworks.com/matlabcentral/fileexchange/101734-tuna-swarm-optimization
 
-    Notes (Plagiarism):
-        0. This is really disgusting, because the source code for this algorithm is almost exactly the same as the source code of Osprey Optimization Algorithm
-        1. Algorithm design is very similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Pelican optimization algorithm (POA),
-        Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA),
-        Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Northern goshawk optimization (NGO),
-        Osprey Optimization Algorithm (OOA), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
-        2. Check the matlab code of all above algorithms
-        2. Same authors, self-plagiarized article with kinda same algorithm with different meta-metaphors
-        4. Check the results of benchmark functions in the papers, they are mostly make up results
+    Notes:
+        1. Two variables that authors consider it as a constants (aa = 0.7 and zz = 0.05)
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.swarm_based.TDO import OriginalTDO
+    >>> from mealpy.swarm_based.TSO import OriginalTSO
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
     >>> problem_dict1 = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
     >>> }
     >>>
     >>> epoch = 1000
     >>> pop_size = 50
-    >>> model = OriginalTDO(epoch, pop_size)
+    >>> model = OriginalTSO(epoch, pop_size)
     >>> best_position, best_fitness = model.solve(problem_dict1)
     >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
 
     References
     ~~~~~~~~~~
-    [1] Dehghani, M., Hubálovský, Š., & Trojovský, P. (2022). Tasmanian devil optimization: a new bio-inspired
-    optimization algorithm for solving optimization algorithm. IEEE Access, 10, 19599-19620.
+    [1] Xie, L., Han, T., Zhou, H., Zhang, Z. R., Han, B., & Tang, A. (2021). Tuna swarm optimization: a novel swarm-based
+    metaheuristic algorithm for global optimization. Computational intelligence and Neuroscience, 2021.
     """
+
     def __init__(self, epoch=10000, pop_size=100, **kwargs):
         """
         Args:
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
         """
         super().__init__(**kwargs)
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
         self.set_parameters(["epoch", "pop_size"])
-        self.support_parallel_modes = False
-        self.sort_flag = False
+        self.P = np.arange(1, 361)
+        self.sort_flag = True
+
+    def initialize_variables(self):
+        self.aa = 0.7
+        self.zz = 0.05
+
+    def get_new_local_pos__(self, C, a1, a2, t, epoch):
+        if np.random.rand() < self.zz:
+            local_pos = self.generate_position(self.problem.lb, self.problem.ub)
+        else:
+            if np.random.rand() < 0.5:
+                r1 = np.random.rand()
+                beta = np.exp(r1 * np.exp(3*np.cos(np.pi*((self.epoch - epoch) / self.epoch)))) * np.cos(2*np.pi*r1)
+                if np.random.rand() < C:
+                    local_pos = a1*(self.g_best[self.ID_POS] + beta * np.abs(self.g_best[self.ID_POS] - self.pop[0][self.ID_POS])) + \
+                        a2 * self.pop[0][self.ID_POS]       # Equation (8.3)
+                else:
+                    rand_pos = self.generate_position(self.problem.lb, self.problem.ub)
+                    local_pos = a1 * (rand_pos + beta*np.abs(rand_pos - self.pop[0][self.ID_POS])) + a2 * self.pop[0][self.ID_POS]  # Equation (8.1)
+            else:
+                tf = np.random.choice([-1, 1])
+                if np.random.rand() < 0.5:
+                    local_pos = tf * t**2 * self.pop[0][self.ID_POS]        # Eq 9.2
+                else:
+                    local_pos = self.g_best[self.ID_POS] + np.random.rand(self.problem.n_dims) * (self.g_best[self.ID_POS] - self.pop[0][self.ID_POS]) + \
+                        tf * t**2 * (self.g_best[self.ID_POS] - self.pop[0][self.ID_POS])
+        return local_pos
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
+        C = (epoch + 1) / self.epoch
+        a1 = self.aa + (1 - self.aa) * C
+        a2 = (1 - self.aa) - (1 - self.aa) * C
+        t = (1 - (epoch+1) / self.epoch) ** ((epoch+1) / self.epoch)
+
+        pop_new = []
         for idx in range(0, self.pop_size):
-            # PHASE1: Hunting Feeding
-            if np.random.rand() > 0.5:
-                # STRATEGY 1: FEEDING BY EATING CARRION (EXPLORATION PHASE)
-                # CARRION selection using (3)
-                kk = np.random.choice(list(set(range(0, self.pop_size)) - {idx}))
-                if self.compare_agent(self.pop[kk], self.pop[idx]):
-                    pos_new = self.pop[idx][self.ID_POS] + np.random.rand(self.problem.n_dims) * (self.pop[kk][self.ID_POS] - np.random.randint(1, 3)*self.pop[idx][self.ID_POS])
-                else:
-                    pos_new = self.pop[idx][self.ID_POS] + np.random.rand(self.problem.n_dims) * (self.pop[idx][self.ID_POS] - self.pop[kk][self.ID_POS])
-                pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-                tar_new = self.get_target_wrapper(pos_new)
-                if self.compare_agent([pos_new, tar_new], self.pop[idx]):
-                    self.pop[idx] = [pos_new, tar_new]
+            if idx == 0:
+                pos_new = self.get_new_local_pos__(C, a1, a2, t, epoch)
             else:
-            # STRATEGY 2: FEEDING BY EATING PREY (EXPLOITATION PHASE)
-            # stage1: prey selection and attack it
-                kk = np.random.choice(list(set(range(0, self.pop_size)) - {idx}))
-                if self.compare_agent(self.pop[kk], self.pop[idx]):
-                    pos_new = self.pop[idx][self.ID_POS] + np.random.rand(self.problem.n_dims) * (self.pop[kk][self.ID_POS] - np.random.randint(1, 3) * self.pop[idx][self.ID_POS])
+                if np.random.rand() < self.zz:
+                    pos_new = self.generate_position(self.problem.lb, self.problem.ub)
                 else:
-                    pos_new = self.pop[idx][self.ID_POS] + np.random.rand(self.problem.n_dims) * (self.pop[idx][self.ID_POS] - self.pop[kk][self.ID_POS])
-                pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-                tar_new = self.get_target_wrapper(pos_new)
-                if self.compare_agent([pos_new, tar_new], self.pop[idx]):
-                    self.pop[idx] = [pos_new, tar_new]
-
-            # stage2: prey chasing
-            rr = 0.01 * (1 - (epoch+1)/self.epoch)      # Calculating the neighborhood radius using(9)
-            pos_new = self.pop[idx][self.ID_POS] + (-rr + 2 * rr * np.random.rand(self.problem.n_dims)) * self.pop[idx][self.ID_POS]
+                    if np.random.rand() > 0.5:
+                        r1 = np.random.rand()
+                        beta = np.exp(r1 * np.exp(3*np.cos(np.pi * (self.epoch - epoch)/self.epoch))) * np.cos(2*np.pi*r1)
+                        if np.random.rand() < C:
+                            pos_new = a1 * (self.g_best[self.ID_POS] + beta*np.abs(self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])) + \
+                                a2 * self.pop[idx-1][self.ID_POS]       # Eq. 8.4
+                        else:
+                            rand_pos = self.generate_position(self.problem.lb, self.problem.ub)
+                            pos_new = a1 * (rand_pos + beta*np.abs(rand_pos - self.pop[idx][self.ID_POS])) + a2 * self.pop[idx-1][self.ID_POS]  # Eq 8.2
+                    else:
+                        tf = np.random.choice([-1, 1])
+                        if np.random.rand() < 0.5:
+                            pos_new = self.g_best[self.ID_POS] + \
+                                      np.random.rand(self.problem.n_dims) * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS]) +\
+                                      tf * t**2 * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])       # Eq 9.1
+                        else:
+                            pos_new = tf * t**2 * self.pop[idx][self.ID_POS]        # Eq 9.2
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-            tar_new = self.get_target_wrapper(pos_new)
-            if self.compare_agent([pos_new, tar_new], self.pop[idx]):
-                self.pop[idx] = [pos_new, tar_new]
+            pop_new.append([pos_new, None])
+            if self.mode not in self.AVAILABLE_MODES:
+                pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
+        self.pop = self.update_target_wrapper_population(pop_new)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/TSO.py` & `mealpy-2.5.4a1/mealpy/system_based/WCA.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,129 +1,150 @@
 #!/usr/bin/env python
-# Created by "Thieu" at 17:52, 21/05/2022 ----------%                                                                               
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
+# Created by "Thieu" at 09:55, 02/03/2021 ----------%
+#       Email: nguyenthieu2102@gmail.com            %
+#       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
+from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
-class OriginalTSO(Optimizer):
+class OriginalWCA(Optimizer):
     """
-    The original version of: Tuna Swarm Optimization (TSO)
+    The original version of: Water Cycle Algorithm (WCA)
 
     Links:
-        1. https://www.hindawi.com/journals/cin/2021/9210050/
-        2. https://www.mathworks.com/matlabcentral/fileexchange/101734-tuna-swarm-optimization
+        1. https://doi.org/10.1016/j.compstruc.2012.07.010
 
-    Notes:
-        1. Two variables that authors consider it as a constants (aa = 0.7 and zz = 0.05)
+    Notes
+    ~~~~~
+    The ideas are (almost the same as ICO algorithm):
+        + 1 sea is global best solution
+        + a few river which are second, third, ...
+        + other left are stream (will flow directed to sea or river)
+
+    Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
+        + nsr (int): [4, 10], Number of rivers + sea (sea = 1), default = 4
+        + wc (float): [1.0, 3.0], Weighting coefficient (C in the paper), default = 2
+        + dmax (float): [1e-6], fixed parameter, Evaporation condition constant, default=1e-6
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.swarm_based.TSO import OriginalTSO
+    >>> from mealpy.system_based.WCA import OriginalWCA
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
     >>> problem_dict1 = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
     >>> }
     >>>
     >>> epoch = 1000
     >>> pop_size = 50
-    >>> model = OriginalTSO(epoch, pop_size)
+    >>> nsr = 4
+    >>> wc = 2.0
+    >>> dmax = 1e-6
+    >>> model = OriginalWCA(epoch, pop_size, nsr, wc, dmax)
     >>> best_position, best_fitness = model.solve(problem_dict1)
     >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
 
     References
     ~~~~~~~~~~
-    [1] Xie, L., Han, T., Zhou, H., Zhang, Z. R., Han, B., & Tang, A. (2021). Tuna swarm optimization: a novel swarm-based
-    metaheuristic algorithm for global optimization. Computational intelligence and Neuroscience, 2021.
+    [1] Eskandar, H., Sadollah, A., Bahreininejad, A. and Hamdi, M., 2012. Water cycle algorithm–A novel metaheuristic
+    optimization method for solving constrained engineering optimization problems. Computers & Structures, 110, pp.151-166.
     """
 
-    def __init__(self, epoch=10000, pop_size=100, **kwargs):
+    def __init__(self, epoch=10000, pop_size=100, nsr=4, wc=2.0, dmax=1e-6, **kwargs):
         """
         Args:
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
+            nsr (int): Number of rivers + sea (sea = 1), default = 4
+            wc (float): Weighting coefficient (C in the paper), default = 2.0
+            dmax (float): Evaporation condition constant, default=1e-6
         """
         super().__init__(**kwargs)
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
-        self.set_parameters(["epoch", "pop_size"])
-        self.P = np.arange(1, 361)
+        self.nsr = self.validator.check_int("nsr", nsr, [2, int(self.pop_size/2)])
+        self.wc = self.validator.check_float("wc", wc, (1.0, 3.0))
+        self.dmax = self.validator.check_float("dmax", dmax, (0, 1.0))
+        self.set_parameters(["epoch", "pop_size", "nsr", "wc", "dmax"])
         self.sort_flag = True
 
-    def initialize_variables(self):
-        self.aa = 0.7
-        self.zz = 0.05
-
-    def get_new_local_pos__(self, C, a1, a2, t, epoch):
-        if np.random.rand() < self.zz:
-            local_pos = self.generate_position(self.problem.lb, self.problem.ub)
-        else:
-            if np.random.rand() < 0.5:
-                r1 = np.random.rand()
-                beta = np.exp(r1 * np.exp(3*np.cos(np.pi*((self.epoch - epoch) / self.epoch)))) * np.cos(2*np.pi*r1)
-                if np.random.rand() < C:
-                    local_pos = a1*(self.g_best[self.ID_POS] + beta * np.abs(self.g_best[self.ID_POS] - self.pop[0][self.ID_POS])) + \
-                        a2 * self.pop[0][self.ID_POS]       # Equation (8.3)
-                else:
-                    rand_pos = self.generate_position(self.problem.lb, self.problem.ub)
-                    local_pos = a1 * (rand_pos + beta*np.abs(rand_pos - self.pop[0][self.ID_POS])) + a2 * self.pop[0][self.ID_POS]  # Equation (8.1)
-            else:
-                tf = np.random.choice([-1, 1])
-                if np.random.rand() < 0.5:
-                    local_pos = tf * t**2 * self.pop[0][self.ID_POS]        # Eq 9.2
-                else:
-                    local_pos = self.g_best[self.ID_POS] + np.random.rand(self.problem.n_dims) * (self.g_best[self.ID_POS] - self.pop[0][self.ID_POS]) + \
-                        tf * t**2 * (self.g_best[self.ID_POS] - self.pop[0][self.ID_POS])
-        return local_pos
+    def initialization(self):
+        if self.pop is None:
+            self.pop = self.create_population(self.pop_size)
+        self.pop, self.g_best = self.get_global_best_solution(self.pop)
+        self.ecc = self.dmax  # Evaporation condition constant - variable
+        n_stream = self.pop_size - self.nsr
+        g_best = deepcopy(self.pop[0])  # Global best solution (sea)
+        self.pop_best = deepcopy(self.pop[:self.nsr])  # Including sea and river (1st solution is sea)
+        self.pop_stream = deepcopy(self.pop[self.nsr:])  # Forming Stream
+
+        # Designate streams to rivers and sea
+        cost_river_list = np.array([solution[self.ID_TAR][self.ID_FIT] for solution in self.pop_best])
+        num_child_in_river_list = np.round(np.abs(cost_river_list / np.sum(cost_river_list)) * n_stream).astype(int)
+        if np.sum(num_child_in_river_list) < n_stream:
+            num_child_in_river_list[-1] += n_stream - np.sum(num_child_in_river_list)
+        streams = {}
+        idx_already_selected = []
+        for i in range(0, self.nsr - 1):
+            streams[i] = []
+            idx_list = np.random.choice(list(set(range(0, n_stream)) - set(idx_already_selected)), num_child_in_river_list[i], replace=False).tolist()
+            idx_already_selected += idx_list
+            for idx in idx_list:
+                streams[i].append(self.pop_stream[idx])
+        idx_last = list(set(range(0, n_stream)) - set(idx_already_selected))
+        streams[self.nsr - 1] = []
+        for idx in idx_last:
+            streams[self.nsr - 1].append(self.pop_stream[idx])
+        self.streams = streams
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        C = (epoch + 1) / self.epoch
-        a1 = self.aa + (1 - self.aa) * C
-        a2 = (1 - self.aa) - (1 - self.aa) * C
-        t = (1 - (epoch+1) / self.epoch) ** ((epoch+1) / self.epoch)
-
-        pop_new = []
-        for idx in range(0, self.pop_size):
-            if idx == 0:
-                pos_new = self.get_new_local_pos__(C, a1, a2, t, epoch)
-            else:
-                if np.random.rand() < self.zz:
-                    pos_new = self.generate_position(self.problem.lb, self.problem.ub)
-                else:
-                    if np.random.rand() > 0.5:
-                        r1 = np.random.rand()
-                        beta = np.exp(r1 * np.exp(3*np.cos(np.pi * (self.epoch - epoch)/self.epoch))) * np.cos(2*np.pi*r1)
-                        if np.random.rand() < C:
-                            pos_new = a1 * (self.g_best[self.ID_POS] + beta*np.abs(self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])) + \
-                                a2 * self.pop[idx-1][self.ID_POS]       # Eq. 8.4
-                        else:
-                            rand_pos = self.generate_position(self.problem.lb, self.problem.ub)
-                            pos_new = a1 * (rand_pos + beta*np.abs(rand_pos - self.pop[idx][self.ID_POS])) + a2 * self.pop[idx-1][self.ID_POS]  # Eq 8.2
-                    else:
-                        tf = np.random.choice([-1, 1])
-                        if np.random.rand() < 0.5:
-                            pos_new = self.g_best[self.ID_POS] + \
-                                      np.random.rand(self.problem.n_dims) * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS]) +\
-                                      tf * t**2 * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])       # Eq 9.1
-                        else:
-                            pos_new = tf * t**2 * self.pop[idx][self.ID_POS]        # Eq 9.2
+        # Update stream and river
+        for idx, stream_list in self.streams.items():
+            # Update stream
+            stream_new = []
+            for idx_stream, stream in enumerate(stream_list):
+                pos_new = stream[self.ID_POS] + np.random.uniform() * self.wc * (self.pop_best[idx][self.ID_POS] - stream[self.ID_POS])
+                pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+                stream_new.append([pos_new, None])
+                if self.mode not in self.AVAILABLE_MODES:
+                    stream_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
+            stream_new = self.update_target_wrapper_population(stream_new)
+            stream_new, stream_best = self.get_global_best_solution(stream_new)
+            self.streams[idx] = stream_new
+            if self.compare_agent(stream_best, self.pop_best[idx]):
+                self.pop_best[idx] = deepcopy(stream_best)
+
+            # Update river
+            pos_new = self.pop_best[idx][self.ID_POS] + np.random.uniform() * self.wc * (self.g_best[self.ID_POS] - self.pop_best[idx][self.ID_POS])
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-            pop_new.append([pos_new, None])
-            if self.mode not in self.AVAILABLE_MODES:
-                pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
-        self.pop = self.update_target_wrapper_population(pop_new)
+            target = self.get_target_wrapper(pos_new)
+            if self.compare_agent([pos_new, target], self.pop_best[idx]):
+                self.pop_best[idx] = [pos_new, target]
+
+        # Evaporation
+        for i in range(1, self.nsr):
+            distance = np.sqrt(np.sum((self.g_best[self.ID_POS] - self.pop_best[i][self.ID_POS]) ** 2))
+            if distance < self.ecc or np.random.rand() < 0.1:
+                child = self.create_solution(self.problem.lb, self.problem.ub)
+                pop_current_best, _ = self.get_global_best_solution(self.streams[i] + [child])
+                self.pop_best[i] = pop_current_best.pop(0)
+                self.streams[i] = pop_current_best
+        self.pop = deepcopy(self.pop_best)
+        for idx, stream_list in self.streams.items():
+            self.pop += stream_list
+        # Reduce the ecc
+        self.ecc = self.ecc - self.ecc / self.epoch
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/WOA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/WOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/WaOA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/WaOA.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,23 +11,19 @@
 class OriginalWaOA(Optimizer):
     """
     The original version of: Walrus Optimization Algorithm (WaOA)
 
     Links:
         1. https://www.researchgate.net/publication/364684780_Walrus_Optimization_Algorithm_A_New_Bio-Inspired_Metaheuristic_Algorithm
 
-    Notes (Plagiarism):
-        0. This is really disgusting, because the source code for this algorithm is exactly the same as the source code of Northern Goshawk Optimization (NGO)
-        1. Algorithm design is very similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Coati Optimization Algorithm (CoatiOA),
-        Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Northern Goshawk Optimization (NGO),
-        Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Pelican Optimization Algorithm (POA),
-        Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
-        2. Check the matlab code of all above algorithms
-        2. Same authors, self-plagiarized article with kinda same algorithm with different meta-metaphors
-        4. Check the results of benchmark functions in the papers, they are mostly make up results
+    Notes:
+        1. This is somewhat concerning, as there appears to be a high degree of similarity between the source code for this algorithm and the Northern Goshawk Optimization (NGO)
+        2. Algorithm design is similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Coati Optimization Algorithm (CoatiOA), Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Northern Goshawk Optimization (NGO), Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Pelican Optimization Algorithm (POA), Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
+        3. It may be useful to compare the Matlab code of this algorithm with those of the similar algorithms to ensure its accuracy and completeness.
+        4. The article may share some similarities with previous work by the same authors, further investigation may be warranted to verify the benchmark results reported in the papers and ensure their reliability and accuracy.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.swarm_based.WaOA import OriginalWaOA
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/swarm_based/ZOA.py` & `mealpy-2.5.4a1/mealpy/swarm_based/ZOA.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,22 +12,19 @@
     """
     The original version of: Zebra Optimization Algorithm (ZOA)
 
     Links:
         1. https://ieeexplore.ieee.org/document/9768820
         2. https://www.mathworks.com/matlabcentral/fileexchange/122942-zebra-optimization-algorithm-zoa
 
-    Notes (Plagiarism):
-        1. Algorithm design is very similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Pelican optimization algorithm (POA),
-        Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA),
-        Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Northern goshawk optimization (NGO),
-        Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO)
-        2. Check the matlab code of all above algorithms
-        2. Same authors, self-plagiarized article with kinda same algorithm with different meta-metaphors
-        4. Check the results of benchmark functions in the papers, they are mostly make up results
+    Notes:
+		1. It's concerning that the author seems to be reusing the same algorithms with minor variations.
+        2. Algorithm design is similar to Zebra Optimization Algorithm (ZOA), Osprey Optimization Algorithm (OOA), Pelican optimization algorithm (POA), Siberian Tiger Optimization (STO), Language Education Optimization (LEO), Serval Optimization Algorithm (SOA), Walrus Optimization Algorithm (WOA), Fennec Fox Optimization (FFO), Three-periods optimization algorithm (TPOA), Teamwork optimization algorithm (TOA), Northern goshawk optimization (NGO), Tasmanian devil optimization (TDO), Archery algorithm (AA), Cat and mouse based optimizer (CMBO).
+        3. It may be useful to compare the Matlab code of this algorithm with those of the similar algorithms to ensure its accuracy and completeness.
+        4. The article may share some similarities with previous work by the same authors, further investigation may be warranted to verify the benchmark results reported in the papers and ensure their reliability and accuracy.
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
     >>> from mealpy.swarm_based.ZOA import OriginalZOA
     >>>
     >>> def fitness_function(solution):
```

### Comparing `mealpy-2.5.3a1/mealpy/system_based/AEO.py` & `mealpy-2.5.4a1/mealpy/system_based/AEO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/system_based/GCO.py` & `mealpy-2.5.4a1/mealpy/utils/problem.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,194 +1,200 @@
 #!/usr/bin/env python
-# Created by "Thieu" at 16:44, 18/03/2020 ----------%
-#       Email: nguyenthieu2102@gmail.com            %
-#       Github: https://github.com/thieu1995        %
+# Created by "Thieu" at 17:28, 13/10/2021 ----------%
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
-from mealpy.optimizer import Optimizer
+from mealpy.utils.logger import Logger
 
 
-class BaseGCO(Optimizer):
-    """
-    The developed version: Germinal Center Optimization (GCO)
+class Problem:
+    """Class representing the mathematical form of the optimization problem.
+
+    Attributes:
+        lb (numpy.ndarray, list, tuple): Lower bounds of the problem.
+        ub (numpy.ndarray, list, tuple): Upper bounds of the problem.
+        minmax (str): Minimization or maximization problem (min, max), default = "min"
 
     Notes
     ~~~~~
-    + The global best solution and 2 random solutions are used instead of randomizing 3 solutions
-
-    Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
-        + cr (float): [0.5, 0.95], crossover rate, default = 0.7 (Same as DE algorithm)
-        + wf (float): [1.0, 2.0], weighting factor (f in the paper), default = 1.25 (Same as DE algorithm)
+    + fit_func (callable): your fitness function
+    + lb (list, int, float): lower bound, should be list of values
+    + ub (list, int, float): upper bound, should be list of values
+    + minmax (str): "min" or "max" problem (Optional, default = "min")
+    + obj_weights: list weights for all your objectives (Optional, default = [1, 1, ...1])
+    + save_population (bool): save history of population or not, default = True (Optional). **Warning**:
+        + this parameter can save you from error related to 'memory' when your model is too big (i.e, training neural network, ...)
+        + when set to False, you can't use the function draw trajectory chart in history object (model.history.save_trajectory_chart)
+    + amend_position(callable): Depend on your problem, may need to design an amend_position function (Optional for continuous domain, Required for discrete domain)
 
     Examples
     ~~~~~~~~
     >>> import numpy as np
-    >>> from mealpy.system_based.GCO import BaseGCO
+    >>> from mealpy.swarm_based.PSO import OriginalPSO
     >>>
     >>> def fitness_function(solution):
     >>>     return np.sum(solution**2)
     >>>
-    >>> problem_dict1 = {
+    >>> problem_dict = {
     >>>     "fit_func": fitness_function,
     >>>     "lb": [-10, -15, -4, -2, -8],
     >>>     "ub": [10, 15, 12, 8, 20],
     >>>     "minmax": "min",
+    >>>     "log_to": None,
+    >>>     "save_population": False,
     >>> }
+    >>> model1 = OriginalPSO(epoch=1000, pop_size=50)
+    >>> model1.solve(problem_dict)
+    >>>
+    >>> ## For discrete problem, you need to design an amend_position function that can (1) bring your solution back to the valid range,
+    >>> ##    (2) can convert float number into integer number (combinatorial or permutation).
+    >>>
+    >>> def amend_position(solution, lb, ub):
+    >>>     ## Bring them back to valid range
+    >>>     solution = np.clip(solution, lb, ub)
+    >>>     ## Convert float to integer number
+    >>>     solution_int = solution.astype(int)
+    >>>     ## If the designed solution is permutation, then need an extra step here
+    >>>     ## .... Do it here and then return the valid solution
+    >>>     return solution_int
     >>>
-    >>> epoch = 1000
-    >>> pop_size = 50
-    >>> cr = 0.7
-    >>> wf = 1.25
-    >>> model = BaseGCO(epoch, pop_size, cr, wf)
-    >>> best_position, best_fitness = model.solve(problem_dict1)
-    >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
+    >>> problem_dict2 = {
+    >>>     "fit_func": fitness_function,
+    >>>     "lb": [-100, ] * 30,
+    >>>     "ub": [100, ] * 30,
+    >>>     "minmax": "min",
+    >>>     "log_to": "file",
+    >>>     "log_file": "records.log",
+    >>>     "amend_position": amend_position
+    >>> }
+    >>> model2 = OriginalPSO(epoch=1000, pop_size=50)
+    >>> best_position, best_fitness = model2.solve(problem_dict2)
+    >>> print(f"Best solution: {best_position}, Best fitness: {best_fitness}")
     """
 
-    def __init__(self, epoch=10000, pop_size=100, cr=0.7, wf=1.25, **kwargs):
-        """
-        Args:
-            epoch (int): maximum number of iterations, default = 10000
-            pop_size (int): number of population size, default = 100
-            cr (float): crossover rate, default = 0.7 (Same as DE algorithm)
-            wf (float): weighting factor (f in the paper), default = 1.25 (Same as DE algorithm)
-        """
-        super().__init__(**kwargs)
-        self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
-        self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
-        self.cr = self.validator.check_float("cr", cr, (0, 1.0))
-        self.wf = self.validator.check_float("wf", wf, (0, 3.0))
-        self.set_parameters(["epoch", "pop_size", "cr", "wf"])
-        self.sort_flag = False
-
-    def initialize_variables(self):
-        self.dyn_list_cell_counter = np.ones(self.pop_size)  # CEll Counter
-        self.dyn_list_life_signal = 70 * np.ones(self.pop_size)  # 70% to duplicate, and 30% to die  # LIfe-Signal
+    SUPPORTED_ARRAY = (list, tuple, np.ndarray)
 
-    def evolve(self, epoch):
-        """
-        The main operations (equations) of algorithm. Inherit from Optimizer class
+    def __init__(self, lb=None, ub=None, minmax="min", **kwargs):
+        r"""Initialize Problem.
 
         Args:
-            epoch (int): The current iteration
-        """
-        ## Dark-zone process    (can be parallelization)
-        pop_new = []
-        for idx in range(0, self.pop_size):
-            if np.random.uniform(0, 100) < self.dyn_list_life_signal[idx]:
-                self.dyn_list_cell_counter[idx] += 1
+            lb (numpy.ndarray, list, tuple): Lower bounds of the problem.
+            ub (numpy.ndarray, list, tuple): Upper bounds of the problem.
+            minmax (str): Minimization or maximization problem (min, max)
+            name (str): Name for this particular problem
+        """
+        self.name, self.log_to, self.log_file = "P", "console", "history.txt"
+        self.n_objs, self.obj_is_list, self.multi_objs, self.obj_weights = 1, False, False, None
+        self.n_dims, self.lb, self.ub, self.save_population = None, None, None, False
+
+        self.__set_keyword_arguments(kwargs)
+        self.__set_domain_range(lb, ub)
+        self.__set_functions(kwargs)
+        self.logger = Logger(self.log_to, log_file=self.log_file).create_logger(name=f"{__name__}.{__class__.__name__}",
+                                    format_str='%(asctime)s, %(levelname)s, %(name)s [line: %(lineno)d]: %(message)s')
+        self.minmax = minmax
+
+    def __set_keyword_arguments(self, kwargs):
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
+    def __set_domain_range(self, lb, ub):
+        if type(lb) in self.SUPPORTED_ARRAY and type(ub) in self.SUPPORTED_ARRAY:
+            self.lb = np.array(lb).flatten()
+            self.ub = np.array(ub).flatten()
+            if len(self.lb) == len(self.ub):
+                self.n_dims = len(self.lb)
+                if len(self.lb) < 1:
+                    raise ValueError(f'Dimensions do not qualify. Length(lb) = {len(self.lb)} < 1.')
+            else:
+                raise ValueError(f"Length of lb and ub do not match. {len(self.lb)} != {len(self.ub)}.")
+        else:
+            raise ValueError(f"lb and ub need to be a list, tuple or np.array.")
+
+    def __set_functions(self, kwargs):
+        tested_solution = self.generate_position(self.lb, self.ub)
+        if "amend_position" in kwargs:
+            if not callable(self.amend_position):
+                raise ValueError(f"Use default 'amend_position()' or passed a callable function. {type(self.amend_position)} != function")
+            else:
+                tested_solution = self.amend_position(tested_solution, self.lb, self.ub)
+        result = self.fit_func(tested_solution)
+        if type(result) in self.SUPPORTED_ARRAY:
+            result = np.array(result).flatten()
+            self.n_objs = len(result)
+            self.obj_is_list = True
+            if self.n_objs > 1:
+                self.multi_objs = True
+                if type(self.obj_weights) in self.SUPPORTED_ARRAY:
+                    self.obj_weights = np.array(self.obj_weights).flatten()
+                    if self.n_objs != len(self.obj_weights):
+                        raise ValueError(f"{self.n_objs}-objective problem, but N weights = {len(self.obj_weights)}.")
+                    self.msg = f"Solving {self.n_objs}-objective optimization problem with weights: {self.obj_weights}."
+                else:
+                    raise ValueError(f"Solving {self.n_objs}-objective optimization, need to set obj_weights list with length: {self.n_objs}")
+            elif self.n_objs == 1:
+                self.multi_objs = False
+                self.obj_weights = np.ones(1)
+                self.msg = f"Solving single objective optimization problem."
             else:
-                self.dyn_list_cell_counter[idx] = 1
+                raise ValueError(f"fit_func needs to return a single value or a list of values list")
+        elif type(result) in (int, float) or isinstance(result, np.floating) or isinstance(result, np.integer):
+            self.multi_objs = False
+            self.obj_is_list = False
+            self.obj_weights = np.ones(1)
+            self.msg = f"Solving single objective optimization problem."
+        else:
+            raise ValueError(f"fit_func needs to return a single value or a list of values list")
 
-            # Mutate process
-            r1, r2 = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 2, replace=False)
-            pos_new = self.g_best[self.ID_POS] + self.wf * (self.pop[r2][self.ID_POS] - self.pop[r1][self.ID_POS])
-            condition = np.random.random(self.problem.n_dims) < self.cr
-            pos_new = np.where(condition, pos_new, self.pop[idx][self.ID_POS])
-            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-            pop_new.append([pos_new, None])
-            if self.mode not in self.AVAILABLE_MODES:
-                pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
-        pop_new = self.update_target_wrapper_population(pop_new)
-        for idx in range(0, self.pop_size):
-            if self.compare_agent(pop_new[idx], self.pop[idx]):
-                self.dyn_list_cell_counter[idx] += 10
-                self.pop[idx] = deepcopy(pop_new[idx])
-
-        ## Light-zone process   (no needs parallelization)
-        for i in range(0, self.pop_size):
-            self.dyn_list_cell_counter[i] = 10
-            fit_list = np.array([item[self.ID_TAR][self.ID_FIT] for item in self.pop])
-            fit_max = max(fit_list)
-            fit_min = min(fit_list)
-            self.dyn_list_cell_counter[i] += 10 * (self.pop[i][self.ID_TAR][self.ID_FIT] - fit_max) / (fit_min - fit_max + self.EPSILON)
+    def fit_func(self, x):
+        """Fitness function
 
+        Args:
+            x (numpy.ndarray): Solution.
 
-class OriginalGCO(BaseGCO):
-    """
-    The original version of: Germinal Center Optimization (GCO)
+        Returns:
+            float: Function value of `x`.
+        """
+        raise NotImplementedError
 
-    Links:
-        1. https://doi.org/10.2991/ijcis.2018.25905179
-        2. https://www.atlantis-press.com/journals/ijcis/25905179/view
-
-    Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
-        + cr (float): [0.5, 0.95], crossover rate, default = 0.7 (Same as DE algorithm)
-        + wf (float): [1.0, 2.0], weighting factor (f in the paper), default = 1.25 (Same as DE algorithm)
+    def get_name(self):
+        """
+        Returns:
+            string: The name of the problem
+        """
+        return self.name
 
-    Examples
-    ~~~~~~~~
-    >>> import numpy as np
-    >>> from mealpy.system_based.GCO import OriginalGCO
-    >>>
-    >>> def fitness_function(solution):
-    >>>     return np.sum(solution**2)
-    >>>
-    >>> problem_dict1 = {
-    >>>     "fit_func": fitness_function,
-    >>>     "lb": [-10, -15, -4, -2, -8],
-    >>>     "ub": [10, 15, 12, 8, 20],
-    >>>     "minmax": "min",
-    >>> }
-    >>>
-    >>> epoch = 1000
-    >>> pop_size = 50
-    >>> cr = 0.7
-    >>> wf = 1.25
-    >>> model = OriginalGCO(epoch, pop_size, cr, wf)
-    >>> best_position, best_fitness = model.solve(problem_dict1)
-    >>> print(f"Solution: {best_position}, Fitness: {best_fitness}")
-
-    References
-    ~~~~~~~~~~
-    [1] Villaseñor, C., Arana-Daniel, N., Alanis, A.Y., López-Franco, C. and Hernandez-Vargas, E.A., 2018.
-    Germinal center optimization algorithm. International Journal of Computational Intelligence Systems, 12(1), p.13.
-    """
+    def get_class_name(self):
+        """Get class name."""
+        return self.__class__.__name__
 
-    def __init__(self, epoch=10000, pop_size=100, cr=0.7, wf=1.25, **kwargs):
+    def generate_position(self, lb=None, ub=None):
         """
+        Generate the position depends on the problem. For discrete problem such as permutation, this method can be override.
+
         Args:
-            epoch (int): maximum number of iterations, default = 10000
-            pop_size (int): number of population size, default = 100
-            cr (float): crossover rate, default = 0.7 (Same as DE algorithm)
-            wf (float): weighting factor (f in the paper), default = 1.25 (Same as DE algorithm)
+            lb: list of lower bound values
+            ub: list of upper bound values
+
+        Returns:
+            np.array: the position (the solution for the problem)
         """
-        super().__init__(epoch, pop_size, cr, wf, **kwargs)
-        self.support_parallel_modes = False
+        return np.random.uniform(lb, ub)
 
-    def evolve(self, epoch):
+    def amend_position(self, position=None, lb=None, ub=None):
         """
-        The main operations (equations) of algorithm. Inherit from Optimizer class
+        This is default function in most algorithms. Otherwise, there will be an overridden function
+        in child of Optimizer class for this function. Depend on what kind of problem are we trying to solve,
+        there will be a different amend_position function to rebound the position of agent into the valid range.
 
         Args:
-            epoch (int): The current iteration
+            position: vector position (location) of the solution.
+            lb: list of lower bound values
+            ub: list of upper bound values
+
+        Returns:
+            Amended position (make the position is in bound)
         """
-        ## Dark-zone process    (can be parallelization)
-        for idx in range(0, self.pop_size):
-            if np.random.uniform(0, 100) < self.dyn_list_life_signal[idx]:
-                self.dyn_list_cell_counter[idx] += 1
-            elif self.dyn_list_cell_counter[idx] > 1:
-                self.dyn_list_cell_counter[idx] -= 1
-
-            # Mutate process
-            p = self.dyn_list_cell_counter / np.sum(self.dyn_list_cell_counter)
-            r1, r2, r3 = np.random.choice(list(set(range(0, self.pop_size))), 3, replace=False, p=p)
-            pos_new = self.pop[r1][self.ID_POS] + self.wf * (self.pop[r2][self.ID_POS] - self.pop[r3][self.ID_POS])
-            condition = np.random.random(self.problem.n_dims) < self.cr
-            pos_new = np.where(condition, pos_new, self.pop[idx][self.ID_POS])
-            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
-            # for each pos_new, generate the fitness
-            target = self.get_target_wrapper(pos_new)
-            if self.compare_agent([pos_new, target], self.pop[idx]):
-                self.pop[idx] = [pos_new, target]
-                self.dyn_list_life_signal[idx] += 10
-
-        ## Light-zone process   (no needs parallelization)
-        self.dyn_list_life_signal -= 10
-        fit_list = np.array([item[self.ID_TAR][self.ID_FIT] for item in self.pop])
-        fit_max = np.max(fit_list)
-        fit_min = np.min(fit_list)
-        fit = (fit_list - fit_max) / (fit_min - fit_max)
-        if self.problem.minmax != 'min':
-            fit = 1 - fit
-        self.dyn_list_life_signal += 10 * fit
+        # return np.maximum(self.problem.lb, np.minimum(self.problem.ub, position))
+        return np.clip(position, lb, ub)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mealpy-2.5.3a1/mealpy/tuner.py` & `mealpy-2.5.4a1/mealpy/tuner.py`

 * *Files 12% similar despite different names*

```diff
@@ -156,14 +156,38 @@
     Args:
         algorithm (Optimizer): the algorithm/optimizer to tune
         param_grid (dict, list): dict or list of dictionaries
         n_trials (int): number of repetitions
         mode (str): set the mode to run (sequential, thread, process), default="sequential"
         n_workers (int): effected only when mode is "thread" or "process".
 
+    Examples
+    --------
+    >>> from opfunu.cec_based.cec2017 import F52017
+    >>> from mealpy.evolutionary_based import GA
+    >>> from mealpy.tuner import Tuner
+    >>> f1 = F52017(30, f_bias=0)
+    >>> p1 = {
+    >>>     "lb": f1.lb,
+    >>>     "ub": f1.ub,
+    >>>     "minmax": "min",
+    >>>     "fit_func": f1.evaluate,
+    >>>     "name": "F5",
+    >>>     "log_to": None,
+    >>> }
+    >>> term = {
+    >>>     "max_epoch": 200,
+    >>>     "max_time": 20,
+    >>>     "max_fe": 10000
+    >>> }
+    >>> param_grid = {'epoch': [50, 100], 'pop_size': [10, 20], 'pc': [0.8, 0.85], 'pm': [0.01, 0.02]}
+    >>> ga_tuner = Tuner(GA.BaseGA(), param_grid)
+    >>> ga_tuner.execute(problem=p1, termination=term, n_trials=5, n_jobs=4, mode="single", n_workers=10, verbose=True)
+    >>> ga_tuner.resolve(mode="thread", n_workers=10, termination=term)
+    >>> ga_tuner.export_results(save_path="history/results", save_as="csv")
     """
     def __init__(self, algorithm=None, param_grid=None, **kwargs):
         self.__set_keyword_arguments(kwargs)
         self.validator = Validator(log_to="console", log_file=None)
         self.algorithm = self.validator.check_is_instance("algorithm", algorithm, Optimizer)
         self.param_grid = self.validator.check_is_instance("param_grid", param_grid, dict)
         self.results, self._best_row, self._best_params, self._best_score, self._best_algorithm = None, None, None, None, None
@@ -210,64 +234,68 @@
         if save_as == "json":
             self.results.to_json(f"{save_path}.json")
         elif save_as == "dataframe":
             self.results.to_pickle(f"{save_path}.pkl")
         else:
             self.results.to_csv(f"{save_path}.csv", header=True, index=False)
 
-    def __run__(self, id_trial):
-        _, best_fitness = self.algorithm.solve(self.problem)
+    def __run__(self, id_trial, mode="single", n_workers=None, termination=None):
+        _, best_fitness = self.algorithm.solve(self.problem, mode=mode, n_workers=n_workers, termination=termination)
         return id_trial, best_fitness
 
-    def execute(self, problem=None, n_trials=2, mode="sequential", n_workers=2, verbose=True):
-        """Execute Tuner utility.
+    def execute(self, problem=None, termination=None, n_trials=2, n_jobs=None, mode="single", n_workers=2, verbose=True):
+        """Execute Tuner utility
 
         Args:
-            problem (dict, Problem): A instance of Problem class or problem dictionary
+            problem (dict, Problem): An instance of Problem class or problem dictionary
+            termination (None, dict, Termination): An instance of Termination class or termination dictionary
             n_trials (int): Number of trials on the Problem
-            mode (str): Execute problem using "sequential" or "parallel" mode, default = "sequential"
-            n_workers (int): Number of processes if mode is "parallel"
+            n_jobs (int, None): Speed up this task (run multiple trials at the same time) by using multiple processes. (<=1 or None: sequential, >=2: parallel)
+            mode (str): Apply on current Problem ("single", "swarm", "thread", "process"), default="single".
+            n_workers (int): Apply on current Problem, number of processes if mode is "thread" or "process'
             verbose (bool): Switch for verbose logging (default: False)
 
         Raises:
             TypeError: Raises TypeError if problem type is not dictionary or an instance Problem class
 
         """
         if not isinstance(problem, Problem):
             if type(problem) is dict:
                 self.problem = Problem(**problem)
             else:
                 raise TypeError(f"Problem is not an instance of Problem class or a Python dict.")
         n_trials = self.validator.check_int("n_trials", n_trials, [1, 100000])
-        mode = self.validator.check_str("mode", mode, ["parallel", "sequential"])
-        if mode == "process":
-            n_workers = self.validator.check_int("n_workers", n_workers, [2, min(61, os.cpu_count() - 1)])
-        else:
-            n_workers = None
+        n_cpus = None
+        if (n_jobs is not None) and (n_jobs >= 1):
+            n_cpus = self.validator.check_int("n_jobs", n_jobs, [2, min(61, os.cpu_count() - 1)])
+
+        if mode not in ("process", "thread", "single", "swarm"):
+            mode = "single"
+
         list_params_grid = list(ParameterGrid(self.param_grid))
         trial_columns = [f"trial_{id_trial}" for id_trial in range(1, n_trials + 1)]
         ascending = True if self.problem.minmax == "min" else False
 
         best_fit_results = []
         for id_params, params in enumerate(list_params_grid):
 
             self.algorithm.set_parameters(params)
             best_fit_results.append({"params": params})
 
             trial_list = list(range(0, n_trials))
-            if mode == "parallel":
-                with parallel.ProcessPoolExecutor(n_workers) as executor:
-                    list_results = executor.map(self.__run__, trial_list)  # Return results as original order not the future object
+            if n_cpus is not None:
+                with parallel.ProcessPoolExecutor(n_cpus) as executor:
+                    list_results = executor.map(partial(self.__run__, n_workers=n_workers, mode=mode, termination=termination), trial_list)
                     for (idx, best_fitness) in list_results:
                         best_fit_results[-1][trial_columns[idx]] = best_fitness
                         if verbose:
                             print(f"Algorithm: {self.algorithm.get_name()}, with params: {params}, trial: {idx + 1}, best fitness: {best_fitness}")
             else:
                 for idx in trial_list:
-                    idx, best_fitness = self.__run__(idx)
+                    idx, best_fitness = self.__run__(idx, mode=mode, n_workers=n_workers, termination=termination)
                     best_fit_results[-1][trial_columns[idx]] = best_fitness
                     if verbose:
                         print(f"Algorithm: {self.algorithm.get_name()}, with params: {params}, trial: {idx+1}, best fitness: {best_fitness}")
 
         df = pd.DataFrame(best_fit_results)
         df["trial_mean"] = df[trial_columns].mean(axis=1)
         df["trial_std"] = df[trial_columns].std(axis=1)
```

### Comparing `mealpy-2.5.3a1/mealpy/utils/history.py` & `mealpy-2.5.4a1/mealpy/utils/history.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/utils/io.py` & `mealpy-2.5.4a1/mealpy/utils/io.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/utils/logger.py` & `mealpy-2.5.4a1/mealpy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/utils/termination.py` & `mealpy-2.5.4a1/mealpy/utils/termination.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/utils/validator.py` & `mealpy-2.5.4a1/mealpy/utils/validator.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy/utils/visualize/linechart.py` & `mealpy-2.5.4a1/mealpy/utils/visualize/linechart.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.3a1/mealpy.egg-info/PKG-INFO` & `mealpy-2.5.4a1/mealpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mealpy
-Version: 2.5.3a1
-Summary: MEALPY: A Framework Of The State-Of-The-Art Meta-Heuristic Algorithms In Python
+Version: 2.5.4a1
+Summary: MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python
 Home-page: https://github.com/thieu1995/mealpy
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mealpy.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mealpy
 Project-URL: Bug Tracker, https://github.com/thieu1995/mealpy/issues
@@ -38,20 +38,24 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-<p align="center"><img src="https://thieu1995.github.io/post/2022-04/19-mealpy-tutorials/mealpy1.png" alt="MEALPY"/></p>
+<p align="center">
+<img style="height:400px;" 
+src="https://thieu1995.github.io/post/2022-04/19-mealpy-tutorials/mealpy5-nobg.png" 
+alt="MEALPY"/>
+</p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-2.5.2-yellow.svg)](https://github.com/thieu1995/mealpy/releases)
+[![GitHub release](https://img.shields.io/badge/release-2.5.3-yellow.svg)](https://github.com/thieu1995/mealpy/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mealpy) 
 [![PyPI version](https://badge.fury.io/py/mealpy.svg)](https://badge.fury.io/py/mealpy)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mealpy.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mealpy.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mealpy.svg)
 [![Downloads](https://pepy.tech/badge/mealpy)](https://pepy.tech/project/mealpy)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mealpy/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mealpy/actions/workflows/publish-package.yaml)
@@ -66,15 +70,15 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 
 MEALPY is the largest python library for most of the cutting-edge nature-inspired meta-heuristic algorithms (population-based). Population meta-heuristic algorithms (PMA) are the most popular algorithms in the field of 
 approximate optimization.
 
 * **Free software:** GNU General Public License (GPL) V3 license
-* **Total algorithms**: 172 (102 original, 45 official variants, 25 developed variants)
+* **Total algorithms**: 174 (102 original, 45 official variants, 27 developed variants)
 * **Documentation:** https://mealpy.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
 * **Dependencies:** numpy, scipy, pandas, matplotlib
 
 
 # Goals
 
@@ -90,15 +94,15 @@
 
 
 # Installation
 
 ### Install with pip
 Install the [current PyPI release](https://pypi.python.org/pypi/mealpy):
 ```sh 
-$ pip install mealpy==2.5.2
+$ pip install mealpy==2.5.3
 ```
 
 ### Install from source
 In case you want to install directly from the source code, use:
 ```sh 
 $ git clone https://github.com/thieu1995/mealpy.git
 $ cd mealpy
@@ -223,19 +227,25 @@
 paras_bbo_grid = {
     "epoch": [100],
     "pop_size": [50],
     "elites": [2, 3, 4, 5],
     "p_m": [0.01, 0.02, 0.05, 0.1, 0.15, 0.2]
 }
 
+term = {
+  "max_fe": 10000
+}
+
 if __name__ == "__main__":
     model = BBO.BaseBBO()
 
     tuner = Tuner(model, paras_bbo_grid)
-    tuner.execute(problem=problem, n_trials=10, mode="parallel", n_workers=4)
+    tuner.execute(problem=problem, termination=term, n_trials=5, n_jobs=5, mode="thread", n_workers=4, verbose=True)
+    ## Solve this problem 5 times (n_trials) using 5 processes (n_jobs), each process will handle 1 trial. 
+    ## The mode to run the solver is thread (mode), we will calculate the fitness of 4 solutions (n_workers) at the same time 
 
     print(tuner.best_score)
     print(tuner.best_params)
     print(tuner.best_algorithm)
     print(tuner.best_algorithm.get_name())
     
     ## Save results to csv file 
@@ -306,20 +316,24 @@
 
 ## Define models
 
 model1 = BBO.BaseBBO(epoch=10, pop_size=50)
 model2 = BBO.OriginalBBO(epoch=10, pop_size=50)
 model3 = DE.BaseDE(epoch=10, pop_size=50)
 
+## Define termination if needed
+term = {
+    "max_fe": 10000
+}
 
 ## Define and run Multitask
-
 if __name__ == "__main__":
-    multitask = Multitask(algorithms=(model1, model2, model3), problems=(p1, p2, p3))
-    multitask.execute(n_trials=3, mode="parallel", n_workers=6, save_path="history", save_as="csv", save_convergence=True, verbose=True)
+    multitask = Multitask(algorithms=(model1, model2, model3), problems=(p1, p2, p3), terminations=(term, ), modes=("thread", ))
+    # default modes = "single", default termination = epoch (as defined in problem dictionary)
+    multitask.execute(n_trials=5, n_jobs=5, save_path="history", save_as="csv", save_convergence=False, verbose=False)
     
     ## Check the directory: history/, you will see list of .csv result files
 ```
 
 For more usage examples please look at [examples](/examples) folder.
 
 More advanced examples can also be found in the [Mealpy-examples repository](https://github.com/thieu1995/mealpy_examples).
@@ -398,23 +412,20 @@
 We share lots of information, questions, and answers there. You will get more support and knowledge there.
 
 ### Cite Us
 
 If you are using mealpy in your project, we would appreciate citations:
 
 ```bibtex 
-@software{nguyen_van_thieu_2022_6684223,
-  author       = {Nguyen Van Thieu and Seyedali Mirjalili},
-  title        = {{MEALPY: a Framework of The State-of-The-Art Meta-Heuristic Algorithms in Python}},
-  month        = jun,
-  year         = 2022,
-  publisher    = {Zenodo},
-  version      = {v2.4.2},
-  doi          = {10.5281/zenodo.6684223},
-  url          = {https://doi.org/10.5281/zenodo.6684223}
+@article{van2023mealpy,
+  title={MEALPY: An open-source library for latest meta-heuristic algorithms in Python},
+  author={Van Thieu, Nguyen and Mirjalili, Seyedali},
+  journal={Journal of Systems Architecture},
+  year={2023},
+  publisher={Elsevier}
 }
 
 @article{van2023groundwater,
   title={Groundwater level modeling using Augmented Artificial Ecosystem Optimization},
   author={Van Thieu, Nguyen and Barma, Surajit Deb and Van Lam, To and Kisi, Ozgur and Mahesha, Amai},
   journal={Journal of Hydrology},
   volume={617},
@@ -495,15 +506,15 @@
     + Physics-based: Idea from physics law such as Newton's law of universal gravitation, black hole, multiverse 
     + Human-based: Idea from human interaction such as queuing search, teaching learning, ... 
     + Biology-based: Idea from biology creature (or microorganism),...
     + System-based: Idea from eco-system, immune-system, network-system, ...
     + Math-based: Idea from mathematical form or mathematical law such as sin-cosin 
     + Music-based: Idea from music instrument
 
-* Difficulty - Difficulty Level (Personal Opinion): Objective observation from author. Depend on the number of 
+* Difficulty - Difficulty Level (Personal Opinion): **Objective observation from author**. Depend on the number of 
   parameters, number of equations, the original ideas, time spend for coding, source lines of code (SLOC).
     + Easy: A few paras, few equations, SLOC very short
     + Medium: more equations than Easy level, SLOC longer than Easy level
     + Hard: Lots of equations, SLOC longer than Medium level, the paper hard to read.
     + Hard* - Very hard: Lots of equations, SLOC too long, the paper is very hard to read.
     
 ** For newbie, we recommend to read the paper of algorithms which difficulty is "easy" or "medium" difficulty level.
@@ -1122,15 +1133,15 @@
   * **OriginalWOA**: Mirjalili, S., & Lewis, A. (2016). The whale optimization algorithm. Advances in engineering software, 95, 51-67.
   * **HI_WOA**: Tang, C., Sun, W., Wu, W., & Xue, M. (2019, July). A hybrid improved whale optimization algorithm. In 2019 IEEE 15th International Conference on Control and Automation (ICCA) (pp. 362-367). IEEE.
 
 * **WHO - Wildebeest Herd Optimization** 
   * **OriginalWHO**: Amali, D., & Dinakaran, M. (2019). Wildebeest herd optimization: A new global optimization algorithm inspired by wildebeest herding behaviour. Journal of Intelligent & Fuzzy Systems, (Preprint), 1-14.
 
 * **WDO - Wind Driven Optimization** 
-  * **OriginalWDO**: Bayraktar, Z., Komurcu, M., & Werner, D. H. (2010, July). Wind Driven Optimization (WDO): A novel nature-inspired optimization algorithm and its application to electromagnetics. In 2010 IEEE antennas and propagation society international symposium (pp. 1-4). IEEE.
+  * **OriginalWDO**: Bayraktar, Z., Komurcu, M., Bossard, J.A. and Werner, D.H., 2013. The wind driven optimization technique and its application in electromagnetics. IEEE transactions on antennas and propagation, 61(5), pp.2745-2757.
 
 
 ### X
 
 ### Y
 
 ### Z
```

### Comparing `mealpy-2.5.3a1/mealpy.egg-info/SOURCES.txt` & `mealpy-2.5.4a1/mealpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 mealpy/human_based/CA.py
 mealpy/human_based/CHIO.py
 mealpy/human_based/FBIO.py
 mealpy/human_based/GSKA.py
 mealpy/human_based/HBO.py
 mealpy/human_based/HCO.py
 mealpy/human_based/ICA.py
+mealpy/human_based/ILA.py
 mealpy/human_based/LCO.py
 mealpy/human_based/QSA.py
 mealpy/human_based/SARO.py
 mealpy/human_based/SPBO.py
 mealpy/human_based/SSDO.py
 mealpy/human_based/TLO.py
 mealpy/human_based/TOA.py
@@ -152,8 +153,9 @@
 mealpy/utils/io.py
 mealpy/utils/logger.py
 mealpy/utils/problem.py
 mealpy/utils/termination.py
 mealpy/utils/validator.py
 mealpy/utils/visualize/__init__.py
 mealpy/utils/visualize/linechart.py
-tests/test_optimizer.py
+tests/test_optimizer.py
+tests/test_tuner.py
```

### Comparing `mealpy-2.5.3a1/setup.py` & `mealpy-2.5.4a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="mealpy",
-    version="2.5.3-alpha.1",
+    version="2.5.4-alpha.1",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
-    description="MEALPY: A Framework Of The State-Of-The-Art Meta-Heuristic Algorithms In Python",
+    description="MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["optimization", "metaheuristics", "MHA", "mathematical optimization", "nature-inspired algorithms",
               "evolutionary computation", "soft computing", "population-based algorithms",
               "Stochastic optimization", "Global optimization", "Convergence analysis", "Search space exploration",
               "Local search", "Computational intelligence", "Black-box optimization", "Robust optimization",
               "Hybrid algorithms", "Benchmark functions", "Metaheuristic design", "Performance analysis",
```

### Comparing `mealpy-2.5.3a1/tests/test_optimizer.py` & `mealpy-2.5.4a1/tests/test_optimizer.py`

 * *Files identical despite different names*

