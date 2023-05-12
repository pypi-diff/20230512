# Comparing `tmp/PyFlyt-0.6.6.tar.gz` & `tmp/PyFlyt-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.6.6.tar", last modified: Fri May 12 21:07:08 2023, max compression
+gzip compressed data, was "PyFlyt-0.6.7.tar", last modified: Fri May 12 21:37:41 2023, max compression
```

## Comparing `PyFlyt-0.6.6.tar` & `PyFlyt-0.6.7.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.6.6/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PKG-INFO
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.754888 PyFlyt-0.6.6/PyFlyt/
--rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.6.6/PyFlyt/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.754888 PyFlyt-0.6.6/PyFlyt/core/
--rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.6.6/PyFlyt/core/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/core/abstractions/
--rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-12 20:44:00.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-05-12 19:45:35.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/base_controller.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-12 20:30:07.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/base_drone.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2757 2023-05-12 21:06:48.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/base_wind_field.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11845 2023-04-12 15:29:31.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/boosters.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4396 2023-05-12 20:47:43.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/boring_bodies.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-12 15:30:11.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/camera.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7376 2023-04-27 19:26:46.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/gimbals.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15316 2023-05-12 20:44:00.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6757 2023-04-12 15:30:45.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/motors.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/pid.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    17626 2023-05-12 20:56:04.000000 PyFlyt-0.6.6/PyFlyt/core/aviary.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/core/drones/
--rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.6.6/PyFlyt/core/drones/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9440 2023-04-12 14:34:17.000000 PyFlyt-0.6.6/PyFlyt/core/drones/fixedwing.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    18011 2023-04-27 19:14:33.000000 PyFlyt-0.6.6/PyFlyt/core/drones/quadx.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11574 2023-05-12 17:55:17.000000 PyFlyt-0.6.6/PyFlyt/core/drones/rocket.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-01 18:23:35.000000 PyFlyt-0.6.6/PyFlyt/core/load_objs.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/gym_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/gym_envs/fixedwing_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6228 2023-04-12 17:52:29.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6877 2023-04-12 17:52:31.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/gym_envs/rocket_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-18 14:26:29.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/waypoint_handler.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/models/
--rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.6.6/PyFlyt/models/landing_pad.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.6.6/PyFlyt/models/race_gate.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.6.6/PyFlyt/models/target.urdf
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.754888 PyFlyt-0.6.6/PyFlyt/models/vehicles/
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/models/vehicles/cf2x/
--rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/cf2x/cf2.dae
--rw-rw-r--   0 jet       (1000) jet       (1000)     2580 2023-03-10 23:54:13.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/cf2x/cf2x.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1241 2023-03-10 22:05:19.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/cf2x/cf2x.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/models/vehicles/fixedwing/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/models/vehicles/primitive_drone/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3501 2023-03-10 23:52:15.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1238 2023-03-10 23:21:42.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/models/vehicles/quadplane/
--rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/quadplane/quadplane.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/quadplane/quadplane.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/models/vehicles/rocket/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/rocket/rocket.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/rocket/rocket.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.754888 PyFlyt-0.6.6/PyFlyt.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-12 21:07:08.000000 PyFlyt-0.6.6/PyFlyt.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)     1939 2023-05-12 21:07:08.000000 PyFlyt-0.6.6/PyFlyt.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-05-12 21:07:08.000000 PyFlyt-0.6.6/PyFlyt.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-05-12 21:07:08.000000 PyFlyt-0.6.6/PyFlyt.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-05-12 21:07:08.000000 PyFlyt-0.6.6/PyFlyt.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     1162 2023-05-12 21:07:02.000000 PyFlyt-0.6.6/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 19:14:33.000000 PyFlyt-0.6.6/readme.md
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.6.6/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/tests/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7685 2023-05-12 20:54:30.000000 PyFlyt-0.6.6/tests/test_core.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-04-23 20:14:07.000000 PyFlyt-0.6.6/tests/test_gym_envs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.378564 PyFlyt-0.6.7/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.6.7/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-12 21:37:41.378564 PyFlyt-0.6.7/PKG-INFO
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.374564 PyFlyt-0.6.7/PyFlyt/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.6.7/PyFlyt/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.374564 PyFlyt-0.6.7/PyFlyt/core/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.6.7/PyFlyt/core/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.374564 PyFlyt-0.6.7/PyFlyt/core/abstractions/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-12 20:44:00.000000 PyFlyt-0.6.7/PyFlyt/core/abstractions/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-05-12 19:45:35.000000 PyFlyt-0.6.7/PyFlyt/core/abstractions/base_controller.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-12 20:30:07.000000 PyFlyt-0.6.7/PyFlyt/core/abstractions/base_drone.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2799 2023-05-12 21:34:19.000000 PyFlyt-0.6.7/PyFlyt/core/abstractions/base_wind_field.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11845 2023-04-12 15:29:31.000000 PyFlyt-0.6.7/PyFlyt/core/abstractions/boosters.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4396 2023-05-12 20:47:43.000000 PyFlyt-0.6.7/PyFlyt/core/abstractions/boring_bodies.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-12 15:30:11.000000 PyFlyt-0.6.7/PyFlyt/core/abstractions/camera.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7376 2023-04-27 19:26:46.000000 PyFlyt-0.6.7/PyFlyt/core/abstractions/gimbals.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15316 2023-05-12 20:44:00.000000 PyFlyt-0.6.7/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6757 2023-04-12 15:30:45.000000 PyFlyt-0.6.7/PyFlyt/core/abstractions/motors.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.6.7/PyFlyt/core/abstractions/pid.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    17933 2023-05-12 21:21:01.000000 PyFlyt-0.6.7/PyFlyt/core/aviary.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.374564 PyFlyt-0.6.7/PyFlyt/core/drones/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.6.7/PyFlyt/core/drones/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9440 2023-04-12 14:34:17.000000 PyFlyt-0.6.7/PyFlyt/core/drones/fixedwing.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    18011 2023-04-27 19:14:33.000000 PyFlyt-0.6.7/PyFlyt/core/drones/quadx.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11574 2023-05-12 17:55:17.000000 PyFlyt-0.6.7/PyFlyt/core/drones/rocket.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-01 18:23:35.000000 PyFlyt-0.6.7/PyFlyt/core/load_objs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.374564 PyFlyt-0.6.7/PyFlyt/core/wind/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-12 21:08:07.000000 PyFlyt-0.6.7/PyFlyt/core/wind/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.374564 PyFlyt-0.6.7/PyFlyt/gym_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.6.7/PyFlyt/gym_envs/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.374564 PyFlyt-0.6.7/PyFlyt/gym_envs/fixedwing_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.6.7/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6228 2023-04-12 17:52:29.000000 PyFlyt-0.6.7/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.374564 PyFlyt-0.6.7/PyFlyt/gym_envs/quadx_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.6.7/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.6.7/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.6.7/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6877 2023-04-12 17:52:31.000000 PyFlyt-0.6.7/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.374564 PyFlyt-0.6.7/PyFlyt/gym_envs/rocket_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.6.7/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-18 14:26:29.000000 PyFlyt-0.6.7/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.6.7/PyFlyt/gym_envs/waypoint_handler.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.378564 PyFlyt-0.6.7/PyFlyt/models/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.6.7/PyFlyt/models/landing_pad.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.6.7/PyFlyt/models/race_gate.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.6.7/PyFlyt/models/target.urdf
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.374564 PyFlyt-0.6.7/PyFlyt/models/vehicles/
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.378564 PyFlyt-0.6.7/PyFlyt/models/vehicles/cf2x/
+-rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.6.7/PyFlyt/models/vehicles/cf2x/cf2.dae
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2580 2023-03-10 23:54:13.000000 PyFlyt-0.6.7/PyFlyt/models/vehicles/cf2x/cf2x.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1241 2023-03-10 22:05:19.000000 PyFlyt-0.6.7/PyFlyt/models/vehicles/cf2x/cf2x.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.378564 PyFlyt-0.6.7/PyFlyt/models/vehicles/fixedwing/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.6.7/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.6.7/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.378564 PyFlyt-0.6.7/PyFlyt/models/vehicles/primitive_drone/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3501 2023-03-10 23:52:15.000000 PyFlyt-0.6.7/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1238 2023-03-10 23:21:42.000000 PyFlyt-0.6.7/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.378564 PyFlyt-0.6.7/PyFlyt/models/vehicles/quadplane/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.6.7/PyFlyt/models/vehicles/quadplane/quadplane.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.6.7/PyFlyt/models/vehicles/quadplane/quadplane.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.378564 PyFlyt-0.6.7/PyFlyt/models/vehicles/rocket/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.6.7/PyFlyt/models/vehicles/rocket/rocket.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.6.7/PyFlyt/models/vehicles/rocket/rocket.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.374564 PyFlyt-0.6.7/PyFlyt.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-12 21:37:41.000000 PyFlyt-0.6.7/PyFlyt.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1968 2023-05-12 21:37:41.000000 PyFlyt-0.6.7/PyFlyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-05-12 21:37:41.000000 PyFlyt-0.6.7/PyFlyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-05-12 21:37:41.000000 PyFlyt-0.6.7/PyFlyt.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-05-12 21:37:41.000000 PyFlyt-0.6.7/PyFlyt.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1162 2023-05-12 21:37:27.000000 PyFlyt-0.6.7/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 19:14:33.000000 PyFlyt-0.6.7/readme.md
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-05-12 21:37:41.378564 PyFlyt-0.6.7/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.6.7/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:37:41.378564 PyFlyt-0.6.7/tests/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8567 2023-05-12 21:34:19.000000 PyFlyt-0.6.7/tests/test_core.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-04-23 20:14:07.000000 PyFlyt-0.6.7/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.6.6/LICENSE.txt` & `PyFlyt-0.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PKG-INFO` & `PyFlyt-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.6.6
+Version: 0.6.7
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.6.6/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.6.7/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/core/abstractions/base_drone.py` & `PyFlyt-0.6.7/PyFlyt/core/abstractions/base_drone.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/core/abstractions/base_wind_field.py` & `PyFlyt-0.6.7/PyFlyt/core/abstractions/base_wind_field.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,32 +31,35 @@
         >>>
         >>> # environment setup, attach the windfield, override the parameter `my_parameter` from the default
         >>> env = Aviary(..., wind_type=MyWindField, wind_options=dict(my_parameter=1.2))
         >>>
         >>> # step as usual
         >>> ...
     """
+
     def __init__(self, np_random: None | np.random.RandomState = None):
         """Initializes the wind_field."""
         self.np_random = np.random.RandomState() if np_random is None else np_random
 
     @abstractmethod
     def __call__(self, time: float, position: np.ndarray) -> np.ndarray:
         """When given the time float and a position as an (n, 3) array, must return a (n, 3) array representing the local wind velocity.
 
         Args:
             time (float): float representing the timestep of the simulation in seconds.
             position (np.ndarray): (n, 3) array representing a series of n positions to sample wind velocites.
         """
         pass
 
-    def _check_wind_field_validity(self):
-        test_velocity = self(0.0, np.array([[0.0, 0.0, 1.0]] * 5))
+    @staticmethod
+    def _check_wind_field_validity(wind_field):
+        test_velocity = wind_field(0.0, np.array([[0.0, 0.0, 1.0]] * 5))
         assert isinstance(
             test_velocity, np.ndarray
         ), f"Returned wind velocity must be a np.ndarray, got {type(test_velocity)}."
         assert np.issubdtype(
             test_velocity.dtype, np.floating
         ), f"Returned wind velocity must be type float, got {test_velocity.dtype}."
-        assert (
-            test_velocity.shape == (5, 3)
+        assert test_velocity.shape == (
+            5,
+            3,
         ), f"Returned wind velocity must be array of shape (n, 3), got (n+({test_velocity.shape[0] - 5}), {test_velocity.shape[1:]})."
```

### Comparing `PyFlyt-0.6.6/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.6.7/PyFlyt/core/abstractions/boosters.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.6.7/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.6.7/PyFlyt/core/abstractions/camera.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.6.7/PyFlyt/core/abstractions/gimbals.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.6.7/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.6.7/PyFlyt/core/abstractions/motors.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.6.7/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/core/aviary.py` & `PyFlyt-0.6.7/PyFlyt/core/aviary.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The Aviary class, the core of how PyFlyt handles UAVs in the PyBullet simulation environment."""
 from __future__ import annotations
 
 import time
 from itertools import repeat
-from typing import Any, Sequence, Type
+from typing import Any, Callable, Sequence, Type
 from warnings import warn
 
 import numpy as np
 import pybullet as p
 import pybullet_data
 from pybullet_utils import bullet_client
 
@@ -212,15 +212,15 @@
             assert self.wind_type in [], f"Unknown wind field model {self.wind_type}."
             self.wind_field = None
         elif callable(self.wind_type):
             # custom wind field, initialize and check
             self.wind_field = self.wind_type(
                 np_random=self.np_random, **self.wind_options
             )
-            self.wind_field._check_wind_field_validity()
+            WindFieldClass._check_wind_field_validity(self.wind_field)
             self.wind_field = self.wind_type(
                 np_random=self.np_random, **self.wind_options
             )
         else:
             # none of the above
             raise LookupError("Invalid setting for wind field.")
 
@@ -257,22 +257,22 @@
         Call this when there is an update in the number of bodies in the environment.
         """
         # collision array
         self.contact_array = np.zeros(
             (self.getNumBodies(), self.getNumBodies()), dtype=bool
         )
 
-    @property
-    def sim_time(self) -> float:
-        """Returns the total amount of time that has elapsed in the simulation.
+    def register_wind_field_function(self, wind_field: Callable):
+        """For less complicated wind field models (time invariant models), this allows the registration of a normal function as a wind field model.
 
-        Returns:
-            float: simulation time elapsed.
+        Args:
+            wind_field (Callable): given the time float and a position as an (n, 3) array, must return a (n, 3) array representing the local wind velocity.
         """
-        return self.aviary_steps * self.update_period
+        assert callable(wind_field), "`wind_field` function must be callable."
+        WindFieldClass._check_wind_field_validity(wind_field)
 
     def state(self, index: DroneIndex) -> np.ndarray:
         """Returns the state for the indexed drone.
 
         Args:
             index (DRONE_INDEX): index
```

### Comparing `PyFlyt-0.6.6/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.6.7/PyFlyt/core/drones/fixedwing.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.6.7/PyFlyt/core/drones/quadx.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.6.7/PyFlyt/core/drones/rocket.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/core/load_objs.py` & `PyFlyt-0.6.7/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.6.7/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.6.7/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.6.7/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.6.7/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.6.7/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.6.7/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.6.7/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.6.7/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.6.7/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.6.7/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/models/race_gate.urdf` & `PyFlyt-0.6.7/PyFlyt/models/race_gate.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/models/vehicles/cf2x/cf2.dae` & `PyFlyt-0.6.7/PyFlyt/models/vehicles/cf2x/cf2.dae`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/models/vehicles/cf2x/cf2x.urdf` & `PyFlyt-0.6.7/PyFlyt/models/vehicles/cf2x/cf2x.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/models/vehicles/cf2x/cf2x.yaml` & `PyFlyt-0.6.7/PyFlyt/models/vehicles/cf2x/cf2x.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf` & `PyFlyt-0.6.7/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml` & `PyFlyt-0.6.7/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf` & `PyFlyt-0.6.7/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml` & `PyFlyt-0.6.7/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/models/vehicles/quadplane/quadplane.urdf` & `PyFlyt-0.6.7/PyFlyt/models/vehicles/quadplane/quadplane.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/models/vehicles/quadplane/quadplane.yaml` & `PyFlyt-0.6.7/PyFlyt/models/vehicles/quadplane/quadplane.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/models/vehicles/rocket/rocket.urdf` & `PyFlyt-0.6.7/PyFlyt/models/vehicles/rocket/rocket.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt/models/vehicles/rocket/rocket.yaml` & `PyFlyt-0.6.7/PyFlyt/models/vehicles/rocket/rocket.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.6.7/PyFlyt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.6.6
+Version: 0.6.7
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.6.6/PyFlyt.egg-info/SOURCES.txt` & `PyFlyt-0.6.7/PyFlyt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 PyFlyt/core/abstractions/lifting_surfaces.py
 PyFlyt/core/abstractions/motors.py
 PyFlyt/core/abstractions/pid.py
 PyFlyt/core/drones/__init__.py
 PyFlyt/core/drones/fixedwing.py
 PyFlyt/core/drones/quadx.py
 PyFlyt/core/drones/rocket.py
+PyFlyt/core/wind/__init__.py
 PyFlyt/gym_envs/__init__.py
 PyFlyt/gym_envs/waypoint_handler.py
 PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
 PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
 PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
 PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
 PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
```

### Comparing `PyFlyt-0.6.6/pyproject.toml` & `PyFlyt-0.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.6.6"
+version = "0.6.7"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `PyFlyt-0.6.6/readme.md` & `PyFlyt-0.6.7/readme.md`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.6/tests/test_core.py` & `PyFlyt-0.6.7/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Tests the the core API functionality."""
 import numpy as np
+import pytest
 from custom_uavs.rocket_brick import RocketBrick
 
-import pytest
 from PyFlyt.core import Aviary
 from PyFlyt.core.abstractions import ControlClass, WindFieldClass
 
 
 def test_simple_spawn():
     """Tests spawning a single drone."""
     # the starting position and orientations
@@ -233,28 +233,62 @@
         env.step()
 
     env.disconnect()
 
 
 @pytest.mark.parametrize(
     "model",
-    [
-        "fixedwing",
-        "rocket"
-    ],
+    ["fixedwing", "rocket"],
+)
+def test_simple_wind(model: str):
+    """Tests the wind field functionality
+
+    Args:
+        model (str): model name
+    """
+
+    # define the wind field
+    def simple_wind(time: float, position: np.ndarray):
+        wind = np.zeros_like(position)
+        wind[:, -1] = np.log(position[:, -1])
+        return wind
+
+    # the starting position and orientations
+    start_pos = np.array([[0.0, 0.0, 1.0]])
+    start_orn = np.array([[0.0, 0.0, 0.0]])
+
+    # environment setup, attach the windfield
+    env = Aviary(
+        start_pos=start_pos, start_orn=start_orn, render=False, drone_type=model
+    )
+    env.register_wind_field_function(simple_wind)
+
+    # simulate for 1000 steps (1000/120 ~= 8 seconds)
+    for i in range(1000):
+        env.step()
+
+    env.disconnect()
+
+
+@pytest.mark.parametrize(
+    "model",
+    ["fixedwing", "rocket"],
 )
-def test_wind_field(model: str):
+def test_custom_wind(model: str):
     """Tests the wind field functionality
 
     Args:
         model (str): model name
     """
+
     # define the wind field
     class MyWindField(WindFieldClass):
-        def __init__(self, my_parameter=1.0, np_random: None | np.random.RandomState = None):
+        def __init__(
+            self, my_parameter=1.0, np_random: None | np.random.RandomState = None
+        ):
             super().__init__(np_random)
             self.strength = my_parameter
 
         def __call__(self, time: float, position: np.ndarray):
             wind = np.zeros_like(position)
             wind[:, -1] = np.log(position[:, -1]) * self.strength
             wind += self.np_random.randn(*wind.shape)
@@ -262,15 +296,19 @@
 
     # the starting position and orientations
     start_pos = np.array([[0.0, 0.0, 1.0]])
     start_orn = np.array([[0.0, 0.0, 0.0]])
 
     # environment setup, attach the windfield
     env = Aviary(
-        start_pos=start_pos, start_orn=start_orn, render=False, drone_type=model, wind_type=MyWindField
+        start_pos=start_pos,
+        start_orn=start_orn,
+        render=False,
+        drone_type=model,
+        wind_type=MyWindField,
     )
 
     # simulate for 1000 steps (1000/120 ~= 8 seconds)
     for i in range(1000):
         env.step()
 
     env.disconnect()
```

### Comparing `PyFlyt-0.6.6/tests/test_gym_envs.py` & `PyFlyt-0.6.7/tests/test_gym_envs.py`

 * *Files identical despite different names*

