# Comparing `tmp/PyFlyt-0.6.5.tar.gz` & `tmp/PyFlyt-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.6.5.tar", last modified: Fri May 12 18:29:04 2023, max compression
+gzip compressed data, was "PyFlyt-0.6.6.tar", last modified: Fri May 12 21:07:08 2023, max compression
```

## Comparing `PyFlyt-0.6.5.tar` & `PyFlyt-0.6.6.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.848505 PyFlyt-0.6.5/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.6.5/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-12 18:29:04.848505 PyFlyt-0.6.5/PKG-INFO
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.844505 PyFlyt-0.6.5/PyFlyt/
--rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.6.5/PyFlyt/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.844505 PyFlyt-0.6.5/PyFlyt/core/
--rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.6.5/PyFlyt/core/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.844505 PyFlyt-0.6.5/PyFlyt/core/abstractions/
--rw-rw-r--   0 jet       (1000) jet       (1000)      352 2023-04-07 22:21:54.000000 PyFlyt-0.6.5/PyFlyt/core/abstractions/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-04-11 22:38:25.000000 PyFlyt-0.6.5/PyFlyt/core/abstractions/base_controller.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-12 18:09:31.000000 PyFlyt-0.6.5/PyFlyt/core/abstractions/base_drone.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11845 2023-04-12 15:29:31.000000 PyFlyt-0.6.5/PyFlyt/core/abstractions/boosters.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4375 2023-05-12 17:55:02.000000 PyFlyt-0.6.5/PyFlyt/core/abstractions/boring_bodies.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-12 15:30:11.000000 PyFlyt-0.6.5/PyFlyt/core/abstractions/camera.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7376 2023-04-27 19:26:46.000000 PyFlyt-0.6.5/PyFlyt/core/abstractions/gimbals.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15265 2023-05-12 17:53:29.000000 PyFlyt-0.6.5/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6757 2023-04-12 15:30:45.000000 PyFlyt-0.6.5/PyFlyt/core/abstractions/motors.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.6.5/PyFlyt/core/abstractions/pid.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    17927 2023-05-12 18:27:59.000000 PyFlyt-0.6.5/PyFlyt/core/aviary.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.844505 PyFlyt-0.6.5/PyFlyt/core/drones/
--rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.6.5/PyFlyt/core/drones/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9440 2023-04-12 14:34:17.000000 PyFlyt-0.6.5/PyFlyt/core/drones/fixedwing.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    18011 2023-04-27 19:14:33.000000 PyFlyt-0.6.5/PyFlyt/core/drones/quadx.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11574 2023-05-12 17:55:17.000000 PyFlyt-0.6.5/PyFlyt/core/drones/rocket.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-01 18:23:35.000000 PyFlyt-0.6.5/PyFlyt/core/load_objs.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.844505 PyFlyt-0.6.5/PyFlyt/gym_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.6.5/PyFlyt/gym_envs/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.844505 PyFlyt-0.6.5/PyFlyt/gym_envs/fixedwing_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.6.5/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6228 2023-04-12 17:52:29.000000 PyFlyt-0.6.5/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.844505 PyFlyt-0.6.5/PyFlyt/gym_envs/quadx_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.6.5/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.6.5/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.6.5/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6877 2023-04-12 17:52:31.000000 PyFlyt-0.6.5/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.844505 PyFlyt-0.6.5/PyFlyt/gym_envs/rocket_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.6.5/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-18 14:26:29.000000 PyFlyt-0.6.5/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.6.5/PyFlyt/gym_envs/waypoint_handler.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.844505 PyFlyt-0.6.5/PyFlyt/models/
--rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.6.5/PyFlyt/models/landing_pad.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.6.5/PyFlyt/models/race_gate.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.6.5/PyFlyt/models/target.urdf
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.844505 PyFlyt-0.6.5/PyFlyt/models/vehicles/
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.848505 PyFlyt-0.6.5/PyFlyt/models/vehicles/cf2x/
--rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.6.5/PyFlyt/models/vehicles/cf2x/cf2.dae
--rw-rw-r--   0 jet       (1000) jet       (1000)     2580 2023-03-10 23:54:13.000000 PyFlyt-0.6.5/PyFlyt/models/vehicles/cf2x/cf2x.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1241 2023-03-10 22:05:19.000000 PyFlyt-0.6.5/PyFlyt/models/vehicles/cf2x/cf2x.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.848505 PyFlyt-0.6.5/PyFlyt/models/vehicles/fixedwing/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.6.5/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.6.5/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.848505 PyFlyt-0.6.5/PyFlyt/models/vehicles/primitive_drone/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3501 2023-03-10 23:52:15.000000 PyFlyt-0.6.5/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1238 2023-03-10 23:21:42.000000 PyFlyt-0.6.5/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.848505 PyFlyt-0.6.5/PyFlyt/models/vehicles/quadplane/
--rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.6.5/PyFlyt/models/vehicles/quadplane/quadplane.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.6.5/PyFlyt/models/vehicles/quadplane/quadplane.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.848505 PyFlyt-0.6.5/PyFlyt/models/vehicles/rocket/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.6.5/PyFlyt/models/vehicles/rocket/rocket.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.6.5/PyFlyt/models/vehicles/rocket/rocket.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.844505 PyFlyt-0.6.5/PyFlyt.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-12 18:29:04.000000 PyFlyt-0.6.5/PyFlyt.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)     1895 2023-05-12 18:29:04.000000 PyFlyt-0.6.5/PyFlyt.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-05-12 18:29:04.000000 PyFlyt-0.6.5/PyFlyt.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-05-12 18:29:04.000000 PyFlyt-0.6.5/PyFlyt.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-05-12 18:29:04.000000 PyFlyt-0.6.5/PyFlyt.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     1162 2023-05-12 18:27:56.000000 PyFlyt-0.6.5/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 19:14:33.000000 PyFlyt-0.6.5/readme.md
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-05-12 18:29:04.848505 PyFlyt-0.6.5/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.6.5/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:29:04.848505 PyFlyt-0.6.5/tests/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7639 2023-05-12 18:11:39.000000 PyFlyt-0.6.5/tests/test_core.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-04-23 20:14:07.000000 PyFlyt-0.6.5/tests/test_gym_envs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.6.6/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PKG-INFO
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.754888 PyFlyt-0.6.6/PyFlyt/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.6.6/PyFlyt/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.754888 PyFlyt-0.6.6/PyFlyt/core/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.6.6/PyFlyt/core/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/core/abstractions/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-12 20:44:00.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-05-12 19:45:35.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/base_controller.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-12 20:30:07.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/base_drone.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2757 2023-05-12 21:06:48.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/base_wind_field.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11845 2023-04-12 15:29:31.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/boosters.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4396 2023-05-12 20:47:43.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/boring_bodies.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-12 15:30:11.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/camera.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7376 2023-04-27 19:26:46.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/gimbals.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15316 2023-05-12 20:44:00.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6757 2023-04-12 15:30:45.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/motors.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.6.6/PyFlyt/core/abstractions/pid.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    17626 2023-05-12 20:56:04.000000 PyFlyt-0.6.6/PyFlyt/core/aviary.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/core/drones/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.6.6/PyFlyt/core/drones/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9440 2023-04-12 14:34:17.000000 PyFlyt-0.6.6/PyFlyt/core/drones/fixedwing.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    18011 2023-04-27 19:14:33.000000 PyFlyt-0.6.6/PyFlyt/core/drones/quadx.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11574 2023-05-12 17:55:17.000000 PyFlyt-0.6.6/PyFlyt/core/drones/rocket.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-01 18:23:35.000000 PyFlyt-0.6.6/PyFlyt/core/load_objs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/gym_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/gym_envs/fixedwing_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6228 2023-04-12 17:52:29.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6877 2023-04-12 17:52:31.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/gym_envs/rocket_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-18 14:26:29.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.6.6/PyFlyt/gym_envs/waypoint_handler.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/models/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.6.6/PyFlyt/models/landing_pad.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.6.6/PyFlyt/models/race_gate.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.6.6/PyFlyt/models/target.urdf
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.754888 PyFlyt-0.6.6/PyFlyt/models/vehicles/
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/models/vehicles/cf2x/
+-rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/cf2x/cf2.dae
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2580 2023-03-10 23:54:13.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/cf2x/cf2x.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1241 2023-03-10 22:05:19.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/cf2x/cf2x.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/models/vehicles/fixedwing/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/models/vehicles/primitive_drone/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3501 2023-03-10 23:52:15.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1238 2023-03-10 23:21:42.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/models/vehicles/quadplane/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/quadplane/quadplane.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/quadplane/quadplane.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/PyFlyt/models/vehicles/rocket/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/rocket/rocket.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.6.6/PyFlyt/models/vehicles/rocket/rocket.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.754888 PyFlyt-0.6.6/PyFlyt.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-12 21:07:08.000000 PyFlyt-0.6.6/PyFlyt.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1939 2023-05-12 21:07:08.000000 PyFlyt-0.6.6/PyFlyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-05-12 21:07:08.000000 PyFlyt-0.6.6/PyFlyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-05-12 21:07:08.000000 PyFlyt-0.6.6/PyFlyt.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-05-12 21:07:08.000000 PyFlyt-0.6.6/PyFlyt.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1162 2023-05-12 21:07:02.000000 PyFlyt-0.6.6/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 19:14:33.000000 PyFlyt-0.6.6/readme.md
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.6.6/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 21:07:08.758888 PyFlyt-0.6.6/tests/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7685 2023-05-12 20:54:30.000000 PyFlyt-0.6.6/tests/test_core.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-04-23 20:14:07.000000 PyFlyt-0.6.6/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.6.5/LICENSE.txt` & `PyFlyt-0.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PKG-INFO` & `PyFlyt-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.6.5
+Version: 0.6.6
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.6.5/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.6.6/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/core/abstractions/base_drone.py` & `PyFlyt-0.6.6/PyFlyt/core/abstractions/base_drone.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.6.6/PyFlyt/core/abstractions/boosters.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.6.6/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
         # get all the velocities
         body_velocities = np.array([item[-2] for item in link_states])
 
         # query for wind if available and add to surface velocities
         if self.p.wind_field is not None:
             body_positions = np.array([item[0] for item in link_states])
-            body_velocities += self.p.wind_field(body_positions)
+            body_velocities += self.p.wind_field(self.p.elapsed_time, body_positions)
 
         # rotate all velocities to be in local frame
         body_velocities = np.matmul(rotation_matrix, body_velocities.T).T
 
         # update the variable
         self.local_body_velocities = body_velocities
```

### Comparing `PyFlyt-0.6.5/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.6.6/PyFlyt/core/abstractions/camera.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.6.6/PyFlyt/core/abstractions/gimbals.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.6.6/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,17 @@
 
         # get all the velocities
         surface_velocities = np.array([item[-2] for item in link_states])
 
         # query for wind if available and add to surface velocities
         if self.p.wind_field is not None:
             surface_positions = np.array([item[0] for item in link_states])
-            surface_velocities += self.p.wind_field(surface_positions)
+            surface_velocities += self.p.wind_field(
+                self.p.elapsed_time, surface_positions
+            )
 
         # convert all to local velocities
         surface_velocities = np.matmul(rotation_matrix, surface_velocities.T).T
 
         # update the velocities of all surfaces
         for surface, velocity in zip(self.surfaces, surface_velocities):
             surface.state_update(velocity)
```

### Comparing `PyFlyt-0.6.5/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.6.6/PyFlyt/core/abstractions/motors.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.6.6/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/core/aviary.py` & `PyFlyt-0.6.6/PyFlyt/core/aviary.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """The Aviary class, the core of how PyFlyt handles UAVs in the PyBullet simulation environment."""
 from __future__ import annotations
 
 import time
 from itertools import repeat
-from typing import Any, Callable, Sequence
+from typing import Any, Sequence, Type
 from warnings import warn
 
 import numpy as np
 import pybullet as p
 import pybullet_data
 from pybullet_utils import bullet_client
 
-from .abstractions import DroneClass
+from .abstractions import DroneClass, WindFieldClass
 from .drones import Fixedwing, QuadX, Rocket
 
 DroneIndex = int
 
 
 class Aviary(bullet_client.BulletClient):
     """Aviary class, the core of how PyFlyt handles UAVs in the PyBullet simulation environment.
@@ -23,48 +23,54 @@
     The `aviary` is a handler for physics stepping, setpoint handling, collisions tracking, and much more.
     It provides a common endpoint from where users may control drones or define tasks.
 
     Args:
         start_pos (np.ndarray): an `(n, 3)` array for the starting X, Y, Z positions for each drone.
         start_orn (np.ndarray): an `(n, 3)` array for the starting orientations for each drone, in terms of Euler angles.
         drone_type (str | Sequence[str]): a _lowercase_ string representing what type of drone to spawn.
-        drone_type_mappings (None | dict(str, DroneClass)): a dictionary mapping of `{str: DroneClass}` for spawning custom drones.
+        drone_type_mappings (None | dict(str, Type[DroneClass])): a dictionary mapping of `{str: DroneClass}` for spawning custom drones.
         drone_options (dict[str, Any] | Sequence[dict[str, Any]]): dictionary mapping of custom parameters for each drone.
+        wind_type (None | str | Type[WindField]): a wind field model that will be used throughout the simulation.
+        wind_options (dict[str, Any] | Sequence[dict[str, Any]]): dictionary mapping of custom parameters for the wind field.
         render (bool): a boolean whether to render the simulation.
         physics_hz (int): physics looprate (not recommended to be changed).
-        worldScale (float): how big to spawn the floor.
+        world_scale (float): how big to spawn the floor.
         seed (None | int): optional int for seeding the simulation RNG.
     """
 
     def __init__(
         self,
         start_pos: np.ndarray,
         start_orn: np.ndarray,
         drone_type: str | Sequence[str],
-        drone_type_mappings: None | dict[str, DroneClass] = None,
+        drone_type_mappings: None | dict[str, type[DroneClass]] = None,
         drone_options: dict[str, Any] | Sequence[dict[str, Any]] = {},
+        wind_type: None | str | type[WindFieldClass] = None,
+        wind_options: dict[str, Any] = {},
         render: bool = False,
         physics_hz: int = 240,
-        worldScale: float = 1.0,
+        world_scale: float = 1.0,
         seed: None | int = None,
     ):
         """Initializes a PyBullet environment that hosts UAVs and other entities.
 
         The Aviary class itself inherits from a BulletClient, so any function that a PyBullet client has, this class will have.
         The Aviary also handles dealing with physics and control looprates, as well as automatic construction of several default UAVs and their corresponding cameras.
 
         Args:
             start_pos (np.ndarray): an `(n, 3)` array for the starting X, Y, Z positions for each drone.
             start_orn (np.ndarray): an `(n, 3)` array for the starting orientations for each drone, in terms of Euler angles.
             drone_type (str | Sequence[str]): a _lowercase_ string representing what type of drone to spawn.
-            drone_type_mappings (None | dict(str, DroneClass)): a dictionary mapping of `{str: DroneClass}` for spawning custom drones.
+            drone_type_mappings (None | dict(str, Type[DroneClass])): a dictionary mapping of `{str: DroneClass}` for spawning custom drones.
             drone_options (dict[str, Any] | Sequence[dict[str, Any]]): dictionary mapping of custom parameters for each drone.
+            wind_type (None | str | Type[WindField]): a wind field model that will be used throughout the simulation.
+            wind_options (dict[str, Any] | Sequence[dict[str, Any]]): dictionary mapping of custom parameters for the wind field.
             render (bool): a boolean whether to render the simulation.
             physics_hz (int): physics looprate (not recommended to be changed).
-            worldScale (float): how big to spawn the floor.
+            world_scale (float): how big to spawn the floor.
             seed (None | int): optional int for seeding the simulation RNG.
         """
         super().__init__(p.GUI if render else p.DIRECT)
         print("\033[A                             \033[A")
 
         # check for starting position and orientation shapes
         assert (
@@ -129,16 +135,20 @@
 
         # store the drone options
         if isinstance(drone_options, (tuple, list)):
             self.drone_options = drone_options
         else:
             self.drone_options = repeat(drone_options)
 
+        # store the wind type and options
+        self.wind_type = wind_type
+        self.wind_options = wind_options
+
         # set the world scale and directories
-        self.worldScale = worldScale
+        self.world_scale = world_scale
         self.setAdditionalSearchPath(pybullet_data.getDataPath())
 
         # render
         self.render = render
         self.rtf_debug_line = self.addUserDebugText(
             text="RTF here", textPosition=[0, 0, 0], textColorRGB=[1, 0, 0]
         )
@@ -149,31 +159,32 @@
         """Resets the simulation.
 
         Args:
             seed (None | int): seed
         """
         self.resetSimulation()
         self.setGravity(0, 0, -9.81)
-        self.wind_field = None
-        self.steps = 0
+        self.physics_steps: int = 0
+        self.aviary_steps: int = 0
+        self.elapsed_time: float = 0
 
         # reset the camera position to a sane place
         self.resetDebugVisualizerCamera(
             cameraDistance=5,
             cameraYaw=30,
             cameraPitch=-30,
             cameraTargetPosition=[0, 0, 1],
         )
 
         # define new RNG
         self.np_random = np.random.RandomState(seed=seed)
 
         # construct the world
         self.planeId = self.loadURDF(
-            "plane.urdf", useFixedBase=True, globalScaling=self.worldScale
+            "plane.urdf", useFixedBase=True, globalScaling=self.world_scale
         )
 
         # spawn drones
         self.drones: list[DroneClass] = []
         for start_pos, start_orn, drone_type, drone_options in zip(
             self.start_pos,
             self.start_orn,
@@ -187,14 +198,36 @@
                     start_orn=start_orn,
                     physics_hz=self.physics_hz,
                     np_random=self.np_random,
                     **drone_options,
                 )
             )
 
+        # initialize the wind field
+        self.wind_field: None | WindFieldClass
+        if self.wind_type is None:
+            # no wind field
+            self.wind_field = None
+        elif isinstance(self.wind_type, str):
+            # default wind fields
+            assert self.wind_type in [], f"Unknown wind field model {self.wind_type}."
+            self.wind_field = None
+        elif callable(self.wind_type):
+            # custom wind field, initialize and check
+            self.wind_field = self.wind_type(
+                np_random=self.np_random, **self.wind_options
+            )
+            self.wind_field._check_wind_field_validity()
+            self.wind_field = self.wind_type(
+                np_random=self.np_random, **self.wind_options
+            )
+        else:
+            # none of the above
+            raise LookupError("Invalid setting for wind field.")
+
         # constants for tracking how many times to step depending on control hz
         all_control_hz = [int(1.0 / drone.control_period) for drone in self.drones]
         self.updates_per_step = int(self.physics_hz / np.min(all_control_hz))
         self.update_period = 1.0 / np.min(all_control_hz)
 
         # sanity check the control looprates
         if len(all_control_hz) > 0:
@@ -202,16 +235,16 @@
             all_ratios = np.array(all_control_hz)[1:] / np.array(all_control_hz)[:-1]
             assert all(
                 r % 1.0 == 0.0 for r in all_ratios
             ), "Looprates must form common multiples of each other."
 
         # rtf tracking parameters
         self.now = time.time()
-        self._frame_time_elapsed = 0.0
-        self._sim_time_elapsed = 0.0
+        self._frame_elapsed = 0.0
+        self._sim_elapsed = 0.0
 
         # arm everything
         self.register_all_new_bodies()
         self.set_armed(True)
 
         # reset all drones and initialize required states
         [drone.reset() for drone in self.drones]
@@ -224,65 +257,22 @@
         Call this when there is an update in the number of bodies in the environment.
         """
         # collision array
         self.contact_array = np.zeros(
             (self.getNumBodies(), self.getNumBodies()), dtype=bool
         )
 
-    def set_wind_field(self, wind_field_function: Callable):
-        """Sets the function for the wind field.
-
-        Args:
-            wind_field_function (Callable): A function that takes in a np.ndarray of size (n, 3) representing world frame coordinates, and returns a np.ndarray of size (n, 3) representing world frame wind velocities.
-
-        Example Usage:
-            >>> # define the aviary
-            >>> env = Aviary(...)
-            >>> ...
-            >>>
-            >>> # define the wind function
-            >>> def my_wind_function(position: np.ndarray):
-            >>>     # simulate a thermal windfield, where the xy velocities are 0,
-            >>>     # but the z velocity varies to the log of height
-            >>>     wind = np.zeros_like(position)
-            >>>     wind[:, -1] = np.log(position[:, -1])
-            >>>     return wind
-            >>>
-            >>> # hook the wind function
-            >>> env.set_wind_field(my_wind_function)
-        """
-        # check the validity of the wind field function
-        test_velocity = wind_field_function(np.array([[0.0, 0.0, 1.0]] * 42))
-        assert isinstance(
-            test_velocity, np.ndarray
-        ), f"Returned wind velocity must be a np.ndarray, got {type(test_velocity)}."
-        assert np.issubdtype(
-            test_velocity.dtype, np.floating
-        ), f"Returned wind velocity must be type float, got {test_velocity.dtype}."
-        assert (
-            len(test_velocity.shape) == 2
-        ), f"Returned wind velocity must be array of shape (n, 3), got (n+({test_velocity.shape[0] - 42}), {test_velocity.shape[1:]})."
-        assert (
-            test_velocity.shape[0] == 42
-        ), f"Returned wind velocity must be array of shape (n, 3), got (n+({test_velocity.shape[0] - 42}), {test_velocity.shape[1:]})."
-        assert (
-            test_velocity.shape[1] == 3
-        ), f"Returned wind velocity must be array of shape (n, 3), got (n+({test_velocity.shape[0] - 42}), {test_velocity.shape[1:]})."
-
-        # all checks pass
-        self.wind_field = wind_field_function
-
     @property
     def sim_time(self) -> float:
         """Returns the total amount of time that has elapsed in the simulation.
 
         Returns:
             float: simulation time elapsed.
         """
-        return self.steps * self.update_period
+        return self.aviary_steps * self.update_period
 
     def state(self, index: DroneIndex) -> np.ndarray:
         """Returns the state for the indexed drone.
 
         Args:
             index (DRONE_INDEX): index
 
@@ -395,54 +385,58 @@
     def step(self):
         """Steps the environment, this automatically handles physics and control looprates, one step is equivalent to one control loop step."""
         # compute rtf if we're rendering
         if self.render:
             elapsed = time.time() - self.now
             self.now = time.time()
 
-            self._sim_time_elapsed += self.update_period * self.updates_per_step
-            self._frame_time_elapsed += elapsed
+            self._sim_elapsed += self.update_period * self.updates_per_step
+            self._frame_elapsed += elapsed
 
-            time.sleep(max(self._sim_time_elapsed - self._frame_time_elapsed, 0.0))
+            time.sleep(max(self._sim_elapsed - self._frame_elapsed, 0.0))
 
             # print RTF every 0.5 seconds, this actually adds considerable overhead
-            if self._frame_time_elapsed >= 0.5:
+            if self._frame_elapsed >= 0.5:
                 # calculate real time factor based on realtime/simtime
-                RTF = self._sim_time_elapsed / (self._frame_time_elapsed + 1e-6)
-                self._sim_time_elapsed = 0.0
-                self._frame_time_elapsed = 0.0
+                RTF = self._sim_elapsed / (self._frame_elapsed + 1e-6)
+                self._sim_elapsed = 0.0
+                self._frame_elapsed = 0.0
 
                 self.rtf_debug_line = self.addUserDebugText(
                     text=f"RTF: {RTF:.3f}",
                     textPosition=[0, 0, 0],
                     textColorRGB=[1, 0, 0],
                     replaceItemUniqueId=self.rtf_debug_line,
                 )
 
         # reset collisions
         self.contact_array &= False
 
         # step the environment enough times for one control loop of the slowest controller
-        for physics_steps in range(self.updates_per_step):
+        for step in range(self.updates_per_step):
             # update onboard avionics conditionally
             [
                 drone.update_control()
                 for drone in self.armed_drones
-                if physics_steps % drone.physics_control_ratio == 0
+                if step % drone.physics_control_ratio == 0
             ]
 
             # update physics and state
             [drone.update_physics() for drone in self.armed_drones]
             [drone.update_state() for drone in self.armed_drones]
 
             # advance pybullet
             self.stepSimulation()
 
             # splice out collisions
             for collision in self.getContactPoints():
                 self.contact_array[collision[1], collision[2]] = True
                 self.contact_array[collision[2], collision[1]] = True
 
+            # increment the number of physics steps
+            self.physics_steps += 1
+            self.elapsed_time = self.physics_steps / self.physics_hz
+
         # update the last components of the drones, this is usually limited to cameras only
         [drone.update_last() for drone in self.armed_drones]
 
-        self.steps += 1
+        self.aviary_steps += 1
```

### Comparing `PyFlyt-0.6.5/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.6.6/PyFlyt/core/drones/fixedwing.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.6.6/PyFlyt/core/drones/quadx.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.6.6/PyFlyt/core/drones/rocket.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/core/load_objs.py` & `PyFlyt-0.6.6/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.6.6/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.6.6/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.6.6/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.6.6/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.6.6/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.6.6/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.6.6/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/models/race_gate.urdf` & `PyFlyt-0.6.6/PyFlyt/models/race_gate.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/models/vehicles/cf2x/cf2.dae` & `PyFlyt-0.6.6/PyFlyt/models/vehicles/cf2x/cf2.dae`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/models/vehicles/cf2x/cf2x.urdf` & `PyFlyt-0.6.6/PyFlyt/models/vehicles/cf2x/cf2x.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/models/vehicles/cf2x/cf2x.yaml` & `PyFlyt-0.6.6/PyFlyt/models/vehicles/cf2x/cf2x.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf` & `PyFlyt-0.6.6/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml` & `PyFlyt-0.6.6/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf` & `PyFlyt-0.6.6/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml` & `PyFlyt-0.6.6/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/models/vehicles/quadplane/quadplane.urdf` & `PyFlyt-0.6.6/PyFlyt/models/vehicles/quadplane/quadplane.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/models/vehicles/quadplane/quadplane.yaml` & `PyFlyt-0.6.6/PyFlyt/models/vehicles/quadplane/quadplane.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/models/vehicles/rocket/rocket.urdf` & `PyFlyt-0.6.6/PyFlyt/models/vehicles/rocket/rocket.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt/models/vehicles/rocket/rocket.yaml` & `PyFlyt-0.6.6/PyFlyt/models/vehicles/rocket/rocket.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.6.6/PyFlyt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.6.5
+Version: 0.6.6
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.6.5/PyFlyt.egg-info/SOURCES.txt` & `PyFlyt-0.6.6/PyFlyt.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 PyFlyt.egg-info/top_level.txt
 PyFlyt/core/__init__.py
 PyFlyt/core/aviary.py
 PyFlyt/core/load_objs.py
 PyFlyt/core/abstractions/__init__.py
 PyFlyt/core/abstractions/base_controller.py
 PyFlyt/core/abstractions/base_drone.py
+PyFlyt/core/abstractions/base_wind_field.py
 PyFlyt/core/abstractions/boosters.py
 PyFlyt/core/abstractions/boring_bodies.py
 PyFlyt/core/abstractions/camera.py
 PyFlyt/core/abstractions/gimbals.py
 PyFlyt/core/abstractions/lifting_surfaces.py
 PyFlyt/core/abstractions/motors.py
 PyFlyt/core/abstractions/pid.py
```

### Comparing `PyFlyt-0.6.5/pyproject.toml` & `PyFlyt-0.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.6.5"
+version = "0.6.6"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `PyFlyt-0.6.5/readme.md` & `PyFlyt-0.6.6/readme.md`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.5/tests/test_core.py` & `PyFlyt-0.6.6/tests/test_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,267 +1,276 @@
 """Tests the the core API functionality."""
 import numpy as np
-import pytest
 from custom_uavs.rocket_brick import RocketBrick
 
+import pytest
 from PyFlyt.core import Aviary
-from PyFlyt.core.abstractions import ControlClass
+from PyFlyt.core.abstractions import ControlClass, WindFieldClass
+
+
+def test_simple_spawn():
+    """Tests spawning a single drone."""
+    # the starting position and orientations
+    start_pos = np.array([[0.0, 0.0, 1.0]])
+    start_orn = np.array([[0.0, 0.0, 0.0]])
+
+    # environment setup
+    env = Aviary(
+        start_pos=start_pos, start_orn=start_orn, render=False, drone_type="quadx"
+    )
+
+    # set to position control
+    env.set_mode(7)
+
+    # simulate for 1000 steps (1000/120 ~= 8 seconds)
+    for i in range(1000):
+        env.step()
+
+    env.disconnect()
+
+
+def test_multi_spawn():
+    """Tests spawning multiple drones, and sets them all to have different control looprates."""
+    # the starting position and orientations
+    start_pos = np.array([[-1.0, 0.0, 1.0], [0.0, 0.0, 1.0], [1.0, 0.0, 1.0]])
+    start_orn = np.zeros_like(start_pos)
+
+    # modify the control hz of the individual drones
+    drone_options = []
+    drone_options.append(dict(control_hz=60))
+    drone_options.append(dict(control_hz=120))
+    drone_options.append(dict(control_hz=240))
+
+    # environment setup
+    env = Aviary(
+        start_pos=start_pos,
+        start_orn=start_orn,
+        render=False,
+        drone_type="quadx",
+        drone_options=drone_options,
+    )
+
+    # set to position control
+    env.set_mode(7)
+
+    # simulate for 1000 steps (1000/120 ~= 8 seconds)
+    for i in range(1000):
+        env.step()
+
+    env.disconnect()
+
+
+def test_default_control():
+    """Tests spawning a single drone and sending control commands."""
+    # the starting position and orientations
+    start_pos = np.array([[0.0, 0.0, 1.0]])
+    start_orn = np.array([[0.0, 0.0, 0.0]])
+
+    # environment setup
+    env = Aviary(
+        start_pos=start_pos, start_orn=start_orn, render=False, drone_type="quadx"
+    )
+
+    # set to position control
+    env.set_mode(7)
+
+    # for the first 500 steps, go to x=1, y=0, z=1
+    setpoint = np.array([1.0, 0.0, 0.0, 1.0])
+    env.set_setpoint(0, setpoint)
+
+    for i in range(500):
+        env.step()
+
+    # for the next 500 steps, go to x=0, y=0, z=2, rotate 45 degrees
+    setpoint = np.array([0.0, 0.0, np.pi / 4, 2.0])
+    env.set_setpoint(0, setpoint)
+
+    for i in range(500, 1000):
+        env.step()
+
+    env.disconnect()
+
+
+def test_camera():
+    """Tests the camera module."""
+    # the starting position and orientations
+    start_pos = np.array([[0.0, 0.0, 1.0]])
+    start_orn = np.array([[0.0, 0.0, 0.0]])
+
+    # environment setup
+    env = Aviary(
+        start_pos=start_pos,
+        start_orn=start_orn,
+        render=False,
+        drone_type="quadx",
+        drone_options=dict(use_camera=True),
+    )
+
+    # set to velocity control
+    env.set_mode(6)
 
-# def test_simple_spawn():
-#     """Tests spawning a single drone."""
-#     # the starting position and orientations
-#     start_pos = np.array([[0.0, 0.0, 1.0]])
-#     start_orn = np.array([[0.0, 0.0, 0.0]])
-
-#     # environment setup
-#     env = Aviary(
-#         start_pos=start_pos, start_orn=start_orn, render=False, drone_type="quadx"
-#     )
-
-#     # set to position control
-#     env.set_mode(7)
-
-#     # simulate for 1000 steps (1000/120 ~= 8 seconds)
-#     for i in range(1000):
-#         env.step()
-
-#     env.disconnect()
-
-
-# def test_multi_spawn():
-#     """Tests spawning multiple drones, and sets them all to have different control looprates."""
-#     # the starting position and orientations
-#     start_pos = np.array([[-1.0, 0.0, 1.0], [0.0, 0.0, 1.0], [1.0, 0.0, 1.0]])
-#     start_orn = np.zeros_like(start_pos)
-
-#     # modify the control hz of the individual drones
-#     drone_options = []
-#     drone_options.append(dict(control_hz=60))
-#     drone_options.append(dict(control_hz=120))
-#     drone_options.append(dict(control_hz=240))
-
-#     # environment setup
-#     env = Aviary(
-#         start_pos=start_pos,
-#         start_orn=start_orn,
-#         render=False,
-#         drone_type="quadx",
-#         drone_options=drone_options,
-#     )
-
-#     # set to position control
-#     env.set_mode(7)
-
-#     # simulate for 1000 steps (1000/120 ~= 8 seconds)
-#     for i in range(1000):
-#         env.step()
-
-#     env.disconnect()
-
-
-# def test_default_control():
-#     """Tests spawning a single drone and sending control commands."""
-#     # the starting position and orientations
-#     start_pos = np.array([[0.0, 0.0, 1.0]])
-#     start_orn = np.array([[0.0, 0.0, 0.0]])
-
-#     # environment setup
-#     env = Aviary(
-#         start_pos=start_pos, start_orn=start_orn, render=False, drone_type="quadx"
-#     )
-
-#     # set to position control
-#     env.set_mode(7)
-
-#     # for the first 500 steps, go to x=1, y=0, z=1
-#     setpoint = np.array([1.0, 0.0, 0.0, 1.0])
-#     env.set_setpoint(0, setpoint)
-
-#     for i in range(500):
-#         env.step()
-
-#     # for the next 500 steps, go to x=0, y=0, z=2, rotate 45 degrees
-#     setpoint = np.array([0.0, 0.0, np.pi / 4, 2.0])
-#     env.set_setpoint(0, setpoint)
-
-#     for i in range(500, 1000):
-#         env.step()
-
-#     env.disconnect()
-
-
-# def test_camera():
-#     """Tests the camera module."""
-#     # the starting position and orientations
-#     start_pos = np.array([[0.0, 0.0, 1.0]])
-#     start_orn = np.array([[0.0, 0.0, 0.0]])
-
-#     # environment setup
-#     env = Aviary(
-#         start_pos=start_pos,
-#         start_orn=start_orn,
-#         render=False,
-#         drone_type="quadx",
-#         drone_options=dict(use_camera=True),
-#     )
-
-#     # set to velocity control
-#     env.set_mode(6)
-
-#     # simulate for 1000 steps (1000/120 ~= 8 seconds)
-#     for i in range(100):
-#         env.step()
-
-#     env.disconnect()
-
-
-# def test_custom_controller():
-#     """Tests implementing a custom controller"""
-
-#     class CustomController(ControlClass):
-#         """A custom controller that inherits from the CtrlClass."""
-
-#         def __init__(self):
-#             """Initialize the controller here."""
-#             pass
-
-#         def reset(self):
-#             """Reset the internal state of the controller here."""
-#             pass
-
-#         def step(self, state: np.ndarray, setpoint: np.ndarray):
-#             """Step the controller here.
-
-#             Args:
-#                 state (np.ndarray): Current state of the UAV
-#                 setpoint (np.ndarray): Desired setpoint
-#             """
-#             # outputs a command to base flight mode 6 that makes the drone stay at x=1, y=1, z=1, yawrate=0.1
-#             target_velocity = np.array([1.0, 1.0, 1.0]) - state[-1]
-#             target_yaw_rate = 0.5
-#             output = np.array(
-#                 [*target_velocity[:2], target_yaw_rate, target_velocity[-1]]
-#             )
-#             return output
-
-#     # the starting position and orientations
-#     start_pos = np.array([[0.0, 0.0, 1.0]])
-#     start_orn = np.array([[0.0, 0.0, 0.0]])
-
-#     # environment setup
-#     env = Aviary(
-#         start_pos=start_pos, start_orn=start_orn, render=False, drone_type="quadx"
-#     )
-
-#     # register our custom controller for the first drone, this controller is id 8, and is based off 6
-#     env.drones[0].register_controller(
-#         controller_constructor=CustomController, controller_id=8, base_mode=6
-#     )
-
-#     # set to our new custom controller
-#     env.set_mode(8)
-
-#     # run the sim
-#     for i in range(1000):
-#         env.step()
-
-#     env.disconnect()
-
-
-# def test_custom_uav():
-#     """Tests spawning in a custom UAV."""
-#     # the starting position and orientations
-#     start_pos = np.array([[0.0, 0.0, 1.0]])
-#     start_orn = np.array([[0.0, 0.0, 0.0]])
-
-#     # define a new drone type
-#     drone_type_mappings = dict()
-#     drone_type_mappings["rocket_brick"] = RocketBrick
-
-#     # environment setup
-#     env = Aviary(
-#         start_pos=start_pos,
-#         start_orn=start_orn,
-#         render=False,
-#         drone_type_mappings=drone_type_mappings,
-#         drone_type="rocket_brick",
-#     )
-
-#     # print out the links and their names in the urdf for debugging
-#     env.drones[0].get_joint_info()
-
-#     # simulate for 1000 steps (1000/120 ~= 8 seconds)
-#     for i in range(1000):
-#         env.step()
-
-#         # ignite the rocket after ~1 seconds
-#         if i > 100:
-#             env.set_all_setpoints(np.array([[1.0, 1.0]]))
-
-#     env.disconnect()
-
-
-# def test_mixed_drones():
-#     """Tests spawning multiple different UAVs, with one having a camera."""
-#     # the starting position and orientations
-#     start_pos = np.array([[0.0, 5.0, 5.0], [0.0, 0.0, 1.0], [5.0, 0.0, 1.0]])
-#     start_orn = np.zeros_like(start_pos)
-
-#     # rotate the rocket upright
-#     start_orn[0, 0] = np.pi / 2
-
-#     # individual spawn options for each drone
-#     rocket_options = dict()
-#     quadx_options = dict(use_camera=True)
-#     fixedwing_options = dict(starting_velocity=np.array([0.0, 0.0, 0.0]))
-
-#     # environment setup
-#     env = Aviary(
-#         start_pos=start_pos,
-#         start_orn=start_orn,
-#         render=False,
-#         drone_type=["rocket", "quadx", "fixedwing"],
-#         drone_options=[rocket_options, quadx_options, fixedwing_options],
-#     )
-
-#     # set quadx to position control and fixedwing as nothing
-#     env.set_mode([0, 7, 0])
-
-#     # simulate for 1000 steps (1000/120 ~= 8 seconds)
-#     for i in range(1000):
-#         _ = env.all_states
-#         env.step()
+    # simulate for 1000 steps (1000/120 ~= 8 seconds)
+    for i in range(100):
+        env.step()
+
+    env.disconnect()
+
+
+def test_custom_controller():
+    """Tests implementing a custom controller"""
+
+    class CustomController(ControlClass):
+        """A custom controller that inherits from the CtrlClass."""
+
+        def __init__(self):
+            """Initialize the controller here."""
+            pass
+
+        def reset(self):
+            """Reset the internal state of the controller here."""
+            pass
+
+        def step(self, state: np.ndarray, setpoint: np.ndarray):
+            """Step the controller here.
+
+            Args:
+                state (np.ndarray): Current state of the UAV
+                setpoint (np.ndarray): Desired setpoint
+            """
+            # outputs a command to base flight mode 6 that makes the drone stay at x=1, y=1, z=1, yawrate=0.1
+            target_velocity = np.array([1.0, 1.0, 1.0]) - state[-1]
+            target_yaw_rate = 0.5
+            output = np.array(
+                [*target_velocity[:2], target_yaw_rate, target_velocity[-1]]
+            )
+            return output
 
-#     env.disconnect()
+    # the starting position and orientations
+    start_pos = np.array([[0.0, 0.0, 1.0]])
+    start_orn = np.array([[0.0, 0.0, 0.0]])
+
+    # environment setup
+    env = Aviary(
+        start_pos=start_pos, start_orn=start_orn, render=False, drone_type="quadx"
+    )
+
+    # register our custom controller for the first drone, this controller is id 8, and is based off 6
+    env.drones[0].register_controller(
+        controller_constructor=CustomController, controller_id=8, base_mode=6
+    )
+
+    # set to our new custom controller
+    env.set_mode(8)
+
+    # run the sim
+    for i in range(1000):
+        env.step()
+
+    env.disconnect()
+
+
+def test_custom_uav():
+    """Tests spawning in a custom UAV."""
+    # the starting position and orientations
+    start_pos = np.array([[0.0, 0.0, 1.0]])
+    start_orn = np.array([[0.0, 0.0, 0.0]])
+
+    # define a new drone type
+    drone_type_mappings = dict()
+    drone_type_mappings["rocket_brick"] = RocketBrick
+
+    # environment setup
+    env = Aviary(
+        start_pos=start_pos,
+        start_orn=start_orn,
+        render=False,
+        drone_type_mappings=drone_type_mappings,
+        drone_type="rocket_brick",
+    )
+
+    # print out the links and their names in the urdf for debugging
+    env.drones[0].get_joint_info()
+
+    # simulate for 1000 steps (1000/120 ~= 8 seconds)
+    for i in range(1000):
+        env.step()
+
+        # ignite the rocket after ~1 seconds
+        if i > 100:
+            env.set_all_setpoints(np.array([[1.0, 1.0]]))
+
+    env.disconnect()
+
+
+def test_mixed_drones():
+    """Tests spawning multiple different UAVs, with one having a camera."""
+    # the starting position and orientations
+    start_pos = np.array([[0.0, 5.0, 5.0], [0.0, 0.0, 1.0], [5.0, 0.0, 1.0]])
+    start_orn = np.zeros_like(start_pos)
+
+    # rotate the rocket upright
+    start_orn[0, 0] = np.pi / 2
+
+    # individual spawn options for each drone
+    rocket_options = dict()
+    quadx_options = dict(use_camera=True)
+    fixedwing_options = dict(starting_velocity=np.array([0.0, 0.0, 0.0]))
+
+    # environment setup
+    env = Aviary(
+        start_pos=start_pos,
+        start_orn=start_orn,
+        render=False,
+        drone_type=["rocket", "quadx", "fixedwing"],
+        drone_options=[rocket_options, quadx_options, fixedwing_options],
+    )
+
+    # set quadx to position control and fixedwing as nothing
+    env.set_mode([0, 7, 0])
+
+    # simulate for 1000 steps (1000/120 ~= 8 seconds)
+    for i in range(1000):
+        _ = env.all_states
+        env.step()
+
+    env.disconnect()
 
 
 @pytest.mark.parametrize(
     "model",
-    ["fixedwing", "rocket"],
+    [
+        "fixedwing",
+        "rocket"
+    ],
 )
 def test_wind_field(model: str):
     """Tests the wind field functionality
 
     Args:
         model (str): model name
     """
+    # define the wind field
+    class MyWindField(WindFieldClass):
+        def __init__(self, my_parameter=1.0, np_random: None | np.random.RandomState = None):
+            super().__init__(np_random)
+            self.strength = my_parameter
+
+        def __call__(self, time: float, position: np.ndarray):
+            wind = np.zeros_like(position)
+            wind[:, -1] = np.log(position[:, -1]) * self.strength
+            wind += self.np_random.randn(*wind.shape)
+            return wind
+
     # the starting position and orientations
     start_pos = np.array([[0.0, 0.0, 1.0]])
     start_orn = np.array([[0.0, 0.0, 0.0]])
 
-    # environment setup
+    # environment setup, attach the windfield
     env = Aviary(
-        start_pos=start_pos, start_orn=start_orn, render=False, drone_type=model
+        start_pos=start_pos, start_orn=start_orn, render=False, drone_type=model, wind_type=MyWindField
     )
 
-    def wind_function(position: np.ndarray):
-        wind = np.zeros_like(position)
-        wind[:, -1] = np.log(position[:, -1])
-        return wind
-
-    env.set_wind_field(wind_function)
-
     # simulate for 1000 steps (1000/120 ~= 8 seconds)
     for i in range(1000):
         env.step()
 
     env.disconnect()
```

### Comparing `PyFlyt-0.6.5/tests/test_gym_envs.py` & `PyFlyt-0.6.6/tests/test_gym_envs.py`

 * *Files identical despite different names*

