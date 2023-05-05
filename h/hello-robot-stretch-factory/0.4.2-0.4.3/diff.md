# Comparing `tmp/hello_robot_stretch_factory-0.4.2.tar.gz` & `tmp/hello_robot_stretch_factory-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_factory-0.4.2.tar", last modified: Tue Apr 18 19:47:03 2023, max compression
+gzip compressed data, was "hello_robot_stretch_factory-0.4.3.tar", last modified: Fri May  5 11:27:53 2023, max compression
```

## Comparing `hello_robot_stretch_factory-0.4.2.tar` & `hello_robot_stretch_factory-0.4.3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-18 19:47:03.653871 hello_robot_stretch_factory-0.4.2/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      935 2023-04-18 19:47:03.653871 hello_robot_stretch_factory-0.4.2/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      355 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/README.md
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-18 19:47:03.653871 hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      935 2023-04-18 19:47:03.000000 hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1785 2023-04-18 19:47:03.000000 hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2023-04-18 19:47:03.000000 hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       74 2023-04-18 19:47:03.000000 hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/requires.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       16 2023-04-18 19:47:03.000000 hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/top_level.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2023-04-18 19:47:03.657871 hello_robot_stretch_factory-0.4.2/setup.cfg
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      995 2023-04-18 19:28:09.000000 hello_robot_stretch_factory-0.4.2/setup.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-18 19:47:03.653871 hello_robot_stretch_factory-0.4.2/stretch_factory/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6326 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/device_mgmt.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4425 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_available.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5248 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_installed.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3861 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_recommended.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    37747 2023-04-18 19:39:17.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_updater.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5254 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2726 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_version.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    20922 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/hello_device_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12828 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/param_mgmt.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-18 19:47:03.653871 hello_robot_stretch_factory-0.4.2/test/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      685 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/test/test_firmware_updater.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      668 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/test/test_usb_reset.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-18 19:47:03.653871 hello_robot_stretch_factory-0.4.2/tools/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2456 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/RE1_migrate_contacts.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6621 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/RE1_migrate_params.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    22012 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_D435i_check.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5418 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_base_calibrate_imu_collect.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    32027 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_base_calibrate_imu_process.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5950 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_base_calibrate_wheel_separation.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4771 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_calibrate_gravity_comp.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7456 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_calibrate_guarded_contact.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3578 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_calibrate_range.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1728 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_cliff_sensor_calibrate.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18552 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_discover_hello_devices.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1442 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_id_change.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1354 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_id_scan.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5045 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1374 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_reboot.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1188 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_set_baud.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4397 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_firmware_flash.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5804 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_firmware_updater.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1583 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_gamepad_configure.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2338 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_gripper_calibrate.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1947 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_hello_dynamixel_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      870 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_stepper_calibration_YAML_to_flash.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      685 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_stepper_calibration_flash_to_YAML.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1168 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_stepper_calibration_run.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18644 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_stepper_ctrl_tuning.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1163 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_stepper_gains.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4064 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_stepper_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      852 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_stepper_mechaduino_menu.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    10577 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_trace_firmware.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7819 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_trace_robot.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2347 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_usb_reset.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1379 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_wacc_calibrate.py
+drwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)        0 2023-05-05 11:27:53.665849 hello_robot_stretch_factory-0.4.3/
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)      929 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/LICENSE.md
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)      853 2023-05-05 11:27:53.665849 hello_robot_stretch_factory-0.4.3/PKG-INFO
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)      355 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/README.md
+drwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)        0 2023-05-05 11:27:53.661849 hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)      853 2023-05-05 11:27:53.000000 hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/PKG-INFO
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)     1796 2023-05-05 11:27:53.000000 hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)        1 2023-05-05 11:27:53.000000 hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)       74 2023-05-05 11:27:53.000000 hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/requires.txt
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)       16 2023-05-05 11:27:53.000000 hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/top_level.txt
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)       38 2023-05-05 11:27:53.665849 hello_robot_stretch_factory-0.4.3/setup.cfg
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)      995 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/setup.py
+drwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)        0 2023-05-05 11:27:53.665849 hello_robot_stretch_factory-0.4.3/stretch_factory/
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)        0 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/__init__.py
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)     6326 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/device_mgmt.py
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)     4641 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_available.py
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)     5248 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_installed.py
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)     3861 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_recommended.py
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)    37747 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_updater.py
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)     5254 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_utils.py
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)     2726 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_version.py
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)    22204 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/hello_device_utils.py
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)    12828 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/stretch_factory/param_mgmt.py
+drwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)        0 2023-05-05 11:27:53.665849 hello_robot_stretch_factory-0.4.3/test/
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)      685 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/test/test_firmware_updater.py
+-rw-rw-r--   0 hello-binit  (1000) hello-binit  (1000)      668 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/test/test_usb_reset.py
+drwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)        0 2023-05-05 11:27:53.661849 hello_robot_stretch_factory-0.4.3/tools/
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     2456 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/RE1_migrate_contacts.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     6621 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/RE1_migrate_params.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)    22012 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_D435i_check.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     5418 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_base_calibrate_imu_collect.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)    32027 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_base_calibrate_imu_process.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     5950 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_base_calibrate_wheel_separation.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     4771 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_calibrate_gravity_comp.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     7456 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_calibrate_guarded_contact.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     3578 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_calibrate_range.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1728 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_cliff_sensor_calibrate.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)    18552 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_discover_hello_devices.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1442 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_id_change.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1354 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_id_scan.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     5045 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_jog.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1374 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_reboot.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1188 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_set_baud.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     2846 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_firmware_flash.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     5804 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_firmware_updater.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1583 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_gamepad_configure.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     2338 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_gripper_calibrate.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1947 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_hello_dynamixel_jog.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)      870 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_stepper_calibration_YAML_to_flash.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)      735 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_stepper_calibration_flash_to_YAML.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1168 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_stepper_calibration_run.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)    18644 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_stepper_ctrl_tuning.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1163 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_stepper_gains.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     4449 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_stepper_jog.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)      852 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_stepper_mechaduino_menu.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)    10577 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_trace_firmware.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     7819 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_trace_robot.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     2347 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_usb_reset.py
+-rwxrwxr-x   0 hello-binit  (1000) hello-binit  (1000)     1379 2023-05-05 11:27:25.000000 hello_robot_stretch_factory-0.4.3/tools/REx_wacc_calibrate.py
```

### Comparing `hello_robot_stretch_factory-0.4.2/PKG-INFO` & `hello_robot_stretch_factory-0.4.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: hello_robot_stretch_factory
-Version: 0.4.2
+Version: 0.4.3
 Summary: Stretch Factory Tools
 Home-page: https://github.com/hello-robot/stretch_factory
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
 License: UNKNOWN
-Description: # Overview
-        
-        The Stretch Factory package provides Python tools for testing and calibration of the Hello Robot Stretch RE1 and RE2. 
-        
-        **These tools are provided for reference only and are intended to be used by qualified Hello Robot production engineers.** 
-        
-        This package can be installed by:
-        
-        ```
-        python -m pip install  -U hello-robot-stretch-factory
-        ```
-        
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Overview
+
+The Stretch Factory package provides Python tools for testing and calibration of the Hello Robot Stretch RE1 and RE2. 
+
+**These tools are provided for reference only and are intended to be used by qualified Hello Robot production engineers.** 
+
+This package can be installed by:
+
+```
+python -m pip install  -U hello-robot-stretch-factory
+```
+
+
+
```

### Comparing `hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/PKG-INFO` & `hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: hello-robot-stretch-factory
-Version: 0.4.2
+Version: 0.4.3
 Summary: Stretch Factory Tools
 Home-page: https://github.com/hello-robot/stretch_factory
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
 License: UNKNOWN
-Description: # Overview
-        
-        The Stretch Factory package provides Python tools for testing and calibration of the Hello Robot Stretch RE1 and RE2. 
-        
-        **These tools are provided for reference only and are intended to be used by qualified Hello Robot production engineers.** 
-        
-        This package can be installed by:
-        
-        ```
-        python -m pip install  -U hello-robot-stretch-factory
-        ```
-        
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Overview
+
+The Stretch Factory package provides Python tools for testing and calibration of the Hello Robot Stretch RE1 and RE2. 
+
+**These tools are provided for reference only and are intended to be used by qualified Hello Robot production engineers.** 
+
+This package can be installed by:
+
+```
+python -m pip install  -U hello-robot-stretch-factory
+```
+
+
+
```

### Comparing `hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/SOURCES.txt` & `hello_robot_stretch_factory-0.4.3/hello_robot_stretch_factory.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 README.md
 setup.py
 ./tools/RE1_migrate_contacts.py
 ./tools/RE1_migrate_params.py
 ./tools/REx_D435i_check.py
 ./tools/REx_base_calibrate_imu_collect.py
 ./tools/REx_base_calibrate_imu_process.py
```

### Comparing `hello_robot_stretch_factory-0.4.2/setup.py` & `hello_robot_stretch_factory-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 script_path='./tools'
 ex_scripts = glob.glob(script_path+'/*.py') + glob.glob(script_path+'/*.sh')
 stretch_scripts=[f for f in ex_scripts if isfile(f)]
 
 setuptools.setup(
     name="hello_robot_stretch_factory",
-    version="0.4.2",
+    version="0.4.3",
     author="Hello Robot Inc.",
     author_email="support@hello-robot.com",
     description="Stretch Factory Tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hello-robot/stretch_factory",
     scripts = stretch_scripts,
```

### Comparing `hello_robot_stretch_factory-0.4.2/stretch_factory/device_mgmt.py` & `hello_robot_stretch_factory-0.4.3/stretch_factory/device_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_available.py` & `hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_available.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         for d in self.use_device:
             if self.use_device[d]:
                 self.versions[d] = []  # List of available versions for that device
         self.__clone_firmware_repo()
         self.__get_available_firmware_versions()
 
     def __clone_firmware_repo(self):
-        print('Collecting information...')
+        print('Collecting information...', end='')
         self.repo_path = '/tmp/stretch_firmware_update'
         if not os.path.isdir(self.repo_path):
             # print('Cloning latest version of Stretch Firmware to %s'% self.repo_path)
             try:
                 git.Repo.clone_from('https://github.com/hello-robot/stretch_firmware', self.repo_path)
             except git.GitCommandError as e:
                 if "could not resolve host" in e.stderr.lower():
@@ -81,15 +81,21 @@
     def get_most_recent_version(self, device_name, supported_protocols):
         """
         For the device and supported protocol versions (eg, '['p0','p1']'), return the most recent version (type FirmwareVersion)
         """
         if len(self.versions[device_name]) == 0:
             return None
         recent = None
-        s = [int(x[1:]) for x in supported_protocols]
+        if supported_protocols is not None:
+            s = [int(x[1:]) for x in supported_protocols]
+        else:
+            class Everything(object):
+                def __contains__(self, other):
+                    return True
+            s = Everything()
         supported_versions = []
         for v in self.versions[device_name]:
             if v.protocol in s:
                 supported_versions.append(v)
         for sv in supported_versions:
             if recent is None or sv > recent:
                 recent = sv
```

### Comparing `hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_installed.py` & `hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_installed.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_recommended.py` & `hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_recommended.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_updater.py` & `hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_utils.py` & `hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_version.py` & `hello_robot_stretch_factory-0.4.3/stretch_factory/firmware_version.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/stretch_factory/hello_device_utils.py` & `hello_robot_stretch_factory-0.4.3/stretch_factory/hello_device_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import requests
 import os
 from subprocess import Popen, PIPE
 import fcntl
 import subprocess
 import sys
 import glob
+import yaml
 from subprocess import Popen, PIPE
 import usb.core
 import stretch_body.hello_utils as hello_utils
 import stretch_body.robot_params
 import stretch_body.device
 
 import serial
@@ -264,56 +265,72 @@
     else:
         print('FTDI port not found')
         return None
 
 
 # ###################################
 
+def create_arduinocli_config_file(firmware_path):
+    arduino_config = {'board_manager': {'additional_urls': []},
+                        'daemon': {'port': '50051'},
+                        'directories': {'data': os.environ['HOME'] + '/.arduino15',
+                                        'downloads': os.environ['HOME'] + '/.arduino15/staging',
+                                        'user': firmware_path + '/arduino'},
+                        'library': {'enable_unsafe_install': False},
+                        'logging': {'file': '', 'format': 'text', 'level': 'info'},
+                        'metrics': {'addr': ':9090', 'enabled': True},
+                        'sketch': {'always_export_binaries': False},
+                        'telemetry': {'addr': ':9090', 'enabled': True}}
+    with open(firmware_path + '/arduino-cli.yaml', 'w') as yaml_file:
+        yaml.dump(arduino_config, yaml_file, default_flow_style=False)
+    return firmware_path + '/arduino-cli.yaml'
 
-def compile_arduino_firmware(sketch_name, repo_path):
+def compile_arduino_firmware(sketch_name, repo_path, config_file=None):
     """
     :param sketch_name: eg 'hello_stepper'
     :return T if success:
     """
     text='------------------------ Compile Arduino Firmware {} ------------------------'.format(sketch_name)
     print(Style.BRIGHT + Fore.BLUE + text + Style.RESET_ALL)
-    compile_command = 'arduino-cli compile --fqbn hello-robot:samd:%s %s/arduino/%s' % (sketch_name, repo_path, sketch_name)
-    print(compile_command)
+    config_file_option = f' --config-file {config_file}' if config_file else ''
+    compile_command = f'arduino-cli compile{config_file_option} --fqbn hello-robot:samd:{sketch_name} {repo_path}/arduino/{sketch_name}'
+    print(f'Running: {compile_command}')
     c = Popen(compile_command, shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().strip()
     return c.find(b'Sketch uses') > -1
 
 
-def burn_arduino_firmware(port, sketch_name,repo_path):
+def burn_arduino_firmware(port, sketch_name, repo_path, config_file=None, verbose=False):
     text='------------------------ Flashing firmware %s | %s ------------------------' % (port, sketch_name)
     print(Style.BRIGHT + Fore.BLUE + text + Style.RESET_ALL)
 
     port_name = Popen("ls -l " + port, shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().strip().split()[-1]
     port_name=port_name.decode("utf-8")
     if '/dev/' != port_name[:5]:
         port_name = f"/dev/{port_name}"
     if port_name is not None:
-        upload_command = 'arduino-cli upload -p %s --fqbn hello-robot:samd:%s %s/arduino/%s' % (port_name, sketch_name,repo_path, sketch_name)
-        print('Running: %s'%upload_command)
+        config_file_option = f' --config-file {config_file}' if config_file else ''
+        upload_command = f'arduino-cli upload{config_file_option} -p {port_name} --fqbn hello-robot:samd:{sketch_name} {repo_path}/arduino/{sketch_name}'
+        print(f'Running: {upload_command}')
         u = Popen(upload_command, shell=True, bufsize=64, stdin=PIPE, stdout=PIPE, close_fds=True).stdout.read().strip()
         uu = u.split(b'\n')
-        #Pretty print the result
-        for l in uu:
-            k=l.split(b'\r')
-            if len(k)==1:
-                print(k[0].decode('utf-8'))
-            else:
-                for m in k:
-                    print(m.decode('utf-8'))
-        print('################')
+        if verbose:
+            #Pretty print the result
+            for l in uu:
+                k=l.split(b'\r')
+                if len(k)==1:
+                    print(k[0].decode('utf-8'))
+                else:
+                    for m in k:
+                        print(m.decode('utf-8'))
+            print('################')
         success=uu[-1]==b'CPU reset.'
         if not success:
             print('Firmware flash. Failed to upload to %s'% ( port))
             return False
-        else:
-            print('Success in firmware flash')
+        print('Success in firmware flash')
         return True
     else:
         print('Firmware flash. Failed to find device %s' % ( port))
         return False
 
 def burn_bootloader(sketch):
     print('-------- Burning bootlader ------------')
```

### Comparing `hello_robot_stretch_factory-0.4.2/stretch_factory/param_mgmt.py` & `hello_robot_stretch_factory-0.4.3/stretch_factory/param_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/test/test_firmware_updater.py` & `hello_robot_stretch_factory-0.4.3/test/test_firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/test/test_usb_reset.py` & `hello_robot_stretch_factory-0.4.3/test/test_usb_reset.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/RE1_migrate_contacts.py` & `hello_robot_stretch_factory-0.4.3/tools/RE1_migrate_contacts.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/RE1_migrate_params.py` & `hello_robot_stretch_factory-0.4.3/tools/RE1_migrate_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_D435i_check.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_D435i_check.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_base_calibrate_imu_collect.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_base_calibrate_imu_collect.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_base_calibrate_imu_process.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_base_calibrate_imu_process.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_base_calibrate_wheel_separation.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_base_calibrate_wheel_separation.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_calibrate_gravity_comp.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_calibrate_gravity_comp.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_calibrate_guarded_contact.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_calibrate_guarded_contact.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_calibrate_range.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_calibrate_range.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_cliff_sensor_calibrate.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_cliff_sensor_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_discover_hello_devices.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_discover_hello_devices.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_id_change.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_id_change.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_id_scan.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_id_scan.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_jog.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_reboot.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_reboot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_set_baud.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_dynamixel_set_baud.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_firmware_updater.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_gamepad_configure.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_gamepad_configure.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_gripper_calibrate.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_gripper_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_hello_dynamixel_jog.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_hello_dynamixel_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_stepper_calibration_YAML_to_flash.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_stepper_calibration_YAML_to_flash.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_stepper_calibration_flash_to_YAML.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_stepper_calibration_flash_to_YAML.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 parser.add_argument('stepper_name', metavar='stepper_name', type=str, nargs=1,help='Provide the stepper name e.g.: hello-motor-lift')
 args=parser.parse_args()
 
 motor = stepper.Stepper('/dev/'+args.stepper_name[0])
 if not motor.startup():
     exit(1)
 
+print('Reading calibration data from stepper...')
 data = motor.read_encoder_calibration_from_flash()
 print('Read data of len',len(data))
 print('Writing calibration data to YAML...')
 motor.write_encoder_calibration_to_YAML(data)
```

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_stepper_calibration_run.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_stepper_calibration_run.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_stepper_ctrl_tuning.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_stepper_ctrl_tuning.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_stepper_gains.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_stepper_gains.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_stepper_jog.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_stepper_jog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import sys
 import stretch_body.stepper as stepper
 import stretch_body.hello_utils as hu
 import argparse
-
+import time
 hu.print_stretch_re_use()
 
 parser=argparse.ArgumentParser(description='Menu interface to a Stepper controller')
 parser.add_argument('stepper_name', metavar='stepper_name', type=str, nargs=1,help='Provide the stepper name e.g.: hello-motor-lift')
 args=parser.parse_args()
 
 motor = stepper.Stepper('/dev/'+args.stepper_name[0])
@@ -37,14 +37,15 @@
     print('y <val>: set safety_feedforward')
     print('p <val>: set i_contact_pos')
     print('n <val>: set i_contact_neg')
     print('i <val>: set current')
     print('z <val>: mark position')
     print('g: set gain')
     print('r: reset board')
+    print('l: load test')
 
 def menu_gains():
     print('-----------')
     for k in motor.gains.keys():
         print(k + '     <val> [' + str(motor.gains[k])+']')
 
 def set_gains():
@@ -122,14 +123,22 @@
             motor.set_command(i_contact_pos=ff)
         if x[0]=='n':
             ff=float(x[1:])
             motor.set_command(i_contact_neg=ff)
         if x[0]=='g':
             menu_gains()
             set_gains()
+        if x[0]=='l':
+            ts = time.time()
+            for i in range(100):
+                print('---------- Load Test %d ----------' % i)
+                motor.push_load_test()
+                motor.pull_load_test()
+            dt = time.time() - ts
+            print('Average roundtrip time for 1024 bytes (ms): %f' % (dt * 1000 / 100))
         if x[0]=='r':
             print('Resetting Board. Restart process...')
             motor.board_reset()
             motor.push_command()
     else:
         motor.pretty_print()
     motor.push_command()
```

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_stepper_mechaduino_menu.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_stepper_mechaduino_menu.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_trace_firmware.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_trace_firmware.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_trace_robot.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_trace_robot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_usb_reset.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_usb_reset.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.2/tools/REx_wacc_calibrate.py` & `hello_robot_stretch_factory-0.4.3/tools/REx_wacc_calibrate.py`

 * *Files identical despite different names*

