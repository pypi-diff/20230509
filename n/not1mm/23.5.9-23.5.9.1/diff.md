# Comparing `tmp/not1mm-23.5.9.tar.gz` & `tmp/not1mm-23.5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-23.5.9.tar", last modified: Tue May  9 15:12:08 2023, max compression
+gzip compressed data, was "not1mm-23.5.9.1.tar", last modified: Tue May  9 20:15:55 2023, max compression
```

## Comparing `not1mm-23.5.9.tar` & `not1mm-23.5.9.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 15:12:08.491272 not1mm-23.5.9/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.9/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    24116 2023-05-09 15:12:08.490272 not1mm-23.5.9/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23371 2023-05-09 15:10:18.000000 not1mm-23.5.9/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 15:12:08.344275 not1mm-23.5.9/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.9/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    79219 2023-05-09 15:06:20.000000 not1mm-23.5.9/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    21634 2023-05-09 14:55:30.000000 not1mm-23.5.9/not1mm/bandmap.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 15:12:08.382274 not1mm-23.5.9/not1mm/data/
--rw-rw-rw-   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.9/not1mm/data/Combinear.qss
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.9/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.9/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.9/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.9/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.9/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.9/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40156 2023-05-06 20:10:52.000000 not1mm-23.5.9/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.9/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.9/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.9/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.9/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.9/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.9/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.9/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.9/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.9/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.9/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.9/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43909 2023-05-08 20:14:41.000000 not1mm-23.5.9/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.5.9/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.9/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 15:12:08.457272 not1mm-23.5.9/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.9/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.9/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.9/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.9/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.9/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.9/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.9/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.9/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.9/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.9/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.9/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.9/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.9/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.9/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.9/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.9/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.9/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.9/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.9/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.9/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.9/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.9/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.9/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.9/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.9/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.9/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.9/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.9/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.9/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.9/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.9/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.9/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.9/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.9/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.9/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.9/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.9/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.9/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.9/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.9/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.9/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.9/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.9/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.9/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.9/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.9/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.9/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.9/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.9/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.9/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.9/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.9/not1mm/data/ssbmacros.txt
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 15:12:08.485272 not1mm-23.5.9/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.9/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.9/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13705 2023-05-07 16:50:54.000000 not1mm-23.5.9/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.9/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34193 2023-05-05 18:13:45.000000 not1mm-23.5.9/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.9/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.9/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.9/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.9/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.9/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.9/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.9/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.9/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.9/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.9/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6188 2023-05-06 20:36:00.000000 not1mm-23.5.9/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-05-09 14:56:56.000000 not1mm-23.5.9/not1mm/lib/version.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    30275 2023-05-09 15:02:00.000000 not1mm-23.5.9/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 15:12:08.489272 not1mm-23.5.9/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13746 2023-05-05 16:08:13.000000 not1mm-23.5.9/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13752 2023-05-05 16:08:31.000000 not1mm-23.5.9/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13759 2023-05-05 16:08:41.000000 not1mm-23.5.9/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13762 2023-05-05 16:08:51.000000 not1mm-23.5.9/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.9/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14549 2023-05-05 16:08:59.000000 not1mm-23.5.9/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14552 2023-05-05 16:09:07.000000 not1mm-23.5.9/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12990 2023-05-05 16:10:17.000000 not1mm-23.5.9/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.5.9/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15941 2023-05-05 19:46:43.000000 not1mm-23.5.9/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15946 2023-05-05 19:54:23.000000 not1mm-23.5.9/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14939 2023-05-08 19:30:37.000000 not1mm-23.5.9/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15026 2023-05-05 16:10:01.000000 not1mm-23.5.9/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-05 16:09:55.000000 not1mm-23.5.9/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13899 2023-05-05 16:11:06.000000 not1mm-23.5.9/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14753 2023-05-05 16:11:03.000000 not1mm-23.5.9/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.5.9/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.5.9/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.5.9/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.5.9/not1mm/plugins/winter_field_day.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 15:12:08.489272 not1mm-23.5.9/not1mm/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-05-05 15:04:14.000000 not1mm-23.5.9/not1mm/testing/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 15:12:08.348275 not1mm-23.5.9/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    24116 2023-05-09 15:12:08.000000 not1mm-23.5.9/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3443 2023-05-09 15:12:08.000000 not1mm-23.5.9/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-09 15:12:08.000000 not1mm-23.5.9/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-09 15:12:08.000000 not1mm-23.5.9/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-09 15:12:08.000000 not1mm-23.5.9/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-09 15:12:08.000000 not1mm-23.5.9/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1217 2023-05-09 14:56:59.000000 not1mm-23.5.9/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-09 15:12:08.491272 not1mm-23.5.9/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 15:12:08.490272 not1mm-23.5.9/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.9/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.971519 not1mm-23.5.9.1/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.9.1/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25054 2023-05-09 20:15:55.971519 not1mm-23.5.9.1/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    24307 2023-05-09 20:15:01.000000 not1mm-23.5.9.1/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.944520 not1mm-23.5.9.1/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.9.1/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    80054 2023-05-09 20:13:32.000000 not1mm-23.5.9.1/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    23860 2023-05-09 20:08:28.000000 not1mm-23.5.9.1/not1mm/bandmap.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.953520 not1mm-23.5.9.1/not1mm/data/
+-rw-rw-rw-   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.9.1/not1mm/data/Combinear.qss
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.9.1/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.9.1/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.9.1/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.9.1/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.9.1/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.9.1/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40156 2023-05-06 20:10:52.000000 not1mm-23.5.9.1/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.9.1/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.9.1/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.9.1/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.9.1/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.9.1/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.9.1/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.9.1/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.9.1/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.9.1/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.9.1/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.9.1/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43909 2023-05-08 20:14:41.000000 not1mm-23.5.9.1/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.5.9.1/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.9.1/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.963520 not1mm-23.5.9.1/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.9.1/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.9.1/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.9.1/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.9.1/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.9.1/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.9.1/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.9.1/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.9.1/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.9.1/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.9.1/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.9.1/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.9.1/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.9.1/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.9.1/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.9.1/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.9.1/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.9.1/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.9.1/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.9.1/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.9.1/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.9.1/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.9.1/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.9.1/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.9.1/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.9.1/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.9.1/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.9.1/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.9.1/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.9.1/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.9.1/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.9.1/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.9.1/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.9.1/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.9.1/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.9.1/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.9.1/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.9.1/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.9.1/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.9.1/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.9.1/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.9.1/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.9.1/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.9.1/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.9.1/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.9.1/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.9.1/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.9.1/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.9.1/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.9.1/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.9.1/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.9.1/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.9.1/not1mm/data/ssbmacros.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.966519 not1mm-23.5.9.1/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.9.1/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.9.1/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13705 2023-05-07 16:50:54.000000 not1mm-23.5.9.1/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.9.1/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34193 2023-05-05 18:13:45.000000 not1mm-23.5.9.1/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.9.1/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.9.1/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.9.1/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.9.1/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.9.1/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.9.1/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.9.1/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.9.1/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.9.1/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.9.1/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6188 2023-05-06 20:36:00.000000 not1mm-23.5.9.1/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       48 2023-05-09 20:07:08.000000 not1mm-23.5.9.1/not1mm/lib/version.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    30275 2023-05-09 15:02:00.000000 not1mm-23.5.9.1/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.970519 not1mm-23.5.9.1/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13746 2023-05-05 16:08:13.000000 not1mm-23.5.9.1/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13752 2023-05-05 16:08:31.000000 not1mm-23.5.9.1/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13759 2023-05-05 16:08:41.000000 not1mm-23.5.9.1/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13762 2023-05-05 16:08:51.000000 not1mm-23.5.9.1/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.9.1/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14549 2023-05-05 16:08:59.000000 not1mm-23.5.9.1/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14552 2023-05-05 16:09:07.000000 not1mm-23.5.9.1/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12990 2023-05-05 16:10:17.000000 not1mm-23.5.9.1/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.5.9.1/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15941 2023-05-05 19:46:43.000000 not1mm-23.5.9.1/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15946 2023-05-05 19:54:23.000000 not1mm-23.5.9.1/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14939 2023-05-08 19:30:37.000000 not1mm-23.5.9.1/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15026 2023-05-05 16:10:01.000000 not1mm-23.5.9.1/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-05 16:09:55.000000 not1mm-23.5.9.1/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13899 2023-05-05 16:11:06.000000 not1mm-23.5.9.1/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14753 2023-05-05 16:11:03.000000 not1mm-23.5.9.1/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.5.9.1/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.5.9.1/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.5.9.1/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.5.9.1/not1mm/plugins/winter_field_day.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.970519 not1mm-23.5.9.1/not1mm/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-05-05 15:04:14.000000 not1mm-23.5.9.1/not1mm/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.944520 not1mm-23.5.9.1/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25054 2023-05-09 20:15:55.000000 not1mm-23.5.9.1/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3443 2023-05-09 20:15:55.000000 not1mm-23.5.9.1/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-09 20:15:55.000000 not1mm-23.5.9.1/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-09 20:15:55.000000 not1mm-23.5.9.1/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-09 20:15:55.000000 not1mm-23.5.9.1/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-09 20:15:55.000000 not1mm-23.5.9.1/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1219 2023-05-09 20:07:09.000000 not1mm-23.5.9.1/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-09 20:15:55.971519 not1mm-23.5.9.1/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-09 20:15:55.970519 not1mm-23.5.9.1/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.9.1/testing/test.py
```

### Comparing `not1mm-23.5.9/LICENSE` & `not1mm-23.5.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/PKG-INFO` & `not1mm-23.5.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.9
+Version: 23.5.9.1
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -60,14 +60,16 @@
   - [Hiding screen elements](#hiding-screen-elements)
   - [Editing macro keys](#editing-macro-keys)
     - [Macro substitutions](#macro-substitutions)
     - [Macro use with voice](#macro-use-with-voice)
   - [cty.dat and QRZ lookups for distance and bearing](#ctydat-and-qrz-lookups-for-distance-and-bearing)
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
+    - [The Main Window](#the-main-window)
+      - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
     - [Bandmap](#bandmap)
   - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
@@ -112,15 +114,15 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother.
+- [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother. Add CTRL-PgUp and CTRL-PgDown keys to jump to the next/prev spots in the bandmap. Fix: Voice not keying on LSB.
 - [23-5-8] Bandmap zoom in/out now centers scale to RX Freq.
 - [23-5-7] Added bandwidth marker to the bandmap.
 - [23-5-6] Added AR Cluster filter options for the bandmap. Added a station ID to the multicast packets. This will prevent erratic bevahiour if 2 stations are on the same network.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
@@ -384,14 +386,30 @@
 - [CW, SSB, RTTY] You can set the mode logged. If you have CAT control this will also change the mode on the radio.
 - [OPON] Change the operator currently logging.
 
 **You must press the SPACE bar after entering any of the above.**
 
 ## Windows
 
+### The Main Window
+
+#### Keyboard commands
+
+- [Esc] Clears the input fields of any text.
+- [CTRL-Esc] Stops cwdaemon from sending Morse.
+- [PgUp] Increases the cwdaemon sending speed.
+- [PgDown] Decreases the cwdaemon sending speed.
+- [CTRL-PgUp] Jump to the next spot above the current VFO cursor in the bamdmap window.
+- [CTRL-PgDown] Jump to the next spot below the current VFO cursor in the bamdmap window.
+- [TAB] Move cursor to the right one field.
+- [Shift-Tab] Move cursor left One field.
+- [SPACE] When in the callsign field, will move the input to the first field needed for the exchange.
+- [Enter] Submits the fields to the log.
+- [F1-F12] Send (CW or Voice) macros.
+
 ### Log Display
 
 `Window`>`Log Window`
 
 The Log display gets updated automatically when a contact is entered. The top half is a list of all contacts.
 
 ![Log Display Window](https://github.com/mbridak/not1mm/raw/master/pic/logdisplay.png)
@@ -400,15 +418,15 @@
 
 ### Bandmap
 
 `Window`>`Bandmap`
 
 Put your callsign in the top and press the connect button.
 
-The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. Clicked on spots now tune the radio and set the callsign field.
+The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
 
 ![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
 
 ## Editing a contact
 
 ![Editing a cell](https://github.com/mbridak/not1mm/raw/master/pic/edit_cell.png)
```

### Comparing `not1mm-23.5.9/README.md` & `not1mm-23.5.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
   - [Hiding screen elements](#hiding-screen-elements)
   - [Editing macro keys](#editing-macro-keys)
     - [Macro substitutions](#macro-substitutions)
     - [Macro use with voice](#macro-use-with-voice)
   - [cty.dat and QRZ lookups for distance and bearing](#ctydat-and-qrz-lookups-for-distance-and-bearing)
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
+    - [The Main Window](#the-main-window)
+      - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
     - [Bandmap](#bandmap)
   - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
@@ -93,15 +95,15 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother.
+- [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother. Add CTRL-PgUp and CTRL-PgDown keys to jump to the next/prev spots in the bandmap. Fix: Voice not keying on LSB.
 - [23-5-8] Bandmap zoom in/out now centers scale to RX Freq.
 - [23-5-7] Added bandwidth marker to the bandmap.
 - [23-5-6] Added AR Cluster filter options for the bandmap. Added a station ID to the multicast packets. This will prevent erratic bevahiour if 2 stations are on the same network.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
@@ -365,14 +367,30 @@
 - [CW, SSB, RTTY] You can set the mode logged. If you have CAT control this will also change the mode on the radio.
 - [OPON] Change the operator currently logging.
 
 **You must press the SPACE bar after entering any of the above.**
 
 ## Windows
 
+### The Main Window
+
+#### Keyboard commands
+
+- [Esc] Clears the input fields of any text.
+- [CTRL-Esc] Stops cwdaemon from sending Morse.
+- [PgUp] Increases the cwdaemon sending speed.
+- [PgDown] Decreases the cwdaemon sending speed.
+- [CTRL-PgUp] Jump to the next spot above the current VFO cursor in the bamdmap window.
+- [CTRL-PgDown] Jump to the next spot below the current VFO cursor in the bamdmap window.
+- [TAB] Move cursor to the right one field.
+- [Shift-Tab] Move cursor left One field.
+- [SPACE] When in the callsign field, will move the input to the first field needed for the exchange.
+- [Enter] Submits the fields to the log.
+- [F1-F12] Send (CW or Voice) macros.
+
 ### Log Display
 
 `Window`>`Log Window`
 
 The Log display gets updated automatically when a contact is entered. The top half is a list of all contacts.
 
 ![Log Display Window](https://github.com/mbridak/not1mm/raw/master/pic/logdisplay.png)
@@ -381,15 +399,15 @@
 
 ### Bandmap
 
 `Window`>`Bandmap`
 
 Put your callsign in the top and press the connect button.
 
-The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. Clicked on spots now tune the radio and set the callsign field.
+The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
 
 ![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
 
 ## Editing a contact
 
 ![Editing a cell](https://github.com/mbridak/not1mm/raw/master/pic/edit_cell.png)
```

### Comparing `not1mm-23.5.9/not1mm/__main__.py` & `not1mm-23.5.9.1/not1mm/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1783,3170 +1783,3222 @@
 00006f60: 3a20 6469 7361 626c 653d 696e 7661 6c69  : disable=invali
 00006f70: 642d 6e61 6d65 0a20 2020 2020 2020 2022  d-name.        "
 00006f80: 2222 5468 6973 206f 7665 7272 6964 6573  ""This overrides
 00006f90: 2051 7420 6b65 7920 6576 656e 742e 2222   Qt key event.""
 00006fa0: 220a 2020 2020 2020 2020 6d6f 6469 6669  ".        modifi
 00006fb0: 6572 203d 2065 7665 6e74 2e6d 6f64 6966  er = event.modif
 00006fc0: 6965 7273 2829 0a20 2020 2020 2020 2069  iers().        i
-00006fd0: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
-00006fe0: 2051 742e 4b65 792e 4b65 795f 4573 6361   Qt.Key.Key_Esca
-00006ff0: 7065 3a20 2023 2070 796c 696e 743a 2064  pe:  # pylint: d
-00007000: 6973 6162 6c65 3d6e 6f2d 6d65 6d62 6572  isable=no-member
-00007010: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007020: 662e 636c 6561 7269 6e70 7574 7328 290a  f.clearinputs().
-00007030: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00007040: 6377 2069 7320 6e6f 7420 4e6f 6e65 2061  cw is not None a
-00007050: 6e64 206d 6f64 6966 6965 7220 3d3d 2051  nd modifier == Q
-00007060: 742e 436f 6e74 726f 6c4d 6f64 6966 6965  t.ControlModifie
-00007070: 723a 0a20 2020 2020 2020 2020 2020 2069  r:.            i
-00007080: 6620 7365 6c66 2e63 772e 7365 7276 6572  f self.cw.server
-00007090: 7479 7065 203d 3d20 313a 0a20 2020 2020  type == 1:.     
-000070a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000070b0: 6377 2e73 656e 6463 7728 225c 7831 6234  cw.sendcw("\x1b4
-000070c0: 2229 0a20 2020 2020 2020 2069 6620 6576  ").        if ev
-000070d0: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
-000070e0: 4b65 792e 4b65 795f 5061 6765 5570 3a0a  Key.Key_PageUp:.
-000070f0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00007100: 656c 662e 6377 2069 7320 6e6f 7420 4e6f  elf.cw is not No
-00007110: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00007120: 2020 2020 6966 2073 656c 662e 6377 2e73      if self.cw.s
-00007130: 6572 7665 7274 7970 6520 3d3d 2031 3a0a  ervertype == 1:.
-00007140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007150: 2020 2020 7365 6c66 2e63 772e 7370 6565      self.cw.spee
-00007160: 6420 2b3d 2031 0a20 2020 2020 2020 2020  d += 1.         
-00007170: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007180: 6377 5f73 7065 6564 2e73 6574 5661 6c75  cw_speed.setValu
-00007190: 6528 7365 6c66 2e63 772e 7370 6565 6429  e(self.cw.speed)
-000071a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000071b0: 2020 2020 2073 656c 662e 6377 2e73 656e       self.cw.sen
-000071c0: 6463 7728 6622 5c78 3162 327b 7365 6c66  dcw(f"\x1b2{self
-000071d0: 2e63 772e 7370 6565 647d 2229 0a20 2020  .cw.speed}").   
-000071e0: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
-000071f0: 7928 2920 3d3d 2051 742e 4b65 792e 4b65  y() == Qt.Key.Ke
-00007200: 795f 5061 6765 446f 776e 3a0a 2020 2020  y_PageDown:.    
-00007210: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00007220: 6377 2069 7320 6e6f 7420 4e6f 6e65 3a0a  cw is not None:.
-00007230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007240: 6966 2073 656c 662e 6377 2e73 6572 7665  if self.cw.serve
-00007250: 7274 7970 6520 3d3d 2031 3a0a 2020 2020  rtype == 1:.    
-00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007270: 7365 6c66 2e63 772e 7370 6565 6420 2d3d  self.cw.speed -=
-00007280: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
-00007290: 2020 2020 2020 2073 656c 662e 6377 5f73         self.cw_s
-000072a0: 7065 6564 2e73 6574 5661 6c75 6528 7365  peed.setValue(se
-000072b0: 6c66 2e63 772e 7370 6565 6429 0a20 2020  lf.cw.speed).   
-000072c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072d0: 2073 656c 662e 6377 2e73 656e 6463 7728   self.cw.sendcw(
-000072e0: 6622 5c78 3162 327b 7365 6c66 2e63 772e  f"\x1b2{self.cw.
-000072f0: 7370 6565 647d 2229 0a20 2020 2020 2020  speed}").       
-00007300: 2023 2069 6620 6576 656e 742e 6b65 7928   # if event.key(
-00007310: 2920 3d3d 2051 742e 4b65 792e 4b65 795f  ) == Qt.Key.Key_
-00007320: 456e 7465 723a 0a20 2020 2020 2020 2023  Enter:.        #
-00007330: 2020 2020 2073 656c 662e 7361 7665 5f63       self.save_c
-00007340: 6f6e 7461 6374 2829 0a20 2020 2020 2020  ontact().       
-00007350: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
-00007360: 3d3d 2051 742e 4b65 792e 4b65 795f 5461  == Qt.Key.Key_Ta
-00007370: 6220 6f72 2065 7665 6e74 2e6b 6579 2829  b or event.key()
-00007380: 203d 3d20 5174 2e4b 6579 2e4b 6579 5f42   == Qt.Key.Key_B
-00007390: 6163 6b74 6162 3a0a 2020 2020 2020 2020  acktab:.        
-000073a0: 2020 2020 6966 2073 656c 662e 7365 6e74      if self.sent
-000073b0: 2e68 6173 466f 6375 7328 293a 0a20 2020  .hasFocus():.   
-000073c0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-000073d0: 6765 722e 6465 6275 6728 2246 726f 6d20  ger.debug("From 
-000073e0: 7365 6e74 2229 0a20 2020 2020 2020 2020  sent").         
-000073f0: 2020 2020 2020 2069 6620 6d6f 6469 6669         if modifi
-00007400: 6572 203d 3d20 5174 2e53 6869 6674 4d6f  er == Qt.ShiftMo
-00007410: 6469 6669 6572 3a0a 2020 2020 2020 2020  difier:.        
-00007420: 2020 2020 2020 2020 2020 2020 7072 6576              prev
-00007430: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
-00007440: 7072 6576 2e67 6574 2873 656c 662e 7365  prev.get(self.se
-00007450: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
-00007460: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-00007470: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
-00007480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007490: 7072 6576 5f74 6162 2e64 6573 656c 6563  prev_tab.deselec
-000074a0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-000074b0: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-000074c0: 2e65 6e64 2846 616c 7365 290a 2020 2020  .end(False).    
-000074d0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000074e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000074f0: 2020 2020 2020 6e65 7874 5f74 6162 203d        next_tab =
-00007500: 2073 656c 662e 7461 625f 6e65 7874 2e67   self.tab_next.g
-00007510: 6574 2873 656c 662e 7365 6e74 290a 2020  et(self.sent).  
-00007520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007530: 2020 6e65 7874 5f74 6162 2e73 6574 466f    next_tab.setFo
-00007540: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
-00007550: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
-00007560: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
-00007570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007580: 2020 6e65 7874 5f74 6162 2e65 6e64 2846    next_tab.end(F
-00007590: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-000075a0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-000075b0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-000075c0: 2e72 6563 6569 7665 2e68 6173 466f 6375  .receive.hasFocu
-000075d0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-000075e0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-000075f0: 6728 2246 726f 6d20 7265 6365 6976 6522  g("From receive"
-00007600: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00007610: 2020 6966 206d 6f64 6966 6965 7220 3d3d    if modifier ==
-00007620: 2051 742e 5368 6966 744d 6f64 6966 6965   Qt.ShiftModifie
-00007630: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-00007640: 2020 2020 2020 2070 7265 765f 7461 6220         prev_tab 
-00007650: 3d20 7365 6c66 2e74 6162 5f70 7265 762e  = self.tab_prev.
-00007660: 6765 7428 7365 6c66 2e72 6563 6569 7665  get(self.receive
-00007670: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00007680: 2020 2020 2020 7072 6576 5f74 6162 2e73        prev_tab.s
-00007690: 6574 466f 6375 7328 290a 2020 2020 2020  etFocus().      
-000076a0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000076b0: 6576 5f74 6162 2e64 6573 656c 6563 7428  ev_tab.deselect(
-000076c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000076d0: 2020 2020 2020 7072 6576 5f74 6162 2e65        prev_tab.e
-000076e0: 6e64 2846 616c 7365 290a 2020 2020 2020  nd(False).      
-000076f0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00007700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007710: 2020 2020 6e65 7874 5f74 6162 203d 2073      next_tab = s
-00007720: 656c 662e 7461 625f 6e65 7874 2e67 6574  elf.tab_next.get
-00007730: 2873 656c 662e 7265 6365 6976 6529 0a20  (self.receive). 
-00007740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007750: 2020 206e 6578 745f 7461 622e 7365 7446     next_tab.setF
-00007760: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
-00007770: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-00007780: 7461 622e 6465 7365 6c65 6374 2829 0a20  tab.deselect(). 
-00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077a0: 2020 206e 6578 745f 7461 622e 656e 6428     next_tab.end(
-000077b0: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
-000077c0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-000077d0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000077e0: 662e 6f74 6865 725f 312e 6861 7346 6f63  f.other_1.hasFoc
-000077f0: 7573 2829 3a0a 2020 2020 2020 2020 2020  us():.          
-00007800: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00007810: 7567 2822 4672 6f6d 206f 7468 6572 5f31  ug("From other_1
-00007820: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00007830: 2020 2069 6620 6d6f 6469 6669 6572 203d     if modifier =
-00007840: 3d20 5174 2e53 6869 6674 4d6f 6469 6669  = Qt.ShiftModifi
-00007850: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-00007860: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-00007870: 203d 2073 656c 662e 7461 625f 7072 6576   = self.tab_prev
-00007880: 2e67 6574 2873 656c 662e 6f74 6865 725f  .get(self.other_
-00007890: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
-000078a0: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
-000078b0: 7365 7446 6f63 7573 2829 0a20 2020 2020  setFocus().     
-000078c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000078d0: 7265 765f 7461 622e 6465 7365 6c65 6374  rev_tab.deselect
-000078e0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-000078f0: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
-00007900: 656e 6428 4661 6c73 6529 0a20 2020 2020  end(False).     
-00007910: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00007920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007930: 2020 2020 206e 6578 745f 7461 6220 3d20       next_tab = 
-00007940: 7365 6c66 2e74 6162 5f6e 6578 742e 6765  self.tab_next.ge
-00007950: 7428 7365 6c66 2e6f 7468 6572 5f31 290a  t(self.other_1).
-00007960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007970: 2020 2020 6e65 7874 5f74 6162 2e73 6574      next_tab.set
-00007980: 466f 6375 7328 290a 2020 2020 2020 2020  Focus().        
-00007990: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-000079a0: 5f74 6162 2e64 6573 656c 6563 7428 290a  _tab.deselect().
-000079b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079c0: 2020 2020 6e65 7874 5f74 6162 2e65 6e64      next_tab.end
-000079d0: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
-000079e0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-000079f0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00007a00: 6c66 2e6f 7468 6572 5f32 2e68 6173 466f  lf.other_2.hasFo
-00007a10: 6375 7328 293a 0a20 2020 2020 2020 2020  cus():.         
-00007a20: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00007a30: 6275 6728 2246 726f 6d20 6f74 6865 725f  bug("From other_
-00007a40: 3222 290a 2020 2020 2020 2020 2020 2020  2").            
-00007a50: 2020 2020 6966 206d 6f64 6966 6965 7220      if modifier 
-00007a60: 3d3d 2051 742e 5368 6966 744d 6f64 6966  == Qt.ShiftModif
-00007a70: 6965 723a 0a20 2020 2020 2020 2020 2020  ier:.           
-00007a80: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
-00007a90: 6220 3d20 7365 6c66 2e74 6162 5f70 7265  b = self.tab_pre
-00007aa0: 762e 6765 7428 7365 6c66 2e6f 7468 6572  v.get(self.other
-00007ab0: 5f32 290a 2020 2020 2020 2020 2020 2020  _2).            
-00007ac0: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-00007ad0: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
-00007ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007af0: 7072 6576 5f74 6162 2e64 6573 656c 6563  prev_tab.deselec
-00007b00: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00007b10: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-00007b20: 2e65 6e64 2846 616c 7365 290a 2020 2020  .end(False).    
-00007b30: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00007b40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007b50: 2020 2020 2020 6e65 7874 5f74 6162 203d        next_tab =
-00007b60: 2073 656c 662e 7461 625f 6e65 7874 2e67   self.tab_next.g
-00007b70: 6574 2873 656c 662e 6f74 6865 725f 3229  et(self.other_2)
-00007b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007b90: 2020 2020 206e 6578 745f 7461 622e 7365       next_tab.se
-00007ba0: 7446 6f63 7573 2829 0a20 2020 2020 2020  tFocus().       
-00007bb0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-00007bc0: 745f 7461 622e 6465 7365 6c65 6374 2829  t_tab.deselect()
-00007bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007be0: 2020 2020 206e 6578 745f 7461 622e 656e       next_tab.en
-00007bf0: 6428 4661 6c73 6529 0a20 2020 2020 2020  d(False).       
-00007c00: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00007c10: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00007c20: 656c 662e 6361 6c6c 7369 676e 2e68 6173  elf.callsign.has
-00007c30: 466f 6375 7328 293a 0a20 2020 2020 2020  Focus():.       
-00007c40: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00007c50: 6465 6275 6728 2246 726f 6d20 6361 6c6c  debug("From call
-00007c60: 7369 676e 2229 0a20 2020 2020 2020 2020  sign").         
-00007c70: 2020 2020 2020 2069 6620 6d6f 6469 6669         if modifi
-00007c80: 6572 203d 3d20 5174 2e53 6869 6674 4d6f  er == Qt.ShiftMo
-00007c90: 6469 6669 6572 3a0a 2020 2020 2020 2020  difier:.        
-00007ca0: 2020 2020 2020 2020 2020 2020 7072 6576              prev
-00007cb0: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
-00007cc0: 7072 6576 2e67 6574 2873 656c 662e 6361  prev.get(self.ca
-00007cd0: 6c6c 7369 676e 290a 2020 2020 2020 2020  llsign).        
-00007ce0: 2020 2020 2020 2020 2020 2020 7072 6576              prev
-00007cf0: 5f74 6162 2e73 6574 466f 6375 7328 290a  _tab.setFocus().
-00007d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d10: 2020 2020 7072 6576 5f74 6162 2e64 6573      prev_tab.des
-00007d20: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
-00007d30: 2020 2020 2020 2020 2020 2020 7072 6576              prev
-00007d40: 5f74 6162 2e65 6e64 2846 616c 7365 290a  _tab.end(False).
-00007d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d60: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00007d70: 2020 2020 2020 2020 2020 7465 7874 203d            text =
-00007d80: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
-00007d90: 6578 7428 290a 2020 2020 2020 2020 2020  ext().          
-00007da0: 2020 2020 2020 2020 2020 7465 7874 203d            text =
-00007db0: 2074 6578 742e 7570 7065 7228 290a 2020   text.upper().  
-00007dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007dd0: 2020 5f74 6865 7468 7265 6164 203d 2074    _thethread = t
-00007de0: 6872 6561 6469 6e67 2e54 6872 6561 6428  hreading.Thread(
-00007df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007e00: 2020 2020 2020 2020 2074 6172 6765 743d           target=
-00007e10: 7365 6c66 2e63 6865 636b 5f63 616c 6c73  self.check_calls
-00007e20: 6967 6e32 2c0a 2020 2020 2020 2020 2020  ign2,.          
-00007e30: 2020 2020 2020 2020 2020 2020 2020 6172                ar
-00007e40: 6773 3d28 7465 7874 2c29 2c0a 2020 2020  gs=(text,),.    
-00007e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e60: 2020 2020 6461 656d 6f6e 3d54 7275 652c      daemon=True,
-00007e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007e80: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00007e90: 2020 2020 2020 2020 2020 205f 7468 6574             _thet
-00007ea0: 6872 6561 642e 7374 6172 7428 290a 2020  hread.start().  
-00007eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ec0: 2020 6e65 7874 5f74 6162 203d 2073 656c    next_tab = sel
-00007ed0: 662e 7461 625f 6e65 7874 2e67 6574 2873  f.tab_next.get(s
-00007ee0: 656c 662e 6361 6c6c 7369 676e 290a 2020  elf.callsign).  
-00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f00: 2020 6e65 7874 5f74 6162 2e73 6574 466f    next_tab.setFo
-00007f10: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
-00007f20: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
-00007f30: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
-00007f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f50: 2020 6e65 7874 5f74 6162 2e65 6e64 2846    next_tab.end(F
-00007f60: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-00007f70: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00007f80: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
-00007f90: 7928 2920 3d3d 2051 742e 4b65 795f 4631  y() == Qt.Key_F1
-00007fa0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00007fb0: 6c66 2e73 656e 6466 3128 290a 2020 2020  lf.sendf1().    
-00007fc0: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
-00007fd0: 2829 203d 3d20 5174 2e4b 6579 5f46 323a  () == Qt.Key_F2:
-00007fe0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007ff0: 662e 7365 6e64 6632 2829 0a20 2020 2020  f.sendf2().     
-00008000: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-00008010: 2920 3d3d 2051 742e 4b65 795f 4633 3a0a  ) == Qt.Key_F3:.
-00008020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008030: 2e73 656e 6466 3328 290a 2020 2020 2020  .sendf3().      
-00008040: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
-00008050: 203d 3d20 5174 2e4b 6579 5f46 343a 0a20   == Qt.Key_F4:. 
-00008060: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008070: 7365 6e64 6634 2829 0a20 2020 2020 2020  sendf4().       
-00008080: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
-00008090: 3d3d 2051 742e 4b65 795f 4635 3a0a 2020  == Qt.Key_F5:.  
-000080a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000080b0: 656e 6466 3528 290a 2020 2020 2020 2020  endf5().        
-000080c0: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
-000080d0: 3d20 5174 2e4b 6579 5f46 363a 0a20 2020  = Qt.Key_F6:.   
-000080e0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000080f0: 6e64 6636 2829 0a20 2020 2020 2020 2069  ndf6().        i
-00008100: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
-00008110: 2051 742e 4b65 795f 4637 3a0a 2020 2020   Qt.Key_F7:.    
-00008120: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-00008130: 6466 3728 290a 2020 2020 2020 2020 6966  df7().        if
-00008140: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-00008150: 5174 2e4b 6579 5f46 383a 0a20 2020 2020  Qt.Key_F8:.     
-00008160: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
-00008170: 6638 2829 0a20 2020 2020 2020 2069 6620  f8().        if 
-00008180: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-00008190: 742e 4b65 795f 4639 3a0a 2020 2020 2020  t.Key_F9:.      
-000081a0: 2020 2020 2020 7365 6c66 2e73 656e 6466        self.sendf
-000081b0: 3928 290a 2020 2020 2020 2020 6966 2065  9().        if e
-000081c0: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
-000081d0: 2e4b 6579 5f46 3130 3a0a 2020 2020 2020  .Key_F10:.      
-000081e0: 2020 2020 2020 7365 6c66 2e73 656e 6466        self.sendf
-000081f0: 3130 2829 0a20 2020 2020 2020 2069 6620  10().        if 
-00008200: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-00008210: 742e 4b65 795f 4631 313a 0a20 2020 2020  t.Key_F11:.     
-00008220: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
-00008230: 6631 3128 290a 2020 2020 2020 2020 6966  f11().        if
-00008240: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-00008250: 5174 2e4b 6579 5f46 3132 3a0a 2020 2020  Qt.Key_F12:.    
-00008260: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-00008270: 6466 3132 2829 0a0a 2020 2020 6465 6620  df12()..    def 
-00008280: 7365 745f 7769 6e64 6f77 5f74 6974 6c65  set_window_title
-00008290: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000082a0: 2222 2253 6574 2077 696e 646f 7720 7469  """Set window ti
-000082b0: 746c 6522 2222 0a20 2020 2020 2020 2076  tle""".        v
-000082c0: 666f 6120 3d20 7365 6c66 2e72 6164 696f  foa = self.radio
-000082d0: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
-000082e0: 222c 2022 2229 0a20 2020 2020 2020 2069  ", "").        i
-000082f0: 6620 7666 6f61 3a0a 2020 2020 2020 2020  f vfoa:.        
-00008300: 2020 2020 7666 6f61 203d 2069 6e74 2876      vfoa = int(v
-00008310: 666f 6129 202f 2031 3030 300a 2020 2020  foa) / 1000.    
-00008320: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00008330: 2020 2020 2020 7666 6f61 203d 2030 2e30        vfoa = 0.0
-00008340: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-00008350: 5f6e 616d 6520 3d20 2222 0a20 2020 2020  _name = "".     
-00008360: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
-00008370: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
-00008380: 636f 6e74 6573 745f 6e61 6d65 203d 2073  contest_name = s
-00008390: 656c 662e 636f 6e74 6573 742e 6e61 6d65  elf.contest.name
-000083a0: 0a20 2020 2020 2020 206c 696e 6520 3d20  .        line = 
-000083b0: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
-000083c0: 7666 6f61 3a7b 726f 756e 6428 7666 6f61  vfoa:{round(vfoa
-000083d0: 2c32 297d 2022 0a20 2020 2020 2020 2020  ,2)} ".         
-000083e0: 2020 2066 226d 6f64 653a 7b73 656c 662e     f"mode:{self.
-000083f0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
-00008400: 276d 6f64 6527 2c20 2727 297d 2022 0a20  'mode', '')} ". 
-00008410: 2020 2020 2020 2020 2020 2066 224f 503a             f"OP:
-00008420: 7b73 656c 662e 6375 7272 656e 745f 6f70  {self.current_op
-00008430: 7d20 7b63 6f6e 7465 7374 5f6e 616d 657d  } {contest_name}
-00008440: 2022 0a20 2020 2020 2020 2020 2020 2066   ".            f
-00008450: 222d 204e 6f74 314d 4d20 767b 5f5f 7665  "- Not1MM v{__ve
-00008460: 7273 696f 6e5f 5f7d 220a 2020 2020 2020  rsion__}".      
-00008470: 2020 290a 2020 2020 2020 2020 6c6f 6767    ).        logg
-00008480: 6572 2e64 6562 7567 2822 2573 222c 206c  er.debug("%s", l
-00008490: 696e 6529 0a20 2020 2020 2020 2073 656c  ine).        sel
-000084a0: 662e 7365 7457 696e 646f 7754 6974 6c65  f.setWindowTitle
-000084b0: 286c 696e 6529 0a0a 2020 2020 6465 6620  (line)..    def 
-000084c0: 636c 6561 7269 6e70 7574 7328 7365 6c66  clearinputs(self
-000084d0: 293a 0a20 2020 2020 2020 2022 2222 436c  ):.        """Cl
-000084e0: 6561 7273 2074 6865 2074 6578 7420 696e  ears the text in
-000084f0: 7075 7420 6669 656c 6473 2061 6e64 2073  put fields and s
-00008500: 6574 7320 666f 6375 7320 746f 2063 616c  ets focus to cal
-00008510: 6c73 6967 6e20 6669 656c 642e 2222 220a  lsign field.""".
-00008520: 2020 2020 2020 2020 7365 6c66 2e64 7570          self.dup
-00008530: 655f 696e 6469 6361 746f 722e 6869 6465  e_indicator.hide
-00008540: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00008550: 636f 6e74 6163 7420 3d20 7365 6c66 2e64  contact = self.d
-00008560: 6174 6162 6173 652e 656d 7074 795f 636f  atabase.empty_co
-00008570: 6e74 6163 740a 2020 2020 2020 2020 7365  ntact.        se
-00008580: 6c66 2e68 6561 6469 6e67 5f64 6973 7461  lf.heading_dista
-00008590: 6e63 652e 7365 7454 6578 7428 2222 290a  nce.setText("").
-000085a0: 2020 2020 2020 2020 7365 6c66 2e64 785f          self.dx_
-000085b0: 656e 7469 7479 2e73 6574 5465 7874 2822  entity.setText("
-000085c0: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
-000085d0: 6c66 2e63 6f6e 7465 7374 3a0a 2020 2020  lf.contest:.    
-000085e0: 2020 2020 2020 2020 6d75 6c74 7320 3d20          mults = 
-000085f0: 7365 6c66 2e63 6f6e 7465 7374 2e73 686f  self.contest.sho
-00008600: 775f 6d75 6c74 7328 7365 6c66 290a 2020  w_mults(self).  
-00008610: 2020 2020 2020 2020 2020 7173 6f73 203d            qsos =
-00008620: 2073 656c 662e 636f 6e74 6573 742e 7368   self.contest.sh
-00008630: 6f77 5f71 736f 2873 656c 6629 0a20 2020  ow_qso(self).   
-00008640: 2020 2020 2020 2020 206d 756c 7473 7472           multstr
-00008650: 696e 6720 3d20 6622 7b71 736f 737d 2f7b  ing = f"{qsos}/{
-00008660: 6d75 6c74 737d 220a 2020 2020 2020 2020  mults}".        
-00008670: 2020 2020 7365 6c66 2e6d 756c 7473 2e73      self.mults.s
-00008680: 6574 5465 7874 286d 756c 7473 7472 696e  etText(multstrin
-00008690: 6729 0a20 2020 2020 2020 2020 2020 2073  g).            s
-000086a0: 636f 7265 203d 2073 656c 662e 636f 6e74  core = self.cont
-000086b0: 6573 742e 6361 6c63 5f73 636f 7265 2873  est.calc_score(s
-000086c0: 656c 6629 0a20 2020 2020 2020 2020 2020  elf).           
-000086d0: 2073 656c 662e 7363 6f72 652e 7365 7454   self.score.setT
-000086e0: 6578 7428 7374 7228 7363 6f72 6529 290a  ext(str(score)).
-000086f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008700: 2e63 6f6e 7465 7374 2e72 6573 6574 5f6c  .contest.reset_l
-00008710: 6162 656c 2873 656c 6629 0a20 2020 2020  abel(self).     
-00008720: 2020 2073 656c 662e 6361 6c6c 7369 676e     self.callsign
-00008730: 2e63 6c65 6172 2829 0a20 2020 2020 2020  .clear().       
-00008740: 2069 6620 7365 6c66 2e63 7572 7265 6e74   if self.current
-00008750: 5f6d 6f64 6520 3d3d 2022 4357 223a 0a20  _mode == "CW":. 
-00008760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008770: 7365 6e74 2e73 6574 5465 7874 2822 3539  sent.setText("59
-00008780: 3922 290a 2020 2020 2020 2020 2020 2020  9").            
-00008790: 7365 6c66 2e72 6563 6569 7665 2e73 6574  self.receive.set
-000087a0: 5465 7874 2822 3539 3922 290a 2020 2020  Text("599").    
-000087b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000087c0: 2020 2020 2020 7365 6c66 2e73 656e 742e        self.sent.
-000087d0: 7365 7454 6578 7428 2235 3922 290a 2020  setText("59").  
-000087e0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-000087f0: 6563 6569 7665 2e73 6574 5465 7874 2822  eceive.setText("
-00008800: 3539 2229 0a20 2020 2020 2020 2073 656c  59").        sel
-00008810: 662e 6f74 6865 725f 312e 636c 6561 7228  f.other_1.clear(
-00008820: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
-00008830: 7468 6572 5f32 2e63 6c65 6172 2829 0a20  ther_2.clear(). 
-00008840: 2020 2020 2020 2073 656c 662e 6361 6c6c         self.call
-00008850: 7369 676e 2e73 6574 466f 6375 7328 290a  sign.setFocus().
-00008860: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
-00008870: 0a20 2020 2020 2020 2063 6d64 5b22 636d  .        cmd["cm
-00008880: 6422 5d20 3d20 2243 414c 4c43 4841 4e47  d"] = "CALLCHANG
-00008890: 4544 220a 2020 2020 2020 2020 636d 645b  ED".        cmd[
-000088a0: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
-000088b0: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
-000088c0: 2020 2020 2063 6d64 5b22 6361 6c6c 225d       cmd["call"]
-000088d0: 203d 2022 220a 2020 2020 2020 2020 7365   = "".        se
-000088e0: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
-000088f0: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
-00008900: 736f 6e28 636d 6429 0a0a 2020 2020 6465  son(cmd)..    de
-00008910: 6620 7361 7665 5f63 6f6e 7461 6374 2873  f save_contact(s
-00008920: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00008930: 2253 6176 6520 746f 2064 6222 2222 0a20  "Save to db""". 
-00008940: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00008950: 6275 6728 2273 6176 696e 6720 636f 6e74  bug("saving cont
-00008960: 6163 7422 290a 2020 2020 2020 2020 6966  act").        if
-00008970: 206c 656e 2873 656c 662e 6361 6c6c 7369   len(self.callsi
-00008980: 676e 2e74 6578 7428 2929 203c 2033 3a0a  gn.text()) < 3:.
-00008990: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000089a0: 726e 0a20 2020 2020 2020 2069 6620 6e6f  rn.        if no
-000089b0: 7420 616e 7928 6368 6172 2e69 7364 6967  t any(char.isdig
-000089c0: 6974 2829 2066 6f72 2063 6861 7220 696e  it() for char in
-000089d0: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
-000089e0: 6578 7428 2929 3a0a 2020 2020 2020 2020  ext()):.        
-000089f0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00008a00: 2020 2069 6620 6e6f 7420 616e 7928 6368     if not any(ch
-00008a10: 6172 2e69 7361 6c70 6861 2829 2066 6f72  ar.isalpha() for
-00008a20: 2063 6861 7220 696e 2073 656c 662e 6361   char in self.ca
-00008a30: 6c6c 7369 676e 2e74 6578 7428 2929 3a0a  llsign.text()):.
-00008a40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00008a50: 726e 0a0a 2020 2020 2020 2020 7365 6c66  rn..        self
-00008a60: 2e63 6f6e 7461 6374 5b22 5453 225d 203d  .contact["TS"] =
-00008a70: 2064 6174 6574 696d 652e 7574 636e 6f77   datetime.utcnow
-00008a80: 2829 2e69 736f 666f 726d 6174 2822 2022  ().isoformat(" "
-00008a90: 295b 3a31 395d 0a20 2020 2020 2020 2073  )[:19].        s
-00008aa0: 656c 662e 636f 6e74 6163 745b 2243 616c  elf.contact["Cal
-00008ab0: 6c22 5d20 3d20 7365 6c66 2e63 616c 6c73  l"] = self.calls
-00008ac0: 6967 6e2e 7465 7874 2829 0a20 2020 2020  ign.text().     
-00008ad0: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
-00008ae0: 2246 7265 7122 5d20 3d20 726f 756e 6428  "Freq"] = round(
-00008af0: 666c 6f61 7428 7365 6c66 2e72 6164 696f  float(self.radio
-00008b00: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
-00008b10: 222c 2030 2e30 2929 202f 2031 3030 302c  ", 0.0)) / 1000,
-00008b20: 2032 290a 2020 2020 2020 2020 7365 6c66   2).        self
-00008b30: 2e63 6f6e 7461 6374 5b22 5153 5846 7265  .contact["QSXFre
-00008b40: 7122 5d20 3d20 726f 756e 6428 0a20 2020  q"] = round(.   
-00008b50: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
-00008b60: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-00008b70: 6765 7428 2276 666f 6122 2c20 302e 3029  get("vfoa", 0.0)
-00008b80: 2920 2f20 3130 3030 2c20 320a 2020 2020  ) / 1000, 2.    
-00008b90: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-00008ba0: 6c66 2e63 6f6e 7461 6374 5b22 4d6f 6465  lf.contact["Mode
-00008bb0: 225d 203d 2073 656c 662e 7261 6469 6f5f  "] = self.radio_
-00008bc0: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
-00008bd0: 2c20 2222 290a 2020 2020 2020 2020 7365  , "").        se
-00008be0: 6c66 2e63 6f6e 7461 6374 5b22 436f 6e74  lf.contact["Cont
-00008bf0: 6573 744e 616d 6522 5d20 3d20 7365 6c66  estName"] = self
-00008c00: 2e63 6f6e 7465 7374 2e63 6162 7269 6c6c  .contest.cabrill
-00008c10: 6f5f 6e61 6d65 0a20 2020 2020 2020 2073  o_name.        s
-00008c20: 656c 662e 636f 6e74 6163 745b 2243 6f6e  elf.contact["Con
-00008c30: 7465 7374 4e52 225d 203d 2073 656c 662e  testNR"] = self.
-00008c40: 7072 6566 2e67 6574 2822 636f 6e74 6573  pref.get("contes
-00008c50: 7422 2c20 2230 2229 0a20 2020 2020 2020  t", "0").       
-00008c60: 2073 656c 662e 636f 6e74 6163 745b 2253   self.contact["S
-00008c70: 7461 7469 6f6e 5072 6566 6978 225d 203d  tationPrefix"] =
-00008c80: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
-00008c90: 7428 2243 616c 6c22 2c20 2222 290a 2020  t("Call", "").  
-00008ca0: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
-00008cb0: 6374 5b22 5750 5850 7265 6669 7822 5d20  ct["WPXPrefix"] 
-00008cc0: 3d20 6361 6c63 756c 6174 655f 7770 785f  = calculate_wpx_
-00008cd0: 7072 6566 6978 2873 656c 662e 6361 6c6c  prefix(self.call
-00008ce0: 7369 676e 2e74 6578 7428 2929 0a20 2020  sign.text()).   
-00008cf0: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-00008d00: 745b 2249 7352 756e 5153 4f22 5d20 3d20  t["IsRunQSO"] = 
-00008d10: 7365 6c66 2e72 6164 696f 4275 7474 6f6e  self.radioButton
-00008d20: 5f72 756e 2e69 7343 6865 636b 6564 2829  _run.isChecked()
-00008d30: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00008d40: 6e74 6163 745b 224f 7065 7261 746f 7222  ntact["Operator"
-00008d50: 5d20 3d20 7365 6c66 2e63 7572 7265 6e74  ] = self.current
-00008d60: 5f6f 700a 2020 2020 2020 2020 7365 6c66  _op.        self
-00008d70: 2e63 6f6e 7461 6374 5b22 4e65 7442 696f  .contact["NetBio
-00008d80: 734e 616d 6522 5d20 3d20 736f 636b 6574  sName"] = socket
-00008d90: 2e67 6574 686f 7374 6e61 6d65 2829 0a20  .gethostname(). 
-00008da0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00008db0: 6163 745b 2249 734f 7269 6769 6e61 6c22  act["IsOriginal"
-00008dc0: 5d20 3d20 310a 2020 2020 2020 2020 7365  ] = 1.        se
-00008dd0: 6c66 2e63 6f6e 7461 6374 5b22 4944 225d  lf.contact["ID"]
-00008de0: 203d 2075 7569 642e 7575 6964 3428 292e   = uuid.uuid4().
-00008df0: 6865 780a 2020 2020 2020 2020 7365 6c66  hex.        self
-00008e00: 2e63 6f6e 7465 7374 2e73 6574 5f63 6f6e  .contest.set_con
-00008e10: 7461 6374 5f76 6172 7328 7365 6c66 290a  tact_vars(self).
-00008e20: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00008e30: 7461 6374 5b22 506f 696e 7473 225d 203d  tact["Points"] =
-00008e40: 2073 656c 662e 636f 6e74 6573 742e 706f   self.contest.po
-00008e50: 696e 7473 2873 656c 6629 0a20 2020 2020  ints(self).     
-00008e60: 2020 2064 6562 7567 5f6f 7574 7075 7420     debug_output 
-00008e70: 3d20 6622 7b73 656c 662e 636f 6e74 6163  = f"{self.contac
-00008e80: 747d 220a 2020 2020 2020 2020 6c6f 6767  t}".        logg
-00008e90: 6572 2e64 6562 7567 2864 6562 7567 5f6f  er.debug(debug_o
-00008ea0: 7574 7075 7429 0a20 2020 2020 2020 2073  utput).        s
-00008eb0: 656c 662e 6461 7461 6261 7365 2e6c 6f67  elf.database.log
-00008ec0: 5f63 6f6e 7461 6374 2873 656c 662e 636f  _contact(self.co
-00008ed0: 6e74 6163 7429 0a20 2020 2020 2020 2073  ntact).        s
-00008ee0: 656c 662e 6e31 6d6d 2e73 656e 645f 636f  elf.n1mm.send_co
-00008ef0: 6e74 6163 745f 696e 666f 2829 0a20 2020  ntact_info().   
-00008f00: 2020 2020 2073 656c 662e 636c 6561 7269       self.cleari
-00008f10: 6e70 7574 7328 290a 2020 2020 2020 2020  nputs().        
-00008f20: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
-00008f30: 2063 6d64 5b22 636d 6422 5d20 3d20 2255   cmd["cmd"] = "U
-00008f40: 5044 4154 454c 4f47 220a 2020 2020 2020  PDATELOG".      
-00008f50: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
-00008f60: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
-00008f70: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00008f80: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
-00008f90: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
-00008fa0: 2863 6d64 290a 2020 2020 2020 2020 2320  (cmd).        # 
-00008fb0: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
-00008fc0: 6e74 6573 744e 616d 6522 5d20 3d20 7365  ntestName"] = se
-00008fd0: 6c66 2e63 6f6e 7465 7374 2e6e 616d 650a  lf.contest.name.
-00008fe0: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
-00008ff0: 6f6e 7461 6374 5b22 534e 5422 5d20 3d20  ontact["SNT"] = 
-00009000: 7365 6c66 2e73 656e 742e 7465 7874 2829  self.sent.text()
-00009010: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
-00009020: 636f 6e74 6163 745b 2252 4356 225d 203d  contact["RCV"] =
-00009030: 2073 656c 662e 7265 6365 6976 652e 7465   self.receive.te
-00009040: 7874 2829 0a20 2020 2020 2020 2023 2073  xt().        # s
-00009050: 656c 662e 636f 6e74 6163 745b 2243 6f75  elf.contact["Cou
-00009060: 6e74 7279 5072 6566 6978 225d 0a20 2020  ntryPrefix"].   
-00009070: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-00009080: 6163 745b 2253 7461 7469 6f6e 5072 6566  act["StationPref
-00009090: 6978 225d 203d 2073 656c 662e 7072 6566  ix"] = self.pref
-000090a0: 2e67 6574 2822 6361 6c6c 7369 676e 222c  .get("callsign",
-000090b0: 2022 2229 0a20 2020 2020 2020 2023 2073   "").        # s
-000090c0: 656c 662e 636f 6e74 6163 745b 2251 5448  elf.contact["QTH
-000090d0: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
-000090e0: 662e 636f 6e74 6163 745b 224e 616d 6522  f.contact["Name"
-000090f0: 5d20 3d20 7365 6c66 2e6f 7468 6572 5f31  ] = self.other_1
-00009100: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-00009110: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
-00009120: 436f 6d6d 656e 7422 5d20 3d20 7365 6c66  Comment"] = self
-00009130: 2e6f 7468 6572 5f32 2e74 6578 7428 290a  .other_2.text().
-00009140: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
-00009150: 6f6e 7461 6374 5b22 4e52 225d 0a20 2020  ontact["NR"].   
-00009160: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-00009170: 6163 745b 2253 6563 7422 5d0a 2020 2020  act["Sect"].    
-00009180: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-00009190: 6374 5b22 5072 6563 225d 0a20 2020 2020  ct["Prec"].     
-000091a0: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-000091b0: 745b 2243 4b22 5d0a 2020 2020 2020 2020  t["CK"].        
-000091c0: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
-000091d0: 5a4e 225d 0a20 2020 2020 2020 2023 2073  ZN"].        # s
-000091e0: 656c 662e 636f 6e74 6163 745b 2253 656e  elf.contact["Sen
-000091f0: 744e 7222 5d0a 2020 2020 2020 2020 2320  tNr"].        # 
-00009200: 7365 6c66 2e63 6f6e 7461 6374 5b22 506f  self.contact["Po
-00009210: 696e 7473 225d 0a20 2020 2020 2020 2023  ints"].        #
-00009220: 2073 656c 662e 636f 6e74 6163 745b 2249   self.contact["I
-00009230: 734d 756c 7469 706c 6965 7231 225d 0a20  sMultiplier1"]. 
-00009240: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-00009250: 6e74 6163 745b 2249 734d 756c 7469 706c  ntact["IsMultipl
-00009260: 6965 7232 225d 0a20 2020 2020 2020 2023  ier2"].        #
-00009270: 2073 656c 662e 636f 6e74 6163 745b 2250   self.contact["P
-00009280: 6f77 6572 225d 0a20 2020 2020 2020 2023  ower"].        #
-00009290: 2073 656c 662e 636f 6e74 6163 745b 2242   self.contact["B
-000092a0: 616e 6422 5d0a 2020 2020 2020 2020 2320  and"].        # 
-000092b0: 7365 6c66 2e63 6f6e 7461 6374 5b22 5750  self.contact["WP
-000092c0: 5850 7265 6669 7822 5d20 3d20 6361 6c63  XPrefix"] = calc
-000092d0: 756c 6174 655f 7770 785f 7072 6566 6978  ulate_wpx_prefix
-000092e0: 2873 656c 662e 6361 6c6c 7369 676e 2e74  (self.callsign.t
-000092f0: 6578 7428 2929 0a20 2020 2020 2020 2023  ext()).        #
-00009300: 2073 656c 662e 636f 6e74 6163 745b 2245   self.contact["E
-00009310: 7863 6861 6e67 6531 225d 0a20 2020 2020  xchange1"].     
-00009320: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-00009330: 745b 2252 6164 696f 4e52 225d 0a20 2020  t["RadioNR"].   
-00009340: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-00009350: 6163 745b 2269 734d 756c 7469 706c 6965  act["isMultiplie
-00009360: 7233 225d 0a20 2020 2020 2020 2023 2073  r3"].        # s
-00009370: 656c 662e 636f 6e74 6163 745b 224d 6973  elf.contact["Mis
-00009380: 6354 6578 7422 5d0a 2020 2020 2020 2020  cText"].        
-00009390: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
-000093a0: 436f 6e74 6163 7454 7970 6522 5d0a 2020  ContactType"].  
-000093b0: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
-000093c0: 7461 6374 5b22 5275 6e31 5275 6e32 225d  tact["Run1Run2"]
-000093d0: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
-000093e0: 636f 6e74 6163 745b 2247 7269 6453 7175  contact["GridSqu
-000093f0: 6172 6522 5d0a 2020 2020 2020 2020 2320  are"].        # 
-00009400: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
-00009410: 6e74 696e 656e 7422 5d0a 2020 2020 2020  ntinent"].      
-00009420: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
-00009430: 5b22 526f 7665 724c 6f63 6174 696f 6e22  ["RoverLocation"
-00009440: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
-00009450: 2e63 6f6e 7461 6374 5b22 5261 6469 6f49  .contact["RadioI
-00009460: 6e74 6572 6661 6365 6422 5d0a 2020 2020  nterfaced"].    
-00009470: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-00009480: 6374 5b22 4e65 7477 6f72 6b65 6443 6f6d  ct["NetworkedCom
-00009490: 704e 7222 5d0a 2020 2020 2020 2020 2320  pNr"].        # 
-000094a0: 7365 6c66 2e63 6f6e 7461 6374 5b22 434c  self.contact["CL
-000094b0: 4149 4d45 4451 534f 225d 0a0a 2020 2020  AIMEDQSO"]..    
-000094c0: 6465 6620 6e65 775f 636f 6e74 6573 745f  def new_contest_
-000094d0: 6469 616c 6f67 2873 656c 6629 3a0a 2020  dialog(self):.  
-000094e0: 2020 2020 2020 2222 2253 686f 7720 6e65        """Show ne
-000094f0: 7720 636f 6e74 6573 7420 6469 616c 6f67  w contest dialog
-00009500: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
-00009510: 6572 2e64 6562 7567 2822 4e65 7720 636f  er.debug("New co
-00009520: 6e74 6573 7420 4469 616c 6f67 2229 0a20  ntest Dialog"). 
-00009530: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00009540: 6573 745f 6469 616c 6f67 203d 204e 6577  est_dialog = New
-00009550: 436f 6e74 6573 7428 574f 524b 494e 475f  Contest(WORKING_
-00009560: 5041 5448 290a 2020 2020 2020 2020 7365  PATH).        se
-00009570: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00009580: 672e 6163 6365 7074 6564 2e63 6f6e 6e65  g.accepted.conne
-00009590: 6374 2873 656c 662e 7361 7665 5f63 6f6e  ct(self.save_con
-000095a0: 7465 7374 290a 2020 2020 2020 2020 6966  test).        if
-000095b0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-000095c0: 6461 726b 5f6d 6f64 6522 293a 0a20 2020  dark_mode"):.   
-000095d0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-000095e0: 6e74 6573 745f 6469 616c 6f67 2e73 6574  ntest_dialog.set
-000095f0: 5374 796c 6553 6865 6574 2844 4152 4b5f  StyleSheet(DARK_
-00009600: 5354 594c 4553 4845 4554 290a 2020 2020  STYLESHEET).    
-00009610: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00009620: 5f64 6961 6c6f 672e 6461 7465 5469 6d65  _dialog.dateTime
-00009630: 4564 6974 2e73 6574 4461 7465 2851 7443  Edit.setDate(QtC
-00009640: 6f72 652e 5144 6174 652e 6375 7272 656e  ore.QDate.curren
-00009650: 7444 6174 6528 2929 0a20 2020 2020 2020  tDate()).       
-00009660: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00009670: 616c 6f67 2e64 6174 6554 696d 6545 6469  alog.dateTimeEdi
-00009680: 742e 7365 7443 616c 656e 6461 7250 6f70  t.setCalendarPop
-00009690: 7570 2854 7275 6529 0a20 2020 2020 2020  up(True).       
-000096a0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-000096b0: 616c 6f67 2e64 6174 6554 696d 6545 6469  alog.dateTimeEdi
-000096c0: 742e 7365 7454 696d 6528 5174 436f 7265  t.setTime(QtCore
-000096d0: 2e51 5469 6d65 2830 2c20 3029 290a 2020  .QTime(0, 0)).  
-000096e0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-000096f0: 7374 5f64 6961 6c6f 672e 706f 7765 722e  st_dialog.power.
-00009700: 7365 7443 7572 7265 6e74 5465 7874 2822  setCurrentText("
-00009710: 4c4f 5722 290a 2020 2020 2020 2020 7365  LOW").        se
-00009720: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00009730: 672e 7374 6174 696f 6e2e 7365 7443 7572  g.station.setCur
-00009740: 7265 6e74 5465 7874 2822 4649 5845 4422  rentText("FIXED"
-00009750: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00009760: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f70  ontest_dialog.op
-00009770: 656e 2829 0a0a 2020 2020 6465 6620 7361  en()..    def sa
-00009780: 7665 5f63 6f6e 7465 7374 2873 656c 6629  ve_contest(self)
-00009790: 3a0a 2020 2020 2020 2020 2222 2253 6176  :.        """Sav
-000097a0: 6520 436f 6e74 6573 7422 2222 0a20 2020  e Contest""".   
-000097b0: 2020 2020 206e 6578 745f 6e75 6d62 6572       next_number
-000097c0: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
-000097d0: 2e67 6574 5f6e 6578 745f 636f 6e74 6573  .get_next_contes
-000097e0: 745f 6e72 2829 0a20 2020 2020 2020 2063  t_nr().        c
-000097f0: 6f6e 7465 7374 203d 207b 7d0a 2020 2020  ontest = {}.    
-00009800: 2020 2020 636f 6e74 6573 745b 2243 6f6e      contest["Con
-00009810: 7465 7374 4e61 6d65 225d 203d 2028 0a20  testName"] = (. 
-00009820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009830: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
-00009840: 6f6e 7465 7374 2e63 7572 7265 6e74 5465  ontest.currentTe
-00009850: 7874 2829 2e6c 6f77 6572 2829 2e72 6570  xt().lower().rep
-00009860: 6c61 6365 2822 2022 2c20 225f 2229 0a20  lace(" ", "_"). 
-00009870: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00009880: 2063 6f6e 7465 7374 5b22 5374 6172 7444   contest["StartD
-00009890: 6174 6522 5d20 3d20 7365 6c66 2e63 6f6e  ate"] = self.con
-000098a0: 7465 7374 5f64 6961 6c6f 672e 6461 7465  test_dialog.date
-000098b0: 5469 6d65 4564 6974 2e64 6174 6554 696d  TimeEdit.dateTim
-000098c0: 6528 292e 746f 5374 7269 6e67 280a 2020  e().toString(.  
-000098d0: 2020 2020 2020 2020 2020 2279 7979 792d            "yyyy-
-000098e0: 4d4d 2d64 6420 6868 3a6d 6d3a 7373 220a  MM-dd hh:mm:ss".
-000098f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00009900: 2020 636f 6e74 6573 745b 224f 7065 7261    contest["Opera
-00009910: 746f 7243 6174 6567 6f72 7922 5d20 3d20  torCategory"] = 
-00009920: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00009930: 6c6f 672e 6f70 6572 6174 6f72 5f63 6c61  log.operator_cla
-00009940: 7373 2e63 7572 7265 6e74 5465 7874 2829  ss.currentText()
-00009950: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-00009960: 5b22 4261 6e64 4361 7465 676f 7279 225d  ["BandCategory"]
-00009970: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-00009980: 6469 616c 6f67 2e62 616e 642e 6375 7272  dialog.band.curr
-00009990: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
-000099a0: 2020 636f 6e74 6573 745b 2250 6f77 6572    contest["Power
-000099b0: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
-000099c0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-000099d0: 2e70 6f77 6572 2e63 7572 7265 6e74 5465  .power.currentTe
-000099e0: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
-000099f0: 7465 7374 5b22 4d6f 6465 4361 7465 676f  test["ModeCatego
-00009a00: 7279 225d 203d 2073 656c 662e 636f 6e74  ry"] = self.cont
-00009a10: 6573 745f 6469 616c 6f67 2e6d 6f64 652e  est_dialog.mode.
-00009a20: 6375 7272 656e 7454 6578 7428 290a 2020  currentText().  
-00009a30: 2020 2020 2020 636f 6e74 6573 745b 224f        contest["O
-00009a40: 7665 726c 6179 4361 7465 676f 7279 225d  verlayCategory"]
-00009a50: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-00009a60: 6469 616c 6f67 2e6f 7665 726c 6179 2e63  dialog.overlay.c
-00009a70: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
-00009a80: 2020 2020 2023 2063 6f6e 7465 7374 5b27       # contest['
-00009a90: 436c 6169 6d65 6453 636f 7265 275d 203d  ClaimedScore'] =
-00009aa0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00009ab0: 616c 6f67 2e0a 2020 2020 2020 2020 636f  alog..        co
-00009ac0: 6e74 6573 745b 224f 7065 7261 746f 7273  ntest["Operators
-00009ad0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-00009ae0: 745f 6469 616c 6f67 2e6f 7065 7261 746f  t_dialog.operato
-00009af0: 7273 2e74 6578 7428 290a 2020 2020 2020  rs.text().      
-00009b00: 2020 636f 6e74 6573 745b 2253 6f61 7062    contest["Soapb
-00009b10: 6f78 225d 203d 2073 656c 662e 636f 6e74  ox"] = self.cont
-00009b20: 6573 745f 6469 616c 6f67 2e73 6f61 7062  est_dialog.soapb
-00009b30: 6f78 2e74 6f50 6c61 696e 5465 7874 2829  ox.toPlainText()
-00009b40: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-00009b50: 5b22 5365 6e74 4578 6368 616e 6765 225d  ["SentExchange"]
-00009b60: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-00009b70: 6469 616c 6f67 2e65 7863 6861 6e67 652e  dialog.exchange.
-00009b80: 7465 7874 2829 0a20 2020 2020 2020 2063  text().        c
-00009b90: 6f6e 7465 7374 5b22 436f 6e74 6573 744e  ontest["ContestN
-00009ba0: 5222 5d20 3d20 6e65 7874 5f6e 756d 6265  R"] = next_numbe
-00009bb0: 722e 6765 7428 2263 6f75 6e74 222c 2031  r.get("count", 1
-00009bc0: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
-00009bd0: 7265 665b 2263 6f6e 7465 7374 225d 203d  ref["contest"] =
-00009be0: 206e 6578 745f 6e75 6d62 6572 2e67 6574   next_number.get
-00009bf0: 2822 636f 756e 7422 2c20 3129 0a20 2020  ("count", 1).   
-00009c00: 2020 2020 2023 2063 6f6e 7465 7374 5b27       # contest['
-00009c10: 5375 6254 7970 6527 5d20 3d20 7365 6c66  SubType'] = self
-00009c20: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00009c30: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-00009c40: 5b22 5374 6174 696f 6e43 6174 6567 6f72  ["StationCategor
-00009c50: 7922 5d20 3d20 7365 6c66 2e63 6f6e 7465  y"] = self.conte
-00009c60: 7374 5f64 6961 6c6f 672e 7374 6174 696f  st_dialog.statio
-00009c70: 6e2e 6375 7272 656e 7454 6578 7428 290a  n.currentText().
-00009c80: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
-00009c90: 2241 7373 6973 7465 6443 6174 6567 6f72  "AssistedCategor
-00009ca0: 7922 5d20 3d20 7365 6c66 2e63 6f6e 7465  y"] = self.conte
-00009cb0: 7374 5f64 6961 6c6f 672e 6173 7369 7374  st_dialog.assist
-00009cc0: 6564 2e63 7572 7265 6e74 5465 7874 2829  ed.currentText()
-00009cd0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-00009ce0: 5b22 5472 616e 736d 6974 7465 7243 6174  ["TransmitterCat
-00009cf0: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
-00009d00: 6f6e 7465 7374 5f64 6961 6c6f 672e 7472  ontest_dialog.tr
-00009d10: 616e 736d 6974 7465 722e 6375 7272 656e  ansmitter.curren
-00009d20: 7454 6578 7428 290a 2020 2020 2020 2020  tText().        
-00009d30: 2320 636f 6e74 6573 745b 2754 696d 6543  # contest['TimeC
-00009d40: 6174 6567 6f72 7927 5d20 3d20 7365 6c66  ategory'] = self
-00009d50: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00009d60: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00009d70: 6465 6275 6728 2225 7322 2c20 6622 7b63  debug("%s", f"{c
-00009d80: 6f6e 7465 7374 7d22 290a 2020 2020 2020  ontest}").      
-00009d90: 2020 7365 6c66 2e64 6174 6162 6173 652e    self.database.
-00009da0: 6164 645f 636f 6e74 6573 7428 636f 6e74  add_contest(cont
-00009db0: 6573 7429 0a20 2020 2020 2020 2073 656c  est).        sel
-00009dc0: 662e 7772 6974 655f 7072 6566 6572 656e  f.write_preferen
-00009dd0: 6365 2829 0a20 2020 2020 2020 2073 656c  ce().        sel
-00009de0: 662e 6c6f 6164 5f63 6f6e 7465 7374 2829  f.load_contest()
-00009df0: 0a0a 2020 2020 6465 6620 6564 6974 5f73  ..    def edit_s
-00009e00: 7461 7469 6f6e 5f73 6574 7469 6e67 7328  tation_settings(
-00009e10: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00009e20: 2222 5368 6f77 2073 6574 7469 6e67 7320  ""Show settings 
-00009e30: 6469 616c 6f67 2222 220a 2020 2020 2020  dialog""".      
-00009e40: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-00009e50: 5374 6174 696f 6e20 5365 7474 696e 6773  Station Settings
-00009e60: 2073 656c 6563 7465 6422 290a 2020 2020   selected").    
-00009e70: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-00009e80: 735f 6469 616c 6f67 203d 2045 6469 7453  s_dialog = EditS
-00009e90: 7461 7469 6f6e 2857 4f52 4b49 4e47 5f50  tation(WORKING_P
-00009ea0: 4154 4829 0a20 2020 2020 2020 2069 6620  ATH).        if 
-00009eb0: 7365 6c66 2e70 7265 662e 6765 7428 2264  self.pref.get("d
-00009ec0: 6172 6b5f 6d6f 6465 2229 3a0a 2020 2020  ark_mode"):.    
-00009ed0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00009ee0: 7469 6e67 735f 6469 616c 6f67 2e73 6574  tings_dialog.set
-00009ef0: 5374 796c 6553 6865 6574 2844 4152 4b5f  StyleSheet(DARK_
-00009f00: 5354 594c 4553 4845 4554 290a 2020 2020  STYLESHEET).    
-00009f10: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-00009f20: 735f 6469 616c 6f67 2e61 6363 6570 7465  s_dialog.accepte
-00009f30: 642e 636f 6e6e 6563 7428 7365 6c66 2e73  d.connect(self.s
-00009f40: 6176 655f 7365 7474 696e 6773 290a 2020  ave_settings).  
-00009f50: 2020 2020 2020 2320 6966 2073 656c 662e        # if self.
-00009f60: 7072 6566 2e67 6574 2822 6461 726b 5f6d  pref.get("dark_m
-00009f70: 6f64 6522 293a 0a20 2020 2020 2020 2023  ode"):.        #
-00009f80: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-00009f90: 6773 5f64 6961 6c6f 672e 7365 7453 7479  gs_dialog.setSty
-00009fa0: 6c65 5368 6565 7428 4441 524b 5f53 5459  leSheet(DARK_STY
-00009fb0: 4c45 5348 4545 5429 0a0a 2020 2020 2020  LESHEET)..      
-00009fc0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-00009fd0: 6469 616c 6f67 2e43 616c 6c2e 7365 7454  dialog.Call.setT
-00009fe0: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
-00009ff0: 2e67 6574 2822 4361 6c6c 222c 2022 2229  .get("Call", "")
-0000a000: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000a010: 6574 7469 6e67 735f 6469 616c 6f67 2e4e  ettings_dialog.N
-0000a020: 616d 652e 7365 7454 6578 7428 7365 6c66  ame.setText(self
-0000a030: 2e73 7461 7469 6f6e 2e67 6574 2822 4e61  .station.get("Na
-0000a040: 6d65 222c 2022 2229 290a 2020 2020 2020  me", "")).      
-0000a050: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-0000a060: 6469 616c 6f67 2e41 6464 7265 7373 312e  dialog.Address1.
-0000a070: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
-0000a080: 7469 6f6e 2e67 6574 2822 5374 7265 6574  tion.get("Street
-0000a090: 3122 2c20 2222 2929 0a20 2020 2020 2020  1", "")).       
-0000a0a0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000a0b0: 6961 6c6f 672e 4164 6472 6573 7332 2e73  ialog.Address2.s
-0000a0c0: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
-0000a0d0: 696f 6e2e 6765 7428 2253 7472 6565 7432  ion.get("Street2
-0000a0e0: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
-0000a0f0: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000a100: 616c 6f67 2e43 6974 792e 7365 7454 6578  alog.City.setTex
-0000a110: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
-0000a120: 6574 2822 4369 7479 222c 2022 2229 290a  et("City", "")).
-0000a130: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000a140: 7469 6e67 735f 6469 616c 6f67 2e53 7461  tings_dialog.Sta
-0000a150: 7465 2e73 6574 5465 7874 2873 656c 662e  te.setText(self.
-0000a160: 7374 6174 696f 6e2e 6765 7428 2253 7461  station.get("Sta
-0000a170: 7465 222c 2022 2229 290a 2020 2020 2020  te", "")).      
-0000a180: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-0000a190: 6469 616c 6f67 2e5a 6970 2e73 6574 5465  dialog.Zip.setTe
-0000a1a0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
-0000a1b0: 6765 7428 225a 6970 222c 2022 2229 290a  get("Zip", "")).
-0000a1c0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000a1d0: 7469 6e67 735f 6469 616c 6f67 2e43 6f75  tings_dialog.Cou
-0000a1e0: 6e74 7279 2e73 6574 5465 7874 2873 656c  ntry.setText(sel
-0000a1f0: 662e 7374 6174 696f 6e2e 6765 7428 2243  f.station.get("C
-0000a200: 6f75 6e74 7279 222c 2022 2229 290a 2020  ountry", "")).  
-0000a210: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-0000a220: 6e67 735f 6469 616c 6f67 2e47 7269 6453  ngs_dialog.GridS
-0000a230: 7175 6172 652e 7365 7454 6578 7428 7365  quare.setText(se
-0000a240: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-0000a250: 4772 6964 5371 7561 7265 222c 2022 2229  GridSquare", "")
-0000a260: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000a270: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
-0000a280: 515a 6f6e 652e 7365 7454 6578 7428 7374  QZone.setText(st
-0000a290: 7228 7365 6c66 2e73 7461 7469 6f6e 2e67  r(self.station.g
-0000a2a0: 6574 2822 4351 5a6f 6e65 222c 2022 2229  et("CQZone", "")
-0000a2b0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0000a2c0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000a2d0: 4954 555a 6f6e 652e 7365 7454 6578 7428  ITUZone.setText(
-0000a2e0: 7374 7228 7365 6c66 2e73 7461 7469 6f6e  str(self.station
-0000a2f0: 2e67 6574 2822 4941 5255 5a6f 6e65 222c  .get("IARUZone",
-0000a300: 2022 2229 2929 0a20 2020 2020 2020 2073   ""))).        s
-0000a310: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000a320: 6c6f 672e 4c69 6365 6e73 652e 7365 7454  log.License.setT
-0000a330: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
-0000a340: 2e67 6574 2822 4c69 6365 6e73 6543 6c61  .get("LicenseCla
-0000a350: 7373 222c 2022 2229 290a 2020 2020 2020  ss", "")).      
-0000a360: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-0000a370: 6469 616c 6f67 2e4c 6174 6974 7564 652e  dialog.Latitude.
-0000a380: 7365 7454 6578 7428 7374 7228 7365 6c66  setText(str(self
-0000a390: 2e73 7461 7469 6f6e 2e67 6574 2822 4c61  .station.get("La
-0000a3a0: 7469 7475 6465 222c 2022 2229 2929 0a20  titude", ""))). 
-0000a3b0: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000a3c0: 696e 6773 5f64 6961 6c6f 672e 4c6f 6e67  ings_dialog.Long
-0000a3d0: 6974 7564 652e 7365 7454 6578 7428 7374  itude.setText(st
-0000a3e0: 7228 7365 6c66 2e73 7461 7469 6f6e 2e67  r(self.station.g
-0000a3f0: 6574 2822 4c6f 6e67 6974 7564 6522 2c20  et("Longitude", 
-0000a400: 2222 2929 290a 2020 2020 2020 2020 7365  ""))).        se
-0000a410: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000a420: 6f67 2e53 7461 7469 6f6e 5458 5258 2e73  og.StationTXRX.s
-0000a430: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
-0000a440: 696f 6e2e 6765 7428 2273 7461 7469 6f6e  ion.get("station
-0000a450: 7478 7278 222c 2022 2229 290a 2020 2020  txrx", "")).    
-0000a460: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-0000a470: 735f 6469 616c 6f67 2e50 6f77 6572 2e73  s_dialog.Power.s
-0000a480: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
-0000a490: 696f 6e2e 6765 7428 2253 506f 7765 222c  ion.get("SPowe",
-0000a4a0: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
-0000a4b0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000a4c0: 6f67 2e41 6e74 656e 6e61 2e73 6574 5465  og.Antenna.setTe
-0000a4d0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
-0000a4e0: 6765 7428 2253 416e 7465 222c 2022 2229  get("SAnte", "")
-0000a4f0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000a500: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
-0000a510: 6e74 4865 6967 6874 2e73 6574 5465 7874  ntHeight.setText
-0000a520: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-0000a530: 7428 2253 416e 7448 3122 2c20 2222 2929  t("SAntH1", ""))
-0000a540: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000a550: 7474 696e 6773 5f64 6961 6c6f 672e 4153  ttings_dialog.AS
-0000a560: 4c2e 7365 7454 6578 7428 7365 6c66 2e73  L.setText(self.s
-0000a570: 7461 7469 6f6e 2e67 6574 2822 5341 6e74  tation.get("SAnt
-0000a580: 4832 222c 2022 2229 290a 2020 2020 2020  H2", "")).      
-0000a590: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-0000a5a0: 6469 616c 6f67 2e41 5252 4c53 6563 7469  dialog.ARRLSecti
-0000a5b0: 6f6e 2e73 6574 5465 7874 2873 656c 662e  on.setText(self.
-0000a5c0: 7374 6174 696f 6e2e 6765 7428 2241 5252  station.get("ARR
-0000a5d0: 4c53 6563 7469 6f6e 222c 2022 2229 290a  LSection", "")).
-0000a5e0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000a5f0: 7469 6e67 735f 6469 616c 6f67 2e52 6f76  tings_dialog.Rov
-0000a600: 6572 5154 482e 7365 7454 6578 7428 7365  erQTH.setText(se
-0000a610: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-0000a620: 526f 7665 7251 5448 222c 2022 2229 290a  RoverQTH", "")).
-0000a630: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000a640: 7469 6e67 735f 6469 616c 6f67 2e43 6c75  tings_dialog.Clu
-0000a650: 622e 7365 7454 6578 7428 7365 6c66 2e73  b.setText(self.s
-0000a660: 7461 7469 6f6e 2e67 6574 2822 436c 7562  tation.get("Club
-0000a670: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
-0000a680: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000a690: 616c 6f67 2e45 6d61 696c 2e73 6574 5465  alog.Email.setTe
-0000a6a0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
-0000a6b0: 6765 7428 2245 6d61 696c 222c 2022 2229  get("Email", "")
-0000a6c0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000a6d0: 6574 7469 6e67 735f 6469 616c 6f67 2e6f  ettings_dialog.o
-0000a6e0: 7065 6e28 290a 0a20 2020 2064 6566 2073  pen()..    def s
-0000a6f0: 6176 655f 7365 7474 696e 6773 2873 656c  ave_settings(sel
-0000a700: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
-0000a710: 6176 6520 7365 7474 696e 6773 2222 220a  ave settings""".
-0000a720: 2020 2020 2020 2020 6373 203d 2073 656c          cs = sel
-0000a730: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000a740: 672e 4361 6c6c 2e74 6578 7428 290a 2020  g.Call.text().  
-0000a750: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-0000a760: 6f6e 203d 207b 7d0a 2020 2020 2020 2020  on = {}.        
-0000a770: 7365 6c66 2e73 7461 7469 6f6e 5b22 4361  self.station["Ca
-0000a780: 6c6c 225d 203d 2063 732e 7570 7065 7228  ll"] = cs.upper(
-0000a790: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000a7a0: 7461 7469 6f6e 5b22 4e61 6d65 225d 203d  tation["Name"] =
-0000a7b0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000a7c0: 6961 6c6f 672e 4e61 6d65 2e74 6578 7428  ialog.Name.text(
-0000a7d0: 292e 7469 746c 6528 290a 2020 2020 2020  ).title().      
-0000a7e0: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
-0000a7f0: 5374 7265 6574 3122 5d20 3d20 7365 6c66  Street1"] = self
-0000a800: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000a810: 2e41 6464 7265 7373 312e 7465 7874 2829  .Address1.text()
-0000a820: 2e74 6974 6c65 2829 0a20 2020 2020 2020  .title().       
-0000a830: 2073 656c 662e 7374 6174 696f 6e5b 2253   self.station["S
-0000a840: 7472 6565 7432 225d 203d 2073 656c 662e  treet2"] = self.
-0000a850: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000a860: 4164 6472 6573 7332 2e74 6578 7428 292e  Address2.text().
-0000a870: 7469 746c 6528 290a 2020 2020 2020 2020  title().        
-0000a880: 7365 6c66 2e73 7461 7469 6f6e 5b22 4369  self.station["Ci
-0000a890: 7479 225d 203d 2073 656c 662e 7365 7474  ty"] = self.sett
-0000a8a0: 696e 6773 5f64 6961 6c6f 672e 4369 7479  ings_dialog.City
-0000a8b0: 2e74 6578 7428 292e 7469 746c 6528 290a  .text().title().
-0000a8c0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0000a8d0: 7469 6f6e 5b22 5374 6174 6522 5d20 3d20  tion["State"] = 
-0000a8e0: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000a8f0: 616c 6f67 2e53 7461 7465 2e74 6578 7428  alog.State.text(
-0000a900: 292e 7570 7065 7228 290a 2020 2020 2020  ).upper().      
-0000a910: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
-0000a920: 5a69 7022 5d20 3d20 7365 6c66 2e73 6574  Zip"] = self.set
-0000a930: 7469 6e67 735f 6469 616c 6f67 2e5a 6970  tings_dialog.Zip
-0000a940: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-0000a950: 7365 6c66 2e73 7461 7469 6f6e 5b22 436f  self.station["Co
-0000a960: 756e 7472 7922 5d20 3d20 7365 6c66 2e73  untry"] = self.s
-0000a970: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
-0000a980: 6f75 6e74 7279 2e74 6578 7428 292e 7469  ountry.text().ti
-0000a990: 746c 6528 290a 2020 2020 2020 2020 7365  tle().        se
-0000a9a0: 6c66 2e73 7461 7469 6f6e 5b22 4772 6964  lf.station["Grid
-0000a9b0: 5371 7561 7265 225d 203d 2073 656c 662e  Square"] = self.
-0000a9c0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000a9d0: 4772 6964 5371 7561 7265 2e74 6578 7428  GridSquare.text(
+00006fd0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00006fe0: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
+00006ff0: 742e 4b65 792e 4b65 795f 4573 6361 7065  t.Key.Key_Escape
+00007000: 2061 6e64 206d 6f64 6966 6965 7220 213d   and modifier !=
+00007010: 2051 742e 436f 6e74 726f 6c4d 6f64 6966   Qt.ControlModif
+00007020: 6965 720a 2020 2020 2020 2020 293a 2020  ier.        ):  
+00007030: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
+00007040: 653d 6e6f 2d6d 656d 6265 720a 2020 2020  e=no-member.    
+00007050: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
+00007060: 6172 696e 7075 7473 2829 0a20 2020 2020  arinputs().     
+00007070: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00007080: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
+00007090: 6579 2829 203d 3d20 5174 2e4b 6579 2e4b  ey() == Qt.Key.K
+000070a0: 6579 5f45 7363 6170 6520 616e 6420 6d6f  ey_Escape and mo
+000070b0: 6469 6669 6572 203d 3d20 5174 2e43 6f6e  difier == Qt.Con
+000070c0: 7472 6f6c 4d6f 6469 6669 6572 3a0a 2020  trolModifier:.  
+000070d0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+000070e0: 662e 6377 2069 7320 6e6f 7420 4e6f 6e65  f.cw is not None
+000070f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007100: 2020 6966 2073 656c 662e 6377 2e73 6572    if self.cw.ser
+00007110: 7665 7274 7970 6520 3d3d 2031 3a0a 2020  vertype == 1:.  
+00007120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007130: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
+00007140: 2822 5c78 3162 3422 290a 2020 2020 2020  ("\x1b4").      
+00007150: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00007160: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+00007170: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
+00007180: 742e 4b65 792e 4b65 795f 5061 6765 5570  t.Key.Key_PageUp
+00007190: 2061 6e64 206d 6f64 6966 6965 7220 3d3d   and modifier ==
+000071a0: 2051 742e 436f 6e74 726f 6c4d 6f64 6966   Qt.ControlModif
+000071b0: 6965 723a 0a20 2020 2020 2020 2020 2020  ier:.           
+000071c0: 2063 6d64 203d 207b 7d0a 2020 2020 2020   cmd = {}.      
+000071d0: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
+000071e0: 203d 2022 4e45 5854 5350 4f54 220a 2020   = "NEXTSPOT".  
+000071f0: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
+00007200: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
+00007210: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
+00007220: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
+00007230: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
+00007240: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
+00007250: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00007260: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+00007270: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
+00007280: 742e 4b65 792e 4b65 795f 5061 6765 446f  t.Key.Key_PageDo
+00007290: 776e 2061 6e64 206d 6f64 6966 6965 7220  wn and modifier 
+000072a0: 3d3d 2051 742e 436f 6e74 726f 6c4d 6f64  == Qt.ControlMod
+000072b0: 6966 6965 723a 0a20 2020 2020 2020 2020  ifier:.         
+000072c0: 2020 2063 6d64 203d 207b 7d0a 2020 2020     cmd = {}.    
+000072d0: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
+000072e0: 225d 203d 2022 5052 4556 5350 4f54 220a  "] = "PREVSPOT".
+000072f0: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+00007300: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
+00007310: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
+00007320: 2020 2020 2020 2020 2073 656c 662e 6d75           self.mu
+00007330: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
+00007340: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
+00007350: 6d64 290a 2020 2020 2020 2020 2020 2020  md).            
+00007360: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
+00007370: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+00007380: 2051 742e 4b65 792e 4b65 795f 5061 6765   Qt.Key.Key_Page
+00007390: 5570 2061 6e64 206d 6f64 6966 6965 7220  Up and modifier 
+000073a0: 213d 2051 742e 436f 6e74 726f 6c4d 6f64  != Qt.ControlMod
+000073b0: 6966 6965 723a 0a20 2020 2020 2020 2020  ifier:.         
+000073c0: 2020 2069 6620 7365 6c66 2e63 7720 6973     if self.cw is
+000073d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000073e0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000073f0: 6c66 2e63 772e 7365 7276 6572 7479 7065  lf.cw.servertype
+00007400: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
+00007410: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007420: 6377 2e73 7065 6564 202b 3d20 310a 2020  cw.speed += 1.  
+00007430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007440: 2020 7365 6c66 2e63 775f 7370 6565 642e    self.cw_speed.
+00007450: 7365 7456 616c 7565 2873 656c 662e 6377  setValue(self.cw
+00007460: 2e73 7065 6564 290a 2020 2020 2020 2020  .speed).        
+00007470: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007480: 2e63 772e 7365 6e64 6377 2866 225c 7831  .cw.sendcw(f"\x1
+00007490: 6232 7b73 656c 662e 6377 2e73 7065 6564  b2{self.cw.speed
+000074a0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+000074b0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+000074c0: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
+000074d0: 6b65 7928 2920 3d3d 2051 742e 4b65 792e  key() == Qt.Key.
+000074e0: 4b65 795f 5061 6765 446f 776e 2061 6e64  Key_PageDown and
+000074f0: 206d 6f64 6966 6965 7220 213d 2051 742e   modifier != Qt.
+00007500: 436f 6e74 726f 6c4d 6f64 6966 6965 723a  ControlModifier:
+00007510: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00007520: 7365 6c66 2e63 7720 6973 206e 6f74 204e  self.cw is not N
+00007530: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00007540: 2020 2020 2069 6620 7365 6c66 2e63 772e       if self.cw.
+00007550: 7365 7276 6572 7479 7065 203d 3d20 313a  servertype == 1:
+00007560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007570: 2020 2020 2073 656c 662e 6377 2e73 7065       self.cw.spe
+00007580: 6564 202d 3d20 310a 2020 2020 2020 2020  ed -= 1.        
+00007590: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000075a0: 2e63 775f 7370 6565 642e 7365 7456 616c  .cw_speed.setVal
+000075b0: 7565 2873 656c 662e 6377 2e73 7065 6564  ue(self.cw.speed
+000075c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000075d0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+000075e0: 6e64 6377 2866 225c 7831 6232 7b73 656c  ndcw(f"\x1b2{sel
+000075f0: 662e 6377 2e73 7065 6564 7d22 290a 2020  f.cw.speed}").  
+00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007610: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00007620: 2023 2069 6620 6576 656e 742e 6b65 7928   # if event.key(
+00007630: 2920 3d3d 2051 742e 4b65 792e 4b65 795f  ) == Qt.Key.Key_
+00007640: 456e 7465 723a 0a20 2020 2020 2020 2023  Enter:.        #
+00007650: 2020 2020 2073 656c 662e 7361 7665 5f63       self.save_c
+00007660: 6f6e 7461 6374 2829 0a20 2020 2020 2020  ontact().       
+00007670: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
+00007680: 3d3d 2051 742e 4b65 792e 4b65 795f 5461  == Qt.Key.Key_Ta
+00007690: 6220 6f72 2065 7665 6e74 2e6b 6579 2829  b or event.key()
+000076a0: 203d 3d20 5174 2e4b 6579 2e4b 6579 5f42   == Qt.Key.Key_B
+000076b0: 6163 6b74 6162 3a0a 2020 2020 2020 2020  acktab:.        
+000076c0: 2020 2020 6966 2073 656c 662e 7365 6e74      if self.sent
+000076d0: 2e68 6173 466f 6375 7328 293a 0a20 2020  .hasFocus():.   
+000076e0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+000076f0: 6765 722e 6465 6275 6728 2246 726f 6d20  ger.debug("From 
+00007700: 7365 6e74 2229 0a20 2020 2020 2020 2020  sent").         
+00007710: 2020 2020 2020 2069 6620 6d6f 6469 6669         if modifi
+00007720: 6572 203d 3d20 5174 2e53 6869 6674 4d6f  er == Qt.ShiftMo
+00007730: 6469 6669 6572 3a0a 2020 2020 2020 2020  difier:.        
+00007740: 2020 2020 2020 2020 2020 2020 7072 6576              prev
+00007750: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
+00007760: 7072 6576 2e67 6574 2873 656c 662e 7365  prev.get(self.se
+00007770: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
+00007780: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
+00007790: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
+000077a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077b0: 7072 6576 5f74 6162 2e64 6573 656c 6563  prev_tab.deselec
+000077c0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+000077d0: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
+000077e0: 2e65 6e64 2846 616c 7365 290a 2020 2020  .end(False).    
+000077f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00007800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007810: 2020 2020 2020 6e65 7874 5f74 6162 203d        next_tab =
+00007820: 2073 656c 662e 7461 625f 6e65 7874 2e67   self.tab_next.g
+00007830: 6574 2873 656c 662e 7365 6e74 290a 2020  et(self.sent).  
+00007840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007850: 2020 6e65 7874 5f74 6162 2e73 6574 466f    next_tab.setFo
+00007860: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
+00007870: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
+00007880: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
+00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078a0: 2020 6e65 7874 5f74 6162 2e65 6e64 2846    next_tab.end(F
+000078b0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+000078c0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+000078d0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000078e0: 2e72 6563 6569 7665 2e68 6173 466f 6375  .receive.hasFocu
+000078f0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+00007900: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00007910: 6728 2246 726f 6d20 7265 6365 6976 6522  g("From receive"
+00007920: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00007930: 2020 6966 206d 6f64 6966 6965 7220 3d3d    if modifier ==
+00007940: 2051 742e 5368 6966 744d 6f64 6966 6965   Qt.ShiftModifie
+00007950: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+00007960: 2020 2020 2020 2070 7265 765f 7461 6220         prev_tab 
+00007970: 3d20 7365 6c66 2e74 6162 5f70 7265 762e  = self.tab_prev.
+00007980: 6765 7428 7365 6c66 2e72 6563 6569 7665  get(self.receive
+00007990: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000079a0: 2020 2020 2020 7072 6576 5f74 6162 2e73        prev_tab.s
+000079b0: 6574 466f 6375 7328 290a 2020 2020 2020  etFocus().      
+000079c0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000079d0: 6576 5f74 6162 2e64 6573 656c 6563 7428  ev_tab.deselect(
+000079e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000079f0: 2020 2020 2020 7072 6576 5f74 6162 2e65        prev_tab.e
+00007a00: 6e64 2846 616c 7365 290a 2020 2020 2020  nd(False).      
+00007a10: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a30: 2020 2020 6e65 7874 5f74 6162 203d 2073      next_tab = s
+00007a40: 656c 662e 7461 625f 6e65 7874 2e67 6574  elf.tab_next.get
+00007a50: 2873 656c 662e 7265 6365 6976 6529 0a20  (self.receive). 
+00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a70: 2020 206e 6578 745f 7461 622e 7365 7446     next_tab.setF
+00007a80: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
+00007a90: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00007aa0: 7461 622e 6465 7365 6c65 6374 2829 0a20  tab.deselect(). 
+00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ac0: 2020 206e 6578 745f 7461 622e 656e 6428     next_tab.end(
+00007ad0: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+00007ae0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00007af0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00007b00: 662e 6f74 6865 725f 312e 6861 7346 6f63  f.other_1.hasFoc
+00007b10: 7573 2829 3a0a 2020 2020 2020 2020 2020  us():.          
+00007b20: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00007b30: 7567 2822 4672 6f6d 206f 7468 6572 5f31  ug("From other_1
+00007b40: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00007b50: 2020 2069 6620 6d6f 6469 6669 6572 203d     if modifier =
+00007b60: 3d20 5174 2e53 6869 6674 4d6f 6469 6669  = Qt.ShiftModifi
+00007b70: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+00007b80: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
+00007b90: 203d 2073 656c 662e 7461 625f 7072 6576   = self.tab_prev
+00007ba0: 2e67 6574 2873 656c 662e 6f74 6865 725f  .get(self.other_
+00007bb0: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
+00007bc0: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
+00007bd0: 7365 7446 6f63 7573 2829 0a20 2020 2020  setFocus().     
+00007be0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00007bf0: 7265 765f 7461 622e 6465 7365 6c65 6374  rev_tab.deselect
+00007c00: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00007c10: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
+00007c20: 656e 6428 4661 6c73 6529 0a20 2020 2020  end(False).     
+00007c30: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00007c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007c50: 2020 2020 206e 6578 745f 7461 6220 3d20       next_tab = 
+00007c60: 7365 6c66 2e74 6162 5f6e 6578 742e 6765  self.tab_next.ge
+00007c70: 7428 7365 6c66 2e6f 7468 6572 5f31 290a  t(self.other_1).
+00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c90: 2020 2020 6e65 7874 5f74 6162 2e73 6574      next_tab.set
+00007ca0: 466f 6375 7328 290a 2020 2020 2020 2020  Focus().        
+00007cb0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00007cc0: 5f74 6162 2e64 6573 656c 6563 7428 290a  _tab.deselect().
+00007cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ce0: 2020 2020 6e65 7874 5f74 6162 2e65 6e64      next_tab.end
+00007cf0: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
+00007d00: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00007d10: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00007d20: 6c66 2e6f 7468 6572 5f32 2e68 6173 466f  lf.other_2.hasFo
+00007d30: 6375 7328 293a 0a20 2020 2020 2020 2020  cus():.         
+00007d40: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00007d50: 6275 6728 2246 726f 6d20 6f74 6865 725f  bug("From other_
+00007d60: 3222 290a 2020 2020 2020 2020 2020 2020  2").            
+00007d70: 2020 2020 6966 206d 6f64 6966 6965 7220      if modifier 
+00007d80: 3d3d 2051 742e 5368 6966 744d 6f64 6966  == Qt.ShiftModif
+00007d90: 6965 723a 0a20 2020 2020 2020 2020 2020  ier:.           
+00007da0: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
+00007db0: 6220 3d20 7365 6c66 2e74 6162 5f70 7265  b = self.tab_pre
+00007dc0: 762e 6765 7428 7365 6c66 2e6f 7468 6572  v.get(self.other
+00007dd0: 5f32 290a 2020 2020 2020 2020 2020 2020  _2).            
+00007de0: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
+00007df0: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
+00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e10: 7072 6576 5f74 6162 2e64 6573 656c 6563  prev_tab.deselec
+00007e20: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00007e30: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
+00007e40: 2e65 6e64 2846 616c 7365 290a 2020 2020  .end(False).    
+00007e50: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00007e60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007e70: 2020 2020 2020 6e65 7874 5f74 6162 203d        next_tab =
+00007e80: 2073 656c 662e 7461 625f 6e65 7874 2e67   self.tab_next.g
+00007e90: 6574 2873 656c 662e 6f74 6865 725f 3229  et(self.other_2)
+00007ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007eb0: 2020 2020 206e 6578 745f 7461 622e 7365       next_tab.se
+00007ec0: 7446 6f63 7573 2829 0a20 2020 2020 2020  tFocus().       
+00007ed0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+00007ee0: 745f 7461 622e 6465 7365 6c65 6374 2829  t_tab.deselect()
+00007ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007f00: 2020 2020 206e 6578 745f 7461 622e 656e       next_tab.en
+00007f10: 6428 4661 6c73 6529 0a20 2020 2020 2020  d(False).       
+00007f20: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00007f30: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00007f40: 656c 662e 6361 6c6c 7369 676e 2e68 6173  elf.callsign.has
+00007f50: 466f 6375 7328 293a 0a20 2020 2020 2020  Focus():.       
+00007f60: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00007f70: 6465 6275 6728 2246 726f 6d20 6361 6c6c  debug("From call
+00007f80: 7369 676e 2229 0a20 2020 2020 2020 2020  sign").         
+00007f90: 2020 2020 2020 2069 6620 6d6f 6469 6669         if modifi
+00007fa0: 6572 203d 3d20 5174 2e53 6869 6674 4d6f  er == Qt.ShiftMo
+00007fb0: 6469 6669 6572 3a0a 2020 2020 2020 2020  difier:.        
+00007fc0: 2020 2020 2020 2020 2020 2020 7072 6576              prev
+00007fd0: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
+00007fe0: 7072 6576 2e67 6574 2873 656c 662e 6361  prev.get(self.ca
+00007ff0: 6c6c 7369 676e 290a 2020 2020 2020 2020  llsign).        
+00008000: 2020 2020 2020 2020 2020 2020 7072 6576              prev
+00008010: 5f74 6162 2e73 6574 466f 6375 7328 290a  _tab.setFocus().
+00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008030: 2020 2020 7072 6576 5f74 6162 2e64 6573      prev_tab.des
+00008040: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
+00008050: 2020 2020 2020 2020 2020 2020 7072 6576              prev
+00008060: 5f74 6162 2e65 6e64 2846 616c 7365 290a  _tab.end(False).
+00008070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008080: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00008090: 2020 2020 2020 2020 2020 7465 7874 203d            text =
+000080a0: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
+000080b0: 6578 7428 290a 2020 2020 2020 2020 2020  ext().          
+000080c0: 2020 2020 2020 2020 2020 7465 7874 203d            text =
+000080d0: 2074 6578 742e 7570 7065 7228 290a 2020   text.upper().  
+000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080f0: 2020 5f74 6865 7468 7265 6164 203d 2074    _thethread = t
+00008100: 6872 6561 6469 6e67 2e54 6872 6561 6428  hreading.Thread(
+00008110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008120: 2020 2020 2020 2020 2074 6172 6765 743d           target=
+00008130: 7365 6c66 2e63 6865 636b 5f63 616c 6c73  self.check_calls
+00008140: 6967 6e32 2c0a 2020 2020 2020 2020 2020  ign2,.          
+00008150: 2020 2020 2020 2020 2020 2020 2020 6172                ar
+00008160: 6773 3d28 7465 7874 2c29 2c0a 2020 2020  gs=(text,),.    
+00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008180: 2020 2020 6461 656d 6f6e 3d54 7275 652c      daemon=True,
+00008190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000081a0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000081b0: 2020 2020 2020 2020 2020 205f 7468 6574             _thet
+000081c0: 6872 6561 642e 7374 6172 7428 290a 2020  hread.start().  
+000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081e0: 2020 6e65 7874 5f74 6162 203d 2073 656c    next_tab = sel
+000081f0: 662e 7461 625f 6e65 7874 2e67 6574 2873  f.tab_next.get(s
+00008200: 656c 662e 6361 6c6c 7369 676e 290a 2020  elf.callsign).  
+00008210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008220: 2020 6e65 7874 5f74 6162 2e73 6574 466f    next_tab.setFo
+00008230: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
+00008240: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
+00008250: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
+00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008270: 2020 6e65 7874 5f74 6162 2e65 6e64 2846    next_tab.end(F
+00008280: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+00008290: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+000082a0: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
+000082b0: 7928 2920 3d3d 2051 742e 4b65 795f 4631  y() == Qt.Key_F1
+000082c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000082d0: 6c66 2e73 656e 6466 3128 290a 2020 2020  lf.sendf1().    
+000082e0: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
+000082f0: 2829 203d 3d20 5174 2e4b 6579 5f46 323a  () == Qt.Key_F2:
+00008300: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00008310: 662e 7365 6e64 6632 2829 0a20 2020 2020  f.sendf2().     
+00008320: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
+00008330: 2920 3d3d 2051 742e 4b65 795f 4633 3a0a  ) == Qt.Key_F3:.
+00008340: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008350: 2e73 656e 6466 3328 290a 2020 2020 2020  .sendf3().      
+00008360: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
+00008370: 203d 3d20 5174 2e4b 6579 5f46 343a 0a20   == Qt.Key_F4:. 
+00008380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008390: 7365 6e64 6634 2829 0a20 2020 2020 2020  sendf4().       
+000083a0: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
+000083b0: 3d3d 2051 742e 4b65 795f 4635 3a0a 2020  == Qt.Key_F5:.  
+000083c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000083d0: 656e 6466 3528 290a 2020 2020 2020 2020  endf5().        
+000083e0: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
+000083f0: 3d20 5174 2e4b 6579 5f46 363a 0a20 2020  = Qt.Key_F6:.   
+00008400: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00008410: 6e64 6636 2829 0a20 2020 2020 2020 2069  ndf6().        i
+00008420: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+00008430: 2051 742e 4b65 795f 4637 3a0a 2020 2020   Qt.Key_F7:.    
+00008440: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
+00008450: 6466 3728 290a 2020 2020 2020 2020 6966  df7().        if
+00008460: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
+00008470: 5174 2e4b 6579 5f46 383a 0a20 2020 2020  Qt.Key_F8:.     
+00008480: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
+00008490: 6638 2829 0a20 2020 2020 2020 2069 6620  f8().        if 
+000084a0: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
+000084b0: 742e 4b65 795f 4639 3a0a 2020 2020 2020  t.Key_F9:.      
+000084c0: 2020 2020 2020 7365 6c66 2e73 656e 6466        self.sendf
+000084d0: 3928 290a 2020 2020 2020 2020 6966 2065  9().        if e
+000084e0: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
+000084f0: 2e4b 6579 5f46 3130 3a0a 2020 2020 2020  .Key_F10:.      
+00008500: 2020 2020 2020 7365 6c66 2e73 656e 6466        self.sendf
+00008510: 3130 2829 0a20 2020 2020 2020 2069 6620  10().        if 
+00008520: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
+00008530: 742e 4b65 795f 4631 313a 0a20 2020 2020  t.Key_F11:.     
+00008540: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
+00008550: 6631 3128 290a 2020 2020 2020 2020 6966  f11().        if
+00008560: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
+00008570: 5174 2e4b 6579 5f46 3132 3a0a 2020 2020  Qt.Key_F12:.    
+00008580: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
+00008590: 6466 3132 2829 0a0a 2020 2020 6465 6620  df12()..    def 
+000085a0: 7365 745f 7769 6e64 6f77 5f74 6974 6c65  set_window_title
+000085b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000085c0: 2222 2253 6574 2077 696e 646f 7720 7469  """Set window ti
+000085d0: 746c 6522 2222 0a20 2020 2020 2020 2076  tle""".        v
+000085e0: 666f 6120 3d20 7365 6c66 2e72 6164 696f  foa = self.radio
+000085f0: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
+00008600: 222c 2022 2229 0a20 2020 2020 2020 2069  ", "").        i
+00008610: 6620 7666 6f61 3a0a 2020 2020 2020 2020  f vfoa:.        
+00008620: 2020 2020 7666 6f61 203d 2069 6e74 2876      vfoa = int(v
+00008630: 666f 6129 202f 2031 3030 300a 2020 2020  foa) / 1000.    
+00008640: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008650: 2020 2020 2020 7666 6f61 203d 2030 2e30        vfoa = 0.0
+00008660: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+00008670: 5f6e 616d 6520 3d20 2222 0a20 2020 2020  _name = "".     
+00008680: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
+00008690: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+000086a0: 636f 6e74 6573 745f 6e61 6d65 203d 2073  contest_name = s
+000086b0: 656c 662e 636f 6e74 6573 742e 6e61 6d65  elf.contest.name
+000086c0: 0a20 2020 2020 2020 206c 696e 6520 3d20  .        line = 
+000086d0: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
+000086e0: 7666 6f61 3a7b 726f 756e 6428 7666 6f61  vfoa:{round(vfoa
+000086f0: 2c32 297d 2022 0a20 2020 2020 2020 2020  ,2)} ".         
+00008700: 2020 2066 226d 6f64 653a 7b73 656c 662e     f"mode:{self.
+00008710: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+00008720: 276d 6f64 6527 2c20 2727 297d 2022 0a20  'mode', '')} ". 
+00008730: 2020 2020 2020 2020 2020 2066 224f 503a             f"OP:
+00008740: 7b73 656c 662e 6375 7272 656e 745f 6f70  {self.current_op
+00008750: 7d20 7b63 6f6e 7465 7374 5f6e 616d 657d  } {contest_name}
+00008760: 2022 0a20 2020 2020 2020 2020 2020 2066   ".            f
+00008770: 222d 204e 6f74 314d 4d20 767b 5f5f 7665  "- Not1MM v{__ve
+00008780: 7273 696f 6e5f 5f7d 220a 2020 2020 2020  rsion__}".      
+00008790: 2020 290a 2020 2020 2020 2020 6c6f 6767    ).        logg
+000087a0: 6572 2e64 6562 7567 2822 2573 222c 206c  er.debug("%s", l
+000087b0: 696e 6529 0a20 2020 2020 2020 2073 656c  ine).        sel
+000087c0: 662e 7365 7457 696e 646f 7754 6974 6c65  f.setWindowTitle
+000087d0: 286c 696e 6529 0a0a 2020 2020 6465 6620  (line)..    def 
+000087e0: 636c 6561 7269 6e70 7574 7328 7365 6c66  clearinputs(self
+000087f0: 293a 0a20 2020 2020 2020 2022 2222 436c  ):.        """Cl
+00008800: 6561 7273 2074 6865 2074 6578 7420 696e  ears the text in
+00008810: 7075 7420 6669 656c 6473 2061 6e64 2073  put fields and s
+00008820: 6574 7320 666f 6375 7320 746f 2063 616c  ets focus to cal
+00008830: 6c73 6967 6e20 6669 656c 642e 2222 220a  lsign field.""".
+00008840: 2020 2020 2020 2020 7365 6c66 2e64 7570          self.dup
+00008850: 655f 696e 6469 6361 746f 722e 6869 6465  e_indicator.hide
+00008860: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00008870: 636f 6e74 6163 7420 3d20 7365 6c66 2e64  contact = self.d
+00008880: 6174 6162 6173 652e 656d 7074 795f 636f  atabase.empty_co
+00008890: 6e74 6163 740a 2020 2020 2020 2020 7365  ntact.        se
+000088a0: 6c66 2e68 6561 6469 6e67 5f64 6973 7461  lf.heading_dista
+000088b0: 6e63 652e 7365 7454 6578 7428 2222 290a  nce.setText("").
+000088c0: 2020 2020 2020 2020 7365 6c66 2e64 785f          self.dx_
+000088d0: 656e 7469 7479 2e73 6574 5465 7874 2822  entity.setText("
+000088e0: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
+000088f0: 6c66 2e63 6f6e 7465 7374 3a0a 2020 2020  lf.contest:.    
+00008900: 2020 2020 2020 2020 6d75 6c74 7320 3d20          mults = 
+00008910: 7365 6c66 2e63 6f6e 7465 7374 2e73 686f  self.contest.sho
+00008920: 775f 6d75 6c74 7328 7365 6c66 290a 2020  w_mults(self).  
+00008930: 2020 2020 2020 2020 2020 7173 6f73 203d            qsos =
+00008940: 2073 656c 662e 636f 6e74 6573 742e 7368   self.contest.sh
+00008950: 6f77 5f71 736f 2873 656c 6629 0a20 2020  ow_qso(self).   
+00008960: 2020 2020 2020 2020 206d 756c 7473 7472           multstr
+00008970: 696e 6720 3d20 6622 7b71 736f 737d 2f7b  ing = f"{qsos}/{
+00008980: 6d75 6c74 737d 220a 2020 2020 2020 2020  mults}".        
+00008990: 2020 2020 7365 6c66 2e6d 756c 7473 2e73      self.mults.s
+000089a0: 6574 5465 7874 286d 756c 7473 7472 696e  etText(multstrin
+000089b0: 6729 0a20 2020 2020 2020 2020 2020 2073  g).            s
+000089c0: 636f 7265 203d 2073 656c 662e 636f 6e74  core = self.cont
+000089d0: 6573 742e 6361 6c63 5f73 636f 7265 2873  est.calc_score(s
+000089e0: 656c 6629 0a20 2020 2020 2020 2020 2020  elf).           
+000089f0: 2073 656c 662e 7363 6f72 652e 7365 7454   self.score.setT
+00008a00: 6578 7428 7374 7228 7363 6f72 6529 290a  ext(str(score)).
+00008a10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008a20: 2e63 6f6e 7465 7374 2e72 6573 6574 5f6c  .contest.reset_l
+00008a30: 6162 656c 2873 656c 6629 0a20 2020 2020  abel(self).     
+00008a40: 2020 2073 656c 662e 6361 6c6c 7369 676e     self.callsign
+00008a50: 2e63 6c65 6172 2829 0a20 2020 2020 2020  .clear().       
+00008a60: 2069 6620 7365 6c66 2e63 7572 7265 6e74   if self.current
+00008a70: 5f6d 6f64 6520 3d3d 2022 4357 223a 0a20  _mode == "CW":. 
+00008a80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008a90: 7365 6e74 2e73 6574 5465 7874 2822 3539  sent.setText("59
+00008aa0: 3922 290a 2020 2020 2020 2020 2020 2020  9").            
+00008ab0: 7365 6c66 2e72 6563 6569 7665 2e73 6574  self.receive.set
+00008ac0: 5465 7874 2822 3539 3922 290a 2020 2020  Text("599").    
+00008ad0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008ae0: 2020 2020 2020 7365 6c66 2e73 656e 742e        self.sent.
+00008af0: 7365 7454 6578 7428 2235 3922 290a 2020  setText("59").  
+00008b00: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00008b10: 6563 6569 7665 2e73 6574 5465 7874 2822  eceive.setText("
+00008b20: 3539 2229 0a20 2020 2020 2020 2073 656c  59").        sel
+00008b30: 662e 6f74 6865 725f 312e 636c 6561 7228  f.other_1.clear(
+00008b40: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
+00008b50: 7468 6572 5f32 2e63 6c65 6172 2829 0a20  ther_2.clear(). 
+00008b60: 2020 2020 2020 2073 656c 662e 6361 6c6c         self.call
+00008b70: 7369 676e 2e73 6574 466f 6375 7328 290a  sign.setFocus().
+00008b80: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
+00008b90: 0a20 2020 2020 2020 2063 6d64 5b22 636d  .        cmd["cm
+00008ba0: 6422 5d20 3d20 2243 414c 4c43 4841 4e47  d"] = "CALLCHANG
+00008bb0: 4544 220a 2020 2020 2020 2020 636d 645b  ED".        cmd[
+00008bc0: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
+00008bd0: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
+00008be0: 2020 2020 2063 6d64 5b22 6361 6c6c 225d       cmd["call"]
+00008bf0: 203d 2022 220a 2020 2020 2020 2020 7365   = "".        se
+00008c00: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
+00008c10: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
+00008c20: 736f 6e28 636d 6429 0a0a 2020 2020 6465  son(cmd)..    de
+00008c30: 6620 7361 7665 5f63 6f6e 7461 6374 2873  f save_contact(s
+00008c40: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00008c50: 2253 6176 6520 746f 2064 6222 2222 0a20  "Save to db""". 
+00008c60: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00008c70: 6275 6728 2273 6176 696e 6720 636f 6e74  bug("saving cont
+00008c80: 6163 7422 290a 2020 2020 2020 2020 6966  act").        if
+00008c90: 206c 656e 2873 656c 662e 6361 6c6c 7369   len(self.callsi
+00008ca0: 676e 2e74 6578 7428 2929 203c 2033 3a0a  gn.text()) < 3:.
+00008cb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00008cc0: 726e 0a20 2020 2020 2020 2069 6620 6e6f  rn.        if no
+00008cd0: 7420 616e 7928 6368 6172 2e69 7364 6967  t any(char.isdig
+00008ce0: 6974 2829 2066 6f72 2063 6861 7220 696e  it() for char in
+00008cf0: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
+00008d00: 6578 7428 2929 3a0a 2020 2020 2020 2020  ext()):.        
+00008d10: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00008d20: 2020 2069 6620 6e6f 7420 616e 7928 6368     if not any(ch
+00008d30: 6172 2e69 7361 6c70 6861 2829 2066 6f72  ar.isalpha() for
+00008d40: 2063 6861 7220 696e 2073 656c 662e 6361   char in self.ca
+00008d50: 6c6c 7369 676e 2e74 6578 7428 2929 3a0a  llsign.text()):.
+00008d60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00008d70: 726e 0a0a 2020 2020 2020 2020 7365 6c66  rn..        self
+00008d80: 2e63 6f6e 7461 6374 5b22 5453 225d 203d  .contact["TS"] =
+00008d90: 2064 6174 6574 696d 652e 7574 636e 6f77   datetime.utcnow
+00008da0: 2829 2e69 736f 666f 726d 6174 2822 2022  ().isoformat(" "
+00008db0: 295b 3a31 395d 0a20 2020 2020 2020 2073  )[:19].        s
+00008dc0: 656c 662e 636f 6e74 6163 745b 2243 616c  elf.contact["Cal
+00008dd0: 6c22 5d20 3d20 7365 6c66 2e63 616c 6c73  l"] = self.calls
+00008de0: 6967 6e2e 7465 7874 2829 0a20 2020 2020  ign.text().     
+00008df0: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
+00008e00: 2246 7265 7122 5d20 3d20 726f 756e 6428  "Freq"] = round(
+00008e10: 666c 6f61 7428 7365 6c66 2e72 6164 696f  float(self.radio
+00008e20: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
+00008e30: 222c 2030 2e30 2929 202f 2031 3030 302c  ", 0.0)) / 1000,
+00008e40: 2032 290a 2020 2020 2020 2020 7365 6c66   2).        self
+00008e50: 2e63 6f6e 7461 6374 5b22 5153 5846 7265  .contact["QSXFre
+00008e60: 7122 5d20 3d20 726f 756e 6428 0a20 2020  q"] = round(.   
+00008e70: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
+00008e80: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+00008e90: 6765 7428 2276 666f 6122 2c20 302e 3029  get("vfoa", 0.0)
+00008ea0: 2920 2f20 3130 3030 2c20 320a 2020 2020  ) / 1000, 2.    
+00008eb0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+00008ec0: 6c66 2e63 6f6e 7461 6374 5b22 4d6f 6465  lf.contact["Mode
+00008ed0: 225d 203d 2073 656c 662e 7261 6469 6f5f  "] = self.radio_
+00008ee0: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
+00008ef0: 2c20 2222 290a 2020 2020 2020 2020 7365  , "").        se
+00008f00: 6c66 2e63 6f6e 7461 6374 5b22 436f 6e74  lf.contact["Cont
+00008f10: 6573 744e 616d 6522 5d20 3d20 7365 6c66  estName"] = self
+00008f20: 2e63 6f6e 7465 7374 2e63 6162 7269 6c6c  .contest.cabrill
+00008f30: 6f5f 6e61 6d65 0a20 2020 2020 2020 2073  o_name.        s
+00008f40: 656c 662e 636f 6e74 6163 745b 2243 6f6e  elf.contact["Con
+00008f50: 7465 7374 4e52 225d 203d 2073 656c 662e  testNR"] = self.
+00008f60: 7072 6566 2e67 6574 2822 636f 6e74 6573  pref.get("contes
+00008f70: 7422 2c20 2230 2229 0a20 2020 2020 2020  t", "0").       
+00008f80: 2073 656c 662e 636f 6e74 6163 745b 2253   self.contact["S
+00008f90: 7461 7469 6f6e 5072 6566 6978 225d 203d  tationPrefix"] =
+00008fa0: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
+00008fb0: 7428 2243 616c 6c22 2c20 2222 290a 2020  t("Call", "").  
+00008fc0: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
+00008fd0: 6374 5b22 5750 5850 7265 6669 7822 5d20  ct["WPXPrefix"] 
+00008fe0: 3d20 6361 6c63 756c 6174 655f 7770 785f  = calculate_wpx_
+00008ff0: 7072 6566 6978 2873 656c 662e 6361 6c6c  prefix(self.call
+00009000: 7369 676e 2e74 6578 7428 2929 0a20 2020  sign.text()).   
+00009010: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+00009020: 745b 2249 7352 756e 5153 4f22 5d20 3d20  t["IsRunQSO"] = 
+00009030: 7365 6c66 2e72 6164 696f 4275 7474 6f6e  self.radioButton
+00009040: 5f72 756e 2e69 7343 6865 636b 6564 2829  _run.isChecked()
+00009050: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00009060: 6e74 6163 745b 224f 7065 7261 746f 7222  ntact["Operator"
+00009070: 5d20 3d20 7365 6c66 2e63 7572 7265 6e74  ] = self.current
+00009080: 5f6f 700a 2020 2020 2020 2020 7365 6c66  _op.        self
+00009090: 2e63 6f6e 7461 6374 5b22 4e65 7442 696f  .contact["NetBio
+000090a0: 734e 616d 6522 5d20 3d20 736f 636b 6574  sName"] = socket
+000090b0: 2e67 6574 686f 7374 6e61 6d65 2829 0a20  .gethostname(). 
+000090c0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+000090d0: 6163 745b 2249 734f 7269 6769 6e61 6c22  act["IsOriginal"
+000090e0: 5d20 3d20 310a 2020 2020 2020 2020 7365  ] = 1.        se
+000090f0: 6c66 2e63 6f6e 7461 6374 5b22 4944 225d  lf.contact["ID"]
+00009100: 203d 2075 7569 642e 7575 6964 3428 292e   = uuid.uuid4().
+00009110: 6865 780a 2020 2020 2020 2020 7365 6c66  hex.        self
+00009120: 2e63 6f6e 7465 7374 2e73 6574 5f63 6f6e  .contest.set_con
+00009130: 7461 6374 5f76 6172 7328 7365 6c66 290a  tact_vars(self).
+00009140: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00009150: 7461 6374 5b22 506f 696e 7473 225d 203d  tact["Points"] =
+00009160: 2073 656c 662e 636f 6e74 6573 742e 706f   self.contest.po
+00009170: 696e 7473 2873 656c 6629 0a20 2020 2020  ints(self).     
+00009180: 2020 2064 6562 7567 5f6f 7574 7075 7420     debug_output 
+00009190: 3d20 6622 7b73 656c 662e 636f 6e74 6163  = f"{self.contac
+000091a0: 747d 220a 2020 2020 2020 2020 6c6f 6767  t}".        logg
+000091b0: 6572 2e64 6562 7567 2864 6562 7567 5f6f  er.debug(debug_o
+000091c0: 7574 7075 7429 0a20 2020 2020 2020 2073  utput).        s
+000091d0: 656c 662e 6461 7461 6261 7365 2e6c 6f67  elf.database.log
+000091e0: 5f63 6f6e 7461 6374 2873 656c 662e 636f  _contact(self.co
+000091f0: 6e74 6163 7429 0a20 2020 2020 2020 2073  ntact).        s
+00009200: 656c 662e 6e31 6d6d 2e73 656e 645f 636f  elf.n1mm.send_co
+00009210: 6e74 6163 745f 696e 666f 2829 0a20 2020  ntact_info().   
+00009220: 2020 2020 2073 656c 662e 636c 6561 7269       self.cleari
+00009230: 6e70 7574 7328 290a 2020 2020 2020 2020  nputs().        
+00009240: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
+00009250: 2063 6d64 5b22 636d 6422 5d20 3d20 2255   cmd["cmd"] = "U
+00009260: 5044 4154 454c 4f47 220a 2020 2020 2020  PDATELOG".      
+00009270: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
+00009280: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
+00009290: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+000092a0: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+000092b0: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
+000092c0: 2863 6d64 290a 2020 2020 2020 2020 2320  (cmd).        # 
+000092d0: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
+000092e0: 6e74 6573 744e 616d 6522 5d20 3d20 7365  ntestName"] = se
+000092f0: 6c66 2e63 6f6e 7465 7374 2e6e 616d 650a  lf.contest.name.
+00009300: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
+00009310: 6f6e 7461 6374 5b22 534e 5422 5d20 3d20  ontact["SNT"] = 
+00009320: 7365 6c66 2e73 656e 742e 7465 7874 2829  self.sent.text()
+00009330: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+00009340: 636f 6e74 6163 745b 2252 4356 225d 203d  contact["RCV"] =
+00009350: 2073 656c 662e 7265 6365 6976 652e 7465   self.receive.te
+00009360: 7874 2829 0a20 2020 2020 2020 2023 2073  xt().        # s
+00009370: 656c 662e 636f 6e74 6163 745b 2243 6f75  elf.contact["Cou
+00009380: 6e74 7279 5072 6566 6978 225d 0a20 2020  ntryPrefix"].   
+00009390: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+000093a0: 6163 745b 2253 7461 7469 6f6e 5072 6566  act["StationPref
+000093b0: 6978 225d 203d 2073 656c 662e 7072 6566  ix"] = self.pref
+000093c0: 2e67 6574 2822 6361 6c6c 7369 676e 222c  .get("callsign",
+000093d0: 2022 2229 0a20 2020 2020 2020 2023 2073   "").        # s
+000093e0: 656c 662e 636f 6e74 6163 745b 2251 5448  elf.contact["QTH
+000093f0: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
+00009400: 662e 636f 6e74 6163 745b 224e 616d 6522  f.contact["Name"
+00009410: 5d20 3d20 7365 6c66 2e6f 7468 6572 5f31  ] = self.other_1
+00009420: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+00009430: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+00009440: 436f 6d6d 656e 7422 5d20 3d20 7365 6c66  Comment"] = self
+00009450: 2e6f 7468 6572 5f32 2e74 6578 7428 290a  .other_2.text().
+00009460: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
+00009470: 6f6e 7461 6374 5b22 4e52 225d 0a20 2020  ontact["NR"].   
+00009480: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+00009490: 6163 745b 2253 6563 7422 5d0a 2020 2020  act["Sect"].    
+000094a0: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+000094b0: 6374 5b22 5072 6563 225d 0a20 2020 2020  ct["Prec"].     
+000094c0: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+000094d0: 745b 2243 4b22 5d0a 2020 2020 2020 2020  t["CK"].        
+000094e0: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+000094f0: 5a4e 225d 0a20 2020 2020 2020 2023 2073  ZN"].        # s
+00009500: 656c 662e 636f 6e74 6163 745b 2253 656e  elf.contact["Sen
+00009510: 744e 7222 5d0a 2020 2020 2020 2020 2320  tNr"].        # 
+00009520: 7365 6c66 2e63 6f6e 7461 6374 5b22 506f  self.contact["Po
+00009530: 696e 7473 225d 0a20 2020 2020 2020 2023  ints"].        #
+00009540: 2073 656c 662e 636f 6e74 6163 745b 2249   self.contact["I
+00009550: 734d 756c 7469 706c 6965 7231 225d 0a20  sMultiplier1"]. 
+00009560: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
+00009570: 6e74 6163 745b 2249 734d 756c 7469 706c  ntact["IsMultipl
+00009580: 6965 7232 225d 0a20 2020 2020 2020 2023  ier2"].        #
+00009590: 2073 656c 662e 636f 6e74 6163 745b 2250   self.contact["P
+000095a0: 6f77 6572 225d 0a20 2020 2020 2020 2023  ower"].        #
+000095b0: 2073 656c 662e 636f 6e74 6163 745b 2242   self.contact["B
+000095c0: 616e 6422 5d0a 2020 2020 2020 2020 2320  and"].        # 
+000095d0: 7365 6c66 2e63 6f6e 7461 6374 5b22 5750  self.contact["WP
+000095e0: 5850 7265 6669 7822 5d20 3d20 6361 6c63  XPrefix"] = calc
+000095f0: 756c 6174 655f 7770 785f 7072 6566 6978  ulate_wpx_prefix
+00009600: 2873 656c 662e 6361 6c6c 7369 676e 2e74  (self.callsign.t
+00009610: 6578 7428 2929 0a20 2020 2020 2020 2023  ext()).        #
+00009620: 2073 656c 662e 636f 6e74 6163 745b 2245   self.contact["E
+00009630: 7863 6861 6e67 6531 225d 0a20 2020 2020  xchange1"].     
+00009640: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+00009650: 745b 2252 6164 696f 4e52 225d 0a20 2020  t["RadioNR"].   
+00009660: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+00009670: 6163 745b 2269 734d 756c 7469 706c 6965  act["isMultiplie
+00009680: 7233 225d 0a20 2020 2020 2020 2023 2073  r3"].        # s
+00009690: 656c 662e 636f 6e74 6163 745b 224d 6973  elf.contact["Mis
+000096a0: 6354 6578 7422 5d0a 2020 2020 2020 2020  cText"].        
+000096b0: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+000096c0: 436f 6e74 6163 7454 7970 6522 5d0a 2020  ContactType"].  
+000096d0: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
+000096e0: 7461 6374 5b22 5275 6e31 5275 6e32 225d  tact["Run1Run2"]
+000096f0: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+00009700: 636f 6e74 6163 745b 2247 7269 6453 7175  contact["GridSqu
+00009710: 6172 6522 5d0a 2020 2020 2020 2020 2320  are"].        # 
+00009720: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
+00009730: 6e74 696e 656e 7422 5d0a 2020 2020 2020  ntinent"].      
+00009740: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
+00009750: 5b22 526f 7665 724c 6f63 6174 696f 6e22  ["RoverLocation"
+00009760: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
+00009770: 2e63 6f6e 7461 6374 5b22 5261 6469 6f49  .contact["RadioI
+00009780: 6e74 6572 6661 6365 6422 5d0a 2020 2020  nterfaced"].    
+00009790: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+000097a0: 6374 5b22 4e65 7477 6f72 6b65 6443 6f6d  ct["NetworkedCom
+000097b0: 704e 7222 5d0a 2020 2020 2020 2020 2320  pNr"].        # 
+000097c0: 7365 6c66 2e63 6f6e 7461 6374 5b22 434c  self.contact["CL
+000097d0: 4149 4d45 4451 534f 225d 0a0a 2020 2020  AIMEDQSO"]..    
+000097e0: 6465 6620 6e65 775f 636f 6e74 6573 745f  def new_contest_
+000097f0: 6469 616c 6f67 2873 656c 6629 3a0a 2020  dialog(self):.  
+00009800: 2020 2020 2020 2222 2253 686f 7720 6e65        """Show ne
+00009810: 7720 636f 6e74 6573 7420 6469 616c 6f67  w contest dialog
+00009820: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
+00009830: 6572 2e64 6562 7567 2822 4e65 7720 636f  er.debug("New co
+00009840: 6e74 6573 7420 4469 616c 6f67 2229 0a20  ntest Dialog"). 
+00009850: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00009860: 6573 745f 6469 616c 6f67 203d 204e 6577  est_dialog = New
+00009870: 436f 6e74 6573 7428 574f 524b 494e 475f  Contest(WORKING_
+00009880: 5041 5448 290a 2020 2020 2020 2020 7365  PATH).        se
+00009890: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+000098a0: 672e 6163 6365 7074 6564 2e63 6f6e 6e65  g.accepted.conne
+000098b0: 6374 2873 656c 662e 7361 7665 5f63 6f6e  ct(self.save_con
+000098c0: 7465 7374 290a 2020 2020 2020 2020 6966  test).        if
+000098d0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+000098e0: 6461 726b 5f6d 6f64 6522 293a 0a20 2020  dark_mode"):.   
+000098f0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00009900: 6e74 6573 745f 6469 616c 6f67 2e73 6574  ntest_dialog.set
+00009910: 5374 796c 6553 6865 6574 2844 4152 4b5f  StyleSheet(DARK_
+00009920: 5354 594c 4553 4845 4554 290a 2020 2020  STYLESHEET).    
+00009930: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+00009940: 5f64 6961 6c6f 672e 6461 7465 5469 6d65  _dialog.dateTime
+00009950: 4564 6974 2e73 6574 4461 7465 2851 7443  Edit.setDate(QtC
+00009960: 6f72 652e 5144 6174 652e 6375 7272 656e  ore.QDate.curren
+00009970: 7444 6174 6528 2929 0a20 2020 2020 2020  tDate()).       
+00009980: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00009990: 616c 6f67 2e64 6174 6554 696d 6545 6469  alog.dateTimeEdi
+000099a0: 742e 7365 7443 616c 656e 6461 7250 6f70  t.setCalendarPop
+000099b0: 7570 2854 7275 6529 0a20 2020 2020 2020  up(True).       
+000099c0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+000099d0: 616c 6f67 2e64 6174 6554 696d 6545 6469  alog.dateTimeEdi
+000099e0: 742e 7365 7454 696d 6528 5174 436f 7265  t.setTime(QtCore
+000099f0: 2e51 5469 6d65 2830 2c20 3029 290a 2020  .QTime(0, 0)).  
+00009a00: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+00009a10: 7374 5f64 6961 6c6f 672e 706f 7765 722e  st_dialog.power.
+00009a20: 7365 7443 7572 7265 6e74 5465 7874 2822  setCurrentText("
+00009a30: 4c4f 5722 290a 2020 2020 2020 2020 7365  LOW").        se
+00009a40: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00009a50: 672e 7374 6174 696f 6e2e 7365 7443 7572  g.station.setCur
+00009a60: 7265 6e74 5465 7874 2822 4649 5845 4422  rentText("FIXED"
+00009a70: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00009a80: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f70  ontest_dialog.op
+00009a90: 656e 2829 0a0a 2020 2020 6465 6620 7361  en()..    def sa
+00009aa0: 7665 5f63 6f6e 7465 7374 2873 656c 6629  ve_contest(self)
+00009ab0: 3a0a 2020 2020 2020 2020 2222 2253 6176  :.        """Sav
+00009ac0: 6520 436f 6e74 6573 7422 2222 0a20 2020  e Contest""".   
+00009ad0: 2020 2020 206e 6578 745f 6e75 6d62 6572       next_number
+00009ae0: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
+00009af0: 2e67 6574 5f6e 6578 745f 636f 6e74 6573  .get_next_contes
+00009b00: 745f 6e72 2829 0a20 2020 2020 2020 2063  t_nr().        c
+00009b10: 6f6e 7465 7374 203d 207b 7d0a 2020 2020  ontest = {}.    
+00009b20: 2020 2020 636f 6e74 6573 745b 2243 6f6e      contest["Con
+00009b30: 7465 7374 4e61 6d65 225d 203d 2028 0a20  testName"] = (. 
+00009b40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009b50: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
+00009b60: 6f6e 7465 7374 2e63 7572 7265 6e74 5465  ontest.currentTe
+00009b70: 7874 2829 2e6c 6f77 6572 2829 2e72 6570  xt().lower().rep
+00009b80: 6c61 6365 2822 2022 2c20 225f 2229 0a20  lace(" ", "_"). 
+00009b90: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00009ba0: 2063 6f6e 7465 7374 5b22 5374 6172 7444   contest["StartD
+00009bb0: 6174 6522 5d20 3d20 7365 6c66 2e63 6f6e  ate"] = self.con
+00009bc0: 7465 7374 5f64 6961 6c6f 672e 6461 7465  test_dialog.date
+00009bd0: 5469 6d65 4564 6974 2e64 6174 6554 696d  TimeEdit.dateTim
+00009be0: 6528 292e 746f 5374 7269 6e67 280a 2020  e().toString(.  
+00009bf0: 2020 2020 2020 2020 2020 2279 7979 792d            "yyyy-
+00009c00: 4d4d 2d64 6420 6868 3a6d 6d3a 7373 220a  MM-dd hh:mm:ss".
+00009c10: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00009c20: 2020 636f 6e74 6573 745b 224f 7065 7261    contest["Opera
+00009c30: 746f 7243 6174 6567 6f72 7922 5d20 3d20  torCategory"] = 
+00009c40: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00009c50: 6c6f 672e 6f70 6572 6174 6f72 5f63 6c61  log.operator_cla
+00009c60: 7373 2e63 7572 7265 6e74 5465 7874 2829  ss.currentText()
+00009c70: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+00009c80: 5b22 4261 6e64 4361 7465 676f 7279 225d  ["BandCategory"]
+00009c90: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+00009ca0: 6469 616c 6f67 2e62 616e 642e 6375 7272  dialog.band.curr
+00009cb0: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
+00009cc0: 2020 636f 6e74 6573 745b 2250 6f77 6572    contest["Power
+00009cd0: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
+00009ce0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00009cf0: 2e70 6f77 6572 2e63 7572 7265 6e74 5465  .power.currentTe
+00009d00: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
+00009d10: 7465 7374 5b22 4d6f 6465 4361 7465 676f  test["ModeCatego
+00009d20: 7279 225d 203d 2073 656c 662e 636f 6e74  ry"] = self.cont
+00009d30: 6573 745f 6469 616c 6f67 2e6d 6f64 652e  est_dialog.mode.
+00009d40: 6375 7272 656e 7454 6578 7428 290a 2020  currentText().  
+00009d50: 2020 2020 2020 636f 6e74 6573 745b 224f        contest["O
+00009d60: 7665 726c 6179 4361 7465 676f 7279 225d  verlayCategory"]
+00009d70: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+00009d80: 6469 616c 6f67 2e6f 7665 726c 6179 2e63  dialog.overlay.c
+00009d90: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
+00009da0: 2020 2020 2023 2063 6f6e 7465 7374 5b27       # contest['
+00009db0: 436c 6169 6d65 6453 636f 7265 275d 203d  ClaimedScore'] =
+00009dc0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00009dd0: 616c 6f67 2e0a 2020 2020 2020 2020 636f  alog..        co
+00009de0: 6e74 6573 745b 224f 7065 7261 746f 7273  ntest["Operators
+00009df0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
+00009e00: 745f 6469 616c 6f67 2e6f 7065 7261 746f  t_dialog.operato
+00009e10: 7273 2e74 6578 7428 290a 2020 2020 2020  rs.text().      
+00009e20: 2020 636f 6e74 6573 745b 2253 6f61 7062    contest["Soapb
+00009e30: 6f78 225d 203d 2073 656c 662e 636f 6e74  ox"] = self.cont
+00009e40: 6573 745f 6469 616c 6f67 2e73 6f61 7062  est_dialog.soapb
+00009e50: 6f78 2e74 6f50 6c61 696e 5465 7874 2829  ox.toPlainText()
+00009e60: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+00009e70: 5b22 5365 6e74 4578 6368 616e 6765 225d  ["SentExchange"]
+00009e80: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+00009e90: 6469 616c 6f67 2e65 7863 6861 6e67 652e  dialog.exchange.
+00009ea0: 7465 7874 2829 0a20 2020 2020 2020 2063  text().        c
+00009eb0: 6f6e 7465 7374 5b22 436f 6e74 6573 744e  ontest["ContestN
+00009ec0: 5222 5d20 3d20 6e65 7874 5f6e 756d 6265  R"] = next_numbe
+00009ed0: 722e 6765 7428 2263 6f75 6e74 222c 2031  r.get("count", 1
+00009ee0: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
+00009ef0: 7265 665b 2263 6f6e 7465 7374 225d 203d  ref["contest"] =
+00009f00: 206e 6578 745f 6e75 6d62 6572 2e67 6574   next_number.get
+00009f10: 2822 636f 756e 7422 2c20 3129 0a20 2020  ("count", 1).   
+00009f20: 2020 2020 2023 2063 6f6e 7465 7374 5b27       # contest['
+00009f30: 5375 6254 7970 6527 5d20 3d20 7365 6c66  SubType'] = self
+00009f40: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00009f50: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+00009f60: 5b22 5374 6174 696f 6e43 6174 6567 6f72  ["StationCategor
+00009f70: 7922 5d20 3d20 7365 6c66 2e63 6f6e 7465  y"] = self.conte
+00009f80: 7374 5f64 6961 6c6f 672e 7374 6174 696f  st_dialog.statio
+00009f90: 6e2e 6375 7272 656e 7454 6578 7428 290a  n.currentText().
+00009fa0: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+00009fb0: 2241 7373 6973 7465 6443 6174 6567 6f72  "AssistedCategor
+00009fc0: 7922 5d20 3d20 7365 6c66 2e63 6f6e 7465  y"] = self.conte
+00009fd0: 7374 5f64 6961 6c6f 672e 6173 7369 7374  st_dialog.assist
+00009fe0: 6564 2e63 7572 7265 6e74 5465 7874 2829  ed.currentText()
+00009ff0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+0000a000: 5b22 5472 616e 736d 6974 7465 7243 6174  ["TransmitterCat
+0000a010: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
+0000a020: 6f6e 7465 7374 5f64 6961 6c6f 672e 7472  ontest_dialog.tr
+0000a030: 616e 736d 6974 7465 722e 6375 7272 656e  ansmitter.curren
+0000a040: 7454 6578 7428 290a 2020 2020 2020 2020  tText().        
+0000a050: 2320 636f 6e74 6573 745b 2754 696d 6543  # contest['TimeC
+0000a060: 6174 6567 6f72 7927 5d20 3d20 7365 6c66  ategory'] = self
+0000a070: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+0000a080: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000a090: 6465 6275 6728 2225 7322 2c20 6622 7b63  debug("%s", f"{c
+0000a0a0: 6f6e 7465 7374 7d22 290a 2020 2020 2020  ontest}").      
+0000a0b0: 2020 7365 6c66 2e64 6174 6162 6173 652e    self.database.
+0000a0c0: 6164 645f 636f 6e74 6573 7428 636f 6e74  add_contest(cont
+0000a0d0: 6573 7429 0a20 2020 2020 2020 2073 656c  est).        sel
+0000a0e0: 662e 7772 6974 655f 7072 6566 6572 656e  f.write_preferen
+0000a0f0: 6365 2829 0a20 2020 2020 2020 2073 656c  ce().        sel
+0000a100: 662e 6c6f 6164 5f63 6f6e 7465 7374 2829  f.load_contest()
+0000a110: 0a0a 2020 2020 6465 6620 6564 6974 5f73  ..    def edit_s
+0000a120: 7461 7469 6f6e 5f73 6574 7469 6e67 7328  tation_settings(
+0000a130: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000a140: 2222 5368 6f77 2073 6574 7469 6e67 7320  ""Show settings 
+0000a150: 6469 616c 6f67 2222 220a 2020 2020 2020  dialog""".      
+0000a160: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000a170: 5374 6174 696f 6e20 5365 7474 696e 6773  Station Settings
+0000a180: 2073 656c 6563 7465 6422 290a 2020 2020   selected").    
+0000a190: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000a1a0: 735f 6469 616c 6f67 203d 2045 6469 7453  s_dialog = EditS
+0000a1b0: 7461 7469 6f6e 2857 4f52 4b49 4e47 5f50  tation(WORKING_P
+0000a1c0: 4154 4829 0a20 2020 2020 2020 2069 6620  ATH).        if 
+0000a1d0: 7365 6c66 2e70 7265 662e 6765 7428 2264  self.pref.get("d
+0000a1e0: 6172 6b5f 6d6f 6465 2229 3a0a 2020 2020  ark_mode"):.    
+0000a1f0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000a200: 7469 6e67 735f 6469 616c 6f67 2e73 6574  tings_dialog.set
+0000a210: 5374 796c 6553 6865 6574 2844 4152 4b5f  StyleSheet(DARK_
+0000a220: 5354 594c 4553 4845 4554 290a 2020 2020  STYLESHEET).    
+0000a230: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000a240: 735f 6469 616c 6f67 2e61 6363 6570 7465  s_dialog.accepte
+0000a250: 642e 636f 6e6e 6563 7428 7365 6c66 2e73  d.connect(self.s
+0000a260: 6176 655f 7365 7474 696e 6773 290a 2020  ave_settings).  
+0000a270: 2020 2020 2020 2320 6966 2073 656c 662e        # if self.
+0000a280: 7072 6566 2e67 6574 2822 6461 726b 5f6d  pref.get("dark_m
+0000a290: 6f64 6522 293a 0a20 2020 2020 2020 2023  ode"):.        #
+0000a2a0: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
+0000a2b0: 6773 5f64 6961 6c6f 672e 7365 7453 7479  gs_dialog.setSty
+0000a2c0: 6c65 5368 6565 7428 4441 524b 5f53 5459  leSheet(DARK_STY
+0000a2d0: 4c45 5348 4545 5429 0a0a 2020 2020 2020  LESHEET)..      
+0000a2e0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000a2f0: 6469 616c 6f67 2e43 616c 6c2e 7365 7454  dialog.Call.setT
+0000a300: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
+0000a310: 2e67 6574 2822 4361 6c6c 222c 2022 2229  .get("Call", "")
+0000a320: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000a330: 6574 7469 6e67 735f 6469 616c 6f67 2e4e  ettings_dialog.N
+0000a340: 616d 652e 7365 7454 6578 7428 7365 6c66  ame.setText(self
+0000a350: 2e73 7461 7469 6f6e 2e67 6574 2822 4e61  .station.get("Na
+0000a360: 6d65 222c 2022 2229 290a 2020 2020 2020  me", "")).      
+0000a370: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000a380: 6469 616c 6f67 2e41 6464 7265 7373 312e  dialog.Address1.
+0000a390: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
+0000a3a0: 7469 6f6e 2e67 6574 2822 5374 7265 6574  tion.get("Street
+0000a3b0: 3122 2c20 2222 2929 0a20 2020 2020 2020  1", "")).       
+0000a3c0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+0000a3d0: 6961 6c6f 672e 4164 6472 6573 7332 2e73  ialog.Address2.s
+0000a3e0: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
+0000a3f0: 696f 6e2e 6765 7428 2253 7472 6565 7432  ion.get("Street2
+0000a400: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
+0000a410: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000a420: 616c 6f67 2e43 6974 792e 7365 7454 6578  alog.City.setTex
+0000a430: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
+0000a440: 6574 2822 4369 7479 222c 2022 2229 290a  et("City", "")).
+0000a450: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000a460: 7469 6e67 735f 6469 616c 6f67 2e53 7461  tings_dialog.Sta
+0000a470: 7465 2e73 6574 5465 7874 2873 656c 662e  te.setText(self.
+0000a480: 7374 6174 696f 6e2e 6765 7428 2253 7461  station.get("Sta
+0000a490: 7465 222c 2022 2229 290a 2020 2020 2020  te", "")).      
+0000a4a0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000a4b0: 6469 616c 6f67 2e5a 6970 2e73 6574 5465  dialog.Zip.setTe
+0000a4c0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+0000a4d0: 6765 7428 225a 6970 222c 2022 2229 290a  get("Zip", "")).
+0000a4e0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000a4f0: 7469 6e67 735f 6469 616c 6f67 2e43 6f75  tings_dialog.Cou
+0000a500: 6e74 7279 2e73 6574 5465 7874 2873 656c  ntry.setText(sel
+0000a510: 662e 7374 6174 696f 6e2e 6765 7428 2243  f.station.get("C
+0000a520: 6f75 6e74 7279 222c 2022 2229 290a 2020  ountry", "")).  
+0000a530: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000a540: 6e67 735f 6469 616c 6f67 2e47 7269 6453  ngs_dialog.GridS
+0000a550: 7175 6172 652e 7365 7454 6578 7428 7365  quare.setText(se
+0000a560: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+0000a570: 4772 6964 5371 7561 7265 222c 2022 2229  GridSquare", "")
+0000a580: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000a590: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
+0000a5a0: 515a 6f6e 652e 7365 7454 6578 7428 7374  QZone.setText(st
+0000a5b0: 7228 7365 6c66 2e73 7461 7469 6f6e 2e67  r(self.station.g
+0000a5c0: 6574 2822 4351 5a6f 6e65 222c 2022 2229  et("CQZone", "")
+0000a5d0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000a5e0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000a5f0: 4954 555a 6f6e 652e 7365 7454 6578 7428  ITUZone.setText(
+0000a600: 7374 7228 7365 6c66 2e73 7461 7469 6f6e  str(self.station
+0000a610: 2e67 6574 2822 4941 5255 5a6f 6e65 222c  .get("IARUZone",
+0000a620: 2022 2229 2929 0a20 2020 2020 2020 2073   ""))).        s
+0000a630: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+0000a640: 6c6f 672e 4c69 6365 6e73 652e 7365 7454  log.License.setT
+0000a650: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
+0000a660: 2e67 6574 2822 4c69 6365 6e73 6543 6c61  .get("LicenseCla
+0000a670: 7373 222c 2022 2229 290a 2020 2020 2020  ss", "")).      
+0000a680: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000a690: 6469 616c 6f67 2e4c 6174 6974 7564 652e  dialog.Latitude.
+0000a6a0: 7365 7454 6578 7428 7374 7228 7365 6c66  setText(str(self
+0000a6b0: 2e73 7461 7469 6f6e 2e67 6574 2822 4c61  .station.get("La
+0000a6c0: 7469 7475 6465 222c 2022 2229 2929 0a20  titude", ""))). 
+0000a6d0: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
+0000a6e0: 696e 6773 5f64 6961 6c6f 672e 4c6f 6e67  ings_dialog.Long
+0000a6f0: 6974 7564 652e 7365 7454 6578 7428 7374  itude.setText(st
+0000a700: 7228 7365 6c66 2e73 7461 7469 6f6e 2e67  r(self.station.g
+0000a710: 6574 2822 4c6f 6e67 6974 7564 6522 2c20  et("Longitude", 
+0000a720: 2222 2929 290a 2020 2020 2020 2020 7365  ""))).        se
+0000a730: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000a740: 6f67 2e53 7461 7469 6f6e 5458 5258 2e73  og.StationTXRX.s
+0000a750: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
+0000a760: 696f 6e2e 6765 7428 2273 7461 7469 6f6e  ion.get("station
+0000a770: 7478 7278 222c 2022 2229 290a 2020 2020  txrx", "")).    
+0000a780: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000a790: 735f 6469 616c 6f67 2e50 6f77 6572 2e73  s_dialog.Power.s
+0000a7a0: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
+0000a7b0: 696f 6e2e 6765 7428 2253 506f 7765 222c  ion.get("SPowe",
+0000a7c0: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
+0000a7d0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000a7e0: 6f67 2e41 6e74 656e 6e61 2e73 6574 5465  og.Antenna.setTe
+0000a7f0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+0000a800: 6765 7428 2253 416e 7465 222c 2022 2229  get("SAnte", "")
+0000a810: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000a820: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
+0000a830: 6e74 4865 6967 6874 2e73 6574 5465 7874  ntHeight.setText
+0000a840: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
+0000a850: 7428 2253 416e 7448 3122 2c20 2222 2929  t("SAntH1", ""))
+0000a860: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0000a870: 7474 696e 6773 5f64 6961 6c6f 672e 4153  ttings_dialog.AS
+0000a880: 4c2e 7365 7454 6578 7428 7365 6c66 2e73  L.setText(self.s
+0000a890: 7461 7469 6f6e 2e67 6574 2822 5341 6e74  tation.get("SAnt
+0000a8a0: 4832 222c 2022 2229 290a 2020 2020 2020  H2", "")).      
+0000a8b0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000a8c0: 6469 616c 6f67 2e41 5252 4c53 6563 7469  dialog.ARRLSecti
+0000a8d0: 6f6e 2e73 6574 5465 7874 2873 656c 662e  on.setText(self.
+0000a8e0: 7374 6174 696f 6e2e 6765 7428 2241 5252  station.get("ARR
+0000a8f0: 4c53 6563 7469 6f6e 222c 2022 2229 290a  LSection", "")).
+0000a900: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000a910: 7469 6e67 735f 6469 616c 6f67 2e52 6f76  tings_dialog.Rov
+0000a920: 6572 5154 482e 7365 7454 6578 7428 7365  erQTH.setText(se
+0000a930: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+0000a940: 526f 7665 7251 5448 222c 2022 2229 290a  RoverQTH", "")).
+0000a950: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000a960: 7469 6e67 735f 6469 616c 6f67 2e43 6c75  tings_dialog.Clu
+0000a970: 622e 7365 7454 6578 7428 7365 6c66 2e73  b.setText(self.s
+0000a980: 7461 7469 6f6e 2e67 6574 2822 436c 7562  tation.get("Club
+0000a990: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
+0000a9a0: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000a9b0: 616c 6f67 2e45 6d61 696c 2e73 6574 5465  alog.Email.setTe
+0000a9c0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+0000a9d0: 6765 7428 2245 6d61 696c 222c 2022 2229  get("Email", "")
 0000a9e0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000a9f0: 7461 7469 6f6e 5b22 4351 5a6f 6e65 225d  tation["CQZone"]
-0000aa00: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-0000aa10: 5f64 6961 6c6f 672e 4351 5a6f 6e65 2e74  _dialog.CQZone.t
-0000aa20: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
-0000aa30: 6c66 2e73 7461 7469 6f6e 5b22 4941 5255  lf.station["IARU
-0000aa40: 5a6f 6e65 225d 203d 2073 656c 662e 7365  Zone"] = self.se
-0000aa50: 7474 696e 6773 5f64 6961 6c6f 672e 4954  ttings_dialog.IT
-0000aa60: 555a 6f6e 652e 7465 7874 2829 0a20 2020  UZone.text().   
-0000aa70: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-0000aa80: 6e5b 224c 6963 656e 7365 436c 6173 7322  n["LicenseClass"
-0000aa90: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
-0000aaa0: 735f 6469 616c 6f67 2e4c 6963 656e 7365  s_dialog.License
-0000aab0: 2e74 6578 7428 292e 7469 746c 6528 290a  .text().title().
-0000aac0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0000aad0: 7469 6f6e 5b22 4c61 7469 7475 6465 225d  tion["Latitude"]
-0000aae0: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-0000aaf0: 5f64 6961 6c6f 672e 4c61 7469 7475 6465  _dialog.Latitude
-0000ab00: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-0000ab10: 7365 6c66 2e73 7461 7469 6f6e 5b22 4c6f  self.station["Lo
-0000ab20: 6e67 6974 7564 6522 5d20 3d20 7365 6c66  ngitude"] = self
-0000ab30: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000ab40: 2e4c 6f6e 6769 7475 6465 2e74 6578 7428  .Longitude.text(
-0000ab50: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000ab60: 7461 7469 6f6e 5b22 5354 5865 7122 5d20  tation["STXeq"] 
-0000ab70: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
-0000ab80: 6469 616c 6f67 2e53 7461 7469 6f6e 5458  dialog.StationTX
-0000ab90: 5258 2e74 6578 7428 290a 2020 2020 2020  RX.text().      
-0000aba0: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
-0000abb0: 5350 6f77 6522 5d20 3d20 7365 6c66 2e73  SPowe"] = self.s
-0000abc0: 6574 7469 6e67 735f 6469 616c 6f67 2e50  ettings_dialog.P
-0000abd0: 6f77 6572 2e74 6578 7428 290a 2020 2020  ower.text().    
-0000abe0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
-0000abf0: 5b22 5341 6e74 6522 5d20 3d20 7365 6c66  ["SAnte"] = self
-0000ac00: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000ac10: 2e41 6e74 656e 6e61 2e74 6578 7428 290a  .Antenna.text().
-0000ac20: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0000ac30: 7469 6f6e 5b22 5341 6e74 4831 225d 203d  tion["SAntH1"] =
-0000ac40: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000ac50: 6961 6c6f 672e 416e 7448 6569 6768 742e  ialog.AntHeight.
-0000ac60: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
-0000ac70: 656c 662e 7374 6174 696f 6e5b 2253 416e  elf.station["SAn
-0000ac80: 7448 3222 5d20 3d20 7365 6c66 2e73 6574  tH2"] = self.set
-0000ac90: 7469 6e67 735f 6469 616c 6f67 2e41 534c  tings_dialog.ASL
-0000aca0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-0000acb0: 7365 6c66 2e73 7461 7469 6f6e 5b22 4152  self.station["AR
-0000acc0: 524c 5365 6374 696f 6e22 5d20 3d20 7365  RLSection"] = se
-0000acd0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000ace0: 6f67 2e41 5252 4c53 6563 7469 6f6e 2e74  og.ARRLSection.t
-0000acf0: 6578 7428 292e 7570 7065 7228 290a 2020  ext().upper().  
-0000ad00: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-0000ad10: 6f6e 5b22 526f 7665 7251 5448 225d 203d  on["RoverQTH"] =
-0000ad20: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000ad30: 6961 6c6f 672e 526f 7665 7251 5448 2e74  ialog.RoverQTH.t
+0000a9f0: 6574 7469 6e67 735f 6469 616c 6f67 2e6f  ettings_dialog.o
+0000aa00: 7065 6e28 290a 0a20 2020 2064 6566 2073  pen()..    def s
+0000aa10: 6176 655f 7365 7474 696e 6773 2873 656c  ave_settings(sel
+0000aa20: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
+0000aa30: 6176 6520 7365 7474 696e 6773 2222 220a  ave settings""".
+0000aa40: 2020 2020 2020 2020 6373 203d 2073 656c          cs = sel
+0000aa50: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000aa60: 672e 4361 6c6c 2e74 6578 7428 290a 2020  g.Call.text().  
+0000aa70: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000aa80: 6f6e 203d 207b 7d0a 2020 2020 2020 2020  on = {}.        
+0000aa90: 7365 6c66 2e73 7461 7469 6f6e 5b22 4361  self.station["Ca
+0000aaa0: 6c6c 225d 203d 2063 732e 7570 7065 7228  ll"] = cs.upper(
+0000aab0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000aac0: 7461 7469 6f6e 5b22 4e61 6d65 225d 203d  tation["Name"] =
+0000aad0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+0000aae0: 6961 6c6f 672e 4e61 6d65 2e74 6578 7428  ialog.Name.text(
+0000aaf0: 292e 7469 746c 6528 290a 2020 2020 2020  ).title().      
+0000ab00: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000ab10: 5374 7265 6574 3122 5d20 3d20 7365 6c66  Street1"] = self
+0000ab20: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000ab30: 2e41 6464 7265 7373 312e 7465 7874 2829  .Address1.text()
+0000ab40: 2e74 6974 6c65 2829 0a20 2020 2020 2020  .title().       
+0000ab50: 2073 656c 662e 7374 6174 696f 6e5b 2253   self.station["S
+0000ab60: 7472 6565 7432 225d 203d 2073 656c 662e  treet2"] = self.
+0000ab70: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000ab80: 4164 6472 6573 7332 2e74 6578 7428 292e  Address2.text().
+0000ab90: 7469 746c 6528 290a 2020 2020 2020 2020  title().        
+0000aba0: 7365 6c66 2e73 7461 7469 6f6e 5b22 4369  self.station["Ci
+0000abb0: 7479 225d 203d 2073 656c 662e 7365 7474  ty"] = self.sett
+0000abc0: 696e 6773 5f64 6961 6c6f 672e 4369 7479  ings_dialog.City
+0000abd0: 2e74 6578 7428 292e 7469 746c 6528 290a  .text().title().
+0000abe0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0000abf0: 7469 6f6e 5b22 5374 6174 6522 5d20 3d20  tion["State"] = 
+0000ac00: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000ac10: 616c 6f67 2e53 7461 7465 2e74 6578 7428  alog.State.text(
+0000ac20: 292e 7570 7065 7228 290a 2020 2020 2020  ).upper().      
+0000ac30: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000ac40: 5a69 7022 5d20 3d20 7365 6c66 2e73 6574  Zip"] = self.set
+0000ac50: 7469 6e67 735f 6469 616c 6f67 2e5a 6970  tings_dialog.Zip
+0000ac60: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000ac70: 7365 6c66 2e73 7461 7469 6f6e 5b22 436f  self.station["Co
+0000ac80: 756e 7472 7922 5d20 3d20 7365 6c66 2e73  untry"] = self.s
+0000ac90: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
+0000aca0: 6f75 6e74 7279 2e74 6578 7428 292e 7469  ountry.text().ti
+0000acb0: 746c 6528 290a 2020 2020 2020 2020 7365  tle().        se
+0000acc0: 6c66 2e73 7461 7469 6f6e 5b22 4772 6964  lf.station["Grid
+0000acd0: 5371 7561 7265 225d 203d 2073 656c 662e  Square"] = self.
+0000ace0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000acf0: 4772 6964 5371 7561 7265 2e74 6578 7428  GridSquare.text(
+0000ad00: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000ad10: 7461 7469 6f6e 5b22 4351 5a6f 6e65 225d  tation["CQZone"]
+0000ad20: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
+0000ad30: 5f64 6961 6c6f 672e 4351 5a6f 6e65 2e74  _dialog.CQZone.t
 0000ad40: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
-0000ad50: 6c66 2e73 7461 7469 6f6e 5b22 436c 7562  lf.station["Club
-0000ad60: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
-0000ad70: 6773 5f64 6961 6c6f 672e 436c 7562 2e74  gs_dialog.Club.t
-0000ad80: 6578 7428 292e 7469 746c 6528 290a 2020  ext().title().  
-0000ad90: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-0000ada0: 6f6e 5b22 456d 6169 6c22 5d20 3d20 7365  on["Email"] = se
-0000adb0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000adc0: 6f67 2e45 6d61 696c 2e74 6578 7428 290a  og.Email.text().
-0000add0: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
-0000ade0: 6162 6173 652e 6164 645f 7374 6174 696f  abase.add_statio
-0000adf0: 6e28 7365 6c66 2e73 7461 7469 6f6e 290a  n(self.station).
-0000ae00: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000ae10: 7469 6e67 735f 6469 616c 6f67 2e63 6c6f  tings_dialog.clo
-0000ae20: 7365 2829 0a20 2020 2020 2020 2069 6620  se().        if 
-0000ae30: 7365 6c66 2e63 7572 7265 6e74 5f6f 7020  self.current_op 
-0000ae40: 3d3d 2022 223a 0a20 2020 2020 2020 2020  == "":.         
-0000ae50: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
-0000ae60: 6f70 203d 2073 656c 662e 7374 6174 696f  op = self.statio
-0000ae70: 6e2e 6765 7428 2243 616c 6c22 2c20 2222  n.get("Call", ""
-0000ae80: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0000ae90: 6c66 2e6d 616b 655f 6f70 5f64 6972 2829  lf.make_op_dir()
-0000aea0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-0000aeb0: 5f63 6f75 6e74 203d 2073 656c 662e 6461  _count = self.da
-0000aec0: 7461 6261 7365 2e66 6574 6368 5f61 6c6c  tabase.fetch_all
-0000aed0: 5f63 6f6e 7465 7374 7328 290a 2020 2020  _contests().    
-0000aee0: 2020 2020 6966 206c 656e 2863 6f6e 7465      if len(conte
-0000aef0: 7374 5f63 6f75 6e74 2920 3d3d 2030 3a0a  st_count) == 0:.
-0000af00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000af10: 2e6e 6577 5f63 6f6e 7465 7374 5f64 6961  .new_contest_dia
-0000af20: 6c6f 6728 290a 0a20 2020 2064 6566 2065  log()..    def e
-0000af30: 6469 745f 6d61 6372 6f28 7365 6c66 2c20  dit_macro(self, 
-0000af40: 6675 6e63 7469 6f6e 5f6b 6579 293a 0a20  function_key):. 
-0000af50: 2020 2020 2020 2022 2222 5368 6f77 2065         """Show e
-0000af60: 6469 7420 6d61 6372 6f20 6469 616c 6f67  dit macro dialog
-0000af70: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-0000af80: 2e65 6469 745f 6d61 6372 6f5f 6469 616c  .edit_macro_dial
-0000af90: 6f67 203d 2045 6469 744d 6163 726f 2866  og = EditMacro(f
-0000afa0: 756e 6374 696f 6e5f 6b65 792c 2057 4f52  unction_key, WOR
-0000afb0: 4b49 4e47 5f50 4154 4829 0a20 2020 2020  KING_PATH).     
-0000afc0: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000afd0: 726f 5f64 6961 6c6f 672e 6163 6365 7074  ro_dialog.accept
-0000afe0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-0000aff0: 6564 6974 6564 5f6d 6163 726f 290a 2020  edited_macro).  
-0000b000: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-0000b010: 6566 2e67 6574 2822 6461 726b 5f6d 6f64  ef.get("dark_mod
-0000b020: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
-0000b030: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000b040: 5f64 6961 6c6f 672e 7365 7453 7479 6c65  _dialog.setStyle
-0000b050: 5368 6565 7428 4441 524b 5f53 5459 4c45  Sheet(DARK_STYLE
-0000b060: 5348 4545 5429 0a20 2020 2020 2020 2073  SHEET).        s
-0000b070: 656c 662e 6564 6974 5f6d 6163 726f 5f64  elf.edit_macro_d
-0000b080: 6961 6c6f 672e 6f70 656e 2829 0a0a 2020  ialog.open()..  
-0000b090: 2020 6465 6620 6564 6974 6564 5f6d 6163    def edited_mac
-0000b0a0: 726f 2873 656c 6629 3a0a 2020 2020 2020  ro(self):.      
-0000b0b0: 2020 2222 2253 6176 6520 6564 6974 6564    """Save edited
-0000b0c0: 206d 6163 726f 2222 220a 2020 2020 2020   macro""".      
-0000b0d0: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
-0000b0e0: 6f5f 6469 616c 6f67 2e66 756e 6374 696f  o_dialog.functio
-0000b0f0: 6e5f 6b65 792e 7365 7454 6578 7428 0a20  n_key.setText(. 
-0000b100: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b110: 6564 6974 5f6d 6163 726f 5f64 6961 6c6f  edit_macro_dialo
-0000b120: 672e 6d61 6372 6f5f 6c61 6265 6c2e 7465  g.macro_label.te
-0000b130: 7874 2829 0a20 2020 2020 2020 2029 0a20  xt().        ). 
-0000b140: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-0000b150: 5f6d 6163 726f 5f64 6961 6c6f 672e 6675  _macro_dialog.fu
-0000b160: 6e63 7469 6f6e 5f6b 6579 2e73 6574 546f  nction_key.setTo
-0000b170: 6f6c 5469 7028 0a20 2020 2020 2020 2020  olTip(.         
-0000b180: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000b190: 726f 5f64 6961 6c6f 672e 7468 655f 6d61  ro_dialog.the_ma
-0000b1a0: 6372 6f2e 7465 7874 2829 0a20 2020 2020  cro.text().     
-0000b1b0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-0000b1c0: 662e 6564 6974 5f6d 6163 726f 5f64 6961  f.edit_macro_dia
-0000b1d0: 6c6f 672e 636c 6f73 6528 290a 0a20 2020  log.close()..   
-0000b1e0: 2064 6566 2065 6469 745f 4631 2873 656c   def edit_F1(sel
-0000b1f0: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000b200: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000b210: 6f67 6765 722e 6465 6275 6728 2246 3120  ogger.debug("F1 
-0000b220: 5269 6768 7420 436c 6963 6b65 642e 2229  Right Clicked.")
-0000b230: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
-0000b240: 6974 5f6d 6163 726f 2873 656c 662e 4631  it_macro(self.F1
-0000b250: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
-0000b260: 4632 2873 656c 6629 3a0a 2020 2020 2020  F2(self):.      
-0000b270: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000b280: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000b290: 6728 2246 3220 5269 6768 7420 436c 6963  g("F2 Right Clic
-0000b2a0: 6b65 642e 2229 0a20 2020 2020 2020 2073  ked.").        s
-0000b2b0: 656c 662e 6564 6974 5f6d 6163 726f 2873  elf.edit_macro(s
-0000b2c0: 656c 662e 4632 290a 0a20 2020 2064 6566  elf.F2)..    def
-0000b2d0: 2065 6469 745f 4633 2873 656c 6629 3a0a   edit_F3(self):.
-0000b2e0: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
-0000b2f0: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
-0000b300: 722e 6465 6275 6728 2246 3320 5269 6768  r.debug("F3 Righ
-0000b310: 7420 436c 6963 6b65 642e 2229 0a20 2020  t Clicked.").   
-0000b320: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
-0000b330: 6163 726f 2873 656c 662e 4633 290a 0a20  acro(self.F3).. 
-0000b340: 2020 2064 6566 2065 6469 745f 4634 2873     def edit_F4(s
-0000b350: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000b360: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
-0000b370: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-0000b380: 3420 5269 6768 7420 436c 6963 6b65 642e  4 Right Clicked.
-0000b390: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000b3a0: 6564 6974 5f6d 6163 726f 2873 656c 662e  edit_macro(self.
-0000b3b0: 4634 290a 0a20 2020 2064 6566 2065 6469  F4)..    def edi
-0000b3c0: 745f 4635 2873 656c 6629 3a0a 2020 2020  t_F5(self):.    
-0000b3d0: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
-0000b3e0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000b3f0: 6275 6728 2246 3520 5269 6768 7420 436c  bug("F5 Right Cl
-0000b400: 6963 6b65 642e 2229 0a20 2020 2020 2020  icked.").       
-0000b410: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000b420: 2873 656c 662e 4635 290a 0a20 2020 2064  (self.F5)..    d
-0000b430: 6566 2065 6469 745f 4636 2873 656c 6629  ef edit_F6(self)
-0000b440: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
-0000b450: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
-0000b460: 6765 722e 6465 6275 6728 2246 3620 5269  ger.debug("F6 Ri
-0000b470: 6768 7420 436c 6963 6b65 642e 2229 0a20  ght Clicked."). 
-0000b480: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-0000b490: 5f6d 6163 726f 2873 656c 662e 4636 290a  _macro(self.F6).
-0000b4a0: 0a20 2020 2064 6566 2065 6469 745f 4637  .    def edit_F7
-0000b4b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000b4c0: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
-0000b4d0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000b4e0: 2246 3720 5269 6768 7420 436c 6963 6b65  "F7 Right Clicke
-0000b4f0: 642e 2229 0a20 2020 2020 2020 2073 656c  d.").        sel
-0000b500: 662e 6564 6974 5f6d 6163 726f 2873 656c  f.edit_macro(sel
-0000b510: 662e 4637 290a 0a20 2020 2064 6566 2065  f.F7)..    def e
-0000b520: 6469 745f 4638 2873 656c 6629 3a0a 2020  dit_F8(self):.  
-0000b530: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
-0000b540: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000b550: 6465 6275 6728 2246 3820 5269 6768 7420  debug("F8 Right 
-0000b560: 436c 6963 6b65 642e 2229 0a20 2020 2020  Clicked.").     
-0000b570: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000b580: 726f 2873 656c 662e 4638 290a 0a20 2020  ro(self.F8)..   
-0000b590: 2064 6566 2065 6469 745f 4639 2873 656c   def edit_F9(sel
-0000b5a0: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000b5b0: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000b5c0: 6f67 6765 722e 6465 6275 6728 2246 3920  ogger.debug("F9 
-0000b5d0: 5269 6768 7420 436c 6963 6b65 642e 2229  Right Clicked.")
-0000b5e0: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
-0000b5f0: 6974 5f6d 6163 726f 2873 656c 662e 4639  it_macro(self.F9
-0000b600: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
-0000b610: 4631 3028 7365 6c66 293a 0a20 2020 2020  F10(self):.     
-0000b620: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
-0000b630: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000b640: 7567 2822 4631 3020 5269 6768 7420 436c  ug("F10 Right Cl
-0000b650: 6963 6b65 642e 2229 0a20 2020 2020 2020  icked.").       
-0000b660: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000b670: 2873 656c 662e 4631 3029 0a0a 2020 2020  (self.F10)..    
-0000b680: 6465 6620 6564 6974 5f46 3131 2873 656c  def edit_F11(sel
-0000b690: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000b6a0: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000b6b0: 6f67 6765 722e 6465 6275 6728 2246 3131  ogger.debug("F11
-0000b6c0: 2052 6967 6874 2043 6c69 636b 6564 2e22   Right Clicked."
-0000b6d0: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
-0000b6e0: 6469 745f 6d61 6372 6f28 7365 6c66 2e46  dit_macro(self.F
-0000b6f0: 3131 290a 0a20 2020 2064 6566 2065 6469  11)..    def edi
-0000b700: 745f 4631 3228 7365 6c66 293a 0a20 2020  t_F12(self):.   
-0000b710: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
-0000b720: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000b730: 6562 7567 2822 4631 3220 5269 6768 7420  ebug("F12 Right 
-0000b740: 436c 6963 6b65 642e 2229 0a20 2020 2020  Clicked.").     
-0000b750: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000b760: 726f 2873 656c 662e 4631 3229 0a0a 2020  ro(self.F12)..  
-0000b770: 2020 6465 6620 7072 6f63 6573 735f 6d61    def process_ma
-0000b780: 6372 6f28 7365 6c66 2c20 6d61 6372 6f3a  cro(self, macro:
-0000b790: 2073 7472 2920 2d3e 2073 7472 3a0a 2020   str) -> str:.  
-0000b7a0: 2020 2020 2020 2222 2250 726f 6365 7373        """Process
-0000b7b0: 2043 5720 6d61 6372 6f20 7375 6273 7469   CW macro substi
-0000b7c0: 7475 7469 6f6e 7322 2222 0a20 2020 2020  tutions""".     
-0000b7d0: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-0000b7e0: 2e64 6174 6162 6173 652e 6765 745f 7365  .database.get_se
-0000b7f0: 7269 616c 2829 0a20 2020 2020 2020 2070  rial().        p
-0000b800: 7269 6e74 2872 6573 756c 7429 0a20 2020  rint(result).   
-0000b810: 2020 2020 206e 6578 745f 7365 7269 616c       next_serial
-0000b820: 203d 2073 7472 2872 6573 756c 742e 6765   = str(result.ge
-0000b830: 7428 2273 6572 6961 6c5f 6e72 222c 2022  t("serial_nr", "
-0000b840: 3122 2929 0a20 2020 2020 2020 2069 6620  1")).        if 
-0000b850: 6e65 7874 5f73 6572 6961 6c20 3d3d 2022  next_serial == "
-0000b860: 4e6f 6e65 223a 0a20 2020 2020 2020 2020  None":.         
-0000b870: 2020 206e 6578 745f 7365 7269 616c 203d     next_serial =
-0000b880: 2022 3122 0a20 2020 2020 2020 2070 7269   "1".        pri
-0000b890: 6e74 286e 6578 745f 7365 7269 616c 290a  nt(next_serial).
-0000b8a0: 2020 2020 2020 2020 6d61 6372 6f20 3d20          macro = 
-0000b8b0: 6d61 6372 6f2e 7570 7065 7228 290a 2020  macro.upper().  
-0000b8c0: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
-0000b8d0: 6372 6f2e 7265 706c 6163 6528 2223 222c  cro.replace("#",
-0000b8e0: 206e 6578 745f 7365 7269 616c 290a 2020   next_serial).  
-0000b8f0: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
-0000b900: 6372 6f2e 7265 706c 6163 6528 227b 4d59  cro.replace("{MY
-0000b910: 4341 4c4c 7d22 2c20 7365 6c66 2e73 7461  CALL}", self.sta
-0000b920: 7469 6f6e 2e67 6574 2822 4361 6c6c 222c  tion.get("Call",
-0000b930: 2022 2229 290a 2020 2020 2020 2020 6d61   "")).        ma
-0000b940: 6372 6f20 3d20 6d61 6372 6f2e 7265 706c  cro = macro.repl
-0000b950: 6163 6528 227b 4849 5343 414c 4c7d 222c  ace("{HISCALL}",
-0000b960: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
-0000b970: 6578 7428 2929 0a20 2020 2020 2020 2069  ext()).        i
-0000b980: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
-0000b990: 7465 2e67 6574 2822 6d6f 6465 2229 203d  te.get("mode") =
-0000b9a0: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
-0000b9b0: 2020 2020 6d61 6372 6f20 3d20 6d61 6372      macro = macr
-0000b9c0: 6f2e 7265 706c 6163 6528 227b 534e 547d  o.replace("{SNT}
-0000b9d0: 222c 2073 656c 662e 7365 6e74 2e74 6578  ", self.sent.tex
-0000b9e0: 7428 292e 7265 706c 6163 6528 2239 222c  t().replace("9",
-0000b9f0: 2022 6e22 2929 0a20 2020 2020 2020 2065   "n")).        e
-0000ba00: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000ba10: 206d 6163 726f 203d 206d 6163 726f 2e72   macro = macro.r
-0000ba20: 6570 6c61 6365 2822 7b53 4e54 7d22 2c20  eplace("{SNT}", 
-0000ba30: 7365 6c66 2e73 656e 742e 7465 7874 2829  self.sent.text()
-0000ba40: 290a 2020 2020 2020 2020 6d61 6372 6f20  ).        macro 
-0000ba50: 3d20 6d61 6372 6f2e 7265 706c 6163 6528  = macro.replace(
-0000ba60: 227b 5345 4e54 4e52 7d22 2c20 7365 6c66  "{SENTNR}", self
-0000ba70: 2e6f 7468 6572 5f31 2e74 6578 7428 2929  .other_1.text())
-0000ba80: 0a20 2020 2020 2020 206d 6163 726f 203d  .        macro =
-0000ba90: 206d 6163 726f 2e72 6570 6c61 6365 280a   macro.replace(.
-0000baa0: 2020 2020 2020 2020 2020 2020 227b 4558              "{EX
-0000bab0: 4348 7d22 2c20 7365 6c66 2e63 6f6e 7465  CH}", self.conte
-0000bac0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
-0000bad0: 2253 656e 7445 7863 6861 6e67 6522 2c20  "SentExchange", 
-0000bae0: 2278 7878 2229 0a20 2020 2020 2020 2029  "xxx").        )
-0000baf0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000bb00: 6d61 6372 6f0a 0a20 2020 2064 6566 2076  macro..    def v
-0000bb10: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
-0000bb20: 2c20 7468 655f 7374 7269 6e67 3a20 7374  , the_string: st
-0000bb30: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
-0000bb40: 2020 2020 2222 2276 6f69 6365 7320 7374      """voices st
-0000bb50: 7269 6e67 2075 7369 6e67 206e 6174 6f20  ring using nato 
-0000bb60: 7068 6f6e 6574 6963 7322 2222 0a20 2020  phonetics""".   
-0000bb70: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000bb80: 6728 2256 6f69 6369 6e67 3a20 2573 222c  g("Voicing: %s",
-0000bb90: 2074 6865 5f73 7472 696e 6729 0a20 2020   the_string).   
-0000bba0: 2020 2020 206f 705f 7061 7468 203d 2050       op_path = P
-0000bbb0: 6174 6828 4441 5441 5f50 4154 4829 202f  ath(DATA_PATH) /
-0000bbc0: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
-0000bbd0: 0a20 2020 2020 2020 2069 6620 225b 2220  .        if "[" 
-0000bbe0: 696e 2074 6865 5f73 7472 696e 673a 0a20  in the_string:. 
-0000bbf0: 2020 2020 2020 2020 2020 2073 7562 5f73             sub_s
-0000bc00: 7472 696e 6720 3d20 7468 655f 7374 7269  tring = the_stri
-0000bc10: 6e67 2e73 7472 6970 2822 5b5d 2229 2e6c  ng.strip("[]").l
-0000bc20: 6f77 6572 2829 0a20 2020 2020 2020 2020  ower().         
-0000bc30: 2020 2066 696c 656e 616d 6520 3d20 6622     filename = f"
-0000bc40: 7b73 7472 286f 705f 7061 7468 297d 2f7b  {str(op_path)}/{
-0000bc50: 7375 625f 7374 7269 6e67 7d2e 7761 7622  sub_string}.wav"
-0000bc60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000bc70: 5061 7468 2866 696c 656e 616d 6529 2e69  Path(filename).i
-0000bc80: 735f 6669 6c65 2829 3a0a 2020 2020 2020  s_file():.      
-0000bc90: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000bca0: 2e64 6562 7567 2822 566f 6963 696e 673a  .debug("Voicing:
-0000bcb0: 2025 7322 2c20 6669 6c65 6e61 6d65 290a   %s", filename).
-0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcd0: 6461 7461 2c20 5f66 7320 3d20 7366 2e72  data, _fs = sf.r
-0000bce0: 6561 6428 6669 6c65 6e61 6d65 2c20 6474  ead(filename, dt
-0000bcf0: 7970 653d 2266 6c6f 6174 3332 2229 0a20  ype="float32"). 
-0000bd00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000bd10: 656c 662e 7074 745f 6f6e 2829 0a20 2020  elf.ptt_on().   
-0000bd20: 2020 2020 2020 2020 2020 2020 2074 7279               try
-0000bd30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000bd40: 2020 2020 2020 7364 2e64 6566 6175 6c74        sd.default
-0000bd50: 2e64 6576 6963 6520 3d20 7365 6c66 2e70  .device = self.p
-0000bd60: 7265 662e 6765 7428 2273 6f75 6e64 6465  ref.get("soundde
-0000bd70: 7669 6365 222c 2022 6465 6661 756c 7422  vice", "default"
-0000bd80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000bd90: 2020 2020 2020 7364 2e64 6566 6175 6c74        sd.default
-0000bda0: 2e73 616d 706c 6572 6174 6520 3d20 3434  .samplerate = 44
-0000bdb0: 3130 302e 300a 2020 2020 2020 2020 2020  100.0.          
-0000bdc0: 2020 2020 2020 2020 2020 7364 2e70 6c61            sd.pla
-0000bdd0: 7928 6461 7461 290a 2020 2020 2020 2020  y(data).        
-0000bde0: 2020 2020 2020 2020 2020 2020 5f73 7461              _sta
-0000bdf0: 7475 7320 3d20 7364 2e77 6169 7428 290a  tus = sd.wait().
-0000be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be10: 2020 2020 2320 6874 7470 733a 2f2f 736e      # https://sn
-0000be20: 796b 2e69 6f2f 6164 7669 736f 722f 7079  yk.io/advisor/py
-0000be30: 7468 6f6e 2f73 6f75 6e64 6465 7669 6365  thon/sounddevice
-0000be40: 2f66 756e 6374 696f 6e73 2f73 6f75 6e64  /functions/sound
-0000be50: 6465 7669 6365 2e50 6f72 7441 7564 696f  device.PortAudio
-0000be60: 4572 726f 720a 2020 2020 2020 2020 2020  Error.          
-0000be70: 2020 2020 2020 6578 6365 7074 2073 642e        except sd.
-0000be80: 506f 7274 4175 6469 6f45 7272 6f72 2061  PortAudioError a
-0000be90: 7320 6572 723a 0a20 2020 2020 2020 2020  s err:.         
-0000bea0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000beb0: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
-0000bec0: 7b65 7272 7d22 290a 0a20 2020 2020 2020  {err}")..       
-0000bed0: 2020 2020 2020 2020 2073 656c 662e 7074           self.pt
-0000bee0: 745f 6f66 6628 290a 2020 2020 2020 2020  t_off().        
-0000bef0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000bf00: 2020 2073 656c 662e 7074 745f 6f6e 2829     self.ptt_on()
-0000bf10: 0a20 2020 2020 2020 2066 6f72 206c 6574  .        for let
-0000bf20: 7465 7220 696e 2074 6865 5f73 7472 696e  ter in the_strin
-0000bf30: 672e 6c6f 7765 7228 293a 0a20 2020 2020  g.lower():.     
-0000bf40: 2020 2020 2020 2069 6620 6c65 7474 6572         if letter
-0000bf50: 2069 6e20 2261 6263 6465 6667 6869 6a6b   in "abcdefghijk
-0000bf60: 6c6d 6e6f 7071 7273 7475 7677 7879 7a20  lmnopqrstuvwxyz 
-0000bf70: 3132 3334 3536 3738 3930 223a 0a20 2020  1234567890":.   
-0000bf80: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000bf90: 6c65 7474 6572 203d 3d20 2220 223a 0a20  letter == " ":. 
-0000bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfb0: 2020 206c 6574 7465 7220 3d20 2273 7061     letter = "spa
-0000bfc0: 6365 220a 2020 2020 2020 2020 2020 2020  ce".            
-0000bfd0: 2020 2020 6669 6c65 6e61 6d65 203d 2066      filename = f
-0000bfe0: 227b 7374 7228 6f70 5f70 6174 6829 7d2f  "{str(op_path)}/
-0000bff0: 7b6c 6574 7465 727d 2e77 6176 220a 2020  {letter}.wav".  
-0000c000: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000c010: 2050 6174 6828 6669 6c65 6e61 6d65 292e   Path(filename).
-0000c020: 6973 5f66 696c 6528 293a 0a20 2020 2020  is_file():.     
-0000c030: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000c040: 6f67 6765 722e 6465 6275 6728 2256 6f69  ogger.debug("Voi
-0000c050: 6369 6e67 3a20 2573 222c 2066 696c 656e  cing: %s", filen
-0000c060: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-0000c070: 2020 2020 2020 2020 2064 6174 612c 205f           data, _
-0000c080: 6673 203d 2073 662e 7265 6164 2866 696c  fs = sf.read(fil
-0000c090: 656e 616d 652c 2064 7479 7065 3d22 666c  ename, dtype="fl
-0000c0a0: 6f61 7433 3222 290a 2020 2020 2020 2020  oat32").        
-0000c0b0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-0000c0c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c0d0: 2020 2020 2020 2020 2073 642e 6465 6661           sd.defa
-0000c0e0: 756c 742e 6465 7669 6365 203d 2073 656c  ult.device = sel
-0000c0f0: 662e 7072 6566 2e67 6574 2822 736f 756e  f.pref.get("soun
-0000c100: 6464 6576 6963 6522 2c20 2264 6566 6175  ddevice", "defau
-0000c110: 6c74 2229 0a20 2020 2020 2020 2020 2020  lt").           
-0000c120: 2020 2020 2020 2020 2020 2020 2073 642e               sd.
-0000c130: 6465 6661 756c 742e 7361 6d70 6c65 7261  default.samplera
-0000c140: 7465 203d 2034 3431 3030 2e30 0a20 2020  te = 44100.0.   
-0000c150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c160: 2020 2020 2073 642e 706c 6179 2864 6174       sd.play(dat
-0000c170: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
-0000c180: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000c190: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
-0000c1a0: 7b73 642e 7761 6974 2829 7d22 290a 2020  {sd.wait()}").  
-0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1c0: 2020 6578 6365 7074 2073 642e 506f 7274    except sd.Port
-0000c1d0: 4175 6469 6f45 7272 6f72 2061 7320 6572  AudioError as er
-0000c1e0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-0000c1f0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000c200: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
-0000c210: 7b65 7272 7d22 290a 2020 2020 2020 2020  {err}").        
-0000c220: 7365 6c66 2e70 7474 5f6f 6666 2829 0a0a  self.ptt_off()..
-0000c230: 2020 2020 6465 6620 7074 745f 6f6e 2873      def ptt_on(s
-0000c240: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000c250: 2274 7572 6e20 6f6e 2070 7474 2222 220a  "turn on ptt""".
-0000c260: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000c270: 7269 675f 636f 6e74 726f 6c3a 0a20 2020  rig_control:.   
-0000c280: 2020 2020 2020 2020 2073 656c 662e 6c65           self.le
-0000c290: 6674 646f 742e 7365 7450 6978 6d61 7028  ftdot.setPixmap(
-0000c2a0: 7365 6c66 2e67 7265 656e 646f 7429 0a20  self.greendot). 
-0000c2b0: 2020 2020 2020 2020 2020 2061 7070 2e70             app.p
-0000c2c0: 726f 6365 7373 4576 656e 7473 2829 0a20  rocessEvents(). 
-0000c2d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c2e0: 7269 675f 636f 6e74 726f 6c2e 7074 745f  rig_control.ptt_
-0000c2f0: 6f6e 2829 0a0a 2020 2020 6465 6620 7074  on()..    def pt
-0000c300: 745f 6f66 6628 7365 6c66 293a 0a20 2020  t_off(self):.   
-0000c310: 2020 2020 2022 2222 7475 726e 206f 6666       """turn off
-0000c320: 2070 7474 2222 220a 2020 2020 2020 2020   ptt""".        
-0000c330: 7365 6c66 2e6c 6566 7464 6f74 2e73 6574  self.leftdot.set
-0000c340: 5069 786d 6170 2873 656c 662e 7265 6464  Pixmap(self.redd
-0000c350: 6f74 290a 2020 2020 2020 2020 6170 702e  ot).        app.
-0000c360: 7072 6f63 6573 7345 7665 6e74 7328 290a  processEvents().
-0000c370: 2020 2020 2020 2020 7365 6c66 2e72 6967          self.rig
-0000c380: 5f63 6f6e 7472 6f6c 2e70 7474 5f6f 6666  _control.ptt_off
-0000c390: 2829 0a0a 2020 2020 6465 6620 7365 6e64  ()..    def send
-0000c3a0: 6631 2873 656c 6629 3a0a 2020 2020 2020  f1(self):.      
-0000c3b0: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000c3c0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000c3d0: 6728 2246 3120 436c 6963 6b65 6422 290a  g("F1 Clicked").
-0000c3e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000c3f0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
-0000c400: 226d 6f64 6522 2920 696e 205b 2255 5342  "mode") in ["USB
-0000c410: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
-0000c420: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
-0000c430: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
-0000c440: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
-0000c450: 2e46 312e 746f 6f6c 5469 7028 2929 290a  .F1.toolTip())).
-0000c460: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c470: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
-0000c480: 6c66 2e63 773a 0a20 2020 2020 2020 2020  lf.cw:.         
-0000c490: 2020 2023 2069 6620 7365 6c66 2e70 7265     # if self.pre
-0000c4a0: 6665 7265 6e63 652e 6765 7428 2273 656e  ference.get("sen
-0000c4b0: 645f 6e31 6d6d 5f70 6163 6b65 7473 2229  d_n1mm_packets")
-0000c4c0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-0000c4d0: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
-0000c4e0: 6469 6f5f 696e 666f 5b22 4675 6e63 7469  dio_info["Functi
-0000c4f0: 6f6e 4b65 7943 6170 7469 6f6e 225d 203d  onKeyCaption"] =
-0000c500: 2073 656c 662e 4631 2e74 6578 7428 290a   self.F1.text().
-0000c510: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c520: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
-0000c530: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
-0000c540: 6c66 2e46 312e 746f 6f6c 5469 7028 2929  lf.F1.toolTip())
-0000c550: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
-0000c560: 3228 7365 6c66 293a 0a20 2020 2020 2020  2(self):.       
-0000c570: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
-0000c580: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000c590: 2822 4632 2043 6c69 636b 6564 2229 0a20  ("F2 Clicked"). 
-0000c5a0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0000c5b0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-0000c5c0: 6d6f 6465 2229 2069 6e20 5b22 5553 4222  mode") in ["USB"
-0000c5d0: 2c20 2253 5342 225d 3a0a 2020 2020 2020  , "SSB"]:.      
-0000c5e0: 2020 2020 2020 7365 6c66 2e76 6f69 6365        self.voice
-0000c5f0: 5f73 7472 696e 6728 7365 6c66 2e70 726f  _string(self.pro
-0000c600: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
-0000c610: 4632 2e74 6f6f 6c54 6970 2829 2929 0a20  F2.toolTip())). 
-0000c620: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000c630: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
-0000c640: 662e 6377 3a0a 2020 2020 2020 2020 2020  f.cw:.          
-0000c650: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
-0000c660: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
-0000c670: 6372 6f28 7365 6c66 2e46 322e 746f 6f6c  cro(self.F2.tool
-0000c680: 5469 7028 2929 290a 0a20 2020 2064 6566  Tip()))..    def
-0000c690: 2073 656e 6466 3328 7365 6c66 293a 0a20   sendf3(self):. 
-0000c6a0: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
-0000c6b0: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-0000c6c0: 2e64 6562 7567 2822 4633 2043 6c69 636b  .debug("F3 Click
-0000c6d0: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
-0000c6e0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-0000c6f0: 2e67 6574 2822 6d6f 6465 2229 2069 6e20  .get("mode") in 
-0000c700: 5b22 5553 4222 2c20 2253 5342 225d 3a0a  ["USB", "SSB"]:.
-0000c710: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c720: 2e76 6f69 6365 5f73 7472 696e 6728 7365  .voice_string(se
-0000c730: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
-0000c740: 2873 656c 662e 4633 2e74 6f6f 6c54 6970  (self.F3.toolTip
-0000c750: 2829 2929 0a20 2020 2020 2020 2020 2020  ())).           
-0000c760: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000c770: 6966 2073 656c 662e 6377 3a0a 2020 2020  if self.cw:.    
-0000c780: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
-0000c790: 7365 6e64 6377 2873 656c 662e 7072 6f63  sendcw(self.proc
-0000c7a0: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
-0000c7b0: 332e 746f 6f6c 5469 7028 2929 290a 0a20  3.toolTip())).. 
-0000c7c0: 2020 2064 6566 2073 656e 6466 3428 7365     def sendf4(se
-0000c7d0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000c7e0: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
-0000c7f0: 6c6f 6767 6572 2e64 6562 7567 2822 4634  logger.debug("F4
-0000c800: 2043 6c69 636b 6564 2229 0a20 2020 2020   Clicked").     
-0000c810: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
-0000c820: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
-0000c830: 2229 2069 6e20 5b22 5553 4222 2c20 2253  ") in ["USB", "S
-0000c840: 5342 225d 3a0a 2020 2020 2020 2020 2020  SB"]:.          
-0000c850: 2020 7365 6c66 2e76 6f69 6365 5f73 7472    self.voice_str
-0000c860: 696e 6728 7365 6c66 2e70 726f 6365 7373  ing(self.process
-0000c870: 5f6d 6163 726f 2873 656c 662e 4634 2e74  _macro(self.F4.t
-0000c880: 6f6f 6c54 6970 2829 2929 0a20 2020 2020  oolTip())).     
-0000c890: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0000c8a0: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
-0000c8b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000c8c0: 6c66 2e63 772e 7365 6e64 6377 2873 656c  lf.cw.sendcw(sel
-0000c8d0: 662e 7072 6f63 6573 735f 6d61 6372 6f28  f.process_macro(
-0000c8e0: 7365 6c66 2e46 342e 746f 6f6c 5469 7028  self.F4.toolTip(
-0000c8f0: 2929 290a 0a20 2020 2064 6566 2073 656e  )))..    def sen
-0000c900: 6466 3528 7365 6c66 293a 0a20 2020 2020  df5(self):.     
-0000c910: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
-0000c920: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000c930: 7567 2822 4635 2043 6c69 636b 6564 2229  ug("F5 Clicked")
-0000c940: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000c950: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-0000c960: 2822 6d6f 6465 2229 2069 6e20 5b22 5553  ("mode") in ["US
-0000c970: 4222 2c20 2253 5342 225d 3a0a 2020 2020  B", "SSB"]:.    
-0000c980: 2020 2020 2020 2020 7365 6c66 2e76 6f69          self.voi
-0000c990: 6365 5f73 7472 696e 6728 7365 6c66 2e70  ce_string(self.p
-0000c9a0: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
-0000c9b0: 662e 4635 2e74 6f6f 6c54 6970 2829 2929  f.F5.toolTip()))
-0000c9c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000c9d0: 7572 6e0a 2020 2020 2020 2020 6966 2073  urn.        if s
-0000c9e0: 656c 662e 6377 3a0a 2020 2020 2020 2020  elf.cw:.        
-0000c9f0: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
-0000ca00: 6377 2873 656c 662e 7072 6f63 6573 735f  cw(self.process_
-0000ca10: 6d61 6372 6f28 7365 6c66 2e46 352e 746f  macro(self.F5.to
-0000ca20: 6f6c 5469 7028 2929 290a 0a20 2020 2064  olTip()))..    d
-0000ca30: 6566 2073 656e 6466 3628 7365 6c66 293a  ef sendf6(self):
-0000ca40: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
-0000ca50: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
-0000ca60: 6572 2e64 6562 7567 2822 4636 2043 6c69  er.debug("F6 Cli
-0000ca70: 636b 6564 2229 0a20 2020 2020 2020 2069  cked").        i
-0000ca80: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
-0000ca90: 7465 2e67 6574 2822 6d6f 6465 2229 2069  te.get("mode") i
-0000caa0: 6e20 5b22 5553 4222 2c20 2253 5342 225d  n ["USB", "SSB"]
-0000cab0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000cac0: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
-0000cad0: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
-0000cae0: 726f 2873 656c 662e 4636 2e74 6f6f 6c54  ro(self.F6.toolT
-0000caf0: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
-0000cb00: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-0000cb10: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
-0000cb20: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000cb30: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
-0000cb40: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
-0000cb50: 2e46 362e 746f 6f6c 5469 7028 2929 290a  .F6.toolTip())).
-0000cb60: 0a20 2020 2064 6566 2073 656e 6466 3728  .    def sendf7(
-0000cb70: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000cb80: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
-0000cb90: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-0000cba0: 4637 2043 6c69 636b 6564 2229 0a20 2020  F7 Clicked").   
-0000cbb0: 2020 2020 2069 6620 7365 6c66 2e72 6164       if self.rad
-0000cbc0: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
-0000cbd0: 6465 2229 2069 6e20 5b22 5553 4222 2c20  de") in ["USB", 
-0000cbe0: 2253 5342 225d 3a0a 2020 2020 2020 2020  "SSB"]:.        
-0000cbf0: 2020 2020 7365 6c66 2e76 6f69 6365 5f73      self.voice_s
-0000cc00: 7472 696e 6728 7365 6c66 2e70 726f 6365  tring(self.proce
-0000cc10: 7373 5f6d 6163 726f 2873 656c 662e 4637  ss_macro(self.F7
-0000cc20: 2e74 6f6f 6c54 6970 2829 2929 0a20 2020  .toolTip())).   
-0000cc30: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000cc40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000cc50: 6377 3a0a 2020 2020 2020 2020 2020 2020  cw:.            
-0000cc60: 7365 6c66 2e63 772e 7365 6e64 6377 2873  self.cw.sendcw(s
-0000cc70: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
-0000cc80: 6f28 7365 6c66 2e46 372e 746f 6f6c 5469  o(self.F7.toolTi
-0000cc90: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
-0000cca0: 656e 6466 3828 7365 6c66 293a 0a20 2020  endf8(self):.   
-0000ccb0: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
-0000ccc0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000ccd0: 6562 7567 2822 4638 2043 6c69 636b 6564  ebug("F8 Clicked
-0000cce0: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
-0000ccf0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-0000cd00: 6574 2822 6d6f 6465 2229 2069 6e20 5b22  et("mode") in ["
-0000cd10: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
-0000cd20: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-0000cd30: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
-0000cd40: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000cd50: 656c 662e 4638 2e74 6f6f 6c54 6970 2829  elf.F8.toolTip()
-0000cd60: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
-0000cd70: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-0000cd80: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
-0000cd90: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
-0000cda0: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
-0000cdb0: 735f 6d61 6372 6f28 7365 6c66 2e46 382e  s_macro(self.F8.
-0000cdc0: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
-0000cdd0: 2064 6566 2073 656e 6466 3928 7365 6c66   def sendf9(self
-0000cde0: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
-0000cdf0: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
-0000ce00: 6767 6572 2e64 6562 7567 2822 4639 2043  gger.debug("F9 C
-0000ce10: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
-0000ce20: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
-0000ce30: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
-0000ce40: 2069 6e20 5b22 5553 4222 2c20 2253 5342   in ["USB", "SSB
-0000ce50: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-0000ce60: 7365 6c66 2e76 6f69 6365 5f73 7472 696e  self.voice_strin
-0000ce70: 6728 7365 6c66 2e70 726f 6365 7373 5f6d  g(self.process_m
-0000ce80: 6163 726f 2873 656c 662e 4639 2e74 6f6f  acro(self.F9.too
-0000ce90: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
-0000cea0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000ceb0: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
-0000cec0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ced0: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
-0000cee0: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
-0000cef0: 6c66 2e46 392e 746f 6f6c 5469 7028 2929  lf.F9.toolTip())
-0000cf00: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
-0000cf10: 3130 2873 656c 6629 3a0a 2020 2020 2020  10(self):.      
-0000cf20: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000cf30: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000cf40: 6728 2246 3130 2043 6c69 636b 6564 2229  g("F10 Clicked")
-0000cf50: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000cf60: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-0000cf70: 2822 6d6f 6465 2229 2069 6e20 5b22 5553  ("mode") in ["US
-0000cf80: 4222 2c20 2253 5342 225d 3a0a 2020 2020  B", "SSB"]:.    
-0000cf90: 2020 2020 2020 2020 7365 6c66 2e76 6f69          self.voi
-0000cfa0: 6365 5f73 7472 696e 6728 7365 6c66 2e70  ce_string(self.p
-0000cfb0: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
-0000cfc0: 662e 4631 302e 746f 6f6c 5469 7028 2929  f.F10.toolTip())
-0000cfd0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-0000cfe0: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
-0000cff0: 7365 6c66 2e63 773a 0a20 2020 2020 2020  self.cw:.       
-0000d000: 2020 2020 2073 656c 662e 6377 2e73 656e       self.cw.sen
-0000d010: 6463 7728 7365 6c66 2e70 726f 6365 7373  dcw(self.process
-0000d020: 5f6d 6163 726f 2873 656c 662e 4631 302e  _macro(self.F10.
-0000d030: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
-0000d040: 2064 6566 2073 656e 6466 3131 2873 656c   def sendf11(sel
-0000d050: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000d060: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000d070: 6f67 6765 722e 6465 6275 6728 2246 3131  ogger.debug("F11
-0000d080: 2043 6c69 636b 6564 2229 0a20 2020 2020   Clicked").     
-0000d090: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
-0000d0a0: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
-0000d0b0: 2229 2069 6e20 5b22 5553 4222 2c20 2253  ") in ["USB", "S
-0000d0c0: 5342 225d 3a0a 2020 2020 2020 2020 2020  SB"]:.          
-0000d0d0: 2020 7365 6c66 2e76 6f69 6365 5f73 7472    self.voice_str
-0000d0e0: 696e 6728 7365 6c66 2e70 726f 6365 7373  ing(self.process
-0000d0f0: 5f6d 6163 726f 2873 656c 662e 4631 312e  _macro(self.F11.
-0000d100: 746f 6f6c 5469 7028 2929 290a 2020 2020  toolTip())).    
-0000d110: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-0000d120: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0000d130: 773a 0a20 2020 2020 2020 2020 2020 2073  w:.            s
-0000d140: 656c 662e 6377 2e73 656e 6463 7728 7365  elf.cw.sendcw(se
-0000d150: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
-0000d160: 2873 656c 662e 4631 312e 746f 6f6c 5469  (self.F11.toolTi
-0000d170: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
-0000d180: 656e 6466 3132 2873 656c 6629 3a0a 2020  endf12(self):.  
-0000d190: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
-0000d1a0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000d1b0: 6465 6275 6728 2246 3132 2043 6c69 636b  debug("F12 Click
-0000d1c0: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
-0000d1d0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-0000d1e0: 2e67 6574 2822 6d6f 6465 2229 2069 6e20  .get("mode") in 
-0000d1f0: 5b22 5553 4222 2c20 2253 5342 225d 3a0a  ["USB", "SSB"]:.
-0000d200: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d210: 2e76 6f69 6365 5f73 7472 696e 6728 7365  .voice_string(se
-0000d220: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
-0000d230: 2873 656c 662e 4631 322e 746f 6f6c 5469  (self.F12.toolTi
-0000d240: 7028 2929 290a 2020 2020 2020 2020 2020  p())).          
-0000d250: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-0000d260: 2069 6620 7365 6c66 2e63 773a 0a20 2020   if self.cw:.   
-0000d270: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
-0000d280: 2e73 656e 6463 7728 7365 6c66 2e70 726f  .sendcw(self.pro
-0000d290: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
-0000d2a0: 4631 322e 746f 6f6c 5469 7028 2929 290a  F12.toolTip())).
-0000d2b0: 0a20 2020 2064 6566 2072 756e 5f73 705f  .    def run_sp_
-0000d2c0: 6275 7474 6f6e 735f 636c 6963 6b65 6428  buttons_clicked(
-0000d2d0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000d2e0: 2222 4861 6e64 6c65 2072 756e 2f73 2670  ""Handle run/s&p
-0000d2f0: 206d 6f64 6522 2222 0a20 2020 2020 2020   mode""".       
-0000d300: 2073 656c 662e 7072 6566 5b22 7275 6e5f   self.pref["run_
-0000d310: 7374 6174 6522 5d20 3d20 7365 6c66 2e72  state"] = self.r
-0000d320: 6164 696f 4275 7474 6f6e 5f72 756e 2e69  adioButton_run.i
-0000d330: 7343 6865 636b 6564 2829 0a20 2020 2020  sChecked().     
-0000d340: 2020 2073 656c 662e 7772 6974 655f 7072     self.write_pr
-0000d350: 6566 6572 656e 6365 2829 0a20 2020 2020  eference().     
-0000d360: 2020 2073 656c 662e 7265 6164 5f63 775f     self.read_cw_
-0000d370: 6d61 6372 6f73 2829 0a0a 2020 2020 6465  macros()..    de
-0000d380: 6620 7772 6974 655f 7072 6566 6572 656e  f write_preferen
-0000d390: 6365 2873 656c 6629 3a0a 2020 2020 2020  ce(self):.      
-0000d3a0: 2020 2222 220a 2020 2020 2020 2020 5772    """.        Wr
-0000d3b0: 6974 6520 7072 6566 6572 656e 6365 7320  ite preferences 
-0000d3c0: 746f 206a 736f 6e20 6669 6c65 2e0a 2020  to json file..  
-0000d3d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000d3e0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-0000d3f0: 2020 2077 6974 6820 6f70 656e 280a 2020     with open(.  
-0000d400: 2020 2020 2020 2020 2020 2020 2020 434f                CO
-0000d410: 4e46 4947 5f50 4154 4820 2b20 222f 6e6f  NFIG_PATH + "/no
-0000d420: 7431 6d6d 2e6a 736f 6e22 2c20 2277 7422  t1mm.json", "wt"
-0000d430: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
-0000d440: 3822 0a20 2020 2020 2020 2020 2020 2029  8".            )
-0000d450: 2061 7320 6669 6c65 5f64 6573 6372 6970   as file_descrip
-0000d460: 746f 723a 0a20 2020 2020 2020 2020 2020  tor:.           
-0000d470: 2020 2020 2066 696c 655f 6465 7363 7269       file_descri
-0000d480: 7074 6f72 2e77 7269 7465 2864 756d 7073  ptor.write(dumps
-0000d490: 2873 656c 662e 7072 6566 2c20 696e 6465  (self.pref, inde
-0000d4a0: 6e74 3d34 2929 0a20 2020 2020 2020 2020  nt=4)).         
-0000d4b0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-0000d4c0: 666f 2822 7772 6974 696e 673a 2025 7322  fo("writing: %s"
-0000d4d0: 2c20 7365 6c66 2e70 7265 6629 0a20 2020  , self.pref).   
-0000d4e0: 2020 2020 2065 7863 6570 7420 494f 4572       except IOEr
-0000d4f0: 726f 7220 6173 2065 7863 6570 7469 6f6e  ror as exception
-0000d500: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-0000d510: 6767 6572 2e63 7269 7469 6361 6c28 2277  gger.critical("w
-0000d520: 7269 7465 7072 6566 6572 656e 6365 733a  ritepreferences:
-0000d530: 2025 7322 2c20 6578 6365 7074 696f 6e29   %s", exception)
-0000d540: 0a0a 2020 2020 6465 6620 7265 6164 7072  ..    def readpr
-0000d550: 6566 6572 656e 6365 7328 7365 6c66 293a  eferences(self):
-0000d560: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000d570: 2020 2020 2052 6573 746f 7265 2070 7265       Restore pre
-0000d580: 6665 7265 6e63 6573 2069 6620 7468 6579  ferences if they
-0000d590: 2065 7869 7374 2c20 6f74 6865 7277 6973   exist, otherwis
-0000d5a0: 6520 6372 6561 7465 2073 6f6d 6520 7361  e create some sa
-0000d5b0: 6e65 2064 6566 6175 6c74 732e 0a20 2020  ne defaults..   
-0000d5c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000d5d0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0000d5e0: 2020 6966 206f 732e 7061 7468 2e65 7869    if os.path.exi
-0000d5f0: 7374 7328 434f 4e46 4947 5f50 4154 4820  sts(CONFIG_PATH 
-0000d600: 2b20 222f 6e6f 7431 6d6d 2e6a 736f 6e22  + "/not1mm.json"
-0000d610: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000d620: 2020 2077 6974 6820 6f70 656e 280a 2020     with open(.  
-0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d640: 2020 434f 4e46 4947 5f50 4154 4820 2b20    CONFIG_PATH + 
-0000d650: 222f 6e6f 7431 6d6d 2e6a 736f 6e22 2c20  "/not1mm.json", 
-0000d660: 2272 7422 2c20 656e 636f 6469 6e67 3d22  "rt", encoding="
-0000d670: 7574 662d 3822 0a20 2020 2020 2020 2020  utf-8".         
-0000d680: 2020 2020 2020 2029 2061 7320 6669 6c65         ) as file
-0000d690: 5f64 6573 6372 6970 746f 723a 0a20 2020  _descriptor:.   
-0000d6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6b0: 2073 656c 662e 7072 6566 203d 206c 6f61   self.pref = loa
-0000d6c0: 6473 2866 696c 655f 6465 7363 7269 7074  ds(file_descript
-0000d6d0: 6f72 2e72 6561 6428 2929 0a20 2020 2020  or.read()).     
-0000d6e0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000d6f0: 6f67 6765 722e 696e 666f 2822 2573 222c  ogger.info("%s",
-0000d700: 2073 656c 662e 7072 6566 290a 2020 2020   self.pref).    
-0000d710: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000d720: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000d730: 6767 6572 2e69 6e66 6f28 224e 6f20 7072  gger.info("No pr
-0000d740: 6566 6572 656e 6365 2066 696c 652e 2057  eference file. W
-0000d750: 7269 7469 6e67 2070 7265 6665 7265 6e63  riting preferenc
-0000d760: 652e 2229 0a20 2020 2020 2020 2020 2020  e.").           
-0000d770: 2020 2020 2077 6974 6820 6f70 656e 280a       with open(.
-0000d780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d790: 2020 2020 434f 4e46 4947 5f50 4154 4820      CONFIG_PATH 
-0000d7a0: 2b20 222f 6e6f 7431 6d6d 2e6a 736f 6e22  + "/not1mm.json"
-0000d7b0: 2c20 2277 7422 2c20 656e 636f 6469 6e67  , "wt", encoding
-0000d7c0: 3d22 7574 662d 3822 0a20 2020 2020 2020  ="utf-8".       
-0000d7d0: 2020 2020 2020 2020 2029 2061 7320 6669           ) as fi
-0000d7e0: 6c65 5f64 6573 6372 6970 746f 723a 0a20  le_descriptor:. 
-0000d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d800: 2020 2073 656c 662e 7072 6566 203d 2073     self.pref = s
-0000d810: 656c 662e 7072 6566 5f72 6566 2e63 6f70  elf.pref_ref.cop
-0000d820: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-0000d830: 2020 2020 2020 2020 6669 6c65 5f64 6573          file_des
-0000d840: 6372 6970 746f 722e 7772 6974 6528 6475  criptor.write(du
-0000d850: 6d70 7328 7365 6c66 2e70 7265 662c 2069  mps(self.pref, i
-0000d860: 6e64 656e 743d 3429 290a 2020 2020 2020  ndent=4)).      
-0000d870: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000d880: 6767 6572 2e69 6e66 6f28 2225 7322 2c20  gger.info("%s", 
-0000d890: 7365 6c66 2e70 7265 6629 0a20 2020 2020  self.pref).     
-0000d8a0: 2020 2065 7863 6570 7420 494f 4572 726f     except IOErro
-0000d8b0: 7220 6173 2065 7863 6570 7469 6f6e 3a0a  r as exception:.
-0000d8c0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000d8d0: 6572 2e63 7269 7469 6361 6c28 2245 7272  er.critical("Err
-0000d8e0: 6f72 3a20 2573 222c 2065 7863 6570 7469  or: %s", excepti
-0000d8f0: 6f6e 290a 0a20 2020 2020 2020 2073 656c  on)..        sel
-0000d900: 662e 6c6f 6f6b 5f75 7020 3d20 4e6f 6e65  f.look_up = None
-0000d910: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000d920: 2e70 7265 662e 6765 7428 2275 7365 7172  .pref.get("useqr
-0000d930: 7a22 293a 0a20 2020 2020 2020 2020 2020  z"):.           
-0000d940: 2073 656c 662e 6c6f 6f6b 5f75 7020 3d20   self.look_up = 
-0000d950: 5152 5a6c 6f6f 6b75 7028 0a20 2020 2020  QRZlookup(.     
-0000d960: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d970: 7072 6566 2e67 6574 2822 6c6f 6f6b 7570  pref.get("lookup
-0000d980: 7573 6572 6e61 6d65 2229 2c0a 2020 2020  username"),.    
-0000d990: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d9a0: 2e70 7265 662e 6765 7428 226c 6f6f 6b75  .pref.get("looku
-0000d9b0: 7070 6173 7377 6f72 6422 292c 0a20 2020  ppassword"),.   
-0000d9c0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000d9d0: 2020 2023 2069 6620 7365 6c66 2e70 7265     # if self.pre
-0000d9e0: 662e 6765 7428 2275 7365 6861 6d64 6222  f.get("usehamdb"
-0000d9f0: 293a 0a20 2020 2020 2020 2023 2020 2020  ):.        #    
-0000da00: 2073 656c 662e 6c6f 6f6b 5f75 7020 3d20   self.look_up = 
-0000da10: 4861 6d44 426c 6f6f 6b75 7028 290a 2020  HamDBlookup().  
-0000da20: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-0000da30: 6566 2e67 6574 2822 7573 6568 616d 7174  ef.get("usehamqt
-0000da40: 6822 293a 0a20 2020 2020 2020 2020 2020  h"):.           
-0000da50: 2073 656c 662e 6c6f 6f6b 5f75 7020 3d20   self.look_up = 
-0000da60: 4861 6d51 5448 280a 2020 2020 2020 2020  HamQTH(.        
-0000da70: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
-0000da80: 662e 6765 7428 226c 6f6f 6b75 7075 7365  f.get("lookupuse
-0000da90: 726e 616d 6522 292c 0a20 2020 2020 2020  rname"),.       
-0000daa0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000dab0: 6566 2e67 6574 2822 6c6f 6f6b 7570 7061  ef.get("lookuppa
-0000dac0: 7373 776f 7264 2229 2c0a 2020 2020 2020  ssword"),.      
-0000dad0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000dae0: 2069 6620 7365 6c66 2e70 7265 662e 6765   if self.pref.ge
-0000daf0: 7428 2272 756e 5f73 7461 7465 2229 3a0a  t("run_state"):.
-0000db00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000db10: 2e72 6164 696f 4275 7474 6f6e 5f72 756e  .radioButton_run
-0000db20: 2e73 6574 4368 6563 6b65 6428 5472 7565  .setChecked(True
-0000db30: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000db40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000db50: 2e72 6164 696f 4275 7474 6f6e 5f73 702e  .radioButton_sp.
-0000db60: 7365 7443 6865 636b 6564 2854 7275 6529  setChecked(True)
-0000db70: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-0000db80: 662e 7072 6566 2e67 6574 2822 6461 726b  f.pref.get("dark
-0000db90: 5f6d 6f64 6522 293a 0a20 2020 2020 2020  _mode"):.       
-0000dba0: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-0000dbb0: 4461 726b 5f4d 6f64 652e 7365 7443 6865  Dark_Mode.setChe
-0000dbc0: 636b 6564 2854 7275 6529 0a20 2020 2020  cked(True).     
-0000dbd0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000dbe0: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-0000dbf0: 4461 726b 5f4d 6f64 652e 7365 7443 6865  Dark_Mode.setChe
-0000dc00: 636b 6564 2846 616c 7365 290a 0a20 2020  cked(False)..   
-0000dc10: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
-0000dc20: 662e 6765 7428 2263 6f6d 6d61 6e64 5f62  f.get("command_b
-0000dc30: 7574 746f 6e73 2229 3a0a 2020 2020 2020  uttons"):.      
-0000dc40: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-0000dc50: 6e43 6f6d 6d61 6e64 5f42 7574 746f 6e73  nCommand_Buttons
-0000dc60: 2e73 6574 4368 6563 6b65 6428 5472 7565  .setChecked(True
-0000dc70: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000dc80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000dc90: 2e61 6374 696f 6e43 6f6d 6d61 6e64 5f42  .actionCommand_B
-0000dca0: 7574 746f 6e73 2e73 6574 4368 6563 6b65  uttons.setChecke
-0000dcb0: 6428 4661 6c73 6529 0a0a 2020 2020 2020  d(False)..      
-0000dcc0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
-0000dcd0: 6574 2822 6377 5f6d 6163 726f 7322 293a  et("cw_macros"):
-0000dce0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000dcf0: 662e 6163 7469 6f6e 4357 5f4d 6163 726f  f.actionCW_Macro
-0000dd00: 732e 7365 7443 6865 636b 6564 2854 7275  s.setChecked(Tru
-0000dd10: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
-0000dd20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000dd30: 662e 6163 7469 6f6e 4357 5f4d 6163 726f  f.actionCW_Macro
-0000dd40: 732e 7365 7443 6865 636b 6564 2846 616c  s.setChecked(Fal
-0000dd50: 7365 290a 0a20 2020 2020 2020 2069 6620  se)..        if 
-0000dd60: 7365 6c66 2e70 7265 662e 6765 7428 2262  self.pref.get("b
-0000dd70: 616e 6473 5f6d 6f64 6573 2229 3a0a 2020  ands_modes"):.  
-0000dd80: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000dd90: 6374 696f 6e4d 6f64 655f 616e 645f 4261  ctionMode_and_Ba
-0000dda0: 6e64 732e 7365 7443 6865 636b 6564 2854  nds.setChecked(T
-0000ddb0: 7275 6529 0a20 2020 2020 2020 2065 6c73  rue).        els
-0000ddc0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000ddd0: 656c 662e 6163 7469 6f6e 4d6f 6465 5f61  elf.actionMode_a
-0000dde0: 6e64 5f42 616e 6473 2e73 6574 4368 6563  nd_Bands.setChec
-0000ddf0: 6b65 6428 4661 6c73 6529 0a0a 2020 2020  ked(False)..    
-0000de00: 2020 2020 6d75 6c74 6963 6173 745f 6772      multicast_gr
-0000de10: 6f75 7020 3d20 7365 6c66 2e70 7265 662e  oup = self.pref.
-0000de20: 6765 7428 226d 756c 7469 6361 7374 5f67  get("multicast_g
-0000de30: 726f 7570 222c 2022 3232 342e 312e 312e  roup", "224.1.1.
-0000de40: 3122 290a 2020 2020 2020 2020 6d75 6c74  1").        mult
-0000de50: 6963 6173 745f 706f 7274 203d 2073 656c  icast_port = sel
-0000de60: 662e 7072 6566 2e67 6574 2822 6d75 6c74  f.pref.get("mult
-0000de70: 6963 6173 745f 706f 7274 222c 2032 3233  icast_port", 223
-0000de80: 3929 0a20 2020 2020 2020 2069 6e74 6572  9).        inter
-0000de90: 6661 6365 5f69 7020 3d20 7365 6c66 2e70  face_ip = self.p
-0000dea0: 7265 662e 6765 7428 2269 6e74 6572 6661  ref.get("interfa
-0000deb0: 6365 5f69 7022 2c20 2230 2e30 2e30 2e30  ce_ip", "0.0.0.0
-0000dec0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000ded0: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
-0000dee0: 6163 6520 3d20 4d75 6c74 6963 6173 7428  ace = Multicast(
-0000def0: 0a20 2020 2020 2020 2020 2020 206d 756c  .            mul
-0000df00: 7469 6361 7374 5f67 726f 7570 2c20 6d75  ticast_group, mu
-0000df10: 6c74 6963 6173 745f 706f 7274 2c20 696e  lticast_port, in
-0000df20: 7465 7266 6163 655f 6970 0a20 2020 2020  terface_ip.     
-0000df30: 2020 2029 0a0a 2020 2020 2020 2020 7365     )..        se
-0000df40: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 203d  lf.rig_control =
-0000df50: 204e 6f6e 650a 0a20 2020 2020 2020 2069   None..        i
-0000df60: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
-0000df70: 2275 7365 666c 7269 6722 2c20 4661 6c73  "useflrig", Fals
-0000df80: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-0000df90: 6c6f 6767 6572 2e64 6562 7567 280a 2020  logger.debug(.  
-0000dfa0: 2020 2020 2020 2020 2020 2020 2020 2255                "U
-0000dfb0: 7369 6e67 2066 6c72 6967 3a20 2573 222c  sing flrig: %s",
-0000dfc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dfd0: 2066 227b 7365 6c66 2e70 7265 662e 6765   f"{self.pref.ge
-0000dfe0: 7428 2743 4154 5f69 7027 297d 207b 7365  t('CAT_ip')} {se
-0000dff0: 6c66 2e70 7265 662e 6765 7428 2743 4154  lf.pref.get('CAT
-0000e000: 5f70 6f72 7427 297d 222c 0a20 2020 2020  _port')}",.     
-0000e010: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000e020: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
-0000e030: 6e74 726f 6c20 3d20 4341 5428 0a20 2020  ntrol = CAT(.   
-0000e040: 2020 2020 2020 2020 2020 2020 2022 666c               "fl
-0000e050: 7269 6722 2c0a 2020 2020 2020 2020 2020  rig",.          
-0000e060: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
-0000e070: 6765 7428 2243 4154 5f69 7022 2c20 2231  get("CAT_ip", "1
-0000e080: 3237 2e30 2e30 2e31 2229 2c0a 2020 2020  27.0.0.1"),.    
-0000e090: 2020 2020 2020 2020 2020 2020 696e 7428              int(
-0000e0a0: 7365 6c66 2e70 7265 662e 6765 7428 2243  self.pref.get("C
-0000e0b0: 4154 5f70 6f72 7422 2c20 3132 3334 3529  AT_port", 12345)
-0000e0c0: 292c 0a20 2020 2020 2020 2020 2020 2029  ),.            )
-0000e0d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000e0e0: 2e70 7265 662e 6765 7428 2275 7365 7269  .pref.get("useri
-0000e0f0: 6763 746c 6422 2c20 4661 6c73 6529 3a0a  gctld", False):.
-0000e100: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000e110: 6572 2e64 6562 7567 280a 2020 2020 2020  er.debug(.      
-0000e120: 2020 2020 2020 2020 2020 2255 7369 6e67            "Using
-0000e130: 2072 6967 6374 6c64 3a20 2573 222c 0a20   rigctld: %s",. 
-0000e140: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000e150: 227b 7365 6c66 2e70 7265 662e 6765 7428  "{self.pref.get(
-0000e160: 2743 4154 5f69 7027 297d 207b 7365 6c66  'CAT_ip')} {self
-0000e170: 2e70 7265 662e 6765 7428 2743 4154 5f70  .pref.get('CAT_p
-0000e180: 6f72 7427 297d 222c 0a20 2020 2020 2020  ort')}",.       
-0000e190: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000e1a0: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
-0000e1b0: 726f 6c20 3d20 4341 5428 0a20 2020 2020  rol = CAT(.     
-0000e1c0: 2020 2020 2020 2020 2020 2022 7269 6763             "rigc
-0000e1d0: 746c 6422 2c0a 2020 2020 2020 2020 2020  tld",.          
-0000e1e0: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
-0000e1f0: 6765 7428 2243 4154 5f69 7022 2c20 2231  get("CAT_ip", "1
-0000e200: 3237 2e30 2e30 2e31 2229 2c0a 2020 2020  27.0.0.1"),.    
-0000e210: 2020 2020 2020 2020 2020 2020 696e 7428              int(
-0000e220: 7365 6c66 2e70 7265 662e 6765 7428 2243  self.pref.get("C
-0000e230: 4154 5f70 6f72 7422 2c20 3435 3332 2929  AT_port", 4532))
-0000e240: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000e250: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000e260: 2e70 7265 662e 6765 7428 2263 7774 7970  .pref.get("cwtyp
-0000e270: 6522 2c20 3029 203d 3d20 303a 0a20 2020  e", 0) == 0:.   
-0000e280: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
-0000e290: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000e2a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000e2b0: 2020 7365 6c66 2e63 7720 3d20 4357 280a    self.cw = CW(.
-0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2d0: 696e 7428 7365 6c66 2e70 7265 662e 6765  int(self.pref.ge
-0000e2e0: 7428 2263 7774 7970 6522 2929 2c0a 2020  t("cwtype")),.  
-0000e2f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e300: 6c66 2e70 7265 662e 6765 7428 2263 7769  lf.pref.get("cwi
-0000e310: 7022 292c 0a20 2020 2020 2020 2020 2020  p"),.           
-0000e320: 2020 2020 2069 6e74 2873 656c 662e 7072       int(self.pr
-0000e330: 6566 2e67 6574 2822 6377 706f 7274 222c  ef.get("cwport",
-0000e340: 2036 3738 3929 292c 0a20 2020 2020 2020   6789)),.       
-0000e350: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000e360: 2020 2073 656c 662e 6377 2e73 7065 6564     self.cw.speed
-0000e370: 203d 2032 300a 0a20 2020 2020 2020 2073   = 20..        s
-0000e380: 656c 662e 6461 726b 5f6d 6f64 6528 290a  elf.dark_mode().
-0000e390: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
-0000e3a0: 775f 636f 6d6d 616e 645f 6275 7474 6f6e  w_command_button
-0000e3b0: 7328 290a 2020 2020 2020 2020 7365 6c66  s().        self
-0000e3c0: 2e73 686f 775f 4357 5f6d 6163 726f 7328  .show_CW_macros(
-0000e3d0: 290a 2020 2020 2020 2020 2320 7365 6c66  ).        # self
-0000e3e0: 2e73 686f 775f 6261 6e64 5f6d 6f64 6528  .show_band_mode(
-0000e3f0: 290a 0a20 2020 2064 6566 2077 6174 6368  )..    def watch
-0000e400: 5f75 6470 2873 656c 6629 3a0a 2020 2020  _udp(self):.    
-0000e410: 2020 2020 2222 2250 7574 7320 5544 5020      """Puts UDP 
-0000e420: 6461 7461 6772 616d 7320 696e 2061 2046  datagrams in a F
-0000e430: 4946 4f20 7175 6575 6522 2222 0a20 2020  IFO queue""".   
-0000e440: 2020 2020 2077 6869 6c65 2054 7275 653a       while True:
-0000e450: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-0000e460: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e470: 2020 6461 7461 6772 616d 203d 2073 656c    datagram = sel
-0000e480: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
-0000e490: 7266 6163 652e 7365 7276 6572 5f75 6470  rface.server_udp
-0000e4a0: 2e72 6563 7628 3135 3030 290a 2020 2020  .recv(1500).    
-0000e4b0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000e4c0: 6572 2e64 6562 7567 2864 6174 6167 7261  er.debug(datagra
-0000e4d0: 6d2e 6465 636f 6465 2829 290a 2020 2020  m.decode()).    
-0000e4e0: 2020 2020 2020 2020 6578 6365 7074 2073          except s
-0000e4f0: 6f63 6b65 742e 7469 6d65 6f75 743a 0a20  ocket.timeout:. 
-0000e500: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000e510: 696d 652e 736c 6565 7028 302e 3129 0a20  ime.sleep(0.1). 
-0000e520: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000e530: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-0000e540: 2020 2020 6966 2064 6174 6167 7261 6d3a      if datagram:
-0000e550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e560: 2073 656c 662e 7564 705f 6669 666f 2e70   self.udp_fifo.p
-0000e570: 7574 2864 6174 6167 7261 6d29 0a0a 2020  ut(datagram)..  
-0000e580: 2020 6465 6620 6368 6563 6b5f 7564 705f    def check_udp_
-0000e590: 7472 6166 6669 6328 7365 6c66 293a 0a20  traffic(self):. 
-0000e5a0: 2020 2020 2020 2022 2222 4368 6563 6b73         """Checks
-0000e5b0: 2055 4450 2054 7261 6666 6963 2222 220a   UDP Traffic""".
-0000e5c0: 2020 2020 2020 2020 7768 696c 6520 6e6f          while no
-0000e5d0: 7420 7365 6c66 2e75 6470 5f66 6966 6f2e  t self.udp_fifo.
-0000e5e0: 656d 7074 7928 293a 0a20 2020 2020 2020  empty():.       
-0000e5f0: 2020 2020 2064 6174 6167 7261 6d20 3d20       datagram = 
-0000e600: 7365 6c66 2e75 6470 5f66 6966 6f2e 6765  self.udp_fifo.ge
-0000e610: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-0000e620: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0000e630: 2020 2020 2064 6562 7567 5f69 6e66 6f20       debug_info 
-0000e640: 3d20 6622 7b64 6174 6167 7261 6d2e 6465  = f"{datagram.de
-0000e650: 636f 6465 2829 7d22 0a20 2020 2020 2020  code()}".       
-0000e660: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-0000e670: 6465 6275 6728 6465 6275 675f 696e 666f  debug(debug_info
-0000e680: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e690: 2020 6a73 6f6e 5f64 6174 6120 3d20 6c6f    json_data = lo
-0000e6a0: 6164 7328 6461 7461 6772 616d 2e64 6563  ads(datagram.dec
-0000e6b0: 6f64 6528 2929 0a20 2020 2020 2020 2020  ode()).         
-0000e6c0: 2020 2065 7863 6570 7420 556e 6963 6f64     except Unicod
-0000e6d0: 6544 6563 6f64 6545 7272 6f72 2061 7320  eDecodeError as 
-0000e6e0: 6572 723a 0a20 2020 2020 2020 2020 2020  err:.           
-0000e6f0: 2020 2020 2074 6865 5f65 7272 6f72 203d       the_error =
-0000e700: 2066 224e 6f74 2055 6e69 636f 6465 3a20   f"Not Unicode: 
-0000e710: 7b65 7272 7d5c 6e7b 6461 7461 6772 616d  {err}\n{datagram
-0000e720: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-0000e730: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000e740: 7468 655f 6572 726f 7229 0a20 2020 2020  the_error).     
-0000e750: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-0000e760: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
-0000e770: 6578 6365 7074 204a 534f 4e44 6563 6f64  except JSONDecod
-0000e780: 6545 7272 6f72 2061 7320 6572 723a 0a20  eError as err:. 
-0000e790: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000e7a0: 6865 5f65 7272 6f72 203d 2066 224e 6f74  he_error = f"Not
-0000e7b0: 204a 534f 4e3a 207b 6572 727d 5c6e 7b64   JSON: {err}\n{d
-0000e7c0: 6174 6167 7261 6d7d 220a 2020 2020 2020  atagram}".      
-0000e7d0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000e7e0: 2e64 6562 7567 2874 6865 5f65 7272 6f72  .debug(the_error
-0000e7f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e800: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-0000e810: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
-0000e820: 2020 2020 2020 2020 2020 2020 6a73 6f6e              json
-0000e830: 5f64 6174 612e 6765 7428 2263 6d64 222c  _data.get("cmd",
-0000e840: 2022 2229 203d 3d20 2247 4554 434f 4c55   "") == "GETCOLU
-0000e850: 4d4e 5322 0a20 2020 2020 2020 2020 2020  MNS".           
-0000e860: 2020 2020 2061 6e64 206a 736f 6e5f 6461       and json_da
-0000e870: 7461 2e67 6574 2822 7374 6174 696f 6e22  ta.get("station"
-0000e880: 2c20 2222 2920 3d3d 2070 6c61 7466 6f72  , "") == platfor
-0000e890: 6d2e 6e6f 6465 2829 0a20 2020 2020 2020  m.node().       
-0000e8a0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-0000e8b0: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
-0000e8c0: 7472 2873 656c 662e 636f 6e74 6573 742c  tr(self.contest,
-0000e8d0: 2022 636f 6c75 6d6e 7322 293a 0a20 2020   "columns"):.   
-0000e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8f0: 2063 6d64 203d 207b 7d0a 2020 2020 2020   cmd = {}.      
-0000e900: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-0000e910: 645b 2263 6d64 225d 203d 2022 5348 4f57  d["cmd"] = "SHOW
-0000e920: 434f 4c55 4d4e 5322 0a20 2020 2020 2020  COLUMNS".       
-0000e930: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-0000e940: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
-0000e950: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
-0000e960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e970: 2020 636d 645b 2243 4f4c 554d 4e53 225d    cmd["COLUMNS"]
-0000e980: 203d 2073 656c 662e 636f 6e74 6573 742e   = self.contest.
-0000e990: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
-0000e9a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e9b0: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
-0000e9c0: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
-0000e9d0: 6e28 636d 6429 0a20 2020 2020 2020 2020  n(cmd).         
-0000e9e0: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-0000e9f0: 2020 2020 2020 2020 6a73 6f6e 5f64 6174          json_dat
-0000ea00: 612e 6765 7428 2263 6d64 222c 2022 2229  a.get("cmd", "")
-0000ea10: 203d 3d20 2254 554e 4522 0a20 2020 2020   == "TUNE".     
-0000ea20: 2020 2020 2020 2020 2020 2061 6e64 206a             and j
-0000ea30: 736f 6e5f 6461 7461 2e67 6574 2822 7374  son_data.get("st
-0000ea40: 6174 696f 6e22 2c20 2222 2920 3d3d 2070  ation", "") == p
-0000ea50: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
-0000ea60: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-0000ea70: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000ea80: 6227 7b22 636d 6422 3a20 2254 554e 4522  b'{"cmd": "TUNE"
-0000ea90: 2c20 2266 7265 7122 3a20 372e 3032 3335  , "freq": 7.0235
-0000eaa0: 2c20 2273 706f 7422 3a20 224d 4d30 4447  , "spot": "MM0DG
-0000eab0: 4922 7d27 0a20 2020 2020 2020 2020 2020  I"}'.           
-0000eac0: 2020 2020 2076 666f 203d 206a 736f 6e5f       vfo = json_
-0000ead0: 6461 7461 2e67 6574 2822 6672 6571 2229  data.get("freq")
-0000eae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eaf0: 2076 666f 203d 2066 6c6f 6174 2876 666f   vfo = float(vfo
-0000eb00: 2920 2a20 3130 3030 3030 300a 2020 2020  ) * 1000000.    
-0000eb10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000eb20: 2e72 6164 696f 5f73 7461 7465 5b22 7666  .radio_state["vf
-0000eb30: 6f61 225d 203d 2069 6e74 2876 666f 290a  oa"] = int(vfo).
-0000eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb50: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
-0000eb60: 726f 6c3a 0a20 2020 2020 2020 2020 2020  rol:.           
-0000eb70: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
-0000eb80: 675f 636f 6e74 726f 6c2e 7365 745f 7666  g_control.set_vf
-0000eb90: 6f28 696e 7428 7666 6f29 290a 2020 2020  o(int(vfo)).    
-0000eba0: 2020 2020 2020 2020 2020 2020 7370 6f74              spot
-0000ebb0: 203d 206a 736f 6e5f 6461 7461 2e67 6574   = json_data.get
-0000ebc0: 2822 7370 6f74 222c 2022 2229 0a20 2020  ("spot", "").   
-0000ebd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ebe0: 662e 6361 6c6c 7369 676e 2e73 6574 5465  f.callsign.setTe
-0000ebf0: 7874 2873 706f 7429 0a20 2020 2020 2020  xt(spot).       
-0000ec00: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
-0000ec10: 6c6c 7369 676e 5f63 6861 6e67 6564 2829  llsign_changed()
-0000ec20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ec30: 2073 656c 662e 6361 6c6c 7369 676e 2e73   self.callsign.s
-0000ec40: 6574 466f 6375 7328 290a 2020 2020 2020  etFocus().      
-0000ec50: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000ec60: 616c 6c73 6967 6e2e 6163 7469 7661 7465  allsign.activate
-0000ec70: 5769 6e64 6f77 2829 0a20 2020 2020 2020  Window().       
-0000ec80: 2020 2020 2020 2020 2077 696e 646f 772e           window.
-0000ec90: 7261 6973 655f 2829 0a0a 2020 2020 6465  raise_()..    de
-0000eca0: 6620 6461 726b 5f6d 6f64 655f 7374 6174  f dark_mode_stat
-0000ecb0: 655f 6368 616e 6765 2873 656c 6629 3a0a  e_change(self):.
-0000ecc0: 2020 2020 2020 2020 2222 2264 6172 6b6d          """darkm
-0000ecd0: 6f64 6520 6472 6f70 646f 776e 2063 6865  ode dropdown che
-0000ece0: 636b 6d61 726b 2063 6861 6e67 6564 2222  ckmark changed""
-0000ecf0: 220a 2020 2020 2020 2020 7365 6c66 2e70  ".        self.p
-0000ed00: 7265 665b 2264 6172 6b5f 6d6f 6465 225d  ref["dark_mode"]
-0000ed10: 203d 2073 656c 662e 6163 7469 6f6e 4461   = self.actionDa
-0000ed20: 726b 5f4d 6f64 652e 6973 4368 6563 6b65  rk_Mode.isChecke
-0000ed30: 6428 290a 2020 2020 2020 2020 7365 6c66  d().        self
-0000ed40: 2e77 7269 7465 5f70 7265 6665 7265 6e63  .write_preferenc
-0000ed50: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
-0000ed60: 2e64 6172 6b5f 6d6f 6465 2829 0a0a 2020  .dark_mode()..  
-0000ed70: 2020 6465 6620 6461 726b 5f6d 6f64 6528    def dark_mode(
-0000ed80: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000ed90: 2222 6368 616e 6765 2064 6973 706c 6179  ""change display
-0000eda0: 206d 6f64 6522 2222 0a20 2020 2020 2020   mode""".       
-0000edb0: 2069 6620 7365 6c66 2e70 7265 662e 6765   if self.pref.ge
-0000edc0: 7428 2264 6172 6b5f 6d6f 6465 2229 3a0a  t("dark_mode"):.
-0000edd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ede0: 2e73 6574 5374 796c 6553 6865 6574 2844  .setStyleSheet(D
-0000edf0: 4152 4b5f 5354 594c 4553 4845 4554 290a  ARK_STYLESHEET).
-0000ee00: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000ee10: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000ee20: 6574 5374 796c 6553 6865 6574 2822 2229  etStyleSheet("")
-0000ee30: 0a0a 2020 2020 6465 6620 6377 5f6d 6163  ..    def cw_mac
-0000ee40: 726f 735f 7374 6174 655f 6368 616e 6765  ros_state_change
-0000ee50: 6428 7365 6c66 293a 0a20 2020 2020 2020  d(self):.       
-0000ee60: 2022 2222 4d65 6e75 2069 7465 6d20 746f   """Menu item to
-0000ee70: 2073 686f 772f 6869 6465 206d 6163 726f   show/hide macro
-0000ee80: 2062 7574 746f 6e73 2222 220a 2020 2020   buttons""".    
-0000ee90: 2020 2020 7365 6c66 2e70 7265 665b 2263      self.pref["c
-0000eea0: 775f 6d61 6372 6f73 225d 203d 2073 656c  w_macros"] = sel
-0000eeb0: 662e 6163 7469 6f6e 4357 5f4d 6163 726f  f.actionCW_Macro
-0000eec0: 732e 6973 4368 6563 6b65 6428 290a 2020  s.isChecked().  
-0000eed0: 2020 2020 2020 7365 6c66 2e77 7269 7465        self.write
-0000eee0: 5f70 7265 6665 7265 6e63 6528 290a 2020  _preference().  
-0000eef0: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
-0000ef00: 4357 5f6d 6163 726f 7328 290a 0a20 2020  CW_macros()..   
-0000ef10: 2064 6566 2073 686f 775f 4357 5f6d 6163   def show_CW_mac
-0000ef20: 726f 7328 7365 6c66 293a 0a20 2020 2020  ros(self):.     
-0000ef30: 2020 2022 2222 6d61 6372 6f20 6275 7474     """macro butt
-0000ef40: 6f6e 2073 7461 7465 2063 6861 6e67 6522  on state change"
-0000ef50: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
-0000ef60: 6c66 2e70 7265 662e 6765 7428 2263 775f  lf.pref.get("cw_
-0000ef70: 6d61 6372 6f73 2229 3a0a 2020 2020 2020  macros"):.      
-0000ef80: 2020 2020 2020 7365 6c66 2e42 7574 746f        self.Butto
-0000ef90: 6e5f 526f 7731 2e73 686f 7728 290a 2020  n_Row1.show().  
-0000efa0: 2020 2020 2020 2020 2020 7365 6c66 2e42            self.B
-0000efb0: 7574 746f 6e5f 526f 7732 2e73 686f 7728  utton_Row2.show(
-0000efc0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000efd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000efe0: 2e42 7574 746f 6e5f 526f 7731 2e68 6964  .Button_Row1.hid
-0000eff0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-0000f000: 7365 6c66 2e42 7574 746f 6e5f 526f 7732  self.Button_Row2
-0000f010: 2e68 6964 6528 290a 0a20 2020 2064 6566  .hide()..    def
-0000f020: 2063 6f6d 6d61 6e64 5f62 7574 746f 6e73   command_buttons
-0000f030: 5f73 7461 7465 5f63 6861 6e67 6528 7365  _state_change(se
-0000f040: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000f050: 4d65 6e75 2069 7465 6d20 746f 2073 686f  Menu item to sho
-0000f060: 772f 6869 6465 2063 6f6d 6d61 6e64 2062  w/hide command b
-0000f070: 7574 746f 6e73 2222 220a 2020 2020 2020  uttons""".      
-0000f080: 2020 7365 6c66 2e70 7265 665b 2263 6f6d    self.pref["com
-0000f090: 6d61 6e64 5f62 7574 746f 6e73 225d 203d  mand_buttons"] =
-0000f0a0: 2073 656c 662e 6163 7469 6f6e 436f 6d6d   self.actionComm
-0000f0b0: 616e 645f 4275 7474 6f6e 732e 6973 4368  and_Buttons.isCh
-0000f0c0: 6563 6b65 6428 290a 2020 2020 2020 2020  ecked().        
-0000f0d0: 7365 6c66 2e77 7269 7465 5f70 7265 6665  self.write_prefe
-0000f0e0: 7265 6e63 6528 290a 2020 2020 2020 2020  rence().        
-0000f0f0: 7365 6c66 2e73 686f 775f 636f 6d6d 616e  self.show_comman
-0000f100: 645f 6275 7474 6f6e 7328 290a 0a20 2020  d_buttons()..   
-0000f110: 2064 6566 2073 686f 775f 636f 6d6d 616e   def show_comman
-0000f120: 645f 6275 7474 6f6e 7328 7365 6c66 293a  d_buttons(self):
-0000f130: 0a20 2020 2020 2020 2022 2222 636f 6d6d  .        """comm
-0000f140: 616e 6420 6275 7474 6f6e 2073 7461 7465  and button state
-0000f150: 2063 6861 6e67 6522 2222 0a20 2020 2020   change""".     
-0000f160: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
-0000f170: 6765 7428 2263 6f6d 6d61 6e64 5f62 7574  get("command_but
-0000f180: 746f 6e73 2229 3a0a 2020 2020 2020 2020  tons"):.        
-0000f190: 2020 2020 7365 6c66 2e43 6f6d 6d61 6e64      self.Command
-0000f1a0: 5f42 7574 746f 6e73 2e73 686f 7728 290a  _Buttons.show().
-0000f1b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000f1c0: 2020 2020 2020 2020 2020 7365 6c66 2e43            self.C
-0000f1d0: 6f6d 6d61 6e64 5f42 7574 746f 6e73 2e68  ommand_Buttons.h
-0000f1e0: 6964 6528 290a 0a20 2020 2064 6566 2069  ide()..    def i
-0000f1f0: 735f 666c 6f61 7461 626c 6528 7365 6c66  s_floatable(self
-0000f200: 2c20 6974 656d 3a20 7374 7229 202d 3e20  , item: str) -> 
-0000f210: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-0000f220: 2263 6865 636b 2074 6f20 7365 6520 6966  "check to see if
-0000f230: 2073 7472 696e 6720 6361 6e20 6265 2061   string can be a
-0000f240: 2066 6c6f 6174 2222 220a 2020 2020 2020   float""".      
-0000f250: 2020 6966 2069 7465 6d2e 6973 6e75 6d65    if item.isnume
-0000f260: 7269 6328 293a 0a20 2020 2020 2020 2020  ric():.         
-0000f270: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-0000f280: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-0000f290: 2020 2020 2020 2020 5f74 6573 7420 3d20          _test = 
-0000f2a0: 666c 6f61 7428 6974 656d 290a 2020 2020  float(item).    
-0000f2b0: 2020 2020 6578 6365 7074 2056 616c 7565      except Value
-0000f2c0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
-0000f2d0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-0000f2e0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0000f2f0: 7275 650a 0a20 2020 2064 6566 206f 7468  rue..    def oth
-0000f300: 6572 5f32 5f63 6861 6e67 6564 2873 656c  er_2_changed(sel
-0000f310: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
-0000f320: 616c 6c65 6420 7768 656e 2077 6520 6e65  alled when we ne
-0000f330: 6564 2074 6f20 7061 7273 6520 5353 2065  ed to parse SS e
-0000f340: 7863 6861 6e67 652e 2222 220a 2020 2020  xchange.""".    
-0000f350: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
-0000f360: 6573 743a 0a20 2020 2020 2020 2020 2020  est:.           
-0000f370: 2069 6620 2241 5252 4c20 5377 6565 7073   if "ARRL Sweeps
-0000f380: 7461 6b65 7322 2069 6e20 7365 6c66 2e63  takes" in self.c
-0000f390: 6f6e 7465 7374 2e6e 616d 653a 0a20 2020  ontest.name:.   
-0000f3a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f3b0: 662e 636f 6e74 6573 742e 7061 7273 655f  f.contest.parse_
-0000f3c0: 6578 6368 616e 6765 2873 656c 6629 0a0a  exchange(self)..
-0000f3d0: 2020 2020 6465 6620 6361 6c6c 7369 676e      def callsign
-0000f3e0: 5f63 6861 6e67 6564 2873 656c 6629 3a0a  _changed(self):.
-0000f3f0: 2020 2020 2020 2020 2222 2243 616c 6c65          """Calle
-0000f400: 6420 7768 656e 2074 6578 7420 696e 2074  d when text in t
-0000f410: 6865 2063 616c 6c73 6967 6e20 6669 656c  he callsign fiel
-0000f420: 6420 6861 7320 6368 616e 6765 6422 2222  d has changed"""
-0000f430: 0a20 2020 2020 2020 2074 6578 7420 3d20  .        text = 
-0000f440: 7365 6c66 2e63 616c 6c73 6967 6e2e 7465  self.callsign.te
-0000f450: 7874 2829 0a20 2020 2020 2020 2074 6578  xt().        tex
-0000f460: 7420 3d20 7465 7874 2e75 7070 6572 2829  t = text.upper()
-0000f470: 0a20 2020 2020 2020 2070 6f73 6974 696f  .        positio
-0000f480: 6e20 3d20 7365 6c66 2e63 616c 6c73 6967  n = self.callsig
-0000f490: 6e2e 6375 7273 6f72 506f 7369 7469 6f6e  n.cursorPosition
-0000f4a0: 2829 0a20 2020 2020 2020 2073 7472 6970  ().        strip
-0000f4b0: 7065 645f 7465 7874 203d 2074 6578 742e  ped_text = text.
-0000f4c0: 7374 7269 7028 292e 7265 706c 6163 6528  strip().replace(
-0000f4d0: 2220 222c 2022 2229 0a20 2020 2020 2020  " ", "").       
-0000f4e0: 2073 656c 662e 6361 6c6c 7369 676e 2e73   self.callsign.s
-0000f4f0: 6574 5465 7874 2873 7472 6970 7065 645f  etText(stripped_
-0000f500: 7465 7874 290a 2020 2020 2020 2020 7365  text).        se
-0000f510: 6c66 2e63 616c 6c73 6967 6e2e 7365 7443  lf.callsign.setC
-0000f520: 7572 736f 7250 6f73 6974 696f 6e28 706f  ursorPosition(po
-0000f530: 7369 7469 6f6e 290a 0a20 2020 2020 2020  sition)..       
-0000f540: 2069 6620 2220 2220 696e 2074 6578 743a   if " " in text:
-0000f550: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000f560: 7374 7269 7070 6564 5f74 6578 7420 3d3d  stripped_text ==
-0000f570: 2022 4357 223a 0a20 2020 2020 2020 2020   "CW":.         
-0000f580: 2020 2020 2020 2073 656c 662e 7365 746d         self.setm
-0000f590: 6f64 6528 2243 5722 290a 2020 2020 2020  ode("CW").      
-0000f5a0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000f5b0: 6164 696f 5f73 7461 7465 5b22 6d6f 6465  adio_state["mode
-0000f5c0: 225d 203d 2022 4357 220a 2020 2020 2020  "] = "CW".      
-0000f5d0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000f5e0: 662e 7269 675f 636f 6e74 726f 6c3a 0a20  f.rig_control:. 
-0000f5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f600: 2020 2069 6620 7365 6c66 2e72 6967 5f63     if self.rig_c
-0000f610: 6f6e 7472 6f6c 2e6f 6e6c 696e 653a 0a20  ontrol.online:. 
-0000f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f630: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
-0000f640: 636f 6e74 726f 6c2e 7365 745f 6d6f 6465  control.set_mode
-0000f650: 2822 4357 2229 0a20 2020 2020 2020 2020  ("CW").         
-0000f660: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
-0000f670: 7769 6e64 6f77 5f74 6974 6c65 2829 0a20  window_title(). 
-0000f680: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f690: 656c 662e 636c 6561 7269 6e70 7574 7328  elf.clearinputs(
-0000f6a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f6b0: 2020 7365 6c66 2e72 6561 645f 6377 5f6d    self.read_cw_m
-0000f6c0: 6163 726f 7328 290a 2020 2020 2020 2020  acros().        
-0000f6d0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-0000f6e0: 2020 2020 2020 2020 2020 2069 6620 7374             if st
-0000f6f0: 7269 7070 6564 5f74 6578 7420 3d3d 2022  ripped_text == "
-0000f700: 5254 5459 223a 0a20 2020 2020 2020 2020  RTTY":.         
-0000f710: 2020 2020 2020 2073 656c 662e 7365 746d         self.setm
-0000f720: 6f64 6528 2252 5454 5922 290a 2020 2020  ode("RTTY").    
-0000f730: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000f740: 656c 662e 7269 675f 636f 6e74 726f 6c3a  elf.rig_control:
-0000f750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f760: 2020 2020 2069 6620 7365 6c66 2e72 6967       if self.rig
-0000f770: 5f63 6f6e 7472 6f6c 2e6f 6e6c 696e 653a  _control.online:
-0000f780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f790: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
-0000f7a0: 675f 636f 6e74 726f 6c2e 7365 745f 6d6f  g_control.set_mo
-0000f7b0: 6465 2822 5254 5459 2229 0a20 2020 2020  de("RTTY").     
-0000f7c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000f7d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000f7e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f7f0: 662e 7261 6469 6f5f 7374 6174 655b 226d  f.radio_state["m
-0000f800: 6f64 6522 5d20 3d20 2252 5454 5922 0a20  ode"] = "RTTY". 
-0000f810: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f820: 656c 662e 7365 745f 7769 6e64 6f77 5f74  elf.set_window_t
-0000f830: 6974 6c65 2829 0a20 2020 2020 2020 2020  itle().         
-0000f840: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
-0000f850: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
-0000f860: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000f870: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000f880: 7374 7269 7070 6564 5f74 6578 7420 3d3d  stripped_text ==
-0000f890: 2022 5353 4222 3a0a 2020 2020 2020 2020   "SSB":.        
-0000f8a0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000f8b0: 6d6f 6465 2822 5353 4222 290a 2020 2020  mode("SSB").    
-0000f8c0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0000f8d0: 6e74 2873 656c 662e 7261 6469 6f5f 7374  nt(self.radio_st
-0000f8e0: 6174 652e 6765 7428 2276 666f 6122 2c20  ate.get("vfoa", 
-0000f8f0: 3029 2920 3e20 3130 3030 3030 3030 3a0a  0)) > 10000000:.
-0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f910: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
-0000f920: 7461 7465 5b22 6d6f 6465 225d 203d 2022  tate["mode"] = "
-0000f930: 5553 4222 0a20 2020 2020 2020 2020 2020  USB".           
-0000f940: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000f950: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f960: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
-0000f970: 226d 6f64 6522 5d20 3d20 224c 5342 220a  "mode"] = "LSB".
-0000f980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f990: 7365 6c66 2e73 6574 5f77 696e 646f 775f  self.set_window_
-0000f9a0: 7469 746c 6528 290a 2020 2020 2020 2020  title().        
-0000f9b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f9c0: 7269 675f 636f 6e74 726f 6c3a 0a20 2020  rig_control:.   
-0000f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9e0: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
-0000f9f0: 6c2e 7365 745f 6d6f 6465 2873 656c 662e  l.set_mode(self.
-0000fa00: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
-0000fa10: 226d 6f64 6522 2929 0a20 2020 2020 2020  "mode")).       
-0000fa20: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
-0000fa30: 6561 7269 6e70 7574 7328 290a 2020 2020  earinputs().    
-0000fa40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fa50: 2e72 6561 645f 6377 5f6d 6163 726f 7328  .read_cw_macros(
-0000fa60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000fa70: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-0000fa80: 2020 2020 2069 6620 7374 7269 7070 6564       if stripped
-0000fa90: 5f74 6578 7420 3d3d 2022 4f50 4f4e 223a  _text == "OPON":
-0000faa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fab0: 2073 656c 662e 6765 745f 6f70 6f6e 2829   self.get_opon()
-0000fac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fad0: 2073 656c 662e 636c 6561 7269 6e70 7574   self.clearinput
-0000fae0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-0000faf0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000fb00: 2020 2020 2020 2069 6620 7374 7269 7070         if stripp
-0000fb10: 6564 5f74 6578 7420 3d3d 2022 5445 5354  ed_text == "TEST
-0000fb20: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-0000fb30: 2020 2073 656c 662e 7368 6f77 5f6d 6573     self.show_mes
-0000fb40: 7361 6765 5f62 6f78 2822 5468 6973 2069  sage_box("This i
-0000fb50: 7320 6120 7465 7374 2229 0a20 2020 2020  s a test").     
-0000fb60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fb70: 636c 6561 7269 6e70 7574 7328 290a 2020  clearinputs().  
-0000fb80: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000fb90: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-0000fba0: 2069 6620 7365 6c66 2e69 735f 666c 6f61   if self.is_floa
-0000fbb0: 7461 626c 6528 7374 7269 7070 6564 5f74  table(stripped_t
-0000fbc0: 6578 7429 3a0a 2020 2020 2020 2020 2020  ext):.          
-0000fbd0: 2020 2020 2020 7666 6f20 3d20 666c 6f61        vfo = floa
-0000fbe0: 7428 7374 7269 7070 6564 5f74 6578 7429  t(stripped_text)
-0000fbf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fc00: 2076 666f 203d 2069 6e74 2876 666f 202a   vfo = int(vfo *
-0000fc10: 2031 3030 3029 0a20 2020 2020 2020 2020   1000).         
-0000fc20: 2020 2020 2020 2062 616e 6420 3d20 6765         band = ge
-0000fc30: 7462 616e 6428 7374 7228 7666 6f29 290a  tband(str(vfo)).
-0000fc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc50: 7365 6c66 2e73 6574 5f62 616e 645f 696e  self.set_band_in
-0000fc60: 6469 6361 746f 7228 6261 6e64 290a 2020  dicator(band).  
-0000fc70: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000fc80: 7365 6c66 2e63 6f6e 7461 6374 5b22 4261  self.contact["Ba
-0000fc90: 6e64 225d 203d 2067 6574 5f6c 6f67 6765  nd"] = get_logge
-0000fca0: 645f 6261 6e64 2873 7472 2873 656c 662e  d_band(str(self.
-0000fcb0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
-0000fcc0: 2276 666f 6122 2c20 302e 3029 2929 0a20  "vfoa", 0.0))). 
-0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fce0: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
-0000fcf0: 2276 666f 6122 5d20 3d20 7666 6f0a 2020  "vfoa"] = vfo.  
-0000fd00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fd10: 6c66 2e73 6574 5f77 696e 646f 775f 7469  lf.set_window_ti
-0000fd20: 746c 6528 290a 2020 2020 2020 2020 2020  tle().          
-0000fd30: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
-0000fd40: 696e 7075 7473 2829 0a20 2020 2020 2020  inputs().       
-0000fd50: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000fd60: 2e72 6967 5f63 6f6e 7472 6f6c 3a0a 2020  .rig_control:.  
-0000fd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd80: 2020 7365 6c66 2e72 6967 5f63 6f6e 7472    self.rig_contr
-0000fd90: 6f6c 2e73 6574 5f76 666f 2876 666f 290a  ol.set_vfo(vfo).
-0000fda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdb0: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
-0000fdc0: 2020 2020 7365 6c66 2e63 6865 636b 5f63      self.check_c
-0000fdd0: 616c 6c73 6967 6e28 7374 7269 7070 6564  allsign(stripped
-0000fde0: 5f74 6578 7429 0a20 2020 2020 2020 2020  _text).         
-0000fdf0: 2020 2069 6620 7365 6c66 2e63 6865 636b     if self.check
-0000fe00: 5f64 7570 6528 7374 7269 7070 6564 5f74  _dupe(stripped_t
-0000fe10: 6578 7429 3a0a 2020 2020 2020 2020 2020  ext):.          
-0000fe20: 2020 2020 2020 7365 6c66 2e64 7570 655f        self.dupe_
-0000fe30: 696e 6469 6361 746f 722e 7368 6f77 2829  indicator.show()
-0000fe40: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000fe50: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000fe60: 2020 2073 656c 662e 6475 7065 5f69 6e64     self.dupe_ind
-0000fe70: 6963 6174 6f72 2e68 6964 6528 290a 2020  icator.hide().  
-0000fe80: 2020 2020 2020 2020 2020 5f74 6865 7468            _theth
-0000fe90: 7265 6164 203d 2074 6872 6561 6469 6e67  read = threading
-0000fea0: 2e54 6872 6561 6428 0a20 2020 2020 2020  .Thread(.       
-0000feb0: 2020 2020 2020 2020 2074 6172 6765 743d           target=
-0000fec0: 7365 6c66 2e63 6865 636b 5f63 616c 6c73  self.check_calls
-0000fed0: 6967 6e32 2c0a 2020 2020 2020 2020 2020  ign2,.          
-0000fee0: 2020 2020 2020 6172 6773 3d28 7465 7874        args=(text
-0000fef0: 2c29 2c0a 2020 2020 2020 2020 2020 2020  ,),.            
-0000ff00: 2020 2020 6461 656d 6f6e 3d54 7275 652c      daemon=True,
-0000ff10: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000ff20: 2020 2020 2020 2020 2020 205f 7468 6574             _thet
-0000ff30: 6872 6561 642e 7374 6172 7428 290a 2020  hread.start().  
-0000ff40: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0000ff50: 6578 745f 6669 656c 642e 7365 7446 6f63  ext_field.setFoc
-0000ff60: 7573 2829 0a20 2020 2020 2020 2020 2020  us().           
-0000ff70: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000ff80: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
-0000ff90: 2063 6d64 5b22 636d 6422 5d20 3d20 2243   cmd["cmd"] = "C
-0000ffa0: 414c 4c43 4841 4e47 4544 220a 2020 2020  ALLCHANGED".    
-0000ffb0: 2020 2020 636d 645b 2273 7461 7469 6f6e      cmd["station
-0000ffc0: 225d 203d 2070 6c61 7466 6f72 6d2e 6e6f  "] = platform.no
-0000ffd0: 6465 2829 0a20 2020 2020 2020 2063 6d64  de().        cmd
-0000ffe0: 5b22 6361 6c6c 225d 203d 2073 7472 6970  ["call"] = strip
-0000fff0: 7065 645f 7465 7874 0a20 2020 2020 2020  ped_text.       
-00010000: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
-00010010: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
-00010020: 735f 6a73 6f6e 2863 6d64 290a 2020 2020  s_json(cmd).    
-00010030: 2020 2020 7365 6c66 2e63 6865 636b 5f63      self.check_c
-00010040: 616c 6c73 6967 6e28 7374 7269 7070 6564  allsign(stripped
-00010050: 5f74 6578 7429 0a0a 2020 2020 6465 6620  _text)..    def 
-00010060: 6368 6563 6b5f 6361 6c6c 7369 676e 2873  check_callsign(s
-00010070: 656c 662c 2063 616c 6c73 6967 6e29 3a0a  elf, callsign):.
-00010080: 2020 2020 2020 2020 2222 2243 6865 636b          """Check
-00010090: 2063 616c 6c20 6173 2065 6e74 6572 6564   call as entered
-000100a0: 2222 220a 2020 2020 2020 2020 7265 7375  """.        resu
-000100b0: 6c74 203d 2063 7479 5f6c 6f6f 6b75 7028  lt = cty_lookup(
-000100c0: 6361 6c6c 7369 676e 290a 2020 2020 2020  callsign).      
-000100d0: 2020 6465 6275 675f 7265 7375 6c74 203d    debug_result =
-000100e0: 2066 227b 7265 7375 6c74 7d22 0a20 2020   f"{result}".   
-000100f0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00010100: 6728 2225 7322 2c20 6465 6275 675f 7265  g("%s", debug_re
-00010110: 7375 6c74 290a 2020 2020 2020 2020 6966  sult).        if
-00010120: 2072 6573 756c 743a 0a20 2020 2020 2020   result:.       
-00010130: 2020 2020 2066 6f72 2061 2069 6e20 7265       for a in re
-00010140: 7375 6c74 2e69 7465 6d73 2829 3a0a 2020  sult.items():.  
-00010150: 2020 2020 2020 2020 2020 2020 2020 656e                en
-00010160: 7469 7479 203d 2061 5b31 5d2e 6765 7428  tity = a[1].get(
-00010170: 2265 6e74 6974 7922 2c20 2222 290a 2020  "entity", "").  
-00010180: 2020 2020 2020 2020 2020 2020 2020 6371                cq
-00010190: 203d 2061 5b31 5d2e 6765 7428 2263 7122   = a[1].get("cq"
-000101a0: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
-000101b0: 2020 2020 2020 6974 7520 3d20 615b 315d        itu = a[1]
-000101c0: 2e67 6574 2822 6974 7522 2c20 2222 290a  .get("itu", "").
-000101d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101e0: 636f 6e74 696e 656e 7420 3d20 615b 315d  continent = a[1]
-000101f0: 2e67 6574 2822 636f 6e74 696e 656e 7422  .get("continent"
-00010200: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010210: 2020 6c61 7420 3d20 666c 6f61 7428 615b    lat = float(a[
-00010220: 315d 2e67 6574 2822 6c61 7422 2c20 2230  1].get("lat", "0
-00010230: 2e30 2229 290a 2020 2020 2020 2020 2020  .0")).          
-00010240: 2020 2020 2020 6c6f 6e20 3d20 666c 6f61        lon = floa
-00010250: 7428 615b 315d 2e67 6574 2822 6c6f 6e67  t(a[1].get("long
-00010260: 222c 2022 302e 3022 2929 0a20 2020 2020  ", "0.0")).     
-00010270: 2020 2020 2020 2020 2020 206c 6f6e 203d             lon =
-00010280: 206c 6f6e 202a 202d 3120 2023 2063 7479   lon * -1  # cty
-00010290: 2e64 6174 2066 696c 6520 696e 7665 7274  .dat file invert
-000102a0: 7320 6c6f 6e67 6974 7564 6573 0a20 2020  s longitudes.   
-000102b0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000102c0: 6d61 7279 5f70 6678 203d 2061 5b31 5d2e  mary_pfx = a[1].
-000102d0: 6765 7428 2270 7269 6d61 7279 5f70 6678  get("primary_pfx
-000102e0: 222c 2022 2229 0a20 2020 2020 2020 2020  ", "").         
-000102f0: 2020 2020 2020 2068 6561 6469 6e67 203d         heading =
-00010300: 2062 6561 7269 6e67 5f77 6974 685f 6c61   bearing_with_la
-00010310: 746c 6f6e 2873 656c 662e 7374 6174 696f  tlon(self.statio
-00010320: 6e2e 6765 7428 2247 7269 6453 7175 6172  n.get("GridSquar
-00010330: 6522 292c 206c 6174 2c20 6c6f 6e29 0a20  e"), lat, lon). 
-00010340: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00010350: 696c 6f6d 6574 6572 7320 3d20 6469 7374  ilometers = dist
-00010360: 616e 6365 5f77 6974 685f 6c61 746c 6f6e  ance_with_latlon
-00010370: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00010380: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-00010390: 6f6e 2e67 6574 2822 4772 6964 5371 7561  on.get("GridSqua
-000103a0: 7265 2229 2c20 6c61 742c 206c 6f6e 0a20  re"), lat, lon. 
-000103b0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000103c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000103d0: 2073 656c 662e 6865 6164 696e 675f 6469   self.heading_di
-000103e0: 7374 616e 6365 2e73 6574 5465 7874 280a  stance.setText(.
-000103f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010400: 2020 2020 6622 5265 6769 6f6e 616c 2048      f"Regional H
-00010410: 6467 207b 6865 6164 696e 677d c2b0 204c  dg {heading}.. L
-00010420: 5020 7b72 6563 6970 726f 636f 6c28 6865  P {reciprocol(he
-00010430: 6164 696e 6729 7dc2 b020 2f20 220a 2020  ading)}.. / ".  
-00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010450: 2020 6622 6469 7374 616e 6365 207b 696e    f"distance {in
-00010460: 7428 6b69 6c6f 6d65 7465 7273 2a30 2e36  t(kilometers*0.6
-00010470: 3231 3337 3129 7d6d 6920 7b6b 696c 6f6d  21371)}mi {kilom
-00010480: 6574 6572 737d 6b6d 220a 2020 2020 2020  eters}km".      
-00010490: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000104a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000104b0: 2e63 6f6e 7461 6374 5b22 436f 756e 7472  .contact["Countr
-000104c0: 7950 7265 6669 7822 5d20 3d20 7072 696d  yPrefix"] = prim
-000104d0: 6172 795f 7066 780a 2020 2020 2020 2020  ary_pfx.        
-000104e0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000104f0: 7461 6374 5b22 5a4e 225d 203d 2069 6e74  tact["ZN"] = int
-00010500: 2863 7129 0a20 2020 2020 2020 2020 2020  (cq).           
-00010510: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-00010520: 745b 2243 6f6e 7469 6e65 6e74 225d 203d  t["Continent"] =
-00010530: 2063 6f6e 7469 6e65 6e74 0a20 2020 2020   continent.     
-00010540: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010550: 6478 5f65 6e74 6974 792e 7365 7454 6578  dx_entity.setTex
-00010560: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00010570: 2020 2020 2020 2066 227b 7072 696d 6172         f"{primar
-00010580: 795f 7066 787d 3a20 7b63 6f6e 7469 6e65  y_pfx}: {contine
-00010590: 6e74 7d2f 7b65 6e74 6974 797d 2063 713a  nt}/{entity} cq:
-000105a0: 7b63 717d 2069 7475 3a7b 6974 757d 220a  {cq} itu:{itu}".
-000105b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000105d0: 2020 6966 206c 656e 2863 616c 6c73 6967    if len(callsig
-000105e0: 6e29 203e 2032 3a0a 2020 2020 2020 2020  n) > 2:.        
-000105f0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00010600: 656c 662e 636f 6e74 6573 743a 0a20 2020  elf.contest:.   
-00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010620: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00010630: 742e 7072 6566 696c 6c28 7365 6c66 290a  t.prefill(self).
-00010640: 0a20 2020 2064 6566 2063 6865 636b 5f63  .    def check_c
-00010650: 616c 6c73 6967 6e32 2873 656c 662c 2063  allsign2(self, c
-00010660: 616c 6c73 6967 6e29 3a0a 2020 2020 2020  allsign):.      
-00010670: 2020 2222 2243 6865 636b 2063 616c 6c20    """Check call 
-00010680: 6f6e 6365 2065 6e74 6572 6564 2222 220a  once entered""".
-00010690: 2020 2020 2020 2020 6361 6c6c 7369 676e          callsign
-000106a0: 203d 2063 616c 6c73 6967 6e2e 7374 7269   = callsign.stri
-000106b0: 7028 290a 2020 2020 2020 2020 6465 6275  p().        debu
-000106c0: 675f 6c6f 6f6b 7570 203d 2066 227b 7365  g_lookup = f"{se
-000106d0: 6c66 2e6c 6f6f 6b5f 7570 7d22 0a20 2020  lf.look_up}".   
-000106e0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-000106f0: 6728 2225 732c 2025 7322 2c20 6361 6c6c  g("%s, %s", call
-00010700: 7369 676e 2c20 6465 6275 675f 6c6f 6f6b  sign, debug_look
-00010710: 7570 290a 2020 2020 2020 2020 6966 2068  up).        if h
-00010720: 6173 6174 7472 2873 656c 662e 6c6f 6f6b  asattr(self.look
-00010730: 5f75 702c 2022 7365 7373 696f 6e22 293a  _up, "session"):
-00010740: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00010750: 7365 6c66 2e6c 6f6f 6b5f 7570 2e73 6573  self.look_up.ses
-00010760: 7369 6f6e 3a0a 2020 2020 2020 2020 2020  sion:.          
-00010770: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-00010780: 2073 656c 662e 6c6f 6f6b 5f75 702e 6c6f   self.look_up.lo
-00010790: 6f6b 7570 2863 616c 6c73 6967 6e29 0a20  okup(callsign). 
-000107a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000107b0: 6562 7567 5f72 6573 706f 6e73 6520 3d20  ebug_response = 
-000107c0: 6622 7b72 6573 706f 6e73 657d 220a 2020  f"{response}".  
-000107d0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000107e0: 6767 6572 2e64 6562 7567 2822 5468 6520  gger.debug("The 
-000107f0: 5265 7370 6f6e 7365 3a20 2573 5c6e 222c  Response: %s\n",
-00010800: 2064 6562 7567 5f72 6573 706f 6e73 6529   debug_response)
-00010810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010820: 2069 6620 7265 7370 6f6e 7365 3a0a 2020   if response:.  
-00010830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010840: 2020 7468 6569 7267 7269 6420 3d20 7265    theirgrid = re
-00010850: 7370 6f6e 7365 2e67 6574 2822 6772 6964  sponse.get("grid
-00010860: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00010870: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00010880: 6163 745b 2247 7269 6453 7175 6172 6522  act["GridSquare"
-00010890: 5d20 3d20 7468 6569 7267 7269 640a 2020  ] = theirgrid.  
-000108a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108b0: 2020 5f74 6865 6972 636f 756e 7472 7920    _theircountry 
-000108c0: 3d20 7265 7370 6f6e 7365 2e67 6574 2822  = response.get("
-000108d0: 636f 756e 7472 7922 290a 2020 2020 2020  country").      
-000108e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000108f0: 2073 656c 662e 7374 6174 696f 6e2e 6765   self.station.ge
-00010900: 7428 2247 7269 6453 7175 6172 6522 2c20  t("GridSquare", 
-00010910: 2222 293a 0a20 2020 2020 2020 2020 2020  ""):.           
-00010920: 2020 2020 2020 2020 2020 2020 2068 6561               hea
-00010930: 6469 6e67 203d 2062 6561 7269 6e67 2873  ding = bearing(s
-00010940: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-00010950: 2247 7269 6453 7175 6172 6522 2c20 2222  "GridSquare", ""
-00010960: 292c 2074 6865 6972 6772 6964 290a 2020  ), theirgrid).  
-00010970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010980: 2020 2020 2020 6b69 6c6f 6d65 7465 7273        kilometers
-00010990: 203d 2064 6973 7461 6e63 6528 7365 6c66   = distance(self
-000109a0: 2e73 7461 7469 6f6e 2e67 6574 2822 4772  .station.get("Gr
-000109b0: 6964 5371 7561 7265 2229 2c20 7468 6569  idSquare"), thei
-000109c0: 7267 7269 6429 0a20 2020 2020 2020 2020  rgrid).         
-000109d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000109e0: 656c 662e 6865 6164 696e 675f 6469 7374  elf.heading_dist
-000109f0: 616e 6365 2e73 6574 5465 7874 280a 2020  ance.setText(.  
-00010a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a10: 2020 2020 2020 2020 2020 6622 7b74 6865            f"{the
-00010a20: 6972 6772 6964 7d20 4864 6720 7b68 6561  irgrid} Hdg {hea
-00010a30: 6469 6e67 7dc2 b020 4c50 207b 7265 6369  ding}.. LP {reci
-00010a40: 7072 6f63 6f6c 2868 6561 6469 6e67 297d  procol(heading)}
-00010a50: c2b0 202f 2022 0a20 2020 2020 2020 2020  .. / ".         
-00010a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a70: 2020 2066 2264 6973 7461 6e63 6520 7b69     f"distance {i
-00010a80: 6e74 286b 696c 6f6d 6574 6572 732a 302e  nt(kilometers*0.
-00010a90: 3632 3133 3731 297d 6d69 207b 6b69 6c6f  621371)}mi {kilo
-00010aa0: 6d65 7465 7273 7d6b 6d22 0a20 2020 2020  meters}km".     
-00010ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ac0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00010ad0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-00010ae0: 6478 5f65 6e74 6974 792e 7365 7454 6578  dx_entity.setTex
-00010af0: 7428 6622 7b74 6865 6972 636f 756e 7472  t(f"{theircountr
-00010b00: 797d 2229 0a20 2020 2020 2020 2020 2020  y}").           
-00010b10: 2020 2020 2023 2065 6c73 653a 0a20 2020       # else:.   
-00010b20: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-00010b30: 656c 662e 6865 6164 696e 675f 6469 7374  elf.heading_dist
-00010b40: 616e 6365 2e73 6574 5465 7874 2822 4c6f  ance.setText("Lo
-00010b50: 6f6b 7570 2066 6169 6c65 642e 2229 0a0a  okup failed.")..
-00010b60: 2020 2020 6465 6620 6368 6563 6b5f 6475      def check_du
-00010b70: 7065 2873 656c 662c 2063 616c 6c3a 2073  pe(self, call: s
-00010b80: 7472 2920 2d3e 2062 6f6f 6c3a 0a20 2020  tr) -> bool:.   
-00010b90: 2020 2020 2022 2222 4368 6563 6b73 2069       """Checks i
-00010ba0: 6620 6120 6361 6c6c 7369 676e 2069 7320  f a callsign is 
-00010bb0: 6120 6475 7065 206f 6e20 6375 7272 656e  a dupe on curren
-00010bc0: 7420 6261 6e64 2f6d 6f64 652e 2222 220a  t band/mode.""".
-00010bd0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00010be0: 7465 7374 2e70 7265 6475 7065 2873 656c  test.predupe(sel
-00010bf0: 6629 0a20 2020 2020 2020 2062 616e 6420  f).        band 
-00010c00: 3d20 666c 6f61 7428 6765 745f 6c6f 6767  = float(get_logg
-00010c10: 6564 5f62 616e 6428 7374 7228 7365 6c66  ed_band(str(self
-00010c20: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-00010c30: 2822 7666 6f61 222c 2030 2e30 2929 2929  ("vfoa", 0.0))))
-00010c40: 0a20 2020 2020 2020 206d 6f64 6520 3d20  .        mode = 
-00010c50: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-00010c60: 2e67 6574 2822 6d6f 6465 222c 2022 2229  .get("mode", "")
-00010c70: 0a20 2020 2020 2020 2064 6562 7567 6c69  .        debugli
-00010c80: 6e65 203d 2028 0a20 2020 2020 2020 2020  ne = (.         
-00010c90: 2020 2066 2243 616c 6c3a 207b 6361 6c6c     f"Call: {call
-00010ca0: 7d20 4261 6e64 3a20 7b62 616e 647d 204d  } Band: {band} M
-00010cb0: 6f64 653a 207b 6d6f 6465 7d20 4475 7065  ode: {mode} Dupe
-00010cc0: 7479 7065 3a20 7b73 656c 662e 636f 6e74  type: {self.cont
-00010cd0: 6573 742e 6475 7065 5f74 7970 657d 220a  est.dupe_type}".
-00010ce0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00010cf0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-00010d00: 2573 222c 2064 6562 7567 6c69 6e65 290a  %s", debugline).
-00010d10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00010d20: 636f 6e74 6573 742e 6475 7065 5f74 7970  contest.dupe_typ
-00010d30: 6520 3d3d 2031 3a0a 2020 2020 2020 2020  e == 1:.        
-00010d40: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
-00010d50: 662e 6461 7461 6261 7365 2e63 6865 636b  f.database.check
-00010d60: 5f64 7570 6528 6361 6c6c 290a 2020 2020  _dupe(call).    
-00010d70: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
-00010d80: 6573 742e 6475 7065 5f74 7970 6520 3d3d  est.dupe_type ==
-00010d90: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-00010da0: 7265 7375 6c74 203d 2073 656c 662e 6461  result = self.da
-00010db0: 7461 6261 7365 2e63 6865 636b 5f64 7570  tabase.check_dup
-00010dc0: 655f 6f6e 5f62 616e 6428 6361 6c6c 2c20  e_on_band(call, 
-00010dd0: 6261 6e64 290a 2020 2020 2020 2020 6966  band).        if
-00010de0: 2073 656c 662e 636f 6e74 6573 742e 6475   self.contest.du
-00010df0: 7065 5f74 7970 6520 3d3d 2033 3a0a 2020  pe_type == 3:.  
-00010e00: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00010e10: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
-00010e20: 2e63 6865 636b 5f64 7570 655f 6f6e 5f62  .check_dupe_on_b
-00010e30: 616e 645f 6d6f 6465 2863 616c 6c2c 2062  and_mode(call, b
-00010e40: 616e 642c 206d 6f64 6529 0a20 2020 2020  and, mode).     
-00010e50: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
-00010e60: 7374 2e64 7570 655f 7479 7065 203d 3d20  st.dupe_type == 
-00010e70: 343a 0a20 2020 2020 2020 2020 2020 2072  4:.            r
-00010e80: 6573 756c 7420 3d20 7b22 6973 6475 7065  esult = {"isdupe
-00010e90: 223a 2046 616c 7365 7d0a 2020 2020 2020  ": False}.      
-00010ea0: 2020 6465 6275 676c 696e 6520 3d20 6622    debugline = f"
-00010eb0: 7b72 6573 756c 747d 220a 2020 2020 2020  {result}".      
-00010ec0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-00010ed0: 2573 222c 2064 6562 7567 6c69 6e65 290a  %s", debugline).
-00010ee0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00010ef0: 6573 756c 742e 6765 7428 2269 7364 7570  esult.get("isdup
-00010f00: 6522 2c20 4661 6c73 6529 0a0a 2020 2020  e", False)..    
-00010f10: 6465 6620 7365 746d 6f64 6528 7365 6c66  def setmode(self
-00010f20: 2c20 6d6f 6465 3a20 7374 7229 202d 3e20  , mode: str) -> 
-00010f30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00010f40: 2273 7475 6220 666f 7220 7768 656e 2074  "stub for when t
-00010f50: 6865 206d 6f64 6520 6368 616e 6765 732e  he mode changes.
-00010f60: 2222 220a 2020 2020 2020 2020 6966 206d  """.        if m
-00010f70: 6f64 6520 3d3d 2022 4357 223a 0a20 2020  ode == "CW":.   
-00010f80: 2020 2020 2020 2020 2073 656c 662e 6375           self.cu
-00010f90: 7272 656e 745f 6d6f 6465 203d 2022 4357  rrent_mode = "CW
-00010fa0: 220a 2020 2020 2020 2020 2020 2020 2320  ".            # 
-00010fb0: 7365 6c66 2e6d 6f64 652e 7365 7454 6578  self.mode.setTex
-00010fc0: 7428 2243 5722 290a 2020 2020 2020 2020  t("CW").        
-00010fd0: 2020 2020 7365 6c66 2e73 656e 742e 7365      self.sent.se
-00010fe0: 7454 6578 7428 2235 3939 2229 0a20 2020  tText("599").   
-00010ff0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00011000: 6365 6976 652e 7365 7454 6578 7428 2235  ceive.setText("5
-00011010: 3939 2229 0a20 2020 2020 2020 2020 2020  99").           
-00011020: 2073 656c 662e 7265 6164 5f63 775f 6d61   self.read_cw_ma
-00011030: 6372 6f73 2829 0a20 2020 2020 2020 2020  cros().         
-00011040: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00011050: 2020 6966 206d 6f64 6520 3d3d 2022 5353    if mode == "SS
-00011060: 4222 3a0a 2020 2020 2020 2020 2020 2020  B":.            
-00011070: 7365 6c66 2e63 7572 7265 6e74 5f6d 6f64  self.current_mod
-00011080: 6520 3d20 2253 5342 220a 2020 2020 2020  e = "SSB".      
-00011090: 2020 2020 2020 2320 7365 6c66 2e6d 6f64        # self.mod
-000110a0: 652e 7365 7454 6578 7428 2253 5342 2229  e.setText("SSB")
-000110b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000110c0: 662e 7365 6e74 2e73 6574 5465 7874 2822  f.sent.setText("
-000110d0: 3539 2229 0a20 2020 2020 2020 2020 2020  59").           
-000110e0: 2073 656c 662e 7265 6365 6976 652e 7365   self.receive.se
-000110f0: 7454 6578 7428 2235 3922 290a 2020 2020  tText("59").    
-00011100: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
-00011110: 645f 6377 5f6d 6163 726f 7328 290a 2020  d_cw_macros().  
-00011120: 2020 2020 2020 6966 206d 6f64 6520 3d3d        if mode ==
-00011130: 2022 5254 5459 223a 0a20 2020 2020 2020   "RTTY":.       
-00011140: 2020 2020 2073 656c 662e 6375 7272 656e       self.curren
-00011150: 745f 6d6f 6465 203d 2022 5254 5459 220a  t_mode = "RTTY".
-00011160: 2020 2020 2020 2020 2020 2020 2320 7365              # se
-00011170: 6c66 2e6d 6f64 652e 7365 7454 6578 7428  lf.mode.setText(
-00011180: 2252 5454 5922 290a 2020 2020 2020 2020  "RTTY").        
-00011190: 2020 2020 7365 6c66 2e73 656e 742e 7365      self.sent.se
-000111a0: 7454 6578 7428 2235 3922 290a 2020 2020  tText("59").    
-000111b0: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
-000111c0: 6569 7665 2e73 6574 5465 7874 2822 3539  eive.setText("59
-000111d0: 2229 0a0a 2020 2020 6465 6620 6765 745f  ")..    def get_
-000111e0: 6f70 6f6e 2873 656c 6629 3a0a 2020 2020  opon(self):.    
-000111f0: 2020 2020 2222 2243 7472 6c2b 4f20 6f72      """Ctrl+O or
-00011200: 204f 504f 4e20 6469 616c 6f67 2222 220a   OPON dialog""".
-00011210: 2020 2020 2020 2020 7365 6c66 2e6f 706f          self.opo
-00011220: 6e5f 6469 616c 6f67 203d 204f 704f 6e28  n_dialog = OpOn(
-00011230: 574f 524b 494e 475f 5041 5448 290a 2020  WORKING_PATH).  
-00011240: 2020 2020 2020 7365 6c66 2e6f 706f 6e5f        self.opon_
-00011250: 6469 616c 6f67 2e61 6363 6570 7465 642e  dialog.accepted.
-00011260: 636f 6e6e 6563 7428 7365 6c66 2e6e 6577  connect(self.new
-00011270: 5f6f 7029 0a20 2020 2020 2020 2073 656c  _op).        sel
-00011280: 662e 6f70 6f6e 5f64 6961 6c6f 672e 6f70  f.opon_dialog.op
-00011290: 656e 2829 0a0a 2020 2020 6465 6620 6e65  en()..    def ne
-000112a0: 775f 6f70 2873 656c 6629 3a0a 2020 2020  w_op(self):.    
-000112b0: 2020 2020 2222 2253 6176 6520 6e65 7720      """Save new 
-000112c0: 4f50 2222 220a 2020 2020 2020 2020 6966  OP""".        if
-000112d0: 2073 656c 662e 6f70 6f6e 5f64 6961 6c6f   self.opon_dialo
-000112e0: 672e 4e65 774f 7065 7261 746f 722e 7465  g.NewOperator.te
-000112f0: 7874 2829 3a0a 2020 2020 2020 2020 2020  xt():.          
-00011300: 2020 7365 6c66 2e63 7572 7265 6e74 5f6f    self.current_o
-00011310: 7020 3d20 7365 6c66 2e6f 706f 6e5f 6469  p = self.opon_di
-00011320: 616c 6f67 2e4e 6577 4f70 6572 6174 6f72  alog.NewOperator
-00011330: 2e74 6578 7428 292e 7570 7065 7228 290a  .text().upper().
-00011340: 2020 2020 2020 2020 7365 6c66 2e6f 706f          self.opo
-00011350: 6e5f 6469 616c 6f67 2e63 6c6f 7365 2829  n_dialog.close()
-00011360: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00011370: 6465 6275 6728 224e 6577 204f 703a 2025  debug("New Op: %
-00011380: 7322 2c20 7365 6c66 2e63 7572 7265 6e74  s", self.current
-00011390: 5f6f 7029 0a20 2020 2020 2020 2073 656c  _op).        sel
-000113a0: 662e 6d61 6b65 5f6f 705f 6469 7228 290a  f.make_op_dir().
-000113b0: 0a20 2020 2064 6566 206d 616b 655f 6f70  .    def make_op
-000113c0: 5f64 6972 2873 656c 6629 3a0a 2020 2020  _dir(self):.    
-000113d0: 2020 2020 2222 2243 7265 6174 6520 4f50      """Create OP
-000113e0: 2064 6972 6563 746f 7279 2069 6620 6974   directory if it
-000113f0: 2064 6f65 7320 6e6f 7420 6578 6973 742e   does not exist.
-00011400: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-00011410: 656c 662e 6375 7272 656e 745f 6f70 3a0a  elf.current_op:.
-00011420: 2020 2020 2020 2020 2020 2020 6f70 5f70              op_p
-00011430: 6174 6820 3d20 5061 7468 2844 4154 415f  ath = Path(DATA_
-00011440: 5041 5448 2920 2f20 7365 6c66 2e63 7572  PATH) / self.cur
-00011450: 7265 6e74 5f6f 700a 2020 2020 2020 2020  rent_op.        
-00011460: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00011470: 2822 6f70 5f70 6174 683a 2025 7322 2c20  ("op_path: %s", 
-00011480: 7374 7228 6f70 5f70 6174 6829 290a 2020  str(op_path)).  
-00011490: 2020 2020 2020 2020 2020 6966 206f 705f            if op_
-000114a0: 7061 7468 2e69 735f 6469 7228 2920 6973  path.is_dir() is
-000114b0: 2046 616c 7365 3a0a 2020 2020 2020 2020   False:.        
-000114c0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-000114d0: 6562 7567 2822 4372 6561 7469 6e67 204f  ebug("Creating O
-000114e0: 7020 4469 7265 6374 6f72 793a 2025 7322  p Directory: %s"
-000114f0: 2c20 7374 7228 6f70 5f70 6174 6829 290a  , str(op_path)).
-00011500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011510: 6f73 2e6d 6b64 6972 2873 7472 286f 705f  os.mkdir(str(op_
-00011520: 7061 7468 2929 0a20 2020 2020 2020 2020  path)).         
-00011530: 2020 2069 6620 6f70 5f70 6174 682e 6973     if op_path.is
-00011540: 5f64 6972 2829 3a0a 2020 2020 2020 2020  _dir():.        
-00011550: 2020 2020 2020 2020 736f 7572 6365 5f70          source_p
-00011560: 6174 6820 3d20 5061 7468 2857 4f52 4b49  ath = Path(WORKI
-00011570: 4e47 5f50 4154 4829 202f 2022 6461 7461  NG_PATH) / "data
-00011580: 2220 2f20 2270 686f 6e65 7469 6373 220a  " / "phonetics".
-00011590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115a0: 6c6f 6767 6572 2e64 6562 7567 2822 736f  logger.debug("so
-000115b0: 7572 6365 5f70 6174 683a 2025 7322 2c20  urce_path: %s", 
-000115c0: 7374 7228 736f 7572 6365 5f70 6174 6829  str(source_path)
-000115d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000115e0: 2020 666f 7220 6368 696c 6420 696e 2073    for child in s
-000115f0: 6f75 7263 655f 7061 7468 2e69 7465 7264  ource_path.iterd
-00011600: 6972 2829 3a0a 2020 2020 2020 2020 2020  ir():.          
-00011610: 2020 2020 2020 2020 2020 6465 7374 696e            destin
-00011620: 6174 696f 6e5f 6669 6c65 203d 206f 705f  ation_file = op_
-00011630: 7061 7468 202f 2063 6869 6c64 2e6e 616d  path / child.nam
-00011640: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00011650: 2020 2020 2020 6966 2064 6573 7469 6e61        if destina
-00011660: 7469 6f6e 5f66 696c 652e 6973 5f66 696c  tion_file.is_fil
-00011670: 6528 2920 6973 2046 616c 7365 3a0a 2020  e() is False:.  
-00011680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011690: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-000116a0: 7567 2822 4465 7374 696e 6174 696f 6e3a  ug("Destination:
-000116b0: 2025 7322 2c20 7374 7228 6465 7374 696e   %s", str(destin
-000116c0: 6174 696f 6e5f 6669 6c65 2929 0a20 2020  ation_file)).   
-000116d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116e0: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
-000116f0: 5f66 696c 652e 7772 6974 655f 6279 7465  _file.write_byte
-00011700: 7328 6368 696c 642e 7265 6164 5f62 7974  s(child.read_byt
-00011710: 6573 2829 290a 0a20 2020 2064 6566 2070  es())..    def p
-00011720: 6f6c 6c5f 7261 6469 6f28 7365 6c66 293a  oll_radio(self):
-00011730: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
-00011740: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-00011750: 656c 662e 7269 675f 636f 6e74 726f 6c3a  elf.rig_control:
-00011760: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011770: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-00011780: 2e6f 6e6c 696e 653a 0a20 2020 2020 2020  .online:.       
-00011790: 2020 2020 2020 2020 2076 666f 203d 2073           vfo = s
-000117a0: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
-000117b0: 6765 745f 7666 6f28 290a 2020 2020 2020  get_vfo().      
-000117c0: 2020 2020 2020 2020 2020 6d6f 6465 203d            mode =
-000117d0: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
-000117e0: 6c2e 6765 745f 6d6f 6465 2829 0a20 2020  l.get_mode().   
-000117f0: 2020 2020 2020 2020 2020 2020 2062 7720               bw 
-00011800: 3d20 7365 6c66 2e72 6967 5f63 6f6e 7472  = self.rig_contr
-00011810: 6f6c 2e67 6574 5f62 7728 290a 2020 2020  ol.get_bw().    
-00011820: 2020 2020 2020 2020 2020 2020 2320 7365              # se
-00011830: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
-00011840: 7074 7422 5d20 3d20 7365 6c66 2e72 6967  ptt"] = self.rig
-00011850: 5f63 6f6e 7472 6f6c 2e67 6574 5f70 7474  _control.get_ptt
-00011860: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00011870: 2020 2023 2069 6620 7365 6c66 2e72 6164     # if self.rad
-00011880: 696f 5f73 7461 7465 2e67 6574 2822 7074  io_state.get("pt
-00011890: 7422 2c20 3029 203d 3d20 313a 0a20 2020  t", 0) == 1:.   
-000118a0: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-000118b0: 2020 2073 656c 662e 6c65 6674 646f 742e     self.leftdot.
-000118c0: 7365 7450 6978 6d61 7028 7365 6c66 2e67  setPixmap(self.g
-000118d0: 7265 656e 646f 7429 0a20 2020 2020 2020  reendot).       
-000118e0: 2020 2020 2020 2020 2023 2065 6c73 653a           # else:
-000118f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011900: 2023 2020 2020 2073 656c 662e 6c65 6674   #     self.left
-00011910: 646f 742e 7365 7450 6978 6d61 7028 7365  dot.setPixmap(se
-00011920: 6c66 2e72 6564 646f 7429 0a20 2020 2020  lf.reddot).     
-00011930: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
-00011940: 6465 203d 3d20 2243 5722 3a0a 2020 2020  de == "CW":.    
-00011950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011960: 7365 6c66 2e73 6574 6d6f 6465 286d 6f64  self.setmode(mod
-00011970: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00011980: 2020 2069 6620 6d6f 6465 203d 3d20 224c     if mode == "L
-00011990: 5342 2220 6f72 206d 6f64 6520 3d3d 2022  SB" or mode == "
-000119a0: 5553 4222 3a0a 2020 2020 2020 2020 2020  USB":.          
-000119b0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000119c0: 6574 6d6f 6465 2822 5353 4222 290a 2020  etmode("SSB").  
-000119d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000119e0: 206d 6f64 6520 3d3d 2022 5254 5459 223a   mode == "RTTY":
-000119f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011a00: 2020 2020 2073 656c 662e 7365 746d 6f64       self.setmod
-00011a10: 6528 2252 5454 5922 290a 2020 2020 2020  e("RTTY").      
-00011a20: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00011a30: 6164 696f 5f73 7461 7465 5b22 7666 6f61  adio_state["vfoa
-00011a40: 225d 203d 2076 666f 0a20 2020 2020 2020  "] = vfo.       
-00011a50: 2020 2020 2020 2020 2062 616e 6420 3d20           band = 
-00011a60: 6765 7462 616e 6428 7374 7228 7666 6f29  getband(str(vfo)
-00011a70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011a80: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
-00011a90: 7465 5b22 6261 6e64 225d 203d 2062 616e  te["band"] = ban
-00011aa0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00011ab0: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
-00011ac0: 4261 6e64 225d 203d 2067 6574 5f6c 6f67  Band"] = get_log
-00011ad0: 6765 645f 6261 6e64 2873 7472 2876 666f  ged_band(str(vfo
-00011ae0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00011af0: 2020 2073 656c 662e 7365 745f 6261 6e64     self.set_band
-00011b00: 5f69 6e64 6963 6174 6f72 2862 616e 6429  _indicator(band)
-00011b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011b20: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-00011b30: 655b 226d 6f64 6522 5d20 3d20 6d6f 6465  e["mode"] = mode
-00011b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011b50: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-00011b60: 655b 2262 7722 5d20 3d20 6277 0a20 2020  e["bw"] = bw.   
-00011b70: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00011b80: 6765 722e 6465 6275 6728 2256 464f 3a20  ger.debug("VFO: 
-00011b90: 2573 2020 4d4f 4445 3a20 2573 2042 573a  %s  MODE: %s BW:
-00011ba0: 2025 7322 2c20 7666 6f2c 206d 6f64 652c   %s", vfo, mode,
-00011bb0: 2062 7729 0a20 2020 2020 2020 2020 2020   bw).           
-00011bc0: 2020 2020 2073 656c 662e 7365 745f 7769       self.set_wi
-00011bd0: 6e64 6f77 5f74 6974 6c65 2829 0a20 2020  ndow_title().   
-00011be0: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-00011bf0: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
-00011c00: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
-00011c10: 203d 2022 5241 4449 4f5f 5354 4154 4522   = "RADIO_STATE"
-00011c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011c30: 2063 6d64 5b22 7374 6174 696f 6e22 5d20   cmd["station"] 
-00011c40: 3d20 706c 6174 666f 726d 2e6e 6f64 6528  = platform.node(
-00011c50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011c60: 2020 636d 645b 2262 616e 6422 5d20 3d20    cmd["band"] = 
-00011c70: 6261 6e64 0a20 2020 2020 2020 2020 2020  band.           
-00011c80: 2020 2020 2063 6d64 5b22 7666 6f61 225d       cmd["vfoa"]
-00011c90: 203d 2076 666f 0a20 2020 2020 2020 2020   = vfo.         
-00011ca0: 2020 2020 2020 2063 6d64 5b22 6d6f 6465         cmd["mode
-00011cb0: 225d 203d 206d 6f64 650a 2020 2020 2020  "] = mode.      
-00011cc0: 2020 2020 2020 2020 2020 636d 645b 2262            cmd["b
-00011cd0: 7722 5d20 3d20 6277 0a20 2020 2020 2020  w"] = bw.       
-00011ce0: 2020 2020 2020 2020 2073 656c 662e 6d75           self.mu
-00011cf0: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
-00011d00: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
-00011d10: 6d64 290a 0a20 2020 2064 6566 2065 6469  md)..    def edi
-00011d20: 745f 6377 5f6d 6163 726f 7328 7365 6c66  t_cw_macros(self
-00011d30: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00011d40: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-00011d50: 616c 6c73 2074 6865 2064 6566 6175 6c74  alls the default
-00011d60: 2074 6578 7420 6564 6974 6f72 2074 6f20   text editor to 
-00011d70: 6564 6974 2074 6865 2043 5720 6d61 6372  edit the CW macr
-00011d80: 6f20 6669 6c65 2e0a 2020 2020 2020 2020  o file..        
-00011d90: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-00011da0: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-00011db0: 6765 7428 226d 6f64 6522 2920 3d3d 2022  get("mode") == "
-00011dc0: 4357 223a 0a20 2020 2020 2020 2020 2020  CW":.           
-00011dd0: 206d 6163 726f 5f66 696c 6520 3d20 222f   macro_file = "/
-00011de0: 6377 6d61 6372 6f73 2e74 7874 220a 2020  cwmacros.txt".  
-00011df0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00011e00: 2020 2020 2020 2020 6d61 6372 6f5f 6669          macro_fi
-00011e10: 6c65 203d 2022 2f73 7362 6d61 6372 6f73  le = "/ssbmacros
-00011e20: 2e74 7874 220a 2020 2020 2020 2020 6966  .txt".        if
-00011e30: 206e 6f74 2050 6174 6828 4441 5441 5f50   not Path(DATA_P
-00011e40: 4154 4820 2b20 6d61 6372 6f5f 6669 6c65  ATH + macro_file
-00011e50: 292e 6578 6973 7473 2829 3a0a 2020 2020  ).exists():.    
-00011e60: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00011e70: 6562 7567 2822 7265 6164 5f63 775f 6d61  ebug("read_cw_ma
-00011e80: 6372 6f73 3a20 636f 7079 696e 6720 6465  cros: copying de
-00011e90: 6661 756c 7420 6d61 6372 6f20 6669 6c65  fault macro file
-00011ea0: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-00011eb0: 636f 7079 6669 6c65 2857 4f52 4b49 4e47  copyfile(WORKING
-00011ec0: 5f50 4154 4820 2b20 222f 6461 7461 2220  _PATH + "/data" 
-00011ed0: 2b20 6d61 6372 6f5f 6669 6c65 2c20 4441  + macro_file, DA
-00011ee0: 5441 5f50 4154 4820 2b20 6d61 6372 6f5f  TA_PATH + macro_
-00011ef0: 6669 6c65 290a 2020 2020 2020 2020 6f73  file).        os
-00011f00: 2e73 7973 7465 6d28 6622 7864 672d 6f70  .system(f"xdg-op
-00011f10: 656e 207b 4441 5441 5f50 4154 487d 7b6d  en {DATA_PATH}{m
-00011f20: 6163 726f 5f66 696c 657d 2229 0a0a 2020  acro_file}")..  
-00011f30: 2020 6465 6620 7265 6164 5f63 775f 6d61    def read_cw_ma
-00011f40: 6372 6f73 2873 656c 6629 202d 3e20 4e6f  cros(self) -> No
-00011f50: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00011f60: 2020 2020 2020 2020 5265 6164 7320 696e          Reads in
-00011f70: 2074 6865 2043 5720 6d61 6372 6f73 2c20   the CW macros, 
-00011f80: 6669 7273 7473 2069 7420 6368 6563 6b73  firsts it checks
-00011f90: 2074 6f20 7365 6520 6966 2074 6865 2066   to see if the f
-00011fa0: 696c 6520 6578 6973 7473 2e20 4966 2069  ile exists. If i
-00011fb0: 7420 646f 6573 206e 6f74 2c0a 2020 2020  t does not,.    
-00011fc0: 2020 2020 616e 6420 7468 6973 2068 6173      and this has
-00011fd0: 2062 6565 6e20 7061 636b 6167 6564 2077   been packaged w
-00011fe0: 6974 6820 7079 696e 7374 616c 6c65 7220  ith pyinstaller 
-00011ff0: 6974 2077 696c 6c20 636f 7079 2074 6865  it will copy the
-00012000: 2064 6566 6175 6c74 2066 696c 6520 6672   default file fr
-00012010: 6f6d 2074 6865 0a20 2020 2020 2020 2074  om the.        t
-00012020: 656d 7020 6469 7265 6374 6f72 7920 7468  emp directory th
-00012030: 6973 2069 7320 7275 6e6e 696e 6720 6672  is is running fr
-00012040: 6f6d 2e2e 2e20 496e 2074 6865 6f72 792e  om... In theory.
-00012050: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00012060: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
-00012070: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
-00012080: 6f64 6522 2920 3d3d 2022 4357 223a 0a20  ode") == "CW":. 
-00012090: 2020 2020 2020 2020 2020 206d 6163 726f             macro
-000120a0: 5f66 696c 6520 3d20 222f 6377 6d61 6372  _file = "/cwmacr
-000120b0: 6f73 2e74 7874 220a 2020 2020 2020 2020  os.txt".        
-000120c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000120d0: 2020 6d61 6372 6f5f 6669 6c65 203d 2022    macro_file = "
-000120e0: 2f73 7362 6d61 6372 6f73 2e74 7874 220a  /ssbmacros.txt".
-000120f0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00012100: 5061 7468 2844 4154 415f 5041 5448 202b  Path(DATA_PATH +
-00012110: 206d 6163 726f 5f66 696c 6529 2e65 7869   macro_file).exi
-00012120: 7374 7328 293a 0a20 2020 2020 2020 2020  sts():.         
-00012130: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00012140: 2272 6561 645f 6377 5f6d 6163 726f 733a  "read_cw_macros:
-00012150: 2063 6f70 7969 6e67 2064 6566 6175 6c74   copying default
-00012160: 206d 6163 726f 2066 696c 652e 2229 0a20   macro file."). 
-00012170: 2020 2020 2020 2020 2020 2063 6f70 7966             copyf
-00012180: 696c 6528 574f 524b 494e 475f 5041 5448  ile(WORKING_PATH
-00012190: 202b 2022 2f64 6174 6122 202b 206d 6163   + "/data" + mac
-000121a0: 726f 5f66 696c 652c 2044 4154 415f 5041  ro_file, DATA_PA
-000121b0: 5448 202b 206d 6163 726f 5f66 696c 6529  TH + macro_file)
-000121c0: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
-000121d0: 656e 2844 4154 415f 5041 5448 202b 206d  en(DATA_PATH + m
-000121e0: 6163 726f 5f66 696c 652c 2022 7222 2c20  acro_file, "r", 
-000121f0: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
-00012200: 2920 6173 2066 696c 655f 6465 7363 7269  ) as file_descri
-00012210: 7074 6f72 3a0a 2020 2020 2020 2020 2020  ptor:.          
-00012220: 2020 666f 7220 6c69 6e65 2069 6e20 6669    for line in fi
-00012230: 6c65 5f64 6573 6372 6970 746f 723a 0a20  le_descriptor:. 
-00012240: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00012250: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00012260: 2020 2020 2020 2020 6d6f 6465 2c20 666b          mode, fk
-00012270: 6579 2c20 6275 7474 6f6e 6e61 6d65 2c20  ey, buttonname, 
-00012280: 6377 7465 7874 203d 206c 696e 652e 7370  cwtext = line.sp
-00012290: 6c69 7428 227c 2229 0a20 2020 2020 2020  lit("|").       
-000122a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000122b0: 6d6f 6465 2e73 7472 6970 2829 2e75 7070  mode.strip().upp
-000122c0: 6572 2829 203d 3d20 2252 2220 616e 6420  er() == "R" and 
-000122d0: 7365 6c66 2e70 7265 662e 6765 7428 2272  self.pref.get("r
-000122e0: 756e 5f73 7461 7465 2229 3a0a 2020 2020  un_state"):.    
-000122f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012300: 2020 2020 7365 6c66 2e66 6b65 7973 5b66      self.fkeys[f
-00012310: 6b65 792e 7374 7269 7028 295d 203d 2028  key.strip()] = (
-00012320: 6275 7474 6f6e 6e61 6d65 2e73 7472 6970  buttonname.strip
-00012330: 2829 2c20 6377 7465 7874 2e73 7472 6970  (), cwtext.strip
-00012340: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-00012350: 2020 2020 2020 2020 6966 206d 6f64 652e          if mode.
-00012360: 7374 7269 7028 292e 7570 7065 7228 2920  strip().upper() 
-00012370: 213d 2022 5222 2061 6e64 206e 6f74 2073  != "R" and not s
-00012380: 656c 662e 7072 6566 2e67 6574 2822 7275  elf.pref.get("ru
-00012390: 6e5f 7374 6174 6522 293a 0a20 2020 2020  n_state"):.     
-000123a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123b0: 2020 2073 656c 662e 666b 6579 735b 666b     self.fkeys[fk
-000123c0: 6579 2e73 7472 6970 2829 5d20 3d20 2862  ey.strip()] = (b
-000123d0: 7574 746f 6e6e 616d 652e 7374 7269 7028  uttonname.strip(
-000123e0: 292c 2063 7774 6578 742e 7374 7269 7028  ), cwtext.strip(
-000123f0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00012400: 2020 2065 7863 6570 7420 5661 6c75 6545     except ValueE
-00012410: 7272 6f72 2061 7320 6572 723a 0a20 2020  rror as err:.   
-00012420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012430: 206c 6f67 6765 722e 696e 666f 2822 7265   logger.info("re
-00012440: 6164 5f63 775f 6d61 6372 6f73 3a20 2573  ad_cw_macros: %s
-00012450: 222c 2065 7272 290a 2020 2020 2020 2020  ", err).        
-00012460: 6b65 7973 203d 2073 656c 662e 666b 6579  keys = self.fkey
-00012470: 732e 6b65 7973 2829 0a20 2020 2020 2020  s.keys().       
-00012480: 2069 6620 2246 3122 2069 6e20 6b65 7973   if "F1" in keys
-00012490: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000124a0: 6c66 2e46 312e 7365 7454 6578 7428 6622  lf.F1.setText(f"
-000124b0: 4631 3a20 7b73 656c 662e 666b 6579 735b  F1: {self.fkeys[
-000124c0: 2746 3127 5d5b 305d 7d22 290a 2020 2020  'F1'][0]}").    
-000124d0: 2020 2020 2020 2020 7365 6c66 2e46 312e          self.F1.
-000124e0: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
-000124f0: 666b 6579 735b 2246 3122 5d5b 315d 290a  fkeys["F1"][1]).
-00012500: 2020 2020 2020 2020 6966 2022 4632 2220          if "F2" 
-00012510: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
-00012520: 2020 2020 2073 656c 662e 4632 2e73 6574       self.F2.set
-00012530: 5465 7874 2866 2246 323a 207b 7365 6c66  Text(f"F2: {self
-00012540: 2e66 6b65 7973 5b27 4632 275d 5b30 5d7d  .fkeys['F2'][0]}
-00012550: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-00012560: 656c 662e 4632 2e73 6574 546f 6f6c 5469  elf.F2.setToolTi
-00012570: 7028 7365 6c66 2e66 6b65 7973 5b22 4632  p(self.fkeys["F2
-00012580: 225d 5b31 5d29 0a20 2020 2020 2020 2069  "][1]).        i
-00012590: 6620 2246 3322 2069 6e20 6b65 7973 3a0a  f "F3" in keys:.
-000125a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000125b0: 2e46 332e 7365 7454 6578 7428 6622 4633  .F3.setText(f"F3
-000125c0: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
-000125d0: 3327 5d5b 305d 7d22 290a 2020 2020 2020  3'][0]}").      
-000125e0: 2020 2020 2020 7365 6c66 2e46 332e 7365        self.F3.se
-000125f0: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
-00012600: 6579 735b 2246 3322 5d5b 315d 290a 2020  eys["F3"][1]).  
-00012610: 2020 2020 2020 6966 2022 4634 2220 696e        if "F4" in
-00012620: 206b 6579 733a 0a20 2020 2020 2020 2020   keys:.         
-00012630: 2020 2073 656c 662e 4634 2e73 6574 5465     self.F4.setTe
-00012640: 7874 2866 2246 343a 207b 7365 6c66 2e66  xt(f"F4: {self.f
-00012650: 6b65 7973 5b27 4634 275d 5b30 5d7d 2229  keys['F4'][0]}")
-00012660: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012670: 662e 4634 2e73 6574 546f 6f6c 5469 7028  f.F4.setToolTip(
-00012680: 7365 6c66 2e66 6b65 7973 5b22 4634 225d  self.fkeys["F4"]
-00012690: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
-000126a0: 2246 3522 2069 6e20 6b65 7973 3a0a 2020  "F5" in keys:.  
-000126b0: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-000126c0: 352e 7365 7454 6578 7428 6622 4635 3a20  5.setText(f"F5: 
-000126d0: 7b73 656c 662e 666b 6579 735b 2746 3527  {self.fkeys['F5'
-000126e0: 5d5b 305d 7d22 290a 2020 2020 2020 2020  ][0]}").        
-000126f0: 2020 2020 7365 6c66 2e46 352e 7365 7454      self.F5.setT
-00012700: 6f6f 6c54 6970 2873 656c 662e 666b 6579  oolTip(self.fkey
-00012710: 735b 2246 3522 5d5b 315d 290a 2020 2020  s["F5"][1]).    
-00012720: 2020 2020 6966 2022 4636 2220 696e 206b      if "F6" in k
-00012730: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
-00012740: 2073 656c 662e 4636 2e73 6574 5465 7874   self.F6.setText
-00012750: 2866 2246 363a 207b 7365 6c66 2e66 6b65  (f"F6: {self.fke
-00012760: 7973 5b27 4636 275d 5b30 5d7d 2229 0a20  ys['F6'][0]}"). 
-00012770: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012780: 4636 2e73 6574 546f 6f6c 5469 7028 7365  F6.setToolTip(se
-00012790: 6c66 2e66 6b65 7973 5b22 4636 225d 5b31  lf.fkeys["F6"][1
-000127a0: 5d29 0a20 2020 2020 2020 2069 6620 2246  ]).        if "F
-000127b0: 3722 2069 6e20 6b65 7973 3a0a 2020 2020  7" in keys:.    
-000127c0: 2020 2020 2020 2020 7365 6c66 2e46 372e          self.F7.
-000127d0: 7365 7454 6578 7428 6622 4637 3a20 7b73  setText(f"F7: {s
-000127e0: 656c 662e 666b 6579 735b 2746 3727 5d5b  elf.fkeys['F7'][
-000127f0: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
-00012800: 2020 7365 6c66 2e46 372e 7365 7454 6f6f    self.F7.setToo
-00012810: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
-00012820: 2246 3722 5d5b 315d 290a 2020 2020 2020  "F7"][1]).      
-00012830: 2020 6966 2022 4638 2220 696e 206b 6579    if "F8" in key
-00012840: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00012850: 656c 662e 4638 2e73 6574 5465 7874 2866  elf.F8.setText(f
-00012860: 2246 383a 207b 7365 6c66 2e66 6b65 7973  "F8: {self.fkeys
-00012870: 5b27 4638 275d 5b30 5d7d 2229 0a20 2020  ['F8'][0]}").   
-00012880: 2020 2020 2020 2020 2073 656c 662e 4638           self.F8
-00012890: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
-000128a0: 2e66 6b65 7973 5b22 4638 225d 5b31 5d29  .fkeys["F8"][1])
-000128b0: 0a20 2020 2020 2020 2069 6620 2246 3922  .        if "F9"
-000128c0: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
-000128d0: 2020 2020 2020 7365 6c66 2e46 392e 7365        self.F9.se
-000128e0: 7454 6578 7428 6622 4639 3a20 7b73 656c  tText(f"F9: {sel
-000128f0: 662e 666b 6579 735b 2746 3927 5d5b 305d  f.fkeys['F9'][0]
-00012900: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-00012910: 7365 6c66 2e46 392e 7365 7454 6f6f 6c54  self.F9.setToolT
-00012920: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
-00012930: 3922 5d5b 315d 290a 2020 2020 2020 2020  9"][1]).        
-00012940: 6966 2022 4631 3022 2069 6e20 6b65 7973  if "F10" in keys
-00012950: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00012960: 6c66 2e46 3130 2e73 6574 5465 7874 2866  lf.F10.setText(f
-00012970: 2246 3130 3a20 7b73 656c 662e 666b 6579  "F10: {self.fkey
-00012980: 735b 2746 3130 275d 5b30 5d7d 2229 0a20  s['F10'][0]}"). 
-00012990: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000129a0: 4631 302e 7365 7454 6f6f 6c54 6970 2873  F10.setToolTip(s
-000129b0: 656c 662e 666b 6579 735b 2246 3130 225d  elf.fkeys["F10"]
-000129c0: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
-000129d0: 2246 3131 2220 696e 206b 6579 733a 0a20  "F11" in keys:. 
-000129e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000129f0: 4631 312e 7365 7454 6578 7428 6622 4631  F11.setText(f"F1
-00012a00: 313a 207b 7365 6c66 2e66 6b65 7973 5b27  1: {self.fkeys['
-00012a10: 4631 3127 5d5b 305d 7d22 290a 2020 2020  F11'][0]}").    
-00012a20: 2020 2020 2020 2020 7365 6c66 2e46 3131          self.F11
-00012a30: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
-00012a40: 2e66 6b65 7973 5b22 4631 3122 5d5b 315d  .fkeys["F11"][1]
-00012a50: 290a 2020 2020 2020 2020 6966 2022 4631  ).        if "F1
-00012a60: 3222 2069 6e20 6b65 7973 3a0a 2020 2020  2" in keys:.    
-00012a70: 2020 2020 2020 2020 7365 6c66 2e46 3132          self.F12
-00012a80: 2e73 6574 5465 7874 2866 2246 3132 3a20  .setText(f"F12: 
-00012a90: 7b73 656c 662e 666b 6579 735b 2746 3132  {self.fkeys['F12
-00012aa0: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
-00012ab0: 2020 2020 2073 656c 662e 4631 322e 7365       self.F12.se
-00012ac0: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
-00012ad0: 6579 735b 2246 3132 225d 5b31 5d29 0a0a  eys["F12"][1])..
-00012ae0: 2020 2020 6465 6620 6765 6e65 7261 7465      def generate
-00012af0: 5f61 6469 6628 7365 6c66 293a 0a20 2020  _adif(self):.   
-00012b00: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
-00012b10: 2041 4449 4622 2222 0a20 2020 2020 2020   ADIF""".       
-00012b20: 206c 6f67 6765 722e 6465 6275 6728 222a   logger.debug("*
-00012b30: 2a2a 2a2a 2a41 4449 462a 2a2a 2a2a 2229  *****ADIF*****")
-00012b40: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00012b50: 6e74 6573 742e 6164 6966 2873 656c 6629  ntest.adif(self)
-00012b60: 0a0a 2020 2020 6465 6620 6765 6e65 7261  ..    def genera
-00012b70: 7465 5f63 6162 7269 6c6c 6f28 7365 6c66  te_cabrillo(self
-00012b80: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
-00012b90: 6e65 7261 7465 7320 4361 6272 696c 6c6f  nerates Cabrillo
-00012ba0: 2066 696c 652e 204d 6179 6265 2e22 2222   file. Maybe."""
-00012bb0: 0a20 2020 2020 2020 2023 2068 7474 7073  .        # https
-00012bc0: 3a2f 2f77 7777 2e63 7177 7078 2e63 6f6d  ://www.cqwpx.com
-00012bd0: 2f63 6162 7269 6c6c 6f2e 6874 6d0a 2020  /cabrillo.htm.  
-00012be0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00012bf0: 7567 2822 2a2a 2a2a 2a2a 4361 6272 696c  ug("******Cabril
-00012c00: 6c6f 2a2a 2a2a 2a22 290a 2020 2020 2020  lo*****").      
-00012c10: 2020 7365 6c66 2e63 6f6e 7465 7374 2e63    self.contest.c
-00012c20: 6162 7269 6c6c 6f28 7365 6c66 290a 0a0a  abrillo(self)...
-00012c30: 6465 6620 6c6f 6164 5f66 6f6e 7473 5f66  def load_fonts_f
-00012c40: 726f 6d5f 6469 7228 6469 7265 6374 6f72  rom_dir(director
-00012c50: 793a 2073 7472 2920 2d3e 2073 6574 3a0a  y: str) -> set:.
-00012c60: 2020 2020 2222 220a 2020 2020 5765 6c6c      """.    Well
-00012c70: 2069 7420 6c6f 6164 7320 666f 6e74 7320   it loads fonts 
-00012c80: 6672 6f6d 2061 2064 6972 6563 746f 7279  from a directory
-00012c90: 2e2e 2e0a 2020 2020 2222 220a 2020 2020  ....    """.    
-00012ca0: 666f 6e74 5f66 616d 696c 6965 7320 3d20  font_families = 
-00012cb0: 7365 7428 290a 2020 2020 666f 7220 5f66  set().    for _f
-00012cc0: 6920 696e 2051 4469 7228 6469 7265 6374  i in QDir(direct
-00012cd0: 6f72 7929 2e65 6e74 7279 496e 666f 4c69  ory).entryInfoLi
-00012ce0: 7374 285b 222a 2e74 7466 222c 2022 2a2e  st(["*.ttf", "*.
-00012cf0: 776f 6666 222c 2022 2a2e 776f 6666 3222  woff", "*.woff2"
-00012d00: 5d29 3a0a 2020 2020 2020 2020 5f69 6420  ]):.        _id 
-00012d10: 3d20 5146 6f6e 7444 6174 6162 6173 652e  = QFontDatabase.
-00012d20: 6164 6441 7070 6c69 6361 7469 6f6e 466f  addApplicationFo
-00012d30: 6e74 285f 6669 2e61 6273 6f6c 7574 6546  nt(_fi.absoluteF
-00012d40: 696c 6550 6174 6828 2929 0a20 2020 2020  ilePath()).     
-00012d50: 2020 2066 6f6e 745f 6661 6d69 6c69 6573     font_families
-00012d60: 207c 3d20 7365 7428 5146 6f6e 7444 6174   |= set(QFontDat
-00012d70: 6162 6173 652e 6170 706c 6963 6174 696f  abase.applicatio
-00012d80: 6e46 6f6e 7446 616d 696c 6965 7328 5f69  nFontFamilies(_i
-00012d90: 6429 290a 2020 2020 7265 7475 726e 2066  d)).    return f
-00012da0: 6f6e 745f 6661 6d69 6c69 6573 0a0a 0a64  ont_families...d
-00012db0: 6566 2069 6e73 7461 6c6c 5f69 636f 6e73  ef install_icons
-00012dc0: 2829 3a0a 2020 2020 2222 2249 6e73 7461  ():.    """Insta
-00012dd0: 6c6c 2069 636f 6e73 2222 220a 2020 2020  ll icons""".    
-00012de0: 6f73 2e73 7973 7465 6d28 0a20 2020 2020  os.system(.     
-00012df0: 2020 2022 7864 672d 6963 6f6e 2d72 6573     "xdg-icon-res
-00012e00: 6f75 7263 6520 696e 7374 616c 6c20 2d2d  ource install --
-00012e10: 7369 7a65 2033 3220 2d2d 636f 6e74 6578  size 32 --contex
-00012e20: 7420 6170 7073 202d 2d6d 6f64 6520 7573  t apps --mode us
-00012e30: 6572 2022 0a20 2020 2020 2020 2066 227b  er ".        f"{
-00012e40: 574f 524b 494e 475f 5041 5448 7d2f 6461  WORKING_PATH}/da
-00012e50: 7461 2f6b 3667 7465 2e6e 6f74 316d 6d2d  ta/k6gte.not1mm-
-00012e60: 3332 2e70 6e67 206b 3667 7465 2d6e 6f74  32.png k6gte-not
-00012e70: 316d 6d22 0a20 2020 2029 0a20 2020 206f  1mm".    ).    o
-00012e80: 732e 7379 7374 656d 280a 2020 2020 2020  s.system(.      
-00012e90: 2020 2278 6467 2d69 636f 6e2d 7265 736f    "xdg-icon-reso
-00012ea0: 7572 6365 2069 6e73 7461 6c6c 202d 2d73  urce install --s
-00012eb0: 697a 6520 3634 202d 2d63 6f6e 7465 7874  ize 64 --context
-00012ec0: 2061 7070 7320 2d2d 6d6f 6465 2075 7365   apps --mode use
-00012ed0: 7220 220a 2020 2020 2020 2020 6622 7b57  r ".        f"{W
-00012ee0: 4f52 4b49 4e47 5f50 4154 487d 2f64 6174  ORKING_PATH}/dat
-00012ef0: 612f 6b36 6774 652e 6e6f 7431 6d6d 2d36  a/k6gte.not1mm-6
-00012f00: 342e 706e 6720 6b36 6774 652d 6e6f 7431  4.png k6gte-not1
-00012f10: 6d6d 220a 2020 2020 290a 2020 2020 6f73  mm".    ).    os
-00012f20: 2e73 7973 7465 6d28 0a20 2020 2020 2020  .system(.       
-00012f30: 2022 7864 672d 6963 6f6e 2d72 6573 6f75   "xdg-icon-resou
-00012f40: 7263 6520 696e 7374 616c 6c20 2d2d 7369  rce install --si
-00012f50: 7a65 2031 3238 202d 2d63 6f6e 7465 7874  ze 128 --context
-00012f60: 2061 7070 7320 2d2d 6d6f 6465 2075 7365   apps --mode use
-00012f70: 7220 220a 2020 2020 2020 2020 6622 7b57  r ".        f"{W
-00012f80: 4f52 4b49 4e47 5f50 4154 487d 2f64 6174  ORKING_PATH}/dat
-00012f90: 612f 6b36 6774 652e 6e6f 7431 6d6d 2d31  a/k6gte.not1mm-1
-00012fa0: 3238 2e70 6e67 206b 3667 7465 2d6e 6f74  28.png k6gte-not
-00012fb0: 316d 6d22 0a20 2020 2029 0a20 2020 206f  1mm".    ).    o
-00012fc0: 732e 7379 7374 656d 2866 2278 6467 2d64  s.system(f"xdg-d
-00012fd0: 6573 6b74 6f70 2d6d 656e 7520 696e 7374  esktop-menu inst
-00012fe0: 616c 6c20 7b57 4f52 4b49 4e47 5f50 4154  all {WORKING_PAT
-00012ff0: 487d 2f64 6174 612f 6b36 6774 652d 6e6f  H}/data/k6gte-no
-00013000: 7431 6d6d 2e64 6573 6b74 6f70 2229 0a0a  t1mm.desktop")..
-00013010: 0a64 6566 2064 6f69 6d70 286d 6f64 6e61  .def doimp(modna
-00013020: 6d65 293a 0a20 2020 2022 2222 7265 7475  me):.    """retu
-00013030: 726e 206d 6f64 756c 6520 7061 7468 2222  rn module path""
-00013040: 220a 2020 2020 7265 7475 726e 2069 6d70  ".    return imp
-00013050: 6f72 746c 6962 2e69 6d70 6f72 745f 6d6f  ortlib.import_mo
-00013060: 6475 6c65 2866 226e 6f74 316d 6d2e 706c  dule(f"not1mm.pl
-00013070: 7567 696e 732e 7b6d 6f64 6e61 6d65 7d22  ugins.{modname}"
-00013080: 290a 0a0a 6465 6620 7275 6e28 293a 0a20  )...def run():. 
-00013090: 2020 2022 2222 0a20 2020 204d 6169 6e20     """.    Main 
-000130a0: 456e 7472 790a 2020 2020 2222 220a 0a20  Entry.    """.. 
-000130b0: 2020 2069 6e73 7461 6c6c 5f69 636f 6e73     install_icons
-000130c0: 2829 0a20 2020 2074 696d 6572 2e73 7461  ().    timer.sta
-000130d0: 7274 2831 3030 290a 2020 2020 7469 6d65  rt(100).    time
-000130e0: 7232 2e73 7461 7274 2832 3530 290a 0a20  r2.start(250).. 
-000130f0: 2020 2073 7973 2e65 7869 7428 6170 702e     sys.exit(app.
-00013100: 6578 6563 2829 290a 0a0a 6c6f 6767 6572  exec())...logger
-00013110: 203d 206c 6f67 6769 6e67 2e67 6574 4c6f   = logging.getLo
-00013120: 6767 6572 2822 5f5f 6d61 696e 5f5f 2229  gger("__main__")
-00013130: 0a68 616e 646c 6572 203d 206c 6f67 6769  .handler = loggi
-00013140: 6e67 2e53 7472 6561 6d48 616e 646c 6572  ng.StreamHandler
-00013150: 2829 0a66 6f72 6d61 7474 6572 203d 206c  ().formatter = l
-00013160: 6f67 6769 6e67 2e46 6f72 6d61 7474 6572  ogging.Formatter
-00013170: 280a 2020 2020 6461 7465 666d 743d 2225  (.    datefmt="%
-00013180: 483a 254d 3a25 5322 2c0a 2020 2020 666d  H:%M:%S",.    fm
-00013190: 743d 225b 2528 6173 6374 696d 6529 735d  t="[%(asctime)s]
-000131a0: 2025 286c 6576 656c 6e61 6d65 2973 2025   %(levelname)s %
-000131b0: 286d 6f64 756c 6529 7320 2d20 2528 6675  (module)s - %(fu
-000131c0: 6e63 4e61 6d65 2973 204c 696e 6520 2528  ncName)s Line %(
-000131d0: 6c69 6e65 6e6f 2964 3a20 2528 6d65 7373  lineno)d: %(mess
-000131e0: 6167 6529 7322 2c0a 290a 6861 6e64 6c65  age)s",.).handle
-000131f0: 722e 7365 7446 6f72 6d61 7474 6572 2866  r.setFormatter(f
-00013200: 6f72 6d61 7474 6572 290a 6c6f 6767 6572  ormatter).logger
-00013210: 2e61 6464 4861 6e64 6c65 7228 6861 6e64  .addHandler(hand
-00013220: 6c65 7229 0a0a 6966 2050 6174 6828 222e  ler)..if Path(".
-00013230: 2f64 6562 7567 2229 2e65 7869 7374 7328  /debug").exists(
-00013240: 293a 0a20 2020 206c 6f67 6765 722e 7365  ):.    logger.se
-00013250: 744c 6576 656c 286c 6f67 6769 6e67 2e44  tLevel(logging.D
-00013260: 4542 5547 290a 2020 2020 6c6f 6767 6572  EBUG).    logger
-00013270: 2e64 6562 7567 2822 6465 6275 6767 696e  .debug("debuggin
-00013280: 6720 6f6e 2229 0a65 6c73 653a 0a20 2020  g on").else:.   
-00013290: 206c 6f67 6765 722e 7365 744c 6576 656c   logger.setLevel
-000132a0: 286c 6f67 6769 6e67 2e57 4152 4e49 4e47  (logging.WARNING
-000132b0: 290a 2020 2020 6c6f 6767 6572 2e77 6172  ).    logger.war
-000132c0: 6e69 6e67 2822 6465 6275 6767 696e 6720  ning("debugging 
-000132d0: 6f66 6622 290a 0a61 7070 203d 2051 7457  off")..app = QtW
-000132e0: 6964 6765 7473 2e51 4170 706c 6963 6174  idgets.QApplicat
-000132f0: 696f 6e28 7379 732e 6172 6776 290a 2320  ion(sys.argv).# 
-00013300: 6170 702e 7365 7453 7479 6c65 2822 4675  app.setStyle("Fu
-00013310: 7369 6f6e 2229 0a66 6f6e 745f 7061 7468  sion").font_path
-00013320: 203d 2057 4f52 4b49 4e47 5f50 4154 4820   = WORKING_PATH 
-00013330: 2b20 222f 6461 7461 220a 6661 6d69 6c69  + "/data".famili
-00013340: 6573 203d 206c 6f61 645f 666f 6e74 735f  es = load_fonts_
-00013350: 6672 6f6d 5f64 6972 286f 732e 6673 7061  from_dir(os.fspa
-00013360: 7468 2866 6f6e 745f 7061 7468 2929 0a6c  th(font_path)).l
-00013370: 6f67 6765 722e 696e 666f 2866 616d 696c  ogger.info(famil
-00013380: 6965 7329 0a77 696e 646f 7720 3d20 4d61  ies).window = Ma
-00013390: 696e 5769 6e64 6f77 2829 0a68 6569 6768  inWindow().heigh
-000133a0: 7420 3d20 7769 6e64 6f77 2e70 7265 662e  t = window.pref.
-000133b0: 6765 7428 2277 696e 646f 775f 6865 6967  get("window_heig
-000133c0: 6874 222c 2033 3030 290a 7769 6474 6820  ht", 300).width 
-000133d0: 3d20 7769 6e64 6f77 2e70 7265 662e 6765  = window.pref.ge
-000133e0: 7428 2277 696e 646f 775f 7769 6474 6822  t("window_width"
-000133f0: 2c20 3730 3029 0a78 203d 2077 696e 646f  , 700).x = windo
-00013400: 772e 7072 6566 2e67 6574 2822 7769 6e64  w.pref.get("wind
-00013410: 6f77 5f78 222c 202d 3129 0a79 203d 2077  ow_x", -1).y = w
-00013420: 696e 646f 772e 7072 6566 2e67 6574 2822  indow.pref.get("
-00013430: 7769 6e64 6f77 5f79 222c 202d 3129 0a77  window_y", -1).w
-00013440: 696e 646f 772e 7365 7447 656f 6d65 7472  indow.setGeometr
-00013450: 7928 782c 2079 2c20 7769 6474 682c 2068  y(x, y, width, h
-00013460: 6569 6768 7429 0a23 2077 696e 646f 772e  eight).# window.
-00013470: 7365 7457 696e 646f 7754 6974 6c65 2866  setWindowTitle(f
-00013480: 224e 6f74 314d 4d20 767b 5f5f 7665 7273  "Not1MM v{__vers
-00013490: 696f 6e5f 5f7d 2229 0a77 696e 646f 772e  ion__}").window.
-000134a0: 6361 6c6c 7369 676e 2e73 6574 466f 6375  callsign.setFocu
-000134b0: 7328 290a 7769 6e64 6f77 2e73 686f 7728  s().window.show(
-000134c0: 290a 7469 6d65 7220 3d20 5174 436f 7265  ).timer = QtCore
-000134d0: 2e51 5469 6d65 7228 290a 7469 6d65 722e  .QTimer().timer.
-000134e0: 7469 6d65 6f75 742e 636f 6e6e 6563 7428  timeout.connect(
-000134f0: 7769 6e64 6f77 2e70 6f6c 6c5f 7261 6469  window.poll_radi
-00013500: 6f29 0a74 696d 6572 3220 3d20 5174 436f  o).timer2 = QtCo
-00013510: 7265 2e51 5469 6d65 7228 290a 7469 6d65  re.QTimer().time
-00013520: 7232 2e74 696d 656f 7574 2e63 6f6e 6e65  r2.timeout.conne
-00013530: 6374 2877 696e 646f 772e 6368 6563 6b5f  ct(window.check_
-00013540: 7564 705f 7472 6166 6669 6329 0a0a 6966  udp_traffic)..if
-00013550: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
-00013560: 6d61 696e 5f5f 223a 0a20 2020 2072 756e  main__":.    run
-00013570: 2829 0a                                  ().
+0000ad50: 6c66 2e73 7461 7469 6f6e 5b22 4941 5255  lf.station["IARU
+0000ad60: 5a6f 6e65 225d 203d 2073 656c 662e 7365  Zone"] = self.se
+0000ad70: 7474 696e 6773 5f64 6961 6c6f 672e 4954  ttings_dialog.IT
+0000ad80: 555a 6f6e 652e 7465 7874 2829 0a20 2020  UZone.text().   
+0000ad90: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
+0000ada0: 6e5b 224c 6963 656e 7365 436c 6173 7322  n["LicenseClass"
+0000adb0: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
+0000adc0: 735f 6469 616c 6f67 2e4c 6963 656e 7365  s_dialog.License
+0000add0: 2e74 6578 7428 292e 7469 746c 6528 290a  .text().title().
+0000ade0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0000adf0: 7469 6f6e 5b22 4c61 7469 7475 6465 225d  tion["Latitude"]
+0000ae00: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
+0000ae10: 5f64 6961 6c6f 672e 4c61 7469 7475 6465  _dialog.Latitude
+0000ae20: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000ae30: 7365 6c66 2e73 7461 7469 6f6e 5b22 4c6f  self.station["Lo
+0000ae40: 6e67 6974 7564 6522 5d20 3d20 7365 6c66  ngitude"] = self
+0000ae50: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000ae60: 2e4c 6f6e 6769 7475 6465 2e74 6578 7428  .Longitude.text(
+0000ae70: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000ae80: 7461 7469 6f6e 5b22 5354 5865 7122 5d20  tation["STXeq"] 
+0000ae90: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
+0000aea0: 6469 616c 6f67 2e53 7461 7469 6f6e 5458  dialog.StationTX
+0000aeb0: 5258 2e74 6578 7428 290a 2020 2020 2020  RX.text().      
+0000aec0: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000aed0: 5350 6f77 6522 5d20 3d20 7365 6c66 2e73  SPowe"] = self.s
+0000aee0: 6574 7469 6e67 735f 6469 616c 6f67 2e50  ettings_dialog.P
+0000aef0: 6f77 6572 2e74 6578 7428 290a 2020 2020  ower.text().    
+0000af00: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000af10: 5b22 5341 6e74 6522 5d20 3d20 7365 6c66  ["SAnte"] = self
+0000af20: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000af30: 2e41 6e74 656e 6e61 2e74 6578 7428 290a  .Antenna.text().
+0000af40: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0000af50: 7469 6f6e 5b22 5341 6e74 4831 225d 203d  tion["SAntH1"] =
+0000af60: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+0000af70: 6961 6c6f 672e 416e 7448 6569 6768 742e  ialog.AntHeight.
+0000af80: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
+0000af90: 656c 662e 7374 6174 696f 6e5b 2253 416e  elf.station["SAn
+0000afa0: 7448 3222 5d20 3d20 7365 6c66 2e73 6574  tH2"] = self.set
+0000afb0: 7469 6e67 735f 6469 616c 6f67 2e41 534c  tings_dialog.ASL
+0000afc0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000afd0: 7365 6c66 2e73 7461 7469 6f6e 5b22 4152  self.station["AR
+0000afe0: 524c 5365 6374 696f 6e22 5d20 3d20 7365  RLSection"] = se
+0000aff0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000b000: 6f67 2e41 5252 4c53 6563 7469 6f6e 2e74  og.ARRLSection.t
+0000b010: 6578 7428 292e 7570 7065 7228 290a 2020  ext().upper().  
+0000b020: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000b030: 6f6e 5b22 526f 7665 7251 5448 225d 203d  on["RoverQTH"] =
+0000b040: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+0000b050: 6961 6c6f 672e 526f 7665 7251 5448 2e74  ialog.RoverQTH.t
+0000b060: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
+0000b070: 6c66 2e73 7461 7469 6f6e 5b22 436c 7562  lf.station["Club
+0000b080: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
+0000b090: 6773 5f64 6961 6c6f 672e 436c 7562 2e74  gs_dialog.Club.t
+0000b0a0: 6578 7428 292e 7469 746c 6528 290a 2020  ext().title().  
+0000b0b0: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000b0c0: 6f6e 5b22 456d 6169 6c22 5d20 3d20 7365  on["Email"] = se
+0000b0d0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000b0e0: 6f67 2e45 6d61 696c 2e74 6578 7428 290a  og.Email.text().
+0000b0f0: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
+0000b100: 6162 6173 652e 6164 645f 7374 6174 696f  abase.add_statio
+0000b110: 6e28 7365 6c66 2e73 7461 7469 6f6e 290a  n(self.station).
+0000b120: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000b130: 7469 6e67 735f 6469 616c 6f67 2e63 6c6f  tings_dialog.clo
+0000b140: 7365 2829 0a20 2020 2020 2020 2069 6620  se().        if 
+0000b150: 7365 6c66 2e63 7572 7265 6e74 5f6f 7020  self.current_op 
+0000b160: 3d3d 2022 223a 0a20 2020 2020 2020 2020  == "":.         
+0000b170: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
+0000b180: 6f70 203d 2073 656c 662e 7374 6174 696f  op = self.statio
+0000b190: 6e2e 6765 7428 2243 616c 6c22 2c20 2222  n.get("Call", ""
+0000b1a0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0000b1b0: 6c66 2e6d 616b 655f 6f70 5f64 6972 2829  lf.make_op_dir()
+0000b1c0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+0000b1d0: 5f63 6f75 6e74 203d 2073 656c 662e 6461  _count = self.da
+0000b1e0: 7461 6261 7365 2e66 6574 6368 5f61 6c6c  tabase.fetch_all
+0000b1f0: 5f63 6f6e 7465 7374 7328 290a 2020 2020  _contests().    
+0000b200: 2020 2020 6966 206c 656e 2863 6f6e 7465      if len(conte
+0000b210: 7374 5f63 6f75 6e74 2920 3d3d 2030 3a0a  st_count) == 0:.
+0000b220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b230: 2e6e 6577 5f63 6f6e 7465 7374 5f64 6961  .new_contest_dia
+0000b240: 6c6f 6728 290a 0a20 2020 2064 6566 2065  log()..    def e
+0000b250: 6469 745f 6d61 6372 6f28 7365 6c66 2c20  dit_macro(self, 
+0000b260: 6675 6e63 7469 6f6e 5f6b 6579 293a 0a20  function_key):. 
+0000b270: 2020 2020 2020 2022 2222 5368 6f77 2065         """Show e
+0000b280: 6469 7420 6d61 6372 6f20 6469 616c 6f67  dit macro dialog
+0000b290: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+0000b2a0: 2e65 6469 745f 6d61 6372 6f5f 6469 616c  .edit_macro_dial
+0000b2b0: 6f67 203d 2045 6469 744d 6163 726f 2866  og = EditMacro(f
+0000b2c0: 756e 6374 696f 6e5f 6b65 792c 2057 4f52  unction_key, WOR
+0000b2d0: 4b49 4e47 5f50 4154 4829 0a20 2020 2020  KING_PATH).     
+0000b2e0: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
+0000b2f0: 726f 5f64 6961 6c6f 672e 6163 6365 7074  ro_dialog.accept
+0000b300: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+0000b310: 6564 6974 6564 5f6d 6163 726f 290a 2020  edited_macro).  
+0000b320: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000b330: 6566 2e67 6574 2822 6461 726b 5f6d 6f64  ef.get("dark_mod
+0000b340: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
+0000b350: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
+0000b360: 5f64 6961 6c6f 672e 7365 7453 7479 6c65  _dialog.setStyle
+0000b370: 5368 6565 7428 4441 524b 5f53 5459 4c45  Sheet(DARK_STYLE
+0000b380: 5348 4545 5429 0a20 2020 2020 2020 2073  SHEET).        s
+0000b390: 656c 662e 6564 6974 5f6d 6163 726f 5f64  elf.edit_macro_d
+0000b3a0: 6961 6c6f 672e 6f70 656e 2829 0a0a 2020  ialog.open()..  
+0000b3b0: 2020 6465 6620 6564 6974 6564 5f6d 6163    def edited_mac
+0000b3c0: 726f 2873 656c 6629 3a0a 2020 2020 2020  ro(self):.      
+0000b3d0: 2020 2222 2253 6176 6520 6564 6974 6564    """Save edited
+0000b3e0: 206d 6163 726f 2222 220a 2020 2020 2020   macro""".      
+0000b3f0: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+0000b400: 6f5f 6469 616c 6f67 2e66 756e 6374 696f  o_dialog.functio
+0000b410: 6e5f 6b65 792e 7365 7454 6578 7428 0a20  n_key.setText(. 
+0000b420: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b430: 6564 6974 5f6d 6163 726f 5f64 6961 6c6f  edit_macro_dialo
+0000b440: 672e 6d61 6372 6f5f 6c61 6265 6c2e 7465  g.macro_label.te
+0000b450: 7874 2829 0a20 2020 2020 2020 2029 0a20  xt().        ). 
+0000b460: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
+0000b470: 5f6d 6163 726f 5f64 6961 6c6f 672e 6675  _macro_dialog.fu
+0000b480: 6e63 7469 6f6e 5f6b 6579 2e73 6574 546f  nction_key.setTo
+0000b490: 6f6c 5469 7028 0a20 2020 2020 2020 2020  olTip(.         
+0000b4a0: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
+0000b4b0: 726f 5f64 6961 6c6f 672e 7468 655f 6d61  ro_dialog.the_ma
+0000b4c0: 6372 6f2e 7465 7874 2829 0a20 2020 2020  cro.text().     
+0000b4d0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+0000b4e0: 662e 6564 6974 5f6d 6163 726f 5f64 6961  f.edit_macro_dia
+0000b4f0: 6c6f 672e 636c 6f73 6528 290a 0a20 2020  log.close()..   
+0000b500: 2064 6566 2065 6469 745f 4631 2873 656c   def edit_F1(sel
+0000b510: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
+0000b520: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
+0000b530: 6f67 6765 722e 6465 6275 6728 2246 3120  ogger.debug("F1 
+0000b540: 5269 6768 7420 436c 6963 6b65 642e 2229  Right Clicked.")
+0000b550: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
+0000b560: 6974 5f6d 6163 726f 2873 656c 662e 4631  it_macro(self.F1
+0000b570: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
+0000b580: 4632 2873 656c 6629 3a0a 2020 2020 2020  F2(self):.      
+0000b590: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
+0000b5a0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000b5b0: 6728 2246 3220 5269 6768 7420 436c 6963  g("F2 Right Clic
+0000b5c0: 6b65 642e 2229 0a20 2020 2020 2020 2073  ked.").        s
+0000b5d0: 656c 662e 6564 6974 5f6d 6163 726f 2873  elf.edit_macro(s
+0000b5e0: 656c 662e 4632 290a 0a20 2020 2064 6566  elf.F2)..    def
+0000b5f0: 2065 6469 745f 4633 2873 656c 6629 3a0a   edit_F3(self):.
+0000b600: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
+0000b610: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
+0000b620: 722e 6465 6275 6728 2246 3320 5269 6768  r.debug("F3 Righ
+0000b630: 7420 436c 6963 6b65 642e 2229 0a20 2020  t Clicked.").   
+0000b640: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
+0000b650: 6163 726f 2873 656c 662e 4633 290a 0a20  acro(self.F3).. 
+0000b660: 2020 2064 6566 2065 6469 745f 4634 2873     def edit_F4(s
+0000b670: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000b680: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
+0000b690: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
+0000b6a0: 3420 5269 6768 7420 436c 6963 6b65 642e  4 Right Clicked.
+0000b6b0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000b6c0: 6564 6974 5f6d 6163 726f 2873 656c 662e  edit_macro(self.
+0000b6d0: 4634 290a 0a20 2020 2064 6566 2065 6469  F4)..    def edi
+0000b6e0: 745f 4635 2873 656c 6629 3a0a 2020 2020  t_F5(self):.    
+0000b6f0: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
+0000b700: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000b710: 6275 6728 2246 3520 5269 6768 7420 436c  bug("F5 Right Cl
+0000b720: 6963 6b65 642e 2229 0a20 2020 2020 2020  icked.").       
+0000b730: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
+0000b740: 2873 656c 662e 4635 290a 0a20 2020 2064  (self.F5)..    d
+0000b750: 6566 2065 6469 745f 4636 2873 656c 6629  ef edit_F6(self)
+0000b760: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
+0000b770: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
+0000b780: 6765 722e 6465 6275 6728 2246 3620 5269  ger.debug("F6 Ri
+0000b790: 6768 7420 436c 6963 6b65 642e 2229 0a20  ght Clicked."). 
+0000b7a0: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
+0000b7b0: 5f6d 6163 726f 2873 656c 662e 4636 290a  _macro(self.F6).
+0000b7c0: 0a20 2020 2064 6566 2065 6469 745f 4637  .    def edit_F7
+0000b7d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000b7e0: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
+0000b7f0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000b800: 2246 3720 5269 6768 7420 436c 6963 6b65  "F7 Right Clicke
+0000b810: 642e 2229 0a20 2020 2020 2020 2073 656c  d.").        sel
+0000b820: 662e 6564 6974 5f6d 6163 726f 2873 656c  f.edit_macro(sel
+0000b830: 662e 4637 290a 0a20 2020 2064 6566 2065  f.F7)..    def e
+0000b840: 6469 745f 4638 2873 656c 6629 3a0a 2020  dit_F8(self):.  
+0000b850: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
+0000b860: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000b870: 6465 6275 6728 2246 3820 5269 6768 7420  debug("F8 Right 
+0000b880: 436c 6963 6b65 642e 2229 0a20 2020 2020  Clicked.").     
+0000b890: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
+0000b8a0: 726f 2873 656c 662e 4638 290a 0a20 2020  ro(self.F8)..   
+0000b8b0: 2064 6566 2065 6469 745f 4639 2873 656c   def edit_F9(sel
+0000b8c0: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
+0000b8d0: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
+0000b8e0: 6f67 6765 722e 6465 6275 6728 2246 3920  ogger.debug("F9 
+0000b8f0: 5269 6768 7420 436c 6963 6b65 642e 2229  Right Clicked.")
+0000b900: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
+0000b910: 6974 5f6d 6163 726f 2873 656c 662e 4639  it_macro(self.F9
+0000b920: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
+0000b930: 4631 3028 7365 6c66 293a 0a20 2020 2020  F10(self):.     
+0000b940: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
+0000b950: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000b960: 7567 2822 4631 3020 5269 6768 7420 436c  ug("F10 Right Cl
+0000b970: 6963 6b65 642e 2229 0a20 2020 2020 2020  icked.").       
+0000b980: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
+0000b990: 2873 656c 662e 4631 3029 0a0a 2020 2020  (self.F10)..    
+0000b9a0: 6465 6620 6564 6974 5f46 3131 2873 656c  def edit_F11(sel
+0000b9b0: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
+0000b9c0: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
+0000b9d0: 6f67 6765 722e 6465 6275 6728 2246 3131  ogger.debug("F11
+0000b9e0: 2052 6967 6874 2043 6c69 636b 6564 2e22   Right Clicked."
+0000b9f0: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
+0000ba00: 6469 745f 6d61 6372 6f28 7365 6c66 2e46  dit_macro(self.F
+0000ba10: 3131 290a 0a20 2020 2064 6566 2065 6469  11)..    def edi
+0000ba20: 745f 4631 3228 7365 6c66 293a 0a20 2020  t_F12(self):.   
+0000ba30: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000ba40: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000ba50: 6562 7567 2822 4631 3220 5269 6768 7420  ebug("F12 Right 
+0000ba60: 436c 6963 6b65 642e 2229 0a20 2020 2020  Clicked.").     
+0000ba70: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
+0000ba80: 726f 2873 656c 662e 4631 3229 0a0a 2020  ro(self.F12)..  
+0000ba90: 2020 6465 6620 7072 6f63 6573 735f 6d61    def process_ma
+0000baa0: 6372 6f28 7365 6c66 2c20 6d61 6372 6f3a  cro(self, macro:
+0000bab0: 2073 7472 2920 2d3e 2073 7472 3a0a 2020   str) -> str:.  
+0000bac0: 2020 2020 2020 2222 2250 726f 6365 7373        """Process
+0000bad0: 2043 5720 6d61 6372 6f20 7375 6273 7469   CW macro substi
+0000bae0: 7475 7469 6f6e 7322 2222 0a20 2020 2020  tutions""".     
+0000baf0: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
+0000bb00: 2e64 6174 6162 6173 652e 6765 745f 7365  .database.get_se
+0000bb10: 7269 616c 2829 0a20 2020 2020 2020 206e  rial().        n
+0000bb20: 6578 745f 7365 7269 616c 203d 2073 7472  ext_serial = str
+0000bb30: 2872 6573 756c 742e 6765 7428 2273 6572  (result.get("ser
+0000bb40: 6961 6c5f 6e72 222c 2022 3122 2929 0a20  ial_nr", "1")). 
+0000bb50: 2020 2020 2020 2069 6620 6e65 7874 5f73         if next_s
+0000bb60: 6572 6961 6c20 3d3d 2022 4e6f 6e65 223a  erial == "None":
+0000bb70: 0a20 2020 2020 2020 2020 2020 206e 6578  .            nex
+0000bb80: 745f 7365 7269 616c 203d 2022 3122 0a20  t_serial = "1". 
+0000bb90: 2020 2020 2020 206d 6163 726f 203d 206d         macro = m
+0000bba0: 6163 726f 2e75 7070 6572 2829 0a20 2020  acro.upper().   
+0000bbb0: 2020 2020 206d 6163 726f 203d 206d 6163       macro = mac
+0000bbc0: 726f 2e72 6570 6c61 6365 2822 2322 2c20  ro.replace("#", 
+0000bbd0: 6e65 7874 5f73 6572 6961 6c29 0a20 2020  next_serial).   
+0000bbe0: 2020 2020 206d 6163 726f 203d 206d 6163       macro = mac
+0000bbf0: 726f 2e72 6570 6c61 6365 2822 7b4d 5943  ro.replace("{MYC
+0000bc00: 414c 4c7d 222c 2073 656c 662e 7374 6174  ALL}", self.stat
+0000bc10: 696f 6e2e 6765 7428 2243 616c 6c22 2c20  ion.get("Call", 
+0000bc20: 2222 2929 0a20 2020 2020 2020 206d 6163  "")).        mac
+0000bc30: 726f 203d 206d 6163 726f 2e72 6570 6c61  ro = macro.repla
+0000bc40: 6365 2822 7b48 4953 4341 4c4c 7d22 2c20  ce("{HISCALL}", 
+0000bc50: 7365 6c66 2e63 616c 6c73 6967 6e2e 7465  self.callsign.te
+0000bc60: 7874 2829 290a 2020 2020 2020 2020 6966  xt()).        if
+0000bc70: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+0000bc80: 652e 6765 7428 226d 6f64 6522 2920 3d3d  e.get("mode") ==
+0000bc90: 2022 4357 223a 0a20 2020 2020 2020 2020   "CW":.         
+0000bca0: 2020 206d 6163 726f 203d 206d 6163 726f     macro = macro
+0000bcb0: 2e72 6570 6c61 6365 2822 7b53 4e54 7d22  .replace("{SNT}"
+0000bcc0: 2c20 7365 6c66 2e73 656e 742e 7465 7874  , self.sent.text
+0000bcd0: 2829 2e72 6570 6c61 6365 2822 3922 2c20  ().replace("9", 
+0000bce0: 226e 2229 290a 2020 2020 2020 2020 656c  "n")).        el
+0000bcf0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000bd00: 6d61 6372 6f20 3d20 6d61 6372 6f2e 7265  macro = macro.re
+0000bd10: 706c 6163 6528 227b 534e 547d 222c 2073  place("{SNT}", s
+0000bd20: 656c 662e 7365 6e74 2e74 6578 7428 2929  elf.sent.text())
+0000bd30: 0a20 2020 2020 2020 206d 6163 726f 203d  .        macro =
+0000bd40: 206d 6163 726f 2e72 6570 6c61 6365 2822   macro.replace("
+0000bd50: 7b53 454e 544e 527d 222c 2073 656c 662e  {SENTNR}", self.
+0000bd60: 6f74 6865 725f 312e 7465 7874 2829 290a  other_1.text()).
+0000bd70: 2020 2020 2020 2020 6d61 6372 6f20 3d20          macro = 
+0000bd80: 6d61 6372 6f2e 7265 706c 6163 6528 0a20  macro.replace(. 
+0000bd90: 2020 2020 2020 2020 2020 2022 7b45 5843             "{EXC
+0000bda0: 487d 222c 2073 656c 662e 636f 6e74 6573  H}", self.contes
+0000bdb0: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
+0000bdc0: 5365 6e74 4578 6368 616e 6765 222c 2022  SentExchange", "
+0000bdd0: 7878 7822 290a 2020 2020 2020 2020 290a  xxx").        ).
+0000bde0: 2020 2020 2020 2020 7265 7475 726e 206d          return m
+0000bdf0: 6163 726f 0a0a 2020 2020 6465 6620 766f  acro..    def vo
+0000be00: 6963 655f 7374 7269 6e67 2873 656c 662c  ice_string(self,
+0000be10: 2074 6865 5f73 7472 696e 673a 2073 7472   the_string: str
+0000be20: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000be30: 2020 2022 2222 766f 6963 6573 2073 7472     """voices str
+0000be40: 696e 6720 7573 696e 6720 6e61 746f 2070  ing using nato p
+0000be50: 686f 6e65 7469 6373 2222 220a 2020 2020  honetics""".    
+0000be60: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000be70: 2822 566f 6963 696e 673a 2025 7322 2c20  ("Voicing: %s", 
+0000be80: 7468 655f 7374 7269 6e67 290a 2020 2020  the_string).    
+0000be90: 2020 2020 6f70 5f70 6174 6820 3d20 5061      op_path = Pa
+0000bea0: 7468 2844 4154 415f 5041 5448 2920 2f20  th(DATA_PATH) / 
+0000beb0: 7365 6c66 2e63 7572 7265 6e74 5f6f 700a  self.current_op.
+0000bec0: 2020 2020 2020 2020 6966 2022 5b22 2069          if "[" i
+0000bed0: 6e20 7468 655f 7374 7269 6e67 3a0a 2020  n the_string:.  
+0000bee0: 2020 2020 2020 2020 2020 7375 625f 7374            sub_st
+0000bef0: 7269 6e67 203d 2074 6865 5f73 7472 696e  ring = the_strin
+0000bf00: 672e 7374 7269 7028 225b 5d22 292e 6c6f  g.strip("[]").lo
+0000bf10: 7765 7228 290a 2020 2020 2020 2020 2020  wer().          
+0000bf20: 2020 6669 6c65 6e61 6d65 203d 2066 227b    filename = f"{
+0000bf30: 7374 7228 6f70 5f70 6174 6829 7d2f 7b73  str(op_path)}/{s
+0000bf40: 7562 5f73 7472 696e 677d 2e77 6176 220a  ub_string}.wav".
+0000bf50: 2020 2020 2020 2020 2020 2020 6966 2050              if P
+0000bf60: 6174 6828 6669 6c65 6e61 6d65 292e 6973  ath(filename).is
+0000bf70: 5f66 696c 6528 293a 0a20 2020 2020 2020  _file():.       
+0000bf80: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0000bf90: 6465 6275 6728 2256 6f69 6369 6e67 3a20  debug("Voicing: 
+0000bfa0: 2573 222c 2066 696c 656e 616d 6529 0a20  %s", filename). 
+0000bfb0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000bfc0: 6174 612c 205f 6673 203d 2073 662e 7265  ata, _fs = sf.re
+0000bfd0: 6164 2866 696c 656e 616d 652c 2064 7479  ad(filename, dty
+0000bfe0: 7065 3d22 666c 6f61 7433 3222 290a 2020  pe="float32").  
+0000bff0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000c000: 6c66 2e70 7474 5f6f 6e28 290a 2020 2020  lf.ptt_on().    
+0000c010: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+0000c020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c030: 2020 2020 2073 642e 6465 6661 756c 742e       sd.default.
+0000c040: 6465 7669 6365 203d 2073 656c 662e 7072  device = self.pr
+0000c050: 6566 2e67 6574 2822 736f 756e 6464 6576  ef.get("sounddev
+0000c060: 6963 6522 2c20 2264 6566 6175 6c74 2229  ice", "default")
+0000c070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c080: 2020 2020 2073 642e 6465 6661 756c 742e       sd.default.
+0000c090: 7361 6d70 6c65 7261 7465 203d 2034 3431  samplerate = 441
+0000c0a0: 3030 2e30 0a20 2020 2020 2020 2020 2020  00.0.           
+0000c0b0: 2020 2020 2020 2020 2073 642e 706c 6179           sd.play
+0000c0c0: 2864 6174 6129 0a20 2020 2020 2020 2020  (data).         
+0000c0d0: 2020 2020 2020 2020 2020 205f 7374 6174             _stat
+0000c0e0: 7573 203d 2073 642e 7761 6974 2829 0a20  us = sd.wait(). 
+0000c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c100: 2020 2023 2068 7474 7073 3a2f 2f73 6e79     # https://sny
+0000c110: 6b2e 696f 2f61 6476 6973 6f72 2f70 7974  k.io/advisor/pyt
+0000c120: 686f 6e2f 736f 756e 6464 6576 6963 652f  hon/sounddevice/
+0000c130: 6675 6e63 7469 6f6e 732f 736f 756e 6464  functions/soundd
+0000c140: 6576 6963 652e 506f 7274 4175 6469 6f45  evice.PortAudioE
+0000c150: 7272 6f72 0a20 2020 2020 2020 2020 2020  rror.           
+0000c160: 2020 2020 2065 7863 6570 7420 7364 2e50       except sd.P
+0000c170: 6f72 7441 7564 696f 4572 726f 7220 6173  ortAudioError as
+0000c180: 2065 7272 3a0a 2020 2020 2020 2020 2020   err:.          
+0000c190: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000c1a0: 2e64 6562 7567 2822 2573 222c 2066 227b  .debug("%s", f"{
+0000c1b0: 6572 727d 2229 0a0a 2020 2020 2020 2020  err}")..        
+0000c1c0: 2020 2020 2020 2020 7365 6c66 2e70 7474          self.ptt
+0000c1d0: 5f6f 6666 2829 0a20 2020 2020 2020 2020  _off().         
+0000c1e0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000c1f0: 2020 7365 6c66 2e70 7474 5f6f 6e28 290a    self.ptt_on().
+0000c200: 2020 2020 2020 2020 666f 7220 6c65 7474          for lett
+0000c210: 6572 2069 6e20 7468 655f 7374 7269 6e67  er in the_string
+0000c220: 2e6c 6f77 6572 2829 3a0a 2020 2020 2020  .lower():.      
+0000c230: 2020 2020 2020 6966 206c 6574 7465 7220        if letter 
+0000c240: 696e 2022 6162 6364 6566 6768 696a 6b6c  in "abcdefghijkl
+0000c250: 6d6e 6f70 7172 7374 7576 7778 797a 2031  mnopqrstuvwxyz 1
+0000c260: 3233 3435 3637 3839 3022 3a0a 2020 2020  234567890":.    
+0000c270: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+0000c280: 6574 7465 7220 3d3d 2022 2022 3a0a 2020  etter == " ":.  
+0000c290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2a0: 2020 6c65 7474 6572 203d 2022 7370 6163    letter = "spac
+0000c2b0: 6522 0a20 2020 2020 2020 2020 2020 2020  e".             
+0000c2c0: 2020 2066 696c 656e 616d 6520 3d20 6622     filename = f"
+0000c2d0: 7b73 7472 286f 705f 7061 7468 297d 2f7b  {str(op_path)}/{
+0000c2e0: 6c65 7474 6572 7d2e 7761 7622 0a20 2020  letter}.wav".   
+0000c2f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000c300: 5061 7468 2866 696c 656e 616d 6529 2e69  Path(filename).i
+0000c310: 735f 6669 6c65 2829 3a0a 2020 2020 2020  s_file():.      
+0000c320: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0000c330: 6767 6572 2e64 6562 7567 2822 566f 6963  gger.debug("Voic
+0000c340: 696e 673a 2025 7322 2c20 6669 6c65 6e61  ing: %s", filena
+0000c350: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+0000c360: 2020 2020 2020 2020 6461 7461 2c20 5f66          data, _f
+0000c370: 7320 3d20 7366 2e72 6561 6428 6669 6c65  s = sf.read(file
+0000c380: 6e61 6d65 2c20 6474 7970 653d 2266 6c6f  name, dtype="flo
+0000c390: 6174 3332 2229 0a20 2020 2020 2020 2020  at32").         
+0000c3a0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+0000c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3c0: 2020 2020 2020 2020 7364 2e64 6566 6175          sd.defau
+0000c3d0: 6c74 2e64 6576 6963 6520 3d20 7365 6c66  lt.device = self
+0000c3e0: 2e70 7265 662e 6765 7428 2273 6f75 6e64  .pref.get("sound
+0000c3f0: 6465 7669 6365 222c 2022 6465 6661 756c  device", "defaul
+0000c400: 7422 290a 2020 2020 2020 2020 2020 2020  t").            
+0000c410: 2020 2020 2020 2020 2020 2020 7364 2e64              sd.d
+0000c420: 6566 6175 6c74 2e73 616d 706c 6572 6174  efault.samplerat
+0000c430: 6520 3d20 3434 3130 302e 300a 2020 2020  e = 44100.0.    
+0000c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c450: 2020 2020 7364 2e70 6c61 7928 6461 7461      sd.play(data
+0000c460: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000c470: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000c480: 2e64 6562 7567 2822 2573 222c 2066 227b  .debug("%s", f"{
+0000c490: 7364 2e77 6169 7428 297d 2229 0a20 2020  sd.wait()}").   
+0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4b0: 2065 7863 6570 7420 7364 2e50 6f72 7441   except sd.PortA
+0000c4c0: 7564 696f 4572 726f 7220 6173 2065 7272  udioError as err
+0000c4d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c4e0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000c4f0: 2e64 6562 7567 2822 2573 222c 2066 227b  .debug("%s", f"{
+0000c500: 6572 727d 2229 0a20 2020 2020 2020 2073  err}").        s
+0000c510: 656c 662e 7074 745f 6f66 6628 290a 0a20  elf.ptt_off().. 
+0000c520: 2020 2064 6566 2070 7474 5f6f 6e28 7365     def ptt_on(se
+0000c530: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000c540: 7475 726e 206f 6e20 7074 7422 2222 0a20  turn on ptt""". 
+0000c550: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0000c560: 6967 5f63 6f6e 7472 6f6c 3a0a 2020 2020  ig_control:.    
+0000c570: 2020 2020 2020 2020 7365 6c66 2e6c 6566          self.lef
+0000c580: 7464 6f74 2e73 6574 5069 786d 6170 2873  tdot.setPixmap(s
+0000c590: 656c 662e 6772 6565 6e64 6f74 290a 2020  elf.greendot).  
+0000c5a0: 2020 2020 2020 2020 2020 6170 702e 7072            app.pr
+0000c5b0: 6f63 6573 7345 7665 6e74 7328 290a 2020  ocessEvents().  
+0000c5c0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0000c5d0: 6967 5f63 6f6e 7472 6f6c 2e70 7474 5f6f  ig_control.ptt_o
+0000c5e0: 6e28 290a 0a20 2020 2064 6566 2070 7474  n()..    def ptt
+0000c5f0: 5f6f 6666 2873 656c 6629 3a0a 2020 2020  _off(self):.    
+0000c600: 2020 2020 2222 2274 7572 6e20 6f66 6620      """turn off 
+0000c610: 7074 7422 2222 0a20 2020 2020 2020 2073  ptt""".        s
+0000c620: 656c 662e 6c65 6674 646f 742e 7365 7450  elf.leftdot.setP
+0000c630: 6978 6d61 7028 7365 6c66 2e72 6564 646f  ixmap(self.reddo
+0000c640: 7429 0a20 2020 2020 2020 2061 7070 2e70  t).        app.p
+0000c650: 726f 6365 7373 4576 656e 7473 2829 0a20  rocessEvents(). 
+0000c660: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
+0000c670: 636f 6e74 726f 6c2e 7074 745f 6f66 6628  control.ptt_off(
+0000c680: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
+0000c690: 3128 7365 6c66 293a 0a20 2020 2020 2020  1(self):.       
+0000c6a0: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000c6b0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000c6c0: 2822 4631 2043 6c69 636b 6564 2229 0a20  ("F1 Clicked"). 
+0000c6d0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0000c6e0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
+0000c6f0: 6d6f 6465 2229 2069 6e20 5b22 4c53 4222  mode") in ["LSB"
+0000c700: 2c20 2255 5342 222c 2022 5353 4222 5d3a  , "USB", "SSB"]:
+0000c710: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c720: 662e 766f 6963 655f 7374 7269 6e67 2873  f.voice_string(s
+0000c730: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
+0000c740: 6f28 7365 6c66 2e46 312e 746f 6f6c 5469  o(self.F1.toolTi
+0000c750: 7028 2929 290a 2020 2020 2020 2020 2020  p())).          
+0000c760: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0000c770: 2069 6620 7365 6c66 2e63 773a 0a20 2020   if self.cw:.   
+0000c780: 2020 2020 2020 2020 2023 2069 6620 7365           # if se
+0000c790: 6c66 2e70 7265 6665 7265 6e63 652e 6765  lf.preference.ge
+0000c7a0: 7428 2273 656e 645f 6e31 6d6d 5f70 6163  t("send_n1mm_pac
+0000c7b0: 6b65 7473 2229 3a0a 2020 2020 2020 2020  kets"):.        
+0000c7c0: 2020 2020 2320 2020 2020 7365 6c66 2e6e      #     self.n
+0000c7d0: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
+0000c7e0: 4675 6e63 7469 6f6e 4b65 7943 6170 7469  FunctionKeyCapti
+0000c7f0: 6f6e 225d 203d 2073 656c 662e 4631 2e74  on"] = self.F1.t
+0000c800: 6578 7428 290a 2020 2020 2020 2020 2020  ext().          
+0000c810: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
+0000c820: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
+0000c830: 6372 6f28 7365 6c66 2e46 312e 746f 6f6c  cro(self.F1.tool
+0000c840: 5469 7028 2929 290a 0a20 2020 2064 6566  Tip()))..    def
+0000c850: 2073 656e 6466 3228 7365 6c66 293a 0a20   sendf2(self):. 
+0000c860: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
+0000c870: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+0000c880: 2e64 6562 7567 2822 4632 2043 6c69 636b  .debug("F2 Click
+0000c890: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
+0000c8a0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+0000c8b0: 2e67 6574 2822 6d6f 6465 2229 2069 6e20  .get("mode") in 
+0000c8c0: 5b22 4c53 4222 2c20 2255 5342 222c 2022  ["LSB", "USB", "
+0000c8d0: 5353 4222 5d3a 0a20 2020 2020 2020 2020  SSB"]:.         
+0000c8e0: 2020 2073 656c 662e 766f 6963 655f 7374     self.voice_st
+0000c8f0: 7269 6e67 2873 656c 662e 7072 6f63 6573  ring(self.proces
+0000c900: 735f 6d61 6372 6f28 7365 6c66 2e46 322e  s_macro(self.F2.
+0000c910: 746f 6f6c 5469 7028 2929 290a 2020 2020  toolTip())).    
+0000c920: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000c930: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0000c940: 773a 0a20 2020 2020 2020 2020 2020 2073  w:.            s
+0000c950: 656c 662e 6377 2e73 656e 6463 7728 7365  elf.cw.sendcw(se
+0000c960: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
+0000c970: 2873 656c 662e 4632 2e74 6f6f 6c54 6970  (self.F2.toolTip
+0000c980: 2829 2929 0a0a 2020 2020 6465 6620 7365  ()))..    def se
+0000c990: 6e64 6633 2873 656c 6629 3a0a 2020 2020  ndf3(self):.    
+0000c9a0: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
+0000c9b0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000c9c0: 6275 6728 2246 3320 436c 6963 6b65 6422  bug("F3 Clicked"
+0000c9d0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000c9e0: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+0000c9f0: 7428 226d 6f64 6522 2920 696e 205b 224c  t("mode") in ["L
+0000ca00: 5342 222c 2022 5553 4222 2c20 2253 5342  SB", "USB", "SSB
+0000ca10: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+0000ca20: 7365 6c66 2e76 6f69 6365 5f73 7472 696e  self.voice_strin
+0000ca30: 6728 7365 6c66 2e70 726f 6365 7373 5f6d  g(self.process_m
+0000ca40: 6163 726f 2873 656c 662e 4633 2e74 6f6f  acro(self.F3.too
+0000ca50: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
+0000ca60: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000ca70: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
+0000ca80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ca90: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
+0000caa0: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000cab0: 6c66 2e46 332e 746f 6f6c 5469 7028 2929  lf.F3.toolTip())
+0000cac0: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
+0000cad0: 3428 7365 6c66 293a 0a20 2020 2020 2020  4(self):.       
+0000cae0: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000caf0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000cb00: 2822 4634 2043 6c69 636b 6564 2229 0a20  ("F4 Clicked"). 
+0000cb10: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0000cb20: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
+0000cb30: 6d6f 6465 2229 2069 6e20 5b22 4c53 4222  mode") in ["LSB"
+0000cb40: 2c20 2255 5342 222c 2022 5353 4222 5d3a  , "USB", "SSB"]:
+0000cb50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000cb60: 662e 766f 6963 655f 7374 7269 6e67 2873  f.voice_string(s
+0000cb70: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
+0000cb80: 6f28 7365 6c66 2e46 342e 746f 6f6c 5469  o(self.F4.toolTi
+0000cb90: 7028 2929 290a 2020 2020 2020 2020 2020  p())).          
+0000cba0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0000cbb0: 2069 6620 7365 6c66 2e63 773a 0a20 2020   if self.cw:.   
+0000cbc0: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
+0000cbd0: 2e73 656e 6463 7728 7365 6c66 2e70 726f  .sendcw(self.pro
+0000cbe0: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
+0000cbf0: 4634 2e74 6f6f 6c54 6970 2829 2929 0a0a  F4.toolTip()))..
+0000cc00: 2020 2020 6465 6620 7365 6e64 6635 2873      def sendf5(s
+0000cc10: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000cc20: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
+0000cc30: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
+0000cc40: 3520 436c 6963 6b65 6422 290a 2020 2020  5 Clicked").    
+0000cc50: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
+0000cc60: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
+0000cc70: 6522 2920 696e 205b 224c 5342 222c 2022  e") in ["LSB", "
+0000cc80: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
+0000cc90: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
+0000cca0: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
+0000ccb0: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
+0000ccc0: 656c 662e 4635 2e74 6f6f 6c54 6970 2829  elf.F5.toolTip()
+0000ccd0: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+0000cce0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+0000ccf0: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
+0000cd00: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+0000cd10: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
+0000cd20: 735f 6d61 6372 6f28 7365 6c66 2e46 352e  s_macro(self.F5.
+0000cd30: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
+0000cd40: 2064 6566 2073 656e 6466 3628 7365 6c66   def sendf6(self
+0000cd50: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+0000cd60: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+0000cd70: 6767 6572 2e64 6562 7567 2822 4636 2043  gger.debug("F6 C
+0000cd80: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
+0000cd90: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
+0000cda0: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
+0000cdb0: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
+0000cdc0: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
+0000cdd0: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
+0000cde0: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
+0000cdf0: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000ce00: 2e46 362e 746f 6f6c 5469 7028 2929 290a  .F6.toolTip())).
+0000ce10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000ce20: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
+0000ce30: 6c66 2e63 773a 0a20 2020 2020 2020 2020  lf.cw:.         
+0000ce40: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
+0000ce50: 7728 7365 6c66 2e70 726f 6365 7373 5f6d  w(self.process_m
+0000ce60: 6163 726f 2873 656c 662e 4636 2e74 6f6f  acro(self.F6.too
+0000ce70: 6c54 6970 2829 2929 0a0a 2020 2020 6465  lTip()))..    de
+0000ce80: 6620 7365 6e64 6637 2873 656c 6629 3a0a  f sendf7(self):.
+0000ce90: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
+0000cea0: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
+0000ceb0: 722e 6465 6275 6728 2246 3720 436c 6963  r.debug("F7 Clic
+0000cec0: 6b65 6422 290a 2020 2020 2020 2020 6966  ked").        if
+0000ced0: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+0000cee0: 652e 6765 7428 226d 6f64 6522 2920 696e  e.get("mode") in
+0000cef0: 205b 224c 5342 222c 2022 5553 4222 2c20   ["LSB", "USB", 
+0000cf00: 2253 5342 225d 3a0a 2020 2020 2020 2020  "SSB"]:.        
+0000cf10: 2020 2020 7365 6c66 2e76 6f69 6365 5f73      self.voice_s
+0000cf20: 7472 696e 6728 7365 6c66 2e70 726f 6365  tring(self.proce
+0000cf30: 7373 5f6d 6163 726f 2873 656c 662e 4637  ss_macro(self.F7
+0000cf40: 2e74 6f6f 6c54 6970 2829 2929 0a20 2020  .toolTip())).   
+0000cf50: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0000cf60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000cf70: 6377 3a0a 2020 2020 2020 2020 2020 2020  cw:.            
+0000cf80: 7365 6c66 2e63 772e 7365 6e64 6377 2873  self.cw.sendcw(s
+0000cf90: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
+0000cfa0: 6f28 7365 6c66 2e46 372e 746f 6f6c 5469  o(self.F7.toolTi
+0000cfb0: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
+0000cfc0: 656e 6466 3828 7365 6c66 293a 0a20 2020  endf8(self):.   
+0000cfd0: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000cfe0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000cff0: 6562 7567 2822 4638 2043 6c69 636b 6564  ebug("F8 Clicked
+0000d000: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
+0000d010: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+0000d020: 6574 2822 6d6f 6465 2229 2069 6e20 5b22  et("mode") in ["
+0000d030: 4c53 4222 2c20 2255 5342 222c 2022 5353  LSB", "USB", "SS
+0000d040: 4222 5d3a 0a20 2020 2020 2020 2020 2020  B"]:.           
+0000d050: 2073 656c 662e 766f 6963 655f 7374 7269   self.voice_stri
+0000d060: 6e67 2873 656c 662e 7072 6f63 6573 735f  ng(self.process_
+0000d070: 6d61 6372 6f28 7365 6c66 2e46 382e 746f  macro(self.F8.to
+0000d080: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
+0000d090: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+0000d0a0: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
+0000d0b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d0c0: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
+0000d0d0: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
+0000d0e0: 656c 662e 4638 2e74 6f6f 6c54 6970 2829  elf.F8.toolTip()
+0000d0f0: 2929 0a0a 2020 2020 6465 6620 7365 6e64  ))..    def send
+0000d100: 6639 2873 656c 6629 3a0a 2020 2020 2020  f9(self):.      
+0000d110: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
+0000d120: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000d130: 6728 2246 3920 436c 6963 6b65 6422 290a  g("F9 Clicked").
+0000d140: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000d150: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+0000d160: 226d 6f64 6522 2920 696e 205b 224c 5342  "mode") in ["LSB
+0000d170: 222c 2022 5553 4222 2c20 2253 5342 225d  ", "USB", "SSB"]
+0000d180: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000d190: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
+0000d1a0: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
+0000d1b0: 726f 2873 656c 662e 4639 2e74 6f6f 6c54  ro(self.F9.toolT
+0000d1c0: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
+0000d1d0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000d1e0: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
+0000d1f0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000d200: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
+0000d210: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000d220: 2e46 392e 746f 6f6c 5469 7028 2929 290a  .F9.toolTip())).
+0000d230: 0a20 2020 2064 6566 2073 656e 6466 3130  .    def sendf10
+0000d240: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000d250: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
+0000d260: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000d270: 2246 3130 2043 6c69 636b 6564 2229 0a20  "F10 Clicked"). 
+0000d280: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0000d290: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
+0000d2a0: 6d6f 6465 2229 2069 6e20 5b22 4c53 4222  mode") in ["LSB"
+0000d2b0: 2c20 2255 5342 222c 2022 5353 4222 5d3a  , "USB", "SSB"]:
+0000d2c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d2d0: 662e 766f 6963 655f 7374 7269 6e67 2873  f.voice_string(s
+0000d2e0: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
+0000d2f0: 6f28 7365 6c66 2e46 3130 2e74 6f6f 6c54  o(self.F10.toolT
+0000d300: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
+0000d310: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000d320: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
+0000d330: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000d340: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
+0000d350: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000d360: 2e46 3130 2e74 6f6f 6c54 6970 2829 2929  .F10.toolTip()))
+0000d370: 0a0a 2020 2020 6465 6620 7365 6e64 6631  ..    def sendf1
+0000d380: 3128 7365 6c66 293a 0a20 2020 2020 2020  1(self):.       
+0000d390: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000d3a0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000d3b0: 2822 4631 3120 436c 6963 6b65 6422 290a  ("F11 Clicked").
+0000d3c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000d3d0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+0000d3e0: 226d 6f64 6522 2920 696e 205b 224c 5342  "mode") in ["LSB
+0000d3f0: 222c 2022 5553 4222 2c20 2253 5342 225d  ", "USB", "SSB"]
+0000d400: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000d410: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
+0000d420: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
+0000d430: 726f 2873 656c 662e 4631 312e 746f 6f6c  ro(self.F11.tool
+0000d440: 5469 7028 2929 290a 2020 2020 2020 2020  Tip())).        
+0000d450: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0000d460: 2020 2069 6620 7365 6c66 2e63 773a 0a20     if self.cw:. 
+0000d470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d480: 6377 2e73 656e 6463 7728 7365 6c66 2e70  cw.sendcw(self.p
+0000d490: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
+0000d4a0: 662e 4631 312e 746f 6f6c 5469 7028 2929  f.F11.toolTip())
+0000d4b0: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
+0000d4c0: 3132 2873 656c 6629 3a0a 2020 2020 2020  12(self):.      
+0000d4d0: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
+0000d4e0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000d4f0: 6728 2246 3132 2043 6c69 636b 6564 2229  g("F12 Clicked")
+0000d500: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000d510: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+0000d520: 2822 6d6f 6465 2229 2069 6e20 5b22 4c53  ("mode") in ["LS
+0000d530: 4222 2c20 2255 5342 222c 2022 5353 4222  B", "USB", "SSB"
+0000d540: 5d3a 0a20 2020 2020 2020 2020 2020 2073  ]:.            s
+0000d550: 656c 662e 766f 6963 655f 7374 7269 6e67  elf.voice_string
+0000d560: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
+0000d570: 6372 6f28 7365 6c66 2e46 3132 2e74 6f6f  cro(self.F12.too
+0000d580: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
+0000d590: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000d5a0: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
+0000d5b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d5c0: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
+0000d5d0: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000d5e0: 6c66 2e46 3132 2e74 6f6f 6c54 6970 2829  lf.F12.toolTip()
+0000d5f0: 2929 0a0a 2020 2020 6465 6620 7275 6e5f  ))..    def run_
+0000d600: 7370 5f62 7574 746f 6e73 5f63 6c69 636b  sp_buttons_click
+0000d610: 6564 2873 656c 6629 3a0a 2020 2020 2020  ed(self):.      
+0000d620: 2020 2222 2248 616e 646c 6520 7275 6e2f    """Handle run/
+0000d630: 7326 7020 6d6f 6465 2222 220a 2020 2020  s&p mode""".    
+0000d640: 2020 2020 7365 6c66 2e70 7265 665b 2272      self.pref["r
+0000d650: 756e 5f73 7461 7465 225d 203d 2073 656c  un_state"] = sel
+0000d660: 662e 7261 6469 6f42 7574 746f 6e5f 7275  f.radioButton_ru
+0000d670: 6e2e 6973 4368 6563 6b65 6428 290a 2020  n.isChecked().  
+0000d680: 2020 2020 2020 7365 6c66 2e77 7269 7465        self.write
+0000d690: 5f70 7265 6665 7265 6e63 6528 290a 2020  _preference().  
+0000d6a0: 2020 2020 2020 7365 6c66 2e72 6561 645f        self.read_
+0000d6b0: 6377 5f6d 6163 726f 7328 290a 0a20 2020  cw_macros()..   
+0000d6c0: 2064 6566 2077 7269 7465 5f70 7265 6665   def write_prefe
+0000d6d0: 7265 6e63 6528 7365 6c66 293a 0a20 2020  rence(self):.   
+0000d6e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000d6f0: 2057 7269 7465 2070 7265 6665 7265 6e63   Write preferenc
+0000d700: 6573 2074 6f20 6a73 6f6e 2066 696c 652e  es to json file.
+0000d710: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d720: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0000d730: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+0000d740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d750: 2043 4f4e 4649 475f 5041 5448 202b 2022   CONFIG_PATH + "
+0000d760: 2f6e 6f74 316d 6d2e 6a73 6f6e 222c 2022  /not1mm.json", "
+0000d770: 7774 222c 2065 6e63 6f64 696e 673d 2275  wt", encoding="u
+0000d780: 7466 2d38 220a 2020 2020 2020 2020 2020  tf-8".          
+0000d790: 2020 2920 6173 2066 696c 655f 6465 7363    ) as file_desc
+0000d7a0: 7269 7074 6f72 3a0a 2020 2020 2020 2020  riptor:.        
+0000d7b0: 2020 2020 2020 2020 6669 6c65 5f64 6573          file_des
+0000d7c0: 6372 6970 746f 722e 7772 6974 6528 6475  criptor.write(du
+0000d7d0: 6d70 7328 7365 6c66 2e70 7265 662c 2069  mps(self.pref, i
+0000d7e0: 6e64 656e 743d 3429 290a 2020 2020 2020  ndent=4)).      
+0000d7f0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000d800: 2e69 6e66 6f28 2277 7269 7469 6e67 3a20  .info("writing: 
+0000d810: 2573 222c 2073 656c 662e 7072 6566 290a  %s", self.pref).
+0000d820: 2020 2020 2020 2020 6578 6365 7074 2049          except I
+0000d830: 4f45 7272 6f72 2061 7320 6578 6365 7074  OError as except
+0000d840: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+0000d850: 206c 6f67 6765 722e 6372 6974 6963 616c   logger.critical
+0000d860: 2822 7772 6974 6570 7265 6665 7265 6e63  ("writepreferenc
+0000d870: 6573 3a20 2573 222c 2065 7863 6570 7469  es: %s", excepti
+0000d880: 6f6e 290a 0a20 2020 2064 6566 2072 6561  on)..    def rea
+0000d890: 6470 7265 6665 7265 6e63 6573 2873 656c  dpreferences(sel
+0000d8a0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+0000d8b0: 2020 2020 2020 2020 5265 7374 6f72 6520          Restore 
+0000d8c0: 7072 6566 6572 656e 6365 7320 6966 2074  preferences if t
+0000d8d0: 6865 7920 6578 6973 742c 206f 7468 6572  hey exist, other
+0000d8e0: 7769 7365 2063 7265 6174 6520 736f 6d65  wise create some
+0000d8f0: 2073 616e 6520 6465 6661 756c 7473 2e0a   sane defaults..
+0000d900: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000d910: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000d920: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
+0000d930: 6578 6973 7473 2843 4f4e 4649 475f 5041  exists(CONFIG_PA
+0000d940: 5448 202b 2022 2f6e 6f74 316d 6d2e 6a73  TH + "/not1mm.js
+0000d950: 6f6e 2229 3a0a 2020 2020 2020 2020 2020  on"):.          
+0000d960: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+0000d970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d980: 2020 2020 2043 4f4e 4649 475f 5041 5448       CONFIG_PATH
+0000d990: 202b 2022 2f6e 6f74 316d 6d2e 6a73 6f6e   + "/not1mm.json
+0000d9a0: 222c 2022 7274 222c 2065 6e63 6f64 696e  ", "rt", encodin
+0000d9b0: 673d 2275 7466 2d38 220a 2020 2020 2020  g="utf-8".      
+0000d9c0: 2020 2020 2020 2020 2020 2920 6173 2066            ) as f
+0000d9d0: 696c 655f 6465 7363 7269 7074 6f72 3a0a  ile_descriptor:.
+0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9f0: 2020 2020 7365 6c66 2e70 7265 6620 3d20      self.pref = 
+0000da00: 6c6f 6164 7328 6669 6c65 5f64 6573 6372  loads(file_descr
+0000da10: 6970 746f 722e 7265 6164 2829 290a 2020  iptor.read()).  
+0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da30: 2020 6c6f 6767 6572 2e69 6e66 6f28 2225    logger.info("%
+0000da40: 7322 2c20 7365 6c66 2e70 7265 6629 0a20  s", self.pref). 
+0000da50: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000da60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000da70: 206c 6f67 6765 722e 696e 666f 2822 4e6f   logger.info("No
+0000da80: 2070 7265 6665 7265 6e63 6520 6669 6c65   preference file
+0000da90: 2e20 5772 6974 696e 6720 7072 6566 6572  . Writing prefer
+0000daa0: 656e 6365 2e22 290a 2020 2020 2020 2020  ence.").        
+0000dab0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+0000dac0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+0000dad0: 2020 2020 2020 2043 4f4e 4649 475f 5041         CONFIG_PA
+0000dae0: 5448 202b 2022 2f6e 6f74 316d 6d2e 6a73  TH + "/not1mm.js
+0000daf0: 6f6e 222c 2022 7774 222c 2065 6e63 6f64  on", "wt", encod
+0000db00: 696e 673d 2275 7466 2d38 220a 2020 2020  ing="utf-8".    
+0000db10: 2020 2020 2020 2020 2020 2020 2920 6173              ) as
+0000db20: 2066 696c 655f 6465 7363 7269 7074 6f72   file_descriptor
+0000db30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000db40: 2020 2020 2020 7365 6c66 2e70 7265 6620        self.pref 
+0000db50: 3d20 7365 6c66 2e70 7265 665f 7265 662e  = self.pref_ref.
+0000db60: 636f 7079 2829 0a20 2020 2020 2020 2020  copy().         
+0000db70: 2020 2020 2020 2020 2020 2066 696c 655f             file_
+0000db80: 6465 7363 7269 7074 6f72 2e77 7269 7465  descriptor.write
+0000db90: 2864 756d 7073 2873 656c 662e 7072 6566  (dumps(self.pref
+0000dba0: 2c20 696e 6465 6e74 3d34 2929 0a20 2020  , indent=4)).   
+0000dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbc0: 206c 6f67 6765 722e 696e 666f 2822 2573   logger.info("%s
+0000dbd0: 222c 2073 656c 662e 7072 6566 290a 2020  ", self.pref).  
+0000dbe0: 2020 2020 2020 6578 6365 7074 2049 4f45        except IOE
+0000dbf0: 7272 6f72 2061 7320 6578 6365 7074 696f  rror as exceptio
+0000dc00: 6e3a 0a20 2020 2020 2020 2020 2020 206c  n:.            l
+0000dc10: 6f67 6765 722e 6372 6974 6963 616c 2822  ogger.critical("
+0000dc20: 4572 726f 723a 2025 7322 2c20 6578 6365  Error: %s", exce
+0000dc30: 7074 696f 6e29 0a0a 2020 2020 2020 2020  ption)..        
+0000dc40: 7365 6c66 2e6c 6f6f 6b5f 7570 203d 204e  self.look_up = N
+0000dc50: 6f6e 650a 2020 2020 2020 2020 6966 2073  one.        if s
+0000dc60: 656c 662e 7072 6566 2e67 6574 2822 7573  elf.pref.get("us
+0000dc70: 6571 727a 2229 3a0a 2020 2020 2020 2020  eqrz"):.        
+0000dc80: 2020 2020 7365 6c66 2e6c 6f6f 6b5f 7570      self.look_up
+0000dc90: 203d 2051 525a 6c6f 6f6b 7570 280a 2020   = QRZlookup(.  
+0000dca0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000dcb0: 6c66 2e70 7265 662e 6765 7428 226c 6f6f  lf.pref.get("loo
+0000dcc0: 6b75 7075 7365 726e 616d 6522 292c 0a20  kupusername"),. 
+0000dcd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000dce0: 656c 662e 7072 6566 2e67 6574 2822 6c6f  elf.pref.get("lo
+0000dcf0: 6f6b 7570 7061 7373 776f 7264 2229 2c0a  okuppassword"),.
+0000dd00: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000dd10: 2020 2020 2020 2320 6966 2073 656c 662e        # if self.
+0000dd20: 7072 6566 2e67 6574 2822 7573 6568 616d  pref.get("useham
+0000dd30: 6462 2229 3a0a 2020 2020 2020 2020 2320  db"):.        # 
+0000dd40: 2020 2020 7365 6c66 2e6c 6f6f 6b5f 7570      self.look_up
+0000dd50: 203d 2048 616d 4442 6c6f 6f6b 7570 2829   = HamDBlookup()
+0000dd60: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000dd70: 2e70 7265 662e 6765 7428 2275 7365 6861  .pref.get("useha
+0000dd80: 6d71 7468 2229 3a0a 2020 2020 2020 2020  mqth"):.        
+0000dd90: 2020 2020 7365 6c66 2e6c 6f6f 6b5f 7570      self.look_up
+0000dda0: 203d 2048 616d 5154 4828 0a20 2020 2020   = HamQTH(.     
+0000ddb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ddc0: 7072 6566 2e67 6574 2822 6c6f 6f6b 7570  pref.get("lookup
+0000ddd0: 7573 6572 6e61 6d65 2229 2c0a 2020 2020  username"),.    
+0000dde0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ddf0: 2e70 7265 662e 6765 7428 226c 6f6f 6b75  .pref.get("looku
+0000de00: 7070 6173 7377 6f72 6422 292c 0a20 2020  ppassword"),.   
+0000de10: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000de20: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
+0000de30: 2e67 6574 2822 7275 6e5f 7374 6174 6522  .get("run_state"
+0000de40: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000de50: 656c 662e 7261 6469 6f42 7574 746f 6e5f  elf.radioButton_
+0000de60: 7275 6e2e 7365 7443 6865 636b 6564 2854  run.setChecked(T
+0000de70: 7275 6529 0a20 2020 2020 2020 2065 6c73  rue).        els
+0000de80: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000de90: 656c 662e 7261 6469 6f42 7574 746f 6e5f  elf.radioButton_
+0000dea0: 7370 2e73 6574 4368 6563 6b65 6428 5472  sp.setChecked(Tr
+0000deb0: 7565 290a 0a20 2020 2020 2020 2069 6620  ue)..        if 
+0000dec0: 7365 6c66 2e70 7265 662e 6765 7428 2264  self.pref.get("d
+0000ded0: 6172 6b5f 6d6f 6465 2229 3a0a 2020 2020  ark_mode"):.    
+0000dee0: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+0000def0: 696f 6e44 6172 6b5f 4d6f 6465 2e73 6574  ionDark_Mode.set
+0000df00: 4368 6563 6b65 6428 5472 7565 290a 2020  Checked(True).  
+0000df10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000df20: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+0000df30: 696f 6e44 6172 6b5f 4d6f 6465 2e73 6574  ionDark_Mode.set
+0000df40: 4368 6563 6b65 6428 4661 6c73 6529 0a0a  Checked(False)..
+0000df50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000df60: 7072 6566 2e67 6574 2822 636f 6d6d 616e  pref.get("comman
+0000df70: 645f 6275 7474 6f6e 7322 293a 0a20 2020  d_buttons"):.   
+0000df80: 2020 2020 2020 2020 2073 656c 662e 6163           self.ac
+0000df90: 7469 6f6e 436f 6d6d 616e 645f 4275 7474  tionCommand_Butt
+0000dfa0: 6f6e 732e 7365 7443 6865 636b 6564 2854  ons.setChecked(T
+0000dfb0: 7275 6529 0a20 2020 2020 2020 2065 6c73  rue).        els
+0000dfc0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000dfd0: 656c 662e 6163 7469 6f6e 436f 6d6d 616e  elf.actionComman
+0000dfe0: 645f 4275 7474 6f6e 732e 7365 7443 6865  d_Buttons.setChe
+0000dff0: 636b 6564 2846 616c 7365 290a 0a20 2020  cked(False)..   
+0000e000: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
+0000e010: 662e 6765 7428 2263 775f 6d61 6372 6f73  f.get("cw_macros
+0000e020: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+0000e030: 7365 6c66 2e61 6374 696f 6e43 575f 4d61  self.actionCW_Ma
+0000e040: 6372 6f73 2e73 6574 4368 6563 6b65 6428  cros.setChecked(
+0000e050: 5472 7565 290a 2020 2020 2020 2020 656c  True).        el
+0000e060: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000e070: 7365 6c66 2e61 6374 696f 6e43 575f 4d61  self.actionCW_Ma
+0000e080: 6372 6f73 2e73 6574 4368 6563 6b65 6428  cros.setChecked(
+0000e090: 4661 6c73 6529 0a0a 2020 2020 2020 2020  False)..        
+0000e0a0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
+0000e0b0: 2822 6261 6e64 735f 6d6f 6465 7322 293a  ("bands_modes"):
+0000e0c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000e0d0: 662e 6163 7469 6f6e 4d6f 6465 5f61 6e64  f.actionMode_and
+0000e0e0: 5f42 616e 6473 2e73 6574 4368 6563 6b65  _Bands.setChecke
+0000e0f0: 6428 5472 7565 290a 2020 2020 2020 2020  d(True).        
+0000e100: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000e110: 2020 7365 6c66 2e61 6374 696f 6e4d 6f64    self.actionMod
+0000e120: 655f 616e 645f 4261 6e64 732e 7365 7443  e_and_Bands.setC
+0000e130: 6865 636b 6564 2846 616c 7365 290a 0a20  hecked(False).. 
+0000e140: 2020 2020 2020 206d 756c 7469 6361 7374         multicast
+0000e150: 5f67 726f 7570 203d 2073 656c 662e 7072  _group = self.pr
+0000e160: 6566 2e67 6574 2822 6d75 6c74 6963 6173  ef.get("multicas
+0000e170: 745f 6772 6f75 7022 2c20 2232 3234 2e31  t_group", "224.1
+0000e180: 2e31 2e31 2229 0a20 2020 2020 2020 206d  .1.1").        m
+0000e190: 756c 7469 6361 7374 5f70 6f72 7420 3d20  ulticast_port = 
+0000e1a0: 7365 6c66 2e70 7265 662e 6765 7428 226d  self.pref.get("m
+0000e1b0: 756c 7469 6361 7374 5f70 6f72 7422 2c20  ulticast_port", 
+0000e1c0: 3232 3339 290a 2020 2020 2020 2020 696e  2239).        in
+0000e1d0: 7465 7266 6163 655f 6970 203d 2073 656c  terface_ip = sel
+0000e1e0: 662e 7072 6566 2e67 6574 2822 696e 7465  f.pref.get("inte
+0000e1f0: 7266 6163 655f 6970 222c 2022 302e 302e  rface_ip", "0.0.
+0000e200: 302e 3022 290a 2020 2020 2020 2020 7365  0.0").        se
+0000e210: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
+0000e220: 6572 6661 6365 203d 204d 756c 7469 6361  erface = Multica
+0000e230: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
+0000e240: 6d75 6c74 6963 6173 745f 6772 6f75 702c  multicast_group,
+0000e250: 206d 756c 7469 6361 7374 5f70 6f72 742c   multicast_port,
+0000e260: 2069 6e74 6572 6661 6365 5f69 700a 2020   interface_ip.  
+0000e270: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000e280: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+0000e290: 6c20 3d20 4e6f 6e65 0a0a 2020 2020 2020  l = None..      
+0000e2a0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
+0000e2b0: 6574 2822 7573 6566 6c72 6967 222c 2046  et("useflrig", F
+0000e2c0: 616c 7365 293a 0a20 2020 2020 2020 2020  alse):.         
+0000e2d0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000e2e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e2f0: 2022 5573 696e 6720 666c 7269 673a 2025   "Using flrig: %
+0000e300: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+0000e310: 2020 2020 6622 7b73 656c 662e 7072 6566      f"{self.pref
+0000e320: 2e67 6574 2827 4341 545f 6970 2729 7d20  .get('CAT_ip')} 
+0000e330: 7b73 656c 662e 7072 6566 2e67 6574 2827  {self.pref.get('
+0000e340: 4341 545f 706f 7274 2729 7d22 2c0a 2020  CAT_port')}",.  
+0000e350: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000e360: 2020 2020 2020 2020 7365 6c66 2e72 6967          self.rig
+0000e370: 5f63 6f6e 7472 6f6c 203d 2043 4154 280a  _control = CAT(.
+0000e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e390: 2266 6c72 6967 222c 0a20 2020 2020 2020  "flrig",.       
+0000e3a0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000e3b0: 6566 2e67 6574 2822 4341 545f 6970 222c  ef.get("CAT_ip",
+0000e3c0: 2022 3132 372e 302e 302e 3122 292c 0a20   "127.0.0.1"),. 
+0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000e3e0: 6e74 2873 656c 662e 7072 6566 2e67 6574  nt(self.pref.get
+0000e3f0: 2822 4341 545f 706f 7274 222c 2031 3233  ("CAT_port", 123
+0000e400: 3435 2929 2c0a 2020 2020 2020 2020 2020  45)),.          
+0000e410: 2020 290a 2020 2020 2020 2020 6966 2073    ).        if s
+0000e420: 656c 662e 7072 6566 2e67 6574 2822 7573  elf.pref.get("us
+0000e430: 6572 6967 6374 6c64 222c 2046 616c 7365  erigctld", False
+0000e440: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
+0000e450: 6f67 6765 722e 6465 6275 6728 0a20 2020  ogger.debug(.   
+0000e460: 2020 2020 2020 2020 2020 2020 2022 5573               "Us
+0000e470: 696e 6720 7269 6763 746c 643a 2025 7322  ing rigctld: %s"
+0000e480: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e490: 2020 6622 7b73 656c 662e 7072 6566 2e67    f"{self.pref.g
+0000e4a0: 6574 2827 4341 545f 6970 2729 7d20 7b73  et('CAT_ip')} {s
+0000e4b0: 656c 662e 7072 6566 2e67 6574 2827 4341  elf.pref.get('CA
+0000e4c0: 545f 706f 7274 2729 7d22 2c0a 2020 2020  T_port')}",.    
+0000e4d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000e4e0: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
+0000e4f0: 6f6e 7472 6f6c 203d 2043 4154 280a 2020  ontrol = CAT(.  
+0000e500: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+0000e510: 6967 6374 6c64 222c 0a20 2020 2020 2020  igctld",.       
+0000e520: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000e530: 6566 2e67 6574 2822 4341 545f 6970 222c  ef.get("CAT_ip",
+0000e540: 2022 3132 372e 302e 302e 3122 292c 0a20   "127.0.0.1"),. 
+0000e550: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000e560: 6e74 2873 656c 662e 7072 6566 2e67 6574  nt(self.pref.get
+0000e570: 2822 4341 545f 706f 7274 222c 2034 3533  ("CAT_port", 453
+0000e580: 3229 292c 0a20 2020 2020 2020 2020 2020  2)),.           
+0000e590: 2029 0a0a 2020 2020 2020 2020 6966 2073   )..        if s
+0000e5a0: 656c 662e 7072 6566 2e67 6574 2822 6377  elf.pref.get("cw
+0000e5b0: 7479 7065 222c 2030 2920 3d3d 2030 3a0a  type", 0) == 0:.
+0000e5c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e5d0: 2e63 7720 3d20 4e6f 6e65 0a20 2020 2020  .cw = None.     
+0000e5e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000e5f0: 2020 2020 2073 656c 662e 6377 203d 2043       self.cw = C
+0000e600: 5728 0a20 2020 2020 2020 2020 2020 2020  W(.             
+0000e610: 2020 2069 6e74 2873 656c 662e 7072 6566     int(self.pref
+0000e620: 2e67 6574 2822 6377 7479 7065 2229 292c  .get("cwtype")),
+0000e630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e640: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+0000e650: 6377 6970 2229 2c0a 2020 2020 2020 2020  cwip"),.        
+0000e660: 2020 2020 2020 2020 696e 7428 7365 6c66          int(self
+0000e670: 2e70 7265 662e 6765 7428 2263 7770 6f72  .pref.get("cwpor
+0000e680: 7422 2c20 3637 3839 2929 2c0a 2020 2020  t", 6789)),.    
+0000e690: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000e6a0: 2020 2020 2020 7365 6c66 2e63 772e 7370        self.cw.sp
+0000e6b0: 6565 6420 3d20 3230 0a0a 2020 2020 2020  eed = 20..      
+0000e6c0: 2020 7365 6c66 2e64 6172 6b5f 6d6f 6465    self.dark_mode
+0000e6d0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000e6e0: 7368 6f77 5f63 6f6d 6d61 6e64 5f62 7574  show_command_but
+0000e6f0: 746f 6e73 2829 0a20 2020 2020 2020 2073  tons().        s
+0000e700: 656c 662e 7368 6f77 5f43 575f 6d61 6372  elf.show_CW_macr
+0000e710: 6f73 2829 0a20 2020 2020 2020 2023 2073  os().        # s
+0000e720: 656c 662e 7368 6f77 5f62 616e 645f 6d6f  elf.show_band_mo
+0000e730: 6465 2829 0a0a 2020 2020 6465 6620 7761  de()..    def wa
+0000e740: 7463 685f 7564 7028 7365 6c66 293a 0a20  tch_udp(self):. 
+0000e750: 2020 2020 2020 2022 2222 5075 7473 2055         """Puts U
+0000e760: 4450 2064 6174 6167 7261 6d73 2069 6e20  DP datagrams in 
+0000e770: 6120 4649 464f 2071 7565 7565 2222 220a  a FIFO queue""".
+0000e780: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
+0000e790: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+0000e7a0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000e7b0: 2020 2020 2064 6174 6167 7261 6d20 3d20       datagram = 
+0000e7c0: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+0000e7d0: 6e74 6572 6661 6365 2e73 6572 7665 725f  nterface.server_
+0000e7e0: 7564 702e 7265 6376 2831 3530 3029 0a20  udp.recv(1500). 
+0000e7f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000e800: 6f67 6765 722e 6465 6275 6728 6461 7461  ogger.debug(data
+0000e810: 6772 616d 2e64 6563 6f64 6528 2929 0a20  gram.decode()). 
+0000e820: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+0000e830: 7420 736f 636b 6574 2e74 696d 656f 7574  t socket.timeout
+0000e840: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e850: 2020 7469 6d65 2e73 6c65 6570 2830 2e31    time.sleep(0.1
+0000e860: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000e870: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+0000e880: 2020 2020 2020 2069 6620 6461 7461 6772         if datagr
+0000e890: 616d 3a0a 2020 2020 2020 2020 2020 2020  am:.            
+0000e8a0: 2020 2020 7365 6c66 2e75 6470 5f66 6966      self.udp_fif
+0000e8b0: 6f2e 7075 7428 6461 7461 6772 616d 290a  o.put(datagram).
+0000e8c0: 0a20 2020 2064 6566 2063 6865 636b 5f75  .    def check_u
+0000e8d0: 6470 5f74 7261 6666 6963 2873 656c 6629  dp_traffic(self)
+0000e8e0: 3a0a 2020 2020 2020 2020 2222 2243 6865  :.        """Che
+0000e8f0: 636b 7320 5544 5020 5472 6166 6669 6322  cks UDP Traffic"
+0000e900: 2222 0a20 2020 2020 2020 2077 6869 6c65  "".        while
+0000e910: 206e 6f74 2073 656c 662e 7564 705f 6669   not self.udp_fi
+0000e920: 666f 2e65 6d70 7479 2829 3a0a 2020 2020  fo.empty():.    
+0000e930: 2020 2020 2020 2020 6461 7461 6772 616d          datagram
+0000e940: 203d 2073 656c 662e 7564 705f 6669 666f   = self.udp_fifo
+0000e950: 2e67 6574 2829 0a20 2020 2020 2020 2020  .get().         
+0000e960: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000e970: 2020 2020 2020 2020 6465 6275 675f 696e          debug_in
+0000e980: 666f 203d 2066 227b 6461 7461 6772 616d  fo = f"{datagram
+0000e990: 2e64 6563 6f64 6528 297d 220a 2020 2020  .decode()}".    
+0000e9a0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+0000e9b0: 6572 2e64 6562 7567 2864 6562 7567 5f69  er.debug(debug_i
+0000e9c0: 6e66 6f29 0a20 2020 2020 2020 2020 2020  nfo).           
+0000e9d0: 2020 2020 206a 736f 6e5f 6461 7461 203d       json_data =
+0000e9e0: 206c 6f61 6473 2864 6174 6167 7261 6d2e   loads(datagram.
+0000e9f0: 6465 636f 6465 2829 290a 2020 2020 2020  decode()).      
+0000ea00: 2020 2020 2020 6578 6365 7074 2055 6e69        except Uni
+0000ea10: 636f 6465 4465 636f 6465 4572 726f 7220  codeDecodeError 
+0000ea20: 6173 2065 7272 3a0a 2020 2020 2020 2020  as err:.        
+0000ea30: 2020 2020 2020 2020 7468 655f 6572 726f          the_erro
+0000ea40: 7220 3d20 6622 4e6f 7420 556e 6963 6f64  r = f"Not Unicod
+0000ea50: 653a 207b 6572 727d 5c6e 7b64 6174 6167  e: {err}\n{datag
+0000ea60: 7261 6d7d 220a 2020 2020 2020 2020 2020  ram}".          
+0000ea70: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000ea80: 7567 2874 6865 5f65 7272 6f72 290a 2020  ug(the_error).  
+0000ea90: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000eaa0: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+0000eab0: 2020 2065 7863 6570 7420 4a53 4f4e 4465     except JSONDe
+0000eac0: 636f 6465 4572 726f 7220 6173 2065 7272  codeError as err
+0000ead0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000eae0: 2020 7468 655f 6572 726f 7220 3d20 6622    the_error = f"
+0000eaf0: 4e6f 7420 4a53 4f4e 3a20 7b65 7272 7d5c  Not JSON: {err}\
+0000eb00: 6e7b 6461 7461 6772 616d 7d22 0a20 2020  n{datagram}".   
+0000eb10: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+0000eb20: 6765 722e 6465 6275 6728 7468 655f 6572  ger.debug(the_er
+0000eb30: 726f 7229 0a20 2020 2020 2020 2020 2020  ror).           
+0000eb40: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+0000eb50: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
+0000eb60: 2020 2020 2020 2020 2020 2020 2020 206a                 j
+0000eb70: 736f 6e5f 6461 7461 2e67 6574 2822 636d  son_data.get("cm
+0000eb80: 6422 2c20 2222 2920 3d3d 2022 4745 5443  d", "") == "GETC
+0000eb90: 4f4c 554d 4e53 220a 2020 2020 2020 2020  OLUMNS".        
+0000eba0: 2020 2020 2020 2020 616e 6420 6a73 6f6e          and json
+0000ebb0: 5f64 6174 612e 6765 7428 2273 7461 7469  _data.get("stati
+0000ebc0: 6f6e 222c 2022 2229 203d 3d20 706c 6174  on", "") == plat
+0000ebd0: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
+0000ebe0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+0000ebf0: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
+0000ec00: 7361 7474 7228 7365 6c66 2e63 6f6e 7465  sattr(self.conte
+0000ec10: 7374 2c20 2263 6f6c 756d 6e73 2229 3a0a  st, "columns"):.
+0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec30: 2020 2020 636d 6420 3d20 7b7d 0a20 2020      cmd = {}.   
+0000ec40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec50: 2063 6d64 5b22 636d 6422 5d20 3d20 2253   cmd["cmd"] = "S
+0000ec60: 484f 5743 4f4c 554d 4e53 220a 2020 2020  HOWCOLUMNS".    
+0000ec70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec80: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
+0000ec90: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
+0000eca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ecb0: 2020 2020 2063 6d64 5b22 434f 4c55 4d4e       cmd["COLUMN
+0000ecc0: 5322 5d20 3d20 7365 6c66 2e63 6f6e 7465  S"] = self.conte
+0000ecd0: 7374 2e63 6f6c 756d 6e73 0a20 2020 2020  st.columns.     
+0000ece0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ecf0: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
+0000ed00: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
+0000ed10: 6a73 6f6e 2863 6d64 290a 2020 2020 2020  json(cmd).      
+0000ed20: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
+0000ed30: 2020 2020 2020 2020 2020 206a 736f 6e5f             json_
+0000ed40: 6461 7461 2e67 6574 2822 636d 6422 2c20  data.get("cmd", 
+0000ed50: 2222 2920 3d3d 2022 5455 4e45 220a 2020  "") == "TUNE".  
+0000ed60: 2020 2020 2020 2020 2020 2020 2020 616e                an
+0000ed70: 6420 6a73 6f6e 5f64 6174 612e 6765 7428  d json_data.get(
+0000ed80: 2273 7461 7469 6f6e 222c 2022 2229 203d  "station", "") =
+0000ed90: 3d20 706c 6174 666f 726d 2e6e 6f64 6528  = platform.node(
+0000eda0: 290a 2020 2020 2020 2020 2020 2020 293a  ).            ):
+0000edb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000edc0: 2023 2062 277b 2263 6d64 223a 2022 5455   # b'{"cmd": "TU
+0000edd0: 4e45 222c 2022 6672 6571 223a 2037 2e30  NE", "freq": 7.0
+0000ede0: 3233 352c 2022 7370 6f74 223a 2022 4d4d  235, "spot": "MM
+0000edf0: 3044 4749 227d 270a 2020 2020 2020 2020  0DGI"}'.        
+0000ee00: 2020 2020 2020 2020 7666 6f20 3d20 6a73          vfo = js
+0000ee10: 6f6e 5f64 6174 612e 6765 7428 2266 7265  on_data.get("fre
+0000ee20: 7122 290a 2020 2020 2020 2020 2020 2020  q").            
+0000ee30: 2020 2020 7666 6f20 3d20 666c 6f61 7428      vfo = float(
+0000ee40: 7666 6f29 202a 2031 3030 3030 3030 0a20  vfo) * 1000000. 
+0000ee50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ee60: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
+0000ee70: 2276 666f 6122 5d20 3d20 696e 7428 7666  "vfoa"] = int(vf
+0000ee80: 6f29 0a20 2020 2020 2020 2020 2020 2020  o).             
+0000ee90: 2020 2069 6620 7365 6c66 2e72 6967 5f63     if self.rig_c
+0000eea0: 6f6e 7472 6f6c 3a0a 2020 2020 2020 2020  ontrol:.        
+0000eeb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000eec0: 2e72 6967 5f63 6f6e 7472 6f6c 2e73 6574  .rig_control.set
+0000eed0: 5f76 666f 2869 6e74 2876 666f 2929 0a20  _vfo(int(vfo)). 
+0000eee0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000eef0: 706f 7420 3d20 6a73 6f6e 5f64 6174 612e  pot = json_data.
+0000ef00: 6765 7428 2273 706f 7422 2c20 2222 290a  get("spot", "").
+0000ef10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef20: 7365 6c66 2e63 616c 6c73 6967 6e2e 7365  self.callsign.se
+0000ef30: 7454 6578 7428 7370 6f74 290a 2020 2020  tText(spot).    
+0000ef40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ef50: 2e63 616c 6c73 6967 6e5f 6368 616e 6765  .callsign_change
+0000ef60: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
+0000ef70: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
+0000ef80: 6e2e 7365 7446 6f63 7573 2829 0a20 2020  n.setFocus().   
+0000ef90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000efa0: 662e 6361 6c6c 7369 676e 2e61 6374 6976  f.callsign.activ
+0000efb0: 6174 6557 696e 646f 7728 290a 2020 2020  ateWindow().    
+0000efc0: 2020 2020 2020 2020 2020 2020 7769 6e64              wind
+0000efd0: 6f77 2e72 6169 7365 5f28 290a 0a20 2020  ow.raise_()..   
+0000efe0: 2064 6566 2064 6172 6b5f 6d6f 6465 5f73   def dark_mode_s
+0000eff0: 7461 7465 5f63 6861 6e67 6528 7365 6c66  tate_change(self
+0000f000: 293a 0a20 2020 2020 2020 2022 2222 6461  ):.        """da
+0000f010: 726b 6d6f 6465 2064 726f 7064 6f77 6e20  rkmode dropdown 
+0000f020: 6368 6563 6b6d 6172 6b20 6368 616e 6765  checkmark change
+0000f030: 6422 2222 0a20 2020 2020 2020 2073 656c  d""".        sel
+0000f040: 662e 7072 6566 5b22 6461 726b 5f6d 6f64  f.pref["dark_mod
+0000f050: 6522 5d20 3d20 7365 6c66 2e61 6374 696f  e"] = self.actio
+0000f060: 6e44 6172 6b5f 4d6f 6465 2e69 7343 6865  nDark_Mode.isChe
+0000f070: 636b 6564 2829 0a20 2020 2020 2020 2073  cked().        s
+0000f080: 656c 662e 7772 6974 655f 7072 6566 6572  elf.write_prefer
+0000f090: 656e 6365 2829 0a20 2020 2020 2020 2073  ence().        s
+0000f0a0: 656c 662e 6461 726b 5f6d 6f64 6528 290a  elf.dark_mode().
+0000f0b0: 0a20 2020 2064 6566 2064 6172 6b5f 6d6f  .    def dark_mo
+0000f0c0: 6465 2873 656c 6629 3a0a 2020 2020 2020  de(self):.      
+0000f0d0: 2020 2222 2263 6861 6e67 6520 6469 7370    """change disp
+0000f0e0: 6c61 7920 6d6f 6465 2222 220a 2020 2020  lay mode""".    
+0000f0f0: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
+0000f100: 2e67 6574 2822 6461 726b 5f6d 6f64 6522  .get("dark_mode"
+0000f110: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000f120: 656c 662e 7365 7453 7479 6c65 5368 6565  elf.setStyleShee
+0000f130: 7428 4441 524b 5f53 5459 4c45 5348 4545  t(DARK_STYLESHEE
+0000f140: 5429 0a20 2020 2020 2020 2065 6c73 653a  T).        else:
+0000f150: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f160: 662e 7365 7453 7479 6c65 5368 6565 7428  f.setStyleSheet(
+0000f170: 2222 290a 0a20 2020 2064 6566 2063 775f  "")..    def cw_
+0000f180: 6d61 6372 6f73 5f73 7461 7465 5f63 6861  macros_state_cha
+0000f190: 6e67 6564 2873 656c 6629 3a0a 2020 2020  nged(self):.    
+0000f1a0: 2020 2020 2222 224d 656e 7520 6974 656d      """Menu item
+0000f1b0: 2074 6f20 7368 6f77 2f68 6964 6520 6d61   to show/hide ma
+0000f1c0: 6372 6f20 6275 7474 6f6e 7322 2222 0a20  cro buttons""". 
+0000f1d0: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
+0000f1e0: 5b22 6377 5f6d 6163 726f 7322 5d20 3d20  ["cw_macros"] = 
+0000f1f0: 7365 6c66 2e61 6374 696f 6e43 575f 4d61  self.actionCW_Ma
+0000f200: 6372 6f73 2e69 7343 6865 636b 6564 2829  cros.isChecked()
+0000f210: 0a20 2020 2020 2020 2073 656c 662e 7772  .        self.wr
+0000f220: 6974 655f 7072 6566 6572 656e 6365 2829  ite_preference()
+0000f230: 0a20 2020 2020 2020 2073 656c 662e 7368  .        self.sh
+0000f240: 6f77 5f43 575f 6d61 6372 6f73 2829 0a0a  ow_CW_macros()..
+0000f250: 2020 2020 6465 6620 7368 6f77 5f43 575f      def show_CW_
+0000f260: 6d61 6372 6f73 2873 656c 6629 3a0a 2020  macros(self):.  
+0000f270: 2020 2020 2020 2222 226d 6163 726f 2062        """macro b
+0000f280: 7574 746f 6e20 7374 6174 6520 6368 616e  utton state chan
+0000f290: 6765 2222 220a 2020 2020 2020 2020 6966  ge""".        if
+0000f2a0: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+0000f2b0: 6377 5f6d 6163 726f 7322 293a 0a20 2020  cw_macros"):.   
+0000f2c0: 2020 2020 2020 2020 2073 656c 662e 4275           self.Bu
+0000f2d0: 7474 6f6e 5f52 6f77 312e 7368 6f77 2829  tton_Row1.show()
+0000f2e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f2f0: 662e 4275 7474 6f6e 5f52 6f77 322e 7368  f.Button_Row2.sh
+0000f300: 6f77 2829 0a20 2020 2020 2020 2065 6c73  ow().        els
+0000f310: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000f320: 656c 662e 4275 7474 6f6e 5f52 6f77 312e  elf.Button_Row1.
+0000f330: 6869 6465 2829 0a20 2020 2020 2020 2020  hide().         
+0000f340: 2020 2073 656c 662e 4275 7474 6f6e 5f52     self.Button_R
+0000f350: 6f77 322e 6869 6465 2829 0a0a 2020 2020  ow2.hide()..    
+0000f360: 6465 6620 636f 6d6d 616e 645f 6275 7474  def command_butt
+0000f370: 6f6e 735f 7374 6174 655f 6368 616e 6765  ons_state_change
+0000f380: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000f390: 2222 224d 656e 7520 6974 656d 2074 6f20  """Menu item to 
+0000f3a0: 7368 6f77 2f68 6964 6520 636f 6d6d 616e  show/hide comman
+0000f3b0: 6420 6275 7474 6f6e 7322 2222 0a20 2020  d buttons""".   
+0000f3c0: 2020 2020 2073 656c 662e 7072 6566 5b22       self.pref["
+0000f3d0: 636f 6d6d 616e 645f 6275 7474 6f6e 7322  command_buttons"
+0000f3e0: 5d20 3d20 7365 6c66 2e61 6374 696f 6e43  ] = self.actionC
+0000f3f0: 6f6d 6d61 6e64 5f42 7574 746f 6e73 2e69  ommand_Buttons.i
+0000f400: 7343 6865 636b 6564 2829 0a20 2020 2020  sChecked().     
+0000f410: 2020 2073 656c 662e 7772 6974 655f 7072     self.write_pr
+0000f420: 6566 6572 656e 6365 2829 0a20 2020 2020  eference().     
+0000f430: 2020 2073 656c 662e 7368 6f77 5f63 6f6d     self.show_com
+0000f440: 6d61 6e64 5f62 7574 746f 6e73 2829 0a0a  mand_buttons()..
+0000f450: 2020 2020 6465 6620 7368 6f77 5f63 6f6d      def show_com
+0000f460: 6d61 6e64 5f62 7574 746f 6e73 2873 656c  mand_buttons(sel
+0000f470: 6629 3a0a 2020 2020 2020 2020 2222 2263  f):.        """c
+0000f480: 6f6d 6d61 6e64 2062 7574 746f 6e20 7374  ommand button st
+0000f490: 6174 6520 6368 616e 6765 2222 220a 2020  ate change""".  
+0000f4a0: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000f4b0: 6566 2e67 6574 2822 636f 6d6d 616e 645f  ef.get("command_
+0000f4c0: 6275 7474 6f6e 7322 293a 0a20 2020 2020  buttons"):.     
+0000f4d0: 2020 2020 2020 2073 656c 662e 436f 6d6d         self.Comm
+0000f4e0: 616e 645f 4275 7474 6f6e 732e 7368 6f77  and_Buttons.show
+0000f4f0: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
+0000f500: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f510: 662e 436f 6d6d 616e 645f 4275 7474 6f6e  f.Command_Button
+0000f520: 732e 6869 6465 2829 0a0a 2020 2020 6465  s.hide()..    de
+0000f530: 6620 6973 5f66 6c6f 6174 6162 6c65 2873  f is_floatable(s
+0000f540: 656c 662c 2069 7465 6d3a 2073 7472 2920  elf, item: str) 
+0000f550: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+0000f560: 2022 2222 6368 6563 6b20 746f 2073 6565   """check to see
+0000f570: 2069 6620 7374 7269 6e67 2063 616e 2062   if string can b
+0000f580: 6520 6120 666c 6f61 7422 2222 0a20 2020  e a float""".   
+0000f590: 2020 2020 2069 6620 6974 656d 2e69 736e       if item.isn
+0000f5a0: 756d 6572 6963 2829 3a0a 2020 2020 2020  umeric():.      
+0000f5b0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+0000f5c0: 650a 2020 2020 2020 2020 7472 793a 0a20  e.        try:. 
+0000f5d0: 2020 2020 2020 2020 2020 205f 7465 7374             _test
+0000f5e0: 203d 2066 6c6f 6174 2869 7465 6d29 0a20   = float(item). 
+0000f5f0: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
+0000f600: 6c75 6545 7272 6f72 3a0a 2020 2020 2020  lueError:.      
+0000f610: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0000f620: 7365 0a20 2020 2020 2020 2072 6574 7572  se.        retur
+0000f630: 6e20 5472 7565 0a0a 2020 2020 6465 6620  n True..    def 
+0000f640: 6f74 6865 725f 325f 6368 616e 6765 6428  other_2_changed(
+0000f650: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000f660: 2222 4361 6c6c 6564 2077 6865 6e20 7765  ""Called when we
+0000f670: 206e 6565 6420 746f 2070 6172 7365 2053   need to parse S
+0000f680: 5320 6578 6368 616e 6765 2e22 2222 0a20  S exchange.""". 
+0000f690: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0000f6a0: 6f6e 7465 7374 3a0a 2020 2020 2020 2020  ontest:.        
+0000f6b0: 2020 2020 6966 2022 4152 524c 2053 7765      if "ARRL Swe
+0000f6c0: 6570 7374 616b 6573 2220 696e 2073 656c  epstakes" in sel
+0000f6d0: 662e 636f 6e74 6573 742e 6e61 6d65 3a0a  f.contest.name:.
+0000f6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6f0: 7365 6c66 2e63 6f6e 7465 7374 2e70 6172  self.contest.par
+0000f700: 7365 5f65 7863 6861 6e67 6528 7365 6c66  se_exchange(self
+0000f710: 290a 0a20 2020 2064 6566 2063 616c 6c73  )..    def calls
+0000f720: 6967 6e5f 6368 616e 6765 6428 7365 6c66  ign_changed(self
+0000f730: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
+0000f740: 6c6c 6564 2077 6865 6e20 7465 7874 2069  lled when text i
+0000f750: 6e20 7468 6520 6361 6c6c 7369 676e 2066  n the callsign f
+0000f760: 6965 6c64 2068 6173 2063 6861 6e67 6564  ield has changed
+0000f770: 2222 220a 2020 2020 2020 2020 7465 7874  """.        text
+0000f780: 203d 2073 656c 662e 6361 6c6c 7369 676e   = self.callsign
+0000f790: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000f7a0: 7465 7874 203d 2074 6578 742e 7570 7065  text = text.uppe
+0000f7b0: 7228 290a 2020 2020 2020 2020 706f 7369  r().        posi
+0000f7c0: 7469 6f6e 203d 2073 656c 662e 6361 6c6c  tion = self.call
+0000f7d0: 7369 676e 2e63 7572 736f 7250 6f73 6974  sign.cursorPosit
+0000f7e0: 696f 6e28 290a 2020 2020 2020 2020 7374  ion().        st
+0000f7f0: 7269 7070 6564 5f74 6578 7420 3d20 7465  ripped_text = te
+0000f800: 7874 2e73 7472 6970 2829 2e72 6570 6c61  xt.strip().repla
+0000f810: 6365 2822 2022 2c20 2222 290a 2020 2020  ce(" ", "").    
+0000f820: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
+0000f830: 6e2e 7365 7454 6578 7428 7374 7269 7070  n.setText(stripp
+0000f840: 6564 5f74 6578 7429 0a20 2020 2020 2020  ed_text).       
+0000f850: 2073 656c 662e 6361 6c6c 7369 676e 2e73   self.callsign.s
+0000f860: 6574 4375 7273 6f72 506f 7369 7469 6f6e  etCursorPosition
+0000f870: 2870 6f73 6974 696f 6e29 0a0a 2020 2020  (position)..    
+0000f880: 2020 2020 6966 2022 2022 2069 6e20 7465      if " " in te
+0000f890: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
+0000f8a0: 6966 2073 7472 6970 7065 645f 7465 7874  if stripped_text
+0000f8b0: 203d 3d20 2243 5722 3a0a 2020 2020 2020   == "CW":.      
+0000f8c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000f8d0: 6574 6d6f 6465 2822 4357 2229 0a20 2020  etmode("CW").   
+0000f8e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f8f0: 662e 7261 6469 6f5f 7374 6174 655b 226d  f.radio_state["m
+0000f900: 6f64 6522 5d20 3d20 2243 5722 0a20 2020  ode"] = "CW".   
+0000f910: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000f920: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+0000f930: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f940: 2020 2020 2020 6966 2073 656c 662e 7269        if self.ri
+0000f950: 675f 636f 6e74 726f 6c2e 6f6e 6c69 6e65  g_control.online
+0000f960: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f970: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0000f980: 6967 5f63 6f6e 7472 6f6c 2e73 6574 5f6d  ig_control.set_m
+0000f990: 6f64 6528 2243 5722 290a 2020 2020 2020  ode("CW").      
+0000f9a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000f9b0: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
+0000f9c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000f9d0: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
+0000f9e0: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
+0000f9f0: 2020 2020 2073 656c 662e 7265 6164 5f63       self.read_c
+0000fa00: 775f 6d61 6372 6f73 2829 0a20 2020 2020  w_macros().     
+0000fa10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000fa20: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
+0000fa30: 2073 7472 6970 7065 645f 7465 7874 203d   stripped_text =
+0000fa40: 3d20 2252 5454 5922 3a0a 2020 2020 2020  = "RTTY":.      
+0000fa50: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000fa60: 6574 6d6f 6465 2822 5254 5459 2229 0a20  etmode("RTTY"). 
+0000fa70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000fa80: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
+0000fa90: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
+0000faa0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000fab0: 7269 675f 636f 6e74 726f 6c2e 6f6e 6c69  rig_control.onli
+0000fac0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000fad0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fae0: 2e72 6967 5f63 6f6e 7472 6f6c 2e73 6574  .rig_control.set
+0000faf0: 5f6d 6f64 6528 2252 5454 5922 290a 2020  _mode("RTTY").  
+0000fb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb30: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+0000fb40: 5b22 6d6f 6465 225d 203d 2022 5254 5459  ["mode"] = "RTTY
+0000fb50: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000fb60: 2020 7365 6c66 2e73 6574 5f77 696e 646f    self.set_windo
+0000fb70: 775f 7469 746c 6528 290a 2020 2020 2020  w_title().      
+0000fb80: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000fb90: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
+0000fba0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000fbb0: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
+0000fbc0: 6966 2073 7472 6970 7065 645f 7465 7874  if stripped_text
+0000fbd0: 203d 3d20 2253 5342 223a 0a20 2020 2020   == "SSB":.     
+0000fbe0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fbf0: 7365 746d 6f64 6528 2253 5342 2229 0a20  setmode("SSB"). 
+0000fc00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000fc10: 6620 696e 7428 7365 6c66 2e72 6164 696f  f int(self.radio
+0000fc20: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
+0000fc30: 222c 2030 2929 203e 2031 3030 3030 3030  ", 0)) > 1000000
+0000fc40: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+0000fc50: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
+0000fc60: 6f5f 7374 6174 655b 226d 6f64 6522 5d20  o_state["mode"] 
+0000fc70: 3d20 2255 5342 220a 2020 2020 2020 2020  = "USB".        
+0000fc80: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000fc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fca0: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
+0000fcb0: 7465 5b22 6d6f 6465 225d 203d 2022 4c53  te["mode"] = "LS
+0000fcc0: 4222 0a20 2020 2020 2020 2020 2020 2020  B".             
+0000fcd0: 2020 2073 656c 662e 7365 745f 7769 6e64     self.set_wind
+0000fce0: 6f77 5f74 6974 6c65 2829 0a20 2020 2020  ow_title().     
+0000fcf0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000fd00: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 3a0a  lf.rig_control:.
+0000fd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd20: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
+0000fd30: 7472 6f6c 2e73 6574 5f6d 6f64 6528 7365  trol.set_mode(se
+0000fd40: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+0000fd50: 6574 2822 6d6f 6465 2229 290a 2020 2020  et("mode")).    
+0000fd60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fd70: 2e63 6c65 6172 696e 7075 7473 2829 0a20  .clearinputs(). 
+0000fd80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fd90: 656c 662e 7265 6164 5f63 775f 6d61 6372  elf.read_cw_macr
+0000fda0: 6f73 2829 0a20 2020 2020 2020 2020 2020  os().           
+0000fdb0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000fdc0: 2020 2020 2020 2020 6966 2073 7472 6970          if strip
+0000fdd0: 7065 645f 7465 7874 203d 3d20 224f 504f  ped_text == "OPO
+0000fde0: 4e22 3a0a 2020 2020 2020 2020 2020 2020  N":.            
+0000fdf0: 2020 2020 7365 6c66 2e67 6574 5f6f 706f      self.get_opo
+0000fe00: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
+0000fe10: 2020 2020 7365 6c66 2e63 6c65 6172 696e      self.clearin
+0000fe20: 7075 7473 2829 0a20 2020 2020 2020 2020  puts().         
+0000fe30: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+0000fe40: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+0000fe50: 6970 7065 645f 7465 7874 203d 3d20 2254  ipped_text == "T
+0000fe60: 4553 5422 3a0a 2020 2020 2020 2020 2020  EST":.          
+0000fe70: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
+0000fe80: 6d65 7373 6167 655f 626f 7828 2254 6869  message_box("Thi
+0000fe90: 7320 6973 2061 2074 6573 7422 290a 2020  s is a test").  
+0000fea0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000feb0: 6c66 2e63 6c65 6172 696e 7075 7473 2829  lf.clearinputs()
+0000fec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fed0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+0000fee0: 2020 2020 6966 2073 656c 662e 6973 5f66      if self.is_f
+0000fef0: 6c6f 6174 6162 6c65 2873 7472 6970 7065  loatable(strippe
+0000ff00: 645f 7465 7874 293a 0a20 2020 2020 2020  d_text):.       
+0000ff10: 2020 2020 2020 2020 2076 666f 203d 2066           vfo = f
+0000ff20: 6c6f 6174 2873 7472 6970 7065 645f 7465  loat(stripped_te
+0000ff30: 7874 290a 2020 2020 2020 2020 2020 2020  xt).            
+0000ff40: 2020 2020 7666 6f20 3d20 696e 7428 7666      vfo = int(vf
+0000ff50: 6f20 2a20 3130 3030 290a 2020 2020 2020  o * 1000).      
+0000ff60: 2020 2020 2020 2020 2020 6261 6e64 203d            band =
+0000ff70: 2067 6574 6261 6e64 2873 7472 2876 666f   getband(str(vfo
+0000ff80: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0000ff90: 2020 2073 656c 662e 7365 745f 6261 6e64     self.set_band
+0000ffa0: 5f69 6e64 6963 6174 6f72 2862 616e 6429  _indicator(band)
+0000ffb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ffc0: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
+0000ffd0: 2242 616e 6422 5d20 3d20 6765 745f 6c6f  "Band"] = get_lo
+0000ffe0: 6767 6564 5f62 616e 6428 7374 7228 7365  gged_band(str(se
+0000fff0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+00010000: 6574 2822 7666 6f61 222c 2030 2e30 2929  et("vfoa", 0.0))
+00010010: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00010020: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
+00010030: 7465 5b22 7666 6f61 225d 203d 2076 666f  te["vfoa"] = vfo
+00010040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010050: 2073 656c 662e 7365 745f 7769 6e64 6f77   self.set_window
+00010060: 5f74 6974 6c65 2829 0a20 2020 2020 2020  _title().       
+00010070: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
+00010080: 6561 7269 6e70 7574 7328 290a 2020 2020  earinputs().    
+00010090: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000100a0: 656c 662e 7269 675f 636f 6e74 726f 6c3a  elf.rig_control:
+000100b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000100c0: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
+000100d0: 6e74 726f 6c2e 7365 745f 7666 6f28 7666  ntrol.set_vfo(vf
+000100e0: 6f29 0a20 2020 2020 2020 2020 2020 2020  o).             
+000100f0: 2020 2072 6574 7572 6e0a 0a20 2020 2020     return..     
+00010100: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
+00010110: 6b5f 6361 6c6c 7369 676e 2873 7472 6970  k_callsign(strip
+00010120: 7065 645f 7465 7874 290a 2020 2020 2020  ped_text).      
+00010130: 2020 2020 2020 6966 2073 656c 662e 6368        if self.ch
+00010140: 6563 6b5f 6475 7065 2873 7472 6970 7065  eck_dupe(strippe
+00010150: 645f 7465 7874 293a 0a20 2020 2020 2020  d_text):.       
+00010160: 2020 2020 2020 2020 2073 656c 662e 6475           self.du
+00010170: 7065 5f69 6e64 6963 6174 6f72 2e73 686f  pe_indicator.sho
+00010180: 7728 290a 2020 2020 2020 2020 2020 2020  w().            
+00010190: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000101a0: 2020 2020 2020 7365 6c66 2e64 7570 655f        self.dupe_
+000101b0: 696e 6469 6361 746f 722e 6869 6465 2829  indicator.hide()
+000101c0: 0a20 2020 2020 2020 2020 2020 205f 7468  .            _th
+000101d0: 6574 6872 6561 6420 3d20 7468 7265 6164  ethread = thread
+000101e0: 696e 672e 5468 7265 6164 280a 2020 2020  ing.Thread(.    
+000101f0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+00010200: 6574 3d73 656c 662e 6368 6563 6b5f 6361  et=self.check_ca
+00010210: 6c6c 7369 676e 322c 0a20 2020 2020 2020  llsign2,.       
+00010220: 2020 2020 2020 2020 2061 7267 733d 2874           args=(t
+00010230: 6578 742c 292c 0a20 2020 2020 2020 2020  ext,),.         
+00010240: 2020 2020 2020 2064 6165 6d6f 6e3d 5472         daemon=Tr
+00010250: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00010260: 290a 2020 2020 2020 2020 2020 2020 5f74  ).            _t
+00010270: 6865 7468 7265 6164 2e73 7461 7274 2829  hethread.start()
+00010280: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010290: 662e 6e65 7874 5f66 6965 6c64 2e73 6574  f.next_field.set
+000102a0: 466f 6375 7328 290a 2020 2020 2020 2020  Focus().        
+000102b0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+000102c0: 2020 2063 6d64 203d 207b 7d0a 2020 2020     cmd = {}.    
+000102d0: 2020 2020 636d 645b 2263 6d64 225d 203d      cmd["cmd"] =
+000102e0: 2022 4341 4c4c 4348 414e 4745 4422 0a20   "CALLCHANGED". 
+000102f0: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
+00010300: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
+00010310: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
+00010320: 636d 645b 2263 616c 6c22 5d20 3d20 7374  cmd["call"] = st
+00010330: 7269 7070 6564 5f74 6578 740a 2020 2020  ripped_text.    
+00010340: 2020 2020 7365 6c66 2e6d 756c 7469 6361      self.multica
+00010350: 7374 5f69 6e74 6572 6661 6365 2e73 656e  st_interface.sen
+00010360: 645f 6173 5f6a 736f 6e28 636d 6429 0a20  d_as_json(cmd). 
+00010370: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
+00010380: 6b5f 6361 6c6c 7369 676e 2873 7472 6970  k_callsign(strip
+00010390: 7065 645f 7465 7874 290a 0a20 2020 2064  ped_text)..    d
+000103a0: 6566 2063 6865 636b 5f63 616c 6c73 6967  ef check_callsig
+000103b0: 6e28 7365 6c66 2c20 6361 6c6c 7369 676e  n(self, callsign
+000103c0: 293a 0a20 2020 2020 2020 2022 2222 4368  ):.        """Ch
+000103d0: 6563 6b20 6361 6c6c 2061 7320 656e 7465  eck call as ente
+000103e0: 7265 6422 2222 0a20 2020 2020 2020 2072  red""".        r
+000103f0: 6573 756c 7420 3d20 6374 795f 6c6f 6f6b  esult = cty_look
+00010400: 7570 2863 616c 6c73 6967 6e29 0a20 2020  up(callsign).   
+00010410: 2020 2020 2064 6562 7567 5f72 6573 756c       debug_resul
+00010420: 7420 3d20 6622 7b72 6573 756c 747d 220a  t = f"{result}".
+00010430: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00010440: 6562 7567 2822 2573 222c 2064 6562 7567  ebug("%s", debug
+00010450: 5f72 6573 756c 7429 0a20 2020 2020 2020  _result).       
+00010460: 2069 6620 7265 7375 6c74 3a0a 2020 2020   if result:.    
+00010470: 2020 2020 2020 2020 666f 7220 6120 696e          for a in
+00010480: 2072 6573 756c 742e 6974 656d 7328 293a   result.items():
+00010490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000104a0: 2065 6e74 6974 7920 3d20 615b 315d 2e67   entity = a[1].g
+000104b0: 6574 2822 656e 7469 7479 222c 2022 2229  et("entity", "")
+000104c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000104d0: 2063 7120 3d20 615b 315d 2e67 6574 2822   cq = a[1].get("
+000104e0: 6371 222c 2022 2229 0a20 2020 2020 2020  cq", "").       
+000104f0: 2020 2020 2020 2020 2069 7475 203d 2061           itu = a
+00010500: 5b31 5d2e 6765 7428 2269 7475 222c 2022  [1].get("itu", "
+00010510: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00010520: 2020 2063 6f6e 7469 6e65 6e74 203d 2061     continent = a
+00010530: 5b31 5d2e 6765 7428 2263 6f6e 7469 6e65  [1].get("contine
+00010540: 6e74 2229 0a20 2020 2020 2020 2020 2020  nt").           
+00010550: 2020 2020 206c 6174 203d 2066 6c6f 6174       lat = float
+00010560: 2861 5b31 5d2e 6765 7428 226c 6174 222c  (a[1].get("lat",
+00010570: 2022 302e 3022 2929 0a20 2020 2020 2020   "0.0")).       
+00010580: 2020 2020 2020 2020 206c 6f6e 203d 2066           lon = f
+00010590: 6c6f 6174 2861 5b31 5d2e 6765 7428 226c  loat(a[1].get("l
+000105a0: 6f6e 6722 2c20 2230 2e30 2229 290a 2020  ong", "0.0")).  
+000105b0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+000105c0: 6e20 3d20 6c6f 6e20 2a20 2d31 2020 2320  n = lon * -1  # 
+000105d0: 6374 792e 6461 7420 6669 6c65 2069 6e76  cty.dat file inv
+000105e0: 6572 7473 206c 6f6e 6769 7475 6465 730a  erts longitudes.
+000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010600: 7072 696d 6172 795f 7066 7820 3d20 615b  primary_pfx = a[
+00010610: 315d 2e67 6574 2822 7072 696d 6172 795f  1].get("primary_
+00010620: 7066 7822 2c20 2222 290a 2020 2020 2020  pfx", "").      
+00010630: 2020 2020 2020 2020 2020 6865 6164 696e            headin
+00010640: 6720 3d20 6265 6172 696e 675f 7769 7468  g = bearing_with
+00010650: 5f6c 6174 6c6f 6e28 7365 6c66 2e73 7461  _latlon(self.sta
+00010660: 7469 6f6e 2e67 6574 2822 4772 6964 5371  tion.get("GridSq
+00010670: 7561 7265 2229 2c20 6c61 742c 206c 6f6e  uare"), lat, lon
+00010680: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00010690: 2020 6b69 6c6f 6d65 7465 7273 203d 2064    kilometers = d
+000106a0: 6973 7461 6e63 655f 7769 7468 5f6c 6174  istance_with_lat
+000106b0: 6c6f 6e28 0a20 2020 2020 2020 2020 2020  lon(.           
+000106c0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+000106d0: 6174 696f 6e2e 6765 7428 2247 7269 6453  ation.get("GridS
+000106e0: 7175 6172 6522 292c 206c 6174 2c20 6c6f  quare"), lat, lo
+000106f0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00010700: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00010710: 2020 2020 7365 6c66 2e68 6561 6469 6e67      self.heading
+00010720: 5f64 6973 7461 6e63 652e 7365 7454 6578  _distance.setTex
+00010730: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00010740: 2020 2020 2020 2066 2252 6567 696f 6e61         f"Regiona
+00010750: 6c20 4864 6720 7b68 6561 6469 6e67 7dc2  l Hdg {heading}.
+00010760: b020 4c50 207b 7265 6369 7072 6f63 6f6c  . LP {reciprocol
+00010770: 2868 6561 6469 6e67 297d c2b0 202f 2022  (heading)}.. / "
+00010780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010790: 2020 2020 2066 2264 6973 7461 6e63 6520       f"distance 
+000107a0: 7b69 6e74 286b 696c 6f6d 6574 6572 732a  {int(kilometers*
+000107b0: 302e 3632 3133 3731 297d 6d69 207b 6b69  0.621371)}mi {ki
+000107c0: 6c6f 6d65 7465 7273 7d6b 6d22 0a20 2020  lometers}km".   
+000107d0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+000107e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000107f0: 656c 662e 636f 6e74 6163 745b 2243 6f75  elf.contact["Cou
+00010800: 6e74 7279 5072 6566 6978 225d 203d 2070  ntryPrefix"] = p
+00010810: 7269 6d61 7279 5f70 6678 0a20 2020 2020  rimary_pfx.     
+00010820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010830: 636f 6e74 6163 745b 225a 4e22 5d20 3d20  contact["ZN"] = 
+00010840: 696e 7428 6371 290a 2020 2020 2020 2020  int(cq).        
+00010850: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00010860: 7461 6374 5b22 436f 6e74 696e 656e 7422  tact["Continent"
+00010870: 5d20 3d20 636f 6e74 696e 656e 740a 2020  ] = continent.  
+00010880: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010890: 6c66 2e64 785f 656e 7469 7479 2e73 6574  lf.dx_entity.set
+000108a0: 5465 7874 280a 2020 2020 2020 2020 2020  Text(.          
+000108b0: 2020 2020 2020 2020 2020 6622 7b70 7269            f"{pri
+000108c0: 6d61 7279 5f70 6678 7d3a 207b 636f 6e74  mary_pfx}: {cont
+000108d0: 696e 656e 747d 2f7b 656e 7469 7479 7d20  inent}/{entity} 
+000108e0: 6371 3a7b 6371 7d20 6974 753a 7b69 7475  cq:{cq} itu:{itu
+000108f0: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+00010900: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00010910: 2020 2020 2069 6620 6c65 6e28 6361 6c6c       if len(call
+00010920: 7369 676e 2920 3e20 323a 0a20 2020 2020  sign) > 2:.     
+00010930: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010940: 6620 7365 6c66 2e63 6f6e 7465 7374 3a0a  f self.contest:.
+00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010960: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00010970: 7465 7374 2e70 7265 6669 6c6c 2873 656c  test.prefill(sel
+00010980: 6629 0a0a 2020 2020 6465 6620 6368 6563  f)..    def chec
+00010990: 6b5f 6361 6c6c 7369 676e 3228 7365 6c66  k_callsign2(self
+000109a0: 2c20 6361 6c6c 7369 676e 293a 0a20 2020  , callsign):.   
+000109b0: 2020 2020 2022 2222 4368 6563 6b20 6361       """Check ca
+000109c0: 6c6c 206f 6e63 6520 656e 7465 7265 6422  ll once entered"
+000109d0: 2222 0a20 2020 2020 2020 2063 616c 6c73  "".        calls
+000109e0: 6967 6e20 3d20 6361 6c6c 7369 676e 2e73  ign = callsign.s
+000109f0: 7472 6970 2829 0a20 2020 2020 2020 2064  trip().        d
+00010a00: 6562 7567 5f6c 6f6f 6b75 7020 3d20 6622  ebug_lookup = f"
+00010a10: 7b73 656c 662e 6c6f 6f6b 5f75 707d 220a  {self.look_up}".
+00010a20: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00010a30: 6562 7567 2822 2573 2c20 2573 222c 2063  ebug("%s, %s", c
+00010a40: 616c 6c73 6967 6e2c 2064 6562 7567 5f6c  allsign, debug_l
+00010a50: 6f6f 6b75 7029 0a20 2020 2020 2020 2069  ookup).        i
+00010a60: 6620 6861 7361 7474 7228 7365 6c66 2e6c  f hasattr(self.l
+00010a70: 6f6f 6b5f 7570 2c20 2273 6573 7369 6f6e  ook_up, "session
+00010a80: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00010a90: 6966 2073 656c 662e 6c6f 6f6b 5f75 702e  if self.look_up.
+00010aa0: 7365 7373 696f 6e3a 0a20 2020 2020 2020  session:.       
+00010ab0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+00010ac0: 6520 3d20 7365 6c66 2e6c 6f6f 6b5f 7570  e = self.look_up
+00010ad0: 2e6c 6f6f 6b75 7028 6361 6c6c 7369 676e  .lookup(callsign
+00010ae0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00010af0: 2020 6465 6275 675f 7265 7370 6f6e 7365    debug_response
+00010b00: 203d 2066 227b 7265 7370 6f6e 7365 7d22   = f"{response}"
+00010b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b20: 206c 6f67 6765 722e 6465 6275 6728 2254   logger.debug("T
+00010b30: 6865 2052 6573 706f 6e73 653a 2025 735c  he Response: %s\
+00010b40: 6e22 2c20 6465 6275 675f 7265 7370 6f6e  n", debug_respon
+00010b50: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+00010b60: 2020 2020 6966 2072 6573 706f 6e73 653a      if response:
+00010b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b80: 2020 2020 2074 6865 6972 6772 6964 203d       theirgrid =
+00010b90: 2072 6573 706f 6e73 652e 6765 7428 2267   response.get("g
+00010ba0: 7269 6422 290a 2020 2020 2020 2020 2020  rid").          
+00010bb0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00010bc0: 6f6e 7461 6374 5b22 4772 6964 5371 7561  ontact["GridSqua
+00010bd0: 7265 225d 203d 2074 6865 6972 6772 6964  re"] = theirgrid
+00010be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010bf0: 2020 2020 205f 7468 6569 7263 6f75 6e74       _theircount
+00010c00: 7279 203d 2072 6573 706f 6e73 652e 6765  ry = response.ge
+00010c10: 7428 2263 6f75 6e74 7279 2229 0a20 2020  t("country").   
+00010c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c30: 2069 6620 7365 6c66 2e73 7461 7469 6f6e   if self.station
+00010c40: 2e67 6574 2822 4772 6964 5371 7561 7265  .get("GridSquare
+00010c50: 222c 2022 2229 3a0a 2020 2020 2020 2020  ", ""):.        
+00010c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c70: 6865 6164 696e 6720 3d20 6265 6172 696e  heading = bearin
+00010c80: 6728 7365 6c66 2e73 7461 7469 6f6e 2e67  g(self.station.g
+00010c90: 6574 2822 4772 6964 5371 7561 7265 222c  et("GridSquare",
+00010ca0: 2022 2229 2c20 7468 6569 7267 7269 6429   ""), theirgrid)
+00010cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010cc0: 2020 2020 2020 2020 206b 696c 6f6d 6574           kilomet
+00010cd0: 6572 7320 3d20 6469 7374 616e 6365 2873  ers = distance(s
+00010ce0: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+00010cf0: 2247 7269 6453 7175 6172 6522 292c 2074  "GridSquare"), t
+00010d00: 6865 6972 6772 6964 290a 2020 2020 2020  heirgrid).      
+00010d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d20: 2020 7365 6c66 2e68 6561 6469 6e67 5f64    self.heading_d
+00010d30: 6973 7461 6e63 652e 7365 7454 6578 7428  istance.setText(
+00010d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010d50: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
+00010d60: 7468 6569 7267 7269 647d 2048 6467 207b  theirgrid} Hdg {
+00010d70: 6865 6164 696e 677d c2b0 204c 5020 7b72  heading}.. LP {r
+00010d80: 6563 6970 726f 636f 6c28 6865 6164 696e  eciprocol(headin
+00010d90: 6729 7dc2 b020 2f20 220a 2020 2020 2020  g)}.. / ".      
+00010da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010db0: 2020 2020 2020 6622 6469 7374 616e 6365        f"distance
+00010dc0: 207b 696e 7428 6b69 6c6f 6d65 7465 7273   {int(kilometers
+00010dd0: 2a30 2e36 3231 3337 3129 7d6d 6920 7b6b  *0.621371)}mi {k
+00010de0: 696c 6f6d 6574 6572 737d 6b6d 220a 2020  ilometers}km".  
+00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00010e10: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+00010e20: 6c66 2e64 785f 656e 7469 7479 2e73 6574  lf.dx_entity.set
+00010e30: 5465 7874 2866 227b 7468 6569 7263 6f75  Text(f"{theircou
+00010e40: 6e74 7279 7d22 290a 2020 2020 2020 2020  ntry}").        
+00010e50: 2020 2020 2020 2020 2320 656c 7365 3a0a          # else:.
+00010e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e70: 2320 7365 6c66 2e68 6561 6469 6e67 5f64  # self.heading_d
+00010e80: 6973 7461 6e63 652e 7365 7454 6578 7428  istance.setText(
+00010e90: 224c 6f6f 6b75 7020 6661 696c 6564 2e22  "Lookup failed."
+00010ea0: 290a 0a20 2020 2064 6566 2063 6865 636b  )..    def check
+00010eb0: 5f64 7570 6528 7365 6c66 2c20 6361 6c6c  _dupe(self, call
+00010ec0: 3a20 7374 7229 202d 3e20 626f 6f6c 3a0a  : str) -> bool:.
+00010ed0: 2020 2020 2020 2020 2222 2243 6865 636b          """Check
+00010ee0: 7320 6966 2061 2063 616c 6c73 6967 6e20  s if a callsign 
+00010ef0: 6973 2061 2064 7570 6520 6f6e 2063 7572  is a dupe on cur
+00010f00: 7265 6e74 2062 616e 642f 6d6f 6465 2e22  rent band/mode."
+00010f10: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+00010f20: 636f 6e74 6573 742e 7072 6564 7570 6528  contest.predupe(
+00010f30: 7365 6c66 290a 2020 2020 2020 2020 6261  self).        ba
+00010f40: 6e64 203d 2066 6c6f 6174 2867 6574 5f6c  nd = float(get_l
+00010f50: 6f67 6765 645f 6261 6e64 2873 7472 2873  ogged_band(str(s
+00010f60: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+00010f70: 6765 7428 2276 666f 6122 2c20 302e 3029  get("vfoa", 0.0)
+00010f80: 2929 290a 2020 2020 2020 2020 6d6f 6465  ))).        mode
+00010f90: 203d 2073 656c 662e 7261 6469 6f5f 7374   = self.radio_st
+00010fa0: 6174 652e 6765 7428 226d 6f64 6522 2c20  ate.get("mode", 
+00010fb0: 2222 290a 2020 2020 2020 2020 6465 6275  "").        debu
+00010fc0: 676c 696e 6520 3d20 280a 2020 2020 2020  gline = (.      
+00010fd0: 2020 2020 2020 6622 4361 6c6c 3a20 7b63        f"Call: {c
+00010fe0: 616c 6c7d 2042 616e 643a 207b 6261 6e64  all} Band: {band
+00010ff0: 7d20 4d6f 6465 3a20 7b6d 6f64 657d 2044  } Mode: {mode} D
+00011000: 7570 6574 7970 653a 207b 7365 6c66 2e63  upetype: {self.c
+00011010: 6f6e 7465 7374 2e64 7570 655f 7479 7065  ontest.dupe_type
+00011020: 7d22 0a20 2020 2020 2020 2029 0a20 2020  }".        ).   
+00011030: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00011040: 6728 2225 7322 2c20 6465 6275 676c 696e  g("%s", debuglin
+00011050: 6529 0a20 2020 2020 2020 2069 6620 7365  e).        if se
+00011060: 6c66 2e63 6f6e 7465 7374 2e64 7570 655f  lf.contest.dupe_
+00011070: 7479 7065 203d 3d20 313a 0a20 2020 2020  type == 1:.     
+00011080: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00011090: 7365 6c66 2e64 6174 6162 6173 652e 6368  self.database.ch
+000110a0: 6563 6b5f 6475 7065 2863 616c 6c29 0a20  eck_dupe(call). 
+000110b0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+000110c0: 6f6e 7465 7374 2e64 7570 655f 7479 7065  ontest.dupe_type
+000110d0: 203d 3d20 323a 0a20 2020 2020 2020 2020   == 2:.         
+000110e0: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
+000110f0: 2e64 6174 6162 6173 652e 6368 6563 6b5f  .database.check_
+00011100: 6475 7065 5f6f 6e5f 6261 6e64 2863 616c  dupe_on_band(cal
+00011110: 6c2c 2062 616e 6429 0a20 2020 2020 2020  l, band).       
+00011120: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
+00011130: 2e64 7570 655f 7479 7065 203d 3d20 333a  .dupe_type == 3:
+00011140: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00011150: 756c 7420 3d20 7365 6c66 2e64 6174 6162  ult = self.datab
+00011160: 6173 652e 6368 6563 6b5f 6475 7065 5f6f  ase.check_dupe_o
+00011170: 6e5f 6261 6e64 5f6d 6f64 6528 6361 6c6c  n_band_mode(call
+00011180: 2c20 6261 6e64 2c20 6d6f 6465 290a 2020  , band, mode).  
+00011190: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+000111a0: 6e74 6573 742e 6475 7065 5f74 7970 6520  ntest.dupe_type 
+000111b0: 3d3d 2034 3a0a 2020 2020 2020 2020 2020  == 4:.          
+000111c0: 2020 7265 7375 6c74 203d 207b 2269 7364    result = {"isd
+000111d0: 7570 6522 3a20 4661 6c73 657d 0a20 2020  upe": False}.   
+000111e0: 2020 2020 2064 6562 7567 6c69 6e65 203d       debugline =
+000111f0: 2066 227b 7265 7375 6c74 7d22 0a20 2020   f"{result}".   
+00011200: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00011210: 6728 2225 7322 2c20 6465 6275 676c 696e  g("%s", debuglin
+00011220: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
+00011230: 6e20 7265 7375 6c74 2e67 6574 2822 6973  n result.get("is
+00011240: 6475 7065 222c 2046 616c 7365 290a 0a20  dupe", False).. 
+00011250: 2020 2064 6566 2073 6574 6d6f 6465 2873     def setmode(s
+00011260: 656c 662c 206d 6f64 653a 2073 7472 2920  elf, mode: str) 
+00011270: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00011280: 2022 2222 7374 7562 2066 6f72 2077 6865   """stub for whe
+00011290: 6e20 7468 6520 6d6f 6465 2063 6861 6e67  n the mode chang
+000112a0: 6573 2e22 2222 0a20 2020 2020 2020 2069  es.""".        i
+000112b0: 6620 6d6f 6465 203d 3d20 2243 5722 3a0a  f mode == "CW":.
+000112c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000112d0: 2e63 7572 7265 6e74 5f6d 6f64 6520 3d20  .current_mode = 
+000112e0: 2243 5722 0a20 2020 2020 2020 2020 2020  "CW".           
+000112f0: 2023 2073 656c 662e 6d6f 6465 2e73 6574   # self.mode.set
+00011300: 5465 7874 2822 4357 2229 0a20 2020 2020  Text("CW").     
+00011310: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
+00011320: 2e73 6574 5465 7874 2822 3539 3922 290a  .setText("599").
+00011330: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011340: 2e72 6563 6569 7665 2e73 6574 5465 7874  .receive.setText
+00011350: 2822 3539 3922 290a 2020 2020 2020 2020  ("599").        
+00011360: 2020 2020 7365 6c66 2e72 6561 645f 6377      self.read_cw
+00011370: 5f6d 6163 726f 7328 290a 2020 2020 2020  _macros().      
+00011380: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00011390: 2020 2020 2069 6620 6d6f 6465 203d 3d20       if mode == 
+000113a0: 2253 5342 223a 0a20 2020 2020 2020 2020  "SSB":.         
+000113b0: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
+000113c0: 6d6f 6465 203d 2022 5353 4222 0a20 2020  mode = "SSB".   
+000113d0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+000113e0: 6d6f 6465 2e73 6574 5465 7874 2822 5353  mode.setText("SS
+000113f0: 4222 290a 2020 2020 2020 2020 2020 2020  B").            
+00011400: 7365 6c66 2e73 656e 742e 7365 7454 6578  self.sent.setTex
+00011410: 7428 2235 3922 290a 2020 2020 2020 2020  t("59").        
+00011420: 2020 2020 7365 6c66 2e72 6563 6569 7665      self.receive
+00011430: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
+00011440: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011450: 7265 6164 5f63 775f 6d61 6372 6f73 2829  read_cw_macros()
+00011460: 0a20 2020 2020 2020 2069 6620 6d6f 6465  .        if mode
+00011470: 203d 3d20 2252 5454 5922 3a0a 2020 2020   == "RTTY":.    
+00011480: 2020 2020 2020 2020 7365 6c66 2e63 7572          self.cur
+00011490: 7265 6e74 5f6d 6f64 6520 3d20 2252 5454  rent_mode = "RTT
+000114a0: 5922 0a20 2020 2020 2020 2020 2020 2023  Y".            #
+000114b0: 2073 656c 662e 6d6f 6465 2e73 6574 5465   self.mode.setTe
+000114c0: 7874 2822 5254 5459 2229 0a20 2020 2020  xt("RTTY").     
+000114d0: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
+000114e0: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
+000114f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011500: 7265 6365 6976 652e 7365 7454 6578 7428  receive.setText(
+00011510: 2235 3922 290a 0a20 2020 2064 6566 2067  "59")..    def g
+00011520: 6574 5f6f 706f 6e28 7365 6c66 293a 0a20  et_opon(self):. 
+00011530: 2020 2020 2020 2022 2222 4374 726c 2b4f         """Ctrl+O
+00011540: 206f 7220 4f50 4f4e 2064 6961 6c6f 6722   or OPON dialog"
+00011550: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+00011560: 6f70 6f6e 5f64 6961 6c6f 6720 3d20 4f70  opon_dialog = Op
+00011570: 4f6e 2857 4f52 4b49 4e47 5f50 4154 4829  On(WORKING_PATH)
+00011580: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
+00011590: 6f6e 5f64 6961 6c6f 672e 6163 6365 7074  on_dialog.accept
+000115a0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+000115b0: 6e65 775f 6f70 290a 2020 2020 2020 2020  new_op).        
+000115c0: 7365 6c66 2e6f 706f 6e5f 6469 616c 6f67  self.opon_dialog
+000115d0: 2e6f 7065 6e28 290a 0a20 2020 2064 6566  .open()..    def
+000115e0: 206e 6577 5f6f 7028 7365 6c66 293a 0a20   new_op(self):. 
+000115f0: 2020 2020 2020 2022 2222 5361 7665 206e         """Save n
+00011600: 6577 204f 5022 2222 0a20 2020 2020 2020  ew OP""".       
+00011610: 2069 6620 7365 6c66 2e6f 706f 6e5f 6469   if self.opon_di
+00011620: 616c 6f67 2e4e 6577 4f70 6572 6174 6f72  alog.NewOperator
+00011630: 2e74 6578 7428 293a 0a20 2020 2020 2020  .text():.       
+00011640: 2020 2020 2073 656c 662e 6375 7272 656e       self.curren
+00011650: 745f 6f70 203d 2073 656c 662e 6f70 6f6e  t_op = self.opon
+00011660: 5f64 6961 6c6f 672e 4e65 774f 7065 7261  _dialog.NewOpera
+00011670: 746f 722e 7465 7874 2829 2e75 7070 6572  tor.text().upper
+00011680: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00011690: 6f70 6f6e 5f64 6961 6c6f 672e 636c 6f73  opon_dialog.clos
+000116a0: 6528 290a 2020 2020 2020 2020 6c6f 6767  e().        logg
+000116b0: 6572 2e64 6562 7567 2822 4e65 7720 4f70  er.debug("New Op
+000116c0: 3a20 2573 222c 2073 656c 662e 6375 7272  : %s", self.curr
+000116d0: 656e 745f 6f70 290a 2020 2020 2020 2020  ent_op).        
+000116e0: 7365 6c66 2e6d 616b 655f 6f70 5f64 6972  self.make_op_dir
+000116f0: 2829 0a0a 2020 2020 6465 6620 6d61 6b65  ()..    def make
+00011700: 5f6f 705f 6469 7228 7365 6c66 293a 0a20  _op_dir(self):. 
+00011710: 2020 2020 2020 2022 2222 4372 6561 7465         """Create
+00011720: 204f 5020 6469 7265 6374 6f72 7920 6966   OP directory if
+00011730: 2069 7420 646f 6573 206e 6f74 2065 7869   it does not exi
+00011740: 7374 2e22 2222 0a20 2020 2020 2020 2069  st.""".        i
+00011750: 6620 7365 6c66 2e63 7572 7265 6e74 5f6f  f self.current_o
+00011760: 703a 0a20 2020 2020 2020 2020 2020 206f  p:.            o
+00011770: 705f 7061 7468 203d 2050 6174 6828 4441  p_path = Path(DA
+00011780: 5441 5f50 4154 4829 202f 2073 656c 662e  TA_PATH) / self.
+00011790: 6375 7272 656e 745f 6f70 0a20 2020 2020  current_op.     
+000117a0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+000117b0: 6275 6728 226f 705f 7061 7468 3a20 2573  bug("op_path: %s
+000117c0: 222c 2073 7472 286f 705f 7061 7468 2929  ", str(op_path))
+000117d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000117e0: 6f70 5f70 6174 682e 6973 5f64 6972 2829  op_path.is_dir()
+000117f0: 2069 7320 4661 6c73 653a 0a20 2020 2020   is False:.     
+00011800: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00011810: 722e 6465 6275 6728 2243 7265 6174 696e  r.debug("Creatin
+00011820: 6720 4f70 2044 6972 6563 746f 7279 3a20  g Op Directory: 
+00011830: 2573 222c 2073 7472 286f 705f 7061 7468  %s", str(op_path
+00011840: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00011850: 2020 206f 732e 6d6b 6469 7228 7374 7228     os.mkdir(str(
+00011860: 6f70 5f70 6174 6829 290a 2020 2020 2020  op_path)).      
+00011870: 2020 2020 2020 6966 206f 705f 7061 7468        if op_path
+00011880: 2e69 735f 6469 7228 293a 0a20 2020 2020  .is_dir():.     
+00011890: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+000118a0: 655f 7061 7468 203d 2050 6174 6828 574f  e_path = Path(WO
+000118b0: 524b 494e 475f 5041 5448 2920 2f20 2264  RKING_PATH) / "d
+000118c0: 6174 6122 202f 2022 7068 6f6e 6574 6963  ata" / "phonetic
+000118d0: 7322 0a20 2020 2020 2020 2020 2020 2020  s".             
+000118e0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+000118f0: 2273 6f75 7263 655f 7061 7468 3a20 2573  "source_path: %s
+00011900: 222c 2073 7472 2873 6f75 7263 655f 7061  ", str(source_pa
+00011910: 7468 2929 0a20 2020 2020 2020 2020 2020  th)).           
+00011920: 2020 2020 2066 6f72 2063 6869 6c64 2069       for child i
+00011930: 6e20 736f 7572 6365 5f70 6174 682e 6974  n source_path.it
+00011940: 6572 6469 7228 293a 0a20 2020 2020 2020  erdir():.       
+00011950: 2020 2020 2020 2020 2020 2020 2064 6573               des
+00011960: 7469 6e61 7469 6f6e 5f66 696c 6520 3d20  tination_file = 
+00011970: 6f70 5f70 6174 6820 2f20 6368 696c 642e  op_path / child.
+00011980: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
+00011990: 2020 2020 2020 2020 2069 6620 6465 7374           if dest
+000119a0: 696e 6174 696f 6e5f 6669 6c65 2e69 735f  ination_file.is_
+000119b0: 6669 6c65 2829 2069 7320 4661 6c73 653a  file() is False:
+000119c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000119d0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+000119e0: 6465 6275 6728 2244 6573 7469 6e61 7469  debug("Destinati
+000119f0: 6f6e 3a20 2573 222c 2073 7472 2864 6573  on: %s", str(des
+00011a00: 7469 6e61 7469 6f6e 5f66 696c 6529 290a  tination_file)).
+00011a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a20: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
+00011a30: 696f 6e5f 6669 6c65 2e77 7269 7465 5f62  ion_file.write_b
+00011a40: 7974 6573 2863 6869 6c64 2e72 6561 645f  ytes(child.read_
+00011a50: 6279 7465 7328 2929 0a0a 2020 2020 6465  bytes())..    de
+00011a60: 6620 706f 6c6c 5f72 6164 696f 2873 656c  f poll_radio(sel
+00011a70: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
+00011a80: 7475 6222 2222 0a20 2020 2020 2020 2069  tub""".        i
+00011a90: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
+00011aa0: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
+00011ab0: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
+00011ac0: 726f 6c2e 6f6e 6c69 6e65 3a0a 2020 2020  rol.online:.    
+00011ad0: 2020 2020 2020 2020 2020 2020 7666 6f20              vfo 
+00011ae0: 3d20 7365 6c66 2e72 6967 5f63 6f6e 7472  = self.rig_contr
+00011af0: 6f6c 2e67 6574 5f76 666f 2829 0a20 2020  ol.get_vfo().   
+00011b00: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+00011b10: 6520 3d20 7365 6c66 2e72 6967 5f63 6f6e  e = self.rig_con
+00011b20: 7472 6f6c 2e67 6574 5f6d 6f64 6528 290a  trol.get_mode().
+00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b40: 6277 203d 2073 656c 662e 7269 675f 636f  bw = self.rig_co
+00011b50: 6e74 726f 6c2e 6765 745f 6277 2829 0a20  ntrol.get_bw(). 
+00011b60: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00011b70: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+00011b80: 655b 2270 7474 225d 203d 2073 656c 662e  e["ptt"] = self.
+00011b90: 7269 675f 636f 6e74 726f 6c2e 6765 745f  rig_control.get_
+00011ba0: 7074 7428 290a 2020 2020 2020 2020 2020  ptt().          
+00011bb0: 2020 2020 2020 2320 6966 2073 656c 662e        # if self.
+00011bc0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+00011bd0: 2270 7474 222c 2030 2920 3d3d 2031 3a0a  "ptt", 0) == 1:.
+00011be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bf0: 2320 2020 2020 7365 6c66 2e6c 6566 7464  #     self.leftd
+00011c00: 6f74 2e73 6574 5069 786d 6170 2873 656c  ot.setPixmap(sel
+00011c10: 662e 6772 6565 6e64 6f74 290a 2020 2020  f.greendot).    
+00011c20: 2020 2020 2020 2020 2020 2020 2320 656c              # el
+00011c30: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00011c40: 2020 2020 2320 2020 2020 7365 6c66 2e6c      #     self.l
+00011c50: 6566 7464 6f74 2e73 6574 5069 786d 6170  eftdot.setPixmap
+00011c60: 2873 656c 662e 7265 6464 6f74 290a 2020  (self.reddot).  
+00011c70: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011c80: 206d 6f64 6520 3d3d 2022 4357 223a 0a20   mode == "CW":. 
+00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ca0: 2020 2073 656c 662e 7365 746d 6f64 6528     self.setmode(
+00011cb0: 6d6f 6465 290a 2020 2020 2020 2020 2020  mode).          
+00011cc0: 2020 2020 2020 6966 206d 6f64 6520 3d3d        if mode ==
+00011cd0: 2022 4c53 4222 206f 7220 6d6f 6465 203d   "LSB" or mode =
+00011ce0: 3d20 2255 5342 223a 0a20 2020 2020 2020  = "USB":.       
+00011cf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011d00: 662e 7365 746d 6f64 6528 2253 5342 2229  f.setmode("SSB")
+00011d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011d20: 2069 6620 6d6f 6465 203d 3d20 2252 5454   if mode == "RTT
+00011d30: 5922 3a0a 2020 2020 2020 2020 2020 2020  Y":.            
+00011d40: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00011d50: 6d6f 6465 2822 5254 5459 2229 0a20 2020  mode("RTTY").   
+00011d60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011d70: 662e 7261 6469 6f5f 7374 6174 655b 2276  f.radio_state["v
+00011d80: 666f 6122 5d20 3d20 7666 6f0a 2020 2020  foa"] = vfo.    
+00011d90: 2020 2020 2020 2020 2020 2020 6261 6e64              band
+00011da0: 203d 2067 6574 6261 6e64 2873 7472 2876   = getband(str(v
+00011db0: 666f 2929 0a20 2020 2020 2020 2020 2020  fo)).           
+00011dc0: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
+00011dd0: 7374 6174 655b 2262 616e 6422 5d20 3d20  state["band"] = 
+00011de0: 6261 6e64 0a20 2020 2020 2020 2020 2020  band.           
+00011df0: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+00011e00: 745b 2242 616e 6422 5d20 3d20 6765 745f  t["Band"] = get_
+00011e10: 6c6f 6767 6564 5f62 616e 6428 7374 7228  logged_band(str(
+00011e20: 7666 6f29 290a 2020 2020 2020 2020 2020  vfo)).          
+00011e30: 2020 2020 2020 7365 6c66 2e73 6574 5f62        self.set_b
+00011e40: 616e 645f 696e 6469 6361 746f 7228 6261  and_indicator(ba
+00011e50: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
+00011e60: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
+00011e70: 7461 7465 5b22 6d6f 6465 225d 203d 206d  tate["mode"] = m
+00011e80: 6f64 650a 2020 2020 2020 2020 2020 2020  ode.            
+00011e90: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
+00011ea0: 7461 7465 5b22 6277 225d 203d 2062 770a  tate["bw"] = bw.
+00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ec0: 6c6f 6767 6572 2e64 6562 7567 2822 5646  logger.debug("VF
+00011ed0: 4f3a 2025 7320 204d 4f44 453a 2025 7320  O: %s  MODE: %s 
+00011ee0: 4257 3a20 2573 222c 2076 666f 2c20 6d6f  BW: %s", vfo, mo
+00011ef0: 6465 2c20 6277 290a 2020 2020 2020 2020  de, bw).        
+00011f00: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00011f10: 5f77 696e 646f 775f 7469 746c 6528 290a  _window_title().
+00011f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f30: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
+00011f40: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
+00011f50: 6422 5d20 3d20 2252 4144 494f 5f53 5441  d"] = "RADIO_STA
+00011f60: 5445 220a 2020 2020 2020 2020 2020 2020  TE".            
+00011f70: 2020 2020 636d 645b 2273 7461 7469 6f6e      cmd["station
+00011f80: 225d 203d 2070 6c61 7466 6f72 6d2e 6e6f  "] = platform.no
+00011f90: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
+00011fa0: 2020 2020 2063 6d64 5b22 6261 6e64 225d       cmd["band"]
+00011fb0: 203d 2062 616e 640a 2020 2020 2020 2020   = band.        
+00011fc0: 2020 2020 2020 2020 636d 645b 2276 666f          cmd["vfo
+00011fd0: 6122 5d20 3d20 7666 6f0a 2020 2020 2020  a"] = vfo.      
+00011fe0: 2020 2020 2020 2020 2020 636d 645b 226d            cmd["m
+00011ff0: 6f64 6522 5d20 3d20 6d6f 6465 0a20 2020  ode"] = mode.   
+00012000: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+00012010: 5b22 6277 225d 203d 2062 770a 2020 2020  ["bw"] = bw.    
+00012020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012030: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
+00012040: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
+00012050: 6e28 636d 6429 0a0a 2020 2020 6465 6620  n(cmd)..    def 
+00012060: 6564 6974 5f63 775f 6d61 6372 6f73 2873  edit_cw_macros(s
+00012070: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00012080: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012090: 2020 4361 6c6c 7320 7468 6520 6465 6661    Calls the defa
+000120a0: 756c 7420 7465 7874 2065 6469 746f 7220  ult text editor 
+000120b0: 746f 2065 6469 7420 7468 6520 4357 206d  to edit the CW m
+000120c0: 6163 726f 2066 696c 652e 0a20 2020 2020  acro file..     
+000120d0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+000120e0: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
+000120f0: 7465 2e67 6574 2822 6d6f 6465 2229 203d  te.get("mode") =
+00012100: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
+00012110: 2020 2020 6d61 6372 6f5f 6669 6c65 203d      macro_file =
+00012120: 2022 2f63 776d 6163 726f 732e 7478 7422   "/cwmacros.txt"
+00012130: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00012140: 2020 2020 2020 2020 2020 206d 6163 726f             macro
+00012150: 5f66 696c 6520 3d20 222f 7373 626d 6163  _file = "/ssbmac
+00012160: 726f 732e 7478 7422 0a20 2020 2020 2020  ros.txt".       
+00012170: 2069 6620 6e6f 7420 5061 7468 2844 4154   if not Path(DAT
+00012180: 415f 5041 5448 202b 206d 6163 726f 5f66  A_PATH + macro_f
+00012190: 696c 6529 2e65 7869 7374 7328 293a 0a20  ile).exists():. 
+000121a0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+000121b0: 722e 6465 6275 6728 2272 6561 645f 6377  r.debug("read_cw
+000121c0: 5f6d 6163 726f 733a 2063 6f70 7969 6e67  _macros: copying
+000121d0: 2064 6566 6175 6c74 206d 6163 726f 2066   default macro f
+000121e0: 696c 652e 2229 0a20 2020 2020 2020 2020  ile.").         
+000121f0: 2020 2063 6f70 7966 696c 6528 574f 524b     copyfile(WORK
+00012200: 494e 475f 5041 5448 202b 2022 2f64 6174  ING_PATH + "/dat
+00012210: 6122 202b 206d 6163 726f 5f66 696c 652c  a" + macro_file,
+00012220: 2044 4154 415f 5041 5448 202b 206d 6163   DATA_PATH + mac
+00012230: 726f 5f66 696c 6529 0a20 2020 2020 2020  ro_file).       
+00012240: 206f 732e 7379 7374 656d 2866 2278 6467   os.system(f"xdg
+00012250: 2d6f 7065 6e20 7b44 4154 415f 5041 5448  -open {DATA_PATH
+00012260: 7d7b 6d61 6372 6f5f 6669 6c65 7d22 290a  }{macro_file}").
+00012270: 0a20 2020 2064 6566 2072 6561 645f 6377  .    def read_cw
+00012280: 5f6d 6163 726f 7328 7365 6c66 2920 2d3e  _macros(self) ->
+00012290: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+000122a0: 2222 0a20 2020 2020 2020 2052 6561 6473  "".        Reads
+000122b0: 2069 6e20 7468 6520 4357 206d 6163 726f   in the CW macro
+000122c0: 732c 2066 6972 7374 7320 6974 2063 6865  s, firsts it che
+000122d0: 636b 7320 746f 2073 6565 2069 6620 7468  cks to see if th
+000122e0: 6520 6669 6c65 2065 7869 7374 732e 2049  e file exists. I
+000122f0: 6620 6974 2064 6f65 7320 6e6f 742c 0a20  f it does not,. 
+00012300: 2020 2020 2020 2061 6e64 2074 6869 7320         and this 
+00012310: 6861 7320 6265 656e 2070 6163 6b61 6765  has been package
+00012320: 6420 7769 7468 2070 7969 6e73 7461 6c6c  d with pyinstall
+00012330: 6572 2069 7420 7769 6c6c 2063 6f70 7920  er it will copy 
+00012340: 7468 6520 6465 6661 756c 7420 6669 6c65  the default file
+00012350: 2066 726f 6d20 7468 650a 2020 2020 2020   from the.      
+00012360: 2020 7465 6d70 2064 6972 6563 746f 7279    temp directory
+00012370: 2074 6869 7320 6973 2072 756e 6e69 6e67   this is running
+00012380: 2066 726f 6d2e 2e2e 2049 6e20 7468 656f   from... In theo
+00012390: 7279 2e0a 2020 2020 2020 2020 2222 220a  ry..        """.
+000123a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000123b0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+000123c0: 2822 6d6f 6465 2229 203d 3d20 2243 5722  ("mode") == "CW"
+000123d0: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
+000123e0: 6372 6f5f 6669 6c65 203d 2022 2f63 776d  cro_file = "/cwm
+000123f0: 6163 726f 732e 7478 7422 0a20 2020 2020  acros.txt".     
+00012400: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00012410: 2020 2020 206d 6163 726f 5f66 696c 6520       macro_file 
+00012420: 3d20 222f 7373 626d 6163 726f 732e 7478  = "/ssbmacros.tx
+00012430: 7422 0a0a 2020 2020 2020 2020 6966 206e  t"..        if n
+00012440: 6f74 2050 6174 6828 4441 5441 5f50 4154  ot Path(DATA_PAT
+00012450: 4820 2b20 6d61 6372 6f5f 6669 6c65 292e  H + macro_file).
+00012460: 6578 6973 7473 2829 3a0a 2020 2020 2020  exists():.      
+00012470: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00012480: 7567 2822 7265 6164 5f63 775f 6d61 6372  ug("read_cw_macr
+00012490: 6f73 3a20 636f 7079 696e 6720 6465 6661  os: copying defa
+000124a0: 756c 7420 6d61 6372 6f20 6669 6c65 2e22  ult macro file."
+000124b0: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
+000124c0: 7079 6669 6c65 2857 4f52 4b49 4e47 5f50  pyfile(WORKING_P
+000124d0: 4154 4820 2b20 222f 6461 7461 2220 2b20  ATH + "/data" + 
+000124e0: 6d61 6372 6f5f 6669 6c65 2c20 4441 5441  macro_file, DATA
+000124f0: 5f50 4154 4820 2b20 6d61 6372 6f5f 6669  _PATH + macro_fi
+00012500: 6c65 290a 2020 2020 2020 2020 7769 7468  le).        with
+00012510: 206f 7065 6e28 4441 5441 5f50 4154 4820   open(DATA_PATH 
+00012520: 2b20 6d61 6372 6f5f 6669 6c65 2c20 2272  + macro_file, "r
+00012530: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
+00012540: 2d38 2229 2061 7320 6669 6c65 5f64 6573  -8") as file_des
+00012550: 6372 6970 746f 723a 0a20 2020 2020 2020  criptor:.       
+00012560: 2020 2020 2066 6f72 206c 696e 6520 696e       for line in
+00012570: 2066 696c 655f 6465 7363 7269 7074 6f72   file_descriptor
+00012580: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012590: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000125a0: 2020 2020 2020 2020 2020 206d 6f64 652c             mode,
+000125b0: 2066 6b65 792c 2062 7574 746f 6e6e 616d   fkey, buttonnam
+000125c0: 652c 2063 7774 6578 7420 3d20 6c69 6e65  e, cwtext = line
+000125d0: 2e73 706c 6974 2822 7c22 290a 2020 2020  .split("|").    
+000125e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125f0: 6966 206d 6f64 652e 7374 7269 7028 292e  if mode.strip().
+00012600: 7570 7065 7228 2920 3d3d 2022 5222 2061  upper() == "R" a
+00012610: 6e64 2073 656c 662e 7072 6566 2e67 6574  nd self.pref.get
+00012620: 2822 7275 6e5f 7374 6174 6522 293a 0a20  ("run_state"):. 
+00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012640: 2020 2020 2020 2073 656c 662e 666b 6579         self.fkey
+00012650: 735b 666b 6579 2e73 7472 6970 2829 5d20  s[fkey.strip()] 
+00012660: 3d20 2862 7574 746f 6e6e 616d 652e 7374  = (buttonname.st
+00012670: 7269 7028 292c 2063 7774 6578 742e 7374  rip(), cwtext.st
+00012680: 7269 7028 2929 0a20 2020 2020 2020 2020  rip()).         
+00012690: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
+000126a0: 6465 2e73 7472 6970 2829 2e75 7070 6572  de.strip().upper
+000126b0: 2829 2021 3d20 2252 2220 616e 6420 6e6f  () != "R" and no
+000126c0: 7420 7365 6c66 2e70 7265 662e 6765 7428  t self.pref.get(
+000126d0: 2272 756e 5f73 7461 7465 2229 3a0a 2020  "run_state"):.  
+000126e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126f0: 2020 2020 2020 7365 6c66 2e66 6b65 7973        self.fkeys
+00012700: 5b66 6b65 792e 7374 7269 7028 295d 203d  [fkey.strip()] =
+00012710: 2028 6275 7474 6f6e 6e61 6d65 2e73 7472   (buttonname.str
+00012720: 6970 2829 2c20 6377 7465 7874 2e73 7472  ip(), cwtext.str
+00012730: 6970 2829 290a 2020 2020 2020 2020 2020  ip()).          
+00012740: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
+00012750: 7565 4572 726f 7220 6173 2065 7272 3a0a  ueError as err:.
+00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012770: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+00012780: 2272 6561 645f 6377 5f6d 6163 726f 733a  "read_cw_macros:
+00012790: 2025 7322 2c20 6572 7229 0a20 2020 2020   %s", err).     
+000127a0: 2020 206b 6579 7320 3d20 7365 6c66 2e66     keys = self.f
+000127b0: 6b65 7973 2e6b 6579 7328 290a 2020 2020  keys.keys().    
+000127c0: 2020 2020 6966 2022 4631 2220 696e 206b      if "F1" in k
+000127d0: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
+000127e0: 2073 656c 662e 4631 2e73 6574 5465 7874   self.F1.setText
+000127f0: 2866 2246 313a 207b 7365 6c66 2e66 6b65  (f"F1: {self.fke
+00012800: 7973 5b27 4631 275d 5b30 5d7d 2229 0a20  ys['F1'][0]}"). 
+00012810: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012820: 4631 2e73 6574 546f 6f6c 5469 7028 7365  F1.setToolTip(se
+00012830: 6c66 2e66 6b65 7973 5b22 4631 225d 5b31  lf.fkeys["F1"][1
+00012840: 5d29 0a20 2020 2020 2020 2069 6620 2246  ]).        if "F
+00012850: 3222 2069 6e20 6b65 7973 3a0a 2020 2020  2" in keys:.    
+00012860: 2020 2020 2020 2020 7365 6c66 2e46 322e          self.F2.
+00012870: 7365 7454 6578 7428 6622 4632 3a20 7b73  setText(f"F2: {s
+00012880: 656c 662e 666b 6579 735b 2746 3227 5d5b  elf.fkeys['F2'][
+00012890: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
+000128a0: 2020 7365 6c66 2e46 322e 7365 7454 6f6f    self.F2.setToo
+000128b0: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
+000128c0: 2246 3222 5d5b 315d 290a 2020 2020 2020  "F2"][1]).      
+000128d0: 2020 6966 2022 4633 2220 696e 206b 6579    if "F3" in key
+000128e0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+000128f0: 656c 662e 4633 2e73 6574 5465 7874 2866  elf.F3.setText(f
+00012900: 2246 333a 207b 7365 6c66 2e66 6b65 7973  "F3: {self.fkeys
+00012910: 5b27 4633 275d 5b30 5d7d 2229 0a20 2020  ['F3'][0]}").   
+00012920: 2020 2020 2020 2020 2073 656c 662e 4633           self.F3
+00012930: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
+00012940: 2e66 6b65 7973 5b22 4633 225d 5b31 5d29  .fkeys["F3"][1])
+00012950: 0a20 2020 2020 2020 2069 6620 2246 3422  .        if "F4"
+00012960: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
+00012970: 2020 2020 2020 7365 6c66 2e46 342e 7365        self.F4.se
+00012980: 7454 6578 7428 6622 4634 3a20 7b73 656c  tText(f"F4: {sel
+00012990: 662e 666b 6579 735b 2746 3427 5d5b 305d  f.fkeys['F4'][0]
+000129a0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+000129b0: 7365 6c66 2e46 342e 7365 7454 6f6f 6c54  self.F4.setToolT
+000129c0: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
+000129d0: 3422 5d5b 315d 290a 2020 2020 2020 2020  4"][1]).        
+000129e0: 6966 2022 4635 2220 696e 206b 6579 733a  if "F5" in keys:
+000129f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00012a00: 662e 4635 2e73 6574 5465 7874 2866 2246  f.F5.setText(f"F
+00012a10: 353a 207b 7365 6c66 2e66 6b65 7973 5b27  5: {self.fkeys['
+00012a20: 4635 275d 5b30 5d7d 2229 0a20 2020 2020  F5'][0]}").     
+00012a30: 2020 2020 2020 2073 656c 662e 4635 2e73         self.F5.s
+00012a40: 6574 546f 6f6c 5469 7028 7365 6c66 2e66  etToolTip(self.f
+00012a50: 6b65 7973 5b22 4635 225d 5b31 5d29 0a20  keys["F5"][1]). 
+00012a60: 2020 2020 2020 2069 6620 2246 3622 2069         if "F6" i
+00012a70: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
+00012a80: 2020 2020 7365 6c66 2e46 362e 7365 7454      self.F6.setT
+00012a90: 6578 7428 6622 4636 3a20 7b73 656c 662e  ext(f"F6: {self.
+00012aa0: 666b 6579 735b 2746 3627 5d5b 305d 7d22  fkeys['F6'][0]}"
+00012ab0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00012ac0: 6c66 2e46 362e 7365 7454 6f6f 6c54 6970  lf.F6.setToolTip
+00012ad0: 2873 656c 662e 666b 6579 735b 2246 3622  (self.fkeys["F6"
+00012ae0: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
+00012af0: 2022 4637 2220 696e 206b 6579 733a 0a20   "F7" in keys:. 
+00012b00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012b10: 4637 2e73 6574 5465 7874 2866 2246 373a  F7.setText(f"F7:
+00012b20: 207b 7365 6c66 2e66 6b65 7973 5b27 4637   {self.fkeys['F7
+00012b30: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
+00012b40: 2020 2020 2073 656c 662e 4637 2e73 6574       self.F7.set
+00012b50: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
+00012b60: 7973 5b22 4637 225d 5b31 5d29 0a20 2020  ys["F7"][1]).   
+00012b70: 2020 2020 2069 6620 2246 3822 2069 6e20       if "F8" in 
+00012b80: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
+00012b90: 2020 7365 6c66 2e46 382e 7365 7454 6578    self.F8.setTex
+00012ba0: 7428 6622 4638 3a20 7b73 656c 662e 666b  t(f"F8: {self.fk
+00012bb0: 6579 735b 2746 3827 5d5b 305d 7d22 290a  eys['F8'][0]}").
+00012bc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012bd0: 2e46 382e 7365 7454 6f6f 6c54 6970 2873  .F8.setToolTip(s
+00012be0: 656c 662e 666b 6579 735b 2246 3822 5d5b  elf.fkeys["F8"][
+00012bf0: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
+00012c00: 4639 2220 696e 206b 6579 733a 0a20 2020  F9" in keys:.   
+00012c10: 2020 2020 2020 2020 2073 656c 662e 4639           self.F9
+00012c20: 2e73 6574 5465 7874 2866 2246 393a 207b  .setText(f"F9: {
+00012c30: 7365 6c66 2e66 6b65 7973 5b27 4639 275d  self.fkeys['F9']
+00012c40: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
+00012c50: 2020 2073 656c 662e 4639 2e73 6574 546f     self.F9.setTo
+00012c60: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
+00012c70: 5b22 4639 225d 5b31 5d29 0a20 2020 2020  ["F9"][1]).     
+00012c80: 2020 2069 6620 2246 3130 2220 696e 206b     if "F10" in k
+00012c90: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
+00012ca0: 2073 656c 662e 4631 302e 7365 7454 6578   self.F10.setTex
+00012cb0: 7428 6622 4631 303a 207b 7365 6c66 2e66  t(f"F10: {self.f
+00012cc0: 6b65 7973 5b27 4631 3027 5d5b 305d 7d22  keys['F10'][0]}"
+00012cd0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00012ce0: 6c66 2e46 3130 2e73 6574 546f 6f6c 5469  lf.F10.setToolTi
+00012cf0: 7028 7365 6c66 2e66 6b65 7973 5b22 4631  p(self.fkeys["F1
+00012d00: 3022 5d5b 315d 290a 2020 2020 2020 2020  0"][1]).        
+00012d10: 6966 2022 4631 3122 2069 6e20 6b65 7973  if "F11" in keys
+00012d20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00012d30: 6c66 2e46 3131 2e73 6574 5465 7874 2866  lf.F11.setText(f
+00012d40: 2246 3131 3a20 7b73 656c 662e 666b 6579  "F11: {self.fkey
+00012d50: 735b 2746 3131 275d 5b30 5d7d 2229 0a20  s['F11'][0]}"). 
+00012d60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012d70: 4631 312e 7365 7454 6f6f 6c54 6970 2873  F11.setToolTip(s
+00012d80: 656c 662e 666b 6579 735b 2246 3131 225d  elf.fkeys["F11"]
+00012d90: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
+00012da0: 2246 3132 2220 696e 206b 6579 733a 0a20  "F12" in keys:. 
+00012db0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012dc0: 4631 322e 7365 7454 6578 7428 6622 4631  F12.setText(f"F1
+00012dd0: 323a 207b 7365 6c66 2e66 6b65 7973 5b27  2: {self.fkeys['
+00012de0: 4631 3227 5d5b 305d 7d22 290a 2020 2020  F12'][0]}").    
+00012df0: 2020 2020 2020 2020 7365 6c66 2e46 3132          self.F12
+00012e00: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
+00012e10: 2e66 6b65 7973 5b22 4631 3222 5d5b 315d  .fkeys["F12"][1]
+00012e20: 290a 0a20 2020 2064 6566 2067 656e 6572  )..    def gener
+00012e30: 6174 655f 6164 6966 2873 656c 6629 3a0a  ate_adif(self):.
+00012e40: 2020 2020 2020 2020 2222 2247 656e 6572          """Gener
+00012e50: 6174 6520 4144 4946 2222 220a 2020 2020  ate ADIF""".    
+00012e60: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00012e70: 2822 2a2a 2a2a 2a2a 4144 4946 2a2a 2a2a  ("******ADIF****
+00012e80: 2a22 290a 2020 2020 2020 2020 7365 6c66  *").        self
+00012e90: 2e63 6f6e 7465 7374 2e61 6469 6628 7365  .contest.adif(se
+00012ea0: 6c66 290a 0a20 2020 2064 6566 2067 656e  lf)..    def gen
+00012eb0: 6572 6174 655f 6361 6272 696c 6c6f 2873  erate_cabrillo(s
+00012ec0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00012ed0: 2247 656e 6572 6174 6573 2043 6162 7269  "Generates Cabri
+00012ee0: 6c6c 6f20 6669 6c65 2e20 4d61 7962 652e  llo file. Maybe.
+00012ef0: 2222 220a 2020 2020 2020 2020 2320 6874  """.        # ht
+00012f00: 7470 733a 2f2f 7777 772e 6371 7770 782e  tps://www.cqwpx.
+00012f10: 636f 6d2f 6361 6272 696c 6c6f 2e68 746d  com/cabrillo.htm
+00012f20: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00012f30: 6465 6275 6728 222a 2a2a 2a2a 2a43 6162  debug("******Cab
+00012f40: 7269 6c6c 6f2a 2a2a 2a2a 2229 0a20 2020  rillo*****").   
+00012f50: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00012f60: 742e 6361 6272 696c 6c6f 2873 656c 6629  t.cabrillo(self)
+00012f70: 0a0a 0a64 6566 206c 6f61 645f 666f 6e74  ...def load_font
+00012f80: 735f 6672 6f6d 5f64 6972 2864 6972 6563  s_from_dir(direc
+00012f90: 746f 7279 3a20 7374 7229 202d 3e20 7365  tory: str) -> se
+00012fa0: 743a 0a20 2020 2022 2222 0a20 2020 2057  t:.    """.    W
+00012fb0: 656c 6c20 6974 206c 6f61 6473 2066 6f6e  ell it loads fon
+00012fc0: 7473 2066 726f 6d20 6120 6469 7265 6374  ts from a direct
+00012fd0: 6f72 792e 2e2e 0a20 2020 2022 2222 0a20  ory....    """. 
+00012fe0: 2020 2066 6f6e 745f 6661 6d69 6c69 6573     font_families
+00012ff0: 203d 2073 6574 2829 0a20 2020 2066 6f72   = set().    for
+00013000: 205f 6669 2069 6e20 5144 6972 2864 6972   _fi in QDir(dir
+00013010: 6563 746f 7279 292e 656e 7472 7949 6e66  ectory).entryInf
+00013020: 6f4c 6973 7428 5b22 2a2e 7474 6622 2c20  oList(["*.ttf", 
+00013030: 222a 2e77 6f66 6622 2c20 222a 2e77 6f66  "*.woff", "*.wof
+00013040: 6632 225d 293a 0a20 2020 2020 2020 205f  f2"]):.        _
+00013050: 6964 203d 2051 466f 6e74 4461 7461 6261  id = QFontDataba
+00013060: 7365 2e61 6464 4170 706c 6963 6174 696f  se.addApplicatio
+00013070: 6e46 6f6e 7428 5f66 692e 6162 736f 6c75  nFont(_fi.absolu
+00013080: 7465 4669 6c65 5061 7468 2829 290a 2020  teFilePath()).  
+00013090: 2020 2020 2020 666f 6e74 5f66 616d 696c        font_famil
+000130a0: 6965 7320 7c3d 2073 6574 2851 466f 6e74  ies |= set(QFont
+000130b0: 4461 7461 6261 7365 2e61 7070 6c69 6361  Database.applica
+000130c0: 7469 6f6e 466f 6e74 4661 6d69 6c69 6573  tionFontFamilies
+000130d0: 285f 6964 2929 0a20 2020 2072 6574 7572  (_id)).    retur
+000130e0: 6e20 666f 6e74 5f66 616d 696c 6965 730a  n font_families.
+000130f0: 0a0a 6465 6620 696e 7374 616c 6c5f 6963  ..def install_ic
+00013100: 6f6e 7328 293a 0a20 2020 2022 2222 496e  ons():.    """In
+00013110: 7374 616c 6c20 6963 6f6e 7322 2222 0a20  stall icons""". 
+00013120: 2020 206f 732e 7379 7374 656d 280a 2020     os.system(.  
+00013130: 2020 2020 2020 2278 6467 2d69 636f 6e2d        "xdg-icon-
+00013140: 7265 736f 7572 6365 2069 6e73 7461 6c6c  resource install
+00013150: 202d 2d73 697a 6520 3332 202d 2d63 6f6e   --size 32 --con
+00013160: 7465 7874 2061 7070 7320 2d2d 6d6f 6465  text apps --mode
+00013170: 2075 7365 7220 220a 2020 2020 2020 2020   user ".        
+00013180: 6622 7b57 4f52 4b49 4e47 5f50 4154 487d  f"{WORKING_PATH}
+00013190: 2f64 6174 612f 6b36 6774 652e 6e6f 7431  /data/k6gte.not1
+000131a0: 6d6d 2d33 322e 706e 6720 6b36 6774 652d  mm-32.png k6gte-
+000131b0: 6e6f 7431 6d6d 220a 2020 2020 290a 2020  not1mm".    ).  
+000131c0: 2020 6f73 2e73 7973 7465 6d28 0a20 2020    os.system(.   
+000131d0: 2020 2020 2022 7864 672d 6963 6f6e 2d72       "xdg-icon-r
+000131e0: 6573 6f75 7263 6520 696e 7374 616c 6c20  esource install 
+000131f0: 2d2d 7369 7a65 2036 3420 2d2d 636f 6e74  --size 64 --cont
+00013200: 6578 7420 6170 7073 202d 2d6d 6f64 6520  ext apps --mode 
+00013210: 7573 6572 2022 0a20 2020 2020 2020 2066  user ".        f
+00013220: 227b 574f 524b 494e 475f 5041 5448 7d2f  "{WORKING_PATH}/
+00013230: 6461 7461 2f6b 3667 7465 2e6e 6f74 316d  data/k6gte.not1m
+00013240: 6d2d 3634 2e70 6e67 206b 3667 7465 2d6e  m-64.png k6gte-n
+00013250: 6f74 316d 6d22 0a20 2020 2029 0a20 2020  ot1mm".    ).   
+00013260: 206f 732e 7379 7374 656d 280a 2020 2020   os.system(.    
+00013270: 2020 2020 2278 6467 2d69 636f 6e2d 7265      "xdg-icon-re
+00013280: 736f 7572 6365 2069 6e73 7461 6c6c 202d  source install -
+00013290: 2d73 697a 6520 3132 3820 2d2d 636f 6e74  -size 128 --cont
+000132a0: 6578 7420 6170 7073 202d 2d6d 6f64 6520  ext apps --mode 
+000132b0: 7573 6572 2022 0a20 2020 2020 2020 2066  user ".        f
+000132c0: 227b 574f 524b 494e 475f 5041 5448 7d2f  "{WORKING_PATH}/
+000132d0: 6461 7461 2f6b 3667 7465 2e6e 6f74 316d  data/k6gte.not1m
+000132e0: 6d2d 3132 382e 706e 6720 6b36 6774 652d  m-128.png k6gte-
+000132f0: 6e6f 7431 6d6d 220a 2020 2020 290a 2020  not1mm".    ).  
+00013300: 2020 6f73 2e73 7973 7465 6d28 6622 7864    os.system(f"xd
+00013310: 672d 6465 736b 746f 702d 6d65 6e75 2069  g-desktop-menu i
+00013320: 6e73 7461 6c6c 207b 574f 524b 494e 475f  nstall {WORKING_
+00013330: 5041 5448 7d2f 6461 7461 2f6b 3667 7465  PATH}/data/k6gte
+00013340: 2d6e 6f74 316d 6d2e 6465 736b 746f 7022  -not1mm.desktop"
+00013350: 290a 0a0a 6465 6620 646f 696d 7028 6d6f  )...def doimp(mo
+00013360: 646e 616d 6529 3a0a 2020 2020 2222 2272  dname):.    """r
+00013370: 6574 7572 6e20 6d6f 6475 6c65 2070 6174  eturn module pat
+00013380: 6822 2222 0a20 2020 2072 6574 7572 6e20  h""".    return 
+00013390: 696d 706f 7274 6c69 622e 696d 706f 7274  importlib.import
+000133a0: 5f6d 6f64 756c 6528 6622 6e6f 7431 6d6d  _module(f"not1mm
+000133b0: 2e70 6c75 6769 6e73 2e7b 6d6f 646e 616d  .plugins.{modnam
+000133c0: 657d 2229 0a0a 0a64 6566 2072 756e 2829  e}")...def run()
+000133d0: 3a0a 2020 2020 2222 220a 2020 2020 4d61  :.    """.    Ma
+000133e0: 696e 2045 6e74 7279 0a20 2020 2022 2222  in Entry.    """
+000133f0: 0a0a 2020 2020 696e 7374 616c 6c5f 6963  ..    install_ic
+00013400: 6f6e 7328 290a 2020 2020 7469 6d65 722e  ons().    timer.
+00013410: 7374 6172 7428 3130 3029 0a20 2020 2074  start(100).    t
+00013420: 696d 6572 322e 7374 6172 7428 3235 3029  imer2.start(250)
+00013430: 0a0a 2020 2020 7379 732e 6578 6974 2861  ..    sys.exit(a
+00013440: 7070 2e65 7865 6328 2929 0a0a 0a6c 6f67  pp.exec())...log
+00013450: 6765 7220 3d20 6c6f 6767 696e 672e 6765  ger = logging.ge
+00013460: 744c 6f67 6765 7228 225f 5f6d 6169 6e5f  tLogger("__main_
+00013470: 5f22 290a 6861 6e64 6c65 7220 3d20 6c6f  _").handler = lo
+00013480: 6767 696e 672e 5374 7265 616d 4861 6e64  gging.StreamHand
+00013490: 6c65 7228 290a 666f 726d 6174 7465 7220  ler().formatter 
+000134a0: 3d20 6c6f 6767 696e 672e 466f 726d 6174  = logging.Format
+000134b0: 7465 7228 0a20 2020 2064 6174 6566 6d74  ter(.    datefmt
+000134c0: 3d22 2548 3a25 4d3a 2553 222c 0a20 2020  ="%H:%M:%S",.   
+000134d0: 2066 6d74 3d22 5b25 2861 7363 7469 6d65   fmt="[%(asctime
+000134e0: 2973 5d20 2528 6c65 7665 6c6e 616d 6529  )s] %(levelname)
+000134f0: 7320 2528 6d6f 6475 6c65 2973 202d 2025  s %(module)s - %
+00013500: 2866 756e 634e 616d 6529 7320 4c69 6e65  (funcName)s Line
+00013510: 2025 286c 696e 656e 6f29 643a 2025 286d   %(lineno)d: %(m
+00013520: 6573 7361 6765 2973 222c 0a29 0a68 616e  essage)s",.).han
+00013530: 646c 6572 2e73 6574 466f 726d 6174 7465  dler.setFormatte
+00013540: 7228 666f 726d 6174 7465 7229 0a6c 6f67  r(formatter).log
+00013550: 6765 722e 6164 6448 616e 646c 6572 2868  ger.addHandler(h
+00013560: 616e 646c 6572 290a 0a69 6620 5061 7468  andler)..if Path
+00013570: 2822 2e2f 6465 6275 6722 292e 6578 6973  ("./debug").exis
+00013580: 7473 2829 3a0a 2020 2020 6c6f 6767 6572  ts():.    logger
+00013590: 2e73 6574 4c65 7665 6c28 6c6f 6767 696e  .setLevel(loggin
+000135a0: 672e 4445 4255 4729 0a20 2020 206c 6f67  g.DEBUG).    log
+000135b0: 6765 722e 6465 6275 6728 2264 6562 7567  ger.debug("debug
+000135c0: 6769 6e67 206f 6e22 290a 656c 7365 3a0a  ging on").else:.
+000135d0: 2020 2020 6c6f 6767 6572 2e73 6574 4c65      logger.setLe
+000135e0: 7665 6c28 6c6f 6767 696e 672e 5741 524e  vel(logging.WARN
+000135f0: 494e 4729 0a20 2020 206c 6f67 6765 722e  ING).    logger.
+00013600: 7761 726e 696e 6728 2264 6562 7567 6769  warning("debuggi
+00013610: 6e67 206f 6666 2229 0a0a 6170 7020 3d20  ng off")..app = 
+00013620: 5174 5769 6467 6574 732e 5141 7070 6c69  QtWidgets.QAppli
+00013630: 6361 7469 6f6e 2873 7973 2e61 7267 7629  cation(sys.argv)
+00013640: 0a23 2061 7070 2e73 6574 5374 796c 6528  .# app.setStyle(
+00013650: 2246 7573 696f 6e22 290a 666f 6e74 5f70  "Fusion").font_p
+00013660: 6174 6820 3d20 574f 524b 494e 475f 5041  ath = WORKING_PA
+00013670: 5448 202b 2022 2f64 6174 6122 0a66 616d  TH + "/data".fam
+00013680: 696c 6965 7320 3d20 6c6f 6164 5f66 6f6e  ilies = load_fon
+00013690: 7473 5f66 726f 6d5f 6469 7228 6f73 2e66  ts_from_dir(os.f
+000136a0: 7370 6174 6828 666f 6e74 5f70 6174 6829  spath(font_path)
+000136b0: 290a 6c6f 6767 6572 2e69 6e66 6f28 6661  ).logger.info(fa
+000136c0: 6d69 6c69 6573 290a 7769 6e64 6f77 203d  milies).window =
+000136d0: 204d 6169 6e57 696e 646f 7728 290a 6865   MainWindow().he
+000136e0: 6967 6874 203d 2077 696e 646f 772e 7072  ight = window.pr
+000136f0: 6566 2e67 6574 2822 7769 6e64 6f77 5f68  ef.get("window_h
+00013700: 6569 6768 7422 2c20 3330 3029 0a77 6964  eight", 300).wid
+00013710: 7468 203d 2077 696e 646f 772e 7072 6566  th = window.pref
+00013720: 2e67 6574 2822 7769 6e64 6f77 5f77 6964  .get("window_wid
+00013730: 7468 222c 2037 3030 290a 7820 3d20 7769  th", 700).x = wi
+00013740: 6e64 6f77 2e70 7265 662e 6765 7428 2277  ndow.pref.get("w
+00013750: 696e 646f 775f 7822 2c20 2d31 290a 7920  indow_x", -1).y 
+00013760: 3d20 7769 6e64 6f77 2e70 7265 662e 6765  = window.pref.ge
+00013770: 7428 2277 696e 646f 775f 7922 2c20 2d31  t("window_y", -1
+00013780: 290a 7769 6e64 6f77 2e73 6574 4765 6f6d  ).window.setGeom
+00013790: 6574 7279 2878 2c20 792c 2077 6964 7468  etry(x, y, width
+000137a0: 2c20 6865 6967 6874 290a 2320 7769 6e64  , height).# wind
+000137b0: 6f77 2e73 6574 5769 6e64 6f77 5469 746c  ow.setWindowTitl
+000137c0: 6528 6622 4e6f 7431 4d4d 2076 7b5f 5f76  e(f"Not1MM v{__v
+000137d0: 6572 7369 6f6e 5f5f 7d22 290a 7769 6e64  ersion__}").wind
+000137e0: 6f77 2e63 616c 6c73 6967 6e2e 7365 7446  ow.callsign.setF
+000137f0: 6f63 7573 2829 0a77 696e 646f 772e 7368  ocus().window.sh
+00013800: 6f77 2829 0a74 696d 6572 203d 2051 7443  ow().timer = QtC
+00013810: 6f72 652e 5154 696d 6572 2829 0a74 696d  ore.QTimer().tim
+00013820: 6572 2e74 696d 656f 7574 2e63 6f6e 6e65  er.timeout.conne
+00013830: 6374 2877 696e 646f 772e 706f 6c6c 5f72  ct(window.poll_r
+00013840: 6164 696f 290a 7469 6d65 7232 203d 2051  adio).timer2 = Q
+00013850: 7443 6f72 652e 5154 696d 6572 2829 0a74  tCore.QTimer().t
+00013860: 696d 6572 322e 7469 6d65 6f75 742e 636f  imer2.timeout.co
+00013870: 6e6e 6563 7428 7769 6e64 6f77 2e63 6865  nnect(window.che
+00013880: 636b 5f75 6470 5f74 7261 6666 6963 290a  ck_udp_traffic).
+00013890: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
+000138a0: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
+000138b0: 7275 6e28 290a                           run().
```

### Comparing `not1mm-23.5.9/not1mm/bandmap.py` & `not1mm-23.5.9.1/not1mm/bandmap.py`

 * *Files 8% similar despite different names*

```diff
@@ -173,14 +173,28 @@
     def getspotsinband(self, start: float, end: float) -> list:
         """ "return a list of dict where freq range is defined"""
         self.cursor.execute(
             f"select * from spots where freq >= {start} and freq <= {end} order by freq ASC;"
         )
         return self.cursor.fetchall()
 
+    def get_next_spot(self, current: float, limit: float) -> dict:
+        """ "return a list of dict where freq range is defined"""
+        self.cursor.execute(
+            f"select * from spots where freq > {current} and freq <= {limit} order by freq ASC;"
+        )
+        return self.cursor.fetchone()
+
+    def get_prev_spot(self, current: float, limit: float) -> dict:
+        """ "return a list of dict where freq range is defined"""
+        self.cursor.execute(
+            f"select * from spots where freq < {current} and freq >= {limit} order by freq DESC;"
+        )
+        return self.cursor.fetchone()
+
     def delete_spots(self, minutes: int):
         """doc"""
         self.cursor.execute(
             f"delete from spots where ts < datetime('now', '-{minutes} minutes');"
         )
 
 
@@ -278,14 +292,51 @@
             ):
                 self.set_band(packet.get("band") + "m", False)
                 self.rx_freq = float(packet.get("vfoa")) / 1000000
                 self.tx_freq = self.rx_freq
                 self.bandwidth = int(packet.get("bw", "0"))
                 step, _ = self.determine_step_digits()
                 self.drawTXRXMarks(step)
+            if (
+                packet.get("cmd", "") == "NEXTSPOT"
+                and packet.get("station", "") == platform.node()
+            ):
+                spot = self.spots.get_next_spot(
+                    self.rx_freq + 0.000001, self.currentBand.end
+                )
+                if spot:
+                    cmd = {}
+                    cmd["cmd"] = "TUNE"
+                    cmd["station"] = platform.node()
+                    cmd["freq"] = spot.get("freq", self.rx_freq)
+                    cmd["spot"] = spot.get("callsign", "")
+                    packet = bytes(dumps(cmd), encoding="ascii")
+                    self.udpsocket.writeDatagram(
+                        packet, QtNetwork.QHostAddress(MULTICAST_GROUP), MULTICAST_PORT
+                    )
+                continue
+
+            if (
+                packet.get("cmd", "") == "PREVSPOT"
+                and packet.get("station", "") == platform.node()
+            ):
+                spot = self.spots.get_prev_spot(
+                    self.rx_freq - 0.000001, self.currentBand.start
+                )
+                if spot:
+                    cmd = {}
+                    cmd["cmd"] = "TUNE"
+                    cmd["station"] = platform.node()
+                    cmd["freq"] = spot.get("freq", self.rx_freq)
+                    cmd["spot"] = spot.get("callsign", "")
+                    packet = bytes(dumps(cmd), encoding="ascii")
+                    self.udpsocket.writeDatagram(
+                        packet, QtNetwork.QHostAddress(MULTICAST_GROUP), MULTICAST_PORT
+                    )
+                continue
 
     def spot_clicked(self):
         """dunno"""
         items = self.bandmap_scene.selectedItems()
         for item in items:
             if item:
                 cmd = {}
```

### Comparing `not1mm-23.5.9/not1mm/data/Combinear.qss` & `not1mm-23.5.9.1/not1mm/data/Combinear.qss`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-23.5.9.1/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/MASTER.SCP` & `not1mm-23.5.9.1/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/about.ui` & `not1mm-23.5.9.1/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/bandmap.ui` & `not1mm-23.5.9.1/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/configuration.ui` & `not1mm-23.5.9.1/not1mm/data/configuration.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/contests.sql` & `not1mm-23.5.9.1/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/cty.json` & `not1mm-23.5.9.1/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/editcontact.ui` & `not1mm-23.5.9.1/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/editmacro.ui` & `not1mm-23.5.9.1/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/k6gte.not1mm-128.png` & `not1mm-23.5.9.1/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/k6gte.not1mm-32.png` & `not1mm-23.5.9.1/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/k6gte.not1mm-64.png` & `not1mm-23.5.9.1/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/logwindow.ui` & `not1mm-23.5.9.1/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/main.ui` & `not1mm-23.5.9.1/not1mm/data/main.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/new_contest.ui` & `not1mm-23.5.9.1/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/opon.ui` & `not1mm-23.5.9.1/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/0.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/1.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/2.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/3.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/4.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/5.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/6.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/7.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/73.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/8.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/9.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/a.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/again.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/b.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/c.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/contest.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/cq.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/d.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/e.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/f.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/g.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/h.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/i.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/j.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/k.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/k6gte.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/l.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/m.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/mynumber.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/n.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/nil.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/o.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/p.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/q.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/r.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/roger.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/s.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/space.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/t.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/thankyou.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/u.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/v.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/w.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/x.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/y.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/yourcall.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/phonetics/z.wav` & `not1mm-23.5.9.1/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/pickcontest.ui` & `not1mm-23.5.9.1/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/reddot.png` & `not1mm-23.5.9.1/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/data/settings.ui` & `not1mm-23.5.9.1/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/lib/cat_interface.py` & `not1mm-23.5.9.1/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/lib/cwinterface.py` & `not1mm-23.5.9.1/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/lib/database.py` & `not1mm-23.5.9.1/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/lib/edit_macro.py` & `not1mm-23.5.9.1/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/lib/edit_station.py` & `not1mm-23.5.9.1/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/lib/ham_utility.py` & `not1mm-23.5.9.1/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/lib/lookup.py` & `not1mm-23.5.9.1/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/lib/multicast.py` & `not1mm-23.5.9.1/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/lib/n1mm.py` & `not1mm-23.5.9.1/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/lib/settings.py` & `not1mm-23.5.9.1/not1mm/lib/settings.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/logwindow.py` & `not1mm-23.5.9.1/not1mm/logwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/10_10_fall_cw.py` & `not1mm-23.5.9.1/not1mm/plugins/10_10_fall_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/10_10_spring_cw.py` & `not1mm-23.5.9.1/not1mm/plugins/10_10_spring_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/10_10_summer_phone.py` & `not1mm-23.5.9.1/not1mm/plugins/10_10_summer_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/10_10_winter_phone.py` & `not1mm-23.5.9.1/not1mm/plugins/10_10_winter_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/arrl_dx_cw.py` & `not1mm-23.5.9.1/not1mm/plugins/arrl_dx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-23.5.9.1/not1mm/plugins/arrl_dx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/arrl_field_day.py` & `not1mm-23.5.9.1/not1mm/plugins/arrl_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-23.5.9.1/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/arrl_ss_cw.py` & `not1mm-23.5.9.1/not1mm/plugins/arrl_ss_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/arrl_ss_phone.py` & `not1mm-23.5.9.1/not1mm/plugins/arrl_ss_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/cq_wpx_cw.py` & `not1mm-23.5.9.1/not1mm/plugins/cq_wpx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-23.5.9.1/not1mm/plugins/cq_wpx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/cq_ww_cw.py` & `not1mm-23.5.9.1/not1mm/plugins/cq_ww_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/cq_ww_ssb.py` & `not1mm-23.5.9.1/not1mm/plugins/cq_ww_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/cwt.py` & `not1mm-23.5.9.1/not1mm/plugins/cwt.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/general_logging.py` & `not1mm-23.5.9.1/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/jidx_cw.py` & `not1mm-23.5.9.1/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/jidx_ph.py` & `not1mm-23.5.9.1/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/plugins/winter_field_day.py` & `not1mm-23.5.9.1/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm/testing/test.py` & `not1mm-23.5.9.1/not1mm/testing/test.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/not1mm.egg-info/PKG-INFO` & `not1mm-23.5.9.1/not1mm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.9
+Version: 23.5.9.1
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -60,14 +60,16 @@
   - [Hiding screen elements](#hiding-screen-elements)
   - [Editing macro keys](#editing-macro-keys)
     - [Macro substitutions](#macro-substitutions)
     - [Macro use with voice](#macro-use-with-voice)
   - [cty.dat and QRZ lookups for distance and bearing](#ctydat-and-qrz-lookups-for-distance-and-bearing)
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
+    - [The Main Window](#the-main-window)
+      - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
     - [Bandmap](#bandmap)
   - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
@@ -112,15 +114,15 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother.
+- [23-5-9] Removed 1 second timers in the bandmap and log window, made them UDP readyRead(). Much smoother. Add CTRL-PgUp and CTRL-PgDown keys to jump to the next/prev spots in the bandmap. Fix: Voice not keying on LSB.
 - [23-5-8] Bandmap zoom in/out now centers scale to RX Freq.
 - [23-5-7] Added bandwidth marker to the bandmap.
 - [23-5-6] Added AR Cluster filter options for the bandmap. Added a station ID to the multicast packets. This will prevent erratic bevahiour if 2 stations are on the same network.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
@@ -384,14 +386,30 @@
 - [CW, SSB, RTTY] You can set the mode logged. If you have CAT control this will also change the mode on the radio.
 - [OPON] Change the operator currently logging.
 
 **You must press the SPACE bar after entering any of the above.**
 
 ## Windows
 
+### The Main Window
+
+#### Keyboard commands
+
+- [Esc] Clears the input fields of any text.
+- [CTRL-Esc] Stops cwdaemon from sending Morse.
+- [PgUp] Increases the cwdaemon sending speed.
+- [PgDown] Decreases the cwdaemon sending speed.
+- [CTRL-PgUp] Jump to the next spot above the current VFO cursor in the bamdmap window.
+- [CTRL-PgDown] Jump to the next spot below the current VFO cursor in the bamdmap window.
+- [TAB] Move cursor to the right one field.
+- [Shift-Tab] Move cursor left One field.
+- [SPACE] When in the callsign field, will move the input to the first field needed for the exchange.
+- [Enter] Submits the fields to the log.
+- [F1-F12] Send (CW or Voice) macros.
+
 ### Log Display
 
 `Window`>`Log Window`
 
 The Log display gets updated automatically when a contact is entered. The top half is a list of all contacts.
 
 ![Log Display Window](https://github.com/mbridak/not1mm/raw/master/pic/logdisplay.png)
@@ -400,15 +418,15 @@
 
 ### Bandmap
 
 `Window`>`Bandmap`
 
 Put your callsign in the top and press the connect button.
 
-The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. Clicked on spots now tune the radio and set the callsign field.
+The bandmap window is, as with everything, a work in progress. The bandmap now follows the VFO. VFO indicator now displays as small triangle in the frequency tickmarks. A small blue rectangle shows the receivers bandwidth. Clicked on spots now tune the radio and set the callsign field.
 
 ![Bandmap Window](https://github.com/mbridak/not1mm/raw/master/pic/bandmap.png)
 
 ## Editing a contact
 
 ![Editing a cell](https://github.com/mbridak/not1mm/raw/master/pic/edit_cell.png)
```

### Comparing `not1mm-23.5.9/not1mm.egg-info/SOURCES.txt` & `not1mm-23.5.9.1/not1mm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.9/pyproject.toml` & `not1mm-23.5.9.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "23.5.9"
+version = "23.5.9.1"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

### Comparing `not1mm-23.5.9/testing/test.py` & `not1mm-23.5.9.1/testing/test.py`

 * *Files identical despite different names*

