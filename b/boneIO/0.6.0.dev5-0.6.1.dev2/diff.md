# Comparing `tmp/boneIO-0.6.0.dev5.tar.gz` & `tmp/boneIO-0.6.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boneIO-0.6.0.dev5.tar", last modified: Sun May  7 10:27:55 2023, max compression
+gzip compressed data, was "boneIO-0.6.1.dev2.tar", last modified: Fri May 12 08:18:06 2023, max compression
```

## Comparing `boneIO-0.6.0.dev5.tar` & `boneIO-0.6.1.dev2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    35149 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/LICENSE
--rw-r--r--   0        0        0      474 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/README.md
--rw-r--r--   0        0        0      147 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/__init__.py
--rw-r--r--   0        0        0     3341 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/bonecli.py
--rw-r--r--   0        0        0     2924 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/const.py
--rw-r--r--   0        0        0     8454 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/cover.py
--rw-r--r--   0        0        0        0 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/__init__.py
--rw-r--r--   0        0        0      168 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/adc.yaml
--rw-r--r--   0        0        0      326 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/config.yaml
--rw-r--r--   0        0        0      150 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/cover.yaml
--rw-r--r--   0        0        0     2883 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/input.yaml
--rw-r--r--   0        0        0     3392 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/led32x4A.yaml
--rw-r--r--   0        0        0     1691 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/output24x16A.yaml
--rw-r--r--   0        0        0     2403 2023-05-07 10:27:24.540294 boneIO-0.6.0.dev5/boneio/example_config/output32x5A.yaml
--rw-r--r--   0        0        0    19372 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/fonts/danube__.ttf
--rw-r--r--   0        0        0     2039 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/__init__.py
--rw-r--r--   0        0        0      985 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/async_updater.py
--rw-r--r--   0        0        0     1169 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/click_timer.py
--rw-r--r--   0        0        0     2233 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/config.py
--rw-r--r--   0        0        0     7494 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/events.py
--rw-r--r--   0        0        0      717 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/exceptions.py
--rw-r--r--   0        0        0      885 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/filter.py
--rw-r--r--   0        0        0     2718 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/gpio.py
--rw-r--r--   0        0        0     6278 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/ha_discovery.py
--rw-r--r--   0        0        0    13547 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/loader.py
--rw-r--r--   0        0        0     1801 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/logger.py
--rw-r--r--   0        0        0      765 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/mqtt.py
--rw-r--r--   0        0        0      351 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/oled.py
--rw-r--r--   0        0        0     2430 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/onewire/W1ThermSensor.py
--rw-r--r--   0        0        0      448 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/onewire/__init__.py
--rw-r--r--   0        0        0     5169 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/onewire/ds2482.py
--rw-r--r--   0        0        0     2497 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/onewire/onewire.py
--rw-r--r--   0        0        0     1066 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/queue.py
--rw-r--r--   0        0        0     1994 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/state_manager.py
--rw-r--r--   0        0        0     5693 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/stats.py
--rw-r--r--   0        0        0     5806 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/timeperiod.py
--rw-r--r--   0        0        0      508 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/util.py
--rw-r--r--   0        0        0    11304 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/helper/yaml_util.py
--rw-r--r--   0        0        0       99 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/input/__init__.py
--rw-r--r--   0        0        0     2597 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/input/gpio.py
--rw-r--r--   0        0        0    21023 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/manager.py
--rw-r--r--   0        0        0     4176 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/modbus.py
--rw-r--r--   0        0        0     8331 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/mqtt_client.py
--rw-r--r--   0        0        0     5244 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/oled.py
--rw-r--r--   0        0        0      181 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/relay/__init__.py
--rw-r--r--   0        0        0     2623 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/relay/basic.py
--rw-r--r--   0        0        0     1163 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/relay/gpio.py
--rw-r--r--   0        0        0     2669 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/relay/mcp.py
--rw-r--r--   0        0        0     4873 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/relay/pca.py
--rw-r--r--   0        0        0     2569 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/runner.py
--rw-r--r--   0        0        0     1030 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/actions.yaml
--rw-r--r--   0        0        0      124 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/actions_sensor.yaml
--rw-r--r--   0        0        0      129 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/actions_switch.yaml
--rw-r--r--   0        0        0      286 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/filters.yaml
--rw-r--r--   0        0        0      304 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/filters_adc.yaml
--rw-r--r--   0        0        0       75 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/id.yaml
--rw-r--r--   0        0        0    12988 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/schema.yaml
--rw-r--r--   0        0        0       65 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/temp_unit.yaml
--rw-r--r--   0        0        0      133 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/schema/update_interval.yaml
--rw-r--r--   0        0        0      431 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/__init__.py
--rw-r--r--   0        0        0     1281 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/adc.py
--rw-r--r--   0        0        0     1303 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/gpio.py
--rw-r--r--   0        0        0     8500 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/modbus/__init__.py
--rw-r--r--   0        0        0     8810 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/modbus/dts1964_3f.json
--rw-r--r--   0        0        0      526 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/modbus/pt100.json
--rw-r--r--   0        0        0     2735 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/modbus/r4dcb08.json
--rw-r--r--   0        0        0     4145 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/modbus/sdm120.json
--rw-r--r--   0        0        0    10969 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/modbus/sdm630.json
--rw-r--r--   0        0        0     5592 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/modbus/sofar.json
--rw-r--r--   0        0        0     1659 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/temp/__init__.py
--rw-r--r--   0        0        0     2485 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/temp/dallas.py
--rw-r--r--   0        0        0      243 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/temp/lm75.py
--rw-r--r--   0        0        0      271 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/sensor/temp/mcp9808.py
--rw-r--r--   0        0        0       41 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/boneio/version.py
--rw-r--r--   0        0        0     1873 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/pyproject.toml
--rw-r--r--   0        0        0      166 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/tests/32_5_config.yaml
--rw-r--r--   0        0        0      224 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/tests/bandit.yaml
--rw-r--r--   0        0        0     1070 2023-05-07 10:27:24.544294 boneIO-0.6.0.dev5/tests/relay_32_5.py
--rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 boneIO-0.6.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/LICENSE
+-rw-r--r--   0        0        0      474 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/README.md
+-rw-r--r--   0        0        0      147 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/__init__.py
+-rw-r--r--   0        0        0     3341 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/bonecli.py
+-rw-r--r--   0        0        0     2924 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/const.py
+-rw-r--r--   0        0        0     8454 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/cover.py
+-rw-r--r--   0        0        0        0 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/example_config/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/example_config/adc.yaml
+-rw-r--r--   0        0        0      326 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/example_config/config.yaml
+-rw-r--r--   0        0        0      150 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/example_config/cover.yaml
+-rw-r--r--   0        0        0     2883 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/example_config/input.yaml
+-rw-r--r--   0        0        0     3392 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/example_config/led32x4A.yaml
+-rw-r--r--   0        0        0     1691 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/example_config/output24x16A.yaml
+-rw-r--r--   0        0        0     2403 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/example_config/output32x5A.yaml
+-rw-r--r--   0        0        0    19372 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/fonts/danube__.ttf
+-rw-r--r--   0        0        0     2039 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/__init__.py
+-rw-r--r--   0        0        0      985 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/async_updater.py
+-rw-r--r--   0        0        0     1169 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/click_timer.py
+-rw-r--r--   0        0        0     2277 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/config.py
+-rw-r--r--   0        0        0     7494 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/events.py
+-rw-r--r--   0        0        0      717 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/exceptions.py
+-rw-r--r--   0        0        0      885 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/filter.py
+-rw-r--r--   0        0        0     2718 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/gpio.py
+-rw-r--r--   0        0        0     6278 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/ha_discovery.py
+-rw-r--r--   0        0        0    13547 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/loader.py
+-rw-r--r--   0        0        0     1801 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/logger.py
+-rw-r--r--   0        0        0      765 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/mqtt.py
+-rw-r--r--   0        0        0      351 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/oled.py
+-rw-r--r--   0        0        0     2430 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/onewire/W1ThermSensor.py
+-rw-r--r--   0        0        0      448 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/onewire/__init__.py
+-rw-r--r--   0        0        0     5169 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/onewire/ds2482.py
+-rw-r--r--   0        0        0     2497 2023-05-12 08:17:31.350783 boneIO-0.6.1.dev2/boneio/helper/onewire/onewire.py
+-rw-r--r--   0        0        0     1066 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/helper/queue.py
+-rw-r--r--   0        0        0     1994 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/helper/state_manager.py
+-rw-r--r--   0        0        0     5693 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/helper/stats.py
+-rw-r--r--   0        0        0     5806 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/helper/timeperiod.py
+-rw-r--r--   0        0        0      508 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/helper/util.py
+-rw-r--r--   0        0        0    11304 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/helper/yaml_util.py
+-rw-r--r--   0        0        0       99 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/input/__init__.py
+-rw-r--r--   0        0        0     2597 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/input/gpio.py
+-rw-r--r--   0        0        0    21023 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/manager.py
+-rw-r--r--   0        0        0     4176 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/modbus.py
+-rw-r--r--   0        0        0     8331 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/mqtt_client.py
+-rw-r--r--   0        0        0     5244 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/oled.py
+-rw-r--r--   0        0        0      181 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/relay/__init__.py
+-rw-r--r--   0        0        0     2623 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/relay/basic.py
+-rw-r--r--   0        0        0     1163 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/relay/gpio.py
+-rw-r--r--   0        0        0     2669 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/relay/mcp.py
+-rw-r--r--   0        0        0     4873 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/relay/pca.py
+-rw-r--r--   0        0        0     2569 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/runner.py
+-rw-r--r--   0        0        0     1030 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/schema/actions.yaml
+-rw-r--r--   0        0        0      124 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/schema/actions_sensor.yaml
+-rw-r--r--   0        0        0      129 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/schema/actions_switch.yaml
+-rw-r--r--   0        0        0      286 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/schema/filters.yaml
+-rw-r--r--   0        0        0      304 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/schema/filters_adc.yaml
+-rw-r--r--   0        0        0       75 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/schema/id.yaml
+-rw-r--r--   0        0        0    12988 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/schema/schema.yaml
+-rw-r--r--   0        0        0       65 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/schema/temp_unit.yaml
+-rw-r--r--   0        0        0      133 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/schema/update_interval.yaml
+-rw-r--r--   0        0        0      431 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/sensor/__init__.py
+-rw-r--r--   0        0        0     1281 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/sensor/adc.py
+-rw-r--r--   0        0        0     1303 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/sensor/gpio.py
+-rw-r--r--   0        0        0     8520 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/sensor/modbus/__init__.py
+-rw-r--r--   0        0        0     8810 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/sensor/modbus/dts1964_3f.json
+-rw-r--r--   0        0        0      526 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/sensor/modbus/pt100.json
+-rw-r--r--   0        0        0     2735 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/sensor/modbus/r4dcb08.json
+-rw-r--r--   0        0        0     4145 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/sensor/modbus/sdm120.json
+-rw-r--r--   0        0        0    10969 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/sensor/modbus/sdm630.json
+-rw-r--r--   0        0        0     5592 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/sensor/modbus/sofar.json
+-rw-r--r--   0        0        0     1808 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/sensor/temp/__init__.py
+-rw-r--r--   0        0        0     2485 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/sensor/temp/dallas.py
+-rw-r--r--   0        0        0      243 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/sensor/temp/lm75.py
+-rw-r--r--   0        0        0      271 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/sensor/temp/mcp9808.py
+-rw-r--r--   0        0        0       41 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/boneio/version.py
+-rw-r--r--   0        0        0     1873 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/tests/32_5_config.yaml
+-rw-r--r--   0        0        0      224 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/tests/bandit.yaml
+-rw-r--r--   0        0        0     1070 2023-05-12 08:17:31.354783 boneIO-0.6.1.dev2/tests/relay_32_5.py
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 boneIO-0.6.1.dev2/PKG-INFO
```

### Comparing `boneIO-0.6.0.dev5/LICENSE` & `boneIO-0.6.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/bonecli.py` & `boneIO-0.6.1.dev2/boneio/bonecli.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/const.py` & `boneIO-0.6.1.dev2/boneio/const.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/cover.py` & `boneIO-0.6.1.dev2/boneio/cover.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/example_config/input.yaml` & `boneIO-0.6.1.dev2/boneio/example_config/input.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/example_config/led32x4A.yaml` & `boneIO-0.6.1.dev2/boneio/example_config/led32x4A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/example_config/output24x16A.yaml` & `boneIO-0.6.1.dev2/boneio/example_config/output24x16A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/example_config/output32x5A.yaml` & `boneIO-0.6.1.dev2/boneio/example_config/output32x5A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/fonts/danube__.ttf` & `boneIO-0.6.1.dev2/boneio/fonts/danube__.ttf`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/__init__.py` & `boneIO-0.6.1.dev2/boneio/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/async_updater.py` & `boneIO-0.6.1.dev2/boneio/helper/async_updater.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/click_timer.py` & `boneIO-0.6.1.dev2/boneio/helper/click_timer.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/config.py` & `boneIO-0.6.1.dev2/boneio/helper/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Module to provide basic config options.
 """
 from __future__ import annotations
 from _collections_abc import dict_values
+from typing import Union
 from boneio.const import BONEIO, HOMEASSISTANT, LIGHT, SENSOR, COVER, BUTTON, SWITCH, BINARY_SENSOR
 
 
 class ConfigHelper:
     def __init__(
         self,
         topic_prefix: str = BONEIO,
@@ -43,15 +44,15 @@
     def cmd_topic_prefix(self) -> str:
         return f"{self.topic_prefix}/cmd/"
 
     @property
     def subscribe_topic(self) -> str:
         return f"{self.cmd_topic_prefix}+/+/#"
 
-    def add_autodiscovery_msg(self, ha_type: str, topic: str, payload: str):
+    def add_autodiscovery_msg(self, ha_type: str, topic: str, payload: Union[str, dict, None]):
         """Add autodiscovery message."""
         self._autodiscovery_messages[ha_type][topic] = {"topic": topic, "payload": payload}
 
     @property
     def ha_types(self) -> list[str]:
         return list(self._autodiscovery_messages.keys())
```

### Comparing `boneIO-0.6.0.dev5/boneio/helper/events.py` & `boneIO-0.6.1.dev2/boneio/helper/events.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/exceptions.py` & `boneIO-0.6.1.dev2/boneio/helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/filter.py` & `boneIO-0.6.1.dev2/boneio/helper/filter.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/gpio.py` & `boneIO-0.6.1.dev2/boneio/helper/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/ha_discovery.py` & `boneIO-0.6.1.dev2/boneio/helper/ha_discovery.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/loader.py` & `boneIO-0.6.1.dev2/boneio/helper/loader.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/logger.py` & `boneIO-0.6.1.dev2/boneio/helper/logger.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/mqtt.py` & `boneIO-0.6.1.dev2/boneio/helper/mqtt.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/onewire/W1ThermSensor.py` & `boneIO-0.6.1.dev2/boneio/helper/onewire/W1ThermSensor.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/onewire/ds2482.py` & `boneIO-0.6.1.dev2/boneio/helper/onewire/ds2482.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/onewire/onewire.py` & `boneIO-0.6.1.dev2/boneio/helper/onewire/onewire.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/queue.py` & `boneIO-0.6.1.dev2/boneio/helper/queue.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/state_manager.py` & `boneIO-0.6.1.dev2/boneio/helper/state_manager.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/stats.py` & `boneIO-0.6.1.dev2/boneio/helper/stats.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/timeperiod.py` & `boneIO-0.6.1.dev2/boneio/helper/timeperiod.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/helper/yaml_util.py` & `boneIO-0.6.1.dev2/boneio/helper/yaml_util.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/input/gpio.py` & `boneIO-0.6.1.dev2/boneio/input/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/manager.py` & `boneIO-0.6.1.dev2/boneio/manager.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/modbus.py` & `boneIO-0.6.1.dev2/boneio/modbus.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/mqtt_client.py` & `boneIO-0.6.1.dev2/boneio/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/oled.py` & `boneIO-0.6.1.dev2/boneio/oled.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/relay/basic.py` & `boneIO-0.6.1.dev2/boneio/relay/basic.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/relay/gpio.py` & `boneIO-0.6.1.dev2/boneio/relay/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/relay/mcp.py` & `boneIO-0.6.1.dev2/boneio/relay/mcp.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/relay/pca.py` & `boneIO-0.6.1.dev2/boneio/relay/pca.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/runner.py` & `boneIO-0.6.1.dev2/boneio/runner.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/schema/actions.yaml` & `boneIO-0.6.1.dev2/boneio/schema/actions.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/schema/schema.yaml` & `boneIO-0.6.1.dev2/boneio/schema/schema.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/sensor/adc.py` & `boneIO-0.6.1.dev2/boneio/sensor/adc.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/sensor/gpio.py` & `boneIO-0.6.1.dev2/boneio/sensor/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/sensor/modbus/__init__.py` & `boneIO-0.6.1.dev2/boneio/sensor/modbus/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,18 +134,18 @@
             topic=self._config_helper.topic_prefix,
             id=id,
             name=sdm_name,
             model=self._model,
             sensor_id=sensor_id,
             **kwargs,
         )
-        self._config_helper.add_autodiscovery_msg(topic=topic, payload=payload)
+        self._config_helper.add_autodiscovery_msg(topic=topic, payload=payload, ha_type=SENSOR)
         self._send_message(topic=topic, payload=payload)
 
-    def _send_discovery_for_all_registers(self, register: int = 0) -> bool:
+    def _send_discovery_for_all_registers(self, register: int = 0) -> datetime:
         """Send discovery message to HA for each register."""
         for data in self._db[REGISTERS_BASE]:
             for register in data[REGISTERS]:
                 value_template = (
                     f'{{{{ value_json.{register.get("name").replace(" ", "")} | '
                     f'{register.get("ha_filter", "round(2)")} }}}}'
                 )
```

### Comparing `boneIO-0.6.0.dev5/boneio/sensor/modbus/dts1964_3f.json` & `boneIO-0.6.1.dev2/boneio/sensor/modbus/dts1964_3f.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/sensor/modbus/pt100.json` & `boneIO-0.6.1.dev2/boneio/sensor/modbus/pt100.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/sensor/modbus/r4dcb08.json` & `boneIO-0.6.1.dev2/boneio/sensor/modbus/r4dcb08.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/sensor/modbus/sdm120.json` & `boneIO-0.6.1.dev2/boneio/sensor/modbus/sdm120.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/sensor/modbus/sdm630.json` & `boneIO-0.6.1.dev2/boneio/sensor/modbus/sdm630.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/sensor/modbus/sofar.json` & `boneIO-0.6.1.dev2/boneio/sensor/modbus/sofar.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/boneio/sensor/temp/__init__.py` & `boneIO-0.6.1.dev2/boneio/sensor/temp/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,17 +40,21 @@
     @property
     def state(self) -> float:
         """Give rounded value of temperature."""
         return self._state
 
     def update(self, time: datetime) -> None:
         """Fetch temperature periodically and send to MQTT."""
-        _temp = self._pct.temperature
-        _LOGGER.debug("Fetched temperature %s. Applying filters.", _temp)
-        _temp = self._apply_filters(value=self._pct.temperature)
+        try:
+            _temp = self._pct.temperature
+            _LOGGER.debug("Fetched temperature %s. Applying filters.", _temp)
+            _temp = self._apply_filters(value=self._pct.temperature)
+        except RuntimeError as err:
+            _temp = None
+            _LOGGER.error("Sensor error: %s %s", err, self.id)
         if _temp is None:
             return
         self._state = _temp
         self._send_message(
             topic=self._send_topic,
             payload={STATE: self._state},
         )
```

### Comparing `boneIO-0.6.0.dev5/boneio/sensor/temp/dallas.py` & `boneIO-0.6.1.dev2/boneio/sensor/temp/dallas.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/pyproject.toml` & `boneIO-0.6.1.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Adafruit-BBIO>=1.2.0",
     "psutil>=5.9.5",
     "adafruit-circuitpython-onewire>=2.0.4",
     "w1thermsensor[async]>=2.0.0",
     "adafruit-circuitpython-pca9685>=3.4.8",
 ]
 requires-python = ">=3.7"
-version = "0.6.0.dev5"
+version = "0.6.1.dev2"
 
 [project.license]
 text = "GNU General Public License v3.0"
 
 [project.urls]
 Homepage = "https://boneio.eu"
 Repository = "https://github.com/boneIO-eu/app_bbb"
```

### Comparing `boneIO-0.6.0.dev5/tests/relay_32_5.py` & `boneIO-0.6.1.dev2/tests/relay_32_5.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.0.dev5/PKG-INFO` & `boneIO-0.6.1.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boneIO
-Version: 0.6.0.dev5
+Version: 0.6.1.dev2
 Summary: Python App for BoneIO
 License: GNU General Public License v3.0
 Author-email: Paweł Szafer <pszafer@gmail.com>
 Requires-Python: >=3.7
 Project-URL: Changelog, https://github.com/boneIO-eu/app_bbb/releases
 Project-URL: Documentation, https://boneio.eu/docs/intro/
 Project-URL: Homepage, https://boneio.eu
```

