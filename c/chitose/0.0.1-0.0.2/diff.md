# Comparing `tmp/chitose-0.0.1.tar.gz` & `tmp/chitose-0.0.2.tar.gz`

## Comparing `chitose-0.0.1.tar` & `chitose-0.0.2.tar`

### file list

```diff
@@ -1,148 +1,148 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 chitose-0.0.1/.gitmodules
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 chitose-0.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/__init__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/agent.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/object.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/record.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/xrpc.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/__init__.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/__init__.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/actor/profile.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/embed/external.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/embed/images.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/embed/record.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/feed/defs.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/feed/get_posts.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/feed/like.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/feed/post.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/feed/repost.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/graph/block.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/graph/follow.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/graph/get_blocks.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/__init__.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/__init__.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0    10189 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/defs.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/label/__init__.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/label/defs.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/create_account.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/create_session.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/defs.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/get_session.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 chitose-0.0.1/chitose/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/make.bat
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.app.bsky.actor.rst
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.app.bsky.embed.rst
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.app.bsky.feed.rst
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.app.bsky.graph.rst
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.app.bsky.notification.rst
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.app.bsky.richtext.rst
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.app.bsky.rst
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.app.bsky.unspecced.rst
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.app.rst
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.com.atproto.admin.rst
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.com.atproto.identity.rst
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.com.atproto.label.rst
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.com.atproto.moderation.rst
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.com.atproto.repo.rst
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.com.atproto.rst
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.com.atproto.server.rst
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.com.atproto.sync.rst
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.com.rst
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/chitose.rst
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/conf.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/index.rst
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 chitose-0.0.1/docs/source/modules.rst
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 chitose-0.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 chitose-0.0.1/LICENSE
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 chitose-0.0.1/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 chitose-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 chitose-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 chitose-0.0.2/.gitmodules
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 chitose-0.0.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/agent.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/object.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/record.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/xrpc.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/__init__.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/__init__.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/embed/record.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/block.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/__init__.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/__init__.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0    11200 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/label/defs.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 chitose-0.0.2/chitose/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/make.bat
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.actor.rst
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.embed.rst
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.feed.rst
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.graph.rst
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.notification.rst
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.richtext.rst
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.rst
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.bsky.unspecced.rst
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.app.rst
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.admin.rst
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.identity.rst
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.label.rst
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.moderation.rst
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.repo.rst
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.rst
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.server.rst
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.atproto.sync.rst
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.com.rst
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/chitose.rst
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/conf.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/index.rst
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 chitose-0.0.2/docs/source/modules.rst
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 chitose-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 chitose-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 chitose-0.0.2/README.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 chitose-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 chitose-0.0.2/PKG-INFO
```

### Comparing `chitose-0.0.1/chitose/agent.py` & `chitose-0.0.2/chitose/agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from __future__ import annotations
 import json
 
-from .app import App
-from .com import Com
-from chitose.com.atproto.server import create_session
+from .app import App_
+from .com import Com_
 
 
 class BskyAgent:
     def __init__(self, service: str) -> None:
         self.service = service
-        self.headers = {}
+        self.headers: dict[str, str] = {}
 
     @property
     def app(self):
-        return App(self.service, self.headers)
+        return App_(self.service, self.headers)
 
     @property
     def com(self):
-        return Com(self.service, self.headers)
+        return Com_(self.service, self.headers)
 
     def login(self, identifier: str, password: str) -> None:
         session = json.loads(
-            create_session(service=self.service, headers={},
-                           identifier=identifier, password=password))
+            self.com.atproto.server.create_session(
+                identifier=identifier, password=password))
         if 'accessJwt' in session:
             self.headers['authorization'] \
                 = f'Bearer {session["accessJwt"]}'
```

### Comparing `chitose-0.0.1/chitose/xrpc.py` & `chitose-0.0.2/chitose/xrpc.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/chitose/app/bsky/__init__.py` & `chitose-0.0.2/chitose/app/bsky/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from .actor import Actor
-from .embed import Embed
-from .feed import Feed
-from .graph import Graph
-from .notification import Notification
-from .richtext import Richtext
-from .unspecced import Unspecced
+from .actor import Actor_
+from .embed import Embed_
+from .feed import Feed_
+from .graph import Graph_
+from .notification import Notification_
+from .richtext import Richtext_
+from .unspecced import Unspecced_
 
-class Bsky:
+class Bsky_:
 
     def __init__(self, service: str, headers: dict[str, str]):
         self.service = service
         self.headers = headers
 
     @property
     def actor(self):
-        return Actor(self.service, self.headers)
+        return Actor_(self.service, self.headers)
 
     @property
     def embed(self):
-        return Embed(self.service, self.headers)
+        return Embed_(self.service, self.headers)
 
     @property
     def feed(self):
-        return Feed(self.service, self.headers)
+        return Feed_(self.service, self.headers)
 
     @property
     def graph(self):
-        return Graph(self.service, self.headers)
+        return Graph_(self.service, self.headers)
 
     @property
     def notification(self):
-        return Notification(self.service, self.headers)
+        return Notification_(self.service, self.headers)
 
     @property
     def richtext(self):
-        return Richtext(self.service, self.headers)
+        return Richtext_(self.service, self.headers)
 
     @property
     def unspecced(self):
-        return Unspecced(self.service, self.headers)
+        return Unspecced_(self.service, self.headers)
```

### Comparing `chitose-0.0.1/chitose/app/bsky/actor/defs.py` & `chitose-0.0.2/chitose/app/bsky/actor/defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
+import chitose.app.bsky.actor.defs
 import chitose.com.atproto.label.defs
 import typing
 
 class ProfileViewBasic(chitose.Object):
 
-    def __init__(self, did: str, handle: str, display_name: typing.Optional[str]=None, avatar: typing.Optional[str]=None, viewer: typing.Optional[ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
+    def __init__(self, did: str, handle: str, display_name: typing.Optional[str]=None, avatar: typing.Optional[str]=None, viewer: typing.Optional[chitose.app.bsky.actor.defs.ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.did = did
         self.handle = handle
         self.display_name = display_name
         self.avatar = avatar
         self.viewer = viewer
         self.labels = labels
 
     def to_dict(self):
         return {'did': self.did, 'handle': self.handle, 'displayName': self.display_name, 'avatar': self.avatar, 'viewer': self.viewer, 'labels': self.labels}
 
 class ProfileView(chitose.Object):
 
-    def __init__(self, did: str, handle: str, display_name: typing.Optional[str]=None, description: typing.Optional[str]=None, avatar: typing.Optional[str]=None, indexed_at: typing.Optional[str]=None, viewer: typing.Optional[ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
+    def __init__(self, did: str, handle: str, display_name: typing.Optional[str]=None, description: typing.Optional[str]=None, avatar: typing.Optional[str]=None, indexed_at: typing.Optional[str]=None, viewer: typing.Optional[chitose.app.bsky.actor.defs.ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.did = did
         self.handle = handle
         self.display_name = display_name
         self.description = description
         self.avatar = avatar
         self.indexed_at = indexed_at
         self.viewer = viewer
         self.labels = labels
 
     def to_dict(self):
         return {'did': self.did, 'handle': self.handle, 'displayName': self.display_name, 'description': self.description, 'avatar': self.avatar, 'indexedAt': self.indexed_at, 'viewer': self.viewer, 'labels': self.labels}
 
 class ProfileViewDetailed(chitose.Object):
 
-    def __init__(self, did: str, handle: str, display_name: typing.Optional[str]=None, description: typing.Optional[str]=None, avatar: typing.Optional[str]=None, banner: typing.Optional[str]=None, followers_count: typing.Optional[int]=None, follows_count: typing.Optional[int]=None, posts_count: typing.Optional[int]=None, indexed_at: typing.Optional[str]=None, viewer: typing.Optional[ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
+    def __init__(self, did: str, handle: str, display_name: typing.Optional[str]=None, description: typing.Optional[str]=None, avatar: typing.Optional[str]=None, banner: typing.Optional[str]=None, followers_count: typing.Optional[int]=None, follows_count: typing.Optional[int]=None, posts_count: typing.Optional[int]=None, indexed_at: typing.Optional[str]=None, viewer: typing.Optional[chitose.app.bsky.actor.defs.ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.did = did
         self.handle = handle
         self.display_name = display_name
         self.description = description
         self.avatar = avatar
         self.banner = banner
         self.followers_count = followers_count
```

### Comparing `chitose-0.0.1/chitose/app/bsky/actor/profile.py` & `chitose-0.0.2/chitose/app/bsky/actor/profile.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/chitose/app/bsky/embed/external.py` & `chitose-0.0.2/chitose/app/bsky/embed/external.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
+import chitose.app.bsky.embed.external
 import typing
 
 class External(chitose.Object):
 
-    def __init__(self, external: External) -> None:
+    def __init__(self, external: chitose.app.bsky.embed.external.ExternalExternal) -> None:
         self.external = external
 
     def to_dict(self):
         return {'external': self.external}
 
-class External(chitose.Object):
+class ExternalExternal(chitose.Object):
 
     def __init__(self, uri: str, title: str, description: str, thumb: typing.Optional[typing.Any]=None) -> None:
         self.uri = uri
         self.title = title
         self.description = description
         self.thumb = thumb
 
     def to_dict(self):
         return {'uri': self.uri, 'title': self.title, 'description': self.description, 'thumb': self.thumb}
 
 class View(chitose.Object):
 
-    def __init__(self, external: ViewExternal) -> None:
+    def __init__(self, external: chitose.app.bsky.embed.external.ViewExternal) -> None:
         self.external = external
 
     def to_dict(self):
         return {'external': self.external}
 
 class ViewExternal(chitose.Object):
```

### Comparing `chitose-0.0.1/chitose/app/bsky/embed/images.py` & `chitose-0.0.2/chitose/app/bsky/embed/images.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
+import chitose.app.bsky.embed.images
 import typing
 
 class Images(chitose.Object):
 
-    def __init__(self, images: list[Image]) -> None:
+    def __init__(self, images: list[chitose.app.bsky.embed.images.Image]) -> None:
         self.images = images
 
     def to_dict(self):
         return {'images': self.images}
 
 class Image(chitose.Object):
 
@@ -18,15 +19,15 @@
         self.alt = alt
 
     def to_dict(self):
         return {'image': self.image, 'alt': self.alt}
 
 class View(chitose.Object):
 
-    def __init__(self, images: list[ViewImage]) -> None:
+    def __init__(self, images: list[chitose.app.bsky.embed.images.ViewImage]) -> None:
         self.images = images
 
     def to_dict(self):
         return {'images': self.images}
 
 class ViewImage(chitose.Object):
```

### Comparing `chitose-0.0.1/chitose/app/bsky/embed/record.py` & `chitose-0.0.2/chitose/app/bsky/embed/record.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.actor.defs
 import chitose.app.bsky.embed.external
 import chitose.app.bsky.embed.images
+import chitose.app.bsky.embed.record
 import chitose.app.bsky.embed.record_with_media
 import chitose.com.atproto.label.defs
-import chitose.com.atproto.repo
+import chitose.com.atproto.repo.strong_ref
 import typing
 
 class Record(chitose.Object):
 
-    def __init__(self, record: chitose.com.atproto.repo.StrongRef) -> None:
+    def __init__(self, record: chitose.com.atproto.repo.strong_ref.StrongRef) -> None:
         self.record = record
 
     def to_dict(self):
         return {'record': self.record}
 
 class View(chitose.Object):
 
-    def __init__(self, record: typing.Union[ViewRecord, ViewNotFound, ViewBlocked]) -> None:
+    def __init__(self, record: typing.Union[chitose.app.bsky.embed.record.ViewRecord, chitose.app.bsky.embed.record.ViewNotFound, chitose.app.bsky.embed.record.ViewBlocked]) -> None:
         self.record = record
 
     def to_dict(self):
         return {'record': self.record}
 
 class ViewRecord(chitose.Object):
 
-    def __init__(self, uri: str, cid: str, author: chitose.app.bsky.actor.defs.ProfileViewBasic, value: typing.Any, indexed_at: str, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None, embeds: typing.Optional[list[typing.Union[chitose.app.bsky.embed.images.View, chitose.app.bsky.embed.external.View, View, chitose.app.bsky.embed.record_with_media.View]]]=None) -> None:
+    def __init__(self, uri: str, cid: str, author: chitose.app.bsky.actor.defs.ProfileViewBasic, value: typing.Any, indexed_at: str, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None, embeds: typing.Optional[list[typing.Union[chitose.app.bsky.embed.images.View, chitose.app.bsky.embed.external.View, chitose.app.bsky.embed.record.View, chitose.app.bsky.embed.record_with_media.View]]]=None) -> None:
         self.uri = uri
         self.cid = cid
         self.author = author
         self.value = value
         self.indexed_at = indexed_at
         self.labels = labels
         self.embeds = embeds
```

### Comparing `chitose-0.0.1/chitose/app/bsky/embed/record_with_media.py` & `chitose-0.0.2/chitose/app/bsky/embed/record_with_media.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
-import chitose.app.bsky.embed
 import chitose.app.bsky.embed.external
 import chitose.app.bsky.embed.images
 import chitose.app.bsky.embed.record
 import typing
 
 class RecordWithMedia(chitose.Object):
 
-    def __init__(self, record: chitose.app.bsky.embed.Record, media: typing.Union[chitose.app.bsky.embed.Images, chitose.app.bsky.embed.External]) -> None:
+    def __init__(self, record: chitose.app.bsky.embed.record.Record, media: typing.Union[chitose.app.bsky.embed.images.Images, chitose.app.bsky.embed.external.External]) -> None:
         self.record = record
         self.media = media
 
     def to_dict(self):
         return {'record': self.record, 'media': self.media}
 
 class View(chitose.Object):
```

### Comparing `chitose-0.0.1/chitose/app/bsky/feed/__init__.py` & `chitose-0.0.2/chitose/app/bsky/feed/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from .defs import *
-from .get_author_feed import *
-from .get_likes import *
-from .get_post_thread import *
-from .get_posts import *
-from .get_reposted_by import *
-from .get_timeline import *
-from .like import *
-from .post import *
-from .repost import *
+from .get_author_feed import _get_author_feed
+from .get_likes import _get_likes
+from .get_post_thread import _get_post_thread
+from .get_posts import _get_posts
+from .get_reposted_by import _get_reposted_by
+from .get_timeline import _get_timeline
+import chitose
+import typing
 
-class Feed:
+class Feed_:
 
     def __init__(self, service: str, headers: dict[str, str]):
         self.service = service
         self.headers = headers
 
     def get_timeline(self, algorithm: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
-        return get_timeline(self.service, self.headers, algorithm, limit, cursor)
+        """A view of the user's home timeline."""
+        return _get_timeline(self.service, self.headers, algorithm, limit, cursor)
 
     def get_author_feed(self, actor: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
-        return get_author_feed(self.service, self.headers, actor, limit, cursor)
+        """A view of an actor's feed."""
+        return _get_author_feed(self.service, self.headers, actor, limit, cursor)
 
     def get_likes(self, uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
-        return get_likes(self.service, self.headers, uri, cid, limit, cursor)
+        """"""
+        return _get_likes(self.service, self.headers, uri, cid, limit, cursor)
 
     def get_post_thread(self, uri: str, depth: typing.Optional[int]=None):
-        return get_post_thread(self.service, self.headers, uri, depth)
+        """"""
+        return _get_post_thread(self.service, self.headers, uri, depth)
 
     def get_reposted_by(self, uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
-        return get_reposted_by(self.service, self.headers, uri, cid, limit, cursor)
+        """"""
+        return _get_reposted_by(self.service, self.headers, uri, cid, limit, cursor)
 
     def get_posts(self, uris: list[str]):
-        return get_posts(self.service, self.headers, uris)
+        """A view of an actor's feed."""
+        return _get_posts(self.service, self.headers, uris)
```

### Comparing `chitose-0.0.1/chitose/app/bsky/feed/defs.py` & `chitose-0.0.2/chitose/app/bsky/feed/post.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,52 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
-import chitose.app.bsky.actor.defs
 import chitose.app.bsky.embed.external
 import chitose.app.bsky.embed.images
 import chitose.app.bsky.embed.record
 import chitose.app.bsky.embed.record_with_media
-import chitose.com.atproto.label.defs
+import chitose.app.bsky.feed.post
+import chitose.app.bsky.richtext.facet
+import chitose.com.atproto.repo.strong_ref
 import typing
 
-class PostView(chitose.Object):
+class Post(chitose.Record):
 
-    def __init__(self, uri: str, cid: str, author: chitose.app.bsky.actor.defs.ProfileViewBasic, record: typing.Any, indexed_at: str, embed: typing.Optional[typing.Union[chitose.app.bsky.embed.images.View, chitose.app.bsky.embed.external.View, chitose.app.bsky.embed.record.View, chitose.app.bsky.embed.record_with_media.View]]=None, reply_count: typing.Optional[int]=None, repost_count: typing.Optional[int]=None, like_count: typing.Optional[int]=None, viewer: typing.Optional[ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
-        self.uri = uri
-        self.cid = cid
-        self.author = author
-        self.record = record
-        self.indexed_at = indexed_at
-        self.embed = embed
-        self.reply_count = reply_count
-        self.repost_count = repost_count
-        self.like_count = like_count
-        self.viewer = viewer
-        self.labels = labels
-
-    def to_dict(self):
-        return {'uri': self.uri, 'cid': self.cid, 'author': self.author, 'record': self.record, 'indexedAt': self.indexed_at, 'embed': self.embed, 'replyCount': self.reply_count, 'repostCount': self.repost_count, 'likeCount': self.like_count, 'viewer': self.viewer, 'labels': self.labels}
-
-class ViewerState(chitose.Object):
-
-    def __init__(self, repost: typing.Optional[str]=None, like: typing.Optional[str]=None) -> None:
-        self.repost = repost
-        self.like = like
-
-    def to_dict(self):
-        return {'repost': self.repost, 'like': self.like}
-
-class FeedViewPost(chitose.Object):
-
-    def __init__(self, post: PostView, reply: typing.Optional[ReplyRef]=None, reason: typing.Optional[ReasonRepost]=None) -> None:
-        self.post = post
+    def __init__(self, text: str, created_at: str, entities: typing.Optional[list[chitose.app.bsky.feed.post.Entity]]=None, facets: typing.Optional[list[chitose.app.bsky.richtext.facet.Facet]]=None, reply: typing.Optional[chitose.app.bsky.feed.post.ReplyRef]=None, embed: typing.Optional[typing.Union[chitose.app.bsky.embed.images.Images, chitose.app.bsky.embed.external.External, chitose.app.bsky.embed.record.Record, chitose.app.bsky.embed.record_with_media.RecordWithMedia]]=None) -> None:
+        self.text = text
+        self.created_at = created_at
+        self.entities = entities
+        self.facets = facets
         self.reply = reply
-        self.reason = reason
+        self.embed = embed
 
     def to_dict(self):
-        return {'post': self.post, 'reply': self.reply, 'reason': self.reason}
+        return {'text': self.text, 'createdAt': self.created_at, 'entities': self.entities, 'facets': self.facets, 'reply': self.reply, 'embed': self.embed}
 
 class ReplyRef(chitose.Object):
 
-    def __init__(self, root: PostView, parent: PostView) -> None:
+    def __init__(self, root: chitose.com.atproto.repo.strong_ref.StrongRef, parent: chitose.com.atproto.repo.strong_ref.StrongRef) -> None:
         self.root = root
         self.parent = parent
 
     def to_dict(self):
         return {'root': self.root, 'parent': self.parent}
 
-class ReasonRepost(chitose.Object):
-
-    def __init__(self, by: chitose.app.bsky.actor.defs.ProfileViewBasic, indexed_at: str) -> None:
-        self.by = by
-        self.indexed_at = indexed_at
-
-    def to_dict(self):
-        return {'by': self.by, 'indexedAt': self.indexed_at}
-
-class ThreadViewPost(chitose.Object):
-
-    def __init__(self, post: PostView, parent: typing.Optional[typing.Union[ThreadViewPost, NotFoundPost, BlockedPost]]=None, replies: typing.Optional[list[typing.Union[ThreadViewPost, NotFoundPost, BlockedPost]]]=None) -> None:
-        self.post = post
-        self.parent = parent
-        self.replies = replies
-
-    def to_dict(self):
-        return {'post': self.post, 'parent': self.parent, 'replies': self.replies}
-
-class NotFoundPost(chitose.Object):
+class Entity(chitose.Object):
 
-    def __init__(self, uri: str, not_found: str) -> None:
-        self.uri = uri
-        self.not_found = not_found
+    def __init__(self, index: chitose.app.bsky.feed.post.TextSlice, type: str, value: str) -> None:
+        self.index = index
+        self.type = type
+        self.value = value
 
     def to_dict(self):
-        return {'uri': self.uri, 'notFound': self.not_found}
+        return {'index': self.index, 'type': self.type, 'value': self.value}
 
-class BlockedPost(chitose.Object):
+class TextSlice(chitose.Object):
 
-    def __init__(self, uri: str, blocked: str) -> None:
-        self.uri = uri
-        self.blocked = blocked
+    def __init__(self, start: int, end: int) -> None:
+        self.start = start
+        self.end = end
 
     def to_dict(self):
-        return {'uri': self.uri, 'blocked': self.blocked}
+        return {'start': self.start, 'end': self.end}
```

### Comparing `chitose-0.0.1/chitose/app/bsky/feed/get_likes.py` & `chitose-0.0.2/chitose/app/bsky/feed/get_likes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.actor.defs
 import typing
 
-def get_likes(service: str, headers: dict[str, str], uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+def _get_likes(service: str, headers: dict[str, str], uri: str, cid: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
     """"""
     return chitose.xrpc.call('app.bsky.feed.getLikes', [('uri', uri), ('cid', cid), ('limit', limit), ('cursor', cursor)], None, service, {} | headers)
 
 class Like(chitose.Object):
 
     def __init__(self, indexed_at: str, created_at: str, actor: chitose.app.bsky.actor.defs.ProfileView) -> None:
         self.indexed_at = indexed_at
```

### Comparing `chitose-0.0.1/chitose/app/bsky/notification/__init__.py` & `chitose-0.0.2/chitose/app/bsky/unspecced/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from .get_unread_count import *
-from .list_notifications import *
-from .update_seen import *
+from .get_popular import _get_popular
+import typing
 
-class Notification:
+class Unspecced_:
 
     def __init__(self, service: str, headers: dict[str, str]):
         self.service = service
         self.headers = headers
 
-    def update_seen(self, seen_at: str):
-        return update_seen(self.service, self.headers, seen_at)
-
-    def list_notifications(self, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, seen_at: typing.Optional[str]=None):
-        return list_notifications(self.service, self.headers, limit, cursor, seen_at)
-
-    def get_unread_count(self, seen_at: typing.Optional[str]=None):
-        return get_unread_count(self.service, self.headers, seen_at)
+    def get_popular(self, include_nsfw: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+        """An unspecced view of globally popular items"""
+        return _get_popular(self.service, self.headers, include_nsfw, limit, cursor)
```

### Comparing `chitose-0.0.1/chitose/app/bsky/notification/list_notifications.py` & `chitose-0.0.2/chitose/app/bsky/notification/list_notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.actor.defs
 import chitose.com.atproto.label.defs
 import typing
 
-def list_notifications(service: str, headers: dict[str, str], limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, seen_at: typing.Optional[str]=None):
+def _list_notifications(service: str, headers: dict[str, str], limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, seen_at: typing.Optional[str]=None):
     """"""
     return chitose.xrpc.call('app.bsky.notification.listNotifications', [('limit', limit), ('cursor', cursor), ('seenAt', seen_at)], None, service, {} | headers)
 
 class Notification(chitose.Object):
 
     def __init__(self, uri: str, cid: str, author: chitose.app.bsky.actor.defs.ProfileView, reason: str, record: typing.Any, is_read: str, indexed_at: str, reason_subject: typing.Optional[str]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.uri = uri
```

### Comparing `chitose-0.0.1/chitose/app/bsky/richtext/facet.py` & `chitose-0.0.2/chitose/app/bsky/richtext/facet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
+import chitose.app.bsky.richtext.facet
 import typing
 
 class Facet(chitose.Object):
 
-    def __init__(self, index: ByteSlice, features: list[typing.Union[Mention, Link]]) -> None:
+    def __init__(self, index: chitose.app.bsky.richtext.facet.ByteSlice, features: list[typing.Union[chitose.app.bsky.richtext.facet.Mention, chitose.app.bsky.richtext.facet.Link]]) -> None:
         self.index = index
         self.features = features
 
     def to_dict(self):
         return {'index': self.index, 'features': self.features}
 
 class Mention(chitose.Object):
```

### Comparing `chitose-0.0.1/chitose/com/atproto/__init__.py` & `chitose-0.0.2/chitose/com/atproto/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from .admin import Admin
-from .identity import Identity
-from .label import Label
-from .moderation import Moderation
-from .repo import Repo
-from .server import Server
-from .sync import Sync
+from .admin import Admin_
+from .identity import Identity_
+from .label import Label_
+from .moderation import Moderation_
+from .repo import Repo_
+from .server import Server_
+from .sync import Sync_
 
-class Atproto:
+class Atproto_:
 
     def __init__(self, service: str, headers: dict[str, str]):
         self.service = service
         self.headers = headers
 
     @property
     def admin(self):
-        return Admin(self.service, self.headers)
+        return Admin_(self.service, self.headers)
 
     @property
     def identity(self):
-        return Identity(self.service, self.headers)
+        return Identity_(self.service, self.headers)
 
     @property
     def label(self):
-        return Label(self.service, self.headers)
+        return Label_(self.service, self.headers)
 
     @property
     def moderation(self):
-        return Moderation(self.service, self.headers)
+        return Moderation_(self.service, self.headers)
 
     @property
     def repo(self):
-        return Repo(self.service, self.headers)
+        return Repo_(self.service, self.headers)
 
     @property
     def server(self):
-        return Server(self.service, self.headers)
+        return Server_(self.service, self.headers)
 
     @property
     def sync(self):
-        return Sync(self.service, self.headers)
+        return Sync_(self.service, self.headers)
```

### Comparing `chitose-0.0.1/chitose/com/atproto/admin/defs.py` & `chitose-0.0.2/chitose/com/atproto/admin/defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
+import chitose.com.atproto.admin.defs
 import chitose.com.atproto.label.defs
 import chitose.com.atproto.moderation.defs
-import chitose.com.atproto.repo
+import chitose.com.atproto.repo.strong_ref
 import chitose.com.atproto.server.defs
 import enum
 import typing
 
 class ActionView(chitose.Object):
 
-    def __init__(self, id: int, action: ActionType, subject: typing.Union[RepoRef, chitose.com.atproto.repo.StrongRef], subject_blob_cids: list[str], reason: str, created_by: str, created_at: str, resolved_report_ids: list[int], create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None, reversal: typing.Optional[ActionReversal]=None) -> None:
+    def __init__(self, id: int, action: chitose.com.atproto.admin.defs.ActionType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], subject_blob_cids: list[str], reason: str, created_by: str, created_at: str, resolved_report_ids: list[int], create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None, reversal: typing.Optional[chitose.com.atproto.admin.defs.ActionReversal]=None) -> None:
         self.id = id
         self.action = action
         self.subject = subject
         self.subject_blob_cids = subject_blob_cids
         self.reason = reason
         self.created_by = created_by
         self.created_at = created_at
@@ -24,15 +25,15 @@
         self.reversal = reversal
 
     def to_dict(self):
         return {'id': self.id, 'action': self.action, 'subject': self.subject, 'subjectBlobCids': self.subject_blob_cids, 'reason': self.reason, 'createdBy': self.created_by, 'createdAt': self.created_at, 'resolvedReportIds': self.resolved_report_ids, 'createLabelVals': self.create_label_vals, 'negateLabelVals': self.negate_label_vals, 'reversal': self.reversal}
 
 class ActionViewDetail(chitose.Object):
 
-    def __init__(self, id: int, action: ActionType, subject: typing.Union[RepoView, RecordView], subject_blobs: list[BlobView], reason: str, created_by: str, created_at: str, resolved_reports: list[ReportView], create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None, reversal: typing.Optional[ActionReversal]=None) -> None:
+    def __init__(self, id: int, action: chitose.com.atproto.admin.defs.ActionType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoView, chitose.com.atproto.admin.defs.RecordView], subject_blobs: list[chitose.com.atproto.admin.defs.BlobView], reason: str, created_by: str, created_at: str, resolved_reports: list[chitose.com.atproto.admin.defs.ReportView], create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None, reversal: typing.Optional[chitose.com.atproto.admin.defs.ActionReversal]=None) -> None:
         self.id = id
         self.action = action
         self.subject = subject
         self.subject_blobs = subject_blobs
         self.reason = reason
         self.created_by = created_by
         self.created_at = created_at
@@ -42,15 +43,15 @@
         self.reversal = reversal
 
     def to_dict(self):
         return {'id': self.id, 'action': self.action, 'subject': self.subject, 'subjectBlobs': self.subject_blobs, 'reason': self.reason, 'createdBy': self.created_by, 'createdAt': self.created_at, 'resolvedReports': self.resolved_reports, 'createLabelVals': self.create_label_vals, 'negateLabelVals': self.negate_label_vals, 'reversal': self.reversal}
 
 class ActionViewCurrent(chitose.Object):
 
-    def __init__(self, id: int, action: ActionType) -> None:
+    def __init__(self, id: int, action: chitose.com.atproto.admin.defs.ActionType) -> None:
         self.id = id
         self.action = action
 
     def to_dict(self):
         return {'id': self.id, 'action': self.action}
 
 class ActionReversal(chitose.Object):
@@ -63,63 +64,65 @@
     def to_dict(self):
         return {'reason': self.reason, 'createdBy': self.created_by, 'createdAt': self.created_at}
 
 class ActionType(enum.Enum):
     TAKEDOWN = '#takedown'
     FLAG = '#flag'
     ACKNOWLEDGE = '#acknowledge'
+    ESCALATE = '#escalate'
 TAKEDOWN = 'com.atproto.admin.defs#takedown'
 FLAG = 'com.atproto.admin.defs#flag'
 ACKNOWLEDGE = 'com.atproto.admin.defs#acknowledge'
+ESCALATE = 'com.atproto.admin.defs#escalate'
 
 class ReportView(chitose.Object):
 
-    def __init__(self, id: int, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[RepoRef, chitose.com.atproto.repo.StrongRef], reported_by: str, created_at: str, resolved_by_action_ids: list[int], reason: typing.Optional[str]=None) -> None:
+    def __init__(self, id: int, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reported_by: str, created_at: str, resolved_by_action_ids: list[int], reason: typing.Optional[str]=None) -> None:
         self.id = id
         self.reason_type = reason_type
         self.subject = subject
         self.reported_by = reported_by
         self.created_at = created_at
         self.resolved_by_action_ids = resolved_by_action_ids
         self.reason = reason
 
     def to_dict(self):
         return {'id': self.id, 'reasonType': self.reason_type, 'subject': self.subject, 'reportedBy': self.reported_by, 'createdAt': self.created_at, 'resolvedByActionIds': self.resolved_by_action_ids, 'reason': self.reason}
 
 class ReportViewDetail(chitose.Object):
 
-    def __init__(self, id: int, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[RepoView, RecordView], reported_by: str, created_at: str, resolved_by_actions: list[ActionView], reason: typing.Optional[str]=None) -> None:
+    def __init__(self, id: int, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoView, chitose.com.atproto.admin.defs.RecordView], reported_by: str, created_at: str, resolved_by_actions: list[chitose.com.atproto.admin.defs.ActionView], reason: typing.Optional[str]=None) -> None:
         self.id = id
         self.reason_type = reason_type
         self.subject = subject
         self.reported_by = reported_by
         self.created_at = created_at
         self.resolved_by_actions = resolved_by_actions
         self.reason = reason
 
     def to_dict(self):
         return {'id': self.id, 'reasonType': self.reason_type, 'subject': self.subject, 'reportedBy': self.reported_by, 'createdAt': self.created_at, 'resolvedByActions': self.resolved_by_actions, 'reason': self.reason}
 
 class RepoView(chitose.Object):
 
-    def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: Moderation, email: typing.Optional[str]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None) -> None:
+    def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: chitose.com.atproto.admin.defs.Moderation, email: typing.Optional[str]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None) -> None:
         self.did = did
         self.handle = handle
         self.related_records = related_records
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.email = email
         self.invited_by = invited_by
 
     def to_dict(self):
         return {'did': self.did, 'handle': self.handle, 'relatedRecords': self.related_records, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'email': self.email, 'invitedBy': self.invited_by}
 
 class RepoViewDetail(chitose.Object):
 
-    def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: ModerationDetail, email: typing.Optional[str]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None, invites: typing.Optional[list[chitose.com.atproto.server.defs.InviteCode]]=None) -> None:
+    def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: chitose.com.atproto.admin.defs.ModerationDetail, email: typing.Optional[str]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None, invites: typing.Optional[list[chitose.com.atproto.server.defs.InviteCode]]=None) -> None:
         self.did = did
         self.handle = handle
         self.related_records = related_records
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.email = email
         self.labels = labels
@@ -135,62 +138,62 @@
         self.did = did
 
     def to_dict(self):
         return {'did': self.did}
 
 class RecordView(chitose.Object):
 
-    def __init__(self, uri: str, cid: str, value: typing.Any, blob_cids: list[str], indexed_at: str, moderation: Moderation, repo: RepoView) -> None:
+    def __init__(self, uri: str, cid: str, value: typing.Any, blob_cids: list[str], indexed_at: str, moderation: chitose.com.atproto.admin.defs.Moderation, repo: chitose.com.atproto.admin.defs.RepoView) -> None:
         self.uri = uri
         self.cid = cid
         self.value = value
         self.blob_cids = blob_cids
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.repo = repo
 
     def to_dict(self):
         return {'uri': self.uri, 'cid': self.cid, 'value': self.value, 'blobCids': self.blob_cids, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'repo': self.repo}
 
 class RecordViewDetail(chitose.Object):
 
-    def __init__(self, uri: str, cid: str, value: typing.Any, blobs: list[BlobView], indexed_at: str, moderation: ModerationDetail, repo: RepoView, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
+    def __init__(self, uri: str, cid: str, value: typing.Any, blobs: list[chitose.com.atproto.admin.defs.BlobView], indexed_at: str, moderation: chitose.com.atproto.admin.defs.ModerationDetail, repo: chitose.com.atproto.admin.defs.RepoView, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.uri = uri
         self.cid = cid
         self.value = value
         self.blobs = blobs
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.repo = repo
         self.labels = labels
 
     def to_dict(self):
         return {'uri': self.uri, 'cid': self.cid, 'value': self.value, 'blobs': self.blobs, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'repo': self.repo, 'labels': self.labels}
 
 class Moderation(chitose.Object):
 
-    def __init__(self, current_action: typing.Optional[ActionViewCurrent]=None) -> None:
+    def __init__(self, current_action: typing.Optional[chitose.com.atproto.admin.defs.ActionViewCurrent]=None) -> None:
         self.current_action = current_action
 
     def to_dict(self):
         return {'currentAction': self.current_action}
 
 class ModerationDetail(chitose.Object):
 
-    def __init__(self, actions: list[ActionView], reports: list[ReportView], current_action: typing.Optional[ActionViewCurrent]=None) -> None:
+    def __init__(self, actions: list[chitose.com.atproto.admin.defs.ActionView], reports: list[chitose.com.atproto.admin.defs.ReportView], current_action: typing.Optional[chitose.com.atproto.admin.defs.ActionViewCurrent]=None) -> None:
         self.actions = actions
         self.reports = reports
         self.current_action = current_action
 
     def to_dict(self):
         return {'actions': self.actions, 'reports': self.reports, 'currentAction': self.current_action}
 
 class BlobView(chitose.Object):
 
-    def __init__(self, cid: str, mime_type: str, size: int, created_at: str, details: typing.Optional[typing.Union[ImageDetails, VideoDetails]]=None, moderation: typing.Optional[Moderation]=None) -> None:
+    def __init__(self, cid: str, mime_type: str, size: int, created_at: str, details: typing.Optional[typing.Union[chitose.com.atproto.admin.defs.ImageDetails, chitose.com.atproto.admin.defs.VideoDetails]]=None, moderation: typing.Optional[chitose.com.atproto.admin.defs.Moderation]=None) -> None:
         self.cid = cid
         self.mime_type = mime_type
         self.size = size
         self.created_at = created_at
         self.details = details
         self.moderation = moderation
```

### Comparing `chitose-0.0.1/chitose/com/atproto/admin/get_moderation_reports.py` & `chitose-0.0.2/chitose/com/atproto/admin/get_moderation_reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import typing
 
-def get_moderation_reports(service: str, headers: dict[str, str], subject: typing.Optional[str]=None, resolved: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+def _get_moderation_reports(service: str, headers: dict[str, str], subject: typing.Optional[str]=None, resolved: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
     """List moderation reports related to a subject."""
     return chitose.xrpc.call('com.atproto.admin.getModerationReports', [('subject', subject), ('resolved', resolved), ('limit', limit), ('cursor', cursor)], None, service, {} | headers)
```

### Comparing `chitose-0.0.1/chitose/com/atproto/admin/search_repos.py` & `chitose-0.0.2/chitose/com/atproto/admin/search_repos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import typing
 
-def search_repos(service: str, headers: dict[str, str], term: typing.Optional[str]=None, invited_by: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+def _search_repos(service: str, headers: dict[str, str], term: typing.Optional[str]=None, invited_by: typing.Optional[str]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
     """Find repositories based on a search term."""
     return chitose.xrpc.call('com.atproto.admin.searchRepos', [('term', term), ('invitedBy', invited_by), ('limit', limit), ('cursor', cursor)], None, service, {} | headers)
```

### Comparing `chitose-0.0.1/chitose/com/atproto/admin/take_moderation_action.py` & `chitose-0.0.2/chitose/com/atproto/admin/take_moderation_action.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.admin.defs
-import chitose.com.atproto.repo
+import chitose.com.atproto.repo.strong_ref
 import typing
 
-def take_moderation_action(service: str, headers: dict[str, str], action: str, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None):
+def _take_moderation_action(service: str, headers: dict[str, str], action: str, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None):
     """Take a moderation action on a repo."""
     return chitose.xrpc.call('com.atproto.admin.takeModerationAction', [], {'action': action, 'subject': subject, 'subjectBlobCids': subject_blob_cids, 'createLabelVals': create_label_vals, 'negateLabelVals': negate_label_vals, 'reason': reason, 'createdBy': created_by}, service, {'Content-Type': 'application/json'} | headers)
```

### Comparing `chitose-0.0.1/chitose/com/atproto/label/defs.py` & `chitose-0.0.2/chitose/com/atproto/label/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/chitose/com/atproto/label/query_labels.py` & `chitose-0.0.2/chitose/com/atproto/label/query_labels.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import typing
 
-def query_labels(service: str, headers: dict[str, str], uri_patterns: list[str], sources: typing.Optional[list[str]]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
-    """Find labels relevant to the provided URI patterns."""
+def _query_labels(service: str, headers: dict[str, str], uri_patterns: list[str], sources: typing.Optional[list[str]]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+    """Find labels relevant to the provided URI patterns.
+
+
+    :param uri_patterns: List of AT URI patterns to match (boolean 'OR'). Each may be a prefix (ending with '*'; will match inclusive of the string leading to '*'), or a full URI
+
+    :param sources: Optional list of label sources (DIDs) to filter on
+    """
     return chitose.xrpc.call('com.atproto.label.queryLabels', [('uriPatterns', uri_patterns), ('sources', sources), ('limit', limit), ('cursor', cursor)], None, service, {} | headers)
```

### Comparing `chitose-0.0.1/chitose/com/atproto/label/subscribe_labels.py` & `chitose-0.0.2/chitose/com/atproto/label/subscribe_labels.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/chitose/com/atproto/moderation/__init__.py` & `chitose-0.0.2/chitose/com/atproto/moderation/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
-from .create_report import *
-from .defs import *
+from .create_report import _create_report
+import chitose
+import typing
 
-class Moderation:
+class Moderation_:
 
     def __init__(self, service: str, headers: dict[str, str]):
         self.service = service
         self.headers = headers
 
-    def create_report(self, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.StrongRef], reason: typing.Optional[str]=None):
-        return create_report(self.service, self.headers, reason_type, subject, reason)
+    def create_report(self, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: typing.Optional[str]=None):
+        """Report a repo or a record."""
+        return _create_report(self.service, self.headers, reason_type, subject, reason)
```

### Comparing `chitose-0.0.1/chitose/com/atproto/moderation/create_report.py` & `chitose-0.0.2/chitose/com/atproto/moderation/create_report.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.admin.defs
 import chitose.com.atproto.moderation.defs
-import chitose.com.atproto.repo
+import chitose.com.atproto.repo.strong_ref
 import typing
 
-def create_report(service: str, headers: dict[str, str], reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.StrongRef], reason: typing.Optional[str]=None):
+def _create_report(service: str, headers: dict[str, str], reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: typing.Optional[str]=None):
     """Report a repo or a record."""
     return chitose.xrpc.call('com.atproto.moderation.createReport', [], {'reasonType': reason_type, 'reason': reason, 'subject': subject}, service, {'Content-Type': 'application/json'} | headers)
```

### Comparing `chitose-0.0.1/chitose/com/atproto/moderation/defs.py` & `chitose-0.0.2/chitose/com/atproto/moderation/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/chitose/com/atproto/repo/apply_writes.py` & `chitose-0.0.2/chitose/com/atproto/repo/apply_writes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
+import chitose.com.atproto.repo.apply_writes
 import typing
 
-def apply_writes(service: str, headers: dict[str, str], repo: str, writes: list[typing.Union[Create, Update, Delete]], validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None):
-    """Apply a batch transaction of creates, updates, and deletes."""
+def _apply_writes(service: str, headers: dict[str, str], repo: str, writes: list[typing.Union[chitose.com.atproto.repo.apply_writes.Create, chitose.com.atproto.repo.apply_writes.Update, chitose.com.atproto.repo.apply_writes.Delete]], validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None):
+    """Apply a batch transaction of creates, updates, and deletes.
+
+
+    :param repo: The handle or DID of the repo.
+
+    :param validate: Validate the records?
+    """
     return chitose.xrpc.call('com.atproto.repo.applyWrites', [], {'repo': repo, 'validate': validate, 'writes': writes, 'swapCommit': swap_commit}, service, {'Content-Type': 'application/json'} | headers)
 
 class Create(chitose.Object):
 
     def __init__(self, collection: str, value: typing.Any, rkey: typing.Optional[str]) -> None:
         self.collection = collection
         self.value = value
```

### Comparing `chitose-0.0.1/chitose/com/atproto/repo/delete_record.py` & `chitose-0.0.2/chitose/com/atproto/repo/create_record.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,22 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import typing
 
-def delete_record(service: str, headers: dict[str, str], repo: str, collection: str, rkey: str, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None):
-    """Delete a record, or ensure it doesn't exist."""
-    return chitose.xrpc.call('com.atproto.repo.deleteRecord', [], {'repo': repo, 'collection': collection, 'rkey': rkey, 'swapRecord': swap_record, 'swapCommit': swap_commit}, service, {'Content-Type': 'application/json'} | headers)
+def _create_record(service: str, headers: dict[str, str], repo: str, collection: str, record: typing.Any, rkey: typing.Optional[str]=None, validate: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None):
+    """Create a new record.
+
+
+    :param repo: The handle or DID of the repo.
+
+    :param collection: The NSID of the record collection.
+
+    :param record: The record to create.
+
+    :param rkey: The key of the record.
+
+    :param validate: Validate the record?
+
+    :param swap_commit: Compare and swap with the previous commit by cid.
+    """
+    return chitose.xrpc.call('com.atproto.repo.createRecord', [], {'repo': repo, 'collection': collection, 'rkey': rkey, 'validate': validate, 'record': record, 'swapCommit': swap_commit}, service, {'Content-Type': 'application/json'} | headers)
```

### Comparing `chitose-0.0.1/chitose/com/atproto/repo/list_records.py` & `chitose-0.0.2/chitose/com/atproto/repo/list_records.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import typing
 
-def list_records(service: str, headers: dict[str, str], repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[str]=None):
-    """List a range of records in a collection."""
+def _list_records(service: str, headers: dict[str, str], repo: str, collection: str, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, rkey_start: typing.Optional[str]=None, rkey_end: typing.Optional[str]=None, reverse: typing.Optional[str]=None):
+    """List a range of records in a collection.
+
+
+    :param repo: The handle or DID of the repo.
+
+    :param collection: The NSID of the record type.
+
+    :param limit: The number of records to return.
+
+    :param rkey_start: DEPRECATED: The lowest sort-ordered rkey to start from (exclusive)
+
+    :param rkey_end: DEPRECATED: The highest sort-ordered rkey to stop at (exclusive)
+
+    :param reverse: Reverse the order of the returned records?
+    """
     return chitose.xrpc.call('com.atproto.repo.listRecords', [('repo', repo), ('collection', collection), ('limit', limit), ('cursor', cursor), ('rkeyStart', rkey_start), ('rkeyEnd', rkey_end), ('reverse', reverse)], None, service, {} | headers)
 
 class Record(chitose.Object):
 
     def __init__(self, uri: str, cid: str, value: typing.Any) -> None:
         self.uri = uri
         self.cid = cid
```

### Comparing `chitose-0.0.1/chitose/com/atproto/repo/put_record.py` & `chitose-0.0.2/chitose/com/atproto/repo/delete_record.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,20 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import typing
 
-def put_record(service: str, headers: dict[str, str], repo: str, collection: str, rkey: str, record: typing.Any, validate: typing.Optional[str]=None, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None):
-    """Write a record, creating or updating it as needed."""
-    return chitose.xrpc.call('com.atproto.repo.putRecord', [], {'repo': repo, 'collection': collection, 'rkey': rkey, 'validate': validate, 'record': record, 'swapRecord': swap_record, 'swapCommit': swap_commit}, service, {'Content-Type': 'application/json'} | headers)
+def _delete_record(service: str, headers: dict[str, str], repo: str, collection: str, rkey: str, swap_record: typing.Optional[str]=None, swap_commit: typing.Optional[str]=None):
+    """Delete a record, or ensure it doesn't exist.
+
+
+    :param repo: The handle or DID of the repo.
+
+    :param collection: The NSID of the record collection.
+
+    :param rkey: The key of the record.
+
+    :param swap_record: Compare and swap with the previous record by cid.
+
+    :param swap_commit: Compare and swap with the previous commit by cid.
+    """
+    return chitose.xrpc.call('com.atproto.repo.deleteRecord', [], {'repo': repo, 'collection': collection, 'rkey': rkey, 'swapRecord': swap_record, 'swapCommit': swap_commit}, service, {'Content-Type': 'application/json'} | headers)
```

### Comparing `chitose-0.0.1/chitose/com/atproto/server/create_account.py` & `chitose-0.0.2/chitose/com/atproto/server/create_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import typing
 
-def create_account(service: str, headers: dict[str, str], email: str, handle: str, password: str, invite_code: typing.Optional[str]=None, recovery_key: typing.Optional[str]=None):
+def _create_account(service: str, headers: dict[str, str], email: str, handle: str, password: str, invite_code: typing.Optional[str]=None, recovery_key: typing.Optional[str]=None):
     """Create an account."""
     return chitose.xrpc.call('com.atproto.server.createAccount', [], {'email': email, 'handle': handle, 'inviteCode': invite_code, 'password': password, 'recoveryKey': recovery_key}, service, {'Content-Type': 'application/json'} | headers)
```

### Comparing `chitose-0.0.1/chitose/com/atproto/server/create_app_password.py` & `chitose-0.0.2/chitose/com/atproto/server/create_app_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 
-def create_app_password(service: str, headers: dict[str, str], name: str):
+def _create_app_password(service: str, headers: dict[str, str], name: str):
     """Create an app-specific password."""
     return chitose.xrpc.call('com.atproto.server.createAppPassword', [], {'name': name}, service, {'Content-Type': 'application/json'} | headers)
 
 class AppPassword(chitose.Object):
 
     def __init__(self, name: str, password: str, created_at: str) -> None:
         self.name = name
```

### Comparing `chitose-0.0.1/chitose/com/atproto/server/create_invite_codes.py` & `chitose-0.0.2/chitose/com/atproto/server/create_invite_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import typing
 
-def create_invite_codes(service: str, headers: dict[str, str], code_count: int, use_count: int, for_accounts: typing.Optional[list[str]]=None):
+def _create_invite_codes(service: str, headers: dict[str, str], code_count: int, use_count: int, for_accounts: typing.Optional[list[str]]=None):
     """Create an invite code."""
     return chitose.xrpc.call('com.atproto.server.createInviteCodes', [], {'codeCount': code_count, 'useCount': use_count, 'forAccounts': for_accounts}, service, {'Content-Type': 'application/json'} | headers)
 
 class AccountCodes(chitose.Object):
 
     def __init__(self, account: str, codes: list[str]) -> None:
         self.account = account
```

### Comparing `chitose-0.0.1/chitose/com/atproto/server/defs.py` & `chitose-0.0.2/chitose/com/atproto/server/defs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
+import chitose.com.atproto.server.defs
 
 class InviteCode(chitose.Object):
 
-    def __init__(self, code: str, available: int, disabled: str, for_account: str, created_by: str, created_at: str, uses: list[InviteCodeUse]) -> None:
+    def __init__(self, code: str, available: int, disabled: str, for_account: str, created_by: str, created_at: str, uses: list[chitose.com.atproto.server.defs.InviteCodeUse]) -> None:
         self.code = code
         self.available = available
         self.disabled = disabled
         self.for_account = for_account
         self.created_by = created_by
         self.created_at = created_at
         self.uses = uses
```

### Comparing `chitose-0.0.1/chitose/com/atproto/server/describe_server.py` & `chitose-0.0.2/chitose/com/atproto/server/describe_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import typing
 
-def describe_server(service: str, headers: dict[str, str]):
+def _describe_server(service: str, headers: dict[str, str]):
     """Get a document describing the service's accounts configuration."""
     return chitose.xrpc.call('com.atproto.server.describeServer', [], None, service, {} | headers)
 
 class Links(chitose.Object):
 
     def __init__(self, privacy_policy: typing.Optional[str]=None, terms_of_service: typing.Optional[str]=None) -> None:
         self.privacy_policy = privacy_policy
```

### Comparing `chitose-0.0.1/chitose/com/atproto/server/list_app_passwords.py` & `chitose-0.0.2/chitose/com/atproto/server/list_app_passwords.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 
-def list_app_passwords(service: str, headers: dict[str, str]):
+def _list_app_passwords(service: str, headers: dict[str, str]):
     """List all app-specific passwords."""
     return chitose.xrpc.call('com.atproto.server.listAppPasswords', [], None, service, {} | headers)
 
 class AppPassword(chitose.Object):
 
     def __init__(self, name: str, created_at: str) -> None:
         self.name = name
```

### Comparing `chitose-0.0.1/chitose/com/atproto/sync/list_repos.py` & `chitose-0.0.2/chitose/com/atproto/sync/list_repos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
 import typing
 
-def list_repos(service: str, headers: dict[str, str], limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
+def _list_repos(service: str, headers: dict[str, str], limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None):
     """List dids and root cids of hosted repos"""
     return chitose.xrpc.call('com.atproto.sync.listRepos', [('limit', limit), ('cursor', cursor)], None, service, {} | headers)
 
 class Repo(chitose.Object):
 
     def __init__(self, did: str, head: str) -> None:
         self.did = did
```

### Comparing `chitose-0.0.1/chitose/com/atproto/sync/subscribe_repos.py` & `chitose-0.0.2/chitose/com/atproto/sync/subscribe_repos.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 import chitose
+import chitose.com.atproto.sync.subscribe_repos
 import typing
 
 class Commit(chitose.Object):
 
-    def __init__(self, seq: int, rebase: str, too_big: str, repo: str, commit: typing.Any, prev: typing.Any, blocks: typing.Any, ops: list[RepoOp], blobs: list[typing.Any], time: str) -> None:
+    def __init__(self, seq: int, rebase: str, too_big: str, repo: str, commit: typing.Any, prev: typing.Any, blocks: typing.Any, ops: list[chitose.com.atproto.sync.subscribe_repos.RepoOp], blobs: list[typing.Any], time: str) -> None:
         self.seq = seq
         self.rebase = rebase
         self.too_big = too_big
         self.repo = repo
         self.commit = commit
         self.prev = prev
         self.blocks = blocks
```

### Comparing `chitose-0.0.1/docs/Makefile` & `chitose-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/make.bat` & `chitose-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/source/chitose.app.bsky.actor.rst` & `chitose-0.0.2/docs/source/chitose.app.bsky.actor.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/source/chitose.app.bsky.embed.rst` & `chitose-0.0.2/docs/source/chitose.app.bsky.embed.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/source/chitose.app.bsky.feed.rst` & `chitose-0.0.2/docs/source/chitose.app.bsky.feed.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/source/chitose.app.bsky.graph.rst` & `chitose-0.0.2/docs/source/chitose.app.bsky.graph.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/source/chitose.app.bsky.notification.rst` & `chitose-0.0.2/docs/source/chitose.app.bsky.notification.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/source/chitose.com.atproto.admin.rst` & `chitose-0.0.2/docs/source/chitose.com.atproto.admin.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/source/chitose.com.atproto.identity.rst` & `chitose-0.0.2/docs/source/chitose.com.atproto.identity.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/source/chitose.com.atproto.label.rst` & `chitose-0.0.2/docs/source/chitose.com.atproto.label.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/source/chitose.com.atproto.moderation.rst` & `chitose-0.0.2/docs/source/chitose.com.atproto.moderation.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/source/chitose.com.atproto.repo.rst` & `chitose-0.0.2/docs/source/chitose.com.atproto.repo.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/source/chitose.com.atproto.server.rst` & `chitose-0.0.2/docs/source/chitose.com.atproto.server.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/source/chitose.com.atproto.sync.rst` & `chitose-0.0.2/docs/source/chitose.com.atproto.sync.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/source/chitose.rst` & `chitose-0.0.2/docs/source/chitose.rst`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/docs/source/conf.py` & `chitose-0.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/.gitignore` & `chitose-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/LICENSE` & `chitose-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chitose-0.0.1/README.md` & `chitose-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,59 @@
 # Chitose
 
-Chitose is a client library for the AT Protocol.
+Chitose is a Python client library for the AT Protocol.
 
 ## Usage
 
-Replace `YOUR_USERNAME` and `YOUR_PASSWORD` with your username and your password respectively:
+The API of Chitose is similar to [the ATP API](https://github.com/bluesky-social/atproto/tree/main/packages/api#advanced-api-calls).
 
+For example, you can use `app.bsky.feed.get_timeline()` to get the timeline as shown below. Replace `YOUR_USERNAME` and `YOUR_PASSWORD` with your username and your password respectively:
 ```
 $ git clone https://github.com/mnogu/chitose.git
 $ cd chitose
 $ python3
 >>> from chitose.agent import BskyAgent
 >>> agent = BskyAgent(service='https://bsky.social')
 >>> agent.login(identifier='YOUR_USERNAME', password='YOUR_PASSWORD')
 >>> agent.app.bsky.feed.get_timeline(limit=1)
 ```
 
+You can also post with `com.atproto.repo.create_record()`:
 ```python
 from datetime import datetime
 from chitose.agent import BskyAgent
-from chitose.app.bsky.feed import Post
+from chitose.app.bsky.feed.post import Post
 
 agent = BskyAgent(service='https://example.com')
 agent.login(identifier='alice@mail.com', password='hunter2')
 
 record = Post(text='Hello, world!', created_at=datetime.now().isoformat())
 agent.com.atproto.repo.create_record(
     repo=alice.did, collection='app.bsky.feed.post', record=record)
 ```
 
 ## Documentation
 
-[Chitose’s documentation](https://chitose.readthedocs.io/en/latest/)
+For all the functions and classes available in Chitose, refer to [the Chitose’s documentation](https://chitose.readthedocs.io/en/latest/).
+
+## Installing
+
+While you can use Chitose without installing its Python package, you can install [the package](https://pypi.org/project/chitose/):
+```
+$ python3 -m pip install chitose
+```
+
+Alternatively, you can build a Python package and install it:
+```
+$ git clone https://github.com/mnogu/chitose.git
+$ cd chitose
+$ python3 -m pip install --upgrade build
+$ python3 -m build
+$ python3 -m pip install dist/chitose-*-py3-none-any.whl
+```
 
 ## Generating Code
 
 Most source files of Chitose are generated from the Lexicon files in the `atproto` directory, and you can generate Python code from these files by yourself:
 ```
 $ git clone https://github.com/mnogu/chitose.git
 $ cd chitose
@@ -50,11 +68,11 @@
 
 You may want to add new Python code to the repository or update the documentation:
 ```
 $ git add chitose
 $ git commit
 ```
 ```
-$ pip3 install sphinx
+$ python3 -m pip install sphinx
 $ cd docs
 $ sphinx-apidoc -o ./source ../chitose -f
 ```
```

### Comparing `chitose-0.0.1/pyproject.toml` & `chitose-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "chitose"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Muneyuki Noguchi", email="nogu.dev@gmail.com" },
 ]
 description = "A client library for the AT Protocol (Bluesky) "
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `chitose-0.0.1/PKG-INFO` & `chitose-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chitose
-Version: 0.0.1
+Version: 0.0.2
 Summary: A client library for the AT Protocol (Bluesky) 
 Project-URL: Homepage, https://github.com/mnogu/chitose
 Project-URL: Bug Tracker, https://github.com/mnogu/chitose/issues
 Author-email: Muneyuki Noguchi <nogu.dev@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -12,46 +12,64 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation :: Sphinx
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Chitose
 
-Chitose is a client library for the AT Protocol.
+Chitose is a Python client library for the AT Protocol.
 
 ## Usage
 
-Replace `YOUR_USERNAME` and `YOUR_PASSWORD` with your username and your password respectively:
+The API of Chitose is similar to [the ATP API](https://github.com/bluesky-social/atproto/tree/main/packages/api#advanced-api-calls).
 
+For example, you can use `app.bsky.feed.get_timeline()` to get the timeline as shown below. Replace `YOUR_USERNAME` and `YOUR_PASSWORD` with your username and your password respectively:
 ```
 $ git clone https://github.com/mnogu/chitose.git
 $ cd chitose
 $ python3
 >>> from chitose.agent import BskyAgent
 >>> agent = BskyAgent(service='https://bsky.social')
 >>> agent.login(identifier='YOUR_USERNAME', password='YOUR_PASSWORD')
 >>> agent.app.bsky.feed.get_timeline(limit=1)
 ```
 
+You can also post with `com.atproto.repo.create_record()`:
 ```python
 from datetime import datetime
 from chitose.agent import BskyAgent
-from chitose.app.bsky.feed import Post
+from chitose.app.bsky.feed.post import Post
 
 agent = BskyAgent(service='https://example.com')
 agent.login(identifier='alice@mail.com', password='hunter2')
 
 record = Post(text='Hello, world!', created_at=datetime.now().isoformat())
 agent.com.atproto.repo.create_record(
     repo=alice.did, collection='app.bsky.feed.post', record=record)
 ```
 
 ## Documentation
 
-[Chitose’s documentation](https://chitose.readthedocs.io/en/latest/)
+For all the functions and classes available in Chitose, refer to [the Chitose’s documentation](https://chitose.readthedocs.io/en/latest/).
+
+## Installing
+
+While you can use Chitose without installing its Python package, you can install [the package](https://pypi.org/project/chitose/):
+```
+$ python3 -m pip install chitose
+```
+
+Alternatively, you can build a Python package and install it:
+```
+$ git clone https://github.com/mnogu/chitose.git
+$ cd chitose
+$ python3 -m pip install --upgrade build
+$ python3 -m build
+$ python3 -m pip install dist/chitose-*-py3-none-any.whl
+```
 
 ## Generating Code
 
 Most source files of Chitose are generated from the Lexicon files in the `atproto` directory, and you can generate Python code from these files by yourself:
 ```
 $ git clone https://github.com/mnogu/chitose.git
 $ cd chitose
@@ -66,11 +84,11 @@
 
 You may want to add new Python code to the repository or update the documentation:
 ```
 $ git add chitose
 $ git commit
 ```
 ```
-$ pip3 install sphinx
+$ python3 -m pip install sphinx
 $ cd docs
 $ sphinx-apidoc -o ./source ../chitose -f
 ```
```

