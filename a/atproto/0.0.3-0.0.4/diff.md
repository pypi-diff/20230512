# Comparing `tmp/atproto-0.0.3.tar.gz` & `tmp/atproto-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atproto-0.0.3.tar", max compression
+gzip compressed data, was "atproto-0.0.4.tar", max compression
```

## Comparing `atproto-0.0.3.tar` & `atproto-0.0.4.tar`

### file list

```diff
@@ -1,152 +1,152 @@
--rw-r--r--   0        0        0     1061 2023-05-08 19:05:45.792914 atproto-0.0.3/LICENSE
--rw-r--r--   0        0        0     9776 2023-05-08 19:05:45.792914 atproto-0.0.3/README.md
--rw-r--r--   0        0        0      300 2023-05-08 19:05:45.792914 atproto-0.0.3/atproto/__init__.py
--rw-r--r--   0        0        0      619 2023-05-08 19:05:45.792914 atproto-0.0.3/atproto/cid/__init__.py
--rw-r--r--   0        0        0       23 2023-05-08 19:05:45.792914 atproto-0.0.3/atproto/cli/__init__.py
--rw-r--r--   0        0        0     2767 2023-05-08 19:05:45.792914 atproto-0.0.3/atproto/codegen/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/clients/__init__.py
--rw-r--r--   0        0        0     1156 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/clients/generate_async_client.py
--rw-r--r--   0        0        0        0 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/models/__init__.py
--rw-r--r--   0        0        0     2317 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/models/builder.py
--rw-r--r--   0        0        0    18794 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/models/generator.py
--rw-r--r--   0        0        0        0 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/namespaces/__init__.py
--rw-r--r--   0        0        0     2562 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/namespaces/builder.py
--rw-r--r--   0        0        0    11855 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/codegen/namespaces/generator.py
--rw-r--r--   0        0        0      944 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/lexicon/__init__.py
--rw-r--r--   0        0        0     4658 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/lexicon/models.py
--rw-r--r--   0        0        0     3871 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/lexicon/parser.py
--rw-r--r--   0        0        0     5298 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/nsid/__init__.py
--rw-r--r--   0        0        0     3075 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/uri/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/client/__init__.py
--rw-r--r--   0        0        0     5994 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/client/async_client.py
--rw-r--r--   0        0        0      489 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/client/async_raw.py
--rw-r--r--   0        0        0     3719 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/client/base.py
--rw-r--r--   0        0        0     5555 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/client/client.py
--rw-r--r--   0        0        0      469 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/client/raw.py
--rw-r--r--   0        0        0    10098 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/__init__.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/__init__.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/__init__.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0     3057 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      836 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      890 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0     1014 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      927 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/profile.py
--rw-r--r--   0        0        0     1061 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      970 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0     1619 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/external.py
--rw-r--r--   0        0        0     1417 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/images.py
--rw-r--r--   0        0        0     2248 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/record.py
--rw-r--r--   0        0        0     1192 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0     3913 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/defs.py
--rw-r--r--   0        0        0     1041 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0     1449 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0     1076 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0      855 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
--rw-r--r--   0        0        0     1181 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0     1066 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      734 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/like.py
--rw-r--r--   0        0        0     2298 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/post.py
--rw-r--r--   0        0        0      738 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/repost.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      665 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/block.py
--rw-r--r--   0        0        0      667 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/follow.py
--rw-r--r--   0        0        0     1004 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
--rw-r--r--   0        0        0     1133 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0     1123 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0      999 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0      574 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0      576 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      830 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0     1859 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0      586 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0     1580 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0     1082 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0      553 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/base.py
--rw-r--r--   0        0        0      713 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/blob_ref.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/__init__.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/__init__.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0     9028 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/defs.py
--rw-r--r--   0        0        0      712 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0     1071 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      839 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0     1097 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      839 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0     1161 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      890 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      824 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0      953 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0      911 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0     1129 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0     1370 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0      651 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0      621 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      887 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0      586 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/label/__init__.py
--rw-r--r--   0        0        0     1191 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/label/defs.py
--rw-r--r--   0        0        0     1323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0      957 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0     1499 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0      825 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0     1972 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0     1236 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0      969 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0     1038 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0     1171 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0     1761 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0     1319 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0      644 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0      742 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_account.py
--rw-r--r--   0        0        0      983 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0      880 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0     1282 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0     1117 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_session.py
--rw-r--r--   0        0        0     1183 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/defs.py
--rw-r--r--   0        0        0      659 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0     1211 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0     1028 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      704 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/get_session.py
--rw-r--r--   0        0        0      956 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0      729 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0      589 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0      628 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0      583 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0      323 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      752 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      744 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      822 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0      986 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      764 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      872 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      916 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0      969 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0     1201 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      637 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      640 2023-05-08 19:05:45.796914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0     2426 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0      425 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/models/type_conversion.py
--rw-r--r--   0        0        0     3175 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/models/utils.py
--rw-r--r--   0        0        0        0 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/namespaces/__init__.py
--rw-r--r--   0        0        0    65433 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/namespaces/async_ns.py
--rw-r--r--   0        0        0      361 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/namespaces/base.py
--rw-r--r--   0        0        0    64495 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/namespaces/sync_ns.py
--rw-r--r--   0        0        0     4353 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_client/request.py
--rw-r--r--   0        0        0       43 2023-05-08 19:05:45.800914 atproto-0.0.3/atproto/xrpc_server/__init__.py
--rw-r--r--   0        0        0     2083 2023-05-08 19:05:45.808914 atproto-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    11596 1970-01-01 00:00:00.000000 atproto-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-12 18:48:38.738671 atproto-0.0.4/LICENSE
+-rw-r--r--   0        0        0     9588 2023-05-12 18:48:38.738671 atproto-0.0.4/README.md
+-rw-r--r--   0        0        0      300 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/__init__.py
+-rw-r--r--   0        0        0      619 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/cid/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/cli/__init__.py
+-rw-r--r--   0        0        0     2767 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/clients/__init__.py
+-rw-r--r--   0        0        0     1156 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/clients/generate_async_client.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/models/__init__.py
+-rw-r--r--   0        0        0     2317 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/models/builder.py
+-rw-r--r--   0        0        0    18860 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/models/generator.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/namespaces/__init__.py
+-rw-r--r--   0        0        0     2562 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/namespaces/builder.py
+-rw-r--r--   0        0        0    11855 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/codegen/namespaces/generator.py
+-rw-r--r--   0        0        0      944 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/lexicon/__init__.py
+-rw-r--r--   0        0        0     4658 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/lexicon/models.py
+-rw-r--r--   0        0        0     3871 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/lexicon/parser.py
+-rw-r--r--   0        0        0     5298 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/nsid/__init__.py
+-rw-r--r--   0        0        0     3075 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/uri/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/client/__init__.py
+-rw-r--r--   0        0        0     5994 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/client/async_client.py
+-rw-r--r--   0        0        0      489 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/client/async_raw.py
+-rw-r--r--   0        0        0     3719 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/client/base.py
+-rw-r--r--   0        0        0     5555 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/client/client.py
+-rw-r--r--   0        0        0      469 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/client/raw.py
+-rw-r--r--   0        0        0    10098 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0     3278 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      836 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      890 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0     1014 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      927 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0     1061 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      970 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0     1778 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1564 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2457 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/record.py
+-rw-r--r--   0        0        0     1248 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0     4321 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0     1041 2023-05-12 18:48:38.738671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0     1497 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0     1076 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      855 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0     1181 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0     1066 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      734 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2441 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      738 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      665 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/block.py
+-rw-r--r--   0        0        0      667 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0     1004 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0     1133 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0     1123 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0      999 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0      574 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      576 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      830 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1932 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      586 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0     1735 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0     1082 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      553 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/base.py
+-rw-r--r--   0        0        0      713 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/blob_ref.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0     9928 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      712 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0     1071 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      839 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0     1097 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      839 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0     1161 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      890 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      824 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      953 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      911 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0     1129 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0     1370 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      651 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      621 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      887 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      586 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/label/defs.py
+-rw-r--r--   0        0        0     1323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0     1077 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0     1499 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      825 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0     2140 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0     1236 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      969 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0     1038 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0     1171 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1817 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1319 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      644 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      742 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0     1052 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      880 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0     1352 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0     1117 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1296 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      659 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0     1271 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0     1028 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      704 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0     1024 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      729 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      589 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      628 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      583 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0      323 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      752 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      744 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      822 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      986 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      764 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      872 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      916 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      969 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0     1253 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      637 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      640 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     2782 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0      425 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/type_conversion.py
+-rw-r--r--   0        0        0     3285 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/models/utils.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/namespaces/__init__.py
+-rw-r--r--   0        0        0    65433 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/namespaces/async_ns.py
+-rw-r--r--   0        0        0      361 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/namespaces/base.py
+-rw-r--r--   0        0        0    64495 2023-05-12 18:48:38.742671 atproto-0.0.4/atproto/xrpc_client/namespaces/sync_ns.py
+-rw-r--r--   0        0        0     4353 2023-05-12 18:48:38.746671 atproto-0.0.4/atproto/xrpc_client/request.py
+-rw-r--r--   0        0        0       43 2023-05-12 18:48:38.746671 atproto-0.0.4/atproto/xrpc_server/__init__.py
+-rw-r--r--   0        0        0     2083 2023-05-12 18:48:38.754671 atproto-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    11408 1970-01-01 00:00:00.000000 atproto-0.0.4/PKG-INFO
```

### Comparing `atproto-0.0.3/LICENSE` & `atproto-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/README.md` & `atproto-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 <p align="center">
     <a href="https://github.com/MarshalX/atproto">
-        <picture>
-            <source media="(prefers-color-scheme: dark)" srcset="https://github.com/MarshalX/atproto/raw/main/.github/images/logo_dark.png">
-            <img alt="Logo of atproto SDK for Python by Midjourney'" src="https://github.com/MarshalX/atproto/raw/main/.github/images/logo_white.png">
-        </picture>
+        <img alt="Logo of atproto SDK for Python by Midjourney'" src="https://github.com/MarshalX/atproto/raw/main/.github/images/logo.png">
     </a>
     <br>
     <b>Autogenerated from lexicons, well type hinted, documented, sync and async SDK for Python</b>
     <br>
     <a href="https://github.com/MarshalX/atproto/tree/main/examples">
         Examples
     </a>
```

### Comparing `atproto-0.0.3/atproto/cid/__init__.py` & `atproto-0.0.4/atproto/cid/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/codegen/__init__.py` & `atproto-0.0.4/atproto/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/codegen/clients/generate_async_client.py` & `atproto-0.0.4/atproto/codegen/clients/generate_async_client.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/codegen/models/builder.py` & `atproto-0.0.4/atproto/codegen/models/builder.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/codegen/models/generator.py` & `atproto-0.0.4/atproto/codegen/models/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,16 +315,19 @@
 def _generate_def_model(nsid: NSID, def_name: str, def_model: models.LexObject, model_type: ModelType) -> str:
     lines = [
         _get_model_class_def(def_name, model_type),
         _get_model_docstring(nsid, def_model, model_type),
         _get_model(nsid, def_model),
     ]
 
+    def_type = f'{nsid}#{def_name}'
     if def_name == 'main':
-        lines.append(f"{_(1)}_type: str = '{nsid}'")
+        def_type = str(nsid)
+
+    lines.append(f"{_(1)}_type: str = '{def_type}'")
 
     lines.append('')
 
     return join_code(lines)
 
 
 def _generate_def_token(def_name: str) -> str:
```

### Comparing `atproto-0.0.3/atproto/codegen/namespaces/builder.py` & `atproto-0.0.4/atproto/codegen/namespaces/builder.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/codegen/namespaces/generator.py` & `atproto-0.0.4/atproto/codegen/namespaces/generator.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/exceptions.py` & `atproto-0.0.4/atproto/exceptions.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/lexicon/models.py` & `atproto-0.0.4/atproto/lexicon/models.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/lexicon/parser.py` & `atproto-0.0.4/atproto/lexicon/parser.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/nsid/__init__.py` & `atproto-0.0.4/atproto/nsid/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/uri/__init__.py` & `atproto-0.0.4/atproto/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/client/async_client.py` & `atproto-0.0.4/atproto/xrpc_client/client/async_client.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/client/base.py` & `atproto-0.0.4/atproto/xrpc_client/client/base.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/client/client.py` & `atproto-0.0.4/atproto/xrpc_client/client/client.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/__init__.py` & `atproto-0.0.4/atproto/xrpc_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/defs.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     did: str
     handle: str
     avatar: Optional[str] = None
     displayName: Optional[str] = None
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
     viewer: Optional['models.AppBskyActorDefs.ViewerState'] = None
 
+    _type: str = 'app.bsky.actor.defs#profileViewBasic'
+
 
 @dataclass
 class ProfileView(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.actor.defs`.
 
     Attributes:
@@ -55,14 +57,16 @@
     avatar: Optional[str] = None
     description: Optional[str] = None
     displayName: Optional[str] = None
     indexedAt: Optional[str] = None
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
     viewer: Optional['models.AppBskyActorDefs.ViewerState'] = None
 
+    _type: str = 'app.bsky.actor.defs#profileView'
+
 
 @dataclass
 class ProfileViewDetailed(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.actor.defs`.
 
     Attributes:
@@ -89,14 +93,16 @@
     followersCount: Optional[int] = None
     followsCount: Optional[int] = None
     indexedAt: Optional[str] = None
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
     postsCount: Optional[int] = None
     viewer: Optional['models.AppBskyActorDefs.ViewerState'] = None
 
+    _type: str = 'app.bsky.actor.defs#profileViewDetailed'
+
 
 @dataclass
 class ViewerState(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.actor.defs`.
 
     Attributes:
@@ -108,7 +114,9 @@
     """
 
     blockedBy: Optional[bool] = None
     blocking: Optional[str] = None
     followedBy: Optional[str] = None
     following: Optional[str] = None
     muted: Optional[bool] = None
+
+    _type: str = 'app.bsky.actor.defs#viewerState'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/get_profile.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/get_profile.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/profile.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/profile.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/search_actors.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/search_actors.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/external.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/external.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,26 +40,30 @@
     """
 
     description: str
     title: str
     uri: str
     thumb: Optional[BlobRef] = None
 
+    _type: str = 'app.bsky.embed.external#external'
+
 
 @dataclass
 class View(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.embed.external`.
 
     Attributes:
         external: External.
     """
 
     external: 'models.AppBskyEmbedExternal.ViewExternal'
 
+    _type: str = 'app.bsky.embed.external#view'
+
 
 @dataclass
 class ViewExternal(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.embed.external`.
 
     Attributes:
@@ -69,7 +73,9 @@
         thumb: Thumb.
     """
 
     description: str
     title: str
     uri: str
     thumb: Optional[str] = None
+
+    _type: str = 'app.bsky.embed.external#viewExternal'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/images.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/images.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,26 +36,30 @@
         image: Image.
         alt: Alt.
     """
 
     alt: str
     image: BlobRef
 
+    _type: str = 'app.bsky.embed.images#image'
+
 
 @dataclass
 class View(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.embed.images`.
 
     Attributes:
         images: Images.
     """
 
     images: List['models.AppBskyEmbedImages.ViewImage']
 
+    _type: str = 'app.bsky.embed.images#view'
+
 
 @dataclass
 class ViewImage(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.embed.images`.
 
     Attributes:
@@ -63,7 +67,9 @@
         fullsize: Fullsize.
         alt: Alt.
     """
 
     alt: str
     fullsize: str
     thumb: str
+
+    _type: str = 'app.bsky.embed.images#viewImage'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/record.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/record.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     record: Union[
         'models.AppBskyEmbedRecord.ViewRecord',
         'models.AppBskyEmbedRecord.ViewNotFound',
         'models.AppBskyEmbedRecord.ViewBlocked',
         'Dict[str, Any]',
     ]
 
+    _type: str = 'app.bsky.embed.record#view'
+
 
 @dataclass
 class ViewRecord(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.embed.record`.
 
     Attributes:
@@ -72,30 +74,36 @@
                 'models.AppBskyEmbedRecordWithMedia.View',
                 'Dict[str, Any]',
             ]
         ]
     ] = None
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
 
+    _type: str = 'app.bsky.embed.record#viewRecord'
+
 
 @dataclass
 class ViewNotFound(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.embed.record`.
 
     Attributes:
         uri: Uri.
     """
 
     uri: str
 
+    _type: str = 'app.bsky.embed.record#viewNotFound'
+
 
 @dataclass
 class ViewBlocked(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.embed.record`.
 
     Attributes:
         uri: Uri.
     """
 
     uri: str
+
+    _type: str = 'app.bsky.embed.record#viewBlocked'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,7 +36,9 @@
     Attributes:
         record: Record.
         media: Media.
     """
 
     media: Union['models.AppBskyEmbedImages.View', 'models.AppBskyEmbedExternal.View', 'Dict[str, Any]']
     record: 'models.AppBskyEmbedRecord.View'
+
+    _type: str = 'app.bsky.embed.recordWithMedia#view'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/defs.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,28 +47,32 @@
     ] = None
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
     likeCount: Optional[int] = None
     replyCount: Optional[int] = None
     repostCount: Optional[int] = None
     viewer: Optional['models.AppBskyFeedDefs.ViewerState'] = None
 
+    _type: str = 'app.bsky.feed.defs#postView'
+
 
 @dataclass
 class ViewerState(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.feed.defs`.
 
     Attributes:
         repost: Repost.
         like: Like.
     """
 
     like: Optional[str] = None
     repost: Optional[str] = None
 
+    _type: str = 'app.bsky.feed.defs#viewerState'
+
 
 @dataclass
 class FeedViewPost(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.feed.defs`.
 
     Attributes:
@@ -77,42 +81,48 @@
         reason: Reason.
     """
 
     post: 'models.AppBskyFeedDefs.PostView'
     reason: Optional[Union['models.AppBskyFeedDefs.ReasonRepost', 'Dict[str, Any]']] = None
     reply: Optional['models.AppBskyFeedDefs.ReplyRef'] = None
 
+    _type: str = 'app.bsky.feed.defs#feedViewPost'
+
 
 @dataclass
 class ReplyRef(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.feed.defs`.
 
     Attributes:
         root: Root.
         parent: Parent.
     """
 
     parent: 'models.AppBskyFeedDefs.PostView'
     root: 'models.AppBskyFeedDefs.PostView'
 
+    _type: str = 'app.bsky.feed.defs#replyRef'
+
 
 @dataclass
 class ReasonRepost(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.feed.defs`.
 
     Attributes:
         by: By.
         indexedAt: Indexed at.
     """
 
     by: 'models.AppBskyActorDefs.ProfileViewBasic'
     indexedAt: str
 
+    _type: str = 'app.bsky.feed.defs#reasonRepost'
+
 
 @dataclass
 class ThreadViewPost(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.feed.defs`.
 
     Attributes:
@@ -137,34 +147,40 @@
                 'models.AppBskyFeedDefs.NotFoundPost',
                 'models.AppBskyFeedDefs.BlockedPost',
                 'Dict[str, Any]',
             ]
         ]
     ] = None
 
+    _type: str = 'app.bsky.feed.defs#threadViewPost'
+
 
 @dataclass
 class NotFoundPost(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.feed.defs`.
 
     Attributes:
         uri: Uri.
         notFound: Not found.
     """
 
     notFound: bool
     uri: str
 
+    _type: str = 'app.bsky.feed.defs#notFoundPost'
+
 
 @dataclass
 class BlockedPost(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.feed.defs`.
 
     Attributes:
         uri: Uri.
         blocked: Blocked.
     """
 
     blocked: bool
     uri: str
+
+    _type: str = 'app.bsky.feed.defs#blockedPost'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_likes.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_likes.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,7 +58,9 @@
         createdAt: Created at.
         actor: Actor.
     """
 
     actor: 'models.AppBskyActorDefs.ProfileView'
     createdAt: str
     indexedAt: str
+
+    _type: str = 'app.bsky.feed.getLikes#like'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_posts.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_posts.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/like.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/like.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/post.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/post.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         root: Root.
         parent: Parent.
     """
 
     parent: 'models.ComAtprotoRepoStrongRef.Main'
     root: 'models.ComAtprotoRepoStrongRef.Main'
 
+    _type: str = 'app.bsky.feed.post#replyRef'
+
 
 @dataclass
 class Entity(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.feed.post`. Deprecated: use facets instead.
 
     Attributes:
@@ -37,28 +39,32 @@
         value: Value.
     """
 
     index: 'models.AppBskyFeedPost.TextSlice'
     type: str
     value: str
 
+    _type: str = 'app.bsky.feed.post#entity'
+
 
 @dataclass
 class TextSlice(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.feed.post`. Deprecated. Use app.bsky.richtext instead -- A text segment. Start is inclusive, end is exclusive. Indices are for utf16-encoded strings.
 
     Attributes:
         start: Start.
         end: End.
     """
 
     end: int
     start: int
 
+    _type: str = 'app.bsky.feed.post#textSlice'
+
 
 @dataclass
 class Main(base.RecordModelBase):
 
     """Record model for :obj:`app.bsky.feed.post`.
 
     Attributes:
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/feed/repost.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/feed/repost.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/block.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/block.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/follow.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/follow.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_followers.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_followers.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_follows.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_follows.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,7 +64,9 @@
     indexedAt: str
     isRead: bool
     reason: str
     record: 'base.RecordModelBase'
     uri: str
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
     reasonSubject: Optional[str] = None
+
+    _type: str = 'app.bsky.notification.listNotifications#notification'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/notification/update_seen.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/notification/update_seen.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/richtext/facet.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/richtext/facet.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,32 +35,38 @@
 
     Attributes:
         did: Did.
     """
 
     did: str
 
+    _type: str = 'app.bsky.richtext.facet#mention'
+
 
 @dataclass
 class Link(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.richtext.facet`. A facet feature for links.
 
     Attributes:
         uri: Uri.
     """
 
     uri: str
 
+    _type: str = 'app.bsky.richtext.facet#link'
+
 
 @dataclass
 class ByteSlice(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.richtext.facet`. A text segment. Start is inclusive, end is exclusive. Indices are for utf8-encoded strings.
 
     Attributes:
         byteStart: Byte start.
         byteEnd: Byte end.
     """
 
     byteEnd: int
     byteStart: int
+
+    _type: str = 'app.bsky.richtext.facet#byteSlice'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py` & `atproto-0.0.4/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/base.py` & `atproto-0.0.4/atproto/xrpc_client/models/base.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/blob_ref.py` & `atproto-0.0.4/atproto/xrpc_client/models/blob_ref.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/defs.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,16 @@
     resolvedReportIds: List[int]
     subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 'Dict[str, Any]']
     subjectBlobCids: List[str]
     createLabelVals: Optional[List[str]] = None
     negateLabelVals: Optional[List[str]] = None
     reversal: Optional['models.ComAtprotoAdminDefs.ActionReversal'] = None
 
+    _type: str = 'com.atproto.admin.defs#actionView'
+
 
 @dataclass
 class ActionViewDetail(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
@@ -73,28 +75,32 @@
     resolvedReports: List['models.ComAtprotoAdminDefs.ReportView']
     subject: Union['models.ComAtprotoAdminDefs.RepoView', 'models.ComAtprotoAdminDefs.RecordView', 'Dict[str, Any]']
     subjectBlobs: List['models.ComAtprotoAdminDefs.BlobView']
     createLabelVals: Optional[List[str]] = None
     negateLabelVals: Optional[List[str]] = None
     reversal: Optional['models.ComAtprotoAdminDefs.ActionReversal'] = None
 
+    _type: str = 'com.atproto.admin.defs#actionViewDetail'
+
 
 @dataclass
 class ActionViewCurrent(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
         id: Id.
         action: Action.
     """
 
     action: 'models.ComAtprotoAdminDefs.ActionType'
     id: int
 
+    _type: str = 'com.atproto.admin.defs#actionViewCurrent'
+
 
 @dataclass
 class ActionReversal(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
@@ -103,14 +109,16 @@
         createdAt: Created at.
     """
 
     createdAt: str
     createdBy: str
     reason: str
 
+    _type: str = 'com.atproto.admin.defs#actionReversal'
+
 
 ActionType = Literal['Takedown', 'Flag', 'Acknowledge', 'Escalate']
 
 Takedown: Literal['takedown'] = 'takedown'
 
 Flag: Literal['flag'] = 'flag'
 
@@ -138,14 +146,16 @@
     id: int
     reasonType: 'models.ComAtprotoModerationDefs.ReasonType'
     reportedBy: str
     resolvedByActionIds: List[int]
     subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 'Dict[str, Any]']
     reason: Optional[str] = None
 
+    _type: str = 'com.atproto.admin.defs#reportView'
+
 
 @dataclass
 class ReportViewDetail(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
@@ -162,14 +172,16 @@
     id: int
     reasonType: 'models.ComAtprotoModerationDefs.ReasonType'
     reportedBy: str
     resolvedByActions: List['models.ComAtprotoAdminDefs.ActionView']
     subject: Union['models.ComAtprotoAdminDefs.RepoView', 'models.ComAtprotoAdminDefs.RecordView', 'Dict[str, Any]']
     reason: Optional[str] = None
 
+    _type: str = 'com.atproto.admin.defs#reportViewDetail'
+
 
 @dataclass
 class RepoView(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
@@ -186,14 +198,16 @@
     handle: str
     indexedAt: str
     moderation: 'models.ComAtprotoAdminDefs.Moderation'
     relatedRecords: List['base.RecordModelBase']
     email: Optional[str] = None
     invitedBy: Optional['models.ComAtprotoServerDefs.InviteCode'] = None
 
+    _type: str = 'com.atproto.admin.defs#repoView'
+
 
 @dataclass
 class RepoViewDetail(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
@@ -214,26 +228,30 @@
     moderation: 'models.ComAtprotoAdminDefs.ModerationDetail'
     relatedRecords: List['base.RecordModelBase']
     email: Optional[str] = None
     invitedBy: Optional['models.ComAtprotoServerDefs.InviteCode'] = None
     invites: Optional[List['models.ComAtprotoServerDefs.InviteCode']] = None
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
 
+    _type: str = 'com.atproto.admin.defs#repoViewDetail'
+
 
 @dataclass
 class RepoRef(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
         did: Did.
     """
 
     did: str
 
+    _type: str = 'com.atproto.admin.defs#repoRef'
+
 
 @dataclass
 class RecordView(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
@@ -250,14 +268,16 @@
     cid: str
     indexedAt: str
     moderation: 'models.ComAtprotoAdminDefs.Moderation'
     repo: 'models.ComAtprotoAdminDefs.RepoView'
     uri: str
     value: 'base.RecordModelBase'
 
+    _type: str = 'com.atproto.admin.defs#recordView'
+
 
 @dataclass
 class RecordViewDetail(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
@@ -276,26 +296,30 @@
     indexedAt: str
     moderation: 'models.ComAtprotoAdminDefs.ModerationDetail'
     repo: 'models.ComAtprotoAdminDefs.RepoView'
     uri: str
     value: 'base.RecordModelBase'
     labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
 
+    _type: str = 'com.atproto.admin.defs#recordViewDetail'
+
 
 @dataclass
 class Moderation(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
         currentAction: Current action.
     """
 
     currentAction: Optional['models.ComAtprotoAdminDefs.ActionViewCurrent'] = None
 
+    _type: str = 'com.atproto.admin.defs#moderation'
+
 
 @dataclass
 class ModerationDetail(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
@@ -304,14 +328,16 @@
         reports: Reports.
     """
 
     actions: List['models.ComAtprotoAdminDefs.ActionView']
     reports: List['models.ComAtprotoAdminDefs.ReportView']
     currentAction: Optional['models.ComAtprotoAdminDefs.ActionViewCurrent'] = None
 
+    _type: str = 'com.atproto.admin.defs#moderationDetail'
+
 
 @dataclass
 class BlobView(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
@@ -328,28 +354,32 @@
     mimeType: str
     size: int
     details: Optional[
         Union['models.ComAtprotoAdminDefs.ImageDetails', 'models.ComAtprotoAdminDefs.VideoDetails', 'Dict[str, Any]']
     ] = None
     moderation: Optional['models.ComAtprotoAdminDefs.Moderation'] = None
 
+    _type: str = 'com.atproto.admin.defs#blobView'
+
 
 @dataclass
 class ImageDetails(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
         width: Width.
         height: Height.
     """
 
     height: int
     width: int
 
+    _type: str = 'com.atproto.admin.defs#imageDetails'
+
 
 @dataclass
 class VideoDetails(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
@@ -357,7 +387,9 @@
         height: Height.
         length: Length.
     """
 
     height: int
     length: int
     width: int
+
+    _type: str = 'com.atproto.admin.defs#videoDetails'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_record.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/get_repo.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/get_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/search_repos.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/search_repos.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/identity/update_handle.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/identity/update_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/label/defs.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/label/defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,7 +27,9 @@
 
     cts: str
     src: str
     uri: str
     val: str
     cid: Optional[str] = None
     neg: Optional[bool] = None
+
+    _type: str = 'com.atproto.label.defs#label'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/label/query_labels.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/label/query_labels.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,20 +21,24 @@
         seq: Seq.
         labels: Labels.
     """
 
     labels: List['models.ComAtprotoLabelDefs.Label']
     seq: int
 
+    _type: str = 'com.atproto.label.subscribeLabels#labels'
+
 
 @dataclass
 class Info(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.label.subscribeLabels`.
 
     Attributes:
         name: Name.
         message: Message.
     """
 
     name: str
     message: Optional[str] = None
+
+    _type: str = 'com.atproto.label.subscribeLabels#info'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/moderation/create_report.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/moderation/create_report.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/moderation/defs.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/moderation/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py`

 * *Files 21% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         value: Value.
     """
 
     collection: str
     value: 'base.RecordModelBase'
     rkey: Optional[str] = None
 
+    _type: str = 'com.atproto.repo.applyWrites#create'
+
 
 @dataclass
 class Update(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.repo.applyWrites`. Update an existing record.
 
     Attributes:
@@ -64,20 +66,24 @@
         value: Value.
     """
 
     collection: str
     rkey: str
     value: 'base.RecordModelBase'
 
+    _type: str = 'com.atproto.repo.applyWrites#update'
+
 
 @dataclass
 class Delete(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.repo.applyWrites`. Delete an existing record.
 
     Attributes:
         collection: Collection.
         rkey: Rkey.
     """
 
     collection: str
     rkey: str
+
+    _type: str = 'com.atproto.repo.applyWrites#delete'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/create_record.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/create_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/delete_record.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/delete_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/get_record.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/get_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/list_records.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/list_records.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,7 +60,9 @@
         cid: Cid.
         value: Value.
     """
 
     cid: str
     uri: str
     value: 'base.RecordModelBase'
+
+    _type: str = 'com.atproto.repo.listRecords#record'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/put_record.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/put_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_account.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_account.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_app_password.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_app_password.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,10 +34,12 @@
         createdAt: Created at.
     """
 
     createdAt: str
     name: str
     password: str
 
+    _type: str = 'com.atproto.server.createAppPassword#appPassword'
+
 
 #: Response reference to :obj:`AppPassword` model.
 ResponseRef: Type[AppPassword] = AppPassword
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,7 +48,9 @@
     Attributes:
         account: Account.
         codes: Codes.
     """
 
     account: str
     codes: List[str]
+
+    _type: str = 'com.atproto.server.createInviteCodes#accountCodes'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/create_session.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/create_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/defs.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,20 +31,24 @@
     code: str
     createdAt: str
     createdBy: str
     disabled: bool
     forAccount: str
     uses: List['models.ComAtprotoServerDefs.InviteCodeUse']
 
+    _type: str = 'com.atproto.server.defs#inviteCode'
+
 
 @dataclass
 class InviteCodeUse(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.server.defs`.
 
     Attributes:
         usedBy: Used by.
         usedAt: Used at.
     """
 
     usedAt: str
     usedBy: str
+
+    _type: str = 'com.atproto.server.defs#inviteCodeUse'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/delete_account.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/delete_account.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/describe_server.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/describe_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,7 +36,9 @@
     Attributes:
         privacyPolicy: Privacy policy.
         termsOfService: Terms of service.
     """
 
     privacyPolicy: Optional[str] = None
     termsOfService: Optional[str] = None
+
+    _type: str = 'com.atproto.server.describeServer#links'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/get_session.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/get_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,7 +32,9 @@
     Attributes:
         name: Name.
         createdAt: Created at.
     """
 
     createdAt: str
     name: str
+
+    _type: str = 'com.atproto.server.listAppPasswords#appPassword'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/refresh_session.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/refresh_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/reset_password.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/reset_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_blob.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_blob.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_head.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_head.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_record.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/get_repo.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/get_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/list_repos.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/list_repos.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,7 +48,9 @@
     Attributes:
         did: Did.
         head: Head.
     """
 
     did: str
     head: str
+
+    _type: str = 'com.atproto.sync.listRepos#repo'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py` & `atproto-0.0.4/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     rebase: bool
     repo: str
     seq: int
     time: str
     tooBig: bool
     prev: Optional[CID] = None
 
+    _type: str = 'com.atproto.sync.subscribeRepos#commit'
+
 
 @dataclass
 class Handle(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.sync.subscribeRepos`.
 
     Attributes:
@@ -56,14 +58,16 @@
     """
 
     did: str
     handle: str
     seq: int
     time: str
 
+    _type: str = 'com.atproto.sync.subscribeRepos#handle'
+
 
 @dataclass
 class Migrate(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.sync.subscribeRepos`.
 
     Attributes:
@@ -74,14 +78,16 @@
     """
 
     did: str
     seq: int
     time: str
     migrateTo: Optional[str] = None
 
+    _type: str = 'com.atproto.sync.subscribeRepos#migrate'
+
 
 @dataclass
 class Tombstone(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.sync.subscribeRepos`.
 
     Attributes:
@@ -90,28 +96,32 @@
         time: Time.
     """
 
     did: str
     seq: int
     time: str
 
+    _type: str = 'com.atproto.sync.subscribeRepos#tombstone'
+
 
 @dataclass
 class Info(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.sync.subscribeRepos`.
 
     Attributes:
         name: Name.
         message: Message.
     """
 
     name: str
     message: Optional[str] = None
 
+    _type: str = 'com.atproto.sync.subscribeRepos#info'
+
 
 @dataclass
 class RepoOp(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.sync.subscribeRepos`.
 
     Attributes:
@@ -119,7 +129,9 @@
         path: Path.
         cid: Cid.
     """
 
     action: str
     path: str
     cid: Optional[CID] = None
+
+    _type: str = 'com.atproto.sync.subscribeRepos#repoOp'
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/models/utils.py` & `atproto-0.0.4/atproto/xrpc_client/models/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
     try:
         # validate unexpected fields
         model(**model_data)
 
         return from_dict(model, model_data, config=_DACITE_CONFIG)
     except TypeError as e:
+        # FIXME(MarshalX): "Params missing 1 required positional argument: 'rkey'" should raise another error
         msg = str(e).replace('__init__()', model.__name__)
         raise UnexpectedFieldError(msg)
     except exceptions.MissingValueError as e:
         raise MissingValueError(str(e))
     except exceptions.WrongTypeError as e:
         raise WrongTypeError(str(e))
     except exceptions.DaciteFieldError as e:
```

### Comparing `atproto-0.0.3/atproto/xrpc_client/namespaces/async_ns.py` & `atproto-0.0.4/atproto/xrpc_client/namespaces/async_ns.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/namespaces/sync_ns.py` & `atproto-0.0.4/atproto/xrpc_client/namespaces/sync_ns.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/atproto/xrpc_client/request.py` & `atproto-0.0.4/atproto/xrpc_client/request.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.3/pyproject.toml` & `atproto-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atproto"
-version = "0.0.3"
+version = "0.0.4"
 description = "The AT Protocol SDK"
 authors = ["Ilya (Marshal) <ilya@marshal.dev>"]
 license = "MIT"
 repository = "https://github.com/MarshalX/atproto"
 readme = "README.md"
 keywords = ["library", "sdk", "codegen", "xrpc", "xrpc-client", "atprotocol", "atproto", "lexicon", "parser", "schema", "bluesky", "bluesky-api", "at", "uri", "atp", "nsid", "did", "cid"]
 classifiers = [
```

### Comparing `atproto-0.0.3/PKG-INFO` & `atproto-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atproto
-Version: 0.0.3
+Version: 0.0.4
 Summary: The AT Protocol SDK
 Home-page: https://github.com/MarshalX/atproto
 License: MIT
 Keywords: library,sdk,codegen,xrpc,xrpc-client,atprotocol,atproto,lexicon,parser,schema,bluesky,bluesky-api,at,uri,atp,nsid,did,cid
 Author: Ilya (Marshal)
 Author-email: ilya@marshal.dev
 Requires-Python: >=3.7,<4.0
@@ -37,18 +37,15 @@
 Project-URL: Documentation, https://atproto.rtfd.io
 Project-URL: Repository, https://github.com/MarshalX/atproto
 Project-URL: Tracker, https://github.com/MarshalX/atproto/issues
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="https://github.com/MarshalX/atproto">
-        <picture>
-            <source media="(prefers-color-scheme: dark)" srcset="https://github.com/MarshalX/atproto/raw/main/.github/images/logo_dark.png">
-            <img alt="Logo of atproto SDK for Python by Midjourney'" src="https://github.com/MarshalX/atproto/raw/main/.github/images/logo_white.png">
-        </picture>
+        <img alt="Logo of atproto SDK for Python by Midjourney'" src="https://github.com/MarshalX/atproto/raw/main/.github/images/logo.png">
     </a>
     <br>
     <b>Autogenerated from lexicons, well type hinted, documented, sync and async SDK for Python</b>
     <br>
     <a href="https://github.com/MarshalX/atproto/tree/main/examples">
         Examples
     </a>
```

