# Comparing `tmp/djaodjin-survey-0.9.6.tar.gz` & `tmp/djaodjin-survey-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djaodjin-survey-0.9.6.tar", last modified: Fri Apr 28 01:52:28 2023, max compression
+gzip compressed data, was "djaodjin-survey-0.9.7.tar", last modified: Fri May  5 18:13:48 2023, max compression
```

## Comparing `djaodjin-survey-0.9.6.tar` & `djaodjin-survey-0.9.7.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.934970 djaodjin-survey-0.9.6/
--rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/LICENSE.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/MANIFEST.in
--rw-r--r--   0 smirolo    (501) staff       (20)     1981 2023-04-28 01:52:28.935036 djaodjin-survey-0.9.6/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     1222 2023-04-28 01:50:26.000000 djaodjin-survey-0.9.6/README.md
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.917536 djaodjin-survey-0.9.6/djaodjin_survey.egg-info/
--rw-r--r--   0 smirolo    (501) staff       (20)     1981 2023-04-28 01:52:28.000000 djaodjin-survey-0.9.6/djaodjin_survey.egg-info/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     2399 2023-04-28 01:52:28.000000 djaodjin-survey-0.9.6/djaodjin_survey.egg-info/SOURCES.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-04-28 01:52:28.000000 djaodjin-survey-0.9.6/djaodjin_survey.egg-info/dependency_links.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       73 2023-04-28 01:52:28.000000 djaodjin-survey-0.9.6/djaodjin_survey.egg-info/requires.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-04-28 01:52:28.000000 djaodjin-survey-0.9.6/djaodjin_survey.egg-info/top_level.txt
--rw-r--r--   0 smirolo    (501) staff       (20)     1358 2023-04-18 19:54:04.000000 djaodjin-survey-0.9.6/pyproject.toml
--rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-04-28 01:52:28.935243 djaodjin-survey-0.9.6/setup.cfg
--rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-04-18 16:17:24.000000 djaodjin-survey-0.9.6/setup.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.921543 djaodjin-survey-0.9.6/survey/
--rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-04-28 01:50:37.000000 djaodjin-survey-0.9.6/survey/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1842 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/admin.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.924667 djaodjin-survey-0.9.6/survey/api/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-09-14 00:28:06.000000 djaodjin-survey-0.9.6/survey/api/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)    45132 2023-04-20 22:58:59.000000 djaodjin-survey-0.9.6/survey/api/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)    12575 2023-01-27 18:26:55.000000 djaodjin-survey-0.9.6/survey/api/metrics.py
--rw-r--r--   0 smirolo    (501) staff       (20)    23591 2023-03-23 22:52:31.000000 djaodjin-survey-0.9.6/survey/api/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)    56385 2023-04-07 16:36:46.000000 djaodjin-survey-0.9.6/survey/api/sample.py
--rw-r--r--   0 smirolo    (501) staff       (20)    23875 2023-04-20 22:58:12.000000 djaodjin-survey-0.9.6/survey/api/serializers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2929 2023-03-10 17:42:57.000000 djaodjin-survey-0.9.6/survey/api/serializers_overrides.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5569 2023-04-13 17:06:50.000000 djaodjin-survey-0.9.6/survey/api/units.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4094 2022-09-26 17:15:24.000000 djaodjin-survey-0.9.6/survey/compat.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2316 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/docs.py
--rw-r--r--   0 smirolo    (501) staff       (20)    17450 2023-04-07 16:40:09.000000 djaodjin-survey-0.9.6/survey/filters.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8639 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/forms.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6173 2023-04-05 16:25:51.000000 djaodjin-survey-0.9.6/survey/helpers.py
--rw-r--r--   0 smirolo    (501) staff       (20)    14690 2023-04-18 18:56:44.000000 djaodjin-survey-0.9.6/survey/mixins.py
--rw-r--r--   0 smirolo    (501) staff       (20)    39683 2023-04-05 17:20:30.000000 djaodjin-survey-0.9.6/survey/models.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4007 2023-04-05 18:59:23.000000 djaodjin-survey-0.9.6/survey/pagination.py
--rw-r--r--   0 smirolo    (501) staff       (20)    13064 2023-04-05 17:26:46.000000 djaodjin-survey-0.9.6/survey/queries.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4395 2023-03-21 20:59:50.000000 djaodjin-survey-0.9.6/survey/settings.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1955 2022-10-04 20:48:04.000000 djaodjin-survey-0.9.6/survey/signals.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.915319 djaodjin-survey-0.9.6/survey/static/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.924927 djaodjin-survey-0.9.6/survey/static/css/
--rw-r--r--   0 smirolo    (501) staff       (20)      296 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/static/css/matrix-chart.css
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.926879 djaodjin-survey-0.9.6/survey/static/js/
--rw-r--r--   0 smirolo    (501) staff       (20)    12547 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/static/js/djaodjin-categorize.js
--rw-r--r--   0 smirolo    (501) staff       (20)    15443 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/static/js/djaodjin-matrix.js
--rw-r--r--   0 smirolo    (501) staff       (20)    51604 2023-04-14 15:55:35.000000 djaodjin-survey-0.9.6/survey/static/js/djaodjin-resources-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)     5462 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/static/js/djaodjin-set.js
--rw-r--r--   0 smirolo    (501) staff       (20)    17193 2023-04-14 16:37:55.000000 djaodjin-survey-0.9.6/survey/static/js/djaodjin-survey-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)      544 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/static/js/djaodjin-survey.js
--rw-r--r--   0 smirolo    (501) staff       (20)    12995 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/static/js/matrix-chart.js
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.915434 djaodjin-survey-0.9.6/survey/templates/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.928635 djaodjin-survey-0.9.6/survey/templates/survey/
--rw-r--r--   0 smirolo    (501) staff       (20)      667 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/answer_form.html
--rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/campaign_form.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.928770 djaodjin-survey-0.9.6/survey/templates/survey/campaigns/
--rw-r--r--   0 smirolo    (501) staff       (20)     1184 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/campaigns/index.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2529 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/categorize.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.929430 djaodjin-survey-0.9.6/survey/templates/survey/matrix/
--rw-r--r--   0 smirolo    (501) staff       (20)       62 2023-01-19 22:34:30.000000 djaodjin-survey-0.9.6/survey/templates/survey/matrix/compare.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2087 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/matrix/index.html
--rw-r--r--   0 smirolo    (501) staff       (20)     4088 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/matrix/matrix.html
--rw-r--r--   0 smirolo    (501) staff       (20)     9287 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/portfolios.html
--rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/question_form.html
--rw-r--r--   0 smirolo    (501) staff       (20)     1572 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/question_list.html
--rw-r--r--   0 smirolo    (501) staff       (20)      471 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/respondent_list.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2077 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/result.html
--rw-r--r--   0 smirolo    (501) staff       (20)      983 2023-03-10 17:29:52.000000 djaodjin-survey-0.9.6/survey/templates/survey/result_quizz.html
--rw-r--r--   0 smirolo    (501) staff       (20)      562 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/sample_create.html
--rw-r--r--   0 smirolo    (501) staff       (20)      356 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/sample_update.html
--rw-r--r--   0 smirolo    (501) staff       (20)      245 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templates/survey/send.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.929655 djaodjin-survey-0.9.6/survey/templatetags/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/templatetags/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1769 2023-02-10 21:30:25.000000 djaodjin-survey-0.9.6/survey/templatetags/survey_tags.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.929873 djaodjin-survey-0.9.6/survey/urls/
--rw-r--r--   0 smirolo    (501) staff       (20)     1533 2022-09-25 23:08:10.000000 djaodjin-survey-0.9.6/survey/urls/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.931523 djaodjin-survey-0.9.6/survey/urls/api/
--rw-r--r--   0 smirolo    (501) staff       (20)     1718 2023-03-22 18:00:00.000000 djaodjin-survey-0.9.6/survey/urls/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1653 2022-09-26 00:12:56.000000 djaodjin-survey-0.9.6/survey/urls/api/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2772 2022-09-26 02:10:24.000000 djaodjin-survey-0.9.6/survey/urls/api/filters.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2125 2023-04-07 17:48:09.000000 djaodjin-survey-0.9.6/survey/urls/api/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1717 2022-09-26 00:13:35.000000 djaodjin-survey-0.9.6/survey/urls/api/metrics.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1622 2022-09-26 00:12:26.000000 djaodjin-survey-0.9.6/survey/urls/api/noauth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2390 2023-03-07 21:45:05.000000 djaodjin-survey-0.9.6/survey/urls/api/portfolios.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.932192 djaodjin-survey-0.9.6/survey/urls/api/sample/
--rw-r--r--   0 smirolo    (501) staff       (20)     1512 2022-09-26 00:09:27.000000 djaodjin-survey-0.9.6/survey/urls/api/sample/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1722 2023-02-21 21:54:31.000000 djaodjin-survey-0.9.6/survey/urls/api/sample/reset.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2830 2023-04-07 17:59:33.000000 djaodjin-survey-0.9.6/survey/urls/api/sample/update.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.933471 djaodjin-survey-0.9.6/survey/urls/views/
--rw-r--r--   0 smirolo    (501) staff       (20)     1714 2023-03-22 18:07:23.000000 djaodjin-survey-0.9.6/survey/urls/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2942 2022-09-26 00:06:32.000000 djaodjin-survey-0.9.6/survey/urls/views/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2105 2023-01-19 22:50:22.000000 djaodjin-survey-0.9.6/survey/urls/views/matrices.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1894 2023-01-25 23:37:48.000000 djaodjin-survey-0.9.6/survey/urls/views/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2180 2022-09-26 00:14:39.000000 djaodjin-survey-0.9.6/survey/urls/views/samples.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9471 2023-04-20 22:32:58.000000 djaodjin-survey-0.9.6/survey/utils.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-28 01:52:28.934726 djaodjin-survey-0.9.6/survey/views/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8457 2023-03-21 21:02:40.000000 djaodjin-survey-0.9.6/survey/views/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5626 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/views/createquestion.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1898 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.6/survey/views/edit.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6155 2023-04-07 17:48:37.000000 djaodjin-survey-0.9.6/survey/views/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4391 2023-03-21 21:10:13.000000 djaodjin-survey-0.9.6/survey/views/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)    11685 2023-03-21 20:44:41.000000 djaodjin-survey-0.9.6/survey/views/sample.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.669855 djaodjin-survey-0.9.7/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/LICENSE.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/MANIFEST.in
+-rw-r--r--   0 smirolo    (501) staff       (20)     1932 2023-05-05 18:13:48.669922 djaodjin-survey-0.9.7/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     1173 2023-05-05 18:12:15.000000 djaodjin-survey-0.9.7/README.md
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.651610 djaodjin-survey-0.9.7/djaodjin_survey.egg-info/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1932 2023-05-05 18:13:48.000000 djaodjin-survey-0.9.7/djaodjin_survey.egg-info/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     2399 2023-05-05 18:13:48.000000 djaodjin-survey-0.9.7/djaodjin_survey.egg-info/SOURCES.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-05-05 18:13:48.000000 djaodjin-survey-0.9.7/djaodjin_survey.egg-info/dependency_links.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       73 2023-05-05 18:13:48.000000 djaodjin-survey-0.9.7/djaodjin_survey.egg-info/requires.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-05-05 18:13:48.000000 djaodjin-survey-0.9.7/djaodjin_survey.egg-info/top_level.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)     1358 2023-04-18 19:54:04.000000 djaodjin-survey-0.9.7/pyproject.toml
+-rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-05-05 18:13:48.670123 djaodjin-survey-0.9.7/setup.cfg
+-rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-04-18 16:17:24.000000 djaodjin-survey-0.9.7/setup.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.655850 djaodjin-survey-0.9.7/survey/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-05-05 18:11:51.000000 djaodjin-survey-0.9.7/survey/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1842 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/admin.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.659905 djaodjin-survey-0.9.7/survey/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-09-14 00:28:06.000000 djaodjin-survey-0.9.7/survey/api/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    45858 2023-05-05 17:40:52.000000 djaodjin-survey-0.9.7/survey/api/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12575 2023-01-27 18:26:55.000000 djaodjin-survey-0.9.7/survey/api/metrics.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    26832 2023-05-05 17:25:00.000000 djaodjin-survey-0.9.7/survey/api/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    58251 2023-05-05 17:22:48.000000 djaodjin-survey-0.9.7/survey/api/sample.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    24572 2023-05-05 17:16:15.000000 djaodjin-survey-0.9.7/survey/api/serializers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2929 2023-03-10 17:42:57.000000 djaodjin-survey-0.9.7/survey/api/serializers_overrides.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5569 2023-04-13 17:06:50.000000 djaodjin-survey-0.9.7/survey/api/units.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4094 2022-09-26 17:15:24.000000 djaodjin-survey-0.9.7/survey/compat.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2316 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/docs.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    17450 2023-04-07 16:40:09.000000 djaodjin-survey-0.9.7/survey/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8639 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/forms.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6173 2023-04-05 16:25:51.000000 djaodjin-survey-0.9.7/survey/helpers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    14735 2023-05-04 19:49:21.000000 djaodjin-survey-0.9.7/survey/mixins.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    39897 2023-05-02 16:54:48.000000 djaodjin-survey-0.9.7/survey/models.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4007 2023-04-05 18:59:23.000000 djaodjin-survey-0.9.7/survey/pagination.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    13064 2023-04-05 17:26:46.000000 djaodjin-survey-0.9.7/survey/queries.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4395 2023-03-21 20:59:50.000000 djaodjin-survey-0.9.7/survey/settings.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1955 2022-10-04 20:48:04.000000 djaodjin-survey-0.9.7/survey/signals.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.649420 djaodjin-survey-0.9.7/survey/static/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.660166 djaodjin-survey-0.9.7/survey/static/css/
+-rw-r--r--   0 smirolo    (501) staff       (20)      296 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/static/css/matrix-chart.css
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.662171 djaodjin-survey-0.9.7/survey/static/js/
+-rw-r--r--   0 smirolo    (501) staff       (20)    12547 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/static/js/djaodjin-categorize.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    15443 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/static/js/djaodjin-matrix.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    51604 2023-04-14 15:55:35.000000 djaodjin-survey-0.9.7/survey/static/js/djaodjin-resources-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     5462 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/static/js/djaodjin-set.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    17193 2023-04-14 16:37:55.000000 djaodjin-survey-0.9.7/survey/static/js/djaodjin-survey-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)      544 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/static/js/djaodjin-survey.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    12995 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/static/js/matrix-chart.js
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.649535 djaodjin-survey-0.9.7/survey/templates/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.663943 djaodjin-survey-0.9.7/survey/templates/survey/
+-rw-r--r--   0 smirolo    (501) staff       (20)      667 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/answer_form.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/campaign_form.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.664077 djaodjin-survey-0.9.7/survey/templates/survey/campaigns/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1184 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/campaigns/index.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2529 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/categorize.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.664664 djaodjin-survey-0.9.7/survey/templates/survey/matrix/
+-rw-r--r--   0 smirolo    (501) staff       (20)       62 2023-01-19 22:34:30.000000 djaodjin-survey-0.9.7/survey/templates/survey/matrix/compare.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2087 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/matrix/index.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     4088 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/matrix/matrix.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     9287 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/portfolios.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/question_form.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     1572 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/question_list.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      471 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/respondent_list.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2077 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/result.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      983 2023-03-10 17:29:52.000000 djaodjin-survey-0.9.7/survey/templates/survey/result_quizz.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      562 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/sample_create.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      356 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/sample_update.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      245 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/send.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.664893 djaodjin-survey-0.9.7/survey/templatetags/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templatetags/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1769 2023-02-10 21:30:25.000000 djaodjin-survey-0.9.7/survey/templatetags/survey_tags.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.665095 djaodjin-survey-0.9.7/survey/urls/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1533 2022-09-25 23:08:10.000000 djaodjin-survey-0.9.7/survey/urls/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.666601 djaodjin-survey-0.9.7/survey/urls/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1718 2023-03-22 18:00:00.000000 djaodjin-survey-0.9.7/survey/urls/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1653 2022-09-26 00:12:56.000000 djaodjin-survey-0.9.7/survey/urls/api/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2772 2022-09-26 02:10:24.000000 djaodjin-survey-0.9.7/survey/urls/api/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2125 2023-04-07 17:48:09.000000 djaodjin-survey-0.9.7/survey/urls/api/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1717 2022-09-26 00:13:35.000000 djaodjin-survey-0.9.7/survey/urls/api/metrics.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1622 2022-09-26 00:12:26.000000 djaodjin-survey-0.9.7/survey/urls/api/noauth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2390 2023-03-07 21:45:05.000000 djaodjin-survey-0.9.7/survey/urls/api/portfolios.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.667163 djaodjin-survey-0.9.7/survey/urls/api/sample/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1512 2022-09-26 00:09:27.000000 djaodjin-survey-0.9.7/survey/urls/api/sample/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1722 2023-02-21 21:54:31.000000 djaodjin-survey-0.9.7/survey/urls/api/sample/reset.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2830 2023-04-07 17:59:33.000000 djaodjin-survey-0.9.7/survey/urls/api/sample/update.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.668301 djaodjin-survey-0.9.7/survey/urls/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1714 2023-03-22 18:07:23.000000 djaodjin-survey-0.9.7/survey/urls/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2942 2022-09-26 00:06:32.000000 djaodjin-survey-0.9.7/survey/urls/views/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2105 2023-01-19 22:50:22.000000 djaodjin-survey-0.9.7/survey/urls/views/matrices.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1894 2023-01-25 23:37:48.000000 djaodjin-survey-0.9.7/survey/urls/views/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2180 2022-09-26 00:14:39.000000 djaodjin-survey-0.9.7/survey/urls/views/samples.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9471 2023-04-20 22:32:58.000000 djaodjin-survey-0.9.7/survey/utils.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.669602 djaodjin-survey-0.9.7/survey/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8457 2023-03-21 21:02:40.000000 djaodjin-survey-0.9.7/survey/views/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5626 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/views/createquestion.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1898 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/views/edit.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6155 2023-04-07 17:48:37.000000 djaodjin-survey-0.9.7/survey/views/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4391 2023-03-21 21:10:13.000000 djaodjin-survey-0.9.7/survey/views/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    11685 2023-03-21 20:44:41.000000 djaodjin-survey-0.9.7/survey/views/sample.py
```

### Comparing `djaodjin-survey-0.9.6/LICENSE.txt` & `djaodjin-survey-0.9.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/PKG-INFO` & `djaodjin-survey-0.9.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djaodjin-survey
-Version: 0.9.6
+Version: 0.9.7
 Summary: Django app for qualitative and quantitative surveys
 Author-email: The DjaoDjin Team <help@djaodjin.com>
 Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/djaodjin/djaodjin-survey
 Project-URL: documentation, https://djaodjin-survey.readthedocs.io/
 Project-URL: changelog, https://github.com/djaodjin/djaodjin-survey/changelog
@@ -47,17 +47,16 @@
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest)
 - **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.9.6
+0.9.7
 
-  * serializes default_unit.system correctly in benchmarks API
-  * renames data series name from 'printable_name' to 'title' for consistency
-  * computes rate on target dates
+  * prevents extra data to leak through API under unexpected conditions
+  * uses prefix to filter questions in benchmarks API
 
 [previous release notes](changelog)
 
 
 Models have been completely re-designed between version 0.1.7 and 0.2.0
```

### Comparing `djaodjin-survey-0.9.6/djaodjin_survey.egg-info/PKG-INFO` & `djaodjin-survey-0.9.7/djaodjin_survey.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djaodjin-survey
-Version: 0.9.6
+Version: 0.9.7
 Summary: Django app for qualitative and quantitative surveys
 Author-email: The DjaoDjin Team <help@djaodjin.com>
 Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/djaodjin/djaodjin-survey
 Project-URL: documentation, https://djaodjin-survey.readthedocs.io/
 Project-URL: changelog, https://github.com/djaodjin/djaodjin-survey/changelog
@@ -47,17 +47,16 @@
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest)
 - **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.9.6
+0.9.7
 
-  * serializes default_unit.system correctly in benchmarks API
-  * renames data series name from 'printable_name' to 'title' for consistency
-  * computes rate on target dates
+  * prevents extra data to leak through API under unexpected conditions
+  * uses prefix to filter questions in benchmarks API
 
 [previous release notes](changelog)
 
 
 Models have been completely re-designed between version 0.1.7 and 0.2.0
```

### Comparing `djaodjin-survey-0.9.6/djaodjin_survey.egg-info/SOURCES.txt` & `djaodjin-survey-0.9.7/djaodjin_survey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/pyproject.toml` & `djaodjin-survey-0.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/setup.py` & `djaodjin-survey-0.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/__init__.py` & `djaodjin-survey-0.9.7/survey/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the survey django app.
 """
 
-__version__ = '0.9.6'
+__version__ = '0.9.7'
```

### Comparing `djaodjin-survey-0.9.6/survey/admin.py` & `djaodjin-survey-0.9.7/survey/admin.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/api/campaigns.py` & `djaodjin-survey-0.9.7/survey/api/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/api/matrix.py` & `djaodjin-survey-0.9.7/survey/api/matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,19 +71,20 @@
         return get_accessible_accounts(grantees, campaign=self.campaign)
 
     def get_questions(self, prefix):
         """
         Overrides CampaignContentMixin.get_questions to return a list
         of questions based on the answers available in the benchmarkd samples.
         """
-        if not prefix.endswith(settings.DB_PATH_SEP):
-            prefix = prefix + settings.DB_PATH_SEP
+        qualified_prefix = prefix
+        if not qualified_prefix.endswith(settings.DB_PATH_SEP):
+            qualified_prefix = qualified_prefix + settings.DB_PATH_SEP
 
         questions_queryset = get_question_model().objects.filter(
-            path__startswith=self.db_path).values(
+            Q(path=prefix) | Q(path__startswith=qualified_prefix)).values(
             'pk', 'path', 'ui_hint', 'content__title',
             'default_unit__slug', 'default_unit__title',
             'default_unit__system')
         questions_by_key = {question['pk']: {
             'path': question['path'],
             'title': question['content__title'],
             'ui_hint': question['ui_hint'],
@@ -123,19 +124,23 @@
                 }
                 for key, val in six.iteritems(question.get('rate', {})):
                     account_benchmark['values'] += [(key, int(val))]
                 question['benchmarks'] += [account_benchmark]
 
 
     def attach_results(self, questions_by_key, account=None):
+        account_slug = "all"
+        account_title = "All"
         if not account:
             account = self.account
+            account_slug = account.slug
+            account_title = account.printable_name
         accessible_accounts = self.get_accessible_accounts([account])
         self._attach_results(questions_by_key, accessible_accounts,
-            account.printable_name, account.slug)
+            account_title, account_slug)
 
 
 class BenchmarkAPIView(BenchmarkMixin, generics.ListAPIView):
     """
     Aggregated benchmark for requested accounts
 
     **Examples**:
@@ -187,15 +192,36 @@
         {
           "count": 4,
           "results": []
         }
     """
 
 
-class SampleBenchmarksAPIView(SampleMixin, BenchmarkAPIView):
+class SampleBenchmarkMixin(SampleMixin, BenchmarkMixin):
+
+    @property
+    def campaign(self):
+        #pylint:disable=attribute-defined-outside-init
+        if not hasattr(self, '_campaign'):
+            self._campaign = self.sample.campaign
+        return self._campaign
+
+    @property
+    def ends_at(self):
+        #pylint:disable=attribute-defined-outside-init
+        if not hasattr(self, '_ends_at'):
+            self._ends_at = (self.sample.created_at if self.sample.is_frozen
+                else datetime_or_now())
+        return self._ends_at
+
+    def get_accessible_accounts(self, grantees):
+        return get_account_model().objects.all()
+
+
+class SampleBenchmarksAPIView(SampleBenchmarkMixin, generics.ListAPIView):
     """
     Benchmark a sub-tree of questions against peers
 
     **Examples**:
 
     .. code-block:: http
 
@@ -208,31 +234,26 @@
 
 
         {
           "count": 4,
           "results": []
         }
     """
-    @property
-    def campaign(self):
-        #pylint:disable=attribute-defined-outside-init
-        if not hasattr(self, '_campaign'):
-            self._campaign = self.sample.campaign
-        return self._campaign
+    serializer_class = SampleBenchmarksSerializer
+    pagination_class = MetricsPagination
 
-    @property
-    def ends_at(self):
-        #pylint:disable=attribute-defined-outside-init
-        if not hasattr(self, '_ends_at'):
-            self._ends_at = (self.sample.created_at if self.sample.is_frozen
-                else datetime_or_now())
-        return self._ends_at
+    def get_serializer_context(self):
+        context = super(SampleBenchmarksAPIView, self).get_serializer_context()
+        context.update({
+            'prefix': self.db_path if self.db_path else settings.DB_PATH_SEP,
+        })
+        return context
 
-    def get_accessible_accounts(self, grantees):
-        return get_account_model().objects.all()
+    def get_queryset(self):
+        return self.get_questions(self.db_path)
 
 
 class SampleBenchmarksIndexAPIView(SampleBenchmarksAPIView):
     """
     Benchmark against peers
 
     **Examples**:
```

### Comparing `djaodjin-survey-0.9.6/survey/api/metrics.py` & `djaodjin-survey-0.9.7/survey/api/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/api/portfolios.py` & `djaodjin-survey-0.9.7/survey/api/portfolios.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, DjaoDjin inc.
+# Copyright (c) 2023, DjaoDjin inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -22,39 +22,37 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import logging
 
 from dateutil.relativedelta import relativedelta
 from django.db import transaction
-from django.db.models import Q
+from django.db.models import Max, Q
 from rest_framework import generics, status
 from rest_framework.exceptions import ValidationError
 from rest_framework.response import Response as HttpResponse
 
 from .. import settings, signals
 from ..compat import six, gettext_lazy as _
 from ..docs import OpenAPIResponse, swagger_auto_schema
 from ..mixins import AccountMixin
-from ..models import PortfolioDoubleOptIn
-from .serializers import (NoModelSerializer, PortfolioOptInSerializer,
-    PortfolioOptInUpdateSerializer, PortfolioGrantCreateSerializer,
-    PortfolioRequestCreateSerializer)
+from ..models import Portfolio, PortfolioDoubleOptIn, Sample
+from .serializers import (NoModelSerializer, PortfolioReceivedSerializer,
+    PortfolioOptInSerializer, PortfolioOptInUpdateSerializer,
+    PortfolioGrantCreateSerializer, PortfolioRequestCreateSerializer)
 from ..filters import (DateRangeFilter, DoubleOptInStateFilter, OrderingFilter,
      SearchFilter)
 from ..utils import datetime_or_now, get_account_model
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 class SmartPortfolioListMixin(AccountMixin):
 
-    serializer_class = PortfolioOptInSerializer
-
     search_fields = (
         'grantee__full_name',
         'account__full_name',
     )
 
     ordering_fields = [
         ('grantee__full_name', 'grantee'),
@@ -96,31 +94,84 @@
             "count": 1,
             "next": null,
             "previous": null,
             "results": [
               {
                 "grantee": "energy-utility",
                 "account": "supplier-1",
-                "campaign": "sustainability",
+                "campaign": {
+                    "slug": "sustainability",
+                    "title": "ESG/Environmental practices",
+                    "account": "tspproject"
+                },
                 "ends_at": "2022-01-01T00:00:00Z",
                 "state": "request-initiated",
                 "api_accept": "/api/supplier-1/portfolios/requests/\
 0000000000000000000000000000000000000002/"
               }
             ]
         }
     """
+    serializer_class = PortfolioReceivedSerializer
+
+    def decorate_queryset(self, queryset):
+        latest_frozen_by_campaigns = {}
+        latest_shared_by_campaigns = {}
+        for optin in queryset:
+            campaign = optin.campaign
+            query_kwargs = {'campaign': campaign} if campaign else {}
+            optin.expected_behavior = optin.EXPECTED_CREATE
+            if campaign:
+                latest_frozen_at = latest_frozen_by_campaigns.get(campaign)
+                if (not latest_frozen_at and
+                    campaign not in latest_frozen_by_campaigns):
+                    latest_frozen_at = Sample.objects.filter(
+                        account=self.account, is_frozen=True,
+                        **query_kwargs).aggregate(Max('created_at'))
+                    if latest_frozen_at:
+                        latest_frozen_at = latest_frozen_at.get(
+                            'created_at__max')
+                    latest_frozen_by_campaigns.update({
+                        campaign: latest_frozen_at})
+
+                latest_shared_at = latest_shared_by_campaigns.get(campaign)
+                if (not latest_shared_at and
+                    campaign not in latest_shared_by_campaigns):
+                    latest_shared_at = Portfolio.objects.filter(
+                        account=self.account, grantee=optin.grantee,
+                        **query_kwargs).aggregate(Max('ends_at'))
+                    if latest_shared_at:
+                        latest_shared_at = latest_shared_at.get('ends_at__max')
+                    latest_shared_by_campaigns.update({
+                        campaign: latest_shared_at})
+
+                # compute expected behavior
+                if not latest_frozen_at:
+                    optin.expected_behavior = optin.EXPECTED_CREATE
+                elif (not latest_shared_at and
+                      latest_frozen_at < latest_shared_at and
+                      latest_shared_at < optin.created_at):
+                    optin.expected_behavior = optin.EXPECTED_UPDATE
+                else:
+                    optin.expected_behavior = optin.EXPECTED_SHARE
+
+        return queryset
+
 
     def get_queryset(self):
         return PortfolioDoubleOptIn.objects.filter(
             (Q(account=self.account) &
             Q(state=PortfolioDoubleOptIn.OPTIN_REQUEST_INITIATED)) |
             (Q(grantee=self.account) &
             Q(state=PortfolioDoubleOptIn.OPTIN_GRANT_INITIATED)))
 
+    def paginate_queryset(self, queryset):
+        page = super(PortfoliosAPIView, self).paginate_queryset(queryset)
+        return self.decorate_queryset(page if page else queryset)
+
 
 class PortfoliosGrantsAPIView(SmartPortfolioListMixin,
                               generics.ListCreateAPIView):
     """
     Lists initiated grants
 
     Lists all grants currently pending initiated by *account*.
@@ -141,25 +192,29 @@
             "count": 1,
             "next": null,
             "previous": null,
             "results": [
                 {
                   "grantee": "water-utility",
                   "account": "supplier-1",
-                  "campaign": "sustainability",
+                  "campaign": {
+                      "slug": "sustainability",
+                      "title": "ESG/Environmental practices",
+                      "account": "tspproject"
+                  },
                   "ends_at": "2022-01-01T00:00:00Z",
                   "state": "grant-initiated",
                   "api_accept": "/api/water-utility/portfolios/grants\
 /0000000000000000000000000000000000000003/"
                  }
             ]
         }
     """
-    serializer_class = PortfolioOptInSerializer
     lookup_field = settings.ACCOUNT_LOOKUP_FIELD
+    serializer_class = PortfolioOptInSerializer
 
     def get_queryset(self):
         return PortfolioDoubleOptIn.objects.filter(
             Q(account=self.account) &
             Q(state=PortfolioDoubleOptIn.OPTIN_GRANT_INITIATED))
 
     def get_serializer_class(self):
@@ -198,15 +253,15 @@
         .. code-block:: json
 
             {
                "count": 1,
                "results": [{
                  "grantee": "water-utility",
                  "account": "supplier-1",
-                 "campaign": "sustainability",
+                 "campaign": null,
                  "ends_at": "2022-01-01T00:00:00Z",
                  "state": "grant-initiated",
                  "api_accept": "/api/water-utility/portfolios/grants\
 /0000000000000000000000000000000000000003/"
                }]
             }
         """
@@ -418,32 +473,44 @@
             "count": 3,
             "next": null,
             "previous": null,
             "results": [
               {
                 "grantee": "energy-utility",
                 "account": "supplier-1",
-                "campaign": "sustainability",
+                "campaign": {
+                    "slug": "sustainability",
+                    "title": "ESG/Environmental practices",
+                    "account": "tspproject"
+                },
                 "ends_at": "2022-01-01T00:00:00Z",
                 "state": "request-denied",
                 "api_accept": null
               },
               {
                 "grantee": "energy-utility",
                 "account": "supplier-1",
-                "campaign": "sustainability",
+                "campaign": {
+                    "slug": "sustainability",
+                    "title": "ESG/Environmental practices",
+                    "account": "tspproject"
+                },
                 "ends_at": "2022-01-01T00:00:00Z",
                 "state": "request-initiated",
                 "api_accept": "/api/supplier-1/portfolios/requests/\
 0000000000000000000000000000000000000002/"
               },
               {
                 "grantee": "energy-utility",
                 "account": "andy-shop",
-                "campaign": "sustainability",
+                "campaign": {
+                    "slug": "sustainability",
+                    "title": "ESG/Environmental practices",
+                    "account": "tspproject"
+                },
                 "ends_at": "2022-01-01T00:00:00Z",
                 "state": "request-initiated",
                 "api_accept": "/api/andy-shop/portfolios/requests/\
 0000000000000000000000000000000000000004/"
               }
             ]
         }
@@ -651,15 +718,19 @@
     responds
 
     .. code-block:: json
 
         {
           "grantee": "energy-utility",
           "account": "supplier-1",
-          "campaign": "sustainability",
+          "campaign": {
+              "slug": "sustainability",
+              "title": "ESG/Environmental practices",
+              "account": "tspproject"
+          },
           "ends_at": "2022-01-01T00:00:00Z",
           "state": "request-denied",
           "api_accept": null,
           "extra": {"tags": "tier1"}
         }
     """
     target_url_kwarg = 'target'
```

### Comparing `djaodjin-survey-0.9.6/survey/api/sample.py` & `djaodjin-survey-0.9.7/survey/api/sample.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from rest_framework.generics import get_object_or_404
 from rest_framework.status import HTTP_200_OK, HTTP_201_CREATED
 
 from ..compat import six, is_authenticated
 from ..docs import OpenAPIResponse, swagger_auto_schema
 from ..filters import DateRangeFilter, OrderingFilter, SampleStateFilter
 from ..mixins import AccountMixin, SampleMixin
-from ..models import Answer, Choice, Sample, Unit, UnitEquivalences
+from ..models import Answer, Choice, Portfolio, Sample, Unit, UnitEquivalences
 from ..queries import is_sqlite3
 from ..utils import datetime_or_now, get_question_model, get_user_serializer
 from .serializers import (AnswerSerializer, NoModelSerializer,
     SampleAnswerSerializer, SampleCreateSerializer, SampleSerializer)
 
 
 LOGGER = logging.getLogger(__name__)
@@ -307,15 +307,18 @@
 
     {
         "slug": "46f66f70f5ad41b29c4df08f683a9a7a",
         "created_at": "2018-01-24T17:03:34.926193Z",
         "updated_at": "2018-01-24T17:03:34.926193Z",
         "is_frozen": false,
         "account": "supplier-1",
-        "campaign": "sustainability"
+        "campaign": {
+            "slug": "sustainability",
+            "title": "ESG/Environmental practices"
+        }
     }
     """
     serializer_class = SampleSerializer
 
     def get_object(self):
         return self.sample
 
@@ -731,15 +734,16 @@
         user = self.request.user if is_authenticated(self.request) else None
         created_at = datetime_or_now()
         at_least_one_created = False
         results = []
         errors = []
 
         if self.sample.is_frozen:
-            raise ValidationError("sample is frozen")
+            raise ValidationError({
+                'detail': "cannot update answers in a frozen sample"})
 
         for datapoint in validated_data:
             measured = datapoint.get('measured', None)
             if not measured:
                 continue
             try:
                 answer, created = update_or_create_answer(
@@ -1056,15 +1060,16 @@
         if self.request.method.lower() == 'post':
             return NoModelSerializer
         return super(SampleCandidatesAPIView, self).get_serializer_class()
 
     def create(self, request, *args, **kwargs):
         #pylint:disable=too-many-locals
         if self.sample.is_frozen:
-            raise ValidationError("sample is frozen")
+            raise ValidationError({
+                'detail': "cannot update answers in a frozen sample"})
 
         at_time = datetime_or_now()
         at_least_one_created = False
         first_answer = not(Answer.objects.filter(
             collected_by=self.request.user).exists())
         answered = Answer.objects.filter(
             sample=self.sample).values_list('question_id', flat=True)
@@ -1360,14 +1365,16 @@
             "campaign": "sustainability",
             "is_frozen": true
         }
     """
     serializer_class = SampleSerializer
 
     def create(self, request, *args, **kwargs):
+        if self.sample.is_frozen:
+            raise ValidationError({'detail': "sample is already frozen"})
         self.sample.is_frozen = True
         self.sample.save()
         serializer = self.get_serializer(self.sample)
         return http.Response(serializer.data)
 
 
 class SampleResetAPIView(SampleMixin, generics.CreateAPIView):
@@ -1400,14 +1407,17 @@
             "created_at": "2018-01-24T17:03:34.926193Z",
             "campaign": "sustainability"
         }
     """
     serializer_class = SampleSerializer
 
     def create(self, request, *args, **kwargs):
+        if self.sample.is_frozen:
+            raise ValidationError({
+                'detail': "cannot update answers in a frozen sample"})
         prefix = self.path
         if prefix:
             queryset = self.sample.answers.filter(
                 question__path__startswith=prefix)
         else:
             queryset = self.sample.answers.all()
         unit_slug = request.query_params.get('unit')
@@ -1450,17 +1460,17 @@
             "created_at": "2018-01-24T17:03:34.926193Z",
             "campaign": "sustainability"
         }
     """
 
 class SampleRecentCreateAPIView(AccountMixin, generics.ListCreateAPIView):
     """
-    Lists updatable samples
+    Lists historical samples
 
-    This API end-point returns all samples which have not been frozen
+    This API end-point returns all samples which have or have not been frozen
     for an account.
 
     **Tags**: assessments
 
     **Examples**
 
     .. code-block:: http
@@ -1501,20 +1511,52 @@
 
     ordering = ('-created_at',)
 
     filter_backends = (DateRangeFilter, SampleStateFilter, OrderingFilter)
 
     serializer_class = SampleSerializer
 
+    def decorate_queryset(self, queryset):
+        frozen_by_campaigns = {}
+        for sample in queryset:
+            if sample.is_frozen:
+                if sample.campaign not in frozen_by_campaigns:
+                    frozen_by_campaigns[sample.campaign] = [sample]
+                else:
+                    frozen_by_campaigns[sample.campaign] += [sample]
+        for campaign, samples in six.iteritems(frozen_by_campaigns):
+            next_level = Portfolio.objects.filter(
+                account=self.account, campaign=campaign).values(
+                    'ends_at', 'grantee__slug').order_by('-ends_at')
+            for sample in sorted(samples,
+                        key=lambda smp: smp.created_at, reverse=True):
+                sample.grantees = []
+                level = next_level
+                next_level = []
+                for accessible in level:
+                    ends_at = accessible.get('ends_at')
+                    grantee = accessible.get('grantee__slug')
+                    if sample.created_at <= ends_at:
+                        sample.grantees += [grantee]
+                    else:
+                        next_level += [accessible]
+        return queryset
+
+
     def get_queryset(self):
         return Sample.objects.filter(
             account=self.account,
             extra__isnull=True         # XXX convinience
         ).select_related('campaign')
 
+    def paginate_queryset(self, queryset):
+        page = super(
+            SampleRecentCreateAPIView, self).paginate_queryset(queryset)
+        return self.decorate_queryset(page if page else queryset)
+
     @swagger_auto_schema(request_body=SampleCreateSerializer)
     def post(self, request, *args, **kwargs):
         """
         Creates a new sample
 
         Creates a new sample to record qualitative and/or quantitative data.
```

### Comparing `djaodjin-survey-0.9.6/survey/api/serializers.py` & `djaodjin-survey-0.9.7/survey/api/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,15 @@
     """
     Short description of the campaign.
     """
 
     account = serializers.SlugRelatedField(
         slug_field=settings.BELONGS_LOOKUP_FIELD,
         queryset=get_belongs_model().objects.all(),
-        help_text=("Account this sample belongs to."))
+        help_text=_("Account this sample belongs to."))
 
     class Meta(object):
         model = Campaign
         fields = ('slug', 'account', 'title', 'description', 'created_at',
             'active')
         read_only_fields = ('slug', 'account', 'created_at')
 
@@ -278,52 +278,54 @@
 
 
 class CampaignDetailSerializer(serializers.ModelSerializer):
 
     account = serializers.SlugRelatedField(
         slug_field=settings.BELONGS_LOOKUP_FIELD,
         queryset=get_belongs_model().objects.all(),
-        help_text=("Account this sample belongs to."))
+        help_text=_("Account this sample belongs to."))
     questions = QuestionSerializer(many=True)
 
     class Meta(object):
         model = Campaign
         fields = ('slug', 'account', 'title', 'description', 'active',
             'quizz_mode', 'questions')
         read_only_fields = ('slug',)
 
 
 class SampleCreateSerializer(serializers.ModelSerializer):
 
     campaign = serializers.SlugRelatedField(slug_field='slug',
         queryset=Campaign.objects.all(), required=False,
-        help_text=("Campaign this sample is part of."))
+        help_text=_("Campaign this sample is part of."))
 
     class Meta(object):
         model = Sample
         fields = ('campaign',)
 
 
 class SampleSerializer(SampleCreateSerializer):
 
     campaign = CampaignSerializer(
         read_only=True, allow_null=True,
-        help_text=("Campaign this sample is part of."))
+        help_text=_("Campaign this sample is part of"))
     account = serializers.SlugRelatedField(slug_field='slug',
         read_only=True, required=False,
-        help_text=("Account this sample belongs to."))
+        help_text=_("Account this sample belongs to"))
     location = serializers.URLField(read_only=True, allow_null=True,
-        help_text=("URL at which the response is visible."))
+        help_text=_("URL at which the response is visible"))
+    grantees = serializers.ListField(required=False,
+        help_text=_("Profiles with which sample was shared"))
 
     class Meta(object):
         model = Sample
         fields = ('campaign', 'slug', 'account', 'created_at',
-            'updated_at', 'is_frozen', 'location')
+            'updated_at', 'is_frozen', 'location', 'grantees')
         read_only_fields = ('campaign', 'slug', 'account', 'created_at',
-            'updated_at', 'is_frozen', 'location')
+            'updated_at', 'is_frozen', 'location', 'grantees')
 
     @staticmethod
     def get_location(obj):
         return getattr(obj, 'location', None)
 
 
 class DatapointSerializer(AnswerSerializer):
@@ -582,36 +584,39 @@
         help_text=_("Extra meta data (can be stringify JSON)"))
 
     class Meta:
         model = PortfolioDoubleOptIn
         fields = ('extra',)
 
 
-class PortfolioOptInSerializer(serializers.ModelSerializer):
+class PortfolioReceivedSerializer(serializers.ModelSerializer):
+
+    # `PortfolioReceivedSerializer` is used in `PortfoliosAPIView` which
+    # is used by the receiving profile.
 
     grantee = serializers.SlugRelatedField(
         queryset=get_account_model().objects.all(),
         slug_field=settings.ACCOUNT_LOOKUP_FIELD)
     account = serializers.SlugRelatedField(
         queryset=get_account_model().objects.all(),
         slug_field=settings.ACCOUNT_LOOKUP_FIELD)
-    campaign = serializers.SlugRelatedField(
-        queryset=Campaign.objects.all(), slug_field='slug')
+    campaign = CampaignSerializer(allow_null=True,
+        help_text=_("Campaign granted/requested"))
     state = EnumField(choices=PortfolioDoubleOptIn.STATES)
+    expected_behavior = EnumField(
+        choices=PortfolioDoubleOptIn.EXPECTED_BEHAVIOR, required=False)
     api_accept = serializers.SerializerMethodField()
     api_remove = serializers.SerializerMethodField()
-    extra = ExtraField(required=False,
-        help_text=_("Extra meta data (can be stringify JSON)"))
 
     class Meta:
         model = PortfolioDoubleOptIn
         fields = ('grantee', 'account', 'campaign', 'created_at', 'ends_at',
-            'state', 'api_accept', 'api_remove', 'extra')
+            'state', 'expected_behavior', 'api_accept', 'api_remove')
         read_only_fields = ('created_at', 'ends_at',
-            'state', 'api_accept', 'api_remove')
+            'state', 'expected_behavior', 'api_accept', 'api_remove')
 
     def get_api_accept(self, obj):
         api_endpoint = None
         view = self.context.get('view')
         if (obj.state == PortfolioDoubleOptIn.OPTIN_GRANT_INITIATED and
             view.account == obj.grantee):
             api_endpoint = reverse('api_portfolios_grant_accept',
@@ -638,14 +643,26 @@
                 args=(obj.grantee, obj.verification_key,))
         request = self.context.get('request')
         if request and api_endpoint:
             return request.build_absolute_uri(api_endpoint)
         return api_endpoint
 
 
+class PortfolioOptInSerializer(PortfolioReceivedSerializer):
+
+    extra = ExtraField(required=False,
+        help_text=_("Extra meta data (can be stringify JSON)"))
+
+    class Meta(PortfolioReceivedSerializer.Meta):
+        fields = PortfolioReceivedSerializer.Meta.fields + (
+            'extra',)
+        read_only_fields = PortfolioReceivedSerializer.Meta.read_only_fields + (
+            'extra',)
+
+
 class AccountsFilterAddSerializer(serializers.ModelSerializer):
 
     slug = serializers.CharField(required=False)
     full_name = serializers.CharField()
     extra = ExtraField(required=False,
         help_text=_("Extra meta data (can be stringify JSON)"))
```

### Comparing `djaodjin-survey-0.9.6/survey/api/serializers_overrides.py` & `djaodjin-survey-0.9.7/survey/api/serializers_overrides.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/api/units.py` & `djaodjin-survey-0.9.7/survey/api/units.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/compat.py` & `djaodjin-survey-0.9.7/survey/compat.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/docs.py` & `djaodjin-survey-0.9.7/survey/docs.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/filters.py` & `djaodjin-survey-0.9.7/survey/filters.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/forms.py` & `djaodjin-survey-0.9.7/survey/forms.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/helpers.py` & `djaodjin-survey-0.9.7/survey/helpers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/mixins.py` & `djaodjin-survey-0.9.7/survey/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,16 @@
             # the user has rights to it.
             try:
                 if settings.BYPASS_SAMPLE_AVAILABLE:
                     queryset = Sample.objects.filter(slug=sample_slug)
                 else:
                     queryset = Sample.objects.filter(
                         Q(account=self.account) |
-                        (Q(account__portfolios__grantee=self.account) &
+                        (Q(is_frozen=True) &
+                         Q(account__portfolios__grantee=self.account) &
                          Q(account__portfolios__ends_at__gte=F('created_at'))),
                         slug=sample_slug)
                 sample = queryset.select_related('campaign').distinct().get()
             except Sample.DoesNotExist:
                 raise Http404("Cannot find Sample(slug='%s')" % sample_slug)
         else:
             # Well no id, let's see if we can find a sample from
```

### Comparing `djaodjin-survey-0.9.6/survey/models.py` & `djaodjin-survey-0.9.7/survey/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -914,14 +914,24 @@
         (OPTIN_GRANT_EXPIRED, 'grant-expired'),
         (OPTIN_REQUEST_INITIATED, 'request-initiated'),
         (OPTIN_REQUEST_ACCEPTED, 'request-accepted'),
         (OPTIN_REQUEST_DENIED, 'request-denied'),
         (OPTIN_REQUEST_EXPIRED, 'request-expired'),
     ]
 
+    EXPECTED_SHARE = 0
+    EXPECTED_CREATE = 1
+    EXPECTED_UPDATE = 2
+
+    EXPECTED_BEHAVIOR = [
+        (EXPECTED_SHARE, 'share'),
+        (EXPECTED_CREATE, 'create'),
+        (EXPECTED_UPDATE, 'update'),
+    ]
+
     objects = PortfolioDoubleOptInManager()
 
     created_at = models.DateTimeField(auto_now_add=True,
         help_text=_("Date/time at which the grant/request was created"))
     # Either we have an AccountModel or we have an e-mail to invite
     # someone to register an AccountModel.
     grantee = models.ForeignKey(settings.ACCOUNT_MODEL, null=True,
```

### Comparing `djaodjin-survey-0.9.6/survey/pagination.py` & `djaodjin-survey-0.9.7/survey/pagination.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/queries.py` & `djaodjin-survey-0.9.7/survey/queries.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/settings.py` & `djaodjin-survey-0.9.7/survey/settings.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/signals.py` & `djaodjin-survey-0.9.7/survey/signals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/static/js/djaodjin-categorize.js` & `djaodjin-survey-0.9.7/survey/static/js/djaodjin-categorize.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/static/js/djaodjin-matrix.js` & `djaodjin-survey-0.9.7/survey/static/js/djaodjin-matrix.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/static/js/djaodjin-resources-vue.js` & `djaodjin-survey-0.9.7/survey/static/js/djaodjin-resources-vue.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/static/js/djaodjin-set.js` & `djaodjin-survey-0.9.7/survey/static/js/djaodjin-set.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/static/js/djaodjin-survey-vue.js` & `djaodjin-survey-0.9.7/survey/static/js/djaodjin-survey-vue.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/static/js/djaodjin-survey.js` & `djaodjin-survey-0.9.7/survey/static/js/djaodjin-survey.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/static/js/matrix-chart.js` & `djaodjin-survey-0.9.7/survey/static/js/matrix-chart.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/templates/survey/answer_form.html` & `djaodjin-survey-0.9.7/survey/templates/survey/answer_form.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/templates/survey/campaigns/index.html` & `djaodjin-survey-0.9.7/survey/templates/survey/campaigns/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/templates/survey/categorize.html` & `djaodjin-survey-0.9.7/survey/templates/survey/categorize.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/templates/survey/matrix/index.html` & `djaodjin-survey-0.9.7/survey/templates/survey/matrix/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/templates/survey/matrix/matrix.html` & `djaodjin-survey-0.9.7/survey/templates/survey/matrix/matrix.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/templates/survey/portfolios.html` & `djaodjin-survey-0.9.7/survey/templates/survey/portfolios.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/templates/survey/question_list.html` & `djaodjin-survey-0.9.7/survey/templates/survey/question_list.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/templates/survey/result.html` & `djaodjin-survey-0.9.7/survey/templates/survey/result.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/templates/survey/result_quizz.html` & `djaodjin-survey-0.9.7/survey/templates/survey/result_quizz.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/templates/survey/sample_create.html` & `djaodjin-survey-0.9.7/survey/templates/survey/sample_create.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/templatetags/survey_tags.py` & `djaodjin-survey-0.9.7/survey/templatetags/survey_tags.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/__init__.py` & `djaodjin-survey-0.9.7/survey/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/api/__init__.py` & `djaodjin-survey-0.9.7/survey/urls/api/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/api/campaigns.py` & `djaodjin-survey-0.9.7/survey/urls/api/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/api/filters.py` & `djaodjin-survey-0.9.7/survey/urls/api/filters.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/api/matrix.py` & `djaodjin-survey-0.9.7/survey/urls/api/matrix.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/api/metrics.py` & `djaodjin-survey-0.9.7/survey/urls/api/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/api/noauth.py` & `djaodjin-survey-0.9.7/survey/urls/api/noauth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/api/portfolios.py` & `djaodjin-survey-0.9.7/survey/urls/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/api/sample/__init__.py` & `djaodjin-survey-0.9.7/survey/urls/api/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/api/sample/reset.py` & `djaodjin-survey-0.9.7/survey/urls/api/sample/reset.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/api/sample/update.py` & `djaodjin-survey-0.9.7/survey/urls/api/sample/update.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/views/__init__.py` & `djaodjin-survey-0.9.7/survey/urls/views/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/views/campaigns.py` & `djaodjin-survey-0.9.7/survey/urls/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/views/matrices.py` & `djaodjin-survey-0.9.7/survey/urls/views/matrices.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/views/portfolios.py` & `djaodjin-survey-0.9.7/survey/urls/views/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/urls/views/samples.py` & `djaodjin-survey-0.9.7/survey/urls/views/samples.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/utils.py` & `djaodjin-survey-0.9.7/survey/utils.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/views/campaigns.py` & `djaodjin-survey-0.9.7/survey/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/views/createquestion.py` & `djaodjin-survey-0.9.7/survey/views/createquestion.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/views/edit.py` & `djaodjin-survey-0.9.7/survey/views/edit.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/views/matrix.py` & `djaodjin-survey-0.9.7/survey/views/matrix.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/views/portfolios.py` & `djaodjin-survey-0.9.7/survey/views/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.6/survey/views/sample.py` & `djaodjin-survey-0.9.7/survey/views/sample.py`

 * *Files identical despite different names*

