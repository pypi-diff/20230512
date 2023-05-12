# Comparing `tmp/mozart-api-2.5.3.123.0.tar.gz` & `tmp/mozart-api-2.5.3.123.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozart-api-2.5.3.123.0.tar", last modified: Tue Mar 28 14:47:45 2023, max compression
+gzip compressed data, was "mozart-api-2.5.3.123.1.tar", last modified: Fri May 12 13:01:41 2023, max compression
```

## Comparing `mozart-api-2.5.3.123.0.tar` & `mozart-api-2.5.3.123.1.tar`

### file list

```diff
@@ -1,443 +1,443 @@
-drwxr-xr-x   0 markus    (1000) markus    (1000)        0 2023-03-28 14:47:45.185761 mozart-api-2.5.3.123.0/
--rwxr-xr-x   0 markus    (1000) markus    (1000)     1074 2023-03-28 14:47:35.000000 mozart-api-2.5.3.123.0/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)       16 2023-03-28 14:47:36.000000 mozart-api-2.5.3.123.0/MANIFEST.in
--rw-r--r--   0 markus    (1000) markus    (1000)     2322 2023-03-28 14:47:45.185761 mozart-api-2.5.3.123.0/PKG-INFO
--rw-r--r--   0 markus    (1000) markus    (1000)     1473 2023-03-28 14:47:37.000000 mozart-api-2.5.3.123.0/README.md
-drwxr-xr-x   0 markus    (1000) markus    (1000)        0 2023-03-28 14:47:45.142428 mozart-api-2.5.3.123.0/mozart_api/
--rw-r--r--   0 markus    (1000) markus    (1000)    15570 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/__init__.py
-drwxr-xr-x   0 markus    (1000) markus    (1000)        0 2023-03-28 14:47:45.142428 mozart-api-2.5.3.123.0/mozart_api/api/
--rw-r--r--   0 markus    (1000) markus    (1000)      855 2023-03-28 14:47:31.000000 mozart-api-2.5.3.123.0/mozart_api/api/__init__.py
--rw-r--r--   0 markus    (1000) markus    (1000)    53234 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api/beolink_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5189 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api/bluetooth_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5655 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api/content_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5563 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api/deezer_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)   284471 2023-03-28 14:47:41.000000 mozart-api-2.5.3.123.0/mozart_api/api/mozart_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6583 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api/overlay_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)    58466 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api/playback_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)    13498 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api/power_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)    10515 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api/product_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)    16255 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api/remote_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)    20274 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api/scenes_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)    19137 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api/settings_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5182 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api/software_update_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)    64619 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api/sound_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5159 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api/speaker_group_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)    25429 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/api_client.py
--rw-r--r--   0 markus    (1000) markus    (1000)    12514 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/configuration.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3826 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/mozart_api/exceptions.py
-drwxr-xr-x   0 markus    (1000) markus    (1000)        0 2023-03-28 14:47:45.162428 mozart-api-2.5.3.123.0/mozart_api/models/
--rw-r--r--   0 markus    (1000) markus    (1000)    14388 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/__init__.py
--rw-r--r--   0 markus    (1000) markus    (1000)    20396 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/action.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6091 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/alarm_timer_event_data.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4578 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/alarm_triggered_info.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3760 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/ambience.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5967 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/ambience_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4929 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/ambience_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6218 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/art.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3750 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/balance.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5881 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/balance_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4849 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/balance_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3708 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/bass.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5819 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/bass_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4382 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/bass_management.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6733 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/bass_management_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5048 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/bass_management_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4817 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/bass_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     7324 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/battery_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4735 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/beo_remote_button.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3816 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/beolink_available_listener.py
--rw-r--r--   0 markus    (1000) markus    (1000)    12595 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/beolink_experience.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3983 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/beolink_experiences_request.py
--rw-r--r--   0 markus    (1000) markus    (1000)     7215 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/beolink_experiences_result.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5743 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/beolink_join_request.py
--rw-r--r--   0 markus    (1000) markus    (1000)     9947 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/beolink_join_result.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4834 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/beolink_leader.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3744 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/beolink_listener.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4810 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/beolink_peer.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5033 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/bluetooth_device.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3723 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/bluetooth_device_list.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4382 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/button_event.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4365 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/compression.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6641 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/compression_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4961 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/compression_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     7067 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/content_item.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4452 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/directivity.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6788 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/directivity_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5021 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/directivity_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5700 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/error_model.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3730 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/fader.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5813 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/fader_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4793 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/fader_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4464 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/hdmi_input.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5838 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/hdmi_video_format.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3453 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/home_control_uri.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4435 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/install_record_id_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2790 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/listening_mode.py
--rw-r--r--   0 markus    (1000) markus    (1000)    17047 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/listening_mode_features.py
--rw-r--r--   0 markus    (1000) markus    (1000)    11020 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/listening_mode_props.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4815 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/listening_mode_ref.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2818 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/listening_mode_trigger.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3453 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/loudness.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4080 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/microphone_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5092 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/microphones_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     7964 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/overlay_play_request.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4881 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/overlay_play_request_common.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3947 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/overlay_play_request_from_usb.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4787 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/overlay_play_request_from_usb_from_usb.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4194 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/overlay_play_request_text_to_speech.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5633 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/overlay_play_request_text_to_speech_text_to_speech.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3547 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/overlay_play_request_uri.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6183 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/paired_remote.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3690 2023-03-28 14:47:42.000000 mozart-api-2.5.3.123.0/mozart_api/models/paired_remote_response.py
--rw-r--r--   0 markus    (1000) markus    (1000)     9528 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/play_queue_item.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4381 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/play_queue_item_type.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6507 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/play_queue_settings.py
--rw-r--r--   0 markus    (1000) markus    (1000)    29353 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/playback_content_metadata.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4376 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/playback_error.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5114 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/playback_progress.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6340 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/playback_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3839 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/power_link_trigger.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4228 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/power_state_enum.py
--rw-r--r--   0 markus    (1000) markus    (1000)     8324 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/preset.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6499 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/preset_all_of.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5035 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/product_curtain_status.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3916 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/product_friendly_name.py
--rw-r--r--   0 markus    (1000) markus    (1000)    10189 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/product_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)    15235 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/remote_menu_item.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6600 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/remote_menu_item_all_of.py
--rw-r--r--   0 markus    (1000) markus    (1000)    11924 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/remote_menu_item_properties.py
--rw-r--r--   0 markus    (1000) markus    (1000)     9975 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/remote_menu_item_properties_all_of.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5004 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/remote_ui_key_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4326 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/rendering_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4102 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5794 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_current_measurement.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3557 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_debug.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3573 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_enabled.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4228 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_error_details.py
--rw-r--r--   0 markus    (1000) markus    (1000)     8314 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     8661 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_info.py
--rw-r--r--   0 markus    (1000) markus    (1000)     8014 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_measurement_error.py
--rw-r--r--   0 markus    (1000) markus    (1000)    12966 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_properties.py
--rw-r--r--   0 markus    (1000) markus    (1000)    11074 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_properties_all_of.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6880 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4404 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_response.py
--rw-r--r--   0 markus    (1000) markus    (1000)     9962 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_result.py
--rw-r--r--   0 markus    (1000) markus    (1000)    13859 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)    12522 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_state_all_of.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4374 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_state_value.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4781 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_type.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5203 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_version.py
--rw-r--r--   0 markus    (1000) markus    (1000)     8526 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/scene.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4222 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/scene_classification.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4334 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/scene_match.py
--rw-r--r--   0 markus    (1000) markus    (1000)     7362 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/scene_properties.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4936 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/scene_trigger_base_properties.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5762 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/software_update_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     8842 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/software_update_status.py
--rw-r--r--   0 markus    (1000) markus    (1000)     8249 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/sound_adjustments.py
--rw-r--r--   0 markus    (1000) markus    (1000)    20213 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/sound_feature_set.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5880 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/sound_settings.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4690 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/sound_tone_touch.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6678 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/source.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3569 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/source_array.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4937 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/source_type_enum.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3862 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_envelopment.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6291 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_envelopment_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5183 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_envelopment_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3812 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_height.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6121 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_height_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5020 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_height_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4469 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_processing.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6892 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_processing_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5132 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_processing_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3832 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_surround.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6189 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_surround_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5076 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_surround_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3802 2023-03-28 14:47:43.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_width.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6087 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_width_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4992 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/spatial_width_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)    12236 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/speaker_group.py
--rw-r--r--   0 markus    (1000) markus    (1000)    11526 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/speaker_group_member.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5371 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/speaker_group_member_location.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5944 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/speaker_group_overview.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4114 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/speaker_role_enum.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3812 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/speech_enhance.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6121 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/speech_enhance_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5020 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/speech_enhance_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3585 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/stand_connected.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3499 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/stand_position.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4161 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/tone_touch.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3708 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/tone_touch_type.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5079 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/tone_touch_type_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6028 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/tone_touch_x_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6028 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/tone_touch_y_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3728 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/treble.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5887 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/treble_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4873 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/treble_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3806 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/tv_info_event_data.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4135 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/tv_integration_types.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5323 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/tv_properties.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4563 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/tv_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3470 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/uri.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3488 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/user_flow.py
--rw-r--r--   0 markus    (1000) markus    (1000)     8739 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/video_pixel_format.py
--rw-r--r--   0 markus    (1000) markus    (1000)     6538 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/video_timings.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3471 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/volume_level.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3469 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/volume_mute.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4444 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/volume_settings.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5999 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/volume_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4756 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_active_hdmi_input_signal.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4805 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_active_listening_mode.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4809 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_active_speaker_group.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4706 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_alarm_timer.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4745 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_alarm_triggered.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4612 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_battery.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4733 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_beo_remote_button.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5341 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_beolink_experiences_result.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5201 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_beolink_join_result.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4592 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_button.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4689 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_curtains.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4805 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_hdmi_video_format_signal.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4769 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_notification.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4692 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_playback_error.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4809 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_playback_metadata.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4752 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_playback_progress.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4647 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_playback_source.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4700 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_playback_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4665 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_power_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4882 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_puc_install_remote_id_status.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4601 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_role.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5206 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_room_compensation_current_measurement_event.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4894 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_room_compensation_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4813 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_software_update_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4692 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_sound_settings.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4623 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_source_change.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4645 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_speaker_group_changed.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4712 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_stand_connected.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4692 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_stand_position.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4626 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_tv_info.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4592 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_volume.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5101 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_wisa_out_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5359 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/websocket_notification_tag.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4198 2023-03-28 14:47:44.000000 mozart-api-2.5.3.123.0/mozart_api/models/wisa_out_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)    10942 2023-03-28 14:47:36.000000 mozart-api-2.5.3.123.0/mozart_api/mozart_cli.py
--rw-r--r--   0 markus    (1000) markus    (1000)    25833 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/mozart_client.py
--rw-r--r--   0 markus    (1000) markus    (1000)    12570 2023-03-28 14:47:40.000000 mozart-api-2.5.3.123.0/mozart_api/rest.py
-drwxr-xr-x   0 markus    (1000) markus    (1000)        0 2023-03-28 14:47:45.142428 mozart-api-2.5.3.123.0/mozart_api.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     2322 2023-03-28 14:47:45.000000 mozart-api-2.5.3.123.0/mozart_api.egg-info/PKG-INFO
--rw-r--r--   0 markus    (1000) markus    (1000)    16305 2023-03-28 14:47:45.000000 mozart-api-2.5.3.123.0/mozart_api.egg-info/SOURCES.txt
--rw-r--r--   0 markus    (1000) markus    (1000)        1 2023-03-28 14:47:45.000000 mozart-api-2.5.3.123.0/mozart_api.egg-info/dependency_links.txt
--rw-r--r--   0 markus    (1000) markus    (1000)       66 2023-03-28 14:47:45.000000 mozart-api-2.5.3.123.0/mozart_api.egg-info/entry_points.txt
--rw-r--r--   0 markus    (1000) markus    (1000)       64 2023-03-28 14:47:45.000000 mozart-api-2.5.3.123.0/mozart_api.egg-info/requires.txt
--rw-r--r--   0 markus    (1000) markus    (1000)       11 2023-03-28 14:47:45.000000 mozart-api-2.5.3.123.0/mozart_api.egg-info/top_level.txt
--rw-r--r--   0 markus    (1000) markus    (1000)       69 2023-03-28 14:47:45.185761 mozart-api-2.5.3.123.0/setup.cfg
--rw-r--r--   0 markus    (1000) markus    (1000)     3264 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/setup.py
-drwxr-xr-x   0 markus    (1000) markus    (1000)        0 2023-03-28 14:47:45.185761 mozart-api-2.5.3.123.0/test/
--rw-r--r--   0 markus    (1000) markus    (1000)     4281 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_action.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1405 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_alarm_timer_event_data.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1376 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_alarm_triggered_info.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1298 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_ambience.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1952 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_ambience_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1872 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_ambience_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1248 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_art.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1287 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_balance.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1933 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_balance_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1853 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_balance_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1248 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_bass.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1858 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_bass_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1364 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_bass_management.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2075 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_bass_management_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1988 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_bass_management_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1784 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_bass_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1475 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_battery_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1350 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_beo_remote_button.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2628 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_beolink_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1601 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_beolink_available_listener.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1809 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_beolink_experience.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1604 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_beolink_experiences_request.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2596 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_beolink_experiences_result.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1646 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_beolink_join_request.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1798 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_beolink_join_result.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1523 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_beolink_leader.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1491 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_beolink_listener.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1501 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_beolink_peer.py
--rw-r--r--   0 markus    (1000) markus    (1000)      889 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_bluetooth_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1361 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_bluetooth_device.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1630 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_bluetooth_device_list.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1301 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_button_event.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1331 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_compression.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2009 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_compression_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1929 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_compression_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)      842 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_content_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1697 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_content_item.py
--rw-r--r--   0 markus    (1000) markus    (1000)      910 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_deezer_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1335 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_directivity.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2021 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_directivity_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1937 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_directivity_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1316 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_error_model.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1265 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_fader.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1895 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_fader_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1815 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_fader_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1284 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_hdmi_input.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1893 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_hdmi_video_format.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1322 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_home_control_uri.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1395 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_install_record_id_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1302 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_listening_mode.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3432 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_listening_mode_features.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3866 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_listening_mode_props.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1412 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_listening_mode_ref.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1381 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_listening_mode_trigger.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1255 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_loudness.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1334 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_microphone_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1627 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_microphones_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)    10662 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_mozart_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)      835 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_overlay_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1910 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_overlay_play_request.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1453 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_overlay_play_request_common.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1636 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_overlay_play_request_from_usb.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1595 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_overlay_play_request_from_usb_from_usb.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1746 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_overlay_play_request_text_to_speech.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1705 2023-03-28 14:47:38.000000 mozart-api-2.5.3.123.0/test/test_overlay_play_request_text_to_speech_text_to_speech.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1515 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_overlay_play_request_uri.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1397 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_paired_remote.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1636 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_paired_remote_response.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3351 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_play_queue_item.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1403 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_play_queue_item_type.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1432 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_play_queue_settings.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2662 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_playback_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2746 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_playback_content_metadata.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2909 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_playback_error.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1373 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_playback_progress.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3557 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_playback_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1146 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_power_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1357 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_power_link_trigger.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1337 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_power_state_enum.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1798 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_preset.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1578 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_preset_all_of.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1029 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_product_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1412 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_product_curtain_status.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1387 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_product_friendly_name.py
--rw-r--r--   0 markus    (1000) markus    (1000)    10158 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_product_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1164 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_remote_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2061 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_remote_menu_item.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1612 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_remote_menu_item_all_of.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1957 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_remote_menu_item_properties.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1737 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_remote_menu_item_properties_all_of.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1357 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_remote_ui_key_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1325 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_rendering_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1388 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1615 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_current_measurement.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1411 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_debug.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1433 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_enabled.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1759 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_error_details.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1645 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4329 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_info.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1593 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_measurement_error.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1705 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_properties.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1732 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_properties_all_of.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1581 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1458 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_response.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3425 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_result.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2120 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2143 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_state_all_of.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1476 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_state_value.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1395 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_type.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1450 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_room_compensation_version.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1860 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_scene.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1391 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_scene_classification.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1290 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_scene_match.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1931 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_scene_properties.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1750 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_scene_trigger_base_properties.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1379 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_scenes_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1390 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_settings_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)      921 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_software_update_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1404 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_software_update_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2200 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_software_update_status.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1556 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_sound_adjustments.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3256 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_sound_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1932 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_sound_feature_set.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5139 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_sound_settings.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1340 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_sound_tone_touch.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1481 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_source.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1711 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_source_array.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1330 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_source_type_enum.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1410 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_envelopment.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2157 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_envelopment_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2077 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_envelopment_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1355 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_height.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2053 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_height_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1973 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_height_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1405 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_processing.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2156 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_processing_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2070 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_processing_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1377 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_surround.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2100 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_surround_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2011 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_surround_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1344 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_width.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2034 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_width_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1954 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_spatial_width_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2207 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_speaker_group.py
--rw-r--r--   0 markus    (1000) markus    (1000)      895 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_speaker_group_api.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1813 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_speaker_group_member.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1553 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_speaker_group_member_location.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1534 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_speaker_group_overview.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1344 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_speaker_role_enum.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1355 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_speech_enhance.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2053 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_speech_enhance_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1973 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_speech_enhance_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1327 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_stand_connected.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1313 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_stand_position.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1509 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_tone_touch.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1357 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_tone_touch_type.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1979 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_tone_touch_type_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2026 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_tone_touch_x_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2026 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_tone_touch_y_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1270 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_treble.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1896 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_treble_feature.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1822 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_treble_range.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1486 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_tv_info_event_data.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1377 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_tv_integration_types.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1511 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_tv_properties.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1711 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_tv_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1202 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_uri.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1258 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_user_flow.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1499 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_video_pixel_format.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1455 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_video_timings.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1288 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_volume_level.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1279 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_volume_mute.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1560 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_volume_settings.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1661 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_volume_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1762 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_active_hdmi_input_signal.py
--rw-r--r--   0 markus    (1000) markus    (1000)     4403 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_active_listening_mode.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1789 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_active_speaker_group.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1686 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_alarm_timer.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1691 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_alarm_triggered.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1727 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_battery.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1705 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_beo_remote_button.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3166 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_beolink_experiences_result.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2305 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_beolink_join_result.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1581 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_button.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1641 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_curtains.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2313 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_hdmi_video_format_signal.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1663 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_notification.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3364 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_playback_error.py
--rw-r--r--   0 markus    (1000) markus    (1000)     3122 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_playback_metadata.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1749 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_playback_progress.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1879 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_playback_source.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1646 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_playback_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1624 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_power_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1787 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_puc_install_remote_id_status.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1545 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_role.py
--rw-r--r--   0 markus    (1000) markus    (1000)     2027 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_room_compensation_current_measurement_event.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1768 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_room_compensation_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1767 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_software_update_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     5750 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_sound_settings.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1857 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_source_change.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1569 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_speaker_group_changed.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1659 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_stand_connected.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1643 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_stand_position.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1697 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_tv_info.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1863 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_volume.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1806 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_web_socket_event_wisa_out_state.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1455 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_websocket_notification_tag.py
--rw-r--r--   0 markus    (1000) markus    (1000)     1305 2023-03-28 14:47:39.000000 mozart-api-2.5.3.123.0/test/test_wisa_out_state.py
+drwxr-xr-x   0 markus    (1000) markus    (1000)        0 2023-05-12 13:01:41.194820 mozart-api-2.5.3.123.1/
+-rwxr-xr-x   0 markus    (1000) markus    (1000)     1074 2023-05-12 13:01:32.000000 mozart-api-2.5.3.123.1/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)       16 2023-05-12 13:01:33.000000 mozart-api-2.5.3.123.1/MANIFEST.in
+-rw-r--r--   0 markus    (1000) markus    (1000)     2557 2023-05-12 13:01:41.194820 mozart-api-2.5.3.123.1/PKG-INFO
+-rw-r--r--   0 markus    (1000) markus    (1000)     1706 2023-05-12 13:01:33.000000 mozart-api-2.5.3.123.1/README.md
+drwxr-xr-x   0 markus    (1000) markus    (1000)        0 2023-05-12 13:01:41.148153 mozart-api-2.5.3.123.1/mozart_api/
+-rw-r--r--   0 markus    (1000) markus    (1000)    15570 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/__init__.py
+drwxr-xr-x   0 markus    (1000) markus    (1000)        0 2023-05-12 13:01:41.151486 mozart-api-2.5.3.123.1/mozart_api/api/
+-rw-r--r--   0 markus    (1000) markus    (1000)      855 2023-05-12 13:01:27.000000 mozart-api-2.5.3.123.1/mozart_api/api/__init__.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    53234 2023-05-12 13:01:37.000000 mozart-api-2.5.3.123.1/mozart_api/api/beolink_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5189 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/api/bluetooth_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5655 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/api/content_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5563 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/api/deezer_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)   284471 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/api/mozart_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6583 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/api/overlay_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    58466 2023-05-12 13:01:37.000000 mozart-api-2.5.3.123.1/mozart_api/api/playback_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    13498 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/api/power_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    10515 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/api/product_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    16255 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/api/remote_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    20274 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/api/scenes_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    19137 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/api/settings_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5182 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/api/software_update_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    64619 2023-05-12 13:01:37.000000 mozart-api-2.5.3.123.1/mozart_api/api/sound_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5159 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/api/speaker_group_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    25428 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/api_client.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    12514 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/configuration.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3826 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/exceptions.py
+drwxr-xr-x   0 markus    (1000) markus    (1000)        0 2023-05-12 13:01:41.171487 mozart-api-2.5.3.123.1/mozart_api/models/
+-rw-r--r--   0 markus    (1000) markus    (1000)    14388 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/__init__.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    20402 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/action.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6097 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/alarm_timer_event_data.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4584 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/alarm_triggered_info.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3766 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/ambience.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5973 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/ambience_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4935 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/ambience_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6224 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/art.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3756 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/balance.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5887 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/balance_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4855 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/balance_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3714 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/bass.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5825 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/bass_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4388 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/bass_management.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6739 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/bass_management_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5054 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/bass_management_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4823 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/bass_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     7330 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/battery_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4741 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/beo_remote_button.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3822 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/beolink_available_listener.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    12601 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/beolink_experience.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3989 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/beolink_experiences_request.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     7221 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/beolink_experiences_result.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5749 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/beolink_join_request.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     9953 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/beolink_join_result.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4840 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/beolink_leader.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3750 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/beolink_listener.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4816 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/beolink_peer.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5039 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/bluetooth_device.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3729 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/bluetooth_device_list.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4388 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/button_event.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4371 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/compression.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6647 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/compression_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4967 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/compression_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     7073 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/content_item.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4458 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/directivity.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6794 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/directivity_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5027 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/directivity_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5706 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/error_model.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3736 2023-05-12 13:01:38.000000 mozart-api-2.5.3.123.1/mozart_api/models/fader.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5819 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/fader_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4799 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/fader_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4470 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/hdmi_input.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5844 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/hdmi_video_format.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3459 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/home_control_uri.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4441 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/install_record_id_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2796 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/listening_mode.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    17053 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/listening_mode_features.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    11026 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/listening_mode_props.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4821 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/listening_mode_ref.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2824 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/listening_mode_trigger.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3459 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/loudness.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4086 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/microphone_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5098 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/microphones_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     7970 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/overlay_play_request.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4887 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/overlay_play_request_common.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3953 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/overlay_play_request_from_usb.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4793 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/overlay_play_request_from_usb_from_usb.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4200 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/overlay_play_request_text_to_speech.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5639 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/overlay_play_request_text_to_speech_text_to_speech.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3553 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/overlay_play_request_uri.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6189 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/paired_remote.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3696 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/paired_remote_response.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     9534 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/play_queue_item.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4387 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/play_queue_item_type.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6513 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/play_queue_settings.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    29359 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/playback_content_metadata.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4382 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/playback_error.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5120 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/playback_progress.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6346 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/playback_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3845 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/power_link_trigger.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4234 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/power_state_enum.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     8330 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/preset.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6505 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/preset_all_of.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5041 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/product_curtain_status.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3922 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/product_friendly_name.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    10195 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/product_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    15241 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/remote_menu_item.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6606 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/remote_menu_item_all_of.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    11930 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/remote_menu_item_properties.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     9981 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/remote_menu_item_properties_all_of.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5010 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/remote_ui_key_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4332 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/rendering_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4108 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5800 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_current_measurement.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3563 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_debug.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3579 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_enabled.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4234 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_error_details.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     8320 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     8667 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_info.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     8020 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_measurement_error.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    12972 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_properties.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    11080 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_properties_all_of.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6886 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4410 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_response.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     9968 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_result.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    13865 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    12528 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_state_all_of.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4380 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_state_value.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4787 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_type.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5209 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_version.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     8532 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/scene.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4228 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/scene_classification.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4340 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/scene_match.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     7368 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/scene_properties.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4942 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/scene_trigger_base_properties.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5768 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/software_update_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     8848 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/software_update_status.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     8255 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/sound_adjustments.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    20219 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/sound_feature_set.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5886 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/sound_settings.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4696 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/sound_tone_touch.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6684 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/source.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3575 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/source_array.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4943 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/source_type_enum.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3868 2023-05-12 13:01:39.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_envelopment.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6297 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_envelopment_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5189 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_envelopment_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3818 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_height.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6127 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_height_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5026 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_height_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4475 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_processing.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6898 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_processing_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5138 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_processing_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3838 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_surround.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6195 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_surround_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5082 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_surround_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3808 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_width.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6093 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_width_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4998 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/spatial_width_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    12242 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/speaker_group.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    11532 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/speaker_group_member.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5377 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/speaker_group_member_location.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5950 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/speaker_group_overview.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4120 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/speaker_role_enum.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3818 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/speech_enhance.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6127 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/speech_enhance_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5026 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/speech_enhance_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3591 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/stand_connected.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3505 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/stand_position.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4167 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/tone_touch.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3714 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/tone_touch_type.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5085 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/tone_touch_type_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6034 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/tone_touch_x_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6034 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/tone_touch_y_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3734 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/treble.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5893 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/treble_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4879 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/treble_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3812 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/tv_info_event_data.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4141 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/tv_integration_types.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5329 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/tv_properties.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4569 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/tv_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3476 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/uri.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3494 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/user_flow.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     8745 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/video_pixel_format.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6544 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/video_timings.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3477 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/volume_level.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3475 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/volume_mute.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4450 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/volume_settings.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     6005 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/volume_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4762 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_active_hdmi_input_signal.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4811 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_active_listening_mode.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4815 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_active_speaker_group.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4712 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_alarm_timer.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4751 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_alarm_triggered.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4618 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_battery.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4739 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_beo_remote_button.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5347 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_beolink_experiences_result.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5207 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_beolink_join_result.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4598 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_button.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4695 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_curtains.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4811 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_hdmi_video_format_signal.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4775 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_notification.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4698 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_playback_error.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4815 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_playback_metadata.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4758 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_playback_progress.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4653 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_playback_source.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4706 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_playback_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4671 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_power_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4888 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_puc_install_remote_id_status.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4607 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_role.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5212 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_room_compensation_current_measurement_event.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4900 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_room_compensation_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4819 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_software_update_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4698 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_sound_settings.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4629 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_source_change.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4651 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_speaker_group_changed.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4718 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_stand_connected.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4698 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_stand_position.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4632 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_tv_info.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4598 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_volume.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5107 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_wisa_out_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5365 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/websocket_notification_tag.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4204 2023-05-12 13:01:40.000000 mozart-api-2.5.3.123.1/mozart_api/models/wisa_out_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    11060 2023-05-12 13:01:32.000000 mozart-api-2.5.3.123.1/mozart_api/mozart_cli.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    25833 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/mozart_client.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    12570 2023-05-12 13:01:36.000000 mozart-api-2.5.3.123.1/mozart_api/rest.py
+drwxr-xr-x   0 markus    (1000) markus    (1000)        0 2023-05-12 13:01:41.151486 mozart-api-2.5.3.123.1/mozart_api.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     2557 2023-05-12 13:01:41.000000 mozart-api-2.5.3.123.1/mozart_api.egg-info/PKG-INFO
+-rw-r--r--   0 markus    (1000) markus    (1000)    16305 2023-05-12 13:01:41.000000 mozart-api-2.5.3.123.1/mozart_api.egg-info/SOURCES.txt
+-rw-r--r--   0 markus    (1000) markus    (1000)        1 2023-05-12 13:01:41.000000 mozart-api-2.5.3.123.1/mozart_api.egg-info/dependency_links.txt
+-rw-r--r--   0 markus    (1000) markus    (1000)       66 2023-05-12 13:01:41.000000 mozart-api-2.5.3.123.1/mozart_api.egg-info/entry_points.txt
+-rw-r--r--   0 markus    (1000) markus    (1000)       64 2023-05-12 13:01:41.000000 mozart-api-2.5.3.123.1/mozart_api.egg-info/requires.txt
+-rw-r--r--   0 markus    (1000) markus    (1000)       11 2023-05-12 13:01:41.000000 mozart-api-2.5.3.123.1/mozart_api.egg-info/top_level.txt
+-rw-r--r--   0 markus    (1000) markus    (1000)       69 2023-05-12 13:01:41.194820 mozart-api-2.5.3.123.1/setup.cfg
+-rw-r--r--   0 markus    (1000) markus    (1000)     3499 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/setup.py
+drwxr-xr-x   0 markus    (1000) markus    (1000)        0 2023-05-12 13:01:41.194820 mozart-api-2.5.3.123.1/test/
+-rw-r--r--   0 markus    (1000) markus    (1000)     4281 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_action.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1405 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_alarm_timer_event_data.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1376 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_alarm_triggered_info.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1298 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_ambience.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1952 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_ambience_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1872 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_ambience_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1248 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_art.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1287 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_balance.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1933 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_balance_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1853 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_balance_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1248 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_bass.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1858 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_bass_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1364 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_bass_management.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2075 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_bass_management_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1988 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_bass_management_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1784 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_bass_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1475 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_battery_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1350 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_beo_remote_button.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2628 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_beolink_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1601 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_beolink_available_listener.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1809 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_beolink_experience.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1604 2023-05-12 13:01:34.000000 mozart-api-2.5.3.123.1/test/test_beolink_experiences_request.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2596 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_beolink_experiences_result.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1646 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_beolink_join_request.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1798 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_beolink_join_result.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1523 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_beolink_leader.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1491 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_beolink_listener.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1501 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_beolink_peer.py
+-rw-r--r--   0 markus    (1000) markus    (1000)      889 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_bluetooth_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1361 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_bluetooth_device.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1630 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_bluetooth_device_list.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1301 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_button_event.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1331 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_compression.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2009 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_compression_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1929 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_compression_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)      842 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_content_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1697 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_content_item.py
+-rw-r--r--   0 markus    (1000) markus    (1000)      910 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_deezer_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1335 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_directivity.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2021 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_directivity_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1937 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_directivity_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1316 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_error_model.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1265 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_fader.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1895 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_fader_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1815 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_fader_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1284 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_hdmi_input.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1893 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_hdmi_video_format.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1322 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_home_control_uri.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1395 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_install_record_id_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1302 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_listening_mode.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3432 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_listening_mode_features.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3866 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_listening_mode_props.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1412 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_listening_mode_ref.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1381 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_listening_mode_trigger.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1255 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_loudness.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1334 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_microphone_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1627 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_microphones_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    10662 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_mozart_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)      835 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_overlay_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1910 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_overlay_play_request.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1453 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_overlay_play_request_common.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1636 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_overlay_play_request_from_usb.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1595 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_overlay_play_request_from_usb_from_usb.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1746 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_overlay_play_request_text_to_speech.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1705 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_overlay_play_request_text_to_speech_text_to_speech.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1515 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_overlay_play_request_uri.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1397 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_paired_remote.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1636 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_paired_remote_response.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3351 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_play_queue_item.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1403 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_play_queue_item_type.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1432 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_play_queue_settings.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2662 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_playback_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2746 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_playback_content_metadata.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2909 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_playback_error.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1373 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_playback_progress.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3557 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_playback_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1146 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_power_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1357 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_power_link_trigger.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1337 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_power_state_enum.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1798 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_preset.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1578 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_preset_all_of.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1029 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_product_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1412 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_product_curtain_status.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1387 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_product_friendly_name.py
+-rw-r--r--   0 markus    (1000) markus    (1000)    10158 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_product_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1164 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_remote_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2061 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_remote_menu_item.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1612 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_remote_menu_item_all_of.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1957 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_remote_menu_item_properties.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1737 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_remote_menu_item_properties_all_of.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1357 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_remote_ui_key_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1325 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_rendering_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1388 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1615 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_current_measurement.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1411 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_debug.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1433 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_enabled.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1759 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_error_details.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1645 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4329 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_info.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1593 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_measurement_error.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1705 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_properties.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1732 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_properties_all_of.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1581 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1458 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_response.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3425 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_result.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2120 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2143 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_state_all_of.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1476 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_state_value.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1395 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_type.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1450 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_room_compensation_version.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1860 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_scene.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1391 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_scene_classification.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1290 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_scene_match.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1931 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_scene_properties.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1750 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_scene_trigger_base_properties.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1379 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_scenes_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1390 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_settings_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)      921 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_software_update_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1404 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_software_update_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2200 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_software_update_status.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1556 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_sound_adjustments.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3256 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_sound_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1932 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_sound_feature_set.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5139 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_sound_settings.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1340 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_sound_tone_touch.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1481 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_source.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1711 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_source_array.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1330 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_source_type_enum.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1410 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_envelopment.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2157 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_envelopment_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2077 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_envelopment_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1355 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_height.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2053 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_height_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1973 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_height_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1405 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_processing.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2156 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_processing_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2070 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_processing_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1377 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_surround.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2100 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_surround_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2011 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_surround_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1344 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_width.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2034 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_width_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1954 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_spatial_width_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2207 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_speaker_group.py
+-rw-r--r--   0 markus    (1000) markus    (1000)      895 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_speaker_group_api.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1813 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_speaker_group_member.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1553 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_speaker_group_member_location.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1534 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_speaker_group_overview.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1344 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_speaker_role_enum.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1355 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_speech_enhance.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2053 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_speech_enhance_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1973 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_speech_enhance_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1327 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_stand_connected.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1313 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_stand_position.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1509 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_tone_touch.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1357 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_tone_touch_type.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1979 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_tone_touch_type_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2026 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_tone_touch_x_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2026 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_tone_touch_y_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1270 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_treble.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1896 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_treble_feature.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1822 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_treble_range.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1486 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_tv_info_event_data.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1377 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_tv_integration_types.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1511 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_tv_properties.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1711 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_tv_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1202 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_uri.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1258 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_user_flow.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1499 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_video_pixel_format.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1455 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_video_timings.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1288 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_volume_level.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1279 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_volume_mute.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1560 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_volume_settings.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1661 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_volume_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1762 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_active_hdmi_input_signal.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     4403 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_active_listening_mode.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1789 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_active_speaker_group.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1686 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_alarm_timer.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1691 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_alarm_triggered.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1727 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_battery.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1705 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_beo_remote_button.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3166 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_beolink_experiences_result.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2305 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_beolink_join_result.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1581 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_button.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1641 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_curtains.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2313 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_hdmi_video_format_signal.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1663 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_notification.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3364 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_playback_error.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     3122 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_playback_metadata.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1749 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_playback_progress.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1879 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_playback_source.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1646 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_playback_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1624 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_power_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1787 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_puc_install_remote_id_status.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1545 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_role.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     2027 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_room_compensation_current_measurement_event.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1768 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_room_compensation_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1767 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_software_update_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     5750 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_sound_settings.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1857 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_source_change.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1569 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_speaker_group_changed.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1659 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_stand_connected.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1643 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_stand_position.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1697 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_tv_info.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1863 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_volume.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1806 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_web_socket_event_wisa_out_state.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1455 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_websocket_notification_tag.py
+-rw-r--r--   0 markus    (1000) markus    (1000)     1305 2023-05-12 13:01:35.000000 mozart-api-2.5.3.123.1/test/test_wisa_out_state.py
```

### Comparing `mozart-api-2.5.3.123.0/LICENSE` & `mozart-api-2.5.3.123.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/PKG-INFO` & `mozart-api-2.5.3.123.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: mozart-api
-Version: 2.5.3.123.0
+Version: 2.5.3.123.1
 Summary: Mozart platform API
 Home-page: https://pypi.org/project/mozart-api/
 Author: BangOlufsen
 Author-email: support@bang-olufsen.dk
 License: MIT
 Project-URL: Github, https://github.com/bang-olufsen/mozart-open-api
 Project-URL: Documentation, https://bang-olufsen.github.io/mozart-open-api/
 Project-URL: Bug tracker, https://github.com/bang-olufsen/mozart-open-api/issues
 Keywords: OpenAPI,OpenAPI-Generator,Mozart platform API
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Multimedia
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Mozart platform API
 
 [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/bang-olufsen/mozart-open-api/blob/main/LICENSE)
 [![Version](https://img.shields.io/pypi/v/mozart-api?color=g)](https://pypi.org/project/mozart-api)
@@ -30,13 +30,16 @@
 [![Balance stereo](https://raw.githubusercontent.com/bang-olufsen/mozart-open-api/main/docs/media/balance_stereo.png)](https://www.bang-olufsen.com/en/dk/speakers/beosound-balance-stereo-set?variant=beosound-balance-gva-naturaloak-bundle)
 
 The Mozart API is a REST API with async capabilities and WebSocket notification channel for immediate state information. Currently the API is distributed as a Python package and as an OpenAPI document that can be found in the [Github releases](https://github.com/bang-olufsen/mozart-open-api/releases).
 
 Supported by:
 
 - [Beolab 28](https://www.bang-olufsen.com/en/dk/speakers/beolab-28)
+- [Beosound 2 3rd gen](https://www.bang-olufsen.com/en/dk/speakers/beosound-2)
+- [Beosound A5](https://www.bang-olufsen.com/en/dk/speakers/beosound-a5)
+- [Beosound A9 5th gen](https://www.bang-olufsen.com/en/dk/speakers/beosound-a9)
 - [Beosound Balance](https://www.bang-olufsen.com/en/dk/speakers/beosound-balance)
 - [Beosound Emerge](https://www.bang-olufsen.com/en/dk/speakers/beosound-emerge)
 - [Beosound Level](https://www.bang-olufsen.com/en/dk/speakers/beosound-level)
 - [Beosound Theatre](https://www.bang-olufsen.com/en/dk/soundbars/beosound-theatre)
 
 API documentation can be found on the [Github page](https://bang-olufsen.github.io/mozart-open-api).
```

### Comparing `mozart-api-2.5.3.123.0/README.md` & `mozart-api-2.5.3.123.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,13 +8,16 @@
 [![Balance stereo](https://raw.githubusercontent.com/bang-olufsen/mozart-open-api/main/docs/media/balance_stereo.png)](https://www.bang-olufsen.com/en/dk/speakers/beosound-balance-stereo-set?variant=beosound-balance-gva-naturaloak-bundle)
 
 The Mozart API is a REST API with async capabilities and WebSocket notification channel for immediate state information. Currently the API is distributed as a Python package and as an OpenAPI document that can be found in the [Github releases](https://github.com/bang-olufsen/mozart-open-api/releases).
 
 Supported by:
 
 - [Beolab 28](https://www.bang-olufsen.com/en/dk/speakers/beolab-28)
+- [Beosound 2 3rd gen](https://www.bang-olufsen.com/en/dk/speakers/beosound-2)
+- [Beosound A5](https://www.bang-olufsen.com/en/dk/speakers/beosound-a5)
+- [Beosound A9 5th gen](https://www.bang-olufsen.com/en/dk/speakers/beosound-a9)
 - [Beosound Balance](https://www.bang-olufsen.com/en/dk/speakers/beosound-balance)
 - [Beosound Emerge](https://www.bang-olufsen.com/en/dk/speakers/beosound-emerge)
 - [Beosound Level](https://www.bang-olufsen.com/en/dk/speakers/beosound-level)
 - [Beosound Theatre](https://www.bang-olufsen.com/en/dk/soundbars/beosound-theatre)
 
 API documentation can be found on the [Github page](https://bang-olufsen.github.io/mozart-open-api).
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/__init__.py` & `mozart-api-2.5.3.123.1/mozart_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: support@bang-olufsen.dk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.5.3.123.0"
+__version__ = "2.5.3.123.1"
 
 # import apis into sdk package
 from mozart_api.api.beolink_api import BeolinkApi
 from mozart_api.api.bluetooth_api import BluetoothApi
 from mozart_api.api.content_api import ContentApi
 from mozart_api.api.deezer_api import DeezerApi
 from mozart_api.api.overlay_api import OverlayApi
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/__init__.py` & `mozart-api-2.5.3.123.1/mozart_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/beolink_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/beolink_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/bluetooth_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/bluetooth_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/content_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/content_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/deezer_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/deezer_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/mozart_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/mozart_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/overlay_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/overlay_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/playback_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/playback_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/power_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/power_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/product_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/product_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/remote_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/remote_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/scenes_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/scenes_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/settings_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/settings_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/software_update_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/software_update_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/sound_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/sound_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api/speaker_group_api.py` & `mozart-api-2.5.3.123.1/mozart_api/api/speaker_group_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/api_client.py` & `mozart-api-2.5.3.123.1/mozart_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "OpenAPI-Generator/2.5.3.123.0/python"
+        self.user_agent = "OpenAPI-Generator/2.5.3.123.1/python"
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
@@ -139,15 +139,14 @@
         auth_settings=None,
         _return_http_data_only=None,
         collection_formats=None,
         _preload_content=True,
         _request_timeout=None,
         _host=None,
     ):
-
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
         if self.cookie:
             header_params["Cookie"] = self.cookie
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/configuration.py` & `mozart-api-2.5.3.123.1/mozart_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: 0.2.0\n"
-            "SDK Package Version: 2.5.3.123.0".format(
+            "SDK Package Version: 2.5.3.123.1".format(
                 env=sys.platform, pyversion=sys.version
             )
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/exceptions.py` & `mozart-api-2.5.3.123.1/mozart_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/__init__.py` & `mozart-api-2.5.3.123.1/mozart_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/action.py` & `mozart-api-2.5.3.123.1/mozart_api/models/action.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.source_type_enum import SourceTypeEnum
-from mozart_api.models.play_queue_settings import PlayQueueSettings
 from mozart_api.models.stand_position import StandPosition
+from mozart_api.models.play_queue_settings import PlayQueueSettings
 from mozart_api.models.play_queue_item import PlayQueueItem
 
 from mozart_api.configuration import Configuration
 
 
 class Action(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/alarm_timer_event_data.py` & `mozart-api-2.5.3.123.1/mozart_api/models/alarm_timer_event_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class AlarmTimerEventData(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/alarm_triggered_info.py` & `mozart-api-2.5.3.123.1/mozart_api/models/alarm_triggered_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class AlarmTriggeredInfo(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/ambience.py` & `mozart-api-2.5.3.123.1/mozart_api/models/ambience.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class Ambience(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/ambience_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/ambience_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.ambience import Ambience
 
 from mozart_api.configuration import Configuration
 
 
 class AmbienceFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/ambience_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/ambience_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.ambience import Ambience
 
 from mozart_api.configuration import Configuration
 
 
 class AmbienceRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/art.py` & `mozart-api-2.5.3.123.1/mozart_api/models/art.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class Art(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/balance.py` & `mozart-api-2.5.3.123.1/mozart_api/models/balance.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class Balance(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/balance_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/balance_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.balance import Balance
 
 from mozart_api.configuration import Configuration
 
 
 class BalanceFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/balance_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/balance_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.balance import Balance
 
 from mozart_api.configuration import Configuration
 
 
 class BalanceRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/bass.py` & `mozart-api-2.5.3.123.1/mozart_api/models/bass.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class Bass(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/bass_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/bass_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.bass import Bass
 
 from mozart_api.configuration import Configuration
 
 
 class BassFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/bass_management.py` & `mozart-api-2.5.3.123.1/mozart_api/models/bass_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class BassManagement(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/bass_management_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/bass_management_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.bass_management import BassManagement
 
 from mozart_api.configuration import Configuration
 
 
 class BassManagementFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/bass_management_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/bass_management_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.bass_management import BassManagement
 
 from mozart_api.configuration import Configuration
 
 
 class BassManagementRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/bass_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/bass_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.bass import Bass
 
 from mozart_api.configuration import Configuration
 
 
 class BassRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/battery_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/battery_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class BatteryState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/beo_remote_button.py` & `mozart-api-2.5.3.123.1/mozart_api/models/beo_remote_button.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class BeoRemoteButton(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/beolink_available_listener.py` & `mozart-api-2.5.3.123.1/mozart_api/models/beolink_available_listener.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class BeolinkAvailableListener(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/beolink_experience.py` & `mozart-api-2.5.3.123.1/mozart_api/models/beolink_experience.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class BeolinkExperience(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/beolink_experiences_request.py` & `mozart-api-2.5.3.123.1/mozart_api/models/beolink_experiences_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class BeolinkExperiencesRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/beolink_experiences_result.py` & `mozart-api-2.5.3.123.1/mozart_api/models/beolink_experiences_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.beolink_experience import BeolinkExperience
 
 from mozart_api.configuration import Configuration
 
 
 class BeolinkExperiencesResult(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/beolink_join_request.py` & `mozart-api-2.5.3.123.1/mozart_api/models/beolink_join_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class BeolinkJoinRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/beolink_join_result.py` & `mozart-api-2.5.3.123.1/mozart_api/models/beolink_join_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class BeolinkJoinResult(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/beolink_leader.py` & `mozart-api-2.5.3.123.1/mozart_api/models/beolink_leader.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class BeolinkLeader(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/beolink_listener.py` & `mozart-api-2.5.3.123.1/mozart_api/models/beolink_listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class BeolinkListener(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/beolink_peer.py` & `mozart-api-2.5.3.123.1/mozart_api/models/beolink_peer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class BeolinkPeer(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/bluetooth_device.py` & `mozart-api-2.5.3.123.1/mozart_api/models/bluetooth_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class BluetoothDevice(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/bluetooth_device_list.py` & `mozart-api-2.5.3.123.1/mozart_api/models/bluetooth_device_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.bluetooth_device import BluetoothDevice
 
 from mozart_api.configuration import Configuration
 
 
 class BluetoothDeviceList(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/button_event.py` & `mozart-api-2.5.3.123.1/mozart_api/models/button_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class ButtonEvent(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/compression.py` & `mozart-api-2.5.3.123.1/mozart_api/models/compression.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class Compression(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/compression_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/compression_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.compression import Compression
 
 from mozart_api.configuration import Configuration
 
 
 class CompressionFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/compression_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/compression_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.compression import Compression
 
 from mozart_api.configuration import Configuration
 
 
 class CompressionRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/content_item.py` & `mozart-api-2.5.3.123.1/mozart_api/models/content_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.source_type_enum import SourceTypeEnum
 
 from mozart_api.configuration import Configuration
 
 
 class ContentItem(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/directivity.py` & `mozart-api-2.5.3.123.1/mozart_api/models/directivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class Directivity(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/directivity_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/directivity_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.directivity import Directivity
 
 from mozart_api.configuration import Configuration
 
 
 class DirectivityFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/directivity_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/directivity_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.directivity import Directivity
 
 from mozart_api.configuration import Configuration
 
 
 class DirectivityRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/error_model.py` & `mozart-api-2.5.3.123.1/mozart_api/models/error_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class ErrorModel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/fader.py` & `mozart-api-2.5.3.123.1/mozart_api/models/fader.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class Fader(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/fader_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/fader_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.fader import Fader
 
 from mozart_api.configuration import Configuration
 
 
 class FaderFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/fader_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/fader_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.fader import Fader
 
 from mozart_api.configuration import Configuration
 
 
 class FaderRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/hdmi_input.py` & `mozart-api-2.5.3.123.1/mozart_api/models/hdmi_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class HdmiInput(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/hdmi_video_format.py` & `mozart-api-2.5.3.123.1/mozart_api/models/hdmi_video_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
-from mozart_api.models.video_timings import VideoTimings
 from mozart_api.models.video_pixel_format import VideoPixelFormat
+from mozart_api.models.video_timings import VideoTimings
 
 from mozart_api.configuration import Configuration
 
 
 class HdmiVideoFormat(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/home_control_uri.py` & `mozart-api-2.5.3.123.1/mozart_api/models/home_control_uri.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class HomeControlUri(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/install_record_id_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/install_record_id_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class InstallRecordIdState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/listening_mode.py` & `mozart-api-2.5.3.123.1/mozart_api/models/listening_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class ListeningMode(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/listening_mode_features.py` & `mozart-api-2.5.3.123.1/mozart_api/models/listening_mode_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
+from mozart_api.models.room_compensation import RoomCompensation
 from mozart_api.models.speech_enhance import SpeechEnhance
-from mozart_api.models.balance import Balance
 from mozart_api.models.fader import Fader
-from mozart_api.models.spatial_width import SpatialWidth
-from mozart_api.models.bass_management import BassManagement
-from mozart_api.models.room_compensation import RoomCompensation
-from mozart_api.models.tone_touch import ToneTouch
 from mozart_api.models.spatial_height import SpatialHeight
 from mozart_api.models.spatial_processing import SpatialProcessing
 from mozart_api.models.spatial_surround import SpatialSurround
+from mozart_api.models.balance import Balance
+from mozart_api.models.directivity import Directivity
 from mozart_api.models.compression import Compression
+from mozart_api.models.tone_touch import ToneTouch
 from mozart_api.models.spatial_envelopment import SpatialEnvelopment
-from mozart_api.models.directivity import Directivity
 from mozart_api.models.ambience import Ambience
+from mozart_api.models.spatial_width import SpatialWidth
+from mozart_api.models.bass_management import BassManagement
 
 from mozart_api.configuration import Configuration
 
 
 class ListeningModeFeatures(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/listening_mode_props.py` & `mozart-api-2.5.3.123.1/mozart_api/models/listening_mode_props.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.listening_mode_features import ListeningModeFeatures
 from mozart_api.models.listening_mode_trigger import ListeningModeTrigger
 
 from mozart_api.configuration import Configuration
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/listening_mode_ref.py` & `mozart-api-2.5.3.123.1/mozart_api/models/listening_mode_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class ListeningModeRef(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/listening_mode_trigger.py` & `mozart-api-2.5.3.123.1/mozart_api/models/listening_mode_trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class ListeningModeTrigger(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/loudness.py` & `mozart-api-2.5.3.123.1/mozart_api/models/loudness.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class Loudness(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/microphone_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/microphone_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class MicrophoneState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/microphones_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/microphones_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.microphone_state import MicrophoneState
 
 from mozart_api.configuration import Configuration
 
 
 class MicrophonesState(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/overlay_play_request.py` & `mozart-api-2.5.3.123.1/mozart_api/models/overlay_play_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
+from mozart_api.models.overlay_play_request_from_usb_from_usb import (
+    OverlayPlayRequestFromUsbFromUsb,
+)
 from mozart_api.models.uri import Uri
 from mozart_api.models.overlay_play_request_text_to_speech_text_to_speech import (
     OverlayPlayRequestTextToSpeechTextToSpeech,
 )
-from mozart_api.models.overlay_play_request_from_usb_from_usb import (
-    OverlayPlayRequestFromUsbFromUsb,
-)
 
 from mozart_api.configuration import Configuration
 
 
 class OverlayPlayRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/overlay_play_request_common.py` & `mozart-api-2.5.3.123.1/mozart_api/models/overlay_play_request_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class OverlayPlayRequestCommon(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/overlay_play_request_from_usb.py` & `mozart-api-2.5.3.123.1/mozart_api/models/overlay_play_request_from_usb.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.overlay_play_request_from_usb_from_usb import (
     OverlayPlayRequestFromUsbFromUsb,
 )
 
 from mozart_api.configuration import Configuration
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/overlay_play_request_from_usb_from_usb.py` & `mozart-api-2.5.3.123.1/mozart_api/models/overlay_play_request_from_usb_from_usb.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class OverlayPlayRequestFromUsbFromUsb(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/overlay_play_request_text_to_speech.py` & `mozart-api-2.5.3.123.1/mozart_api/models/overlay_play_request_text_to_speech.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.overlay_play_request_text_to_speech_text_to_speech import (
     OverlayPlayRequestTextToSpeechTextToSpeech,
 )
 
 from mozart_api.configuration import Configuration
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/overlay_play_request_text_to_speech_text_to_speech.py` & `mozart-api-2.5.3.123.1/mozart_api/models/overlay_play_request_text_to_speech_text_to_speech.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class OverlayPlayRequestTextToSpeechTextToSpeech(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/overlay_play_request_uri.py` & `mozart-api-2.5.3.123.1/mozart_api/models/overlay_play_request_uri.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.uri import Uri
 
 from mozart_api.configuration import Configuration
 
 
 class OverlayPlayRequestUri(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/paired_remote.py` & `mozart-api-2.5.3.123.1/mozart_api/models/paired_remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class PairedRemote(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/paired_remote_response.py` & `mozart-api-2.5.3.123.1/mozart_api/models/paired_remote_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.paired_remote import PairedRemote
 
 from mozart_api.configuration import Configuration
 
 
 class PairedRemoteResponse(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/play_queue_item.py` & `mozart-api-2.5.3.123.1/mozart_api/models/play_queue_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
-from mozart_api.models.play_queue_item_type import PlayQueueItemType
 from mozart_api.models.playback_content_metadata import PlaybackContentMetadata
+from mozart_api.models.play_queue_item_type import PlayQueueItemType
 
 from mozart_api.configuration import Configuration
 
 
 class PlayQueueItem(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/play_queue_item_type.py` & `mozart-api-2.5.3.123.1/mozart_api/models/play_queue_item_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class PlayQueueItemType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/play_queue_settings.py` & `mozart-api-2.5.3.123.1/mozart_api/models/play_queue_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class PlayQueueSettings(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/playback_content_metadata.py` & `mozart-api-2.5.3.123.1/mozart_api/models/playback_content_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
-from mozart_api.models.art import Art
 from mozart_api.models.beolink_leader import BeolinkLeader
+from mozart_api.models.art import Art
 
 from mozart_api.configuration import Configuration
 
 
 class PlaybackContentMetadata(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/playback_error.py` & `mozart-api-2.5.3.123.1/mozart_api/models/playback_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.playback_content_metadata import PlaybackContentMetadata
 
 from mozart_api.configuration import Configuration
 
 
 class PlaybackError(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/playback_progress.py` & `mozart-api-2.5.3.123.1/mozart_api/models/playback_progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class PlaybackProgress(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/playback_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/playback_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.playback_content_metadata import PlaybackContentMetadata
 from mozart_api.models.source import Source
-from mozart_api.models.playback_progress import PlaybackProgress
 from mozart_api.models.rendering_state import RenderingState
+from mozart_api.models.playback_progress import PlaybackProgress
 
 from mozart_api.configuration import Configuration
 
 
 class PlaybackState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/power_link_trigger.py` & `mozart-api-2.5.3.123.1/mozart_api/models/power_link_trigger.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class PowerLinkTrigger(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/power_state_enum.py` & `mozart-api-2.5.3.123.1/mozart_api/models/power_state_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class PowerStateEnum(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/preset.py` & `mozart-api-2.5.3.123.1/mozart_api/models/preset.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.content_item import ContentItem
 from mozart_api.models.source_type_enum import SourceTypeEnum
 from mozart_api.models.action import Action
 
 from mozart_api.configuration import Configuration
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/preset_all_of.py` & `mozart-api-2.5.3.123.1/mozart_api/models/preset_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.content_item import ContentItem
 from mozart_api.models.source_type_enum import SourceTypeEnum
 
 from mozart_api.configuration import Configuration
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/product_curtain_status.py` & `mozart-api-2.5.3.123.1/mozart_api/models/product_curtain_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class ProductCurtainStatus(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/product_friendly_name.py` & `mozart-api-2.5.3.123.1/mozart_api/models/product_friendly_name.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class ProductFriendlyName(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/product_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/product_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
+from mozart_api.models.microphones_state import MicrophonesState
+from mozart_api.models.power_state_enum import PowerStateEnum
 from mozart_api.models.tv_state import TvState
 from mozart_api.models.playback_state import PlaybackState
-from mozart_api.models.volume_state import VolumeState
-from mozart_api.models.software_update_state import SoftwareUpdateState
-from mozart_api.models.power_state_enum import PowerStateEnum
 from mozart_api.models.source import Source
-from mozart_api.models.microphones_state import MicrophonesState
+from mozart_api.models.software_update_state import SoftwareUpdateState
+from mozart_api.models.volume_state import VolumeState
 from mozart_api.models.sound_settings import SoundSettings
 
 from mozart_api.configuration import Configuration
 
 
 class ProductState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/remote_menu_item.py` & `mozart-api-2.5.3.123.1/mozart_api/models/remote_menu_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.content_item import ContentItem
 from mozart_api.models.action import Action
 
 from mozart_api.configuration import Configuration
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/remote_menu_item_all_of.py` & `mozart-api-2.5.3.123.1/mozart_api/models/remote_menu_item_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.content_item import ContentItem
 
 from mozart_api.configuration import Configuration
 
 
 class RemoteMenuItemAllOf(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/remote_menu_item_properties.py` & `mozart-api-2.5.3.123.1/mozart_api/models/remote_menu_item_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.action import Action
 
 from mozart_api.configuration import Configuration
 
 
 class RemoteMenuItemProperties(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/remote_menu_item_properties_all_of.py` & `mozart-api-2.5.3.123.1/mozart_api/models/remote_menu_item_properties_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RemoteMenuItemPropertiesAllOf(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/remote_ui_key_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/remote_ui_key_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RemoteUIKeyState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/rendering_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/rendering_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RenderingState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensation(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_current_measurement.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_current_measurement.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensationCurrentMeasurement(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_debug.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensationDebug(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_enabled.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_enabled.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensationEnabled(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_error_details.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_error_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.room_compensation_measurement_error import (
     RoomCompensationMeasurementError,
 )
 
 from mozart_api.configuration import Configuration
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensationFeature(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_info.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.room_compensation_version import RoomCompensationVersion
-from mozart_api.models.room_compensation_debug import RoomCompensationDebug
-from mozart_api.models.room_compensation_state import RoomCompensationState
 from mozart_api.models.room_compensation_result import RoomCompensationResult
 from mozart_api.models.room_compensation_type import RoomCompensationType
+from mozart_api.models.room_compensation_state import RoomCompensationState
 from mozart_api.models.room_compensation_enabled import RoomCompensationEnabled
+from mozart_api.models.room_compensation_debug import RoomCompensationDebug
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensationInfo(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_measurement_error.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_measurement_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensationMeasurementError(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_properties.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensationProperties(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_properties_all_of.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_properties_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensationPropertiesAllOf(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensationRange(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_response.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensationResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_result.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
-from mozart_api.models.speaker_group import SpeakerGroup
 from mozart_api.models.room_compensation_response import RoomCompensationResponse
+from mozart_api.models.speaker_group import SpeakerGroup
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensationResult(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.room_compensation_error_details import (
     RoomCompensationErrorDetails,
 )
 from mozart_api.models.room_compensation_properties import RoomCompensationProperties
 
 from mozart_api.configuration import Configuration
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_state_all_of.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_state_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.room_compensation_error_details import (
     RoomCompensationErrorDetails,
 )
 from mozart_api.models.room_compensation_properties import RoomCompensationProperties
 
 from mozart_api.configuration import Configuration
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_state_value.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_state_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensationStateValue(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_type.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensationType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/room_compensation_version.py` & `mozart-api-2.5.3.123.1/mozart_api/models/room_compensation_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class RoomCompensationVersion(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/scene.py` & `mozart-api-2.5.3.123.1/mozart_api/models/scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.action import Action
 
 from mozart_api.configuration import Configuration
 
 
 class Scene(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/scene_classification.py` & `mozart-api-2.5.3.123.1/mozart_api/models/scene_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SceneClassification(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/scene_match.py` & `mozart-api-2.5.3.123.1/mozart_api/models/scene_match.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SceneMatch(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/scene_properties.py` & `mozart-api-2.5.3.123.1/mozart_api/models/scene_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.action import Action
 
 from mozart_api.configuration import Configuration
 
 
 class SceneProperties(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/scene_trigger_base_properties.py` & `mozart-api-2.5.3.123.1/mozart_api/models/scene_trigger_base_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.action import Action
 
 from mozart_api.configuration import Configuration
 
 
 class SceneTriggerBaseProperties(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/software_update_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/software_update_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SoftwareUpdateState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/software_update_status.py` & `mozart-api-2.5.3.123.1/mozart_api/models/software_update_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.software_update_state import SoftwareUpdateState
 
 from mozart_api.configuration import Configuration
 
 
 class SoftwareUpdateStatus(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/sound_adjustments.py` & `mozart-api-2.5.3.123.1/mozart_api/models/sound_adjustments.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SoundAdjustments(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/sound_feature_set.py` & `mozart-api-2.5.3.123.1/mozart_api/models/sound_feature_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,33 +13,33 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
-from mozart_api.models.fader_feature import FaderFeature
-from mozart_api.models.spatial_surround_feature import SpatialSurroundFeature
+from mozart_api.models.spatial_envelopment_feature import SpatialEnvelopmentFeature
+from mozart_api.models.room_compensation_feature import RoomCompensationFeature
 from mozart_api.models.compression_feature import CompressionFeature
-from mozart_api.models.speech_enhance_feature import SpeechEnhanceFeature
+from mozart_api.models.spatial_height_feature import SpatialHeightFeature
+from mozart_api.models.spatial_width_feature import SpatialWidthFeature
+from mozart_api.models.spatial_processing_feature import SpatialProcessingFeature
 from mozart_api.models.treble_feature import TrebleFeature
+from mozart_api.models.tone_touch_y_feature import ToneTouchYFeature
 from mozart_api.models.balance_feature import BalanceFeature
+from mozart_api.models.spatial_surround_feature import SpatialSurroundFeature
+from mozart_api.models.directivity_feature import DirectivityFeature
 from mozart_api.models.bass_feature import BassFeature
-from mozart_api.models.tone_touch_y_feature import ToneTouchYFeature
-from mozart_api.models.spatial_processing_feature import SpatialProcessingFeature
-from mozart_api.models.bass_management_feature import BassManagementFeature
-from mozart_api.models.spatial_envelopment_feature import SpatialEnvelopmentFeature
-from mozart_api.models.spatial_height_feature import SpatialHeightFeature
-from mozart_api.models.room_compensation_feature import RoomCompensationFeature
-from mozart_api.models.spatial_width_feature import SpatialWidthFeature
+from mozart_api.models.fader_feature import FaderFeature
 from mozart_api.models.ambience_feature import AmbienceFeature
 from mozart_api.models.tone_touch_x_feature import ToneTouchXFeature
-from mozart_api.models.directivity_feature import DirectivityFeature
+from mozart_api.models.bass_management_feature import BassManagementFeature
+from mozart_api.models.speech_enhance_feature import SpeechEnhanceFeature
 
 from mozart_api.configuration import Configuration
 
 
 class SoundFeatureSet(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/sound_settings.py` & `mozart-api-2.5.3.123.1/mozart_api/models/sound_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.sound_adjustments import SoundAdjustments
-from mozart_api.models.sound_tone_touch import SoundToneTouch
 from mozart_api.models.room_compensation_info import RoomCompensationInfo
+from mozart_api.models.sound_tone_touch import SoundToneTouch
 
 from mozart_api.configuration import Configuration
 
 
 class SoundSettings(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/sound_tone_touch.py` & `mozart-api-2.5.3.123.1/mozart_api/models/sound_tone_touch.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SoundToneTouch(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/source.py` & `mozart-api-2.5.3.123.1/mozart_api/models/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.source_type_enum import SourceTypeEnum
 
 from mozart_api.configuration import Configuration
 
 
 class Source(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/source_array.py` & `mozart-api-2.5.3.123.1/mozart_api/models/source_array.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.source import Source
 
 from mozart_api.configuration import Configuration
 
 
 class SourceArray(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/source_type_enum.py` & `mozart-api-2.5.3.123.1/mozart_api/models/source_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SourceTypeEnum(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_envelopment.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_envelopment.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialEnvelopment(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_envelopment_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_envelopment_feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.spatial_envelopment import SpatialEnvelopment
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialEnvelopmentFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_envelopment_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_envelopment_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.spatial_envelopment import SpatialEnvelopment
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialEnvelopmentRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_height.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_height.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialHeight(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_height_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_height_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.spatial_height import SpatialHeight
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialHeightFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_height_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_height_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.spatial_height import SpatialHeight
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialHeightRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_processing.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialProcessing(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_processing_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_processing_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.spatial_processing import SpatialProcessing
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialProcessingFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_processing_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_processing_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.spatial_processing import SpatialProcessing
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialProcessingRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_surround.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_surround.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialSurround(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_surround_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_surround_feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.spatial_surround import SpatialSurround
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialSurroundFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_surround_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_surround_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.spatial_surround import SpatialSurround
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialSurroundRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_width.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_width.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialWidth(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_width_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_width_feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.spatial_width import SpatialWidth
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialWidthFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/spatial_width_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/spatial_width_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.spatial_width import SpatialWidth
 
 from mozart_api.configuration import Configuration
 
 
 class SpatialWidthRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/speaker_group.py` & `mozart-api-2.5.3.123.1/mozart_api/models/speaker_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.speaker_group_member import SpeakerGroupMember
 
 from mozart_api.configuration import Configuration
 
 
 class SpeakerGroup(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/speaker_group_member.py` & `mozart-api-2.5.3.123.1/mozart_api/models/speaker_group_member.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.speaker_group_member_location import SpeakerGroupMemberLocation
 
 from mozart_api.configuration import Configuration
 
 
 class SpeakerGroupMember(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/speaker_group_member_location.py` & `mozart-api-2.5.3.123.1/mozart_api/models/speaker_group_member_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SpeakerGroupMemberLocation(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/speaker_group_overview.py` & `mozart-api-2.5.3.123.1/mozart_api/models/speaker_group_overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SpeakerGroupOverview(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/speaker_role_enum.py` & `mozart-api-2.5.3.123.1/mozart_api/models/speaker_role_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SpeakerRoleEnum(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/speech_enhance.py` & `mozart-api-2.5.3.123.1/mozart_api/models/speech_enhance.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class SpeechEnhance(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/speech_enhance_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/speech_enhance_feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.speech_enhance import SpeechEnhance
 
 from mozart_api.configuration import Configuration
 
 
 class SpeechEnhanceFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/speech_enhance_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/speech_enhance_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.speech_enhance import SpeechEnhance
 
 from mozart_api.configuration import Configuration
 
 
 class SpeechEnhanceRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/stand_connected.py` & `mozart-api-2.5.3.123.1/mozart_api/models/stand_connected.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class StandConnected(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/stand_position.py` & `mozart-api-2.5.3.123.1/mozart_api/models/stand_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class StandPosition(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/tone_touch.py` & `mozart-api-2.5.3.123.1/mozart_api/models/tone_touch.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.tone_touch_type import ToneTouchType
 
 from mozart_api.configuration import Configuration
 
 
 class ToneTouch(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/tone_touch_type.py` & `mozart-api-2.5.3.123.1/mozart_api/models/tone_touch_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class ToneTouchType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/tone_touch_type_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/tone_touch_type_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.tone_touch_type import ToneTouchType
 
 from mozart_api.configuration import Configuration
 
 
 class ToneTouchTypeRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/tone_touch_x_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/tone_touch_x_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.tone_touch_type import ToneTouchType
 
 from mozart_api.configuration import Configuration
 
 
 class ToneTouchXFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/tone_touch_y_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/tone_touch_y_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.tone_touch_type import ToneTouchType
 
 from mozart_api.configuration import Configuration
 
 
 class ToneTouchYFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/treble.py` & `mozart-api-2.5.3.123.1/mozart_api/models/treble.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class Treble(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/treble_feature.py` & `mozart-api-2.5.3.123.1/mozart_api/models/treble_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.treble import Treble
 
 from mozart_api.configuration import Configuration
 
 
 class TrebleFeature(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/treble_range.py` & `mozart-api-2.5.3.123.1/mozart_api/models/treble_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.treble import Treble
 
 from mozart_api.configuration import Configuration
 
 
 class TrebleRange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/tv_info_event_data.py` & `mozart-api-2.5.3.123.1/mozart_api/models/tv_info_event_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.tv_integration_types import TvIntegrationTypes
 
 from mozart_api.configuration import Configuration
 
 
 class TvInfoEventData(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/tv_integration_types.py` & `mozart-api-2.5.3.123.1/mozart_api/models/tv_integration_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class TvIntegrationTypes(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/tv_properties.py` & `mozart-api-2.5.3.123.1/mozart_api/models/tv_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.tv_integration_types import TvIntegrationTypes
 
 from mozart_api.configuration import Configuration
 
 
 class TvProperties(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/tv_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/tv_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.tv_properties import TvProperties
 from mozart_api.models.tv_integration_types import TvIntegrationTypes
 
 from mozart_api.configuration import Configuration
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/uri.py` & `mozart-api-2.5.3.123.1/mozart_api/models/uri.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class Uri(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/user_flow.py` & `mozart-api-2.5.3.123.1/mozart_api/models/user_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class UserFlow(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/video_pixel_format.py` & `mozart-api-2.5.3.123.1/mozart_api/models/video_pixel_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class VideoPixelFormat(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/video_timings.py` & `mozart-api-2.5.3.123.1/mozart_api/models/video_timings.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class VideoTimings(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/volume_level.py` & `mozart-api-2.5.3.123.1/mozart_api/models/volume_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class VolumeLevel(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/volume_mute.py` & `mozart-api-2.5.3.123.1/mozart_api/models/volume_mute.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class VolumeMute(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/volume_settings.py` & `mozart-api-2.5.3.123.1/mozart_api/models/volume_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.volume_level import VolumeLevel
 
 from mozart_api.configuration import Configuration
 
 
 class VolumeSettings(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/volume_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/volume_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.volume_mute import VolumeMute
 from mozart_api.models.volume_level import VolumeLevel
 
 from mozart_api.configuration import Configuration
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_active_hdmi_input_signal.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_active_hdmi_input_signal.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.hdmi_input import HdmiInput
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventActiveHdmiInputSignal(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_active_listening_mode.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_active_listening_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.listening_mode_props import ListeningModeProps
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventActiveListeningMode(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_active_speaker_group.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_active_speaker_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.speaker_group_overview import SpeakerGroupOverview
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventActiveSpeakerGroup(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_alarm_timer.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_alarm_timer.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.alarm_timer_event_data import AlarmTimerEventData
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventAlarmTimer(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_alarm_triggered.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_alarm_triggered.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.alarm_triggered_info import AlarmTriggeredInfo
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventAlarmTriggered(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_battery.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_battery.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.battery_state import BatteryState
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventBattery(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_beo_remote_button.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_beo_remote_button.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.beo_remote_button import BeoRemoteButton
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventBeoRemoteButton(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_beolink_experiences_result.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_beolink_experiences_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.beolink_experiences_result import BeolinkExperiencesResult
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventBeolinkExperiencesResult(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_beolink_join_result.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_beolink_join_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.beolink_join_result import BeolinkJoinResult
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventBeolinkJoinResult(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_button.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_button.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.button_event import ButtonEvent
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventButton(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_curtains.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_curtains.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.product_curtain_status import ProductCurtainStatus
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventCurtains(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_hdmi_video_format_signal.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_hdmi_video_format_signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.hdmi_video_format import HdmiVideoFormat
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventHdmiVideoFormatSignal(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_notification.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.websocket_notification_tag import WebsocketNotificationTag
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventNotification(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_playback_error.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_playback_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.playback_error import PlaybackError
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventPlaybackError(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_playback_metadata.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_playback_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.playback_content_metadata import PlaybackContentMetadata
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventPlaybackMetadata(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_playback_progress.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_playback_progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.playback_progress import PlaybackProgress
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventPlaybackProgress(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_playback_source.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_playback_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.source import Source
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventPlaybackSource(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_playback_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_playback_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.rendering_state import RenderingState
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventPlaybackState(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_power_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_power_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.power_state_enum import PowerStateEnum
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventPowerState(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_puc_install_remote_id_status.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_puc_install_remote_id_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.install_record_id_state import InstallRecordIdState
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventPucInstallRemoteIdStatus(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_role.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.speaker_role_enum import SpeakerRoleEnum
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventRole(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_room_compensation_current_measurement_event.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_room_compensation_current_measurement_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.room_compensation_current_measurement import (
     RoomCompensationCurrentMeasurement,
 )
 
 from mozart_api.configuration import Configuration
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_room_compensation_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_room_compensation_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.room_compensation_state_value import RoomCompensationStateValue
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventRoomCompensationState(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_software_update_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_software_update_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.software_update_state import SoftwareUpdateState
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventSoftwareUpdateState(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_sound_settings.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_sound_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.sound_settings import SoundSettings
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventSoundSettings(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_source_change.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_source_change.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.source import Source
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventSourceChange(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_speaker_group_changed.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_speaker_group_changed.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventSpeakerGroupChanged(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_stand_connected.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_stand_connected.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.stand_connected import StandConnected
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventStandConnected(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_stand_position.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_stand_position.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.stand_position import StandPosition
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventStandPosition(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_tv_info.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_tv_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.tv_info_event_data import TvInfoEventData
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventTvInfo(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_volume.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.volume_state import VolumeState
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventVolume(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/web_socket_event_wisa_out_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/web_socket_event_wisa_out_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 from mozart_api.models.wisa_out_state import WisaOutState
 
 from mozart_api.configuration import Configuration
 
 
 class WebSocketEventWisaOutState(object):
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/websocket_notification_tag.py` & `mozart-api-2.5.3.123.1/mozart_api/models/websocket_notification_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class WebsocketNotificationTag(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/models/wisa_out_state.py` & `mozart-api-2.5.3.123.1/mozart_api/models/wisa_out_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from datetime import datetime
-from typing import List, Literal, Optional
+from typing import List, Dict, Literal, Optional
 
 
 from mozart_api.configuration import Configuration
 
 
 class WisaOutState(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/mozart_cli.py` & `mozart-api-2.5.3.123.1/mozart_api/mozart_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 ]
 
 
 @dataclass
 class MozartDevice:
     """Dataclass for describing Zeroconf discovered Mozart devices."""
 
-    friendly_name: str = ""
+    friendly_name: str | None = ""
     model_name: str = ""
     serial_number: str = ""
     ip_address: str = ""
     sw_version: str = ""
 
 
 mozart_devices: list[MozartDevice] = []
@@ -68,22 +68,24 @@
         # Unused
         pass
 
     def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:
         info = zc.get_service_info(type_, name)
 
         # Create MozartDevice object from MDNS discovered information.
-        try:
-            ip_address = info.parsed_addresses()[0]
-            serial_number = info.properties.get(b"sn").decode("utf-8")
-            model_name = info.server[:-16].replace("-", " ")
-            sw_version = info.properties.get(b"fv").decode("utf-8")
-            friendly_name = info.properties.get(b"fn").decode("utf-8")
-        except AttributeError:
-            pass
+        ip_address = info.parsed_addresses()[0]
+        serial_number = info.properties.get(b"sn").decode("utf-8")
+        model_name = info.server[:-16].replace("-", " ")
+        sw_version = info.properties.get(b"fv").decode("utf-8")
+
+        friendly_name = info.properties.get(b"fn")
+
+        # MDNS devices other than Mozart devices may not have friendly names
+        if friendly_name is not None:
+            friendly_name = friendly_name.decode("utf-8")
 
         mozart_device = MozartDevice(
             friendly_name, model_name, serial_number, ip_address, sw_version
         )
 
         mozart_devices.append(mozart_device)
 
@@ -102,15 +104,15 @@
     event = threading.Event()
 
     zeroconf = Zeroconf()
     listener = MozartListener(mode, verbose, event)
     browser = ServiceBrowser(zeroconf, MOZART_MDNS_TYPE, listener)
 
     if mode == "discover" or verbose:
-        print("Discovering Mozart devices.")
+        print("Discovering Mozart devices. Scanning _bangolufsen._tcp.local.")
 
     if timeout == -1:
         input("Press any key to stop discovery.\n\r")
 
     else:
         # Stop if the serial number has been found with MDNS
         timeout_status = event.wait(timeout)
@@ -313,15 +315,14 @@
             )
 
         elif self.command == "join":
             status = asyncio.run(self._beolink_join())
 
         # Currently show battery state, product state
         elif self.command == "info":
-
             battery_state = self.mozart_client.get_battery_state()
             print(f"Battery state: {battery_state}")
 
             power_state = self.mozart_client.get_product_state()
             print(f"Product state: {power_state}")
 
         elif self.command == "allstandby":
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api/mozart_client.py` & `mozart-api-2.5.3.123.1/mozart_api/mozart_client.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api/rest.py` & `mozart-api-2.5.3.123.1/mozart_api/rest.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/mozart_api.egg-info/PKG-INFO` & `mozart-api-2.5.3.123.1/mozart_api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: mozart-api
-Version: 2.5.3.123.0
+Version: 2.5.3.123.1
 Summary: Mozart platform API
 Home-page: https://pypi.org/project/mozart-api/
 Author: BangOlufsen
 Author-email: support@bang-olufsen.dk
 License: MIT
 Project-URL: Github, https://github.com/bang-olufsen/mozart-open-api
 Project-URL: Documentation, https://bang-olufsen.github.io/mozart-open-api/
 Project-URL: Bug tracker, https://github.com/bang-olufsen/mozart-open-api/issues
 Keywords: OpenAPI,OpenAPI-Generator,Mozart platform API
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Multimedia
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Mozart platform API
 
 [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/bang-olufsen/mozart-open-api/blob/main/LICENSE)
 [![Version](https://img.shields.io/pypi/v/mozart-api?color=g)](https://pypi.org/project/mozart-api)
@@ -30,13 +30,16 @@
 [![Balance stereo](https://raw.githubusercontent.com/bang-olufsen/mozart-open-api/main/docs/media/balance_stereo.png)](https://www.bang-olufsen.com/en/dk/speakers/beosound-balance-stereo-set?variant=beosound-balance-gva-naturaloak-bundle)
 
 The Mozart API is a REST API with async capabilities and WebSocket notification channel for immediate state information. Currently the API is distributed as a Python package and as an OpenAPI document that can be found in the [Github releases](https://github.com/bang-olufsen/mozart-open-api/releases).
 
 Supported by:
 
 - [Beolab 28](https://www.bang-olufsen.com/en/dk/speakers/beolab-28)
+- [Beosound 2 3rd gen](https://www.bang-olufsen.com/en/dk/speakers/beosound-2)
+- [Beosound A5](https://www.bang-olufsen.com/en/dk/speakers/beosound-a5)
+- [Beosound A9 5th gen](https://www.bang-olufsen.com/en/dk/speakers/beosound-a9)
 - [Beosound Balance](https://www.bang-olufsen.com/en/dk/speakers/beosound-balance)
 - [Beosound Emerge](https://www.bang-olufsen.com/en/dk/speakers/beosound-emerge)
 - [Beosound Level](https://www.bang-olufsen.com/en/dk/speakers/beosound-level)
 - [Beosound Theatre](https://www.bang-olufsen.com/en/dk/soundbars/beosound-theatre)
 
 API documentation can be found on the [Github page](https://bang-olufsen.github.io/mozart-open-api).
```

### Comparing `mozart-api-2.5.3.123.0/mozart_api.egg-info/SOURCES.txt` & `mozart-api-2.5.3.123.1/mozart_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/setup.py` & `mozart-api-2.5.3.123.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "mozart-api"
-VERSION = "2.5.3.123.0"
+VERSION = "2.5.3.123.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -54,14 +54,17 @@
 [![Balance stereo](https://raw.githubusercontent.com/bang-olufsen/mozart-open-api/main/docs/media/balance_stereo.png)](https://www.bang-olufsen.com/en/dk/speakers/beosound-balance-stereo-set?variant=beosound-balance-gva-naturaloak-bundle)
 
 The Mozart API is a REST API with async capabilities and WebSocket notification channel for immediate state information. Currently the API is distributed as a Python package and as an OpenAPI document that can be found in the [Github releases](https://github.com/bang-olufsen/mozart-open-api/releases).
 
 Supported by:
 
 - [Beolab 28](https://www.bang-olufsen.com/en/dk/speakers/beolab-28)
+- [Beosound 2 3rd gen](https://www.bang-olufsen.com/en/dk/speakers/beosound-2)
+- [Beosound A5](https://www.bang-olufsen.com/en/dk/speakers/beosound-a5)
+- [Beosound A9 5th gen](https://www.bang-olufsen.com/en/dk/speakers/beosound-a9)
 - [Beosound Balance](https://www.bang-olufsen.com/en/dk/speakers/beosound-balance)
 - [Beosound Emerge](https://www.bang-olufsen.com/en/dk/speakers/beosound-emerge)
 - [Beosound Level](https://www.bang-olufsen.com/en/dk/speakers/beosound-level)
 - [Beosound Theatre](https://www.bang-olufsen.com/en/dk/soundbars/beosound-theatre)
 
 API documentation can be found on the [Github page](https://bang-olufsen.github.io/mozart-open-api).
 """,
@@ -70,17 +73,17 @@
         "console_scripts": ["mozart_api = mozart_api.mozart_cli:MozartApiCli"]
     },
     project_urls={
         "Github": "https://github.com/bang-olufsen/mozart-open-api",
         "Documentation": "https://bang-olufsen.github.io/mozart-open-api/",
         "Bug tracker": "https://github.com/bang-olufsen/mozart-open-api/issues",
     },
-    python_requires=">=3.8",
+    python_requires=">=3.10",
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Multimedia",
         "Intended Audience :: Developers",
     ],
 )
```

### Comparing `mozart-api-2.5.3.123.0/test/test_action.py` & `mozart-api-2.5.3.123.1/test/test_action.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_alarm_timer_event_data.py` & `mozart-api-2.5.3.123.1/test/test_alarm_timer_event_data.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_alarm_triggered_info.py` & `mozart-api-2.5.3.123.1/test/test_alarm_triggered_info.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_ambience.py` & `mozart-api-2.5.3.123.1/test/test_ambience.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_ambience_feature.py` & `mozart-api-2.5.3.123.1/test/test_ambience_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_ambience_range.py` & `mozart-api-2.5.3.123.1/test/test_ambience_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_art.py` & `mozart-api-2.5.3.123.1/test/test_art.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_balance.py` & `mozart-api-2.5.3.123.1/test/test_balance.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_balance_feature.py` & `mozart-api-2.5.3.123.1/test/test_balance_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_balance_range.py` & `mozart-api-2.5.3.123.1/test/test_balance_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_bass.py` & `mozart-api-2.5.3.123.1/test/test_bass.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_bass_feature.py` & `mozart-api-2.5.3.123.1/test/test_bass_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_bass_management.py` & `mozart-api-2.5.3.123.1/test/test_bass_management.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_bass_management_feature.py` & `mozart-api-2.5.3.123.1/test/test_bass_management_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_bass_management_range.py` & `mozart-api-2.5.3.123.1/test/test_bass_management_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_bass_range.py` & `mozart-api-2.5.3.123.1/test/test_bass_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_battery_state.py` & `mozart-api-2.5.3.123.1/test/test_battery_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_beo_remote_button.py` & `mozart-api-2.5.3.123.1/test/test_beo_remote_button.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_beolink_api.py` & `mozart-api-2.5.3.123.1/test/test_beolink_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_beolink_available_listener.py` & `mozart-api-2.5.3.123.1/test/test_beolink_available_listener.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_beolink_experience.py` & `mozart-api-2.5.3.123.1/test/test_beolink_experience.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_beolink_experiences_request.py` & `mozart-api-2.5.3.123.1/test/test_beolink_experiences_request.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_beolink_experiences_result.py` & `mozart-api-2.5.3.123.1/test/test_beolink_experiences_result.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_beolink_join_request.py` & `mozart-api-2.5.3.123.1/test/test_beolink_join_request.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_beolink_join_result.py` & `mozart-api-2.5.3.123.1/test/test_beolink_join_result.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_beolink_leader.py` & `mozart-api-2.5.3.123.1/test/test_beolink_leader.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_beolink_listener.py` & `mozart-api-2.5.3.123.1/test/test_beolink_listener.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_beolink_peer.py` & `mozart-api-2.5.3.123.1/test/test_beolink_peer.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_bluetooth_api.py` & `mozart-api-2.5.3.123.1/test/test_bluetooth_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_bluetooth_device.py` & `mozart-api-2.5.3.123.1/test/test_bluetooth_device.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_bluetooth_device_list.py` & `mozart-api-2.5.3.123.1/test/test_bluetooth_device_list.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_button_event.py` & `mozart-api-2.5.3.123.1/test/test_button_event.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_compression.py` & `mozart-api-2.5.3.123.1/test/test_compression.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_compression_feature.py` & `mozart-api-2.5.3.123.1/test/test_compression_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_compression_range.py` & `mozart-api-2.5.3.123.1/test/test_compression_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_content_api.py` & `mozart-api-2.5.3.123.1/test/test_content_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_content_item.py` & `mozart-api-2.5.3.123.1/test/test_content_item.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_deezer_api.py` & `mozart-api-2.5.3.123.1/test/test_deezer_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_directivity.py` & `mozart-api-2.5.3.123.1/test/test_directivity.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_directivity_feature.py` & `mozart-api-2.5.3.123.1/test/test_directivity_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_directivity_range.py` & `mozart-api-2.5.3.123.1/test/test_directivity_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_error_model.py` & `mozart-api-2.5.3.123.1/test/test_error_model.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_fader.py` & `mozart-api-2.5.3.123.1/test/test_fader.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_fader_feature.py` & `mozart-api-2.5.3.123.1/test/test_fader_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_fader_range.py` & `mozart-api-2.5.3.123.1/test/test_fader_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_hdmi_input.py` & `mozart-api-2.5.3.123.1/test/test_hdmi_input.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_hdmi_video_format.py` & `mozart-api-2.5.3.123.1/test/test_hdmi_video_format.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_home_control_uri.py` & `mozart-api-2.5.3.123.1/test/test_home_control_uri.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_install_record_id_state.py` & `mozart-api-2.5.3.123.1/test/test_install_record_id_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_listening_mode.py` & `mozart-api-2.5.3.123.1/test/test_listening_mode.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_listening_mode_features.py` & `mozart-api-2.5.3.123.1/test/test_listening_mode_features.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_listening_mode_props.py` & `mozart-api-2.5.3.123.1/test/test_listening_mode_props.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_listening_mode_ref.py` & `mozart-api-2.5.3.123.1/test/test_listening_mode_ref.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_listening_mode_trigger.py` & `mozart-api-2.5.3.123.1/test/test_listening_mode_trigger.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_loudness.py` & `mozart-api-2.5.3.123.1/test/test_loudness.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_microphone_state.py` & `mozart-api-2.5.3.123.1/test/test_microphone_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_microphones_state.py` & `mozart-api-2.5.3.123.1/test/test_microphones_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_mozart_api.py` & `mozart-api-2.5.3.123.1/test/test_mozart_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_overlay_api.py` & `mozart-api-2.5.3.123.1/test/test_overlay_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_overlay_play_request.py` & `mozart-api-2.5.3.123.1/test/test_overlay_play_request.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_overlay_play_request_common.py` & `mozart-api-2.5.3.123.1/test/test_overlay_play_request_common.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_overlay_play_request_from_usb.py` & `mozart-api-2.5.3.123.1/test/test_overlay_play_request_from_usb.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_overlay_play_request_from_usb_from_usb.py` & `mozart-api-2.5.3.123.1/test/test_overlay_play_request_from_usb_from_usb.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_overlay_play_request_text_to_speech.py` & `mozart-api-2.5.3.123.1/test/test_overlay_play_request_text_to_speech.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_overlay_play_request_text_to_speech_text_to_speech.py` & `mozart-api-2.5.3.123.1/test/test_overlay_play_request_text_to_speech_text_to_speech.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_overlay_play_request_uri.py` & `mozart-api-2.5.3.123.1/test/test_overlay_play_request_uri.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_paired_remote.py` & `mozart-api-2.5.3.123.1/test/test_paired_remote.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_paired_remote_response.py` & `mozart-api-2.5.3.123.1/test/test_paired_remote_response.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_play_queue_item.py` & `mozart-api-2.5.3.123.1/test/test_play_queue_item.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_play_queue_item_type.py` & `mozart-api-2.5.3.123.1/test/test_play_queue_item_type.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_play_queue_settings.py` & `mozart-api-2.5.3.123.1/test/test_play_queue_settings.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_playback_api.py` & `mozart-api-2.5.3.123.1/test/test_playback_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_playback_content_metadata.py` & `mozart-api-2.5.3.123.1/test/test_playback_content_metadata.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_playback_error.py` & `mozart-api-2.5.3.123.1/test/test_playback_error.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_playback_progress.py` & `mozart-api-2.5.3.123.1/test/test_playback_progress.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_playback_state.py` & `mozart-api-2.5.3.123.1/test/test_playback_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_power_api.py` & `mozart-api-2.5.3.123.1/test/test_power_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_power_link_trigger.py` & `mozart-api-2.5.3.123.1/test/test_power_link_trigger.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_power_state_enum.py` & `mozart-api-2.5.3.123.1/test/test_power_state_enum.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_preset.py` & `mozart-api-2.5.3.123.1/test/test_preset.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_preset_all_of.py` & `mozart-api-2.5.3.123.1/test/test_preset_all_of.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_product_api.py` & `mozart-api-2.5.3.123.1/test/test_product_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_product_curtain_status.py` & `mozart-api-2.5.3.123.1/test/test_product_curtain_status.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_product_friendly_name.py` & `mozart-api-2.5.3.123.1/test/test_product_friendly_name.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_product_state.py` & `mozart-api-2.5.3.123.1/test/test_product_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_remote_api.py` & `mozart-api-2.5.3.123.1/test/test_remote_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_remote_menu_item.py` & `mozart-api-2.5.3.123.1/test/test_remote_menu_item.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_remote_menu_item_all_of.py` & `mozart-api-2.5.3.123.1/test/test_remote_menu_item_all_of.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_remote_menu_item_properties.py` & `mozart-api-2.5.3.123.1/test/test_remote_menu_item_properties.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_remote_menu_item_properties_all_of.py` & `mozart-api-2.5.3.123.1/test/test_remote_menu_item_properties_all_of.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_remote_ui_key_state.py` & `mozart-api-2.5.3.123.1/test/test_remote_ui_key_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_rendering_state.py` & `mozart-api-2.5.3.123.1/test/test_rendering_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_current_measurement.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_current_measurement.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_debug.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_debug.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_enabled.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_enabled.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_error_details.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_error_details.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_feature.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_info.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_info.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_measurement_error.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_measurement_error.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_properties.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_properties.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_properties_all_of.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_properties_all_of.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_range.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_response.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_response.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_result.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_result.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_state.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_state_all_of.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_state_all_of.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_state_value.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_state_value.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_type.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_type.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_room_compensation_version.py` & `mozart-api-2.5.3.123.1/test/test_room_compensation_version.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_scene.py` & `mozart-api-2.5.3.123.1/test/test_scene.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_scene_classification.py` & `mozart-api-2.5.3.123.1/test/test_scene_classification.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_scene_match.py` & `mozart-api-2.5.3.123.1/test/test_scene_match.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_scene_properties.py` & `mozart-api-2.5.3.123.1/test/test_scene_properties.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_scene_trigger_base_properties.py` & `mozart-api-2.5.3.123.1/test/test_scene_trigger_base_properties.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_scenes_api.py` & `mozart-api-2.5.3.123.1/test/test_scenes_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_settings_api.py` & `mozart-api-2.5.3.123.1/test/test_settings_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_software_update_api.py` & `mozart-api-2.5.3.123.1/test/test_software_update_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_software_update_state.py` & `mozart-api-2.5.3.123.1/test/test_software_update_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_software_update_status.py` & `mozart-api-2.5.3.123.1/test/test_software_update_status.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_sound_adjustments.py` & `mozart-api-2.5.3.123.1/test/test_sound_adjustments.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_sound_api.py` & `mozart-api-2.5.3.123.1/test/test_sound_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_sound_feature_set.py` & `mozart-api-2.5.3.123.1/test/test_sound_feature_set.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_sound_settings.py` & `mozart-api-2.5.3.123.1/test/test_sound_settings.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_sound_tone_touch.py` & `mozart-api-2.5.3.123.1/test/test_sound_tone_touch.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_source.py` & `mozart-api-2.5.3.123.1/test/test_source.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_source_array.py` & `mozart-api-2.5.3.123.1/test/test_source_array.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_source_type_enum.py` & `mozart-api-2.5.3.123.1/test/test_source_type_enum.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_envelopment.py` & `mozart-api-2.5.3.123.1/test/test_spatial_envelopment.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_envelopment_feature.py` & `mozart-api-2.5.3.123.1/test/test_spatial_envelopment_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_envelopment_range.py` & `mozart-api-2.5.3.123.1/test/test_spatial_envelopment_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_height.py` & `mozart-api-2.5.3.123.1/test/test_spatial_height.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_height_feature.py` & `mozart-api-2.5.3.123.1/test/test_spatial_height_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_height_range.py` & `mozart-api-2.5.3.123.1/test/test_spatial_height_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_processing.py` & `mozart-api-2.5.3.123.1/test/test_spatial_processing.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_processing_feature.py` & `mozart-api-2.5.3.123.1/test/test_spatial_processing_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_processing_range.py` & `mozart-api-2.5.3.123.1/test/test_spatial_processing_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_surround.py` & `mozart-api-2.5.3.123.1/test/test_spatial_surround.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_surround_feature.py` & `mozart-api-2.5.3.123.1/test/test_spatial_surround_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_surround_range.py` & `mozart-api-2.5.3.123.1/test/test_spatial_surround_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_width.py` & `mozart-api-2.5.3.123.1/test/test_spatial_width.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_width_feature.py` & `mozart-api-2.5.3.123.1/test/test_spatial_width_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_spatial_width_range.py` & `mozart-api-2.5.3.123.1/test/test_spatial_width_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_speaker_group.py` & `mozart-api-2.5.3.123.1/test/test_speaker_group.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_speaker_group_api.py` & `mozart-api-2.5.3.123.1/test/test_speaker_group_api.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_speaker_group_member.py` & `mozart-api-2.5.3.123.1/test/test_speaker_group_member.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_speaker_group_member_location.py` & `mozart-api-2.5.3.123.1/test/test_speaker_group_member_location.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_speaker_group_overview.py` & `mozart-api-2.5.3.123.1/test/test_speaker_group_overview.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_speaker_role_enum.py` & `mozart-api-2.5.3.123.1/test/test_speaker_role_enum.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_speech_enhance.py` & `mozart-api-2.5.3.123.1/test/test_speech_enhance.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_speech_enhance_feature.py` & `mozart-api-2.5.3.123.1/test/test_speech_enhance_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_speech_enhance_range.py` & `mozart-api-2.5.3.123.1/test/test_speech_enhance_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_stand_connected.py` & `mozart-api-2.5.3.123.1/test/test_stand_connected.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_stand_position.py` & `mozart-api-2.5.3.123.1/test/test_stand_position.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_tone_touch.py` & `mozart-api-2.5.3.123.1/test/test_tone_touch.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_tone_touch_type.py` & `mozart-api-2.5.3.123.1/test/test_tone_touch_type.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_tone_touch_type_range.py` & `mozart-api-2.5.3.123.1/test/test_tone_touch_type_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_tone_touch_x_feature.py` & `mozart-api-2.5.3.123.1/test/test_tone_touch_x_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_tone_touch_y_feature.py` & `mozart-api-2.5.3.123.1/test/test_tone_touch_y_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_treble.py` & `mozart-api-2.5.3.123.1/test/test_treble.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_treble_feature.py` & `mozart-api-2.5.3.123.1/test/test_treble_feature.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_treble_range.py` & `mozart-api-2.5.3.123.1/test/test_treble_range.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_tv_info_event_data.py` & `mozart-api-2.5.3.123.1/test/test_tv_info_event_data.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_tv_integration_types.py` & `mozart-api-2.5.3.123.1/test/test_tv_integration_types.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_tv_properties.py` & `mozart-api-2.5.3.123.1/test/test_tv_properties.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_tv_state.py` & `mozart-api-2.5.3.123.1/test/test_tv_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_uri.py` & `mozart-api-2.5.3.123.1/test/test_uri.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_user_flow.py` & `mozart-api-2.5.3.123.1/test/test_user_flow.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_video_pixel_format.py` & `mozart-api-2.5.3.123.1/test/test_video_pixel_format.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_video_timings.py` & `mozart-api-2.5.3.123.1/test/test_video_timings.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_volume_level.py` & `mozart-api-2.5.3.123.1/test/test_volume_level.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_volume_mute.py` & `mozart-api-2.5.3.123.1/test/test_volume_mute.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_volume_settings.py` & `mozart-api-2.5.3.123.1/test/test_volume_settings.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_volume_state.py` & `mozart-api-2.5.3.123.1/test/test_volume_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_active_hdmi_input_signal.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_active_hdmi_input_signal.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_active_listening_mode.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_active_listening_mode.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_active_speaker_group.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_active_speaker_group.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_alarm_timer.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_alarm_timer.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_alarm_triggered.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_alarm_triggered.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_battery.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_battery.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_beo_remote_button.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_beo_remote_button.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_beolink_experiences_result.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_beolink_experiences_result.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_beolink_join_result.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_beolink_join_result.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_button.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_button.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_curtains.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_curtains.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_hdmi_video_format_signal.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_hdmi_video_format_signal.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_notification.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_notification.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_playback_error.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_playback_error.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_playback_metadata.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_playback_metadata.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_playback_progress.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_playback_progress.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_playback_source.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_playback_source.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_playback_state.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_playback_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_power_state.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_power_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_puc_install_remote_id_status.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_puc_install_remote_id_status.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_role.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_role.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_room_compensation_current_measurement_event.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_room_compensation_current_measurement_event.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_room_compensation_state.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_room_compensation_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_software_update_state.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_software_update_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_sound_settings.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_sound_settings.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_source_change.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_source_change.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_speaker_group_changed.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_speaker_group_changed.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_stand_connected.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_stand_connected.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_stand_position.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_stand_position.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_tv_info.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_tv_info.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_volume.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_volume.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_web_socket_event_wisa_out_state.py` & `mozart-api-2.5.3.123.1/test/test_web_socket_event_wisa_out_state.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_websocket_notification_tag.py` & `mozart-api-2.5.3.123.1/test/test_websocket_notification_tag.py`

 * *Files identical despite different names*

### Comparing `mozart-api-2.5.3.123.0/test/test_wisa_out_state.py` & `mozart-api-2.5.3.123.1/test/test_wisa_out_state.py`

 * *Files identical despite different names*

