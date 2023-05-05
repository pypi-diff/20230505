# Comparing `tmp/velbus-aio-2023.2.0.tar.gz` & `tmp/velbus-aio-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velbus-aio-2023.2.0.tar", last modified: Mon Feb  6 16:28:48 2023, max compression
+gzip compressed data, was "velbus-aio-2023.5.0.tar", last modified: Fri May  5 17:41:24 2023, max compression
```

## Comparing `velbus-aio-2023.2.0.tar` & `velbus-aio-2023.5.0.tar`

### file list

```diff
@@ -1,121 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 16:28:48.836973 velbus-aio-2023.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-02-06 16:28:48.836973 velbus-aio-2023.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 16:28:48.824972 velbus-aio-2023.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/examples/discover.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/examples/load_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/examples/read_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/examples/read_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 16:28:48.836973 velbus-aio-2023.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 16:28:48.824972 velbus-aio-2023.2.0/velbus_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-02-06 16:28:48.000000 velbus-aio-2023.2.0/velbus_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-02-06 16:28:48.000000 velbus-aio-2023.2.0/velbus_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 16:28:48.000000 velbus-aio-2023.2.0/velbus_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 16:28:48.000000 velbus-aio-2023.2.0/velbus_aio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-06 16:28:48.000000 velbus-aio-2023.2.0/velbus_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-06 16:28:48.000000 velbus-aio-2023.2.0/velbus_aio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 16:28:48.824972 velbus-aio-2023.2.0/velbusaio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/command_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 16:28:48.836973 velbus-aio-2023.2.0/velbusaio/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/blind_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/bus_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/bus_error_counter_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/bus_error_counter_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/bus_off.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/channel_name_part1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/channel_name_part2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/channel_name_part3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/channel_name_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/clear_led.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/counter_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/counter_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/cover_down.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/cover_off.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/cover_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/cover_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/dali_device_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/dali_device_settings_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/dali_dim_value_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/dimmer_channel_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/dimmer_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/edge_set_custom_color.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/fast_blinking_led.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/forced_off.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/forced_on.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/interface_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/ir_receiver_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/kwh_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/light_value_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/memo_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/memory_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/memory_data_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/memory_dump_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/meteo_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/module_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/module_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/module_subtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/module_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/module_type_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/push_button_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/read_data_block_from_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/read_data_from_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/realtime_clock_status_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/receive_buffer_full.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/receive_ready.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/relay_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/restore_dimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/select_program.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/sensor_settings_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/sensor_temp_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/sensor_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/set_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/set_daylight_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/set_dimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/set_led.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/set_realtime_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/set_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/slider_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/slow_blinking_led.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/start_relay_blinking_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/start_relay_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/switch_relay_off.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/switch_relay_on.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/switch_to_comfort.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/switch_to_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/switch_to_night.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/switch_to_safe.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/temp_sensor_settings_part1.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/temp_sensor_settings_part2.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/temp_sensor_settings_part3.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/temp_sensor_settings_part4.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/temp_sensor_settings_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/temp_sensor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/temp_set_cooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/temp_set_heating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/update_led_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/very_fast_blinking_led.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/write_data_to_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/write_memory_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/messages/write_module_address_and_serial_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    34676 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 16:28:48.836973 velbus-aio-2023.2.0/velbusaio/moduleprotocol/
--rw-r--r--   0 runner    (1001) docker     (123)   883766 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/moduleprotocol/protocol.json
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/raw_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-02-06 16:28:37.000000 velbus-aio-2023.2.0/velbusaio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:41:24.776804 velbus-aio-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-05 17:41:24.776804 velbus-aio-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:41:24.776804 velbus-aio-2023.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:41:24.764804 velbus-aio-2023.5.0/velbus_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-05 17:41:24.000000 velbus-aio-2023.5.0/velbus_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-05 17:41:24.000000 velbus-aio-2023.5.0/velbus_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:41:24.000000 velbus-aio-2023.5.0/velbus_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:41:24.000000 velbus-aio-2023.5.0/velbus_aio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 17:41:24.000000 velbus-aio-2023.5.0/velbus_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 17:41:24.000000 velbus-aio-2023.5.0/velbus_aio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:41:24.768804 velbus-aio-2023.5.0/velbusaio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22129 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/command_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:41:24.776804 velbus-aio-2023.5.0/velbusaio/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/blind_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/bus_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/bus_error_counter_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/bus_error_counter_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/bus_off.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/channel_name_part1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/channel_name_part2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/channel_name_part3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/channel_name_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/clear_led.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/counter_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/counter_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/cover_down.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/cover_off.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/cover_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/cover_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/dali_device_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/dali_device_settings_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/dali_dim_value_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/dimmer_channel_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/dimmer_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/edge_set_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/edge_set_custom_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/fast_blinking_led.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/forced_off.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/forced_on.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/interface_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/ir_receiver_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/kwh_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/light_value_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/memo_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/memory_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/memory_data_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/memory_dump_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/meteo_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/module_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/module_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/module_subtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/module_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/module_type_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/push_button_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/read_data_block_from_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/read_data_from_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/realtime_clock_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/receive_buffer_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/receive_ready.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/relay_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/restore_dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/select_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/sensor_settings_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/sensor_temp_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/sensor_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/set_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/set_daylight_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/set_dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/set_led.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/set_realtime_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/set_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/slider_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/slow_blinking_led.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/start_relay_blinking_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/start_relay_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/switch_relay_off.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/switch_relay_on.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/switch_to_comfort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/switch_to_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/switch_to_night.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/switch_to_safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_set_cooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/temp_set_heating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/update_led_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/very_fast_blinking_led.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/write_data_to_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/write_memory_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/messages/write_module_address_and_serial_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34889 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:41:24.776804 velbus-aio-2023.5.0/velbusaio/moduleprotocol/
+-rw-r--r--   0 runner    (1001) docker     (123)   883766 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/moduleprotocol/protocol.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/raw_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-05 17:41:15.000000 velbus-aio-2023.5.0/velbusaio/util.py
```

### Comparing `velbus-aio-2023.2.0/LICENSE` & `velbus-aio-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/PKG-INFO` & `velbus-aio-2023.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velbus-aio
-Version: 2023.2.0
+Version: 2023.5.0
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/Cereal2nd/velbus-aio
 Project-URL: Bug Reports, https://github.com/Cereal2nd/velbus-aio/issues
 Keywords: home,velbus,automation
 Platform: any
```

### Comparing `velbus-aio-2023.2.0/README.md` & `velbus-aio-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/pyproject.toml` & `velbus-aio-2023.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name        = "velbus-aio"
-version     = "2023.2.0"
 license     = {text = "MIT"}
+version     = "2023.5.0"
 description = "Open-source home automation platform running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Maikel Punie", email = "maikel.punie@gmail.com"}
 ]
 keywords    = ["home", "velbus", "automation"]
 classifiers = [
@@ -39,8 +39,30 @@
 
 [tool.setuptools]
 platforms = ["any"]
 zip-safe  = false
 include-package-data = true
 
 [tool.setuptools.packages.find]
-exclude = ["tests", "tests.*"]
+exclude = ["tests", "tests.*", "examples"]
+
+[tool.bumpver]
+current_version = "2023.5.0"
+version_pattern = "YYYY.MM.INC0"
+commit_message = "bump version {old_version} -> {new_version}"
+commit = true
+tag = true
+push = true
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = [
+    'version = "{version}"',
+    'current_version = "{version}"',
+]
+"setup.py" = [
+    "{version}",
+    "{pep440_version}",
+]
+"README.md" = [
+    "{version}",
+    "{pep440_version}",
+]
```

### Comparing `velbus-aio-2023.2.0/velbus_aio.egg-info/PKG-INFO` & `velbus-aio-2023.5.0/velbus_aio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velbus-aio
-Version: 2023.2.0
+Version: 2023.5.0
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/Cereal2nd/velbus-aio
 Project-URL: Bug Reports, https://github.com/Cereal2nd/velbus-aio/issues
 Keywords: home,velbus,automation
 Platform: any
```

### Comparing `velbus-aio-2023.2.0/velbus_aio.egg-info/SOURCES.txt` & `velbus-aio-2023.5.0/velbus_aio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
-examples/discover.py
-examples/load_modules.py
-examples/read_bus.py
-examples/read_cache.py
 velbus_aio.egg-info/PKG-INFO
 velbus_aio.egg-info/SOURCES.txt
 velbus_aio.egg-info/dependency_links.txt
 velbus_aio.egg-info/not-zip-safe
 velbus_aio.egg-info/requires.txt
 velbus_aio.egg-info/top_level.txt
 velbusaio/__init__.py
@@ -47,14 +43,15 @@
 velbusaio/messages/cover_position.py
 velbusaio/messages/cover_up.py
 velbusaio/messages/dali_device_settings.py
 velbusaio/messages/dali_device_settings_request.py
 velbusaio/messages/dali_dim_value_status.py
 velbusaio/messages/dimmer_channel_status.py
 velbusaio/messages/dimmer_status.py
+velbusaio/messages/edge_set_color.py
 velbusaio/messages/edge_set_custom_color.py
 velbusaio/messages/fast_blinking_led.py
 velbusaio/messages/forced_off.py
 velbusaio/messages/forced_on.py
 velbusaio/messages/interface_status_request.py
 velbusaio/messages/ir_receiver_status.py
 velbusaio/messages/kwh_status.py
```

### Comparing `velbus-aio-2023.2.0/velbusaio/channels.py` & `velbus-aio-2023.5.0/velbusaio/channels.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     DEVICE_CLASS_TEMPERATURE,
     ENERGY_KILO_WATT_HOUR,
     TEMP_CELSIUS,
     VOLUME_CUBIC_METER_HOUR,
     VOLUME_LITERS_HOUR,
 )
 from velbusaio.message import Message
+from velbusaio.messages.edge_set_color import SetEdgeColorMessage, CustomColorPriority
 from velbusaio.messages.module_status import PROGRAM_SELECTION
 
 if TYPE_CHECKING:
     from velbusaio.module import Module
 
 
 class Channel:
@@ -271,14 +272,15 @@
     """
     A Button channel
     """
 
     _enabled = True
     _closed = False
     _led_state = None
+    _long = False
 
     def get_categories(self) -> list[str]:
         if self._enabled:
             return ["binary_sensor", "led", "button"]
         return []
 
     def is_closed(self) -> bool:
@@ -698,16 +700,50 @@
 
 
 class EdgeLit(Channel):
     """
     An EdgeLit channel
     """
 
-    # def get_categories(self):
-    #    return ["light"]
+    async def reset_color(self, left=True, top=True, right=True, bottom=True):
+        msg = SetEdgeColorMessage(self._address)
+        msg.apply_background_color = True
+        msg.color_idx = 0
+        msg.apply_to_left_edge = left
+        msg.apply_to_top_edge = top
+        msg.apply_to_right_edge = right
+        msg.apply_to_bottom_edge = bottom
+        msg.apply_to_all_pages = True
+        await self._writer(msg)
+
+    async def set_color(
+        self,
+        color_idx: int,
+        left=True,
+        top=True,
+        right=True,
+        bottom=True,
+        blinking=False,
+        priority=CustomColorPriority.LOW_PRIORITY,
+    ) -> None:
+        """
+        Send the turn off message
+        """
+
+        msg = SetEdgeColorMessage(self._address)
+        msg.apply_background_color = True
+        msg.background_blinking = blinking
+        msg.color_idx = color_idx
+        msg.apply_to_left_edge = left
+        msg.apply_to_top_edge = top
+        msg.apply_to_right_edge = right
+        msg.apply_to_bottom_edge = bottom
+        msg.apply_to_all_pages = True
+        msg.custom_color_priority = priority
+        await self._writer(msg)
 
 
 class Memo(Channel):
     """
     A Memo text
     """
```

### Comparing `velbus-aio-2023.2.0/velbusaio/command_registry.py` & `velbus-aio-2023.5.0/velbusaio/command_registry.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/const.py` & `velbus-aio-2023.5.0/velbusaio/const.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/controller.py` & `velbus-aio-2023.5.0/velbusaio/controller.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/discovery.py` & `velbus-aio-2023.5.0/velbusaio/discovery.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/handler.py` & `velbus-aio-2023.5.0/velbusaio/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             module_type = self._velbus.get_module(address).get_type()
             if commandRegistry.has_command(int(command_value), module_type):
                 command = commandRegistry.get_command(command_value, module_type)
                 msg = command()
                 msg.populate(priority, address, rtr, data)
                 self._log.debug(f"Received {msg}")
                 # send the message to the modules
-                await (self._velbus.get_module(msg.address)).on_message(msg)
+                await self._velbus.get_module(msg.address).on_message(msg)
             else:
                 self._log.warning(
                     "NOT FOUND IN command_registry: addr={} cmd={} packet={}".format(
                         address, command_value, ":".join(format(x, "02x") for x in data)
                     )
                 )
         elif self._scan_complete:
```

### Comparing `velbus-aio-2023.2.0/velbusaio/helpers.py` & `velbus-aio-2023.5.0/velbusaio/helpers.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/message.py` & `velbus-aio-2023.5.0/velbusaio/message.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/__init__.py` & `velbus-aio-2023.5.0/velbusaio/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/blind_status.py` & `velbus-aio-2023.5.0/velbusaio/messages/blind_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/bus_active.py` & `velbus-aio-2023.5.0/velbusaio/messages/bus_active.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/bus_error_counter_status.py` & `velbus-aio-2023.5.0/velbusaio/messages/bus_error_counter_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/bus_error_counter_status_request.py` & `velbus-aio-2023.5.0/velbusaio/messages/bus_error_counter_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/bus_off.py` & `velbus-aio-2023.5.0/velbusaio/messages/bus_off.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/channel_name_part1.py` & `velbus-aio-2023.5.0/velbusaio/messages/channel_name_part1.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/channel_name_part2.py` & `velbus-aio-2023.5.0/velbusaio/messages/channel_name_part2.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/channel_name_part3.py` & `velbus-aio-2023.5.0/velbusaio/messages/channel_name_part3.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/channel_name_request.py` & `velbus-aio-2023.5.0/velbusaio/messages/channel_name_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/clear_led.py` & `velbus-aio-2023.5.0/velbusaio/messages/clear_led.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/counter_status.py` & `velbus-aio-2023.5.0/velbusaio/messages/counter_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/counter_status_request.py` & `velbus-aio-2023.5.0/velbusaio/messages/counter_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/cover_down.py` & `velbus-aio-2023.5.0/velbusaio/messages/cover_down.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/cover_off.py` & `velbus-aio-2023.5.0/velbusaio/messages/cover_off.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/cover_position.py` & `velbus-aio-2023.5.0/velbusaio/messages/cover_position.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/cover_up.py` & `velbus-aio-2023.5.0/velbusaio/messages/cover_up.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/dali_device_settings.py` & `velbus-aio-2023.5.0/velbusaio/messages/dali_device_settings.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/dali_device_settings_request.py` & `velbus-aio-2023.5.0/velbusaio/messages/dali_device_settings_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/dali_dim_value_status.py` & `velbus-aio-2023.5.0/velbusaio/messages/dali_dim_value_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/dimmer_channel_status.py` & `velbus-aio-2023.5.0/velbusaio/messages/dimmer_channel_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/dimmer_status.py` & `velbus-aio-2023.5.0/velbusaio/messages/dimmer_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/edge_set_custom_color.py` & `velbus-aio-2023.5.0/velbusaio/messages/edge_set_custom_color.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0xD4
 
 
-@register(COMMAND_CODE)
+@register(COMMAND_CODE, ["VMBEL1", "VMBEL2", "VMBEL4", "VMBELO"])
 class EdgeSetCustomColor(Message):
     """
     send by:
-    received by: VMB4RYLD
+    received by: VMBEL1, VMBEL2, VMBEL4, VMBELO
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
         self.set_defaults(address)
         self.pallet = 31
         self.rgb = False
```

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/fast_blinking_led.py` & `velbus-aio-2023.5.0/velbusaio/messages/fast_blinking_led.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/forced_off.py` & `velbus-aio-2023.5.0/velbusaio/messages/forced_off.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/forced_on.py` & `velbus-aio-2023.5.0/velbusaio/messages/forced_on.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/interface_status_request.py` & `velbus-aio-2023.5.0/velbusaio/messages/interface_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/kwh_status.py` & `velbus-aio-2023.5.0/velbusaio/messages/kwh_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/light_value_request.py` & `velbus-aio-2023.5.0/velbusaio/messages/light_value_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/memo_text.py` & `velbus-aio-2023.5.0/velbusaio/messages/memo_text.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/memory_data.py` & `velbus-aio-2023.5.0/velbusaio/messages/memory_data.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/memory_data_block.py` & `velbus-aio-2023.5.0/velbusaio/messages/memory_data_block.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/memory_dump_request.py` & `velbus-aio-2023.5.0/velbusaio/messages/memory_dump_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/meteo_raw.py` & `velbus-aio-2023.5.0/velbusaio/messages/meteo_raw.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/module_status.py` & `velbus-aio-2023.5.0/velbusaio/messages/module_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/module_status_request.py` & `velbus-aio-2023.5.0/velbusaio/messages/module_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/module_subtype.py` & `velbus-aio-2023.5.0/velbusaio/messages/module_subtype.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/module_type.py` & `velbus-aio-2023.5.0/velbusaio/messages/module_type.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/module_type_request.py` & `velbus-aio-2023.5.0/velbusaio/messages/module_type_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/push_button_status.py` & `velbus-aio-2023.5.0/velbusaio/messages/push_button_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/read_data_block_from_memory.py` & `velbus-aio-2023.5.0/velbusaio/messages/read_data_block_from_memory.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/read_data_from_memory.py` & `velbus-aio-2023.5.0/velbusaio/messages/read_data_from_memory.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/realtime_clock_status_request.py` & `velbus-aio-2023.5.0/velbusaio/messages/realtime_clock_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/receive_buffer_full.py` & `velbus-aio-2023.5.0/velbusaio/messages/receive_buffer_full.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/receive_ready.py` & `velbus-aio-2023.5.0/velbusaio/messages/receive_ready.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/relay_status.py` & `velbus-aio-2023.5.0/velbusaio/messages/relay_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/restore_dimmer.py` & `velbus-aio-2023.5.0/velbusaio/messages/set_dimmer.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,62 +2,71 @@
 :author: Frank van Breugel
 """
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0x11
+COMMAND_CODE = 0x07
 
 
-@register(COMMAND_CODE)
-class RestoreDimmerMessage(Message):
+@register(COMMAND_CODE, ["VMBDME", "VMB4DC", "VMBDMI", "VMBDMI-R", "VMB1LED"])
+class SetDimmerMessage(Message):
     """
     send by:
     received by: VMBDME, VMB4DC
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
         self.dimmer_channels = []
+        self.dimmer_state = 0
+        self.dimmer_transitiontime = 0
         self.set_defaults(address)
 
     def set_defaults(self, address):
         if address is not None:
             self.set_address(address)
         self.set_high_priority()
         self.set_no_rtr()
 
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_high_priority(priority)
         self.needs_no_rtr(rtr)
-        self.needs_data(data, 1)
+        self.needs_data(data, 4)
         self.set_attributes(priority, address, rtr)
         self.dimmer_channels = self.byte_to_channels(data[0])
+        self.dimmer_state = data[1]
         self.dimmer_transitiontime = int.from_bytes(
             data[2:3], byteorder="big", signed=False
         )
 
     def data_to_binary(self):
         """
         :return: bytes
         """
         return bytes(
             [
                 COMMAND_CODE,
                 self.channels_to_byte(self.dimmer_channels),
-                0,
+                self.dimmer_state,
             ]
         ) + self.dimmer_transitiontime.to_bytes(2, byteorder="big", signed=False)
 
 
 @register(COMMAND_CODE, ["VMBDALI"])
-class RestoreDimmerMessage2(RestoreDimmerMessage):
+class SetDimmerMessage2(SetDimmerMessage):
+    """
+    send by:
+    received by: VMBDALI
+    """
+
     def byte_to_channels(self, byte: int) -> list[int]:
         return [byte]
 
-    def channels_to_byte(self, channels: list[int]) -> int:
-        assert len(channels) == 1
+    def channels_to_byte(self, channels) -> int:
+        if len(channels) != 1:
+            raise ValueError("We should have exact one channel")
         return channels[0]
```

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/select_program.py` & `velbus-aio-2023.5.0/velbusaio/messages/select_program.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/sensor_settings_request.py` & `velbus-aio-2023.5.0/velbusaio/messages/sensor_settings_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/sensor_temp_request.py` & `velbus-aio-2023.5.0/velbusaio/messages/sensor_temp_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/sensor_temperature.py` & `velbus-aio-2023.5.0/velbusaio/messages/sensor_temperature.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/set_date.py` & `velbus-aio-2023.5.0/velbusaio/messages/set_date.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/set_daylight_saving.py` & `velbus-aio-2023.5.0/velbusaio/messages/set_daylight_saving.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/set_dimmer.py` & `velbus-aio-2023.5.0/velbusaio/messages/restore_dimmer.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,70 +2,63 @@
 :author: Frank van Breugel
 """
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
-COMMAND_CODE = 0x07
+COMMAND_CODE = 0x11
 
 
-@register(COMMAND_CODE, ["VMBDME", "VMB4DC", "VMBDMI", "VMBDMI-R", "VMB1LED"])
-class SetDimmerMessage(Message):
+@register(COMMAND_CODE)
+class RestoreDimmerMessage(Message):
     """
     send by:
     received by: VMBDME, VMB4DC
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
         self.dimmer_channels = []
-        self.dimmer_state = 0
-        self.dimmer_transitiontime = 0
         self.set_defaults(address)
 
     def set_defaults(self, address):
         if address is not None:
             self.set_address(address)
         self.set_high_priority()
         self.set_no_rtr()
 
     def populate(self, priority, address, rtr, data):
         """
         :return: None
         """
         self.needs_high_priority(priority)
         self.needs_no_rtr(rtr)
-        self.needs_data(data, 4)
+        self.needs_data(data, 1)
         self.set_attributes(priority, address, rtr)
         self.dimmer_channels = self.byte_to_channels(data[0])
-        self.dimmer_state = data[1]
         self.dimmer_transitiontime = int.from_bytes(
             data[2:3], byteorder="big", signed=False
         )
 
     def data_to_binary(self):
         """
         :return: bytes
         """
         return bytes(
             [
                 COMMAND_CODE,
                 self.channels_to_byte(self.dimmer_channels),
-                self.dimmer_state,
+                0,
             ]
         ) + self.dimmer_transitiontime.to_bytes(2, byteorder="big", signed=False)
 
 
 @register(COMMAND_CODE, ["VMBDALI"])
-class SetDimmerMessage2(SetDimmerMessage):
-    """
-    send by:
-    received by: VMBDALI
-    """
-
+class RestoreDimmerMessage2(RestoreDimmerMessage):
     def byte_to_channels(self, byte: int) -> list[int]:
         return [byte]
 
-    def channels_to_byte(self, channels) -> int:
-        assert len(channels) == 1
+    def channels_to_byte(self, channels: list[int]) -> int:
+        if len(channels) != 1:
+            raise ValueError("We should have exact one channel")
         return channels[0]
```

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/set_led.py` & `velbus-aio-2023.5.0/velbusaio/messages/set_led.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/set_realtime_clock.py` & `velbus-aio-2023.5.0/velbusaio/messages/set_realtime_clock.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/set_temperature.py` & `velbus-aio-2023.5.0/velbusaio/messages/set_temperature.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/slider_status.py` & `velbus-aio-2023.5.0/velbusaio/messages/slider_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/slow_blinking_led.py` & `velbus-aio-2023.5.0/velbusaio/messages/slow_blinking_led.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/start_relay_blinking_timer.py` & `velbus-aio-2023.5.0/velbusaio/messages/start_relay_blinking_timer.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/start_relay_timer.py` & `velbus-aio-2023.5.0/velbusaio/messages/start_relay_timer.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/switch_relay_off.py` & `velbus-aio-2023.5.0/velbusaio/messages/switch_relay_off.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/switch_relay_on.py` & `velbus-aio-2023.5.0/velbusaio/messages/switch_relay_on.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/switch_to_comfort.py` & `velbus-aio-2023.5.0/velbusaio/messages/switch_to_comfort.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/switch_to_day.py` & `velbus-aio-2023.5.0/velbusaio/messages/switch_to_day.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/switch_to_night.py` & `velbus-aio-2023.5.0/velbusaio/messages/switch_to_night.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/switch_to_safe.py` & `velbus-aio-2023.5.0/velbusaio/messages/switch_to_safe.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/temp_sensor_settings_part1.py` & `velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part1.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/temp_sensor_settings_part2.py` & `velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part2.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/temp_sensor_settings_part3.py` & `velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part3.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/temp_sensor_settings_part4.py` & `velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_part4.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/temp_sensor_settings_request.py` & `velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_settings_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/temp_sensor_status.py` & `velbus-aio-2023.5.0/velbusaio/messages/temp_sensor_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/temp_set_cooling.py` & `velbus-aio-2023.5.0/velbusaio/messages/temp_set_cooling.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/temp_set_heating.py` & `velbus-aio-2023.5.0/velbusaio/messages/temp_set_heating.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/update_led_status.py` & `velbus-aio-2023.5.0/velbusaio/messages/update_led_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/very_fast_blinking_led.py` & `velbus-aio-2023.5.0/velbusaio/messages/very_fast_blinking_led.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/write_data_to_memory.py` & `velbus-aio-2023.5.0/velbusaio/messages/write_data_to_memory.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/write_memory_block.py` & `velbus-aio-2023.5.0/velbusaio/messages/write_memory_block.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/messages/write_module_address_and_serial_number.py` & `velbus-aio-2023.5.0/velbusaio/messages/write_module_address_and_serial_number.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/module.py` & `velbus-aio-2023.5.0/velbusaio/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         # and doesn't start on a boundary of 8.
         # E.g. The VMBGP4 has one subaddress, so since the second subaddress is not defined,
         # this function will delete channels 17-24 while 17 and 18 belong to the temperature channels.
         #
         # The solution would be that this functions knows were the temperature channels are located
         # and/or what the max number of subaddresses are for each module.
         if self._sub_address == {}:
-            assert "No subaddresses defined"
+            raise Exception("No subaddresses defined")
         for sub in range(1, 4):
             if sub not in self._sub_address:
                 for i in range(((sub * 8) + 1), (((sub + 1) * 8) + 1)):
                     if i in self._channels:
                         del self._channels[i]
 
     def _cache(self) -> None:
@@ -368,16 +368,20 @@
                         _update_buttons = True
                         break
             if _update_buttons:
                 for channel_id in range(1, 9):
                     channel = self._translate_channel_name(channel_id + _channel_offset)
                     if channel_id in message.closed:
                         await self._update_channel(channel, {"closed": True})
+                    if channel_id in message.closed_long:
+                        await self._update_channel(channel, {"long": True})
                     if channel_id in message.opened:
-                        await self._update_channel(channel, {"closed": False})
+                        await self._update_channel(
+                            channel, {"closed": False, "long": False}
+                        )
         elif isinstance(message, (ModuleStatusMessage)):
             for channel_id in range(1, 9):
                 channel = self._translate_channel_name(channel_id + _channel_offset)
                 if channel_id in message.closed:
                     await self._update_channel(channel, {"closed": True})
                 elif channel in self._channels and isinstance(
                     self._channels[channel], (Button, ButtonCounter)
```

### Comparing `velbus-aio-2023.2.0/velbusaio/moduleprotocol/protocol.json` & `velbus-aio-2023.5.0/velbusaio/moduleprotocol/protocol.json`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/protocol.py` & `velbus-aio-2023.5.0/velbusaio/protocol.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2023.2.0/velbusaio/raw_message.py` & `velbus-aio-2023.5.0/velbusaio/raw_message.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,18 +74,18 @@
 
 
 class ParseError(Exception):
     pass
 
 
 def _parse(rawmessage: bytearray) -> Tuple[Optional[RawMessage], bytearray]:
-    assert (
-        MINIMUM_MESSAGE_SIZE <= len(rawmessage) <= MAXIMUM_MESSAGE_SIZE
-    ), "Received a raw message with an illegal length"
-    assert rawmessage[0] == START_BYTE
+    if len(rawmessage) < MINIMUM_MESSAGE_SIZE or len(rawmessage) > MAXIMUM_MESSAGE_SIZE:
+        raise ValueError("Received a raw message with an illegal lemgth")
+    if rawmessage[0] != START_BYTE:
+        raise ValueError("Received a raw message with the wrong startbyte")
 
     priority = rawmessage[1]
     if priority not in PRIORITIES:
         raise ParseError(
             f"Invalid priority byte: {priority:02x} in {binascii.hexlify(rawmessage)}"
         )
```

