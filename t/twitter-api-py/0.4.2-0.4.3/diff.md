# Comparing `tmp/twitter_api_py-0.4.2.tar.gz` & `tmp/twitter_api_py-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter_api_py-0.4.2.tar", max compression
+gzip compressed data, was "twitter_api_py-0.4.3.tar", max compression
```

## Comparing `twitter_api_py-0.4.2.tar` & `twitter_api_py-0.4.3.tar`

### file list

```diff
@@ -1,269 +1,269 @@
--rw-r--r--   0        0        0     1497 2023-05-03 13:16:42.851501 twitter_api_py-0.4.2/LICENSE
--rw-r--r--   0        0        0     2126 2023-05-03 13:16:42.851501 twitter_api_py-0.4.2/README.md
--rw-r--r--   0        0        0     1516 2023-05-05 12:06:22.383190 twitter_api_py-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      480 2023-05-05 00:14:01.094855 twitter_api_py-0.4.2/twitter_api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.4.2/twitter_api/client/oauth_flow/__init__.py
--rw-r--r--   0        0        0     1041 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py
--rw-r--r--   0        0        0      311 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth1_access_token_mock_client.py
--rw-r--r--   0        0        0     1388 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py
--rw-r--r--   0        0        0      306 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth1_authorization_mock_client.py
--rw-r--r--   0        0        0      808 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py
--rw-r--r--   0        0        0      315 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth1_request_token_mock_client.py
--rw-r--r--   0        0        0     1211 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py
--rw-r--r--   0        0        0      311 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth2_access_token_mock_client.py
--rw-r--r--   0        0        0      831 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py
--rw-r--r--   0        0        0      306 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth2_authorization_mock_client.py
--rw-r--r--   0        0        0        0 2023-04-09 09:46:11.283030 twitter_api_py-0.4.2/twitter_api/client/oauth_session/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/__init__.py
--rw-r--r--   0        0        0      365 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth1_access_token/__init__.py
--rw-r--r--   0        0        0     1140 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py
--rw-r--r--   0        0        0      451 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth1_authenticate/__init__.py
--rw-r--r--   0        0        0      793 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py
--rw-r--r--   0        0        0      433 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth1_authorize/__init__.py
--rw-r--r--   0        0        0      722 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py
--rw-r--r--   0        0        0      392 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth1_request_token/__init__.py
--rw-r--r--   0        0        0      798 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py
--rw-r--r--   0        0        0      501 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth2_authorize/__init__.py
--rw-r--r--   0        0        0      751 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py
--rw-r--r--   0        0        0      648 2023-05-03 13:16:42.861501 twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/session_resources.py
--rw-r--r--   0        0        0      376 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/v2_oauth2_token/__init__.py
--rw-r--r--   0        0        0     1596 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py
--rw-r--r--   0        0        0     1793 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py
--rw-r--r--   0        0        0     3885 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/oauth_session/twitter_oauth1_real_session.py
--rw-r--r--   0        0        0     1103 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/oauth_session/twitter_oauth1_session.py
--rw-r--r--   0        0        0     1561 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py
--rw-r--r--   0        0        0     3397 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/oauth_session/twitter_oauth2_real_session.py
--rw-r--r--   0        0        0      823 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/oauth_session/twitter_oauth2_session.py
--rw-r--r--   0        0        0        0 2023-04-01 17:37:10.337565 twitter_api_py-0.4.2/twitter_api/client/request/__init__.py
--rw-r--r--   0        0        0     1577 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/request/request_async_client.py
--rw-r--r--   0        0        0      236 2023-04-22 10:21:01.811509 twitter_api_py-0.4.2/twitter_api/client/request/request_async_mock_client.py
--rw-r--r--   0        0        0     5182 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/request/request_async_real_client.py
--rw-r--r--   0        0        0     1967 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/request/request_client.py
--rw-r--r--   0        0        0     3368 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/request/request_mock_client.py
--rw-r--r--   0        0        0     7235 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/request/request_real_client.py
--rw-r--r--   0        0        0    32304 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/twitter_api_async_client.py
--rw-r--r--   0        0        0    14518 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/twitter_api_async_mock_client.py
--rw-r--r--   0        0        0    14743 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/twitter_api_async_real_client.py
--rw-r--r--   0        0        0    32063 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/twitter_api_client.py
--rw-r--r--   0        0        0    26895 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/twitter_api_mock_client.py
--rw-r--r--   0        0        0    13583 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/client/twitter_api_real_client.py
--rw-r--r--   0        0        0    10636 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/error.py
--rw-r--r--   0        0        0        0 2023-04-02 08:29:19.122099 twitter_api_py-0.4.2/twitter_api/rate_limit/__init__.py
--rw-r--r--   0        0        0      603 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/rate_limit/manager/__init__.py
--rw-r--r--   0        0        0     2232 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/rate_limit/manager/dict_rate_limit_manager.py
--rw-r--r--   0        0        0      976 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py
--rw-r--r--   0        0        0        0 2023-04-23 01:25:28.771650 twitter_api_py-0.4.2/twitter_api/rate_limit/manager/handlers/__init__.py
--rw-r--r--   0        0        0     1022 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py
--rw-r--r--   0        0        0     3316 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py
--rw-r--r--   0        0        0      705 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py
--rw-r--r--   0        0        0     1232 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/rate_limit/manager/rate_limit_manager.py
--rw-r--r--   0        0        0     3303 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/rate_limit/rate_limit.py
--rw-r--r--   0        0        0      291 2023-05-02 14:52:07.203654 twitter_api_py-0.4.2/twitter_api/rate_limit/rate_limit_info.py
--rw-r--r--   0        0        0       91 2023-05-02 14:52:07.203654 twitter_api_py-0.4.2/twitter_api/rate_limit/rate_limit_target.py
--rw-r--r--   0        0        0      281 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/api_resources.py
--rw-r--r--   0        0        0      437 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/oauth2_invalidate_token/__init__.py
--rw-r--r--   0        0        0     2295 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py
--rw-r--r--   0        0        0      332 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/oauth2_token/__init__.py
--rw-r--r--   0        0        0     2187 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/oauth2_token/post_oauth2_token.py
--rw-r--r--   0        0        0      541 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversation_messages/__init__.py
--rw-r--r--   0        0        0     2316 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py
--rw-r--r--   0        0        0      441 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversations/__init__.py
--rw-r--r--   0        0        0     2164 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py
--rw-r--r--   0        0        0      673 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py
--rw-r--r--   0        0        0     8907 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py
--rw-r--r--   0        0        0      676 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py
--rw-r--r--   0        0        0     2390 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py
--rw-r--r--   0        0        0      429 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweet/__init__.py
--rw-r--r--   0        0        0     1438 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweet/delete_v2_tweet.py
--rw-r--r--   0        0        0     3088 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweet/get_v2_tweet.py
--rw-r--r--   0        0        0      458 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweet_retweeted_by/__init__.py
--rw-r--r--   0        0        0     6561 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py
--rw-r--r--   0        0        0      428 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweets/__init__.py
--rw-r--r--   0        0        0     2977 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweets/get_v2_tweets.py
--rw-r--r--   0        0        0     2926 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweets/post_v2_tweets.py
--rw-r--r--   0        0        0      438 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_all/__init__.py
--rw-r--r--   0        0        0     6032 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py
--rw-r--r--   0        0        0      471 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_recent/__init__.py
--rw-r--r--   0        0        0     6131 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py
--rw-r--r--   0        0        0      471 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_stream/__init__.py
--rw-r--r--   0        0        0     3615 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py
--rw-r--r--   0        0        0      770 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py
--rw-r--r--   0        0        0     2111 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py
--rw-r--r--   0        0        0     3096 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py
--rw-r--r--   0        0        0      275 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_user/__init__.py
--rw-r--r--   0        0        0     2780 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_user/get_v2_user.py
--rw-r--r--   0        0        0      371 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_user_followers/__init__.py
--rw-r--r--   0        0        0     6510 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_user_followers/get_v2_user_followers.py
--rw-r--r--   0        0        0      376 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_user_following/__init__.py
--rw-r--r--   0        0        0     1909 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_user_following/post_v2_user_following.py
--rw-r--r--   0        0        0      391 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_user_liked_tweets/__init__.py
--rw-r--r--   0        0        0     7931 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py
--rw-r--r--   0        0        0      367 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_user_retweets/__init__.py
--rw-r--r--   0        0        0     1911 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py
--rw-r--r--   0        0        0      331 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_user_tweets/__init__.py
--rw-r--r--   0        0        0     8344 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py
--rw-r--r--   0        0        0      279 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_users/__init__.py
--rw-r--r--   0        0        0     2680 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_users/get_v2_users.py
--rw-r--r--   0        0        0      299 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_users_by/__init__.py
--rw-r--r--   0        0        0     2755 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_users_by/get_v2_users_by.py
--rw-r--r--   0        0        0      396 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_users_by_username/__init__.py
--rw-r--r--   0        0        0     3025 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py
--rw-r--r--   0        0        0        0 2023-04-01 17:37:01.267513 twitter_api_py-0.4.2/twitter_api/types/__init__.py
--rw-r--r--   0        0        0      386 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/_chainable.py
--rw-r--r--   0        0        0      570 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/_generic_client.py
--rw-r--r--   0        0        0     2362 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/_model.py
--rw-r--r--   0        0        0     3458 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/_paging.py
--rw-r--r--   0        0        0      697 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/comma_separatable.py
--rw-r--r--   0        0        0      234 2023-04-02 10:01:26.462016 twitter_api_py-0.4.2/twitter_api/types/endpoint.py
--rw-r--r--   0        0        0     1581 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/extra_permissive_model.py
--rw-r--r--   0        0        0      616 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/http.py
--rw-r--r--   0        0        0      734 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/httpx.py
--rw-r--r--   0        0        0     1942 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/oauth.py
--rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/oauth1/__init__.py
--rw-r--r--   0        0        0     2037 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/oauth1/oauth1_access_token.py
--rw-r--r--   0        0        0     3474 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/oauth1/oauth1_authorization.py
--rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/oauth2/__init__.py
--rw-r--r--   0        0        0     1975 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/oauth2/oauth2_access_token.py
--rw-r--r--   0        0        0     3593 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/oauth2/oauth2_authorization.py
--rw-r--r--   0        0        0       63 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/pagination_token.py
--rw-r--r--   0        0        0       55 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_cashtag.py
--rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_dm_conversation/__init__.py
--rw-r--r--   0        0        0      337 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_dm_conversation/dm_conversation.py
--rw-r--r--   0        0        0      201 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_dm_conversation/dm_conversation_attachment.py
--rw-r--r--   0        0        0       64 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_dm_conversation/dm_conversation_id.py
--rw-r--r--   0        0        0      594 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_dm_conversation/dm_conversation_message.py
--rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_dm_event/__init__.py
--rw-r--r--   0        0        0      331 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_dm_event/dm_event_expansion.py
--rw-r--r--   0        0        0      437 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_dm_event/dm_event_field.py
--rw-r--r--   0        0        0       57 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_dm_event/dm_event_id.py
--rw-r--r--   0        0        0      238 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_dm_event/dm_event_type.py
--rw-r--r--   0        0        0      338 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_domain.py
--rw-r--r--   0        0        0        0 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_entity/__init__.py
--rw-r--r--   0        0        0      286 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_entity/entity.py
--rw-r--r--   0        0        0       56 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_entity/entity_id.py
--rw-r--r--   0        0        0       58 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_entity/entity_name.py
--rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_geo/__init__.py
--rw-r--r--   0        0        0      209 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_geo/geo.py
--rw-r--r--   0        0        0       55 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_hashtag.py
--rw-r--r--   0        0        0      762 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_language.py
--rw-r--r--   0        0        0        0 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_list/__init__.py
--rw-r--r--   0        0        0       54 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_list/list_id.py
--rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_media/__init__.py
--rw-r--r--   0        0        0     1356 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_media/media.py
--rw-r--r--   0        0        0      570 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_media/media_field.py
--rw-r--r--   0        0        0      100 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_media/media_id.py
--rw-r--r--   0        0        0       56 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_media/media_key.py
--rw-r--r--   0        0        0      376 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_media/media_non_public_metrics.py
--rw-r--r--   0        0        0      411 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_media/media_organic_metrics.py
--rw-r--r--   0        0        0      412 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_media/media_promoted_metrics.py
--rw-r--r--   0        0        0      190 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_media/media_public_metrics.py
--rw-r--r--   0        0        0      211 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_media/media_variants.py
--rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_place/__init__.py
--rw-r--r--   0        0        0      933 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_place/place.py
--rw-r--r--   0        0        0     2712 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_place/place_country_code.py
--rw-r--r--   0        0        0      348 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_place/place_field.py
--rw-r--r--   0        0        0       61 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_place/place_full_name.py
--rw-r--r--   0        0        0       94 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_place/place_id.py
--rw-r--r--   0        0        0       57 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_place/place_name.py
--rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_poll/__init__.py
--rw-r--r--   0        0        0      593 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_poll/poll.py
--rw-r--r--   0        0        0      272 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_poll/poll_field.py
--rw-r--r--   0        0        0       54 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_poll/poll_id.py
--rw-r--r--   0        0        0      164 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_poll/poll_option.py
--rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_retweet/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_retweet/retweet.py
--rw-r--r--   0        0        0      392 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_retweet/retweet_entities.py
--rw-r--r--   0        0        0      913 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_retweet/retweet_entities_description.py
--rw-r--r--   0        0        0      237 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_retweet/retweet_entities_description_cashtag.py
--rw-r--r--   0        0        0      237 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_retweet/retweet_entities_description_hashtag.py
--rw-r--r--   0        0        0      246 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_retweet/retweet_entities_description_mention.py
--rw-r--r--   0        0        0      258 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_retweet/retweet_entities_description_url.py
--rw-r--r--   0        0        0      338 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_retweet/retweet_entities_url.py
--rw-r--r--   0        0        0      254 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_retweet/retweet_includes.py
--rw-r--r--   0        0        0      219 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_retweet/retweet_public_metrics.py
--rw-r--r--   0        0        0      352 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_retweet/retweet_withheld.py
--rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_rule/__init__.py
--rw-r--r--   0        0        0      311 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_rule/rule.py
--rw-r--r--   0        0        0       54 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_rule/rule_id.py
--rw-r--r--   0        0        0       55 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_rule/rule_tag.py
--rw-r--r--   0        0        0     1411 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_scope.py
--rw-r--r--   0        0        0        0 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/__init__.py
--rw-r--r--   0        0        0      917 2023-05-05 10:48:31.793871 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/_and_operator.py
--rw-r--r--   0        0        0      305 2023-05-04 12:42:31.224094 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/_markable_operator.py
--rw-r--r--   0        0        0      803 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/_not_operator.py
--rw-r--r--   0        0        0      706 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/_or_operator.py
--rw-r--r--   0        0        0      666 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/bounding_box_operator.py
--rw-r--r--   0        0        0      369 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/cashtag_operator.py
--rw-r--r--   0        0        0     1361 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/context_operator.py
--rw-r--r--   0        0        0      410 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/conversation_id_operator.py
--rw-r--r--   0        0        0      371 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/entity_operator.py
--rw-r--r--   0        0        0      454 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/from_user_operator.py
--rw-r--r--   0        0        0     1991 2023-05-05 11:08:58.964264 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/group_operator.py
--rw-r--r--   0        0        0      239 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/has_cashtags_operator.py
--rw-r--r--   0        0        0      229 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/has_geo_operator.py
--rw-r--r--   0        0        0      239 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/has_hashtags_operator.py
--rw-r--r--   0        0        0      235 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/has_images_operator.py
--rw-r--r--   0        0        0      233 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/has_links_operator.py
--rw-r--r--   0        0        0      233 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/has_media_operator.py
--rw-r--r--   0        0        0      239 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/has_mentions_operator.py
--rw-r--r--   0        0        0      242 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/has_video_link_operator.py
--rw-r--r--   0        0        0      369 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/hashtag_operator.py
--rw-r--r--   0        0        0      379 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/in_reply_to_tweet_id_operator.py
--rw-r--r--   0        0        0      442 2023-05-05 00:14:01.104855 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/is_nullcast_operator.py
--rw-r--r--   0        0        0      231 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/is_quote_operator.py
--rw-r--r--   0        0        0      231 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/is_reply_operator.py
--rw-r--r--   0        0        0      235 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/is_retweet_operator.py
--rw-r--r--   0        0        0      237 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/is_verified_operator.py
--rw-r--r--   0        0        0      446 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/keyword_operator.py
--rw-r--r--   0        0        0      359 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/lang_operator.py
--rw-r--r--   0        0        0      347 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/list_operator.py
--rw-r--r--   0        0        0      379 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/mention_operator.py
--rw-r--r--   0        0        0     2347 2023-05-05 12:02:00.300988 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/operator.py
--rw-r--r--   0        0        0      400 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/place_country_operator.py
--rw-r--r--   0        0        0      574 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/place_operator.py
--rw-r--r--   0        0        0     1280 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/point_radius_operator.py
--rw-r--r--   0        0        0      384 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/quotes_of_tweet_id_operator.py
--rw-r--r--   0        0        0      462 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/retweet_of_operator.py
--rw-r--r--   0        0        0      380 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/retweets_of_tweet_id_operator.py
--rw-r--r--   0        0        0      450 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/to_user_operator.py
--rw-r--r--   0        0        0      292 2023-05-05 10:37:28.028143 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/url_operator.py
--rw-r--r--   0        0        0    16964 2023-05-05 12:05:36.752806 twitter_api_py-0.4.2/twitter_api/types/v2_search_query/search_query.py
--rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/__init__.py
--rw-r--r--   0        0        0     7856 2023-05-04 12:42:31.234094 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet.py
--rw-r--r--   0        0        0      309 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_attachments.py
--rw-r--r--   0        0        0      267 2023-05-04 12:42:31.234094 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_context_annotation.py
--rw-r--r--   0        0        0      314 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_edit_controls.py
--rw-r--r--   0        0        0      720 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_entities.py
--rw-r--r--   0        0        0      333 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_entities_annotation.py
--rw-r--r--   0        0        0      247 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_entities_cashtag.py
--rw-r--r--   0        0        0      247 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_entities_hashtag.py
--rw-r--r--   0        0        0      313 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_entities_mention.py
--rw-r--r--   0        0        0      415 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_entities_url.py
--rw-r--r--   0        0        0      632 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_expansion.py
--rw-r--r--   0        0        0     1910 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_field.py
--rw-r--r--   0        0        0      288 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_geo.py
--rw-r--r--   0        0        0      231 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_geo_coordinates.py
--rw-r--r--   0        0        0      100 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_id.py
--rw-r--r--   0        0        0      287 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_non_public_metrics.py
--rw-r--r--   0        0        0      285 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_organic_metrics.py
--rw-r--r--   0        0        0      286 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_promoted_metrics.py
--rw-r--r--   0        0        0      437 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_public_metrics.py
--rw-r--r--   0        0        0      256 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_referenced_tweet.py
--rw-r--r--   0        0        0     7050 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_response_body.py
--rw-r--r--   0        0        0      387 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_withheld.py
--rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_user/__init__.py
--rw-r--r--   0        0        0      969 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_user/user.py
--rw-r--r--   0        0        0      157 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_user/user_expantion.py
--rw-r--r--   0        0        0      608 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_user/user_field.py
--rw-r--r--   0        0        0       54 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_user/user_id.py
--rw-r--r--   0        0        0       97 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_user/user_verified_type.py
--rw-r--r--   0        0        0      128 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/types/v2_user/username.py
--rw-r--r--   0        0        0        0 2023-04-01 09:17:10.085603 twitter_api_py-0.4.2/twitter_api/utils/__init__.py
--rw-r--r--   0        0        0      123 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/utils/_datetime.py
--rw-r--r--   0        0        0      716 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/utils/_functional.py
--rw-r--r--   0        0        0      904 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/utils/_oauth.py
--rw-r--r--   0        0        0      790 2023-05-05 00:14:01.104855 twitter_api_py-0.4.2/twitter_api/utils/json.py
--rw-r--r--   0        0        0      630 2023-05-03 13:16:42.871502 twitter_api_py-0.4.2/twitter_api/warning.py
--rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 twitter_api_py-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-05-03 13:16:42.851501 twitter_api_py-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2126 2023-05-03 13:16:42.851501 twitter_api_py-0.4.3/README.md
+-rw-r--r--   0        0        0     1516 2023-05-05 13:08:53.994701 twitter_api_py-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      480 2023-05-05 00:14:01.094855 twitter_api_py-0.4.3/twitter_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.4.3/twitter_api/client/oauth_flow/__init__.py
+-rw-r--r--   0        0        0     1041 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py
+-rw-r--r--   0        0        0      311 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth1_access_token_mock_client.py
+-rw-r--r--   0        0        0     1388 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py
+-rw-r--r--   0        0        0      306 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth1_authorization_mock_client.py
+-rw-r--r--   0        0        0      808 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py
+-rw-r--r--   0        0        0      315 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth1_request_token_mock_client.py
+-rw-r--r--   0        0        0     1211 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py
+-rw-r--r--   0        0        0      311 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth2_access_token_mock_client.py
+-rw-r--r--   0        0        0      831 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py
+-rw-r--r--   0        0        0      306 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth2_authorization_mock_client.py
+-rw-r--r--   0        0        0        0 2023-04-09 09:46:11.283030 twitter_api_py-0.4.3/twitter_api/client/oauth_session/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 10:21:01.811509 twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/__init__.py
+-rw-r--r--   0        0        0      365 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth1_access_token/__init__.py
+-rw-r--r--   0        0        0     1140 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py
+-rw-r--r--   0        0        0      451 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth1_authenticate/__init__.py
+-rw-r--r--   0        0        0      793 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py
+-rw-r--r--   0        0        0      433 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth1_authorize/__init__.py
+-rw-r--r--   0        0        0      722 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py
+-rw-r--r--   0        0        0      392 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth1_request_token/__init__.py
+-rw-r--r--   0        0        0      798 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py
+-rw-r--r--   0        0        0      501 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth2_authorize/__init__.py
+-rw-r--r--   0        0        0      751 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py
+-rw-r--r--   0        0        0      648 2023-05-03 13:16:42.861501 twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/session_resources.py
+-rw-r--r--   0        0        0      376 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/v2_oauth2_token/__init__.py
+-rw-r--r--   0        0        0     1596 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py
+-rw-r--r--   0        0        0     1793 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py
+-rw-r--r--   0        0        0     3885 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/oauth_session/twitter_oauth1_real_session.py
+-rw-r--r--   0        0        0     1103 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/oauth_session/twitter_oauth1_session.py
+-rw-r--r--   0        0        0     1561 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py
+-rw-r--r--   0        0        0     3397 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/oauth_session/twitter_oauth2_real_session.py
+-rw-r--r--   0        0        0      823 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/oauth_session/twitter_oauth2_session.py
+-rw-r--r--   0        0        0        0 2023-04-01 17:37:10.337565 twitter_api_py-0.4.3/twitter_api/client/request/__init__.py
+-rw-r--r--   0        0        0     1577 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/request/request_async_client.py
+-rw-r--r--   0        0        0      236 2023-04-22 10:21:01.811509 twitter_api_py-0.4.3/twitter_api/client/request/request_async_mock_client.py
+-rw-r--r--   0        0        0     5182 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/request/request_async_real_client.py
+-rw-r--r--   0        0        0     1967 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/request/request_client.py
+-rw-r--r--   0        0        0     3368 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/request/request_mock_client.py
+-rw-r--r--   0        0        0     7235 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/request/request_real_client.py
+-rw-r--r--   0        0        0    32304 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/twitter_api_async_client.py
+-rw-r--r--   0        0        0    14518 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/twitter_api_async_mock_client.py
+-rw-r--r--   0        0        0    14743 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/twitter_api_async_real_client.py
+-rw-r--r--   0        0        0    32063 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/twitter_api_client.py
+-rw-r--r--   0        0        0    26895 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/twitter_api_mock_client.py
+-rw-r--r--   0        0        0    13583 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/client/twitter_api_real_client.py
+-rw-r--r--   0        0        0    10636 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/error.py
+-rw-r--r--   0        0        0        0 2023-04-02 08:29:19.122099 twitter_api_py-0.4.3/twitter_api/rate_limit/__init__.py
+-rw-r--r--   0        0        0      603 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/rate_limit/manager/__init__.py
+-rw-r--r--   0        0        0     2232 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/rate_limit/manager/dict_rate_limit_manager.py
+-rw-r--r--   0        0        0      976 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py
+-rw-r--r--   0        0        0        0 2023-04-23 01:25:28.771650 twitter_api_py-0.4.3/twitter_api/rate_limit/manager/handlers/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py
+-rw-r--r--   0        0        0     3316 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py
+-rw-r--r--   0        0        0      705 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py
+-rw-r--r--   0        0        0     1232 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/rate_limit/manager/rate_limit_manager.py
+-rw-r--r--   0        0        0     3303 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/rate_limit/rate_limit.py
+-rw-r--r--   0        0        0      291 2023-05-02 14:52:07.203654 twitter_api_py-0.4.3/twitter_api/rate_limit/rate_limit_info.py
+-rw-r--r--   0        0        0       91 2023-05-02 14:52:07.203654 twitter_api_py-0.4.3/twitter_api/rate_limit/rate_limit_target.py
+-rw-r--r--   0        0        0      281 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/api_resources.py
+-rw-r--r--   0        0        0      437 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/oauth2_invalidate_token/__init__.py
+-rw-r--r--   0        0        0     2295 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py
+-rw-r--r--   0        0        0      332 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/oauth2_token/__init__.py
+-rw-r--r--   0        0        0     2187 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/oauth2_token/post_oauth2_token.py
+-rw-r--r--   0        0        0      541 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversation_messages/__init__.py
+-rw-r--r--   0        0        0     2316 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py
+-rw-r--r--   0        0        0      441 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversations/__init__.py
+-rw-r--r--   0        0        0     2164 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py
+-rw-r--r--   0        0        0      673 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py
+-rw-r--r--   0        0        0     8907 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py
+-rw-r--r--   0        0        0      676 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py
+-rw-r--r--   0        0        0     2390 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py
+-rw-r--r--   0        0        0      429 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweet/__init__.py
+-rw-r--r--   0        0        0     1438 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweet/delete_v2_tweet.py
+-rw-r--r--   0        0        0     3088 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweet/get_v2_tweet.py
+-rw-r--r--   0        0        0      458 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweet_retweeted_by/__init__.py
+-rw-r--r--   0        0        0     6561 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py
+-rw-r--r--   0        0        0      428 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweets/__init__.py
+-rw-r--r--   0        0        0     2977 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweets/get_v2_tweets.py
+-rw-r--r--   0        0        0     2926 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweets/post_v2_tweets.py
+-rw-r--r--   0        0        0      438 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_all/__init__.py
+-rw-r--r--   0        0        0     6032 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py
+-rw-r--r--   0        0        0      471 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_recent/__init__.py
+-rw-r--r--   0        0        0     6131 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py
+-rw-r--r--   0        0        0      471 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_stream/__init__.py
+-rw-r--r--   0        0        0     3615 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py
+-rw-r--r--   0        0        0      770 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py
+-rw-r--r--   0        0        0     2111 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py
+-rw-r--r--   0        0        0     3096 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py
+-rw-r--r--   0        0        0      275 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_user/__init__.py
+-rw-r--r--   0        0        0     2780 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_user/get_v2_user.py
+-rw-r--r--   0        0        0      371 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_user_followers/__init__.py
+-rw-r--r--   0        0        0     6510 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_user_followers/get_v2_user_followers.py
+-rw-r--r--   0        0        0      376 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_user_following/__init__.py
+-rw-r--r--   0        0        0     1909 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_user_following/post_v2_user_following.py
+-rw-r--r--   0        0        0      391 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_user_liked_tweets/__init__.py
+-rw-r--r--   0        0        0     7931 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py
+-rw-r--r--   0        0        0      367 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_user_retweets/__init__.py
+-rw-r--r--   0        0        0     1911 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py
+-rw-r--r--   0        0        0      331 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_user_tweets/__init__.py
+-rw-r--r--   0        0        0     8344 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py
+-rw-r--r--   0        0        0      279 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_users/__init__.py
+-rw-r--r--   0        0        0     2680 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_users/get_v2_users.py
+-rw-r--r--   0        0        0      299 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_users_by/__init__.py
+-rw-r--r--   0        0        0     2755 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_users_by/get_v2_users_by.py
+-rw-r--r--   0        0        0      396 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_users_by_username/__init__.py
+-rw-r--r--   0        0        0     3025 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py
+-rw-r--r--   0        0        0        0 2023-04-01 17:37:01.267513 twitter_api_py-0.4.3/twitter_api/types/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/_chainable.py
+-rw-r--r--   0        0        0      570 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/_generic_client.py
+-rw-r--r--   0        0        0     2362 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/_model.py
+-rw-r--r--   0        0        0     3458 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/_paging.py
+-rw-r--r--   0        0        0      697 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/comma_separatable.py
+-rw-r--r--   0        0        0      234 2023-04-02 10:01:26.462016 twitter_api_py-0.4.3/twitter_api/types/endpoint.py
+-rw-r--r--   0        0        0     1581 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/extra_permissive_model.py
+-rw-r--r--   0        0        0      616 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/http.py
+-rw-r--r--   0        0        0      734 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/httpx.py
+-rw-r--r--   0        0        0     1942 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/oauth.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/oauth1/__init__.py
+-rw-r--r--   0        0        0     2037 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/oauth1/oauth1_access_token.py
+-rw-r--r--   0        0        0     3474 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/oauth1/oauth1_authorization.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/oauth2/__init__.py
+-rw-r--r--   0        0        0     1975 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/oauth2/oauth2_access_token.py
+-rw-r--r--   0        0        0     3593 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/oauth2/oauth2_authorization.py
+-rw-r--r--   0        0        0       63 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/pagination_token.py
+-rw-r--r--   0        0        0       55 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_cashtag.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_dm_conversation/__init__.py
+-rw-r--r--   0        0        0      337 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_dm_conversation/dm_conversation.py
+-rw-r--r--   0        0        0      201 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_dm_conversation/dm_conversation_attachment.py
+-rw-r--r--   0        0        0       64 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_dm_conversation/dm_conversation_id.py
+-rw-r--r--   0        0        0      594 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_dm_conversation/dm_conversation_message.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_dm_event/__init__.py
+-rw-r--r--   0        0        0      331 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_dm_event/dm_event_expansion.py
+-rw-r--r--   0        0        0      437 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_dm_event/dm_event_field.py
+-rw-r--r--   0        0        0       57 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_dm_event/dm_event_id.py
+-rw-r--r--   0        0        0      238 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_dm_event/dm_event_type.py
+-rw-r--r--   0        0        0      338 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_domain.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_entity/__init__.py
+-rw-r--r--   0        0        0      286 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_entity/entity.py
+-rw-r--r--   0        0        0       56 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_entity/entity_id.py
+-rw-r--r--   0        0        0       58 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_entity/entity_name.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_geo/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_geo/geo.py
+-rw-r--r--   0        0        0       55 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_hashtag.py
+-rw-r--r--   0        0        0      762 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_language.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_list/__init__.py
+-rw-r--r--   0        0        0       54 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_list/list_id.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_media/__init__.py
+-rw-r--r--   0        0        0     1356 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_media/media.py
+-rw-r--r--   0        0        0      570 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_media/media_field.py
+-rw-r--r--   0        0        0      100 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_media/media_id.py
+-rw-r--r--   0        0        0       56 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_media/media_key.py
+-rw-r--r--   0        0        0      376 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_media/media_non_public_metrics.py
+-rw-r--r--   0        0        0      411 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_media/media_organic_metrics.py
+-rw-r--r--   0        0        0      412 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_media/media_promoted_metrics.py
+-rw-r--r--   0        0        0      190 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_media/media_public_metrics.py
+-rw-r--r--   0        0        0      211 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_media/media_variants.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_place/__init__.py
+-rw-r--r--   0        0        0      933 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_place/place.py
+-rw-r--r--   0        0        0     2712 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_place/place_country_code.py
+-rw-r--r--   0        0        0      348 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_place/place_field.py
+-rw-r--r--   0        0        0       61 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_place/place_full_name.py
+-rw-r--r--   0        0        0       94 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_place/place_id.py
+-rw-r--r--   0        0        0       57 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_place/place_name.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_poll/__init__.py
+-rw-r--r--   0        0        0      593 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_poll/poll.py
+-rw-r--r--   0        0        0      272 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_poll/poll_field.py
+-rw-r--r--   0        0        0       54 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_poll/poll_id.py
+-rw-r--r--   0        0        0      164 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_poll/poll_option.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_retweet/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_retweet/retweet.py
+-rw-r--r--   0        0        0      392 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_retweet/retweet_entities.py
+-rw-r--r--   0        0        0      913 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_retweet/retweet_entities_description.py
+-rw-r--r--   0        0        0      237 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_retweet/retweet_entities_description_cashtag.py
+-rw-r--r--   0        0        0      237 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_retweet/retweet_entities_description_hashtag.py
+-rw-r--r--   0        0        0      246 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_retweet/retweet_entities_description_mention.py
+-rw-r--r--   0        0        0      258 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_retweet/retweet_entities_description_url.py
+-rw-r--r--   0        0        0      338 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_retweet/retweet_entities_url.py
+-rw-r--r--   0        0        0      254 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_retweet/retweet_includes.py
+-rw-r--r--   0        0        0      219 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_retweet/retweet_public_metrics.py
+-rw-r--r--   0        0        0      352 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_retweet/retweet_withheld.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_rule/__init__.py
+-rw-r--r--   0        0        0      311 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_rule/rule.py
+-rw-r--r--   0        0        0       54 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_rule/rule_id.py
+-rw-r--r--   0        0        0       55 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_rule/rule_tag.py
+-rw-r--r--   0        0        0     1411 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_scope.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/__init__.py
+-rw-r--r--   0        0        0      860 2023-05-05 13:03:07.001788 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/_and_operator.py
+-rw-r--r--   0        0        0      305 2023-05-04 12:42:31.224094 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/_markable_operator.py
+-rw-r--r--   0        0        0      756 2023-05-05 13:03:52.152168 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/_not_operator.py
+-rw-r--r--   0        0        0      649 2023-05-05 13:03:15.331858 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/_or_operator.py
+-rw-r--r--   0        0        0      666 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/bounding_box_operator.py
+-rw-r--r--   0        0        0      369 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/cashtag_operator.py
+-rw-r--r--   0        0        0     1361 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/context_operator.py
+-rw-r--r--   0        0        0      410 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/conversation_id_operator.py
+-rw-r--r--   0        0        0      371 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/entity_operator.py
+-rw-r--r--   0        0        0      454 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/from_user_operator.py
+-rw-r--r--   0        0        0     1506 2023-05-05 13:04:07.162294 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/group_operator.py
+-rw-r--r--   0        0        0      239 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/has_cashtags_operator.py
+-rw-r--r--   0        0        0      229 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/has_geo_operator.py
+-rw-r--r--   0        0        0      239 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/has_hashtags_operator.py
+-rw-r--r--   0        0        0      235 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/has_images_operator.py
+-rw-r--r--   0        0        0      233 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/has_links_operator.py
+-rw-r--r--   0        0        0      233 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/has_media_operator.py
+-rw-r--r--   0        0        0      239 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/has_mentions_operator.py
+-rw-r--r--   0        0        0      242 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/has_video_link_operator.py
+-rw-r--r--   0        0        0      369 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/hashtag_operator.py
+-rw-r--r--   0        0        0      379 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/in_reply_to_tweet_id_operator.py
+-rw-r--r--   0        0        0      442 2023-05-05 00:14:01.104855 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/is_nullcast_operator.py
+-rw-r--r--   0        0        0      231 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/is_quote_operator.py
+-rw-r--r--   0        0        0      231 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/is_reply_operator.py
+-rw-r--r--   0        0        0      235 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/is_retweet_operator.py
+-rw-r--r--   0        0        0      237 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/is_verified_operator.py
+-rw-r--r--   0        0        0      446 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/keyword_operator.py
+-rw-r--r--   0        0        0      359 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/lang_operator.py
+-rw-r--r--   0        0        0      347 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/list_operator.py
+-rw-r--r--   0        0        0      379 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/mention_operator.py
+-rw-r--r--   0        0        0     2347 2023-05-05 12:02:00.300988 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/operator.py
+-rw-r--r--   0        0        0      400 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/place_country_operator.py
+-rw-r--r--   0        0        0      574 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/place_operator.py
+-rw-r--r--   0        0        0     1280 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/point_radius_operator.py
+-rw-r--r--   0        0        0      384 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/quotes_of_tweet_id_operator.py
+-rw-r--r--   0        0        0      462 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/retweet_of_operator.py
+-rw-r--r--   0        0        0      380 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/retweets_of_tweet_id_operator.py
+-rw-r--r--   0        0        0      450 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/to_user_operator.py
+-rw-r--r--   0        0        0      292 2023-05-05 10:37:28.028143 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/url_operator.py
+-rw-r--r--   0        0        0    17105 2023-05-05 13:00:59.780720 twitter_api_py-0.4.3/twitter_api/types/v2_search_query/search_query.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/__init__.py
+-rw-r--r--   0        0        0     7856 2023-05-04 12:42:31.234094 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet.py
+-rw-r--r--   0        0        0      309 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_attachments.py
+-rw-r--r--   0        0        0      267 2023-05-04 12:42:31.234094 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_context_annotation.py
+-rw-r--r--   0        0        0      314 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_edit_controls.py
+-rw-r--r--   0        0        0      720 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_entities.py
+-rw-r--r--   0        0        0      333 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_entities_annotation.py
+-rw-r--r--   0        0        0      247 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_entities_cashtag.py
+-rw-r--r--   0        0        0      247 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_entities_hashtag.py
+-rw-r--r--   0        0        0      313 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_entities_mention.py
+-rw-r--r--   0        0        0      415 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_entities_url.py
+-rw-r--r--   0        0        0      632 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_expansion.py
+-rw-r--r--   0        0        0     1910 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_field.py
+-rw-r--r--   0        0        0      288 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_geo.py
+-rw-r--r--   0        0        0      231 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_geo_coordinates.py
+-rw-r--r--   0        0        0      100 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_id.py
+-rw-r--r--   0        0        0      287 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_non_public_metrics.py
+-rw-r--r--   0        0        0      285 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_organic_metrics.py
+-rw-r--r--   0        0        0      286 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_promoted_metrics.py
+-rw-r--r--   0        0        0      437 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_public_metrics.py
+-rw-r--r--   0        0        0      256 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_referenced_tweet.py
+-rw-r--r--   0        0        0     7050 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_response_body.py
+-rw-r--r--   0        0        0      387 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_withheld.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_user/__init__.py
+-rw-r--r--   0        0        0      969 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_user/user.py
+-rw-r--r--   0        0        0      157 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_user/user_expantion.py
+-rw-r--r--   0        0        0      608 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_user/user_field.py
+-rw-r--r--   0        0        0       54 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_user/user_id.py
+-rw-r--r--   0        0        0       97 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_user/user_verified_type.py
+-rw-r--r--   0        0        0      128 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/types/v2_user/username.py
+-rw-r--r--   0        0        0        0 2023-04-01 09:17:10.085603 twitter_api_py-0.4.3/twitter_api/utils/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/utils/_datetime.py
+-rw-r--r--   0        0        0      716 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/utils/_functional.py
+-rw-r--r--   0        0        0      904 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/utils/_oauth.py
+-rw-r--r--   0        0        0      790 2023-05-05 00:14:01.104855 twitter_api_py-0.4.3/twitter_api/utils/json.py
+-rw-r--r--   0        0        0      630 2023-05-03 13:16:42.871502 twitter_api_py-0.4.3/twitter_api/warning.py
+-rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 twitter_api_py-0.4.3/PKG-INFO
```

### Comparing `twitter_api_py-0.4.2/LICENSE` & `twitter_api_py-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/README.md` & `twitter_api_py-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/pyproject.toml` & `twitter_api_py-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["yassun4dev <yassun4dev@outlook.com>"]
 description = "Twitter API Client by Typed Python."
 name = "twitter-api-py"
 packages = [{include = "twitter_api"}]
 readme = "README.md"
-version = "0.4.2"
+version = "0.4.3"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/twitter-api-py"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
```

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth1_access_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth1_authorization_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth1_request_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth2_access_token_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_flow/twitter_oauth2_authorization_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth1_access_token/post_oauth1_access_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth1_authenticate/generate_authorization_url_oauth1_authenticate.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth1_authorize/generate_authorization_url_oauth1_authorize.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth1_request_token/post_oauth1_request_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/oauth2_authorize/generate_authorization_url_oauth2_authorize.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/session_resources.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/session_resources.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_session/resources/v2_oauth2_token/post_v2_oauth2_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_session/twitter_oauth1_mock_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_session/twitter_oauth1_real_session.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_session/twitter_oauth1_real_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_session/twitter_oauth1_session.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_session/twitter_oauth1_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_session/twitter_oauth2_mock_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_session/twitter_oauth2_real_session.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_session/twitter_oauth2_real_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/oauth_session/twitter_oauth2_session.py` & `twitter_api_py-0.4.3/twitter_api/client/oauth_session/twitter_oauth2_session.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/request/request_async_client.py` & `twitter_api_py-0.4.3/twitter_api/client/request/request_async_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/request/request_async_real_client.py` & `twitter_api_py-0.4.3/twitter_api/client/request/request_async_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/request/request_client.py` & `twitter_api_py-0.4.3/twitter_api/client/request/request_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/request/request_mock_client.py` & `twitter_api_py-0.4.3/twitter_api/client/request/request_mock_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/request/request_real_client.py` & `twitter_api_py-0.4.3/twitter_api/client/request/request_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/twitter_api_async_client.py` & `twitter_api_py-0.4.3/twitter_api/client/twitter_api_async_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/twitter_api_async_mock_client.py` & `twitter_api_py-0.4.3/twitter_api/client/twitter_api_async_mock_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/twitter_api_async_real_client.py` & `twitter_api_py-0.4.3/twitter_api/client/twitter_api_async_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/twitter_api_client.py` & `twitter_api_py-0.4.3/twitter_api/client/twitter_api_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/twitter_api_mock_client.py` & `twitter_api_py-0.4.3/twitter_api/client/twitter_api_mock_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/client/twitter_api_real_client.py` & `twitter_api_py-0.4.3/twitter_api/client/twitter_api_real_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/error.py` & `twitter_api_py-0.4.3/twitter_api/error.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/rate_limit/manager/__init__.py` & `twitter_api_py-0.4.3/twitter_api/rate_limit/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/rate_limit/manager/dict_rate_limit_manager.py` & `twitter_api_py-0.4.3/twitter_api/rate_limit/manager/dict_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py` & `twitter_api_py-0.4.3/twitter_api/rate_limit/manager/dict_sleep_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py` & `twitter_api_py-0.4.3/twitter_api/rate_limit/manager/handlers/raise_rate_limit_handler.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py` & `twitter_api_py-0.4.3/twitter_api/rate_limit/manager/handlers/sleep_rate_limit_handler.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py` & `twitter_api_py-0.4.3/twitter_api/rate_limit/manager/no_operation_rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/rate_limit/manager/rate_limit_manager.py` & `twitter_api_py-0.4.3/twitter_api/rate_limit/manager/rate_limit_manager.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/rate_limit/rate_limit.py` & `twitter_api_py-0.4.3/twitter_api/rate_limit/rate_limit.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py` & `twitter_api_py-0.4.3/twitter_api/resources/oauth2_invalidate_token/post_oauth2_invalidate_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/oauth2_token/post_oauth2_token.py` & `twitter_api_py-0.4.3/twitter_api/resources/oauth2_token/post_oauth2_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversation_messages/__init__.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversation_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversation_messages/post_v2_dm_conversations_messages.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversations/post_v2_dm_conversations.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversations_with_participant_dm_events/get_v2_dm_conversations_with_participant_dm_events.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_dm_conversations_with_participant_messages/post_v2_dm_conversations_with_participant_messages.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_tweet/delete_v2_tweet.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_tweet/delete_v2_tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_tweet/get_v2_tweet.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_tweet/get_v2_tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_tweet_retweeted_by/get_v2_tweet_retweeted_by.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_tweets/get_v2_tweets.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_tweets/get_v2_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_tweets/post_v2_tweets.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_tweets/post_v2_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_all/get_v2_tweets_search_all.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_recent/get_v2_tweets_search_recent.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_stream/get_v2_tweets_search_stream.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_stream_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_stream_rules/get_v2_tweets_search_stream_rules.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_tweets_search_stream_rules/post_v2_tweets_search_stream_rules.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_user/get_v2_user.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_user/get_v2_user.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_user_followers/get_v2_user_followers.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_user_followers/get_v2_user_followers.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_user_following/post_v2_user_following.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_user_following/post_v2_user_following.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_user_liked_tweets/get_v2_user_liked_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_user_retweets/post_v2_user_retweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_user_tweets/get_v2_user_tweets.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_users/get_v2_users.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_users/get_v2_users.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_users_by/get_v2_users_by.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_users_by/get_v2_users_by.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py` & `twitter_api_py-0.4.3/twitter_api/resources/v2_users_by_username/get_v2_users_by_username.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/_generic_client.py` & `twitter_api_py-0.4.3/twitter_api/types/_generic_client.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/_model.py` & `twitter_api_py-0.4.3/twitter_api/types/_model.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/_paging.py` & `twitter_api_py-0.4.3/twitter_api/types/_paging.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/comma_separatable.py` & `twitter_api_py-0.4.3/twitter_api/types/comma_separatable.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/extra_permissive_model.py` & `twitter_api_py-0.4.3/twitter_api/types/extra_permissive_model.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/http.py` & `twitter_api_py-0.4.3/twitter_api/types/http.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/httpx.py` & `twitter_api_py-0.4.3/twitter_api/types/httpx.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/oauth.py` & `twitter_api_py-0.4.3/twitter_api/types/oauth.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/oauth1/oauth1_access_token.py` & `twitter_api_py-0.4.3/twitter_api/types/oauth1/oauth1_access_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/oauth1/oauth1_authorization.py` & `twitter_api_py-0.4.3/twitter_api/types/oauth1/oauth1_authorization.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/oauth2/oauth2_access_token.py` & `twitter_api_py-0.4.3/twitter_api/types/oauth2/oauth2_access_token.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/oauth2/oauth2_authorization.py` & `twitter_api_py-0.4.3/twitter_api/types/oauth2/oauth2_authorization.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_dm_conversation/dm_conversation_message.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_dm_conversation/dm_conversation_message.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_language.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_language.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_media/media.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_media/media.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_media/media_field.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_media/media_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_place/place.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_place/place.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_place/place_country_code.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_place/place_country_code.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_poll/poll.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_poll/poll.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_retweet/retweet.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_retweet/retweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_retweet/retweet_entities_description.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_retweet/retweet_entities_description.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_scope.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_scope.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/_and_operator.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/_or_operator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,22 @@
-from typing import overload
-
-from .group_operator import grouping
 from .operator import CorrectOperator, Operator, WeakOperator
 
 
-class AndOperator(Operator):
+class OrOperator(Operator):
     def __init__(self, left: Operator, right: Operator) -> None:
         self._left = left
         self._right = right
 
     def __str__(self) -> str:
-        return f"{grouping(self._left)} {grouping(self._right)}"
+        return f"{self._left} OR {self._right}"
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({repr(self._left)}, {repr(self._right)})"
 
 
-class WeakAndOperator(AndOperator, WeakOperator):
+class WeakOrOperator(OrOperator, WeakOperator):
     pass
 
 
-class CorrectAndOperator(AndOperator, CorrectOperator[Operator]):
-    @overload
-    def __init__(self, left: CorrectOperator, right: Operator) -> None:
-        ...
-
-    @overload
-    def __init__(self, left: Operator, right: CorrectOperator) -> None:
-        ...
-
-    def __init__(self, left, right) -> None:
-        self._left = left
-        self._right = right
+class CorrectOrOperator(OrOperator, CorrectOperator[Operator]):
+    def __init__(self, left: CorrectOperator, right: CorrectOperator) -> None:
+        super().__init__(left, right)
```

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/_not_operator.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/_not_operator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from .group_operator import grouping
 from .operator import Operator, WeakOperator
 
 
 class NotOperator(
     # NOTE: 否定は CorrectOperator ではなく、 WeakOperator である。
     #       言い換えれば、クエリの最初、またはグループの最初は否定以外から開始しなければならない。
     #       そうでないクエリを作成することはできるだろうが、検索効率の悪いクエリになる。
     #       本ツールでは、意図的に否定から開始するクエリを禁止する。
     WeakOperator,
 ):
     def __init__(self, op: Operator) -> None:
         self._op = op
 
     def __str__(self) -> str:
-        return f"-{grouping(self._op)}"
+        return f"-{self._op}"
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({repr(self._op)})"
```

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/bounding_box_operator.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/bounding_box_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/context_operator.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/context_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/group_operator.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/group_operator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,41 @@
-from itertools import chain
-
 from .operator import CorrectOperator, Operator, WeakOperator
 
 
 class GroupOperator(
     # NOTE: 公式ドキュメントでは否定をグループに対して行わないように書かれており、
     #       "skiing -(snow OR day OR noschool)" よりも
     #       "skiing -snow -day -noschool" の方が推奨されている。
     #       そのため、本ツールではグループへの否定演算子は対応しない。
     #
     # refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/integrate/build-a-query
     #
     # InvertibleOperator[Operator],
     Operator,
 ):
-    def __init__(self, operator: Operator, *operators: Operator):
-        if len(operators) == 0 and isinstance(operator, GroupOperator):
+    def __init__(self, operator: Operator):
+        if isinstance(operator, GroupOperator):
             # GroupOperator の重ね掛けはまとめる。
-            self._operators = operator._operators
+            self._operator = operator._operator
         else:
-            self._operators = tuple(chain((operator,), operators))
-
-    def __len__(self) -> int:
-        return len(self._operators)
+            self._operator = operator
 
     def __str__(self) -> str:
         from ._and_operator import AndOperator
         from ._not_operator import NotOperator
         from ._or_operator import OrOperator
 
-        if len(self._operators) == 1 and isinstance(
-            self._operators[0], (AndOperator, OrOperator, NotOperator)
-        ):
-            return f"({self._operators[0]})"
-
-        return " ".join(map(grouping, self._operators))
+        if isinstance(self._operator, (AndOperator, OrOperator, NotOperator)):
+            return f"({self._operator})"
+        return str(self._operator)
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({', '.join(map(repr, self._operators))})"
+        return f"{self.__class__.__name__}({repr(self._operator)})"
 
 
 class WeakGroupOperator(GroupOperator, WeakOperator):
     pass
 
 
 class CorrectGroupOperator(GroupOperator, CorrectOperator[Operator]):
-    def __init__(self, operator: CorrectOperator, *operators: Operator):
-        super().__init__(operator, *operators)
-
-
-def grouping(operator: Operator) -> str:
-    if isinstance(operator, GroupOperator) and len(operator) > 1:
-        return f"({operator})"
-    else:
-        return str(operator)
+    def __init__(self, operator: CorrectOperator):
+        super().__init__(operator)
```

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/operator.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/place_operator.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/place_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_search_query/operators/point_radius_operator.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_search_query/operators/point_radius_operator.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_search_query/search_query.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_search_query/search_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,19 @@
 from twitter_api.types.v2_user.username import Username
 
 from .operators.cashtag_operator import CashtagOperator
 from .operators.context_operator import ContextOperator
 from .operators.conversation_id_operator import ConversationIdOperator
 from .operators.entity_operator import EntityOperator
 from .operators.from_user_operator import FromUserOperator
-from .operators.group_operator import CorrectGroupOperator, WeakGroupOperator, grouping
+from .operators.group_operator import (
+    CorrectGroupOperator,
+    GroupOperator,
+    WeakGroupOperator,
+)
 from .operators.hashtag_operator import HashtagOperator
 from .operators.in_reply_to_tweet_id_operator import InReplyToTweetIdOperator
 from .operators.keyword_operator import KeywordOperator
 from .operators.list_operator import ListOperator
 from .operators.mention_operator import MentionOperator
 from .operators.operator import CorrectOperator, Operator
 from .operators.quotes_of_tweet_id_operator import QuotesOfTweetIdOperator
@@ -89,30 +93,31 @@
     検索クエリの作成をエディタの支援を受けながら行うためのクラス。
 
     SearchQuery.build を用いて作成する。
 
     refer: https://developer.twitter.com/en/docs/twitter-api/tweets/search/integrate/build-a-query
     """
 
-    def __init__(self, *query: Operator) -> None:
+    def __init__(self, query: Operator) -> None:
         self._query = query
 
     def __str__(self) -> str:
-        return " ".join(map(grouping, self._query))
+        # ルートが Group の場合は括弧で囲まない。
+        if isinstance(self._query, GroupOperator):
+            return str(self._query._operator)
+        else:
+            return str(self._query)
 
     def __repr__(self):
-        return f"{self.__class__.__name__}({', '.join(map(repr, self._query))})"
+        return f"{self.__class__.__name__}({repr(self._query)})"
 
     @classmethod
     def build(
         cls,
-        building: Callable[
-            ["SearchQueryBuilder"],
-            CorrectOperator,
-        ],
+        building: Callable[["SearchQueryBuilder"], CorrectOperator[Operator]],
     ):
         """
         検索クエリを組み立てる。
 
         静的解析でエラーを出さずにクエリを組み立てるには、下記のルールに従う。
 
         - AND 演算（ & 結合）は左右のどちらかがクエリとして成立する場合、結合結果もクエリとして成立する。
@@ -133,15 +138,15 @@
         ...         & q.is_retweet()
         ...     )
         ... )
         >>> str(query)
         'day (#Twitter OR #Xcorp) @elonmusk -@SpaceX is:retweet'
         """
 
-        return SearchQuery(building(_SearchQueryBuilder))
+        return SearchQuery(build(building))
 
 
 class _SearchQueryBuilder(metaclass=ABCMeta):
     @abstractmethod
     def __init__(self) -> None:
         ...
 
@@ -179,35 +184,33 @@
 
         先頭に $ がない場合、 $ をつけて処理される。
         """
         return CashtagOperator(cashtag)
 
     @overload
     @classmethod
-    def group(
-        cls, operator: CorrectOperator, *operators: Operator
-    ) -> CorrectGroupOperator:
+    def group(cls, operator: CorrectOperator) -> CorrectGroupOperator:
         ...
 
     @overload
     @classmethod
-    def group(cls, operator: Operator, *operators: Operator) -> WeakGroupOperator:
+    def group(cls, operator: Operator) -> WeakGroupOperator:
         ...
 
     @classmethod
-    def group(cls, operator: Union[CorrectOperator, Operator], *operators: Operator):
+    def group(cls, operator: Union[CorrectOperator, Operator]):
         """
         括弧で囲みたい対象を指定する。括弧で囲まれた対象は優先的に計算される。
 
         要素数が 1 つの場合は括弧をつけない。
         """
         if isinstance(operator, CorrectOperator):
-            return CorrectGroupOperator(operator, *operators)
+            return CorrectGroupOperator(operator)
         else:
-            return WeakGroupOperator(operator, *operators)
+            return WeakGroupOperator(operator)
 
     @classmethod
     def from_user(cls, user: Union[UserId, Username]) -> FromUserOperator:
         """
         どのユーザからツイートされたかで絞り込む。
         """
         return FromUserOperator(user)
@@ -509,7 +512,11 @@
         return LangOperator(lang)
 
 
 SearchQueryBuilder: TypeAlias = Type[_SearchQueryBuilder]
 """
 クエリの生成関数をユーザが定義したい場合のための型定義。
 """
+
+
+def build(building: Callable[[SearchQueryBuilder], Operator]) -> Operator:
+    return building(_SearchQueryBuilder)
```

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_entities.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_entities.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_expansion.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_expansion.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_field.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_tweet/tweet_response_body.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_tweet/tweet_response_body.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_user/user.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_user/user.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/types/v2_user/user_field.py` & `twitter_api_py-0.4.3/twitter_api/types/v2_user/user_field.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/utils/_functional.py` & `twitter_api_py-0.4.3/twitter_api/utils/_functional.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/utils/_oauth.py` & `twitter_api_py-0.4.3/twitter_api/utils/_oauth.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/utils/json.py` & `twitter_api_py-0.4.3/twitter_api/utils/json.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/twitter_api/warning.py` & `twitter_api_py-0.4.3/twitter_api/warning.py`

 * *Files identical despite different names*

### Comparing `twitter_api_py-0.4.2/PKG-INFO` & `twitter_api_py-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-py
-Version: 0.4.2
+Version: 0.4.3
 Summary: Twitter API Client by Typed Python.
 Home-page: https://github.com/yassun4dev/twitter-api-py
 License: BSD-3-Clause
 Author: yassun4dev
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

