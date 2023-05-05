# Comparing `tmp/urgxy_env-0.1.9.tar.gz` & `tmp/urgxy_env-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urgxy_env-0.1.9.tar", last modified: Fri May  5 06:45:56 2023, max compression
+gzip compressed data, was "urgxy_env-0.2.0.tar", last modified: Fri May  5 07:03:01 2023, max compression
```

## Comparing `urgxy_env-0.1.9.tar` & `urgxy_env-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 06:45:56.990992 urgxy_env-0.1.9/
--rw-rw-rw-   0        0        0      175 2023-05-05 06:45:56.990992 urgxy_env-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-05 06:45:56.991992 urgxy_env-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      381 2023-05-05 06:45:46.000000 urgxy_env-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:45:56.962992 urgxy_env-0.1.9/urgxy_env/
--rw-rw-rw-   0        0        0      131 2023-05-05 06:45:46.000000 urgxy_env-0.1.9/urgxy_env/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:45:56.989994 urgxy_env-0.1.9/urgxy_env/envs/
--rw-rw-rw-   0        0        0       49 2023-04-27 13:33:10.000000 urgxy_env-0.1.9/urgxy_env/envs/__init__.py
--rw-rw-rw-   0        0        0    11517 2023-05-05 06:45:46.000000 urgxy_env-0.1.9/urgxy_env/envs/env_urgxy.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:45:56.986991 urgxy_env-0.1.9/urgxy_env.egg-info/
--rw-rw-rw-   0        0        0      175 2023-05-05 06:45:56.000000 urgxy_env-0.1.9/urgxy_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-05-05 06:45:56.000000 urgxy_env-0.1.9/urgxy_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 06:45:56.000000 urgxy_env-0.1.9/urgxy_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-05 06:45:56.000000 urgxy_env-0.1.9/urgxy_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-05 06:45:56.000000 urgxy_env-0.1.9/urgxy_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 07:03:01.158038 urgxy_env-0.2.0/
+-rw-rw-rw-   0        0        0      175 2023-05-05 07:03:01.158038 urgxy_env-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-05 07:03:01.158038 urgxy_env-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      381 2023-05-05 07:02:57.000000 urgxy_env-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:03:01.135038 urgxy_env-0.2.0/urgxy_env/
+-rw-rw-rw-   0        0        0      131 2023-05-05 07:02:57.000000 urgxy_env-0.2.0/urgxy_env/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:03:01.156041 urgxy_env-0.2.0/urgxy_env/envs/
+-rw-rw-rw-   0        0        0       49 2023-04-27 13:33:10.000000 urgxy_env-0.2.0/urgxy_env/envs/__init__.py
+-rw-rw-rw-   0        0        0    11516 2023-05-05 07:02:44.000000 urgxy_env-0.2.0/urgxy_env/envs/env_urgxy.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:03:01.153036 urgxy_env-0.2.0/urgxy_env.egg-info/
+-rw-rw-rw-   0        0        0      175 2023-05-05 07:03:00.000000 urgxy_env-0.2.0/urgxy_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-05 07:03:01.000000 urgxy_env-0.2.0/urgxy_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 07:03:00.000000 urgxy_env-0.2.0/urgxy_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-05 07:03:00.000000 urgxy_env-0.2.0/urgxy_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 07:03:00.000000 urgxy_env-0.2.0/urgxy_env.egg-info/top_level.txt
```

### Comparing `urgxy_env-0.1.9/urgxy_env/envs/env_urgxy.py` & `urgxy_env-0.2.0/urgxy_env/envs/env_urgxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         #fingers = action[3]
 
         currentPose = p.getLinkState(self.pandaUid,20)
         currentPosition = currentPose[0]
         # orientation = p.getLinkState(self.pandaUid,20)[1]
         #currentPose = p.getLinkState(self.pandaUid, 11)
 
-        orientation = [-0.33465454802778005, 0.8028657828683929, -0.4474897090250233, -0.20776387679321207]
+        orientation = [0.8043483397135041, -0.33107533918552434, 0.16951176159778775, 0.46333425392834304]
         newPosition = [currentPosition[0] + dx,
                        currentPosition[1] + dy,
                        currentPosition[2] + dz]
         #jointPoses = p.calculateInverseKinematics(self.pandaUid,20,newPosition, orientation)[0:7]
         jointPoses = p.calculateInverseKinematics(self.pandaUid, 20, newPosition, orientation)[0:12]  #得到角度
         #p.setJointMotorControlArray(self.pandaUid, list(range(12)), p.POSITION_CONTROL, list(jointPoses))
         # p.setJointMotorControl2(self.pandaUid, 15 , p.POSITION_CONTROL, jointPoses[6])
```

