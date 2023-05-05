# Comparing `tmp/not1mm-23.5.4.tar.gz` & `tmp/not1mm-23.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-23.5.4.tar", last modified: Thu May  4 16:53:15 2023, max compression
+gzip compressed data, was "not1mm-23.5.5.tar", last modified: Fri May  5 20:09:14 2023, max compression
```

## Comparing `not1mm-23.5.4.tar` & `not1mm-23.5.5.tar`

### file list

```diff
@@ -1,138 +1,137 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.873883 not1mm-23.5.4/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.4/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21350 2023-05-04 16:53:15.873883 not1mm-23.5.4/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20605 2023-05-04 16:51:42.000000 not1mm-23.5.4/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.841884 not1mm-23.5.4/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.4/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    77543 2023-05-04 02:56:26.000000 not1mm-23.5.4/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    18606 2023-05-03 01:46:35.000000 not1mm-23.5.4/not1mm/bandmap.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.850884 not1mm-23.5.4/not1mm/data/
--rw-rw-rw-   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.4/not1mm/data/Combinear.qss
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.4/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.4/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.4/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.4/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.4/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.4/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39001 2023-05-01 19:49:53.000000 not1mm-23.5.4/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.4/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.4/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.4/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.4/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.4/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.4/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.4/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.4/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.4/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.4/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.4/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43658 2023-05-01 15:38:56.000000 not1mm-23.5.4/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17745 2023-05-01 21:11:17.000000 not1mm-23.5.4/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.4/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.862883 not1mm-23.5.4/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.4/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.4/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.4/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.4/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.4/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.4/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.4/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.4/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.4/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.4/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.4/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.4/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.4/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.4/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.4/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.4/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.4/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.4/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.4/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.4/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.4/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.4/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.4/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.4/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.4/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.4/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.4/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.4/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.4/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.4/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.4/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.4/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.4/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.4/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.4/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.4/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.4/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.4/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.4/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.4/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.4/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.4/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.4/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.4/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.4/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.4/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.4/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.4/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.4/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.4/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.4/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.4/not1mm/data/ssbmacros.txt
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.869883 not1mm-23.5.4/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.4/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.4/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12468 2023-04-25 15:08:00.000000 not1mm-23.5.4/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.4/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32966 2023-04-24 03:05:48.000000 not1mm-23.5.4/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.4/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.4/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.4/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.4/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.4/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.4/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.4/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.4/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.4/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.4/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5781 2023-05-01 19:29:49.000000 not1mm-23.5.4/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-05-04 16:47:26.000000 not1mm-23.5.4/not1mm/lib/version.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    31143 2023-05-01 19:53:26.000000 not1mm-23.5.4/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.872883 not1mm-23.5.4/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13552 2023-05-01 21:04:22.000000 not1mm-23.5.4/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13558 2023-05-01 16:14:59.000000 not1mm-23.5.4/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13565 2023-05-01 21:07:00.000000 not1mm-23.5.4/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13568 2023-05-01 21:07:03.000000 not1mm-23.5.4/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.4/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14348 2023-04-24 14:53:10.000000 not1mm-23.5.4/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14351 2023-04-24 14:53:19.000000 not1mm-23.5.4/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12719 2023-04-24 14:53:32.000000 not1mm-23.5.4/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2590 2023-04-24 14:53:43.000000 not1mm-23.5.4/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2591 2023-04-24 14:53:53.000000 not1mm-23.5.4/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2594 2023-04-24 14:54:04.000000 not1mm-23.5.4/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14807 2023-05-04 16:44:11.000000 not1mm-23.5.4/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14811 2023-05-04 16:45:09.000000 not1mm-23.5.4/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13701 2023-04-24 14:54:47.000000 not1mm-23.5.4/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13772 2023-04-24 14:54:56.000000 not1mm-23.5.4/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14624 2023-04-24 14:52:00.000000 not1mm-23.5.4/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7272 2023-04-24 14:55:06.000000 not1mm-23.5.4/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13650 2023-04-24 14:55:15.000000 not1mm-23.5.4/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13651 2023-04-24 14:55:25.000000 not1mm-23.5.4/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2851 2023-04-24 14:55:37.000000 not1mm-23.5.4/not1mm/plugins/winter_field_day.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.872883 not1mm-23.5.4/not1mm/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2297 2023-03-29 19:50:12.000000 not1mm-23.5.4/not1mm/testing/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.842884 not1mm-23.5.4/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21350 2023-05-04 16:53:15.000000 not1mm-23.5.4/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3460 2023-05-04 16:53:15.000000 not1mm-23.5.4/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-04 16:53:15.000000 not1mm-23.5.4/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-04 16:53:15.000000 not1mm-23.5.4/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-04 16:53:15.000000 not1mm-23.5.4/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-04 16:53:15.000000 not1mm-23.5.4/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1217 2023-05-04 16:47:34.000000 not1mm-23.5.4/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-04 16:53:15.873883 not1mm-23.5.4/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-04 16:53:15.873883 not1mm-23.5.4/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.4/testing/test.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-21 20:18:16.000000 not1mm-23.5.4/testing/text2.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.606593 not1mm-23.5.5/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.5/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23536 2023-05-05 20:09:14.605593 not1mm-23.5.5/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22791 2023-05-05 20:07:53.000000 not1mm-23.5.5/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.507595 not1mm-23.5.5/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.5/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    77867 2023-05-05 16:13:26.000000 not1mm-23.5.5/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    18606 2023-05-03 01:46:35.000000 not1mm-23.5.5/not1mm/bandmap.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.528594 not1mm-23.5.5/not1mm/data/
+-rw-rw-rw-   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.5/not1mm/data/Combinear.qss
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.5/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.5/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.5/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.5/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.5/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.5/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39001 2023-05-01 19:49:53.000000 not1mm-23.5.5/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.5/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.5/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.5/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.5/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.5/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.5/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.5/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.5/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.5/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.5/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.5/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43663 2023-05-04 21:24:02.000000 not1mm-23.5.5/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.5.5/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.5/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.595593 not1mm-23.5.5/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.5/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.5/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.5/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.5/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.5/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.5/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.5/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.5/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.5/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.5/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.5/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.5/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.5/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.5/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.5/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.5/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.5/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.5/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.5/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.5/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.5/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.5/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.5/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.5/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.5/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.5/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.5/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.5/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.5/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.5/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.5/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.5/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.5/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.5/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.5/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.5/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.5/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.5/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.5/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.5/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.5/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.5/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.5/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.5/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.5/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.5/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.5/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.5/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.5/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.5/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.5/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.5/not1mm/data/ssbmacros.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.602593 not1mm-23.5.5/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.5/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.5/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12468 2023-04-25 15:08:00.000000 not1mm-23.5.5/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.5/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34193 2023-05-05 18:13:45.000000 not1mm-23.5.5/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.5/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.5/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.5/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.5/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.5/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.5/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.5/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.5/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.5/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.5/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5781 2023-05-01 19:29:49.000000 not1mm-23.5.5/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-05-05 20:06:58.000000 not1mm-23.5.5/not1mm/lib/version.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    30050 2023-05-05 15:32:10.000000 not1mm-23.5.5/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.605593 not1mm-23.5.5/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13746 2023-05-05 16:08:13.000000 not1mm-23.5.5/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13752 2023-05-05 16:08:31.000000 not1mm-23.5.5/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13759 2023-05-05 16:08:41.000000 not1mm-23.5.5/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13762 2023-05-05 16:08:51.000000 not1mm-23.5.5/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.5/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14549 2023-05-05 16:08:59.000000 not1mm-23.5.5/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14552 2023-05-05 16:09:07.000000 not1mm-23.5.5/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12990 2023-05-05 16:10:17.000000 not1mm-23.5.5/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.5.5/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15941 2023-05-05 19:46:43.000000 not1mm-23.5.5/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15946 2023-05-05 19:54:23.000000 not1mm-23.5.5/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15022 2023-05-05 16:10:06.000000 not1mm-23.5.5/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15026 2023-05-05 16:10:01.000000 not1mm-23.5.5/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-05 16:09:55.000000 not1mm-23.5.5/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13899 2023-05-05 16:11:06.000000 not1mm-23.5.5/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14753 2023-05-05 16:11:03.000000 not1mm-23.5.5/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.5.5/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.5.5/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.5.5/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.5.5/not1mm/plugins/winter_field_day.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.605593 not1mm-23.5.5/not1mm/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-05-05 15:04:14.000000 not1mm-23.5.5/not1mm/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.509595 not1mm-23.5.5/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23536 2023-05-05 20:09:14.000000 not1mm-23.5.5/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3443 2023-05-05 20:09:14.000000 not1mm-23.5.5/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-05 20:09:14.000000 not1mm-23.5.5/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-05 20:09:14.000000 not1mm-23.5.5/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-05 20:09:14.000000 not1mm-23.5.5/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-05 20:09:14.000000 not1mm-23.5.5/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1217 2023-05-05 20:06:54.000000 not1mm-23.5.5/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-05 20:09:14.606593 not1mm-23.5.5/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-05 20:09:14.605593 not1mm-23.5.5/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.5/testing/test.py
```

### Comparing `not1mm-23.5.4/LICENSE` & `not1mm-23.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/PKG-INFO` & `not1mm-23.5.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.4
+Version: 23.5.5
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -68,14 +68,18 @@
     - [Log Display](#log-display)
     - [Bandmap](#bandmap)
   - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
+  - [Contest specific notes](#contest-specific-notes)
+    - [ARRL Sweekstakes](#arrl-sweekstakes)
+      - [The exchange parser](#the-exchange-parser)
+      - [The exchange](#the-exchange)
 
 ## What and why is Not1MM
 
 Not1MM's interface is a blantent ripoff of N1MM.
 It is NOT N1MM and any problem you have with this software should in no way reflect on their software.
 
 If you use Windows(tm) you should run away from this and use someother program.
@@ -103,24 +107,27 @@
 - General Logging
 - 10 10 Fall CW
 - 10 10 Spring CW
 - 10 10 Summer Phone
 - 10 10 Winter Phone
 - ARRL DX CW
 - ARRL DX SSB
+- ARRL Sweepstakes CW
+- ARRL Sweepstakes SSB
 - CQ WPX CW
 - CQ WPX SSB
 - CQ World Wide CW
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
+- [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
 <summary>April 2023</summary>
@@ -437,7 +444,33 @@
 Boom... ADIF
 
 `StationCall`_`ContestName`.adi
 
 ## Dupe checking
 
 Added dupe checking. Big Red 'Dupe' will appear if it's a dupe...
+
+## Contest specific notes
+
+I found it might be beneficial to have a section devoted to wierd quirky things about operating a specific contests.
+
+### ARRL Sweekstakes
+
+#### The exchange parser
+
+This was a pain in the tukus. There are so many elements to the exchange, and one input field aside from the callsign field. So I had to write sort of a 'parser'. The parser moves over your input string following some basic rules and is re-evaluated with each keypress and the parsed result will be displayed in the label over the field. The exchange looks like `124 A K6GTE 17 ORG`, a Serial number, Precidence, Callsign, Year Licenced and Section. even though the callsign is given as part of the exchange, the callsign does not have to be entered and is pulled from the callsign field. If the exchange was entered as `124 A 17 ORG` you would see:
+
+![SS Parser Result](https://github.com/mbridak/not1mm/raw/master/pic/ss_parser_1.png)
+
+You can enter the serial number and precidence, or the year and section as pairs. For instance `124A 17ORG`. This would ensure the values get parsed correctly.
+
+You do not have to go back to correct typing. You can just tack the correct items to the end of the field and the older values will get overwritten. So if you entered `124A 17ORG Q`, the precidence will change from A to Q. If you need to change the serial number you must append the precidence to it, `125A`.
+
+If the callsign was entered wrong in the callsign field, you can put the correct callsign some where in the exchange. As long as it shows up in the parsed label above correctly your good.
+
+The best thing you can do is play around with it to see how it behaves.
+
+#### The exchange
+
+In the `Sent Exchange` field of the New Contest dialog put in the Precidence, Call, Check and Section. Example: `A K6GTE 17 ORG`.
+
+For the Run Exchange macro I'd put `{HISCALL} # A K6GTE 17 ORG`.
```

### Comparing `not1mm-23.5.4/README.md` & `not1mm-23.5.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,18 @@
     - [Log Display](#log-display)
     - [Bandmap](#bandmap)
   - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
+  - [Contest specific notes](#contest-specific-notes)
+    - [ARRL Sweekstakes](#arrl-sweekstakes)
+      - [The exchange parser](#the-exchange-parser)
+      - [The exchange](#the-exchange)
 
 ## What and why is Not1MM
 
 Not1MM's interface is a blantent ripoff of N1MM.
 It is NOT N1MM and any problem you have with this software should in no way reflect on their software.
 
 If you use Windows(tm) you should run away from this and use someother program.
@@ -84,24 +88,27 @@
 - General Logging
 - 10 10 Fall CW
 - 10 10 Spring CW
 - 10 10 Summer Phone
 - 10 10 Winter Phone
 - ARRL DX CW
 - ARRL DX SSB
+- ARRL Sweepstakes CW
+- ARRL Sweepstakes SSB
 - CQ WPX CW
 - CQ WPX SSB
 - CQ World Wide CW
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
+- [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
 <summary>April 2023</summary>
@@ -418,7 +425,33 @@
 Boom... ADIF
 
 `StationCall`_`ContestName`.adi
 
 ## Dupe checking
 
 Added dupe checking. Big Red 'Dupe' will appear if it's a dupe...
+
+## Contest specific notes
+
+I found it might be beneficial to have a section devoted to wierd quirky things about operating a specific contests.
+
+### ARRL Sweekstakes
+
+#### The exchange parser
+
+This was a pain in the tukus. There are so many elements to the exchange, and one input field aside from the callsign field. So I had to write sort of a 'parser'. The parser moves over your input string following some basic rules and is re-evaluated with each keypress and the parsed result will be displayed in the label over the field. The exchange looks like `124 A K6GTE 17 ORG`, a Serial number, Precidence, Callsign, Year Licenced and Section. even though the callsign is given as part of the exchange, the callsign does not have to be entered and is pulled from the callsign field. If the exchange was entered as `124 A 17 ORG` you would see:
+
+![SS Parser Result](https://github.com/mbridak/not1mm/raw/master/pic/ss_parser_1.png)
+
+You can enter the serial number and precidence, or the year and section as pairs. For instance `124A 17ORG`. This would ensure the values get parsed correctly.
+
+You do not have to go back to correct typing. You can just tack the correct items to the end of the field and the older values will get overwritten. So if you entered `124A 17ORG Q`, the precidence will change from A to Q. If you need to change the serial number you must append the precidence to it, `125A`.
+
+If the callsign was entered wrong in the callsign field, you can put the correct callsign some where in the exchange. As long as it shows up in the parsed label above correctly your good.
+
+The best thing you can do is play around with it to see how it behaves.
+
+#### The exchange
+
+In the `Sent Exchange` field of the New Contest dialog put in the Precidence, Call, Check and Section. Example: `A K6GTE 17 ORG`.
+
+For the Run Exchange macro I'd put `{HISCALL} # A K6GTE 17 ORG`.
```

### Comparing `not1mm-23.5.4/not1mm/__main__.py` & `not1mm-23.5.5/not1mm/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,14 +240,15 @@
         self.score.setText("0")
         self.callsign.textEdited.connect(self.callsign_changed)
         self.callsign.returnPressed.connect(self.save_contact)
         self.sent.returnPressed.connect(self.save_contact)
         self.receive.returnPressed.connect(self.save_contact)
         self.other_1.returnPressed.connect(self.save_contact)
         self.other_2.returnPressed.connect(self.save_contact)
+        self.other_2.textEdited.connect(self.other_2_changed)
         self.sent.setText("59")
         self.receive.setText("59")
         icon_path = WORKING_PATH + "/data/"
         self.greendot = QtGui.QPixmap(icon_path + "greendot.png")
         self.reddot = QtGui.QPixmap(icon_path + "reddot.png")
         self.leftdot.setPixmap(self.greendot)
         self.rightdot.setPixmap(self.reddot)
@@ -855,14 +856,15 @@
         if self.contest:
             mults = self.contest.show_mults(self)
             qsos = self.contest.show_qso(self)
             multstring = f"{qsos}/{mults}"
             self.mults.setText(multstring)
             score = self.contest.calc_score(self)
             self.score.setText(str(score))
+            self.contest.reset_label(self)
         self.callsign.clear()
         if self.current_mode == "CW":
             self.sent.setText("599")
             self.receive.setText("599")
         else:
             self.sent.setText("59")
             self.receive.setText("59")
@@ -1540,14 +1542,20 @@
             return True
         try:
             _test = float(item)
         except ValueError:
             return False
         return True
 
+    def other_2_changed(self):
+        """Called when we need to parse SS exchange."""
+        if self.contest:
+            if "ARRL Sweepstakes" in self.contest.name:
+                self.contest.parse_exchange(self)
+
     def callsign_changed(self):
         """Called when text in the callsign field has changed"""
         text = self.callsign.text()
         text = text.upper()
         position = self.callsign.cursorPosition()
         stripped_text = text.strip().replace(" ", "")
         self.callsign.setText(stripped_text)
```

### Comparing `not1mm-23.5.4/not1mm/bandmap.py` & `not1mm-23.5.5/not1mm/bandmap.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/Combinear.qss` & `not1mm-23.5.5/not1mm/data/Combinear.qss`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-23.5.5/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/MASTER.SCP` & `not1mm-23.5.5/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/about.ui` & `not1mm-23.5.5/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/bandmap.ui` & `not1mm-23.5.5/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/configuration.ui` & `not1mm-23.5.5/not1mm/data/configuration.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/contests.sql` & `not1mm-23.5.5/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/cty.json` & `not1mm-23.5.5/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/editcontact.ui` & `not1mm-23.5.5/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/editmacro.ui` & `not1mm-23.5.5/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/k6gte.not1mm-128.png` & `not1mm-23.5.5/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/k6gte.not1mm-32.png` & `not1mm-23.5.5/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/k6gte.not1mm-64.png` & `not1mm-23.5.5/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/logwindow.ui` & `not1mm-23.5.5/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/main.ui` & `not1mm-23.5.5/not1mm/data/main.ui`

 * *Files 0% similar despite different names*

#### Comparing `not1mm-23.5.4/not1mm/data/main.ui` & `not1mm-23.5.5/not1mm/data/main.ui`

```diff
@@ -514,15 +514,15 @@
                         <item>
                           <widget class="QFrame" name="field4">
                             <layout class="QVBoxLayout" name="verticalLayout_2">
                               <property name="sizeConstraint">
                                 <enum>QLayout::SetDefaultConstraint</enum>
                               </property>
                               <item>
-                                <widget class="QLabel" name="label">
+                                <widget class="QLabel" name="exch_label">
                                   <property name="text">
                                     <string>OTHER_2</string>
                                   </property>
                                   <property name="textFormat">
                                     <enum>Qt::AutoText</enum>
                                   </property>
                                   <property name="alignment">
```

### Comparing `not1mm-23.5.4/not1mm/data/new_contest.ui` & `not1mm-23.5.5/not1mm/data/new_contest.ui`

 * *Files 0% similar despite different names*

#### Comparing `not1mm-23.5.4/not1mm/data/new_contest.ui` & `not1mm-23.5.5/not1mm/data/new_contest.ui`

```diff
@@ -194,14 +194,24 @@
           <item>
             <property name="text">
               <string>ARRL Field Day</string>
             </property>
           </item>
           <item>
             <property name="text">
+              <string>ARRL SS CW</string>
+            </property>
+          </item>
+          <item>
+            <property name="text">
+              <string>ARRL SS PHONE</string>
+            </property>
+          </item>
+          <item>
+            <property name="text">
               <string>CQ WPX CW</string>
             </property>
           </item>
           <item>
             <property name="text">
               <string>CQ WPX SSB</string>
             </property>
@@ -238,15 +248,15 @@
           </item>
         </widget>
       </item>
       <item row="2" column="2">
         <widget class="QDateTimeEdit" name="dateTimeEdit">
           <property name="time">
             <time>
-              <hour>8</hour>
+              <hour>16</hour>
               <minute>0</minute>
               <second>0</second>
             </time>
           </property>
           <property name="maximumDateTime">
             <datetime>
               <hour>7</hour>
```

### Comparing `not1mm-23.5.4/not1mm/data/opon.ui` & `not1mm-23.5.5/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/0.wav` & `not1mm-23.5.5/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/1.wav` & `not1mm-23.5.5/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/2.wav` & `not1mm-23.5.5/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/3.wav` & `not1mm-23.5.5/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/4.wav` & `not1mm-23.5.5/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/5.wav` & `not1mm-23.5.5/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/6.wav` & `not1mm-23.5.5/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/7.wav` & `not1mm-23.5.5/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/73.wav` & `not1mm-23.5.5/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/8.wav` & `not1mm-23.5.5/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/9.wav` & `not1mm-23.5.5/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/a.wav` & `not1mm-23.5.5/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/again.wav` & `not1mm-23.5.5/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/b.wav` & `not1mm-23.5.5/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/c.wav` & `not1mm-23.5.5/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/contest.wav` & `not1mm-23.5.5/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/cq.wav` & `not1mm-23.5.5/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/d.wav` & `not1mm-23.5.5/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/e.wav` & `not1mm-23.5.5/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/f.wav` & `not1mm-23.5.5/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/g.wav` & `not1mm-23.5.5/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/h.wav` & `not1mm-23.5.5/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/i.wav` & `not1mm-23.5.5/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/j.wav` & `not1mm-23.5.5/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/k.wav` & `not1mm-23.5.5/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/k6gte.wav` & `not1mm-23.5.5/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/l.wav` & `not1mm-23.5.5/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/m.wav` & `not1mm-23.5.5/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/mynumber.wav` & `not1mm-23.5.5/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/n.wav` & `not1mm-23.5.5/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/nil.wav` & `not1mm-23.5.5/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/o.wav` & `not1mm-23.5.5/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/p.wav` & `not1mm-23.5.5/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/q.wav` & `not1mm-23.5.5/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/r.wav` & `not1mm-23.5.5/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/roger.wav` & `not1mm-23.5.5/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/s.wav` & `not1mm-23.5.5/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/space.wav` & `not1mm-23.5.5/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/t.wav` & `not1mm-23.5.5/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/thankyou.wav` & `not1mm-23.5.5/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-23.5.5/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/u.wav` & `not1mm-23.5.5/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/v.wav` & `not1mm-23.5.5/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/w.wav` & `not1mm-23.5.5/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/x.wav` & `not1mm-23.5.5/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/y.wav` & `not1mm-23.5.5/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/yourcall.wav` & `not1mm-23.5.5/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/phonetics/z.wav` & `not1mm-23.5.5/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/pickcontest.ui` & `not1mm-23.5.5/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/reddot.png` & `not1mm-23.5.5/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/data/settings.ui` & `not1mm-23.5.5/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/lib/cat_interface.py` & `not1mm-23.5.5/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/lib/cwinterface.py` & `not1mm-23.5.5/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/lib/database.py` & `not1mm-23.5.5/not1mm/lib/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -683,14 +683,42 @@
                     f"select count(*) as wpx_count from dxlog where  TS < '{time_stamp}' and WPXPrefix = '{wpx}' and ContestNR = {self.current_contest};"
                 )
                 return cursor.fetchone()
         except sqlite3.OperationalError as exception:
             logger.debug("%s", exception)
             return {}
 
+    def fetch_sect_exists(self, sect) -> dict:
+        """returns a dict key of sect_count"""
+        try:
+            with sqlite3.connect(self.database) as conn:
+                conn.row_factory = self.row_factory
+                cursor = conn.cursor()
+                cursor.execute(
+                    f"select count(*) as sect_count from dxlog where Sect = '{sect}' and ContestNR = {self.current_contest};"
+                )
+                return cursor.fetchone()
+        except sqlite3.OperationalError as exception:
+            logger.debug("%s", exception)
+            return {}
+
+    def fetch_sect_exists_before_me(self, sec, time_stamp) -> dict:
+        """returns a dict key of sect_count"""
+        try:
+            with sqlite3.connect(self.database) as conn:
+                conn.row_factory = self.row_factory
+                cursor = conn.cursor()
+                cursor.execute(
+                    f"select count(*) as sect_count from dxlog where  TS < '{time_stamp}' and Sect = '{sec}' and ContestNR = {self.current_contest};"
+                )
+                return cursor.fetchone()
+        except sqlite3.OperationalError as exception:
+            logger.debug("%s", exception)
+            return {}
+
     def check_dupe_on_band_mode(self, call, band, mode) -> dict:
         """Checks if a call is dupe on band/mode"""
         try:
             with sqlite3.connect(self.database) as conn:
                 conn.row_factory = self.row_factory
                 cursor = conn.cursor()
                 cursor.execute(
```

### Comparing `not1mm-23.5.4/not1mm/lib/edit_macro.py` & `not1mm-23.5.5/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/lib/edit_station.py` & `not1mm-23.5.5/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/lib/ham_utility.py` & `not1mm-23.5.5/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/lib/lookup.py` & `not1mm-23.5.5/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/lib/multicast.py` & `not1mm-23.5.5/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/lib/n1mm.py` & `not1mm-23.5.5/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/lib/settings.py` & `not1mm-23.5.5/not1mm/lib/settings.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.4/not1mm/logwindow.py` & `not1mm-23.5.5/not1mm/logwindow.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,14 +59,37 @@
     The main window
     """
 
     # dbname = DATA_PATH + "/ham.db"
     dbname = None
     edit_contact_dialog = None
     pref = {}
+    columns = {
+        0: "YYYY-MM-DD HH:MM:SS",
+        1: "Call",
+        2: "Freq",
+        3: "Snt",
+        4: "Rcv",
+        5: "SentNr",
+        6: "RcvNr",
+        7: "Exchange1",
+        8: "CK",
+        9: "Prec",
+        10: "Sect",
+        11: "WPX",
+        12: "Power",
+        13: "M1",
+        14: "ZN",
+        15: "M2",
+        16: "PFX",
+        17: "PTS",
+        18: "Name",
+        19: "Comment",
+        20: "UUID",
+    }
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._udpwatch = None
         self.udp_fifo = queue.Queue()
         self.load_pref()
         self.dbname = DATA_PATH + "/" + self.pref.get("current_database", "ham.db")
@@ -74,121 +97,54 @@
         self.database.current_contest = self.pref.get("contest", 0)
         self.contact = self.database.empty_contact
         data_path = WORKING_PATH + "/data/logwindow.ui"
         uic.loadUi(data_path, self)
         self.setWindowTitle(
             f"Log Display - {self.pref.get('current_database', 'ham.db')}"
         )
-        self.generalLog.setColumnCount(19)
-        self.focusedLog.setColumnCount(19)
+        self.generalLog.setColumnCount(len(self.columns))
+        self.focusedLog.setColumnCount(len(self.columns))
         icon_path = WORKING_PATH + "/data/"
         self.checkmark = QtGui.QPixmap(icon_path + "check.png")
         self.checkicon = QtGui.QIcon()
         self.checkicon.addPixmap(self.checkmark)
         self.generalLog.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         self.generalLog.customContextMenuRequested.connect(self.edit_contact_selected)
-        self.generalLog.setHorizontalHeaderItem(
-            0, QtWidgets.QTableWidgetItem("YYYY-MM-DD HH:MM:SS")
-        )
-        self.generalLog.verticalHeader().setVisible(False)
-        self.generalLog.setHorizontalHeaderItem(1, QtWidgets.QTableWidgetItem("Call"))
-        self.generalLog.setHorizontalHeaderItem(2, QtWidgets.QTableWidgetItem("Freq"))
-        self.generalLog.setHorizontalHeaderItem(3, QtWidgets.QTableWidgetItem("Snt"))
-        self.generalLog.setHorizontalHeaderItem(4, QtWidgets.QTableWidgetItem("Rcv"))
-        self.generalLog.setHorizontalHeaderItem(5, QtWidgets.QTableWidgetItem("SentNr"))
-        self.generalLog.setHorizontalHeaderItem(6, QtWidgets.QTableWidgetItem("RcvNr"))
-
-        self.generalLog.setHorizontalHeaderItem(
-            7, QtWidgets.QTableWidgetItem("Exchange1")
-        )
-        self.generalLog.setHorizontalHeaderItem(8, QtWidgets.QTableWidgetItem("Sect"))
+        for column_number, column_name in self.columns.items():
+            self.generalLog.setHorizontalHeaderItem(
+                column_number, QtWidgets.QTableWidgetItem(column_name)
+            )
+            self.focusedLog.setHorizontalHeaderItem(
+                column_number, QtWidgets.QTableWidgetItem(column_name)
+            )
 
-        self.generalLog.setHorizontalHeaderItem(9, QtWidgets.QTableWidgetItem("WPX"))
-        self.generalLog.setHorizontalHeaderItem(10, QtWidgets.QTableWidgetItem("Power"))
-        self.generalLog.setHorizontalHeaderItem(11, QtWidgets.QTableWidgetItem("M1"))
-        self.generalLog.setHorizontalHeaderItem(12, QtWidgets.QTableWidgetItem("ZN"))
-        self.generalLog.setHorizontalHeaderItem(13, QtWidgets.QTableWidgetItem("M2"))
-        self.generalLog.setHorizontalHeaderItem(14, QtWidgets.QTableWidgetItem("PFX"))
-        self.generalLog.setHorizontalHeaderItem(15, QtWidgets.QTableWidgetItem("PTS"))
-        self.generalLog.setHorizontalHeaderItem(16, QtWidgets.QTableWidgetItem("Name"))
-        self.generalLog.setHorizontalHeaderItem(
-            17, QtWidgets.QTableWidgetItem("Comment")
-        )
-        self.generalLog.setHorizontalHeaderItem(18, QtWidgets.QTableWidgetItem("UUID"))
-        self.generalLog.setColumnWidth(0, 200)
-        self.generalLog.setColumnWidth(3, 50)
-        self.generalLog.setColumnWidth(4, 50)
-        self.generalLog.setColumnWidth(5, 75)
-        self.generalLog.setColumnWidth(6, 75)
-
-        self.generalLog.setColumnWidth(9, 50)
-        self.generalLog.setColumnWidth(10, 50)
-        self.generalLog.setColumnWidth(11, 50)
-        self.generalLog.setColumnWidth(12, 50)
-        self.generalLog.setColumnWidth(15, 50)
-        self.generalLog.setColumnWidth(16, 75)
-        self.generalLog.setColumnWidth(17, 200)
         self.generalLog.cellDoubleClicked.connect(self.double_clicked)
         self.generalLog.cellChanged.connect(self.cell_changed)
-        # self.generalLog.setColumnHidden(11, True)
-        # self.generalLog.setColumnHidden(12, True)
-        # self.generalLog.setColumnHidden(13, True)
-        self.generalLog.setColumnHidden(18, True)
 
         self.focusedLog.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         self.focusedLog.customContextMenuRequested.connect(
             self.edit_focused_contact_selected
         )
-        self.focusedLog.setHorizontalHeaderItem(
-            0, QtWidgets.QTableWidgetItem("YYYY-MM-DD HH:MM:SS")
-        )
-        self.focusedLog.verticalHeader().setVisible(False)
-        self.focusedLog.setHorizontalHeaderItem(1, QtWidgets.QTableWidgetItem("Call"))
-        self.focusedLog.setHorizontalHeaderItem(2, QtWidgets.QTableWidgetItem("Freq"))
-        self.focusedLog.setHorizontalHeaderItem(3, QtWidgets.QTableWidgetItem("Snt"))
-        self.focusedLog.setHorizontalHeaderItem(4, QtWidgets.QTableWidgetItem("Rcv"))
-        self.focusedLog.setHorizontalHeaderItem(5, QtWidgets.QTableWidgetItem("SentNr"))
-        self.focusedLog.setHorizontalHeaderItem(6, QtWidgets.QTableWidgetItem("RcvNr"))
+        for log in (self.generalLog, self.focusedLog):
+            log.setColumnWidth(self.get_column("YYYY-MM-DD HH:MM:SS"), 200)
+            log.setColumnWidth(self.get_column("Snt"), 50)
+            log.setColumnWidth(self.get_column("Rcv"), 50)
+            log.setColumnWidth(self.get_column("SentNr"), 75)
+            log.setColumnWidth(self.get_column("RcvNr"), 75)
+
+            log.setColumnWidth(self.get_column("WPX"), 50)
+            log.setColumnWidth(self.get_column("Power"), 50)
+            log.setColumnWidth(self.get_column("M1"), 50)
+            log.setColumnWidth(self.get_column("ZN"), 50)
+            log.setColumnWidth(self.get_column("PTS"), 50)
+            log.setColumnWidth(self.get_column("Name"), 75)
+            log.setColumnWidth(self.get_column("Comment"), 200)
+            log.setColumnHidden(self.get_column("UUID"), True)
+            log.verticalHeader().setVisible(False)
 
-        self.focusedLog.setHorizontalHeaderItem(
-            7, QtWidgets.QTableWidgetItem("Exchange1")
-        )
-        self.focusedLog.setHorizontalHeaderItem(8, QtWidgets.QTableWidgetItem("Sect"))
-
-        self.focusedLog.setHorizontalHeaderItem(9, QtWidgets.QTableWidgetItem("WPX"))
-        self.focusedLog.setHorizontalHeaderItem(10, QtWidgets.QTableWidgetItem("Power"))
-        self.focusedLog.setHorizontalHeaderItem(11, QtWidgets.QTableWidgetItem("M1"))
-        self.focusedLog.setHorizontalHeaderItem(12, QtWidgets.QTableWidgetItem("ZN"))
-        self.focusedLog.setHorizontalHeaderItem(13, QtWidgets.QTableWidgetItem("M2"))
-        self.focusedLog.setHorizontalHeaderItem(14, QtWidgets.QTableWidgetItem("PFX"))
-        self.focusedLog.setHorizontalHeaderItem(15, QtWidgets.QTableWidgetItem("PTS"))
-        self.focusedLog.setHorizontalHeaderItem(16, QtWidgets.QTableWidgetItem("Name"))
-        self.focusedLog.setHorizontalHeaderItem(
-            17, QtWidgets.QTableWidgetItem("Comment")
-        )
-        self.focusedLog.setHorizontalHeaderItem(18, QtWidgets.QTableWidgetItem("UUID"))
-        self.focusedLog.setColumnWidth(0, 200)
-        self.focusedLog.setColumnWidth(3, 50)
-        self.focusedLog.setColumnWidth(4, 50)
-        self.focusedLog.setColumnWidth(5, 75)
-        self.focusedLog.setColumnWidth(6, 75)
-
-        self.focusedLog.setColumnWidth(9, 50)
-        self.focusedLog.setColumnWidth(10, 50)
-        self.focusedLog.setColumnWidth(11, 50)
-        self.focusedLog.setColumnWidth(12, 50)
-        self.focusedLog.setColumnWidth(15, 50)
-        self.focusedLog.setColumnWidth(16, 75)
-        self.focusedLog.setColumnWidth(17, 200)
-        # self.focusedLog.cellDoubleClicked.connect(self.double_clicked)
-        # self.focusedLog.cellChanged.connect(self.cell_changed)
-        # self.focusedLog.setColumnHidden(11, True)
-        # self.focusedLog.setColumnHidden(12, True)
-        # self.focusedLog.setColumnHidden(13, True)
-        self.focusedLog.setColumnHidden(18, True)
         self.get_log()
         self.multicast_interface = Multicast(
             MULTICAST_GROUP, MULTICAST_PORT, INTERFACE_IP
         )
 
         if self._udpwatch is None:
             self._udpwatch = threading.Thread(
@@ -201,14 +157,20 @@
         self.multicast_interface.send_as_json(cmd)
         # self.n1mm = N1MM(
         #     ip_address=self.preference.get("n1mm_ip"),
         #     radioport=self.preference.get("n1mm_radioport"),
         #     contactport=self.preference.get("n1mm_contactport"),
         # )
 
+    def get_column(self, name: str) -> int:
+        """returns the column number of the given column name."""
+        for key, value in self.columns.items():
+            if value == name:
+                return key
+
     def load_pref(self):
         """Load preference file to get current db filename."""
         try:
             if os.path.exists(CONFIG_PATH + "/not1mm.json"):
                 with open(
                     CONFIG_PATH + "/not1mm.json", "rt", encoding="utf-8"
                 ) as file_descriptor:
@@ -239,53 +201,59 @@
         logger.debug("DoubleClicked")
 
     def cell_changed(self, row, column):
         """Slot for changed cell"""
         if self.table_loading:
             return
         db_record = {
-            "TS": self.generalLog.item(row, 0).text(),
-            "Call": self.generalLog.item(row, 1).text().upper(),
-            "Freq": self.generalLog.item(row, 2).text(),
-            "SNT": self.generalLog.item(row, 3).text(),
-            "RCV": self.generalLog.item(row, 4).text(),
-            "SentNr": self.generalLog.item(row, 5).text(),
-            "NR": self.generalLog.item(row, 6).text(),
-            "Exchange1": self.generalLog.item(row, 7).text(),
-            "Sect": self.generalLog.item(row, 8).text(),
-            "WPXPrefix": self.generalLog.item(row, 9).text(),
-            "Power": self.generalLog.item(row, 10).text(),
-            "IsMultiplier1": self.generalLog.item(row, 11).text(),
-            "ZN": self.generalLog.item(row, 12).text(),
-            "IsMultiplier2": self.generalLog.item(row, 13).text().upper(),
-            "CountryPrefix": self.generalLog.item(row, 14).text(),
-            "Points": self.generalLog.item(row, 15).text(),
-            "Name": self.generalLog.item(row, 16).text(),
-            "Comment": self.generalLog.item(row, 17).text(),
-            "ID": self.generalLog.item(row, 18).text(),
+            "TS": self.generalLog.item(
+                row, self.get_column("YYYY-MM-DD HH:MM:SS")
+            ).text(),
+            "Call": self.generalLog.item(row, self.get_column("Call")).text().upper(),
+            "Freq": self.generalLog.item(row, self.get_column("Freq")).text(),
+            "SNT": self.generalLog.item(row, self.get_column("Snt")).text(),
+            "RCV": self.generalLog.item(row, self.get_column("Rcv")).text(),
+            "SentNr": self.generalLog.item(row, self.get_column("SentNr")).text(),
+            "NR": self.generalLog.item(row, self.get_column("RcvNr")).text(),
+            "Exchange1": self.generalLog.item(row, self.get_column("Exchange1")).text(),
+            "CK": self.generalLog.item(row, self.get_column("CK")).text(),
+            "Prec": self.generalLog.item(row, self.get_column("Prec")).text(),
+            "Sect": self.generalLog.item(row, self.get_column("Sect")).text(),
+            "WPXPrefix": self.generalLog.item(row, self.get_column("WPX")).text(),
+            "Power": self.generalLog.item(row, self.get_column("Power")).text(),
+            "IsMultiplier1": self.generalLog.item(row, self.get_column("M1")).text(),
+            "ZN": self.generalLog.item(row, self.get_column("ZN")).text(),
+            "IsMultiplier2": self.generalLog.item(row, self.get_column("M2"))
+            .text()
+            .upper(),
+            "CountryPrefix": self.generalLog.item(row, self.get_column("PFX")).text(),
+            "Points": self.generalLog.item(row, self.get_column("PTS")).text(),
+            "Name": self.generalLog.item(row, self.get_column("Name")).text(),
+            "Comment": self.generalLog.item(row, self.get_column("Comment")).text(),
+            "ID": self.generalLog.item(row, self.get_column("UUID")).text(),
         }
         self.database.change_contact(db_record)
         self.get_log()
         self.generalLog.scrollToItem(self.generalLog.item(row, column))
 
     def dummy(self):
         """the dummy"""
 
     def edit_focused_contact_selected(self, clicked_cell):
         """Show edit contact dialog"""
         logger.debug("Opening EditContact dialog")
         item = self.focusedLog.itemAt(clicked_cell)
-        uuid = self.focusedLog.item(item.row(), 18).text()
+        uuid = self.focusedLog.item(item.row(), self.get_column("UUID")).text()
         self.edit_contact(uuid)
 
     def edit_contact_selected(self, clicked_cell):
         """Show edit contact dialog"""
         logger.debug("Opening EditContact dialog")
         item = self.generalLog.itemAt(clicked_cell)
-        uuid = self.generalLog.item(item.row(), 18).text()
+        uuid = self.generalLog.item(item.row(), self.get_column("UUID")).text()
         self.edit_contact(uuid)
 
     def edit_contact(self, uuid):
         """Show edit contact dialog"""
         logger.debug("Edit: %s", uuid)
         self.edit_contact_dialog = EditContact(WORKING_PATH)
         self.edit_contact_dialog.accepted.connect(self.save_edited_contact)
@@ -417,126 +385,132 @@
         current_log = self.database.fetch_all_contacts_asc()
         self.generalLog.setRowCount(0)
         for log_item in current_log:
             number_of_rows = self.generalLog.rowCount()
             self.generalLog.insertRow(number_of_rows)
             time_stamp = log_item.get("TS", "YY-MM-DD HH:MM:SS")
             first_item = QtWidgets.QTableWidgetItem(time_stamp)
-            self.generalLog.setItem(number_of_rows, 0, first_item)
+            self.generalLog.setItem(
+                number_of_rows, self.get_column("YYYY-MM-DD HH:MM:SS"), first_item
+            )
             self.generalLog.setCurrentItem(first_item, QItemSelectionModel.NoUpdate)
-            self.generalLog.item(number_of_rows, 0).setTextAlignment(0x0004 | 0x0080)
+            self.generalLog.item(
+                number_of_rows, self.get_column("YYYY-MM-DD HH:MM:SS")
+            ).setTextAlignment(0x0004 | 0x0080)
 
             self.generalLog.setItem(
                 number_of_rows,
-                1,
+                self.get_column("Call"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("Call", ""))),
             )
             freq = log_item.get("Freq", "")
             self.generalLog.setItem(
                 number_of_rows,
-                2,
+                self.get_column("Freq"),
                 QtWidgets.QTableWidgetItem(str(round(float(freq), 2))),
             )
             self.generalLog.setItem(
                 number_of_rows,
-                3,
+                self.get_column("Snt"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("SNT", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
-                4,
+                self.get_column("Rcv"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("RCV", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
-                5,
+                self.get_column("SentNr"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("SentNr", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
-                6,
+                self.get_column("RcvNr"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("NR", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
-                7,
+                self.get_column("Exchange1"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("Exchange1", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
-                8,
+                self.get_column("CK"),
+                QtWidgets.QTableWidgetItem(str(log_item.get("CK", ""))),
+            )
+            self.generalLog.setItem(
+                number_of_rows,
+                self.get_column("Prec"),
+                QtWidgets.QTableWidgetItem(str(log_item.get("Prec", ""))),
+            )
+            self.generalLog.setItem(
+                number_of_rows,
+                self.get_column("Sect"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("Sect", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
-                9,
+                self.get_column("WPX"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("WPXPrefix", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
-                10,
+                self.get_column("Power"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("Power", ""))),
             )
             item = QtWidgets.QTableWidgetItem()
             if log_item.get("IsMultiplier1", False):
                 item.setIcon(self.checkicon)
             self.generalLog.setItem(
                 number_of_rows,
-                11,
+                self.get_column("M1"),
                 item,
             )
             self.generalLog.setItem(
                 number_of_rows,
-                12,
+                self.get_column("ZN"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("ZN", ""))),
             )
             item = QtWidgets.QTableWidgetItem()
             if log_item.get("IsMultiplier2", False):
                 item.setIcon(self.checkicon)
             self.generalLog.setItem(
                 number_of_rows,
-                13,
+                self.get_column("M2"),
                 item,
             )
             self.generalLog.setItem(
                 number_of_rows,
-                14,
+                self.get_column("PFX"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("CountryPrefix", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
-                15,
+                self.get_column("PTS"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("Points", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
-                16,
+                self.get_column("Name"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("Name", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
-                17,
+                self.get_column("Comment"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("Comment", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
-                18,
+                self.get_column("UUID"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("ID", ""))),
             )
         self.table_loading = False
         self.generalLog.cellChanged.connect(self.cell_changed)
 
-    # def testing(self, a):
-    #     """ignore"""
-    #     item = self.generalLog.itemAt(a)
-    #     if item:
-    #         print(
-    #             f"{item.row()}, {item.column()} {item.icon().isNull()}*TESTING*"
-    #         )
-
     def watch_udp(self):
         """Puts UDP datagrams in a FIFO queue"""
         while True:
             try:
                 datagram = self.multicast_interface.server_udp.recv(1500)
                 logger.debug(datagram.decode())
             except socket.timeout:
@@ -555,118 +529,130 @@
         logger.debug(debug_line)
         self.focusedLog.setRowCount(0)
         for log_item in lines:
             number_of_rows = self.focusedLog.rowCount()
             self.focusedLog.insertRow(number_of_rows)
             time_stamp = log_item.get("TS", "YY-MM-DD HH:MM:SS")
             first_item = QtWidgets.QTableWidgetItem(time_stamp)
-            self.focusedLog.setItem(number_of_rows, 0, first_item)
+            self.focusedLog.setItem(
+                number_of_rows, self.get_column("YYYY-MM-DD HH:MM:SS"), first_item
+            )
             self.focusedLog.setCurrentItem(first_item, QItemSelectionModel.NoUpdate)
             try:
-                self.focusedLog.item(number_of_rows, 0).setTextAlignment(
-                    0x0004 | 0x0080
-                )
+                self.focusedLog.item(
+                    number_of_rows, self.get_column("YYYY-MM-DD HH:MM:SS")
+                ).setTextAlignment(0x0004 | 0x0080)
             except AttributeError:
                 ...
             self.focusedLog.setItem(
                 number_of_rows,
-                1,
+                self.get_column("Call"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("Call", ""))),
             )
             freq = log_item.get("Freq", "")
             self.focusedLog.setItem(
                 number_of_rows,
-                2,
+                self.get_column("Freq"),
                 QtWidgets.QTableWidgetItem(str(round(float(freq), 2))),
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                3,
+                self.get_column("Snt"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("SNT", ""))),
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                4,
+                self.get_column("Rcv"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("RCV", ""))),
             )
 
             self.focusedLog.setItem(
                 number_of_rows,
-                5,
+                self.get_column("SentNr"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("SentNr", ""))),
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                6,
+                self.get_column("RcvNr"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("NR", ""))),
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                7,
+                self.get_column("Exchange1"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("Exchange1", ""))),
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                8,
+                self.get_column("CK"),
+                QtWidgets.QTableWidgetItem(str(log_item.get("CK", ""))),
+            )
+            self.focusedLog.setItem(
+                number_of_rows,
+                self.get_column("Prec"),
+                QtWidgets.QTableWidgetItem(str(log_item.get("Prec", ""))),
+            )
+            self.focusedLog.setItem(
+                number_of_rows,
+                self.get_column("Sect"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("Sect", ""))),
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                9,
+                self.get_column("WPX"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("WPXPrefix", ""))),
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                10,
+                self.get_column("Power"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("Power", ""))),
             )
             item = QtWidgets.QTableWidgetItem()
             if log_item.get("IsMultiplier1", False):
                 item.setIcon(self.checkicon)
             self.focusedLog.setItem(
                 number_of_rows,
-                11,
+                self.get_column("M1"),
                 item,
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                12,
+                self.get_column("ZN"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("ZN", ""))),
             )
             item = QtWidgets.QTableWidgetItem()
             if log_item.get("IsMultiplier2", False):
                 item.setIcon(self.checkicon)
             self.focusedLog.setItem(
                 number_of_rows,
-                13,
+                self.get_column("M2"),
                 item,
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                14,
+                self.get_column("PFX"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("CountryPrefix", ""))),
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                15,
+                self.get_column("PTS"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("Points", ""))),
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                16,
+                self.get_column("Name"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("Name", ""))),
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                17,
+                self.get_column("Comment"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("Comment", ""))),
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                18,
+                self.get_column("UUID"),
                 QtWidgets.QTableWidgetItem(str(log_item.get("ID", ""))),
             )
 
     def check_udp_traffic(self):
         """Checks UDP Traffic"""
         while not self.udp_fifo.empty():
             datagram = self.udp_fifo.get()
@@ -687,22 +673,21 @@
                 self.get_log()
             if json_data.get("cmd", "") == "CALLCHANGED":
                 call = json_data.get("call", "")
                 self.show_like_calls(call)
             if json_data.get("cmd", "") == "NEWDB":
                 self.load_new_db()
             if json_data.get("cmd", "") == "SHOWCOLUMNS":
+                for column in range(len(self.columns)):
+                    self.generalLog.setColumnHidden(column, True)
+                    self.focusedLog.setColumnHidden(column, True)
                 columns_to_show = json_data.get("COLUMNS", [])
-                for column in range(18):
-                    if column in columns_to_show:
-                        self.generalLog.setColumnHidden(column, False)
-                        self.focusedLog.setColumnHidden(column, False)
-                    else:
-                        self.generalLog.setColumnHidden(column, True)
-                        self.focusedLog.setColumnHidden(column, True)
+                for column in columns_to_show:
+                    self.generalLog.setColumnHidden(self.get_column(column), False)
+                    self.focusedLog.setColumnHidden(self.get_column(column), False)
 
 
 def load_fonts_from_dir(directory: str) -> set:
     """
     Well it loads fonts from a directory...
     """
     font_families = set()
```

### Comparing `not1mm-23.5.4/not1mm/plugins/10_10_fall_cw.py` & `not1mm-23.5.5/not1mm/plugins/arrl_field_day.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,128 +1,136 @@
-"""10 10 fall cw plugin"""
+"""ARRL Field Day plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
-from pathlib import Path
 
+from pathlib import Path
 from PyQt5 import QtWidgets
+
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
-name = "10 10 FALL CW"
-cabrillo_name = "10-10-FALL-CW"
-mode = "CW"  # CW SSB BOTH RTTY
-columns = [0, 1, 2, 3, 4, 5, 6, 15]
+name = "ARRL Field Day"
+mode = "BOTH"  # CW SSB BOTH RTTY
+cabrillo_name = "ARRL-FD"
+
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "SentNr",
+    "RcvNr",
+    "Exchange1",
+    "CK",
+    "Prec",
+    "Sect",
+    "WPX",
+    "Power",
+    "M1",
+    "ZN",
+    "M2",
+    "PFX",
+    "PTS",
+    "Name",
+    "Comment",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
-dupe_type = 1
+dupe_type = 3
 
 
 def init_contest(self):
     """setup plugin"""
     set_tab_next(self)
     set_tab_prev(self)
     interface(self)
-    self.next_field = self.other_2
+    self.next_field = self.other_1
 
 
 def interface(self):
     """Setup user interface"""
-    self.field1.show()
-    self.field2.show()
-    self.field3.hide()
+    self.field1.hide()
+    self.field2.hide()
+    self.field3.show()
     self.field4.show()
+    label = self.field3.findChild(QtWidgets.QLabel)
+    label.setText("Class")
     label = self.field4.findChild(QtWidgets.QLabel)
-    label.setText("Name 1010# SPC")
+    label.setText("Section")
+
+
+def reset_label(self):
+    """reset label after field cleared"""
 
 
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
-        self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
-        self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
+        self.callsign: self.field3.findChild(QtWidgets.QLineEdit),
+        self.field1.findChild(QtWidgets.QLineEdit): self.field3.findChild(
             QtWidgets.QLineEdit
         ),
-        self.field2.findChild(QtWidgets.QLineEdit): self.field4.findChild(
+        self.field2.findChild(QtWidgets.QLineEdit): self.field3.findChild(
+            QtWidgets.QLineEdit
+        ),
+        self.field3.findChild(QtWidgets.QLineEdit): self.field4.findChild(
             QtWidgets.QLineEdit
         ),
-        self.field3.findChild(QtWidgets.QLineEdit): self.callsign,
         self.field4.findChild(QtWidgets.QLineEdit): self.callsign,
     }
 
 
 def set_tab_prev(self):
     """Set TAB Advances"""
     self.tab_prev = {
         self.callsign: self.field4.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.callsign,
-        self.field2.findChild(QtWidgets.QLineEdit): self.field1.findChild(
-            QtWidgets.QLineEdit
-        ),
-        self.field3.findChild(QtWidgets.QLineEdit): self.field2.findChild(
-            QtWidgets.QLineEdit
-        ),
-        self.field4.findChild(QtWidgets.QLineEdit): self.field2.findChild(
+        self.field2.findChild(QtWidgets.QLineEdit): self.callsign,
+        self.field3.findChild(QtWidgets.QLineEdit): self.callsign,
+        self.field4.findChild(QtWidgets.QLineEdit): self.field3.findChild(
             QtWidgets.QLineEdit
         ),
     }
 
 
-def validate(self):
-    """doc"""
-    exchange = self.other_2.text().upper().split()
-    if len(exchange) == 3:
-        if exchange[0].isalpha() and exchange[1].isdigit() and exchange[2].isalpha():
-            return True
-    return False
-
-
 def set_contact_vars(self):
     """Contest Specific"""
     self.contact["SNT"] = self.sent.text()
     self.contact["RCV"] = self.receive.text()
-    self.contact["NR"] = self.other_2.text().upper()
-    self.contact["SentNr"] = self.contest_settings.get("SentExchange", 0)
-    exchange = self.other_2.text().upper().split()
-    if len(exchange) == 3:
-        self.contact["Name"] = exchange[0]
-        self.contact["Comment"] = name
-    if validate(self) is False:
-        self.show_message_box("The exchange was invalid.")
+    self.contact["Exchange1"] = self.other_1.text().upper()
+    self.contact["Sect"] = self.other_2.text().upper()
 
 
 def predupe(self):
     """called after callsign entered"""
 
 
 def prefill(self):
-    """Fill sentnr"""
-    # if len(self.other_2.text()) == 0:
-    #     self.other_2.setText(str(self.contact.get("ZN", "")))
-    self.other_1.setText(str(self.contest_settings.get("SentExchange", 0)))
+    """Fill SentNR"""
 
 
 def points(self):
     """Calc point"""
-    exchange = self.other_2.text().upper().split()
-    if len(exchange) == 3:
-        try:
-            tentennumber = exchange[1]
-            if int(tentennumber) > 0:
-                return 2
-            return 1
-        except ValueError:
-            ...
+    _mode = self.contact.get("Mode", "")
+    if _mode in "SSB, USB, LSB":
+        return 1
+    if _mode in "CW, RTTY":
+        return 2
     return 0
 
 
 def show_mults(self):
     """Return display string for mults"""
+    result = self.database.get_unique_band_and_mode()
+    if result:
+        return int(result.get("mult", 0))
     return 0
 
 
 def show_qso(self):
     """Return qso count"""
     result = self.database.fetch_qso_count()
     if result:
@@ -136,22 +144,17 @@
     if result:
         return int(result.get("Points", 0))
     return 0
 
 
 def calc_score(self):
     """Return calculated score"""
-    result = self.database.fetch_points()
-    if result is not None:
-        score = result.get("Points", "0")
-        if score is None:
-            score = "0"
-        contest_points = int(score)
-        return contest_points
-    return 0
+    _points = get_points(self)
+    _mults = show_mults(self)
+    return _points * _mults
 
 
 def adif(self):
     """
     Creates an ADIF file of the contacts made.
     """
     filename = (
@@ -168,16 +171,16 @@
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
                 frequency = str(contact.get("Freq", 0) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
-                sentnr = str(contact.get("SentNr", ""))
-                rcvnr = str(contact.get("NR", ""))
+                sentnr = self.contest_settings.get("SentExchange", "")
+                rcvnr = f"{contact.get('Exchange1', '')} {contact.get('Sect', '')}"
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
                 loggedtime = the_date_and_time[11:13] + the_date_and_time[14:16]
                 print(
                     f"<QSO_DATE:{len(''.join(loggeddate.split('-')))}:d>"
                     f"{''.join(loggeddate.split('-'))}",
@@ -339,15 +342,15 @@
 
             print(
                 f"CLAIMED-SCORE: {calc_score(self)}",
                 end="\r\n",
                 file=file_descriptor,
             )
             print(
-                f"OPERATORS: {self.contest_settings.get('Operators','')}",
+                "OPERATORS: ",
                 end="\r\n",
                 file=file_descriptor,
             )
             print(
                 f"NAME: {self.station.get('Name', '')}",
                 end="\r\n",
                 file=file_descriptor,
@@ -390,19 +393,18 @@
                 frequency = str(int(contact.get("Freq", "0"))).rjust(5)
 
                 loggeddate = the_date_and_time[:10]
                 loggedtime = the_date_and_time[11:13] + the_date_and_time[14:16]
                 print(
                     f"QSO: {frequency} {themode} {loggeddate} {loggedtime} "
                     f"{contact.get('StationPrefix', '').ljust(13)} "
-                    f"{str(contact.get('SNT', '')).ljust(3)} "
-                    f"{str(contact.get('SentNr', '')).ljust(6)} "
+                    f"{self.contest_settings.get('SentExchange', '').ljust(9)}"
                     f"{contact.get('Call', '').ljust(13)} "
-                    f"{str(contact.get('RCV', '')).ljust(3)} "
-                    f"{str(contact.get('NR', '')).ljust(6)}",
+                    f"{str(contact.get('Exchange1', '')).ljust(3)} "
+                    f"{str(contact.get('Sect', '')).ljust(6)}",
                     end="\r\n",
                     file=file_descriptor,
                 )
             print("END-OF-LOG:", end="\r\n", file=file_descriptor)
     except IOError as exception:
         logger.critical("cabrillo: IO error: %s, writing to %s", exception, filename)
         return
```

### Comparing `not1mm-23.5.4/not1mm/plugins/10_10_spring_cw.py` & `not1mm-23.5.5/not1mm/plugins/10_10_winter_phone.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,33 @@
-"""10 10 spring cw plugin"""
+"""10 10 winter phone plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
 from pathlib import Path
 
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
-name = "10 10 SPRING CW"
-cabrillo_name = "10-10-SPRING-CW"
-mode = "CW"  # CW SSB BOTH RTTY
-columns = [0, 1, 2, 3, 4, 5, 6, 15]
+name = "10 10 WINTER PHONE"
+cabrillo_name = "10-10-SPRING-PHONE"
+mode = "SSB"  # CW SSB BOTH RTTY
+# columns = [0, 1, 2, 3, 4, 5, 6, 15]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "SentNr",
+    "RcvNr",
+    "PTS",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 1
 
 
 def init_contest(self):
     """setup plugin"""
@@ -33,14 +43,18 @@
     self.field2.show()
     self.field3.hide()
     self.field4.show()
     label = self.field4.findChild(QtWidgets.QLabel)
     label.setText("Name 1010# SPC")
 
 
+def reset_label(self):
+    """reset label after field cleared"""
+
+
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
```

### Comparing `not1mm-23.5.4/not1mm/plugins/10_10_summer_phone.py` & `not1mm-23.5.5/not1mm/plugins/10_10_fall_cw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,33 @@
-"""10 10 summer cw plugin"""
+"""10 10 fall cw plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
 from pathlib import Path
 
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
-name = "10 10 SUMMER PHONE"
-cabrillo_name = "10-10-SUMMER-PHONE"
-mode = "SSB"  # CW SSB BOTH RTTY
-columns = [0, 1, 2, 3, 4, 5, 6, 15]
+name = "10 10 FALL CW"
+cabrillo_name = "10-10-FALL-CW"
+mode = "CW"  # CW SSB BOTH RTTY
+# columns = [0, 1, 2, 3, 4, 5, 6, 15]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "SentNr",
+    "RcvNr",
+    "PTS",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 1
 
 
 def init_contest(self):
     """setup plugin"""
@@ -33,14 +43,18 @@
     self.field2.show()
     self.field3.hide()
     self.field4.show()
     label = self.field4.findChild(QtWidgets.QLabel)
     label.setText("Name 1010# SPC")
 
 
+def reset_label(self):
+    """reset label after field cleared"""
+
+
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
```

### Comparing `not1mm-23.5.4/not1mm/plugins/10_10_winter_phone.py` & `not1mm-23.5.5/not1mm/plugins/10_10_spring_cw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,33 @@
-"""10 10 winter phone plugin"""
+"""10 10 spring cw plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
 from pathlib import Path
 
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
-name = "10 10 WINTER PHONE"
-cabrillo_name = "10-10-SPRING-PHONE"
-mode = "SSB"  # CW SSB BOTH RTTY
-columns = [0, 1, 2, 3, 4, 5, 6, 15]
+name = "10 10 SPRING CW"
+cabrillo_name = "10-10-SPRING-CW"
+mode = "CW"  # CW SSB BOTH RTTY
+# columns = [0, 1, 2, 3, 4, 5, 6, 15]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "SentNr",
+    "RcvNr",
+    "PTS",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 1
 
 
 def init_contest(self):
     """setup plugin"""
@@ -33,14 +43,18 @@
     self.field2.show()
     self.field3.hide()
     self.field4.show()
     label = self.field4.findChild(QtWidgets.QLabel)
     label.setText("Name 1010# SPC")
 
 
+def reset_label(self):
+    """reset label after field cleared"""
+
+
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
```

### Comparing `not1mm-23.5.4/not1mm/plugins/arrl_dx_cw.py` & `not1mm-23.5.5/not1mm/plugins/arrl_dx_cw.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,26 @@
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "ARRL DX CW"
 cabrillo_name = "ARRL-DX-CW"
 mode = "CW"  # CW SSB BOTH RTTY
-columns = [0, 1, 2, 3, 4, 10, 11, 14, 15]
+# columns = [0, 1, 2, 3, 4, 10, 11, 14, 15]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "Power",
+    "M1",
+    "PFX",
+    "PTS",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 2
 
 
 def init_contest(self):
     """setup plugin"""
@@ -33,14 +44,18 @@
     self.field2.show()
     self.field3.hide()
     self.field4.show()
     label = self.field4.findChild(QtWidgets.QLabel)
     label.setText("Power")
 
 
+def reset_label(self):
+    """reset label after field cleared"""
+
+
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
```

### Comparing `not1mm-23.5.4/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-23.5.5/not1mm/plugins/arrl_dx_ssb.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,26 @@
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "ARRL DX SSB"
 cabrillo_name = "ARRL-DX-SSB"
 mode = "SSB"  # CW SSB BOTH RTTY
-columns = [0, 1, 2, 3, 4, 10, 11, 14, 15]
+# columns = [0, 1, 2, 3, 4, 10, 11, 14, 15]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "Power",
+    "M1",
+    "PFX",
+    "PTS",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 2
 
 
 def init_contest(self):
     """setup plugin"""
@@ -33,14 +44,18 @@
     self.field2.show()
     self.field3.hide()
     self.field4.show()
     label = self.field4.findChild(QtWidgets.QLabel)
     label.setText("Power")
 
 
+def reset_label(self):
+    """reset label after field cleared"""
+
+
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
```

### Comparing `not1mm-23.5.4/not1mm/plugins/arrl_field_day.py` & `not1mm-23.5.5/not1mm/plugins/10_10_summer_phone.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,110 +1,142 @@
-"""ARRL Field Day plugin"""
+"""10 10 summer cw plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 import logging
-
 from pathlib import Path
-from PyQt5 import QtWidgets
 
+from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
-name = "ARRL Field Day"
-mode = "BOTH"  # CW SSB BOTH RTTY
-cabrillo_name = "ARRL-FD"
-columns = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
+name = "10 10 SUMMER PHONE"
+cabrillo_name = "10-10-SUMMER-PHONE"
+mode = "SSB"  # CW SSB BOTH RTTY
+# columns = [0, 1, 2, 3, 4, 5, 6, 15]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "SentNr",
+    "RcvNr",
+    "PTS",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
-dupe_type = 3
+dupe_type = 1
 
 
 def init_contest(self):
     """setup plugin"""
     set_tab_next(self)
     set_tab_prev(self)
     interface(self)
-    self.next_field = self.other_1
+    self.next_field = self.other_2
 
 
 def interface(self):
     """Setup user interface"""
-    self.field1.hide()
-    self.field2.hide()
-    self.field3.show()
+    self.field1.show()
+    self.field2.show()
+    self.field3.hide()
     self.field4.show()
-    label = self.field3.findChild(QtWidgets.QLabel)
-    label.setText("Class")
     label = self.field4.findChild(QtWidgets.QLabel)
-    label.setText("Section")
+    label.setText("Name 1010# SPC")
+
+
+def reset_label(self):
+    """reset label after field cleared"""
 
 
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
-        self.callsign: self.field3.findChild(QtWidgets.QLineEdit),
-        self.field1.findChild(QtWidgets.QLineEdit): self.field3.findChild(
+        self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
+        self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
-        self.field2.findChild(QtWidgets.QLineEdit): self.field3.findChild(
-            QtWidgets.QLineEdit
-        ),
-        self.field3.findChild(QtWidgets.QLineEdit): self.field4.findChild(
+        self.field2.findChild(QtWidgets.QLineEdit): self.field4.findChild(
             QtWidgets.QLineEdit
         ),
+        self.field3.findChild(QtWidgets.QLineEdit): self.callsign,
         self.field4.findChild(QtWidgets.QLineEdit): self.callsign,
     }
 
 
 def set_tab_prev(self):
     """Set TAB Advances"""
     self.tab_prev = {
         self.callsign: self.field4.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.callsign,
-        self.field2.findChild(QtWidgets.QLineEdit): self.callsign,
-        self.field3.findChild(QtWidgets.QLineEdit): self.callsign,
-        self.field4.findChild(QtWidgets.QLineEdit): self.field3.findChild(
+        self.field2.findChild(QtWidgets.QLineEdit): self.field1.findChild(
+            QtWidgets.QLineEdit
+        ),
+        self.field3.findChild(QtWidgets.QLineEdit): self.field2.findChild(
+            QtWidgets.QLineEdit
+        ),
+        self.field4.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
     }
 
 
+def validate(self):
+    """doc"""
+    exchange = self.other_2.text().upper().split()
+    if len(exchange) == 3:
+        if exchange[0].isalpha() and exchange[1].isdigit() and exchange[2].isalpha():
+            return True
+    return False
+
+
 def set_contact_vars(self):
     """Contest Specific"""
     self.contact["SNT"] = self.sent.text()
     self.contact["RCV"] = self.receive.text()
-    self.contact["Exchange1"] = self.other_1.text().upper()
-    self.contact["Sect"] = self.other_2.text().upper()
+    self.contact["NR"] = self.other_2.text().upper()
+    self.contact["SentNr"] = self.contest_settings.get("SentExchange", 0)
+    exchange = self.other_2.text().upper().split()
+    if len(exchange) == 3:
+        self.contact["Name"] = exchange[0]
+        self.contact["Comment"] = name
+    if validate(self) is False:
+        self.show_message_box("The exchange was invalid.")
 
 
 def predupe(self):
     """called after callsign entered"""
 
 
 def prefill(self):
-    """Fill SentNR"""
+    """Fill sentnr"""
+    # if len(self.other_2.text()) == 0:
+    #     self.other_2.setText(str(self.contact.get("ZN", "")))
+    self.other_1.setText(str(self.contest_settings.get("SentExchange", 0)))
 
 
 def points(self):
     """Calc point"""
-    _mode = self.contact.get("Mode", "")
-    if _mode in "SSB, USB, LSB":
-        return 1
-    if _mode in "CW, RTTY":
-        return 2
+    exchange = self.other_2.text().upper().split()
+    if len(exchange) == 3:
+        try:
+            tentennumber = exchange[1]
+            if int(tentennumber) > 0:
+                return 2
+            return 1
+        except ValueError:
+            ...
     return 0
 
 
 def show_mults(self):
     """Return display string for mults"""
-    result = self.database.get_unique_band_and_mode()
-    if result:
-        return int(result.get("mult", 0))
     return 0
 
 
 def show_qso(self):
     """Return qso count"""
     result = self.database.fetch_qso_count()
     if result:
@@ -118,17 +150,22 @@
     if result:
         return int(result.get("Points", 0))
     return 0
 
 
 def calc_score(self):
     """Return calculated score"""
-    _points = get_points(self)
-    _mults = show_mults(self)
-    return _points * _mults
+    result = self.database.fetch_points()
+    if result is not None:
+        score = result.get("Points", "0")
+        if score is None:
+            score = "0"
+        contest_points = int(score)
+        return contest_points
+    return 0
 
 
 def adif(self):
     """
     Creates an ADIF file of the contacts made.
     """
     filename = (
@@ -145,16 +182,16 @@
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
                 frequency = str(contact.get("Freq", 0) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
-                sentnr = self.contest_settings.get("SentExchange", "")
-                rcvnr = f"{contact.get('Exchange1', '')} {contact.get('Sect', '')}"
+                sentnr = str(contact.get("SentNr", ""))
+                rcvnr = str(contact.get("NR", ""))
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
                 loggedtime = the_date_and_time[11:13] + the_date_and_time[14:16]
                 print(
                     f"<QSO_DATE:{len(''.join(loggeddate.split('-')))}:d>"
                     f"{''.join(loggeddate.split('-'))}",
@@ -316,15 +353,15 @@
 
             print(
                 f"CLAIMED-SCORE: {calc_score(self)}",
                 end="\r\n",
                 file=file_descriptor,
             )
             print(
-                "OPERATORS: ",
+                f"OPERATORS: {self.contest_settings.get('Operators','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             print(
                 f"NAME: {self.station.get('Name', '')}",
                 end="\r\n",
                 file=file_descriptor,
@@ -367,18 +404,19 @@
                 frequency = str(int(contact.get("Freq", "0"))).rjust(5)
 
                 loggeddate = the_date_and_time[:10]
                 loggedtime = the_date_and_time[11:13] + the_date_and_time[14:16]
                 print(
                     f"QSO: {frequency} {themode} {loggeddate} {loggedtime} "
                     f"{contact.get('StationPrefix', '').ljust(13)} "
-                    f"{self.contest_settings.get('SentExchange', '').ljust(9)}"
+                    f"{str(contact.get('SNT', '')).ljust(3)} "
+                    f"{str(contact.get('SentNr', '')).ljust(6)} "
                     f"{contact.get('Call', '').ljust(13)} "
-                    f"{str(contact.get('Exchange1', '')).ljust(3)} "
-                    f"{str(contact.get('Sect', '')).ljust(6)}",
+                    f"{str(contact.get('RCV', '')).ljust(3)} "
+                    f"{str(contact.get('NR', '')).ljust(6)}",
                     end="\r\n",
                     file=file_descriptor,
                 )
             print("END-OF-LOG:", end="\r\n", file=file_descriptor)
     except IOError as exception:
         logger.critical("cabrillo: IO error: %s, writing to %s", exception, filename)
         return
```

### Comparing `not1mm-23.5.4/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-23.5.5/not1mm/plugins/winter_field_day.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,62 @@
-"""ARRL plugin"""
+"""Winter Field Day plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 from PyQt5 import QtWidgets
 
-name = "ARRL RTTY Round Up"
-mode = "BOTH"  # CW SSB BOTH RTTY
-columns = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
-
+name = "Winter Field Day"
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
+mode = "BOTH"  # CW SSB BOTH RTTY
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "SentNr",
+    "RcvNr",
+    "Exchange1",
+    "CK",
+    "Prec",
+    "Sect",
+    "WPX",
+    "Power",
+    "M1",
+    "ZN",
+    "M2",
+    "PFX",
+    "PTS",
+    "Name",
+    "Comment",
+]
 dupe_type = 4
 
 
 def init_contest(self):
     """setup plugin"""
     set_tab_next(self)
     set_tab_prev(self)
     interface(self)
 
 
 def interface(self):
     """Setup user interface"""
+    self.field1.hide()
+    self.field2.hide()
+    self.field3.show()
+    self.field4.show()
+    label = self.field3.findChild(QtWidgets.QLabel)
+    label.setText("Class")
+    label = self.field4.findChild(QtWidgets.QLabel)
+    label.setText("Section")
+
+
+def reset_label(self):
+    """reset label after field cleared"""
 
 
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
```

### Comparing `not1mm-23.5.4/not1mm/plugins/arrl_ss_cw.py` & `not1mm-23.5.5/not1mm/plugins/arrl_rtty_ru.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,37 @@
 """ARRL plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 from PyQt5 import QtWidgets
 
-name = "ARRL Sweepstakes CW"
+name = "ARRL RTTY Round Up"
 mode = "BOTH"  # CW SSB BOTH RTTY
-columns = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "SentNr",
+    "RcvNr",
+    "Exchange1",
+    "CK",
+    "Prec",
+    "Sect",
+    "WPX",
+    "Power",
+    "M1",
+    "ZN",
+    "M2",
+    "PFX",
+    "PTS",
+    "Name",
+    "Comment",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 4
 
 
 def init_contest(self):
     """setup plugin"""
@@ -19,14 +40,18 @@
     interface(self)
 
 
 def interface(self):
     """Setup user interface"""
 
 
+def reset_label(self):
+    """reset label after field cleared"""
+
+
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
```

### Comparing `not1mm-23.5.4/not1mm/plugins/cq_wpx_cw.py` & `not1mm-23.5.5/not1mm/plugins/cq_wpx_ssb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,35 @@
-"""CQ WPX CW plugin"""
+"""CQ WPX SSB plugin"""
 
 # pylint: disable=invalid-name
 import logging
 from pathlib import Path
 
 from PyQt5 import QtWidgets
 
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
-name = "CQ WPX CW"
-cabrillo_name = "CQ-WPX-CW"
-mode = "CW"  # CW SSB BOTH RTTY
-columns = [0, 1, 2, 3, 4, 5, 6, 9, 11, 15]
+name = "CQ WPX SSB"
+cabrillo_name = "CQ-WPX-SSB"
+mode = "SSB"  # CW SSB BOTH RTTY
+# columns = [0, 1, 2, 3, 4, 5, 6, 9, 11, 15]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "SentNr",
+    "RcvNr",
+    "WPX",
+    "M1",
+    "PTS",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 2
 
 
 def init_contest(self):
     """setup plugin"""
@@ -35,14 +47,18 @@
     self.field4.show()
     label = self.field3.findChild(QtWidgets.QLabel)
     label.setText("SentNR")
     label = self.field4.findChild(QtWidgets.QLabel)
     label.setText("RcvNR")
 
 
+def reset_label(self):
+    """reset label after field cleared"""
+
+
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
```

### Comparing `not1mm-23.5.4/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-23.5.5/not1mm/plugins/cq_wpx_cw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,35 @@
-"""CQ WPX SSB plugin"""
+"""CQ WPX CW plugin"""
 
 # pylint: disable=invalid-name
 import logging
 from pathlib import Path
 
 from PyQt5 import QtWidgets
 
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
-name = "CQ WPX SSB"
-cabrillo_name = "CQ-WPX-SSB"
-mode = "SSB"  # CW SSB BOTH RTTY
-columns = [0, 1, 2, 3, 4, 5, 6, 9, 11, 15]
+name = "CQ WPX CW"
+cabrillo_name = "CQ-WPX-CW"
+mode = "CW"  # CW SSB BOTH RTTY
+# columns = [0, 1, 2, 3, 4, 5, 6, 9, 11, 15]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "SentNr",
+    "RcvNr",
+    "WPX",
+    "M1",
+    "PTS",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 2
 
 
 def init_contest(self):
     """setup plugin"""
@@ -35,14 +47,18 @@
     self.field4.show()
     label = self.field3.findChild(QtWidgets.QLabel)
     label.setText("SentNR")
     label = self.field4.findChild(QtWidgets.QLabel)
     label.setText("RcvNR")
 
 
+def reset_label(self):
+    """reset label after field cleared"""
+
+
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
```

### Comparing `not1mm-23.5.4/not1mm/plugins/cq_ww_cw.py` & `not1mm-23.5.5/not1mm/plugins/cq_ww_cw.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,25 @@
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "CQ WW CW"
 cabrillo_name = "CQ-WW-CW"
 mode = "CW"  # CW SSB BOTH RTTY
-columns = [0, 1, 2, 3, 4, 5, 6, 15]
+# columns = [0, 1, 2, 3, 4, 5, 6, 15]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "SentNr",
+    "RcvNr",
+    "PTS",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 2
 
 
 def init_contest(self):
     """setup plugin"""
@@ -33,14 +43,18 @@
     self.field2.show()
     self.field3.hide()
     self.field4.show()
     label = self.field4.findChild(QtWidgets.QLabel)
     label.setText("CQ Zone")
 
 
+def reset_label(self):
+    """reset label after field cleared"""
+
+
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
```

### Comparing `not1mm-23.5.4/not1mm/plugins/cq_ww_ssb.py` & `not1mm-23.5.5/not1mm/plugins/cq_ww_ssb.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,25 @@
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "CQ WW SSB"
 cabrillo_name = "CQ-WW-SSB"
 mode = "SSB"  # CW SSB BOTH RTTY
-# columns = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
-columns = [0, 1, 2, 3, 4, 5, 6, 15]
+# columns = [0, 1, 2, 3, 4, 5, 6, 15]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "SentNr",
+    "RcvNr",
+    "PTS",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 2
 
 
 def init_contest(self):
     """setup plugin"""
@@ -34,14 +43,18 @@
     self.field2.show()
     self.field3.hide()
     self.field4.show()
     label = self.field4.findChild(QtWidgets.QLabel)
     label.setText("CQ Zone")
 
 
+def reset_label(self):
+    """reset label after field cleared"""
+
+
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
```

### Comparing `not1mm-23.5.4/not1mm/plugins/cwt.py` & `not1mm-23.5.5/not1mm/plugins/cwt.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,26 @@
 
 from PyQt5 import QtWidgets
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 name = "CWT"
 mode = "CW"  # CW SSB BOTH RTTY
-columns = [0, 1, 2, 3, 4, 5, 6, 11, 15]
-# columns = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17]
+# columns = [0, 1, 2, 3, 4, 5, 6, 11, 15]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "SentNr",
+    "RcvNr",
+    "M1",
+    "PTS",
+]
 cabrillo_name = "CWOPS-CWT"
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 2
 
 
 def init_contest(self):
@@ -35,14 +45,18 @@
     self.field4.show()
     label = self.field3.findChild(QtWidgets.QLabel)
     label.setText("Name")
     label = self.field4.findChild(QtWidgets.QLabel)
     label.setText("ST/DX/#")
 
 
+def reset_label(self):
+    """reset label after field cleared"""
+
+
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
```

### Comparing `not1mm-23.5.4/not1mm/plugins/general_logging.py` & `not1mm-23.5.5/not1mm/plugins/general_logging.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,23 @@
 
 logger = logging.getLogger("__main__")
 
 name = "General Logging"
 cabrillo_name = "General-Logging"
 mode = "BOTH"  # CW SSB BOTH RTTY
 columns = [0, 1, 2, 3, 4, 16, 17]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "Name",
+    "Comment",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 4
 
 
 def init_contest(self):
     """setup plugin"""
@@ -35,14 +44,18 @@
     self.field4.show()
     label = self.field3.findChild(QtWidgets.QLabel)
     label.setText("Name")
     label = self.field4.findChild(QtWidgets.QLabel)
     label.setText("Comment")
 
 
+def reset_label(self):
+    """reset label after field cleared"""
+
+
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
```

### Comparing `not1mm-23.5.4/not1mm/plugins/jidx_cw.py` & `not1mm-23.5.5/not1mm/plugins/jidx_cw.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,26 @@
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "JIDX CW"
 cabrillo_name = "JIDX-CW"
 mode = "CW"  # CW SSB BOTH RTTY
-columns = [0, 1, 2, 3, 4, 5, 6, 11, 15]
+# columns = [0, 1, 2, 3, 4, 5, 6, 11, 15]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "SentNr",
+    "RcvNr",
+    "M1",
+    "PTS",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 2
 
 
 def init_contest(self):
     """setup plugin"""
@@ -35,14 +46,18 @@
     self.field4.show()
     label = self.field3.findChild(QtWidgets.QLabel)
     label.setText("SentNR")
     label = self.field4.findChild(QtWidgets.QLabel)
     label.setText("RcvNR")
 
 
+def reset_label(self):
+    """reset label after field cleared"""
+
+
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
```

### Comparing `not1mm-23.5.4/not1mm/plugins/jidx_ph.py` & `not1mm-23.5.5/not1mm/plugins/jidx_ph.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,26 @@
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "JIDX PH"
 cabrillo_name = "JIDX-PH"
 mode = "SSB"  # CW SSB BOTH RTTY
-columns = [0, 1, 2, 3, 4, 5, 6, 11, 15]
+# columns = [0, 1, 2, 3, 4, 5, 6, 11, 15]
+columns = [
+    "YYYY-MM-DD HH:MM:SS",
+    "Call",
+    "Freq",
+    "Snt",
+    "Rcv",
+    "SentNr",
+    "RcvNr",
+    "M1",
+    "PTS",
+]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 2
 
 
 def init_contest(self):
     """setup plugin"""
@@ -35,14 +46,18 @@
     self.field4.show()
     label = self.field3.findChild(QtWidgets.QLabel)
     label.setText("SentNR")
     label = self.field4.findChild(QtWidgets.QLabel)
     label.setText("RcvNR")
 
 
+def reset_label(self):
+    """reset label after field cleared"""
+
+
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
```

### Comparing `not1mm-23.5.4/not1mm/testing/test.py` & `not1mm-23.5.5/testing/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-"""Testing"""
-
-from json import loads
-
 import great_circle_calculator.great_circle_calculator as gcc
+from json import loads, dumps
 
 LOCATION = "/home/mbridak/Nextcloud/dev/not1mm/not1mm/data/cty.json"
 
 ctyfile = {}
 
-with open(LOCATION, "r", encoding="utf-8") as fd:
+with open(LOCATION, "r") as fd:
     ctyfile = loads(fd.read())
 
+""""""
+
 
 def cty_lookup(callsign: str):
-    """lookup"""
     callsign = callsign.upper()
-    for index in reversed(range(len(callsign))):
-        searchitem = callsign[: index + 1]
-        _result = {key: val for key, val in ctyfile.items() if key == searchitem}
-        if not _result:
+    for x in reversed(range(len(callsign))):
+        searchitem = callsign[: x + 1]
+        result = {key: val for key, val in ctyfile.items() if key == searchitem}
+        if not result:
             continue
-        if _result.get(searchitem).get("exact_match"):
+        if result.get(searchitem).get("exact_match"):
             if searchitem == callsign:
-                return _result
+                return result
             else:
                 continue
-        return _result
+        return result
 
 
 def gridtolatlon(maiden):
     """
     Converts a maidenhead gridsquare to a latitude longitude pair.
     """
     maiden = str(maiden).strip().upper()
```

### Comparing `not1mm-23.5.4/not1mm.egg-info/PKG-INFO` & `not1mm-23.5.5/not1mm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.4
+Version: 23.5.5
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -68,14 +68,18 @@
     - [Log Display](#log-display)
     - [Bandmap](#bandmap)
   - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
+  - [Contest specific notes](#contest-specific-notes)
+    - [ARRL Sweekstakes](#arrl-sweekstakes)
+      - [The exchange parser](#the-exchange-parser)
+      - [The exchange](#the-exchange)
 
 ## What and why is Not1MM
 
 Not1MM's interface is a blantent ripoff of N1MM.
 It is NOT N1MM and any problem you have with this software should in no way reflect on their software.
 
 If you use Windows(tm) you should run away from this and use someother program.
@@ -103,24 +107,27 @@
 - General Logging
 - 10 10 Fall CW
 - 10 10 Spring CW
 - 10 10 Summer Phone
 - 10 10 Winter Phone
 - ARRL DX CW
 - ARRL DX SSB
+- ARRL Sweepstakes CW
+- ARRL Sweepstakes SSB
 - CQ WPX CW
 - CQ WPX SSB
 - CQ World Wide CW
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
+- [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
 <summary>April 2023</summary>
@@ -437,7 +444,33 @@
 Boom... ADIF
 
 `StationCall`_`ContestName`.adi
 
 ## Dupe checking
 
 Added dupe checking. Big Red 'Dupe' will appear if it's a dupe...
+
+## Contest specific notes
+
+I found it might be beneficial to have a section devoted to wierd quirky things about operating a specific contests.
+
+### ARRL Sweekstakes
+
+#### The exchange parser
+
+This was a pain in the tukus. There are so many elements to the exchange, and one input field aside from the callsign field. So I had to write sort of a 'parser'. The parser moves over your input string following some basic rules and is re-evaluated with each keypress and the parsed result will be displayed in the label over the field. The exchange looks like `124 A K6GTE 17 ORG`, a Serial number, Precidence, Callsign, Year Licenced and Section. even though the callsign is given as part of the exchange, the callsign does not have to be entered and is pulled from the callsign field. If the exchange was entered as `124 A 17 ORG` you would see:
+
+![SS Parser Result](https://github.com/mbridak/not1mm/raw/master/pic/ss_parser_1.png)
+
+You can enter the serial number and precidence, or the year and section as pairs. For instance `124A 17ORG`. This would ensure the values get parsed correctly.
+
+You do not have to go back to correct typing. You can just tack the correct items to the end of the field and the older values will get overwritten. So if you entered `124A 17ORG Q`, the precidence will change from A to Q. If you need to change the serial number you must append the precidence to it, `125A`.
+
+If the callsign was entered wrong in the callsign field, you can put the correct callsign some where in the exchange. As long as it shows up in the parsed label above correctly your good.
+
+The best thing you can do is play around with it to see how it behaves.
+
+#### The exchange
+
+In the `Sent Exchange` field of the New Contest dialog put in the Precidence, Call, Check and Section. Example: `A K6GTE 17 ORG`.
+
+For the Run Exchange macro I'd put `{HISCALL} # A K6GTE 17 ORG`.
```

### Comparing `not1mm-23.5.4/not1mm.egg-info/SOURCES.txt` & `not1mm-23.5.5/not1mm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -119,9 +119,8 @@
 not1mm/plugins/cq_ww_ssb.py
 not1mm/plugins/cwt.py
 not1mm/plugins/general_logging.py
 not1mm/plugins/jidx_cw.py
 not1mm/plugins/jidx_ph.py
 not1mm/plugins/winter_field_day.py
 not1mm/testing/test.py
-testing/test.py
-testing/text2.py
+testing/test.py
```

### Comparing `not1mm-23.5.4/pyproject.toml` & `not1mm-23.5.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "23.5.4"
+version = "23.5.5"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

