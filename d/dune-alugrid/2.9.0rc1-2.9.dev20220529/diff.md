# Comparing `tmp/dune-alugrid-2.9.0rc1.tar.gz` & `tmp/dune-alugrid-2.9.dev20220529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune-alugrid-2.9.0rc1.tar", last modified: Fri Oct 21 08:17:15 2022, max compression
+gzip compressed data, was "dune-alugrid-2.9.dev20220529.tar", last modified: Sun May 29 21:03:52 2022, max compression
```

## Comparing `dune-alugrid-2.9.0rc1.tar` & `dune-alugrid-2.9.dev20220529.tar`

### file list

```diff
@@ -1,484 +1,481 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.835889 dune-alugrid-2.9.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16886 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/INSTALL
--rw-r--r--   0 runner    (1001) docker     (121)     3605 2022-10-21 08:17:15.835889 dune-alugrid-2.9.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/TODO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.791890 dune-alugrid-2.9.0rc1/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.795890 dune-alugrid-2.9.0rc1/cmake/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/cmake/modules/AlugridTortureTests.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/cmake/modules/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3120 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/cmake/modules/DuneAlugridMacros.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/cmake/modules/FindDLMalloc.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2509 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/cmake/modules/FindPThreads.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     4068 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/cmake/modules/FindSIONlib.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/cmake/modules/FindZOLTAN.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/config.h.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.795890 dune-alugrid-2.9.0rc1/doc/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/doc/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.795890 dune-alugrid-2.9.0rc1/doc/doxygen/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/doc/doxygen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/doc/doxygen/Doxylocal
--rw-r--r--   0 runner    (1001) docker     (121)     2209 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/doc/doxygen/mainpage.txt
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/doc/dunealugrid.bib
--rw-r--r--   0 runner    (1001) docker     (121)    18558 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/doc/hexahedron_alugrid.svg
--rw-r--r--   0 runner    (1001) docker     (121)    24121 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/doc/hexahedron_edges_alugrid.svg
--rw-r--r--   0 runner    (1001) docker     (121)    13104 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/doc/tetrahedron_alugrid.svg
--rw-r--r--   0 runner    (1001) docker     (121)    13316 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/doc/tetrahedron_edges_alugrid.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.795890 dune-alugrid-2.9.0rc1/dune/
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.795890 dune-alugrid-2.9.0rc1/dune/alugrid/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.799890 dune-alugrid-2.9.0rc1/dune/alugrid/3d/
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15644 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/alu3dinclude.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/alu3diterators.hh
--rw-r--r--   0 runner    (1001) docker     (121)    54015 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/alu3diterators_imp.cc
--rw-r--r--   0 runner    (1001) docker     (121)     9627 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/alugrid.hh
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/aluinline.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12690 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/communication.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/datacollectorcaps.hh
--rw-r--r--   0 runner    (1001) docker     (121)    39059 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/datahandle.hh
--rw-r--r--   0 runner    (1001) docker     (121)    22594 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/entity.hh
--rw-r--r--   0 runner    (1001) docker     (121)    36851 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/entity_imp.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8824 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/entity_inline.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13401 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/entityseed.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6850 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/faceutility.cc
--rw-r--r--   0 runner    (1001) docker     (121)    20921 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/faceutility.hh
--rw-r--r--   0 runner    (1001) docker     (121)    38378 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/faceutility_imp.cc
--rw-r--r--   0 runner    (1001) docker     (121)    23476 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/geometry.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15836 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/geometry_imp.cc
--rw-r--r--   0 runner    (1001) docker     (121)    50976 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/grid.hh
--rw-r--r--   0 runner    (1001) docker     (121)    22558 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/grid_imp.cc
--rw-r--r--   0 runner    (1001) docker     (121)    17814 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/grid_inline.hh
--rw-r--r--   0 runner    (1001) docker     (121)    47628 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/gridfactory.cc
--rw-r--r--   0 runner    (1001) docker     (121)    25127 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/gridfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12759 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/gridview.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16715 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/indexsets.cc
--rw-r--r--   0 runner    (1001) docker     (121)    22173 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/indexsets.hh
--rw-r--r--   0 runner    (1001) docker     (121)    69352 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/iterator.cc
--rw-r--r--   0 runner    (1001) docker     (121)    27452 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/iterator.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19571 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/iterator_imp.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10841 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/mappings.cc
--rw-r--r--   0 runner    (1001) docker     (121)    14653 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/mappings.hh
--rw-r--r--   0 runner    (1001) docker     (121)    41750 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/mappings_imp.cc
--rw-r--r--   0 runner    (1001) docker     (121)    21915 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/topology.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7637 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/3d/topology.hh
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.799890 dune-alugrid-2.9.0rc1/dune/alugrid/common/
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/alugrid_assert.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/backuprestore.hh
--rw-r--r--   0 runner    (1001) docker     (121)    34130 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/bisectioncompatibility.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3151 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/bndprojection.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4260 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/capabilities.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3096 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/declaration.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13591 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/defaultindexsets.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/duneassert.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6706 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/fromtogridfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9669 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/geostorage.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7258 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/hsfc.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/interfaces.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13055 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/intersectioniteratorwrapper.hh
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/ldbhandleif.hh
--rw-r--r--   0 runner    (1001) docker     (121)     7688 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/macrogridview.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6661 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/memory.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12719 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/meshquality.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2457 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/persistentcontainer.hh
--rw-r--r--   0 runner    (1001) docker     (121)    16570 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/structuredgridfactory.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/transformation.hh
--rw-r--r--   0 runner    (1001) docker     (121)    17025 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/twists.hh
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/typetraits.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9610 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/common/writeparalleldgf.hh
--rw-r--r--   0 runner    (1001) docker     (121)    20369 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/dgf.hh
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/grid.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.799890 dune-alugrid-2.9.0rc1/dune/alugrid/impl/
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4324 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/binaryio.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/binaryio.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/byteorder.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.799890 dune-alugrid-2.9.0rc1/dune/alugrid/impl/duneinterface/
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/duneinterface/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/duneinterface/gitter_dune_impl.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13893 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/duneinterface/gitter_dune_impl.h
--rw-r--r--   0 runner    (1001) docker     (121)    45086 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/duneinterface/gitter_dune_pll_impl.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10450 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/duneinterface/gitter_dune_pll_impl.h
--rw-r--r--   0 runner    (1001) docker     (121)    12220 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/indexstack.h
--rw-r--r--   0 runner    (1001) docker     (121)     5379 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/macrofileheader.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3187 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/macrofileheader.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.803890 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/
--rw-r--r--   0 runner    (1001) docker     (121)      797 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/alumetis.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10992 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/alusfc.hh
--rw-r--r--   0 runner    (1001) docker     (121)    15426 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/aluzoltan.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5746 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_hexa_top_pll.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10248 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_hexa_top_pll.h
--rw-r--r--   0 runner    (1001) docker     (121)    29106 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_idn.cc
--rw-r--r--   0 runner    (1001) docker     (121)    83299 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_impl.cc
--rw-r--r--   0 runner    (1001) docker     (121)    47351 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_impl.h
--rw-r--r--   0 runner    (1001) docker     (121)    35599 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_ldb.cc
--rw-r--r--   0 runner    (1001) docker     (121)    15045 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_ldb.h
--rw-r--r--   0 runner    (1001) docker     (121)    42399 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_mgb.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2285 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_mgb.h
--rw-r--r--   0 runner    (1001) docker     (121)    63601 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_sti.cc
--rw-r--r--   0 runner    (1001) docker     (121)    23285 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_sti.h
--rw-r--r--   0 runner    (1001) docker     (121)     7019 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_tetra_top_pll.cc
--rw-r--r--   0 runner    (1001) docker     (121)    10465 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_tetra_top_pll.h
--rw-r--r--   0 runner    (1001) docker     (121)     5841 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/mpAccess.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13274 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/mpAccess.h
--rw-r--r--   0 runner    (1001) docker     (121)     5685 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/mpAccess_MPI.h
--rw-r--r--   0 runner    (1001) docker     (121)    31958 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/mpAccess_MPI_inline.h
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/zcurve.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/projectvertex.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.807890 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4786 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gatherscatter.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9133 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/ghost_elements.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5073 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/ghost_elements.h
--rw-r--r--   0 runner    (1001) docker     (121)     4620 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/ghost_info.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5447 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/ghost_info.h
--rw-r--r--   0 runner    (1001) docker     (121)    37430 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_geo.cc
--rw-r--r--   0 runner    (1001) docker     (121)    55773 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_hexa_top.cc
--rw-r--r--   0 runner    (1001) docker     (121)    44118 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_hexa_top.h
--rw-r--r--   0 runner    (1001) docker     (121)    26189 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_impl.cc
--rw-r--r--   0 runner    (1001) docker     (121)    21559 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_impl.h
--rw-r--r--   0 runner    (1001) docker     (121)    36134 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_mgb.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13843 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_mgb.h
--rw-r--r--   0 runner    (1001) docker     (121)    34950 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_sti.cc
--rw-r--r--   0 runner    (1001) docker     (121)   160395 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_sti.h
--rw-r--r--   0 runner    (1001) docker     (121)   101152 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_tetra_top.cc
--rw-r--r--   0 runner    (1001) docker     (121)    46703 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_tetra_top.h
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/iterator_sti.h
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/key.h
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/lock.h
--rw-r--r--   0 runner    (1001) docker     (121)     5231 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/mapp_cube_3d.cc
--rw-r--r--   0 runner    (1001) docker     (121)    16883 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/mapp_cube_3d.h
--rw-r--r--   0 runner    (1001) docker     (121)    18280 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/mapp_tetra_3d.cc
--rw-r--r--   0 runner    (1001) docker     (121)    12303 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/mapp_tetra_3d.h
--rw-r--r--   0 runner    (1001) docker     (121)     4036 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/mapp_tetra_3d_ext.h
--rw-r--r--   0 runner    (1001) docker     (121)     7132 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/myalloc.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3198 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/myalloc.h
--rw-r--r--   0 runner    (1001) docker     (121)    10676 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/parallel.h
--rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/refcount.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14790 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/refinementrules.h
--rw-r--r--   0 runner    (1001) docker     (121)    17076 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/serialize.h
--rw-r--r--   0 runner    (1001) docker     (121)    25115 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/walk.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.807890 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10096 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/adapt.cc
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/alugrid.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     9977 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/backuprestore.cc
--rw-r--r--   0 runner    (1001) docker     (121)     9171 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/checkrefinement.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.807890 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/arbitrary.hexa
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube.hexa
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube.tetra
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube.triang
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_12.tetra
--rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_48.tetra
--rw-r--r--   0 runner    (1001) docker     (121)    76066 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_512.hexa
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_hc_16.hexa
--rw-r--r--   0 runner    (1001) docker     (121)   111788 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_hc_3072.tetra
--rw-r--r--   0 runner    (1001) docker     (121)    78982 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_hc_512.hexa
--rw-r--r--   0 runner    (1001) docker     (121)    12711 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_hc_64.hexa
--rw-r--r--   0 runner    (1001) docker     (121)    76022 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_hs_512.hexa
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/hexa.test.2
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/hexa.test.converted
--rw-r--r--   0 runner    (1001) docker     (121)    10175 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/macro.big
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/macro.small
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/reference.hexa
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/reference.tetra
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/tetra.test.1
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/tetra.test.2
--rw-r--r--   0 runner    (1001) docker     (121)   112090 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/unitcube.tet
--rw-r--r--   0 runner    (1001) docker     (121)    10097 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/unstructured.tetra
--rw-r--r--   0 runner    (1001) docker     (121)    10097 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/unstructured_218.tetra
--rw-r--r--   0 runner    (1001) docker     (121)     4071 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/sizes.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8013 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/threadsafety.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.811890 dune-alugrid-2.9.0rc1/dune/alugrid/test/
--rw-r--r--   0 runner    (1001) docker     (121)      861 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    27683 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/checkintersectionit.hh
--rw-r--r--   0 runner    (1001) docker     (121)     8693 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/checktwists.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.811890 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/2-3-testgrid.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/ball.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/circle-cube.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/circle.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/cube-testgrid-2-2.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/cube-testgrid-2-3.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/cubedsphere2d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/grid2d_str1d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/half-circle.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/periodic2.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/periodic3.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/periodic_2quads.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     2549 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/periodic_unstructured.dgf
--rw-r--r--   0 runner    (1001) docker     (121)    25512 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/periodic_unstructured_fine.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     2824 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/simplex-testgrid-2-2.dgf
--rw-r--r--   0 runner    (1001) docker     (121)    29383 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/simplex-testgrid-2-3-noproj.dgf
--rw-r--r--   0 runner    (1001) docker     (121)    29431 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/simplex-testgrid-2-3.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     7627 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/simplex-testgrid-3-3.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/sphere.dgf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.811890 dune-alugrid-2.9.0rc1/dune/alugrid/test/gmsh/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/gmsh/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/gmsh/circle2ndorder.msh
--rw-r--r--   0 runner    (1001) docker     (121)    22999 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/gmsh/curved2d.msh
--rw-r--r--   0 runner    (1001) docker     (121)    11575 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/gmsh/telescope.msh
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/gmsh/unitsquare_quads_2x2.msh
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/insertgrid.hh
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/pyramid.tetra.converted
--rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-adaptivity.cc
--rw-r--r--   0 runner    (1001) docker     (121)    32378 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-alugrid.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-backup-restore.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-ball-projection.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2635 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-dgf.cc
--rw-r--r--   0 runner    (1001) docker     (121)     7338 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-entities.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-fromtogridfactory.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5626 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-geometries.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3754 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-gmsh.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-hierarchic.cc
--rw-r--r--   0 runner    (1001) docker     (121)     8150 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-iterators.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-periodic.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-structuredgridfactory.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1268 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-threadsafety.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/alugrid/test/test-twists.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.811890 dune-alugrid-2.9.0rc1/dune/python/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.811890 dune-alugrid-2.9.0rc1/dune/python/test/
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/python/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/python/test/dgfparser.log
--rw-r--r--   0 runner    (1001) docker     (121)     3653 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/python/test/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/python/test/test_gf1.py
--rw-r--r--   0 runner    (1001) docker     (121)     4396 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/python/test/test_gf2.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune/python/test/test_indexset.py
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune-alugrid.pc.in
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/dune.module
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.811890 dune-alugrid-2.9.0rc1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10367 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/adaptation.hh
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/alugrid.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.811890 dune-alugrid-2.9.0rc1/examples/backuprestore/
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/backuprestore/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5233 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/backuprestore/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/backuprestore/paralleldgf.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4322 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/backuprestore/sionlib.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.815890 dune-alugrid-2.9.0rc1/examples/callback/
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/callback/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11052 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/callback/adaptation.hh
--rwxr-xr-x   0 runner    (1001) docker     (121)      979 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/callback/check-adaptation.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/callback/datamap.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11474 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/callback/diagnostics.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13500 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/callback/fvscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)     9418 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/callback/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/callback/paralleldgf.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19039 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/callback/piecewisefunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/callback/problem-ball.hh
--rw-r--r--   0 runner    (1001) docker     (121)    24822 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/callback/problem-euler.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12059 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/callback/problem-transport.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3159 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/callback/problem.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.815890 dune-alugrid-2.9.0rc1/examples/communication/
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/communication/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10367 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/communication/adaptation.hh
--rwxr-xr-x   0 runner    (1001) docker     (121)      623 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/communication/check-communication.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/communication/datamap.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11474 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/communication/diagnostics.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14763 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/communication/fvscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10052 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/communication/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/communication/paralleldgf.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19039 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/communication/piecewisefunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/communication/problem-ball.hh
--rw-r--r--   0 runner    (1001) docker     (121)    24822 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/communication/problem-euler.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12059 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/communication/problem-transport.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3159 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/communication/problem.hh
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/datamap.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.827890 dune-alugrid-2.9.0rc1/examples/dgf/
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/cube3d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/cube3d.dgf.3
--rw-r--r--   0 runner    (1001) docker     (121)   406352 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/cube3d.dgf.3.0
--rw-r--r--   0 runner    (1001) docker     (121)   393417 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/cube3d.dgf.3.1
--rw-r--r--   0 runner    (1001) docker     (121)   322442 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/cube3d.dgf.3.2
--rw-r--r--   0 runner    (1001) docker     (121)  4136286 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/cube_hc_32768.dgf
--rw-r--r--   0 runner    (1001) docker     (121)   531120 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/cube_hc_4096.dgf
--rw-r--r--   0 runner    (1001) docker     (121)    73622 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/cube_hc_512.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/ffs2d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/ffs3d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/ffs3d_fine.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/periodic2.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/periodic3.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/sb2d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/sb2d_6400.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/sb2d_65536.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/sb3d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/sb3d_1024.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/sb3d_128.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/sb3d_16.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/sb3d_65536.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/sb3d_8192.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     8162 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tet.0.msh.dgf
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tet.00.msh.dgf
--rw-r--r--   0 runner    (1001) docker     (121)    64832 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tet.1.msh.dgf
--rw-r--r--   0 runner    (1001) docker     (121)   120624 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tet.2.msh.dgf
--rw-r--r--   0 runner    (1001) docker     (121)   246625 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tet.3.msh.dgf
--rw-r--r--   0 runner    (1001) docker     (121)   495132 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tet.4.msh.dgf
--rw-r--r--   0 runner    (1001) docker     (121)   985766 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tet.5.msh.dgf
--rw-r--r--   0 runner    (1001) docker     (121)  1986455 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tet.6.msh.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tet_120k.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tet_240k.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tet_480k.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tet_960k.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tetexp.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tetgen.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/tetmsh.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/unitcube2d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/dgf/unitcube3d.dgf
--rw-r--r--   0 runner    (1001) docker     (121)    11474 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/diagnostics.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13500 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/fvscheme.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.827890 dune-alugrid-2.9.0rc1/examples/loadbalance/
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7349 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/adaptation.hh
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/alugrid.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/datamap.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11474 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/diagnostics.hh
--rw-r--r--   0 runner    (1001) docker     (121)    13500 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/fvscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/loadbalance_simple.hh
--rw-r--r--   0 runner    (1001) docker     (121)    20722 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/loadbalance_zoltan.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10481 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/paralleldgf.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19039 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/piecewisefunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/problem-ball.hh
--rw-r--r--   0 runner    (1001) docker     (121)    24822 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/problem-euler.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12059 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/problem-transport.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3159 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/loadbalance/problem.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10021 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/paralleldgf.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19039 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/piecewisefunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/problem-ball.hh
--rw-r--r--   0 runner    (1001) docker     (121)    24822 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/problem-euler.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12059 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/problem-transport.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3159 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/problem.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.831889 dune-alugrid-2.9.0rc1/examples/quality/
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10367 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/adaptation.hh
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/alugrid.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/datamap.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11474 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/diagnostics.hh
--rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/estimate-closure.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13500 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/fvscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/gmsh2dgf.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2378 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/io.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/io.hh
--rw-r--r--   0 runner    (1001) docker     (121)     6830 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/paralleldgf.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19039 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/piecewisefunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3351 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/problem-globalrefine.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12059 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/problem-transport.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3159 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/problem.hh
--rwxr-xr-x   0 runner    (1001) docker     (121)      460 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/quality/tetSequenceStudy.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.831889 dune-alugrid-2.9.0rc1/examples/testEfficiency/
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/testEfficiency/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11052 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/testEfficiency/adaptation.hh
--rwxr-xr-x   0 runner    (1001) docker     (121)      941 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/testEfficiency/check-efficiency.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/testEfficiency/datamap.hh
--rw-r--r--   0 runner    (1001) docker     (121)    11474 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/testEfficiency/diagnostics.hh
--rw-r--r--   0 runner    (1001) docker     (121)    14763 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/testEfficiency/fvscheme.hh
--rw-r--r--   0 runner    (1001) docker     (121)    10341 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/testEfficiency/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/testEfficiency/paralleldgf.hh
--rw-r--r--   0 runner    (1001) docker     (121)    19039 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/testEfficiency/piecewisefunction.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/testEfficiency/problem-ball.hh
--rw-r--r--   0 runner    (1001) docker     (121)    24822 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/testEfficiency/problem-euler.hh
--rw-r--r--   0 runner    (1001) docker     (121)    12059 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/testEfficiency/problem-transport.hh
--rw-r--r--   0 runner    (1001) docker     (121)     3159 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/examples/testEfficiency/problem.hh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.831889 dune-alugrid-2.9.0rc1/lib/
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/lib/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/lib/dunealugridam2cmake.lib
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.831889 dune-alugrid-2.9.0rc1/misc/
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/alugrid.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      350 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/checkversion.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.831889 dune-alugrid-2.9.0rc1/misc/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/2.tetra
--rw-r--r--   0 runner    (1001) docker     (121)     4859 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/adapt.cc
--rw-r--r--   0 runner    (1001) docker     (121)     5856 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/backuprestore.cc
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/cube.tetra
--rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/example.cc
--rw-r--r--   0 runner    (1001) docker     (121)     3914 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/examplepara.cc
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/howmuch.cc
--rw-r--r--   0 runner    (1001) docker     (121)     4605 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/loadlb.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.831889 dune-alugrid-2.9.0rc1/misc/examples/macrogrids/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/macrogrids/arbitrary.hexa
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/macrogrids/cube.hexa
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/macrogrids/cube.tetra
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/macrogrids/cube.triang
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/macrogrids/cube_12.tetra
--rw-r--r--   0 runner    (1001) docker     (121)     3576 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/macrogrids/cube_48.tetra
--rw-r--r--   0 runner    (1001) docker     (121)   115517 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/macrogrids/cube_hc_3072.tetra
--rw-r--r--   0 runner    (1001) docker     (121)    78982 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/macrogrids/cube_hc_512.hexa
--rw-r--r--   0 runner    (1001) docker     (121)    10157 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/macrogrids/macro.big
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/macrogrids/macro.small
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/macrogrids/reference.hexa
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/macrogrids/reference.tetra
--rw-r--r--   0 runner    (1001) docker     (121)    10635 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/macrogrids/unstructured.tetra
--rw-r--r--   0 runner    (1001) docker     (121)     3637 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/memdata_new.hexa
--rw-r--r--   0 runner    (1001) docker     (121)     3433 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/memdata_new.tetra
--rw-r--r--   0 runner    (1001) docker     (121)     3652 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/memdata_old.hexa
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/memdata_old.tetra
--rw-r--r--   0 runner    (1001) docker     (121)     5094 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/memdata_oldpara.hexa
--rw-r--r--   0 runner    (1001) docker     (121)     4721 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/memdata_oldpara.tetra
--rw-r--r--   0 runner    (1001) docker     (121)     6929 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/periodic.cc
--rw-r--r--   0 runner    (1001) docker     (121)     9248 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/sizes.cc
--rw-r--r--   0 runner    (1001) docker     (121)     1705 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/timer.hh
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/examples/twist.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.835889 dune-alugrid-2.9.0rc1/misc/macrogrids/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/macrogrids/arbitrary.hexa
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/macrogrids/cube.hexa
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/macrogrids/cube.tetra
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/macrogrids/cube.triang
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/macrogrids/cube_12.tetra
--rw-r--r--   0 runner    (1001) docker     (121)     3576 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/macrogrids/cube_48.tetra
--rw-r--r--   0 runner    (1001) docker     (121)   115517 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/macrogrids/cube_hc_3072.tetra
--rw-r--r--   0 runner    (1001) docker     (121)    78982 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/macrogrids/cube_hc_512.hexa
--rw-r--r--   0 runner    (1001) docker     (121)    10157 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/macrogrids/macro.big
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/macrogrids/macro.small
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/macrogrids/reference.hexa
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/macrogrids/reference.tetra
--rw-r--r--   0 runner    (1001) docker     (121)    10635 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/macrogrids/unstructured.tetra
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.835889 dune-alugrid-2.9.0rc1/misc/versioncheck/
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/misc/versioncheck/alugridversion.cc
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.835889 dune-alugrid-2.9.0rc1/python/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.835889 dune-alugrid-2.9.0rc1/python/dune/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/python/dune/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.835889 dune-alugrid-2.9.0rc1/python/dune/alugrid/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/python/dune/alugrid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/python/dune/alugrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6738 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/python/dune/alugrid/_grids.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.835889 dune-alugrid-2.9.0rc1/python/dune_alugrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3605 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/python/dune_alugrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15015 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/python/dune_alugrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/python/dune_alugrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/python/dune_alugrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/python/dune_alugrid.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.835889 dune-alugrid-2.9.0rc1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3004 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/scripts/build-dune-alugrid.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      337 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/scripts/version.sh
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 08:17:15.835889 dune-alugrid-2.9.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.835889 dune-alugrid-2.9.0rc1/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/utils/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.835889 dune-alugrid-2.9.0rc1/utils/bisection-compatibility/
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/utils/bisection-compatibility/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/utils/bisection-compatibility/bisectioncompatibility.hh
--rw-r--r--   0 runner    (1001) docker     (121)     4750 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/utils/bisection-compatibility/estimate-closure.cc
--rw-r--r--   0 runner    (1001) docker     (121)     2824 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/utils/bisection-compatibility/test-compatibility.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 08:17:15.835889 dune-alugrid-2.9.0rc1/utils/convert-macrogrid/
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/utils/convert-macrogrid/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/utils/convert-macrogrid/dgfparser.hh
--rw-r--r--   0 runner    (1001) docker     (121)    26762 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/utils/convert-macrogrid/main.cc
--rw-r--r--   0 runner    (1001) docker     (121)    13140 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/utils/convert-macrogrid/partition.hh
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/utils/convert-macrogrid/test.dgf
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-10-21 08:17:15.000000 dune-alugrid-2.9.0rc1/utils/convert-macrogrid/timing.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.491832 dune-alugrid-2.9.dev20220529/
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    16886 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-05-29 21:03:52.491832 dune-alugrid-2.9.dev20220529/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-05-29 21:03:52.000000 dune-alugrid-2.9.dev20220529/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/TODO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.443832 dune-alugrid-2.9.dev20220529/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.447832 dune-alugrid-2.9.dev20220529/cmake/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/cmake/modules/AlugridTortureTests.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3120 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/cmake/modules/DuneAlugridMacros.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/cmake/modules/FindDLMalloc.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2509 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/cmake/modules/FindPThreads.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     4068 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/cmake/modules/FindSIONlib.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/cmake/modules/FindZOLTAN.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/config.h.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.447832 dune-alugrid-2.9.dev20220529/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/doc/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.447832 dune-alugrid-2.9.dev20220529/doc/doxygen/
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/doc/doxygen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/doc/doxygen/Doxylocal
+-rw-r--r--   0 runner    (1001) docker     (121)     2209 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/doc/doxygen/mainpage.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/doc/dunealugrid.bib
+-rw-r--r--   0 runner    (1001) docker     (121)    18558 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/doc/hexahedron_alugrid.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    24121 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/doc/hexahedron_edges_alugrid.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    13104 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/doc/tetrahedron_alugrid.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    13316 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/doc/tetrahedron_edges_alugrid.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.447832 dune-alugrid-2.9.dev20220529/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.447832 dune-alugrid-2.9.dev20220529/dune/alugrid/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.451832 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/
+-rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    15644 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/alu3dinclude.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2477 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/alu3diterators.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    54015 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/alu3diterators_imp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8459 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/alugrid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/aluinline.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12690 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/communication.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/datacollectorcaps.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    39059 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/datahandle.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    22594 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/entity.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    36851 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/entity_imp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8824 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/entity_inline.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13476 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/entityseed.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6850 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/faceutility.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    20921 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/faceutility.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    38360 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/faceutility_imp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    23510 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/geometry.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15836 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/geometry_imp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    50778 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/grid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    22541 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/grid_imp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    17814 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/grid_inline.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    47650 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/gridfactory.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    25271 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/gridfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12721 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/gridview.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16715 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/indexsets.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    22173 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/indexsets.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    69352 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/iterator.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    27452 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    18979 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/iterator_imp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    10841 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/mappings.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    14653 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/mappings.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    41750 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/mappings_imp.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    21915 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/topology.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7637 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/3d/topology.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.451832 dune-alugrid-2.9.dev20220529/dune/alugrid/common/
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/alugrid_assert.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/backuprestore.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    34130 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/bisectioncompatibility.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3151 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/bndprojection.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4219 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/capabilities.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/declaration.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13591 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/defaultindexsets.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/duneassert.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6706 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/fromtogridfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9669 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/geostorage.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7388 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/hsfc.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/interfaces.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13055 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/intersectioniteratorwrapper.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/ldbhandleif.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     7771 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/macrogridview.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6661 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/memory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    12611 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/meshquality.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2457 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/persistentcontainer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    16660 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/structuredgridfactory.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/transformation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    17025 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/twists.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/typetraits.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9610 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/common/writeparalleldgf.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    20369 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/dgf.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/grid.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.451832 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/
+-rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4324 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/binaryio.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/binaryio.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/byteorder.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.451832 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/duneinterface/
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/duneinterface/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/duneinterface/gitter_dune_impl.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    13893 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/duneinterface/gitter_dune_impl.h
+-rw-r--r--   0 runner    (1001) docker     (121)    45086 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/duneinterface/gitter_dune_pll_impl.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    10450 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/duneinterface/gitter_dune_pll_impl.h
+-rw-r--r--   0 runner    (1001) docker     (121)    12220 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/indexstack.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5379 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/macrofileheader.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3187 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/macrofileheader.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.455832 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/
+-rw-r--r--   0 runner    (1001) docker     (121)      797 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/alumetis.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10992 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/alusfc.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    15440 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/aluzoltan.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5746 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_hexa_top_pll.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    10248 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_hexa_top_pll.h
+-rw-r--r--   0 runner    (1001) docker     (121)    29146 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_idn.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    83299 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_impl.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    47351 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_impl.h
+-rw-r--r--   0 runner    (1001) docker     (121)    35597 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_ldb.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    15045 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_ldb.h
+-rw-r--r--   0 runner    (1001) docker     (121)    42399 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_mgb.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2285 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_mgb.h
+-rw-r--r--   0 runner    (1001) docker     (121)    63580 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_sti.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    23285 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_sti.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7019 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_tetra_top_pll.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    10465 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_tetra_top_pll.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5876 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/mpAccess.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    13274 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/mpAccess.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5685 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/mpAccess_MPI.h
+-rw-r--r--   0 runner    (1001) docker     (121)    31958 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/mpAccess_MPI_inline.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/zcurve.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/projectvertex.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.459832 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4786 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gatherscatter.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9133 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/ghost_elements.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5073 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/ghost_elements.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4620 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/ghost_info.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5447 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/ghost_info.h
+-rw-r--r--   0 runner    (1001) docker     (121)    37430 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_geo.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    55773 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_hexa_top.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    44118 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_hexa_top.h
+-rw-r--r--   0 runner    (1001) docker     (121)    26189 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_impl.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    21559 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_impl.h
+-rw-r--r--   0 runner    (1001) docker     (121)    36134 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_mgb.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    13843 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_mgb.h
+-rw-r--r--   0 runner    (1001) docker     (121)    34950 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_sti.cc
+-rw-r--r--   0 runner    (1001) docker     (121)   160395 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_sti.h
+-rw-r--r--   0 runner    (1001) docker     (121)    99121 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_tetra_top.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    46661 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_tetra_top.h
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/iterator_sti.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/key.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/lock.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5231 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/mapp_cube_3d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    16883 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/mapp_cube_3d.h
+-rw-r--r--   0 runner    (1001) docker     (121)    18280 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/mapp_tetra_3d.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    12303 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/mapp_tetra_3d.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4036 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/mapp_tetra_3d_ext.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7132 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/myalloc.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3198 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/myalloc.h
+-rw-r--r--   0 runner    (1001) docker     (121)    10676 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/parallel.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/refcount.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14790 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/refinementrules.h
+-rw-r--r--   0 runner    (1001) docker     (121)    17076 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/serialize.h
+-rw-r--r--   0 runner    (1001) docker     (121)    25115 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/walk.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.459832 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      519 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10096 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/adapt.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/alugrid.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     9977 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/backuprestore.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9171 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/checkrefinement.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.459832 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/arbitrary.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube.triang
+-rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_12.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_48.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)    76066 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_512.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)     2477 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_hc_16.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)   111788 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_hc_3072.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)    78982 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_hc_512.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)    12711 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_hc_64.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)    76022 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_hs_512.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/hexa.test.2
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/hexa.test.converted
+-rw-r--r--   0 runner    (1001) docker     (121)    10175 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/macro.big
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/macro.small
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/reference.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/reference.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/tetra.test.1
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/tetra.test.2
+-rw-r--r--   0 runner    (1001) docker     (121)   112090 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/unitcube.tet
+-rw-r--r--   0 runner    (1001) docker     (121)    10097 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/unstructured.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)    10097 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/unstructured_218.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)     4071 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/sizes.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8013 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/threadsafety.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.463832 dune-alugrid-2.9.dev20220529/dune/alugrid/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      861 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    27683 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/checkintersectionit.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8693 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/checktwists.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.463832 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/2-3-testgrid.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      828 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/ball.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/circle-cube.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      322 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/circle.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/cube-testgrid-2-2.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/cube-testgrid-2-3.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/cubedsphere2d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/grid2d_str1d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/half-circle.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/periodic2.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/periodic3.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     2824 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/simplex-testgrid-2-2.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)    29383 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/simplex-testgrid-2-3-noproj.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)    29431 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/simplex-testgrid-2-3.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     7627 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/simplex-testgrid-3-3.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/sphere.dgf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.463832 dune-alugrid-2.9.dev20220529/dune/alugrid/test/gmsh/
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/gmsh/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/gmsh/circle2ndorder.msh
+-rw-r--r--   0 runner    (1001) docker     (121)    22999 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/gmsh/curved2d.msh
+-rw-r--r--   0 runner    (1001) docker     (121)    11575 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/gmsh/telescope.msh
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/gmsh/unitsquare_quads_2x2.msh
+-rw-r--r--   0 runner    (1001) docker     (121)     2621 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/insertgrid.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/pyramid.tetra.converted
+-rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-adaptivity.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    32472 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-alugrid.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-backup-restore.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-ball-projection.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2635 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-dgf.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     7338 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-entities.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-fromtogridfactory.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5626 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-geometries.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3754 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-gmsh.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-hierarchic.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     8150 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-iterators.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2476 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-periodic.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-structuredgridfactory.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1268 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-threadsafety.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-twists.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.463832 dune-alugrid-2.9.dev20220529/dune/python/
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.463832 dune-alugrid-2.9.dev20220529/dune/python/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/python/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/python/test/dgfparser.log
+-rw-r--r--   0 runner    (1001) docker     (121)     3653 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/python/test/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/python/test/test_gf1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4396 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/python/test/test_gf2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune/python/test/test_indexset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune-alugrid.pc.in
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/dune.module
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.467832 dune-alugrid-2.9.dev20220529/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1866 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10367 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/adaptation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/alugrid.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.467832 dune-alugrid-2.9.dev20220529/examples/backuprestore/
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/backuprestore/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5233 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/backuprestore/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/backuprestore/paralleldgf.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4322 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/backuprestore/sionlib.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.467832 dune-alugrid-2.9.dev20220529/examples/callback/
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/callback/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11052 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/callback/adaptation.hh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      979 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/callback/check-adaptation.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/callback/datamap.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11484 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/callback/diagnostics.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13500 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/callback/fvscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     9418 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/callback/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/callback/paralleldgf.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19039 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/callback/piecewisefunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/callback/problem-ball.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    24822 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/callback/problem-euler.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8688 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/callback/problem-transport.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/callback/problem.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.467832 dune-alugrid-2.9.dev20220529/examples/communication/
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/communication/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10367 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/communication/adaptation.hh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      623 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/communication/check-communication.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/communication/datamap.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11484 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/communication/diagnostics.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14763 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/communication/fvscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10052 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/communication/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/communication/paralleldgf.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19039 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/communication/piecewisefunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/communication/problem-ball.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    24822 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/communication/problem-euler.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8688 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/communication/problem-transport.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/communication/problem.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/datamap.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.483832 dune-alugrid-2.9.dev20220529/examples/dgf/
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/cube3d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/cube3d.dgf.3
+-rw-r--r--   0 runner    (1001) docker     (121)   406352 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/cube3d.dgf.3.0
+-rw-r--r--   0 runner    (1001) docker     (121)   393417 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/cube3d.dgf.3.1
+-rw-r--r--   0 runner    (1001) docker     (121)   322442 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/cube3d.dgf.3.2
+-rw-r--r--   0 runner    (1001) docker     (121)  4136286 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/cube_hc_32768.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)   531120 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/cube_hc_4096.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)    73622 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/cube_hc_512.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/ffs2d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/ffs3d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/ffs3d_fine.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/periodic2.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/periodic3.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      725 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/sb2d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/sb2d_6400.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/sb2d_65536.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/sb3d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/sb3d_1024.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/sb3d_128.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/sb3d_16.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/sb3d_65536.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/sb3d_8192.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     8162 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tet.0.msh.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tet.00.msh.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)    64832 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tet.1.msh.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)   120624 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tet.2.msh.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)   246625 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tet.3.msh.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)   495132 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tet.4.msh.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)   985766 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tet.5.msh.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)  1986455 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tet.6.msh.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tet_120k.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tet_240k.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tet_480k.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tet_960k.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tetexp.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tetgen.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      410 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/tetmsh.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/unitcube2d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/dgf/unitcube3d.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)    11484 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/diagnostics.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13500 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/fvscheme.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.483832 dune-alugrid-2.9.dev20220529/examples/loadbalance/
+-rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7349 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/adaptation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/alugrid.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/datamap.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11484 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/diagnostics.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    13500 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/fvscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/loadbalance_simple.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    20722 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/loadbalance_zoltan.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10481 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/paralleldgf.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19039 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/piecewisefunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/problem-ball.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    24822 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/problem-euler.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8688 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/problem-transport.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/loadbalance/problem.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10021 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/paralleldgf.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19039 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/piecewisefunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/problem-ball.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    24822 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/problem-euler.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8688 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/problem-transport.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/problem.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.483832 dune-alugrid-2.9.dev20220529/examples/quality/
+-rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10367 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/adaptation.hh
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/alugrid.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/datamap.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11484 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/diagnostics.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/estimate-closure.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    13500 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/fvscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/gmsh2dgf.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2378 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/io.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/io.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     6830 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/paralleldgf.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19039 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/piecewisefunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3351 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/problem-globalrefine.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8688 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/problem-transport.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/problem.hh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      460 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/quality/tetSequenceStudy.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.483832 dune-alugrid-2.9.dev20220529/examples/testEfficiency/
+-rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/testEfficiency/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11052 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/testEfficiency/adaptation.hh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      941 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/testEfficiency/check-efficiency.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/testEfficiency/datamap.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    11484 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/testEfficiency/diagnostics.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    14763 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/testEfficiency/fvscheme.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    10341 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/testEfficiency/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/testEfficiency/paralleldgf.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    19039 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/testEfficiency/piecewisefunction.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/testEfficiency/problem-ball.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    24822 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/testEfficiency/problem-euler.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     8688 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/testEfficiency/problem-transport.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/examples/testEfficiency/problem.hh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.483832 dune-alugrid-2.9.dev20220529/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/lib/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/lib/dunealugridam2cmake.lib
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.483832 dune-alugrid-2.9.dev20220529/misc/
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/alugrid.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)      350 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/checkversion.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.487832 dune-alugrid-2.9.dev20220529/misc/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/2.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)     4859 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/adapt.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     5856 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/backuprestore.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/cube.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/example.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     3914 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/examplepara.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/howmuch.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     4605 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/loadlb.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.487832 dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/arbitrary.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/cube.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/cube.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/cube.triang
+-rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/cube_12.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)     3576 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/cube_48.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)   115517 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/cube_hc_3072.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)    78982 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/cube_hc_512.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)    10157 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/macro.big
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/macro.small
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/reference.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/reference.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)    10635 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/unstructured.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)     3637 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/memdata_new.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)     3433 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/memdata_new.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)     3652 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/memdata_old.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)     3439 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/memdata_old.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)     5094 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/memdata_oldpara.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)     4721 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/memdata_oldpara.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)     6929 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/periodic.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     9248 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/sizes.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     1705 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/timer.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/examples/twist.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.487832 dune-alugrid-2.9.dev20220529/misc/macrogrids/
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/macrogrids/arbitrary.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/macrogrids/cube.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/macrogrids/cube.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/macrogrids/cube.triang
+-rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/macrogrids/cube_12.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)     3576 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/macrogrids/cube_48.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)   115517 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/macrogrids/cube_hc_3072.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)    78982 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/macrogrids/cube_hc_512.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)    10157 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/macrogrids/macro.big
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/macrogrids/macro.small
+-rw-r--r--   0 runner    (1001) docker     (121)      398 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/macrogrids/reference.hexa
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/macrogrids/reference.tetra
+-rw-r--r--   0 runner    (1001) docker     (121)    10635 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/macrogrids/unstructured.tetra
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.487832 dune-alugrid-2.9.dev20220529/misc/versioncheck/
+-rw-r--r--   0 runner    (1001) docker     (121)      879 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/misc/versioncheck/alugridversion.cc
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-05-29 21:03:52.000000 dune-alugrid-2.9.dev20220529/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.487832 dune-alugrid-2.9.dev20220529/python/
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.487832 dune-alugrid-2.9.dev20220529/python/dune/
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/python/dune/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.491832 dune-alugrid-2.9.dev20220529/python/dune/alugrid/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/python/dune/alugrid/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/python/dune/alugrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6118 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/python/dune/alugrid/_grids.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.491832 dune-alugrid-2.9.dev20220529/python/dune_alugrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-05-29 21:03:52.000000 dune-alugrid-2.9.dev20220529/python/dune_alugrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14872 2022-05-29 21:03:52.000000 dune-alugrid-2.9.dev20220529/python/dune_alugrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-29 21:03:52.000000 dune-alugrid-2.9.dev20220529/python/dune_alugrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-05-29 21:03:52.000000 dune-alugrid-2.9.dev20220529/python/dune_alugrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-05-29 21:03:52.000000 dune-alugrid-2.9.dev20220529/python/dune_alugrid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.491832 dune-alugrid-2.9.dev20220529/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3004 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/scripts/build-dune-alugrid.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      337 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/scripts/version.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-29 21:03:52.491832 dune-alugrid-2.9.dev20220529/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-05-29 21:03:52.000000 dune-alugrid-2.9.dev20220529/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.491832 dune-alugrid-2.9.dev20220529/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/utils/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.491832 dune-alugrid-2.9.dev20220529/utils/bisection-compatibility/
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/utils/bisection-compatibility/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/utils/bisection-compatibility/bisectioncompatibility.hh
+-rw-r--r--   0 runner    (1001) docker     (121)     4750 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/utils/bisection-compatibility/estimate-closure.cc
+-rw-r--r--   0 runner    (1001) docker     (121)     2824 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/utils/bisection-compatibility/test-compatibility.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-29 21:03:52.491832 dune-alugrid-2.9.dev20220529/utils/convert-macrogrid/
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/utils/convert-macrogrid/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/utils/convert-macrogrid/dgfparser.hh
+-rw-r--r--   0 runner    (1001) docker     (121)    26762 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/utils/convert-macrogrid/main.cc
+-rw-r--r--   0 runner    (1001) docker     (121)    13140 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/utils/convert-macrogrid/partition.hh
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/utils/convert-macrogrid/test.dgf
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-05-29 21:03:51.000000 dune-alugrid-2.9.dev20220529/utils/convert-macrogrid/timing.txt
```

### Comparing `dune-alugrid-2.9.0rc1/.gitlab-ci.yml` & `dune-alugrid-2.9.dev20220529/.gitlab-ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
   DUNECI_CMAKE_FLAGS: "-DCMAKE_DISABLE_FIND_PACKAGE_Alberta=TRUE -DCMAKE_DISABLE_FIND_PACKAGE_Vc=TRUE -DCMAKE_DISABLE_DOCUMENTATION=TRUE -DENABLE_HEADERCHECK=ON"
   
 before_script:
   - duneci-install-module https://gitlab.dune-project.org/core/dune-common.git
   - duneci-install-module https://gitlab.dune-project.org/core/dune-geometry.git
   - duneci-install-module https://gitlab.dune-project.org/core/dune-grid.git
 
+
 ubuntu:20.04-clang-10-17:
   image: registry.dune-project.org/docker/ci/ubuntu:20.04
   script: duneci-standard-test
   variables:
     DUNECI_TOOLCHAIN: clang-10-17
     # cmake flags we use for all dune moudle - important is that build shared libs is set (need some better way of doi
     DUNECI_CMAKE_FLAGS: $DUNE_CMAKE_FLAGS
```

### Comparing `dune-alugrid-2.9.0rc1/AUTHORS` & `dune-alugrid-2.9.dev20220529/AUTHORS`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/COPYING` & `dune-alugrid-2.9.dev20220529/COPYING`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/PKG-INFO` & `dune-alugrid-2.9.dev20220529/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-alugrid
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: Module providing the DUNE grid interface for unstructured simplicial and cube grids in 2 and 3 space dimensions
 Home-page: https://gitlab.dune-project.org/extensions/dune-alugrid
 Author: Robert Kloefkorn, Martin Alkaemper, Andreas Dedner and Martin Nolte
 Author-email: dune-devel@lists.dune-project.org
 License: UNKNOWN
 Description: DUNE-ALUGrid
         ============
@@ -61,15 +61,15 @@
         [2]: http://www.dune-project.org/doc/installation
         [3]: http://journals.ub.uni-heidelberg.de/index.php/ans/article/view/23252
         [4]: http://www.cs.sandia.gov/Zoltan/
         [5]: https://gitlab.dune-project.org/extensions/dune-alugrid/blob/master/COPYING
         [6]: https://gitlab.dune-project.org/extensions/dune-alugrid/blob/master/doc/dunealugrid.bib
         
         
-        git-2788e7cc0e8b9bf32f589656a94323342045a4b5
+        git-9fede971172df042602dab6c13bd1ead94419ac4
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-alugrid-2.9.0rc1/README.md` & `dune-alugrid-2.9.dev20220529/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -53,8 +53,8 @@
 [2]: http://www.dune-project.org/doc/installation
 [3]: http://journals.ub.uni-heidelberg.de/index.php/ans/article/view/23252
 [4]: http://www.cs.sandia.gov/Zoltan/
 [5]: https://gitlab.dune-project.org/extensions/dune-alugrid/blob/master/COPYING
 [6]: https://gitlab.dune-project.org/extensions/dune-alugrid/blob/master/doc/dunealugrid.bib
 
 
-git-2788e7cc0e8b9bf32f589656a94323342045a4b5
+git-9fede971172df042602dab6c13bd1ead94419ac4
```

### Comparing `dune-alugrid-2.9.0rc1/cmake/modules/DuneAlugridMacros.cmake` & `dune-alugrid-2.9.dev20220529/cmake/modules/DuneAlugridMacros.cmake`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/cmake/modules/FindDLMalloc.cmake` & `dune-alugrid-2.9.dev20220529/cmake/modules/FindDLMalloc.cmake`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/cmake/modules/FindPThreads.cmake` & `dune-alugrid-2.9.dev20220529/cmake/modules/FindPThreads.cmake`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/cmake/modules/FindSIONlib.cmake` & `dune-alugrid-2.9.dev20220529/cmake/modules/FindSIONlib.cmake`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/cmake/modules/FindZOLTAN.cmake` & `dune-alugrid-2.9.dev20220529/cmake/modules/FindZOLTAN.cmake`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/config.h.cmake` & `dune-alugrid-2.9.dev20220529/config.h.cmake`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/doc/doxygen/Doxylocal` & `dune-alugrid-2.9.dev20220529/doc/doxygen/Doxylocal`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/doc/doxygen/mainpage.txt` & `dune-alugrid-2.9.dev20220529/doc/doxygen/mainpage.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/doc/hexahedron_alugrid.svg` & `dune-alugrid-2.9.dev20220529/doc/hexahedron_alugrid.svg`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/doc/hexahedron_edges_alugrid.svg` & `dune-alugrid-2.9.dev20220529/doc/hexahedron_edges_alugrid.svg`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/doc/tetrahedron_alugrid.svg` & `dune-alugrid-2.9.dev20220529/doc/tetrahedron_alugrid.svg`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/doc/tetrahedron_edges_alugrid.svg` & `dune-alugrid-2.9.dev20220529/doc/tetrahedron_edges_alugrid.svg`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/alu3dinclude.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/alu3dinclude.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/alu3diterators.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/alu3diterators.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/alu3diterators_imp.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/alu3diterators_imp.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/alugrid.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/alugrid.hh`

 * *Files 10% similar despite different names*

```diff
@@ -34,32 +34,14 @@
 
     // the cube version of ALUGrid only works with nonconforming refinement
     static_assert( elType == cube ? refineType == nonconforming : true, "cube only works with nonconforming refinement");
 
     typedef ALUGrid< dim, dimworld, elType, refineType, Comm > This;
     typedef typename ALUGridBaseGrid< dim, dimworld, elType, Comm > :: BaseGrid  BaseType;
 
-    ALUGridRefinementType getRefinementType( const ALUGridRefinementType defaultRefType )
-    {
-      // for simplex grid we allow to dynamically switch to conforming refinement (experimental)
-      if constexpr ( elType == Dune::simplex && refineType == nonconforming )
-      {
-        // if environment var has been set (mainly from Python side)
-        if( getenv("ALUGRID_CONFORMING_REFINEMENT") )
-        {
-          const int conformingRefinement = atoi(getenv("ALUGRID_CONFORMING_REFINEMENT"));
-          if( bool(ALUGridExternalParameters::verbosityLevel()) )
-            std::cout << "ALUGrid: setting conforming refinement in constructor!" <<std::endl;
-          return conformingRefinement ? Dune::conforming : Dune::nonconforming;
-        }
-      }
-
-      return defaultRefType;
-    }
-
    public:
     typedef typename BaseType::MPICommunicatorType MPICommunicatorType;
 
     //! type of boundary projection
     typedef typename BaseType :: ALUGridVertexProjectionPairType  ALUGridVertexProjectionPairType;
 
     enum { dimension=BaseType::dimension,  dimensionworld=BaseType::dimensionworld};
@@ -86,30 +68,30 @@
     //!                   this pointer and will delete it in the desctructor
     //! \param verb       Whether to write a notice about grid creation to
     //!                   stdout.
     ALUGrid(const std::string macroName,
             const MPICommunicatorType mpiComm = BaseType::defaultCommunicator(),
             const ALUGridVertexProjectionPairType& bndPrj = ALUGridVertexProjectionPairType(),
             const bool verb = true ) :
-      BaseType(macroName, mpiComm, bndPrj, getRefinementType(refinementType) )
+      BaseType(macroName, mpiComm, bndPrj, refineType )
     {
       const bool verbose = verb && (this->comm().rank() == 0) && bool(ALUGridExternalParameters::verbosityLevel());
       if( verbose )
       {
-        std::cout << "\nCreated " << ALUGridParallelSerial< Comm >() << " " << name() << nameSuffix( this->conformingRefinement() )
+        std::cout << "\nCreated " << ALUGridParallelSerial< Comm >() << " " << name() << nameSuffix()
                   << " from macro grid file '" << macroName << "'. \n\n";
       }
     }
 
     static std::string name () { return std::string("ALUGrid"); }
 
-    static std::string nameSuffix( const bool conformingRefinement = false )
+    static std::string nameSuffix()
     {
-      std::string elt ( elType == cube ? "cube>" : "simplex>" );
-      std::string ref ( conformingRefinement ? " (conforming)": "" );
+      std::string elt ( elType == cube ? "cube," : "simplex," );
+      std::string ref ( refineType == nonconforming ? "nonconforming>" : "conforming>" );
       std::stringstream suffix;
       suffix << "<"<< dimension <<","<< dimensionworld <<"," << elt << ref;
       return suffix.str();
     }
 
 
     //! \brief constructor called from ALUGridFactory
@@ -121,36 +103,35 @@
     //! \param macroName filename from which ALUGrid is being generated
     //! \param verb       Whether to write a notice about grid creation to
     //!                   stdout.
     ALUGrid(const MPICommunicatorType mpiComm,
             const ALUGridVertexProjectionPairType& bndPrj,
             const std::string macroName,
             const bool verb = true ) :
-      BaseType("", mpiComm, bndPrj, getRefinementType(refinementType) )
+      BaseType("", mpiComm, bndPrj, refineType )
     {
       const bool verbose = verb && (this->comm().rank() == 0) && bool(ALUGridExternalParameters::verbosityLevel());
       if( verbose )
       {
-        std::cout << "\nCreated " << ALUGridParallelSerial< Comm >() << " " << name() << nameSuffix( this->conformingRefinement() );
+        std::cout << "\nCreated " << ALUGridParallelSerial< Comm >() << " " << name() << nameSuffix();
         if( macroName.empty() )
           std::cout << " from input stream. \n";
         else
           std::cout << " from macro grid file '" << macroName << "'. \n";
         std::cout << std::endl;
       }
     }
 
     //! constructor creating empty grid, empty string creates empty grid
     ALUGrid(const MPICommunicatorType mpiComm = BaseType::defaultCommunicator()) :
-      BaseType("", mpiComm, ALUGridVertexProjectionPairType(), getRefinementType(refinementType) )
+      BaseType("", mpiComm, ALUGridVertexProjectionPairType(), refineType )
     {
       if(this->comm().rank() == 0 && bool(ALUGridExternalParameters::verbosityLevel()) )
       {
-        std::cout << "\nCreated empty " << ALUGridParallelSerial< Comm >() << " "
-                  << name() << nameSuffix( this->conformingRefinement() ) << "." << std::endl << std::endl;
+        std::cout << "\nCreated empty " << ALUGridParallelSerial< Comm >() << " " << name() << nameSuffix() << "." << std::endl << std::endl;
       }
     }
 
     // ALUGrid only typedefs
     typedef typename BaseType::HierarchicIteratorImp HierarchicIteratorImp;
     typedef typename BaseType::ObjectStreamType      ObjectStreamType;
 
@@ -210,14 +191,11 @@
     //! Copy constructor should not be used
     ALUGrid( const ALUGrid & g ); //  : BaseType(g) {}
 
     //! assignment operator should not be used
     This& operator = (const ALUGrid& g);
   };
 
-  //template< int dim, int dimworld, ALUGridElementType elType, ALUGridRefinementType refineType, class Comm >
-  //using ALUGrid = ALUGrid< dim, dimworld, elType, Comm >;
-
 } //end  namespace Dune
 
 //#undef alu_inline
 #endif // #ifndef DUNE_ALU3DGRID_ALUGRID_HH
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/aluinline.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/aluinline.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/communication.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/communication.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/datacollectorcaps.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/datacollectorcaps.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/datahandle.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/datahandle.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/entity.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/entity.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/entity_imp.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/entity_imp.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/entity_inline.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/entity_inline.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/entityseed.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/entityseed.hh`

 * *Files 2% similar despite different names*

```diff
@@ -37,22 +37,22 @@
   typedef typename ImplTraits::HBndSegType HBndSegType;
 
   template <int cd, class Key>
   struct Bnd
   {
     static Key* toKey(const HBndSegType*)
     {
-      return nullptr;
+      return (Key*) 0;
     }
     static HElementType* getItem(KeyType* key)
     {
       return static_cast< HElementType* > ( key );
     }
     static bool isGhost(KeyType*) { return false; }
-    static BNDFaceType* ghost( KeyType*  ) { return nullptr; }
+    static BNDFaceType* ghost( KeyType*  ) { return ( BNDFaceType* ) 0; }
   };
   template <class Key>
   struct Bnd<0, Key>
   {
     static Key* toKey(const HBndSegType* ghostFace)
     {
       return static_cast< KeyType* > (const_cast< BNDFaceType* >( static_cast<const BNDFaceType*> (ghostFace)));
@@ -69,15 +69,15 @@
         {
           // we cannot cast to HElement here, since only the implementation is derived
           // from hasFace
           return static_cast< HElementType * > (static_cast< ImplementationType* > (key));
         }
       }
       else
-        return nullptr;
+        return static_cast< HElementType * > (0) ;
     }
     static bool isGhost(KeyType* key) { alugrid_assert ( key ); return key->isboundary(); }
     static BNDFaceType* ghost( KeyType* key ) { alugrid_assert ( key ); return (static_cast< BNDFaceType* > ( key )); }
   };
 public:
   static const int defaultValue = -1 ;
   static const int defaultTwist = 0 ;
@@ -148,15 +148,15 @@
   //////////////////////////////////////////////////////
   //! equality
   bool equals (const ALU3dGridEntitySeedType& i) const;
 
   //! invalidate seed
   void clear()
   {
-    item_ = nullptr;
+    item_ = 0;
   }
 
   //! get item from key
   HElementType* item() const { return Bnd<codim,KeyType>::getItem( item_ ); }
 
   //! return iterior item
   HElementType* interior() const
@@ -232,16 +232,20 @@
   //! type of Entity
   typedef typename GridImp::template Codim<cd>::Entity Entity;
 
   //! typedef of my type
   typedef ALU3dGridEntitySeed<cd,GridImp> ALU3dGridEntitySeedType;
 
   //! Constructor for EntitySeed that points to an element
-  //! this constructor should only be called by codim=0 entity keys
-  ALU3dGridEntitySeed(const ImplementationType & item) = delete;
+  ALU3dGridEntitySeed(const ImplementationType & item)
+  {
+    // this constructor should only be called by codim=0 entity keys
+    alugrid_assert ( false );
+    abort();
+  }
 
   //! Constructor for EntitySeed that points to an element
   ALU3dGridEntitySeed(const HElementType & item,
                       const int level,
                       const int twist = defaultTwist
                     );
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/faceutility.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/faceutility.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/faceutility.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/faceutility.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/faceutility_imp.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/faceutility_imp.cc`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
       // set to default boundary (with domain boundary)
       bndType_ = domainBoundary ;
 
       // check for ghosts
       // this check is only need in the parallel case
       // if this cast fails we have a periodic element
       const BNDFaceType * bnd = dynamic_cast<const BNDFaceType *> (outerElement_);
-      const bool periodicBnd = ( bnd == nullptr ) ;
+      const bool periodicBnd = ( bnd == 0 ) ;
 
       if( periodicBnd ) // the periodic case
       {
         bndType_ = periodicBoundary ;
         alugrid_assert ( dynamic_cast< const GEOPeriodicType* > ( outerElement_ ) );
         const GEOPeriodicType* periodicClosure = static_cast< const GEOPeriodicType* > ( outerElement_ ) ;
 
@@ -394,17 +394,16 @@
 
     const int mappedZero =
       FaceTopo::twist(ElementTopo::dune2aluFaceVertex( faceIdx, 0), aluTwist);
 
     const int twist =
       (ElementTopo::faceOrientation( faceIdx ) * sign(aluTwist) < 0 ?
        mappedZero : -mappedZero-1);
-
     // see topology.* files for aluTwistMap
-    if constexpr ( dim == 2 )
+    if( dim == 2 )
     {
       // in 2d twists are either 0 or 1, but because
       // of the underlying 3d alu grid they could be different
       // therefore we adjust to the right range
       const int duneTwst = FaceTopo :: aluTwistMap( twist );
       return (duneTwst == 0) ? 0 : 1;
     }
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/geometry.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/geometry.hh`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #define DUNE_ALU3DGRIDGEOMETRY_HH
 
 // System includes
 #include <memory>
 #include <type_traits>
 
 // Dune includes
+#include <dune/common/version.hh>
 #include <dune/common/math.hh>
 
 #include <dune/grid/common/grid.hh>
 
 // Local includes
 #include "alu3dinclude.hh"
 #include "topology.hh"
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/geometry_imp.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/geometry_imp.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/grid.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/grid.hh`

 * *Files 2% similar despite different names*

```diff
@@ -120,16 +120,15 @@
   struct ALU3dGridCommunications< dim, dimworld, elType, ALUGridNoComm >
   {
     typedef ALU3dGridLocalIdSet< dim, dimworld, elType, ALUGridNoComm > GlobalIdSet;
     typedef int GlobalId;
 
     typedef ALU3DSPACE GitterDuneImpl GitterImplType;
 
-    typedef Dune::Communication< No_Comm > Communication;
-    typedef Communication CollectiveCommunication;
+    typedef Dune::CollectiveCommunication< No_Comm > CollectiveCommunication;
 
     explicit ALU3dGridCommunications ( ALUGridNoComm comm ) {}
 
     int nlinks () const { return 0; }
 
     GitterImplType *createALUGrid ( const std::string &macroName, const ALU3DSPACE ProjectVertexPtrPair& projections,
                                     const bool conformingRefinement )
@@ -160,28 +159,27 @@
     }
 
     static void completeGrid ( GitterImplType &grid ) {}
 
     void print( std::ostream& out ) const
     {}
 
-    Communication ccobj_;
+    CollectiveCommunication ccobj_;
   };
 
 #if ALU3DGRID_PARALLEL
   template< int dim, int dimworld, ALU3dGridElementType elType >
   struct ALU3dGridCommunications< dim, dimworld, elType, ALUGridMPIComm >
   {
     typedef ALU3dGridGlobalIdSet< dim, dimworld, elType, ALUGridMPIComm > GlobalIdSet;
     typedef ALUGridId< ALUMacroKey > GlobalId;
 
     typedef ALU3DSPACE GitterDunePll GitterImplType;
 
-    typedef Dune::Communication< MPI_Comm > Communication;
-    typedef Communication CollectiveCommunication;
+    typedef Dune::CollectiveCommunication< MPI_Comm > CollectiveCommunication;
 
     explicit ALU3dGridCommunications ( MPI_Comm comm )
     : ccobj_( comm ), mpAccess_( comm )
     {}
 
     int nlinks () const { return mpAccess_.sendLinks(); }
 
@@ -225,15 +223,15 @@
     {
       // setup communication patterns
       grid.notifyMacroGridChanges();
       // rebuild ghost cells
       grid.rebuildGhostCells();
     }
 
-    Communication ccobj_;
+    CollectiveCommunication ccobj_;
     ALU3DSPACE MpAccessMPI mpAccess_;
   };
 #endif // #if ALU3DGRID_PARALLEL
 
 
 
   // ALU3dGridTwist
@@ -378,18 +376,15 @@
 
       typedef IndexSet< Grid, LevelIndexSetImp > LevelIndexSet;
       typedef IndexSet< Grid, LeafIndexSetImp > LeafIndexSet;
       typedef IdSet< Grid, LocalIdSetImp, LocalIdType > LocalIdSet;
       typedef IdSet< Grid, GlobalIdSetImp, GlobalIdType > GlobalIdSet;
 
       //! Type of the communication class
-      typedef typename ALU3dGridCommunications< dim, dimworld, elType, Comm >::Communication Communication;
-
-      [[deprecated("Use Communication instead!")]]
-      typedef Communication CollectiveCommunication;
+      typedef typename ALU3dGridCommunications< dim, dimworld, elType, Comm >::CollectiveCommunication CollectiveCommunication;
     }; // struct Traits
 
     //! Type of the level index set implementation
     typedef typename Traits :: LevelIndexSetImp  LevelIndexSetImp;
 
     //! Type of the leaf index set implementation
     typedef typename Traits :: LeafIndexSetImp   LeafIndexSetImp;
@@ -550,18 +545,15 @@
     typedef ALU3DSPACE ProjectVertex  ALUGridVertexProjectionType;
 
     //! type of ALUGrid Vertex Projection Interface (shared_ptr)
     typedef ALU3DSPACE ProjectVertexPtr       ALUGridVertexProjectionPointerType;
     typedef ALU3DSPACE ProjectVertexPtrPair   ALUGridVertexProjectionPairType;
 
     //! type of collective communication object
-    typedef typename Traits::Communication Communication;
-
-    [[deprecated("Use Communication instead!")]]
-    typedef Communication CollectiveCommunication;
+    typedef typename Traits::CollectiveCommunication CollectiveCommunication;
 
     typedef ALULeafCommunication< dim, dimworld, elType, Comm > LeafCommunication;
     typedef ALULevelCommunication< dim, dimworld, elType, Comm > LevelCommunication;
 
   protected:
     //! Type of the local id set
     typedef typename GridFamily::LocalIdSetImp LocalIdSetImp;
@@ -1002,15 +994,15 @@
     void finalizeGridCreation();
 
     //! clear all entity new markers
     void clearIsNewMarkers( );
 
   public:
     /** \brief @copydoc Dune::Grid::comm() */
-    const Communication &comm () const { return communications().ccobj_; }
+    const CollectiveCommunication &comm () const { return communications().ccobj_; }
 
     //! returns if a least one entity was marked for coarsening
     bool preAdapt ( );
 
     //! clear all entity new markers if lockPostAdapt_ is set
     void postAdapt ( );
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/grid_imp.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/grid_imp.cc`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     typedef typename ImplTraits::VertexType VertexType;
 
     enum { nVx = ElementTopologyMapping < elType > :: numVertices };
 
     ElementIteratorType it ( grid, grid.maxLevel() , grid.nlinks() );
 
 #ifdef ALUGRIDDEBUG
-    [[maybe_unused]] int count = 0;
+    int count = 0;
 #endif
     for( it.first(); !it.done() ; it.next())
     {
       val_t & item = it.item();
 
       IMPLElementType * elem = 0;
       if( item.first )
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/grid_inline.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/grid_inline.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/gridfactory.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/gridfactory.cc`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
     // if type of curve is chosen to be None, nothing more to be done here
     if( curveType_ == SpaceFillingCurveOrderingType :: None )
       return ;
 
     {
       // apply space filling curve orderung to the inserted elements
       // see common/hsfc.hh for details
-      typename ALUGrid::Communication comm( communicator_ );
+      typename ALUGrid::CollectiveCommunication comm( communicator_ );
 
       // if we are in parallel insertion mode we need communication
       const bool foundGlobalIndex = comm.max( foundGlobalIndex_ );
       if( foundGlobalIndex && comm.size() > 1 )
       {
         if( comm.rank() == 0 )
           std::cerr << "WARNING: Space filling curve ordering does not work for parallel grid factory, yet!" << std::endl;
@@ -818,29 +818,29 @@
             perel[ i+0 ] = globalId( facePair.first.first[ i ] );
             perel[ i+4 ] = globalId( facePair.second.first[ i ] );
           }
 
           typedef typename ALU3DSPACE Gitter::hbndseg::bnd_t bnd_t ;
           bnd_t bndId[ 2 ] = { bnd_t( facePair.first.second ),
                                bnd_t( facePair.second.second ) };
-          mgb.InsertUniquePeriodic( perel, bndId );
+          mgb.InsertUniquePeriodic4( perel, bndId );
 
         }
         else if( elementType == tetra )
         {
           int perel[ 6 ];
           for( unsigned int i = 0; i < 3; ++i )
           {
             perel[ i+0 ] = globalId( facePair.first.first[ (3 - i) % 3 ] );
             perel[ i+3 ] = globalId( facePair.second.first[ (3 - i) % 3 ] );
           }
           typedef typename ALU3DSPACE Gitter::hbndseg::bnd_t bnd_t ;
           bnd_t bndId[ 2 ] = { bnd_t( facePair.first.second ),
                                bnd_t( facePair.second.second ) };
-          mgb.InsertUniquePeriodic( perel, bndId );
+          mgb.InsertUniquePeriodic3( perel, bndId );
         }
         else
           DUNE_THROW( GridError, "Invalid element type" );
       }
     }
 
     // free memory
@@ -1300,15 +1300,15 @@
     for( const auto& key : toBeDeletedFaces )
     {
       faceMap.erase( key );
     }
 
     // communicate unidentified boundaries and find process borders)
     // use the Grids communicator (ALUGridNoComm or ALUGridMPIComm)
-    typename ALUGrid::Communication comm( communicator_ );
+    typename ALUGrid::CollectiveCommunication comm( communicator_ );
 
     int numBoundariesMine = faceMap.size();
     std::vector< int > boundariesMine( numFaceCorners * numBoundariesMine );
     typedef std::map< FaceType, FaceType, FaceLess > GlobalToLocalFaceMap;
     GlobalToLocalFaceMap globalFaceMap;
     {
       const FaceIterator faceEnd = faceMap.end();
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/gridfactory.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/gridfactory.hh`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 #include <algorithm>
 #include <array>
 #include <map>
 #include <memory>
 #include <vector>
 
+// #include <dune/common/shared_ptr.hh>
 #include <dune/common/parallel/mpihelper.hh>
+#include <dune/common/version.hh>
 
 #include <dune/geometry/referenceelements.hh>
 
 #include <dune/grid/common/gridfactory.hh>
 #include <dune/grid/common/boundaryprojection.hh>
 
 #include <dune/alugrid/common/transformation.hh>
@@ -53,15 +55,15 @@
     typedef ALUGridTransformation< ctype, dimensionworld > Transformation;
 
     //! type of vector for world coordinates
     typedef typename Transformation::WorldVector WorldVector;
     //! type of matrix from world coordinates to world coordinates
     typedef typename Transformation::WorldMatrix WorldMatrix;
 
-    typedef typename Grid::Communication Communication;
+    typedef typename Grid::CollectiveCommunication Communication;
 
     // typedef grid pointer type based on what the grid factory interface defines
     typedef decltype(std::declval< Dune::GridFactoryInterface< Grid >* >()->createGrid())  GridPtrType;
 
   private:
     static_assert ( (elementType == tetra || elementType == hexa),
                     "ALU3dGridFactory supports only grids containing "
@@ -412,14 +414,15 @@
     bool markLongestEdge_;
   };
 
 
 
   template< class ALUGrid >
   struct ALU3dGridFactory< ALUGrid >::FaceLess
+  : public std::binary_function< FaceType, FaceType, bool >
   {
     bool operator() ( const FaceType &a, const FaceType &b ) const
     {
       for( unsigned int i = 0; i < numFaceCorners; ++i )
       {
         if( a[ i ] != b[ i ] )
           return (a[ i ] < b[ i ]);
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/gridview.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/gridview.hh`

 * *Files 3% similar despite different names*

```diff
@@ -33,17 +33,16 @@
     /** \brief type of the intersection */
     typedef typename Grid :: Traits :: LevelIntersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Grid :: Traits :: LevelIntersectionIterator
     IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Grid :: Traits :: Communication Communication;
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Grid :: Traits :: CollectiveCommunication CollectiveCommunication;
 
     template< int cd >
     struct Codim
     {
       typedef typename Grid::Traits::template Codim< cd >::Twists Twists;
       typedef typename Twists::Twist Twist;
 
@@ -88,17 +87,16 @@
 
     /** \brief type of the intersection */
     typedef typename Traits :: Intersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Traits :: IntersectionIterator IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Traits :: Communication Communication;
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Traits :: CollectiveCommunication CollectiveCommunication;
 
     /** \brief Codim Structure */
     template< int cd >
     struct Codim : public Traits :: template Codim<cd> {};
 
     enum { conforming = Traits :: conforming };
 
@@ -178,16 +176,16 @@
     /** \brief obtain end intersection iterator with respect to this view */
     IntersectionIterator
     iend ( const typename Codim< 0 > :: Entity &entity ) const
     {
       return grid().ilevelend( entity );
     }
 
-    /** \brief obtain communication object */
-    const Communication &comm () const
+    /** \brief obtain collective communication object */
+    const CollectiveCommunication &comm () const
     {
       return grid().comm();
     }
 
     /** \brief Return size of the overlap region for a given codim on the grid view.  */
     int overlapSize(int codim) const
     {
@@ -234,17 +232,16 @@
     /** \brief type of the intersection */
     typedef typename Grid :: Traits :: LeafIntersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Grid :: Traits :: LeafIntersectionIterator
     IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Grid :: Traits :: Communication Communication;
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Grid :: Traits :: CollectiveCommunication CollectiveCommunication;
 
     template< int cd >
     struct Codim
     {
       typedef typename Grid::Traits::template Codim< cd >::Twists Twists;
       typedef typename Twists::Twist Twist;
 
@@ -289,17 +286,16 @@
 
     /** \brief type of the intersection */
     typedef typename Traits :: Intersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Traits :: IntersectionIterator IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Traits :: Communication Communication;
-    typedef Communication CollectiveCommunication;
+    /** \brief type of the collective communication */
+    typedef typename Traits :: CollectiveCommunication CollectiveCommunication;
 
     /** \brief Codim Structure */
     template< int cd >
     struct Codim : public Traits :: template Codim<cd> {};
 
     enum { conforming = Traits :: conforming };
 
@@ -374,16 +370,16 @@
     /** \brief obtain end intersection iterator with respect to this view */
     IntersectionIterator
     iend ( const typename Codim< 0 > :: Entity &entity ) const
     {
       return grid().ileafend( entity );
     }
 
-    /** \brief obtain communication object */
-    const Communication &comm () const
+    /** \brief obtain collective communication object */
+    const CollectiveCommunication &comm () const
     {
       return grid().comm();
     }
 
     /** \brief Return size of the overlap region for a given codim on the grid view.  */
     int overlapSize(int codim) const
     {
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/indexsets.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/indexsets.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/indexsets.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/indexsets.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/iterator.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/iterator.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/iterator.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/iterator.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/iterator_imp.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/iterator_imp.cc`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 assign(const ALU3dGridIntersectionIterator<GridImp> & org)
 {
   if(org.item_)
   {
     // adjust connector flags
     connector_.setFlags( org.connector_.conformingRefinement(), org.connector_.ghostCellsEnabled() );
 
-    // else it's an end iterator
+    // else it's a end iterator
     item_       = org.item_;
     ghost_      = org.ghost_;
     grid_       = org.grid_;
     innerLevel_ = org.innerLevel_;
     index_      = org.index_;
     connector_.updateFaceInfo(org.connector_.face(),innerLevel_,
                               item_->twist(ElementTopo::dune2aluFace(index_)));
@@ -307,34 +307,15 @@
   return Twist( connector_.duneTwist( indexInInside(), connector_.innerTwist() ) );
 }
 
 template< class GridImp >
 alu_inline typename ALU3dGridIntersectionIterator< GridImp >::Twist
 ALU3dGridIntersectionIterator< GridImp >::twistInOutside () const
 {
-  const int indexOutside = indexInOutside();
-  auto twist = Twist( connector_.duneTwist( indexOutside, connector_.outerTwist() ) );
-
-  if constexpr ( GridImp :: dimension == 2 )
-  {
-    // fix for periodic boundaries (in 2d)
-    if( neighbor() && boundary() )
-    {
-      const int indexInside = indexInInside();
-      // max face number in 2d, 3 for quads and 2 for triangles
-      constexpr int maxFaceNum  = (GridImp::elementType == hexa) ? 3 : 2;
-      if( indexInside == indexOutside ||
-          std::abs(indexInside - indexOutside ) == maxFaceNum )
-      {
-        // flip twist in these cases
-        twist = Twist( 1 - int(twist) );
-      }
-    }
-  }
-  return twist;
+  return Twist( connector_.duneTwist( indexInOutside(), connector_.outerTwist() ) );
 }
 
 template< class GridImp >
 alu_inline typename ALU3dGridIntersectionIterator< GridImp >::LocalGeometry
 ALU3dGridIntersectionIterator< GridImp >::geometryInOutside () const
 {
   alugrid_assert (neighbor());
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/mappings.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/mappings.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/mappings.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/mappings.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/mappings_imp.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/mappings_imp.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/topology.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/topology.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/3d/topology.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/3d/topology.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/backuprestore.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/backuprestore.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/bisectioncompatibility.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/bisectioncompatibility.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/bndprojection.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/bndprojection.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/capabilities.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/capabilities.hh`

 * *Files 1% similar despite different names*

```diff
@@ -63,24 +63,24 @@
     */
     template< int dim, int dimworld, ALUGridElementType eltype, ALUGridRefinementType refinementtype, int codim >
     struct canCommunicate< ALUGrid< dim, dimworld, eltype, refinementtype, ALUGridMPIComm >, codim >
     {
       static const bool v = true;
     };
 
-    /** \brief ALUGrid has potentially nonconforming level grids
+    /** \brief ALUGrid has conforming level grids
     \ingroup ALUGrid
     */
     template< int dim, int dimworld, ALUGridElementType eltype, ALUGridRefinementType refinementtype, class Comm >
     struct isLevelwiseConforming< ALUGrid< dim, dimworld, eltype, refinementtype, Comm > >
     {
-      static const bool v = false;
+      static const bool v = refinementtype == nonconforming;
     };
 
-    /** \brief ALUGrid has potentially nonconforming leaf grids (unless refinementtype is conforming)
+    /** \brief ALUGrid has conforming level grids
     \ingroup ALUGrid
     */
     template< int dim, int dimworld, ALUGridElementType eltype, ALUGridRefinementType refinementtype, class Comm >
     struct isLeafwiseConforming< ALUGrid< dim, dimworld, eltype, refinementtype, Comm > >
     {
       static const bool v = refinementtype == conforming ;
     };
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/declaration.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/declaration.hh`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,16 @@
     simplex, //!< use only simplex elements (i.e., triangles or tetrahedra)
     cube     //!< use only cube elements (i.e., quadrilaterals or hexahedra)
   };
 
   //! \brief available refinement types for ALUGrid
   enum ALUGridRefinementType
   {
-    conforming,   //!< use only conforming bisection refinement
-    nonconforming //!< use non-conforming (red) refinement by default,
-                  //!< conforming can be enabled by env flag (experimental).
+    conforming,   //!< use conforming bisection refinement
+    nonconforming //!< use non-conforming (red) refinement
   };
 
   //! \brief type of class for specialization of serial ALUGrid (No_Comm as communicator)
   struct ALUGridNoComm
   {
     No_Comm noComm_;
     ALUGridNoComm() : noComm_() {}
@@ -57,23 +56,22 @@
    * hexahedral as well as 2D triangular and 3D tetrahedral meshes.
    * This grid can be locally adapted (non-conforming and conforming bisection)
    * and used in parallel computations using dynamic load balancing.
    *
    * \tparam  dim         dimension of the grid (2 or 3)
    * \tparam  dimworld    dimension of the surrounding space (dim <= dimworld <=3)
    * \tparam  elType      type of elements (Dune::simplex or Dune::cube)
-   * \tparam  refineType  defaults to Dune::nonconforming, Dune::conforming is deprecated
+   * \tparam  refineType  type of refinement (Dune::conforming or Dune::nonconforming)
    * \tparam  Comm        type of communicator (Dune::ALUGridMPIComm or Dune::ALUGridNoComm)
    *
    * \note For cube elements, only nonconforming refinement is available.
    * \note The template parameter Comm defaults to ALUGridMPIComm, if MPI is available.
    *       Otherwise it defaults to ALUGridNoComm.
    */
-  template <int dim, int dimworld, ALUGridElementType elType,
-            ALUGridRefinementType refineType = nonconforming,
+  template <int dim, int dimworld, ALUGridElementType elType, ALUGridRefinementType refineType,
             class Comm =
 #if ALU3DGRID_PARALLEL
               ALUGridMPIComm
 #else
               ALUGridNoComm
 #endif
            >
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/defaultindexsets.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/defaultindexsets.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/duneassert.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/duneassert.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/fromtogridfactory.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/fromtogridfactory.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/geostorage.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/geostorage.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/hsfc.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/hsfc.hh`

 * *Files 3% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 
 namespace ALUGridSFC {
 
   template <class Coordinate>
   class ZoltanSpaceFillingCurveOrdering
   {
     // type of communicator
-    typedef Dune :: Communication< typename Dune :: MPIHelper :: MPICommunicator >
-        Communication ;
+    typedef Dune :: CollectiveCommunication< typename Dune :: MPIHelper :: MPICommunicator >
+        CollectiveCommunication ;
 
 #if ! HAVE_ZOLTAN
     typedef void                      Zoltan_Struct;
-    typedef Communication   Zoltan;
+    typedef CollectiveCommunication   Zoltan;
 #endif
 
     // type of Zoltan HSFC ordering function
     typedef double zoltan_hsfc_inv_t(Zoltan_Struct *zz, double *coord);
 
     static const int dimension = Coordinate::dimension;
 
@@ -47,16 +47,16 @@
     zoltan_hsfc_inv_t* hsfcInv_;
 
     mutable Zoltan zz_;
 
   public:
     ZoltanSpaceFillingCurveOrdering( const Coordinate& lower,
                                      const Coordinate& upper,
-                                     const Communication& comm =
-                                     Communication( Dune::MPIHelper::getCommunicator() ) )
+                                     const CollectiveCommunication& comm =
+                                     CollectiveCommunication( Dune::MPIHelper::getCommunicator() ) )
       : lower_( lower ),
         length_( upper ),
 #if HAVE_ZOLTAN
         hsfcInv_( dimension == 3 ? Zoltan_HSFC_InvHilbert3d : Zoltan_HSFC_InvHilbert2d ),
 #else
         hsfcInv_( 0 ),
 #endif
@@ -165,16 +165,16 @@
   template <class Coordinate>
   class SpaceFillingCurveOrdering
   {
     typedef ::ALUGridSFC::ZCurve< long int, Coordinate::dimension>      ZCurveOrderingType;
     typedef ::ALUGridSFC::ZoltanSpaceFillingCurveOrdering< Coordinate > HilbertOrderingType;
 
     // type of communicator
-    typedef Dune :: Communication< typename MPIHelper :: MPICommunicator >
-        Communication ;
+    typedef Dune :: CollectiveCommunication< typename MPIHelper :: MPICommunicator >
+        CollectiveCommunication ;
   public:
     enum CurveType { ZCurve, Hilbert, None };
 
 #if HAVE_ZOLTAN
     static const CurveType DefaultCurve = Hilbert ;
 #else
     static const CurveType DefaultCurve = ZCurve ;
@@ -186,33 +186,33 @@
 
     const CurveType curveType_;
 
   public:
     SpaceFillingCurveOrdering( const CurveType& curveType,
                                const Coordinate& lower,
                                const Coordinate& upper,
-                               const Communication& comm =
-                               Communication( Dune::MPIHelper::getCommunicator() ) )
+                               const CollectiveCommunication& comm =
+                               CollectiveCommunication( Dune::MPIHelper::getCommunicator() ) )
       : zCurve_ ( lower, upper, comm )
       , hilbert_( lower, upper, comm )
       , curveType_( curveType )
     {
     }
 
     template <class OtherComm>
     SpaceFillingCurveOrdering( const CurveType& curveType,
                                const Coordinate& lower,
                                const Coordinate& upper,
                                const OtherComm& otherComm )
       : zCurve_ ( lower, upper,
-                  otherComm.size() > 1 ? Communication( Dune::MPIHelper::getCommunicator() ) :
-                                         Communication( Dune::MPIHelper::getLocalCommunicator() ) )
+                  otherComm.size() > 1 ? CollectiveCommunication( Dune::MPIHelper::getCommunicator() ) :
+                                         CollectiveCommunication( Dune::MPIHelper::getLocalCommunicator() ) )
       , hilbert_( lower, upper,
-                  otherComm.size() > 1 ? Communication( Dune::MPIHelper::getCommunicator() ) :
-                                         Communication( Dune::MPIHelper::getLocalCommunicator() ) )
+                  otherComm.size() > 1 ? CollectiveCommunication( Dune::MPIHelper::getCommunicator() ) :
+                                         CollectiveCommunication( Dune::MPIHelper::getLocalCommunicator() ) )
       , curveType_( curveType )
     {
     }
 
     // return unique hilbert index in interval [0,1] given an element's center
     double index( const Coordinate& point ) const
     {
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/interfaces.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/interfaces.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/intersectioniteratorwrapper.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/intersectioniteratorwrapper.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/macrogridview.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/macrogridview.hh`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     /** \brief type of the intersection */
     typedef typename Grid :: Traits :: LevelIntersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Grid :: Traits :: LevelIntersectionIterator
       IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Grid :: Traits :: Communication Communication;
+    /** \brief type of the collective communication */
+    typedef typename Grid :: Traits :: CollectiveCommunication CollectiveCommunication;
 
     template< int cd >
     struct Codim
     {
       typedef typename Grid :: Traits
         :: template Codim< cd > :: template Partition< pitype > :: LevelIterator
         Iterator;
@@ -84,16 +84,16 @@
 
     /** \brief type of the intersection */
     typedef typename Traits :: Intersection Intersection;
 
     /** \brief type of the intersection iterator */
     typedef typename Traits :: IntersectionIterator IntersectionIterator;
 
-    /** \brief type of the communication */
-    typedef typename Traits :: Communication Communication;
+    /** \brief type of the collective communication */
+    typedef typename Traits :: CollectiveCommunication CollectiveCommunication;
 
     /** \brief Codim Structure */
     template< int cd >
     struct Codim : public Traits :: template Codim<cd> {};
 
     enum {
       //! \brief Export if this grid view is conforming */
@@ -188,16 +188,16 @@
     IntersectionIterator
     iend ( const typename Codim< 0 > :: Entity &entity ) const
     {
       assert( entity.level() == level_ );
       return grid().ilevelend( entity );
     }
 
-    /** \brief obtain communication object */
-    const Communication &comm () const
+    /** \brief obtain collective communication object */
+    const CollectiveCommunication &comm () const
     {
       return grid().comm();
     }
 
     /** \brief Return size of the overlap region for a given codim on the grid view.  */
     int overlapSize(int codim) const
     {
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/memory.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/memory.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/meshquality.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/meshquality.hh`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 namespace Dune {
 
   template <class GridView>
   static void meshQuality( const GridView& gridView, const double time, std::ostream& out )
   {
     static const int dim = GridView::dimension;
-    if ( dim < 3 ) return ;
 
     double minVolShortestEdgeRatio = 1e308;
     double maxVolShortestEdgeRatio = 0;
     double avgVolShortestEdgeRatio = 0;
 
     double minVolLongestEdgeRatio = 1e308;
     double maxVolLongestEdgeRatio = 0;
@@ -69,18 +68,16 @@
     for( const auto& element : elements( gridView, Dune::Partitions::interiorBorder ) )
     {
       const double vol = element.geometry().volume();
       const Dune::GeometryType geomType = element.type();
 
       if( ! geomType.isSimplex() )
       {
-        static bool firstCall = true;
-        if( gridView.comm().rank() == 0 && firstCall )
+        if( gridView.comm().rank() == 0 )
         {
-          firstCall = false;
           std::cout << "MeshQuality check only works for simplex grids, skipping check!" << std::endl;
         }
         return ;
       }
 
       const double factorEdge     = geomType.isCube() ? 1.0 : factorEdgeTet;
       const double factorFaceEdge = geomType.isCube() ? 1.0 : factorFaceEdgeTet;
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/persistentcontainer.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/persistentcontainer.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/structuredgridfactory.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/structuredgridfactory.hh`

 * *Files 2% similar despite different names*

```diff
@@ -73,22 +73,23 @@
       static const int dimension = Grid::dimension;
 
       typedef typename Grid::template Codim< 0 >::Entity Element;
 
       typedef typename Element::Geometry::GlobalCoordinate VertexType;
 
       // type of communicator
-      typedef Dune :: Communication< typename MPIHelper :: MPICommunicator >  Communication ;
+      typedef Dune :: CollectiveCommunication< typename MPIHelper :: MPICommunicator >
+        CollectiveCommunication ;
 
 #ifdef USE_ALUGRID_SFC_ORDERING
       typedef SpaceFillingCurveOrdering< VertexType >  SpaceFillingCurveOrderingType;
 #endif
 
     public:
-      SimplePartitioner ( const GridView &gridView, const Communication& comm,
+      SimplePartitioner ( const GridView &gridView, const CollectiveCommunication& comm,
                           const VertexType& lowerLeft, const VertexType& upperRight )
       : comm_( comm ),
         gridView_( gridView ),
         indexSet_( gridView_.indexSet() ),
         pSize_( comm_.size() ),
         elementCuts_( pSize_, -1 ),
 #ifdef USE_ALUGRID_SFC_ORDERING
@@ -176,15 +177,15 @@
         // of elements per process
         double percentage = (double(nElements) / double( nRanks ));
         percentage -= minPerProc ;
         percentage *= nRanks ;
 
         int rank = 0;
         size_t elementCount  = maxPerProc ;
-        [[maybe_unused]] size_t elementNumber = 0;
+        size_t elementNumber = 0;
         size_t localElementNumber = 0;
         const int lastRank = nRanks - 1;
 
         const size_t size = indexSet_.size( 0 );
         for( size_t i=0; i<size; ++i )
         {
           if( localElementNumber >= elementCount )
@@ -210,15 +211,15 @@
         // set cut for last process
         elementCuts_[ lastRank ] = size ;
 
         //for( int p=0; p<pSize_; ++p )
         //  std::cout << "P[ " << p << " ] = " << elementCuts_[ p ] << std::endl;
       }
 
-      const Communication& comm_;
+      const CollectiveCommunication& comm_;
 
       const GridView& gridView_;
       const IndexSet &indexSet_;
 
       const int pSize_;
       std::vector< long int > elementCuts_ ;
 
@@ -230,16 +231,16 @@
     };
 
   public:
     typedef typename Grid::ctype ctype;
     typedef typename MPIHelper :: MPICommunicator MPICommunicatorType ;
 
     // type of communicator
-    typedef Dune :: Communication< MPICommunicatorType >
-        Communication ;
+    typedef Dune :: CollectiveCommunication< MPICommunicatorType >
+        CollectiveCommunication ;
 
     static SharedPtrType
     createCubeGrid( const std::string& filename,
                     MPICommunicatorType mpiComm = MPIHelper :: getCommunicator() )
     {
       std::ifstream file( filename.c_str() );
       if( ! file )
@@ -250,15 +251,15 @@
     }
 
     static SharedPtrType
     createCubeGrid( std::istream& input,
                     const std::string& name,
                     MPICommunicatorType mpiComm = MPIHelper :: getCommunicator() )
     {
-      Communication comm( MPIHelper :: getCommunicator() );
+      CollectiveCommunication comm( MPIHelper :: getCommunicator() );
       static_assert( dim == dimworld, "YaspGrid is used for creation of the structured grid which only supports dim == dimworld");
 
       // if periodic transformations are active we cannot use the YaspGrid
       // approach to insert the grid cells, otherwise the periodic elements
       // are not inserted
       dgf::PeriodicFaceTransformationBlock trafoBlock( input, dimworld );
       if( trafoBlock.isactive() )
@@ -342,15 +343,15 @@
 
     static SharedPtrType
     createCubeGrid ( const FieldVector<ctype,dimworld>& lowerLeft,
                      const FieldVector<ctype,dimworld>& upperRight,
                      const std::array<unsigned int, dim>& elements,
                      MPICommunicatorType mpiComm = MPIHelper :: getCommunicator() )
     {
-      Communication comm( mpiComm );
+      CollectiveCommunication comm( mpiComm );
       std::string name( "Cartesian ALUGrid via YaspGrid" );
       return createCubeGridImpl( lowerLeft, upperRight, elements, comm, name );
     }
 
   protected:
     template <int codim, class Entity>
     int subEntities ( const Entity& entity ) const
@@ -359,24 +360,24 @@
     }
 
     template < class int_t >
     static SharedPtrType
     createCubeGridImpl ( const FieldVector<ctype,dimworld>& lowerLeft,
                          const FieldVector<ctype,dimworld>& upperRight,
                          const std::array< int_t, dim>& elements,
-                         const Communication& comm,
+                         const CollectiveCommunication& comm,
                          const std::string& name )
     {
       const int myrank = comm.rank();
 
       typedef YaspGrid< dimworld, EquidistantOffsetCoordinates<double,dimworld> > CartesianGridType ;
       std::array< int, dim > dims;
       for( int i=0; i<dim; ++i ) dims[ i ] = elements[ i ];
 
-      Communication commSelf( MPIHelper :: getLocalCommunicator() );
+      CollectiveCommunication commSelf( MPIHelper :: getLocalCommunicator() );
       // create YaspGrid to partition and insert elements that belong to process directly
       CartesianGridType sgrid( lowerLeft, upperRight, dims, std::bitset<dim>(0ULL), 1, commSelf );
 
       typedef typename CartesianGridType :: LeafGridView GridView ;
       typedef typename GridView  :: IndexSet  IndexSet ;
       typedef typename IndexSet  :: IndexType IndexType ;
       typedef typename GridView  :: template Codim< 0 > :: Iterator ElementIterator ;
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/transformation.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/transformation.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/twists.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/twists.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/typetraits.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/typetraits.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/common/writeparalleldgf.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/common/writeparalleldgf.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/dgf.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/dgf.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/grid.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/grid.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/binaryio.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/binaryio.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/binaryio.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/binaryio.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/byteorder.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/byteorder.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/duneinterface/gitter_dune_impl.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/duneinterface/gitter_dune_impl.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/duneinterface/gitter_dune_impl.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/duneinterface/gitter_dune_impl.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/duneinterface/gitter_dune_pll_impl.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/duneinterface/gitter_dune_pll_impl.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/duneinterface/gitter_dune_pll_impl.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/duneinterface/gitter_dune_pll_impl.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/indexstack.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/indexstack.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/macrofileheader.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/macrofileheader.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/macrofileheader.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/macrofileheader.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/alumetis.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/alumetis.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/alusfc.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/alusfc.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/aluzoltan.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/aluzoltan.hh`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 #define HAVE_MPI 1
 #endif
 #undef HAVE_MPI_WAS_UNDEFED_HERE
 #endif // #ifdef HAVE_MPI_WAS_UNDEFED_HERE
 
 #ifdef HAVE_PARMETIS_WAS_UNDEFED_HERE
 // redefine our definition of HAVE_PARMETIS if it was undef'd before
-#define HAVE_PARMETIS 1
+#define HAVE_PARMETIS ENABLE_PARMETIS
 #undef HAVE_PARMETIS_WAS_UNDEFED_HERE
 #endif // #ifdef HAVE_PARMETIS_WAS_UNDEFED_HERE
 
 #endif // #if HAVE_ZOLTAN
 
 namespace ALUGridZoltan
 {
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_hexa_top_pll.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_hexa_top_pll.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_hexa_top_pll.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_hexa_top_pll.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_idn.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_idn.cc`

 * *Files 0% similar despite different names*

```diff
@@ -745,24 +745,26 @@
       // if element is in list then set rank
       if( el != end )
         (*el).second = myrank ;
     }
 
     {
       bool repeat = true ;
+      int count = 0;
       SendRecvElementRankInfo data( elements, db, mpAccess.nlinks() );
       while ( repeat )
       {
         mpAccess.exchange( data );
 
         mpAccess.barrier();
         // make sure every process is done
         repeat = mpAccess.gmax( data.repeat() ) ;
         //repeat = data.repeat() ;
         //alugrid_assert( mpAccess.gmax( data.repeat() ) == repeat );
+        ++ count ;
       }
     }
 
     typedef elrankmap_t :: iterator iterator ;
     for( iterator it = elements.begin(); it != end; ++it )
     {
       // insert element number and master rank info
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_impl.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_impl.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_impl.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_impl.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_ldb.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_ldb.cc`

 * *Files 0% similar despite different names*

```diff
@@ -658,16 +658,16 @@
     else  // this is the METIS section
     {
       // use the vertexSet directly
       ldb_vertex_map_t&  nodes = _vertexSet ;
 
       // 'ned' ist die Anzahl der Kanten im Graphen, 'nel' die Anzahl der Knoten.
       // Der Container 'nodes' enth"alt alle Knoten des gesamten Grobittergraphen
-      // durch Zusammenf"uhren der einzelnen Container aus den Teilgrobgittern.
-      // Der Container 'edges' enth"alt alle Kanten des gesamten Grobgittergraphen
+      // durch Zusammenführen der einzelnen Container aus den Teilgrobgittern.
+      // Der Container 'edges' enthält alle Kanten des gesamten Grobgittergraphen
       // doppelt, einmal mit jeder Orientierung (vorw"arts/r"uckw"arts). Diese Form
       // der Datenhaltung ist vorteilhaft, wenn die Eingangsdaten der Partitionierer
       // im CSR Format daraus erstellt werden m"ussen.
 
       const int ned = edges.size ();
       const int nel = nodes.size ();
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+iso-8859-1
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_ldb.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_ldb.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_mgb.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_mgb.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_mgb.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_mgb.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_sti.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_sti.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1673,15 +1673,15 @@
 
       // store values
       _ldbOver   = buff[ 0 ];
       _ldbUnder  = buff[ 1 ];
       _ldbMethod = (LoadBalancer::DataBase::method ) buff[ 2 ];
     }
 
-    if( mpa.myrank() == 0 && ALUGridExternalParameters::verbosityLevel() > 1)
+    if (ALUGridExternalParameters::verbosityLevel() > 1)
     {
       std::cerr << "ALUGrid-LB values: " << _ldbUnder << " < [balance] < " << _ldbOver << ", partitioning method '" << LoadBalancer::DataBase::methodToString( _ldbMethod ) << "'." << std::endl;
     }
 
     // we possibly need to initialize zoltan at some point - we will do it here...
     LoadBalancer::DataBase::initializeZoltan( _ldbMethod );
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_pll_sti.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_pll_sti.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_tetra_top_pll.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_tetra_top_pll.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/gitter_tetra_top_pll.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/gitter_tetra_top_pll.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/mpAccess.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/mpAccess.cc`

 * *Files 1% similar despite different names*

```diff
@@ -158,23 +158,25 @@
         {
           int n = _sendLinkage.size ();
           _sendLinkage [*i] = n;
         }
       }
     }
 
+    int cnt = 0;
     for( int i = 0; i < psize(); ++i )
     {
       if( std::find (in[ i ].begin(), in[ i ].end(), me) != in[ i ].end()  )
       {
         alugrid_assert (i != me);
         if (_sendLinkage.find (i) == linkageEnd )
         {
           int n = _sendLinkage.size ();
           _sendLinkage [i] = n;
+          cnt ++;
         }
       }
     }
 
     linkage_t().swap( _recvLinkage );
     // since linkage is symmetric, use sendLinkage for both
     _currentRecvLinkage = & _sendLinkage;
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/mpAccess.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/mpAccess.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/mpAccess_MPI.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/mpAccess_MPI.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/mpAccess_MPI_inline.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/mpAccess_MPI_inline.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/parallel/zcurve.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/parallel/zcurve.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/projectvertex.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/projectvertex.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gatherscatter.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gatherscatter.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/ghost_elements.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/ghost_elements.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/ghost_elements.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/ghost_elements.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/ghost_info.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/ghost_info.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/ghost_info.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/ghost_info.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_geo.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_geo.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_hexa_top.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_hexa_top.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_hexa_top.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_hexa_top.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_impl.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_impl.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_impl.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_impl.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_mgb.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_mgb.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_mgb.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_mgb.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_sti.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_sti.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_sti.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_sti.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_tetra_top.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_tetra_top.cc`

 * *Files 1% similar despite different names*

```diff
@@ -2522,63 +2522,59 @@
   }
 
   template< class A > const typename Periodic3Top < A >::myhedge_t * Periodic3Top < A >::subedge (int i, int j) const {
     return ((Periodic3Top < A > *)this)->subedge (i,j) ;
   }
 
   template< class A > typename Periodic3Top < A >:: myhface_t * Periodic3Top < A >::subface (int i, int j) {
-    myhface_t * face = myhface(i);
-    switch (face->getrule ())
-    {
+    switch (myhface (i)->getrule ()) {
     case myhface_t::myrule_t::e01 :
       alugrid_assert ( j < 2 );
       if ( twist(i) == 0 ||  twist(i) == 1  ||  twist(i) == -1 )
-        return face->subface(j) ;
+        return myhface(i)->subface(j) ;
       if ( twist(i) == 2 ||  twist(i) == -2 ||  twist(i) == -3 )
-        return face->subface(!j) ;
+        return myhface(i)->subface(!j) ;
       std::cerr << __FILE__ << " " << __LINE__ << "myhface(i)->subface()" << std::endl;
       return 0;
     case myhface_t::myrule_t::e12 :
       alugrid_assert ( j < 2 );
       if ( twist(i) == 0  ||  twist(i) == 2 ||  twist(i) == -3 )
-        return face->subface(j) ;
+        return myhface(i)->subface(j) ;
       if ( twist(i) == -1 ||  twist(i) == 1 ||  twist(i) == -2 )
-        return face->subface(!j) ;
+        return myhface(i)->subface(!j) ;
       std::cerr << __FILE__ << " " << __LINE__ << "myhface(i)->subface()" << std::endl;
       return 0;
     case myhface_t::myrule_t::e20 :
       alugrid_assert ( j < 2 );
       if ( twist(i) == 1 ||  twist(i) == 2 ||  twist(i) == -2 )
-        return face->subface(j) ;
+        return myhface(i)->subface(j) ;
       if ( twist(i) == 0 ||  twist(i) == -1 || twist(i) == -3 )
         return myhface(i)->subface(!j) ;
       std::cerr << __FILE__ << " " << __LINE__ << "myhface(i)->subface()" << std::endl;
       return 0;
     case myhface_t::myrule_t::iso4 :
       // in 2d case do the same as e12
-      if(face->is2d())
-      {
+      if(this->is2d()){
         alugrid_assert ( j < 2 );
         if ( twist(i) == 0  ||  twist(i) == 2 ||  twist(i) == -3 )
-          return face->subface(j) ;
+          return myhface(i)->subface(j) ;
         if ( twist(i) == -1 ||  twist(i) == 1 ||  twist(i) == -2 )
-          return face->subface(!j) ;
+          return myhface(i)->subface(!j) ;
         std::cerr << __FILE__ << " " << __LINE__ << "myhface(i)->subface()" << std::endl;
         return 0;
       }
-
       alugrid_assert ( j < 4 );
       if ( j == 3 )
       {
-        return face->subface (3) ;
+        return myhface(i)->subface (3) ;
       }
       else // ( j < 3 )
       {
         alugrid_assert( j < 3 );
-        return face->subface (twist(i) < 0 ? (7 - j + twist(i)) % 3 : (j + twist(i)) % 3) ;
+        return myhface (i)->subface (twist(i) < 0 ? (7 - j + twist(i)) % 3 : (j + twist(i)) % 3) ;
       }
     case myhface_t::myrule_t::nosplit :
       std::cerr << "**FEHLER (FATAL): subface () auf nicht verfeinerter Fl\"ache aufgerufen. In " << __FILE__ << " " << __LINE__ << std::endl ;
       std::abort () ;
       return 0 ;
     default:
       std::cerr << "**FEHLER (FATAL): Falsche Verfeinerungsregel [" << myhface(i)->getrule() << "] in " << __FILE__ << " " << __LINE__ << std::endl ;
@@ -2589,15 +2585,14 @@
 
   template< class A > const typename Periodic3Top < A >:: myhface_t * Periodic3Top < A >::subface (int i, int j) const {
     return ((Periodic3Top < A > *)this)->subface (i,j) ;
   }
 
   template< class A > void Periodic3Top < A >::split_iso4 ()
   {
-    alugrid_assert( ! myhface(0)->is2d() );
     const int l = 1 + this->level () ;
     innerperiodic3_t * p0 = new innerperiodic3_t (l, subface (0,0), twist (0), subface (1,0), twist (1), this , 0) ;
     innerperiodic3_t * p1 = new innerperiodic3_t (l, subface (0,1), twist (0), subface (1,2), twist (1), this , 1) ;
     innerperiodic3_t * p2 = new innerperiodic3_t (l, subface (0,2), twist (0), subface (1,1), twist (1), this , 2) ;
 
     // Mir ist nicht ganz klar, warum der Twist auf diese seltsame Art umzurechnen ist,
     // die Zeile (bzw. die Formel) habe ich aus Mario's Tetradeder Split Iso-8 "uber-
@@ -2606,57 +2601,29 @@
     innerperiodic3_t * p3 = new innerperiodic3_t (l, subface (0,3), (twist(0) >= 0 ? (twist(0)+1)%3 : (twist(0)-1)%3-1), subface (1,3), (twist(1)>=0 ? (twist(1)+1)%3 : (twist(1)-1)%3-1) , this , 3) ;
     alugrid_assert (p0 && p1 && p2 && p3) ;
     p0->append(p1) ;
     p1->append(p2) ;
     p2->append(p3) ;
     _dwn = p0 ;
     _rule = myrule_t::iso4 ;
-    p0->_up = p1->_up = p2->_up = p3->_up = this;
-    return ;
-  }
-
-  template< class A > void Periodic3Top < A >::split_bisection (myrule_t r)
-  {
-    alugrid_assert( myhface(0)->is2d() );
-    const int l = 1 + this->level () ;
-    innerperiodic3_t * p0 = new innerperiodic3_t (l, subface (0,1), twist (0), subface (1,0), twist (1), this , 0) ;
-    innerperiodic3_t * p1 = new innerperiodic3_t (l, subface (0,0), twist (0), subface (1,1), twist (1), this , 1) ;
-
-    alugrid_assert (p0 && p1) ;
-    p0->append(p1) ;
-    _dwn = p0 ;
-    // nevertheless, set iso4 rule
-    _rule = r ;
-    p0->_up = p1->_up = this;
+    p0->_up = p1->_up = p2->_up = p3->_up = this; //us
     return ;
   }
 
   template< class A > void Periodic3Top < A >::refineImmediate (myrule_t r) {
 
     // Die Methode wird nur vom restore () und vom refineBalance () auf-
     // gerufen und geht davon aus, dass das betroffene Element noch nicht
     // verfeinert ist -> ist ein Blatt der Hierarchie.
 
     alugrid_assert (this->leaf()) ;
     switch(r)
     {
       case myrule_t::iso4 :
-        if(myhface (0)->is2d()) // 2d refinement
-        {
-          //std::cerr << "**ERROR (FATAL) refinement of Periodic3Top in 2d not implemented yet! " ;
-          //std::cerr << "[" << r << "]. In " << __FILE__ << __LINE__ << std::endl ;
-          //std::abort () ;
-
-          typedef typename myhface_t::myrule_t face3rule_t;
-          myhface (0)->refineImmediate (face3rule_t (r).rotate (twist (0))) ;
-          myhface (1)->refineImmediate (face3rule_t (r).rotate (twist (1))) ;
-          split_bisection (r) ;
-          break ;
-        }
-        else // 3d case
+        if(!this->is2d())
         {
           // Das refineImmediate (..) auf allen Fl"achen wird vom periodic3::refine (..)
           // zwar nicht ben"otigt, da schliesslich alle Fl"achen sauber sind, wenn
           // "uberall hface3::refine (..) true geliefert hat, wohl aber z.B. von
           // restore () oder abgeleiteten Funktionen die eine direkte Verfeinerung
           // erzwingen m"ussen und d"urfen.
 
@@ -2671,29 +2638,14 @@
         std::cerr << "[" << r << "]. In " << __FILE__ << __LINE__ << std::endl ;
         std::abort () ;
         break ;
 
       case myrule_t::e01 :
       case myrule_t::e12 :
       case myrule_t::e20 :
-        if(myhface (0)->is2d()) // 2d refinement
-        {
-          //std::cerr << "**ERROR (FATAL) refinement of Periodic3Top in 2d not implemented yet! " ;
-          //std::cerr << "[" << r << "]. In " << __FILE__ << __LINE__ << std::endl ;
-          //std::abort () ;
-
-          typedef typename myhface_t::myrule_t face3rule_t;
-          myhface (0)->refineImmediate (face3rule_t (r).rotate (twist (0))) ;
-          myhface (1)->refineImmediate (face3rule_t (r).rotate (twist (1))) ;
-          split_bisection( r ) ;
-
-          assert( myhface(0)->level() == myhface(1)->level() );
-
-          break ;
-        }
 
         // Mit den drei anisotropen Regeln k"onnen wir leider noch nichts anfangen.
 
         std::abort () ;
       default :
         std::cerr << "**FEHLER (FATAL) beim unbedingten Verfeinern mit unbekannter Regel: " ;
         std::cerr << "[" << r << "]. In " << __FILE__ << __LINE__ << std::endl ;
@@ -2711,54 +2663,44 @@
     // Anforderung zur Balancierung aus einem anliegenden Element direkt verfeinert.
 
     return true ;
   }
 
   template< class A > bool Periodic3Top < A >::refineBalance (balrule_t r, int fce)
   {
-    switch (r)
+    if (r != balrule_t::iso4)
     {
-      case balrule_t::iso4:
-      case balrule_t::e01:
-      case balrule_t::e12:
-      case balrule_t::e20:
-        {
-          // Der nachfolgende Aufruf nutzt aus, dass die Regel der periodischen R"ander
-          // sich direkt auf die Balancierungsregel des entsprechenden Polygonverbinders
-          // projezieren l"asst (n"amlich 1:1). Deshalb unterscheidet der Aufruf nicht nach
-          // der angeforderten Regel in einer 'case' Anweisung.
-
-          // take opposite face
-          const int opp = 1 - fce ;
-          if (myhface (opp)->refine (typename myhface_t::myrule_t (r).rotate (twist (opp)), twist (opp)))
-          {
-            refineImmediate (r) ;
-            return true ;
-          }
-          else
-          {
-            return false ;
-          }
-        }
+      std::cerr << "**WARNING (IGNORED) in Periodic3Top < A >::refineBalance (..) , file "
+         << __FILE__ << " line " << __LINE__ << " periodic refinement is only implemented for isometric refinement!" << std::endl ;
 
-      default:
-        {
-          std::cerr << "**WARNING (IGNORED) in Periodic3Top < A >::refineBalance ( "<< r << " ) , file "
-             << __FILE__ << ":" << __LINE__ << " periodic refinement is only implemented for isometric refinement!" << std::endl ;
-
-          assert(false);
-          std::abort();
-
-          // Bisher kann die Balancierung nur die isotrope Achtelung handhaben,
-          // falls mehr gew"unscht wird, muss es hier eingebaut werden. Im Moment wird
-          // die Balancierung einfach verweigert, d.h. die Verfeinerung des anfordernden
-          // Elements f"allt flach.
+    // Bisher kann die Balancierung nur die isotrope Achtelung handhaben,
+    // falls mehr gew"unscht wird, muss es hier eingebaut werden. Im Moment wird
+    // die Balancierung einfach verweigert, d.h. die Verfeinerung des anfordernden
+    // Elements f"allt flach.
 
-          return false ;
-        }
+      return false ;
+    }
+    else
+    {
+      // Der nachfolgende Aufruf nutzt aus, dass die Regel der periodischen R"ander
+      // sich direkt auf die Balancierungsregel des entsprechenden Polygonverbinders
+      // projezieren l"asst (n"amlich 1:1). Deshalb unterscheidet der Aufruf nicht nach
+      // der angeforderten Regel in einer 'case' Anweisung.
+
+      // take opposite face
+      const int opp = 1 - fce ;
+      if (myhface (opp)->refine (typename myhface_t::myrule_t (r).rotate (twist (opp)), twist (opp)))
+      {
+        refineImmediate (r) ;
+        return true ;
+      }
+      else
+      {
+        return false ;
+      }
     }
   }
 
   template< class A > bool Periodic3Top < A >::coarse () {
 
     // Das Vergr"obern geschieht auch passiv, sobald ein anliegendes Element
     // vergr"obert wird durch den Aufruf von "bndNotifyCoarsen ()" s.u.
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/gitter_tetra_top.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/gitter_tetra_top.h`

 * *Files 0% similar despite different names*

```diff
@@ -695,17 +695,15 @@
       const signed char _nChild;
       myrule_t _rule;
 
     private :
       void split_e01 ();
       void split_e12 ();
       void split_e20 ();
-
       void split_iso4 ();
-      void split_bisection (myrule_t r);
     protected :
       myhedge_t * subedge (int,int);
       const myhedge_t * subedge (int,int) const;
       myhface_t * subface (int,int);
       const myhface_t * subface (int i, int j) const;
 
       // we need this for the boundary segment index
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/iterator_sti.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/iterator_sti.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/key.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/key.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/lock.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/lock.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/mapp_cube_3d.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/mapp_cube_3d.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/mapp_cube_3d.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/mapp_cube_3d.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/mapp_tetra_3d.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/mapp_tetra_3d.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/mapp_tetra_3d.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/mapp_tetra_3d.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/mapp_tetra_3d_ext.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/mapp_tetra_3d_ext.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/myalloc.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/myalloc.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/myalloc.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/myalloc.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/parallel.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/parallel.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/refcount.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/refcount.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/refinementrules.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/refinementrules.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/serialize.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/serialize.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/serial/walk.h` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/serial/walk.h`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/adapt.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/adapt.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/backuprestore.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/backuprestore.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/checkrefinement.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/checkrefinement.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube.hexa` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube.hexa`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube.tetra` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_12.tetra` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_12.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_48.tetra` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_48.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_512.hexa` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_512.hexa`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_hc_16.hexa` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_hc_16.hexa`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_hc_3072.tetra` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_hc_3072.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_hc_512.hexa` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_hc_512.hexa`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_hc_64.hexa` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_hc_64.hexa`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/cube_hs_512.hexa` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/cube_hs_512.hexa`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/hexa.test.2` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/hexa.test.2`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/hexa.test.converted` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/hexa.test.converted`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/macro.big` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/macro.big`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/unitcube.tet` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/unitcube.tet`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/unstructured.tetra` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/unstructured.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/grids/unstructured_218.tetra` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/grids/unstructured_218.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/sizes.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/sizes.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/impl/test/threadsafety.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/impl/test/threadsafety.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/CMakeLists.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
   test-backup-restore
   test-dgf
 )
 
 set(EXTRA_TESTS
   test-adaptivity
   test-fromtogridfactory
-  test-periodic
   test-iterators
+  test-periodic
   test-twists
   test-hierarchic
   test-ball-projection
   test-gmsh
 )
 
 foreach(TEST ${TESTS})
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/checkintersectionit.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/checkintersectionit.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/checktwists.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/checktwists.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/ball.dgf` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/ball.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/cubedsphere2d.dgf` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/cubedsphere2d.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/simplex-testgrid-2-2.dgf` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/simplex-testgrid-2-2.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/simplex-testgrid-2-3-noproj.dgf` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/simplex-testgrid-2-3-noproj.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/simplex-testgrid-2-3.dgf` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/simplex-testgrid-2-3.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/dgf/simplex-testgrid-3-3.dgf` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/dgf/simplex-testgrid-3-3.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/gmsh/circle2ndorder.msh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/gmsh/circle2ndorder.msh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/gmsh/curved2d.msh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/gmsh/curved2d.msh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/gmsh/telescope.msh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/gmsh/telescope.msh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/insertgrid.hh` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/insertgrid.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/pyramid.tetra.converted` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/pyramid.tetra.converted`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/test-adaptivity.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-adaptivity.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/test-alugrid.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-alugrid.cc`

 * *Files 2% similar despite different names*

```diff
@@ -49,28 +49,39 @@
 
 template< int dim, int dimworld >
 struct EnableLevelIntersectionIteratorCheck< Dune::ALUGrid< dim, dimworld, Dune::simplex, Dune::conforming > >
 {
   static const bool v = false;
 };
 
-template <class Grid>
+template <bool leafconform, class Grid>
 void checkCapabilities(const Grid& grid)
 {
    static_assert ( Dune::Capabilities::hasSingleGeometryType< Grid > :: v == true,
                   "hasSingleGeometryType is not set correctly");
-   static_assert ( Dune::Capabilities::isLevelwiseConforming< Grid > :: v == false,
+   static_assert ( Dune::Capabilities::isLevelwiseConforming< Grid > :: v == ! leafconform,
                   "isLevelwiseConforming is not set correctly");
-   static_assert ( Dune::Capabilities::isLeafwiseConforming< Grid > :: v == (Grid::refinementType == Dune::conforming),
+   static_assert ( Dune::Capabilities::isLeafwiseConforming< Grid > :: v == leafconform,
                   "isLevelwiseConforming is not set correctly");
    static const bool hasEntity = Dune::Capabilities::hasEntity<Grid, 1> :: v == true;
    static_assert ( hasEntity, "hasEntity is not set correctly");
    static_assert ( Dune::Capabilities::hasBackupRestoreFacilities< Grid > :: v == true,
                    "hasBackupRestoreFacilities is not set correctly");
 
+#if !DUNE_VERSION_NEWER(DUNE_GRID,2,5)
+   static const bool reallyParallel =
+#if ALU3DGRID_PARALLEL
+    true ;
+#else
+    false ;
+#endif
+   static_assert ( Dune::Capabilities::isParallel< Grid > :: v == reallyParallel,
+                   "isParallel is not set correctly");
+#endif //#if !DUNE_VERSION_NEWER(DUNE_GRID,2,5)
+
    static const bool reallyCanCommunicate =
 #if ALU3DGRID_PARALLEL
     true ;
 #else
     false ;
 #endif
    static const bool canCommunicate = Dune::Capabilities::canCommunicate< Grid, 1 > :: v
@@ -492,15 +503,15 @@
     DUNE_THROW( Dune::InvalidStateException, "No periodic boundaries found!" );
   }
 }
 
 template <class GridType>
 void checkALUSerial(GridType & grid, int mxl = 2)
 {
-  const bool skipLevelIntersections = grid.conformingRefinement();//! EnableLevelIntersectionIteratorCheck< GridType > :: v ;
+  const bool skipLevelIntersections = ! EnableLevelIntersectionIteratorCheck< GridType > :: v ;
   {
     GridType* gr = new GridType();
     assert ( gr );
     delete gr;
   }
 
   writeFile( grid.leafGridView() );
@@ -509,15 +520,14 @@
   std::ostream& out = (grid.comm().rank() == 0) ? std::cout : null;
 
   out << "  CHECKING: grid size = " << grid.size( 0 ) << std::endl;
 
   // be careful, each global refine create 8 x maxlevel elements
   out << "  CHECKING: Macro" << std::endl;
   checkGrid(grid);
-
   out << "  CHECKING: Macro-intersections" << std::endl;
   checkIntersectionIterator(grid, skipLevelIntersections);
 
   if( GridType :: dimension == 3 )
   {
     // this only works for ALUGrid 3d
     out << "  CHECKING: 3d Twists " << std::endl;
@@ -594,29 +604,22 @@
 
   // check iterators
   checkALUIterators( grid );
 
   // -1 stands for leaf check
   checkCommunication(grid, -1, std::cout);
 
-  if( ! grid.conformingRefinement() )
+  if( Dune :: Capabilities :: isLevelwiseConforming< GridType > :: v )
   {
     for(int l=0; l<= mxl; ++l)
       checkCommunication(grid, l , Dune::dvverb);
   }
 #endif
 }
 
-struct EnableConformingRefinement
-{
-  EnableConformingRefinement() { setenv("ALUGRID_CONFORMING_REFINEMENT", "1", 1 ); }
-  ~EnableConformingRefinement() { unsetenv("ALUGRID_CONFORMING_REFINEMENT"); }
-  void operator = (int) {}
-};
-
 
 int main (int argc , char **argv) {
 
   // this method calls MPI_Init, if MPI is enabled
   Dune::MPIHelper &mpihelper = Dune::MPIHelper::instance( argc, argv );
   int myrank = mpihelper.rank();
   int mysize = mpihelper.size();
@@ -688,88 +691,78 @@
 
 #ifndef NO_3D
       if (myrank == 0 && (testALU3dCube || testALU3dSimplex) )
         std::cout << "Check empty grids" << std::endl;
 
       if( testALU3dCube )
       {
-        Dune::ALUGrid< 3, 3, Dune::cube > grid;
+        Dune::ALUGrid< 3, 3, Dune::cube, Dune::nonconforming > grid;
         checkALUSerial( grid );
       }
 
       if( testALU3dSimplex )
       {
-        Dune::ALUGrid< 3, 3, Dune::simplex > grid;
+        Dune::ALUGrid< 3, 3, Dune::simplex, Dune::nonconforming > grid;
         checkALUSerial( grid );
       }
 
       if( testALU3dConform )
       {
-        EnableConformingRefinement conforming;
-        Dune::ALUGrid< 3, 3, Dune::simplex > grid;
+        Dune::ALUGrid< 3, 3, Dune::simplex, Dune::conforming > grid;
         checkALUSerial( grid );
-        conforming = 0;
       }
 #endif // #ifndef NO_3D
 
 
       // check grid factory (test only available for dune-grid 3.0 or later)
 
       if( myrank == 0 )
         std::cout << "Checking grid factory..." << std::endl;
 
 #if HAVE_DUNE_GRID_TESTGRIDS
 #ifndef NO_2D
       if( testALU2dCube )
-        Dune::checkGridFactory< Dune::ALUGrid< 2, 2, Dune::cube > >( Dune::TestGrids::unitSquare );
+        Dune::checkGridFactory< Dune::ALUGrid< 2, 2, Dune::cube, Dune::nonconforming > >( Dune::TestGrids::unitSquare );
 
       if( testALU2dSimplex )
-        Dune::checkGridFactory< Dune::ALUGrid< 2, 2, Dune::simplex > >( Dune::TestGrids::kuhn2d );
+        Dune::checkGridFactory< Dune::ALUGrid< 2, 2, Dune::simplex, Dune::nonconforming > >( Dune::TestGrids::kuhn2d );
 
       if( testALU2dConform )
-      {
-        EnableConformingRefinement conforming;
-        Dune::checkGridFactory< Dune::ALUGrid< 2, 2, Dune::simplex > >( Dune::TestGrids::kuhn2d );
-        conforming = 0;
-      }
+        Dune::checkGridFactory< Dune::ALUGrid< 2, 2, Dune::simplex, Dune::conforming > >( Dune::TestGrids::kuhn2d );
 #endif // #ifndef NO_2D
 
 #ifndef NO_3D
       if( testALU3dCube )
-        Dune::checkGridFactory< Dune::ALUGrid< 3, 3, Dune::cube > >( Dune::TestGrids::unitCube );
+        Dune::checkGridFactory< Dune::ALUGrid< 3, 3, Dune::cube, Dune::nonconforming > >( Dune::TestGrids::unitCube );
 
       if( testALU3dSimplex )
-        Dune::checkGridFactory< Dune::ALUGrid< 3, 3, Dune::simplex > >( Dune::TestGrids::kuhn3d );
+        Dune::checkGridFactory< Dune::ALUGrid< 3, 3, Dune::simplex, Dune::nonconforming > >( Dune::TestGrids::kuhn3d );
 
       if( testALU3dConform )
-      {
-        EnableConformingRefinement conforming;
-        Dune::checkGridFactory< Dune::ALUGrid< 3, 3, Dune::simplex > >( Dune::TestGrids::kuhn3d );
-        conforming = 0;
-      }
+        Dune::checkGridFactory< Dune::ALUGrid< 3, 3, Dune::simplex, Dune::conforming > >( Dune::TestGrids::kuhn3d );
 #endif // #ifndef NO_3D
 #endif // HAVE_DUNE_GRID_TESTGRIDS
 
 #ifndef NO_2D
       // check non-conform ALUGrid for 2d
       if( testALU2dCube )
       {
-        typedef Dune::ALUGrid< 2, 2, Dune::cube > GridType;
+        typedef Dune::ALUGrid< 2, 2, Dune::cube, Dune::nonconforming > GridType;
         std::string filename;
         if( newfilename )
           filename = newfilename;
         else
           filename = "./dgf/cube-testgrid-2-2.dgf";
         std::cout << "READING from " << filename << std::endl;
         Dune::GridPtr< GridType > gridPtr( filename );
         gridPtr.loadBalance();
 
         GridType & grid = *gridPtr;
 
-        checkCapabilities( grid );
+        checkCapabilities< false >( grid );
 
         {
           std::cout << "Check serial grid" << std::endl;
           checkALUSerial(grid,
                          (mysize == 1) ? 1 : 0 );
         }
 
@@ -782,39 +775,39 @@
           checkALUParallel(grid,0,2);
         }
 
         //CircleBoundaryProjection<2> bndPrj;
         //GridType grid("alu2d.triangle", &bndPrj );
         //checkALUSerial(grid,2);
 
-        typedef Dune::ALUGrid< 2, 3, Dune::cube > SurfaceGridType;
+        typedef Dune::ALUGrid< 2, 3, Dune::cube, Dune::nonconforming > SurfaceGridType;
         std::string surfaceFilename( "./dgf/cube-testgrid-2-3.dgf" );
         std::cout << "READING from '" << surfaceFilename << "'..." << std::endl;
         Dune::GridPtr< SurfaceGridType > surfaceGridPtr( surfaceFilename );
         SurfaceGridType & surfaceGrid = *surfaceGridPtr ;
         surfaceGrid.loadBalance();
-        checkCapabilities( surfaceGrid );
+        checkCapabilities< false >( surfaceGrid );
         checkALUSerial( surfaceGrid, 1 );
       }
 
       // check non-conform ALUGrid for 2d
       if( testALU2dSimplex )
       {
-        typedef Dune::ALUGrid< 2, 2, Dune::simplex > GridType;
+        typedef Dune::ALUGrid< 2, 2, Dune::simplex, Dune::nonconforming > GridType;
         std::string filename;
         if( newfilename )
           filename = newfilename;
         else
           filename = "./dgf/simplex-testgrid-2-2.dgf";
         std::cout << "READING from " << filename << std::endl;
         Dune::GridPtr< GridType > gridPtr( filename );
         gridPtr.loadBalance();
         GridType & grid = *gridPtr;
 
-        checkCapabilities( grid );
+        checkCapabilities< false >( grid );
 
         {
           std::cout << "Check serial grid" << std::endl;
           checkALUSerial(grid,
                          (mysize == 1) ? 1 : 0 );
         }
 
@@ -827,43 +820,40 @@
           checkALUParallel(grid,0,2);
         }
 
         //CircleBoundaryProjection<2> bndPrj;
         //GridType grid("alu2d.triangle", &bndPrj );
         //checkALUSerial(grid,2);
 
-        typedef Dune::ALUGrid< 2, 3, Dune::simplex > SurfaceGridType;
+        typedef Dune::ALUGrid< 2, 3, Dune::simplex, Dune::nonconforming > SurfaceGridType;
         std::string surfaceFilename( "./dgf/simplex-testgrid-2-3-noproj.dgf" );
         std::cout << "READING from '" << surfaceFilename << "'..." << std::endl;
 
-        std::cerr << "WARNING: surface projection disabled for ALUGrid< 2, 3, Dune::simplex >" << std::endl;
+        std::cerr << "WARNING: surface projection disabled for ALUGrid< 2, 3, Dune::simplex, Dune::nonconforming >" << std::endl;
         Dune::GridPtr< SurfaceGridType > surfaceGridPtr( surfaceFilename );
         SurfaceGridType & surfaceGrid = *surfaceGridPtr ;
         surfaceGrid.loadBalance();
-        checkCapabilities( surfaceGrid );
+        checkCapabilities< false >( surfaceGrid );
         checkALUSerial( surfaceGrid, 1 );
       }
 
       // check conform ALUGrid for 2d
       if( testALU2dConform )
       {
-        EnableConformingRefinement conforming;
-
-        //typedef Dune::ALUGrid< 2, 2, Dune::simplex, Dune::conforming > GridType;
-        typedef Dune::ALUGrid< 2, 2, Dune::simplex > GridType;
+        typedef Dune::ALUGrid< 2, 2, Dune::simplex, Dune::conforming > GridType;
         std::string filename;
         if( newfilename )
           filename = newfilename;
         else
           filename = "./dgf/simplex-testgrid-2-2.dgf";
         Dune::GridPtr<GridType> gridPtr( filename );
         gridPtr.loadBalance();
         GridType & grid = *gridPtr;
 
-        checkCapabilities( grid );
+        checkCapabilities< true >( grid );
 
         {
           std::cout << "Check serial grid" << std::endl;
           checkALUSerial(grid,
                          (mysize == 1) ? 1 : 0 );
         }
 
@@ -876,44 +866,42 @@
           checkALUParallel(grid,0,2);
         }
 
         //CircleBoundaryProjection<2> bndPrj;
         //GridType grid("alu2d.triangle", &bndPrj );
         //checkALUSerial(grid,2);
 
-        typedef Dune::ALUGrid< 2, 3, Dune::simplex > SurfaceGridType;
+        typedef Dune::ALUGrid< 2, 3, Dune::simplex, Dune::conforming > SurfaceGridType;
         //typedef ALUConformGrid< 2, 3 > SurfaceGridType;
         std::string surfaceFilename( "./dgf/simplex-testgrid-2-3.dgf" );
         std::cout << "READING from '" << surfaceFilename << "'..." << std::endl;
         Dune::GridPtr< SurfaceGridType > surfaceGridPtr( surfaceFilename );
         surfaceGridPtr.loadBalance();
         SurfaceGridType & surfaceGrid = *surfaceGridPtr ;
-        checkCapabilities( surfaceGrid );
+        checkCapabilities< true >( surfaceGrid );
         checkALUSerial( surfaceGrid, 1 );
-
-        conforming = 0;
       }
 #endif // #ifndef NO_2D
 
 #ifndef NO_3D
       if( testALU3dCube )
       {
         std::string filename;
         if( newfilename )
           filename = newfilename;
         else
           filename = "./dgf/simplex-testgrid-3-3.dgf";
 
-        typedef Dune::ALUGrid< 3, 3, Dune::cube > GridType;
+        typedef Dune::ALUGrid< 3, 3, Dune::cube, Dune::nonconforming > GridType;
         {
           Dune::GridPtr< GridType > gridPtr( filename );
           gridPtr.loadBalance();
           GridType & grid = *gridPtr;
 
-          checkCapabilities( grid );
+          checkCapabilities< false >( grid );
 
           {
             std::cout << "Check serial grid" << std::endl;
             checkALUSerial(grid,
                            (mysize == 1) ? 1 : 0 );
           }
 
@@ -932,15 +920,15 @@
       {
         // check periodic capabilities
         std::string filename;
         if( newfilename )
           filename = newfilename;
         else
           filename = "./dgf/periodic3.dgf";
-        typedef Dune::ALUGrid< 3, 3, Dune::cube > GridType;
+        typedef Dune::ALUGrid< 3, 3, Dune::cube, Dune::nonconforming > GridType;
         // periodic boundaries require certain load balancing methods
         GridType::setLoadBalanceMethod( 10 );
         Dune::GridPtr< GridType > gridPtr( filename );
         gridPtr.loadBalance();
         GridType & grid = *gridPtr;
 
         {
@@ -955,19 +943,19 @@
       {
         std::string filename;
         if( newfilename )
           filename = newfilename;
         else
           filename = "./dgf/simplex-testgrid-3-3.dgf";
 
-        typedef Dune::ALUGrid< 3, 3, Dune::simplex > GridType;
+        typedef Dune::ALUGrid< 3, 3, Dune::simplex, Dune::nonconforming > GridType;
         Dune::GridPtr< GridType > gridPtr( filename );
         gridPtr.loadBalance();
         GridType & grid = *gridPtr;
-        checkCapabilities( grid );
+        checkCapabilities< false >( grid );
 
         {
           std::cout << "Check serial grid" << std::endl;
           checkALUSerial(grid,
                          (mysize == 1) ? 1 : 0);
         }
 
@@ -979,27 +967,25 @@
           if (myrank == 0) std::cout << "Check non-conform grid" << std::endl;
           checkALUParallel(grid,0,2);  //1,3
         }
       }
 
       if( testALU3dConform )
       {
-        EnableConformingRefinement conforming;
-
         std::string filename;
         if( newfilename )
           filename = newfilename;
         else
           filename = "./dgf/simplex-testgrid-3-3.dgf";
 
-        typedef Dune::ALUGrid< 3, 3, Dune::simplex > GridType;
+        typedef Dune::ALUGrid< 3, 3, Dune::simplex, Dune::conforming > GridType;
         Dune::GridPtr< GridType > gridPtr( filename );
         gridPtr.loadBalance();
         GridType & grid = *gridPtr;
-        checkCapabilities( grid );
+        checkCapabilities< true >( grid );
 
         {
           std::cout << "Check serial grid" << std::endl;
           checkALUSerial(grid,
                          (mysize == 1) ? 1 : 0);
         }
 
@@ -1007,16 +993,14 @@
         if(mysize > 1)
         {
           if (myrank == 0) std::cout << "Check conform grid" << std::endl;
           checkALUParallel(grid,0,0);  //1,3
           if (myrank == 0) std::cout << "Check non-conform grid" << std::endl;
           checkALUParallel(grid,0,4);  //1,3
         }
-
-        conforming = 0;
       }
 #endif
     };
 
   }
   catch( Dune::Exception &e )
   {
```

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/test-backup-restore.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-backup-restore.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/test-ball-projection.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-ball-projection.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/test-dgf.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-dgf.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/test-entities.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-entities.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/test-fromtogridfactory.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-fromtogridfactory.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/test-geometries.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-geometries.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/test-gmsh.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-gmsh.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/test-hierarchic.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-hierarchic.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/test-iterators.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-iterators.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/test-structuredgridfactory.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-structuredgridfactory.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/test-threadsafety.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-threadsafety.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/alugrid/test/test-twists.cc` & `dune-alugrid-2.9.dev20220529/dune/alugrid/test/test-twists.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/python/test/interpolate.py` & `dune-alugrid-2.9.dev20220529/dune/python/test/interpolate.py`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/python/test/test_gf1.py` & `dune-alugrid-2.9.dev20220529/dune/python/test/test_gf1.py`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/python/test/test_gf2.py` & `dune-alugrid-2.9.dev20220529/dune/python/test/test_gf2.py`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/dune/python/test/test_indexset.py` & `dune-alugrid-2.9.dev20220529/dune/python/test/test_indexset.py`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/examples/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   add_executable(main_${variant} main.cc )
   dune_target_enable_all_packages(main_${variant})
   set_property(TARGET main_${variant} APPEND PROPERTY LINK_LIBRARIES dunealugrid)
   target_compile_definitions(main_${variant} PRIVATE ${variant_upper})
   if("${variant}" STREQUAL "ball")
     target_compile_definitions(main_${variant} PRIVATE "ALUGRID_COUNT_GLOBALCOMM")
   endif()
-  target_compile_definitions(main_${variant} PUBLIC "ALUGRID_CONFORM" "GRIDDIM=2" "WORLDDIM=2")
+  target_compile_definitions(main_${variant} PUBLIC "ALUGRID_CUBE" "GRIDDIM=2" "WORLDDIM=2")
 
   foreach(type cube simplex conform)
     string(TOUPPER ${type} type_upper)
     foreach(dim RANGE 2 3)
       add_executable(main_${variant}_${type}_${dim}d EXCLUDE_FROM_ALL main.cc)
       target_compile_definitions(main_${variant}_${type}_${dim}d PRIVATE "${variant_upper}" "ALUGRID_${type_upper}" "GRIDDIM=${dim}" "WORLDDIM=${dim}")
       dune_target_enable_all_packages(main_${variant}_${type}_${dim}d)
```

### Comparing `dune-alugrid-2.9.0rc1/examples/adaptation.hh` & `dune-alugrid-2.9.dev20220529/examples/adaptation.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/backuprestore/main.cc` & `dune-alugrid-2.9.dev20220529/examples/backuprestore/main.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/backuprestore/paralleldgf.hh` & `dune-alugrid-2.9.dev20220529/examples/backuprestore/paralleldgf.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/backuprestore/sionlib.hh` & `dune-alugrid-2.9.dev20220529/examples/backuprestore/sionlib.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/callback/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/examples/callback/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/callback/adaptation.hh` & `dune-alugrid-2.9.dev20220529/examples/callback/adaptation.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/callback/check-adaptation.sh` & `dune-alugrid-2.9.dev20220529/examples/callback/check-adaptation.sh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/callback/datamap.hh` & `dune-alugrid-2.9.dev20220529/examples/callback/datamap.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/callback/diagnostics.hh` & `dune-alugrid-2.9.dev20220529/examples/callback/diagnostics.hh`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #endif
 
 namespace Dune {
 
   template <class GridType>
   class Diagnostics
   {
-    typedef typename GridType :: Traits :: Communication CommunicatorType;
+    typedef typename GridType :: Traits :: CollectiveCommunication CommunicatorType;
     const CommunicatorType& comm_;
     const std::string runFileName_;
     const int writeDiagnostics_; // 0 don't, 1 only speedup file, 2 write all runfiles
                                  // 3 only write 0, others at end, 4 all files at end
     std::ostream* diagnosticsFile_;
 
     std::vector< double > times_ ;
```

### Comparing `dune-alugrid-2.9.0rc1/examples/callback/fvscheme.hh` & `dune-alugrid-2.9.dev20220529/examples/callback/fvscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/callback/main.cc` & `dune-alugrid-2.9.dev20220529/examples/callback/main.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/callback/paralleldgf.hh` & `dune-alugrid-2.9.dev20220529/examples/callback/paralleldgf.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/callback/piecewisefunction.hh` & `dune-alugrid-2.9.dev20220529/examples/callback/piecewisefunction.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/callback/problem-ball.hh` & `dune-alugrid-2.9.dev20220529/examples/callback/problem-ball.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/callback/problem-euler.hh` & `dune-alugrid-2.9.dev20220529/examples/callback/problem-euler.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/callback/problem-transport.hh` & `dune-alugrid-2.9.dev20220529/examples/callback/problem-transport.hh`

 * *Files 25% similar despite different names*

```diff
@@ -15,64 +15,37 @@
  */
 template< int dimD >
 class TransportProblemData1
 : public ProblemData< dimD, 1 >
 {
   typedef ProblemData< dimD, 1 > Base;
 
-public:
-  const static int dimDomain = Base::dimDomain;
-  const static int dimRange = Base::dimRange;
-
-  typedef typename Base::DomainType DomainType;
-  typedef typename Base::RangeType RangeType;
-
-protected:
   std::string gridFile_;
-  DomainType velocity_;
-  int problem_;
 public:
-  TransportProblemData1( const int problem ) : problem_( problem )
+  TransportProblemData1( const int problem )
   {
     if( problem == 3 )
     {
       gridFile_ = "/dgf/periodic" + std::to_string(dimDomain) + ".dgf";
     }
     else
     {
       gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
     }
-
-    if( problem < 3 )
-    {
-      // set transport velocity
-      velocity_ = DomainType( 1.25 );
-    }
-    else
-    {
-      velocity_ = 0.0;
-      velocity_[ 0 ] = 1.25;
-    }
   }
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = velocity_;
-  }
+  const static int dimDomain = Base::dimDomain;
+  const static int dimRange = Base::dimRange;
+
+  typedef typename Base::DomainType DomainType;
+  typedef typename Base::RangeType RangeType;
 
   //! \copydoc ProblemData::initial
   RangeType initial ( const DomainType &x ) const
   {
-    if( problem_ == 3 )
-    {
-      DomainType xc( x );
-      xc -= 0.5;
-      return (xc*xc) < 0.0625 ? 1.0 : 0;
-    }
-
     return sin( 2 * M_PI * (x*x) );
   }
 
   //! \copydoc ProblemData::endTime
   double endTime () const
   {
     return 0.8;
@@ -117,168 +90,46 @@
  */
 template< int dimD >
 class TransportProblemData2
 : public ProblemData< dimD, 1 >
 {
   typedef ProblemData< dimD, 1  > Base;
 
-public:
-  const static int dimDomain = Base::dimDomain;
-  const static int dimRange = Base::dimRange;
-
-  typedef typename Base::DomainType DomainType;
-  typedef typename Base::RangeType RangeType;
-
-protected:
   std::string gridFile_;
-  DomainType velocity_;
 public:
   TransportProblemData2( const int problem )
   {
     if( problem == 4 )
     {
       gridFile_ = "/dgf/periodic" + std::to_string(dimDomain) + ".dgf";
     }
     else
     {
       gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
     }
-
-    if( problem < 3 )
-    {
-      // set transport velocity
-      velocity_ = DomainType( 1.25 );
-    }
-    else
-    {
-      velocity_ = 0.0;
-      velocity_[ 0 ] = 1.25;
-    }
-  }
-
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = velocity_;
-  }
-
-  //! \copydoc ProblemData::initial
-  RangeType initial ( const DomainType &x ) const
-  {
-    DomainType r(0.5);
-    return ((x-r).two_norm() < 0.25 ? RangeType( 1 ) : RangeType( 0 ) );
-    //return ((x-r).two_norm() < 0.5 ? RangeType( 1 ) : RangeType( 0 ) );
-  }
-
-  //! \copydoc ProblemData::endTime
-  double endTime () const
-  {
-    return 0.8;
-  }
-
-  //! \copydoc ProblemData::gridFile
-  std::string gridFile ( const std::string &path, const int mpiSize ) const
-  {
-    return path + gridFile_;
-  }
-
-  RangeType boundaryValue ( const DomainType &x, double time ) const
-  {
-    return initial( x );
-  }
-
-  int bndType( const DomainType &normal, const DomainType &x, const double time) const
-  {
-    return 1;
-  }
-
-  double saveInterval () const
-  {
-    return 0.05;
-  }
-  //! \copydoc ProblemData::refineTol
-  double refineTol () const
-  {
-    return 0.1;
-  }
-  double adaptationIndicator ( const DomainType& x, double time,
-                               const RangeType &uLeft, const RangeType &uRight ) const
-  {
-    return std::abs( uLeft[ 0 ] - uRight[ 0 ] );
-  }
-};
-
-/**
- * \brief Solid body rotation
- */
-template< int dimD >
-class SolidBodyRotation
-: public ProblemData< dimD, 1 >
-{
-  typedef ProblemData< dimD, 1  > Base;
-
-  std::string gridFile_;
-public:
-  SolidBodyRotation( const int problem )
-  {
-    gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
   }
 
   const static int dimDomain = Base::dimDomain;
   const static int dimRange = Base::dimRange;
 
   typedef typename Base::DomainType DomainType;
   typedef typename Base::RangeType RangeType;
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    //v = velocity_;
-    double angular_velocity = 1.0;
-    DomainType rotation_centre = DomainType(0.5);
-    DomainType radius = x - rotation_centre;
-    v[0] = -angular_velocity*radius[1];
-    v[1] = angular_velocity*radius[0];
-  }
-
   //! \copydoc ProblemData::initial
   RangeType initial ( const DomainType &x ) const
   {
-    RangeType res(0) ;
-
-    DomainType c1( 0.5 ), c2( 0.5 ), c3( 0.5 ), c4( 0.5 );
-    c1[ 0 ] = 0.5;  c1[ 1 ] = 0.75;
-    c2[ 0 ] = 0.5;  c2[ 1 ] = 0.25;
-    c3[ 0 ] = 0.25; c3[ 1 ] = 0.5;
-    c4[ 0 ] = 0.35; c4[ 1 ] = 0.65;
-    const double r = 0.15;
-
-    // slotted cylinder
-    if( (x - c1).two_norm() < r )
-    {
-      if( (std::abs( x[ 0 ] - c1[ 0 ] ) >= 0.025) || (x[ 1 ] >= c1[ 1 ] + 0.1) )
-        return RangeType( 1.0 );
-      else
-        return RangeType( 0.0 );
-    }
-
-    // cone
-    if( (x - c2).two_norm() < r )
-      return RangeType( (r - (x - c2).two_norm()) / r );
-
-    // hump
-    if( (x - c3).two_norm() < r )
-      return RangeType((1.0 + std::cos( M_PI * (x - c3).two_norm() / r )) / 4.0 );
-
-    // default
-    return RangeType( 0.0 );
+    DomainType r(0.5);
+    return ((x-r).two_norm() < 0.25 ? RangeType( 1 ) : RangeType( 0 ) );
+    //return ((x-r).two_norm() < 0.5 ? RangeType( 1 ) : RangeType( 0 ) );
   }
 
   //! \copydoc ProblemData::endTime
   double endTime () const
   {
-    return 1.5708;
+    return 0.8;
   }
 
   //! \copydoc ProblemData::gridFile
   std::string gridFile ( const std::string &path, const int mpiSize ) const
   {
     return path + gridFile_;
   }
@@ -346,34 +197,48 @@
     case 3:
       problem_.reset( new TransportProblemData1< dimDomain >( problem ) );
       break;
     case 2:
     case 4:
       problem_.reset( new TransportProblemData2< dimDomain >( problem ) );
       break;
-    case 5:
-      problem_.reset( new SolidBodyRotation< dimDomain >( problem ) );
-      break;
     default:
       std::cerr << "Problem " << problem << " does not exists." << std::endl;
       std::abort();
     }
+
+    if( problem < 3 )
+    {
+      // set transport velocity
+      velocity_ = DomainType( 1.25 );
+    }
+    else
+    {
+      velocity_ = 0.0;
+      velocity_[ 0 ] = 1.25;
+    }
   }
 
   /** \brief obtain problem */
   const Problem &problem () const
   {
     return *problem_;
   }
 
   double fixedDt () const
   {
     return -1;
   }
 
+  /** \brief obtain the (constant) velocity for the transport problem */
+  const DomainType &velocity () const
+  {
+    return velocity_;
+  }
+
   /** \brief evaluate the numerical flux on an intersection
    *
    *  \param[in]   normal   scaled normal of the intersection
    *  \param[in]   time     current time
    *  \param[in]   xGlobal  evaluation point in global coordinates
    *  \param[in]   uLeft    value of the solution in the inside entity
    *  \param[in]   uRight   value of the solution in the outside entity
@@ -383,17 +248,15 @@
    */
   double numericalFlux ( const DomainType &normal,
                          const double time,
                          const DomainType &xGlobal,
                          const RangeType &uLeft, const RangeType &uRight,
                          RangeType &flux ) const
   {
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    const double upwind = normal * velocity;
+    const double upwind = normal * velocity();
     flux = upwind * (upwind > 0 ? uLeft : uRight);
     return std::abs( upwind );
   }
 
   /** \brief evaluate the numerical flux on a boundary
    *
    *  \param[in]   normal   scaled normal of the boundary
@@ -408,17 +271,15 @@
                         const double time,
                         const DomainType &xGlobal,
                         const RangeType& uLeft,
                         RangeType &flux ) const
   {
     // exact solution is u0(x-ta)
     DomainType x0( xGlobal );
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    x0.axpy( -time, velocity );
+    x0.axpy( -time, velocity_ );
     RangeType uRight = problem().boundaryValue( x0, time );
     return numericalFlux( normal, time, xGlobal, uLeft, uRight, flux );
   }
 
   /** \brief compute adaptation indicator at intersection
    *
    *  \param[in]   normal   scaled normal of the intersection
@@ -448,20 +309,19 @@
    */
   double boundaryIndicator ( const DomainType &normal,
                              const double time,
                              const DomainType &xGlobal,
                              const RangeType& uLeft) const
   {
     DomainType x0( xGlobal );
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    x0.axpy( -time, velocity );
+    x0.axpy( -time, velocity_ );
     return indicator( normal,time,xGlobal, uLeft, problem().boundaryValue(x0,time) );
   }
 
 protected:
-  TransportModel ( ) : problem_() {}
+  TransportModel ( ) : problem_(), velocity_(1) {}
 private:
   std::unique_ptr< Problem > problem_;
+  DomainType velocity_;
 }; // end class TransportModel
 
 #endif // PROBLEM_TRANSPORT_HH
```

### Comparing `dune-alugrid-2.9.0rc1/examples/callback/problem.hh` & `dune-alugrid-2.9.dev20220529/examples/callback/problem.hh`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,11 @@
 
   /**\brief return number of timestep to pass until load balancing is done again  */
   virtual int balanceStep() const { return 1; }
 
   /**\brief return maximal number of timesteps to run (for scaling experiment) */
   virtual unsigned int maxTimeSteps() const { return std::numeric_limits<unsigned int>::max(); }
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = 0;
-  }
-
 }; // end class ProblemData
 // Code moved to problem-transport.hh
 
 #endif // PROBLEM_HH
```

### Comparing `dune-alugrid-2.9.0rc1/examples/communication/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/examples/communication/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/communication/adaptation.hh` & `dune-alugrid-2.9.dev20220529/examples/communication/adaptation.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/communication/check-communication.sh` & `dune-alugrid-2.9.dev20220529/examples/communication/check-communication.sh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/communication/datamap.hh` & `dune-alugrid-2.9.dev20220529/examples/communication/datamap.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/communication/diagnostics.hh` & `dune-alugrid-2.9.dev20220529/examples/communication/diagnostics.hh`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #endif
 
 namespace Dune {
 
   template <class GridType>
   class Diagnostics
   {
-    typedef typename GridType :: Traits :: Communication CommunicatorType;
+    typedef typename GridType :: Traits :: CollectiveCommunication CommunicatorType;
     const CommunicatorType& comm_;
     const std::string runFileName_;
     const int writeDiagnostics_; // 0 don't, 1 only speedup file, 2 write all runfiles
                                  // 3 only write 0, others at end, 4 all files at end
     std::ostream* diagnosticsFile_;
 
     std::vector< double > times_ ;
```

### Comparing `dune-alugrid-2.9.0rc1/examples/communication/fvscheme.hh` & `dune-alugrid-2.9.dev20220529/examples/communication/fvscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/communication/main.cc` & `dune-alugrid-2.9.dev20220529/examples/communication/main.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/communication/paralleldgf.hh` & `dune-alugrid-2.9.dev20220529/examples/communication/paralleldgf.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/communication/piecewisefunction.hh` & `dune-alugrid-2.9.dev20220529/examples/communication/piecewisefunction.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/communication/problem-ball.hh` & `dune-alugrid-2.9.dev20220529/examples/communication/problem-ball.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/communication/problem-euler.hh` & `dune-alugrid-2.9.dev20220529/examples/communication/problem-euler.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/communication/problem-transport.hh` & `dune-alugrid-2.9.dev20220529/examples/communication/problem-transport.hh`

 * *Files 25% similar despite different names*

```diff
@@ -15,64 +15,37 @@
  */
 template< int dimD >
 class TransportProblemData1
 : public ProblemData< dimD, 1 >
 {
   typedef ProblemData< dimD, 1 > Base;
 
-public:
-  const static int dimDomain = Base::dimDomain;
-  const static int dimRange = Base::dimRange;
-
-  typedef typename Base::DomainType DomainType;
-  typedef typename Base::RangeType RangeType;
-
-protected:
   std::string gridFile_;
-  DomainType velocity_;
-  int problem_;
 public:
-  TransportProblemData1( const int problem ) : problem_( problem )
+  TransportProblemData1( const int problem )
   {
     if( problem == 3 )
     {
       gridFile_ = "/dgf/periodic" + std::to_string(dimDomain) + ".dgf";
     }
     else
     {
       gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
     }
-
-    if( problem < 3 )
-    {
-      // set transport velocity
-      velocity_ = DomainType( 1.25 );
-    }
-    else
-    {
-      velocity_ = 0.0;
-      velocity_[ 0 ] = 1.25;
-    }
   }
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = velocity_;
-  }
+  const static int dimDomain = Base::dimDomain;
+  const static int dimRange = Base::dimRange;
+
+  typedef typename Base::DomainType DomainType;
+  typedef typename Base::RangeType RangeType;
 
   //! \copydoc ProblemData::initial
   RangeType initial ( const DomainType &x ) const
   {
-    if( problem_ == 3 )
-    {
-      DomainType xc( x );
-      xc -= 0.5;
-      return (xc*xc) < 0.0625 ? 1.0 : 0;
-    }
-
     return sin( 2 * M_PI * (x*x) );
   }
 
   //! \copydoc ProblemData::endTime
   double endTime () const
   {
     return 0.8;
@@ -117,168 +90,46 @@
  */
 template< int dimD >
 class TransportProblemData2
 : public ProblemData< dimD, 1 >
 {
   typedef ProblemData< dimD, 1  > Base;
 
-public:
-  const static int dimDomain = Base::dimDomain;
-  const static int dimRange = Base::dimRange;
-
-  typedef typename Base::DomainType DomainType;
-  typedef typename Base::RangeType RangeType;
-
-protected:
   std::string gridFile_;
-  DomainType velocity_;
 public:
   TransportProblemData2( const int problem )
   {
     if( problem == 4 )
     {
       gridFile_ = "/dgf/periodic" + std::to_string(dimDomain) + ".dgf";
     }
     else
     {
       gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
     }
-
-    if( problem < 3 )
-    {
-      // set transport velocity
-      velocity_ = DomainType( 1.25 );
-    }
-    else
-    {
-      velocity_ = 0.0;
-      velocity_[ 0 ] = 1.25;
-    }
-  }
-
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = velocity_;
-  }
-
-  //! \copydoc ProblemData::initial
-  RangeType initial ( const DomainType &x ) const
-  {
-    DomainType r(0.5);
-    return ((x-r).two_norm() < 0.25 ? RangeType( 1 ) : RangeType( 0 ) );
-    //return ((x-r).two_norm() < 0.5 ? RangeType( 1 ) : RangeType( 0 ) );
-  }
-
-  //! \copydoc ProblemData::endTime
-  double endTime () const
-  {
-    return 0.8;
-  }
-
-  //! \copydoc ProblemData::gridFile
-  std::string gridFile ( const std::string &path, const int mpiSize ) const
-  {
-    return path + gridFile_;
-  }
-
-  RangeType boundaryValue ( const DomainType &x, double time ) const
-  {
-    return initial( x );
-  }
-
-  int bndType( const DomainType &normal, const DomainType &x, const double time) const
-  {
-    return 1;
-  }
-
-  double saveInterval () const
-  {
-    return 0.05;
-  }
-  //! \copydoc ProblemData::refineTol
-  double refineTol () const
-  {
-    return 0.1;
-  }
-  double adaptationIndicator ( const DomainType& x, double time,
-                               const RangeType &uLeft, const RangeType &uRight ) const
-  {
-    return std::abs( uLeft[ 0 ] - uRight[ 0 ] );
-  }
-};
-
-/**
- * \brief Solid body rotation
- */
-template< int dimD >
-class SolidBodyRotation
-: public ProblemData< dimD, 1 >
-{
-  typedef ProblemData< dimD, 1  > Base;
-
-  std::string gridFile_;
-public:
-  SolidBodyRotation( const int problem )
-  {
-    gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
   }
 
   const static int dimDomain = Base::dimDomain;
   const static int dimRange = Base::dimRange;
 
   typedef typename Base::DomainType DomainType;
   typedef typename Base::RangeType RangeType;
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    //v = velocity_;
-    double angular_velocity = 1.0;
-    DomainType rotation_centre = DomainType(0.5);
-    DomainType radius = x - rotation_centre;
-    v[0] = -angular_velocity*radius[1];
-    v[1] = angular_velocity*radius[0];
-  }
-
   //! \copydoc ProblemData::initial
   RangeType initial ( const DomainType &x ) const
   {
-    RangeType res(0) ;
-
-    DomainType c1( 0.5 ), c2( 0.5 ), c3( 0.5 ), c4( 0.5 );
-    c1[ 0 ] = 0.5;  c1[ 1 ] = 0.75;
-    c2[ 0 ] = 0.5;  c2[ 1 ] = 0.25;
-    c3[ 0 ] = 0.25; c3[ 1 ] = 0.5;
-    c4[ 0 ] = 0.35; c4[ 1 ] = 0.65;
-    const double r = 0.15;
-
-    // slotted cylinder
-    if( (x - c1).two_norm() < r )
-    {
-      if( (std::abs( x[ 0 ] - c1[ 0 ] ) >= 0.025) || (x[ 1 ] >= c1[ 1 ] + 0.1) )
-        return RangeType( 1.0 );
-      else
-        return RangeType( 0.0 );
-    }
-
-    // cone
-    if( (x - c2).two_norm() < r )
-      return RangeType( (r - (x - c2).two_norm()) / r );
-
-    // hump
-    if( (x - c3).two_norm() < r )
-      return RangeType((1.0 + std::cos( M_PI * (x - c3).two_norm() / r )) / 4.0 );
-
-    // default
-    return RangeType( 0.0 );
+    DomainType r(0.5);
+    return ((x-r).two_norm() < 0.25 ? RangeType( 1 ) : RangeType( 0 ) );
+    //return ((x-r).two_norm() < 0.5 ? RangeType( 1 ) : RangeType( 0 ) );
   }
 
   //! \copydoc ProblemData::endTime
   double endTime () const
   {
-    return 1.5708;
+    return 0.8;
   }
 
   //! \copydoc ProblemData::gridFile
   std::string gridFile ( const std::string &path, const int mpiSize ) const
   {
     return path + gridFile_;
   }
@@ -346,34 +197,48 @@
     case 3:
       problem_.reset( new TransportProblemData1< dimDomain >( problem ) );
       break;
     case 2:
     case 4:
       problem_.reset( new TransportProblemData2< dimDomain >( problem ) );
       break;
-    case 5:
-      problem_.reset( new SolidBodyRotation< dimDomain >( problem ) );
-      break;
     default:
       std::cerr << "Problem " << problem << " does not exists." << std::endl;
       std::abort();
     }
+
+    if( problem < 3 )
+    {
+      // set transport velocity
+      velocity_ = DomainType( 1.25 );
+    }
+    else
+    {
+      velocity_ = 0.0;
+      velocity_[ 0 ] = 1.25;
+    }
   }
 
   /** \brief obtain problem */
   const Problem &problem () const
   {
     return *problem_;
   }
 
   double fixedDt () const
   {
     return -1;
   }
 
+  /** \brief obtain the (constant) velocity for the transport problem */
+  const DomainType &velocity () const
+  {
+    return velocity_;
+  }
+
   /** \brief evaluate the numerical flux on an intersection
    *
    *  \param[in]   normal   scaled normal of the intersection
    *  \param[in]   time     current time
    *  \param[in]   xGlobal  evaluation point in global coordinates
    *  \param[in]   uLeft    value of the solution in the inside entity
    *  \param[in]   uRight   value of the solution in the outside entity
@@ -383,17 +248,15 @@
    */
   double numericalFlux ( const DomainType &normal,
                          const double time,
                          const DomainType &xGlobal,
                          const RangeType &uLeft, const RangeType &uRight,
                          RangeType &flux ) const
   {
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    const double upwind = normal * velocity;
+    const double upwind = normal * velocity();
     flux = upwind * (upwind > 0 ? uLeft : uRight);
     return std::abs( upwind );
   }
 
   /** \brief evaluate the numerical flux on a boundary
    *
    *  \param[in]   normal   scaled normal of the boundary
@@ -408,17 +271,15 @@
                         const double time,
                         const DomainType &xGlobal,
                         const RangeType& uLeft,
                         RangeType &flux ) const
   {
     // exact solution is u0(x-ta)
     DomainType x0( xGlobal );
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    x0.axpy( -time, velocity );
+    x0.axpy( -time, velocity_ );
     RangeType uRight = problem().boundaryValue( x0, time );
     return numericalFlux( normal, time, xGlobal, uLeft, uRight, flux );
   }
 
   /** \brief compute adaptation indicator at intersection
    *
    *  \param[in]   normal   scaled normal of the intersection
@@ -448,20 +309,19 @@
    */
   double boundaryIndicator ( const DomainType &normal,
                              const double time,
                              const DomainType &xGlobal,
                              const RangeType& uLeft) const
   {
     DomainType x0( xGlobal );
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    x0.axpy( -time, velocity );
+    x0.axpy( -time, velocity_ );
     return indicator( normal,time,xGlobal, uLeft, problem().boundaryValue(x0,time) );
   }
 
 protected:
-  TransportModel ( ) : problem_() {}
+  TransportModel ( ) : problem_(), velocity_(1) {}
 private:
   std::unique_ptr< Problem > problem_;
+  DomainType velocity_;
 }; // end class TransportModel
 
 #endif // PROBLEM_TRANSPORT_HH
```

### Comparing `dune-alugrid-2.9.0rc1/examples/communication/problem.hh` & `dune-alugrid-2.9.dev20220529/examples/communication/problem.hh`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,11 @@
 
   /**\brief return number of timestep to pass until load balancing is done again  */
   virtual int balanceStep() const { return 1; }
 
   /**\brief return maximal number of timesteps to run (for scaling experiment) */
   virtual unsigned int maxTimeSteps() const { return std::numeric_limits<unsigned int>::max(); }
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = 0;
-  }
-
 }; // end class ProblemData
 // Code moved to problem-transport.hh
 
 #endif // PROBLEM_HH
```

### Comparing `dune-alugrid-2.9.0rc1/examples/datamap.hh` & `dune-alugrid-2.9.dev20220529/examples/datamap.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/cube3d.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/cube3d.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/cube3d.dgf.3.0` & `dune-alugrid-2.9.dev20220529/examples/dgf/cube3d.dgf.3.0`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/cube3d.dgf.3.1` & `dune-alugrid-2.9.dev20220529/examples/dgf/cube3d.dgf.3.1`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/cube3d.dgf.3.2` & `dune-alugrid-2.9.dev20220529/examples/dgf/cube3d.dgf.3.2`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/cube_hc_32768.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/cube_hc_32768.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/cube_hc_4096.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/cube_hc_4096.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/cube_hc_512.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/cube_hc_512.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/ffs3d.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/ffs3d.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/ffs3d_fine.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/ffs3d_fine.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/sb2d.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/sb2d.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/sb2d_6400.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/sb2d_6400.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/sb2d_65536.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/sb2d_65536.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/sb3d.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/sb3d.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/sb3d_1024.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/sb3d_1024.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/sb3d_128.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/sb3d_128.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/sb3d_16.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/sb3d_16.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/sb3d_65536.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/sb3d_65536.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/sb3d_8192.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/sb3d_8192.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/tet.0.msh.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/tet.0.msh.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/tet.00.msh.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/tet.00.msh.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/tet.1.msh.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/tet.1.msh.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/tet.2.msh.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/tet.2.msh.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/tet.3.msh.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/tet.3.msh.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/tet.4.msh.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/tet.4.msh.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/tet.5.msh.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/tet.5.msh.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/tet.6.msh.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/tet.6.msh.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/tet_120k.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/tet_120k.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/tet_240k.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/tet_240k.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/tet_480k.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/tet_480k.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/tet_960k.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/tet_960k.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/tetexp.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/tetexp.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/tetgen.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/tetgen.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/unitcube2d.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/unitcube2d.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/dgf/unitcube3d.dgf` & `dune-alugrid-2.9.dev20220529/examples/dgf/unitcube3d.dgf`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/diagnostics.hh` & `dune-alugrid-2.9.dev20220529/examples/diagnostics.hh`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #endif
 
 namespace Dune {
 
   template <class GridType>
   class Diagnostics
   {
-    typedef typename GridType :: Traits :: Communication CommunicatorType;
+    typedef typename GridType :: Traits :: CollectiveCommunication CommunicatorType;
     const CommunicatorType& comm_;
     const std::string runFileName_;
     const int writeDiagnostics_; // 0 don't, 1 only speedup file, 2 write all runfiles
                                  // 3 only write 0, others at end, 4 all files at end
     std::ostream* diagnosticsFile_;
 
     std::vector< double > times_ ;
```

### Comparing `dune-alugrid-2.9.0rc1/examples/fvscheme.hh` & `dune-alugrid-2.9.dev20220529/examples/fvscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/loadbalance/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/examples/loadbalance/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/loadbalance/adaptation.hh` & `dune-alugrid-2.9.dev20220529/examples/loadbalance/adaptation.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/loadbalance/datamap.hh` & `dune-alugrid-2.9.dev20220529/examples/loadbalance/datamap.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/loadbalance/diagnostics.hh` & `dune-alugrid-2.9.dev20220529/examples/loadbalance/diagnostics.hh`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #endif
 
 namespace Dune {
 
   template <class GridType>
   class Diagnostics
   {
-    typedef typename GridType :: Traits :: Communication CommunicatorType;
+    typedef typename GridType :: Traits :: CollectiveCommunication CommunicatorType;
     const CommunicatorType& comm_;
     const std::string runFileName_;
     const int writeDiagnostics_; // 0 don't, 1 only speedup file, 2 write all runfiles
                                  // 3 only write 0, others at end, 4 all files at end
     std::ostream* diagnosticsFile_;
 
     std::vector< double > times_ ;
```

### Comparing `dune-alugrid-2.9.0rc1/examples/loadbalance/fvscheme.hh` & `dune-alugrid-2.9.dev20220529/examples/loadbalance/fvscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/loadbalance/loadbalance_simple.hh` & `dune-alugrid-2.9.dev20220529/examples/loadbalance/loadbalance_simple.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/loadbalance/loadbalance_zoltan.hh` & `dune-alugrid-2.9.dev20220529/examples/loadbalance/loadbalance_zoltan.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/loadbalance/main.cc` & `dune-alugrid-2.9.dev20220529/examples/loadbalance/main.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/loadbalance/paralleldgf.hh` & `dune-alugrid-2.9.dev20220529/examples/loadbalance/paralleldgf.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/loadbalance/piecewisefunction.hh` & `dune-alugrid-2.9.dev20220529/examples/loadbalance/piecewisefunction.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/loadbalance/problem-ball.hh` & `dune-alugrid-2.9.dev20220529/examples/loadbalance/problem-ball.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/loadbalance/problem-euler.hh` & `dune-alugrid-2.9.dev20220529/examples/loadbalance/problem-euler.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/loadbalance/problem-transport.hh` & `dune-alugrid-2.9.dev20220529/examples/loadbalance/problem-transport.hh`

 * *Files 25% similar despite different names*

```diff
@@ -15,64 +15,37 @@
  */
 template< int dimD >
 class TransportProblemData1
 : public ProblemData< dimD, 1 >
 {
   typedef ProblemData< dimD, 1 > Base;
 
-public:
-  const static int dimDomain = Base::dimDomain;
-  const static int dimRange = Base::dimRange;
-
-  typedef typename Base::DomainType DomainType;
-  typedef typename Base::RangeType RangeType;
-
-protected:
   std::string gridFile_;
-  DomainType velocity_;
-  int problem_;
 public:
-  TransportProblemData1( const int problem ) : problem_( problem )
+  TransportProblemData1( const int problem )
   {
     if( problem == 3 )
     {
       gridFile_ = "/dgf/periodic" + std::to_string(dimDomain) + ".dgf";
     }
     else
     {
       gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
     }
-
-    if( problem < 3 )
-    {
-      // set transport velocity
-      velocity_ = DomainType( 1.25 );
-    }
-    else
-    {
-      velocity_ = 0.0;
-      velocity_[ 0 ] = 1.25;
-    }
   }
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = velocity_;
-  }
+  const static int dimDomain = Base::dimDomain;
+  const static int dimRange = Base::dimRange;
+
+  typedef typename Base::DomainType DomainType;
+  typedef typename Base::RangeType RangeType;
 
   //! \copydoc ProblemData::initial
   RangeType initial ( const DomainType &x ) const
   {
-    if( problem_ == 3 )
-    {
-      DomainType xc( x );
-      xc -= 0.5;
-      return (xc*xc) < 0.0625 ? 1.0 : 0;
-    }
-
     return sin( 2 * M_PI * (x*x) );
   }
 
   //! \copydoc ProblemData::endTime
   double endTime () const
   {
     return 0.8;
@@ -117,168 +90,46 @@
  */
 template< int dimD >
 class TransportProblemData2
 : public ProblemData< dimD, 1 >
 {
   typedef ProblemData< dimD, 1  > Base;
 
-public:
-  const static int dimDomain = Base::dimDomain;
-  const static int dimRange = Base::dimRange;
-
-  typedef typename Base::DomainType DomainType;
-  typedef typename Base::RangeType RangeType;
-
-protected:
   std::string gridFile_;
-  DomainType velocity_;
 public:
   TransportProblemData2( const int problem )
   {
     if( problem == 4 )
     {
       gridFile_ = "/dgf/periodic" + std::to_string(dimDomain) + ".dgf";
     }
     else
     {
       gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
     }
-
-    if( problem < 3 )
-    {
-      // set transport velocity
-      velocity_ = DomainType( 1.25 );
-    }
-    else
-    {
-      velocity_ = 0.0;
-      velocity_[ 0 ] = 1.25;
-    }
-  }
-
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = velocity_;
-  }
-
-  //! \copydoc ProblemData::initial
-  RangeType initial ( const DomainType &x ) const
-  {
-    DomainType r(0.5);
-    return ((x-r).two_norm() < 0.25 ? RangeType( 1 ) : RangeType( 0 ) );
-    //return ((x-r).two_norm() < 0.5 ? RangeType( 1 ) : RangeType( 0 ) );
-  }
-
-  //! \copydoc ProblemData::endTime
-  double endTime () const
-  {
-    return 0.8;
-  }
-
-  //! \copydoc ProblemData::gridFile
-  std::string gridFile ( const std::string &path, const int mpiSize ) const
-  {
-    return path + gridFile_;
-  }
-
-  RangeType boundaryValue ( const DomainType &x, double time ) const
-  {
-    return initial( x );
-  }
-
-  int bndType( const DomainType &normal, const DomainType &x, const double time) const
-  {
-    return 1;
-  }
-
-  double saveInterval () const
-  {
-    return 0.05;
-  }
-  //! \copydoc ProblemData::refineTol
-  double refineTol () const
-  {
-    return 0.1;
-  }
-  double adaptationIndicator ( const DomainType& x, double time,
-                               const RangeType &uLeft, const RangeType &uRight ) const
-  {
-    return std::abs( uLeft[ 0 ] - uRight[ 0 ] );
-  }
-};
-
-/**
- * \brief Solid body rotation
- */
-template< int dimD >
-class SolidBodyRotation
-: public ProblemData< dimD, 1 >
-{
-  typedef ProblemData< dimD, 1  > Base;
-
-  std::string gridFile_;
-public:
-  SolidBodyRotation( const int problem )
-  {
-    gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
   }
 
   const static int dimDomain = Base::dimDomain;
   const static int dimRange = Base::dimRange;
 
   typedef typename Base::DomainType DomainType;
   typedef typename Base::RangeType RangeType;
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    //v = velocity_;
-    double angular_velocity = 1.0;
-    DomainType rotation_centre = DomainType(0.5);
-    DomainType radius = x - rotation_centre;
-    v[0] = -angular_velocity*radius[1];
-    v[1] = angular_velocity*radius[0];
-  }
-
   //! \copydoc ProblemData::initial
   RangeType initial ( const DomainType &x ) const
   {
-    RangeType res(0) ;
-
-    DomainType c1( 0.5 ), c2( 0.5 ), c3( 0.5 ), c4( 0.5 );
-    c1[ 0 ] = 0.5;  c1[ 1 ] = 0.75;
-    c2[ 0 ] = 0.5;  c2[ 1 ] = 0.25;
-    c3[ 0 ] = 0.25; c3[ 1 ] = 0.5;
-    c4[ 0 ] = 0.35; c4[ 1 ] = 0.65;
-    const double r = 0.15;
-
-    // slotted cylinder
-    if( (x - c1).two_norm() < r )
-    {
-      if( (std::abs( x[ 0 ] - c1[ 0 ] ) >= 0.025) || (x[ 1 ] >= c1[ 1 ] + 0.1) )
-        return RangeType( 1.0 );
-      else
-        return RangeType( 0.0 );
-    }
-
-    // cone
-    if( (x - c2).two_norm() < r )
-      return RangeType( (r - (x - c2).two_norm()) / r );
-
-    // hump
-    if( (x - c3).two_norm() < r )
-      return RangeType((1.0 + std::cos( M_PI * (x - c3).two_norm() / r )) / 4.0 );
-
-    // default
-    return RangeType( 0.0 );
+    DomainType r(0.5);
+    return ((x-r).two_norm() < 0.25 ? RangeType( 1 ) : RangeType( 0 ) );
+    //return ((x-r).two_norm() < 0.5 ? RangeType( 1 ) : RangeType( 0 ) );
   }
 
   //! \copydoc ProblemData::endTime
   double endTime () const
   {
-    return 1.5708;
+    return 0.8;
   }
 
   //! \copydoc ProblemData::gridFile
   std::string gridFile ( const std::string &path, const int mpiSize ) const
   {
     return path + gridFile_;
   }
@@ -346,34 +197,48 @@
     case 3:
       problem_.reset( new TransportProblemData1< dimDomain >( problem ) );
       break;
     case 2:
     case 4:
       problem_.reset( new TransportProblemData2< dimDomain >( problem ) );
       break;
-    case 5:
-      problem_.reset( new SolidBodyRotation< dimDomain >( problem ) );
-      break;
     default:
       std::cerr << "Problem " << problem << " does not exists." << std::endl;
       std::abort();
     }
+
+    if( problem < 3 )
+    {
+      // set transport velocity
+      velocity_ = DomainType( 1.25 );
+    }
+    else
+    {
+      velocity_ = 0.0;
+      velocity_[ 0 ] = 1.25;
+    }
   }
 
   /** \brief obtain problem */
   const Problem &problem () const
   {
     return *problem_;
   }
 
   double fixedDt () const
   {
     return -1;
   }
 
+  /** \brief obtain the (constant) velocity for the transport problem */
+  const DomainType &velocity () const
+  {
+    return velocity_;
+  }
+
   /** \brief evaluate the numerical flux on an intersection
    *
    *  \param[in]   normal   scaled normal of the intersection
    *  \param[in]   time     current time
    *  \param[in]   xGlobal  evaluation point in global coordinates
    *  \param[in]   uLeft    value of the solution in the inside entity
    *  \param[in]   uRight   value of the solution in the outside entity
@@ -383,17 +248,15 @@
    */
   double numericalFlux ( const DomainType &normal,
                          const double time,
                          const DomainType &xGlobal,
                          const RangeType &uLeft, const RangeType &uRight,
                          RangeType &flux ) const
   {
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    const double upwind = normal * velocity;
+    const double upwind = normal * velocity();
     flux = upwind * (upwind > 0 ? uLeft : uRight);
     return std::abs( upwind );
   }
 
   /** \brief evaluate the numerical flux on a boundary
    *
    *  \param[in]   normal   scaled normal of the boundary
@@ -408,17 +271,15 @@
                         const double time,
                         const DomainType &xGlobal,
                         const RangeType& uLeft,
                         RangeType &flux ) const
   {
     // exact solution is u0(x-ta)
     DomainType x0( xGlobal );
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    x0.axpy( -time, velocity );
+    x0.axpy( -time, velocity_ );
     RangeType uRight = problem().boundaryValue( x0, time );
     return numericalFlux( normal, time, xGlobal, uLeft, uRight, flux );
   }
 
   /** \brief compute adaptation indicator at intersection
    *
    *  \param[in]   normal   scaled normal of the intersection
@@ -448,20 +309,19 @@
    */
   double boundaryIndicator ( const DomainType &normal,
                              const double time,
                              const DomainType &xGlobal,
                              const RangeType& uLeft) const
   {
     DomainType x0( xGlobal );
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    x0.axpy( -time, velocity );
+    x0.axpy( -time, velocity_ );
     return indicator( normal,time,xGlobal, uLeft, problem().boundaryValue(x0,time) );
   }
 
 protected:
-  TransportModel ( ) : problem_() {}
+  TransportModel ( ) : problem_(), velocity_(1) {}
 private:
   std::unique_ptr< Problem > problem_;
+  DomainType velocity_;
 }; // end class TransportModel
 
 #endif // PROBLEM_TRANSPORT_HH
```

### Comparing `dune-alugrid-2.9.0rc1/examples/loadbalance/problem.hh` & `dune-alugrid-2.9.dev20220529/examples/loadbalance/problem.hh`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,11 @@
 
   /**\brief return number of timestep to pass until load balancing is done again  */
   virtual int balanceStep() const { return 1; }
 
   /**\brief return maximal number of timesteps to run (for scaling experiment) */
   virtual unsigned int maxTimeSteps() const { return std::numeric_limits<unsigned int>::max(); }
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = 0;
-  }
-
 }; // end class ProblemData
 // Code moved to problem-transport.hh
 
 #endif // PROBLEM_HH
```

### Comparing `dune-alugrid-2.9.0rc1/examples/main.cc` & `dune-alugrid-2.9.dev20220529/examples/main.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/paralleldgf.hh` & `dune-alugrid-2.9.dev20220529/examples/paralleldgf.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/piecewisefunction.hh` & `dune-alugrid-2.9.dev20220529/examples/piecewisefunction.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/problem-ball.hh` & `dune-alugrid-2.9.dev20220529/examples/problem-ball.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/problem-euler.hh` & `dune-alugrid-2.9.dev20220529/examples/problem-euler.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/problem-transport.hh` & `dune-alugrid-2.9.dev20220529/examples/problem-transport.hh`

 * *Files 25% similar despite different names*

```diff
@@ -15,64 +15,37 @@
  */
 template< int dimD >
 class TransportProblemData1
 : public ProblemData< dimD, 1 >
 {
   typedef ProblemData< dimD, 1 > Base;
 
-public:
-  const static int dimDomain = Base::dimDomain;
-  const static int dimRange = Base::dimRange;
-
-  typedef typename Base::DomainType DomainType;
-  typedef typename Base::RangeType RangeType;
-
-protected:
   std::string gridFile_;
-  DomainType velocity_;
-  int problem_;
 public:
-  TransportProblemData1( const int problem ) : problem_( problem )
+  TransportProblemData1( const int problem )
   {
     if( problem == 3 )
     {
       gridFile_ = "/dgf/periodic" + std::to_string(dimDomain) + ".dgf";
     }
     else
     {
       gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
     }
-
-    if( problem < 3 )
-    {
-      // set transport velocity
-      velocity_ = DomainType( 1.25 );
-    }
-    else
-    {
-      velocity_ = 0.0;
-      velocity_[ 0 ] = 1.25;
-    }
   }
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = velocity_;
-  }
+  const static int dimDomain = Base::dimDomain;
+  const static int dimRange = Base::dimRange;
+
+  typedef typename Base::DomainType DomainType;
+  typedef typename Base::RangeType RangeType;
 
   //! \copydoc ProblemData::initial
   RangeType initial ( const DomainType &x ) const
   {
-    if( problem_ == 3 )
-    {
-      DomainType xc( x );
-      xc -= 0.5;
-      return (xc*xc) < 0.0625 ? 1.0 : 0;
-    }
-
     return sin( 2 * M_PI * (x*x) );
   }
 
   //! \copydoc ProblemData::endTime
   double endTime () const
   {
     return 0.8;
@@ -117,168 +90,46 @@
  */
 template< int dimD >
 class TransportProblemData2
 : public ProblemData< dimD, 1 >
 {
   typedef ProblemData< dimD, 1  > Base;
 
-public:
-  const static int dimDomain = Base::dimDomain;
-  const static int dimRange = Base::dimRange;
-
-  typedef typename Base::DomainType DomainType;
-  typedef typename Base::RangeType RangeType;
-
-protected:
   std::string gridFile_;
-  DomainType velocity_;
 public:
   TransportProblemData2( const int problem )
   {
     if( problem == 4 )
     {
       gridFile_ = "/dgf/periodic" + std::to_string(dimDomain) + ".dgf";
     }
     else
     {
       gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
     }
-
-    if( problem < 3 )
-    {
-      // set transport velocity
-      velocity_ = DomainType( 1.25 );
-    }
-    else
-    {
-      velocity_ = 0.0;
-      velocity_[ 0 ] = 1.25;
-    }
-  }
-
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = velocity_;
-  }
-
-  //! \copydoc ProblemData::initial
-  RangeType initial ( const DomainType &x ) const
-  {
-    DomainType r(0.5);
-    return ((x-r).two_norm() < 0.25 ? RangeType( 1 ) : RangeType( 0 ) );
-    //return ((x-r).two_norm() < 0.5 ? RangeType( 1 ) : RangeType( 0 ) );
-  }
-
-  //! \copydoc ProblemData::endTime
-  double endTime () const
-  {
-    return 0.8;
-  }
-
-  //! \copydoc ProblemData::gridFile
-  std::string gridFile ( const std::string &path, const int mpiSize ) const
-  {
-    return path + gridFile_;
-  }
-
-  RangeType boundaryValue ( const DomainType &x, double time ) const
-  {
-    return initial( x );
-  }
-
-  int bndType( const DomainType &normal, const DomainType &x, const double time) const
-  {
-    return 1;
-  }
-
-  double saveInterval () const
-  {
-    return 0.05;
-  }
-  //! \copydoc ProblemData::refineTol
-  double refineTol () const
-  {
-    return 0.1;
-  }
-  double adaptationIndicator ( const DomainType& x, double time,
-                               const RangeType &uLeft, const RangeType &uRight ) const
-  {
-    return std::abs( uLeft[ 0 ] - uRight[ 0 ] );
-  }
-};
-
-/**
- * \brief Solid body rotation
- */
-template< int dimD >
-class SolidBodyRotation
-: public ProblemData< dimD, 1 >
-{
-  typedef ProblemData< dimD, 1  > Base;
-
-  std::string gridFile_;
-public:
-  SolidBodyRotation( const int problem )
-  {
-    gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
   }
 
   const static int dimDomain = Base::dimDomain;
   const static int dimRange = Base::dimRange;
 
   typedef typename Base::DomainType DomainType;
   typedef typename Base::RangeType RangeType;
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    //v = velocity_;
-    double angular_velocity = 1.0;
-    DomainType rotation_centre = DomainType(0.5);
-    DomainType radius = x - rotation_centre;
-    v[0] = -angular_velocity*radius[1];
-    v[1] = angular_velocity*radius[0];
-  }
-
   //! \copydoc ProblemData::initial
   RangeType initial ( const DomainType &x ) const
   {
-    RangeType res(0) ;
-
-    DomainType c1( 0.5 ), c2( 0.5 ), c3( 0.5 ), c4( 0.5 );
-    c1[ 0 ] = 0.5;  c1[ 1 ] = 0.75;
-    c2[ 0 ] = 0.5;  c2[ 1 ] = 0.25;
-    c3[ 0 ] = 0.25; c3[ 1 ] = 0.5;
-    c4[ 0 ] = 0.35; c4[ 1 ] = 0.65;
-    const double r = 0.15;
-
-    // slotted cylinder
-    if( (x - c1).two_norm() < r )
-    {
-      if( (std::abs( x[ 0 ] - c1[ 0 ] ) >= 0.025) || (x[ 1 ] >= c1[ 1 ] + 0.1) )
-        return RangeType( 1.0 );
-      else
-        return RangeType( 0.0 );
-    }
-
-    // cone
-    if( (x - c2).two_norm() < r )
-      return RangeType( (r - (x - c2).two_norm()) / r );
-
-    // hump
-    if( (x - c3).two_norm() < r )
-      return RangeType((1.0 + std::cos( M_PI * (x - c3).two_norm() / r )) / 4.0 );
-
-    // default
-    return RangeType( 0.0 );
+    DomainType r(0.5);
+    return ((x-r).two_norm() < 0.25 ? RangeType( 1 ) : RangeType( 0 ) );
+    //return ((x-r).two_norm() < 0.5 ? RangeType( 1 ) : RangeType( 0 ) );
   }
 
   //! \copydoc ProblemData::endTime
   double endTime () const
   {
-    return 1.5708;
+    return 0.8;
   }
 
   //! \copydoc ProblemData::gridFile
   std::string gridFile ( const std::string &path, const int mpiSize ) const
   {
     return path + gridFile_;
   }
@@ -346,34 +197,48 @@
     case 3:
       problem_.reset( new TransportProblemData1< dimDomain >( problem ) );
       break;
     case 2:
     case 4:
       problem_.reset( new TransportProblemData2< dimDomain >( problem ) );
       break;
-    case 5:
-      problem_.reset( new SolidBodyRotation< dimDomain >( problem ) );
-      break;
     default:
       std::cerr << "Problem " << problem << " does not exists." << std::endl;
       std::abort();
     }
+
+    if( problem < 3 )
+    {
+      // set transport velocity
+      velocity_ = DomainType( 1.25 );
+    }
+    else
+    {
+      velocity_ = 0.0;
+      velocity_[ 0 ] = 1.25;
+    }
   }
 
   /** \brief obtain problem */
   const Problem &problem () const
   {
     return *problem_;
   }
 
   double fixedDt () const
   {
     return -1;
   }
 
+  /** \brief obtain the (constant) velocity for the transport problem */
+  const DomainType &velocity () const
+  {
+    return velocity_;
+  }
+
   /** \brief evaluate the numerical flux on an intersection
    *
    *  \param[in]   normal   scaled normal of the intersection
    *  \param[in]   time     current time
    *  \param[in]   xGlobal  evaluation point in global coordinates
    *  \param[in]   uLeft    value of the solution in the inside entity
    *  \param[in]   uRight   value of the solution in the outside entity
@@ -383,17 +248,15 @@
    */
   double numericalFlux ( const DomainType &normal,
                          const double time,
                          const DomainType &xGlobal,
                          const RangeType &uLeft, const RangeType &uRight,
                          RangeType &flux ) const
   {
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    const double upwind = normal * velocity;
+    const double upwind = normal * velocity();
     flux = upwind * (upwind > 0 ? uLeft : uRight);
     return std::abs( upwind );
   }
 
   /** \brief evaluate the numerical flux on a boundary
    *
    *  \param[in]   normal   scaled normal of the boundary
@@ -408,17 +271,15 @@
                         const double time,
                         const DomainType &xGlobal,
                         const RangeType& uLeft,
                         RangeType &flux ) const
   {
     // exact solution is u0(x-ta)
     DomainType x0( xGlobal );
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    x0.axpy( -time, velocity );
+    x0.axpy( -time, velocity_ );
     RangeType uRight = problem().boundaryValue( x0, time );
     return numericalFlux( normal, time, xGlobal, uLeft, uRight, flux );
   }
 
   /** \brief compute adaptation indicator at intersection
    *
    *  \param[in]   normal   scaled normal of the intersection
@@ -448,20 +309,19 @@
    */
   double boundaryIndicator ( const DomainType &normal,
                              const double time,
                              const DomainType &xGlobal,
                              const RangeType& uLeft) const
   {
     DomainType x0( xGlobal );
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    x0.axpy( -time, velocity );
+    x0.axpy( -time, velocity_ );
     return indicator( normal,time,xGlobal, uLeft, problem().boundaryValue(x0,time) );
   }
 
 protected:
-  TransportModel ( ) : problem_() {}
+  TransportModel ( ) : problem_(), velocity_(1) {}
 private:
   std::unique_ptr< Problem > problem_;
+  DomainType velocity_;
 }; // end class TransportModel
 
 #endif // PROBLEM_TRANSPORT_HH
```

### Comparing `dune-alugrid-2.9.0rc1/examples/problem.hh` & `dune-alugrid-2.9.dev20220529/examples/problem.hh`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,11 @@
 
   /**\brief return number of timestep to pass until load balancing is done again  */
   virtual int balanceStep() const { return 1; }
 
   /**\brief return maximal number of timesteps to run (for scaling experiment) */
   virtual unsigned int maxTimeSteps() const { return std::numeric_limits<unsigned int>::max(); }
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = 0;
-  }
-
 }; // end class ProblemData
 // Code moved to problem-transport.hh
 
 #endif // PROBLEM_HH
```

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/examples/quality/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/adaptation.hh` & `dune-alugrid-2.9.dev20220529/examples/quality/adaptation.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/datamap.hh` & `dune-alugrid-2.9.dev20220529/examples/quality/datamap.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/diagnostics.hh` & `dune-alugrid-2.9.dev20220529/examples/quality/diagnostics.hh`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #endif
 
 namespace Dune {
 
   template <class GridType>
   class Diagnostics
   {
-    typedef typename GridType :: Traits :: Communication CommunicatorType;
+    typedef typename GridType :: Traits :: CollectiveCommunication CommunicatorType;
     const CommunicatorType& comm_;
     const std::string runFileName_;
     const int writeDiagnostics_; // 0 don't, 1 only speedup file, 2 write all runfiles
                                  // 3 only write 0, others at end, 4 all files at end
     std::ostream* diagnosticsFile_;
 
     std::vector< double > times_ ;
```

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/estimate-closure.cc` & `dune-alugrid-2.9.dev20220529/examples/quality/estimate-closure.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/fvscheme.hh` & `dune-alugrid-2.9.dev20220529/examples/quality/fvscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/gmsh2dgf.cc` & `dune-alugrid-2.9.dev20220529/examples/quality/gmsh2dgf.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/io.cc` & `dune-alugrid-2.9.dev20220529/examples/quality/io.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/io.hh` & `dune-alugrid-2.9.dev20220529/examples/quality/io.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/main.cc` & `dune-alugrid-2.9.dev20220529/examples/quality/main.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/paralleldgf.hh` & `dune-alugrid-2.9.dev20220529/examples/quality/paralleldgf.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/piecewisefunction.hh` & `dune-alugrid-2.9.dev20220529/examples/quality/piecewisefunction.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/problem-globalrefine.hh` & `dune-alugrid-2.9.dev20220529/examples/quality/problem-globalrefine.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/problem-transport.hh` & `dune-alugrid-2.9.dev20220529/examples/quality/problem-transport.hh`

 * *Files 25% similar despite different names*

```diff
@@ -15,64 +15,37 @@
  */
 template< int dimD >
 class TransportProblemData1
 : public ProblemData< dimD, 1 >
 {
   typedef ProblemData< dimD, 1 > Base;
 
-public:
-  const static int dimDomain = Base::dimDomain;
-  const static int dimRange = Base::dimRange;
-
-  typedef typename Base::DomainType DomainType;
-  typedef typename Base::RangeType RangeType;
-
-protected:
   std::string gridFile_;
-  DomainType velocity_;
-  int problem_;
 public:
-  TransportProblemData1( const int problem ) : problem_( problem )
+  TransportProblemData1( const int problem )
   {
     if( problem == 3 )
     {
       gridFile_ = "/dgf/periodic" + std::to_string(dimDomain) + ".dgf";
     }
     else
     {
       gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
     }
-
-    if( problem < 3 )
-    {
-      // set transport velocity
-      velocity_ = DomainType( 1.25 );
-    }
-    else
-    {
-      velocity_ = 0.0;
-      velocity_[ 0 ] = 1.25;
-    }
   }
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = velocity_;
-  }
+  const static int dimDomain = Base::dimDomain;
+  const static int dimRange = Base::dimRange;
+
+  typedef typename Base::DomainType DomainType;
+  typedef typename Base::RangeType RangeType;
 
   //! \copydoc ProblemData::initial
   RangeType initial ( const DomainType &x ) const
   {
-    if( problem_ == 3 )
-    {
-      DomainType xc( x );
-      xc -= 0.5;
-      return (xc*xc) < 0.0625 ? 1.0 : 0;
-    }
-
     return sin( 2 * M_PI * (x*x) );
   }
 
   //! \copydoc ProblemData::endTime
   double endTime () const
   {
     return 0.8;
@@ -117,168 +90,46 @@
  */
 template< int dimD >
 class TransportProblemData2
 : public ProblemData< dimD, 1 >
 {
   typedef ProblemData< dimD, 1  > Base;
 
-public:
-  const static int dimDomain = Base::dimDomain;
-  const static int dimRange = Base::dimRange;
-
-  typedef typename Base::DomainType DomainType;
-  typedef typename Base::RangeType RangeType;
-
-protected:
   std::string gridFile_;
-  DomainType velocity_;
 public:
   TransportProblemData2( const int problem )
   {
     if( problem == 4 )
     {
       gridFile_ = "/dgf/periodic" + std::to_string(dimDomain) + ".dgf";
     }
     else
     {
       gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
     }
-
-    if( problem < 3 )
-    {
-      // set transport velocity
-      velocity_ = DomainType( 1.25 );
-    }
-    else
-    {
-      velocity_ = 0.0;
-      velocity_[ 0 ] = 1.25;
-    }
-  }
-
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = velocity_;
-  }
-
-  //! \copydoc ProblemData::initial
-  RangeType initial ( const DomainType &x ) const
-  {
-    DomainType r(0.5);
-    return ((x-r).two_norm() < 0.25 ? RangeType( 1 ) : RangeType( 0 ) );
-    //return ((x-r).two_norm() < 0.5 ? RangeType( 1 ) : RangeType( 0 ) );
-  }
-
-  //! \copydoc ProblemData::endTime
-  double endTime () const
-  {
-    return 0.8;
-  }
-
-  //! \copydoc ProblemData::gridFile
-  std::string gridFile ( const std::string &path, const int mpiSize ) const
-  {
-    return path + gridFile_;
-  }
-
-  RangeType boundaryValue ( const DomainType &x, double time ) const
-  {
-    return initial( x );
-  }
-
-  int bndType( const DomainType &normal, const DomainType &x, const double time) const
-  {
-    return 1;
-  }
-
-  double saveInterval () const
-  {
-    return 0.05;
-  }
-  //! \copydoc ProblemData::refineTol
-  double refineTol () const
-  {
-    return 0.1;
-  }
-  double adaptationIndicator ( const DomainType& x, double time,
-                               const RangeType &uLeft, const RangeType &uRight ) const
-  {
-    return std::abs( uLeft[ 0 ] - uRight[ 0 ] );
-  }
-};
-
-/**
- * \brief Solid body rotation
- */
-template< int dimD >
-class SolidBodyRotation
-: public ProblemData< dimD, 1 >
-{
-  typedef ProblemData< dimD, 1  > Base;
-
-  std::string gridFile_;
-public:
-  SolidBodyRotation( const int problem )
-  {
-    gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
   }
 
   const static int dimDomain = Base::dimDomain;
   const static int dimRange = Base::dimRange;
 
   typedef typename Base::DomainType DomainType;
   typedef typename Base::RangeType RangeType;
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    //v = velocity_;
-    double angular_velocity = 1.0;
-    DomainType rotation_centre = DomainType(0.5);
-    DomainType radius = x - rotation_centre;
-    v[0] = -angular_velocity*radius[1];
-    v[1] = angular_velocity*radius[0];
-  }
-
   //! \copydoc ProblemData::initial
   RangeType initial ( const DomainType &x ) const
   {
-    RangeType res(0) ;
-
-    DomainType c1( 0.5 ), c2( 0.5 ), c3( 0.5 ), c4( 0.5 );
-    c1[ 0 ] = 0.5;  c1[ 1 ] = 0.75;
-    c2[ 0 ] = 0.5;  c2[ 1 ] = 0.25;
-    c3[ 0 ] = 0.25; c3[ 1 ] = 0.5;
-    c4[ 0 ] = 0.35; c4[ 1 ] = 0.65;
-    const double r = 0.15;
-
-    // slotted cylinder
-    if( (x - c1).two_norm() < r )
-    {
-      if( (std::abs( x[ 0 ] - c1[ 0 ] ) >= 0.025) || (x[ 1 ] >= c1[ 1 ] + 0.1) )
-        return RangeType( 1.0 );
-      else
-        return RangeType( 0.0 );
-    }
-
-    // cone
-    if( (x - c2).two_norm() < r )
-      return RangeType( (r - (x - c2).two_norm()) / r );
-
-    // hump
-    if( (x - c3).two_norm() < r )
-      return RangeType((1.0 + std::cos( M_PI * (x - c3).two_norm() / r )) / 4.0 );
-
-    // default
-    return RangeType( 0.0 );
+    DomainType r(0.5);
+    return ((x-r).two_norm() < 0.25 ? RangeType( 1 ) : RangeType( 0 ) );
+    //return ((x-r).two_norm() < 0.5 ? RangeType( 1 ) : RangeType( 0 ) );
   }
 
   //! \copydoc ProblemData::endTime
   double endTime () const
   {
-    return 1.5708;
+    return 0.8;
   }
 
   //! \copydoc ProblemData::gridFile
   std::string gridFile ( const std::string &path, const int mpiSize ) const
   {
     return path + gridFile_;
   }
@@ -346,34 +197,48 @@
     case 3:
       problem_.reset( new TransportProblemData1< dimDomain >( problem ) );
       break;
     case 2:
     case 4:
       problem_.reset( new TransportProblemData2< dimDomain >( problem ) );
       break;
-    case 5:
-      problem_.reset( new SolidBodyRotation< dimDomain >( problem ) );
-      break;
     default:
       std::cerr << "Problem " << problem << " does not exists." << std::endl;
       std::abort();
     }
+
+    if( problem < 3 )
+    {
+      // set transport velocity
+      velocity_ = DomainType( 1.25 );
+    }
+    else
+    {
+      velocity_ = 0.0;
+      velocity_[ 0 ] = 1.25;
+    }
   }
 
   /** \brief obtain problem */
   const Problem &problem () const
   {
     return *problem_;
   }
 
   double fixedDt () const
   {
     return -1;
   }
 
+  /** \brief obtain the (constant) velocity for the transport problem */
+  const DomainType &velocity () const
+  {
+    return velocity_;
+  }
+
   /** \brief evaluate the numerical flux on an intersection
    *
    *  \param[in]   normal   scaled normal of the intersection
    *  \param[in]   time     current time
    *  \param[in]   xGlobal  evaluation point in global coordinates
    *  \param[in]   uLeft    value of the solution in the inside entity
    *  \param[in]   uRight   value of the solution in the outside entity
@@ -383,17 +248,15 @@
    */
   double numericalFlux ( const DomainType &normal,
                          const double time,
                          const DomainType &xGlobal,
                          const RangeType &uLeft, const RangeType &uRight,
                          RangeType &flux ) const
   {
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    const double upwind = normal * velocity;
+    const double upwind = normal * velocity();
     flux = upwind * (upwind > 0 ? uLeft : uRight);
     return std::abs( upwind );
   }
 
   /** \brief evaluate the numerical flux on a boundary
    *
    *  \param[in]   normal   scaled normal of the boundary
@@ -408,17 +271,15 @@
                         const double time,
                         const DomainType &xGlobal,
                         const RangeType& uLeft,
                         RangeType &flux ) const
   {
     // exact solution is u0(x-ta)
     DomainType x0( xGlobal );
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    x0.axpy( -time, velocity );
+    x0.axpy( -time, velocity_ );
     RangeType uRight = problem().boundaryValue( x0, time );
     return numericalFlux( normal, time, xGlobal, uLeft, uRight, flux );
   }
 
   /** \brief compute adaptation indicator at intersection
    *
    *  \param[in]   normal   scaled normal of the intersection
@@ -448,20 +309,19 @@
    */
   double boundaryIndicator ( const DomainType &normal,
                              const double time,
                              const DomainType &xGlobal,
                              const RangeType& uLeft) const
   {
     DomainType x0( xGlobal );
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    x0.axpy( -time, velocity );
+    x0.axpy( -time, velocity_ );
     return indicator( normal,time,xGlobal, uLeft, problem().boundaryValue(x0,time) );
   }
 
 protected:
-  TransportModel ( ) : problem_() {}
+  TransportModel ( ) : problem_(), velocity_(1) {}
 private:
   std::unique_ptr< Problem > problem_;
+  DomainType velocity_;
 }; // end class TransportModel
 
 #endif // PROBLEM_TRANSPORT_HH
```

### Comparing `dune-alugrid-2.9.0rc1/examples/quality/problem.hh` & `dune-alugrid-2.9.dev20220529/examples/quality/problem.hh`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,11 @@
 
   /**\brief return number of timestep to pass until load balancing is done again  */
   virtual int balanceStep() const { return 1; }
 
   /**\brief return maximal number of timesteps to run (for scaling experiment) */
   virtual unsigned int maxTimeSteps() const { return std::numeric_limits<unsigned int>::max(); }
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = 0;
-  }
-
 }; // end class ProblemData
 // Code moved to problem-transport.hh
 
 #endif // PROBLEM_HH
```

### Comparing `dune-alugrid-2.9.0rc1/examples/testEfficiency/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/examples/testEfficiency/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/testEfficiency/adaptation.hh` & `dune-alugrid-2.9.dev20220529/examples/testEfficiency/adaptation.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/testEfficiency/check-efficiency.sh` & `dune-alugrid-2.9.dev20220529/examples/testEfficiency/check-efficiency.sh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/testEfficiency/datamap.hh` & `dune-alugrid-2.9.dev20220529/examples/testEfficiency/datamap.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/testEfficiency/diagnostics.hh` & `dune-alugrid-2.9.dev20220529/examples/testEfficiency/diagnostics.hh`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #endif
 
 namespace Dune {
 
   template <class GridType>
   class Diagnostics
   {
-    typedef typename GridType :: Traits :: Communication CommunicatorType;
+    typedef typename GridType :: Traits :: CollectiveCommunication CommunicatorType;
     const CommunicatorType& comm_;
     const std::string runFileName_;
     const int writeDiagnostics_; // 0 don't, 1 only speedup file, 2 write all runfiles
                                  // 3 only write 0, others at end, 4 all files at end
     std::ostream* diagnosticsFile_;
 
     std::vector< double > times_ ;
```

### Comparing `dune-alugrid-2.9.0rc1/examples/testEfficiency/fvscheme.hh` & `dune-alugrid-2.9.dev20220529/examples/testEfficiency/fvscheme.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/testEfficiency/main.cc` & `dune-alugrid-2.9.dev20220529/examples/testEfficiency/main.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/testEfficiency/paralleldgf.hh` & `dune-alugrid-2.9.dev20220529/examples/testEfficiency/paralleldgf.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/testEfficiency/piecewisefunction.hh` & `dune-alugrid-2.9.dev20220529/examples/testEfficiency/piecewisefunction.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/testEfficiency/problem-ball.hh` & `dune-alugrid-2.9.dev20220529/examples/testEfficiency/problem-ball.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/testEfficiency/problem-euler.hh` & `dune-alugrid-2.9.dev20220529/examples/testEfficiency/problem-euler.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/examples/testEfficiency/problem-transport.hh` & `dune-alugrid-2.9.dev20220529/examples/testEfficiency/problem-transport.hh`

 * *Files 25% similar despite different names*

```diff
@@ -15,64 +15,37 @@
  */
 template< int dimD >
 class TransportProblemData1
 : public ProblemData< dimD, 1 >
 {
   typedef ProblemData< dimD, 1 > Base;
 
-public:
-  const static int dimDomain = Base::dimDomain;
-  const static int dimRange = Base::dimRange;
-
-  typedef typename Base::DomainType DomainType;
-  typedef typename Base::RangeType RangeType;
-
-protected:
   std::string gridFile_;
-  DomainType velocity_;
-  int problem_;
 public:
-  TransportProblemData1( const int problem ) : problem_( problem )
+  TransportProblemData1( const int problem )
   {
     if( problem == 3 )
     {
       gridFile_ = "/dgf/periodic" + std::to_string(dimDomain) + ".dgf";
     }
     else
     {
       gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
     }
-
-    if( problem < 3 )
-    {
-      // set transport velocity
-      velocity_ = DomainType( 1.25 );
-    }
-    else
-    {
-      velocity_ = 0.0;
-      velocity_[ 0 ] = 1.25;
-    }
   }
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = velocity_;
-  }
+  const static int dimDomain = Base::dimDomain;
+  const static int dimRange = Base::dimRange;
+
+  typedef typename Base::DomainType DomainType;
+  typedef typename Base::RangeType RangeType;
 
   //! \copydoc ProblemData::initial
   RangeType initial ( const DomainType &x ) const
   {
-    if( problem_ == 3 )
-    {
-      DomainType xc( x );
-      xc -= 0.5;
-      return (xc*xc) < 0.0625 ? 1.0 : 0;
-    }
-
     return sin( 2 * M_PI * (x*x) );
   }
 
   //! \copydoc ProblemData::endTime
   double endTime () const
   {
     return 0.8;
@@ -117,168 +90,46 @@
  */
 template< int dimD >
 class TransportProblemData2
 : public ProblemData< dimD, 1 >
 {
   typedef ProblemData< dimD, 1  > Base;
 
-public:
-  const static int dimDomain = Base::dimDomain;
-  const static int dimRange = Base::dimRange;
-
-  typedef typename Base::DomainType DomainType;
-  typedef typename Base::RangeType RangeType;
-
-protected:
   std::string gridFile_;
-  DomainType velocity_;
 public:
   TransportProblemData2( const int problem )
   {
     if( problem == 4 )
     {
       gridFile_ = "/dgf/periodic" + std::to_string(dimDomain) + ".dgf";
     }
     else
     {
       gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
     }
-
-    if( problem < 3 )
-    {
-      // set transport velocity
-      velocity_ = DomainType( 1.25 );
-    }
-    else
-    {
-      velocity_ = 0.0;
-      velocity_[ 0 ] = 1.25;
-    }
-  }
-
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = velocity_;
-  }
-
-  //! \copydoc ProblemData::initial
-  RangeType initial ( const DomainType &x ) const
-  {
-    DomainType r(0.5);
-    return ((x-r).two_norm() < 0.25 ? RangeType( 1 ) : RangeType( 0 ) );
-    //return ((x-r).two_norm() < 0.5 ? RangeType( 1 ) : RangeType( 0 ) );
-  }
-
-  //! \copydoc ProblemData::endTime
-  double endTime () const
-  {
-    return 0.8;
-  }
-
-  //! \copydoc ProblemData::gridFile
-  std::string gridFile ( const std::string &path, const int mpiSize ) const
-  {
-    return path + gridFile_;
-  }
-
-  RangeType boundaryValue ( const DomainType &x, double time ) const
-  {
-    return initial( x );
-  }
-
-  int bndType( const DomainType &normal, const DomainType &x, const double time) const
-  {
-    return 1;
-  }
-
-  double saveInterval () const
-  {
-    return 0.05;
-  }
-  //! \copydoc ProblemData::refineTol
-  double refineTol () const
-  {
-    return 0.1;
-  }
-  double adaptationIndicator ( const DomainType& x, double time,
-                               const RangeType &uLeft, const RangeType &uRight ) const
-  {
-    return std::abs( uLeft[ 0 ] - uRight[ 0 ] );
-  }
-};
-
-/**
- * \brief Solid body rotation
- */
-template< int dimD >
-class SolidBodyRotation
-: public ProblemData< dimD, 1 >
-{
-  typedef ProblemData< dimD, 1  > Base;
-
-  std::string gridFile_;
-public:
-  SolidBodyRotation( const int problem )
-  {
-    gridFile_ = "/dgf/unitcube" + std::to_string(dimDomain) + "d.dgf";
   }
 
   const static int dimDomain = Base::dimDomain;
   const static int dimRange = Base::dimRange;
 
   typedef typename Base::DomainType DomainType;
   typedef typename Base::RangeType RangeType;
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    //v = velocity_;
-    double angular_velocity = 1.0;
-    DomainType rotation_centre = DomainType(0.5);
-    DomainType radius = x - rotation_centre;
-    v[0] = -angular_velocity*radius[1];
-    v[1] = angular_velocity*radius[0];
-  }
-
   //! \copydoc ProblemData::initial
   RangeType initial ( const DomainType &x ) const
   {
-    RangeType res(0) ;
-
-    DomainType c1( 0.5 ), c2( 0.5 ), c3( 0.5 ), c4( 0.5 );
-    c1[ 0 ] = 0.5;  c1[ 1 ] = 0.75;
-    c2[ 0 ] = 0.5;  c2[ 1 ] = 0.25;
-    c3[ 0 ] = 0.25; c3[ 1 ] = 0.5;
-    c4[ 0 ] = 0.35; c4[ 1 ] = 0.65;
-    const double r = 0.15;
-
-    // slotted cylinder
-    if( (x - c1).two_norm() < r )
-    {
-      if( (std::abs( x[ 0 ] - c1[ 0 ] ) >= 0.025) || (x[ 1 ] >= c1[ 1 ] + 0.1) )
-        return RangeType( 1.0 );
-      else
-        return RangeType( 0.0 );
-    }
-
-    // cone
-    if( (x - c2).two_norm() < r )
-      return RangeType( (r - (x - c2).two_norm()) / r );
-
-    // hump
-    if( (x - c3).two_norm() < r )
-      return RangeType((1.0 + std::cos( M_PI * (x - c3).two_norm() / r )) / 4.0 );
-
-    // default
-    return RangeType( 0.0 );
+    DomainType r(0.5);
+    return ((x-r).two_norm() < 0.25 ? RangeType( 1 ) : RangeType( 0 ) );
+    //return ((x-r).two_norm() < 0.5 ? RangeType( 1 ) : RangeType( 0 ) );
   }
 
   //! \copydoc ProblemData::endTime
   double endTime () const
   {
-    return 1.5708;
+    return 0.8;
   }
 
   //! \copydoc ProblemData::gridFile
   std::string gridFile ( const std::string &path, const int mpiSize ) const
   {
     return path + gridFile_;
   }
@@ -346,34 +197,48 @@
     case 3:
       problem_.reset( new TransportProblemData1< dimDomain >( problem ) );
       break;
     case 2:
     case 4:
       problem_.reset( new TransportProblemData2< dimDomain >( problem ) );
       break;
-    case 5:
-      problem_.reset( new SolidBodyRotation< dimDomain >( problem ) );
-      break;
     default:
       std::cerr << "Problem " << problem << " does not exists." << std::endl;
       std::abort();
     }
+
+    if( problem < 3 )
+    {
+      // set transport velocity
+      velocity_ = DomainType( 1.25 );
+    }
+    else
+    {
+      velocity_ = 0.0;
+      velocity_[ 0 ] = 1.25;
+    }
   }
 
   /** \brief obtain problem */
   const Problem &problem () const
   {
     return *problem_;
   }
 
   double fixedDt () const
   {
     return -1;
   }
 
+  /** \brief obtain the (constant) velocity for the transport problem */
+  const DomainType &velocity () const
+  {
+    return velocity_;
+  }
+
   /** \brief evaluate the numerical flux on an intersection
    *
    *  \param[in]   normal   scaled normal of the intersection
    *  \param[in]   time     current time
    *  \param[in]   xGlobal  evaluation point in global coordinates
    *  \param[in]   uLeft    value of the solution in the inside entity
    *  \param[in]   uRight   value of the solution in the outside entity
@@ -383,17 +248,15 @@
    */
   double numericalFlux ( const DomainType &normal,
                          const double time,
                          const DomainType &xGlobal,
                          const RangeType &uLeft, const RangeType &uRight,
                          RangeType &flux ) const
   {
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    const double upwind = normal * velocity;
+    const double upwind = normal * velocity();
     flux = upwind * (upwind > 0 ? uLeft : uRight);
     return std::abs( upwind );
   }
 
   /** \brief evaluate the numerical flux on a boundary
    *
    *  \param[in]   normal   scaled normal of the boundary
@@ -408,17 +271,15 @@
                         const double time,
                         const DomainType &xGlobal,
                         const RangeType& uLeft,
                         RangeType &flux ) const
   {
     // exact solution is u0(x-ta)
     DomainType x0( xGlobal );
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    x0.axpy( -time, velocity );
+    x0.axpy( -time, velocity_ );
     RangeType uRight = problem().boundaryValue( x0, time );
     return numericalFlux( normal, time, xGlobal, uLeft, uRight, flux );
   }
 
   /** \brief compute adaptation indicator at intersection
    *
    *  \param[in]   normal   scaled normal of the intersection
@@ -448,20 +309,19 @@
    */
   double boundaryIndicator ( const DomainType &normal,
                              const double time,
                              const DomainType &xGlobal,
                              const RangeType& uLeft) const
   {
     DomainType x0( xGlobal );
-    DomainType velocity( 0 );
-    problem().velocity( xGlobal, time, uLeft, velocity );
-    x0.axpy( -time, velocity );
+    x0.axpy( -time, velocity_ );
     return indicator( normal,time,xGlobal, uLeft, problem().boundaryValue(x0,time) );
   }
 
 protected:
-  TransportModel ( ) : problem_() {}
+  TransportModel ( ) : problem_(), velocity_(1) {}
 private:
   std::unique_ptr< Problem > problem_;
+  DomainType velocity_;
 }; // end class TransportModel
 
 #endif // PROBLEM_TRANSPORT_HH
```

### Comparing `dune-alugrid-2.9.0rc1/examples/testEfficiency/problem.hh` & `dune-alugrid-2.9.dev20220529/examples/testEfficiency/problem.hh`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,11 @@
 
   /**\brief return number of timestep to pass until load balancing is done again  */
   virtual int balanceStep() const { return 1; }
 
   /**\brief return maximal number of timesteps to run (for scaling experiment) */
   virtual unsigned int maxTimeSteps() const { return std::numeric_limits<unsigned int>::max(); }
 
-  virtual void velocity ( const DomainType &x, double time, const RangeType& u, DomainType& v ) const
-  {
-    v = 0;
-  }
-
 }; // end class ProblemData
 // Code moved to problem-transport.hh
 
 #endif // PROBLEM_HH
```

### Comparing `dune-alugrid-2.9.0rc1/lib/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/lib/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/lib/dunealugridam2cmake.lib` & `dune-alugrid-2.9.dev20220529/lib/dunealugridam2cmake.lib`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/adapt.cc` & `dune-alugrid-2.9.dev20220529/misc/examples/adapt.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/backuprestore.cc` & `dune-alugrid-2.9.dev20220529/misc/examples/backuprestore.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/cube.tetra` & `dune-alugrid-2.9.dev20220529/misc/examples/cube.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/example.cc` & `dune-alugrid-2.9.dev20220529/misc/examples/example.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/examplepara.cc` & `dune-alugrid-2.9.dev20220529/misc/examples/examplepara.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/loadlb.cc` & `dune-alugrid-2.9.dev20220529/misc/examples/loadlb.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/macrogrids/cube.tetra` & `dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/cube.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/macrogrids/cube_12.tetra` & `dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/cube_12.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/macrogrids/cube_48.tetra` & `dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/cube_48.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/macrogrids/cube_hc_3072.tetra` & `dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/cube_hc_3072.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/macrogrids/cube_hc_512.hexa` & `dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/cube_hc_512.hexa`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/macrogrids/macro.big` & `dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/macro.big`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/macrogrids/unstructured.tetra` & `dune-alugrid-2.9.dev20220529/misc/examples/macrogrids/unstructured.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/memdata_new.hexa` & `dune-alugrid-2.9.dev20220529/misc/examples/memdata_new.hexa`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/memdata_new.tetra` & `dune-alugrid-2.9.dev20220529/misc/examples/memdata_new.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/memdata_old.hexa` & `dune-alugrid-2.9.dev20220529/misc/examples/memdata_old.hexa`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/memdata_old.tetra` & `dune-alugrid-2.9.dev20220529/misc/examples/memdata_old.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/memdata_oldpara.hexa` & `dune-alugrid-2.9.dev20220529/misc/examples/memdata_oldpara.hexa`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/memdata_oldpara.tetra` & `dune-alugrid-2.9.dev20220529/misc/examples/memdata_oldpara.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/periodic.cc` & `dune-alugrid-2.9.dev20220529/misc/examples/periodic.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/sizes.cc` & `dune-alugrid-2.9.dev20220529/misc/examples/sizes.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/timer.hh` & `dune-alugrid-2.9.dev20220529/misc/examples/timer.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/examples/twist.cc` & `dune-alugrid-2.9.dev20220529/misc/examples/twist.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/macrogrids/cube.tetra` & `dune-alugrid-2.9.dev20220529/misc/macrogrids/cube.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/macrogrids/cube_12.tetra` & `dune-alugrid-2.9.dev20220529/misc/macrogrids/cube_12.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/macrogrids/cube_48.tetra` & `dune-alugrid-2.9.dev20220529/misc/macrogrids/cube_48.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/macrogrids/cube_hc_3072.tetra` & `dune-alugrid-2.9.dev20220529/misc/macrogrids/cube_hc_3072.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/macrogrids/cube_hc_512.hexa` & `dune-alugrid-2.9.dev20220529/misc/macrogrids/cube_hc_512.hexa`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/macrogrids/macro.big` & `dune-alugrid-2.9.dev20220529/misc/macrogrids/macro.big`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/macrogrids/unstructured.tetra` & `dune-alugrid-2.9.dev20220529/misc/macrogrids/unstructured.tetra`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/misc/versioncheck/alugridversion.cc` & `dune-alugrid-2.9.dev20220529/misc/versioncheck/alugridversion.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/pyproject.toml` & `dune-alugrid-2.9.dev20220529/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 #
 # This is uses the `Python-Requires` field in the `dune.modules` file to
 # populate the `requires` entry. Additional packages needed for the package
 # build should be added in the `dune.modules`. These packages will then also be
 # included in the package install from source.
 #
 [build-system]
-requires = ['cmake>=3.13', 'dune-grid<=v2.9.0rc1', 'ninja', 'pip', 'requests', 'scikit-build', 'setuptools', 'wheel']
+requires = ['cmake>=3.13', 'dune-grid<=2.9.dev20220529', 'ninja', 'pip', 'requests', 'scikit-build', 'setuptools', 'wheel']
 build-backend = 'setuptools.build_meta'
```

### Comparing `dune-alugrid-2.9.0rc1/python/dune/alugrid/_grids.py` & `dune-alugrid-2.9.dev20220529/python/dune/alugrid/_grids.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,56 +87,42 @@
     if not (2 <= dimgrid and dimgrid <= dimworld):
         raise KeyError("Parameter error in ALUGrid with dimgrid=" + str(dimgrid) + ": dimgrid has to be either 2 or 3")
     if not (2 <= dimworld and dimworld <= 3):
         raise KeyError("Parameter error in ALUGrid with dimworld=" + str(dimworld) + ": dimworld has to be either 2 or 3")
     if refinement=="Dune::conforming" and elementType=="Dune::cube":
         raise KeyError("Parameter error in ALUGrid with refinement=" + refinement + " and type=" + elementType + ": conforming refinement is only available with simplex element type")
 
-    typeName = "Dune::ALUGrid< " + str(dimgrid) + ", " + str(dimworld) + ", Dune::" + elementType
-    if refinement is not None:
-        assert refinement == 'conforming' or refinement == 'nonconforming', "Refinement should be 'conforming' or 'nonconforming' if selected."
-        typename += ", Dune::" + refinement
-
+    typeName = "Dune::ALUGrid< " + str(dimgrid) + ", " + str(dimworld) + ", Dune::" + elementType + ", Dune::" + refinement
     # if serial flag is true serial version is forced.
     if serial:
         typeName += ", Dune::ALUGridNoComm"
 
     typeName += " >"
     includes = ["dune/alugrid/grid.hh", "dune/alugrid/dgf.hh"]
     gridModule = module(includes, typeName)
 
     if comm is not None:
         raise Exception("Passing communicator to grid construction is not yet implemented in Python bindings of dune-grid")
         # return gridModule.LeafGrid(gridModule.reader(constructor, comm))
 
     gridView = gridModule.LeafGrid(gridModule.reader(constructor))
-
-    # in case of a carteisan domain store if old or new boundary ids was used
-    # this can be removed in later version - it is only used in dune-fem
-    # to give a warning that the boundary ids for the cartesian domains have changed
-    try:
-        gridView.hierarchicalGrid._cartesianConstructionWithIds = constructor.boundaryWasSet
-    except AttributeError:
-        pass
     return gridView
 
 def aluConformGrid(*args, **kwargs):
-    # enable conforming refinement for duration of grid creation
-    refVar = ALUGridEnvVar('ALUGRID_CONFORMING_REFINEMENT', 1)
     aluConformGrid.__doc__ = aluGrid.__doc__
-    return aluGrid(*args, **kwargs, elementType="simplex")
+    return aluGrid(*args, **kwargs, elementType="simplex", refinement="conforming")
 
 def aluCubeGrid(*args, **kwargs):
     aluCubeGrid.__doc__ = aluGrid.__doc__
-    return aluGrid(*args, **kwargs, elementType="cube")
+    return aluGrid(*args, **kwargs, elementType="cube", refinement="nonconforming")
 
 
 def aluSimplexGrid(*args, **kwargs):
     aluSimplexGrid.__doc__ = aluGrid.__doc__
-    return aluGrid(*args, **kwargs, elementType="simplex")
+    return aluGrid(*args, **kwargs, elementType="simplex", refinement="nonconforming")
 
 grid_registry = {
         "ALU"        : aluGrid,
         "ALUConform" : aluConformGrid,
         "ALUCube" :    aluCubeGrid,
         "ALUSimplex" : aluSimplexGrid,
     }
```

### Comparing `dune-alugrid-2.9.0rc1/python/dune_alugrid.egg-info/PKG-INFO` & `dune-alugrid-2.9.dev20220529/python/dune_alugrid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-alugrid
-Version: 2.9.0rc1
+Version: 2.9.dev20220529
 Summary: Module providing the DUNE grid interface for unstructured simplicial and cube grids in 2 and 3 space dimensions
 Home-page: https://gitlab.dune-project.org/extensions/dune-alugrid
 Author: Robert Kloefkorn, Martin Alkaemper, Andreas Dedner and Martin Nolte
 Author-email: dune-devel@lists.dune-project.org
 License: UNKNOWN
 Description: DUNE-ALUGrid
         ============
@@ -61,15 +61,15 @@
         [2]: http://www.dune-project.org/doc/installation
         [3]: http://journals.ub.uni-heidelberg.de/index.php/ans/article/view/23252
         [4]: http://www.cs.sandia.gov/Zoltan/
         [5]: https://gitlab.dune-project.org/extensions/dune-alugrid/blob/master/COPYING
         [6]: https://gitlab.dune-project.org/extensions/dune-alugrid/blob/master/doc/dunealugrid.bib
         
         
-        git-2788e7cc0e8b9bf32f589656a94323342045a4b5
+        git-9fede971172df042602dab6c13bd1ead94419ac4
         
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
```

### Comparing `dune-alugrid-2.9.0rc1/python/dune_alugrid.egg-info/SOURCES.txt` & `dune-alugrid-2.9.dev20220529/python/dune_alugrid.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -214,17 +214,14 @@
 dune/alugrid/test/dgf/cube-testgrid-2-2.dgf
 dune/alugrid/test/dgf/cube-testgrid-2-3.dgf
 dune/alugrid/test/dgf/cubedsphere2d.dgf
 dune/alugrid/test/dgf/grid2d_str1d.dgf
 dune/alugrid/test/dgf/half-circle.dgf
 dune/alugrid/test/dgf/periodic2.dgf
 dune/alugrid/test/dgf/periodic3.dgf
-dune/alugrid/test/dgf/periodic_2quads.dgf
-dune/alugrid/test/dgf/periodic_unstructured.dgf
-dune/alugrid/test/dgf/periodic_unstructured_fine.dgf
 dune/alugrid/test/dgf/simplex-testgrid-2-2.dgf
 dune/alugrid/test/dgf/simplex-testgrid-2-3-noproj.dgf
 dune/alugrid/test/dgf/simplex-testgrid-2-3.dgf
 dune/alugrid/test/dgf/simplex-testgrid-3-3.dgf
 dune/alugrid/test/dgf/sphere.dgf
 dune/alugrid/test/gmsh/CMakeLists.txt
 dune/alugrid/test/gmsh/circle2ndorder.msh
```

### Comparing `dune-alugrid-2.9.0rc1/scripts/build-dune-alugrid.sh` & `dune-alugrid-2.9.dev20220529/scripts/build-dune-alugrid.sh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/utils/bisection-compatibility/CMakeLists.txt` & `dune-alugrid-2.9.dev20220529/utils/bisection-compatibility/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/utils/bisection-compatibility/estimate-closure.cc` & `dune-alugrid-2.9.dev20220529/utils/bisection-compatibility/estimate-closure.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/utils/bisection-compatibility/test-compatibility.cc` & `dune-alugrid-2.9.dev20220529/utils/bisection-compatibility/test-compatibility.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/utils/convert-macrogrid/dgfparser.hh` & `dune-alugrid-2.9.dev20220529/utils/convert-macrogrid/dgfparser.hh`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/utils/convert-macrogrid/main.cc` & `dune-alugrid-2.9.dev20220529/utils/convert-macrogrid/main.cc`

 * *Files identical despite different names*

### Comparing `dune-alugrid-2.9.0rc1/utils/convert-macrogrid/partition.hh` & `dune-alugrid-2.9.dev20220529/utils/convert-macrogrid/partition.hh`

 * *Files identical despite different names*

