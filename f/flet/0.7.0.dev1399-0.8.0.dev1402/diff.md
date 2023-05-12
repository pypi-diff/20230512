# Comparing `tmp/flet-0.7.0.dev1399.tar.gz` & `tmp/flet-0.8.0.dev1402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-0.7.0.dev1399.tar", max compression
+gzip compressed data, was "flet-0.8.0.dev1402.tar", max compression
```

## Comparing `flet-0.7.0.dev1399.tar` & `flet-0.8.0.dev1402.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     2145 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/README.md
--rw-r--r--   0        0        0     1066 2023-05-11 21:51:56.438826 flet-0.7.0.dev1399/pyproject.toml
--rw-r--r--   0        0        0      155 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/__init__.py
--rw-r--r--   0        0        0       72 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/__pyinstaller/__init__.py
--rw-r--r--   0        0        0       20 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/__pyinstaller/config.py
--rw-r--r--   0        0        0      378 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/__pyinstaller/hook-flet.py
--rw-r--r--   0        0        0     2985 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/__pyinstaller/macos_utils.py
--rw-r--r--   0        0        0      187 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
--rw-r--r--   0        0        0       61 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/__pyinstaller/rthooks.dat
--rw-r--r--   0        0        0      562 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/__pyinstaller/utils.py
--rw-r--r--   0        0        0     3620 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/__pyinstaller/win_utils.py
--rw-r--r--   0        0        0     6194 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/async_local_socket_connection.py
--rw-r--r--   0        0        0     7202 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/async_websocket_connection.py
--rw-r--r--   0        0        0     9083 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/auth/authorization.py
--rw-r--r--   0        0        0      128 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/auth/group.py
--rw-r--r--   0        0        0     1499 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/auth/oauth_provider.py
--rw-r--r--   0        0        0      847 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/auth/oauth_token.py
--rw-r--r--   0        0        0      735 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/auth/providers/auth0_oauth_provider.py
--rw-r--r--   0        0        0      840 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/auth/providers/azure_oauth_provider.py
--rw-r--r--   0        0        0     3653 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/auth/providers/github_oauth_provider.py
--rw-r--r--   0        0        0      799 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/auth/providers/google_oauth_provider.py
--rw-r--r--   0        0        0      182 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/auth/user.py
--rw-r--r--   0        0        0       31 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0     2958 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/cli/cli.py
--rw-r--r--   0        0        0     1953 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/cli/commands/base.py
--rw-r--r--   0        0        0      673 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/cli/commands/options.py
--rw-r--r--   0        0        0     8468 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/cli/commands/pack.py
--rw-r--r--   0        0        0     9306 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/cli/commands/publish.py
--rw-r--r--   0        0        0     7297 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/cli/commands/run.py
--rw-r--r--   0        0        0       52 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/constants.py
--rw-r--r--   0        0        0    22023 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/flet.py
--rw-r--r--   0        0        0       55 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/plotly_chart.py
--rw-r--r--   0        0        0    10239 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/pubsub.py
--rw-r--r--   0        0        0     3049 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/reconnecting_websocket.py
--rw-r--r--   0        0        0     1272 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/security.py
--rw-r--r--   0        0        0     6819 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/sync_local_socket_connection.py
--rw-r--r--   0        0        0     5396 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/sync_websocket_connection.py
--rw-r--r--   0        0        0     6955 2023-05-11 21:51:20.374494 flet-0.7.0.dev1399/src/flet/utils.py
--rw-r--r--   0        0        0     1431 2023-05-11 21:51:56.230826 flet-0.7.0.dev1399/src/flet/version.py
--rw-r--r--   0        0        0       32 2023-05-11 21:43:35.000000 flet-0.7.0.dev1399/src/flet/web/.last_build_id
--rw-r--r--   0        0        0      229 2023-05-11 21:43:31.000000 flet-0.7.0.dev1399/src/flet/web/assets/AssetManifest.bin
--rw-r--r--   0        0        0      455 2023-05-11 21:43:31.000000 flet-0.7.0.dev1399/src/flet/web/assets/AssetManifest.json
--rw-r--r--   0        0        0       82 2023-05-11 21:43:31.000000 flet-0.7.0.dev1399/src/flet/web/assets/FontManifest.json
--rw-r--r--   0        0        0  1736959 2023-05-11 21:43:31.000000 flet-0.7.0.dev1399/src/flet/web/assets/NOTICES
--rw-r--r--   0        0        0  1261080 2023-05-11 21:43:34.000000 flet-0.7.0.dev1399/src/flet/web/assets/fonts/MaterialIcons-Regular.otf
--rw-r--r--   0        0        0      298 2023-05-11 21:43:31.000000 flet-0.7.0.dev1399/src/flet/web/assets/packages/window_manager/images/ic_chrome_close.png
--rw-r--r--   0        0        0      271 2023-05-11 21:43:31.000000 flet-0.7.0.dev1399/src/flet/web/assets/packages/window_manager/images/ic_chrome_maximize.png
--rw-r--r--   0        0        0      166 2023-05-11 21:43:31.000000 flet-0.7.0.dev1399/src/flet/web/assets/packages/window_manager/images/ic_chrome_minimize.png
--rw-r--r--   0        0        0      366 2023-05-11 21:43:31.000000 flet-0.7.0.dev1399/src/flet/web/assets/packages/window_manager/images/ic_chrome_unmaximize.png
--rw-r--r--   0        0        0     9242 2023-05-11 21:43:31.000000 flet-0.7.0.dev1399/src/flet/web/assets/shaders/ink_sparkle.frag
--rw-r--r--   0        0        0     1028 2023-05-11 21:43:34.000000 flet-0.7.0.dev1399/src/flet/web/favicon.png
--rw-r--r--   0        0        0    14240 2023-05-11 21:42:14.000000 flet-0.7.0.dev1399/src/flet/web/flutter.js
--rw-r--r--   0        0        0     8316 2023-05-11 21:43:35.000000 flet-0.7.0.dev1399/src/flet/web/flutter_service_worker.js
--rw-r--r--   0        0        0     4699 2023-05-11 21:43:34.000000 flet-0.7.0.dev1399/src/flet/web/icons/apple-touch-icon-192.png
--rw-r--r--   0        0        0     6622 2023-05-11 21:43:34.000000 flet-0.7.0.dev1399/src/flet/web/icons/icon-192.png
--rw-r--r--   0        0        0    18666 2023-05-11 21:43:34.000000 flet-0.7.0.dev1399/src/flet/web/icons/icon-512.png
--rw-r--r--   0        0        0     4128 2023-05-11 21:43:34.000000 flet-0.7.0.dev1399/src/flet/web/icons/icon-maskable-192.png
--rw-r--r--   0        0        0    11906 2023-05-11 21:43:34.000000 flet-0.7.0.dev1399/src/flet/web/icons/icon-maskable-512.png
--rw-r--r--   0        0        0    17040 2023-05-11 21:43:34.000000 flet-0.7.0.dev1399/src/flet/web/icons/loading-animation.png
--rw-r--r--   0        0        0     3088 2023-05-11 21:43:34.000000 flet-0.7.0.dev1399/src/flet/web/index.html
--rw-r--r--   0        0        0  5499046 2023-05-11 21:43:31.000000 flet-0.7.0.dev1399/src/flet/web/main.dart.js
--rw-r--r--   0        0        0      789 2023-05-11 21:43:34.000000 flet-0.7.0.dev1399/src/flet/web/manifest.json
--rw-r--r--   0        0        0     1573 2023-05-11 21:43:34.000000 flet-0.7.0.dev1399/src/flet/web/python-worker.js
--rw-r--r--   0        0        0      744 2023-05-11 21:43:34.000000 flet-0.7.0.dev1399/src/flet/web/python.js
--rw-r--r--   0        0        0       92 2023-05-11 21:43:31.000000 flet-0.7.0.dev1399/src/flet/web/version.json
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 flet-0.7.0.dev1399/PKG-INFO
+-rw-r--r--   0        0        0     2145 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/README.md
+-rw-r--r--   0        0        0     1066 2023-05-11 23:58:02.898872 flet-0.8.0.dev1402/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/src/flet/__init__.py
+-rw-r--r--   0        0        0       72 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/src/flet/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0       20 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/src/flet/__pyinstaller/config.py
+-rw-r--r--   0        0        0      378 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/src/flet/__pyinstaller/hook-flet.py
+-rw-r--r--   0        0        0     2985 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/src/flet/__pyinstaller/macos_utils.py
+-rw-r--r--   0        0        0      187 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
+-rw-r--r--   0        0        0       61 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/src/flet/__pyinstaller/rthooks.dat
+-rw-r--r--   0        0        0      562 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/src/flet/__pyinstaller/utils.py
+-rw-r--r--   0        0        0     3620 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/src/flet/__pyinstaller/win_utils.py
+-rw-r--r--   0        0        0     6194 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/src/flet/async_local_socket_connection.py
+-rw-r--r--   0        0        0     7202 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/src/flet/async_websocket_connection.py
+-rw-r--r--   0        0        0     9083 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/src/flet/auth/authorization.py
+-rw-r--r--   0        0        0      128 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/src/flet/auth/group.py
+-rw-r--r--   0        0        0     1499 2023-05-11 23:57:27.975697 flet-0.8.0.dev1402/src/flet/auth/oauth_provider.py
+-rw-r--r--   0        0        0      847 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/auth/oauth_token.py
+-rw-r--r--   0        0        0      735 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/auth/providers/auth0_oauth_provider.py
+-rw-r--r--   0        0        0      840 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/auth/providers/azure_oauth_provider.py
+-rw-r--r--   0        0        0     3653 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/auth/providers/github_oauth_provider.py
+-rw-r--r--   0        0        0      799 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/auth/providers/google_oauth_provider.py
+-rw-r--r--   0        0        0      182 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/auth/user.py
+-rw-r--r--   0        0        0       31 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0     2958 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/cli/cli.py
+-rw-r--r--   0        0        0     1953 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/cli/commands/base.py
+-rw-r--r--   0        0        0      673 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/cli/commands/options.py
+-rw-r--r--   0        0        0     8468 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/cli/commands/pack.py
+-rw-r--r--   0        0        0     9306 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/cli/commands/publish.py
+-rw-r--r--   0        0        0     7297 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/cli/commands/run.py
+-rw-r--r--   0        0        0       52 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/constants.py
+-rw-r--r--   0        0        0    22023 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0    10239 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/pubsub.py
+-rw-r--r--   0        0        0     3049 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/reconnecting_websocket.py
+-rw-r--r--   0        0        0     1272 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/security.py
+-rw-r--r--   0        0        0     6819 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/sync_local_socket_connection.py
+-rw-r--r--   0        0        0     5396 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/sync_websocket_connection.py
+-rw-r--r--   0        0        0     6955 2023-05-11 23:57:27.979697 flet-0.8.0.dev1402/src/flet/utils.py
+-rw-r--r--   0        0        0     1431 2023-05-11 23:58:02.702871 flet-0.8.0.dev1402/src/flet/version.py
+-rw-r--r--   0        0        0       32 2023-05-11 23:47:14.000000 flet-0.8.0.dev1402/src/flet/web/.last_build_id
+-rw-r--r--   0        0        0      229 2023-05-11 23:47:10.000000 flet-0.8.0.dev1402/src/flet/web/assets/AssetManifest.bin
+-rw-r--r--   0        0        0      455 2023-05-11 23:47:10.000000 flet-0.8.0.dev1402/src/flet/web/assets/AssetManifest.json
+-rw-r--r--   0        0        0       82 2023-05-11 23:47:10.000000 flet-0.8.0.dev1402/src/flet/web/assets/FontManifest.json
+-rw-r--r--   0        0        0  1736959 2023-05-11 23:47:10.000000 flet-0.8.0.dev1402/src/flet/web/assets/NOTICES
+-rw-r--r--   0        0        0  1261080 2023-05-11 23:47:13.000000 flet-0.8.0.dev1402/src/flet/web/assets/fonts/MaterialIcons-Regular.otf
+-rw-r--r--   0        0        0      298 2023-05-11 23:47:10.000000 flet-0.8.0.dev1402/src/flet/web/assets/packages/window_manager/images/ic_chrome_close.png
+-rw-r--r--   0        0        0      271 2023-05-11 23:47:10.000000 flet-0.8.0.dev1402/src/flet/web/assets/packages/window_manager/images/ic_chrome_maximize.png
+-rw-r--r--   0        0        0      166 2023-05-11 23:47:10.000000 flet-0.8.0.dev1402/src/flet/web/assets/packages/window_manager/images/ic_chrome_minimize.png
+-rw-r--r--   0        0        0      366 2023-05-11 23:47:10.000000 flet-0.8.0.dev1402/src/flet/web/assets/packages/window_manager/images/ic_chrome_unmaximize.png
+-rw-r--r--   0        0        0     9242 2023-05-11 23:47:11.000000 flet-0.8.0.dev1402/src/flet/web/assets/shaders/ink_sparkle.frag
+-rw-r--r--   0        0        0     1028 2023-05-11 23:47:13.000000 flet-0.8.0.dev1402/src/flet/web/favicon.png
+-rw-r--r--   0        0        0    14240 2023-05-11 23:45:58.000000 flet-0.8.0.dev1402/src/flet/web/flutter.js
+-rw-r--r--   0        0        0     8316 2023-05-11 23:47:14.000000 flet-0.8.0.dev1402/src/flet/web/flutter_service_worker.js
+-rw-r--r--   0        0        0     4699 2023-05-11 23:47:13.000000 flet-0.8.0.dev1402/src/flet/web/icons/apple-touch-icon-192.png
+-rw-r--r--   0        0        0     6622 2023-05-11 23:47:13.000000 flet-0.8.0.dev1402/src/flet/web/icons/icon-192.png
+-rw-r--r--   0        0        0    18666 2023-05-11 23:47:13.000000 flet-0.8.0.dev1402/src/flet/web/icons/icon-512.png
+-rw-r--r--   0        0        0     4128 2023-05-11 23:47:13.000000 flet-0.8.0.dev1402/src/flet/web/icons/icon-maskable-192.png
+-rw-r--r--   0        0        0    11906 2023-05-11 23:47:13.000000 flet-0.8.0.dev1402/src/flet/web/icons/icon-maskable-512.png
+-rw-r--r--   0        0        0    17040 2023-05-11 23:47:13.000000 flet-0.8.0.dev1402/src/flet/web/icons/loading-animation.png
+-rw-r--r--   0        0        0     3088 2023-05-11 23:47:13.000000 flet-0.8.0.dev1402/src/flet/web/index.html
+-rw-r--r--   0        0        0  5499046 2023-05-11 23:47:10.000000 flet-0.8.0.dev1402/src/flet/web/main.dart.js
+-rw-r--r--   0        0        0      789 2023-05-11 23:47:13.000000 flet-0.8.0.dev1402/src/flet/web/manifest.json
+-rw-r--r--   0        0        0     1573 2023-05-11 23:47:13.000000 flet-0.8.0.dev1402/src/flet/web/python-worker.js
+-rw-r--r--   0        0        0      744 2023-05-11 23:47:13.000000 flet-0.8.0.dev1402/src/flet/web/python.js
+-rw-r--r--   0        0        0       92 2023-05-11 23:47:10.000000 flet-0.8.0.dev1402/src/flet/web/version.json
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 flet-0.8.0.dev1402/PKG-INFO
```

### Comparing `flet-0.7.0.dev1399/README.md` & `flet-0.8.0.dev1402/README.md`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/pyproject.toml` & `flet-0.8.0.dev1402/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet"
-version = "0.7.0.dev1399"
+version = "0.8.0.dev1402"
 description = "Flet for Python - easily build interactive multi-platform apps in Python"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.7.0.dev1399"
+flet-core = "0.8.0.dev1402"
 python = "^3.7"
 typing-extensions = { version = "^4.4.0", python = "<3.8" }
 websocket-client = "^1.4.2"
 watchdog = "^2.2.1"
 oauthlib = "^3.2.2"
 websockets = "^10.4"
 httpx = "^0.23.3"
```

### Comparing `flet-0.7.0.dev1399/src/flet/__pyinstaller/macos_utils.py` & `flet-0.8.0.dev1402/src/flet/__pyinstaller/macos_utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/__pyinstaller/utils.py` & `flet-0.8.0.dev1402/src/flet/__pyinstaller/utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/__pyinstaller/win_utils.py` & `flet-0.8.0.dev1402/src/flet/__pyinstaller/win_utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/async_local_socket_connection.py` & `flet-0.8.0.dev1402/src/flet/async_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/async_websocket_connection.py` & `flet-0.8.0.dev1402/src/flet/async_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/auth/authorization.py` & `flet-0.8.0.dev1402/src/flet/auth/authorization.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/auth/oauth_provider.py` & `flet-0.8.0.dev1402/src/flet/auth/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/auth/oauth_token.py` & `flet-0.8.0.dev1402/src/flet/auth/oauth_token.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/auth/providers/auth0_oauth_provider.py` & `flet-0.8.0.dev1402/src/flet/auth/providers/auth0_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/auth/providers/azure_oauth_provider.py` & `flet-0.8.0.dev1402/src/flet/auth/providers/azure_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/auth/providers/github_oauth_provider.py` & `flet-0.8.0.dev1402/src/flet/auth/providers/github_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/auth/providers/google_oauth_provider.py` & `flet-0.8.0.dev1402/src/flet/auth/providers/google_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/cli/cli.py` & `flet-0.8.0.dev1402/src/flet/cli/cli.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/cli/commands/base.py` & `flet-0.8.0.dev1402/src/flet/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/cli/commands/options.py` & `flet-0.8.0.dev1402/src/flet/cli/commands/options.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/cli/commands/pack.py` & `flet-0.8.0.dev1402/src/flet/cli/commands/pack.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/cli/commands/publish.py` & `flet-0.8.0.dev1402/src/flet/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/cli/commands/run.py` & `flet-0.8.0.dev1402/src/flet/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/flet.py` & `flet-0.8.0.dev1402/src/flet/flet.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/pubsub.py` & `flet-0.8.0.dev1402/src/flet/pubsub.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/reconnecting_websocket.py` & `flet-0.8.0.dev1402/src/flet/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/security.py` & `flet-0.8.0.dev1402/src/flet/security.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/sync_local_socket_connection.py` & `flet-0.8.0.dev1402/src/flet/sync_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/sync_websocket_connection.py` & `flet-0.8.0.dev1402/src/flet/sync_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/utils.py` & `flet-0.8.0.dev1402/src/flet/utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/version.py` & `flet-0.8.0.dev1402/src/flet/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess as sp
 from pathlib import Path
 
 import flet
 from flet.utils import is_windows, which
 
 # this value will be replaced by CI
-version = "0.7.0.dev1399"
+version = "0.8.0.dev1402"
 
 
 def update_version():
     """Return the current version or default."""
     working = Path().absolute()
     os.chdir(Path(flet.__file__).absolute().parent)
     in_repo = which("git.exe" if is_windows() else "git") and sp.run(
```

### Comparing `flet-0.7.0.dev1399/src/flet/web/assets/NOTICES` & `flet-0.8.0.dev1402/src/flet/web/assets/NOTICES`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/web/assets/fonts/MaterialIcons-Regular.otf` & `flet-0.8.0.dev1402/src/flet/web/assets/fonts/MaterialIcons-Regular.otf`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/web/assets/shaders/ink_sparkle.frag` & `flet-0.8.0.dev1402/src/flet/web/assets/shaders/ink_sparkle.frag`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/web/favicon.png` & `flet-0.8.0.dev1402/src/flet/web/favicon.png`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/web/flutter.js` & `flet-0.8.0.dev1402/src/flet/web/flutter.js`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/web/flutter_service_worker.js` & `flet-0.8.0.dev1402/src/flet/web/flutter_service_worker.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -30,16 +30,16 @@
     "canvaskit/skwasm.js": "1df4d741f441fa1a4d10530ced463ef8",
     "canvaskit/canvaskit.js": "76f7d822f42397160c5dfc69cbc9b2de",
     "canvaskit/skwasm.worker.js": "19659053a277272607529ef87acf9d8a",
     "canvaskit/skwasm.wasm": "6711032e17bf49924b2b001cef0d3ea3",
     "canvaskit/chromium/canvaskit.wasm": "fc18c3010856029414b70cae1afc5cd9",
     "canvaskit/chromium/canvaskit.js": "8c8392ce4a4364cbb240aa09b5652e05",
     "python-worker.js": "b961f261b9ad85e06369e83fd2e33bb7",
-    "index.html": "bdb412c3d3be07abcbaa74ab561ae231",
-    "/": "bdb412c3d3be07abcbaa74ab561ae231"
+    "index.html": "ac98dbe57f403a2a0a817c2985d1b10e",
+    "/": "ac98dbe57f403a2a0a817c2985d1b10e"
 };
 // The application shell files that are downloaded before a service worker can
 // start.
 const CORE = ["main.dart.js",
     "index.html",
     "assets/AssetManifest.json",
     "assets/FontManifest.json"
```

### Comparing `flet-0.7.0.dev1399/src/flet/web/icons/apple-touch-icon-192.png` & `flet-0.8.0.dev1402/src/flet/web/icons/apple-touch-icon-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/web/icons/icon-192.png` & `flet-0.8.0.dev1402/src/flet/web/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/web/icons/icon-512.png` & `flet-0.8.0.dev1402/src/flet/web/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/web/icons/icon-maskable-192.png` & `flet-0.8.0.dev1402/src/flet/web/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/web/icons/icon-maskable-512.png` & `flet-0.8.0.dev1402/src/flet/web/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/web/icons/loading-animation.png` & `flet-0.8.0.dev1402/src/flet/web/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/web/index.html` & `flet-0.8.0.dev1402/src/flet/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   <!-- flutterWebRenderer -->
   <!-- useColorEmoji -->
 
   <!-- pyodideCode -->
 
   <script>
     // The value below is injected by flutter build, do not touch.
-    var serviceWorkerVersion = "1754970320";
+    var serviceWorkerVersion = "1958552225";
   </script>
   <!-- This script adds the flutter initialization JS code -->
   <script src="flutter.js" defer></script>
 </head>
 
 <body>
   <div id="loading">
```

### Comparing `flet-0.7.0.dev1399/src/flet/web/main.dart.js` & `flet-0.8.0.dev1402/src/flet/web/main.dart.js`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/web/manifest.json` & `flet-0.8.0.dev1402/src/flet/web/manifest.json`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/web/python-worker.js` & `flet-0.8.0.dev1402/src/flet/web/python-worker.js`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/src/flet/web/python.js` & `flet-0.8.0.dev1402/src/flet/web/python.js`

 * *Files identical despite different names*

### Comparing `flet-0.7.0.dev1399/PKG-INFO` & `flet-0.8.0.dev1402/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flet
-Version: 0.7.0.dev1399
+Version: 0.8.0.dev1402
 Summary: Flet for Python - easily build interactive multi-platform apps in Python
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.7.0.dev1399)
+Requires-Dist: flet-core (==0.8.0.dev1402)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.8"
 Requires-Dist: watchdog (>=2.2.1,<3.0.0)
 Requires-Dist: websocket-client (>=1.4.2,<2.0.0)
 Requires-Dist: websockets (>=10.4,<11.0)
```

