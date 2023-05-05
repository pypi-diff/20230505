# Comparing `tmp/urgxy_env-0.1.8.tar.gz` & `tmp/urgxy_env-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urgxy_env-0.1.8.tar", last modified: Fri May  5 06:42:21 2023, max compression
+gzip compressed data, was "urgxy_env-0.1.9.tar", last modified: Fri May  5 06:45:56 2023, max compression
```

## Comparing `urgxy_env-0.1.8.tar` & `urgxy_env-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 06:42:21.318322 urgxy_env-0.1.8/
--rw-rw-rw-   0        0        0      175 2023-05-05 06:42:21.316310 urgxy_env-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-05 06:42:21.318322 urgxy_env-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      381 2023-05-05 06:39:41.000000 urgxy_env-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:42:21.285310 urgxy_env-0.1.8/urgxy_env/
--rw-rw-rw-   0        0        0      131 2023-05-05 06:39:41.000000 urgxy_env-0.1.8/urgxy_env/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:42:21.315310 urgxy_env-0.1.8/urgxy_env/envs/
--rw-rw-rw-   0        0        0       49 2023-04-27 13:33:10.000000 urgxy_env-0.1.8/urgxy_env/envs/__init__.py
--rw-rw-rw-   0        0        0    11517 2023-05-05 06:39:41.000000 urgxy_env-0.1.8/urgxy_env/envs/env_urgxy.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:42:21.309310 urgxy_env-0.1.8/urgxy_env.egg-info/
--rw-rw-rw-   0        0        0      175 2023-05-05 06:42:20.000000 urgxy_env-0.1.8/urgxy_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-05-05 06:42:21.000000 urgxy_env-0.1.8/urgxy_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 06:42:20.000000 urgxy_env-0.1.8/urgxy_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-05 06:42:20.000000 urgxy_env-0.1.8/urgxy_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-05 06:42:21.000000 urgxy_env-0.1.8/urgxy_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 06:45:56.990992 urgxy_env-0.1.9/
+-rw-rw-rw-   0        0        0      175 2023-05-05 06:45:56.990992 urgxy_env-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-05 06:45:56.991992 urgxy_env-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      381 2023-05-05 06:45:46.000000 urgxy_env-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:45:56.962992 urgxy_env-0.1.9/urgxy_env/
+-rw-rw-rw-   0        0        0      131 2023-05-05 06:45:46.000000 urgxy_env-0.1.9/urgxy_env/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:45:56.989994 urgxy_env-0.1.9/urgxy_env/envs/
+-rw-rw-rw-   0        0        0       49 2023-04-27 13:33:10.000000 urgxy_env-0.1.9/urgxy_env/envs/__init__.py
+-rw-rw-rw-   0        0        0    11517 2023-05-05 06:45:46.000000 urgxy_env-0.1.9/urgxy_env/envs/env_urgxy.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:45:56.986991 urgxy_env-0.1.9/urgxy_env.egg-info/
+-rw-rw-rw-   0        0        0      175 2023-05-05 06:45:56.000000 urgxy_env-0.1.9/urgxy_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-05 06:45:56.000000 urgxy_env-0.1.9/urgxy_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 06:45:56.000000 urgxy_env-0.1.9/urgxy_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-05 06:45:56.000000 urgxy_env-0.1.9/urgxy_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 06:45:56.000000 urgxy_env-0.1.9/urgxy_env.egg-info/top_level.txt
```

### Comparing `urgxy_env-0.1.8/urgxy_env/envs/env_urgxy.py` & `urgxy_env-0.1.9/urgxy_env/envs/env_urgxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
                 file = open('test.csv', 'a+', newline='')
                 writer = csv.writer(file)
                 writer.writerow(np_score)
                 file.close()
                 reward = 0
                 done = True
 
-                self.iscollision = 1
+                self.iscollision = 0
                 list_iscollision = [self.iscollision]
                 np_iscollision = np.array(list_iscollision, 'int')
                 file_iscollision = open('test_iscollision.csv', 'a+', newline='')
                 writer_iscollision = csv.writer(file_iscollision)
                 writer_iscollision.writerow(np_iscollision)
 
                 list_step_counter = [self.step_counter]
```

