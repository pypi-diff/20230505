# Comparing `tmp/django_channels_graphql_ws-1.0.0rc4.tar.gz` & `tmp/django_channels_graphql_ws-1.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_channels_graphql_ws-1.0.0rc4.tar", max compression
+gzip compressed data, was "django_channels_graphql_ws-1.0.0rc5.tar", max compression
```

## Comparing `django_channels_graphql_ws-1.0.0rc4.tar` & `django_channels_graphql_ws-1.0.0rc5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-05-02 12:50:55.308791 django_channels_graphql_ws-1.0.0rc4/LICENSE
--rw-r--r--   0        0        0     1433 2023-05-02 12:50:55.309416 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/__init__.py
--rw-r--r--   0        0        0    10111 2023-05-02 12:50:55.309876 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/client.py
--rw-r--r--   0        0        0     2637 2023-05-02 12:50:55.310121 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/dict_as_object.py
--rw-r--r--   0        0        0    53350 2023-05-04 09:11:03.427948 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/graphql_ws_consumer.py
--rw-r--r--   0        0        0     3850 2023-05-02 12:50:55.310854 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/serializer.py
--rw-r--r--   0        0        0    16451 2023-05-02 12:50:55.311452 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/subscription.py
--rw-r--r--   0        0        0     4816 2023-05-02 12:50:55.311701 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/testing.py
--rw-r--r--   0        0        0     6939 2023-05-02 12:50:55.311889 django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/transport.py
--rw-r--r--   0        0        0     8478 2023-05-04 09:11:03.428885 django_channels_graphql_ws-1.0.0rc4/pyproject.toml
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 django_channels_graphql_ws-1.0.0rc4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-02 12:50:55.308791 django_channels_graphql_ws-1.0.0rc5/LICENSE
+-rw-r--r--   0        0        0     1433 2023-05-02 12:50:55.309416 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/__init__.py
+-rw-r--r--   0        0        0    10108 2023-05-05 11:21:54.816821 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/client.py
+-rw-r--r--   0        0        0     2637 2023-05-02 12:50:55.310121 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/dict_as_object.py
+-rw-r--r--   0        0        0    51298 2023-05-05 10:28:17.582938 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/graphql_ws_consumer.py
+-rw-r--r--   0        0        0     3850 2023-05-02 12:50:55.310854 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/serializer.py
+-rw-r--r--   0        0        0    16185 2023-05-05 10:28:17.583453 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/subscription.py
+-rw-r--r--   0        0        0     4883 2023-05-05 12:36:22.593202 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/testing.py
+-rw-r--r--   0        0        0     6939 2023-05-02 12:50:55.311889 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/transport.py
+-rw-r--r--   0        0        0     8470 2023-05-05 12:44:54.296330 django_channels_graphql_ws-1.0.0rc5/pyproject.toml
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 django_channels_graphql_ws-1.0.0rc5/PKG-INFO
```

### Comparing `django_channels_graphql_ws-1.0.0rc4/LICENSE` & `django_channels_graphql_ws-1.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/__init__.py` & `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/__init__.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/client.py` & `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,17 +143,18 @@
             )
         if assert_id is not None:
             assert response["id"] == assert_id, "Response id != expected id!"
 
         payload = response.get("payload", None)
         if payload is not None and "errors" in payload:
             raise GraphqlWsResponseError(response)
-        if not raw_response:
-            return payload
-        return response
+
+        if raw_response:
+            return response
+        return payload
 
     async def execute(self, query, variables=None):
         """Execute query or mutation request and wait for the reply.
 
         Args:
             query: A GraphQL query string. We `dedent` it, so you do not
                 have to.
```

### Comparing `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/dict_as_object.py` & `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/dict_as_object.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/graphql_ws_consumer.py` & `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/graphql_ws_consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,22 +42,24 @@
 import functools
 import inspect
 import logging
 import threading
 import time
 import traceback
 import weakref
-from collections.abc import Sequence
 from typing import (
     Any,
     AsyncIterator,
     Awaitable,
     Callable,
     Dict,
+    Iterable,
+    List,
     Optional,
+    Tuple,
     Type,
     Union,
     cast,
 )
 
 import channels.db
 import channels.generic.websocket as ch_websocket
@@ -143,18 +145,14 @@
     # For more information read docs:
     # - https://docs.graphene-python.org/en/latest/execution/middleware/#middleware
     # - https://graphql-core-3.readthedocs.io/en/latest/diffs.html#custom-middleware
     # Docs about async middlewares are still missing - read the
     # GraphQL-core sources to know more.
     middleware: Optional[graphql.Middleware] = None
 
-    # Subscription implementation shall return this to tell consumer
-    # to suppress subscription notification.
-    SKIP = object()
-
     async def on_connect(self, payload):
         """Client connection handler.
 
         Called after CONNECTION_INIT message from client. Overwrite and
         raise an Exception to tell the server to reject the connection
         when it's necessary.
 
@@ -185,69 +183,20 @@
     @dataclasses.dataclass
     class _SubInf:
         """Subscription information structure."""
 
         # Subscription identifier - protocol operation identifier.
         sid: int
         # Subscription groups the subscription belongs to.
-        groups: list[str]
+        groups: List[str]
         # A function which triggets subscription.
         enqueue_notification: Callable[[Any], None]
         # The callback to invoke when client unsubscribes.
         unsubscribed_callback: Callable[..., Awaitable[None]]
 
-    class _SubscriptionExecutionContext(graphql.ExecutionContext):
-        """Special execution context for subscriptions.
-
-        Subscription `publish` method is called via `graphql.execute`
-        like normal resolver. But subscription may return
-        `GraphqlWsConsumer.SKIP` object instead of declared result type.
-        When `graphql.execute` can not build resulting type from the
-        resolver return value it sets result to `None` which may lead to
-        GraphQL errors in case of required field or confuse skipped
-        event with missing value. We have to promote
-        `GraphqlWsConsumer.SKIP` value to the GraphQL operation results
-        and remove skipped values from the final response.
-        """
-
-        @staticmethod
-        def build_response(
-            data: Optional[Dict[str, Any]], errors: list[graphql.GraphQLError]
-        ) -> graphql.ExecutionResult:
-            """Remove skipped subscription events from results.
-
-            `data` is a dictionary where the key is subscription field
-            name and value is a subscription resolver result. Value will
-            be `GraphqlWsConsumer.SKIP` object for skipped events.
-            """
-            if data:
-                data = {
-                    field_name: value
-                    for field_name, value in data.items()
-                    if value is not GraphqlWsConsumer.SKIP
-                }
-            return graphql.ExecutionContext.build_response(data, errors)
-
-        def complete_value(
-            self,
-            return_type: graphql.GraphQLOutputType,
-            field_nodes: list[graphql.FieldNode],
-            info: graphql.GraphQLResolveInfo,
-            path: graphql.pyutils.Path,
-            result: Any,
-        ):
-            """Do not create return_type value for skipped events.
-
-            We will remove `GraphqlWsConsumer.SKIP` marks from the final
-            result in the `build_response` method.
-            """
-            if result is GraphqlWsConsumer.SKIP:
-                return result
-            return super().complete_value(return_type, field_nodes, info, path, result)
-
     def __init__(self, *args, **kwargs):
         """Consumer constructor."""
 
         assert self.schema is not None, (
             "An attribute 'schema' is not set! Subclasses must specify "
             "the schema which processes GraphQL subscription queries."
         )
@@ -326,15 +275,15 @@
             LOG.warning("WebSocket connection closed without a code!")
         elif code <= 1001:
             LOG.debug("WebSocket connection closed with code: %s.", code)
         else:
             LOG.warning("WebSocket connection closed with code: %s!", code)
 
         # The list of awaitables to simultaneously wait at the end.
-        waitlist: list[asyncio.Task] = []
+        waitlist: List[asyncio.Task] = []
 
         # Unsubscribe from the Channels groups.
         waitlist += [
             asyncio.create_task(
                 self._channel_layer.group_discard(group, self.channel_name)
             )
             for group in self._sids_by_group
@@ -622,15 +571,14 @@
                     context_value=context,
                     subscribe_field_resolver=functools.partial(
                         self._on_gql_start__initialize_subscription_stream,
                         op_id,
                         op_name,
                     ),
                     middleware=self._middleware,
-                    execution_context_class=self._SubscriptionExecutionContext,
                 )
 
                 # When subscr_result is an AsyncGenerator, consume
                 # stream of notifications and send them to clients.
                 if not isinstance(subscr_result, graphql.ExecutionResult):
                     stream = cast(AsyncIterator[graphql.ExecutionResult], subscr_result)
                     # Send subscription activation message (if enabled)
@@ -757,18 +705,18 @@
                 await self._send_gql_complete(op_id)
             else:
                 # Respond with general error responce.
                 await self._send_gql_error(op_id, ex)
 
     async def _on_gql_start__parse_query(
         self, op_name: str, query: str
-    ) -> tuple[
+    ) -> Tuple[
         Optional[graphql.DocumentNode],
         Optional[graphql.OperationDefinitionNode],
-        Optional[Sequence[graphql.GraphQLError]],
+        Optional[Iterable[graphql.GraphQLError]],
     ]:
         """Parse and validate GraphQL query.
 
         It is highly likely that the same operation will be parsed many
         times, so this function is wrapped with LRU cache.
 
         This async function offloads the GraphQL processing to the
@@ -788,40 +736,40 @@
 
         res = await channels.db.database_sync_to_async(
             self._on_gql_start__parse_query_sync_cached
         )(op_name, query)
 
         doc_ast: Optional[graphql.DocumentNode] = res[0]
         op_ast: Optional[graphql.OperationDefinitionNode] = res[1]
-        errors: Optional[Sequence[graphql.GraphQLError]] = res[2]
+        errors: Optional[Iterable[graphql.GraphQLError]] = res[2]
 
         return (doc_ast, op_ast, errors)
 
     @functools.lru_cache(maxsize=128)
     def _on_gql_start__parse_query_sync_cached(
         self, op_name: str, query: str
-    ) -> tuple[
+    ) -> Tuple[
         Optional[graphql.DocumentNode],
         Optional[graphql.OperationDefinitionNode],
-        Optional[Sequence[graphql.GraphQLError]],
+        Optional[Iterable[graphql.GraphQLError]],
     ]:
         """Parse and validate GraphQL query. Cached sync implementation.
 
         This is a part of START message processing routine so the name
         prefixed with `_on_gql_start__` to make this explicit.
         """
 
         # Parsing.
         try:
             doc_ast = graphql.parse(query)
         except graphql.GraphQLError as ex:
             return None, None, [ex]
 
         # Validation.
-        validation_errors: list[graphql.GraphQLError] = graphql.validate(
+        validation_errors: List[graphql.GraphQLError] = graphql.validate(
             self.schema.graphql_schema, doc_ast
         )
         if validation_errors:
             return None, None, validation_errors
 
         op_ast = graphql.utilities.get_operation_ast(doc_ast, op_name)
 
@@ -881,15 +829,21 @@
                 variable_values,
                 operation_name,
                 field_resolver,
                 middleware=middleware,
                 execution_context_class=execution_context_class,
             )  # type: ignore
             result = await result if inspect.isawaitable(result) else result
-            return cast(graphql.ExecutionResult, result)
+            result = cast(graphql.ExecutionResult, result)
+            # Skip notification if subscription returned `None`.
+            if not result.errors and result.data:
+                for key in list(result.data.keys()):
+                    if result.data[key] is None:
+                        result.data.pop(key)
+            return result
 
         # Map every source value to a ExecutionResult value.
         return graphql.MapAsyncIterator(result_or_stream, map_source_to_response)
 
     async def _on_gql_start__initialize_subscription_stream(
         self,
         operation_id: int,
@@ -948,15 +902,15 @@
             subclass_groups = []
 
         groups += [subscription_class._group_name(group) for group in subclass_groups]
 
         # The subscription notification queue. Required to preserve the
         # order of notifications within a single subscription.
         queue_size = subscription_class.notification_queue_limit
-        if not queue_size or queue_size < 0:
+        if queue_size is None or queue_size <= 0:
             # Take default limit from the Consumer class.
             queue_size = self.subscription_notification_queue_limit
         # The subscription notification queue.
         # NOTE: The asyncio.Queue class is not thread-safe. So use the
         # `notification_queue_lock` as a guard while reading or writing
         # to the queue.
         notification_queue: asyncio.Queue = asyncio.Queue(maxsize=queue_size)
@@ -1067,15 +1021,15 @@
         # Currently only subscriptions can be stopped. But we see but
         # some clients (e.g. GraphiQL) send the stop message even for
         # queries and mutations. We also see that the Apollo server
         # ignores such messages, so we ignore them as well.
         if op_id not in self._subscriptions:
             return
 
-        waitlist: list[asyncio.Task] = []
+        waitlist: List[asyncio.Task] = []
 
         # Remove the subscription from the registry.
         subinf = self._subscriptions.pop(op_id)
 
         # Cancel the task which watches the notification queue.
         consumer_task = self._notifier_tasks.pop(op_id, None)
         if consumer_task:
@@ -1119,15 +1073,15 @@
         """Connection error sent in reply to the `connection_init`."""
         LOG.warning("GraphQL connection error: %s!", error, exc_info=error)
         await self.send_json(
             {"type": "connection_error", "payload": self._format_error(error)}
         )
 
     async def _send_gql_data(
-        self, op_id, data: Optional[dict], errors: Optional[Sequence[Exception]]
+        self, op_id, data: Optional[dict], errors: Optional[Iterable[Exception]]
     ):
         """Send GraphQL `data` message to the client.
 
         Args:
             data: Dict with GraphQL query response.
             errors: List of exceptions occurred during processing the
                 GraphQL query. (Errors happened in resolvers.)
```

### Comparing `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/serializer.py` & `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/serializer.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/subscription.py` & `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/subscription.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         [async] publish(payload, info, *args, **kwds):
             This method invoked each time subscription "triggers".
             Raising an exception here will lead to sending the
             notification with the error. Technically the WebSocket
             message will contain extra field "extensions.code" holding
             the classname of the exception raised. To suppress the
-            notification return `Subscription.SKIP`.
+            notification return `None`.
 
             Can be implemented as both asynchronous (`async def`) or
             synchronous (`def`) function. Asynchronous implementation
             runs blazingly fast in the main event loop of the main
             thread. You must be careful with blocking calls though. You
             can offload blocking operations to a thread in such cases.
             Synchronous implementation always runs in a worker thread
@@ -82,17 +82,15 @@
             Args:
                 payload: The `payload` from the `broadcast` invocation.
                 info: The value of `info.context` is a Channels
                     websocket context with all the connection
                     information.
                 args, kwds: Values of the GraphQL subscription inputs.
             Returns:
-                The same that any Graphene resolver returns. Returning a
-                special object `Subscription.SKIP` indicates that this
-                notification must not be sent to the client at all.
+                The same that any Graphene resolver returns.
 
         [async] subscribe(root, info, *args, **kwds):
             Called when client subscribes. Define this to do some extra
             work when client subscribes and to group subscriptions into
             different subscription groups. Method signature is the same
             as in other GraphQL "resolver" methods but it may return the
             subscription groups names to put the subscription into.
@@ -153,17 +151,14 @@
 
     NOTE: If you call any of these methods from the asynchronous context
     then `await` the result of the call.
     """
 
     # ----------------------------------------------------------------------- PUBLIC API
 
-    # Return this from the `publish` to suppress the notification.
-    SKIP = GraphqlWsConsumer.SKIP
-
     # Subscription notifications queue limit. Set this to control the
     # amount of notifications server keeps in the queue when
     # notifications come faster than server processes them. Setting this
     # to 1 drops all notifications in the queue except the latest one.
     # Useful to skip intermediate notifications, e.g. progress reports.
     notification_queue_limit: Optional[int] = None
```

### Comparing `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/testing.py` & `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 
 class GraphqlWsTransport(channels_graphql_ws.transport.GraphqlWsTransport):
     """Testing client transport to work without WebSocket connection.
 
     Client is implemented based on the Channels `WebsocketCommunicator`.
     """
 
+    # Slightly reduce timeout in testing.
+    TIMEOUT: float = 30
+
     def __init__(self, application, path, communicator_kwds=None):
         """Constructor."""
         self._comm = channels.testing.WebsocketCommunicator(
             application=application,
             path=path,
             subprotocols=["graphql-ws"],
             **(communicator_kwds or {}),
```

### Comparing `django_channels_graphql_ws-1.0.0rc4/channels_graphql_ws/transport.py` & `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/transport.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc4/pyproject.toml` & `django_channels_graphql_ws-1.0.0rc5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 build-backend = "poetry.core.masonry.api"
 
 # --------------------------------------------------------------- POETRY
 # Python packaging and dependency management.
 # Docs: https://python-poetry.org/docs/
 [tool.poetry]
 name = "django-channels-graphql-ws"
-version = "v1.0.0rc4"
+version = "v1.0.0rc5"
 description = """Django Channels based WebSocket GraphQL server with Graphene-like subscriptions"""
 authors = ["Alexander A. Prokhorov <alexander.prokhorov@datadvance.net>"]
 homepage = "https://github.com/datadvance/DjangoChannelsGraphqlWs"
 repository = "https://github.com/datadvance/DjangoChannelsGraphqlWs"
 license = "MIT"
 packages = [
     { include = "channels_graphql_ws/" },
@@ -79,15 +79,15 @@
 pytest-xdist = "*"
 tox = "*"
 
 # ---------------------------------------------------------------- BLACK
 # Black - the uncompromising code formatter.
 # https://black.readthedocs.io/en/stable/index.html
 [tool.black]
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310']
 
 # ---------------------------------------------------------------- ISORT
 # Isort configuration.
 # Docs: https://github.com/timothycrosley/isort/wiki/isort-Settings
 [tool.isort]
 profile="black"
```

### Comparing `django_channels_graphql_ws-1.0.0rc4/PKG-INFO` & `django_channels_graphql_ws-1.0.0rc5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-channels-graphql-ws
-Version: 1.0.0rc4
+Version: 1.0.0rc5
 Summary: Django Channels based WebSocket GraphQL server with Graphene-like subscriptions
 Home-page: https://github.com/datadvance/DjangoChannelsGraphqlWs
 License: MIT
 Author: Alexander A. Prokhorov
 Author-email: alexander.prokhorov@datadvance.net
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

