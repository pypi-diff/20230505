# Comparing `tmp/funboost-20.4-py3-none-any.whl.zip` & `tmp/funboost-20.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 1878653 bytes, number of entries: 216
--rw-rw-rw-  2.0 fat    21053 b- defN 23-Apr-26 11:46 funboost/__init__.py
+Zip file size: 1883926 bytes, number of entries: 218
+-rw-rw-rw-  2.0 fat    21081 b- defN 23-May-05 03:43 funboost/__init__.py
 -rw-rw-rw-  2.0 fat     5910 b- defN 23-Apr-28 02:46 funboost/constant.py
 -rw-rw-rw-  2.0 fat     7100 b- defN 23-Apr-27 08:42 funboost/funboost_config_deafult.py
 -rw-rw-rw-  2.0 fat    14104 b- defN 23-Apr-14 00:56 funboost/helpers.py
 -rw-rw-rw-  2.0 fat     9149 b- defN 23-Apr-13 09:47 funboost/set_frame_config.py
--rw-rw-rw-  2.0 fat     4734 b- defN 23-Apr-28 02:48 funboost/assist/user_custom_broker_register.py
 -rw-rw-rw-  2.0 fat     3930 b- defN 22-Sep-17 06:12 funboost/beggar_version_implementation/beggar_redis_consumer.py
 -rw-rw-rw-  2.0 fat      759 b- defN 22-Dec-19 11:45 funboost/concurrent_pool/__init__.py
 -rw-rw-rw-  2.0 fat     3256 b- defN 21-Dec-27 01:40 funboost/concurrent_pool/async_helper.py
 -rw-rw-rw-  2.0 fat     7227 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/async_pool_executor.py
 -rw-rw-rw-  2.0 fat     4723 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/bounded_processpoolexcutor_gt_py37.py
 -rw-rw-rw-  2.0 fat     3011 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/bounded_processpoolexcutor_py36.py
 -rw-rw-rw-  2.0 fat     1571 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/bounded_threadpoolexcutor.py
@@ -20,54 +19,56 @@
 -rw-rw-rw-  2.0 fat      373 b- defN 21-Dec-27 01:40 funboost/concurrent_pool/single_thread_executor.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-24 11:39 funboost/concurrent_pool/backup/__init__.py
 -rw-rw-rw-  2.0 fat     9548 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor0223.py
 -rw-rw-rw-  2.0 fat     9568 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor_back.py
 -rw-rw-rw-  2.0 fat     5728 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor_janus.py
 -rw-rw-rw-  2.0 fat      126 b- defN 22-Sep-17 06:12 funboost/consumers/__init__.py
 -rw-rw-rw-  2.0 fat    94018 b- defN 23-Apr-26 10:59 funboost/consumers/base_consumer.py
--rw-rw-rw-  2.0 fat     4574 b- defN 23-Apr-27 08:51 funboost/consumers/celery_consumer.py
+-rw-rw-rw-  2.0 fat    11274 b- defN 23-May-05 06:56 funboost/consumers/celery_consumer.py
+-rw-rw-rw-  2.0 fat     4574 b- defN 23-May-04 06:09 funboost/consumers/celery_consumer000.py
 -rw-rw-rw-  2.0 fat     5877 b- defN 23-Mar-29 02:19 funboost/consumers/confirm_mixin.py
--rw-rw-rw-  2.0 fat     2045 b- defN 23-Mar-23 05:32 funboost/consumers/http_consumer.py
+-rw-rw-rw-  2.0 fat     2067 b- defN 23-May-04 12:12 funboost/consumers/http_consumer.py
 -rw-rw-rw-  2.0 fat     4463 b- defN 22-Sep-17 06:12 funboost/consumers/http_consumer000.py
--rw-rw-rw-  2.0 fat     1058 b- defN 22-Sep-17 06:12 funboost/consumers/httpsqs_consumer.py
--rw-rw-rw-  2.0 fat     4196 b- defN 23-Apr-21 02:38 funboost/consumers/kafka_consumer.py
--rw-rw-rw-  2.0 fat     6536 b- defN 23-Apr-21 02:47 funboost/consumers/kafka_consumer_manually_commit.py
--rw-rw-rw-  2.0 fat    10168 b- defN 23-Apr-26 05:47 funboost/consumers/kombu_consumer.py
--rw-rw-rw-  2.0 fat     1272 b- defN 22-Sep-17 06:12 funboost/consumers/local_python_queue_consumer.py
--rw-rw-rw-  2.0 fat     1069 b- defN 22-Sep-17 06:12 funboost/consumers/mongomq_consumer.py
--rw-rw-rw-  2.0 fat     2208 b- defN 22-Sep-17 06:12 funboost/consumers/mqtt_consumer.py
--rw-rw-rw-  2.0 fat     2154 b- defN 23-Apr-28 09:20 funboost/consumers/nameko_consumer.py
--rw-rw-rw-  2.0 fat     1054 b- defN 21-Dec-27 01:40 funboost/consumers/nats_consumer.py
--rw-rw-rw-  2.0 fat     1440 b- defN 22-Sep-17 06:12 funboost/consumers/nsq_consumer.py
--rw-rw-rw-  2.0 fat     1218 b- defN 23-Mar-29 02:34 funboost/consumers/peewee_conusmer.py
--rw-rw-rw-  2.0 fat      982 b- defN 22-Sep-17 06:12 funboost/consumers/persist_queue_consumer.py
--rw-rw-rw-  2.0 fat     2394 b- defN 23-Apr-21 02:47 funboost/consumers/pulsar_consumer.py
--rw-rw-rw-  2.0 fat     1700 b- defN 23-Apr-14 09:24 funboost/consumers/rabbitmq_amqpstorm_consumer.py
--rw-rw-rw-  2.0 fat     5412 b- defN 22-Sep-17 06:12 funboost/consumers/rabbitmq_pika_consumer.py
--rw-rw-rw-  2.0 fat     4653 b- defN 22-Sep-17 06:12 funboost/consumers/rabbitmq_pika_consumerv0.py
--rw-rw-rw-  2.0 fat     1239 b- defN 22-Sep-17 06:12 funboost/consumers/rabbitmq_rabbitpy_consumer.py
--rw-rw-rw-  2.0 fat     3011 b- defN 22-Sep-17 06:12 funboost/consumers/redis_brpoplpush_consumer.py
--rw-rw-rw-  2.0 fat     2808 b- defN 23-Apr-21 02:57 funboost/consumers/redis_consumer.py
--rw-rw-rw-  2.0 fat     7560 b- defN 22-Sep-17 06:12 funboost/consumers/redis_consumer_ack_able.py
--rw-rw-rw-  2.0 fat      899 b- defN 23-Apr-28 03:12 funboost/consumers/redis_consumer_simple.py
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-May-04 12:12 funboost/consumers/httpsqs_consumer.py
+-rw-rw-rw-  2.0 fat     4217 b- defN 23-May-04 12:12 funboost/consumers/kafka_consumer.py
+-rw-rw-rw-  2.0 fat     6556 b- defN 23-May-04 12:12 funboost/consumers/kafka_consumer_manually_commit.py
+-rw-rw-rw-  2.0 fat    10186 b- defN 23-May-04 12:12 funboost/consumers/kombu_consumer.py
+-rw-rw-rw-  2.0 fat     1291 b- defN 23-May-04 12:12 funboost/consumers/local_python_queue_consumer.py
+-rw-rw-rw-  2.0 fat     1090 b- defN 23-May-04 12:12 funboost/consumers/mongomq_consumer.py
+-rw-rw-rw-  2.0 fat     2228 b- defN 23-May-04 12:12 funboost/consumers/mqtt_consumer.py
+-rw-rw-rw-  2.0 fat     2183 b- defN 23-May-04 12:12 funboost/consumers/nameko_consumer.py
+-rw-rw-rw-  2.0 fat     1076 b- defN 23-May-04 12:12 funboost/consumers/nats_consumer.py
+-rw-rw-rw-  2.0 fat     1461 b- defN 23-May-04 12:12 funboost/consumers/nsq_consumer.py
+-rw-rw-rw-  2.0 fat     1238 b- defN 23-May-04 12:12 funboost/consumers/peewee_conusmer.py
+-rw-rw-rw-  2.0 fat     1005 b- defN 23-May-04 12:12 funboost/consumers/persist_queue_consumer.py
+-rw-rw-rw-  2.0 fat     2414 b- defN 23-May-04 12:12 funboost/consumers/pulsar_consumer.py
+-rw-rw-rw-  2.0 fat     1721 b- defN 23-May-04 12:12 funboost/consumers/rabbitmq_amqpstorm_consumer.py
+-rw-rw-rw-  2.0 fat     5433 b- defN 23-May-04 12:12 funboost/consumers/rabbitmq_pika_consumer.py
+-rw-rw-rw-  2.0 fat     4674 b- defN 23-May-04 12:12 funboost/consumers/rabbitmq_pika_consumerv0.py
+-rw-rw-rw-  2.0 fat     1260 b- defN 23-May-04 12:12 funboost/consumers/rabbitmq_rabbitpy_consumer.py
+-rw-rw-rw-  2.0 fat     3031 b- defN 23-May-04 12:12 funboost/consumers/redis_brpoplpush_consumer.py
+-rw-rw-rw-  2.0 fat     2829 b- defN 23-May-04 12:12 funboost/consumers/redis_consumer.py
+-rw-rw-rw-  2.0 fat     7545 b- defN 23-May-04 12:12 funboost/consumers/redis_consumer_ack_able.py
+-rw-rw-rw-  2.0 fat      922 b- defN 23-May-04 12:12 funboost/consumers/redis_consumer_simple.py
 -rw-rw-rw-  2.0 fat     7135 b- defN 22-Sep-17 06:12 funboost/consumers/redis_filter.py
--rw-rw-rw-  2.0 fat     1184 b- defN 22-Sep-17 06:12 funboost/consumers/redis_pubsub_consumer.py
--rw-rw-rw-  2.0 fat     6304 b- defN 21-Dec-27 03:47 funboost/consumers/redis_stream_consumer.py
--rw-rw-rw-  2.0 fat     1633 b- defN 23-Mar-23 05:32 funboost/consumers/rocketmq_consumer.py
--rw-rw-rw-  2.0 fat     1289 b- defN 22-Sep-17 06:12 funboost/consumers/sqlachemy_consumer.py
--rw-rw-rw-  2.0 fat     2025 b- defN 22-Sep-17 06:12 funboost/consumers/tcp_consumer.py
--rw-rw-rw-  2.0 fat     1322 b- defN 22-Sep-17 08:52 funboost/consumers/txt_file_consumer.py
--rw-rw-rw-  2.0 fat     1625 b- defN 22-Sep-17 06:12 funboost/consumers/udp_consumer.py
--rw-rw-rw-  2.0 fat     4137 b- defN 23-Mar-23 05:34 funboost/consumers/zeromq_consumer.py
+-rw-rw-rw-  2.0 fat     1206 b- defN 23-May-04 12:12 funboost/consumers/redis_pubsub_consumer.py
+-rw-rw-rw-  2.0 fat     6324 b- defN 23-May-04 12:12 funboost/consumers/redis_stream_consumer.py
+-rw-rw-rw-  2.0 fat     1653 b- defN 23-May-04 12:12 funboost/consumers/rocketmq_consumer.py
+-rw-rw-rw-  2.0 fat     1309 b- defN 23-May-04 12:12 funboost/consumers/sqlachemy_consumer.py
+-rw-rw-rw-  2.0 fat     2045 b- defN 23-May-04 12:12 funboost/consumers/tcp_consumer.py
+-rw-rw-rw-  2.0 fat     1340 b- defN 23-May-04 12:12 funboost/consumers/txt_file_consumer.py
+-rw-rw-rw-  2.0 fat     1643 b- defN 23-May-04 12:12 funboost/consumers/udp_consumer.py
+-rw-rw-rw-  2.0 fat     4157 b- defN 23-May-04 12:12 funboost/consumers/zeromq_consumer.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Dec-05 10:31 funboost/contrib/__init__.py
 -rw-rw-rw-  2.0 fat     4703 b- defN 23-Mar-29 03:02 funboost/contrib/queue2queue.py
 -rw-rw-rw-  2.0 fat     1817 b- defN 23-Mar-22 02:09 funboost/contrib/redis_consume_latest_msg_broker.py
 -rw-rw-rw-  2.0 fat      178 b- defN 22-Sep-17 06:12 funboost/factories/__init__.py
--rw-rw-rw-  2.0 fat     3357 b- defN 23-Apr-28 02:46 funboost/factories/consumer_factory.py
--rw-rw-rw-  2.0 fat     4587 b- defN 23-Apr-28 01:33 funboost/factories/publisher_factotry.py
+-rw-rw-rw-  2.0 fat     8286 b- defN 23-May-05 06:22 funboost/factories/broker_kind__publsiher_consumer_type_map.py
+-rw-rw-rw-  2.0 fat     1032 b- defN 23-May-05 03:52 funboost/factories/consumer_factory.py
+-rw-rw-rw-  2.0 fat     2115 b- defN 23-May-05 06:20 funboost/factories/publisher_factotry.py
 -rw-rw-rw-  2.0 fat     4841 b- defN 22-Sep-17 06:12 funboost/function_result_web/app.py
 -rw-rw-rw-  2.0 fat     7345 b- defN 23-Mar-08 10:19 funboost/function_result_web/functions.py
 -rw-rw-rw-  2.0 fat     4045 b- defN 22-Feb-21 07:34 funboost/function_result_web/__pycache__/app.cpython-37.pyc
 -rw-rw-rw-  2.0 fat     3921 b- defN 22-Mar-30 13:56 funboost/function_result_web/__pycache__/functions.cpython-37.pyc
 -rw-rw-rw-  2.0 fat     7674 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/assets/css/custom.css
 -rw-rw-rw-  2.0 fat    42839 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/assets/css/jquery.mCustomScrollbar.min.css
 -rw-rw-rw-  2.0 fat    23610 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/assets/img/user.jpg
@@ -79,17 +80,18 @@
 -rw-rw-rw-  2.0 fat     2912 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/tick.png
 -rw-rw-rw-  2.0 fat      622 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/user.png
 -rw-rw-rw-  2.0 fat    96383 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/js/jquery-1.11.0.min.js
 -rw-rw-rw-  2.0 fat    19501 b- defN 22-Feb-21 12:32 funboost/function_result_web/templates/index.html
 -rw-rw-rw-  2.0 fat     2007 b- defN 21-Dec-27 01:40 funboost/function_result_web/templates/login.html
 -rw-rw-rw-  2.0 fat      131 b- defN 22-Sep-17 06:12 funboost/publishers/__init__.py
 -rw-rw-rw-  2.0 fat    14894 b- defN 23-Apr-21 09:06 funboost/publishers/base_publisher.py
--rw-rw-rw-  2.0 fat     3897 b- defN 23-Apr-28 09:23 funboost/publishers/celery_publisher.py
+-rw-rw-rw-  2.0 fat     3660 b- defN 23-May-04 07:41 funboost/publishers/celery_publisher.py
+-rw-rw-rw-  2.0 fat     3897 b- defN 23-May-04 06:09 funboost/publishers/celery_publisher000.py
 -rw-rw-rw-  2.0 fat     3541 b- defN 23-Mar-23 05:32 funboost/publishers/confluent_kafka_publisher.py
--rw-rw-rw-  2.0 fat      777 b- defN 22-Sep-17 06:12 funboost/publishers/http_publisher.py
+-rw-rw-rw-  2.0 fat      753 b- defN 23-May-04 11:53 funboost/publishers/http_publisher.py
 -rw-rw-rw-  2.0 fat     2783 b- defN 22-Sep-17 06:12 funboost/publishers/httpsqs_publisher.py
 -rw-rw-rw-  2.0 fat     2160 b- defN 23-Apr-03 10:55 funboost/publishers/kafka_publisher.py
 -rw-rw-rw-  2.0 fat     5246 b- defN 23-Apr-21 09:40 funboost/publishers/kombu_publisher.py
 -rw-rw-rw-  2.0 fat     1365 b- defN 22-Sep-17 06:12 funboost/publishers/local_python_queue_publisher.py
 -rw-rw-rw-  2.0 fat     1874 b- defN 23-Mar-14 02:56 funboost/publishers/mongomq_publisher.py
 -rw-rw-rw-  2.0 fat     3050 b- defN 22-Sep-17 06:12 funboost/publishers/mqtt_publisher.py
 -rw-rw-rw-  2.0 fat     7782 b- defN 23-Mar-31 03:13 funboost/publishers/msg_result_getter.py
@@ -105,21 +107,21 @@
 -rw-rw-rw-  2.0 fat     3929 b- defN 23-Apr-21 02:47 funboost/publishers/redis_publisher.py
 -rw-rw-rw-  2.0 fat      278 b- defN 22-Sep-17 06:12 funboost/publishers/redis_publisher_lpush.py
 -rw-rw-rw-  2.0 fat      872 b- defN 23-Apr-28 03:12 funboost/publishers/redis_publisher_simple.py
 -rw-rw-rw-  2.0 fat      721 b- defN 22-Sep-17 06:12 funboost/publishers/redis_pubsub_publisher.py
 -rw-rw-rw-  2.0 fat     2037 b- defN 21-Dec-27 01:40 funboost/publishers/redis_stream_publisher.py
 -rw-rw-rw-  2.0 fat     2343 b- defN 23-Mar-23 05:32 funboost/publishers/rocketmq_publisher.py
 -rw-rw-rw-  2.0 fat     1215 b- defN 22-Sep-17 06:12 funboost/publishers/sqla_queue_publisher.py
--rw-rw-rw-  2.0 fat     1359 b- defN 22-Sep-17 06:12 funboost/publishers/tcp_publisher.py
+-rw-rw-rw-  2.0 fat     1335 b- defN 23-May-04 11:53 funboost/publishers/tcp_publisher.py
 -rw-rw-rw-  2.0 fat     1380 b- defN 22-Sep-17 08:52 funboost/publishers/txt_file_publisher.py
--rw-rw-rw-  2.0 fat     1218 b- defN 22-Sep-17 06:12 funboost/publishers/udp_publisher.py
+-rw-rw-rw-  2.0 fat     1194 b- defN 23-May-04 11:53 funboost/publishers/udp_publisher.py
 -rw-rw-rw-  2.0 fat     1002 b- defN 21-Dec-27 01:40 funboost/publishers/zeromq_publisher.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-22 02:44 funboost/queues/__init__.py
 -rw-rw-rw-  2.0 fat     4982 b- defN 22-Aug-08 05:06 funboost/queues/peewee_queue.py
--rw-rw-rw-  2.0 fat    11186 b- defN 23-Mar-23 05:32 funboost/queues/sqla_queue.py
+-rw-rw-rw-  2.0 fat    11024 b- defN 23-May-05 02:38 funboost/queues/sqla_queue.py
 -rw-rw-rw-  2.0 fat     4098 b- defN 23-Mar-27 02:03 funboost/timing_job/__init__.py
 -rw-rw-rw-  2.0 fat      418 b- defN 23-Apr-06 06:09 funboost/timing_job/apscheduler_use_mysql_store.py
 -rw-rw-rw-  2.0 fat      868 b- defN 23-Feb-03 06:47 funboost/timing_job/apscheduler_use_redis_store.py
 -rw-rw-rw-  2.0 fat      996 b- defN 22-Aug-19 01:51 funboost/timing_job/push_fun_for_apscheduler_use_db.py
 -rw-rw-rw-  2.0 fat     1951 b- defN 23-Mar-09 07:27 funboost/utils/__init__.py
 -rw-rw-rw-  2.0 fat     3124 b- defN 21-Dec-27 01:40 funboost/utils/apscheduler_monkey.py
 -rw-rw-rw-  2.0 fat       96 b- defN 23-Jan-29 07:41 funboost/utils/block_exit.py
@@ -206,13 +208,13 @@
 -rw-rw-rw-  2.0 fat      303 b- defN 23-Mar-13 01:28 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-37.pyc
 -rw-rw-rw-  2.0 fat      311 b- defN 23-Mar-21 10:43 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-39.pyc
 -rw-rw-rw-  2.0 fat      909 b- defN 21-Dec-27 01:40 funboost/utils/pysnooper_ydf/__init__.py
 -rw-rw-rw-  2.0 fat     2243 b- defN 21-Dec-27 01:40 funboost/utils/pysnooper_ydf/pycompat.py
 -rw-rw-rw-  2.0 fat    19131 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/tracer.py
 -rw-rw-rw-  2.0 fat     2753 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/utils.py
 -rw-rw-rw-  2.0 fat     3693 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/variables.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Apr-28 10:43 funboost-20.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    24442 b- defN 23-Apr-28 10:43 funboost-20.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Apr-28 10:43 funboost-20.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-28 10:43 funboost-20.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    23845 b- defN 23-Apr-28 10:43 funboost-20.4.dist-info/RECORD
-216 files, 3222090 bytes uncompressed, 1838989 bytes compressed:  42.9%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-05 08:56 funboost-20.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    25817 b- defN 23-May-05 08:56 funboost-20.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-May-05 08:56 funboost-20.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-05 08:56 funboost-20.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    24059 b- defN 23-May-05 08:56 funboost-20.5.dist-info/RECORD
+218 files, 3237751 bytes uncompressed, 1843914 bytes compressed:  43.1%
```

## zipnote {}

```diff
@@ -9,17 +9,14 @@
 
 Filename: funboost/helpers.py
 Comment: 
 
 Filename: funboost/set_frame_config.py
 Comment: 
 
-Filename: funboost/assist/user_custom_broker_register.py
-Comment: 
-
 Filename: funboost/beggar_version_implementation/beggar_redis_consumer.py
 Comment: 
 
 Filename: funboost/concurrent_pool/__init__.py
 Comment: 
 
 Filename: funboost/concurrent_pool/async_helper.py
@@ -72,14 +69,17 @@
 
 Filename: funboost/consumers/base_consumer.py
 Comment: 
 
 Filename: funboost/consumers/celery_consumer.py
 Comment: 
 
+Filename: funboost/consumers/celery_consumer000.py
+Comment: 
+
 Filename: funboost/consumers/confirm_mixin.py
 Comment: 
 
 Filename: funboost/consumers/http_consumer.py
 Comment: 
 
 Filename: funboost/consumers/http_consumer000.py
@@ -183,14 +183,17 @@
 
 Filename: funboost/contrib/redis_consume_latest_msg_broker.py
 Comment: 
 
 Filename: funboost/factories/__init__.py
 Comment: 
 
+Filename: funboost/factories/broker_kind__publsiher_consumer_type_map.py
+Comment: 
+
 Filename: funboost/factories/consumer_factory.py
 Comment: 
 
 Filename: funboost/factories/publisher_factotry.py
 Comment: 
 
 Filename: funboost/function_result_web/app.py
@@ -249,14 +252,17 @@
 
 Filename: funboost/publishers/base_publisher.py
 Comment: 
 
 Filename: funboost/publishers/celery_publisher.py
 Comment: 
 
+Filename: funboost/publishers/celery_publisher000.py
+Comment: 
+
 Filename: funboost/publishers/confluent_kafka_publisher.py
 Comment: 
 
 Filename: funboost/publishers/http_publisher.py
 Comment: 
 
 Filename: funboost/publishers/httpsqs_publisher.py
@@ -627,23 +633,23 @@
 
 Filename: funboost/utils/pysnooper_ydf/utils.py
 Comment: 
 
 Filename: funboost/utils/pysnooper_ydf/variables.py
 Comment: 
 
-Filename: funboost-20.4.dist-info/LICENSE
+Filename: funboost-20.5.dist-info/LICENSE
 Comment: 
 
-Filename: funboost-20.4.dist-info/METADATA
+Filename: funboost-20.5.dist-info/METADATA
 Comment: 
 
-Filename: funboost-20.4.dist-info/WHEEL
+Filename: funboost-20.5.dist-info/WHEEL
 Comment: 
 
-Filename: funboost-20.4.dist-info/top_level.txt
+Filename: funboost-20.5.dist-info/top_level.txt
 Comment: 
 
-Filename: funboost-20.4.dist-info/RECORD
+Filename: funboost-20.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## funboost/__init__.py

```diff
@@ -10,26 +10,28 @@
 # noinspection PyUnresolvedReferences
 import nb_log
 from funboost.set_frame_config import patch_frame_config, show_frame_config
 from funboost.funboost_config_deafult import BoostDecoratorDefaultParams
 from funboost.helpers import (fabric_deploy, kill_all_remote_tasks,
                               multi_process_pub_params_list,
                               run_consumer_with_multi_process)
-from funboost.assist.user_custom_broker_register import register_custom_broker
+
 from funboost.utils.paramiko_util import ParamikoFolderUploader
 from funboost.consumers.base_consumer import (ExceptionForRequeue, ExceptionForRetry, ExceptionForPushToDlxqueue,
                                               AbstractConsumer, ConsumersManager,
                                               FunctionResultStatusPersistanceConfig,
                                               wait_for_possible_has_finish_all_tasks_by_conusmer_list,
                                               ActiveCousumerProcessInfoGetter, FunctionResultStatus)
 from funboost.publishers.base_publisher import (PriorityConsumingControlConfig,
                                                 AbstractPublisher, AsyncResult, HasNotAsyncResult, AioAsyncResult, ResultFromMongo)
+from funboost.factories.broker_kind__publsiher_consumer_type_map import register_custom_broker
 from funboost.factories.publisher_factotry import get_publisher
 from funboost.factories.consumer_factory import get_consumer
 
+
 # noinspection PyUnresolvedReferences
 from funboost.utils import nb_print, patch_print, LogManager, get_logger, LoggerMixin
 from funboost.timing_job import fsdf_background_scheduler, timing_publish_deco
 from funboost.constant import BrokerEnum, ConcurrentModeEnum
 
 
 # 有的包默认没加handlers，原始的日志不漂亮且不可跳转不知道哪里发生的。这里把warnning级别以上的日志默认加上handlers。
@@ -294,18 +296,18 @@
         func.push = func.delay = consumer.publisher_of_same_queue.push
         func.multi_process_pub_params_list = partial(multi_process_pub_params_list, func)
         func.clear = func.clear_queue = consumer.publisher_of_same_queue.clear
         func.get_message_count = consumer.publisher_of_same_queue.get_message_count
 
         func.start_consuming_message = func.consume = func.start = consumer.start_consuming_message
         func.multi_process_start = func.multi_process_consume = partial(run_consumer_with_multi_process, func)
-        if broker_kind == BrokerEnum.CELERY:   # celery作为消息队列
-            from multiprocessing import set_start_method
-            set_start_method('spawn', force=True)  # linux上运行需要这样。
-            func.consume = partial(func.multi_process_consume, 1)
+        # if broker_kind == BrokerEnum.CELERY:   # celery作为消息队列
+        #     from multiprocessing import set_start_method
+        #     set_start_method('spawn', force=True)  # linux上运行需要这样。
+        #     func.consume = partial(func.multi_process_consume, 1)
 
         func.fabric_deploy = partial(fabric_deploy, func)
 
         func.clear_filter_tasks = consumer.clear_filter_tasks
 
         func.wait_for_possible_has_finish_all_tasks = consumer.wait_for_possible_has_finish_all_tasks
```

## funboost/consumers/celery_consumer.py

```diff
@@ -1,122 +1,271 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:32
+import os
+import sys
 import threading
-
+import typing
 from functools import partial
-
+from nb_log import get_logger
+from funboost.constant import BrokerEnum
 from funboost import funboost_config_deafult
-
 from funboost.consumers.base_consumer import AbstractConsumer
-import celery
+from funboost.publishers.celery_publisher import celery_app
+from funboost.constant import ConcurrentModeEnum
 
 
 class CeleryConsumer(AbstractConsumer):
     """
     celery作为中间件实现的。
     """
-    BROKER_KIND = 30
-    BROKER_EXCLUSIVE_CONFIG_DEFAULT = {'celery_app_config': {}}
-
-    # celery的可以配置项大全  https://docs.celeryq.dev/en/stable/userguide/configuration.html#new-lowercase-settings
-
-    def _shedual_task(self):
-        raw_fun = self.consuming_function
 
-        celery_app = celery.Celery(broker=funboost_config_deafult.CELERY_BROKER_URL,
-                                   backend=funboost_config_deafult.CELERY_RESULT_BACKEND,
-                                   task_routes={},timezone=funboost_config_deafult.TIMEZONE,enable_utc=False)
-        celery_app.config_from_object(self.broker_exclusive_config['celery_app_config'])
-        celery_app.conf.task_routes.update({self.queue_name: {"queue": self.queue_name}})
+    BROKER_EXCLUSIVE_CONFIG_DEFAULT = {'celery_task_config': {}}
 
-        celery_app.conf.task_reject_on_worker_lost = True  # 配置这两项可以随意停止
-        celery_app.conf.task_acks_late = True
+    # celery的可以配置项大全  https://docs.celeryq.dev/en/stable/userguide/configuration.html#new-lowercase-settings
+    # celery @app.task() 所有可以配置项可以看  D:\ProgramData\Miniconda3\Lib\site-packages\celery\app\task.py
 
-        # celery_app.conf.worker_task_log_format = '%(asctime)s - %(name)s - "%(pathname)s:%(lineno)d" - %(funcName)s - %(levelname)s - %(message)s'
-        # celery_app.conf.worker_log_format = '%(asctime)s - %(name)s - "%(pathname)s:%(lineno)d" - %(funcName)s - %(levelname)s - %(message)s'
+    '''
+        #: Execution strategy used, or the qualified name of one.
+        Strategy = 'celery.worker.strategy:default'
+
+        #: Request class used, or the qualified name of one.
+        Request = 'celery.worker.request:Request'
+
+        #: The application instance associated with this task class.
+        _app = None
+
+        #: Name of the task.
+        name = None
+
+        #: Enable argument checking.
+        #: You can set this to false if you don't want the signature to be
+        #: checked when calling the task.
+        #: Defaults to :attr:`app.strict_typing <@Celery.strict_typing>`.
+        typing = None
+
+        #: Maximum number of retries before giving up.  If set to :const:`None`,
+        #: it will **never** stop retrying.
+        max_retries = 3
+
+        #: Default time in seconds before a retry of the task should be
+        #: executed.  3 minutes by default.
+        default_retry_delay = 3 * 60
+
+        #: Rate limit for this task type.  Examples: :const:`None` (no rate
+        #: limit), `'100/s'` (hundred tasks a second), `'100/m'` (hundred tasks
+        #: a minute),`'100/h'` (hundred tasks an hour)
+        rate_limit = None
+
+        #: If enabled the worker won't store task state and return values
+        #: for this task.  Defaults to the :setting:`task_ignore_result`
+        #: setting.
+        ignore_result = None
+
+        #: If enabled the request will keep track of subtasks started by
+        #: this task, and this information will be sent with the result
+        #: (``result.children``).
+        trail = True
+
+        #: If enabled the worker will send monitoring events related to
+        #: this task (but only if the worker is configured to send
+        #: task related events).
+        #: Note that this has no effect on the task-failure event case
+        #: where a task is not registered (as it will have no task class
+        #: to check this flag).
+        send_events = True
+
+        #: When enabled errors will be stored even if the task is otherwise
+        #: configured to ignore results.
+        store_errors_even_if_ignored = None
+
+        #: The name of a serializer that are registered with
+        #: :mod:`kombu.serialization.registry`.  Default is `'json'`.
+        serializer = None
+
+        #: Hard time limit.
+        #: Defaults to the :setting:`task_time_limit` setting.
+        time_limit = None
+
+        #: Soft time limit.
+        #: Defaults to the :setting:`task_soft_time_limit` setting.
+        soft_time_limit = None
+
+        #: The result store backend used for this task.
+        backend = None
+
+        #: If enabled the task will report its status as 'started' when the task
+        #: is executed by a worker.  Disabled by default as the normal behavior
+        #: is to not report that level of granularity.  Tasks are either pending,
+        #: finished, or waiting to be retried.
+        #:
+        #: Having a 'started' status can be useful for when there are long
+        #: running tasks and there's a need to report what task is currently
+        #: running.
+        #:
+        #: The application default can be overridden using the
+        #: :setting:`task_track_started` setting.
+        track_started = None
+
+        #: When enabled messages for this task will be acknowledged **after**
+        #: the task has been executed, and not *just before* (the
+        #: default behavior).
+        #:
+        #: Please note that this means the task may be executed twice if the
+        #: worker crashes mid execution.
+        #:
+        #: The application default can be overridden with the
+        #: :setting:`task_acks_late` setting.
+        acks_late = None
+
+        #: When enabled messages for this task will be acknowledged even if it
+        #: fails or times out.
+        #:
+        #: Configuring this setting only applies to tasks that are
+        #: acknowledged **after** they have been executed and only if
+        #: :setting:`task_acks_late` is enabled.
+        #:
+        #: The application default can be overridden with the
+        #: :setting:`task_acks_on_failure_or_timeout` setting.
+        acks_on_failure_or_timeout = None
+
+        #: Even if :attr:`acks_late` is enabled, the worker will
+        #: acknowledge tasks when the worker process executing them abruptly
+        #: exits or is signaled (e.g., :sig:`KILL`/:sig:`INT`, etc).
+        #:
+        #: Setting this to true allows the message to be re-queued instead,
+        #: so that the task will execute again by the same worker, or another
+        #: worker.
+        #:
+        #: Warning: Enabling this can cause message loops; make sure you know
+        #: what you're doing.
+        reject_on_worker_lost = None
+
+        #: Tuple of expected exceptions.
+        #:
+        #: These are errors that are expected in normal operation
+        #: and that shouldn't be regarded as a real error by the worker.
+        #: Currently this means that the state will be updated to an error
+        #: state, but the worker won't log the event as an error.
+        throws = ()
+
+        #: Default task expiry time.
+        expires = None
+
+        #: Default task priority.
+        priority = None
+
+        #: Max length of result representation used in logs and events.
+        resultrepr_maxsize = 1024
+
+        #: Task request stack, the current request will be the topmost.
+        request_stack = None
+    '''
+
+    def custom_init(self):
+        @celery_app.task(name=self.queue_name, rate_limit=f'{self._qps}/s', soft_time_limit=self._function_timeout,
+                         max_retries=self._max_retry_times,
+                         **self.broker_exclusive_config['celery_task_config'])
+        def f(*args, **kwargs):
+            self.logger.debug(f' 这条消息是 celery 从 {self.queue_name} 队列中取出 ,将由 celery 框架处理: args:  {args} ,  kwargs: {kwargs}')
+            return self.consuming_function(*args, **kwargs)
 
-        celery_app.conf.worker_redirect_stdouts = False
+        CeleryHelper.concurrent_mode = self._concurrent_mode
 
-        @celery_app.task(name=self.queue_name)
-        def f(*args, **kwargs):
-            # func_params = json.loads(msg)
-            # func_params.pop('extra')
-            # return raw_fun(**func_params)
-            # print(args)
-            # print(kwargs)
-            self.logger.debug(f' 这条消息将由 funboost 在 celery 框架中处理: args:  {args} ,  kwargs: {kwargs}')
-            return raw_fun(*args, **kwargs)
-
-        # celery_app.worker_main(
-        #     argv=['worker', '--pool=threads', '--concurrency=500', '-n', 'worker1@%h', '--loglevel=INFO',
-        #           f'--queues={self.queue_name}',
-        #           ])
+        # print(type(f), dir(f), f.__dict__)
 
-        # logging.getLevelName(self._log_level)
-        celery_app.worker_main(
-            argv=['worker', '--pool=threads', f'--concurrency={self._concurrent_num}',
-                  '-n', f'worker_{self.queue_name}@%h', f'--loglevel=INFO',
-                  f'--queues={self.queue_name}',
-                  ])
+    # def _shedual_task000(self):
+    #     """ 建议使用 batch_start_celery_consumers([f1,f2]) ,而不是 f1.consume()  f2.consume() 方式"""
+    #
+    #     # # celery_app.worker_main(
+    #     # #     argv=['worker', '--pool=threads', '--concurrency=500', '-n', 'worker1@%h', '--loglevel=INFO',
+    #     # #           f'--queues={self.queue_name}',
+    #     # #           ])
+    #     #
+    #     # # logging.getLevelName(self._log_level)
+    #     def f():
+    #         celery_app.worker_main(
+    #             argv=['worker', '--pool=threads', f'--concurrency={self._concurrent_num}',
+    #                   '-n', f'worker_{self.queue_name}@%h', f'--loglevel=INFO',
+    #                   f'--queues={self.queue_name}',
+    #                   ])
+    #
+    #     # threading.Thread(target=f).start()
+    #     f()
+    #     #
+    #     # # worker = celery_app.Worker()
+    #     # # worker.start()
+    #     # raise Exception('不建议这样启动')
 
-        # worker = celery_app.Worker()
-        # worker.start()
+    def _shedual_task(self):
+        # 不单独每个函数都启动一次celery的worker消费，是把要消费的 queue name放到列表中，realy_start_celery_worker 一次性启动多个函数消费。
+        CeleryHelper.to_be_start_work_celery_queue_name_list.append(self.queue_name)
 
     def _confirm_consume(self, kw):
         pass
 
     def _requeue(self, kw):
         pass
 
 
-class CeleryBeatHelper:
-    def __init__(self, beat_schedule: dict):
-        '''
-
-        celery_app.conf.beat_schedule = {
-    'add-every-30-seconds': {
-        'task': '求和啊',
-        'schedule': timedelta(seconds=2),
-        'args': (10000, 20000)
-    }}
-        :param beat_schedule:
-        '''
-        self.beat_schedule = beat_schedule
-        self.celery_app = None
-
-    def get_celery_app(self):
-        celery_app = celery.Celery(broker=funboost_config_deafult.CELERY_BROKER_URL,
-                                   backend=funboost_config_deafult.CELERY_RESULT_BACKEND,
-                                   task_routes={},timezone=funboost_config_deafult.TIMEZONE,enable_utc=False)
-
-        for k, v in self.beat_schedule.items():
-            queue_name = v['task']
-
-            @celery_app.task(name=queue_name)
-            def f(*args, **kwargs):
-                pass
-
-            celery_app.conf.task_routes.update({queue_name: {"queue": queue_name}})
-        celery_app.conf.beat_schedule = self.beat_schedule
-        # celery_app.worker_main(
-        #     argv=['worker','beat',
-        #           f'--loglevel=INFO',
-        #           ])
-        self.celery_app = celery_app
-        return celery_app
-
-    def start_beat(self):
-        '''
-        celery -A test_celery_beat beat
-        '''
-        beat = partial(self.celery_app.Beat, loglevel='INFO',
-                       )
-        beat().run()
-
-
-def celery_start_beat(beat_schedule: dict):
-    def _f():
-        celery_beat_helper = CeleryBeatHelper(beat_schedule)
-        celery_app = celery_beat_helper.get_celery_app()
-        celery_beat_helper.start_beat()
-    threading.Thread(target=_f).start() # 使得可以很方便启动定时任务，继续启动函数消费
+class CeleryHelper:
+    celery_app = celery_app
+    to_be_start_work_celery_queue_name_list = []  # 存放需要worker运行的queue name。
+    to_be_start_work_celery_queue_name__conmsumer_map = {}
+    logger = get_logger('funboost.CeleryHelper')
+    concurrent_mode = None
+
+    @staticmethod
+    def update_celery_app_conf(celery_app_conf: dict):
+        """
+        更新celery app的配置，celery app配置大全见 https://docs.celeryq.dev/en/stable/userguide/configuration.html
+        :param celery_app_conf:
+        :return:
+        """
+        celery_app.conf.update(celery_app_conf)
+
+    @staticmethod
+    def celery_start_beat(beat_schedule: dict):
+        celery_app.conf.beat_schedule = beat_schedule  # 配置celery定时任务
+
+        def _f():
+            beat = partial(celery_app.Beat, loglevel='INFO', )
+            beat().run()
+
+        threading.Thread(target=_f).start()  # 使得可以很方便启动定时任务，继续启动函数消费
+
+    @staticmethod
+    def start_flower(port=5555):
+        def _f():
+            python_executable = sys.executable
+            # print(python_executable)
+
+            # cmd = f'''{python_executable} -m celery -A funboost.publishers.celery_publisher --broker={funboost_config_deafult.CELERY_BROKER_URL}  --result-backend={funboost_config_deafult.CELERY_RESULT_BACKEND}   flower --address=0.0.0.0 --port={port}  --auto_refresh=True '''
+            cmd = f'''{python_executable} -m celery  --broker={funboost_config_deafult.CELERY_BROKER_URL}  --result-backend={funboost_config_deafult.CELERY_RESULT_BACKEND}   flower --address=0.0.0.0 --port={port}  --auto_refresh=1 '''
+
+            print(f'启动flower命令:   {cmd}')
+            os.system(cmd)
+
+        threading.Thread(target=_f).start()
+
+    @classmethod
+    def realy_start_celery_worker(cls, worker_name=None):
+        queue_names_str = ','.join(cls.to_be_start_work_celery_queue_name_list)
+        # '--concurrency=200',
+        # '--autoscale=5,500' threads 并发模式不支持自动扩大缩小并发数量,
+        worker_name = worker_name or f'pid_{os.getpid()}'
+        pool_name = 'threads'
+        if cls.concurrent_mode == ConcurrentModeEnum.GEVENT:
+            pool_name = 'gevent'
+        if cls.concurrent_mode == ConcurrentModeEnum.EVENTLET:
+            pool_name = 'eventlet'
+        celery_app.worker_main(
+            argv=['worker', f'--pool={pool_name}', '--concurrency=200',
+                  '-n', f'worker_funboost_{worker_name}@%h', f'--loglevel=INFO',
+                  f'--queues={queue_names_str}',
+                  ])
+
+    @classmethod
+    def show_celery_app_conf(cls):
+        cls.logger.debug('展示celery app的配置')
+        for k, v in celery_app.conf.items():
+            print(k, ' : ', v)
```

## funboost/consumers/http_consumer.py

```diff
@@ -3,22 +3,23 @@
 # @Time    : 2022/8/8 0008 13:32
 import asyncio
 import json
 
 from aiohttp import web
 from aiohttp.web_request import Request
 
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 
 
 class HTTPConsumer(AbstractConsumer, ):
     """
     http 实现消息队列，不支持持久化，但不需要安装软件。
     """
-    BROKER_KIND = 23
+
 
     # noinspection PyAttributeOutsideInit
     def custom_init(self):
         try:
             self._ip, self._port = self.queue_name.split(':')
             self._port = int(self._port)
         except BaseException as e:
```

## funboost/consumers/httpsqs_consumer.py

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:32
 import json
 import time
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.publishers.httpsqs_publisher import HttpsqsPublisher
 
 
 class HttpsqsConsumer(AbstractConsumer):
     """
     httpsqs作为中间件
     """
-    BROKER_KIND = 18
+
 
     def custom_init(self):
         # noinspection PyAttributeOutsideInit
         self.httpsqs_publisher = HttpsqsPublisher(self._queue_name)
 
     # noinspection DuplicatedCode
     def _shedual_task(self):
```

## funboost/consumers/kafka_consumer.py

```diff
@@ -4,30 +4,30 @@
 import json
 # noinspection PyPackageRequirements
 from kafka import KafkaConsumer as OfficialKafkaConsumer, KafkaProducer, KafkaAdminClient
 # noinspection PyPackageRequirements
 from kafka.admin import NewTopic
 # noinspection PyPackageRequirements
 from kafka.errors import TopicAlreadyExistsError
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost import funboost_config_deafult
 from nb_log import get_logger, LogManager
 
 # LogManager('kafka').get_logger_and_add_handlers(30)
 get_logger('kafka', log_level_int=30)
 
 
 class KafkaConsumer(AbstractConsumer):
     """
     kafka作为中间件实现的。自动确认消费，最多消费一次，随意重启会丢失正在大批正在运行的任务。推荐使用 confluent_kafka 中间件，kafka_consumer_manually_commit.py。
 
     可以让消费函数内部 sleep60秒，突然停止消费代码，使用 kafka-consumer-groups.sh --bootstrap-server 127.0.0.1:9092 --describe --group funboost 来证实自动确认消费和手动确认消费的区别。
     """
-    BROKER_KIND = 8
+
     BROKER_EXCLUSIVE_CONFIG_DEFAULT = {'group_id':'funboost_kafka','auto_offset_reset':'earliest'}
     # not_all_brokers_general_settings配置 ，支持独立的中间件配置参数是 group_id 和 auto_offset_reset
     """
     auto_offset_reset 介绍
       auto_offset_reset (str): A policy for resetting offsets on
             OffsetOutOfRange errors: 'earliest' will move to the oldest
             available message, 'latest' will move to the most recent. Any
```

## funboost/consumers/kafka_consumer_manually_commit.py

```diff
@@ -11,28 +11,28 @@
 # noinspection PyPackageRequirements
 from kafka import KafkaProducer, KafkaAdminClient
 
 # noinspection PyPackageRequirements
 from kafka.admin import NewTopic
 # noinspection PyPackageRequirements
 from kafka.errors import TopicAlreadyExistsError
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost import funboost_config_deafult
 
 
 class KafkaConsumerManuallyCommit(AbstractConsumer):
     """
     confluent_kafla作为中间件实现的。操作kafka中间件的速度比kafka-python快10倍。
     这个是自动间隔2秒的手动确认，由于是异步在并发池中并发消费，可以防止强制关闭程序造成正在运行的任务丢失，比自动commit好。
     如果使用kafka，推荐这个。
 
     可以让消费函数内部 sleep 60秒，突然停止消费代码，使用 kafka-consumer-groups.sh --bootstrap-server 127.0.0.1:9092 --describe --group frame_group 来证实自动确认消费和手动确认消费的区别。
     """
-    BROKER_KIND = 16
+
     BROKER_EXCLUSIVE_CONFIG_DEFAULT = {'group_id':'funboost_confluent_kafka','auto_offset_reset':'earliest'}
 
     def _shedual_task(self):
 
         from confluent_kafka import Consumer as ConfluentConsumer  # 这个包在win下不好安装，用户用这个中间件的时候自己再想办法安装。win用户需要安装c++ 14.0以上环境。
         try:
             admin_client = KafkaAdminClient(bootstrap_servers=funboost_config_deafult.KAFKA_BOOTSTRAP_SERVERS)
```

## funboost/consumers/kombu_consumer.py

```diff
@@ -10,15 +10,15 @@
 from kombu.connection import Connection
 from kombu.transport.virtual.base import Channel
 from kombu.transport.virtual.base import Message
 from kombu.transport import redis
 from kombu.transport.redis import Empty
 
 from nb_log import get_logger
-
+from funboost.constant import BrokerEnum
 from funboost import funboost_config_deafult
 from funboost.consumers.base_consumer import AbstractConsumer
 
 
 def patch_kombu_redis000():
     # 这个也可以，代码长了一点。
     """
@@ -128,15 +128,14 @@
 
 # noinspection PyAttributeOutsideInit
 class KombuConsumer(AbstractConsumer, ):
     """
     使用kombu作为中间件,这个能直接一次性支持很多种小众中间件，但性能很差，除非是分布式函数调度框架没实现的中间件种类用户才可以用这种，用户也可以自己对比性能。
     """
 
-    BROKER_KIND = 15
     BROKER_EXCLUSIVE_CONFIG_DEFAULT = {'kombu_url': None,  # 如果这里也配置了kombu_url,则优先使用跟着你的kombu_url，否则使用funboost_config. KOMBU_URL
                                        'transport_options': {},  # transport_options是kombu的transport_options 。
                                        'prefetch_count': 500
                                        }
     # prefetch_count 是预获取消息数量
     ''' transport_options是kombu的transport_options 。 
        例如使用kombu使用redis作为中间件时候，可以设置 visibility_timeout 来决定消息取出多久没有ack，就自动重回队列。
```

## funboost/consumers/local_python_queue_consumer.py

```diff
@@ -1,22 +1,21 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:36
 import json
 from queue import Queue
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.publishers import local_python_queue_publisher
 
 
 class LocalPythonQueueConsumer(AbstractConsumer):
     """
     python 内置queue对象作为消息队列，这个要求发布和消费必须在同一python解释器内部运行，不支持分布式。
     """
-    BROKER_KIND = 3
 
     @property
     def local_python_queue(self) -> Queue:
         return local_python_queue_publisher.local_pyhton_queue_name__local_pyhton_queue_obj_map[self._queue_name]
 
     def _shedual_task(self):
         while True:
```

## funboost/consumers/mongomq_consumer.py

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:33
 import time
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.publishers.mongomq_publisher import MongoMixin, MongoMqPublisher
 
 
 class MongoMqConsumer(AbstractConsumer, MongoMixin):
     """
     Mongo queue包实现的基于mongo的消息队列，支持消费确认。
     """
-    BROKER_KIND = 5
+
 
     def _shedual_task(self):
         mp = MongoMqPublisher(self.queue_name)
         while True:
             job = mp.queue.next()
             if job is not None:
                 # self.logger.debug(f'从mongo的 [{self._queue_name}] 队列中 取出的消息是：   消息是：  {job.payload}  ')
```

## funboost/consumers/mqtt_consumer.py

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:32
 import json
 # import time
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost import funboost_config_deafult
 import paho.mqtt.client as mqtt
 
 
 class MqttConsumer(AbstractConsumer):
     """
     emq 作为中间件 实现的消费者 ，使用共享订阅。
     """
-    BROKER_KIND = 17
+
 
     # noinspection PyAttributeOutsideInit
     def custom_init(self):
         # fsdf 表示 funboost.相当于kafka的消费者组作用。
         # 这个是共享订阅，见  https://blog.csdn.net/emqx_broker/article/details/103027813
         self._topic_shared = f'$share/fsdf/{self._queue_name}'
```

## funboost/consumers/nameko_consumer.py

```diff
@@ -2,15 +2,15 @@
 # @Author  : ydf
 # @Time    : 2023/8/8 0008 13:32
 from multiprocessing import Process
 
 import threading
 
 import typing
-
+from funboost.constant import BrokerEnum
 from funboost.concurrent_pool.custom_evenlet_pool_executor import check_evenlet_monkey_patch
 
 from nameko.containers import ServiceContainer
 from nameko.rpc import rpc
 from nameko.runners import ServiceRunner
 
 from funboost.consumers.base_consumer import AbstractConsumer
@@ -19,15 +19,15 @@
 all_queue_name__nameko_service_cls_map = {}
 
 
 class NamekoConsumer(AbstractConsumer, ):
     """
     nameko作为中间件实现的。
     """
-    BROKER_KIND = 2
+
 
     def custom_init(self):
         try:
             check_evenlet_monkey_patch()
         except Exception as e:
             self.logger.critical('nameko 必须使用eventlet 并发，并且eventlet包打猴子补丁')
             raise e
@@ -49,22 +49,23 @@
     def _confirm_consume(self, kw):
         pass
 
     def _requeue(self, kw):
         pass
 
 
-def start_batch_nameko_service(boost_fun_list: typing.List):
+
+def batch_start_nameko_consumers(boost_fun_list: typing.List):
     runner = ServiceRunner(config=NAMEKO_CONFIG)
     for boost_fun in boost_fun_list:
         runner.add_service(all_queue_name__nameko_service_cls_map[boost_fun.queue_name])
     runner.start()
     runner.wait()
 
 
-def start_batch_nameko_service_in_new_thread(boost_fun_list: typing.List):
-    threading.Thread(target=start_batch_nameko_service, args=(boost_fun_list,)).start()
+def batch_start_nameko_service_in_new_thread(boost_fun_list: typing.List):
+    threading.Thread(target=batch_start_nameko_consumers, args=(boost_fun_list,)).start()
 
 
-def start_batch_nameko_service_in_new_process(boost_fun_list: typing.List, process_num=1):
+def batch_start_nameko_service_in_new_process(boost_fun_list: typing.List, process_num=1):
     for i in range(process_num):
-        Process(target=start_batch_nameko_service, args=(boost_fun_list,)).start()
+        Process(target=batch_start_nameko_consumers, args=(boost_fun_list,)).start()
```

## funboost/consumers/nats_consumer.py

```diff
@@ -1,18 +1,19 @@
 ﻿import json
 from pynats import NATSClient, NATSMessage  # noqa
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost import funboost_config_deafult
 
 
 class NatsConsumer(AbstractConsumer):
     """
     nats作为中间件实现的。
     """
-    BROKER_KIND = 24
+
 
     def _shedual_task(self):
         # print(88888888888888)
         nats_client = NATSClient(funboost_config_deafult.NATS_URL, socket_timeout=600, socket_keepalive=True)
         nats_client.connect()
 
         def callback(msg: NATSMessage):
```

## funboost/consumers/nsq_consumer.py

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:32
 import json
 from gnsq import Consumer, Message
-
+from funboost.constant import BrokerEnum
 from funboost import funboost_config_deafult
 from funboost.consumers.base_consumer import AbstractConsumer
 from nb_log import LogManager
 
 LogManager('gnsq').get_logger_and_add_handlers(20)
 
 
 class NsqConsumer(AbstractConsumer):
     """
     nsq作为中间件实现的。
     """
-    BROKER_KIND = 7
+
 
     def _shedual_task(self):
         consumer = Consumer(self._queue_name, 'frame_channel', funboost_config_deafult.NSQD_TCP_ADDRESSES,
                             max_in_flight=self._concurrent_num, heartbeat_interval=60, timeout=600, )  # heartbeat_interval 不能设置为600
 
         @consumer.on_message.connect
         def handler(consumerx: Consumer, message: Message):
```

## funboost/consumers/peewee_conusmer.py

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:33
 import json
-
+from funboost.constant import BrokerEnum
 from funboost import funboost_config_deafult
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.queues.peewee_queue import PeeweeQueue,TaskStatus
 
 
 class PeeweeConsumer(AbstractConsumer):
     """
     peewee实现的操作5种数据库模拟消息队列，支持消费确认。
     """
-    BROKER_KIND = 26
+
 
     def _shedual_task(self):
         self.queue = PeeweeQueue(self.queue_name)
         while True:
             task_dict = self.queue.get()
             # print(task_dict)
             # self.logger.debug(f'从数据库 {frame_config.SQLACHEMY_ENGINE_URL[:25]}。。 的 [{self._queue_name}] 队列中 取出的消息是：   消息是：  {sqla_task_dict}')
```

## funboost/consumers/persist_queue_consumer.py

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:35
 import json
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.publishers.persist_queue_publisher import PersistQueuePublisher
 
 
 class PersistQueueConsumer(AbstractConsumer):
     """
     persist queue包实现的本地持久化消息队列。
     """
-    BROKER_KIND = 6
+
 
     def _shedual_task(self):
         pub = PersistQueuePublisher(self.queue_name)
         while True:
             item = pub.queue.get()
             # self.logger.debug(f'从本地持久化sqlite的 [{self._queue_name}] 队列中 取出的消息是：   {item}  ')
             self._print_message_get_from_broker('本地持久化sqlite', item)
```

## funboost/consumers/pulsar_consumer.py

```diff
@@ -18,24 +18,24 @@
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:32
 import os
 
 import json
 from _pulsar import ConsumerType
 from pulsar.schema import schema
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost import funboost_config_deafult
 
 
 class PulsarConsumer(AbstractConsumer, ):
     """
     pulsar作为中间件实现的。
     """
-    BROKER_KIND = 20
+
     BROKER_EXCLUSIVE_CONFIG_DEFAULT = {'subscription_name': 'funboost_group',
                                        'replicate_subscription_state_enabled': True,
                                        'consumer_type': ConsumerType.Shared,
                                        }
 
     def custom_init(self):
         pass
```

## funboost/consumers/rabbitmq_amqpstorm_consumer.py

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:30
 import json
 import amqpstorm
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.publishers.rabbitmq_amqpstorm_publisher import RabbitmqPublisherUsingAmqpStorm
 
 
 class RabbitmqConsumerAmqpStorm(AbstractConsumer):
     """
     使用AmqpStorm实现的，多线程安全的，不用加锁。
     """
-    BROKER_KIND = 0
+
 
     def _shedual_task(self):
         # noinspection PyTypeChecker
         def callback(amqpstorm_message: amqpstorm.Message):
             body = amqpstorm_message.body
             # self.logger.debug(f'从rabbitmq的 [{self._queue_name}] 队列中 取出的消息是：  {body}')
             self._print_message_get_from_broker('rabbitmq', body)
```

## funboost/consumers/rabbitmq_pika_consumer.py

```diff
@@ -2,30 +2,30 @@
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:27
 import os
 import functools
 import json
 from threading import Lock
 from nb_log import LogManager, get_logger
-
+from funboost.constant import BrokerEnum
 from funboost.publishers.base_publisher import deco_mq_conn_error
 import pikav1.exceptions
 from pikav1.exceptions import AMQPError
 import pikav1
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost import funboost_config_deafult
 
 get_logger('pikav1', log_level_int=20)
 
 
 class RabbitmqConsumer(AbstractConsumer):
     """
     使用pika包实现的。
     """
-    BROKER_KIND = 4
+
 
     # noinspection PyAttributeOutsideInit
     def custom_init(self):
         self._lock_for_pika = Lock()
         self.logger.critical('pika 多线程中操作同一个 channel 有问题，如果使用 rabbitmq 建议设置中间件为 BrokerEnum.RABBITMQ_AMQPSTORM')
         os._exit(444) # noqa
```

## funboost/consumers/rabbitmq_pika_consumerv0.py

```diff
@@ -4,27 +4,27 @@
 import functools
 import json
 from threading import Lock
 
 from funboost.publishers.base_publisher import deco_mq_conn_error
 import pikav0.exceptions
 from pikav0.exceptions import AMQPError
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from nb_log import LogManager, get_logger
 from funboost.utils.rabbitmq_factory import RabbitMqFactory
 
 get_logger('pikav0', log_level_int=20)
 
 
 class RabbitmqConsumer(AbstractConsumer):
     """
     使用pika包实现的。
     """
-    BROKER_KIND = 0
+
 
     # noinspection PyAttributeOutsideInit
     def custom_init(self):
         self._lock_for_pika = Lock()
 
     def _shedual_task(self):
         # channel = RabbitMqFactory(is_use_rabbitpy=0).get_rabbit_cleint().creat_a_channel()
```

## funboost/consumers/rabbitmq_rabbitpy_consumer.py

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:31
 import json
 import rabbitpy
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.utils.rabbitmq_factory import RabbitMqFactory
 
 
 class RabbitmqConsumerRabbitpy(AbstractConsumer):
     """
     使用rabbitpy实现的
     """
-    BROKER_KIND = 1
+
 
     def _shedual_task(self):
         # noinspection PyTypeChecker
         channel = RabbitMqFactory(is_use_rabbitpy=1).get_rabbit_cleint().creat_a_channel()  # type:  rabbitpy.AMQP         #
         channel.queue_declare(queue=self._queue_name, durable=True)
         channel.basic_qos(prefetch_count=self._concurrent_num)
         for message in channel.basic_consume(self._queue_name, no_ack=False):
```

## funboost/consumers/redis_brpoplpush_consumer.py

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:32
 import json
 # import time
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.utils import RedisMixin, decorators
 
 
 class RedisBrpopLpushConsumer(AbstractConsumer, RedisMixin):
     """
     redis作为中间件实现的，使用redis brpoplpush 实现的，并且使用心跳来解决 关闭/掉线 重新分发问题。
 
     """
-    BROKER_KIND = 14
+
 
     def start_consuming_message(self):
         self._is_send_consumer_hearbeat_to_redis = True
         super().start_consuming_message()
         self.keep_circulating(60, block=False)(self._requeue_tasks_which_unconfirmed)()
 
     # noinspection DuplicatedCode
```

## funboost/consumers/redis_consumer.py

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:32
 import json
 # import time
 import time
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.utils import RedisMixin
 
 
 class RedisConsumer(AbstractConsumer, RedisMixin):
     """
     redis作为中间件实现的，使用redis list 结构实现的。
     这个如果消费脚本在运行时候随意反复重启或者非正常关闭或者消费宕机，会丢失大批任务。高可靠需要用rabbitmq或者redis_ack_able或者redis_stream的中间件方式。
 
     这个是复杂版，一次性拉取100个，简单版在 funboost/consumers/redis_consumer_simple.py
     """
-    BROKER_KIND = 2
+
     BROKER_EXCLUSIVE_CONFIG_DEFAULT = {'redis_bulk_push':0}   #redis_bulk_push 是否redis批量推送
 
     # noinspection DuplicatedCode
     def _shedual_task000(self):
         while True:
             result = self.redis_db_frame.blpop(self._queue_name, timeout=60)
             if result:
```

## funboost/consumers/redis_consumer_ack_able.py

```diff
@@ -5,26 +5,27 @@
 
 这个是加强版的可确认消费的redis消费实现，所以比redis_conusmer实现复杂很多。
 这个可以确保随意反复多次停止重启脚本，任务永不丢失
 """
 import json
 import time
 from deprecated.sphinx import deprecated
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.consumers.confirm_mixin import ConsumerConfirmMixinWithTheHelpOfRedis, ConsumerConfirmMixinWithTheHelpOfRedisByHearbeat
 
 
 @deprecated(version='1.0', reason="This class not used")
 class RedisConsumerAckAble000(ConsumerConfirmMixinWithTheHelpOfRedis, AbstractConsumer, ):
     """
     随意重启代码会极小概率丢失1个任务。
     redis作为中间件实现的。将取出来的消息同时放入一个set中，代表unack消费状态。以支持对机器和python进程的随意关闭和断电。
     和celery的配置  task_reject_on_worker_lost = True task_acks_late = True后，处理逻辑几乎不约而同相似。
     """
-    BROKER_KIND = 9
+
 
     def _shedual_task(self):
         while True:
             result = self.redis_db_frame.blpop(self._queue_name, timeout=60)
             # task_bytes = self.redis_db_frame.lpop(self._queue_name)
             if result:
                 task_str = result[1].decode()
@@ -53,15 +54,15 @@
    redis.call('rpush',KEYS[2],v)
     end
    return v'''
     # script_4 = r.register_script(lua_4)
     #
     # print(script_4(keys=["text_pipelien1","text_pipelien1b"]))
     """
-    BROKER_KIND = 9
+
 
     def _shedual_task(self):
         lua = '''
                      local v = redis.call("lpop", KEYS[1])
                      if v then
                      redis.call('zadd',KEYS[2],ARGV[1],v)
                       end
@@ -96,15 +97,15 @@
    redis.call('rpush',KEYS[2],v)
     end
    return v'''
     # script_4 = r.register_script(lua_4)
     #
     # print(script_4(keys=["text_pipelien1","text_pipelien1b"]))
     """
-    BROKER_KIND = 9
+
 
     def _shedual_task000(self):
         # 可以采用lua脚本，也可以采用redis的watch配合pipeline使用。比代码分两行pop和zadd比还能减少一次io交互，还能防止丢失小概率一个任务。
         lua = '''
                      local v = redis.call("lpop", KEYS[1])
                      if v then
                      redis.call('zadd',KEYS[2],ARGV[1],v)
```

## funboost/consumers/redis_consumer_simple.py

```diff
@@ -1,20 +1,21 @@
 ﻿# -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2023/8/8 0008 13:32
 import json
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.utils import RedisMixin
 
 
 class RedisConsumer(AbstractConsumer, RedisMixin):
     """
     redis作为中间件实现的。
     """
-    BROKER_KIND = 2
+
 
     def _shedual_task(self):
         while True:
             result = self.redis_db_frame.blpop(self._queue_name,timeout=60)
             if result:
                 self._print_message_get_from_broker('redis',result[1].decode())
                 task_dict = json.loads(result[1])
```

## funboost/consumers/redis_pubsub_consumer.py

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:32
 import json
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.utils import RedisMixin
 
 
 class RedisPbSubConsumer(AbstractConsumer, RedisMixin):
     """
     redis作为中间件实现的。
     """
-    BROKER_KIND = 27
+
 
     def _shedual_task0000(self):
         pub = self.redis_db_frame.pubsub()
         pub.subscribe(self.queue_name)
         for item in pub.listen():
             if item['type'] == 'message':
                 self._print_message_get_from_broker('reids', item['data'])
```

## funboost/consumers/redis_stream_consumer.py

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2021/4/3 0008 13:32
 import json
 import redis3
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.utils import RedisMixin, decorators
 
 
 class RedisStreamConsumer(AbstractConsumer, RedisMixin):
     """
     redis 的 stream 结构 作为中间件实现的。需要redis 5.0以上，redis stream结构 是redis的消息队列，概念类似kafka，功能远超 list结构。
     """
-    BROKER_KIND = 12
     GROUP = 'funboost_group'
 
     def start_consuming_message(self):
         redis_server_info_dict = self.redis_db_frame_version3.info()
         # print(redis_server_info_dict)
         if float(redis_server_info_dict['redis_version'][0]) < 5:
             raise EnvironmentError('必须是5.0版本以上redis服务端才能支持  stream 数据结构，'
```

## funboost/consumers/rocketmq_consumer.py

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/7/8 0008 13:27
 import json
 import time
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost import funboost_config_deafult
 from funboost.publishers.rocketmq_publisher import RocketmqPublisher
 
 
 class RocketmqConsumer(AbstractConsumer):
     """
     安装
     """
-    BROKER_KIND = 11
+
     GROUP_ID = 'g_funboost'
 
     def _shedual_task(self):
         try:
             from rocketmq.client import PushConsumer
         except BaseException as e:
             # print(traceback.format_exc())
```

## funboost/consumers/sqlachemy_consumer.py

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:33
 import json
-
+from funboost.constant import BrokerEnum
 from funboost import funboost_config_deafult
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost.queues import sqla_queue
 
 
 class SqlachemyConsumer(AbstractConsumer):
     """
     sqlachemy实现的操作5种数据库模拟消息队列，支持消费确认。
     """
-    BROKER_KIND = 10
+
 
     def _shedual_task(self):
         self.queue = sqla_queue.SqlaQueue(self._queue_name, funboost_config_deafult.SQLACHEMY_ENGINE_URL)
         while True:
             sqla_task_dict = self.queue.get()
             # self.logger.debug(f'从数据库 {frame_config.SQLACHEMY_ENGINE_URL[:25]}。。 的 [{self._queue_name}] 队列中 取出的消息是：   消息是：  {sqla_task_dict}')
             self._print_message_get_from_broker(f'从数据库 {funboost_config_deafult.SQLACHEMY_ENGINE_URL[:25]}', sqla_task_dict)
```

## funboost/consumers/tcp_consumer.py

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:32
 import json
 from threading import Thread
 import socket
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 
 
 class TCPConsumer(AbstractConsumer, ):
     """
     socket 实现消息队列，不支持持久化，但不需要安装软件。
     """
-    BROKER_KIND = 22
+
 
     BUFSIZE = 10240
 
     # noinspection PyAttributeOutsideInit
     def custom_init(self):
         ip__port_str = self.queue_name.split(':')
         ip_port = (ip__port_str[0], int(ip__port_str[1]))
```

## funboost/consumers/txt_file_consumer.py

```diff
@@ -1,24 +1,23 @@
 ﻿from pathlib import Path
 
 from nb_filelock import FileLock
 from persistqueue import Queue
 import json
 from persistqueue.serializers import json as json_serializer
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from funboost import funboost_config_deafult
 
 
 class TxtFileConsumer(AbstractConsumer, ):
     """
     txt文件作为消息队列
     这个不想做消费确认了,要消费确认请选 SQLITE_QUEUE 、PERSISTQUEUE中间件
     """
-    BROKER_KIND = 25
 
     def _shedual_task(self):
         file_queue_path = str((Path(funboost_config_deafult.TXT_FILE_PATH) / self.queue_name).absolute())
         file_lock = FileLock(Path(file_queue_path) / f'_funboost_txtfile_{self.queue_name}.lock')
         queue = Queue(str((Path(funboost_config_deafult.TXT_FILE_PATH) / self.queue_name).absolute()), autosave=True, serializer=json_serializer)
         while True:
             with file_lock:
```

## funboost/consumers/udp_consumer.py

```diff
@@ -1,21 +1,20 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:32
 import json
 import socket
-
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 
 
 class UDPConsumer(AbstractConsumer, ):
     """
     socket 实现消息队列，不支持持久化，但不需要安装软件。
     """
-    BROKER_KIND = 21
 
     BUFSIZE = 10240
 
     # noinspection PyAttributeOutsideInit
     def custom_init(self):
         """ udp为消息队列中间件 时候 queue_name 要设置为例如  127.0.0.1:5689"""
         self.__udp_client = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
```

## funboost/consumers/zeromq_consumer.py

```diff
@@ -2,14 +2,15 @@
 # @Author  : ydf
 import os
 import socket
 import json
 # import time
 import zmq
 import multiprocessing
+from funboost.constant import BrokerEnum
 from funboost.consumers.base_consumer import AbstractConsumer
 from nb_log import get_logger
 
 
 # noinspection PyPep8
 def check_port_is_used(ip, port):
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
@@ -59,15 +60,14 @@
         logger_zeromq_broker.warning(e)
 
 
 class ZeroMqConsumer(AbstractConsumer):
     """
     zeromq 中间件的消费者，zeromq基于socket代码，不会持久化，且不需要安装软件。
     """
-    BROKER_KIND = 13
 
     def start_broker_queue_name_as_port(self):
         # threading.Thread(target=self._start_broker).start()
         # noinspection PyBroadException
         try:
             if not (10000 < int(self._queue_name) < 65535):
                 raise ValueError("，请设置queue的名字是一个 10000到65535的之间的一个端口数字")
```

## funboost/factories/consumer_factory.py

```diff
@@ -1,77 +1,23 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:19
-import copy
-# from collections import Callable
-from typing import Callable
 
-# from funboost.consumers.pulsar_consumer import PulsarConsumer
-from funboost.consumers.redis_pubsub_consumer import RedisPbSubConsumer
-from funboost.consumers.http_consumer import HTTPConsumer
-from funboost.consumers.kafka_consumer import KafkaConsumer
-from funboost.consumers.kafka_consumer_manually_commit import KafkaConsumerManuallyCommit
-from funboost.consumers.kombu_consumer import KombuConsumer
-from funboost.consumers.local_python_queue_consumer import LocalPythonQueueConsumer
-from funboost.consumers.mongomq_consumer import MongoMqConsumer
-from funboost.consumers.nats_consumer import NatsConsumer
-from funboost.consumers.nsq_consumer import NsqConsumer
-from funboost.consumers.peewee_conusmer import PeeweeConsumer
-from funboost.consumers.persist_queue_consumer import PersistQueueConsumer
-from funboost.consumers.rabbitmq_amqpstorm_consumer import RabbitmqConsumerAmqpStorm
-from funboost.consumers.rabbitmq_pika_consumer import RabbitmqConsumer
-from funboost.consumers.rabbitmq_rabbitpy_consumer import RabbitmqConsumerRabbitpy
-from funboost.consumers.redis_brpoplpush_consumer import RedisBrpopLpushConsumer
-from funboost.consumers.redis_consumer import RedisConsumer
-from funboost.consumers.redis_consumer_ack_able import RedisConsumerAckAble
-from funboost.consumers.rocketmq_consumer import RocketmqConsumer
-from funboost.consumers.sqlachemy_consumer import SqlachemyConsumer
-from funboost.consumers.redis_stream_consumer import RedisStreamConsumer
-from funboost.consumers.tcp_consumer import TCPConsumer
-from funboost.consumers.txt_file_consumer import TxtFileConsumer
-from funboost.consumers.udp_consumer import UDPConsumer
-from funboost.consumers.zeromq_consumer import ZeroMqConsumer
-from funboost.consumers.mqtt_consumer import MqttConsumer
-from funboost.consumers.httpsqs_consumer import HttpsqsConsumer
 
-broker_kind__consumer_type_map = {
-    0: RabbitmqConsumerAmqpStorm,
-    1: RabbitmqConsumerRabbitpy,
-    2: RedisConsumer,
-    3: LocalPythonQueueConsumer,
-    4: RabbitmqConsumer,
-    5: MongoMqConsumer,
-    6: PersistQueueConsumer,
-    7: NsqConsumer,
-    8: KafkaConsumer,
-    9: RedisConsumerAckAble,
-    10: SqlachemyConsumer,
-    11: RocketmqConsumer,
-    12: RedisStreamConsumer,
-    13: ZeroMqConsumer,
-    14: RedisBrpopLpushConsumer,
-    15: KombuConsumer,
-    16: KafkaConsumerManuallyCommit,
-    17: MqttConsumer,
-    18: HttpsqsConsumer,
-    # 20: PulsarConsumer,  # 用户如果想用pulsar，先pip 安装pulsar-client ,然后代码调用 register_pulsar_broker() 会自动添加到这个字典里面
-    21: UDPConsumer,
-    22: TCPConsumer,
-    23: HTTPConsumer,
-    24: NatsConsumer,
-    25: TxtFileConsumer,
-    26: PeeweeConsumer,
-    27: RedisPbSubConsumer,
-}
+from funboost.constant import BrokerEnum
+from funboost.consumers.base_consumer import AbstractConsumer
 
 
-def get_consumer(*args, broker_kind: int = None, **kwargs):
+def get_consumer(*args, broker_kind: int = None, **kwargs) -> AbstractConsumer:
     """
     :param args: 入参是AbstractConsumer的入参
     :param broker_kind:
     :param kwargs:
     :return:
     """
+    from funboost.factories.broker_kind__publsiher_consumer_type_map import broker_kind__publsiher_consumer_type_map, BrokerRegister
+    if broker_kind in BrokerRegister().broker_kind__regist_fun_map:
+        BrokerRegister().regist_to_funboost(broker_kind)  # 动态注册中间件到框架是为了延迟导入，用户没安装不需要的第三方包不报错。
 
-    if broker_kind not in broker_kind__consumer_type_map:
+    if broker_kind not in broker_kind__publsiher_consumer_type_map:
         raise ValueError(f'设置的中间件种类数字不正确,你设置的值是 {broker_kind} ')
-    return broker_kind__consumer_type_map[broker_kind](*args, **kwargs)
+    return broker_kind__publsiher_consumer_type_map[broker_kind][1](*args, **kwargs)
```

## funboost/factories/publisher_factotry.py

```diff
@@ -1,69 +1,17 @@
 # -*- coding: utf-8 -*-
 # @Author  : ydf
 # @Time    : 2022/8/8 0008 13:16
 import copy
+
 from typing import Callable
 from funboost.publishers.base_publisher import AbstractPublisher
-from funboost.publishers.confluent_kafka_publisher import ConfluentKafkaPublisher
-from funboost.publishers.http_publisher import HTTPPublisher
-from funboost.publishers.kombu_publisher import KombuPublisher
-from funboost.publishers.nats_publisher import NatsPublisher
-from funboost.publishers.peewee_publisher import PeeweePublisher
-# from funboost.publishers.pulsar_publisher import PulsarPublisher
-from funboost.publishers.redis_publisher_lpush import RedisPublisherLpush
-from funboost.publishers.redis_pubsub_publisher import RedisPubSubPublisher
-from funboost.publishers.tcp_publisher import TCPPublisher
-from funboost.publishers.txt_file_publisher import TxtFilePublisher
-from funboost.publishers.udp_publisher import UDPPublisher
-from funboost.publishers.zeromq_publisher import ZeroMqPublisher
-from funboost.publishers.kafka_publisher import KafkaPublisher
-from funboost.publishers.local_python_queue_publisher import LocalPythonQueuePublisher
-from funboost.publishers.mongomq_publisher import MongoMqPublisher
-from funboost.publishers.nsq_publisher import NsqPublisher
-from funboost.publishers.persist_queue_publisher import PersistQueuePublisher
-from funboost.publishers.rabbitmq_amqpstorm_publisher import RabbitmqPublisherUsingAmqpStorm
-from funboost.publishers.rabbitmq_pika_publisher import RabbitmqPublisher
-from funboost.publishers.rabbitmq_rabbitpy_publisher import RabbitmqPublisherUsingRabbitpy
-from funboost.publishers.redis_publisher import RedisPublisher
-from funboost.publishers.rocketmq_publisher import RocketmqPublisher
-from funboost.publishers.sqla_queue_publisher import SqlachemyQueuePublisher
-from funboost.publishers.redis_stream_publisher import RedisStreamPublisher
-from funboost.publishers.mqtt_publisher import MqttPublisher
-from funboost.publishers.httpsqs_publisher import HttpsqsPublisher
-
-broker_kind__publisher_type_map = {
-    0: RabbitmqPublisherUsingAmqpStorm,
-    1: RabbitmqPublisherUsingRabbitpy,
-    2: RedisPublisher,
-    3: LocalPythonQueuePublisher,
-    4: RabbitmqPublisher,
-    5: MongoMqPublisher,
-    6: PersistQueuePublisher,
-    7: NsqPublisher,
-    8: KafkaPublisher,
-    9: RedisPublisher,
-    10: SqlachemyQueuePublisher,
-    11: RocketmqPublisher,
-    12: RedisStreamPublisher,
-    13: ZeroMqPublisher,
-    14: RedisPublisherLpush,
-    15: KombuPublisher,
-    16: ConfluentKafkaPublisher,
-    17: MqttPublisher,
-    18: HttpsqsPublisher,
-    # 20: PulsarPublisher,
-    21: UDPPublisher,
-    22: TCPPublisher,
-    23: HTTPPublisher,
-    24: NatsPublisher,
-    25: TxtFilePublisher,
-    26: PeeweePublisher,
-    27: RedisPubSubPublisher,
-}
+
+
+# broker_kind__publisher_type_map
 
 def get_publisher(queue_name, *, log_level_int=10, logger_prefix='', is_add_file_handler=True,
                   clear_queue_within_init=False, is_add_publish_time=True, consuming_function: Callable = None,
                   broker_kind: int = None,
                   broker_exclusive_config: dict = None,
                   ) -> AbstractPublisher:
     """
@@ -80,10 +28,11 @@
            例如kafka支持消费者组，rabbitmq也支持各种独特概念例如各种ack机制 复杂路由机制，每一种消息队列都有独特的配置参数意义，可以通过这里传递。
 
     :return:
     """
 
     all_kwargs = copy.deepcopy(locals())
     all_kwargs.pop('broker_kind')
-    if broker_kind not in broker_kind__publisher_type_map:
+    from funboost.factories.broker_kind__publsiher_consumer_type_map import broker_kind__publsiher_consumer_type_map
+    if broker_kind not in broker_kind__publsiher_consumer_type_map:
         raise ValueError(f'设置的中间件种类数字不正确,你设置的值是 {broker_kind} ')
-    return broker_kind__publisher_type_map[broker_kind](**all_kwargs)
+    return broker_kind__publsiher_consumer_type_map[broker_kind][0](**all_kwargs)
```

## funboost/publishers/celery_publisher.py

```diff
@@ -9,16 +9,24 @@
 import celery
 import celery.result
 import typing
 
 from funboost.publishers.base_publisher import AbstractPublisher, PriorityConsumingControlConfig
 from funboost import funboost_config_deafult
 
+celery_app = celery.Celery(broker=funboost_config_deafult.CELERY_BROKER_URL,
+                           backend=funboost_config_deafult.CELERY_RESULT_BACKEND,
+                           task_routes={}, timezone=funboost_config_deafult.TIMEZONE, enable_utc=False)
 
-# celery_app = celery.Celery(broker='redis://192.168.64.151:6378/11',task_routes={})
+celery_app.conf.task_acks_late = True
+
+# celery_app.conf.worker_task_log_format = '%(asctime)s - %(name)s - "%(pathname)s:%(lineno)d" - %(funcName)s - %(levelname)s - %(message)s'
+# celery_app.conf.worker_log_format = '%(asctime)s - %(name)s - "%(pathname)s:%(lineno)d" - %(funcName)s - %(levelname)s - %(message)s'
+
+celery_app.conf.worker_redirect_stdouts = False
 
 
 class CeleryPublisher(AbstractPublisher, ):
     """
     使用celery作为中间件
     """
     celery_conf_lock = threading.Lock()
@@ -34,49 +42,31 @@
         # @celery_app.task(name=self.queue_name)
         # def f(*args, **kwargs):
         #     pass
         #
         # self._celery_app = celery_app
         # self._celery_fun = f
 
-        self._has_build_celery_app = False
-
-    def _build_celery_app(self):
-        celery_app = celery.Celery(broker=funboost_config_deafult.CELERY_BROKER_URL,
-                                   backend=funboost_config_deafult.CELERY_RESULT_BACKEND,
-                                   task_routes={}, timezone=funboost_config_deafult.TIMEZONE, enable_utc=False)
-        celery_app.config_from_object(self.broker_exclusive_config['celery_app_config'])
         celery_app.conf.task_routes.update({self.queue_name: {"queue": self.queue_name}})
 
-        @celery_app.task(name=self.queue_name)
-        def f(*args, **kwargs):
-            pass
-
-        self._celery_app = celery_app
-        self._celery_fun = f
-
-        self._has_build_celery_app = True
-
     def publish(self, msg: typing.Union[str, dict], task_id=None,
                 priority_control_config: PriorityConsumingControlConfig = None) -> celery.result.AsyncResult:
         if isinstance(msg, str):
             msg = json.loads(msg)
         msg_function_kw = copy.copy(msg)
         if self.publish_params_checker:
             self.publish_params_checker.check_params(msg)
         task_id = task_id or f'{self._queue_name}_result:{uuid.uuid4()}'
         msg['extra'] = extra_params = {'task_id': task_id, 'publish_time': round(time.time(), 4),
                                        'publish_time_format': time.strftime('%Y-%m-%d %H:%M:%S')}
         if priority_control_config:
             extra_params.update(priority_control_config.to_dict())
-        with self.celery_conf_lock:
-            if not self._has_build_celery_app:
-                self._build_celery_app()
+
         t_start = time.time()
-        celery_result = self._celery_fun.apply_async(kwargs=msg_function_kw, task_id=extra_params['task_id'])  # type: celery.result.AsyncResult
+        celery_result = celery_app.send_task(name=self.queue_name, kwargs=msg_function_kw, task_id=extra_params['task_id'])  # type: celery.result.AsyncResult
         self.logger.debug(f'向{self._queue_name} 队列，推送消息 耗时{round(time.time() - t_start, 4)}秒  {msg_function_kw}')  # 显示msg太长了。
         with self._lock_for_count:
             self.count_per_minute += 1
             self.publish_msg_num_total += 1
             if time.time() - self._current_time > 10:
                 self.logger.info(
                     f'10秒内推送了 {self.count_per_minute} 条消息,累计推送了 {self.publish_msg_num_total} 条消息到 {self._queue_name} 队列中')
```

## funboost/publishers/http_publisher.py

```diff
@@ -7,16 +7,14 @@
 
 
 class HTTPPublisher(AbstractPublisher, ):
     """
     http实现的，不支持持久化。
     """
 
-    BROKER_KIND = 23
-
     # noinspection PyAttributeOutsideInit
     def custom_init(self):
         self._http = PoolManager(10)
 
     def concrete_realization_of_publish(self, msg):
         url = self.queue_name + '/queue'
         self._http.request('post', url, fields={'msg': msg})
```

## funboost/publishers/tcp_publisher.py

```diff
@@ -6,16 +6,14 @@
 
 
 class TCPPublisher(AbstractPublisher, ):
     """
     使用tco作为中间件,不支持持久化，支持分布式
     """
 
-    BROKER_KIND = 21
-
     BUFSIZE = 10240
 
     # noinspection PyAttributeOutsideInit
     def custom_init(self):
         """ tcp为消息队列中间件 时候 queue_name 要设置为例如  127.0.0.1:5689"""
         pass
```

## funboost/publishers/udp_publisher.py

```diff
@@ -6,16 +6,14 @@
 
 
 class UDPPublisher(AbstractPublisher, ):
     """
     使用udp作为中间件,不支持持久化，支持分布式
     """
 
-    BROKER_KIND = 22
-
     BUFSIZE = 10240
 
     # noinspection PyAttributeOutsideInit
     def custom_init(self):
         """ udp为消息队列中间件 时候 queue_name 要设置为例如  127.0.0.1:5689"""
         self.__udp_client = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         ip__port_str = self.queue_name.split(':')
```

## funboost/queues/sqla_queue.py

```diff
@@ -5,27 +5,26 @@
 使用sqlachemy来使5种关系型数据库模拟消息队列。
 """
 import datetime
 import json
 import time
 from pathlib import Path
 
-try:
-    import sqlalchemy
-    from sqlalchemy import Column, func, or_, and_, Table, MetaData
-    from sqlalchemy import Integer
-    from sqlalchemy import String, DateTime
-    from sqlalchemy import create_engine
-    from sqlalchemy.ext.automap import automap_base
-    from sqlalchemy.ext.declarative import declarative_base
-    from sqlalchemy.orm import sessionmaker, scoped_session
-    from sqlalchemy.pool import StaticPool
-    from sqlalchemy_utils import database_exists, create_database
-except ImportError as e:
-    print(f'{e}  不使用sqlalchemy操作数据库模拟消息队列，就可以无视这')
+
+import sqlalchemy
+from sqlalchemy import Column, func, or_, and_, Table, MetaData
+from sqlalchemy import Integer
+from sqlalchemy import String, DateTime
+from sqlalchemy import create_engine
+from sqlalchemy.ext.automap import automap_base
+from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import sessionmaker, scoped_session
+from sqlalchemy.pool import StaticPool
+from sqlalchemy_utils import database_exists, create_database
+
 from funboost.utils import LoggerMixin, decorators, LoggerLevelSetterMixin
 
 
 class TaskStatus:
     TO_BE_CONSUMED = 'to_be_consumed'
     PENGDING = 'pengding'
     FAILED = 'failed'
```

## Comparing `funboost-20.4.dist-info/LICENSE` & `funboost-20.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `funboost-20.4.dist-info/METADATA` & `funboost-20.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funboost
-Version: 20.4
+Version: 20.5
 Summary: pip install funboost，python全功能分布式函数调度框架,。支持python所有类型的并发模式和一切知名消息队列中间件，python函数加速器，框架包罗万象，一统编程思维，兼容50% python业务场景，适用范围广。只需要一行代码即可分布式执行python一切函数，99%用过funboost的pythoner 感受是 方便 快速 强大，相见恨晚 
 Home-page: https://github.com/ydf0509/funboost
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -46,15 +46,15 @@
 Requires-Dist: peewee (==3.15.1)
 Requires-Dist: apscheduler (==3.7.0)
 Requires-Dist: pikav0
 Requires-Dist: pikav1
 Requires-Dist: redis2
 Requires-Dist: redis3
 Requires-Dist: redis
-Requires-Dist: nb-log (>=8.2)
+Requires-Dist: nb-log (>=8.5)
 Requires-Dist: rocketmq
 Requires-Dist: zmq
 Requires-Dist: pyzmq
 Requires-Dist: kombu
 Requires-Dist: paho-mqtt
 Requires-Dist: setuptools-rust
 Requires-Dist: fabric2 (==2.6.0)
@@ -68,14 +68,15 @@
 Requires-Dist: frozenlist
 
 
 # 1.分布式函数调度框架简介
 
 <pre style="color: greenyellow;background-color: #0c1119; font-size: medium;">
 pip install funboost ,python全功能分布式函数调度框架,。 支持python所有类型的并发模式和全球一切知名消息队列中间件，
+同时funboost支持celery整个框架作为核心来发布和消费消息，使用funboost的极简api方式来自动化配置和操作celery,
 python函数加速器，框架包罗万象，一统编程思维，兼容50% python编程业务场景，适用范围广。
 只需要一行代码即可分布式执行python一切函数，99%用过funboost的pythoner 感受是 方便 快速 强大。
 python万能分布式函数调度框架，支持5种并发模式，30种消息中间件，20种任务控制功能。给任意python函数赋能。
 用途概念就是常规经典的 生产者 + 消息队列中间件 + 消费者 编程思想。
 框架只需要学习@boost这一个装饰器的入参就可以，所有用法几乎和1.3例子一摸一样，非常简化简单。
 </pre>
 
@@ -153,15 +154,15 @@
 ## 1.2 框架功能介绍
 
 分布式函数调度框架，支持5种并发模式，20+种消息中间件，20种任务控制功能。<br>
 用途概念就是常规经典的 生产者 + 消息队列中间件 + 消费者 编程思想。
 
 有了这个框架，用户再也无需亲自手写操作进程、线程、协程的并发的代码了。
 
-有了这个框架，用户再也无需亲自手写操作redis rabbitmq socket kafka 了。
+有了这个框架，用户再也无需亲自手写操作redis rabbitmq socket kafka celery nameko了。
 
 [![sgV2xP.png](https://z3.ax1x.com/2021/01/19/sgV2xP.png)](https://imgtu.com/i/sgV2xP)
 
 ### 1.2.1 框架支持5种并发模式
 
 <div   style=" font-size: xx-large; font-family: 黑体,serif; "> threading  <span style="font-size: medium">(使用的是可变线程池，可以智能自动缩小和扩大线程数量) </span> </div> 
 
@@ -190,15 +191,15 @@
 以下两种方式，都是10线程加python内存queue方式运行f函数，有了此框架，用户无需代码手写手动操作线程 协程 进程并发。
 [![T69zJP.png](https://s4.ax1x.com/2021/12/28/T69zJP.png)](https://imgtu.com/i/T69zJP)
 <br>
 [![T6CPsg.md.png](https://s4.ax1x.com/2021/12/28/T6CPsg.md.png)](https://imgtu.com/i/T6CPsg)
 
 ### 1.2.2 框架支持20种中间件
 
-框架支持 rabbitmq redis python自带的queue.Queue  sqlite sqlachemy kafka pulsar mongodb 直接socket 等作为消息中间件。
+框架支持 rabbitmq redis python自带的queue.Queue  sqlite sqlachemy kafka pulsar mongodb 直接socket celery  nameko 等作为消息中间件。
 
 同时此框架也支持操作 kombu 库作为中间件,所以此框架能够支持的中间件类型只会比celery更多。
 
 框架支持的中间件种类大全和选型见文档3.1章节的介绍:   
 
 [3.1 各种中间件选择的场景和优势](https://funboost.readthedocs.io/zh/latest/articles/c3.html#id2) 
 
@@ -404,13 +405,29 @@
 从而体会框架的分布式 并发 控频。
 
 这是最简单的框架，只有@boost 1行代码需要学习。说的是这是最简单框架，这不是最简单的python包。
 如果连只有一个重要函数的框架都学不会，那就学不会学习得了更复杂的其他框架了，大部分框架都很复杂比学习一个包难很多。
 大部分框架，都要深入使用里面的很多个类，还需要继承组合一顿。
 ```
 
+## 1.6 funboost支持支持celery框架整体作为funboost的broker (2023.4新增)
+```
+见11.1章节代码例子，celery框架整体作为funboost的broker，funboost的发布和消费将只作为极简api，核心的消费调度和发布和定时功能，都是由celery框架来完成，funboost框架的发布和调度代码不实际起作用。
+用户操作funboost的api，语法和使用其他消息队列中间件类型一样，funboost自动化操作celery。
+
+用户无需操作celery本身，无需敲击celery难记的命令行启动消费、定时、flower;
+用户无需小心翼翼纠结亲自使用celery时候怎么规划目录结构 文件夹命名 需要怎么在配置写include 写task_routes，
+完全不存在需要固定的celery目录结构，不需要手动配置懵逼的任务路由，不需要配置每个函数怎么使用不同的队列名字，funboost自动搞定这些。
+
+用户只需要使用简单的funboost语法就能操控celery框架了。funboost使用celery作为broker_kind,远远的暴击亲自使用无法ide下代码补全的celery框架的语法。
+```
+
+```
+funboost通过支持celery作为broker_kind,使celer框架变成了funboost的一个子集
+```
+
 [查看分布式函数调度框架完整文档](https://funboost.readthedocs.io/zh/latest/index.html)
 
 ![](https://visitor-badge.glitch.me/badge?page_id=distributed_framework)
 
 <div> </div>
```

## Comparing `funboost-20.4.dist-info/RECORD` & `funboost-20.5.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-funboost/__init__.py,sha256=bA6IaAysO2we8gqOy3JDVrM__-3Px7VQTLYORx5dQQY,21053
+funboost/__init__.py,sha256=8jWW7T0V1u2AVkwpocR4eVxWhjQO5cmpl31y50S7S2Y,21081
 funboost/constant.py,sha256=1PtxXLXFg7LsHMePU2iZeL2XOF4JUXnanI6kDFeh-JU,5910
 funboost/funboost_config_deafult.py,sha256=hQD7MZtJFQykqqJIULmqNJBwHSBEXGcCs_2LX2oDTdc,7100
 funboost/helpers.py,sha256=KApnbT-OXtgKKlY-MGjTnsP7YxBtDn3k3LL_XOn4TGU,14104
 funboost/set_frame_config.py,sha256=hz_38C-IXEulYpHQdr1fhsMcdEDCHIsF2la8MkHiIjA,9149
-funboost/assist/user_custom_broker_register.py,sha256=kgtwpaazLOTugsyrx_Q114FW1y_hdQpuHY1QYVJ4bV0,4734
 funboost/beggar_version_implementation/beggar_redis_consumer.py,sha256=aiucCkj7-GWbLMIWHhevdQrAsxzyc55AL69fue8esYs,3930
 funboost/concurrent_pool/__init__.py,sha256=dGgxgzMSwcXWMexwAnojsML7EMjHAAsmAofNgrxtl2w,759
 funboost/concurrent_pool/async_helper.py,sha256=iyb0Jcjyx-vkUGC_saSUWqN657kcR5K7B-L_SB6cDCE,3256
 funboost/concurrent_pool/async_pool_executor.py,sha256=zCymNAFuPrV5CuW9hXCyzQ8nLCY73ixvvDsWFPNvt90,7227
 funboost/concurrent_pool/bounded_processpoolexcutor_gt_py37.py,sha256=y6tL41X4sC_d5E2k2sNz0JZUJU2hyJDyMcOi2RzkI_w,4723
 funboost/concurrent_pool/bounded_processpoolexcutor_py36.py,sha256=fwhCvXCRILshQbGVv5Y9kFqCZsX0VMKTUdLhI9dLDbg,3011
 funboost/concurrent_pool/bounded_threadpoolexcutor.py,sha256=T1mJA1yxUYAkoDjrJMxCPPxSF3bUH4_5AFpYx3PWjfQ,1571
@@ -19,54 +18,56 @@
 funboost/concurrent_pool/single_thread_executor.py,sha256=NDWOegh8Nxpb-Bp-lUlj-DONWvepSmA9qepL1yNgdQI,373
 funboost/concurrent_pool/backup/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/concurrent_pool/backup/async_pool_executor0223.py,sha256=iTxxJFk2lu1P9ZAIkBip3euq3oEQ4_qTODy3xUaOecY,9548
 funboost/concurrent_pool/backup/async_pool_executor_back.py,sha256=vIgUUyF4Zb0jIRPWgNPqyO09YEkQP32kkpGBldqm4qA,9568
 funboost/concurrent_pool/backup/async_pool_executor_janus.py,sha256=OHMWJ9l3EYTpPpcrPrGGKd4K0tmQ2PN8HiX0Dta0EOo,5728
 funboost/consumers/__init__.py,sha256=ZXY_6Kut1VYNQiF5aWEgIWobsW1ht9YUP0TdRZRWFqI,126
 funboost/consumers/base_consumer.py,sha256=QBm7yYPmKlcSra-HHo3oBUjJvwv35eFhB3vchP6SCTc,94018
-funboost/consumers/celery_consumer.py,sha256=8SF8ppHIMH-BIAHO0NyJYnSQxe_PcT6hv05e7DySG54,4574
+funboost/consumers/celery_consumer.py,sha256=bO5oVYDzo9DubjSa0tEsVMcKviOwF89KncMM2Mg6KCI,11274
+funboost/consumers/celery_consumer000.py,sha256=8SF8ppHIMH-BIAHO0NyJYnSQxe_PcT6hv05e7DySG54,4574
 funboost/consumers/confirm_mixin.py,sha256=H0w07PceU2gGf6X1EXvAB5oD7IavzGv96bQTxm-58sE,5877
-funboost/consumers/http_consumer.py,sha256=n45vdw3u7ta6f-AxSQKJfoMoSu4eV5C0NUOQaDAafQ8,2045
+funboost/consumers/http_consumer.py,sha256=zkEdYTz4xnRhLJq4JftCTehAb5oTjvnVaMjBNEP7Sfk,2067
 funboost/consumers/http_consumer000.py,sha256=NXOSiN1qpLAJfJkuF6SjFpWQ28YxMDULzWCBTNMwYe8,4463
-funboost/consumers/httpsqs_consumer.py,sha256=wfK_7QLxLDnBw3HE8KChPiwR6bzogIHyTQkiRLJYuJQ,1058
-funboost/consumers/kafka_consumer.py,sha256=5dcnWrJH3fpWSeUB54Um_xspNUw7ytrVbW8Bf34rSPs,4196
-funboost/consumers/kafka_consumer_manually_commit.py,sha256=Glox-UMWqPoJGtT-J_fOpv1yPbEAH7_BV9CKQFwAfbE,6536
-funboost/consumers/kombu_consumer.py,sha256=VYxmaQ54q3FVBD3uZ1JGQUOEDQ1YGE-Sbx2o_5JD8Yo,10168
-funboost/consumers/local_python_queue_consumer.py,sha256=bTekCaBY8B65WH-nV-3NJDcRxLSJkQafatErj7-MUVo,1272
-funboost/consumers/mongomq_consumer.py,sha256=J7Z4UX7peztVeyM33Pi0BnDtxmBB-u-HDo-obd7vTuc,1069
-funboost/consumers/mqtt_consumer.py,sha256=8GSlCAQIlByfelK6BHnIzFsXb50sgIwCiAbHbGl324c,2208
-funboost/consumers/nameko_consumer.py,sha256=LLixKkfNKUFLRE511JrxVNwbQgzBYn7va1llnNIkugg,2154
-funboost/consumers/nats_consumer.py,sha256=yv0XJWE1q296UwpwFaXK66dpRHzqbziha1_ophs0Rvc,1054
-funboost/consumers/nsq_consumer.py,sha256=fErxzlM1X-X4crkddkm98UssY9eop8O61-y-4Z8DYmA,1440
-funboost/consumers/peewee_conusmer.py,sha256=6eHZ0mttcVoyRWODD-l8nfgMF5E5KAMTxKrStknGTWY,1218
-funboost/consumers/persist_queue_consumer.py,sha256=J4OThFO2yvNMh3bFxkE1Ff7OFo-PaHbjLfoSi239a84,982
-funboost/consumers/pulsar_consumer.py,sha256=vKhUhiGO3YODuti6bspeDR52R6vy1YyV4asStT3fE78,2394
-funboost/consumers/rabbitmq_amqpstorm_consumer.py,sha256=dw2bv7HloJ2ABWV6-HQxUSbrFkJfaxdeRVXT2l5yad4,1700
-funboost/consumers/rabbitmq_pika_consumer.py,sha256=yYb9QuZeR4RBYhvQcO8sp3D1Gdc8VBHw0wJhA70XHhk,5412
-funboost/consumers/rabbitmq_pika_consumerv0.py,sha256=i9BcTqyapMlQypWjvwb8D4m6hZXFzpbAGLVPDWvXd7s,4653
-funboost/consumers/rabbitmq_rabbitpy_consumer.py,sha256=I0GK7ur2qwJbWajdTfqo67WkLfgR0C72OxwNPjiinhs,1239
-funboost/consumers/redis_brpoplpush_consumer.py,sha256=VDKTVFhOGtqb7RJuW-5m_Aany__T7W0O0JaIUHfvmAc,3011
-funboost/consumers/redis_consumer.py,sha256=kz1rQt5yMHWcq3VMxpPL-bRRnOYjOgUFODvb8FNG86Y,2808
-funboost/consumers/redis_consumer_ack_able.py,sha256=DBKh2Ejp1mY19GdmSvtpJ4lEhRPFv2bUl5hXfGj5vbM,7560
-funboost/consumers/redis_consumer_simple.py,sha256=VheSdKUdsBfs5wMu89nTGrMzK2c29koFDvjQhm8TS_M,899
+funboost/consumers/httpsqs_consumer.py,sha256=LICZzovaMVrZsJY4GgLrk3EaHz8f9ZZBLKZtWl3frMc,1080
+funboost/consumers/kafka_consumer.py,sha256=2BZT5UQIGqjS1emsX--V1J8gWFOhMjCMMiSnWy_Hto0,4217
+funboost/consumers/kafka_consumer_manually_commit.py,sha256=OJvua_kEZ8_MRuRxW9Jz5aiebM1tYSdjzQfVXd0sBd0,6556
+funboost/consumers/kombu_consumer.py,sha256=VlU5LR69G0we6K5UCzWOiz-Ul_LJArWznMvTUCBwyR8,10186
+funboost/consumers/local_python_queue_consumer.py,sha256=29r44zUZPBIREvsHOfw59kRvwvfVBE2AJ8wWmXDh_3Y,1291
+funboost/consumers/mongomq_consumer.py,sha256=W5d4QnYun1OnnCn8K41ZmXuGdpAXmnzAa4EI7H7KQO4,1090
+funboost/consumers/mqtt_consumer.py,sha256=StlfPUeQ6o0HiZBpt7TlC_r2DjzPHBZBF2xLSxQW13A,2228
+funboost/consumers/nameko_consumer.py,sha256=IVwUxBixUx2m3F_q8Xn-UsnJWXayMpnOIZjICCd6mcU,2183
+funboost/consumers/nats_consumer.py,sha256=lIYLKvMHNReHnNqGtBA4wot4Ncaobtk60zVHFgm-9Zc,1076
+funboost/consumers/nsq_consumer.py,sha256=PaMRsP8oeRg0H_tq4FL7YhNUdOWAqJkjrwZWoYPNkqU,1461
+funboost/consumers/peewee_conusmer.py,sha256=fbspeWbv6F3EsIIBAjkM_FNh2vMyrDsydju23WAVHvE,1238
+funboost/consumers/persist_queue_consumer.py,sha256=8HzRcMFE6OKiF_CL3atC42Ien_yf5daG3LU38YBKWi0,1005
+funboost/consumers/pulsar_consumer.py,sha256=2DuklBV5dSY-_gW2EpRWz8QSy-VjZclj0gJUvLTyJHA,2414
+funboost/consumers/rabbitmq_amqpstorm_consumer.py,sha256=1YtnhlpVK1Nk4FnfFZOog1P9FU916TLnWJuezUGkED8,1721
+funboost/consumers/rabbitmq_pika_consumer.py,sha256=9L7CA2wYT-RNpaVfLKrFk6UJtONEIlfuDZYCjxHDOtc,5433
+funboost/consumers/rabbitmq_pika_consumerv0.py,sha256=Yr-GJlgtkYB4qx8hKZZRx8PyCGwKAlSvRFKEf-SBXnM,4674
+funboost/consumers/rabbitmq_rabbitpy_consumer.py,sha256=q-DXy2MHgsFfBssVIlqgziFw2jPkxAT4TyeDnlE0zwI,1260
+funboost/consumers/redis_brpoplpush_consumer.py,sha256=rVdlmODLEQ8_k-gXFnaMFK8LaiKu3EiZMG2q5jmG8qk,3031
+funboost/consumers/redis_consumer.py,sha256=f9nASEQUR3VHk5JH5Plf3RqKXmxogfrshu63RaFnfDM,2829
+funboost/consumers/redis_consumer_ack_able.py,sha256=DlZd76FTPo-AUiTreQd7cSiT5QAM5K9rFItAwLt2n5Y,7545
+funboost/consumers/redis_consumer_simple.py,sha256=9D3uvLw_9WOmLmwys1K39DK3gj1ex_q6NXadXwyGwrs,922
 funboost/consumers/redis_filter.py,sha256=TVyT2i9JhmhsJFyQZDx98phTiwBccNTl9fcErEDGXTM,7135
-funboost/consumers/redis_pubsub_consumer.py,sha256=dEMx5SEAAjW5mwtPnzoSEV5P6pV-ADZ_w3s6YxGHl08,1184
-funboost/consumers/redis_stream_consumer.py,sha256=0r-x_ac6Y6UjIlJc9qcKFIWwu9OOiJLQ4LFjfed6u_8,6304
-funboost/consumers/rocketmq_consumer.py,sha256=Re8O6qlx2cd6K82MqUJhBqpzS7YxPURQ6Oip7BvHLMM,1633
-funboost/consumers/sqlachemy_consumer.py,sha256=TV_BbV1PoOzBZAnL5_MB3BENAC7SA6pVgJlIkNvyjpU,1289
-funboost/consumers/tcp_consumer.py,sha256=KgkhctYIAu15KLuHUKffx7vDzofWH98AU5K78E-6aU8,2025
-funboost/consumers/txt_file_consumer.py,sha256=gQe8WxuniETq0geLV9vjzg-mBLV-y2GLNhBEBIGZgE0,1322
-funboost/consumers/udp_consumer.py,sha256=wDfUk9_RFCTjyx5gLbUTwv_LEfV5-POQQ_sGaWjlpjE,1625
-funboost/consumers/zeromq_consumer.py,sha256=TKcU1wOeKW6URfT5UOVEDRjmUCjvNzkgbBVJDLiD2t0,4137
+funboost/consumers/redis_pubsub_consumer.py,sha256=eSy5QBMPaouiQbeGQ3ZaLVpU1BF8g3B_4CAJHFqhmmI,1206
+funboost/consumers/redis_stream_consumer.py,sha256=UMruqW4k_-nehGVRtI6J2eUne6hU4sr6s78gpxUJ7UM,6324
+funboost/consumers/rocketmq_consumer.py,sha256=sqJwxNFOz7c-4Dbk5Rgj_iJqDVwRVCGsw_tMTArGc2o,1653
+funboost/consumers/sqlachemy_consumer.py,sha256=-pY9pvAVUCw_T-1bRKRT37vNGjvv6BK9h-I5kfelpVk,1309
+funboost/consumers/tcp_consumer.py,sha256=hgjcXOtHyGBDS_h_p0gbOtF__Ba6DS1Chk5P9nc6Its,2045
+funboost/consumers/txt_file_consumer.py,sha256=rd8F7liwUfidk7SXY-qF4Iamx-U1NXJBYsOhOudFyyU,1340
+funboost/consumers/udp_consumer.py,sha256=J-G1ZYktXZ_er_1fg3FdSPVl4V_eEIHZXlBadCNpJmE,1643
+funboost/consumers/zeromq_consumer.py,sha256=7V1RwZKtPDDpjKTKj4GWGuz1AGZ83EBHCnWuYN4ooSM,4157
 funboost/contrib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/contrib/queue2queue.py,sha256=zSIOaj9dPjskV0Rzk-T6gLeO0X-vCZb1pQ1YvCCafOM,4703
 funboost/contrib/redis_consume_latest_msg_broker.py,sha256=V-8-pOyotOXNbs2olS7vig-yN1PxRdw_MeLOtpUufJc,1817
 funboost/factories/__init__.py,sha256=s7kKKjR1HU5eMjPD6r5b-SXTVMo1zBp2JjOAtkyt5Yo,178
-funboost/factories/consumer_factory.py,sha256=d7tiN6QVPD1mduCDL4MibLf_ZBmo6DUd3O5VldLlqy8,3357
-funboost/factories/publisher_factotry.py,sha256=kZBoB8lQhd-5kVLfC3-f0HC_E6Jq2ldYVMpOjzfKNrE,4587
+funboost/factories/broker_kind__publsiher_consumer_type_map.py,sha256=FZmb_ntqkEdGJKkYyePJJm8Z3hP2emqGriaCLIz7H4o,8286
+funboost/factories/consumer_factory.py,sha256=3BcdYqTH1UvH3Q0V7eqZ9ePHLyywDr-07fPlTjJeD8w,1032
+funboost/factories/publisher_factotry.py,sha256=52XUvGiloNkKFkKiOcmJxY6FT1VmtNcEI4fJoMS7Mxo,2115
 funboost/function_result_web/app.py,sha256=xUSDBwwDA5wQVWFdFBXj9Y1s7BOh2itUw5pCZl0URMw,4841
 funboost/function_result_web/functions.py,sha256=OIPMxc4jv51qnhBxFGfTZnpMx5p4lQflPoTviDTbJUc,7345
 funboost/function_result_web/__pycache__/app.cpython-37.pyc,sha256=p-jwU7xf31KOJhmhNXqj6J79PTxjMbiTU16gAotpSEw,4045
 funboost/function_result_web/__pycache__/functions.cpython-37.pyc,sha256=KuU8DnYhFpYN0p9rdDXE9mqFuE7eKkcXHCNze3aAdOw,3921
 funboost/function_result_web/static/assets/css/custom.css,sha256=3brvjy2aBOTIXcTUK4NV6dX5wFRqx6K2aLu_jQn63jM,7674
 funboost/function_result_web/static/assets/css/jquery.mCustomScrollbar.min.css,sha256=JHGEmB629pipTkMag9aMaw32I8zle24p3FpsEeI6oZU,42839
 funboost/function_result_web/static/assets/img/user.jpg,sha256=Vz1A99gho-0bKV67Pt2s_zT25mWhNcPe0mWG-0mRl9U,23610
@@ -78,17 +79,18 @@
 funboost/function_result_web/static/images/tick.png,sha256=S9dZYN4HQzw7JsWPw3ut1dQp4OTJ_Uh2Qp2KUDF1Jv8,2912
 funboost/function_result_web/static/images/user.png,sha256=HxLjNc83WZzZEscZRdmVhGKlPXNdp_EKmmYxafuyb3g,622
 funboost/function_result_web/static/js/jquery-1.11.0.min.js,sha256=ryQZ3RXgnqkTz-lNEw-YcEhnMuV3ZODwLqOEbyBBRu4,96383
 funboost/function_result_web/templates/index.html,sha256=dWe-JFQhsDpoNjSsBF4P6SJWp_KvHX8EP_yECS5r7_o,19501
 funboost/function_result_web/templates/login.html,sha256=q37dj7O0LeyiV38Zd5P1Qn_qmhjdFomuYTRY1Yk48Bo,2007
 funboost/publishers/__init__.py,sha256=xqBHlvsJQVPfbdvP84G0LHmVB7-pFBS7vDnX1Uo9pVY,131
 funboost/publishers/base_publisher.py,sha256=davLWo-tSw7gwqF4fMrxlcz-sitZ9kqpfofb0yjp_ok,14894
-funboost/publishers/celery_publisher.py,sha256=ag2s7MzPPrnNdza3u8vcbDJqtiqbQw4lJJzAVuJ6GF0,3897
+funboost/publishers/celery_publisher.py,sha256=gWZDJpgcAc2YaASaHiGmj1WKLE3XLuMZUsvclrYYL94,3660
+funboost/publishers/celery_publisher000.py,sha256=ag2s7MzPPrnNdza3u8vcbDJqtiqbQw4lJJzAVuJ6GF0,3897
 funboost/publishers/confluent_kafka_publisher.py,sha256=cpbyWvZ0T_kM62LWeBKRUuEuMkJAKOof97UUMSz6-Dk,3541
-funboost/publishers/http_publisher.py,sha256=QbVG-dFdKdltCoElHmKpNSMsjpZY3Ibp-r_IzqrkPMk,777
+funboost/publishers/http_publisher.py,sha256=pS3z_AVqH6h4PAgqB7usihvzLJP5ZzfPKQRMQfHrJHQ,753
 funboost/publishers/httpsqs_publisher.py,sha256=7cf5ijwrbp4smq6ofndrKisruAqG0Wzfo_d_7bnLUk4,2783
 funboost/publishers/kafka_publisher.py,sha256=cmlJ0mvwq0Ajlth4VQqwnoe6v_bZ4eIz49GgkiJr-ZU,2160
 funboost/publishers/kombu_publisher.py,sha256=1tsYCngzx0PR9a4cF2vzvzW3S2wUYObKhfvaqOqDNNo,5246
 funboost/publishers/local_python_queue_publisher.py,sha256=veskMS5tjeneYU9HmrJLXZSK9_UT48NzHzcljjOoy3g,1365
 funboost/publishers/mongomq_publisher.py,sha256=xQr3KMQEKksX4OEvzPlCl8v1VeBHaoZtYw2QujOUyGo,1874
 funboost/publishers/mqtt_publisher.py,sha256=NKVDE5R12QL99IXgRjJtF4phyW8QaXKxHkqW5p_kXr4,3050
 funboost/publishers/msg_result_getter.py,sha256=a2ffSE8Rvz1t1KVEt4UxIPsWgcriaHE_Armkac-JrJY,7782
@@ -104,21 +106,21 @@
 funboost/publishers/redis_publisher.py,sha256=AHGSgtlYHVYIVu48lSa5UqdiIU5VtFp7hXhj-wiQx8c,3929
 funboost/publishers/redis_publisher_lpush.py,sha256=xEWuCTtbDcKFLTxGrECrbIVapFfUwqX2-GHenMClu-Q,278
 funboost/publishers/redis_publisher_simple.py,sha256=hLVWiDjy9ObGTmv7Vtrz21d18Fxkb52IfO5ZzaXjzMQ,872
 funboost/publishers/redis_pubsub_publisher.py,sha256=_6s7sbcGOSXxN2ZkBSDk9ILskmbj9cZTQyYHLQTYOuI,721
 funboost/publishers/redis_stream_publisher.py,sha256=DLxFcTlze0IdYFoaRmTcY8GCOaRwbj4aBNbylkt9gRA,2037
 funboost/publishers/rocketmq_publisher.py,sha256=vY82WgutDPsS9px6rukU1d3AexmsT_tqSS2dmX-Pw-c,2343
 funboost/publishers/sqla_queue_publisher.py,sha256=yUbge08K311-jWlFyOUw6g7-Z-flbxEeWCeCTGnJcic,1215
-funboost/publishers/tcp_publisher.py,sha256=e-QoZVpnnjy536fzj43tW_1TtqFb7m_plsoR1yPaHMs,1359
+funboost/publishers/tcp_publisher.py,sha256=RAoMghY93zH9AVnBbCYjUZ1cdri9t91ZcGh_imD--oQ,1335
 funboost/publishers/txt_file_publisher.py,sha256=twTrqRAYnaNmFkXn0nr1xGBjeHCPJStt83voLX3vPao,1380
-funboost/publishers/udp_publisher.py,sha256=0EAwT7IY_02v9YlvDCs53ubDUP8WvWjYYtURzC-DN64,1218
+funboost/publishers/udp_publisher.py,sha256=TOiKrhmCMjx4teqIgdUwRic0lxyK2cupinafsz--wzY,1194
 funboost/publishers/zeromq_publisher.py,sha256=QCsRDtmgxOdVe2F2z3PwvvkoXv1flmrHWo3Nzsx0X7g,1002
 funboost/queues/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/queues/peewee_queue.py,sha256=pQJ0YkBoZRGASzmBoGyluIfdRp4Orv6l1bqQpHNdPtY,4982
-funboost/queues/sqla_queue.py,sha256=pYqQWJkimKsxtIarAauVi3vv5XeZdIIwYTbuXjcpZrU,11186
+funboost/queues/sqla_queue.py,sha256=PxkMyXHCA_Je7H_p8c81QT7qN8x8Fq6NVmwli7PPhhg,11024
 funboost/timing_job/__init__.py,sha256=xLZNI64seZV5BT6jc8yGDfqhJ01wSpZIqVcDsUNI8yk,4098
 funboost/timing_job/apscheduler_use_mysql_store.py,sha256=zIeK2LETm8m3VX7K6but8YAQOZomfO-P6AKLqeluxys,418
 funboost/timing_job/apscheduler_use_redis_store.py,sha256=KO35PzALht0EdozEXxa7uEzu7As8iON6mksU9ZOVDr0,868
 funboost/timing_job/push_fun_for_apscheduler_use_db.py,sha256=yo3m3iRLZKjicRw9JHZNLqFKO9jk0csNe96fEVhRltg,996
 funboost/utils/__init__.py,sha256=9YTXH5jt-_MulaWy5cbIpiJghy-fVQU9Gd1RHSajI94,1951
 funboost/utils/apscheduler_monkey.py,sha256=CcUISbqX6nMWSxr_QjZ26IvvhUk_ojYZWRaKenpsKfE,3124
 funboost/utils/block_exit.py,sha256=BnfxNYo3lnmhk686RAEoc4u3D4RU_iEMMMgu5L8gIuI,96
@@ -205,12 +207,12 @@
 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-37.pyc,sha256=67Zqz4tjErzQSm9FM9mGaY3uMHYOUj3QYKtPqJQvQpE,303
 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-39.pyc,sha256=a1ajayGg3JjQz--IC3-6YQHRFStG9etoieY8mXEdJ6Q,311
 funboost/utils/pysnooper_ydf/__init__.py,sha256=ctbQdJpLVZ5g_PPstj7Xaqcl0sMIgvUGwZXtcogYyHA,909
 funboost/utils/pysnooper_ydf/pycompat.py,sha256=ehsCfjsLdwoK0_o5fwYWDo3WeqCVfHW5lxekrEZxq4Y,2243
 funboost/utils/pysnooper_ydf/tracer.py,sha256=DYxYeRFSH1jXy4OTB5KIAgQm2EHRWEOwq3EXJig7Yrk,19131
 funboost/utils/pysnooper_ydf/utils.py,sha256=evSmGi_Oul7vSP47AJ0DLjFwoCYCfunJZ1mWxAkwPZw,2753
 funboost/utils/pysnooper_ydf/variables.py,sha256=QejRDESBA06KG9OH4sBT4J1M55eaU29EIHg8K_igaXo,3693
-funboost-20.4.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-funboost-20.4.dist-info/METADATA,sha256=3shGFzjFDKlgfa8Ky0AVdXtWE0EDIDXHz5JBmHpPHuc,24442
-funboost-20.4.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-funboost-20.4.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
-funboost-20.4.dist-info/RECORD,,
+funboost-20.5.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+funboost-20.5.dist-info/METADATA,sha256=sKm7DNRngKJX8aXAdcf-C-JwQUTu9myQzRFgNe6_cOI,25817
+funboost-20.5.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
+funboost-20.5.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
+funboost-20.5.dist-info/RECORD,,
```

