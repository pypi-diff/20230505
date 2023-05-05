# Comparing `tmp/urgxy_env-0.1.7.tar.gz` & `tmp/urgxy_env-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urgxy_env-0.1.7.tar", last modified: Thu May  4 09:04:56 2023, max compression
+gzip compressed data, was "urgxy_env-0.1.8.tar", last modified: Fri May  5 06:42:21 2023, max compression
```

## Comparing `urgxy_env-0.1.7.tar` & `urgxy_env-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 09:04:56.712963 urgxy_env-0.1.7/
--rw-rw-rw-   0        0        0      175 2023-05-04 09:04:56.711963 urgxy_env-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-04 09:04:56.712963 urgxy_env-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      381 2023-05-04 09:04:51.000000 urgxy_env-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:04:56.675908 urgxy_env-0.1.7/urgxy_env/
--rw-rw-rw-   0        0        0      131 2023-05-04 09:04:51.000000 urgxy_env-0.1.7/urgxy_env/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:04:56.710965 urgxy_env-0.1.7/urgxy_env/envs/
--rw-rw-rw-   0        0        0       49 2023-04-27 13:33:10.000000 urgxy_env-0.1.7/urgxy_env/envs/__init__.py
--rw-rw-rw-   0        0        0     9099 2023-05-04 09:03:09.000000 urgxy_env-0.1.7/urgxy_env/envs/env_urgxy.py
-drwxrwxrwx   0        0        0        0 2023-05-04 09:04:56.703963 urgxy_env-0.1.7/urgxy_env.egg-info/
--rw-rw-rw-   0        0        0      175 2023-05-04 09:04:56.000000 urgxy_env-0.1.7/urgxy_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-05-04 09:04:56.000000 urgxy_env-0.1.7/urgxy_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 09:04:56.000000 urgxy_env-0.1.7/urgxy_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-04 09:04:56.000000 urgxy_env-0.1.7/urgxy_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-04 09:04:56.000000 urgxy_env-0.1.7/urgxy_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 06:42:21.318322 urgxy_env-0.1.8/
+-rw-rw-rw-   0        0        0      175 2023-05-05 06:42:21.316310 urgxy_env-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-05 06:42:21.318322 urgxy_env-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      381 2023-05-05 06:39:41.000000 urgxy_env-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:42:21.285310 urgxy_env-0.1.8/urgxy_env/
+-rw-rw-rw-   0        0        0      131 2023-05-05 06:39:41.000000 urgxy_env-0.1.8/urgxy_env/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:42:21.315310 urgxy_env-0.1.8/urgxy_env/envs/
+-rw-rw-rw-   0        0        0       49 2023-04-27 13:33:10.000000 urgxy_env-0.1.8/urgxy_env/envs/__init__.py
+-rw-rw-rw-   0        0        0    11517 2023-05-05 06:39:41.000000 urgxy_env-0.1.8/urgxy_env/envs/env_urgxy.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:42:21.309310 urgxy_env-0.1.8/urgxy_env.egg-info/
+-rw-rw-rw-   0        0        0      175 2023-05-05 06:42:20.000000 urgxy_env-0.1.8/urgxy_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-05 06:42:21.000000 urgxy_env-0.1.8/urgxy_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 06:42:20.000000 urgxy_env-0.1.8/urgxy_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-05 06:42:20.000000 urgxy_env-0.1.8/urgxy_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 06:42:21.000000 urgxy_env-0.1.8/urgxy_env.egg-info/top_level.txt
```

### Comparing `urgxy_env-0.1.7/urgxy_env/envs/env_urgxy.py` & `urgxy_env-0.1.8/urgxy_env/envs/env_urgxy.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,36 +12,38 @@
 
 MAX_EPISODE_LEN = 20*100
 
 class UrgxyEnv(gym.Env):
 
     metadata = {'render.modes': ['human']}
     def __init__(self):
+        self.iscollision = 0
         self.score = 0
         self.step_counter = 0
         p.connect(p.GUI)
         p.resetDebugVisualizerCamera(cameraDistance=1.5, cameraYaw=0, cameraPitch=-40, cameraTargetPosition=[0.55,-0.35,0.2])
         # self.action_space = spaces.Box(np.array([-1]*4), np.array([1]*4))
         #         # self.observation_space = spaces.Box(np.array([-1]*5), np.array([1]*5))
         self.action_space = spaces.Box(np.array([-1] * 3), np.array([1] * 3))
         self.observation_space = spaces.Box(np.array([-1] * 3), np.array([1] * 3))
     def step(self, action):
         p.configureDebugVisualizer(p.COV_ENABLE_SINGLE_STEP_RENDERING)
         #orientation = p.getQuaternionFromEuler([0.,-math.pi,math.pi/2.])
-        dv = 0.05
+        dv = 0.02
         dx = action[0] * dv
         dy = action[1] * dv
         dz = action[2] * dv
         #fingers = action[3]
 
         currentPose = p.getLinkState(self.pandaUid,20)
         currentPosition = currentPose[0]
-        orientation = p.getLinkState(self.pandaUid,20)[1]
+        # orientation = p.getLinkState(self.pandaUid,20)[1]
         #currentPose = p.getLinkState(self.pandaUid, 11)
 
+        orientation = [-0.33465454802778005, 0.8028657828683929, -0.4474897090250233, -0.20776387679321207]
         newPosition = [currentPosition[0] + dx,
                        currentPosition[1] + dy,
                        currentPosition[2] + dz]
         #jointPoses = p.calculateInverseKinematics(self.pandaUid,20,newPosition, orientation)[0:7]
         jointPoses = p.calculateInverseKinematics(self.pandaUid, 20, newPosition, orientation)[0:12]  #得到角度
         #p.setJointMotorControlArray(self.pandaUid, list(range(12)), p.POSITION_CONTROL, list(jointPoses))
         # p.setJointMotorControl2(self.pandaUid, 15 , p.POSITION_CONTROL, jointPoses[6])
@@ -50,71 +52,109 @@
         # p.setJointMotorControl2(self.pandaUid, 18,  p.POSITION_CONTROL, jointPoses[9])
         # p.setJointMotorControl2(self.pandaUid, 19,  p.POSITION_CONTROL, jointPoses[10])
         # p.setJointMotorControl2(self.pandaUid, 20,  p.POSITION_CONTROL, jointPoses[11])
         p.setJointMotorControlArray(self.pandaUid, [15,16,17,18,19,20], p.POSITION_CONTROL, [jointPoses[6],jointPoses[7],jointPoses[8],jointPoses[9],jointPoses[10],jointPoses[11]])
         p.stepSimulation()
         state_robot = p.getLinkState(self.pandaUid, 20)[0]  #得到位置
 
-        done = False
-        goal = np.array( [-0.8746627265025098,-0.46638541744607026,0.23835711380789043] )
-        goal = np.array( [-0.8746627265025098,-0.46638541744607026,0.23835711380789043] )
-        current = np.array( [state_robot[0],state_robot[1],state_robot[2]] )
-        reward = -np.linalg.norm( current-goal )
-        self.score = self.score + reward
-        # reward = 0
-        # if action[0]>0 and state_robot[0]-(-0.8746627265025098) < 0:
-        #     reward += 1
-        #     done = False
-        #
-        # if action[0]<0 and state_robot[0]-(-0.8746627265025098) > 0:
-        #     reward += 1
-        #     done = False
-        #
-        #
-        # if action[1]>0 and state_robot[1]-(-0.46638541744607026) < 0:
-        #     reward += 1
-        #     done = False
-        # # if action[1]>0 and state_robot[1]-(-0.46638541744607026) > 0:
-        # #     reward -= 1
-        # #     done = False
-        # if action[1]<0 and state_robot[1]-(-0.46638541744607026) > 0:
-        #     reward += 1
-        #     done = False
-        # # if action[1]<0 and state_robot[1]-(-0.46638541744607026) < 0:
-        # #     reward -= 1
-        # #     done = False
-        #
-        # if state_robot[1] > -0.2:
-        #     reward -= 10000
-        #     done = True
-        #
-        # if action[2]>0 and state_robot[2]-0.23835711380789043 < 0:
-        #     reward += 1
-        #     done = False
-        # if action[2]>0 and state_robot[2]-0.23835711380789043 > 0:
-        #     reward -= 1
-        #     done = False
-        # if action[2]<0 and state_robot[2]-0.23835711380789043 > 0:
-        #     reward += 1
-        #     done = False
-        # if action[2]<0 and state_robot[2]-0.23835711380789043 < 0:
-        #     reward -= 1
-        #     done = False
+        if bool(p.getContactPoints(self.pandaUid, self.woodplate)) == True:
+            self.iscollision = 1
+            list_iscollision = [self.iscollision]
+            np_iscollision = np.array(list_iscollision, 'int')
+            file_iscollision = open('test_iscollision.csv', 'a+', newline='')
+            writer_iscollision = csv.writer(file_iscollision)
+            writer_iscollision.writerow(np_iscollision)
+
+            list_step_counter = [self.step_counter]
+            np_step_counter = np.array(list_step_counter, 'int')
+            file_step_counter = open('test_step_counter.csv', 'a+', newline='')
+            writer_step_counter = csv.writer(file_step_counter)
+            writer_step_counter.writerow(np_step_counter)
 
-        self.step_counter += 1
-
-        if self.step_counter > MAX_EPISODE_LEN:
+            reward = -10000
+            self.score = self.score + reward
             list_score = [self.score]
-            np_score = np.array(list_score,'float')
+            np_score = np.array(list_score, 'float')
             file = open('test.csv', 'a+', newline='')
             writer = csv.writer(file)
             writer.writerow(np_score)
             file.close()
             reward = 0
             done = True
+        else:
+            done = False
+            # goal = np.array( [-0.8746627265025098,-0.46638541744607026,0.23835711380789043] )
+            goal = np.array( [-0.8746627265025098,-0.46638541744607026,0.23835711380789043] )
+            current = np.array( [state_robot[0],state_robot[1],state_robot[2]] )
+            reward = -5*np.linalg.norm( current-goal )
+            self.score = self.score + reward
+            # reward = 0
+            # if action[0]>0 and state_robot[0]-(-0.8746627265025098) < 0:
+            #     reward += 1
+            #     done = False
+            #
+            # if action[0]<0 and state_robot[0]-(-0.8746627265025098) > 0:
+            #     reward += 1
+            #     done = False
+            #
+            #
+            # if action[1]>0 and state_robot[1]-(-0.46638541744607026) < 0:
+            #     reward += 1
+            #     done = False
+            # # if action[1]>0 and state_robot[1]-(-0.46638541744607026) > 0:
+            # #     reward -= 1
+            # #     done = False
+            # if action[1]<0 and state_robot[1]-(-0.46638541744607026) > 0:
+            #     reward += 1
+            #     done = False
+            # # if action[1]<0 and state_robot[1]-(-0.46638541744607026) < 0:
+            # #     reward -= 1
+            # #     done = False
+            #
+            # if state_robot[1] > -0.2:
+            #     reward -= 10000
+            #     done = True
+            #
+            # if action[2]>0 and state_robot[2]-0.23835711380789043 < 0:
+            #     reward += 1
+            #     done = False
+            # if action[2]>0 and state_robot[2]-0.23835711380789043 > 0:
+            #     reward -= 1
+            #     done = False
+            # if action[2]<0 and state_robot[2]-0.23835711380789043 > 0:
+            #     reward += 1
+            #     done = False
+            # if action[2]<0 and state_robot[2]-0.23835711380789043 < 0:
+            #     reward -= 1
+            #     done = False
+
+            self.step_counter += 1
+
+            if self.step_counter > MAX_EPISODE_LEN:
+                list_score = [self.score]
+                np_score = np.array(list_score,'float')
+                file = open('test.csv', 'a+', newline='')
+                writer = csv.writer(file)
+                writer.writerow(np_score)
+                file.close()
+                reward = 0
+                done = True
+
+                self.iscollision = 1
+                list_iscollision = [self.iscollision]
+                np_iscollision = np.array(list_iscollision, 'int')
+                file_iscollision = open('test_iscollision.csv', 'a+', newline='')
+                writer_iscollision = csv.writer(file_iscollision)
+                writer_iscollision.writerow(np_iscollision)
+
+                list_step_counter = [self.step_counter]
+                np_step_counter = np.array(list_step_counter, 'int')
+                file_step_counter = open('test_step_counter.csv', 'a+', newline='')
+                writer_step_counter = csv.writer(file_step_counter)
+                writer_step_counter.writerow(np_step_counter)
 
         #info = {'object_position': state_object}
         info = {'robot_position':state_robot}
         self.observation = state_robot
         return np.array(self.observation).astype(np.float32), reward, done, info
     def reset(self):
         self.score=0
@@ -124,14 +164,17 @@
         urdfRootPath=pybullet_data.getDataPath()
         #p.setGravity(0,0,-10)
 
         planeUid = p.loadURDF(os.path.join(urdfRootPath,"plane.urdf"), basePosition=[0,0,-0.65])
 
         #rest_poses = [0,-0.215,0,-2.57,0,2.356,2.356,0.08,0.08]
         self.pandaUid = p.loadURDF("C:/Users/guixiangyu/Desktop/artificial_potential/urdf/mobot_rl.urdf",useFixedBase=True,flags=p.URDF_USE_SELF_COLLISION)
+        self.woodplate = p.loadURDF("C:/Users/guixiangyu/Desktop/artificial_potential/urdf/woodplate_rl.urdf",
+                               basePosition=[0, 0, 0], useFixedBase=True)
+
         # for i in range(7):
         #     p.resetJointState(self.pandaUid,i, rest_poses[i])
         # p.resetJointState(self.pandaUid, 9, 0.08)
         # p.resetJointState(self.pandaUid,10, 0.08)
         rest_joints = [15.36 * 0.01745, -86.34 * 0.01745, -125.38 * 0.01745, 248.13 * 0.01745, -84.74 * 0.01745,-74.12 * 0.01745,
                        62.81 * 0.01745, -139.95 * 0.01745, 127.70 * 0.01745, -33.87 * 0.01745, 100.12 * 0.01745,30.01 * 0.01745]
```

