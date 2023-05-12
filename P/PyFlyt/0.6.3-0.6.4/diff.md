# Comparing `tmp/PyFlyt-0.6.3.tar.gz` & `tmp/PyFlyt-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.6.3.tar", last modified: Thu Apr 27 19:27:00 2023, max compression
+gzip compressed data, was "PyFlyt-0.6.4.tar", last modified: Fri May 12 18:12:09 2023, max compression
```

## Comparing `PyFlyt-0.6.3.tar` & `PyFlyt-0.6.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.6.3/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/PKG-INFO
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/
--rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.6.3/PyFlyt/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/core/
--rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.6.3/PyFlyt/core/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/core/abstractions/
--rw-rw-r--   0 jet       (1000) jet       (1000)      352 2023-04-07 22:21:54.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-04-11 22:38:25.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/base_controller.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-04-23 00:11:20.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/base_drone.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11845 2023-04-12 15:29:31.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/boosters.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4277 2023-04-12 15:03:07.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/boring_bodies.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-12 15:30:11.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/camera.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7376 2023-04-27 19:26:46.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/gimbals.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15014 2023-04-12 15:29:07.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6757 2023-04-12 15:30:45.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/motors.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.6.3/PyFlyt/core/abstractions/pid.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15536 2023-04-23 00:13:01.000000 PyFlyt-0.6.3/PyFlyt/core/aviary.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/core/drones/
--rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.6.3/PyFlyt/core/drones/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9440 2023-04-12 14:34:17.000000 PyFlyt-0.6.3/PyFlyt/core/drones/fixedwing.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    18011 2023-04-27 19:14:33.000000 PyFlyt-0.6.3/PyFlyt/core/drones/quadx.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11598 2023-04-27 19:14:33.000000 PyFlyt-0.6.3/PyFlyt/core/drones/rocket.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-01 18:23:35.000000 PyFlyt-0.6.3/PyFlyt/core/load_objs.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/gym_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/gym_envs/fixedwing_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6228 2023-04-12 17:52:29.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6877 2023-04-12 17:52:31.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/gym_envs/rocket_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-18 14:26:29.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.6.3/PyFlyt/gym_envs/waypoint_handler.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/models/
--rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.6.3/PyFlyt/models/landing_pad.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.6.3/PyFlyt/models/race_gate.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.6.3/PyFlyt/models/target.urdf
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt/models/vehicles/
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/PyFlyt/models/vehicles/cf2x/
--rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/cf2x/cf2.dae
--rw-rw-r--   0 jet       (1000) jet       (1000)     2580 2023-03-10 23:54:13.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/cf2x/cf2x.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1241 2023-03-10 22:05:19.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/cf2x/cf2x.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/PyFlyt/models/vehicles/fixedwing/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/PyFlyt/models/vehicles/primitive_drone/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3501 2023-03-10 23:52:15.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1238 2023-03-10 23:21:42.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/PyFlyt/models/vehicles/quadplane/
--rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/quadplane/quadplane.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/quadplane/quadplane.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/PyFlyt/models/vehicles/rocket/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/rocket/rocket.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.6.3/PyFlyt/models/vehicles/rocket/rocket.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.046485 PyFlyt-0.6.3/PyFlyt.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-04-27 19:27:00.000000 PyFlyt-0.6.3/PyFlyt.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)     1895 2023-04-27 19:27:00.000000 PyFlyt-0.6.3/PyFlyt.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-04-27 19:27:00.000000 PyFlyt-0.6.3/PyFlyt.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-04-27 19:27:00.000000 PyFlyt-0.6.3/PyFlyt.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-04-27 19:27:00.000000 PyFlyt-0.6.3/PyFlyt.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     1162 2023-04-27 19:26:54.000000 PyFlyt-0.6.3/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 19:14:33.000000 PyFlyt-0.6.3/readme.md
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.6.3/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-04-27 19:27:00.050485 PyFlyt-0.6.3/tests/
--rw-rw-r--   0 jet       (1000) jet       (1000)     6511 2023-04-01 11:12:22.000000 PyFlyt-0.6.3/tests/test_core.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-04-23 20:14:07.000000 PyFlyt-0.6.3/tests/test_gym_envs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.208534 PyFlyt-0.6.4/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.6.4/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-12 18:12:09.208534 PyFlyt-0.6.4/PKG-INFO
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.204534 PyFlyt-0.6.4/PyFlyt/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.6.4/PyFlyt/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.204534 PyFlyt-0.6.4/PyFlyt/core/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.6.4/PyFlyt/core/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.204534 PyFlyt-0.6.4/PyFlyt/core/abstractions/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      352 2023-04-07 22:21:54.000000 PyFlyt-0.6.4/PyFlyt/core/abstractions/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-04-11 22:38:25.000000 PyFlyt-0.6.4/PyFlyt/core/abstractions/base_controller.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-12 18:09:31.000000 PyFlyt-0.6.4/PyFlyt/core/abstractions/base_drone.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11845 2023-04-12 15:29:31.000000 PyFlyt-0.6.4/PyFlyt/core/abstractions/boosters.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4375 2023-05-12 17:55:02.000000 PyFlyt-0.6.4/PyFlyt/core/abstractions/boring_bodies.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-12 15:30:11.000000 PyFlyt-0.6.4/PyFlyt/core/abstractions/camera.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7376 2023-04-27 19:26:46.000000 PyFlyt-0.6.4/PyFlyt/core/abstractions/gimbals.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15265 2023-05-12 17:53:29.000000 PyFlyt-0.6.4/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6757 2023-04-12 15:30:45.000000 PyFlyt-0.6.4/PyFlyt/core/abstractions/motors.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.6.4/PyFlyt/core/abstractions/pid.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    17709 2023-05-12 18:11:34.000000 PyFlyt-0.6.4/PyFlyt/core/aviary.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.204534 PyFlyt-0.6.4/PyFlyt/core/drones/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.6.4/PyFlyt/core/drones/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9440 2023-04-12 14:34:17.000000 PyFlyt-0.6.4/PyFlyt/core/drones/fixedwing.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    18011 2023-04-27 19:14:33.000000 PyFlyt-0.6.4/PyFlyt/core/drones/quadx.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11574 2023-05-12 17:55:17.000000 PyFlyt-0.6.4/PyFlyt/core/drones/rocket.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-01 18:23:35.000000 PyFlyt-0.6.4/PyFlyt/core/load_objs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.204534 PyFlyt-0.6.4/PyFlyt/gym_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.6.4/PyFlyt/gym_envs/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.204534 PyFlyt-0.6.4/PyFlyt/gym_envs/fixedwing_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.6.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6228 2023-04-12 17:52:29.000000 PyFlyt-0.6.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.204534 PyFlyt-0.6.4/PyFlyt/gym_envs/quadx_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.6.4/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.6.4/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.6.4/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6877 2023-04-12 17:52:31.000000 PyFlyt-0.6.4/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.204534 PyFlyt-0.6.4/PyFlyt/gym_envs/rocket_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.6.4/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-18 14:26:29.000000 PyFlyt-0.6.4/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.6.4/PyFlyt/gym_envs/waypoint_handler.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.204534 PyFlyt-0.6.4/PyFlyt/models/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.6.4/PyFlyt/models/landing_pad.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.6.4/PyFlyt/models/race_gate.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.6.4/PyFlyt/models/target.urdf
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.204534 PyFlyt-0.6.4/PyFlyt/models/vehicles/
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.208534 PyFlyt-0.6.4/PyFlyt/models/vehicles/cf2x/
+-rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.6.4/PyFlyt/models/vehicles/cf2x/cf2.dae
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2580 2023-03-10 23:54:13.000000 PyFlyt-0.6.4/PyFlyt/models/vehicles/cf2x/cf2x.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1241 2023-03-10 22:05:19.000000 PyFlyt-0.6.4/PyFlyt/models/vehicles/cf2x/cf2x.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.208534 PyFlyt-0.6.4/PyFlyt/models/vehicles/fixedwing/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.6.4/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.6.4/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.208534 PyFlyt-0.6.4/PyFlyt/models/vehicles/primitive_drone/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3501 2023-03-10 23:52:15.000000 PyFlyt-0.6.4/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1238 2023-03-10 23:21:42.000000 PyFlyt-0.6.4/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.208534 PyFlyt-0.6.4/PyFlyt/models/vehicles/quadplane/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.6.4/PyFlyt/models/vehicles/quadplane/quadplane.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.6.4/PyFlyt/models/vehicles/quadplane/quadplane.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.208534 PyFlyt-0.6.4/PyFlyt/models/vehicles/rocket/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.6.4/PyFlyt/models/vehicles/rocket/rocket.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.6.4/PyFlyt/models/vehicles/rocket/rocket.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.204534 PyFlyt-0.6.4/PyFlyt.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-12 18:12:09.000000 PyFlyt-0.6.4/PyFlyt.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1895 2023-05-12 18:12:09.000000 PyFlyt-0.6.4/PyFlyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-05-12 18:12:09.000000 PyFlyt-0.6.4/PyFlyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-05-12 18:12:09.000000 PyFlyt-0.6.4/PyFlyt.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-05-12 18:12:09.000000 PyFlyt-0.6.4/PyFlyt.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1162 2023-05-12 18:12:02.000000 PyFlyt-0.6.4/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 19:14:33.000000 PyFlyt-0.6.4/readme.md
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-05-12 18:12:09.208534 PyFlyt-0.6.4/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.6.4/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-12 18:12:09.208534 PyFlyt-0.6.4/tests/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7639 2023-05-12 18:11:39.000000 PyFlyt-0.6.4/tests/test_core.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-04-23 20:14:07.000000 PyFlyt-0.6.4/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.6.3/LICENSE.txt` & `PyFlyt-0.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PKG-INFO` & `PyFlyt-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.6.3
+Version: 0.6.4
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.6.3/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.6.4/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/core/abstractions/base_drone.py` & `PyFlyt-0.6.4/PyFlyt/core/abstractions/base_drone.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.6.4/PyFlyt/core/abstractions/boosters.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.6.4/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,32 +68,35 @@
 
     def get_states(self):
         """`get_states` does not exist for boring bodies, they're boring."""
         raise NotImplementedError(
             "`get_states` does not exist for boring bodies, they're boring."
         )
 
-    def state_update(self, rotation_matrices: np.ndarray):
+    def state_update(self, rotation_matrix: np.ndarray):
         """Updates the local surface velocity of the boring body.
 
         Args:
-            rotation_matrices (np.ndarray): (n, 3, 3) array of rotation matrices of the bodies
+            rotation_matrix (np.ndarray): (3, 3) rotation_matrix of the main body
         """
         # get all the states for all the bodies
-        body_velocities = self.p.getLinkStates(
+        link_states = self.p.getLinkStates(
             self.uav_id, self.body_ids, computeLinkVelocity=True
         )
 
         # get all the velocities
-        body_velocities = np.array([item[-2] for item in body_velocities])
-        body_velocities = np.expand_dims(body_velocities, axis=-1)
+        body_velocities = np.array([item[-2] for item in link_states])
+
+        # query for wind if available and add to surface velocities
+        if self.p.wind_field is not None:
+            body_positions = np.array([item[0] for item in link_states])
+            body_velocities += self.p.wind_field(body_positions)
 
         # rotate all velocities to be in local frame
-        body_velocities = np.matmul(rotation_matrices, body_velocities)
-        body_velocities = np.squeeze(body_velocities, axis=-1)
+        body_velocities = np.matmul(rotation_matrix, body_velocities.T).T
 
         # update the variable
         self.local_body_velocities = body_velocities
 
     def physics_update(self):
         """Applies a force to the boring bodies depending on their local surface velocities."""
         forces = (
```

### Comparing `PyFlyt-0.6.3/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.6.4/PyFlyt/core/abstractions/camera.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.6.4/PyFlyt/core/abstractions/gimbals.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.6.4/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,23 +65,28 @@
 
             surface.physics_update(actuation)
 
     def state_update(self, rotation_matrix: np.ndarray):
         """Updates all local surface velocities of the lifting surface, place under `update_state`.
 
         Args:
-            rotation_matrix (np.ndarray): rotation_matrix of the main body
+            rotation_matrix (np.ndarray): (3, 3) rotation_matrix of the main body
         """
         # get all the states for all the surfaces
-        surface_velocities = self.p.getLinkStates(
+        link_states = self.p.getLinkStates(
             self.uav_id, self.surface_ids, computeLinkVelocity=True
         )
 
         # get all the velocities
-        surface_velocities = np.array([item[-2] for item in surface_velocities])
+        surface_velocities = np.array([item[-2] for item in link_states])
+
+        # query for wind if available and add to surface velocities
+        if self.p.wind_field is not None:
+            surface_positions = np.array([item[0] for item in link_states])
+            surface_velocities += self.p.wind_field(surface_positions)
 
         # convert all to local velocities
         surface_velocities = np.matmul(rotation_matrix, surface_velocities.T).T
 
         # update the velocities of all surfaces
         for surface, velocity in zip(self.surfaces, surface_velocities):
             surface.state_update(velocity)
```

### Comparing `PyFlyt-0.6.3/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.6.4/PyFlyt/core/abstractions/motors.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.6.4/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/core/aviary.py` & `PyFlyt-0.6.4/PyFlyt/core/aviary.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The Aviary class, the core of how PyFlyt handles UAVs in the PyBullet simulation environment."""
 from __future__ import annotations
 
 import time
 from itertools import repeat
-from typing import Any, Sequence
+from typing import Any, Callable, Sequence
 from warnings import warn
 
 import numpy as np
 import pybullet as p
 import pybullet_data
 from pybullet_utils import bullet_client
 
@@ -149,14 +149,15 @@
         """Resets the simulation.
 
         Args:
             seed (None | int): seed
         """
         self.resetSimulation()
         self.setGravity(0, 0, -9.81)
+        self.wind_field = None
         self.steps = 0
 
         # reset the camera position to a sane place
         self.resetDebugVisualizerCamera(
             cameraDistance=5,
             cameraYaw=30,
             cameraPitch=-30,
@@ -223,14 +224,60 @@
         Call this when there is an update in the number of bodies in the environment.
         """
         # collision array
         self.contact_array = np.zeros(
             (self.getNumBodies(), self.getNumBodies()), dtype=bool
         )
 
+    def set_wind_field(self, wind_field_function: Callable):
+        """Sets the function for the wind field.
+
+        The function must take in a np.ndarray of size (n, 3) representing world frame coordinates.
+        It then returns a np.ndarray of size (n, 3) representing world frame wind velocities.
+
+        Args:
+            wind_field_function (Callable): wind_field_function
+
+        Example Usage:
+            >>> # define the aviary
+            >>> env = Aviary(...)
+            >>> ...
+            >>>
+            >>> # define the wind function
+            >>> def my_wind_function(position: np.ndarray):
+            >>>     # simulate a thermal windfield, where the xy velocities are 0,
+            >>>     # but the z velocity varies to the log of height
+            >>>     wind = np.zeros_like(position)
+            >>>     wind[:, -1] = np.log(position[:, -1])
+            >>>     return wind
+            >>>
+            >>> # hook the wind function
+            >>> env.set_wind_field(my_wind_function)
+        """
+        # check the validity of the wind field function
+        test_velocity = wind_field_function(np.array([[0.0, 0.0, 1.0]] * 42))
+        assert isinstance(
+            test_velocity, np.ndarray
+        ), f"Returned wind velocity must be a np.ndarray, got {type(test_velocity)}."
+        assert np.issubdtype(
+            test_velocity.dtype, np.floating
+        ), f"Returned wind velocity must be type float, got {test_velocity.dtype}."
+        assert (
+            len(test_velocity.shape) == 2
+        ), f"Returned wind velocity must be array of shape (n, 3), got (n+({test_velocity.shape[0] - 42}), {test_velocity.shape[1:]})."
+        assert (
+            test_velocity.shape[0] == 42
+        ), f"Returned wind velocity must be array of shape (n, 3), got (n+({test_velocity.shape[0] - 42}), {test_velocity.shape[1:]})."
+        assert (
+            test_velocity.shape[1] == 3
+        ), f"Returned wind velocity must be array of shape (n, 3), got (n+({test_velocity.shape[0] - 42}), {test_velocity.shape[1:]})."
+
+        # all checks pass
+        self.wind_field = wind_field_function
+
     def state(self, index: DroneIndex) -> np.ndarray:
         """Returns the state for the indexed drone.
 
         Args:
             index (DRONE_INDEX): index
 
         Returns:
```

### Comparing `PyFlyt-0.6.3/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.6.4/PyFlyt/core/drones/fixedwing.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.6.4/PyFlyt/core/drones/quadx.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.6.4/PyFlyt/core/drones/rocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
         # ang_pos in euler form
         ang_pos = self.p.getEulerFromQuaternion(ang_pos)
 
         # create the state
         self.state = np.stack([ang_vel, ang_pos, lin_vel, lin_pos], axis=0)
 
         # update all bodies, which is just the booster here
-        self.bodies.state_update(np.expand_dims(rotation, axis=0))
+        self.bodies.state_update(rotation)
 
         # update all lifting surface velocities
         self.lifting_surfaces.state_update(rotation)
 
         # update auxiliary information
         self.aux_state = np.concatenate(
             (
```

### Comparing `PyFlyt-0.6.3/PyFlyt/core/load_objs.py` & `PyFlyt-0.6.4/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.6.4/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.6.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.6.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.6.4/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.6.4/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.6.4/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.6.4/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.6.4/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.6.4/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.6.4/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/models/race_gate.urdf` & `PyFlyt-0.6.4/PyFlyt/models/race_gate.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/models/vehicles/cf2x/cf2.dae` & `PyFlyt-0.6.4/PyFlyt/models/vehicles/cf2x/cf2.dae`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/models/vehicles/cf2x/cf2x.urdf` & `PyFlyt-0.6.4/PyFlyt/models/vehicles/cf2x/cf2x.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/models/vehicles/cf2x/cf2x.yaml` & `PyFlyt-0.6.4/PyFlyt/models/vehicles/cf2x/cf2x.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf` & `PyFlyt-0.6.4/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml` & `PyFlyt-0.6.4/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf` & `PyFlyt-0.6.4/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml` & `PyFlyt-0.6.4/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/models/vehicles/quadplane/quadplane.urdf` & `PyFlyt-0.6.4/PyFlyt/models/vehicles/quadplane/quadplane.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/models/vehicles/quadplane/quadplane.yaml` & `PyFlyt-0.6.4/PyFlyt/models/vehicles/quadplane/quadplane.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/models/vehicles/rocket/rocket.urdf` & `PyFlyt-0.6.4/PyFlyt/models/vehicles/rocket/rocket.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt/models/vehicles/rocket/rocket.yaml` & `PyFlyt-0.6.4/PyFlyt/models/vehicles/rocket/rocket.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.6.4/PyFlyt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.6.3
+Version: 0.6.4
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.6.3/PyFlyt.egg-info/SOURCES.txt` & `PyFlyt-0.6.4/PyFlyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/pyproject.toml` & `PyFlyt-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.6.3"
+version = "0.6.4"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `PyFlyt-0.6.3/readme.md` & `PyFlyt-0.6.4/readme.md`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.6.3/tests/test_gym_envs.py` & `PyFlyt-0.6.4/tests/test_gym_envs.py`

 * *Files identical despite different names*

