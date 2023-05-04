# Comparing `tmp/UAVReaders-0.5.5.tar.gz` & `tmp/UAVReaders-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UAVReaders-0.5.5.tar", last modified: Thu May  4 21:10:35 2023, max compression
+gzip compressed data, was "UAVReaders-0.5.6.tar", last modified: Thu May  4 22:16:10 2023, max compression
```

## Comparing `UAVReaders-0.5.5.tar` & `UAVReaders-0.5.6.tar`

### file list

```diff
@@ -1,457 +1,457 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.980151 UAVReaders-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-04 21:10:07.000000 UAVReaders-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-04 21:10:35.980151 UAVReaders-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-04 21:10:07.000000 UAVReaders-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.940151 UAVReaders-0.5.5/UAVReaders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-04 21:10:35.000000 UAVReaders-0.5.5/UAVReaders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-05-04 21:10:35.000000 UAVReaders-0.5.5/UAVReaders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:10:35.000000 UAVReaders-0.5.5/UAVReaders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 21:10:35.000000 UAVReaders-0.5.5/UAVReaders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-04 21:10:07.000000 UAVReaders-0.5.5/c_introspect.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-04 21:10:07.000000 UAVReaders-0.5.5/c_introspect.h
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-04 21:10:07.000000 UAVReaders-0.5.5/dataflash.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-04 21:10:07.000000 UAVReaders-0.5.5/dataflash.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.940151 UAVReaders-0.5.5/mavlink/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.940151 UAVReaders-0.5.5/mavlink/ASLUAV/
--rw-r--r--   0 runner    (1001) docker     (123)    25765 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/ASLUAV.h
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_asl_obctrl.h
--rw-r--r--   0 runner    (1001) docker     (123)    32302 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_aslctrl_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_aslctrl_debug.h
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_asluav_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_command_int_stamped.h
--rw-r--r--   0 runner    (1001) docker     (123)    25076 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_command_long_stamped.h
--rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_ekf_ext.h
--rw-r--r--   0 runner    (1001) docker     (123)    37305 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_fw_soaring_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_gsm_link_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    18821 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_satcom_link_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_sens_atmos.h
--rw-r--r--   0 runner    (1001) docker     (123)    26167 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_sens_batmon.h
--rw-r--r--   0 runner    (1001) docker     (123)    21554 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_sens_mppt.h
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_sens_power.h
--rw-r--r--   0 runner    (1001) docker     (123)    24857 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_sens_power_board.h
--rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_sensor_airflow_angles.h
--rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_sensorpod_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    66439 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ASLUAV/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.940151 UAVReaders-0.5.5/mavlink/AVSSUAS/
--rw-r--r--   0 runner    (1001) docker     (123)    25409 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/AVSSUAS/AVSSUAS.h
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/AVSSUAS/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/AVSSUAS/mavlink_msg_avss_drone_imu.h
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/AVSSUAS/mavlink_msg_avss_drone_operation_mode.h
--rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/AVSSUAS/mavlink_msg_avss_drone_position.h
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/AVSSUAS/mavlink_msg_avss_prs_sys_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/AVSSUAS/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/AVSSUAS/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.944151 UAVReaders-0.5.5/mavlink/all/
--rw-r--r--   0 runner    (1001) docker     (123)    35977 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/all/all.h
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/all/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/all/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/all/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.948151 UAVReaders-0.5.5/mavlink/ardupilotmega/
--rw-r--r--   0 runner    (1001) docker     (123)   146469 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/ardupilotmega.h
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_adap_tuning.h
--rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_ahrs.h
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_ahrs2.h
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_ahrs3.h
--rw-r--r--   0 runner    (1001) docker     (123)    19616 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_airspeed_autocal.h
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_aoa_ssa.h
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_ap_adc.h
--rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_autopilot_version_request.h
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_battery2.h
--rw-r--r--   0 runner    (1001) docker     (123)    23445 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_camera_feedback.h
--rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_camera_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    14750 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_compassmot_status.h
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_data16.h
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_data32.h
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_data64.h
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_data96.h
--rw-r--r--   0 runner    (1001) docker     (123)    19561 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_deepstall.h
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_device_op_read.h
--rw-r--r--   0 runner    (1001) docker     (123)    14869 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_device_op_read_reply.h
--rw-r--r--   0 runner    (1001) docker     (123)    20176 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_device_op_write.h
--rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_device_op_write_reply.h
--rw-r--r--   0 runner    (1001) docker     (123)    22964 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_digicam_configure.h
--rw-r--r--   0 runner    (1001) docker     (123)    20889 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_digicam_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_ekf_status_report.h
--rw-r--r--   0 runner    (1001) docker     (123)    16696 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_1_to_4.h
--rw-r--r--   0 runner    (1001) docker     (123)    16696 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_5_to_8.h
--rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_9_to_12.h
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_fence_fetch_point.h
--rw-r--r--   0 runner    (1001) docker     (123)    13532 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_fence_point.h
--rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gimbal_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gimbal_report.h
--rw-r--r--   0 runner    (1001) docker     (123)    14917 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gimbal_torque_cmd_report.h
--rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gopro_get_request.h
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gopro_get_response.h
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gopro_heartbeat.h
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gopro_set_request.h
--rw-r--r--   0 runner    (1001) docker     (123)     9542 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gopro_set_response.h
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_hwstatus.h
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_led_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_limits_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    19419 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_mag_cal_progress.h
--rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_mcu_status.h
--rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_meminfo.h
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_mount_configure.h
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_mount_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_mount_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_obstacle_distance_3d.h
--rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_osd_param_config.h
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_osd_param_config_reply.h
--rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config.h
--rw-r--r--   0 runner    (1001) docker     (123)    18684 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config_reply.h
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_pid_tuning.h
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_radio.h
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_rally_fetch_point.h
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_rally_point.h
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_rangefinder.h
--rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_remote_log_block_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_remote_log_data_block.h
--rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_rpm.h
--rw-r--r--   0 runner    (1001) docker     (123)    21565 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_sensor_offsets.h
--rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_set_mag_offsets.h
--rw-r--r--   0 runner    (1001) docker     (123)    17127 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_simstate.h
--rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_vision_position_delta.h
--rw-r--r--   0 runner    (1001) docker     (123)    18313 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_water_depth.h
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_wind.h
--rw-r--r--   0 runner    (1001) docker     (123)   219339 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/ardupilotmega/version.h
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/checksum.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.972151 UAVReaders-0.5.5/mavlink/common/
--rw-r--r--   0 runner    (1001) docker     (123)   164519 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/common.h
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    15007 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_actuator_control_target.h
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_actuator_output_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_adsb_vehicle.h
--rw-r--r--   0 runner    (1001) docker     (123)    27216 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_ais_vessel.h
--rw-r--r--   0 runner    (1001) docker     (123)    22867 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_altitude.h
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_att_pos_mocap.h
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_attitude.h
--rw-r--r--   0 runner    (1001) docker     (123)    21250 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_attitude_quaternion.h
--rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_attitude_quaternion_cov.h
--rw-r--r--   0 runner    (1001) docker     (123)    16735 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_attitude_target.h
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_auth_key.h
--rw-r--r--   0 runner    (1001) docker     (123)    30727 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_autopilot_state_for_gimbal_device.h
--rw-r--r--   0 runner    (1001) docker     (123)    29075 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_autopilot_version.h
--rw-r--r--   0 runner    (1001) docker     (123)    32779 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_battery_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_button_change.h
--rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_capture_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    21741 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_fov_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_image_captured.h
--rw-r--r--   0 runner    (1001) docker     (123)    28706 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_settings.h
--rw-r--r--   0 runner    (1001) docker     (123)    24575 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_tracking_geo_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    25202 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_tracking_image_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_trigger.h
--rw-r--r--   0 runner    (1001) docker     (123)    14952 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_can_filter_modify.h
--rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_can_frame.h
--rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_canfd_frame.h
--rw-r--r--   0 runner    (1001) docker     (123)    20341 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_cellular_config.h
--rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_cellular_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_change_operator_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_change_operator_control_ack.h
--rw-r--r--   0 runner    (1001) docker     (123)    16191 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_collision.h
--rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_command_ack.h
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_command_cancel.h
--rw-r--r--   0 runner    (1001) docker     (123)    21732 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_command_int.h
--rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_command_long.h
--rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_component_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_component_metadata.h
--rw-r--r--   0 runner    (1001) docker     (123)    29561 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_control_system_state.h
--rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_current_event_sequence.h
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_data_stream.h
--rw-r--r--   0 runner    (1001) docker     (123)    17663 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_data_transmission_handshake.h
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_debug.h
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_debug_float_array.h
--rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_debug_vect.h
--rw-r--r--   0 runner    (1001) docker     (123)    27666 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_distance_sensor.h
--rw-r--r--   0 runner    (1001) docker     (123)    32838 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_efi_status.h
--rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_encapsulated_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    20131 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_esc_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_esc_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    21732 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_estimator_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_event.h
--rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_extended_sys_state.h
--rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_fence_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_file_transfer_protocol.h
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_flight_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_follow_target.h
--rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_generator_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    27546 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_device_attitude_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    32438 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_device_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_device_set_attitude.h
--rw-r--r--   0 runner    (1001) docker     (123)    21643 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_manager_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    22236 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_manager_set_attitude.h
--rw-r--r--   0 runner    (1001) docker     (123)    21708 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_manager_set_manual_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_manager_set_pitchyaw.h
--rw-r--r--   0 runner    (1001) docker     (123)    19605 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_manager_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_global_position_int.h
--rw-r--r--   0 runner    (1001) docker     (123)    22136 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_global_position_int_cov.h
--rw-r--r--   0 runner    (1001) docker     (123)    22008 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_global_vision_position_estimate.h
--rw-r--r--   0 runner    (1001) docker     (123)    29060 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps2_raw.h
--rw-r--r--   0 runner    (1001) docker     (123)    23748 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps2_rtk.h
--rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps_global_origin.h
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps_inject_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    30409 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps_input.h
--rw-r--r--   0 runner    (1001) docker     (123)    28204 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps_raw_int.h
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps_rtcm_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    23541 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps_rtk.h
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    36773 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_high_latency.h
--rw-r--r--   0 runner    (1001) docker     (123)    40352 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_high_latency2.h
--rw-r--r--   0 runner    (1001) docker     (123)    25647 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_highres_imu.h
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_actuator_controls.h
--rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_controls.h
--rw-r--r--   0 runner    (1001) docker     (123)    25408 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_gps.h
--rw-r--r--   0 runner    (1001) docker     (123)    26914 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_optical_flow.h
--rw-r--r--   0 runner    (1001) docker     (123)    25694 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_rc_inputs_raw.h
--rw-r--r--   0 runner    (1001) docker     (123)    25462 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_sensor.h
--rw-r--r--   0 runner    (1001) docker     (123)    23587 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_state.h
--rw-r--r--   0 runner    (1001) docker     (123)    28077 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_state_quaternion.h
--rw-r--r--   0 runner    (1001) docker     (123)    26362 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_home_position.h
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_hygrometer_sensor.h
--rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_isbd_link_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_landing_target.h
--rw-r--r--   0 runner    (1001) docker     (123)    22275 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_link_node_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_local_position_ned.h
--rw-r--r--   0 runner    (1001) docker     (123)    23152 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_local_position_ned_cov.h
--rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_local_position_ned_system_global_offset.h
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_log_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_log_entry.h
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_log_erase.h
--rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_log_request_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_log_request_end.h
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_log_request_list.h
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_logging_ack.h
--rw-r--r--   0 runner    (1001) docker     (123)    15228 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_logging_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_logging_data_acked.h
--rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mag_cal_report.h
--rw-r--r--   0 runner    (1001) docker     (123)    25464 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_manual_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_manual_setpoint.h
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_memory_vect.h
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_message_interval.h
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_ack.h
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_clear_all.h
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_count.h
--rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_current.h
--rw-r--r--   0 runner    (1001) docker     (123)    24141 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_item.h
--rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_item_int.h
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_item_reached.h
--rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_request.h
--rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_request_int.h
--rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_request_list.h
--rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_request_partial_list.h
--rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_set_current.h
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_write_partial_list.h
--rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_mount_orientation.h
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_named_value_float.h
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_named_value_int.h
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_nav_controller_output.h
--rw-r--r--   0 runner    (1001) docker     (123)    24972 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_obstacle_distance.h
--rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_odometry.h
--rw-r--r--   0 runner    (1001) docker     (123)    48490 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_onboard_computer_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_arm_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    25685 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_authentication.h
--rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_basic_id.h
--rw-r--r--   0 runner    (1001) docker     (123)    40771 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_location.h
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_message_pack.h
--rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_operator_id.h
--rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_self_id.h
--rw-r--r--   0 runner    (1001) docker     (123)    32622 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_system.h
--rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_system_update.h
--rw-r--r--   0 runner    (1001) docker     (123)    20576 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_optical_flow.h
--rw-r--r--   0 runner    (1001) docker     (123)    26804 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_optical_flow_rad.h
--rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_orbit_execution_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_ext_ack.h
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_ext_request_list.h
--rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_ext_request_read.h
--rw-r--r--   0 runner    (1001) docker     (123)    14708 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_ext_set.h
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_ext_value.h
--rw-r--r--   0 runner    (1001) docker     (123)    22140 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_map_rc.h
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_request_list.h
--rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_request_read.h
--rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_set.h
--rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_value.h
--rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_ping.h
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_play_tune.h
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_play_tune_v2.h
--rw-r--r--   0 runner    (1001) docker     (123)    27839 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_position_target_global_int.h
--rw-r--r--   0 runner    (1001) docker     (123)    26159 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_position_target_local_ned.h
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_power_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    17212 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_radio_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_raw_imu.h
--rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_raw_pressure.h
--rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_raw_rpm.h
--rw-r--r--   0 runner    (1001) docker     (123)    33163 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_rc_channels.h
--rw-r--r--   0 runner    (1001) docker     (123)    44394 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_rc_channels_override.h
--rw-r--r--   0 runner    (1001) docker     (123)    21192 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_rc_channels_raw.h
--rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_rc_channels_scaled.h
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_request_data_stream.h
--rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_request_event.h
--rw-r--r--   0 runner    (1001) docker     (123)    15666 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_resource_request.h
--rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_response_event_error.h
--rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_safety_allowed_area.h
--rw-r--r--   0 runner    (1001) docker     (123)    18702 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_safety_set_allowed_area.h
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_scaled_imu.h
--rw-r--r--   0 runner    (1001) docker     (123)    19078 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_scaled_imu2.h
--rw-r--r--   0 runner    (1001) docker     (123)    19078 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_scaled_imu3.h
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_scaled_pressure.h
--rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_scaled_pressure2.h
--rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_scaled_pressure3.h
--rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_serial_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    31142 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_servo_output_raw.h
--rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_set_actuator_control_target.h
--rw-r--r--   0 runner    (1001) docker     (123)    21827 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_set_attitude_target.h
--rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_set_gps_global_origin.h
--rw-r--r--   0 runner    (1001) docker     (123)    28389 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_set_home_position.h
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_set_mode.h
--rw-r--r--   0 runner    (1001) docker     (123)    31542 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_set_position_target_global_int.h
--rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_set_position_target_local_ned.h
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_setup_signing.h
--rw-r--r--   0 runner    (1001) docker     (123)    33189 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_sim_state.h
--rw-r--r--   0 runner    (1001) docker     (123)    37137 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_smart_battery_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_statustext.h
--rw-r--r--   0 runner    (1001) docker     (123)    27262 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_storage_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_supported_tunes.h
--rw-r--r--   0 runner    (1001) docker     (123)    36382 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_sys_status.h
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_system_time.h
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_terrain_check.h
--rw-r--r--   0 runner    (1001) docker     (123)    12755 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_terrain_data.h
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_terrain_report.h
--rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_terrain_request.h
--rw-r--r--   0 runner    (1001) docker     (123)    17785 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_time_estimate_to_target.h
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_timesync.h
--rw-r--r--   0 runner    (1001) docker     (123)    21152 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_trajectory_representation_bezier.h
--rw-r--r--   0 runner    (1001) docker     (123)    33591 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_trajectory_representation_waypoints.h
--rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_tunnel.h
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_uavcan_node_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_uavcan_node_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    29856 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_utm_global_position.h
--rw-r--r--   0 runner    (1001) docker     (123)    19231 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_v2_extension.h
--rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_vfr_hud.h
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_vibration.h
--rw-r--r--   0 runner    (1001) docker     (123)    18003 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_vicon_position_estimate.h
--rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_video_stream_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_video_stream_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    20723 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_vision_position_estimate.h
--rw-r--r--   0 runner    (1001) docker     (123)    16707 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_vision_speed_estimate.h
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_wheel_distance.h
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_wifi_config_ap.h
--rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_winch_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/mavlink_msg_wind_cov.h
--rw-r--r--   0 runner    (1001) docker     (123)   809444 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/common/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-04 21:10:21.000000 UAVReaders-0.5.5/mavlink/common/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.972151 UAVReaders-0.5.5/mavlink/cubepilot/
--rw-r--r--   0 runner    (1001) docker     (123)    23606 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/cubepilot/cubepilot.h
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/cubepilot/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_resp.h
--rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_start.h
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/cubepilot/mavlink_msg_cubepilot_raw_rc.h
--rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/cubepilot/mavlink_msg_herelink_telem.h
--rw-r--r--   0 runner    (1001) docker     (123)    20451 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/cubepilot/mavlink_msg_herelink_video_stream_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/cubepilot/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/cubepilot/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.976151 UAVReaders-0.5.5/mavlink/development/
--rw-r--r--   0 runner    (1001) docker     (123)    38436 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/development.h
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/mavlink_msg_airspeed.h
--rw-r--r--   0 runner    (1001) docker     (123)    15694 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/mavlink_msg_available_modes.h
--rw-r--r--   0 runner    (1001) docker     (123)    20885 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/mavlink_msg_battery_status_v2.h
--rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/mavlink_msg_component_information_basic.h
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/mavlink_msg_current_mode.h
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/mavlink_msg_figure_eight_execution_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    11639 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/mavlink_msg_group_end.h
--rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/mavlink_msg_group_start.h
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/mavlink_msg_mission_checksum.h
--rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/mavlink_msg_param_ack_transaction.h
--rw-r--r--   0 runner    (1001) docker     (123)    25425 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/mavlink_msg_target_absolute.h
--rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/mavlink_msg_target_relative.h
--rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/mavlink_msg_wifi_network_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    45228 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/development/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.976151 UAVReaders-0.5.5/mavlink/icarous/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/icarous/icarous.h
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/icarous/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/icarous/mavlink_msg_icarous_heartbeat.h
--rw-r--r--   0 runner    (1001) docker     (123)    25956 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/icarous/mavlink_msg_icarous_kinematic_bands.h
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/icarous/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/icarous/version.h
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/mavlink_conversions.h
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/mavlink_get_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    37370 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/mavlink_helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/mavlink_sha256.h
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/mavlink_types.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.976151 UAVReaders-0.5.5/mavlink/minimal/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/minimal/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/minimal/mavlink_msg_heartbeat.h
--rw-r--r--   0 runner    (1001) docker     (123)    15671 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/minimal/mavlink_msg_protocol_version.h
--rw-r--r--   0 runner    (1001) docker     (123)    30757 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/minimal/minimal.h
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/minimal/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/minimal/version.h
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/protocol.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.976151 UAVReaders-0.5.5/mavlink/python_array_test/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/python_array_test/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_0.h
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_1.h
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_3.h
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_4.h
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_5.h
--rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_6.h
--rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_7.h
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_8.h
--rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/python_array_test/python_array_test.h
--rw-r--r--   0 runner    (1001) docker     (123)    26161 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/python_array_test/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/python_array_test/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.976151 UAVReaders-0.5.5/mavlink/standard/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/standard/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/standard/standard.h
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/standard/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/standard/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.980151 UAVReaders-0.5.5/mavlink/storm32/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/storm32/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_frsky_passthrough_array.h
--rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_param_value_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_qshot_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    28610 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_radio_link_stats.h
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_radio_rc_channels.h
--rw-r--r--   0 runner    (1001) docker     (123)    26585 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control.h
--rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control_pitchyaw.h
--rw-r--r--   0 runner    (1001) docker     (123)    16806 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_correct_roll.h
--rw-r--r--   0 runner    (1001) docker     (123)    24582 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    41669 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/storm32/storm32.h
--rw-r--r--   0 runner    (1001) docker     (123)    39288 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/storm32/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/storm32/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.980151 UAVReaders-0.5.5/mavlink/test/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/test/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    31221 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/test/mavlink_msg_test_types.h
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/test/test.h
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/test/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/test/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.980151 UAVReaders-0.5.5/mavlink/uAvionix/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/uAvionix/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_cfg.h
--rw-r--r--   0 runner    (1001) docker     (123)    31688 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_dynamic.h
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/uAvionix/mavlink_msg_uavionix_adsb_transceiver_health_report.h
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/uAvionix/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)    28685 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/uAvionix/uAvionix.h
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/uAvionix/version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:10:35.980151 UAVReaders-0.5.5/mavlink/ualberta/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/ualberta/mavlink.h
--rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/ualberta/mavlink_msg_nav_filter_bias.h
--rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/ualberta/mavlink_msg_radio_calibration.h
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/ualberta/mavlink_msg_ualberta_sys_status.h
--rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/ualberta/testsuite.h
--rw-r--r--   0 runner    (1001) docker     (123)    24427 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/ualberta/ualberta.h
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink/ualberta/version.h
--rw-r--r--   0 runner    (1001) docker     (123)   708323 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink_introspect_gen.c
--rw-r--r--   0 runner    (1001) docker     (123)    24009 2023-05-04 21:10:22.000000 UAVReaders-0.5.5/mavlink_introspect_gen.h
--rw-r--r--   0 runner    (1001) docker     (123)  1126517 2023-05-04 21:10:23.000000 UAVReaders-0.5.5/pyinterop.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-04 21:10:07.000000 UAVReaders-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-04 21:10:07.000000 UAVReaders-0.5.5/readers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-04 21:10:07.000000 UAVReaders-0.5.5/readers.h
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:10:35.980151 UAVReaders-0.5.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-05-04 21:10:07.000000 UAVReaders-0.5.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-04 21:10:07.000000 UAVReaders-0.5.5/table.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.855582 UAVReaders-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-04 22:16:10.855582 UAVReaders-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.775581 UAVReaders-0.5.6/UAVReaders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-04 22:16:10.000000 UAVReaders-0.5.6/UAVReaders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-05-04 22:16:10.000000 UAVReaders-0.5.6/UAVReaders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:16:10.000000 UAVReaders-0.5.6/UAVReaders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 22:16:10.000000 UAVReaders-0.5.6/UAVReaders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/c_introspect.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/c_introspect.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/dataflash.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/dataflash.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.775581 UAVReaders-0.5.6/mavlink/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.779581 UAVReaders-0.5.6/mavlink/ASLUAV/
+-rw-r--r--   0 runner    (1001) docker     (123)    25766 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/ASLUAV.h
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_asl_obctrl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32302 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_aslctrl_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_aslctrl_debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_asluav_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_command_int_stamped.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25076 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_command_long_stamped.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_ekf_ext.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37305 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_fw_soaring_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_gsm_link_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18821 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_satcom_link_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_atmos.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26167 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_batmon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21554 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_mppt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_power.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24857 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_power_board.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sensor_airflow_angles.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sensorpod_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    66439 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ASLUAV/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.783581 UAVReaders-0.5.6/mavlink/AVSSUAS/
+-rw-r--r--   0 runner    (1001) docker     (123)    25408 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/AVSSUAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_drone_imu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_drone_operation_mode.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_drone_position.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_prs_sys_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/AVSSUAS/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.783581 UAVReaders-0.5.6/mavlink/all/
+-rw-r--r--   0 runner    (1001) docker     (123)    35975 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/all/all.h
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/all/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/all/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/all/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.795581 UAVReaders-0.5.6/mavlink/ardupilotmega/
+-rw-r--r--   0 runner    (1001) docker     (123)   146469 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/ardupilotmega.h
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_adap_tuning.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ahrs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ahrs2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ahrs3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19616 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_airspeed_autocal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_aoa_ssa.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ap_adc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_autopilot_version_request.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_battery2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23445 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_camera_feedback.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_camera_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14750 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_compassmot_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data16.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data32.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data64.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data96.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19561 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_deepstall.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_read.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14869 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_read_reply.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20176 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_write.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_write_reply.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22964 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_digicam_configure.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20889 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_digicam_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ekf_status_report.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16696 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_1_to_4.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16696 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_5_to_8.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_9_to_12.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_fence_fetch_point.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13532 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_fence_point.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gimbal_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gimbal_report.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14917 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gimbal_torque_cmd_report.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_get_request.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_get_response.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_heartbeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_set_request.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9542 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_set_response.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_hwstatus.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_led_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_limits_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19419 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mag_cal_progress.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mcu_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_meminfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mount_configure.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mount_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mount_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_obstacle_distance_3d.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_config_reply.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14313 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18684 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config_reply.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_pid_tuning.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_radio.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rally_fetch_point.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rally_point.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rangefinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_remote_log_block_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_remote_log_data_block.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rpm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21565 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_sensor_offsets.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_set_mag_offsets.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17127 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_simstate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_vision_position_delta.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18313 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_water_depth.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_wind.h
+-rw-r--r--   0 runner    (1001) docker     (123)   219339 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/ardupilotmega/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/checksum.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.839582 UAVReaders-0.5.6/mavlink/common/
+-rw-r--r--   0 runner    (1001) docker     (123)   164519 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15007 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_actuator_control_target.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_actuator_output_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_adsb_vehicle.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27216 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_ais_vessel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22867 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_altitude.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_att_pos_mocap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21250 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude_quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude_quaternion_cov.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16735 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude_target.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_auth_key.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30727 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_autopilot_state_for_gimbal_device.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29075 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_autopilot_version.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32779 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_battery_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_button_change.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_capture_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21741 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_fov_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_image_captured.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28706 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_settings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24575 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_tracking_geo_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25202 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_tracking_image_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_trigger.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14952 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_can_filter_modify.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_can_frame.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_canfd_frame.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20341 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_cellular_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_cellular_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_change_operator_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_change_operator_control_ack.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16191 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_collision.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_ack.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_cancel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21732 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_long.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_component_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_component_metadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29561 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_control_system_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_current_event_sequence.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_data_stream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17663 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_data_transmission_handshake.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_debug_float_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_debug_vect.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27666 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_distance_sensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32838 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_efi_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_encapsulated_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20131 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_esc_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_esc_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21732 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_estimator_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_event.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_extended_sys_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_fence_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_file_transfer_protocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_flight_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_follow_target.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_generator_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27546 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_device_attitude_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32438 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_device_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_device_set_attitude.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21643 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22236 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_set_attitude.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21708 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_set_manual_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_set_pitchyaw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19605 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_global_position_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22136 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_global_position_int_cov.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22008 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_global_vision_position_estimate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29060 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps2_raw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23748 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps2_rtk.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_global_origin.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_inject_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30409 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_input.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28204 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_raw_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_rtcm_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23541 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_rtk.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36773 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_high_latency.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40352 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_high_latency2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25647 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_highres_imu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_actuator_controls.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_controls.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25408 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_gps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26914 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_optical_flow.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25694 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_rc_inputs_raw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25462 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_sensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23587 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28077 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_state_quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26362 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_home_position.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_hygrometer_sensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_isbd_link_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_landing_target.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22275 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_link_node_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_local_position_ned.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23152 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_local_position_ned_cov.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_local_position_ned_system_global_offset.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_entry.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_erase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_request_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_request_end.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_request_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_logging_ack.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15228 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_logging_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_logging_data_acked.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mag_cal_report.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25464 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_manual_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_manual_setpoint.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_memory_vect.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_message_interval.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_ack.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_clear_all.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_count.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_current.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24141 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_item.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_item_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_item_reached.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request_partial_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_set_current.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_write_partial_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13896 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_mount_orientation.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_named_value_float.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_named_value_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_nav_controller_output.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24972 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_obstacle_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_odometry.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48490 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_onboard_computer_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_arm_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25685 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_authentication.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_basic_id.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40771 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_location.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_message_pack.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16940 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_operator_id.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_self_id.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32622 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_system.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_system_update.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20576 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_optical_flow.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26804 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_optical_flow_rad.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_orbit_execution_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_ack.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_request_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_request_read.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14708 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_value.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22140 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_map_rc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_request_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_request_read.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_value.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_ping.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_play_tune.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_play_tune_v2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27839 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_position_target_global_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26159 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_position_target_local_ned.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_power_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17212 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_radio_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_raw_imu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_raw_pressure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_raw_rpm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33163 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44394 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels_override.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21192 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels_raw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels_scaled.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_request_data_stream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_request_event.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15666 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_resource_request.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_response_event_error.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_safety_allowed_area.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18702 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_safety_set_allowed_area.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_imu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19078 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_imu2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19078 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_imu3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_pressure.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_pressure2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_pressure3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_serial_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31142 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_servo_output_raw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_actuator_control_target.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21827 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_attitude_target.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_gps_global_origin.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28389 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_home_position.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_mode.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31542 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_position_target_global_int.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_position_target_local_ned.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_setup_signing.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33189 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_sim_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37137 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_smart_battery_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_statustext.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27262 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_storage_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_supported_tunes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36382 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_sys_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_system_time.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_check.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12755 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_report.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_request.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17785 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_time_estimate_to_target.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_timesync.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21152 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_trajectory_representation_bezier.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33591 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_trajectory_representation_waypoints.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_tunnel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_uavcan_node_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_uavcan_node_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29856 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_utm_global_position.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19231 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_v2_extension.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_vfr_hud.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_vibration.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18003 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_vicon_position_estimate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_video_stream_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_video_stream_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20723 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_vision_position_estimate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16707 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_vision_speed_estimate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_wheel_distance.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_wifi_config_ap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17186 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_winch_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/mavlink_msg_wind_cov.h
+-rw-r--r--   0 runner    (1001) docker     (123)   809444 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/common/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-04 22:15:54.000000 UAVReaders-0.5.6/mavlink/common/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.839582 UAVReaders-0.5.6/mavlink/cubepilot/
+-rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/cubepilot.h
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_resp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_start.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_cubepilot_raw_rc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_herelink_telem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20451 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_herelink_video_stream_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/cubepilot/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.843582 UAVReaders-0.5.6/mavlink/development/
+-rw-r--r--   0 runner    (1001) docker     (123)    38436 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/development.h
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_airspeed.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15694 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_available_modes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20885 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_battery_status_v2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_component_information_basic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_current_mode.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_figure_eight_execution_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11639 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_group_end.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_group_start.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_mission_checksum.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_param_ack_transaction.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25425 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_target_absolute.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_target_relative.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/mavlink_msg_wifi_network_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45228 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/development/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.843582 UAVReaders-0.5.6/mavlink/icarous/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/icarous/icarous.h
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/icarous/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/icarous/mavlink_msg_icarous_heartbeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25956 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/icarous/mavlink_msg_icarous_kinematic_bands.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/icarous/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/icarous/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/mavlink_conversions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/mavlink_get_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37370 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/mavlink_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/mavlink_sha256.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/mavlink_types.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.847582 UAVReaders-0.5.6/mavlink/minimal/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/minimal/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/minimal/mavlink_msg_heartbeat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15671 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/minimal/mavlink_msg_protocol_version.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30758 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/minimal/minimal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/minimal/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/minimal/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/protocol.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.847582 UAVReaders-0.5.6/mavlink/python_array_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_0.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_3.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_4.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_5.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_6.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_7.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_8.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/python_array_test.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26161 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/python_array_test/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.847582 UAVReaders-0.5.6/mavlink/standard/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/standard/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/standard/standard.h
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/standard/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/standard/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.851582 UAVReaders-0.5.6/mavlink/storm32/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_frsky_passthrough_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_param_value_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_qshot_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28610 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_radio_link_stats.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_radio_rc_channels.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26585 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control_pitchyaw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16806 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_correct_roll.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24582 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41670 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/storm32.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39288 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/storm32/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.851582 UAVReaders-0.5.6/mavlink/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/test/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31221 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/test/mavlink_msg_test_types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/test/test.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/test/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/test/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.851582 UAVReaders-0.5.6/mavlink/uAvionix/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/uAvionix/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_cfg.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31688 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_dynamic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/uAvionix/mavlink_msg_uavionix_adsb_transceiver_health_report.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/uAvionix/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28686 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/uAvionix/uAvionix.h
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/uAvionix/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:16:10.855582 UAVReaders-0.5.6/mavlink/ualberta/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/ualberta/mavlink.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14284 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/ualberta/mavlink_msg_nav_filter_bias.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/ualberta/mavlink_msg_radio_calibration.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/ualberta/mavlink_msg_ualberta_sys_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/ualberta/testsuite.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24428 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/ualberta/ualberta.h
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink/ualberta/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)   708323 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink_introspect_gen.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24009 2023-05-04 22:15:55.000000 UAVReaders-0.5.6/mavlink_introspect_gen.h
+-rw-r--r--   0 runner    (1001) docker     (123)  1117162 2023-05-04 22:15:56.000000 UAVReaders-0.5.6/pyinterop.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/readers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/readers.h
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 22:16:10.855582 UAVReaders-0.5.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-04 22:15:35.000000 UAVReaders-0.5.6/table.h
```

### Comparing `UAVReaders-0.5.5/PKG-INFO` & `UAVReaders-0.5.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,8 @@
-Metadata-Version: 2.1
-Name: UAVReaders
-Version: 0.5.5
-Summary: Parsers for UAV/Aerial Drone-related formats like MavLink and DataFlash
-Author: Christian Clifford
-Author-email: Christian Clifford <cjclifford@alaska.edu>
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+[![Test UAVReaders](https://github.com/UA-ACUASI-Engineering/UAVReaders/actions/workflows/test_uavreaders.yml/badge.svg)](https://github.com/UA-ACUASI-Engineering/UAVReaders/actions/workflows/test_uavreaders.yml)
 
 # UAVReaders
 Parsers for UAV-related formats like DataFlash and Mavlink
 
 ## Installation and Usage
 
 This package is available from PyPI. You can install it by doing something
```

### Comparing `UAVReaders-0.5.5/README.md` & `UAVReaders-0.5.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: UAVReaders
+Version: 0.5.6
+Summary: Parsers for UAV/Aerial Drone-related formats like MavLink and DataFlash
+Author: Christian Clifford
+Author-email: Christian Clifford <cjclifford@alaska.edu>
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+[![Test UAVReaders](https://github.com/UA-ACUASI-Engineering/UAVReaders/actions/workflows/test_uavreaders.yml/badge.svg)](https://github.com/UA-ACUASI-Engineering/UAVReaders/actions/workflows/test_uavreaders.yml)
+
 # UAVReaders
 Parsers for UAV-related formats like DataFlash and Mavlink
 
 ## Installation and Usage
 
 This package is available from PyPI. You can install it by doing something
 like this: `pip install UAVReaders`.
```

### Comparing `UAVReaders-0.5.5/UAVReaders.egg-info/PKG-INFO` & `UAVReaders-0.5.6/UAVReaders.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: UAVReaders
-Version: 0.5.5
+Version: 0.5.6
 Summary: Parsers for UAV/Aerial Drone-related formats like MavLink and DataFlash
 Author: Christian Clifford
 Author-email: Christian Clifford <cjclifford@alaska.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
+[![Test UAVReaders](https://github.com/UA-ACUASI-Engineering/UAVReaders/actions/workflows/test_uavreaders.yml/badge.svg)](https://github.com/UA-ACUASI-Engineering/UAVReaders/actions/workflows/test_uavreaders.yml)
+
 # UAVReaders
 Parsers for UAV-related formats like DataFlash and Mavlink
 
 ## Installation and Usage
 
 This package is available from PyPI. You can install it by doing something
 like this: `pip install UAVReaders`.
```

### Comparing `UAVReaders-0.5.5/UAVReaders.egg-info/SOURCES.txt` & `UAVReaders-0.5.6/UAVReaders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/c_introspect.h` & `UAVReaders-0.5.6/c_introspect.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/dataflash.cpp` & `UAVReaders-0.5.6/dataflash.cpp`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/dataflash.h` & `UAVReaders-0.5.6/dataflash.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/ASLUAV.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/ASLUAV.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_ASLUAV_H
 #define MAVLINK_ASLUAV_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_ASLUAV.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_ASLUAV_XML_HASH 2196609791571168227
+#define MAVLINK_ASLUAV_XML_HASH -6921207667047634836
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink.h` & `UAVReaders-0.5.6/mavlink/test/mavlink.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from ASLUAV.xml
+ *  @brief MAVLink comm protocol built from test.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 2196609791571168227
+#define MAVLINK_PRIMARY_XML_HASH -5416981559095984788
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "ASLUAV.h"
+#include "test.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_asl_obctrl.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_asl_obctrl.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_aslctrl_data.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_aslctrl_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_aslctrl_debug.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_aslctrl_debug.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_asluav_status.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_asluav_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_command_int_stamped.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_command_int_stamped.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_command_long_stamped.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_command_long_stamped.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_ekf_ext.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_ekf_ext.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_fw_soaring_data.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_fw_soaring_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_gsm_link_status.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_gsm_link_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_satcom_link_status.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_satcom_link_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_sens_atmos.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_atmos.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_sens_batmon.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_batmon.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_sens_mppt.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_mppt.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_sens_power.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_power.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_sens_power_board.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sens_power_board.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_sensor_airflow_angles.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sensor_airflow_angles.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/mavlink_msg_sensorpod_status.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink_msg_sensorpod_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ASLUAV/testsuite.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/AVSSUAS/AVSSUAS.h` & `UAVReaders-0.5.6/mavlink/AVSSUAS/AVSSUAS.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_AVSSUAS_H
 #define MAVLINK_AVSSUAS_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_AVSSUAS.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_AVSSUAS_XML_HASH -4496709155418371116
+#define MAVLINK_AVSSUAS_XML_HASH 2697101801489672959
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink/AVSSUAS/mavlink.h` & `UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink.h`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  *  @brief MAVLink comm protocol built from AVSSUAS.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH -4496709155418371116
+#define MAVLINK_PRIMARY_XML_HASH 2697101801489672959
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
```

### Comparing `UAVReaders-0.5.5/mavlink/AVSSUAS/mavlink_msg_avss_drone_imu.h` & `UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_drone_imu.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/AVSSUAS/mavlink_msg_avss_drone_operation_mode.h` & `UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_drone_operation_mode.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/AVSSUAS/mavlink_msg_avss_drone_position.h` & `UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_drone_position.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/AVSSUAS/mavlink_msg_avss_prs_sys_status.h` & `UAVReaders-0.5.6/mavlink/AVSSUAS/mavlink_msg_avss_prs_sys_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/AVSSUAS/testsuite.h` & `UAVReaders-0.5.6/mavlink/AVSSUAS/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/all/all.h` & `UAVReaders-0.5.6/mavlink/all/all.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_ALL_H
 #define MAVLINK_ALL_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_ALL.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_ALL_XML_HASH -7193503605551725936
+#define MAVLINK_ALL_XML_HASH 176630288810012530
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink/all/mavlink.h` & `UAVReaders-0.5.6/mavlink/common/mavlink.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from all.xml
+ *  @brief MAVLink comm protocol built from common.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH -7193503605551725936
+#define MAVLINK_PRIMARY_XML_HASH 5515211591480474682
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "all.h"
+#include "common.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.5/mavlink/all/testsuite.h` & `UAVReaders-0.5.6/mavlink/all/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/ardupilotmega.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/ardupilotmega.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_ARDUPILOTMEGA_H
 #define MAVLINK_ARDUPILOTMEGA_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_ARDUPILOTMEGA.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_ARDUPILOTMEGA_XML_HASH -6579536692444572412
+#define MAVLINK_ARDUPILOTMEGA_XML_HASH -6398486276474170115
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink.h`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  *  @brief MAVLink comm protocol built from ardupilotmega.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH -6579536692444572412
+#define MAVLINK_PRIMARY_XML_HASH -6398486276474170115
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
```

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_adap_tuning.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_adap_tuning.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_ahrs.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ahrs.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_ahrs2.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ahrs2.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_ahrs3.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ahrs3.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_airspeed_autocal.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_airspeed_autocal.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_aoa_ssa.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_aoa_ssa.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_ap_adc.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ap_adc.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_autopilot_version_request.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_autopilot_version_request.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_battery2.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_battery2.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_camera_feedback.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_camera_feedback.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_camera_status.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_camera_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_compassmot_status.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_compassmot_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_data16.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data16.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_data32.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data32.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_data64.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data64.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_data96.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_data96.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_deepstall.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_deepstall.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_device_op_read.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_read.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_device_op_read_reply.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_read_reply.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_device_op_write.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_write.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_device_op_write_reply.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_device_op_write_reply.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_digicam_configure.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_digicam_configure.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_digicam_control.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_digicam_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_ekf_status_report.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_ekf_status_report.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_1_to_4.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_1_to_4.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_5_to_8.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_5_to_8.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_9_to_12.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_esc_telemetry_9_to_12.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_fence_fetch_point.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_fence_fetch_point.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_fence_point.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_fence_point.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gimbal_control.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gimbal_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gimbal_report.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gimbal_report.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gimbal_torque_cmd_report.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gimbal_torque_cmd_report.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gopro_get_request.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_get_request.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gopro_get_response.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_get_response.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gopro_heartbeat.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_heartbeat.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gopro_set_request.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_set_request.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_gopro_set_response.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_gopro_set_response.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_hwstatus.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_hwstatus.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_led_control.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_led_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_limits_status.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_limits_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_mag_cal_progress.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mag_cal_progress.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_mcu_status.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mcu_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_meminfo.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_meminfo.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_mount_configure.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mount_configure.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_mount_control.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mount_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_mount_status.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_mount_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_obstacle_distance_3d.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_obstacle_distance_3d.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_osd_param_config.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_config.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_osd_param_config_reply.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_config_reply.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config_reply.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_osd_param_show_config_reply.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_pid_tuning.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_pid_tuning.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_radio.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_radio.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_rally_fetch_point.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rally_fetch_point.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_rally_point.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rally_point.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_rangefinder.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rangefinder.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_remote_log_block_status.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_remote_log_block_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_remote_log_data_block.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_remote_log_data_block.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_rpm.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_rpm.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_sensor_offsets.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_sensor_offsets.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_set_mag_offsets.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_set_mag_offsets.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_simstate.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_simstate.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_vision_position_delta.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_vision_position_delta.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_water_depth.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_water_depth.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/mavlink_msg_wind.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/mavlink_msg_wind.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ardupilotmega/testsuite.h` & `UAVReaders-0.5.6/mavlink/ardupilotmega/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/checksum.h` & `UAVReaders-0.5.6/mavlink/checksum.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/common.h` & `UAVReaders-0.5.6/mavlink/common/common.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_COMMON_H
 #define MAVLINK_COMMON_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_COMMON.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_COMMON_XML_HASH 5897007811960217954
+#define MAVLINK_COMMON_XML_HASH 5515211591480474682
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink.h` & `UAVReaders-0.5.6/mavlink/cubepilot/mavlink.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from common.xml
+ *  @brief MAVLink comm protocol built from cubepilot.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 5897007811960217954
+#define MAVLINK_PRIMARY_XML_HASH 4348068059622669928
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "common.h"
+#include "cubepilot.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_actuator_control_target.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_actuator_control_target.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_actuator_output_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_actuator_output_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_adsb_vehicle.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_adsb_vehicle.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_ais_vessel.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_ais_vessel.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_altitude.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_altitude.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_att_pos_mocap.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_att_pos_mocap.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_attitude.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_attitude_quaternion.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude_quaternion.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_attitude_quaternion_cov.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude_quaternion_cov.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_attitude_target.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_attitude_target.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_auth_key.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_auth_key.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_autopilot_state_for_gimbal_device.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_autopilot_state_for_gimbal_device.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_autopilot_version.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_autopilot_version.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_battery_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_battery_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_button_change.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_button_change.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_capture_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_capture_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_fov_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_fov_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_image_captured.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_image_captured.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_information.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_settings.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_settings.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_tracking_geo_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_tracking_geo_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_tracking_image_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_tracking_image_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_camera_trigger.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_camera_trigger.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_can_filter_modify.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_can_filter_modify.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_can_frame.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_can_frame.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_canfd_frame.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_canfd_frame.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_cellular_config.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_cellular_config.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_cellular_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_cellular_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_change_operator_control.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_change_operator_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_change_operator_control_ack.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_change_operator_control_ack.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_collision.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_collision.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_command_ack.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_ack.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_command_cancel.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_cancel.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_command_int.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_command_long.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_command_long.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_component_information.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_component_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_component_metadata.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_component_metadata.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_control_system_state.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_control_system_state.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_current_event_sequence.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_current_event_sequence.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_data_stream.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_data_stream.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_data_transmission_handshake.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_data_transmission_handshake.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_debug.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_debug.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_debug_float_array.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_debug_float_array.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_debug_vect.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_debug_vect.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_distance_sensor.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_distance_sensor.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_efi_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_efi_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_encapsulated_data.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_encapsulated_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_esc_info.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_esc_info.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_esc_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_esc_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_estimator_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_estimator_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_event.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_event.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_extended_sys_state.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_extended_sys_state.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_fence_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_fence_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_file_transfer_protocol.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_file_transfer_protocol.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_flight_information.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_flight_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_follow_target.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_follow_target.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_generator_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_generator_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_device_attitude_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_device_attitude_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_device_information.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_device_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_device_set_attitude.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_device_set_attitude.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_manager_information.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_manager_set_attitude.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_set_attitude.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_manager_set_manual_control.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_set_manual_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_manager_set_pitchyaw.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_set_pitchyaw.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gimbal_manager_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gimbal_manager_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_global_position_int.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_global_position_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_global_position_int_cov.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_global_position_int_cov.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_global_vision_position_estimate.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_global_vision_position_estimate.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps2_raw.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps2_raw.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps2_rtk.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps2_rtk.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps_global_origin.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_global_origin.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps_inject_data.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_inject_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps_input.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_input.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps_raw_int.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_raw_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps_rtcm_data.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_rtcm_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps_rtk.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_rtk.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_gps_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_gps_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_high_latency.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_high_latency.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_high_latency2.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_high_latency2.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_highres_imu.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_highres_imu.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_actuator_controls.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_actuator_controls.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_controls.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_controls.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_gps.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_gps.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_optical_flow.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_optical_flow.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_rc_inputs_raw.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_rc_inputs_raw.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_sensor.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_sensor.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_state.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_state.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_hil_state_quaternion.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hil_state_quaternion.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_home_position.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_home_position.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_hygrometer_sensor.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_hygrometer_sensor.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_isbd_link_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_isbd_link_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_landing_target.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_landing_target.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_link_node_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_link_node_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_local_position_ned.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_local_position_ned.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_local_position_ned_cov.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_local_position_ned_cov.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_local_position_ned_system_global_offset.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_local_position_ned_system_global_offset.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_log_data.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_log_entry.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_entry.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_log_erase.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_erase.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_log_request_data.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_request_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_log_request_end.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_request_end.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_log_request_list.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_log_request_list.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_logging_ack.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_logging_ack.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_logging_data.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_logging_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_logging_data_acked.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_logging_data_acked.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mag_cal_report.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mag_cal_report.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_manual_control.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_manual_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_manual_setpoint.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_manual_setpoint.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_memory_vect.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_memory_vect.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_message_interval.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_message_interval.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_ack.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_ack.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_clear_all.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_clear_all.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_count.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_count.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_current.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_current.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_item.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_item.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_item_int.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_item_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_item_reached.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_item_reached.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_request.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_request_int.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_request_list.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request_list.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_request_partial_list.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_request_partial_list.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_set_current.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_set_current.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mission_write_partial_list.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mission_write_partial_list.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_mount_orientation.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_mount_orientation.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_named_value_float.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_named_value_float.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_named_value_int.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_named_value_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_nav_controller_output.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_nav_controller_output.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_obstacle_distance.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_obstacle_distance.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_odometry.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_odometry.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_onboard_computer_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_onboard_computer_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_arm_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_arm_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_authentication.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_authentication.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_basic_id.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_basic_id.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_location.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_location.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_message_pack.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_message_pack.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_operator_id.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_operator_id.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_self_id.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_self_id.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_system.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_system.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_open_drone_id_system_update.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_open_drone_id_system_update.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_optical_flow.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_optical_flow.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_optical_flow_rad.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_optical_flow_rad.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_orbit_execution_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_orbit_execution_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_ext_ack.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_ack.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_ext_request_list.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_request_list.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_ext_request_read.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_request_read.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_ext_set.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_set.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_ext_value.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_ext_value.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_map_rc.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_map_rc.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_request_list.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_request_list.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_request_read.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_request_read.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_set.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_set.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_param_value.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_param_value.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_ping.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_ping.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_play_tune.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_play_tune.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_play_tune_v2.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_play_tune_v2.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_position_target_global_int.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_position_target_global_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_position_target_local_ned.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_position_target_local_ned.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_power_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_power_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_radio_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_radio_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_raw_imu.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_raw_imu.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_raw_pressure.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_raw_pressure.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_raw_rpm.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_raw_rpm.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_rc_channels.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_rc_channels_override.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels_override.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_rc_channels_raw.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels_raw.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_rc_channels_scaled.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_rc_channels_scaled.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_request_data_stream.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_request_data_stream.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_request_event.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_request_event.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_resource_request.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_resource_request.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_response_event_error.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_response_event_error.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_safety_allowed_area.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_safety_allowed_area.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_safety_set_allowed_area.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_safety_set_allowed_area.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_scaled_imu.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_imu.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_scaled_imu2.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_imu2.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_scaled_imu3.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_imu3.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_scaled_pressure.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_pressure.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_scaled_pressure2.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_pressure2.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_scaled_pressure3.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_scaled_pressure3.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_serial_control.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_serial_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_servo_output_raw.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_servo_output_raw.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_set_actuator_control_target.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_actuator_control_target.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_set_attitude_target.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_attitude_target.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_set_gps_global_origin.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_gps_global_origin.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_set_home_position.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_home_position.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_set_mode.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_mode.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_set_position_target_global_int.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_position_target_global_int.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_set_position_target_local_ned.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_set_position_target_local_ned.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_setup_signing.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_setup_signing.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_sim_state.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_sim_state.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_smart_battery_info.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_smart_battery_info.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_statustext.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_statustext.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_storage_information.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_storage_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_supported_tunes.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_supported_tunes.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_sys_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_sys_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_system_time.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_system_time.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_terrain_check.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_check.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_terrain_data.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_data.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_terrain_report.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_report.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_terrain_request.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_terrain_request.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_time_estimate_to_target.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_time_estimate_to_target.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_timesync.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_timesync.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_trajectory_representation_bezier.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_trajectory_representation_bezier.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_trajectory_representation_waypoints.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_trajectory_representation_waypoints.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_tunnel.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_tunnel.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_uavcan_node_info.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_uavcan_node_info.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_uavcan_node_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_uavcan_node_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_utm_global_position.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_utm_global_position.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_v2_extension.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_v2_extension.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_vfr_hud.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_vfr_hud.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_vibration.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_vibration.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_vicon_position_estimate.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_vicon_position_estimate.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_video_stream_information.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_video_stream_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_video_stream_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_video_stream_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_vision_position_estimate.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_vision_position_estimate.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_vision_speed_estimate.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_vision_speed_estimate.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_wheel_distance.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_wheel_distance.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_wifi_config_ap.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_wifi_config_ap.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_winch_status.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_winch_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/mavlink_msg_wind_cov.h` & `UAVReaders-0.5.6/mavlink/common/mavlink_msg_wind_cov.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/common/testsuite.h` & `UAVReaders-0.5.6/mavlink/common/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/cubepilot/cubepilot.h` & `UAVReaders-0.5.6/mavlink/cubepilot/cubepilot.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_CUBEPILOT_H
 #define MAVLINK_CUBEPILOT_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_CUBEPILOT.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_CUBEPILOT_XML_HASH -4835210297432656092
+#define MAVLINK_CUBEPILOT_XML_HASH 4348068059622669928
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink/cubepilot/mavlink.h` & `UAVReaders-0.5.6/mavlink/all/mavlink.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from cubepilot.xml
+ *  @brief MAVLink comm protocol built from all.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH -4835210297432656092
+#define MAVLINK_PRIMARY_XML_HASH 176630288810012530
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "cubepilot.h"
+#include "all.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.5/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_resp.h` & `UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_resp.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_start.h` & `UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_cubepilot_firmware_update_start.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/cubepilot/mavlink_msg_cubepilot_raw_rc.h` & `UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_cubepilot_raw_rc.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/cubepilot/mavlink_msg_herelink_telem.h` & `UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_herelink_telem.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/cubepilot/mavlink_msg_herelink_video_stream_information.h` & `UAVReaders-0.5.6/mavlink/cubepilot/mavlink_msg_herelink_video_stream_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/cubepilot/testsuite.h` & `UAVReaders-0.5.6/mavlink/cubepilot/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/development/development.h` & `UAVReaders-0.5.6/mavlink/development/development.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_DEVELOPMENT_H
 #define MAVLINK_DEVELOPMENT_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_DEVELOPMENT.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_DEVELOPMENT_XML_HASH -8595811904465569702
+#define MAVLINK_DEVELOPMENT_XML_HASH -4303497761705237489
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink/development/mavlink.h` & `UAVReaders-0.5.6/mavlink/uAvionix/mavlink.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from development.xml
+ *  @brief MAVLink comm protocol built from uAvionix.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH -8595811904465569702
+#define MAVLINK_PRIMARY_XML_HASH -7924362279646143647
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "development.h"
+#include "uAvionix.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.5/mavlink/development/mavlink_msg_airspeed.h` & `UAVReaders-0.5.6/mavlink/development/mavlink_msg_airspeed.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/development/mavlink_msg_available_modes.h` & `UAVReaders-0.5.6/mavlink/development/mavlink_msg_available_modes.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/development/mavlink_msg_battery_status_v2.h` & `UAVReaders-0.5.6/mavlink/development/mavlink_msg_battery_status_v2.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/development/mavlink_msg_component_information_basic.h` & `UAVReaders-0.5.6/mavlink/development/mavlink_msg_component_information_basic.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/development/mavlink_msg_current_mode.h` & `UAVReaders-0.5.6/mavlink/development/mavlink_msg_current_mode.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/development/mavlink_msg_figure_eight_execution_status.h` & `UAVReaders-0.5.6/mavlink/development/mavlink_msg_figure_eight_execution_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/development/mavlink_msg_group_end.h` & `UAVReaders-0.5.6/mavlink/development/mavlink_msg_group_end.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/development/mavlink_msg_group_start.h` & `UAVReaders-0.5.6/mavlink/development/mavlink_msg_group_start.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/development/mavlink_msg_mission_checksum.h` & `UAVReaders-0.5.6/mavlink/development/mavlink_msg_mission_checksum.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/development/mavlink_msg_param_ack_transaction.h` & `UAVReaders-0.5.6/mavlink/development/mavlink_msg_param_ack_transaction.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/development/mavlink_msg_target_absolute.h` & `UAVReaders-0.5.6/mavlink/development/mavlink_msg_target_absolute.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/development/mavlink_msg_target_relative.h` & `UAVReaders-0.5.6/mavlink/development/mavlink_msg_target_relative.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/development/mavlink_msg_wifi_network_info.h` & `UAVReaders-0.5.6/mavlink/development/mavlink_msg_wifi_network_info.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/development/testsuite.h` & `UAVReaders-0.5.6/mavlink/development/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/icarous/icarous.h` & `UAVReaders-0.5.6/mavlink/icarous/icarous.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_ICAROUS_H
 #define MAVLINK_ICAROUS_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_ICAROUS.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_ICAROUS_XML_HASH 835520520414605293
+#define MAVLINK_ICAROUS_XML_HASH 2245595000028289331
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink/icarous/mavlink.h` & `UAVReaders-0.5.6/mavlink/icarous/mavlink.h`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  *  @brief MAVLink comm protocol built from icarous.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 835520520414605293
+#define MAVLINK_PRIMARY_XML_HASH 2245595000028289331
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
```

### Comparing `UAVReaders-0.5.5/mavlink/icarous/mavlink_msg_icarous_heartbeat.h` & `UAVReaders-0.5.6/mavlink/icarous/mavlink_msg_icarous_heartbeat.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/icarous/mavlink_msg_icarous_kinematic_bands.h` & `UAVReaders-0.5.6/mavlink/icarous/mavlink_msg_icarous_kinematic_bands.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/icarous/testsuite.h` & `UAVReaders-0.5.6/mavlink/icarous/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/mavlink_conversions.h` & `UAVReaders-0.5.6/mavlink/mavlink_conversions.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/mavlink_get_info.h` & `UAVReaders-0.5.6/mavlink/mavlink_get_info.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/mavlink_helpers.h` & `UAVReaders-0.5.6/mavlink/mavlink_helpers.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/mavlink_sha256.h` & `UAVReaders-0.5.6/mavlink/mavlink_sha256.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/mavlink_types.h` & `UAVReaders-0.5.6/mavlink/mavlink_types.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/minimal/mavlink.h` & `UAVReaders-0.5.6/mavlink/minimal/mavlink.h`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  *  @brief MAVLink comm protocol built from minimal.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 2061057795176385022
+#define MAVLINK_PRIMARY_XML_HASH -8787493283418306967
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
```

### Comparing `UAVReaders-0.5.5/mavlink/minimal/mavlink_msg_heartbeat.h` & `UAVReaders-0.5.6/mavlink/minimal/mavlink_msg_heartbeat.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/minimal/mavlink_msg_protocol_version.h` & `UAVReaders-0.5.6/mavlink/minimal/mavlink_msg_protocol_version.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/minimal/minimal.h` & `UAVReaders-0.5.6/mavlink/minimal/minimal.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_MINIMAL_H
 #define MAVLINK_MINIMAL_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_MINIMAL.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_MINIMAL_XML_HASH 2061057795176385022
+#define MAVLINK_MINIMAL_XML_HASH -8787493283418306967
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink/minimal/testsuite.h` & `UAVReaders-0.5.6/mavlink/minimal/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/protocol.h` & `UAVReaders-0.5.6/mavlink/protocol.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/python_array_test/mavlink.h` & `UAVReaders-0.5.6/mavlink/python_array_test/mavlink.h`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  *  @brief MAVLink comm protocol built from python_array_test.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 2237550671766149370
+#define MAVLINK_PRIMARY_XML_HASH 1341603429249984703
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
```

### Comparing `UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_0.h` & `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_0.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_1.h` & `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_1.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_3.h` & `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_3.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_4.h` & `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_4.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_5.h` & `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_5.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_6.h` & `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_6.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_7.h` & `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_7.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/python_array_test/mavlink_msg_array_test_8.h` & `UAVReaders-0.5.6/mavlink/python_array_test/mavlink_msg_array_test_8.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/python_array_test/python_array_test.h` & `UAVReaders-0.5.6/mavlink/python_array_test/python_array_test.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_PYTHON_ARRAY_TEST_H
 #define MAVLINK_PYTHON_ARRAY_TEST_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_PYTHON_ARRAY_TEST.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_PYTHON_ARRAY_TEST_XML_HASH 2237550671766149370
+#define MAVLINK_PYTHON_ARRAY_TEST_XML_HASH 1341603429249984703
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink/python_array_test/testsuite.h` & `UAVReaders-0.5.6/mavlink/python_array_test/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/standard/mavlink.h` & `UAVReaders-0.5.6/mavlink/standard/mavlink.h`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  *  @brief MAVLink comm protocol built from standard.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 8119739704804190533
+#define MAVLINK_PRIMARY_XML_HASH -8068599972875758283
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
```

### Comparing `UAVReaders-0.5.5/mavlink/standard/standard.h` & `UAVReaders-0.5.6/mavlink/standard/standard.h`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_STANDARD_H
 #define MAVLINK_STANDARD_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_STANDARD.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_STANDARD_XML_HASH 8119739704804190533
+#define MAVLINK_STANDARD_XML_HASH -8068599972875758283
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink/standard/testsuite.h` & `UAVReaders-0.5.6/mavlink/standard/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/storm32/mavlink.h` & `UAVReaders-0.5.6/mavlink/ualberta/mavlink.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from storm32.xml
+ *  @brief MAVLink comm protocol built from ualberta.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 4202825066288420751
+#define MAVLINK_PRIMARY_XML_HASH -8458791220127004858
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "storm32.h"
+#include "ualberta.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_frsky_passthrough_array.h` & `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_frsky_passthrough_array.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_param_value_array.h` & `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_param_value_array.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_qshot_status.h` & `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_qshot_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_radio_link_stats.h` & `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_radio_link_stats.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_radio_rc_channels.h` & `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_radio_rc_channels.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control.h` & `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control_pitchyaw.h` & `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_control_pitchyaw.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_correct_roll.h` & `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_correct_roll.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_information.h` & `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_information.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_status.h` & `UAVReaders-0.5.6/mavlink/storm32/mavlink_msg_storm32_gimbal_manager_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/storm32/storm32.h` & `UAVReaders-0.5.6/mavlink/storm32/storm32.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_STORM32_H
 #define MAVLINK_STORM32_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_STORM32.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_STORM32_XML_HASH 4202825066288420751
+#define MAVLINK_STORM32_XML_HASH -4905212276485218532
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink/storm32/testsuite.h` & `UAVReaders-0.5.6/mavlink/storm32/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/test/mavlink.h` & `UAVReaders-0.5.6/mavlink/development/mavlink.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from test.xml
+ *  @brief MAVLink comm protocol built from development.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 8652858642551673461
+#define MAVLINK_PRIMARY_XML_HASH -4303497761705237489
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "test.h"
+#include "development.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.5/mavlink/test/mavlink_msg_test_types.h` & `UAVReaders-0.5.6/mavlink/test/mavlink_msg_test_types.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/test/test.h` & `UAVReaders-0.5.6/mavlink/test/test.h`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_TEST_H
 #define MAVLINK_TEST_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_TEST.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_TEST_XML_HASH 8652858642551673461
+#define MAVLINK_TEST_XML_HASH -5416981559095984788
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink/test/testsuite.h` & `UAVReaders-0.5.6/mavlink/test/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/uAvionix/mavlink.h` & `UAVReaders-0.5.6/mavlink/ASLUAV/mavlink.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from uAvionix.xml
+ *  @brief MAVLink comm protocol built from ASLUAV.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 5763353043744799234
+#define MAVLINK_PRIMARY_XML_HASH -6921207667047634836
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "uAvionix.h"
+#include "ASLUAV.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.5/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_cfg.h` & `UAVReaders-0.5.6/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_cfg.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_dynamic.h` & `UAVReaders-0.5.6/mavlink/uAvionix/mavlink_msg_uavionix_adsb_out_dynamic.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/uAvionix/mavlink_msg_uavionix_adsb_transceiver_health_report.h` & `UAVReaders-0.5.6/mavlink/uAvionix/mavlink_msg_uavionix_adsb_transceiver_health_report.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/uAvionix/testsuite.h` & `UAVReaders-0.5.6/mavlink/uAvionix/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/uAvionix/uAvionix.h` & `UAVReaders-0.5.6/mavlink/uAvionix/uAvionix.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_UAVIONIX_H
 #define MAVLINK_UAVIONIX_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_UAVIONIX.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_UAVIONIX_XML_HASH 5763353043744799234
+#define MAVLINK_UAVIONIX_XML_HASH -7924362279646143647
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink/ualberta/mavlink.h` & `UAVReaders-0.5.6/mavlink/storm32/mavlink.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 /** @file
- *  @brief MAVLink comm protocol built from ualberta.xml
+ *  @brief MAVLink comm protocol built from storm32.xml
  *  @see http://mavlink.org
  */
 #pragma once
 #ifndef MAVLINK_H
 #define MAVLINK_H
 
-#define MAVLINK_PRIMARY_XML_HASH 2505511056242801877
+#define MAVLINK_PRIMARY_XML_HASH -4905212276485218532
 
 #ifndef MAVLINK_STX
 #define MAVLINK_STX 253
 #endif
 
 #ifndef MAVLINK_ENDIAN
 #define MAVLINK_ENDIAN MAVLINK_LITTLE_ENDIAN
@@ -25,10 +25,10 @@
 #endif
 
 #ifndef MAVLINK_COMMAND_24BIT
 #define MAVLINK_COMMAND_24BIT 1
 #endif
 
 #include "version.h"
-#include "ualberta.h"
+#include "storm32.h"
 
 #endif // MAVLINK_H
```

### Comparing `UAVReaders-0.5.5/mavlink/ualberta/mavlink_msg_nav_filter_bias.h` & `UAVReaders-0.5.6/mavlink/ualberta/mavlink_msg_nav_filter_bias.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ualberta/mavlink_msg_radio_calibration.h` & `UAVReaders-0.5.6/mavlink/ualberta/mavlink_msg_radio_calibration.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ualberta/mavlink_msg_ualberta_sys_status.h` & `UAVReaders-0.5.6/mavlink/ualberta/mavlink_msg_ualberta_sys_status.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ualberta/testsuite.h` & `UAVReaders-0.5.6/mavlink/ualberta/testsuite.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/mavlink/ualberta/ualberta.h` & `UAVReaders-0.5.6/mavlink/ualberta/ualberta.h`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #ifndef MAVLINK_UALBERTA_H
 #define MAVLINK_UALBERTA_H
 
 #ifndef MAVLINK_H
     #error Wrong include order: MAVLINK_UALBERTA.H MUST NOT BE DIRECTLY USED. Include mavlink.h from the same directory instead or set ALL AND EVERY defines from MAVLINK.H manually accordingly, including the #define MAVLINK_H call.
 #endif
 
-#define MAVLINK_UALBERTA_XML_HASH 2505511056242801877
+#define MAVLINK_UALBERTA_XML_HASH -8458791220127004858
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // MESSAGE LENGTHS AND CRCS
```

### Comparing `UAVReaders-0.5.5/mavlink_introspect_gen.c` & `UAVReaders-0.5.6/mavlink_introspect_gen.c`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-#include "mavlink/AVSSUAS/mavlink.h"
-#include "mavlink/ardupilotmega/mavlink.h"
-#include "mavlink/cubepilot/mavlink.h"
-#include "mavlink/test/mavlink.h"
-#include "mavlink/minimal/mavlink.h"
-#include "mavlink/python_array_test/mavlink.h"
-#include "mavlink/icarous/mavlink.h"
 #include "mavlink/ualberta/mavlink.h"
+#include "mavlink/development/mavlink.h"
+#include "mavlink/storm32/mavlink.h"
+#include "mavlink/icarous/mavlink.h"
+#include "mavlink/minimal/mavlink.h"
+#include "mavlink/ardupilotmega/mavlink.h"
 #include "mavlink/uAvionix/mavlink.h"
+#include "mavlink/AVSSUAS/mavlink.h"
+#include "mavlink/python_array_test/mavlink.h"
 #include "mavlink/ASLUAV/mavlink.h"
 #include "mavlink/common/mavlink.h"
-#include "mavlink/storm32/mavlink.h"
-#include "mavlink/development/mavlink.h"
+#include "mavlink/cubepilot/mavlink.h"
+#include "mavlink/test/mavlink.h"
 #include "mavlink/development/mavlink_msg_wifi_network_info.h"
 #include "mavlink/development/mavlink_msg_target_absolute.h"
 #include "mavlink/development/mavlink_msg_current_mode.h"
 #include "mavlink/development/mavlink_msg_battery_status_v2.h"
 #include "mavlink/development/mavlink_msg_group_start.h"
 #include "mavlink/development/mavlink_msg_figure_eight_execution_status.h"
 #include "mavlink/development/mavlink_msg_group_end.h"
```

### Comparing `UAVReaders-0.5.5/mavlink_introspect_gen.h` & `UAVReaders-0.5.6/mavlink_introspect_gen.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/pyinterop.cpp` & `UAVReaders-0.5.6/pyinterop.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -748,16 +748,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__UAVReaders__pyinterop
-#define __PYX_HAVE_API__UAVReaders__pyinterop
+#define __PYX_HAVE__UAVReaders
+#define __PYX_HAVE_API__UAVReaders
 /* Early includes */
 #include <string.h>
 #include <string>
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
@@ -1087,133 +1087,133 @@
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
 /*--- Type declarations ---*/
-struct __pyx_obj_10UAVReaders_9pyinterop_packet;
-struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader;
-struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader;
-struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable;
-struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile;
-struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__;
-struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__;
+struct __pyx_obj_10UAVReaders_packet;
+struct __pyx_obj_10UAVReaders_mavlink_reader;
+struct __pyx_obj_10UAVReaders_data_flash_reader;
+struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable;
+struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile;
+struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__;
+struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "UAVReaders/pyinterop.pyx":213
+/* "pyinterop.pyx":213
  *     return name, pyObj
  * 
  * cdef class packet(dict):             # <<<<<<<<<<<<<<
  *     """
  *     A class representing a packet.
  */
-struct __pyx_obj_10UAVReaders_9pyinterop_packet {
+struct __pyx_obj_10UAVReaders_packet {
   PyDictObject __pyx_base;
-  struct __pyx_vtabstruct_10UAVReaders_9pyinterop_packet *__pyx_vtab;
+  struct __pyx_vtabstruct_10UAVReaders_packet *__pyx_vtab;
   PyObject *name;
   PyObject *protocol;
   int packet_type;
 };
 
 
-/* "UAVReaders/pyinterop.pyx":283
+/* "pyinterop.pyx":283
  *         return readFile
  * 
  * cdef class mavlink_reader:             # <<<<<<<<<<<<<<
  *     """
  *     Parser for DataFlash .bin files.
  */
-struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader {
+struct __pyx_obj_10UAVReaders_mavlink_reader {
   PyObject_HEAD
   UAVFormatReaders::mavLinkReader *reader;
   PyObject *gen;
 };
 
 
-/* "UAVReaders/pyinterop.pyx":344
+/* "pyinterop.pyx":344
  *                 yield p
  * 
  * cdef class data_flash_reader:             # <<<<<<<<<<<<<<
  *     """
  *     Parser for DataFlash .bin files.
  */
-struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader {
+struct __pyx_obj_10UAVReaders_data_flash_reader {
   PyObject_HEAD
   UAVFormatReaders::dataFlashReader *reader;
   PyObject *gen;
 };
 
 
-/* "UAVReaders/pyinterop.pyx":259
+/* "pyinterop.pyx":259
  *         return self.packet_type
  * 
  * def thing_to_iterable(thing):             # <<<<<<<<<<<<<<
  *     """
  *     Converts certain python objects into
  */
-struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable {
+struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable {
   PyObject_HEAD
   PyObject *__pyx_v_thing;
 };
 
 
-/* "UAVReaders/pyinterop.pyx":274
+/* "pyinterop.pyx":274
  *         return thing
  *     elif type(thing) == str:
  *         def readFile():             # <<<<<<<<<<<<<<
  *             with open(thing, "rb") as f:
  *                 data = f.read(512)
  */
-struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile {
+struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile {
   PyObject_HEAD
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable *__pyx_outer_scope;
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable *__pyx_outer_scope;
   PyObject *__pyx_v_data;
   PyObject *__pyx_v_f;
   PyObject *__pyx_t_0;
   PyObject *__pyx_t_1;
   PyObject *__pyx_t_2;
   PyObject *__pyx_t_3;
 };
 
 
-/* "UAVReaders/pyinterop.pyx":335
+/* "pyinterop.pyx":335
  *             return None
  * 
  *     def __call__(self):             # <<<<<<<<<<<<<<
  *         for thing in self.gen():
  *             self.parseBuffer(thing)
  */
-struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ {
+struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__ {
   PyObject_HEAD
-  struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_p;
+  struct __pyx_obj_10UAVReaders_packet *__pyx_v_p;
   introspect::Struct *__pyx_v_s;
-  struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self;
+  struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self;
   PyObject *__pyx_v_thing;
   PyObject *__pyx_t_0;
   Py_ssize_t __pyx_t_1;
   PyObject *(*__pyx_t_2)(PyObject *);
 };
 
 
-/* "UAVReaders/pyinterop.pyx":396
+/* "pyinterop.pyx":396
  *             return None
  * 
  *     def __call__(self):             # <<<<<<<<<<<<<<
  *         for thing in self.gen():
  *             self.parseBuffer(thing)
  */
-struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ {
+struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__ {
   PyObject_HEAD
-  struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_p;
+  struct __pyx_obj_10UAVReaders_packet *__pyx_v_p;
   introspect::Struct *__pyx_v_s;
-  struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self;
+  struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self;
   PyObject *__pyx_v_thing;
   PyObject *__pyx_t_0;
   Py_ssize_t __pyx_t_1;
   PyObject *(*__pyx_t_2)(PyObject *);
 };
 
 
@@ -1291,26 +1291,26 @@
   PyObject *from_object;
   PyObject *(*to_object_func)(char *);
   int (*to_dtype_func)(char *, PyObject *);
 };
 
 
 
-/* "UAVReaders/pyinterop.pyx":213
+/* "pyinterop.pyx":213
  *     return name, pyObj
  * 
  * cdef class packet(dict):             # <<<<<<<<<<<<<<
  *     """
  *     A class representing a packet.
  */
 
-struct __pyx_vtabstruct_10UAVReaders_9pyinterop_packet {
-  PyObject *(*secret_real_init)(struct __pyx_obj_10UAVReaders_9pyinterop_packet *, introspect::Struct *, std::string);
+struct __pyx_vtabstruct_10UAVReaders_packet {
+  PyObject *(*secret_real_init)(struct __pyx_obj_10UAVReaders_packet *, introspect::Struct *, std::string);
 };
-static struct __pyx_vtabstruct_10UAVReaders_9pyinterop_packet *__pyx_vtabptr_10UAVReaders_9pyinterop_packet;
+static struct __pyx_vtabstruct_10UAVReaders_packet *__pyx_vtabptr_10UAVReaders_packet;
 
 
 /* "View.MemoryView":106
  * 
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
@@ -2288,15 +2288,15 @@
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
-static PyObject *__pyx_f_10UAVReaders_9pyinterop_6packet_secret_real_init(struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_self, introspect::Struct *__pyx_v_ptr, std::string __pyx_v_proto); /* proto*/
+static PyObject *__pyx_f_10UAVReaders_6packet_secret_real_init(struct __pyx_obj_10UAVReaders_packet *__pyx_v_self, introspect::Struct *__pyx_v_ptr, std::string __pyx_v_proto); /* proto*/
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self); /* proto*/
 static char *__pyx_memoryview_get_item_pointer(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index); /* proto*/
 static PyObject *__pyx_memoryview_is_slice(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_obj); /* proto*/
 static PyObject *__pyx_memoryview_setitem_slice_assignment(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_dst, PyObject *__pyx_v_src); /* proto*/
 static PyObject *__pyx_memoryview_setitem_slice_assign_scalar(struct __pyx_memoryview_obj *__pyx_v_self, struct __pyx_memoryview_obj *__pyx_v_dst, PyObject *__pyx_v_value); /* proto*/
 static PyObject *__pyx_memoryview_setitem_indexed(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_value); /* proto*/
 static PyObject *__pyx_memoryview_convert_item_to_object(struct __pyx_memoryview_obj *__pyx_v_self, char *__pyx_v_itemp); /* proto*/
@@ -2312,36 +2312,36 @@
 
 /* Module declarations from 'cython.view' */
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'libc' */
 
-/* Module declarations from 'UAVReaders.pyinterop' */
-static PyTypeObject *__pyx_ptype_10UAVReaders_9pyinterop_packet = 0;
-static PyTypeObject *__pyx_ptype_10UAVReaders_9pyinterop_mavlink_reader = 0;
-static PyTypeObject *__pyx_ptype_10UAVReaders_9pyinterop_data_flash_reader = 0;
-static PyTypeObject *__pyx_ptype_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable = 0;
-static PyTypeObject *__pyx_ptype_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile = 0;
-static PyTypeObject *__pyx_ptype_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ = 0;
-static PyTypeObject *__pyx_ptype_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ = 0;
+/* Module declarations from 'UAVReaders' */
+static PyTypeObject *__pyx_ptype_10UAVReaders_packet = 0;
+static PyTypeObject *__pyx_ptype_10UAVReaders_mavlink_reader = 0;
+static PyTypeObject *__pyx_ptype_10UAVReaders_data_flash_reader = 0;
+static PyTypeObject *__pyx_ptype_10UAVReaders___pyx_scope_struct__thing_to_iterable = 0;
+static PyTypeObject *__pyx_ptype_10UAVReaders___pyx_scope_struct_1_readFile = 0;
+static PyTypeObject *__pyx_ptype_10UAVReaders___pyx_scope_struct_2___call__ = 0;
+static PyTypeObject *__pyx_ptype_10UAVReaders___pyx_scope_struct_3___call__ = 0;
 static PyTypeObject *__pyx_array_type = 0;
 static PyTypeObject *__pyx_MemviewEnum_type = 0;
 static PyTypeObject *__pyx_memoryview_type = 0;
 static PyTypeObject *__pyx_memoryviewslice_type = 0;
 static PyObject *generic = 0;
 static PyObject *strided = 0;
 static PyObject *indirect = 0;
 static PyObject *contiguous = 0;
 static PyObject *indirect_contiguous = 0;
 static int __pyx_memoryview_thread_locks_used;
 static PyThread_type_lock __pyx_memoryview_thread_locks[8];
-static PyObject *__pyx_f_10UAVReaders_9pyinterop_cppToPyStr(std::string); /*proto*/
-static PyObject *__pyx_f_10UAVReaders_9pyinterop_voidToPython(void *, cType, size_t); /*proto*/
-static PyObject *__pyx_f_10UAVReaders_9pyinterop_memberToPy(introspect::abstractStructMember *); /*proto*/
+static PyObject *__pyx_f_10UAVReaders_cppToPyStr(std::string); /*proto*/
+static PyObject *__pyx_f_10UAVReaders_voidToPython(void *, cType, size_t); /*proto*/
+static PyObject *__pyx_f_10UAVReaders_memberToPy(introspect::abstractStructMember *); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &); /*proto*/
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
 static struct __pyx_array_obj *__pyx_array_new(PyObject *, Py_ssize_t, char *, char *, char *); /*proto*/
@@ -2374,19 +2374,19 @@
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *, int, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn_uint8_t__const__ = { "const uint8_t", NULL, sizeof(uint8_t const ), { 0 }, 0, IS_UNSIGNED(uint8_t const ) ? 'U' : 'I', IS_UNSIGNED(uint8_t const ), 0 };
-#define __Pyx_MODULE_NAME "UAVReaders.pyinterop"
-extern int __pyx_module_is_main_UAVReaders__pyinterop;
-int __pyx_module_is_main_UAVReaders__pyinterop = 0;
+#define __Pyx_MODULE_NAME "UAVReaders"
+extern int __pyx_module_is_main_UAVReaders;
+int __pyx_module_is_main_UAVReaders = 0;
 
-/* Implementation of 'UAVReaders.pyinterop' */
+/* Implementation of 'UAVReaders' */
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_UnicodeDecodeError;
 static PyObject *__pyx_builtin_chr;
 static PyObject *__pyx_builtin_super;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_open;
 static PyObject *__pyx_builtin_ValueError;
@@ -2459,14 +2459,15 @@
 static const char __pyx_k_readFile[] = "readFile";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_IndexError[] = "IndexError";
+static const char __pyx_k_UAVReaders[] = "UAVReaders";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_data_flash[] = "data_flash";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_parseBuffer[] = "parseBuffer";
@@ -2483,15 +2484,14 @@
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_data_flash_reader[] = "data_flash_reader";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_thing_to_iterable[] = "thing_to_iterable";
 static const char __pyx_k_UnicodeDecodeError[] = "UnicodeDecodeError";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_strided_and_direct[] = "<strided and direct>";
-static const char __pyx_k_UAVReaders_pyinterop[] = "UAVReaders.pyinterop";
 static const char __pyx_k_strided_and_indirect[] = "<strided and indirect>";
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
 static const char __pyx_k_mavlink_reader___call[] = "mavlink_reader.__call__";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
@@ -2532,15 +2532,15 @@
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
 static PyObject *__pyx_n_b_O;
 static PyObject *__pyx_kp_s_Out_of_bounds_on_buffer_access_a;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_TypeError;
-static PyObject *__pyx_n_s_UAVReaders_pyinterop;
+static PyObject *__pyx_n_s_UAVReaders;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_UnicodeDecodeError;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_append;
 static PyObject *__pyx_n_s_args;
@@ -2632,38 +2632,38 @@
 static PyObject *__pyx_n_s_thing_to_iterable_locals_readFil;
 static PyObject *__pyx_n_s_throw;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_kp_s_utf_8;
-static int __pyx_pf_10UAVReaders_9pyinterop_6packet___cinit__(struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_6packet_8protocol___get__(struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_6packet_4name___get__(struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_6packet_11packet_type___get__(struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_6packet_2__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_6packet_4__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_17thing_to_iterable_readFile(PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_thing_to_iterable(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_thing); /* proto */
-static int __pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader___cinit__(struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self, PyObject *__pyx_v_src); /* proto */
-static void __pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_2__dealloc__(struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_4parseByte(struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self, uint8_t __pyx_v_byte); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_6parseBuffer(struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self, __Pyx_memviewslice __pyx_v_bytes); /* proto */
-static struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_8get_packet(struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_10__call__(struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_13__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_15__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static int __pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader___cinit__(struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self, PyObject *__pyx_v_src); /* proto */
-static void __pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_2__dealloc__(struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_4parseByte(struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self, uint8_t __pyx_v_byte); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_6parseBuffer(struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self, __Pyx_memviewslice __pyx_v_bytes); /* proto */
-static struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_8get_packet(struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_10__call__(struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_13__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_15__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static int __pyx_pf_10UAVReaders_6packet___cinit__(struct __pyx_obj_10UAVReaders_packet *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_6packet_8protocol___get__(struct __pyx_obj_10UAVReaders_packet *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_6packet_4name___get__(struct __pyx_obj_10UAVReaders_packet *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_6packet_11packet_type___get__(struct __pyx_obj_10UAVReaders_packet *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_6packet_2__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_packet *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_6packet_4__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_packet *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_17thing_to_iterable_readFile(PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_thing_to_iterable(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_thing); /* proto */
+static int __pyx_pf_10UAVReaders_14mavlink_reader___cinit__(struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self, PyObject *__pyx_v_src); /* proto */
+static void __pyx_pf_10UAVReaders_14mavlink_reader_2__dealloc__(struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_14mavlink_reader_4parseByte(struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self, uint8_t __pyx_v_byte); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_14mavlink_reader_6parseBuffer(struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self, __Pyx_memviewslice __pyx_v_bytes); /* proto */
+static struct __pyx_obj_10UAVReaders_packet *__pyx_pf_10UAVReaders_14mavlink_reader_8get_packet(struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_14mavlink_reader_10__call__(struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_14mavlink_reader_13__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_14mavlink_reader_15__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static int __pyx_pf_10UAVReaders_17data_flash_reader___cinit__(struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self, PyObject *__pyx_v_src); /* proto */
+static void __pyx_pf_10UAVReaders_17data_flash_reader_2__dealloc__(struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_17data_flash_reader_4parseByte(struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self, uint8_t __pyx_v_byte); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_17data_flash_reader_6parseBuffer(struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self, __Pyx_memviewslice __pyx_v_bytes); /* proto */
+static struct __pyx_obj_10UAVReaders_packet *__pyx_pf_10UAVReaders_17data_flash_reader_8get_packet(struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_17data_flash_reader_10__call__(struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_17data_flash_reader_13__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10UAVReaders_17data_flash_reader_15__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -2698,21 +2698,21 @@
 static PyObject *__pyx_pf___pyx_memoryview___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryview_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_16_memoryviewslice_4base___get__(struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_tp_new_10UAVReaders_9pyinterop_packet(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_10UAVReaders_9pyinterop_mavlink_reader(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_10UAVReaders_9pyinterop_data_flash_reader(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_10UAVReaders_packet(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_10UAVReaders_mavlink_reader(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_10UAVReaders_data_flash_reader(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_10UAVReaders___pyx_scope_struct__thing_to_iterable(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_10UAVReaders___pyx_scope_struct_1_readFile(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_10UAVReaders___pyx_scope_struct_2___call__(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_10UAVReaders___pyx_scope_struct_3___call__(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_512;
@@ -2755,60 +2755,60 @@
 static PyObject *__pyx_tuple__36;
 static PyObject *__pyx_tuple__37;
 static PyObject *__pyx_codeobj__6;
 static PyObject *__pyx_codeobj__31;
 static PyObject *__pyx_codeobj__38;
 /* Late includes */
 
-/* "UAVReaders/pyinterop.pyx":18
+/* "pyinterop.pyx":18
  * from libcpp.string cimport string
  * 
  * cdef cppToPyStr(string cpp_string):             # <<<<<<<<<<<<<<
  *     # Get a pointer to the underlying C string using the c_str() method
  *     cdef const char* c_string_ptr = cpp_string.c_str()
  */
 
-static PyObject *__pyx_f_10UAVReaders_9pyinterop_cppToPyStr(std::string __pyx_v_cpp_string) {
+static PyObject *__pyx_f_10UAVReaders_cppToPyStr(std::string __pyx_v_cpp_string) {
   char const *__pyx_v_c_string_ptr;
   PyObject *__pyx_v_c_bytes = 0;
   PyObject *__pyx_v_a = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("cppToPyStr", 0);
 
-  /* "UAVReaders/pyinterop.pyx":20
+  /* "pyinterop.pyx":20
  * cdef cppToPyStr(string cpp_string):
  *     # Get a pointer to the underlying C string using the c_str() method
  *     cdef const char* c_string_ptr = cpp_string.c_str()             # <<<<<<<<<<<<<<
  * 
  *     # Convert the C string to a Python string by decoding the byte string using UTF-8 encoding
  */
   __pyx_v_c_string_ptr = __pyx_v_cpp_string.c_str();
 
-  /* "UAVReaders/pyinterop.pyx":23
+  /* "pyinterop.pyx":23
  * 
  *     # Convert the C string to a Python string by decoding the byte string using UTF-8 encoding
  *     cdef bytes c_bytes = <bytes>c_string_ptr             # <<<<<<<<<<<<<<
  *     a = c_bytes.decode('utf-8')
  *     return a
  */
   __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_c_string_ptr); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __pyx_t_1;
   __Pyx_INCREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_c_bytes = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "UAVReaders/pyinterop.pyx":24
+  /* "pyinterop.pyx":24
  *     # Convert the C string to a Python string by decoding the byte string using UTF-8 encoding
  *     cdef bytes c_bytes = <bytes>c_string_ptr
  *     a = c_bytes.decode('utf-8')             # <<<<<<<<<<<<<<
  *     return a
  * 
  */
   if (unlikely(__pyx_v_c_bytes == Py_None)) {
@@ -2816,57 +2816,57 @@
     __PYX_ERR(0, 24, __pyx_L1_error)
   }
   __pyx_t_2 = __Pyx_decode_bytes(__pyx_v_c_bytes, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_a = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "UAVReaders/pyinterop.pyx":25
+  /* "pyinterop.pyx":25
  *     cdef bytes c_bytes = <bytes>c_string_ptr
  *     a = c_bytes.decode('utf-8')
  *     return a             # <<<<<<<<<<<<<<
  * 
  * cimport libc.string
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_a);
   __pyx_r = __pyx_v_a;
   goto __pyx_L0;
 
-  /* "UAVReaders/pyinterop.pyx":18
+  /* "pyinterop.pyx":18
  * from libcpp.string cimport string
  * 
  * cdef cppToPyStr(string cpp_string):             # <<<<<<<<<<<<<<
  *     # Get a pointer to the underlying C string using the c_str() method
  *     cdef const char* c_string_ptr = cpp_string.c_str()
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.cppToPyStr", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.cppToPyStr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_c_bytes);
   __Pyx_XDECREF(__pyx_v_a);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":127
+/* "pyinterop.pyx":127
  * 
  * # Yes this is terrible; thank you for pointing it out.
  * cdef object voidToPython(void* ptr, cType t, size_t num):             # <<<<<<<<<<<<<<
  *     l = []
  *     if t == cType.BOOL:
  */
 
-static PyObject *__pyx_f_10UAVReaders_9pyinterop_voidToPython(void *__pyx_v_ptr, cType __pyx_v_t, size_t __pyx_v_num) {
+static PyObject *__pyx_f_10UAVReaders_voidToPython(void *__pyx_v_ptr, cType __pyx_v_t, size_t __pyx_v_num) {
   PyObject *__pyx_v_l = NULL;
   size_t __pyx_v_i;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   size_t __pyx_t_2;
   size_t __pyx_t_3;
@@ -2883,49 +2883,49 @@
   PyObject *__pyx_t_14 = NULL;
   Py_ssize_t __pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("voidToPython", 0);
 
-  /* "UAVReaders/pyinterop.pyx":128
+  /* "pyinterop.pyx":128
  * # Yes this is terrible; thank you for pointing it out.
  * cdef object voidToPython(void* ptr, cType t, size_t num):
  *     l = []             # <<<<<<<<<<<<<<
  *     if t == cType.BOOL:
  *         for i in range(num):
  */
   __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_l = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "UAVReaders/pyinterop.pyx":129
+  /* "pyinterop.pyx":129
  * cdef object voidToPython(void* ptr, cType t, size_t num):
  *     l = []
  *     if t == cType.BOOL:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(bool((<unsigned char*>ptr)[i]))
  */
   switch (__pyx_v_t) {
     case BOOL:
 
-    /* "UAVReaders/pyinterop.pyx":130
+    /* "pyinterop.pyx":130
  *     l = []
  *     if t == cType.BOOL:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(bool((<unsigned char*>ptr)[i]))
  *     elif t == cType.CHAR:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":131
+      /* "pyinterop.pyx":131
  *     if t == cType.BOOL:
  *         for i in range(num):
  *             l.append(bool((<unsigned char*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.CHAR:
  *         if num > 1:
  */
       __pyx_t_1 = __Pyx_PyInt_From_unsigned_char((((unsigned char *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
@@ -2934,45 +2934,45 @@
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_5))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 131, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":129
+    /* "pyinterop.pyx":129
  * cdef object voidToPython(void* ptr, cType t, size_t num):
  *     l = []
  *     if t == cType.BOOL:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(bool((<unsigned char*>ptr)[i]))
  */
     break;
     case CHAR:
 
-    /* "UAVReaders/pyinterop.pyx":133
+    /* "pyinterop.pyx":133
  *             l.append(bool((<unsigned char*>ptr)[i]))
  *     elif t == cType.CHAR:
  *         if num > 1:             # <<<<<<<<<<<<<<
  *             l = ""
  *             try:
  */
     __pyx_t_5 = ((__pyx_v_num > 1) != 0);
     if (__pyx_t_5) {
 
-      /* "UAVReaders/pyinterop.pyx":134
+      /* "pyinterop.pyx":134
  *     elif t == cType.CHAR:
  *         if num > 1:
  *             l = ""             # <<<<<<<<<<<<<<
  *             try:
  *                 l = str(<char*>ptr, encoding="utf-8")
  */
       __Pyx_INCREF(__pyx_kp_s_);
       __Pyx_DECREF_SET(__pyx_v_l, __pyx_kp_s_);
 
-      /* "UAVReaders/pyinterop.pyx":135
+      /* "pyinterop.pyx":135
  *         if num > 1:
  *             l = ""
  *             try:             # <<<<<<<<<<<<<<
  *                 l = str(<char*>ptr, encoding="utf-8")
  *             except UnicodeDecodeError:
  */
       {
@@ -2980,15 +2980,15 @@
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_9);
         /*try:*/ {
 
-          /* "UAVReaders/pyinterop.pyx":136
+          /* "pyinterop.pyx":136
  *             l = ""
  *             try:
  *                 l = str(<char*>ptr, encoding="utf-8")             # <<<<<<<<<<<<<<
  *             except UnicodeDecodeError:
  *                 l = chr((<char*>ptr)[0])
  */
           __pyx_t_1 = __Pyx_PyBytes_FromString(((char *)__pyx_v_ptr)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L6_error)
@@ -3004,15 +3004,15 @@
           __pyx_t_11 = __Pyx_PyObject_Call(((PyObject *)(&PyString_Type)), __pyx_t_10, __pyx_t_1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 136, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_DECREF_SET(__pyx_v_l, __pyx_t_11);
           __pyx_t_11 = 0;
 
-          /* "UAVReaders/pyinterop.pyx":135
+          /* "pyinterop.pyx":135
  *         if num > 1:
  *             l = ""
  *             try:             # <<<<<<<<<<<<<<
  *                 l = str(<char*>ptr, encoding="utf-8")
  *             except UnicodeDecodeError:
  */
         }
@@ -3021,30 +3021,30 @@
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L11_try_end;
         __pyx_L6_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-        /* "UAVReaders/pyinterop.pyx":137
+        /* "pyinterop.pyx":137
  *             try:
  *                 l = str(<char*>ptr, encoding="utf-8")
  *             except UnicodeDecodeError:             # <<<<<<<<<<<<<<
  *                 l = chr((<char*>ptr)[0])
  * 
  */
         __pyx_t_12 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_UnicodeDecodeError);
         if (__pyx_t_12) {
-          __Pyx_AddTraceback("UAVReaders.pyinterop.voidToPython", __pyx_clineno, __pyx_lineno, __pyx_filename);
+          __Pyx_AddTraceback("UAVReaders.voidToPython", __pyx_clineno, __pyx_lineno, __pyx_filename);
           if (__Pyx_GetException(&__pyx_t_11, &__pyx_t_1, &__pyx_t_10) < 0) __PYX_ERR(0, 137, __pyx_L8_except_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_GOTREF(__pyx_t_10);
 
-          /* "UAVReaders/pyinterop.pyx":138
+          /* "pyinterop.pyx":138
  *                 l = str(<char*>ptr, encoding="utf-8")
  *             except UnicodeDecodeError:
  *                 l = chr((<char*>ptr)[0])             # <<<<<<<<<<<<<<
  * 
  *     elif t == cType.SIGNED_CHAR:
  */
           __pyx_t_13 = __Pyx_PyInt_From_char((((char *)__pyx_v_ptr)[0])); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 138, __pyx_L8_except_error)
@@ -3058,15 +3058,15 @@
           __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
           __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
           goto __pyx_L7_exception_handled;
         }
         goto __pyx_L8_except_error;
         __pyx_L8_except_error:;
 
-        /* "UAVReaders/pyinterop.pyx":135
+        /* "pyinterop.pyx":135
  *         if num > 1:
  *             l = ""
  *             try:             # <<<<<<<<<<<<<<
  *                 l = str(<char*>ptr, encoding="utf-8")
  *             except UnicodeDecodeError:
  */
         __Pyx_XGIVEREF(__pyx_t_7);
@@ -3078,46 +3078,46 @@
         __Pyx_XGIVEREF(__pyx_t_7);
         __Pyx_XGIVEREF(__pyx_t_8);
         __Pyx_XGIVEREF(__pyx_t_9);
         __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
         __pyx_L11_try_end:;
       }
 
-      /* "UAVReaders/pyinterop.pyx":133
+      /* "pyinterop.pyx":133
  *             l.append(bool((<unsigned char*>ptr)[i]))
  *     elif t == cType.CHAR:
  *         if num > 1:             # <<<<<<<<<<<<<<
  *             l = ""
  *             try:
  */
     }
 
-    /* "UAVReaders/pyinterop.pyx":132
+    /* "pyinterop.pyx":132
  *         for i in range(num):
  *             l.append(bool((<unsigned char*>ptr)[i]))
  *     elif t == cType.CHAR:             # <<<<<<<<<<<<<<
  *         if num > 1:
  *             l = ""
  */
     break;
     case SIGNED_CHAR:
 
-    /* "UAVReaders/pyinterop.pyx":141
+    /* "pyinterop.pyx":141
  * 
  *     elif t == cType.SIGNED_CHAR:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<char*>ptr)[i]))
  *     elif t == cType.UNSIGNED_CHAR:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":142
+      /* "pyinterop.pyx":142
  *     elif t == cType.SIGNED_CHAR:
  *         for i in range(num):
  *             l.append(int((<char*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.UNSIGNED_CHAR:
  *         for i in range(num):
  */
       __pyx_t_10 = __Pyx_PyInt_From_char((((char *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 142, __pyx_L1_error)
@@ -3125,37 +3125,37 @@
       __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 142, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":140
+    /* "pyinterop.pyx":140
  *                 l = chr((<char*>ptr)[0])
  * 
  *     elif t == cType.SIGNED_CHAR:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<char*>ptr)[i]))
  */
     break;
     case UNSIGNED_CHAR:
 
-    /* "UAVReaders/pyinterop.pyx":144
+    /* "pyinterop.pyx":144
  *             l.append(int((<char*>ptr)[i]))
  *     elif t == cType.UNSIGNED_CHAR:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<unsigned char*>ptr)[i]))
  *     elif t == cType.SHORT:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":145
+      /* "pyinterop.pyx":145
  *     elif t == cType.UNSIGNED_CHAR:
  *         for i in range(num):
  *             l.append(int((<unsigned char*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.SHORT:
  *         for i in range(num):
  */
       __pyx_t_1 = __Pyx_PyInt_From_unsigned_char((((unsigned char *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
@@ -3163,37 +3163,37 @@
       __pyx_t_10 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 145, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_10); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 145, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":143
+    /* "pyinterop.pyx":143
  *         for i in range(num):
  *             l.append(int((<char*>ptr)[i]))
  *     elif t == cType.UNSIGNED_CHAR:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<unsigned char*>ptr)[i]))
  */
     break;
     case SHORT:
 
-    /* "UAVReaders/pyinterop.pyx":147
+    /* "pyinterop.pyx":147
  *             l.append(int((<unsigned char*>ptr)[i]))
  *     elif t == cType.SHORT:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<short*>ptr)[i]))
  *     elif t == cType.UNSIGNED_SHORT:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":148
+      /* "pyinterop.pyx":148
  *     elif t == cType.SHORT:
  *         for i in range(num):
  *             l.append(int((<short*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.UNSIGNED_SHORT:
  *         for i in range(num):
  */
       __pyx_t_10 = __Pyx_PyInt_From_short((((short *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 148, __pyx_L1_error)
@@ -3201,37 +3201,37 @@
       __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 148, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":146
+    /* "pyinterop.pyx":146
  *         for i in range(num):
  *             l.append(int((<unsigned char*>ptr)[i]))
  *     elif t == cType.SHORT:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<short*>ptr)[i]))
  */
     break;
     case UNSIGNED_SHORT:
 
-    /* "UAVReaders/pyinterop.pyx":150
+    /* "pyinterop.pyx":150
  *             l.append(int((<short*>ptr)[i]))
  *     elif t == cType.UNSIGNED_SHORT:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<unsigned short*>ptr)[i]))
  *     elif t == cType.INT:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":151
+      /* "pyinterop.pyx":151
  *     elif t == cType.UNSIGNED_SHORT:
  *         for i in range(num):
  *             l.append(int((<unsigned short*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.INT:
  *         for i in range(num):
  */
       __pyx_t_1 = __Pyx_PyInt_From_unsigned_short((((unsigned short *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
@@ -3239,37 +3239,37 @@
       __pyx_t_10 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 151, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_10); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 151, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":149
+    /* "pyinterop.pyx":149
  *         for i in range(num):
  *             l.append(int((<short*>ptr)[i]))
  *     elif t == cType.UNSIGNED_SHORT:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<unsigned short*>ptr)[i]))
  */
     break;
     case INT:
 
-    /* "UAVReaders/pyinterop.pyx":153
+    /* "pyinterop.pyx":153
  *             l.append(int((<unsigned short*>ptr)[i]))
  *     elif t == cType.INT:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<int*>ptr)[i]))
  *     elif t == cType.UNSIGNED_INT:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":154
+      /* "pyinterop.pyx":154
  *     elif t == cType.INT:
  *         for i in range(num):
  *             l.append(int((<int*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.UNSIGNED_INT:
  *         for i in range(num):
  */
       __pyx_t_10 = __Pyx_PyInt_From_int((((int *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 154, __pyx_L1_error)
@@ -3277,37 +3277,37 @@
       __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 154, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":152
+    /* "pyinterop.pyx":152
  *         for i in range(num):
  *             l.append(int((<unsigned short*>ptr)[i]))
  *     elif t == cType.INT:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<int*>ptr)[i]))
  */
     break;
     case UNSIGNED_INT:
 
-    /* "UAVReaders/pyinterop.pyx":156
+    /* "pyinterop.pyx":156
  *             l.append(int((<int*>ptr)[i]))
  *     elif t == cType.UNSIGNED_INT:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<unsigned int*>ptr)[i]))
  *     elif t == cType.LONG:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":157
+      /* "pyinterop.pyx":157
  *     elif t == cType.UNSIGNED_INT:
  *         for i in range(num):
  *             l.append(int((<unsigned int*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.LONG:
  *         for i in range(num):
  */
       __pyx_t_1 = __Pyx_PyInt_From_unsigned_int((((unsigned int *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
@@ -3315,37 +3315,37 @@
       __pyx_t_10 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 157, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_10); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 157, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":155
+    /* "pyinterop.pyx":155
  *         for i in range(num):
  *             l.append(int((<int*>ptr)[i]))
  *     elif t == cType.UNSIGNED_INT:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<unsigned int*>ptr)[i]))
  */
     break;
     case LONG:
 
-    /* "UAVReaders/pyinterop.pyx":159
+    /* "pyinterop.pyx":159
  *             l.append(int((<unsigned int*>ptr)[i]))
  *     elif t == cType.LONG:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<long*>ptr)[i]))
  *     elif t == cType.UNSIGNED_LONG:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":160
+      /* "pyinterop.pyx":160
  *     elif t == cType.LONG:
  *         for i in range(num):
  *             l.append(int((<long*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.UNSIGNED_LONG:
  *         for i in range(num):
  */
       __pyx_t_10 = __Pyx_PyInt_From_long((((long *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 160, __pyx_L1_error)
@@ -3353,37 +3353,37 @@
       __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 160, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":158
+    /* "pyinterop.pyx":158
  *         for i in range(num):
  *             l.append(int((<unsigned int*>ptr)[i]))
  *     elif t == cType.LONG:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<long*>ptr)[i]))
  */
     break;
     case UNSIGNED_LONG:
 
-    /* "UAVReaders/pyinterop.pyx":162
+    /* "pyinterop.pyx":162
  *             l.append(int((<long*>ptr)[i]))
  *     elif t == cType.UNSIGNED_LONG:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<unsigned long*>ptr)[i]))
  *     elif t == cType.LONG_LONG:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":163
+      /* "pyinterop.pyx":163
  *     elif t == cType.UNSIGNED_LONG:
  *         for i in range(num):
  *             l.append(int((<unsigned long*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.LONG_LONG:
  *         for i in range(num):
  */
       __pyx_t_1 = __Pyx_PyInt_From_unsigned_long((((unsigned long *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
@@ -3391,37 +3391,37 @@
       __pyx_t_10 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 163, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_10); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 163, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":161
+    /* "pyinterop.pyx":161
  *         for i in range(num):
  *             l.append(int((<long*>ptr)[i]))
  *     elif t == cType.UNSIGNED_LONG:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<unsigned long*>ptr)[i]))
  */
     break;
     case LONG_LONG:
 
-    /* "UAVReaders/pyinterop.pyx":165
+    /* "pyinterop.pyx":165
  *             l.append(int((<unsigned long*>ptr)[i]))
  *     elif t == cType.LONG_LONG:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<long long*>ptr)[i]))
  *     elif t == cType.UNSIGNED_LONG_LONG:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":166
+      /* "pyinterop.pyx":166
  *     elif t == cType.LONG_LONG:
  *         for i in range(num):
  *             l.append(int((<long long*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.UNSIGNED_LONG_LONG:
  *         for i in range(num):
  */
       __pyx_t_10 = __Pyx_PyInt_From_PY_LONG_LONG((((PY_LONG_LONG *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 166, __pyx_L1_error)
@@ -3429,37 +3429,37 @@
       __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 166, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":164
+    /* "pyinterop.pyx":164
  *         for i in range(num):
  *             l.append(int((<unsigned long*>ptr)[i]))
  *     elif t == cType.LONG_LONG:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<long long*>ptr)[i]))
  */
     break;
     case UNSIGNED_LONG_LONG:
 
-    /* "UAVReaders/pyinterop.pyx":168
+    /* "pyinterop.pyx":168
  *             l.append(int((<long long*>ptr)[i]))
  *     elif t == cType.UNSIGNED_LONG_LONG:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<unsigned long long*>ptr)[i]))
  *     elif t == cType.INT8_T:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":169
+      /* "pyinterop.pyx":169
  *     elif t == cType.UNSIGNED_LONG_LONG:
  *         for i in range(num):
  *             l.append(int((<unsigned long long*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.INT8_T:
  *         for i in range(num):
  */
       __pyx_t_1 = __Pyx_PyInt_From_unsigned_PY_LONG_LONG((((unsigned PY_LONG_LONG *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
@@ -3467,37 +3467,37 @@
       __pyx_t_10 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 169, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_10); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 169, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":167
+    /* "pyinterop.pyx":167
  *         for i in range(num):
  *             l.append(int((<long long*>ptr)[i]))
  *     elif t == cType.UNSIGNED_LONG_LONG:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<unsigned long long*>ptr)[i]))
  */
     break;
     case INT8_T:
 
-    /* "UAVReaders/pyinterop.pyx":171
+    /* "pyinterop.pyx":171
  *             l.append(int((<unsigned long long*>ptr)[i]))
  *     elif t == cType.INT8_T:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<int8_t*>ptr)[i]))
  *     elif t == cType.UINT8_T:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":172
+      /* "pyinterop.pyx":172
  *     elif t == cType.INT8_T:
  *         for i in range(num):
  *             l.append(int((<int8_t*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.UINT8_T:
  *         for i in range(num):
  */
       __pyx_t_10 = __Pyx_PyInt_From_int8_t((((int8_t *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 172, __pyx_L1_error)
@@ -3505,37 +3505,37 @@
       __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 172, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":170
+    /* "pyinterop.pyx":170
  *         for i in range(num):
  *             l.append(int((<unsigned long long*>ptr)[i]))
  *     elif t == cType.INT8_T:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<int8_t*>ptr)[i]))
  */
     break;
     case UINT8_T:
 
-    /* "UAVReaders/pyinterop.pyx":174
+    /* "pyinterop.pyx":174
  *             l.append(int((<int8_t*>ptr)[i]))
  *     elif t == cType.UINT8_T:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<uint8_t*>ptr)[i]))
  *     elif t == cType.INT16_T:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":175
+      /* "pyinterop.pyx":175
  *     elif t == cType.UINT8_T:
  *         for i in range(num):
  *             l.append(int((<uint8_t*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.INT16_T:
  *         for i in range(num):
  */
       __pyx_t_1 = __Pyx_PyInt_From_uint8_t((((uint8_t *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
@@ -3543,37 +3543,37 @@
       __pyx_t_10 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 175, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_10); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 175, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":173
+    /* "pyinterop.pyx":173
  *         for i in range(num):
  *             l.append(int((<int8_t*>ptr)[i]))
  *     elif t == cType.UINT8_T:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<uint8_t*>ptr)[i]))
  */
     break;
     case INT16_T:
 
-    /* "UAVReaders/pyinterop.pyx":177
+    /* "pyinterop.pyx":177
  *             l.append(int((<uint8_t*>ptr)[i]))
  *     elif t == cType.INT16_T:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<int16_t*>ptr)[i]))
  *     elif t == cType.UINT16_T:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":178
+      /* "pyinterop.pyx":178
  *     elif t == cType.INT16_T:
  *         for i in range(num):
  *             l.append(int((<int16_t*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.UINT16_T:
  *         for i in range(num):
  */
       __pyx_t_10 = __Pyx_PyInt_From_int16_t((((int16_t *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 178, __pyx_L1_error)
@@ -3581,37 +3581,37 @@
       __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 178, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":176
+    /* "pyinterop.pyx":176
  *         for i in range(num):
  *             l.append(int((<uint8_t*>ptr)[i]))
  *     elif t == cType.INT16_T:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<int16_t*>ptr)[i]))
  */
     break;
     case UINT16_T:
 
-    /* "UAVReaders/pyinterop.pyx":180
+    /* "pyinterop.pyx":180
  *             l.append(int((<int16_t*>ptr)[i]))
  *     elif t == cType.UINT16_T:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<uint16_t*>ptr)[i]))
  *     elif t == cType.INT32_T:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":181
+      /* "pyinterop.pyx":181
  *     elif t == cType.UINT16_T:
  *         for i in range(num):
  *             l.append(int((<uint16_t*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.INT32_T:
  *         for i in range(num):
  */
       __pyx_t_1 = __Pyx_PyInt_From_uint16_t((((uint16_t *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
@@ -3619,37 +3619,37 @@
       __pyx_t_10 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 181, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_10); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 181, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":179
+    /* "pyinterop.pyx":179
  *         for i in range(num):
  *             l.append(int((<int16_t*>ptr)[i]))
  *     elif t == cType.UINT16_T:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<uint16_t*>ptr)[i]))
  */
     break;
     case INT32_T:
 
-    /* "UAVReaders/pyinterop.pyx":183
+    /* "pyinterop.pyx":183
  *             l.append(int((<uint16_t*>ptr)[i]))
  *     elif t == cType.INT32_T:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<int32_t*>ptr)[i]))
  *     elif t == cType.UINT32_T:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":184
+      /* "pyinterop.pyx":184
  *     elif t == cType.INT32_T:
  *         for i in range(num):
  *             l.append(int((<int32_t*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.UINT32_T:
  *         for i in range(num):
  */
       __pyx_t_10 = __Pyx_PyInt_From_int32_t((((int32_t *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 184, __pyx_L1_error)
@@ -3657,37 +3657,37 @@
       __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 184, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":182
+    /* "pyinterop.pyx":182
  *         for i in range(num):
  *             l.append(int((<uint16_t*>ptr)[i]))
  *     elif t == cType.INT32_T:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<int32_t*>ptr)[i]))
  */
     break;
     case UINT32_T:
 
-    /* "UAVReaders/pyinterop.pyx":186
+    /* "pyinterop.pyx":186
  *             l.append(int((<int32_t*>ptr)[i]))
  *     elif t == cType.UINT32_T:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<uint32_t*>ptr)[i]))
  *     elif t == cType.INT64_T:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":187
+      /* "pyinterop.pyx":187
  *     elif t == cType.UINT32_T:
  *         for i in range(num):
  *             l.append(int((<uint32_t*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.INT64_T:
  *         for i in range(num):
  */
       __pyx_t_1 = __Pyx_PyInt_From_uint32_t((((uint32_t *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
@@ -3695,37 +3695,37 @@
       __pyx_t_10 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 187, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_10); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 187, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":185
+    /* "pyinterop.pyx":185
  *         for i in range(num):
  *             l.append(int((<int32_t*>ptr)[i]))
  *     elif t == cType.UINT32_T:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<uint32_t*>ptr)[i]))
  */
     break;
     case INT64_T:
 
-    /* "UAVReaders/pyinterop.pyx":189
+    /* "pyinterop.pyx":189
  *             l.append(int((<uint32_t*>ptr)[i]))
  *     elif t == cType.INT64_T:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<int64_t*>ptr)[i]))
  *     elif t == cType.UINT64_T:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":190
+      /* "pyinterop.pyx":190
  *     elif t == cType.INT64_T:
  *         for i in range(num):
  *             l.append(int((<int64_t*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.UINT64_T:
  *         for i in range(num):
  */
       __pyx_t_10 = __Pyx_PyInt_From_int64_t((((int64_t *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 190, __pyx_L1_error)
@@ -3733,37 +3733,37 @@
       __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 190, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":188
+    /* "pyinterop.pyx":188
  *         for i in range(num):
  *             l.append(int((<uint32_t*>ptr)[i]))
  *     elif t == cType.INT64_T:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<int64_t*>ptr)[i]))
  */
     break;
     case UINT64_T:
 
-    /* "UAVReaders/pyinterop.pyx":192
+    /* "pyinterop.pyx":192
  *             l.append(int((<int64_t*>ptr)[i]))
  *     elif t == cType.UINT64_T:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(int((<uint64_t*>ptr)[i]))
  *     elif t == cType.FLOAT:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":193
+      /* "pyinterop.pyx":193
  *     elif t == cType.UINT64_T:
  *         for i in range(num):
  *             l.append(int((<uint64_t*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.FLOAT:
  *         for i in range(num):
  */
       __pyx_t_1 = __Pyx_PyInt_From_uint64_t((((uint64_t *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
@@ -3771,241 +3771,241 @@
       __pyx_t_10 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyInt_Type)), __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 193, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_10); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 193, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":191
+    /* "pyinterop.pyx":191
  *         for i in range(num):
  *             l.append(int((<int64_t*>ptr)[i]))
  *     elif t == cType.UINT64_T:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(int((<uint64_t*>ptr)[i]))
  */
     break;
     case FLOAT:
 
-    /* "UAVReaders/pyinterop.pyx":195
+    /* "pyinterop.pyx":195
  *             l.append(int((<uint64_t*>ptr)[i]))
  *     elif t == cType.FLOAT:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(float((<float*>ptr)[i]))
  *     elif t == cType.DOUBLE:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":196
+      /* "pyinterop.pyx":196
  *     elif t == cType.FLOAT:
  *         for i in range(num):
  *             l.append(float((<float*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     elif t == cType.DOUBLE:
  *         for i in range(num):
  */
       __pyx_t_10 = PyFloat_FromDouble(((double)(((float *)__pyx_v_ptr)[__pyx_v_i]))); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 196, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_10); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 196, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":194
+    /* "pyinterop.pyx":194
  *         for i in range(num):
  *             l.append(int((<uint64_t*>ptr)[i]))
  *     elif t == cType.FLOAT:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(float((<float*>ptr)[i]))
  */
     break;
     case DOUBLE:
 
-    /* "UAVReaders/pyinterop.pyx":198
+    /* "pyinterop.pyx":198
  *             l.append(float((<float*>ptr)[i]))
  *     elif t == cType.DOUBLE:
  *         for i in range(num):             # <<<<<<<<<<<<<<
  *             l.append(float((<double*>ptr)[i]))
  *     if len(l) == 1:
  */
     __pyx_t_2 = __pyx_v_num;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "UAVReaders/pyinterop.pyx":199
+      /* "pyinterop.pyx":199
  *     elif t == cType.DOUBLE:
  *         for i in range(num):
  *             l.append(float((<double*>ptr)[i]))             # <<<<<<<<<<<<<<
  *     if len(l) == 1:
  *         return l[0]
  */
       __pyx_t_10 = PyFloat_FromDouble((((double *)__pyx_v_ptr)[__pyx_v_i])); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 199, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_6 = __Pyx_PyObject_Append(__pyx_v_l, __pyx_t_10); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 199, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
 
-    /* "UAVReaders/pyinterop.pyx":197
+    /* "pyinterop.pyx":197
  *         for i in range(num):
  *             l.append(float((<float*>ptr)[i]))
  *     elif t == cType.DOUBLE:             # <<<<<<<<<<<<<<
  *         for i in range(num):
  *             l.append(float((<double*>ptr)[i]))
  */
     break;
     default: break;
   }
 
-  /* "UAVReaders/pyinterop.pyx":200
+  /* "pyinterop.pyx":200
  *         for i in range(num):
  *             l.append(float((<double*>ptr)[i]))
  *     if len(l) == 1:             # <<<<<<<<<<<<<<
  *         return l[0]
  *     else:
  */
   __pyx_t_15 = PyObject_Length(__pyx_v_l); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 200, __pyx_L1_error)
   __pyx_t_5 = ((__pyx_t_15 == 1) != 0);
   if (__pyx_t_5) {
 
-    /* "UAVReaders/pyinterop.pyx":201
+    /* "pyinterop.pyx":201
  *             l.append(float((<double*>ptr)[i]))
  *     if len(l) == 1:
  *         return l[0]             # <<<<<<<<<<<<<<
  *     else:
  *         return l
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_10 = __Pyx_GetItemInt(__pyx_v_l, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_r = __pyx_t_10;
     __pyx_t_10 = 0;
     goto __pyx_L0;
 
-    /* "UAVReaders/pyinterop.pyx":200
+    /* "pyinterop.pyx":200
  *         for i in range(num):
  *             l.append(float((<double*>ptr)[i]))
  *     if len(l) == 1:             # <<<<<<<<<<<<<<
  *         return l[0]
  *     else:
  */
   }
 
-  /* "UAVReaders/pyinterop.pyx":203
+  /* "pyinterop.pyx":203
  *         return l[0]
  *     else:
  *         return l             # <<<<<<<<<<<<<<
  * 
  * cdef tuple memberToPy(abstractStructMember* member):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_l);
     __pyx_r = __pyx_v_l;
     goto __pyx_L0;
   }
 
-  /* "UAVReaders/pyinterop.pyx":127
+  /* "pyinterop.pyx":127
  * 
  * # Yes this is terrible; thank you for pointing it out.
  * cdef object voidToPython(void* ptr, cType t, size_t num):             # <<<<<<<<<<<<<<
  *     l = []
  *     if t == cType.BOOL:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_14);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.voidToPython", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.voidToPython", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_l);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":205
+/* "pyinterop.pyx":205
  *         return l
  * 
  * cdef tuple memberToPy(abstractStructMember* member):             # <<<<<<<<<<<<<<
  *     cdef cType t = member.getTypeAsEnum()
  *     cdef void * p = member.getInnerPointer()
  */
 
-static PyObject *__pyx_f_10UAVReaders_9pyinterop_memberToPy(introspect::abstractStructMember *__pyx_v_member) {
+static PyObject *__pyx_f_10UAVReaders_memberToPy(introspect::abstractStructMember *__pyx_v_member) {
   cType __pyx_v_t;
   void *__pyx_v_p;
   size_t __pyx_v_num;
   PyObject *__pyx_v_pyObj = 0;
   PyObject *__pyx_v_name = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memberToPy", 0);
 
-  /* "UAVReaders/pyinterop.pyx":206
+  /* "pyinterop.pyx":206
  * 
  * cdef tuple memberToPy(abstractStructMember* member):
  *     cdef cType t = member.getTypeAsEnum()             # <<<<<<<<<<<<<<
  *     cdef void * p = member.getInnerPointer()
  *     cdef size_t num = member.getNumElements()
  */
   __pyx_v_t = __pyx_v_member->getTypeAsEnum();
 
-  /* "UAVReaders/pyinterop.pyx":207
+  /* "pyinterop.pyx":207
  * cdef tuple memberToPy(abstractStructMember* member):
  *     cdef cType t = member.getTypeAsEnum()
  *     cdef void * p = member.getInnerPointer()             # <<<<<<<<<<<<<<
  *     cdef size_t num = member.getNumElements()
  *     cdef object pyObj = voidToPython(p, t, num)
  */
   __pyx_v_p = __pyx_v_member->getInnerPointer();
 
-  /* "UAVReaders/pyinterop.pyx":208
+  /* "pyinterop.pyx":208
  *     cdef cType t = member.getTypeAsEnum()
  *     cdef void * p = member.getInnerPointer()
  *     cdef size_t num = member.getNumElements()             # <<<<<<<<<<<<<<
  *     cdef object pyObj = voidToPython(p, t, num)
  *     name = cppToPyStr(member.getName())
  */
   __pyx_v_num = __pyx_v_member->getNumElements();
 
-  /* "UAVReaders/pyinterop.pyx":209
+  /* "pyinterop.pyx":209
  *     cdef void * p = member.getInnerPointer()
  *     cdef size_t num = member.getNumElements()
  *     cdef object pyObj = voidToPython(p, t, num)             # <<<<<<<<<<<<<<
  *     name = cppToPyStr(member.getName())
  *     return name, pyObj
  */
-  __pyx_t_1 = __pyx_f_10UAVReaders_9pyinterop_voidToPython(__pyx_v_p, __pyx_v_t, __pyx_v_num); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_10UAVReaders_voidToPython(__pyx_v_p, __pyx_v_t, __pyx_v_num); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_pyObj = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "UAVReaders/pyinterop.pyx":210
+  /* "pyinterop.pyx":210
  *     cdef size_t num = member.getNumElements()
  *     cdef object pyObj = voidToPython(p, t, num)
  *     name = cppToPyStr(member.getName())             # <<<<<<<<<<<<<<
  *     return name, pyObj
  * 
  */
-  __pyx_t_1 = __pyx_f_10UAVReaders_9pyinterop_cppToPyStr(__pyx_v_member->getName()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_10UAVReaders_cppToPyStr(__pyx_v_member->getName()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_name = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "UAVReaders/pyinterop.pyx":211
+  /* "pyinterop.pyx":211
  *     cdef object pyObj = voidToPython(p, t, num)
  *     name = cppToPyStr(member.getName())
  *     return name, pyObj             # <<<<<<<<<<<<<<
  * 
  * cdef class packet(dict):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -4017,82 +4017,82 @@
   __Pyx_INCREF(__pyx_v_pyObj);
   __Pyx_GIVEREF(__pyx_v_pyObj);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_pyObj);
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "UAVReaders/pyinterop.pyx":205
+  /* "pyinterop.pyx":205
  *         return l
  * 
  * cdef tuple memberToPy(abstractStructMember* member):             # <<<<<<<<<<<<<<
  *     cdef cType t = member.getTypeAsEnum()
  *     cdef void * p = member.getInnerPointer()
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.memberToPy", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.memberToPy", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pyObj);
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":229
+/* "pyinterop.pyx":229
  *     cdef int packet_type
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         super(packet, self).__init__()
  *         self.name = ""
  */
 
 /* Python wrapper */
-static int __pyx_pw_10UAVReaders_9pyinterop_6packet_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_10UAVReaders_9pyinterop_6packet_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_10UAVReaders_6packet_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_10UAVReaders_6packet_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   if (unlikely(PyTuple_GET_SIZE(__pyx_args) > 0)) {
     __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 0, 0, PyTuple_GET_SIZE(__pyx_args)); return -1;}
   if (unlikely(__pyx_kwds) && unlikely(PyDict_Size(__pyx_kwds) > 0) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__cinit__", 0))) return -1;
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_6packet___cinit__(((struct __pyx_obj_10UAVReaders_9pyinterop_packet *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10UAVReaders_6packet___cinit__(((struct __pyx_obj_10UAVReaders_packet *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_10UAVReaders_9pyinterop_6packet___cinit__(struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_self) {
+static int __pyx_pf_10UAVReaders_6packet___cinit__(struct __pyx_obj_10UAVReaders_packet *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "UAVReaders/pyinterop.pyx":230
+  /* "pyinterop.pyx":230
  * 
  *     def __cinit__(self):
  *         super(packet, self).__init__()             # <<<<<<<<<<<<<<
  *         self.name = ""
  *         self.protocol = ""
  */
   __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(((PyObject *)__pyx_ptype_10UAVReaders_9pyinterop_packet));
-  __Pyx_GIVEREF(((PyObject *)__pyx_ptype_10UAVReaders_9pyinterop_packet));
-  PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_ptype_10UAVReaders_9pyinterop_packet));
+  __Pyx_INCREF(((PyObject *)__pyx_ptype_10UAVReaders_packet));
+  __Pyx_GIVEREF(((PyObject *)__pyx_ptype_10UAVReaders_packet));
+  PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_ptype_10UAVReaders_packet));
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)__pyx_v_self));
   __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 230, __pyx_L1_error)
@@ -4111,80 +4111,80 @@
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "UAVReaders/pyinterop.pyx":231
+  /* "pyinterop.pyx":231
  *     def __cinit__(self):
  *         super(packet, self).__init__()
  *         self.name = ""             # <<<<<<<<<<<<<<
  *         self.protocol = ""
  *         self.packet_type = 0
  */
   __Pyx_INCREF(__pyx_kp_s_);
   __Pyx_GIVEREF(__pyx_kp_s_);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
   __pyx_v_self->name = __pyx_kp_s_;
 
-  /* "UAVReaders/pyinterop.pyx":232
+  /* "pyinterop.pyx":232
  *         super(packet, self).__init__()
  *         self.name = ""
  *         self.protocol = ""             # <<<<<<<<<<<<<<
  *         self.packet_type = 0
  * 
  */
   __Pyx_INCREF(__pyx_kp_s_);
   __Pyx_GIVEREF(__pyx_kp_s_);
   __Pyx_GOTREF(__pyx_v_self->protocol);
   __Pyx_DECREF(__pyx_v_self->protocol);
   __pyx_v_self->protocol = __pyx_kp_s_;
 
-  /* "UAVReaders/pyinterop.pyx":233
+  /* "pyinterop.pyx":233
  *         self.name = ""
  *         self.protocol = ""
  *         self.packet_type = 0             # <<<<<<<<<<<<<<
  * 
  *     cdef secret_real_init(self, Struct* ptr, string proto):
  */
   __pyx_v_self->packet_type = 0;
 
-  /* "UAVReaders/pyinterop.pyx":229
+  /* "pyinterop.pyx":229
  *     cdef int packet_type
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         super(packet, self).__init__()
  *         self.name = ""
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.packet.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.packet.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":235
+/* "pyinterop.pyx":235
  *         self.packet_type = 0
  * 
  *     cdef secret_real_init(self, Struct* ptr, string proto):             # <<<<<<<<<<<<<<
  *         cdef vector[abstractStructMember*] vec = ptr.innerVector()
  *         for i in vec:
  */
 
-static PyObject *__pyx_f_10UAVReaders_9pyinterop_6packet_secret_real_init(struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_self, introspect::Struct *__pyx_v_ptr, std::string __pyx_v_proto) {
+static PyObject *__pyx_f_10UAVReaders_6packet_secret_real_init(struct __pyx_obj_10UAVReaders_packet *__pyx_v_self, introspect::Struct *__pyx_v_ptr, std::string __pyx_v_proto) {
   std::vector<introspect::abstractStructMember *>  __pyx_v_vec;
   introspect::abstractStructMember *__pyx_v_i;
   PyObject *__pyx_v_k = NULL;
   PyObject *__pyx_v_v = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   std::vector<introspect::abstractStructMember *> ::iterator __pyx_t_1;
@@ -4193,45 +4193,45 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("secret_real_init", 0);
 
-  /* "UAVReaders/pyinterop.pyx":236
+  /* "pyinterop.pyx":236
  * 
  *     cdef secret_real_init(self, Struct* ptr, string proto):
  *         cdef vector[abstractStructMember*] vec = ptr.innerVector()             # <<<<<<<<<<<<<<
  *         for i in vec:
  *             k, v = memberToPy(i)
  */
   __pyx_v_vec = __pyx_v_ptr->innerVector();
 
-  /* "UAVReaders/pyinterop.pyx":237
+  /* "pyinterop.pyx":237
  *     cdef secret_real_init(self, Struct* ptr, string proto):
  *         cdef vector[abstractStructMember*] vec = ptr.innerVector()
  *         for i in vec:             # <<<<<<<<<<<<<<
  *             k, v = memberToPy(i)
  *             self[k] = v
  */
   __pyx_t_1 = __pyx_v_vec.begin();
   for (;;) {
     if (!(__pyx_t_1 != __pyx_v_vec.end())) break;
     __pyx_t_2 = *__pyx_t_1;
     ++__pyx_t_1;
     __pyx_v_i = __pyx_t_2;
 
-    /* "UAVReaders/pyinterop.pyx":238
+    /* "pyinterop.pyx":238
  *         cdef vector[abstractStructMember*] vec = ptr.innerVector()
  *         for i in vec:
  *             k, v = memberToPy(i)             # <<<<<<<<<<<<<<
  *             self[k] = v
  * 
  */
-    __pyx_t_3 = __pyx_f_10UAVReaders_9pyinterop_memberToPy(__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __pyx_t_3 = __pyx_f_10UAVReaders_memberToPy(__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (likely(__pyx_t_3 != Py_None)) {
       PyObject* sequence = __pyx_t_3;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
@@ -4253,33 +4253,33 @@
       __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 238, __pyx_L1_error)
     }
     __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_4);
     __pyx_t_4 = 0;
     __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "UAVReaders/pyinterop.pyx":239
+    /* "pyinterop.pyx":239
  *         for i in vec:
  *             k, v = memberToPy(i)
  *             self[k] = v             # <<<<<<<<<<<<<<
  * 
  *         self.protocol = str(proto, encoding="utf-8")
  */
     if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_self), __pyx_v_k, __pyx_v_v) < 0)) __PYX_ERR(0, 239, __pyx_L1_error)
 
-    /* "UAVReaders/pyinterop.pyx":237
+    /* "pyinterop.pyx":237
  *     cdef secret_real_init(self, Struct* ptr, string proto):
  *         cdef vector[abstractStructMember*] vec = ptr.innerVector()
  *         for i in vec:             # <<<<<<<<<<<<<<
  *             k, v = memberToPy(i)
  *             self[k] = v
  */
   }
 
-  /* "UAVReaders/pyinterop.pyx":241
+  /* "pyinterop.pyx":241
  *             self[k] = v
  * 
  *         self.protocol = str(proto, encoding="utf-8")             # <<<<<<<<<<<<<<
  *         self.packet_type = ptr.getType()
  *         self.name = cppToPyStr(ptr.getName())
  */
   __pyx_t_3 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_proto); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 241, __pyx_L1_error)
@@ -4299,262 +4299,262 @@
   if (!(likely(PyString_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_4);
   __Pyx_GOTREF(__pyx_v_self->protocol);
   __Pyx_DECREF(__pyx_v_self->protocol);
   __pyx_v_self->protocol = ((PyObject*)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "UAVReaders/pyinterop.pyx":242
+  /* "pyinterop.pyx":242
  * 
  *         self.protocol = str(proto, encoding="utf-8")
  *         self.packet_type = ptr.getType()             # <<<<<<<<<<<<<<
  *         self.name = cppToPyStr(ptr.getName())
  * 
  */
   __pyx_v_self->packet_type = __pyx_v_ptr->getType();
 
-  /* "UAVReaders/pyinterop.pyx":243
+  /* "pyinterop.pyx":243
  *         self.protocol = str(proto, encoding="utf-8")
  *         self.packet_type = ptr.getType()
  *         self.name = cppToPyStr(ptr.getName())             # <<<<<<<<<<<<<<
  * 
  *         deleteStruct(ptr)
  */
-  __pyx_t_4 = __pyx_f_10UAVReaders_9pyinterop_cppToPyStr(__pyx_v_ptr->getName()); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_10UAVReaders_cppToPyStr(__pyx_v_ptr->getName()); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (!(likely(PyString_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_4);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
   __pyx_v_self->name = ((PyObject*)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "UAVReaders/pyinterop.pyx":245
+  /* "pyinterop.pyx":245
  *         self.name = cppToPyStr(ptr.getName())
  * 
  *         deleteStruct(ptr)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   UAVFormatReaders::deleteStruct(__pyx_v_ptr);
 
-  /* "UAVReaders/pyinterop.pyx":235
+  /* "pyinterop.pyx":235
  *         self.packet_type = 0
  * 
  *     cdef secret_real_init(self, Struct* ptr, string proto):             # <<<<<<<<<<<<<<
  *         cdef vector[abstractStructMember*] vec = ptr.innerVector()
  *         for i in vec:
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.packet.secret_real_init", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.packet.secret_real_init", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_k);
   __Pyx_XDECREF(__pyx_v_v);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":248
+/* "pyinterop.pyx":248
  * 
  *     @property
  *     def protocol(self):             # <<<<<<<<<<<<<<
  *         return self.protocol
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_6packet_8protocol_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_6packet_8protocol_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_10UAVReaders_6packet_8protocol_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_6packet_8protocol_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_6packet_8protocol___get__(((struct __pyx_obj_10UAVReaders_9pyinterop_packet *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10UAVReaders_6packet_8protocol___get__(((struct __pyx_obj_10UAVReaders_packet *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_6packet_8protocol___get__(struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_self) {
+static PyObject *__pyx_pf_10UAVReaders_6packet_8protocol___get__(struct __pyx_obj_10UAVReaders_packet *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "UAVReaders/pyinterop.pyx":249
+  /* "pyinterop.pyx":249
  *     @property
  *     def protocol(self):
  *         return self.protocol             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->protocol);
   __pyx_r = __pyx_v_self->protocol;
   goto __pyx_L0;
 
-  /* "UAVReaders/pyinterop.pyx":248
+  /* "pyinterop.pyx":248
  * 
  *     @property
  *     def protocol(self):             # <<<<<<<<<<<<<<
  *         return self.protocol
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":252
+/* "pyinterop.pyx":252
  * 
  *     @property
  *     def name(self):             # <<<<<<<<<<<<<<
  *         return self.name
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_6packet_4name_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_6packet_4name_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_10UAVReaders_6packet_4name_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_6packet_4name_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_6packet_4name___get__(((struct __pyx_obj_10UAVReaders_9pyinterop_packet *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10UAVReaders_6packet_4name___get__(((struct __pyx_obj_10UAVReaders_packet *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_6packet_4name___get__(struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_self) {
+static PyObject *__pyx_pf_10UAVReaders_6packet_4name___get__(struct __pyx_obj_10UAVReaders_packet *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "UAVReaders/pyinterop.pyx":253
+  /* "pyinterop.pyx":253
  *     @property
  *     def name(self):
  *         return self.name             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->name);
   __pyx_r = __pyx_v_self->name;
   goto __pyx_L0;
 
-  /* "UAVReaders/pyinterop.pyx":252
+  /* "pyinterop.pyx":252
  * 
  *     @property
  *     def name(self):             # <<<<<<<<<<<<<<
  *         return self.name
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":256
+/* "pyinterop.pyx":256
  * 
  *     @property
  *     def packet_type(self):             # <<<<<<<<<<<<<<
  *         return self.packet_type
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_6packet_11packet_type_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_6packet_11packet_type_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_10UAVReaders_6packet_11packet_type_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_6packet_11packet_type_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_6packet_11packet_type___get__(((struct __pyx_obj_10UAVReaders_9pyinterop_packet *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10UAVReaders_6packet_11packet_type___get__(((struct __pyx_obj_10UAVReaders_packet *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_6packet_11packet_type___get__(struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_self) {
+static PyObject *__pyx_pf_10UAVReaders_6packet_11packet_type___get__(struct __pyx_obj_10UAVReaders_packet *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "UAVReaders/pyinterop.pyx":257
+  /* "pyinterop.pyx":257
  *     @property
  *     def packet_type(self):
  *         return self.packet_type             # <<<<<<<<<<<<<<
  * 
  * def thing_to_iterable(thing):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->packet_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "UAVReaders/pyinterop.pyx":256
+  /* "pyinterop.pyx":256
  * 
  *     @property
  *     def packet_type(self):             # <<<<<<<<<<<<<<
  *         return self.packet_type
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.packet.packet_type.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.packet.packet_type.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_6packet_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_6packet_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_10UAVReaders_6packet_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_6packet_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_6packet_2__reduce_cython__(((struct __pyx_obj_10UAVReaders_9pyinterop_packet *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10UAVReaders_6packet_2__reduce_cython__(((struct __pyx_obj_10UAVReaders_packet *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_6packet_2__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_self) {
+static PyObject *__pyx_pf_10UAVReaders_6packet_2__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_packet *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -4576,42 +4576,42 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.packet.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.packet.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_6packet_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_6packet_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_10UAVReaders_6packet_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_6packet_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_6packet_4__setstate_cython__(((struct __pyx_obj_10UAVReaders_9pyinterop_packet *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_10UAVReaders_6packet_4__setstate_cython__(((struct __pyx_obj_10UAVReaders_packet *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_6packet_4__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_10UAVReaders_6packet_4__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_packet *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -4633,106 +4633,106 @@
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.packet.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.packet.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":259
+/* "pyinterop.pyx":259
  *         return self.packet_type
  * 
  * def thing_to_iterable(thing):             # <<<<<<<<<<<<<<
  *     """
  *     Converts certain python objects into
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_1thing_to_iterable(PyObject *__pyx_self, PyObject *__pyx_v_thing); /*proto*/
-static char __pyx_doc_10UAVReaders_9pyinterop_thing_to_iterable[] = "\n    Converts certain python objects into\n    generators returning bytes.\n    Currently accepts strings contining filenames and\n    things that are already generator functions, not touching them.\n\n    Both readers use this internally, but it can be useful to have access to \n    on its own.\n\n    :param thing: A python object to attemt to convert\n    ";
-static PyMethodDef __pyx_mdef_10UAVReaders_9pyinterop_1thing_to_iterable = {"thing_to_iterable", (PyCFunction)__pyx_pw_10UAVReaders_9pyinterop_1thing_to_iterable, METH_O, __pyx_doc_10UAVReaders_9pyinterop_thing_to_iterable};
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_1thing_to_iterable(PyObject *__pyx_self, PyObject *__pyx_v_thing) {
+static PyObject *__pyx_pw_10UAVReaders_1thing_to_iterable(PyObject *__pyx_self, PyObject *__pyx_v_thing); /*proto*/
+static char __pyx_doc_10UAVReaders_thing_to_iterable[] = "\n    Converts certain python objects into\n    generators returning bytes.\n    Currently accepts strings contining filenames and\n    things that are already generator functions, not touching them.\n\n    Both readers use this internally, but it can be useful to have access to \n    on its own.\n\n    :param thing: A python object to attemt to convert\n    ";
+static PyMethodDef __pyx_mdef_10UAVReaders_1thing_to_iterable = {"thing_to_iterable", (PyCFunction)__pyx_pw_10UAVReaders_1thing_to_iterable, METH_O, __pyx_doc_10UAVReaders_thing_to_iterable};
+static PyObject *__pyx_pw_10UAVReaders_1thing_to_iterable(PyObject *__pyx_self, PyObject *__pyx_v_thing) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("thing_to_iterable (wrapper)", 0);
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_thing_to_iterable(__pyx_self, ((PyObject *)__pyx_v_thing));
+  __pyx_r = __pyx_pf_10UAVReaders_thing_to_iterable(__pyx_self, ((PyObject *)__pyx_v_thing));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_10UAVReaders_9pyinterop_17thing_to_iterable_2generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_10UAVReaders_17thing_to_iterable_2generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "UAVReaders/pyinterop.pyx":274
+/* "pyinterop.pyx":274
  *         return thing
  *     elif type(thing) == str:
  *         def readFile():             # <<<<<<<<<<<<<<
  *             with open(thing, "rb") as f:
  *                 data = f.read(512)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_17thing_to_iterable_1readFile(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyMethodDef __pyx_mdef_10UAVReaders_9pyinterop_17thing_to_iterable_1readFile = {"readFile", (PyCFunction)__pyx_pw_10UAVReaders_9pyinterop_17thing_to_iterable_1readFile, METH_NOARGS, 0};
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_17thing_to_iterable_1readFile(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_10UAVReaders_17thing_to_iterable_1readFile(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyMethodDef __pyx_mdef_10UAVReaders_17thing_to_iterable_1readFile = {"readFile", (PyCFunction)__pyx_pw_10UAVReaders_17thing_to_iterable_1readFile, METH_NOARGS, 0};
+static PyObject *__pyx_pw_10UAVReaders_17thing_to_iterable_1readFile(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("readFile (wrapper)", 0);
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_17thing_to_iterable_readFile(__pyx_self);
+  __pyx_r = __pyx_pf_10UAVReaders_17thing_to_iterable_readFile(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_17thing_to_iterable_readFile(PyObject *__pyx_self) {
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile *__pyx_cur_scope;
+static PyObject *__pyx_pf_10UAVReaders_17thing_to_iterable_readFile(PyObject *__pyx_self) {
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("readFile", 0);
-  __pyx_cur_scope = (struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile *)__pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile(__pyx_ptype_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile, __pyx_empty_tuple, NULL);
+  __pyx_cur_scope = (struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile *)__pyx_tp_new_10UAVReaders___pyx_scope_struct_1_readFile(__pyx_ptype_10UAVReaders___pyx_scope_struct_1_readFile, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 274, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
-  __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable *) __Pyx_CyFunction_GetClosure(__pyx_self);
+  __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable *) __Pyx_CyFunction_GetClosure(__pyx_self);
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10UAVReaders_9pyinterop_17thing_to_iterable_2generator2, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_readFile, __pyx_n_s_thing_to_iterable_locals_readFil, __pyx_n_s_UAVReaders_pyinterop); if (unlikely(!gen)) __PYX_ERR(0, 274, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10UAVReaders_17thing_to_iterable_2generator2, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_readFile, __pyx_n_s_thing_to_iterable_locals_readFil, __pyx_n_s_UAVReaders); if (unlikely(!gen)) __PYX_ERR(0, 274, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_AddTraceback("UAVReaders.pyinterop.thing_to_iterable.readFile", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.thing_to_iterable.readFile", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_10UAVReaders_9pyinterop_17thing_to_iterable_2generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_10UAVReaders_17thing_to_iterable_2generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile *__pyx_cur_scope = ((struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile *)__pyx_generator->closure);
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile *__pyx_cur_scope = ((struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
@@ -4753,15 +4753,15 @@
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
   if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 274, __pyx_L1_error)
 
-  /* "UAVReaders/pyinterop.pyx":275
+  /* "pyinterop.pyx":275
  *     elif type(thing) == str:
  *         def readFile():
  *             with open(thing, "rb") as f:             # <<<<<<<<<<<<<<
  *                 data = f.read(512)
  *                 while len(data) > 0:
  */
   /*with:*/ {
@@ -4806,15 +4806,15 @@
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         /*try:*/ {
           __Pyx_GIVEREF(__pyx_t_4);
           __pyx_cur_scope->__pyx_v_f = __pyx_t_4;
           __pyx_t_4 = 0;
 
-          /* "UAVReaders/pyinterop.pyx":276
+          /* "pyinterop.pyx":276
  *         def readFile():
  *             with open(thing, "rb") as f:
  *                 data = f.read(512)             # <<<<<<<<<<<<<<
  *                 while len(data) > 0:
  *                     yield data
  */
           __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_f, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L8_error)
@@ -4834,27 +4834,27 @@
           if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 276, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_GIVEREF(__pyx_t_4);
           __pyx_cur_scope->__pyx_v_data = __pyx_t_4;
           __pyx_t_4 = 0;
 
-          /* "UAVReaders/pyinterop.pyx":277
+          /* "pyinterop.pyx":277
  *             with open(thing, "rb") as f:
  *                 data = f.read(512)
  *                 while len(data) > 0:             # <<<<<<<<<<<<<<
  *                     yield data
  *                     data = f.read(512)
  */
           while (1) {
             __pyx_t_9 = PyObject_Length(__pyx_cur_scope->__pyx_v_data); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 277, __pyx_L8_error)
             __pyx_t_10 = ((__pyx_t_9 > 0) != 0);
             if (!__pyx_t_10) break;
 
-            /* "UAVReaders/pyinterop.pyx":278
+            /* "pyinterop.pyx":278
  *                 data = f.read(512)
  *                 while len(data) > 0:
  *                     yield data             # <<<<<<<<<<<<<<
  *                     data = f.read(512)
  * 
  */
             __Pyx_INCREF(__pyx_cur_scope->__pyx_v_data);
@@ -4884,15 +4884,15 @@
             __pyx_cur_scope->__pyx_t_2 = 0;
             __Pyx_XGOTREF(__pyx_t_7);
             __pyx_t_8 = __pyx_cur_scope->__pyx_t_3;
             __pyx_cur_scope->__pyx_t_3 = 0;
             __Pyx_XGOTREF(__pyx_t_8);
             if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 278, __pyx_L8_error)
 
-            /* "UAVReaders/pyinterop.pyx":279
+            /* "pyinterop.pyx":279
  *                 while len(data) > 0:
  *                     yield data
  *                     data = f.read(512)             # <<<<<<<<<<<<<<
  * 
  *         return readFile
  */
             __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_f, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 279, __pyx_L8_error)
@@ -4914,15 +4914,15 @@
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_data);
             __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_data, __pyx_t_4);
             __Pyx_GIVEREF(__pyx_t_4);
             __pyx_t_4 = 0;
           }
 
-          /* "UAVReaders/pyinterop.pyx":275
+          /* "pyinterop.pyx":275
  *     elif type(thing) == str:
  *         def readFile():
  *             with open(thing, "rb") as f:             # <<<<<<<<<<<<<<
  *                 data = f.read(512)
  *                 while len(data) > 0:
  */
         }
@@ -4932,15 +4932,15 @@
         goto __pyx_L13_try_end;
         __pyx_L8_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
-          __Pyx_AddTraceback("UAVReaders.pyinterop.thing_to_iterable.readFile", __pyx_clineno, __pyx_lineno, __pyx_filename);
+          __Pyx_AddTraceback("UAVReaders.thing_to_iterable.readFile", __pyx_clineno, __pyx_lineno, __pyx_filename);
           if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_2, &__pyx_t_1) < 0) __PYX_ERR(0, 275, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_GOTREF(__pyx_t_1);
           __pyx_t_5 = PyTuple_Pack(3, __pyx_t_4, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 275, __pyx_L10_except_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL);
@@ -4996,15 +4996,15 @@
     __pyx_L4_error:;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L1_error;
     __pyx_L20:;
   }
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "UAVReaders/pyinterop.pyx":274
+  /* "pyinterop.pyx":274
  *         return thing
  *     elif type(thing) == str:
  *         def readFile():             # <<<<<<<<<<<<<<
  *             with open(thing, "rb") as f:
  *                 data = f.read(512)
  */
 
@@ -5024,162 +5024,162 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":259
+/* "pyinterop.pyx":259
  *         return self.packet_type
  * 
  * def thing_to_iterable(thing):             # <<<<<<<<<<<<<<
  *     """
  *     Converts certain python objects into
  */
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_thing_to_iterable(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_thing) {
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable *__pyx_cur_scope;
+static PyObject *__pyx_pf_10UAVReaders_thing_to_iterable(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_thing) {
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable *__pyx_cur_scope;
   PyObject *__pyx_v_readFile = 0;
-  PyObject *__pyx_gb_10UAVReaders_9pyinterop_17thing_to_iterable_2generator2 = 0;
+  PyObject *__pyx_gb_10UAVReaders_17thing_to_iterable_2generator2 = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("thing_to_iterable", 0);
-  __pyx_cur_scope = (struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable *)__pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable(__pyx_ptype_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable, __pyx_empty_tuple, NULL);
+  __pyx_cur_scope = (struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable *)__pyx_tp_new_10UAVReaders___pyx_scope_struct__thing_to_iterable(__pyx_ptype_10UAVReaders___pyx_scope_struct__thing_to_iterable, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 259, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_thing = __pyx_v_thing;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_thing);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_thing);
 
-  /* "UAVReaders/pyinterop.pyx":271
+  /* "pyinterop.pyx":271
  *     :param thing: A python object to attemt to convert
  *     """
  *     if (callable(thing)):             # <<<<<<<<<<<<<<
  *         return thing
  *     elif type(thing) == str:
  */
   __pyx_t_1 = __pyx_cur_scope->__pyx_v_thing;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyCallable_Check(__pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "UAVReaders/pyinterop.pyx":272
+    /* "pyinterop.pyx":272
  *     """
  *     if (callable(thing)):
  *         return thing             # <<<<<<<<<<<<<<
  *     elif type(thing) == str:
  *         def readFile():
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_thing);
     __pyx_r = __pyx_cur_scope->__pyx_v_thing;
     goto __pyx_L0;
 
-    /* "UAVReaders/pyinterop.pyx":271
+    /* "pyinterop.pyx":271
  *     :param thing: A python object to attemt to convert
  *     """
  *     if (callable(thing)):             # <<<<<<<<<<<<<<
  *         return thing
  *     elif type(thing) == str:
  */
   }
 
-  /* "UAVReaders/pyinterop.pyx":273
+  /* "pyinterop.pyx":273
  *     if (callable(thing)):
  *         return thing
  *     elif type(thing) == str:             # <<<<<<<<<<<<<<
  *         def readFile():
  *             with open(thing, "rb") as f:
  */
   __pyx_t_1 = PyObject_RichCompare(((PyObject *)Py_TYPE(__pyx_cur_scope->__pyx_v_thing)), ((PyObject *)(&PyString_Type)), Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
   __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_3) {
 
-    /* "UAVReaders/pyinterop.pyx":274
+    /* "pyinterop.pyx":274
  *         return thing
  *     elif type(thing) == str:
  *         def readFile():             # <<<<<<<<<<<<<<
  *             with open(thing, "rb") as f:
  *                 data = f.read(512)
  */
-    __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_10UAVReaders_9pyinterop_17thing_to_iterable_1readFile, 0, __pyx_n_s_thing_to_iterable_locals_readFil, ((PyObject*)__pyx_cur_scope), __pyx_n_s_UAVReaders_pyinterop, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 274, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_10UAVReaders_17thing_to_iterable_1readFile, 0, __pyx_n_s_thing_to_iterable_locals_readFil, ((PyObject*)__pyx_cur_scope), __pyx_n_s_UAVReaders, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 274, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_readFile = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "UAVReaders/pyinterop.pyx":281
+    /* "pyinterop.pyx":281
  *                     data = f.read(512)
  * 
  *         return readFile             # <<<<<<<<<<<<<<
  * 
  * cdef class mavlink_reader:
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_readFile);
     __pyx_r = __pyx_v_readFile;
     goto __pyx_L0;
 
-    /* "UAVReaders/pyinterop.pyx":273
+    /* "pyinterop.pyx":273
  *     if (callable(thing)):
  *         return thing
  *     elif type(thing) == str:             # <<<<<<<<<<<<<<
  *         def readFile():
  *             with open(thing, "rb") as f:
  */
   }
 
-  /* "UAVReaders/pyinterop.pyx":259
+  /* "pyinterop.pyx":259
  *         return self.packet_type
  * 
  * def thing_to_iterable(thing):             # <<<<<<<<<<<<<<
  *     """
  *     Converts certain python objects into
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.thing_to_iterable", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.thing_to_iterable", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_readFile);
-  __Pyx_XDECREF(__pyx_gb_10UAVReaders_9pyinterop_17thing_to_iterable_2generator2);
+  __Pyx_XDECREF(__pyx_gb_10UAVReaders_17thing_to_iterable_2generator2);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":311
+/* "pyinterop.pyx":311
  *     cdef object gen
  * 
  *     def __cinit__(self, src):             # <<<<<<<<<<<<<<
  *         self.reader = new mavLinkReader()
  *         self.gen = thing_to_iterable(src)
  */
 
 /* Python wrapper */
-static int __pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_10UAVReaders_14mavlink_reader_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_10UAVReaders_14mavlink_reader_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_src = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
@@ -5211,53 +5211,53 @@
     }
     __pyx_v_src = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 311, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("UAVReaders.pyinterop.mavlink_reader.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.mavlink_reader.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader___cinit__(((struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *)__pyx_v_self), __pyx_v_src);
+  __pyx_r = __pyx_pf_10UAVReaders_14mavlink_reader___cinit__(((struct __pyx_obj_10UAVReaders_mavlink_reader *)__pyx_v_self), __pyx_v_src);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader___cinit__(struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self, PyObject *__pyx_v_src) {
+static int __pyx_pf_10UAVReaders_14mavlink_reader___cinit__(struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self, PyObject *__pyx_v_src) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   UAVFormatReaders::mavLinkReader *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "UAVReaders/pyinterop.pyx":312
+  /* "pyinterop.pyx":312
  * 
  *     def __cinit__(self, src):
  *         self.reader = new mavLinkReader()             # <<<<<<<<<<<<<<
  *         self.gen = thing_to_iterable(src)
  * 
  */
   try {
     __pyx_t_1 = new UAVFormatReaders::mavLinkReader();
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 312, __pyx_L1_error)
   }
   __pyx_v_self->reader = __pyx_t_1;
 
-  /* "UAVReaders/pyinterop.pyx":313
+  /* "pyinterop.pyx":313
  *     def __cinit__(self, src):
  *         self.reader = new mavLinkReader()
  *         self.gen = thing_to_iterable(src)             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__ (self):
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_thing_to_iterable); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 313, __pyx_L1_error)
@@ -5279,213 +5279,213 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->gen);
   __Pyx_DECREF(__pyx_v_self->gen);
   __pyx_v_self->gen = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "UAVReaders/pyinterop.pyx":311
+  /* "pyinterop.pyx":311
  *     cdef object gen
  * 
  *     def __cinit__(self, src):             # <<<<<<<<<<<<<<
  *         self.reader = new mavLinkReader()
  *         self.gen = thing_to_iterable(src)
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.mavlink_reader.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.mavlink_reader.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":315
+/* "pyinterop.pyx":315
  *         self.gen = thing_to_iterable(src)
  * 
  *     def __dealloc__ (self):             # <<<<<<<<<<<<<<
  *         del self.reader
  * 
  */
 
 /* Python wrapper */
-static void __pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
-static void __pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_3__dealloc__(PyObject *__pyx_v_self) {
+static void __pyx_pw_10UAVReaders_14mavlink_reader_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
+static void __pyx_pw_10UAVReaders_14mavlink_reader_3__dealloc__(PyObject *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
-  __pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_2__dealloc__(((struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *)__pyx_v_self));
+  __pyx_pf_10UAVReaders_14mavlink_reader_2__dealloc__(((struct __pyx_obj_10UAVReaders_mavlink_reader *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-static void __pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_2__dealloc__(struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self) {
+static void __pyx_pf_10UAVReaders_14mavlink_reader_2__dealloc__(struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "UAVReaders/pyinterop.pyx":316
+  /* "pyinterop.pyx":316
  * 
  *     def __dealloc__ (self):
  *         del self.reader             # <<<<<<<<<<<<<<
  * 
  *     def parseByte(self, const uint8_t byte):
  */
   delete __pyx_v_self->reader;
 
-  /* "UAVReaders/pyinterop.pyx":315
+  /* "pyinterop.pyx":315
  *         self.gen = thing_to_iterable(src)
  * 
  *     def __dealloc__ (self):             # <<<<<<<<<<<<<<
  *         del self.reader
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "UAVReaders/pyinterop.pyx":318
+/* "pyinterop.pyx":318
  *         del self.reader
  * 
  *     def parseByte(self, const uint8_t byte):             # <<<<<<<<<<<<<<
  *         self.reader.parseByte(byte)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_5parseByte(PyObject *__pyx_v_self, PyObject *__pyx_arg_byte); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_5parseByte(PyObject *__pyx_v_self, PyObject *__pyx_arg_byte) {
+static PyObject *__pyx_pw_10UAVReaders_14mavlink_reader_5parseByte(PyObject *__pyx_v_self, PyObject *__pyx_arg_byte); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_14mavlink_reader_5parseByte(PyObject *__pyx_v_self, PyObject *__pyx_arg_byte) {
   uint8_t __pyx_v_byte;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("parseByte (wrapper)", 0);
   assert(__pyx_arg_byte); {
     __pyx_v_byte = __Pyx_PyInt_As_uint8_t(__pyx_arg_byte); if (unlikely((__pyx_v_byte == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 318, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
-  __Pyx_AddTraceback("UAVReaders.pyinterop.mavlink_reader.parseByte", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.mavlink_reader.parseByte", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_4parseByte(((struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *)__pyx_v_self), ((uint8_t)__pyx_v_byte));
+  __pyx_r = __pyx_pf_10UAVReaders_14mavlink_reader_4parseByte(((struct __pyx_obj_10UAVReaders_mavlink_reader *)__pyx_v_self), ((uint8_t)__pyx_v_byte));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_4parseByte(struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self, uint8_t __pyx_v_byte) {
+static PyObject *__pyx_pf_10UAVReaders_14mavlink_reader_4parseByte(struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self, uint8_t __pyx_v_byte) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parseByte", 0);
 
-  /* "UAVReaders/pyinterop.pyx":319
+  /* "pyinterop.pyx":319
  * 
  *     def parseByte(self, const uint8_t byte):
  *         self.reader.parseByte(byte)             # <<<<<<<<<<<<<<
  * 
  *     def parseBuffer(self, const uint8_t[:] bytes):
  */
   try {
     __pyx_v_self->reader->parseByte(__pyx_v_byte);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 319, __pyx_L1_error)
   }
 
-  /* "UAVReaders/pyinterop.pyx":318
+  /* "pyinterop.pyx":318
  *         del self.reader
  * 
  *     def parseByte(self, const uint8_t byte):             # <<<<<<<<<<<<<<
  *         self.reader.parseByte(byte)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("UAVReaders.pyinterop.mavlink_reader.parseByte", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.mavlink_reader.parseByte", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":321
+/* "pyinterop.pyx":321
  *         self.reader.parseByte(byte)
  * 
  *     def parseBuffer(self, const uint8_t[:] bytes):             # <<<<<<<<<<<<<<
  *         cdef uint64_t l = len(bytes)
  *         self.reader.parseBuffer(&bytes[0], l)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_7parseBuffer(PyObject *__pyx_v_self, PyObject *__pyx_arg_bytes); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_7parseBuffer(PyObject *__pyx_v_self, PyObject *__pyx_arg_bytes) {
+static PyObject *__pyx_pw_10UAVReaders_14mavlink_reader_7parseBuffer(PyObject *__pyx_v_self, PyObject *__pyx_arg_bytes); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_14mavlink_reader_7parseBuffer(PyObject *__pyx_v_self, PyObject *__pyx_arg_bytes) {
   __Pyx_memviewslice __pyx_v_bytes = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("parseBuffer (wrapper)", 0);
   assert(__pyx_arg_bytes); {
     __pyx_v_bytes = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_arg_bytes, 0); if (unlikely(!__pyx_v_bytes.memview)) __PYX_ERR(0, 321, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
-  __Pyx_AddTraceback("UAVReaders.pyinterop.mavlink_reader.parseBuffer", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.mavlink_reader.parseBuffer", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_6parseBuffer(((struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *)__pyx_v_self), __pyx_v_bytes);
+  __pyx_r = __pyx_pf_10UAVReaders_14mavlink_reader_6parseBuffer(((struct __pyx_obj_10UAVReaders_mavlink_reader *)__pyx_v_self), __pyx_v_bytes);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_6parseBuffer(struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self, __Pyx_memviewslice __pyx_v_bytes) {
+static PyObject *__pyx_pf_10UAVReaders_14mavlink_reader_6parseBuffer(struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self, __Pyx_memviewslice __pyx_v_bytes) {
   uint64_t __pyx_v_l;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   size_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parseBuffer", 0);
 
-  /* "UAVReaders/pyinterop.pyx":322
+  /* "pyinterop.pyx":322
  * 
  *     def parseBuffer(self, const uint8_t[:] bytes):
  *         cdef uint64_t l = len(bytes)             # <<<<<<<<<<<<<<
  *         self.reader.parseBuffer(&bytes[0], l)
  * 
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_bytes); 
   __pyx_v_l = __pyx_t_1;
 
-  /* "UAVReaders/pyinterop.pyx":323
+  /* "pyinterop.pyx":323
  *     def parseBuffer(self, const uint8_t[:] bytes):
  *         cdef uint64_t l = len(bytes)
  *         self.reader.parseBuffer(&bytes[0], l)             # <<<<<<<<<<<<<<
  * 
  *     def get_packet(self) -> packet:
  */
   __pyx_t_2 = 0;
@@ -5501,247 +5501,247 @@
   try {
     __pyx_v_self->reader->parseBuffer((&(*((uint8_t const  *) ( /* dim=0 */ (__pyx_v_bytes.data + __pyx_t_2 * __pyx_v_bytes.strides[0]) )))), __pyx_v_l);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 323, __pyx_L1_error)
   }
 
-  /* "UAVReaders/pyinterop.pyx":321
+  /* "pyinterop.pyx":321
  *         self.reader.parseByte(byte)
  * 
  *     def parseBuffer(self, const uint8_t[:] bytes):             # <<<<<<<<<<<<<<
  *         cdef uint64_t l = len(bytes)
  *         self.reader.parseBuffer(&bytes[0], l)
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("UAVReaders.pyinterop.mavlink_reader.parseBuffer", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.mavlink_reader.parseBuffer", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_bytes, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":325
+/* "pyinterop.pyx":325
  *         self.reader.parseBuffer(&bytes[0], l)
  * 
  *     def get_packet(self) -> packet:             # <<<<<<<<<<<<<<
  *         cdef int n = self.reader.numAvailable()
  *         if (n > 0):
  */
 
 /* Python wrapper */
-static struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_9get_packet(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_9get_packet(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
-  struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_r = 0;
+static struct __pyx_obj_10UAVReaders_packet *__pyx_pw_10UAVReaders_14mavlink_reader_9get_packet(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static struct __pyx_obj_10UAVReaders_packet *__pyx_pw_10UAVReaders_14mavlink_reader_9get_packet(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  struct __pyx_obj_10UAVReaders_packet *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_packet (wrapper)", 0);
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_8get_packet(((struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10UAVReaders_14mavlink_reader_8get_packet(((struct __pyx_obj_10UAVReaders_mavlink_reader *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_8get_packet(struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self) {
+static struct __pyx_obj_10UAVReaders_packet *__pyx_pf_10UAVReaders_14mavlink_reader_8get_packet(struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self) {
   int __pyx_v_n;
   introspect::Struct *__pyx_v_s;
-  struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_p = NULL;
-  struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_r = NULL;
+  struct __pyx_obj_10UAVReaders_packet *__pyx_v_p = NULL;
+  struct __pyx_obj_10UAVReaders_packet *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   introspect::Struct *__pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   std::string __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_packet", 0);
 
-  /* "UAVReaders/pyinterop.pyx":326
+  /* "pyinterop.pyx":326
  * 
  *     def get_packet(self) -> packet:
  *         cdef int n = self.reader.numAvailable()             # <<<<<<<<<<<<<<
  *         if (n > 0):
  *             s = self.reader.getPacket()
  */
   __pyx_v_n = __pyx_v_self->reader->numAvailable();
 
-  /* "UAVReaders/pyinterop.pyx":327
+  /* "pyinterop.pyx":327
  *     def get_packet(self) -> packet:
  *         cdef int n = self.reader.numAvailable()
  *         if (n > 0):             # <<<<<<<<<<<<<<
  *             s = self.reader.getPacket()
  *             p = packet()
  */
   __pyx_t_1 = ((__pyx_v_n > 0) != 0);
   if (__pyx_t_1) {
 
-    /* "UAVReaders/pyinterop.pyx":328
+    /* "pyinterop.pyx":328
  *         cdef int n = self.reader.numAvailable()
  *         if (n > 0):
  *             s = self.reader.getPacket()             # <<<<<<<<<<<<<<
  *             p = packet()
  *             p.secret_real_init(s, "mavlink")
  */
     try {
       __pyx_t_2 = __pyx_v_self->reader->getPacket();
     } catch(...) {
       __Pyx_CppExn2PyErr();
       __PYX_ERR(0, 328, __pyx_L1_error)
     }
     __pyx_v_s = __pyx_t_2;
 
-    /* "UAVReaders/pyinterop.pyx":329
+    /* "pyinterop.pyx":329
  *         if (n > 0):
  *             s = self.reader.getPacket()
  *             p = packet()             # <<<<<<<<<<<<<<
  *             p.secret_real_init(s, "mavlink")
  *             return p
  */
-    __pyx_t_3 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_10UAVReaders_9pyinterop_packet)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 329, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_10UAVReaders_packet)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_v_p = ((struct __pyx_obj_10UAVReaders_9pyinterop_packet *)__pyx_t_3);
+    __pyx_v_p = ((struct __pyx_obj_10UAVReaders_packet *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "UAVReaders/pyinterop.pyx":330
+    /* "pyinterop.pyx":330
  *             s = self.reader.getPacket()
  *             p = packet()
  *             p.secret_real_init(s, "mavlink")             # <<<<<<<<<<<<<<
  *             return p
  *         else:
  */
     __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_n_b_mavlink); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 330, __pyx_L1_error)
-    __pyx_t_3 = ((struct __pyx_vtabstruct_10UAVReaders_9pyinterop_packet *)__pyx_v_p->__pyx_vtab)->secret_real_init(__pyx_v_p, __pyx_v_s, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 330, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_10UAVReaders_packet *)__pyx_v_p->__pyx_vtab)->secret_real_init(__pyx_v_p, __pyx_v_s, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "UAVReaders/pyinterop.pyx":331
+    /* "pyinterop.pyx":331
  *             p = packet()
  *             p.secret_real_init(s, "mavlink")
  *             return p             # <<<<<<<<<<<<<<
  *         else:
  *             return None
  */
     __Pyx_XDECREF(((PyObject *)__pyx_r));
     __Pyx_INCREF(((PyObject *)__pyx_v_p));
     __pyx_r = __pyx_v_p;
     goto __pyx_L0;
 
-    /* "UAVReaders/pyinterop.pyx":327
+    /* "pyinterop.pyx":327
  *     def get_packet(self) -> packet:
  *         cdef int n = self.reader.numAvailable()
  *         if (n > 0):             # <<<<<<<<<<<<<<
  *             s = self.reader.getPacket()
  *             p = packet()
  */
   }
 
-  /* "UAVReaders/pyinterop.pyx":333
+  /* "pyinterop.pyx":333
  *             return p
  *         else:
  *             return None             # <<<<<<<<<<<<<<
  * 
  *     def __call__(self):
  */
   /*else*/ {
     __Pyx_XDECREF(((PyObject *)__pyx_r));
-    __pyx_r = ((struct __pyx_obj_10UAVReaders_9pyinterop_packet *)Py_None); __Pyx_INCREF(Py_None);
+    __pyx_r = ((struct __pyx_obj_10UAVReaders_packet *)Py_None); __Pyx_INCREF(Py_None);
     goto __pyx_L0;
   }
 
-  /* "UAVReaders/pyinterop.pyx":325
+  /* "pyinterop.pyx":325
  *         self.reader.parseBuffer(&bytes[0], l)
  * 
  *     def get_packet(self) -> packet:             # <<<<<<<<<<<<<<
  *         cdef int n = self.reader.numAvailable()
  *         if (n > 0):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.mavlink_reader.get_packet", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.mavlink_reader.get_packet", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_p);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_10UAVReaders_9pyinterop_14mavlink_reader_12generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_10UAVReaders_14mavlink_reader_12generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "UAVReaders/pyinterop.pyx":335
+/* "pyinterop.pyx":335
  *             return None
  * 
  *     def __call__(self):             # <<<<<<<<<<<<<<
  *         for thing in self.gen():
  *             self.parseBuffer(thing)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_11__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_11__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_10UAVReaders_14mavlink_reader_11__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_14mavlink_reader_11__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__call__ (wrapper)", 0);
   if (unlikely(PyTuple_GET_SIZE(__pyx_args) > 0)) {
     __Pyx_RaiseArgtupleInvalid("__call__", 1, 0, 0, PyTuple_GET_SIZE(__pyx_args)); return NULL;}
   if (unlikely(__pyx_kwds) && unlikely(PyDict_Size(__pyx_kwds) > 0) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__call__", 0))) return NULL;
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_10__call__(((struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10UAVReaders_14mavlink_reader_10__call__(((struct __pyx_obj_10UAVReaders_mavlink_reader *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_10__call__(struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self) {
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ *__pyx_cur_scope;
+static PyObject *__pyx_pf_10UAVReaders_14mavlink_reader_10__call__(struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self) {
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__ *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
-  __pyx_cur_scope = (struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ *)__pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__(__pyx_ptype_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__, __pyx_empty_tuple, NULL);
+  __pyx_cur_scope = (struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__ *)__pyx_tp_new_10UAVReaders___pyx_scope_struct_2___call__(__pyx_ptype_10UAVReaders___pyx_scope_struct_2___call__, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__ *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 335, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10UAVReaders_9pyinterop_14mavlink_reader_12generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_call, __pyx_n_s_mavlink_reader___call, __pyx_n_s_UAVReaders_pyinterop); if (unlikely(!gen)) __PYX_ERR(0, 335, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10UAVReaders_14mavlink_reader_12generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_call, __pyx_n_s_mavlink_reader___call, __pyx_n_s_UAVReaders); if (unlikely(!gen)) __PYX_ERR(0, 335, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_AddTraceback("UAVReaders.pyinterop.mavlink_reader.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.mavlink_reader.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_10UAVReaders_9pyinterop_14mavlink_reader_12generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_10UAVReaders_14mavlink_reader_12generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ *__pyx_cur_scope = ((struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ *)__pyx_generator->closure);
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__ *__pyx_cur_scope = ((struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__ *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   PyObject *(*__pyx_t_5)(PyObject *);
   PyObject *__pyx_t_6 = NULL;
@@ -5759,15 +5759,15 @@
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
   if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 335, __pyx_L1_error)
 
-  /* "UAVReaders/pyinterop.pyx":336
+  /* "pyinterop.pyx":336
  * 
  *     def __call__(self):
  *         for thing in self.gen():             # <<<<<<<<<<<<<<
  *             self.parseBuffer(thing)
  *             while self.reader.numAvailable() > 0:
  */
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self->gen);
@@ -5827,15 +5827,15 @@
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_thing);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_thing, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "UAVReaders/pyinterop.pyx":337
+    /* "pyinterop.pyx":337
  *     def __call__(self):
  *         for thing in self.gen():
  *             self.parseBuffer(thing)             # <<<<<<<<<<<<<<
  *             while self.reader.numAvailable() > 0:
  *                 s = self.reader.getPacket()
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_parseBuffer); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 337, __pyx_L1_error)
@@ -5853,67 +5853,67 @@
     __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_cur_scope->__pyx_v_thing) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_cur_scope->__pyx_v_thing);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "UAVReaders/pyinterop.pyx":338
+    /* "pyinterop.pyx":338
  *         for thing in self.gen():
  *             self.parseBuffer(thing)
  *             while self.reader.numAvailable() > 0:             # <<<<<<<<<<<<<<
  *                 s = self.reader.getPacket()
  *                 p = packet()
  */
     while (1) {
       __pyx_t_7 = ((__pyx_cur_scope->__pyx_v_self->reader->numAvailable() > 0) != 0);
       if (!__pyx_t_7) break;
 
-      /* "UAVReaders/pyinterop.pyx":339
+      /* "pyinterop.pyx":339
  *             self.parseBuffer(thing)
  *             while self.reader.numAvailable() > 0:
  *                 s = self.reader.getPacket()             # <<<<<<<<<<<<<<
  *                 p = packet()
  *                 p.secret_real_init(s, "mavlink")
  */
       try {
         __pyx_t_8 = __pyx_cur_scope->__pyx_v_self->reader->getPacket();
       } catch(...) {
         __Pyx_CppExn2PyErr();
         __PYX_ERR(0, 339, __pyx_L1_error)
       }
       __pyx_cur_scope->__pyx_v_s = __pyx_t_8;
 
-      /* "UAVReaders/pyinterop.pyx":340
+      /* "pyinterop.pyx":340
  *             while self.reader.numAvailable() > 0:
  *                 s = self.reader.getPacket()
  *                 p = packet()             # <<<<<<<<<<<<<<
  *                 p.secret_real_init(s, "mavlink")
  *                 yield p
  */
-      __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_10UAVReaders_9pyinterop_packet)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 340, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_10UAVReaders_packet)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 340, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_XGOTREF(((PyObject *)__pyx_cur_scope->__pyx_v_p));
-      __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_p, ((struct __pyx_obj_10UAVReaders_9pyinterop_packet *)__pyx_t_1));
+      __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_p, ((struct __pyx_obj_10UAVReaders_packet *)__pyx_t_1));
       __Pyx_GIVEREF(__pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "UAVReaders/pyinterop.pyx":341
+      /* "pyinterop.pyx":341
  *                 s = self.reader.getPacket()
  *                 p = packet()
  *                 p.secret_real_init(s, "mavlink")             # <<<<<<<<<<<<<<
  *                 yield p
  * 
  */
       __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_n_b_mavlink); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 341, __pyx_L1_error)
-      __pyx_t_1 = ((struct __pyx_vtabstruct_10UAVReaders_9pyinterop_packet *)__pyx_cur_scope->__pyx_v_p->__pyx_vtab)->secret_real_init(__pyx_cur_scope->__pyx_v_p, __pyx_cur_scope->__pyx_v_s, __pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
+      __pyx_t_1 = ((struct __pyx_vtabstruct_10UAVReaders_packet *)__pyx_cur_scope->__pyx_v_p->__pyx_vtab)->secret_real_init(__pyx_cur_scope->__pyx_v_p, __pyx_cur_scope->__pyx_v_s, __pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "UAVReaders/pyinterop.pyx":342
+      /* "pyinterop.pyx":342
  *                 p = packet()
  *                 p.secret_real_init(s, "mavlink")
  *                 yield p             # <<<<<<<<<<<<<<
  * 
  * cdef class data_flash_reader:
  */
       __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_p));
@@ -5933,26 +5933,26 @@
       __pyx_cur_scope->__pyx_t_0 = 0;
       __Pyx_XGOTREF(__pyx_t_2);
       __pyx_t_4 = __pyx_cur_scope->__pyx_t_1;
       __pyx_t_5 = __pyx_cur_scope->__pyx_t_2;
       if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 342, __pyx_L1_error)
     }
 
-    /* "UAVReaders/pyinterop.pyx":336
+    /* "pyinterop.pyx":336
  * 
  *     def __call__(self):
  *         for thing in self.gen():             # <<<<<<<<<<<<<<
  *             self.parseBuffer(thing)
  *             while self.reader.numAvailable() > 0:
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "UAVReaders/pyinterop.pyx":335
+  /* "pyinterop.pyx":335
  *             return None
  * 
  *     def __call__(self):             # <<<<<<<<<<<<<<
  *         for thing in self.gen():
  *             self.parseBuffer(thing)
  */
 
@@ -5979,27 +5979,27 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_14__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_14__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_10UAVReaders_14mavlink_reader_14__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_14mavlink_reader_14__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_13__reduce_cython__(((struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10UAVReaders_14mavlink_reader_13__reduce_cython__(((struct __pyx_obj_10UAVReaders_mavlink_reader *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_13__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self) {
+static PyObject *__pyx_pf_10UAVReaders_14mavlink_reader_13__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -6021,42 +6021,42 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.mavlink_reader.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.mavlink_reader.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_16__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_16__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_10UAVReaders_14mavlink_reader_16__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_14mavlink_reader_16__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_15__setstate_cython__(((struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_10UAVReaders_14mavlink_reader_15__setstate_cython__(((struct __pyx_obj_10UAVReaders_mavlink_reader *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_14mavlink_reader_15__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_10UAVReaders_14mavlink_reader_15__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_mavlink_reader *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -6078,32 +6078,32 @@
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.mavlink_reader.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.mavlink_reader.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":372
+/* "pyinterop.pyx":372
  *     cdef object gen
  * 
  *     def __cinit__(self, src):             # <<<<<<<<<<<<<<
  *         self.reader = new dataFlashReader()
  *         self.gen = thing_to_iterable(src)
  */
 
 /* Python wrapper */
-static int __pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_10UAVReaders_17data_flash_reader_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_10UAVReaders_17data_flash_reader_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_src = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
@@ -6135,53 +6135,53 @@
     }
     __pyx_v_src = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 372, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("UAVReaders.pyinterop.data_flash_reader.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.data_flash_reader.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader___cinit__(((struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *)__pyx_v_self), __pyx_v_src);
+  __pyx_r = __pyx_pf_10UAVReaders_17data_flash_reader___cinit__(((struct __pyx_obj_10UAVReaders_data_flash_reader *)__pyx_v_self), __pyx_v_src);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader___cinit__(struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self, PyObject *__pyx_v_src) {
+static int __pyx_pf_10UAVReaders_17data_flash_reader___cinit__(struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self, PyObject *__pyx_v_src) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   UAVFormatReaders::dataFlashReader *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "UAVReaders/pyinterop.pyx":373
+  /* "pyinterop.pyx":373
  * 
  *     def __cinit__(self, src):
  *         self.reader = new dataFlashReader()             # <<<<<<<<<<<<<<
  *         self.gen = thing_to_iterable(src)
  * 
  */
   try {
     __pyx_t_1 = new UAVFormatReaders::dataFlashReader();
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 373, __pyx_L1_error)
   }
   __pyx_v_self->reader = __pyx_t_1;
 
-  /* "UAVReaders/pyinterop.pyx":374
+  /* "pyinterop.pyx":374
  *     def __cinit__(self, src):
  *         self.reader = new dataFlashReader()
  *         self.gen = thing_to_iterable(src)             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__ (self):
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_thing_to_iterable); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 374, __pyx_L1_error)
@@ -6203,213 +6203,213 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->gen);
   __Pyx_DECREF(__pyx_v_self->gen);
   __pyx_v_self->gen = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "UAVReaders/pyinterop.pyx":372
+  /* "pyinterop.pyx":372
  *     cdef object gen
  * 
  *     def __cinit__(self, src):             # <<<<<<<<<<<<<<
  *         self.reader = new dataFlashReader()
  *         self.gen = thing_to_iterable(src)
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.data_flash_reader.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.data_flash_reader.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":376
+/* "pyinterop.pyx":376
  *         self.gen = thing_to_iterable(src)
  * 
  *     def __dealloc__ (self):             # <<<<<<<<<<<<<<
  *         del self.reader
  * 
  */
 
 /* Python wrapper */
-static void __pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
-static void __pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_3__dealloc__(PyObject *__pyx_v_self) {
+static void __pyx_pw_10UAVReaders_17data_flash_reader_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
+static void __pyx_pw_10UAVReaders_17data_flash_reader_3__dealloc__(PyObject *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
-  __pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_2__dealloc__(((struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *)__pyx_v_self));
+  __pyx_pf_10UAVReaders_17data_flash_reader_2__dealloc__(((struct __pyx_obj_10UAVReaders_data_flash_reader *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-static void __pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_2__dealloc__(struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self) {
+static void __pyx_pf_10UAVReaders_17data_flash_reader_2__dealloc__(struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "UAVReaders/pyinterop.pyx":377
+  /* "pyinterop.pyx":377
  * 
  *     def __dealloc__ (self):
  *         del self.reader             # <<<<<<<<<<<<<<
  * 
  *     def parseByte(self, const uint8_t byte):
  */
   delete __pyx_v_self->reader;
 
-  /* "UAVReaders/pyinterop.pyx":376
+  /* "pyinterop.pyx":376
  *         self.gen = thing_to_iterable(src)
  * 
  *     def __dealloc__ (self):             # <<<<<<<<<<<<<<
  *         del self.reader
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "UAVReaders/pyinterop.pyx":379
+/* "pyinterop.pyx":379
  *         del self.reader
  * 
  *     def parseByte(self, const uint8_t byte):             # <<<<<<<<<<<<<<
  *         self.reader.parseByte(byte)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_5parseByte(PyObject *__pyx_v_self, PyObject *__pyx_arg_byte); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_5parseByte(PyObject *__pyx_v_self, PyObject *__pyx_arg_byte) {
+static PyObject *__pyx_pw_10UAVReaders_17data_flash_reader_5parseByte(PyObject *__pyx_v_self, PyObject *__pyx_arg_byte); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_17data_flash_reader_5parseByte(PyObject *__pyx_v_self, PyObject *__pyx_arg_byte) {
   uint8_t __pyx_v_byte;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("parseByte (wrapper)", 0);
   assert(__pyx_arg_byte); {
     __pyx_v_byte = __Pyx_PyInt_As_uint8_t(__pyx_arg_byte); if (unlikely((__pyx_v_byte == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 379, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
-  __Pyx_AddTraceback("UAVReaders.pyinterop.data_flash_reader.parseByte", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.data_flash_reader.parseByte", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_4parseByte(((struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *)__pyx_v_self), ((uint8_t)__pyx_v_byte));
+  __pyx_r = __pyx_pf_10UAVReaders_17data_flash_reader_4parseByte(((struct __pyx_obj_10UAVReaders_data_flash_reader *)__pyx_v_self), ((uint8_t)__pyx_v_byte));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_4parseByte(struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self, uint8_t __pyx_v_byte) {
+static PyObject *__pyx_pf_10UAVReaders_17data_flash_reader_4parseByte(struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self, uint8_t __pyx_v_byte) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parseByte", 0);
 
-  /* "UAVReaders/pyinterop.pyx":380
+  /* "pyinterop.pyx":380
  * 
  *     def parseByte(self, const uint8_t byte):
  *         self.reader.parseByte(byte)             # <<<<<<<<<<<<<<
  * 
  *     def parseBuffer(self, const uint8_t[:] bytes):
  */
   try {
     __pyx_v_self->reader->parseByte(__pyx_v_byte);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 380, __pyx_L1_error)
   }
 
-  /* "UAVReaders/pyinterop.pyx":379
+  /* "pyinterop.pyx":379
  *         del self.reader
  * 
  *     def parseByte(self, const uint8_t byte):             # <<<<<<<<<<<<<<
  *         self.reader.parseByte(byte)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("UAVReaders.pyinterop.data_flash_reader.parseByte", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.data_flash_reader.parseByte", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":382
+/* "pyinterop.pyx":382
  *         self.reader.parseByte(byte)
  * 
  *     def parseBuffer(self, const uint8_t[:] bytes):             # <<<<<<<<<<<<<<
  *         cdef uint64_t l = len(bytes)
  *         self.reader.parseBuffer(&bytes[0], l)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_7parseBuffer(PyObject *__pyx_v_self, PyObject *__pyx_arg_bytes); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_7parseBuffer(PyObject *__pyx_v_self, PyObject *__pyx_arg_bytes) {
+static PyObject *__pyx_pw_10UAVReaders_17data_flash_reader_7parseBuffer(PyObject *__pyx_v_self, PyObject *__pyx_arg_bytes); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_17data_flash_reader_7parseBuffer(PyObject *__pyx_v_self, PyObject *__pyx_arg_bytes) {
   __Pyx_memviewslice __pyx_v_bytes = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("parseBuffer (wrapper)", 0);
   assert(__pyx_arg_bytes); {
     __pyx_v_bytes = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_arg_bytes, 0); if (unlikely(!__pyx_v_bytes.memview)) __PYX_ERR(0, 382, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
-  __Pyx_AddTraceback("UAVReaders.pyinterop.data_flash_reader.parseBuffer", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.data_flash_reader.parseBuffer", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_6parseBuffer(((struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *)__pyx_v_self), __pyx_v_bytes);
+  __pyx_r = __pyx_pf_10UAVReaders_17data_flash_reader_6parseBuffer(((struct __pyx_obj_10UAVReaders_data_flash_reader *)__pyx_v_self), __pyx_v_bytes);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_6parseBuffer(struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self, __Pyx_memviewslice __pyx_v_bytes) {
+static PyObject *__pyx_pf_10UAVReaders_17data_flash_reader_6parseBuffer(struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self, __Pyx_memviewslice __pyx_v_bytes) {
   uint64_t __pyx_v_l;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   size_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parseBuffer", 0);
 
-  /* "UAVReaders/pyinterop.pyx":383
+  /* "pyinterop.pyx":383
  * 
  *     def parseBuffer(self, const uint8_t[:] bytes):
  *         cdef uint64_t l = len(bytes)             # <<<<<<<<<<<<<<
  *         self.reader.parseBuffer(&bytes[0], l)
  * 
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_bytes); 
   __pyx_v_l = __pyx_t_1;
 
-  /* "UAVReaders/pyinterop.pyx":384
+  /* "pyinterop.pyx":384
  *     def parseBuffer(self, const uint8_t[:] bytes):
  *         cdef uint64_t l = len(bytes)
  *         self.reader.parseBuffer(&bytes[0], l)             # <<<<<<<<<<<<<<
  * 
  *     def get_packet(self) -> packet:
  */
   __pyx_t_2 = 0;
@@ -6425,247 +6425,247 @@
   try {
     __pyx_v_self->reader->parseBuffer((&(*((uint8_t const  *) ( /* dim=0 */ (__pyx_v_bytes.data + __pyx_t_2 * __pyx_v_bytes.strides[0]) )))), __pyx_v_l);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 384, __pyx_L1_error)
   }
 
-  /* "UAVReaders/pyinterop.pyx":382
+  /* "pyinterop.pyx":382
  *         self.reader.parseByte(byte)
  * 
  *     def parseBuffer(self, const uint8_t[:] bytes):             # <<<<<<<<<<<<<<
  *         cdef uint64_t l = len(bytes)
  *         self.reader.parseBuffer(&bytes[0], l)
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("UAVReaders.pyinterop.data_flash_reader.parseBuffer", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.data_flash_reader.parseBuffer", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_bytes, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "UAVReaders/pyinterop.pyx":386
+/* "pyinterop.pyx":386
  *         self.reader.parseBuffer(&bytes[0], l)
  * 
  *     def get_packet(self) -> packet:             # <<<<<<<<<<<<<<
  *         cdef int n = self.reader.numAvailable()
  *         if (n > 0):
  */
 
 /* Python wrapper */
-static struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_9get_packet(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_9get_packet(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
-  struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_r = 0;
+static struct __pyx_obj_10UAVReaders_packet *__pyx_pw_10UAVReaders_17data_flash_reader_9get_packet(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static struct __pyx_obj_10UAVReaders_packet *__pyx_pw_10UAVReaders_17data_flash_reader_9get_packet(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  struct __pyx_obj_10UAVReaders_packet *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_packet (wrapper)", 0);
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_8get_packet(((struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10UAVReaders_17data_flash_reader_8get_packet(((struct __pyx_obj_10UAVReaders_data_flash_reader *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_8get_packet(struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self) {
+static struct __pyx_obj_10UAVReaders_packet *__pyx_pf_10UAVReaders_17data_flash_reader_8get_packet(struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self) {
   int __pyx_v_n;
   introspect::Struct *__pyx_v_s;
-  struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_v_p = NULL;
-  struct __pyx_obj_10UAVReaders_9pyinterop_packet *__pyx_r = NULL;
+  struct __pyx_obj_10UAVReaders_packet *__pyx_v_p = NULL;
+  struct __pyx_obj_10UAVReaders_packet *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   introspect::Struct *__pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   std::string __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_packet", 0);
 
-  /* "UAVReaders/pyinterop.pyx":387
+  /* "pyinterop.pyx":387
  * 
  *     def get_packet(self) -> packet:
  *         cdef int n = self.reader.numAvailable()             # <<<<<<<<<<<<<<
  *         if (n > 0):
  *             s = self.reader.getPacket()
  */
   __pyx_v_n = __pyx_v_self->reader->numAvailable();
 
-  /* "UAVReaders/pyinterop.pyx":388
+  /* "pyinterop.pyx":388
  *     def get_packet(self) -> packet:
  *         cdef int n = self.reader.numAvailable()
  *         if (n > 0):             # <<<<<<<<<<<<<<
  *             s = self.reader.getPacket()
  *             p = packet()
  */
   __pyx_t_1 = ((__pyx_v_n > 0) != 0);
   if (__pyx_t_1) {
 
-    /* "UAVReaders/pyinterop.pyx":389
+    /* "pyinterop.pyx":389
  *         cdef int n = self.reader.numAvailable()
  *         if (n > 0):
  *             s = self.reader.getPacket()             # <<<<<<<<<<<<<<
  *             p = packet()
  *             p.secret_real_init(s, "data_flash")
  */
     try {
       __pyx_t_2 = __pyx_v_self->reader->getPacket();
     } catch(...) {
       __Pyx_CppExn2PyErr();
       __PYX_ERR(0, 389, __pyx_L1_error)
     }
     __pyx_v_s = __pyx_t_2;
 
-    /* "UAVReaders/pyinterop.pyx":390
+    /* "pyinterop.pyx":390
  *         if (n > 0):
  *             s = self.reader.getPacket()
  *             p = packet()             # <<<<<<<<<<<<<<
  *             p.secret_real_init(s, "data_flash")
  *             return p
  */
-    __pyx_t_3 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_10UAVReaders_9pyinterop_packet)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 390, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_10UAVReaders_packet)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 390, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_v_p = ((struct __pyx_obj_10UAVReaders_9pyinterop_packet *)__pyx_t_3);
+    __pyx_v_p = ((struct __pyx_obj_10UAVReaders_packet *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "UAVReaders/pyinterop.pyx":391
+    /* "pyinterop.pyx":391
  *             s = self.reader.getPacket()
  *             p = packet()
  *             p.secret_real_init(s, "data_flash")             # <<<<<<<<<<<<<<
  *             return p
  *         else:
  */
     __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_n_b_data_flash); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 391, __pyx_L1_error)
-    __pyx_t_3 = ((struct __pyx_vtabstruct_10UAVReaders_9pyinterop_packet *)__pyx_v_p->__pyx_vtab)->secret_real_init(__pyx_v_p, __pyx_v_s, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 391, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_10UAVReaders_packet *)__pyx_v_p->__pyx_vtab)->secret_real_init(__pyx_v_p, __pyx_v_s, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 391, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "UAVReaders/pyinterop.pyx":392
+    /* "pyinterop.pyx":392
  *             p = packet()
  *             p.secret_real_init(s, "data_flash")
  *             return p             # <<<<<<<<<<<<<<
  *         else:
  *             return None
  */
     __Pyx_XDECREF(((PyObject *)__pyx_r));
     __Pyx_INCREF(((PyObject *)__pyx_v_p));
     __pyx_r = __pyx_v_p;
     goto __pyx_L0;
 
-    /* "UAVReaders/pyinterop.pyx":388
+    /* "pyinterop.pyx":388
  *     def get_packet(self) -> packet:
  *         cdef int n = self.reader.numAvailable()
  *         if (n > 0):             # <<<<<<<<<<<<<<
  *             s = self.reader.getPacket()
  *             p = packet()
  */
   }
 
-  /* "UAVReaders/pyinterop.pyx":394
+  /* "pyinterop.pyx":394
  *             return p
  *         else:
  *             return None             # <<<<<<<<<<<<<<
  * 
  *     def __call__(self):
  */
   /*else*/ {
     __Pyx_XDECREF(((PyObject *)__pyx_r));
-    __pyx_r = ((struct __pyx_obj_10UAVReaders_9pyinterop_packet *)Py_None); __Pyx_INCREF(Py_None);
+    __pyx_r = ((struct __pyx_obj_10UAVReaders_packet *)Py_None); __Pyx_INCREF(Py_None);
     goto __pyx_L0;
   }
 
-  /* "UAVReaders/pyinterop.pyx":386
+  /* "pyinterop.pyx":386
  *         self.reader.parseBuffer(&bytes[0], l)
  * 
  *     def get_packet(self) -> packet:             # <<<<<<<<<<<<<<
  *         cdef int n = self.reader.numAvailable()
  *         if (n > 0):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.data_flash_reader.get_packet", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.data_flash_reader.get_packet", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_p);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_10UAVReaders_9pyinterop_17data_flash_reader_12generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_10UAVReaders_17data_flash_reader_12generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "UAVReaders/pyinterop.pyx":396
+/* "pyinterop.pyx":396
  *             return None
  * 
  *     def __call__(self):             # <<<<<<<<<<<<<<
  *         for thing in self.gen():
  *             self.parseBuffer(thing)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_11__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_11__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_10UAVReaders_17data_flash_reader_11__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_17data_flash_reader_11__call__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__call__ (wrapper)", 0);
   if (unlikely(PyTuple_GET_SIZE(__pyx_args) > 0)) {
     __Pyx_RaiseArgtupleInvalid("__call__", 1, 0, 0, PyTuple_GET_SIZE(__pyx_args)); return NULL;}
   if (unlikely(__pyx_kwds) && unlikely(PyDict_Size(__pyx_kwds) > 0) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__call__", 0))) return NULL;
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_10__call__(((struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10UAVReaders_17data_flash_reader_10__call__(((struct __pyx_obj_10UAVReaders_data_flash_reader *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_10__call__(struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self) {
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ *__pyx_cur_scope;
+static PyObject *__pyx_pf_10UAVReaders_17data_flash_reader_10__call__(struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self) {
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__ *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 0);
-  __pyx_cur_scope = (struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ *)__pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__(__pyx_ptype_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__, __pyx_empty_tuple, NULL);
+  __pyx_cur_scope = (struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__ *)__pyx_tp_new_10UAVReaders___pyx_scope_struct_3___call__(__pyx_ptype_10UAVReaders___pyx_scope_struct_3___call__, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ *)Py_None);
+    __pyx_cur_scope = ((struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__ *)Py_None);
     __Pyx_INCREF(Py_None);
     __PYX_ERR(0, 396, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10UAVReaders_9pyinterop_17data_flash_reader_12generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_call, __pyx_n_s_data_flash_reader___call, __pyx_n_s_UAVReaders_pyinterop); if (unlikely(!gen)) __PYX_ERR(0, 396, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10UAVReaders_17data_flash_reader_12generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_call, __pyx_n_s_data_flash_reader___call, __pyx_n_s_UAVReaders); if (unlikely(!gen)) __PYX_ERR(0, 396, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_AddTraceback("UAVReaders.pyinterop.data_flash_reader.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.data_flash_reader.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_10UAVReaders_9pyinterop_17data_flash_reader_12generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_10UAVReaders_17data_flash_reader_12generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ *__pyx_cur_scope = ((struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ *)__pyx_generator->closure);
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__ *__pyx_cur_scope = ((struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__ *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   PyObject *(*__pyx_t_5)(PyObject *);
   PyObject *__pyx_t_6 = NULL;
@@ -6683,15 +6683,15 @@
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
   if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 396, __pyx_L1_error)
 
-  /* "UAVReaders/pyinterop.pyx":397
+  /* "pyinterop.pyx":397
  * 
  *     def __call__(self):
  *         for thing in self.gen():             # <<<<<<<<<<<<<<
  *             self.parseBuffer(thing)
  *             while self.reader.numAvailable() > 0:
  */
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self->gen);
@@ -6751,15 +6751,15 @@
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_thing);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_thing, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "UAVReaders/pyinterop.pyx":398
+    /* "pyinterop.pyx":398
  *     def __call__(self):
  *         for thing in self.gen():
  *             self.parseBuffer(thing)             # <<<<<<<<<<<<<<
  *             while self.reader.numAvailable() > 0:
  *                 s = self.reader.getPacket()
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_parseBuffer); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 398, __pyx_L1_error)
@@ -6777,67 +6777,67 @@
     __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_cur_scope->__pyx_v_thing) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_cur_scope->__pyx_v_thing);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "UAVReaders/pyinterop.pyx":399
+    /* "pyinterop.pyx":399
  *         for thing in self.gen():
  *             self.parseBuffer(thing)
  *             while self.reader.numAvailable() > 0:             # <<<<<<<<<<<<<<
  *                 s = self.reader.getPacket()
  *                 p = packet()
  */
     while (1) {
       __pyx_t_7 = ((__pyx_cur_scope->__pyx_v_self->reader->numAvailable() > 0) != 0);
       if (!__pyx_t_7) break;
 
-      /* "UAVReaders/pyinterop.pyx":400
+      /* "pyinterop.pyx":400
  *             self.parseBuffer(thing)
  *             while self.reader.numAvailable() > 0:
  *                 s = self.reader.getPacket()             # <<<<<<<<<<<<<<
  *                 p = packet()
  *                 p.secret_real_init(s, "data_flash")
  */
       try {
         __pyx_t_8 = __pyx_cur_scope->__pyx_v_self->reader->getPacket();
       } catch(...) {
         __Pyx_CppExn2PyErr();
         __PYX_ERR(0, 400, __pyx_L1_error)
       }
       __pyx_cur_scope->__pyx_v_s = __pyx_t_8;
 
-      /* "UAVReaders/pyinterop.pyx":401
+      /* "pyinterop.pyx":401
  *             while self.reader.numAvailable() > 0:
  *                 s = self.reader.getPacket()
  *                 p = packet()             # <<<<<<<<<<<<<<
  *                 p.secret_real_init(s, "data_flash")
  *                 yield p
  */
-      __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_10UAVReaders_9pyinterop_packet)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_10UAVReaders_packet)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_XGOTREF(((PyObject *)__pyx_cur_scope->__pyx_v_p));
-      __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_p, ((struct __pyx_obj_10UAVReaders_9pyinterop_packet *)__pyx_t_1));
+      __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_p, ((struct __pyx_obj_10UAVReaders_packet *)__pyx_t_1));
       __Pyx_GIVEREF(__pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "UAVReaders/pyinterop.pyx":402
+      /* "pyinterop.pyx":402
  *                 s = self.reader.getPacket()
  *                 p = packet()
  *                 p.secret_real_init(s, "data_flash")             # <<<<<<<<<<<<<<
  *                 yield p
  * 
  */
       __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_n_b_data_flash); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 402, __pyx_L1_error)
-      __pyx_t_1 = ((struct __pyx_vtabstruct_10UAVReaders_9pyinterop_packet *)__pyx_cur_scope->__pyx_v_p->__pyx_vtab)->secret_real_init(__pyx_cur_scope->__pyx_v_p, __pyx_cur_scope->__pyx_v_s, __pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
+      __pyx_t_1 = ((struct __pyx_vtabstruct_10UAVReaders_packet *)__pyx_cur_scope->__pyx_v_p->__pyx_vtab)->secret_real_init(__pyx_cur_scope->__pyx_v_p, __pyx_cur_scope->__pyx_v_s, __pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "UAVReaders/pyinterop.pyx":403
+      /* "pyinterop.pyx":403
  *                 p = packet()
  *                 p.secret_real_init(s, "data_flash")
  *                 yield p             # <<<<<<<<<<<<<<
  * 
  */
       __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_p));
       __pyx_r = ((PyObject *)__pyx_cur_scope->__pyx_v_p);
@@ -6856,26 +6856,26 @@
       __pyx_cur_scope->__pyx_t_0 = 0;
       __Pyx_XGOTREF(__pyx_t_2);
       __pyx_t_4 = __pyx_cur_scope->__pyx_t_1;
       __pyx_t_5 = __pyx_cur_scope->__pyx_t_2;
       if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 403, __pyx_L1_error)
     }
 
-    /* "UAVReaders/pyinterop.pyx":397
+    /* "pyinterop.pyx":397
  * 
  *     def __call__(self):
  *         for thing in self.gen():             # <<<<<<<<<<<<<<
  *             self.parseBuffer(thing)
  *             while self.reader.numAvailable() > 0:
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "UAVReaders/pyinterop.pyx":396
+  /* "pyinterop.pyx":396
  *             return None
  * 
  *     def __call__(self):             # <<<<<<<<<<<<<<
  *         for thing in self.gen():
  *             self.parseBuffer(thing)
  */
 
@@ -6902,27 +6902,27 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_14__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_14__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_10UAVReaders_17data_flash_reader_14__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_17data_flash_reader_14__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_13__reduce_cython__(((struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10UAVReaders_17data_flash_reader_13__reduce_cython__(((struct __pyx_obj_10UAVReaders_data_flash_reader *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_13__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self) {
+static PyObject *__pyx_pf_10UAVReaders_17data_flash_reader_13__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -6944,42 +6944,42 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.data_flash_reader.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.data_flash_reader.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_16__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_16__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_10UAVReaders_17data_flash_reader_16__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_10UAVReaders_17data_flash_reader_16__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_15__setstate_cython__(((struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_10UAVReaders_17data_flash_reader_15__setstate_cython__(((struct __pyx_obj_10UAVReaders_data_flash_reader *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10UAVReaders_9pyinterop_17data_flash_reader_15__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_10UAVReaders_17data_flash_reader_15__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10UAVReaders_data_flash_reader *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -7001,15 +7001,15 @@
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("UAVReaders.pyinterop.data_flash_reader.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("UAVReaders.data_flash_reader.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "string.to_py":31
@@ -20362,87 +20362,87 @@
   __Pyx_AddTraceback("View.MemoryView.__pyx_unpickle_Enum__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static struct __pyx_vtabstruct_10UAVReaders_9pyinterop_packet __pyx_vtable_10UAVReaders_9pyinterop_packet;
+static struct __pyx_vtabstruct_10UAVReaders_packet __pyx_vtable_10UAVReaders_packet;
 
-static PyObject *__pyx_tp_new_10UAVReaders_9pyinterop_packet(PyTypeObject *t, PyObject *a, PyObject *k) {
-  struct __pyx_obj_10UAVReaders_9pyinterop_packet *p;
+static PyObject *__pyx_tp_new_10UAVReaders_packet(PyTypeObject *t, PyObject *a, PyObject *k) {
+  struct __pyx_obj_10UAVReaders_packet *p;
   PyObject *o = (&PyDict_Type)->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
-  p = ((struct __pyx_obj_10UAVReaders_9pyinterop_packet *)o);
-  p->__pyx_vtab = __pyx_vtabptr_10UAVReaders_9pyinterop_packet;
+  p = ((struct __pyx_obj_10UAVReaders_packet *)o);
+  p->__pyx_vtab = __pyx_vtabptr_10UAVReaders_packet;
   p->name = ((PyObject*)Py_None); Py_INCREF(Py_None);
   p->protocol = ((PyObject*)Py_None); Py_INCREF(Py_None);
-  if (unlikely(__pyx_pw_10UAVReaders_9pyinterop_6packet_1__cinit__(o, __pyx_empty_tuple, NULL) < 0)) goto bad;
+  if (unlikely(__pyx_pw_10UAVReaders_6packet_1__cinit__(o, __pyx_empty_tuple, NULL) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
-static void __pyx_tp_dealloc_10UAVReaders_9pyinterop_packet(PyObject *o) {
-  struct __pyx_obj_10UAVReaders_9pyinterop_packet *p = (struct __pyx_obj_10UAVReaders_9pyinterop_packet *)o;
+static void __pyx_tp_dealloc_10UAVReaders_packet(PyObject *o) {
+  struct __pyx_obj_10UAVReaders_packet *p = (struct __pyx_obj_10UAVReaders_packet *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   Py_CLEAR(p->protocol);
   PyObject_GC_Track(o);
   (&PyDict_Type)->tp_dealloc(o);
 }
 
-static int __pyx_tp_traverse_10UAVReaders_9pyinterop_packet(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_10UAVReaders_packet(PyObject *o, visitproc v, void *a) {
   int e;
   if (!(&PyDict_Type)->tp_traverse); else { e = (&PyDict_Type)->tp_traverse(o,v,a); if (e) return e; }
   return 0;
 }
 
-static int __pyx_tp_clear_10UAVReaders_9pyinterop_packet(PyObject *o) {
+static int __pyx_tp_clear_10UAVReaders_packet(PyObject *o) {
   if (!(&PyDict_Type)->tp_clear); else (&PyDict_Type)->tp_clear(o);
   return 0;
 }
 
-static PyObject *__pyx_getprop_10UAVReaders_9pyinterop_6packet_protocol(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_10UAVReaders_9pyinterop_6packet_8protocol_1__get__(o);
+static PyObject *__pyx_getprop_10UAVReaders_6packet_protocol(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_10UAVReaders_6packet_8protocol_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_10UAVReaders_9pyinterop_6packet_name(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_10UAVReaders_9pyinterop_6packet_4name_1__get__(o);
+static PyObject *__pyx_getprop_10UAVReaders_6packet_name(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_10UAVReaders_6packet_4name_1__get__(o);
 }
 
-static PyObject *__pyx_getprop_10UAVReaders_9pyinterop_6packet_packet_type(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_10UAVReaders_9pyinterop_6packet_11packet_type_1__get__(o);
+static PyObject *__pyx_getprop_10UAVReaders_6packet_packet_type(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_10UAVReaders_6packet_11packet_type_1__get__(o);
 }
 
-static PyMethodDef __pyx_methods_10UAVReaders_9pyinterop_packet[] = {
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_10UAVReaders_9pyinterop_6packet_3__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_10UAVReaders_9pyinterop_6packet_5__setstate_cython__, METH_O, 0},
+static PyMethodDef __pyx_methods_10UAVReaders_packet[] = {
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_10UAVReaders_6packet_3__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_10UAVReaders_6packet_5__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
-static struct PyGetSetDef __pyx_getsets_10UAVReaders_9pyinterop_packet[] = {
-  {(char *)"protocol", __pyx_getprop_10UAVReaders_9pyinterop_6packet_protocol, 0, (char *)0, 0},
-  {(char *)"name", __pyx_getprop_10UAVReaders_9pyinterop_6packet_name, 0, (char *)0, 0},
-  {(char *)"packet_type", __pyx_getprop_10UAVReaders_9pyinterop_6packet_packet_type, 0, (char *)0, 0},
+static struct PyGetSetDef __pyx_getsets_10UAVReaders_packet[] = {
+  {(char *)"protocol", __pyx_getprop_10UAVReaders_6packet_protocol, 0, (char *)0, 0},
+  {(char *)"name", __pyx_getprop_10UAVReaders_6packet_name, 0, (char *)0, 0},
+  {(char *)"packet_type", __pyx_getprop_10UAVReaders_6packet_packet_type, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_10UAVReaders_9pyinterop_packet = {
+static PyTypeObject __pyx_type_10UAVReaders_packet = {
   PyVarObject_HEAD_INIT(0, 0)
-  "UAVReaders.pyinterop.packet", /*tp_name*/
-  sizeof(struct __pyx_obj_10UAVReaders_9pyinterop_packet), /*tp_basicsize*/
+  "UAVReaders.packet", /*tp_name*/
+  sizeof(struct __pyx_obj_10UAVReaders_packet), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_10UAVReaders_9pyinterop_packet, /*tp_dealloc*/
+  __pyx_tp_dealloc_10UAVReaders_packet, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -20461,31 +20461,31 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   "\n    A class representing a packet. \n    Basically a dict, but with three additional properties:\n\n     - `.name` name of the packet\n     - `.packet_type` ID representing the type of packet within the \n       context of the packet's source protocol\n     - `.protocol` The source protocol of the packet as a string\n\n    These packets are not meant to be created by users at this time.\n    ", /*tp_doc*/
-  __pyx_tp_traverse_10UAVReaders_9pyinterop_packet, /*tp_traverse*/
-  __pyx_tp_clear_10UAVReaders_9pyinterop_packet, /*tp_clear*/
+  __pyx_tp_traverse_10UAVReaders_packet, /*tp_traverse*/
+  __pyx_tp_clear_10UAVReaders_packet, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_10UAVReaders_9pyinterop_packet, /*tp_methods*/
+  __pyx_methods_10UAVReaders_packet, /*tp_methods*/
   0, /*tp_members*/
-  __pyx_getsets_10UAVReaders_9pyinterop_packet, /*tp_getset*/
+  __pyx_getsets_10UAVReaders_packet, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_10UAVReaders_9pyinterop_packet, /*tp_new*/
+  __pyx_tp_new_10UAVReaders_packet, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -20501,85 +20501,85 @@
   0, /*tp_print*/
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
-static PyObject *__pyx_tp_new_10UAVReaders_9pyinterop_mavlink_reader(PyTypeObject *t, PyObject *a, PyObject *k) {
-  struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *p;
+static PyObject *__pyx_tp_new_10UAVReaders_mavlink_reader(PyTypeObject *t, PyObject *a, PyObject *k) {
+  struct __pyx_obj_10UAVReaders_mavlink_reader *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  p = ((struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *)o);
+  p = ((struct __pyx_obj_10UAVReaders_mavlink_reader *)o);
   p->gen = Py_None; Py_INCREF(Py_None);
-  if (unlikely(__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_1__cinit__(o, a, k) < 0)) goto bad;
+  if (unlikely(__pyx_pw_10UAVReaders_14mavlink_reader_1__cinit__(o, a, k) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
-static void __pyx_tp_dealloc_10UAVReaders_9pyinterop_mavlink_reader(PyObject *o) {
-  struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *p = (struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *)o;
+static void __pyx_tp_dealloc_10UAVReaders_mavlink_reader(PyObject *o) {
+  struct __pyx_obj_10UAVReaders_mavlink_reader *p = (struct __pyx_obj_10UAVReaders_mavlink_reader *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
-    __pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_3__dealloc__(o);
+    __pyx_pw_10UAVReaders_14mavlink_reader_3__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->gen);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
-static int __pyx_tp_traverse_10UAVReaders_9pyinterop_mavlink_reader(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_10UAVReaders_mavlink_reader(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *p = (struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *)o;
+  struct __pyx_obj_10UAVReaders_mavlink_reader *p = (struct __pyx_obj_10UAVReaders_mavlink_reader *)o;
   if (p->gen) {
     e = (*v)(p->gen, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_10UAVReaders_9pyinterop_mavlink_reader(PyObject *o) {
+static int __pyx_tp_clear_10UAVReaders_mavlink_reader(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *p = (struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader *)o;
+  struct __pyx_obj_10UAVReaders_mavlink_reader *p = (struct __pyx_obj_10UAVReaders_mavlink_reader *)o;
   tmp = ((PyObject*)p->gen);
   p->gen = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
-static PyMethodDef __pyx_methods_10UAVReaders_9pyinterop_mavlink_reader[] = {
-  {"parseByte", (PyCFunction)__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_5parseByte, METH_O, 0},
-  {"parseBuffer", (PyCFunction)__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_7parseBuffer, METH_O, 0},
-  {"get_packet", (PyCFunction)__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_9get_packet, METH_NOARGS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_14__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_16__setstate_cython__, METH_O, 0},
+static PyMethodDef __pyx_methods_10UAVReaders_mavlink_reader[] = {
+  {"parseByte", (PyCFunction)__pyx_pw_10UAVReaders_14mavlink_reader_5parseByte, METH_O, 0},
+  {"parseBuffer", (PyCFunction)__pyx_pw_10UAVReaders_14mavlink_reader_7parseBuffer, METH_O, 0},
+  {"get_packet", (PyCFunction)__pyx_pw_10UAVReaders_14mavlink_reader_9get_packet, METH_NOARGS, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_10UAVReaders_14mavlink_reader_14__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_10UAVReaders_14mavlink_reader_16__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_10UAVReaders_9pyinterop_mavlink_reader = {
+static PyTypeObject __pyx_type_10UAVReaders_mavlink_reader = {
   PyVarObject_HEAD_INIT(0, 0)
-  "UAVReaders.pyinterop.mavlink_reader", /*tp_name*/
-  sizeof(struct __pyx_obj_10UAVReaders_9pyinterop_mavlink_reader), /*tp_basicsize*/
+  "UAVReaders.mavlink_reader", /*tp_name*/
+  sizeof(struct __pyx_obj_10UAVReaders_mavlink_reader), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_10UAVReaders_9pyinterop_mavlink_reader, /*tp_dealloc*/
+  __pyx_tp_dealloc_10UAVReaders_mavlink_reader, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -20591,38 +20591,38 @@
   0, /*tp_as_async*/
   #endif
   0, /*tp_repr*/
   0, /*tp_as_number*/
   0, /*tp_as_sequence*/
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
-  __pyx_pw_10UAVReaders_9pyinterop_14mavlink_reader_11__call__, /*tp_call*/
+  __pyx_pw_10UAVReaders_14mavlink_reader_11__call__, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   "\n    Parser for DataFlash .bin files.\n    \n    To use:\n     - Load UAVReaders\n     - create a MavlinkReader\n       by passing the initializer a string filname or a \n       yielding function that returns bytes to parse\n     - Read from the Reader by calling it to obtain a \n       generator.\n    \n    for example,\n\n\n    ```python\n    from UAVReaders import mavlinkReader as mlr\n    reader = mlr(\"file.tlog\")\n    for packet in reader():\n        # do stuff\n    \n    # done!\n    ```\n    :param src: Source of bytes to parse; generator function or filename\n    ", /*tp_doc*/
-  __pyx_tp_traverse_10UAVReaders_9pyinterop_mavlink_reader, /*tp_traverse*/
-  __pyx_tp_clear_10UAVReaders_9pyinterop_mavlink_reader, /*tp_clear*/
+  __pyx_tp_traverse_10UAVReaders_mavlink_reader, /*tp_traverse*/
+  __pyx_tp_clear_10UAVReaders_mavlink_reader, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_10UAVReaders_9pyinterop_mavlink_reader, /*tp_methods*/
+  __pyx_methods_10UAVReaders_mavlink_reader, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_10UAVReaders_9pyinterop_mavlink_reader, /*tp_new*/
+  __pyx_tp_new_10UAVReaders_mavlink_reader, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -20638,85 +20638,85 @@
   0, /*tp_print*/
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
-static PyObject *__pyx_tp_new_10UAVReaders_9pyinterop_data_flash_reader(PyTypeObject *t, PyObject *a, PyObject *k) {
-  struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *p;
+static PyObject *__pyx_tp_new_10UAVReaders_data_flash_reader(PyTypeObject *t, PyObject *a, PyObject *k) {
+  struct __pyx_obj_10UAVReaders_data_flash_reader *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  p = ((struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *)o);
+  p = ((struct __pyx_obj_10UAVReaders_data_flash_reader *)o);
   p->gen = Py_None; Py_INCREF(Py_None);
-  if (unlikely(__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_1__cinit__(o, a, k) < 0)) goto bad;
+  if (unlikely(__pyx_pw_10UAVReaders_17data_flash_reader_1__cinit__(o, a, k) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
-static void __pyx_tp_dealloc_10UAVReaders_9pyinterop_data_flash_reader(PyObject *o) {
-  struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *p = (struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *)o;
+static void __pyx_tp_dealloc_10UAVReaders_data_flash_reader(PyObject *o) {
+  struct __pyx_obj_10UAVReaders_data_flash_reader *p = (struct __pyx_obj_10UAVReaders_data_flash_reader *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
-    __pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_3__dealloc__(o);
+    __pyx_pw_10UAVReaders_17data_flash_reader_3__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->gen);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
-static int __pyx_tp_traverse_10UAVReaders_9pyinterop_data_flash_reader(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_10UAVReaders_data_flash_reader(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *p = (struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *)o;
+  struct __pyx_obj_10UAVReaders_data_flash_reader *p = (struct __pyx_obj_10UAVReaders_data_flash_reader *)o;
   if (p->gen) {
     e = (*v)(p->gen, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_10UAVReaders_9pyinterop_data_flash_reader(PyObject *o) {
+static int __pyx_tp_clear_10UAVReaders_data_flash_reader(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *p = (struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader *)o;
+  struct __pyx_obj_10UAVReaders_data_flash_reader *p = (struct __pyx_obj_10UAVReaders_data_flash_reader *)o;
   tmp = ((PyObject*)p->gen);
   p->gen = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
-static PyMethodDef __pyx_methods_10UAVReaders_9pyinterop_data_flash_reader[] = {
-  {"parseByte", (PyCFunction)__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_5parseByte, METH_O, 0},
-  {"parseBuffer", (PyCFunction)__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_7parseBuffer, METH_O, 0},
-  {"get_packet", (PyCFunction)__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_9get_packet, METH_NOARGS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_14__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_16__setstate_cython__, METH_O, 0},
+static PyMethodDef __pyx_methods_10UAVReaders_data_flash_reader[] = {
+  {"parseByte", (PyCFunction)__pyx_pw_10UAVReaders_17data_flash_reader_5parseByte, METH_O, 0},
+  {"parseBuffer", (PyCFunction)__pyx_pw_10UAVReaders_17data_flash_reader_7parseBuffer, METH_O, 0},
+  {"get_packet", (PyCFunction)__pyx_pw_10UAVReaders_17data_flash_reader_9get_packet, METH_NOARGS, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_10UAVReaders_17data_flash_reader_14__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_10UAVReaders_17data_flash_reader_16__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_10UAVReaders_9pyinterop_data_flash_reader = {
+static PyTypeObject __pyx_type_10UAVReaders_data_flash_reader = {
   PyVarObject_HEAD_INIT(0, 0)
-  "UAVReaders.pyinterop.data_flash_reader", /*tp_name*/
-  sizeof(struct __pyx_obj_10UAVReaders_9pyinterop_data_flash_reader), /*tp_basicsize*/
+  "UAVReaders.data_flash_reader", /*tp_name*/
+  sizeof(struct __pyx_obj_10UAVReaders_data_flash_reader), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_10UAVReaders_9pyinterop_data_flash_reader, /*tp_dealloc*/
+  __pyx_tp_dealloc_10UAVReaders_data_flash_reader, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -20728,38 +20728,38 @@
   0, /*tp_as_async*/
   #endif
   0, /*tp_repr*/
   0, /*tp_as_number*/
   0, /*tp_as_sequence*/
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
-  __pyx_pw_10UAVReaders_9pyinterop_17data_flash_reader_11__call__, /*tp_call*/
+  __pyx_pw_10UAVReaders_17data_flash_reader_11__call__, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   "\n    Parser for DataFlash .bin files.\n    \n    To use:\n     - Load UAVReaders\n     - create a dataFlashReader or MavlinkReader\n       by passing the initializer a string filname or a \n       yielding function that returns bytes to parse\n     - Read from the Reader by calling it to obtain a \n       generator.\n    \n    for example,\n\n\n    ```python\n    from UAVReaders import dataFlashReader as dfr\n    reader = dfr(\"file.bin\")\n    for packet in reader():\n        # do stuff\n    \n    # done!\n    ```\n    :param src: Source of bytes to parse; generator function or filename\n    ", /*tp_doc*/
-  __pyx_tp_traverse_10UAVReaders_9pyinterop_data_flash_reader, /*tp_traverse*/
-  __pyx_tp_clear_10UAVReaders_9pyinterop_data_flash_reader, /*tp_clear*/
+  __pyx_tp_traverse_10UAVReaders_data_flash_reader, /*tp_traverse*/
+  __pyx_tp_clear_10UAVReaders_data_flash_reader, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_10UAVReaders_9pyinterop_data_flash_reader, /*tp_methods*/
+  __pyx_methods_10UAVReaders_data_flash_reader, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_10UAVReaders_9pyinterop_data_flash_reader, /*tp_new*/
+  __pyx_tp_new_10UAVReaders_data_flash_reader, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -20775,66 +20775,66 @@
   0, /*tp_print*/
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
-static struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable *__pyx_freelist_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable[8];
-static int __pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable = 0;
+static struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable *__pyx_freelist_10UAVReaders___pyx_scope_struct__thing_to_iterable[8];
+static int __pyx_freecount_10UAVReaders___pyx_scope_struct__thing_to_iterable = 0;
 
-static PyObject *__pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_10UAVReaders___pyx_scope_struct__thing_to_iterable(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable)))) {
-    o = (PyObject*)__pyx_freelist_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable[--__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable];
-    memset(o, 0, sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable));
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_10UAVReaders___pyx_scope_struct__thing_to_iterable > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable)))) {
+    o = (PyObject*)__pyx_freelist_10UAVReaders___pyx_scope_struct__thing_to_iterable[--__pyx_freecount_10UAVReaders___pyx_scope_struct__thing_to_iterable];
+    memset(o, 0, sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   return o;
 }
 
-static void __pyx_tp_dealloc_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable(PyObject *o) {
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable *p = (struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable *)o;
+static void __pyx_tp_dealloc_10UAVReaders___pyx_scope_struct__thing_to_iterable(PyObject *o) {
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable *p = (struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable *)o;
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_thing);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable)))) {
-    __pyx_freelist_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable[__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable++] = ((struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable *)o);
+  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_10UAVReaders___pyx_scope_struct__thing_to_iterable < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable)))) {
+    __pyx_freelist_10UAVReaders___pyx_scope_struct__thing_to_iterable[__pyx_freecount_10UAVReaders___pyx_scope_struct__thing_to_iterable++] = ((struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
-static int __pyx_tp_traverse_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_10UAVReaders___pyx_scope_struct__thing_to_iterable(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable *p = (struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable *)o;
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable *p = (struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable *)o;
   if (p->__pyx_v_thing) {
     e = (*v)(p->__pyx_v_thing, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable(PyObject *o) {
+static int __pyx_tp_clear_10UAVReaders___pyx_scope_struct__thing_to_iterable(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable *p = (struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable *)o;
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable *p = (struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable *)o;
   tmp = ((PyObject*)p->__pyx_v_thing);
   p->__pyx_v_thing = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
-static PyTypeObject __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable = {
+static PyTypeObject __pyx_type_10UAVReaders___pyx_scope_struct__thing_to_iterable = {
   PyVarObject_HEAD_INIT(0, 0)
-  "UAVReaders.pyinterop.__pyx_scope_struct__thing_to_iterable", /*tp_name*/
-  sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable), /*tp_basicsize*/
+  "UAVReaders.__pyx_scope_struct__thing_to_iterable", /*tp_name*/
+  sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct__thing_to_iterable), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable, /*tp_dealloc*/
+  __pyx_tp_dealloc_10UAVReaders___pyx_scope_struct__thing_to_iterable, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -20853,31 +20853,31 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable, /*tp_traverse*/
-  __pyx_tp_clear_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable, /*tp_clear*/
+  __pyx_tp_traverse_10UAVReaders___pyx_scope_struct__thing_to_iterable, /*tp_traverse*/
+  __pyx_tp_clear_10UAVReaders___pyx_scope_struct__thing_to_iterable, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable, /*tp_new*/
+  __pyx_tp_new_10UAVReaders___pyx_scope_struct__thing_to_iterable, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -20893,51 +20893,51 @@
   0, /*tp_print*/
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
-static struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile *__pyx_freelist_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile[8];
-static int __pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile = 0;
+static struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile *__pyx_freelist_10UAVReaders___pyx_scope_struct_1_readFile[8];
+static int __pyx_freecount_10UAVReaders___pyx_scope_struct_1_readFile = 0;
 
-static PyObject *__pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_10UAVReaders___pyx_scope_struct_1_readFile(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile)))) {
-    o = (PyObject*)__pyx_freelist_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile[--__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile];
-    memset(o, 0, sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile));
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_10UAVReaders___pyx_scope_struct_1_readFile > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile)))) {
+    o = (PyObject*)__pyx_freelist_10UAVReaders___pyx_scope_struct_1_readFile[--__pyx_freecount_10UAVReaders___pyx_scope_struct_1_readFile];
+    memset(o, 0, sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   return o;
 }
 
-static void __pyx_tp_dealloc_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile(PyObject *o) {
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile *p = (struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile *)o;
+static void __pyx_tp_dealloc_10UAVReaders___pyx_scope_struct_1_readFile(PyObject *o) {
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile *p = (struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile *)o;
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_outer_scope);
   Py_CLEAR(p->__pyx_v_data);
   Py_CLEAR(p->__pyx_v_f);
   Py_CLEAR(p->__pyx_t_0);
   Py_CLEAR(p->__pyx_t_1);
   Py_CLEAR(p->__pyx_t_2);
   Py_CLEAR(p->__pyx_t_3);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile)))) {
-    __pyx_freelist_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile[__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile++] = ((struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile *)o);
+  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_10UAVReaders___pyx_scope_struct_1_readFile < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile)))) {
+    __pyx_freelist_10UAVReaders___pyx_scope_struct_1_readFile[__pyx_freecount_10UAVReaders___pyx_scope_struct_1_readFile++] = ((struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
-static int __pyx_tp_traverse_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_10UAVReaders___pyx_scope_struct_1_readFile(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile *p = (struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile *)o;
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile *p = (struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile *)o;
   if (p->__pyx_outer_scope) {
     e = (*v)(((PyObject *)p->__pyx_outer_scope), a); if (e) return e;
   }
   if (p->__pyx_v_data) {
     e = (*v)(p->__pyx_v_data, a); if (e) return e;
   }
   if (p->__pyx_v_f) {
@@ -20954,20 +20954,20 @@
   }
   if (p->__pyx_t_3) {
     e = (*v)(p->__pyx_t_3, a); if (e) return e;
   }
   return 0;
 }
 
-static PyTypeObject __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile = {
+static PyTypeObject __pyx_type_10UAVReaders___pyx_scope_struct_1_readFile = {
   PyVarObject_HEAD_INIT(0, 0)
-  "UAVReaders.pyinterop.__pyx_scope_struct_1_readFile", /*tp_name*/
-  sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile), /*tp_basicsize*/
+  "UAVReaders.__pyx_scope_struct_1_readFile", /*tp_name*/
+  sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct_1_readFile), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile, /*tp_dealloc*/
+  __pyx_tp_dealloc_10UAVReaders___pyx_scope_struct_1_readFile, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -20986,15 +20986,15 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile, /*tp_traverse*/
+  __pyx_tp_traverse_10UAVReaders___pyx_scope_struct_1_readFile, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
@@ -21002,15 +21002,15 @@
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile, /*tp_new*/
+  __pyx_tp_new_10UAVReaders___pyx_scope_struct_1_readFile, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -21026,48 +21026,48 @@
   0, /*tp_print*/
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
-static struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ *__pyx_freelist_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__[8];
-static int __pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ = 0;
+static struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__ *__pyx_freelist_10UAVReaders___pyx_scope_struct_2___call__[8];
+static int __pyx_freecount_10UAVReaders___pyx_scope_struct_2___call__ = 0;
 
-static PyObject *__pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_10UAVReaders___pyx_scope_struct_2___call__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__)))) {
-    o = (PyObject*)__pyx_freelist_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__[--__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__];
-    memset(o, 0, sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__));
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_10UAVReaders___pyx_scope_struct_2___call__ > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__)))) {
+    o = (PyObject*)__pyx_freelist_10UAVReaders___pyx_scope_struct_2___call__[--__pyx_freecount_10UAVReaders___pyx_scope_struct_2___call__];
+    memset(o, 0, sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   return o;
 }
 
-static void __pyx_tp_dealloc_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__(PyObject *o) {
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ *p = (struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ *)o;
+static void __pyx_tp_dealloc_10UAVReaders___pyx_scope_struct_2___call__(PyObject *o) {
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__ *p = (struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__ *)o;
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_p);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_v_thing);
   Py_CLEAR(p->__pyx_t_0);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__)))) {
-    __pyx_freelist_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__[__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__++] = ((struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ *)o);
+  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_10UAVReaders___pyx_scope_struct_2___call__ < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__)))) {
+    __pyx_freelist_10UAVReaders___pyx_scope_struct_2___call__[__pyx_freecount_10UAVReaders___pyx_scope_struct_2___call__++] = ((struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__ *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
-static int __pyx_tp_traverse_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_10UAVReaders___pyx_scope_struct_2___call__(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ *p = (struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ *)o;
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__ *p = (struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__ *)o;
   if (p->__pyx_v_p) {
     e = (*v)(((PyObject *)p->__pyx_v_p), a); if (e) return e;
   }
   if (p->__pyx_v_self) {
     e = (*v)(((PyObject *)p->__pyx_v_self), a); if (e) return e;
   }
   if (p->__pyx_v_thing) {
@@ -21075,20 +21075,20 @@
   }
   if (p->__pyx_t_0) {
     e = (*v)(p->__pyx_t_0, a); if (e) return e;
   }
   return 0;
 }
 
-static PyTypeObject __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ = {
+static PyTypeObject __pyx_type_10UAVReaders___pyx_scope_struct_2___call__ = {
   PyVarObject_HEAD_INIT(0, 0)
-  "UAVReaders.pyinterop.__pyx_scope_struct_2___call__", /*tp_name*/
-  sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__), /*tp_basicsize*/
+  "UAVReaders.__pyx_scope_struct_2___call__", /*tp_name*/
+  sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct_2___call__), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__, /*tp_dealloc*/
+  __pyx_tp_dealloc_10UAVReaders___pyx_scope_struct_2___call__, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -21107,15 +21107,15 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__, /*tp_traverse*/
+  __pyx_tp_traverse_10UAVReaders___pyx_scope_struct_2___call__, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
@@ -21123,15 +21123,15 @@
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__, /*tp_new*/
+  __pyx_tp_new_10UAVReaders___pyx_scope_struct_2___call__, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -21147,48 +21147,48 @@
   0, /*tp_print*/
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
-static struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ *__pyx_freelist_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__[8];
-static int __pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ = 0;
+static struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__ *__pyx_freelist_10UAVReaders___pyx_scope_struct_3___call__[8];
+static int __pyx_freecount_10UAVReaders___pyx_scope_struct_3___call__ = 0;
 
-static PyObject *__pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+static PyObject *__pyx_tp_new_10UAVReaders___pyx_scope_struct_3___call__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
-  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__)))) {
-    o = (PyObject*)__pyx_freelist_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__[--__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__];
-    memset(o, 0, sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__));
+  if (CYTHON_COMPILING_IN_CPYTHON && likely((__pyx_freecount_10UAVReaders___pyx_scope_struct_3___call__ > 0) & (t->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__)))) {
+    o = (PyObject*)__pyx_freelist_10UAVReaders___pyx_scope_struct_3___call__[--__pyx_freecount_10UAVReaders___pyx_scope_struct_3___call__];
+    memset(o, 0, sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else {
     o = (*t->tp_alloc)(t, 0);
     if (unlikely(!o)) return 0;
   }
   return o;
 }
 
-static void __pyx_tp_dealloc_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__(PyObject *o) {
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ *p = (struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ *)o;
+static void __pyx_tp_dealloc_10UAVReaders___pyx_scope_struct_3___call__(PyObject *o) {
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__ *p = (struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__ *)o;
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_p);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_v_thing);
   Py_CLEAR(p->__pyx_t_0);
-  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__)))) {
-    __pyx_freelist_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__[__pyx_freecount_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__++] = ((struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ *)o);
+  if (CYTHON_COMPILING_IN_CPYTHON && ((__pyx_freecount_10UAVReaders___pyx_scope_struct_3___call__ < 8) & (Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__)))) {
+    __pyx_freelist_10UAVReaders___pyx_scope_struct_3___call__[__pyx_freecount_10UAVReaders___pyx_scope_struct_3___call__++] = ((struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__ *)o);
   } else {
     (*Py_TYPE(o)->tp_free)(o);
   }
 }
 
-static int __pyx_tp_traverse_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_10UAVReaders___pyx_scope_struct_3___call__(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ *p = (struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ *)o;
+  struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__ *p = (struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__ *)o;
   if (p->__pyx_v_p) {
     e = (*v)(((PyObject *)p->__pyx_v_p), a); if (e) return e;
   }
   if (p->__pyx_v_self) {
     e = (*v)(((PyObject *)p->__pyx_v_self), a); if (e) return e;
   }
   if (p->__pyx_v_thing) {
@@ -21196,20 +21196,20 @@
   }
   if (p->__pyx_t_0) {
     e = (*v)(p->__pyx_t_0, a); if (e) return e;
   }
   return 0;
 }
 
-static PyTypeObject __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ = {
+static PyTypeObject __pyx_type_10UAVReaders___pyx_scope_struct_3___call__ = {
   PyVarObject_HEAD_INIT(0, 0)
-  "UAVReaders.pyinterop.__pyx_scope_struct_3___call__", /*tp_name*/
-  sizeof(struct __pyx_obj_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__), /*tp_basicsize*/
+  "UAVReaders.__pyx_scope_struct_3___call__", /*tp_name*/
+  sizeof(struct __pyx_obj_10UAVReaders___pyx_scope_struct_3___call__), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__, /*tp_dealloc*/
+  __pyx_tp_dealloc_10UAVReaders___pyx_scope_struct_3___call__, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -21228,15 +21228,15 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__, /*tp_traverse*/
+  __pyx_tp_traverse_10UAVReaders___pyx_scope_struct_3___call__, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   0, /*tp_methods*/
   0, /*tp_members*/
@@ -21244,15 +21244,15 @@
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__, /*tp_new*/
+  __pyx_tp_new_10UAVReaders___pyx_scope_struct_3___call__, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -21390,15 +21390,15 @@
   #endif
   __pyx_array_getbuffer, /*bf_getbuffer*/
   0, /*bf_releasebuffer*/
 };
 
 static PyTypeObject __pyx_type___pyx_array = {
   PyVarObject_HEAD_INIT(0, 0)
-  "UAVReaders.pyinterop.array", /*tp_name*/
+  "UAVReaders.array", /*tp_name*/
   sizeof(struct __pyx_array_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_array, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -21512,15 +21512,15 @@
   {"__reduce_cython__", (PyCFunction)__pyx_pw___pyx_MemviewEnum_1__reduce_cython__, METH_NOARGS, 0},
   {"__setstate_cython__", (PyCFunction)__pyx_pw___pyx_MemviewEnum_3__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type___pyx_MemviewEnum = {
   PyVarObject_HEAD_INIT(0, 0)
-  "UAVReaders.pyinterop.Enum", /*tp_name*/
+  "UAVReaders.Enum", /*tp_name*/
   sizeof(struct __pyx_MemviewEnum_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_Enum, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -21776,15 +21776,15 @@
   #endif
   __pyx_memoryview_getbuffer, /*bf_getbuffer*/
   0, /*bf_releasebuffer*/
 };
 
 static PyTypeObject __pyx_type___pyx_memoryview = {
   PyVarObject_HEAD_INIT(0, 0)
-  "UAVReaders.pyinterop.memoryview", /*tp_name*/
+  "UAVReaders.memoryview", /*tp_name*/
   sizeof(struct __pyx_memoryview_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_memoryview, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -21917,15 +21917,15 @@
 static struct PyGetSetDef __pyx_getsets__memoryviewslice[] = {
   {(char *)"base", __pyx_getprop___pyx_memoryviewslice_base, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
 static PyTypeObject __pyx_type___pyx_memoryviewslice = {
   PyVarObject_HEAD_INIT(0, 0)
-  "UAVReaders.pyinterop._memoryviewslice", /*tp_name*/
+  "UAVReaders._memoryviewslice", /*tp_name*/
   sizeof(struct __pyx_memoryviewslice_obj), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc__memoryviewslice, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -22002,25 +22002,25 @@
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_pyinterop(PyObject* module); /*proto*/
+static int __pyx_pymod_exec_UAVReaders(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_pyinterop},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_UAVReaders},
   {0, NULL}
 };
 #endif
 
 static struct PyModuleDef __pyx_moduledef = {
     PyModuleDef_HEAD_INIT,
-    "pyinterop",
+    "UAVReaders",
     __pyx_k_Pyinterop_pyx_Contributors_Chri, /* m_doc */
   #if CYTHON_PEP489_MULTI_PHASE_INIT
     0, /* m_size */
   #else
     -1, /* m_size */
   #endif
     __pyx_methods /* m_methods */,
@@ -22062,15 +22062,15 @@
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
   {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
   {&__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
-  {&__pyx_n_s_UAVReaders_pyinterop, __pyx_k_UAVReaders_pyinterop, sizeof(__pyx_k_UAVReaders_pyinterop), 0, 0, 1, 1},
+  {&__pyx_n_s_UAVReaders, __pyx_k_UAVReaders, sizeof(__pyx_k_UAVReaders), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_UnicodeDecodeError, __pyx_k_UnicodeDecodeError, sizeof(__pyx_k_UnicodeDecodeError), 0, 0, 1, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
@@ -22205,26 +22205,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "UAVReaders/pyinterop.pyx":275
+  /* "pyinterop.pyx":275
  *     elif type(thing) == str:
  *         def readFile():
  *             with open(thing, "rb") as f:             # <<<<<<<<<<<<<<
  *                 data = f.read(512)
  *                 while len(data) > 0:
  */
   __pyx_tuple__4 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 275, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "UAVReaders/pyinterop.pyx":274
+  /* "pyinterop.pyx":274
  *         return thing
  *     elif type(thing) == str:
  *         def readFile():             # <<<<<<<<<<<<<<
  *             with open(thing, "rb") as f:
  *                 data = f.read(512)
  */
   __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_s_f, __pyx_n_s_data); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 274, __pyx_L1_error)
@@ -22461,15 +22461,15 @@
   __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
   __pyx_tuple__29 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
 
-  /* "UAVReaders/pyinterop.pyx":259
+  /* "pyinterop.pyx":259
  *         return self.packet_type
  * 
  * def thing_to_iterable(thing):             # <<<<<<<<<<<<<<
  *     """
  *     Converts certain python objects into
  */
   __pyx_tuple__30 = PyTuple_Pack(3, __pyx_n_s_thing, __pyx_n_s_readFile, __pyx_n_s_readFile); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 259, __pyx_L1_error)
@@ -22602,80 +22602,80 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  __pyx_vtabptr_10UAVReaders_9pyinterop_packet = &__pyx_vtable_10UAVReaders_9pyinterop_packet;
-  __pyx_vtable_10UAVReaders_9pyinterop_packet.secret_real_init = (PyObject *(*)(struct __pyx_obj_10UAVReaders_9pyinterop_packet *, introspect::Struct *, std::string))__pyx_f_10UAVReaders_9pyinterop_6packet_secret_real_init;
-  __pyx_type_10UAVReaders_9pyinterop_packet.tp_base = (&PyDict_Type);
-  if (PyType_Ready(&__pyx_type_10UAVReaders_9pyinterop_packet) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_vtabptr_10UAVReaders_packet = &__pyx_vtable_10UAVReaders_packet;
+  __pyx_vtable_10UAVReaders_packet.secret_real_init = (PyObject *(*)(struct __pyx_obj_10UAVReaders_packet *, introspect::Struct *, std::string))__pyx_f_10UAVReaders_6packet_secret_real_init;
+  __pyx_type_10UAVReaders_packet.tp_base = (&PyDict_Type);
+  if (PyType_Ready(&__pyx_type_10UAVReaders_packet) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_10UAVReaders_9pyinterop_packet.tp_print = 0;
+  __pyx_type_10UAVReaders_packet.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10UAVReaders_9pyinterop_packet.tp_dictoffset && __pyx_type_10UAVReaders_9pyinterop_packet.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_10UAVReaders_9pyinterop_packet.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10UAVReaders_packet.tp_dictoffset && __pyx_type_10UAVReaders_packet.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_10UAVReaders_packet.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_10UAVReaders_9pyinterop_packet.tp_dict, __pyx_vtabptr_10UAVReaders_9pyinterop_packet) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_packet, (PyObject *)&__pyx_type_10UAVReaders_9pyinterop_packet) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10UAVReaders_9pyinterop_packet) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
-  __pyx_ptype_10UAVReaders_9pyinterop_packet = &__pyx_type_10UAVReaders_9pyinterop_packet;
-  if (PyType_Ready(&__pyx_type_10UAVReaders_9pyinterop_mavlink_reader) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_10UAVReaders_packet.tp_dict, __pyx_vtabptr_10UAVReaders_packet) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_packet, (PyObject *)&__pyx_type_10UAVReaders_packet) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10UAVReaders_packet) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_ptype_10UAVReaders_packet = &__pyx_type_10UAVReaders_packet;
+  if (PyType_Ready(&__pyx_type_10UAVReaders_mavlink_reader) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_10UAVReaders_9pyinterop_mavlink_reader.tp_print = 0;
+  __pyx_type_10UAVReaders_mavlink_reader.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10UAVReaders_9pyinterop_mavlink_reader.tp_dictoffset && __pyx_type_10UAVReaders_9pyinterop_mavlink_reader.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_10UAVReaders_9pyinterop_mavlink_reader.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10UAVReaders_mavlink_reader.tp_dictoffset && __pyx_type_10UAVReaders_mavlink_reader.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_10UAVReaders_mavlink_reader.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_mavlink_reader, (PyObject *)&__pyx_type_10UAVReaders_9pyinterop_mavlink_reader) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10UAVReaders_9pyinterop_mavlink_reader) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
-  __pyx_ptype_10UAVReaders_9pyinterop_mavlink_reader = &__pyx_type_10UAVReaders_9pyinterop_mavlink_reader;
-  if (PyType_Ready(&__pyx_type_10UAVReaders_9pyinterop_data_flash_reader) < 0) __PYX_ERR(0, 344, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_mavlink_reader, (PyObject *)&__pyx_type_10UAVReaders_mavlink_reader) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10UAVReaders_mavlink_reader) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_ptype_10UAVReaders_mavlink_reader = &__pyx_type_10UAVReaders_mavlink_reader;
+  if (PyType_Ready(&__pyx_type_10UAVReaders_data_flash_reader) < 0) __PYX_ERR(0, 344, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_10UAVReaders_9pyinterop_data_flash_reader.tp_print = 0;
+  __pyx_type_10UAVReaders_data_flash_reader.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10UAVReaders_9pyinterop_data_flash_reader.tp_dictoffset && __pyx_type_10UAVReaders_9pyinterop_data_flash_reader.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_10UAVReaders_9pyinterop_data_flash_reader.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10UAVReaders_data_flash_reader.tp_dictoffset && __pyx_type_10UAVReaders_data_flash_reader.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_10UAVReaders_data_flash_reader.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_data_flash_reader, (PyObject *)&__pyx_type_10UAVReaders_9pyinterop_data_flash_reader) < 0) __PYX_ERR(0, 344, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10UAVReaders_9pyinterop_data_flash_reader) < 0) __PYX_ERR(0, 344, __pyx_L1_error)
-  __pyx_ptype_10UAVReaders_9pyinterop_data_flash_reader = &__pyx_type_10UAVReaders_9pyinterop_data_flash_reader;
-  if (PyType_Ready(&__pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_data_flash_reader, (PyObject *)&__pyx_type_10UAVReaders_data_flash_reader) < 0) __PYX_ERR(0, 344, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10UAVReaders_data_flash_reader) < 0) __PYX_ERR(0, 344, __pyx_L1_error)
+  __pyx_ptype_10UAVReaders_data_flash_reader = &__pyx_type_10UAVReaders_data_flash_reader;
+  if (PyType_Ready(&__pyx_type_10UAVReaders___pyx_scope_struct__thing_to_iterable) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable.tp_print = 0;
+  __pyx_type_10UAVReaders___pyx_scope_struct__thing_to_iterable.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable.tp_dictoffset && __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10UAVReaders___pyx_scope_struct__thing_to_iterable.tp_dictoffset && __pyx_type_10UAVReaders___pyx_scope_struct__thing_to_iterable.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_10UAVReaders___pyx_scope_struct__thing_to_iterable.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  __pyx_ptype_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable = &__pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct__thing_to_iterable;
-  if (PyType_Ready(&__pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile) < 0) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_ptype_10UAVReaders___pyx_scope_struct__thing_to_iterable = &__pyx_type_10UAVReaders___pyx_scope_struct__thing_to_iterable;
+  if (PyType_Ready(&__pyx_type_10UAVReaders___pyx_scope_struct_1_readFile) < 0) __PYX_ERR(0, 274, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile.tp_print = 0;
+  __pyx_type_10UAVReaders___pyx_scope_struct_1_readFile.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile.tp_dictoffset && __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10UAVReaders___pyx_scope_struct_1_readFile.tp_dictoffset && __pyx_type_10UAVReaders___pyx_scope_struct_1_readFile.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_10UAVReaders___pyx_scope_struct_1_readFile.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  __pyx_ptype_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile = &__pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_1_readFile;
-  if (PyType_Ready(&__pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__) < 0) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_ptype_10UAVReaders___pyx_scope_struct_1_readFile = &__pyx_type_10UAVReaders___pyx_scope_struct_1_readFile;
+  if (PyType_Ready(&__pyx_type_10UAVReaders___pyx_scope_struct_2___call__) < 0) __PYX_ERR(0, 335, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__.tp_print = 0;
+  __pyx_type_10UAVReaders___pyx_scope_struct_2___call__.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__.tp_dictoffset && __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10UAVReaders___pyx_scope_struct_2___call__.tp_dictoffset && __pyx_type_10UAVReaders___pyx_scope_struct_2___call__.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_10UAVReaders___pyx_scope_struct_2___call__.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  __pyx_ptype_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__ = &__pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_2___call__;
-  if (PyType_Ready(&__pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__) < 0) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_ptype_10UAVReaders___pyx_scope_struct_2___call__ = &__pyx_type_10UAVReaders___pyx_scope_struct_2___call__;
+  if (PyType_Ready(&__pyx_type_10UAVReaders___pyx_scope_struct_3___call__) < 0) __PYX_ERR(0, 396, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__.tp_print = 0;
+  __pyx_type_10UAVReaders___pyx_scope_struct_3___call__.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__.tp_dictoffset && __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10UAVReaders___pyx_scope_struct_3___call__.tp_dictoffset && __pyx_type_10UAVReaders___pyx_scope_struct_3___call__.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_10UAVReaders___pyx_scope_struct_3___call__.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  __pyx_ptype_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__ = &__pyx_type_10UAVReaders_9pyinterop___pyx_scope_struct_3___call__;
+  __pyx_ptype_10UAVReaders___pyx_scope_struct_3___call__ = &__pyx_type_10UAVReaders___pyx_scope_struct_3___call__;
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
   if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 106, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
   #endif
   if (__Pyx_SetVtable(__pyx_type___pyx_array.tp_dict, __pyx_vtabptr_array) < 0) __PYX_ERR(1, 106, __pyx_L1_error)
@@ -22769,19 +22769,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC initpyinterop(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC initpyinterop(void)
+__Pyx_PyMODINIT_FUNC initUAVReaders(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC initUAVReaders(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit_pyinterop(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit_pyinterop(void)
+__Pyx_PyMODINIT_FUNC PyInit_UAVReaders(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit_UAVReaders(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -22840,43 +22840,43 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec_pyinterop(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec_UAVReaders(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   static PyThread_type_lock __pyx_t_2[8];
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module 'pyinterop' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module 'UAVReaders' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_pyinterop(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_UAVReaders(void)", 0);
   if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -22905,15 +22905,15 @@
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("pyinterop", __pyx_methods, __pyx_k_Pyinterop_pyx_Contributors_Chri, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("UAVReaders", __pyx_methods, __pyx_k_Pyinterop_pyx_Contributors_Chri, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
@@ -22923,22 +22923,22 @@
   Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_UAVReaders__pyinterop) {
+  if (__pyx_module_is_main_UAVReaders) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "UAVReaders.pyinterop")) {
-      if (unlikely(PyDict_SetItemString(modules, "UAVReaders.pyinterop", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "UAVReaders")) {
+      if (unlikely(PyDict_SetItemString(modules, "UAVReaders", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -22951,27 +22951,27 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "UAVReaders/pyinterop.pyx":259
+  /* "pyinterop.pyx":259
  *         return self.packet_type
  * 
  * def thing_to_iterable(thing):             # <<<<<<<<<<<<<<
  *     """
  *     Converts certain python objects into
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10UAVReaders_9pyinterop_1thing_to_iterable, NULL, __pyx_n_s_UAVReaders_pyinterop); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10UAVReaders_1thing_to_iterable, NULL, __pyx_n_s_UAVReaders); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_thing_to_iterable, __pyx_t_1) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "UAVReaders/pyinterop.pyx":1
+  /* "pyinterop.pyx":1
  * # distutils: language=c++             # <<<<<<<<<<<<<<
  * """
  * Pyinterop.pyx
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -23133,19 +23133,19 @@
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init UAVReaders.pyinterop", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init UAVReaders", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init UAVReaders.pyinterop");
+    PyErr_SetString(PyExc_ImportError, "init UAVReaders");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
```

### Comparing `UAVReaders-0.5.5/readers.cpp` & `UAVReaders-0.5.6/readers.cpp`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/readers.h` & `UAVReaders-0.5.6/readers.h`

 * *Files identical despite different names*

### Comparing `UAVReaders-0.5.5/setup.py` & `UAVReaders-0.5.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,13 +15,13 @@
         sources=["pyinterop.cpp"] + extrafiles
     )
 ]
 
 setup(
     ext_modules = cythonize(ext_modules),
     name="UAVReaders",
-    version="0.5.5",
+    version="0.5.6",
     author="Christian Clifford",
     author_email="cjclifford@alaska.edu",
     description="Parsers for UAV/Aerial Drone-related formats like MavLink and DataFlash",
     py_modules=[]
 )
```

### Comparing `UAVReaders-0.5.5/table.h` & `UAVReaders-0.5.6/table.h`

 * *Files identical despite different names*

