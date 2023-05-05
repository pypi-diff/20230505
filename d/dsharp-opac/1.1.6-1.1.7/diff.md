# Comparing `tmp/dsharp_opac-1.1.6.tar.gz` & `tmp/dsharp_opac-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dsharp_opac-1.1.6.tar", last modified: Thu Nov 19 08:50:33 2020, max compression
+gzip compressed data, was "dsharp_opac-1.1.7.tar", last modified: Fri May  5 08:54:31 2023, max compression
```

## Comparing `dsharp_opac-1.1.6.tar` & `dsharp_opac-1.1.7.tar`

### file list

```diff
@@ -1,117 +1,145 @@
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.159855 dsharp_opac-1.1.6/
--rw-r--r--   0 birnstiel   (501) staff       (20)      191 2019-02-18 12:52:41.000000 dsharp_opac-1.1.6/.gitignore
--rw-r--r--   0 birnstiel   (501) staff       (20)    35140 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/LICENSE
--rw-r--r--   0 birnstiel   (501) staff       (20)      224 2019-02-18 12:53:11.000000 dsharp_opac-1.1.6/MANIFEST.in
--rw-r--r--   0 birnstiel   (501) staff       (20)     2842 2020-11-19 08:50:33.159448 dsharp_opac-1.1.6/PKG-INFO
--rw-r--r--   0 birnstiel   (501) staff       (20)     2220 2019-03-15 10:56:48.000000 dsharp_opac-1.1.6/README.md
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:32.965770 dsharp_opac-1.1.6/dsharp_opac/
--rw-r--r--   0 birnstiel   (501) staff       (20)     2071 2020-11-19 08:48:17.000000 dsharp_opac-1.1.6/dsharp_opac/__init__.py
--rw-r--r--   0 birnstiel   (501) staff       (20)    11792 2020-11-19 08:45:02.000000 dsharp_opac-1.1.6/dsharp_opac/bhmie_fortran.f90
--rw-r--r--   0 birnstiel   (501) staff       (20)     6931 2019-02-20 21:12:46.000000 dsharp_opac-1.1.6/dsharp_opac/bhmie_python.py
--rw-r--r--   0 birnstiel   (501) staff       (20)      414 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/calldraine.f90
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.007510 dsharp_opac-1.1.6/dsharp_opac/data/
--rw-r--r--   0 birnstiel   (501) staff       (20)     2184 2019-07-30 08:34:28.000000 dsharp_opac-1.1.6/dsharp_opac/data/Kataoka2014-Fig2b-1e-5cm.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     2093 2019-07-30 08:45:33.000000 dsharp_opac-1.1.6/dsharp_opac/data/Kataoka2014-Fig2d-1e-5cm.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     1301 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/data/andrews2009.dat
--rw-r--r--   0 birnstiel   (501) staff       (20)   803630 2019-02-04 20:34:40.000000 dsharp_opac-1.1.6/dsharp_opac/data/default_opacities.npz
--rw-r--r--   0 birnstiel   (501) staff       (20)   803274 2019-02-19 21:16:44.000000 dsharp_opac-1.1.6/dsharp_opac/data/default_opacities_extrapol.npz
--rw-r--r--   0 birnstiel   (501) staff       (20)   853812 2019-02-05 22:29:36.000000 dsharp_opac-1.1.6/dsharp_opac/data/default_opacities_smooth.npz
--rw-r--r--   0 birnstiel   (501) staff       (20)   803316 2019-02-04 20:37:06.000000 dsharp_opac-1.1.6/dsharp_opac/data/icefree_opacities.npz
--rw-r--r--   0 birnstiel   (501) staff       (20)   853427 2019-02-05 22:37:57.000000 dsharp_opac-1.1.6/dsharp_opac/data/icefree_opacities_smooth.npz
--rw-r--r--   0 birnstiel   (501) staff       (20)     2260 2018-12-07 10:13:45.000000 dsharp_opac-1.1.6/dsharp_opac/data/kappa_D01_T100K_p3.5_amax1mm.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)    15708 2018-12-07 10:13:45.000000 dsharp_opac-1.1.6/dsharp_opac/data/kataoka_mix.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)    40865 2020-03-04 15:31:44.000000 dsharp_opac-1.1.6/dsharp_opac/data/ricci_compact.npz
--rwxr-xr-x   0 birnstiel   (501) staff       (20)    89650 2020-11-19 08:47:08.000000 dsharp_opac-1.1.6/dsharp_opac/dsharp_opac.py
--rw-r--r--   0 birnstiel   (501) staff       (20)    25142 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/fit_module.f90
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:32.954657 dsharp_opac-1.1.6/dsharp_opac/optical_constants/
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.009273 dsharp_opac-1.1.6/dsharp_opac/optical_constants/draine/
--rw-r--r--   0 birnstiel   (501) staff       (20)      144 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/draine/.gitignore
--rw-r--r--   0 birnstiel   (501) staff       (20)      827 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/draine/links.json
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.010393 dsharp_opac-1.1.6/dsharp_opac/optical_constants/henning/
--rw-r--r--   0 birnstiel   (501) staff       (20)        6 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/henning/.gitignore
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.011032 dsharp_opac-1.1.6/dsharp_opac/optical_constants/henning/new/
--rw-r--r--   0 birnstiel   (501) staff       (20)     1058 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/henning/new/links.json
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.012139 dsharp_opac-1.1.6/dsharp_opac/optical_constants/henning/old/
--rw-r--r--   0 birnstiel   (501) staff       (20)      599 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/henning/old/links.json
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.026257 dsharp_opac-1.1.6/dsharp_opac/optical_constants/jaeger/
--rw-r--r--   0 birnstiel   (501) staff       (20)       45 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/jaeger/.gitignore
--rw-r--r--   0 birnstiel   (501) staff       (20)      425 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/jaeger/links.json
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.033607 dsharp_opac-1.1.6/dsharp_opac/optical_constants/luca/
--rw-r--r--   0 birnstiel   (501) staff       (20)    75634 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/luca/H2Oice_Warren.dat
--rw-r--r--   0 birnstiel   (501) staff       (20)   132169 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/luca/aC_ACH2_Zubko.dat
--rw-r--r--   0 birnstiel   (501) staff       (20)   132175 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/luca/silicate.dat
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.072559 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/
--rw-r--r--   0 birnstiel   (501) staff       (20)      580 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-iron-k.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)      568 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-iron-n.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-iron.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     1331 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-olivine-k.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     1078 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-olivine-n.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-olivine.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     1656 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-organics-k.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     1168 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-organics-n.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-organics.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     1705 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-k.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     1060 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-n.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)      666 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-troilite-k.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)      505 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-troilite-n.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-troilite.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)     2009 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-waterice-k.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     1425 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-waterice-n.csv
--rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-waterice.lnk
--rw-r--r--   0 birnstiel   (501) staff       (20)      887 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/make_lnk.py
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.090446 dsharp_opac-1.1.6/dsharp_opac/optical_constants/preibisch/
--rw-r--r--   0 birnstiel   (501) staff       (20)       23 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/preibisch/.gitignore
--rw-r--r--   0 birnstiel   (501) staff       (20)      215 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/preibisch/links.json
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.092759 dsharp_opac-1.1.6/dsharp_opac/optical_constants/segelstein_water/
--rw-r--r--   0 birnstiel   (501) staff       (20)       15 2019-03-14 19:07:11.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/segelstein_water/.gitignore
--rw-r--r--   0 birnstiel   (501) staff       (20)      137 2019-03-14 19:07:12.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/segelstein_water/links.json
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.103676 dsharp_opac-1.1.6/dsharp_opac/optical_constants/testfiles_ricci/
--rw-r--r--   0 birnstiel   (501) staff       (20)      882 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/testfiles_ricci/beta.dat
--rw-r--r--   0 birnstiel   (501) staff       (20)  2351704 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/testfiles_ricci/d_test_vacuum30.dust
--rw-r--r--   0 birnstiel   (501) staff       (20)    10382 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/testfiles_ricci/dust_opacities.16
--rw-r--r--   0 birnstiel   (501) staff       (20)      509 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/testfiles_ricci/kappa.dat
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.109348 dsharp_opac-1.1.6/dsharp_opac/optical_constants/warren/
--rw-r--r--   0 birnstiel   (501) staff       (20)       24 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/warren/.gitignore
--rw-r--r--   0 birnstiel   (501) staff       (20)      122 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/warren/links.json
--rw-r--r--   0 birnstiel   (501) staff       (20)    13224 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/warren/warren_1984.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)     4525 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/warren/warren_1984_all_temps.txt
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.125043 dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/
--rw-r--r--   0 birnstiel   (501) staff       (20)     1052 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/zubko_E_ACH2.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)     1097 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/zubko_E_BE.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)      812 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/zubko_k_ACH2.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)      731 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/zubko_k_BE.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)      818 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/zubko_n_ACH2.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)      750 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/zubko_n_BE.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)   915276 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/zubko_ocr.pdf
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:32.969301 dsharp_opac-1.1.6/dsharp_opac.egg-info/
--rw-r--r--   0 birnstiel   (501) staff       (20)     2842 2020-11-19 08:50:32.000000 dsharp_opac-1.1.6/dsharp_opac.egg-info/PKG-INFO
--rw-r--r--   0 birnstiel   (501) staff       (20)     4164 2020-11-19 08:50:32.000000 dsharp_opac-1.1.6/dsharp_opac.egg-info/SOURCES.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)        1 2020-11-19 08:50:32.000000 dsharp_opac-1.1.6/dsharp_opac.egg-info/dependency_links.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)        1 2020-11-19 08:50:32.000000 dsharp_opac-1.1.6/dsharp_opac.egg-info/not-zip-safe
--rw-r--r--   0 birnstiel   (501) staff       (20)       38 2020-11-19 08:50:32.000000 dsharp_opac-1.1.6/dsharp_opac.egg-info/requires.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)       12 2020-11-19 08:50:32.000000 dsharp_opac-1.1.6/dsharp_opac.egg-info/top_level.txt
--rw-r--r--   0 birnstiel   (501) staff       (20)      240 2019-03-15 12:24:14.000000 dsharp_opac-1.1.6/environment.yml
-drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2020-11-19 08:50:33.158356 dsharp_opac-1.1.6/notebooks/
--rw-r--r--   0 birnstiel   (501) staff       (20)    18363 2019-02-20 21:22:37.000000 dsharp_opac-1.1.6/notebooks/AppendixB.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     4632 2019-02-20 21:22:37.000000 dsharp_opac-1.1.6/notebooks/Figure1.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     1719 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/notebooks/Figure2.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     2339 2019-02-20 21:22:37.000000 dsharp_opac-1.1.6/notebooks/Figure3.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     3963 2019-07-30 09:16:58.000000 dsharp_opac-1.1.6/notebooks/Figure4.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     6886 2019-02-20 21:22:37.000000 dsharp_opac-1.1.6/notebooks/Figure56.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     4105 2019-02-20 21:22:37.000000 dsharp_opac-1.1.6/notebooks/Figure7.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)    11407 2019-02-20 21:22:37.000000 dsharp_opac-1.1.6/notebooks/Figure8.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     3854 2019-02-20 21:22:37.000000 dsharp_opac-1.1.6/notebooks/Figure9.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     5874 2018-12-07 10:13:44.000000 dsharp_opac-1.1.6/notebooks/aux_functions.py
--rw-r--r--   0 birnstiel   (501) staff       (20)     5917 2020-06-08 18:32:14.000000 dsharp_opac-1.1.6/notebooks/dsharp_porosity.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)      394 2018-12-10 20:04:26.000000 dsharp_opac-1.1.6/notebooks/header.py
--rw-r--r--   0 birnstiel   (501) staff       (20)     1514 2018-12-07 10:13:45.000000 dsharp_opac-1.1.6/notebooks/index.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)    12688 2019-02-20 20:53:26.000000 dsharp_opac-1.1.6/notebooks/opac_widget.py
--rw-r--r--   0 birnstiel   (501) staff       (20)  1816292 2019-07-26 10:44:58.000000 dsharp_opac-1.1.6/notebooks/opacity_examples.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)   609690 2019-02-20 19:44:13.000000 dsharp_opac-1.1.6/notebooks/opacity_package_tests.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)    50797 2020-03-31 07:16:03.000000 dsharp_opac-1.1.6/notebooks/polarization_fraction.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     8660 2020-03-31 07:18:07.000000 dsharp_opac-1.1.6/notebooks/porosity.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)     6503 2019-07-26 10:45:36.000000 dsharp_opac-1.1.6/notebooks/scattering_phase_functions.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)    16618 2020-06-08 18:18:17.000000 dsharp_opac-1.1.6/notebooks/smoothed_opacities.ipynb
--rw-r--r--   0 birnstiel   (501) staff       (20)       38 2020-11-19 08:50:33.159968 dsharp_opac-1.1.6/setup.cfg
--rw-r--r--   0 birnstiel   (501) staff       (20)     2049 2020-11-11 14:25:34.000000 dsharp_opac-1.1.6/setup.py
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.638718 dsharp_opac-1.1.7/
+-rw-r--r--   0 birnstiel   (501) staff       (20)    35140 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/LICENSE
+-rw-r--r--   0 birnstiel   (501) staff       (20)      224 2019-02-18 12:53:11.000000 dsharp_opac-1.1.7/MANIFEST.in
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2537 2023-05-05 08:54:31.638575 dsharp_opac-1.1.7/PKG-INFO
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2220 2019-03-15 10:56:48.000000 dsharp_opac-1.1.7/README.md
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.589046 dsharp_opac-1.1.7/dsharp_opac/
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2133 2023-05-05 08:53:32.000000 dsharp_opac-1.1.7/dsharp_opac/__init__.py
+-rw-r--r--   0 birnstiel   (501) staff       (20)    11792 2020-11-19 08:45:02.000000 dsharp_opac-1.1.7/dsharp_opac/bhmie_fortran.f90
+-rw-r--r--   0 birnstiel   (501) staff       (20)     6931 2019-02-20 21:12:46.000000 dsharp_opac-1.1.7/dsharp_opac/bhmie_python.py
+-rw-r--r--   0 birnstiel   (501) staff       (20)      414 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/calldraine.f90
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.602161 dsharp_opac-1.1.7/dsharp_opac/data/
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2184 2019-07-30 08:34:28.000000 dsharp_opac-1.1.7/dsharp_opac/data/Kataoka2014-Fig2b-1e-5cm.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2093 2019-07-30 08:45:33.000000 dsharp_opac-1.1.7/dsharp_opac/data/Kataoka2014-Fig2d-1e-5cm.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)     1301 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/data/andrews2009.dat
+-rw-r--r--   0 birnstiel   (501) staff       (20)   803630 2019-02-04 20:34:40.000000 dsharp_opac-1.1.7/dsharp_opac/data/default_opacities.npz
+-rw-r--r--   0 birnstiel   (501) staff       (20)   803274 2019-02-19 21:16:44.000000 dsharp_opac-1.1.7/dsharp_opac/data/default_opacities_extrapol.npz
+-rw-r--r--   0 birnstiel   (501) staff       (20)   853812 2019-02-05 22:29:36.000000 dsharp_opac-1.1.7/dsharp_opac/data/default_opacities_smooth.npz
+-rw-r--r--   0 birnstiel   (501) staff       (20)   843960 2023-03-22 13:18:30.000000 dsharp_opac-1.1.7/dsharp_opac/data/diana.npz
+-rw-r--r--   0 birnstiel   (501) staff       (20)   803316 2019-02-04 20:37:06.000000 dsharp_opac-1.1.7/dsharp_opac/data/icefree_opacities.npz
+-rw-r--r--   0 birnstiel   (501) staff       (20)   853427 2019-02-05 22:37:57.000000 dsharp_opac-1.1.7/dsharp_opac/data/icefree_opacities_smooth.npz
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2260 2018-12-07 10:13:45.000000 dsharp_opac-1.1.7/dsharp_opac/data/kappa_D01_T100K_p3.5_amax1mm.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)    15708 2018-12-07 10:13:45.000000 dsharp_opac-1.1.7/dsharp_opac/data/kataoka_mix.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)  2143594 2021-08-04 15:23:22.000000 dsharp_opac-1.1.7/dsharp_opac/data/ricci_compact.npz
+-rwxr-xr-x   0 birnstiel   (501) staff       (20)    98010 2023-04-18 14:25:51.000000 dsharp_opac-1.1.7/dsharp_opac/dsharp_opac.py
+-rw-r--r--   0 birnstiel   (501) staff       (20)    25142 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/fit_module.f90
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.586661 dsharp_opac-1.1.7/dsharp_opac/optical_constants/
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.609582 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/
+-rw-r--r--   0 birnstiel   (501) staff       (20)      144 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/.gitignore
+-rw-r--r--   0 birnstiel   (501) staff       (20)    22981 2022-02-15 11:30:37.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/callindex.out_CpaD03_0.01
+-rw-r--r--   0 birnstiel   (501) staff       (20)    22981 2022-02-15 11:30:39.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/callindex.out_CpaD03_0.10
+-rw-r--r--   0 birnstiel   (501) staff       (20)    22804 2022-02-15 11:30:40.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/callindex.out_CpeD03_0.01
+-rw-r--r--   0 birnstiel   (501) staff       (20)    22804 2022-02-15 11:30:41.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/callindex.out_CpeD03_0.10
+-rw-r--r--   0 birnstiel   (501) staff       (20)    49590 2022-02-15 11:30:35.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/callindex.out_silD03
+-rw-r--r--   0 birnstiel   (501) staff       (20)    62740 2022-02-15 11:30:34.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/eps_Sil
+-rw-r--r--   0 birnstiel   (501) staff       (20)    70053 2022-02-15 11:30:36.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/eps_suvSil
+-rw-r--r--   0 birnstiel   (501) staff       (20)      827 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/links.json
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.609836 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/
+-rw-r--r--   0 birnstiel   (501) staff       (20)        6 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/.gitignore
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.611465 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/
+-rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:43.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/ironk.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     1058 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/links.json
+-rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:42.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/olivinenewk.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:43.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/olmg60k.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:42.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/olmg70k.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/organicsk.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:43.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/pyrmg100k.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:43.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/pyrmg60k.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:43.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/pyrmg70k.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/troilitek.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     4181 2022-02-15 11:30:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/watericek.lnk
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.612390 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2960 2022-02-15 11:30:41.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/iron.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)      599 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/links.json
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2960 2022-02-15 11:30:41.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/olivine.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2960 2022-02-15 11:30:42.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/organics.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2960 2022-02-15 11:30:41.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/orthopyr.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2960 2022-02-15 11:30:42.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/troilite.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2960 2022-02-15 11:30:42.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/waterice.lnk
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.614068 dsharp_opac-1.1.7/dsharp_opac/optical_constants/jaeger/
+-rw-r--r--   0 birnstiel   (501) staff       (20)       45 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/jaeger/.gitignore
+-rw-r--r--   0 birnstiel   (501) staff       (20)     3796 2022-07-22 11:56:08.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/jaeger/cel1000.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     3588 2022-07-22 11:56:09.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/jaeger/cel400.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     3536 2022-07-22 11:56:09.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/jaeger/cel600.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     3692 2022-07-22 11:56:09.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/jaeger/cel800.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)      425 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/jaeger/links.json
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.615168 dsharp_opac-1.1.7/dsharp_opac/optical_constants/luca/
+-rw-r--r--   0 birnstiel   (501) staff       (20)    75634 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/luca/H2Oice_Warren.dat
+-rw-r--r--   0 birnstiel   (501) staff       (20)   132169 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/luca/aC_ACH2_Zubko.dat
+-rw-r--r--   0 birnstiel   (501) staff       (20)   132175 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/luca/silicate.dat
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.618605 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/
+-rw-r--r--   0 birnstiel   (501) staff       (20)      580 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-iron-k.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)      568 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-iron-n.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-iron.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     1331 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-olivine-k.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)     1078 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-olivine-n.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-olivine.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     1656 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-organics-k.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)     1168 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-organics-n.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-organics.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     1705 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-k.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)     1060 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-n.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)      666 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-troilite-k.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)      505 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-troilite-n.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-troilite.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2009 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-waterice-k.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)     1425 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-waterice-n.csv
+-rw-r--r--   0 birnstiel   (501) staff       (20)     7500 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-waterice.lnk
+-rw-r--r--   0 birnstiel   (501) staff       (20)      887 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/make_lnk.py
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.618907 dsharp_opac-1.1.7/dsharp_opac/optical_constants/preibisch/
+-rw-r--r--   0 birnstiel   (501) staff       (20)       23 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/preibisch/.gitignore
+-rw-r--r--   0 birnstiel   (501) staff       (20)      215 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/preibisch/links.json
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.619202 dsharp_opac-1.1.7/dsharp_opac/optical_constants/segelstein_water/
+-rw-r--r--   0 birnstiel   (501) staff       (20)       15 2019-03-14 19:07:11.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/segelstein_water/.gitignore
+-rw-r--r--   0 birnstiel   (501) staff       (20)      137 2019-03-14 19:07:12.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/segelstein_water/links.json
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.621999 dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/
+-rw-r--r--   0 birnstiel   (501) staff       (20)      882 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/beta.dat
+-rw-r--r--   0 birnstiel   (501) staff       (20)  2351704 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/d_test_vacuum30.dust
+-rw-r--r--   0 birnstiel   (501) staff       (20)    10382 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/dust_opacities.16
+-rw-r--r--   0 birnstiel   (501) staff       (20)      509 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/kappa.dat
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.625852 dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/
+-rw-r--r--   0 birnstiel   (501) staff       (20)       24 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/.gitignore
+-rw-r--r--   0 birnstiel   (501) staff       (20)    16514 2022-02-15 11:30:33.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/IOP_2008_ASCIItable.dat
+-rw-r--r--   0 birnstiel   (501) staff       (20)      122 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/links.json
+-rw-r--r--   0 birnstiel   (501) staff       (20)    13224 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/warren_1984.txt
+-rw-r--r--   0 birnstiel   (501) staff       (20)     4525 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/warren_1984_all_temps.txt
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.626903 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/
+-rw-r--r--   0 birnstiel   (501) staff       (20)     1052 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_E_ACH2.txt
+-rw-r--r--   0 birnstiel   (501) staff       (20)     1097 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_E_BE.txt
+-rw-r--r--   0 birnstiel   (501) staff       (20)      812 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_k_ACH2.txt
+-rw-r--r--   0 birnstiel   (501) staff       (20)      731 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_k_BE.txt
+-rw-r--r--   0 birnstiel   (501) staff       (20)      818 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_n_ACH2.txt
+-rw-r--r--   0 birnstiel   (501) staff       (20)      750 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_n_BE.txt
+-rw-r--r--   0 birnstiel   (501) staff       (20)   915276 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_ocr.pdf
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.590459 dsharp_opac-1.1.7/dsharp_opac.egg-info/
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2537 2023-05-05 08:54:31.000000 dsharp_opac-1.1.7/dsharp_opac.egg-info/PKG-INFO
+-rw-r--r--   0 birnstiel   (501) staff       (20)     5739 2023-05-05 08:54:31.000000 dsharp_opac-1.1.7/dsharp_opac.egg-info/SOURCES.txt
+-rw-r--r--   0 birnstiel   (501) staff       (20)        1 2023-05-05 08:54:31.000000 dsharp_opac-1.1.7/dsharp_opac.egg-info/dependency_links.txt
+-rw-r--r--   0 birnstiel   (501) staff       (20)        1 2022-02-09 13:20:56.000000 dsharp_opac-1.1.7/dsharp_opac.egg-info/not-zip-safe
+-rw-r--r--   0 birnstiel   (501) staff       (20)       38 2023-05-05 08:54:31.000000 dsharp_opac-1.1.7/dsharp_opac.egg-info/requires.txt
+-rw-r--r--   0 birnstiel   (501) staff       (20)       12 2023-05-05 08:54:31.000000 dsharp_opac-1.1.7/dsharp_opac.egg-info/top_level.txt
+drwxr-xr-x   0 birnstiel   (501) staff       (20)        0 2023-05-05 08:54:31.638287 dsharp_opac-1.1.7/notebooks/
+-rw-r--r--   0 birnstiel   (501) staff       (20)    18210 2023-01-27 08:30:29.000000 dsharp_opac-1.1.7/notebooks/AppendixB.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)     4632 2019-02-20 21:22:37.000000 dsharp_opac-1.1.7/notebooks/Figure1.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)     1719 2018-12-07 10:13:44.000000 dsharp_opac-1.1.7/notebooks/Figure2.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2339 2019-02-20 21:22:37.000000 dsharp_opac-1.1.7/notebooks/Figure3.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)     3963 2022-06-13 07:04:00.000000 dsharp_opac-1.1.7/notebooks/Figure4.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)     6886 2023-01-27 08:24:20.000000 dsharp_opac-1.1.7/notebooks/Figure56.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)     4105 2019-02-20 21:22:37.000000 dsharp_opac-1.1.7/notebooks/Figure7.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)    11439 2023-03-30 09:03:24.000000 dsharp_opac-1.1.7/notebooks/Figure8.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)     3854 2019-02-20 21:22:37.000000 dsharp_opac-1.1.7/notebooks/Figure9.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)     5933 2020-12-01 11:32:58.000000 dsharp_opac-1.1.7/notebooks/aux_functions.py
+-rw-r--r--   0 birnstiel   (501) staff       (20)     5917 2020-06-08 18:32:14.000000 dsharp_opac-1.1.7/notebooks/dsharp_porosity.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)      394 2018-12-10 20:04:26.000000 dsharp_opac-1.1.7/notebooks/header.py
+-rw-r--r--   0 birnstiel   (501) staff       (20)     1514 2018-12-07 10:13:45.000000 dsharp_opac-1.1.7/notebooks/index.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)    12688 2019-02-20 20:53:26.000000 dsharp_opac-1.1.7/notebooks/opac_widget.py
+-rw-r--r--   0 birnstiel   (501) staff       (20)  1816292 2019-07-26 10:44:58.000000 dsharp_opac-1.1.7/notebooks/opacity_examples.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)   609690 2019-02-20 19:44:13.000000 dsharp_opac-1.1.7/notebooks/opacity_package_tests.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)    50797 2020-03-31 07:16:03.000000 dsharp_opac-1.1.7/notebooks/polarization_fraction.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)     8660 2020-03-31 07:18:07.000000 dsharp_opac-1.1.7/notebooks/porosity.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)     7303 2023-03-30 09:07:49.000000 dsharp_opac-1.1.7/notebooks/rosseland_mean_opacities.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)     6503 2019-07-26 10:45:36.000000 dsharp_opac-1.1.7/notebooks/scattering_phase_functions.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)    16618 2020-06-08 18:18:17.000000 dsharp_opac-1.1.7/notebooks/smoothed_opacities.ipynb
+-rw-r--r--   0 birnstiel   (501) staff       (20)       38 2023-05-05 08:54:31.638769 dsharp_opac-1.1.7/setup.cfg
+-rw-r--r--   0 birnstiel   (501) staff       (20)     2049 2020-11-11 14:25:34.000000 dsharp_opac-1.1.7/setup.py
```

### Comparing `dsharp_opac-1.1.6/LICENSE` & `dsharp_opac-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/PKG-INFO` & `dsharp_opac-1.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: dsharp_opac
-Version: 1.1.6
+Version: 1.1.7
 Summary: python routines to calculate mie opacities
 Home-page: https://github.com/birnstiel/dsharp_opac
 Author: Til Birnstiel & DSHARP collaboration
 Author-email: til.birnstiel@lmu.de
 License: GPLv3
-Description: [![Codacy Badge](https://api.codacy.com/project/badge/Grade/b04c8f86251749ac92361c6431103a08)](https://app.codacy.com/app/birnstiel/dsharp_opac?utm_source=github.com&utm_medium=referral&utm_content=birnstiel/dsharp_opac&utm_campaign=Badge_Grade_Dashboard)
-        [![DOI](https://zenodo.org/badge/137751482.svg)](https://zenodo.org/badge/latestdoi/137751482)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/birnstiel/dsharp_opac/master?filepath=notebooks%2Findex.ipynb)
-        
-        # DSHARP Mie-Opacity Library
-        
-        This repository contains a module to carry out Mie opacity calculations based on
-        a range of astrophysically relevant optical datasets and to calculate the
-        default opacity tables used in the Disk Substructures at High Angular Resolution
-        Project ([DSHARP](https://almascience.eso.org/almadata/lp/DSHARP/), PI: S. Andrews).
-        
-        This package was created by [T. Birnstiel](https://www.til-birnstiel.de) and [C.P. Dullemond](http://www.ita.uni-heidelberg.de/~dullemond).
-        
-        ## Credit
-        
-        If you use this package, please cite [Birnstiel et al. (2018)](https://doi.org/10.3847/2041-8213/aaf743).
-        
-        If you use any optical constants, please cite the appropriate experimental papers. The reference will be displayed upon import of the constants.
-        
-        ## Installation
-        
-        -   From [source](https://github.com/birnstiel/dsharp_opac/archive/master.zip): go into the base directory (where this `README.md` is) and run
-        
-                pip install .
-        
-              Should you work on the sources, e.g. for including new optical constants or new mehtods, then we recommend linking the installation to the source folder. Changes to the sources will then be reflected upon `import dsharp_opac` without the need to reinstall the package.
-        
-        - last release from [pypi.org](pypi.org):
-        
-                pip install dsharp_opac
-        
-        Note: some of the optical constants rely on data files that will be downloaded
-        upon first use of that particular class.
-        
-        ## Tests & Examples
-        
-        You can find some jupyter notebooks in the [notebooks folder](notebooks/index.ipynb) that demonstrate some of the functionality of this package. It also contains the notebooks and data that were used to create the figures in [Birnstiel et al. (2018)](https://doi.org/10.3847/2041-8213/aaf743).
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Codacy Badge](https://api.codacy.com/project/badge/Grade/b04c8f86251749ac92361c6431103a08)](https://app.codacy.com/app/birnstiel/dsharp_opac?utm_source=github.com&utm_medium=referral&utm_content=birnstiel/dsharp_opac&utm_campaign=Badge_Grade_Dashboard)
+[![DOI](https://zenodo.org/badge/137751482.svg)](https://zenodo.org/badge/latestdoi/137751482)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/birnstiel/dsharp_opac/master?filepath=notebooks%2Findex.ipynb)
+
+# DSHARP Mie-Opacity Library
+
+This repository contains a module to carry out Mie opacity calculations based on
+a range of astrophysically relevant optical datasets and to calculate the
+default opacity tables used in the Disk Substructures at High Angular Resolution
+Project ([DSHARP](https://almascience.eso.org/almadata/lp/DSHARP/), PI: S. Andrews).
+
+This package was created by [T. Birnstiel](https://www.til-birnstiel.de) and [C.P. Dullemond](http://www.ita.uni-heidelberg.de/~dullemond).
+
+## Credit
+
+If you use this package, please cite [Birnstiel et al. (2018)](https://doi.org/10.3847/2041-8213/aaf743).
+
+If you use any optical constants, please cite the appropriate experimental papers. The reference will be displayed upon import of the constants.
+
+## Installation
+
+-   From [source](https://github.com/birnstiel/dsharp_opac/archive/master.zip): go into the base directory (where this `README.md` is) and run
+
+        pip install .
+
+      Should you work on the sources, e.g. for including new optical constants or new mehtods, then we recommend linking the installation to the source folder. Changes to the sources will then be reflected upon `import dsharp_opac` without the need to reinstall the package.
+
+- last release from [pypi.org](pypi.org):
+
+        pip install dsharp_opac
+
+Note: some of the optical constants rely on data files that will be downloaded
+upon first use of that particular class.
+
+## Tests & Examples
+
+You can find some jupyter notebooks in the [notebooks folder](notebooks/index.ipynb) that demonstrate some of the functionality of this package. It also contains the notebooks and data that were used to create the figures in [Birnstiel et al. (2018)](https://doi.org/10.3847/2041-8213/aaf743).
```

### Comparing `dsharp_opac-1.1.6/README.md` & `dsharp_opac-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/__init__.py` & `dsharp_opac-1.1.7/dsharp_opac/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .bhmie_python import bhmie_python
 try:
     from .bhmie_fortran import bhmie_fortran
 except ImportError:
     print('fortran mie routines unavailable')
 
-__version__ = '1.1.6'
+__version__ = '1.1.7'
 
 from .dsharp_opac import \
     progress_bar, \
     diel_const, \
     diel_from_lnk_file, \
     diel_henning, \
     diel_jaeger98, \
@@ -39,15 +39,16 @@
     get_dsharp_mix, \
     get_opacities, \
     size_average_opacity, \
     get_smooth_opacities, \
     distribution, \
     get_B11_fit, \
     get_B11S_fit, \
-    get_datafile
+    get_datafile, \
+    chop_forward_scattering
 
 __all__ = [
     'bhmie_python',
     'bhmie_fortran',
     'progress_bar',
     'diel_const',
     'diel_from_lnk_file',
@@ -80,8 +81,9 @@
     'get_ricci_mix',
     'get_dsharp_mix',
     'get_opacities',
     'size_average_opacity',
     'distribution',
     'get_B11_fit',
     'get_B11S_fit',
-    'get_datafile']
+    'get_datafile',
+    'chop_forward_scattering']
```

### Comparing `dsharp_opac-1.1.6/dsharp_opac/bhmie_fortran.f90` & `dsharp_opac-1.1.7/dsharp_opac/bhmie_fortran.f90`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/bhmie_python.py` & `dsharp_opac-1.1.7/dsharp_opac/bhmie_python.py`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/data/Kataoka2014-Fig2b-1e-5cm.csv` & `dsharp_opac-1.1.7/dsharp_opac/data/Kataoka2014-Fig2b-1e-5cm.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/data/Kataoka2014-Fig2d-1e-5cm.csv` & `dsharp_opac-1.1.7/dsharp_opac/data/Kataoka2014-Fig2d-1e-5cm.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/data/andrews2009.dat` & `dsharp_opac-1.1.7/dsharp_opac/data/andrews2009.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/data/default_opacities.npz` & `dsharp_opac-1.1.7/dsharp_opac/data/default_opacities.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/data/default_opacities_extrapol.npz` & `dsharp_opac-1.1.7/dsharp_opac/data/default_opacities_extrapol.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/data/default_opacities_smooth.npz` & `dsharp_opac-1.1.7/dsharp_opac/data/default_opacities_smooth.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/data/icefree_opacities.npz` & `dsharp_opac-1.1.7/dsharp_opac/data/icefree_opacities.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/data/icefree_opacities_smooth.npz` & `dsharp_opac-1.1.7/dsharp_opac/data/icefree_opacities_smooth.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/data/kappa_D01_T100K_p3.5_amax1mm.csv` & `dsharp_opac-1.1.7/dsharp_opac/data/kappa_D01_T100K_p3.5_amax1mm.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/data/kataoka_mix.lnk` & `dsharp_opac-1.1.7/dsharp_opac/data/kataoka_mix.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/dsharp_opac.py` & `dsharp_opac-1.1.7/dsharp_opac/dsharp_opac.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import numpy as np
 import os
 import sys
 import warnings
 import pkg_resources
 import astropy.constants as const
 from pathlib import Path
+from scipy.interpolate import interp2d, RegularGridInterpolator
 
 au = const.au.cgs.value
 M_sun = const.M_sun.cgs.value
 k_b = const.k_B.cgs.value
 m_p = const.m_p.cgs.value
 G = const.G.cgs.value
 sig_h2 = 2e-15  # cross section of H2 [cm^2]
@@ -1693,15 +1694,15 @@
     n_lam = q_abs.shape[1]
     kappa_abs = q_abs * np.tile(np.pi * a**2 / m, [n_lam, 1]).transpose()
     kappa_sca = q_sca * np.tile(np.pi * a**2 / m, [n_lam, 1]).transpose()
     return kappa_abs, kappa_sca
 
 
 def get_size_averaged_opacity(a, lam, n, rho_s, diel_const=None, q_abs=None,
-                              q_sca=None, kappa_abs=None, kappa_sca=None):
+                              q_sca=None, kappa_abs=None, kappa_sca=None, S1=None, S2=None, theta=None, g=None):
     """
     Averages the opacity over the given size distribution.
 
     Arguments:
     ----------
 
     a : array
@@ -1749,32 +1750,65 @@
     #
     m = 4. * np.pi / 3. * rho_s * a**3
     sig = n * m * a
     sig = sig / sum(sig)
     #
     # calculate the opacities ...
     #
-    if (q_abs is None or q_sca is None) and (kappa_abs is None or kappa_sca is None):
+    if ((q_abs is None or q_sca is None) and (kappa_abs is None or kappa_sca is None)):
         package = get_mie_coefficients(a, lam, diel_const)
         q_abs = package['q_abs']
         q_sca = package['q_sca']
-    elif (kappa_abs is None or kappa_sca is None):
+        g = package['g']
+        S1 = package['S1']
+        S2 = package['S2']
+        theta = package['theta']
+
+    if (kappa_abs is None or kappa_sca is None):
         kappa_abs, kappa_sca = get_kappa_from_q(a, m, q_abs, q_sca)
     #
     # ... average them over the size distribution ...
     #
-    kappa_abs_m = np.zeros(len(lam))
-    kappa_sca_m = np.zeros(len(lam))
-    for i in np.arange(len(lam)):
+    n_lam = len(lam)
+    kappa_abs_m = np.zeros(n_lam)
+    kappa_sca_m = np.zeros(n_lam)
+    # average opacities
+    for i in np.arange(n_lam):
         kappa_abs_m[i] = sum(np.transpose(kappa_abs[:, i]) * sig, 0)
         kappa_sca_m[i] = sum(np.transpose(kappa_sca[:, i]) * sig, 0)
+
+    # average g
+    if g is not None:
+        g_m = np.zeros(n_lam)
+        for i in np.arange(n_lam):
+            g_m[i] = sum(np.transpose(g[:, i]) * sig, 0)
+
+    # average scattering amplitudes
+
+    if theta is not None and S1 is not None and S2 is not None:
+        n_th = len(theta)
+        S1_m = np.zeros([n_lam, n_th])
+        S2_m = np.zeros([n_lam, n_th])
+        for i in np.arange(n_lam):
+            S1_m[i, :] = np.sum(S1[:, i, :].T * sig, -1)
+            S2_m[i, :] = np.sum(S2[:, i, :].T * sig, -1)
+
     #
     # ... and return them
     #
-    return kappa_abs_m, kappa_sca_m
+    res = {
+        'kappa_abs_m': kappa_abs_m,
+        'kappa_sca_m': kappa_sca_m,
+    }
+    if g is not None:
+        res['g'] = g_m
+    if S1 is not None:
+        res['S1'] = S1_m
+        res['S2'] = S2_m
+    return res
 
 
 def get_mie_coefficients(A, LAM, diel_constants, bhmie_function=bhmie_function,
                          nang=3, extrapolate_large_grains=False):
     """
     This calculates the opacity for the given dielectric constants for all
     grain sizes and wavelength specified in LAM and A.
@@ -2086,14 +2120,15 @@
             'a_h',
             'k_abs_h',
             'k_sca_h',
             'q_abs_h',
             'q_sca_h',
             'g_h',
             'S1_h',
+            'zscat',
             'S2_h']:
         if key in opac_dict:
             dictionary[key] = opac_dict[key]
 
     np.savez_compressed(os.path.join(path, fname), **dictionary)
 
 
@@ -2291,15 +2326,109 @@
         f.write('\n')
         for ilam in range(opacity_dict['lam'].size):
             for itheta in range(opacity_dict['theta'].size):
                 f.write('%13.6e %13.6e %13.6e %13.6e %13.6e %13.6e\n' %
                         (opacity_dict['zscat'][index, ilam, itheta, 0], opacity_dict['zscat'][index, ilam, itheta, 1],
                          opacity_dict['zscat'][index, ilam, itheta, 2], opacity_dict['zscat'][index, ilam, itheta, 3],
                          opacity_dict['zscat'][index, ilam, itheta, 4], opacity_dict['zscat'][index, ilam, itheta, 5]))
+            f.write('\n')
+
+
+def interpolate_radmc3d_scatmat_file(a, opacity_dict, name, path='.'):
+    """
+    The RADMC-3D radiative transfer package[1] can perform dust continuum
+    radiative transfer for diagnostic purposes. It is designed for astronomical
+    applications. The code needs the opacities in a particular form. This
+    subroutine writes the opacities out in that form. It will write it to
+    the file dustkapscatmat_<name>.inp.
+
+    Arguments:
+    ----------
+
+    a : float
+        grain size to be written out
+
+    opacity_dict : dict
+        dictionary with the opacity information. the keys are:
+
+        a : array
+            particle size grid in cm
+
+        lam : array
+            wavelength grid in cm
+
+        theta : array
+            angle grid (degree)
+
+        rho_s : float
+            internal density of the particles
+
+        k_abs, k_sca : array
+            absorption and scattering opacities
+            size = len(a), len(lam)
+
+        g_scat : array
+            Henyey-Greenstein coefficient
+            size = len(a), len(lam)
+
+        zscat : array
+            scattering Mueller matrix elements
+            size = len(a), len(lam), len(theta), 6
+
+    name : str
+        name to be used as species name, will be part of the file name
+
+    path : str
+        the directory where the output file will be saved
+
+
+    References:
+    -----------
+
+    - [1] http://www.ita.uni-heidelberg.de/~dullemond/software/radmc-3d/
+
+    """
+    a_grid = opacity_dict['a']
+    zscat = opacity_dict['zscat']
+
+    filename = os.path.join(path, 'dustkapscatmat_{}.inp'.format(name))
+
+    with open(filename, 'w') as f:
+        f.write('# Opacity and scattering matrix file for ' + name + '\n')
+        f.write('# Please do not forget to cite in your publications theo riginal paper of these optical constant measurements\n')
+        f.write('# Made with the DSHARP_OPAC package by Cornelis Dullemond & Til Birnstiel\n')
+        f.write('# using either the bhmie.py Mie code of Bohren and Huffman (python version by Cornelis Dullemond,\n')
+        f.write('# or a F90 version by Til Birnstiel, both after the original bhmie.f code by Bruce Draine)\n')
+        f.write('# Grain size = {0:13.6e} cm\n'.format(a))
+        f.write('# Material density = {0:6.3f} g/cm^3\n'.format(opacity_dict["rho_s"]))
+        f.write('1\n')  # Format number
+        f.write('{0:d}\n'.format(opacity_dict["lam"].size))
+        f.write('{0:d}\n'.format(opacity_dict["theta"].size))
         f.write('\n')
+        for i in range(opacity_dict['lam'].size):
+            f.write('%13.6e %13.6e %13.6e %13.6e\n' % (opacity_dict['lam'][i] * 1e4,
+                                                       np.interp(a, a_grid, opacity_dict['k_abs'][:, i]),
+                                                       np.interp(a, a_grid, opacity_dict['k_sca'][:, i]),
+                                                       np.interp(a, a_grid, opacity_dict['g'][:, i])))
+        f.write('\n')
+        for j in range(opacity_dict['theta'].size):
+            f.write('%13.6e\n' % (opacity_dict['theta'][j]))
+        f.write('\n')
+        for ilam in range(opacity_dict['lam'].size):
+            for itheta in range(opacity_dict['theta'].size):
+                f.write('%13.6e %13.6e %13.6e %13.6e %13.6e %13.6e\n' %
+                        (
+                            np.interp(a, a_grid, zscat[:, ilam, itheta, 0]),
+                            np.interp(a, a_grid, zscat[:, ilam, itheta, 1]),
+                            np.interp(a, a_grid, zscat[:, ilam, itheta, 2]),
+                            np.interp(a, a_grid, zscat[:, ilam, itheta, 3]),
+                            np.interp(a, a_grid, zscat[:, ilam, itheta, 4]),
+                            np.interp(a, a_grid, zscat[:, ilam, itheta, 5])
+                        ))
+            f.write('\n')
 
 
 def read_radmc3d_scatmat_file(name, path='.'):
     """
     Read scattering matrix from species `name` in RADMC3D kapscatmat format
 
     Arguments:
@@ -2579,14 +2708,82 @@
 
     diel_constants = diel_mixed(constants, vol_fract, rule=rule)
     rho_s = sum(densities * np.array(vol_fract))
 
     return diel_constants, rho_s
 
 
+def chop_forward_scattering(opac_dict, chopforward=5):
+    """Chop the forward scattering.
+
+    This part chops the very-forward scattering part of the phase function.
+    This very-forward scattering part is basically the same as no scattering,
+    but is treated by the code as a scattering event. By cutting this part out
+    of the phase function, we avoid those non-scattering scattering events.
+    This needs to recalculate the scattering opacity kappa_sca and asymmetry
+    factor g.
+
+    Parameters
+    ----------
+    opac_dict : dict
+        opacity dictionary as produced by dsharp_opac
+
+    chopforward : float
+        up to which angle to we truncate the forward scattering
+    """
+
+    k_sca = opac_dict['k_sca']
+    theta = opac_dict['theta']
+    g = opac_dict['g']
+    rho_s = opac_dict['rho_s']
+    lam = opac_dict['lam']
+    a = opac_dict['a']
+    m = 4 * np.pi / 3 * rho_s * a ** 3
+
+    n_a = len(a)
+    n_lam = len(lam)
+
+    if 'zscat' in opac_dict:
+        zscat = opac_dict['zscat']
+    else:
+        S1 = opac_dict['S1']
+        S2 = opac_dict['S2']
+        zscat = calculate_mueller_matrix(lam, m, S1, S2)['zscat']
+
+    zscat_nochop = zscat.copy()
+
+    mu = np.cos(theta * np.pi / 180.)
+    # dmu = np.diff(mu)
+
+    for grain in range(n_a):
+        for i in range(n_lam):
+            if chopforward > 0:
+                iang = np.where(theta < chopforward)
+                if theta[0] == 0.0:
+                    iiang = np.max(iang) + 1
+                else:
+                    iiang = np.min(iang) - 1
+                zscat[grain, i, iang, :] = zscat[grain, i, iiang, :]
+
+                # zav = 0.5 * (zscat[grain, i, 1:, 0] + zscat[grain, i, :-1, 0])
+                # dum = -0.5 * zav * dmu
+                # integral = dum.sum() * 4 * np.pi
+                # k_sca[grain, i] = integral
+
+                # g = <mu> = 2 pi / kappa * int(Z11(mu) mu dmu)
+                # mu_av = 0.5 * (mu[1:] + mu[:-1])
+                # P_mu = 2 * np.pi / k_sca[grain, i] * 0.5 * (zscat[grain, i, 1:, 0] + zscat[grain, i, :-1, 0])
+                # g[grain, i] = np.sum(P_mu * mu_av * dmu)
+
+                k_sca[grain, i] = -2 * np.pi * np.trapz(zscat[grain, i, :, 0], x=mu)
+                g[grain, i] = -2 * np.pi * np.trapz(zscat[grain, i, :, 0] * mu, x=mu) / k_sca[grain, i]
+
+    return zscat, zscat_nochop, k_sca, g
+
+
 def get_opacities(a, lam, rho_s, diel_const, bhmie_function=bhmie_function,
                   extrapol=False, n_angle=3,
                   extrapolate_large_grains=False):
     """
     Calculates opacities according to some specified method for
     a given size- and wavelength grid.
 
@@ -2665,15 +2862,15 @@
 
     package['a'] = a
     package['lam'] = lam
 
     return package
 
 
-def size_average_opacity(lam_avg, a, lam, k_abs, k_sca, q=3.5, plot=False, ax=None):
+def size_average_opacity(lam_avg, a, lam, k_abs, k_sca, q=3.5, plot=False, ax=None, g=None, S1=None, S2=None):
     """
     Calculates the opacity as function of maximum particle size for a power-law size distribution
 
     Arguments:
     ----------
     lam_avg : float | array
         wavelength at which to calculate the size-averaged opacities
@@ -2698,61 +2895,99 @@
     plot : bool
         if True, create a plot of the result
 
     ax : None | axes object
         if None: plot is created in new figure, if axes object: uses this object
         for the plotting.
 
+    g, S1, S2: array
+        other quantities (Henyey Greenstein parameter & scattering amplitudes)
+        that will get averaged if passed
+
     Output:
     -------
     k_abs, k_sca, [ax]
 
     k_abs, k_sca : arrays
         size averaged opacities as function of maximum particle size
 
     ax : axes object
         if plot is True: return the axes object
     """
     import matplotlib.pyplot as plt
 
-    # interpolate at the observed frequencies
     lam_avg = np.array(lam_avg, ndmin=1)
     if len(lam_avg) > 1:
         calc_beta = True
     else:
         calc_beta = False
 
-    k_a = []
-    k_s = []
+    # interpolate at the observed frequencies:
+    # - opacities
+
+    f_a = interp2d(lam, a, k_abs)
+    k_a = f_a(lam_avg, a).T
+    f_s = interp2d(lam, a, k_sca)
+    k_s = f_s(lam_avg, a).T
+
+    # - g-factor
 
-    for _lam in lam_avg:
-        k_a += [[np.interp(_lam, lam, k_abs[ia, :]) for ia in range(len(a))]]
-        k_s += [[np.interp(_lam, lam, k_sca[ia, :]) for ia in range(len(a))]]
+    if g is not None:
+        f_g = interp2d(lam, a, g)
+        g_i = f_g(lam_avg, a).T
 
-    k_a = np.array(k_a)
-    k_s = np.array(k_s)
+    # - scattering amplitudes
+
+    if S1 is not None:
+        n_th = S1.shape[-1]
+        th = np.arange(n_th, dtype=float)
+        new_points = np.reshape(np.meshgrid(a, lam_avg, th, indexing='ij'), (3, -1), order='C').T
+
+        f_S1 = RegularGridInterpolator((a, lam, th), S1)
+        S1_i = f_S1(new_points).reshape([len(a), len(lam_avg), len(th)])
+
+        f_S2 = RegularGridInterpolator((a, lam, th), S2)
+        S2_i = f_S2(new_points).reshape([len(a), len(lam_avg), len(th)])
 
     # average over size distributions
 
     ka = np.zeros([len(lam_avg), len(a)])
     ks = np.zeros([len(lam_avg), len(a)])
+
+    if g is not None:
+        g_m = np.zeros([len(lam_avg), len(a)])
+    if S1 is not None:
+        S1_m = np.zeros([len(lam_avg), len(a), n_th])
+        S2_m = np.zeros([len(lam_avg), len(a), n_th])
+
     for ia in range(len(a)):
 
         # make a size distribution
 
         s = (a / a[0])**(4 - q)
         if ia < len(a) - 1:
             s[ia + 1:] = 1e-100
         s = s / s.sum()
 
         for ilam in range(len(lam_avg)):
             ka[ilam, ia] = np.sum(k_a[ilam, :] * s)
             ks[ilam, ia] = np.sum(k_s[ilam, :] * s)
 
+            if g is not None:
+                g_m[ilam, ia] = np.sum(g_i[ilam, :] * s)
+            if S1 is not None:
+                S1_m[ilam, ia, :] = np.sum(S1_i * s[:, None, None], 1)
+                S2_m[ilam, ia, :] = np.sum(S2_i * s[:, None, None], 1)
+
     ret = {'ka': ka, 'ks': ks}
+    if g is not None:
+        ret['g'] = g_m
+    if S1 is not None:
+        ret['S1'] = S1_m
+        ret['S2'] = S2_m
 
     # calculate beta
 
     if calc_beta:
         beta = -np.log10(ka[-1, :] / ka[0, :]) / np.log10(lam_avg[-1] / lam_avg[0])
         ret['beta'] = beta
```

### Comparing `dsharp_opac-1.1.6/dsharp_opac/fit_module.f90` & `dsharp_opac-1.1.7/dsharp_opac/fit_module.f90`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/draine/links.json` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/draine/links.json`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/henning/new/links.json` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/new/links.json`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/henning/old/links.json` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/henning/old/links.json`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/luca/H2Oice_Warren.dat` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/luca/H2Oice_Warren.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/luca/aC_ACH2_Zubko.dat` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/luca/aC_ACH2_Zubko.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/luca/silicate.dat` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/luca/silicate.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-iron-k.csv` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-iron-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-iron-n.csv` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-iron-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-iron.lnk` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-iron.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-olivine-k.csv` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-olivine-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-olivine-n.csv` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-olivine-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-olivine.lnk` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-olivine.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-organics-k.csv` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-organics-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-organics-n.csv` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-organics-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-organics.lnk` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-organics.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-k.csv` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-n.csv` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene.lnk` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-troilite-k.csv` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-troilite-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-troilite.lnk` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-troilite.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-waterice-k.csv` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-waterice-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-waterice-n.csv` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-waterice-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/P94-waterice.lnk` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/P94-waterice.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/pollack1994/make_lnk.py` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/pollack1994/make_lnk.py`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/testfiles_ricci/beta.dat` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/beta.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/testfiles_ricci/d_test_vacuum30.dust` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/d_test_vacuum30.dust`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/testfiles_ricci/dust_opacities.16` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/testfiles_ricci/dust_opacities.16`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/warren/warren_1984.txt` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/warren_1984.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/warren/warren_1984_all_temps.txt` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/warren/warren_1984_all_temps.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/zubko_E_ACH2.txt` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_E_ACH2.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/zubko_E_BE.txt` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_E_BE.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/zubko_k_ACH2.txt` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_k_ACH2.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/zubko_k_BE.txt` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_k_BE.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/zubko_n_ACH2.txt` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_n_ACH2.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/zubko_n_BE.txt` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_n_BE.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac/optical_constants/zubko+1996/zubko_ocr.pdf` & `dsharp_opac-1.1.7/dsharp_opac/optical_constants/zubko+1996/zubko_ocr.pdf`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/dsharp_opac.egg-info/PKG-INFO` & `dsharp_opac-1.1.7/dsharp_opac.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: dsharp-opac
-Version: 1.1.6
+Version: 1.1.7
 Summary: python routines to calculate mie opacities
 Home-page: https://github.com/birnstiel/dsharp_opac
 Author: Til Birnstiel & DSHARP collaboration
 Author-email: til.birnstiel@lmu.de
 License: GPLv3
-Description: [![Codacy Badge](https://api.codacy.com/project/badge/Grade/b04c8f86251749ac92361c6431103a08)](https://app.codacy.com/app/birnstiel/dsharp_opac?utm_source=github.com&utm_medium=referral&utm_content=birnstiel/dsharp_opac&utm_campaign=Badge_Grade_Dashboard)
-        [![DOI](https://zenodo.org/badge/137751482.svg)](https://zenodo.org/badge/latestdoi/137751482)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/birnstiel/dsharp_opac/master?filepath=notebooks%2Findex.ipynb)
-        
-        # DSHARP Mie-Opacity Library
-        
-        This repository contains a module to carry out Mie opacity calculations based on
-        a range of astrophysically relevant optical datasets and to calculate the
-        default opacity tables used in the Disk Substructures at High Angular Resolution
-        Project ([DSHARP](https://almascience.eso.org/almadata/lp/DSHARP/), PI: S. Andrews).
-        
-        This package was created by [T. Birnstiel](https://www.til-birnstiel.de) and [C.P. Dullemond](http://www.ita.uni-heidelberg.de/~dullemond).
-        
-        ## Credit
-        
-        If you use this package, please cite [Birnstiel et al. (2018)](https://doi.org/10.3847/2041-8213/aaf743).
-        
-        If you use any optical constants, please cite the appropriate experimental papers. The reference will be displayed upon import of the constants.
-        
-        ## Installation
-        
-        -   From [source](https://github.com/birnstiel/dsharp_opac/archive/master.zip): go into the base directory (where this `README.md` is) and run
-        
-                pip install .
-        
-              Should you work on the sources, e.g. for including new optical constants or new mehtods, then we recommend linking the installation to the source folder. Changes to the sources will then be reflected upon `import dsharp_opac` without the need to reinstall the package.
-        
-        - last release from [pypi.org](pypi.org):
-        
-                pip install dsharp_opac
-        
-        Note: some of the optical constants rely on data files that will be downloaded
-        upon first use of that particular class.
-        
-        ## Tests & Examples
-        
-        You can find some jupyter notebooks in the [notebooks folder](notebooks/index.ipynb) that demonstrate some of the functionality of this package. It also contains the notebooks and data that were used to create the figures in [Birnstiel et al. (2018)](https://doi.org/10.3847/2041-8213/aaf743).
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Codacy Badge](https://api.codacy.com/project/badge/Grade/b04c8f86251749ac92361c6431103a08)](https://app.codacy.com/app/birnstiel/dsharp_opac?utm_source=github.com&utm_medium=referral&utm_content=birnstiel/dsharp_opac&utm_campaign=Badge_Grade_Dashboard)
+[![DOI](https://zenodo.org/badge/137751482.svg)](https://zenodo.org/badge/latestdoi/137751482)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/birnstiel/dsharp_opac/master?filepath=notebooks%2Findex.ipynb)
+
+# DSHARP Mie-Opacity Library
+
+This repository contains a module to carry out Mie opacity calculations based on
+a range of astrophysically relevant optical datasets and to calculate the
+default opacity tables used in the Disk Substructures at High Angular Resolution
+Project ([DSHARP](https://almascience.eso.org/almadata/lp/DSHARP/), PI: S. Andrews).
+
+This package was created by [T. Birnstiel](https://www.til-birnstiel.de) and [C.P. Dullemond](http://www.ita.uni-heidelberg.de/~dullemond).
+
+## Credit
+
+If you use this package, please cite [Birnstiel et al. (2018)](https://doi.org/10.3847/2041-8213/aaf743).
+
+If you use any optical constants, please cite the appropriate experimental papers. The reference will be displayed upon import of the constants.
+
+## Installation
+
+-   From [source](https://github.com/birnstiel/dsharp_opac/archive/master.zip): go into the base directory (where this `README.md` is) and run
+
+        pip install .
+
+      Should you work on the sources, e.g. for including new optical constants or new mehtods, then we recommend linking the installation to the source folder. Changes to the sources will then be reflected upon `import dsharp_opac` without the need to reinstall the package.
+
+- last release from [pypi.org](pypi.org):
+
+        pip install dsharp_opac
+
+Note: some of the optical constants rely on data files that will be downloaded
+upon first use of that particular class.
+
+## Tests & Examples
+
+You can find some jupyter notebooks in the [notebooks folder](notebooks/index.ipynb) that demonstrate some of the functionality of this package. It also contains the notebooks and data that were used to create the figures in [Birnstiel et al. (2018)](https://doi.org/10.3847/2041-8213/aaf743).
```

### Comparing `dsharp_opac-1.1.6/notebooks/AppendixB.ipynb` & `dsharp_opac-1.1.7/notebooks/AppendixB.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999609375%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(14, 'res_def = opacity.get_opacities(a, lam, "*

 * *            'rho_s=rhos_default, diel_const=d_def, extrapol=True, '*

 * *            "extrapolate_large_grains=True)\\n'), (15, 'res_por = opacity.get_opacities(a, lam, "*

 * *            'rho_s=rhos_porous,  diel_const=d_por, extrapol=True, '*

 * *            "extrapolate_large_grains=True)\\n'), (16, 'res_h2o = opacity.get_opacities(a, lam, "*

 * *            'rho_s=rhos_water,   diel_const=d_h2o, extrapol=True, '*

 * *            "extrapolate_l […]*

```diff
@@ -181,23 +181,23 @@
                 "#d_c03 = opacity.diel_mixed(constants_c03,     fv_c03,     rule='Bruggeman')\n",
                 "#d_c04 = opacity.diel_mixed(constants_c04,     fv_c04,     rule='Bruggeman')\n",
                 "#d_c05 = opacity.diel_mixed(constants_c05,     fv_c05,     rule='Bruggeman')\n",
                 "d_c06 = opacity.diel_mixed(constants_c06,     fv_c06,     rule='Bruggeman')\n",
                 "\n",
                 "# Calculate the Mie opacities, this takes *very* long if `extrapolate_large_grains=False`.\n",
                 "\n",
-                "res_def = opacity.get_opacities(a, lam, rho_s=rhos_default, diel_const=d_def, return_all=True, extrapol=True, extrapolate_large_grains=True)\n",
-                "res_por = opacity.get_opacities(a, lam, rho_s=rhos_porous,  diel_const=d_por, return_all=True, extrapol=True, extrapolate_large_grains=True)\n",
-                "res_h2o = opacity.get_opacities(a, lam, rho_s=rhos_water,   diel_const=d_h2o, return_all=True, extrapol=True, extrapolate_large_grains=True)\n",
-                "res_c01 = opacity.get_opacities(a, lam, rho_s=rhos_c01,     diel_const=d_c01, return_all=True, extrapol=True, extrapolate_large_grains=True)\n",
-                "res_c02 = opacity.get_opacities(a, lam, rho_s=rhos_c02,     diel_const=d_c02, return_all=True, extrapol=True, extrapolate_large_grains=True)\n",
-                "#res_c03 = opacity.get_opacities(a, lam, rho_s=rhos_c03,     diel_const=d_c03, return_all=True, extrapol=True, extrapolate_large_grains=True)\n",
-                "#res_c04 = opacity.get_opacities(a, lam, rho_s=rhos_c04,     diel_const=d_c04, return_all=True, extrapol=True, extrapolate_large_grains=True)\n",
-                "#res_c05 = opacity.get_opacities(a, lam, rho_s=rhos_c05,     diel_const=d_c05, return_all=True, extrapol=True, extrapolate_large_grains=True)\n",
-                "res_c06 = opacity.get_opacities(a, lam, rho_s=rhos_c06,     diel_const=d_c06, return_all=True, extrapol=True, extrapolate_large_grains=True)"
+                "res_def = opacity.get_opacities(a, lam, rho_s=rhos_default, diel_const=d_def, extrapol=True, extrapolate_large_grains=True)\n",
+                "res_por = opacity.get_opacities(a, lam, rho_s=rhos_porous,  diel_const=d_por, extrapol=True, extrapolate_large_grains=True)\n",
+                "res_h2o = opacity.get_opacities(a, lam, rho_s=rhos_water,   diel_const=d_h2o, extrapol=True, extrapolate_large_grains=True)\n",
+                "res_c01 = opacity.get_opacities(a, lam, rho_s=rhos_c01,     diel_const=d_c01, extrapol=True, extrapolate_large_grains=True)\n",
+                "res_c02 = opacity.get_opacities(a, lam, rho_s=rhos_c02,     diel_const=d_c02, extrapol=True, extrapolate_large_grains=True)\n",
+                "#res_c03 = opacity.get_opacities(a, lam, rho_s=rhos_c03,     diel_const=d_c03, extrapol=True, extrapolate_large_grains=True)\n",
+                "#res_c04 = opacity.get_opacities(a, lam, rho_s=rhos_c04,     diel_const=d_c04, extrapol=True, extrapolate_large_grains=True)\n",
+                "#res_c05 = opacity.get_opacities(a, lam, rho_s=rhos_c05,     diel_const=d_c05, extrapol=True, extrapolate_large_grains=True)\n",
+                "res_c06 = opacity.get_opacities(a, lam, rho_s=rhos_c06,     diel_const=d_c06, extrapol=True, extrapolate_large_grains=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Size averaging"
```

### Comparing `dsharp_opac-1.1.6/notebooks/Figure1.ipynb` & `dsharp_opac-1.1.7/notebooks/Figure1.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/notebooks/Figure2.ipynb` & `dsharp_opac-1.1.7/notebooks/Figure2.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/notebooks/Figure3.ipynb` & `dsharp_opac-1.1.7/notebooks/Figure3.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/notebooks/Figure4.ipynb` & `dsharp_opac-1.1.7/notebooks/Figure4.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/notebooks/Figure56.ipynb` & `dsharp_opac-1.1.7/notebooks/Figure56.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99984375%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(7, "        '*

 * *            'f\'https://www.astro.princeton.edu/~draine/dust/extcurvs/{filename}\',\\n")], delete: '*

 * *            '[7]}}}'}*

```diff
@@ -38,15 +38,15 @@
                 "# Download one of the Weingartner & Draine 2001 dust models for comparison\n",
                 "\n",
                 "filename = 'kext_albedo_WD_MW_3.1_60'\n",
                 "if not os.path.isfile(filename):\n",
                 "    from urllib.request import urlretrieve\n",
                 "    print('Downloading file \\'{}\\' ... '.format(filename), end='')\n",
                 "    urlretrieve(\n",
-                "        'ftp://ftp.astro.princeton.edu/draine/dust/mix/{}'.format(filename),\n",
+                "        f'https://www.astro.princeton.edu/~draine/dust/extcurvs/{filename}',\n",
                 "        filename=filename)\n",
                 "    print('Done!')\n",
                 "\n",
                 "with open(filename) as f:\n",
                 "    while not f.readline().startswith('--------'):\n",
                 "        pass\n",
                 "    lam_dr,_,_,_,k_dr = np.loadtxt(f).T"
```

### Comparing `dsharp_opac-1.1.6/notebooks/Figure7.ipynb` & `dsharp_opac-1.1.7/notebooks/Figure7.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/notebooks/Figure8.ipynb` & `dsharp_opac-1.1.7/notebooks/Figure8.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.866170634920635%*

 * *Differences: {"'cells'": "{5: {'metadata': {replace: OrderedDict([('tags', [])])}}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'Python 3 (ipykernel)'}, 'language_info': "*

 * *               "{'version': '3.9.15'}}",*

 * * "'nbformat_minor'": '4'}*

```diff
@@ -67,15 +67,17 @@
                 "\n",
                 "Bnu    = np.array([aux.planck_B_nu(nu, T) for T in T_array])\n",
                 "dBnudT = np.array([aux.planck_dBnu_dT(nu, T) for T in T_array])"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "## Calculate mean opacities for all temperatures\n",
                 "\n",
                 "For the Rosseland Mean, we need the *extinction opacity*\n",
                 "\n",
                 "$$\n",
                 "\\kappa_\\nu^\\mathrm{ext}(a) = \\kappa_\\nu^{abs}(a) + (1-g)\\,\\kappa_\\nu^{sca}(a)\n",
@@ -335,27 +337,27 @@
                 "    )\n",
                 "f.savefig('figures/fig8_mean_opacities.pdf')"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.6.6"
+            "version": "3.9.15"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `dsharp_opac-1.1.6/notebooks/Figure9.ipynb` & `dsharp_opac-1.1.7/notebooks/Figure9.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/notebooks/aux_functions.py` & `dsharp_opac-1.1.7/notebooks/aux_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 style = [
     'default',
     {
         'figure.figsize': (3.5, 3.5 / 1.618),
         'font.size': 9,  # 12
         'image.cmap': 'inferno',
         'figure.dpi': 200,
-        'font.family': ['Times', 'Times New Roman'],
+        'font.family': 'serif',
+        'font.serif': ['Times', 'Times New Roman'] + plt.rcParams['font.serif'],
         'xtick.top': True,
         'xtick.direction': 'in',
         'ytick.right': True,
         'ytick.direction': 'in',
         'mathtext.fontset': 'cm'
         }]
 
-
 def set_style():
     "Set the style of DSHARP"
     plt.style.use(style)
 
 
 def get_style():
     "Get a style context manager for DSHARP"
```

### Comparing `dsharp_opac-1.1.6/notebooks/dsharp_porosity.ipynb` & `dsharp_opac-1.1.7/notebooks/dsharp_porosity.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/notebooks/index.ipynb` & `dsharp_opac-1.1.7/notebooks/index.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/notebooks/opac_widget.py` & `dsharp_opac-1.1.7/notebooks/opac_widget.py`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/notebooks/opacity_examples.ipynb` & `dsharp_opac-1.1.7/notebooks/opacity_examples.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/notebooks/opacity_package_tests.ipynb` & `dsharp_opac-1.1.7/notebooks/opacity_package_tests.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/notebooks/polarization_fraction.ipynb` & `dsharp_opac-1.1.7/notebooks/polarization_fraction.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/notebooks/porosity.ipynb` & `dsharp_opac-1.1.7/notebooks/porosity.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/notebooks/scattering_phase_functions.ipynb` & `dsharp_opac-1.1.7/notebooks/scattering_phase_functions.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/notebooks/smoothed_opacities.ipynb` & `dsharp_opac-1.1.7/notebooks/smoothed_opacities.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.6/setup.py` & `dsharp_opac-1.1.7/setup.py`

 * *Files identical despite different names*

