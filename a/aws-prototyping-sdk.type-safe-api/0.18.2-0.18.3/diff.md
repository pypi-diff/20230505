# Comparing `tmp/aws_prototyping_sdk.type_safe_api-0.18.2.tar.gz` & `tmp/aws_prototyping_sdk.type_safe_api-0.18.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.18.2.tar", last modified: Thu May  4 06:18:26 2023, max compression
+gzip compressed data, was "aws_prototyping_sdk.type_safe_api-0.18.3.tar", last modified: Fri May  5 00:19:26 2023, max compression
```

## Comparing `aws_prototyping_sdk.type_safe_api-0.18.2.tar` & `aws_prototyping_sdk.type_safe_api-0.18.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:18:26.326030 aws_prototyping_sdk.type_safe_api-0.18.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    56337 2023-05-04 06:18:26.326030 aws_prototyping_sdk.type_safe_api-0.18.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    55396 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 06:18:26.326030 aws_prototyping_sdk.type_safe_api-0.18.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:18:26.322030 aws_prototyping_sdk.type_safe_api-0.18.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:18:26.322030 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:18:26.322030 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/type_safe_api/
--rw-r--r--   0 runner    (1001) docker     (123)   288160 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/type_safe_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:18:26.322030 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/type_safe_api/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   855054 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:18:17.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/type_safe_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:18:26.322030 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    56337 2023-05-04 06:18:26.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-04 06:18:26.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:18:26.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-04 06:18:26.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 06:18:26.000000 aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:19:26.521305 aws_prototyping_sdk.type_safe_api-0.18.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-05 00:19:18.000000 aws_prototyping_sdk.type_safe_api-0.18.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 00:19:18.000000 aws_prototyping_sdk.type_safe_api-0.18.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    61023 2023-05-05 00:19:26.521305 aws_prototyping_sdk.type_safe_api-0.18.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    60082 2023-05-05 00:19:18.000000 aws_prototyping_sdk.type_safe_api-0.18.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 00:19:18.000000 aws_prototyping_sdk.type_safe_api-0.18.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 00:19:26.521305 aws_prototyping_sdk.type_safe_api-0.18.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-05 00:19:18.000000 aws_prototyping_sdk.type_safe_api-0.18.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:19:26.517305 aws_prototyping_sdk.type_safe_api-0.18.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:19:26.517305 aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:19:26.517305 aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk/type_safe_api/
+-rw-r--r--   0 runner    (1001) docker     (123)   303094 2023-05-05 00:19:18.000000 aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk/type_safe_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:19:26.521305 aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk/type_safe_api/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-05 00:19:18.000000 aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   877854 2023-05-05 00:19:18.000000 aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:19:18.000000 aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk/type_safe_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:19:26.517305 aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk.type_safe_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    61023 2023-05-05 00:19:26.000000 aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-05 00:19:26.000000 aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:19:26.000000 aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-05 00:19:26.000000 aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 00:19:26.000000 aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.2/LICENSE` & `aws_prototyping_sdk.type_safe_api-0.18.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.2/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.18.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: aws_prototyping_sdk.type_safe_api
-Version: 0.18.2
-Summary: @aws-prototyping-sdk/type-safe-api
-Home-page: https://github.com/aws/aws-prototyping-sdk
-Author: AWS APJ COPE<apj-cope@amazon.com>
-License: Apache-2.0
-Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Typing :: Typed
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Type Safe API
 
 Define your APIs using [Smithy](https://smithy.io/2.0/) or [OpenAPI v3](https://swagger.io/specification/), and leverage the power of generated client and server types, infrastructure, documentation, and automatic input validation!
 
 This package vends a projen project type which allows you to define an API using either [Smithy](https://smithy.io/2.0/) or [OpenAPI v3](https://swagger.io/specification/), and a construct which manages deploying this API in API Gateway, given an integration (eg a lambda) for every operation.
 
 The project will generate "runtime" projects from your API definition in your desired languages, which can be utilised both client side for interacting with your API, or server side for implementing your API. The project also generates a type-safe CDK construct which ensures an integration is provided for every API operation.
@@ -72,15 +48,19 @@
   // CDK infrastructure in TypeScript
   infrastructure: {
     language: Language.TYPESCRIPT,
   },
   // Generate HTML documentation
   documentation: {
     formats: [DocumentationFormat.HTML_REDOC],
-  }
+  },
+  // Generate react-query hooks to interact with the UI from a React website
+  library: {
+    libraries: [Library.TYPESCRIPT_REACT_QUERY_HOOKS],
+  },
 });
 
 // Create a CDK infrastructure project. Can also consider PDKPipelineTsProject as an alternative!
 const infra = new AwsCdkTypeScriptApp({ ... });
 
 // Infrastructure can depend on the generated API infrastructure and runtime
 infra.addDeps(api.infrastructure.typescript!.package.packageName);
@@ -270,14 +250,16 @@
     |_ python
     |_ java
 |_ documentation/ - generated documentation in the formats you specified
     |_ html2
     |_ html_redoc
     |_ plantuml
     |_ markdown
+|_ library/ - generated libraries if specified
+    |_ typescript-react-query-hooks
 ```
 
 ### Smithy IDL
 
 Please refer to the [Smithy documentation](https://smithy.io/2.0/quickstart.html) for how to write models in Smithy. A basic example is provided below:
 
 ```smithy
@@ -1054,14 +1036,154 @@
         return SayHello200Response.of(HelloResponse.builder()
                 .message(String.format("Hello %s!", sayHelloRequestInput.getInput().getRequestParameters().getName()))
                 .build());
     }
 }
 ```
 
+### Libraries
+
+Libraries are generated code projects which are not fully-fledged runtime languages.
+
+#### TypeScript React Query Hooks
+
+This library contains generated [react-query](https://tanstack.com/query/latest) hooks for interacting with your API from a React website. You can generate these by adding the following options to your `TypeSafeApiProject` in your `.projenrc`:
+
+```python
+new TypeSafeApiProject({
+  library: {
+    libraries: [Library.TYPESCRIPT_REACT_QUERY_HOOKS],
+  },
+  ...
+});
+```
+
+##### Usage in a React Website
+
+First, make sure you create an instance of the API client (making sure to set the base URL and fetch instance). For example:
+
+```python
+export const useMyApiClient = () => useMemo(() => new MyApi(new Configuration({
+  basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
+  fetchApi: window.fetch.bind(window),
+})), []);
+```
+
+Note that if you are using the [Cloudscape React Website](../cloudscape-react-ts-website/README.md) with [AWS NorthStar](https://aws.github.io/aws-northstar/) and IAM (Sigv4) Auth for your API, you can use NorthStar's [`useSigv4Client()` hook](https://aws.github.io/aws-northstar/?path=/story/components-cognitoauth-sigv4client-docs--page) to create
+an instance of `fetch` which will sign requests with the logged in user's credentials. For example:
+
+```python
+export const useMyApiClient = () => {
+  const { client } = useSigv4Client();
+  return useMemo(() => client.current ? new MyApi(new Configuration({
+    basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
+    fetchApi: client.current,
+  })) : undefined, [client.current]);
+};
+```
+
+Next, instantiate the client provider above where you would like to use the hooks in your component hierarchy (such as above your router). For example:
+
+```tsx
+const api = useMyApiClient();
+
+return api ? (
+  <MyApiClientContext.Provider value={api}>
+    { /* Components within the provider may make use of the hooks */ }
+  </MyApiClientContext.Provider>
+) : <p>Loading...</p>;
+```
+
+Finally, you can import and use your generated hooks. For example:
+
+```tsx
+export const MyComponent: FC<MyComponentProps> = () => {
+  const sayHello = useSayHello({ name: 'World' });
+
+  return (
+    sayHello.isLoading ? (
+      <p>Loading...</p>
+    ) : (
+      sayHello.isError ? (
+        <p>Error!</p>
+      ) : (
+        <h1>{sayHello.data.message}</h1>
+      )
+    )
+  );
+};
+```
+
+##### Paginated Operations
+
+You can generate `useInfiniteQuery` hooks instead of `useQuery` hooks for paginated API operations, by making use of the vendor extension `x-paginated` in your operation in the OpenAPI specification. You must specify both the `inputToken` and `outputToken`, which indicate the properties from the input and output used for pagination. For example in OpenAPI:
+
+```yaml
+paths:
+  /pets:
+    get:
+      x-paginated:
+        # Input property with the token to request the next page
+        inputToken: nextToken
+        # Output property with the token to request the next page
+        outputToken: nextToken
+      parameters:
+        - in: query
+          name: nextToken
+          schema:
+            type: string
+          required: true
+      responses:
+        200:
+          description: Successful response
+          content:
+            application/json:
+              schema:
+                type: object
+                properties:
+                  nextToken:
+                    type: string
+```
+
+In Smithy, until [custom vendor extensions can be rendered via traits](https://github.com/awslabs/smithy/pull/1609), you can add the `x-paginated` vendor extension via `smithyBuildOptions` in your `TypeSafeApiProject`, for example:
+
+```python
+new TypeSafeApiProject({
+  model: {
+    language: ModelLanguage.SMITHY,
+    options: {
+      smithy: {
+        serviceName: {
+          namespace: 'com.mycompany',
+          serviceName: 'MyApi',
+        },
+        smithyBuildOptions: {
+          projections: {
+            openapi: {
+              plugins: {
+                openapi: {
+                  jsonAdd: {
+                    // Add the x-paginated vendor extension to the GET /pets operation
+                    '/paths/~1pets/get/x-paginated': {
+                      inputToken: 'nextToken',
+                      outputToken: 'nextToken',
+                    },
+                  },
+                },
+              },
+            },
+          },
+        },
+      },
+    },
+  },
+  ...
+});
+```
+
 ### Quick Start: Python
 
 This guide assumes you want to write your CDK infrastructure in Python and your lambda handlers in Python, however note that you your infrastructure language and lambda handler language(s) are not tied to one another, you can mix and match as you like. Just specify the language in `runtime.languages` for any language you would like to write lambda handlers in.
 
 #### Create Your API Project
 
 Use the project in your `.projenrc.ts`. It can either be part of an [`nx-monorepo`](../nx-monorepo/README.md) (recommended) or used in a standalone fashion.
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.2/README.md` & `aws_prototyping_sdk.type_safe_api-0.18.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: aws_prototyping_sdk.type_safe_api
+Version: 0.18.3
+Summary: @aws-prototyping-sdk/type-safe-api
+Home-page: https://github.com/aws/aws-prototyping-sdk
+Author: AWS APJ COPE<apj-cope@amazon.com>
+License: Apache-2.0
+Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Type Safe API
 
 Define your APIs using [Smithy](https://smithy.io/2.0/) or [OpenAPI v3](https://swagger.io/specification/), and leverage the power of generated client and server types, infrastructure, documentation, and automatic input validation!
 
 This package vends a projen project type which allows you to define an API using either [Smithy](https://smithy.io/2.0/) or [OpenAPI v3](https://swagger.io/specification/), and a construct which manages deploying this API in API Gateway, given an integration (eg a lambda) for every operation.
 
 The project will generate "runtime" projects from your API definition in your desired languages, which can be utilised both client side for interacting with your API, or server side for implementing your API. The project also generates a type-safe CDK construct which ensures an integration is provided for every API operation.
@@ -48,15 +72,19 @@
   // CDK infrastructure in TypeScript
   infrastructure: {
     language: Language.TYPESCRIPT,
   },
   // Generate HTML documentation
   documentation: {
     formats: [DocumentationFormat.HTML_REDOC],
-  }
+  },
+  // Generate react-query hooks to interact with the UI from a React website
+  library: {
+    libraries: [Library.TYPESCRIPT_REACT_QUERY_HOOKS],
+  },
 });
 
 // Create a CDK infrastructure project. Can also consider PDKPipelineTsProject as an alternative!
 const infra = new AwsCdkTypeScriptApp({ ... });
 
 // Infrastructure can depend on the generated API infrastructure and runtime
 infra.addDeps(api.infrastructure.typescript!.package.packageName);
@@ -246,14 +274,16 @@
     |_ python
     |_ java
 |_ documentation/ - generated documentation in the formats you specified
     |_ html2
     |_ html_redoc
     |_ plantuml
     |_ markdown
+|_ library/ - generated libraries if specified
+    |_ typescript-react-query-hooks
 ```
 
 ### Smithy IDL
 
 Please refer to the [Smithy documentation](https://smithy.io/2.0/quickstart.html) for how to write models in Smithy. A basic example is provided below:
 
 ```smithy
@@ -1030,14 +1060,154 @@
         return SayHello200Response.of(HelloResponse.builder()
                 .message(String.format("Hello %s!", sayHelloRequestInput.getInput().getRequestParameters().getName()))
                 .build());
     }
 }
 ```
 
+### Libraries
+
+Libraries are generated code projects which are not fully-fledged runtime languages.
+
+#### TypeScript React Query Hooks
+
+This library contains generated [react-query](https://tanstack.com/query/latest) hooks for interacting with your API from a React website. You can generate these by adding the following options to your `TypeSafeApiProject` in your `.projenrc`:
+
+```python
+new TypeSafeApiProject({
+  library: {
+    libraries: [Library.TYPESCRIPT_REACT_QUERY_HOOKS],
+  },
+  ...
+});
+```
+
+##### Usage in a React Website
+
+First, make sure you create an instance of the API client (making sure to set the base URL and fetch instance). For example:
+
+```python
+export const useMyApiClient = () => useMemo(() => new MyApi(new Configuration({
+  basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
+  fetchApi: window.fetch.bind(window),
+})), []);
+```
+
+Note that if you are using the [Cloudscape React Website](../cloudscape-react-ts-website/README.md) with [AWS NorthStar](https://aws.github.io/aws-northstar/) and IAM (Sigv4) Auth for your API, you can use NorthStar's [`useSigv4Client()` hook](https://aws.github.io/aws-northstar/?path=/story/components-cognitoauth-sigv4client-docs--page) to create
+an instance of `fetch` which will sign requests with the logged in user's credentials. For example:
+
+```python
+export const useMyApiClient = () => {
+  const { client } = useSigv4Client();
+  return useMemo(() => client.current ? new MyApi(new Configuration({
+    basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
+    fetchApi: client.current,
+  })) : undefined, [client.current]);
+};
+```
+
+Next, instantiate the client provider above where you would like to use the hooks in your component hierarchy (such as above your router). For example:
+
+```tsx
+const api = useMyApiClient();
+
+return api ? (
+  <MyApiClientContext.Provider value={api}>
+    { /* Components within the provider may make use of the hooks */ }
+  </MyApiClientContext.Provider>
+) : <p>Loading...</p>;
+```
+
+Finally, you can import and use your generated hooks. For example:
+
+```tsx
+export const MyComponent: FC<MyComponentProps> = () => {
+  const sayHello = useSayHello({ name: 'World' });
+
+  return (
+    sayHello.isLoading ? (
+      <p>Loading...</p>
+    ) : (
+      sayHello.isError ? (
+        <p>Error!</p>
+      ) : (
+        <h1>{sayHello.data.message}</h1>
+      )
+    )
+  );
+};
+```
+
+##### Paginated Operations
+
+You can generate `useInfiniteQuery` hooks instead of `useQuery` hooks for paginated API operations, by making use of the vendor extension `x-paginated` in your operation in the OpenAPI specification. You must specify both the `inputToken` and `outputToken`, which indicate the properties from the input and output used for pagination. For example in OpenAPI:
+
+```yaml
+paths:
+  /pets:
+    get:
+      x-paginated:
+        # Input property with the token to request the next page
+        inputToken: nextToken
+        # Output property with the token to request the next page
+        outputToken: nextToken
+      parameters:
+        - in: query
+          name: nextToken
+          schema:
+            type: string
+          required: true
+      responses:
+        200:
+          description: Successful response
+          content:
+            application/json:
+              schema:
+                type: object
+                properties:
+                  nextToken:
+                    type: string
+```
+
+In Smithy, until [custom vendor extensions can be rendered via traits](https://github.com/awslabs/smithy/pull/1609), you can add the `x-paginated` vendor extension via `smithyBuildOptions` in your `TypeSafeApiProject`, for example:
+
+```python
+new TypeSafeApiProject({
+  model: {
+    language: ModelLanguage.SMITHY,
+    options: {
+      smithy: {
+        serviceName: {
+          namespace: 'com.mycompany',
+          serviceName: 'MyApi',
+        },
+        smithyBuildOptions: {
+          projections: {
+            openapi: {
+              plugins: {
+                openapi: {
+                  jsonAdd: {
+                    // Add the x-paginated vendor extension to the GET /pets operation
+                    '/paths/~1pets/get/x-paginated': {
+                      inputToken: 'nextToken',
+                      outputToken: 'nextToken',
+                    },
+                  },
+                },
+              },
+            },
+          },
+        },
+      },
+    },
+  },
+  ...
+});
+```
+
 ### Quick Start: Python
 
 This guide assumes you want to write your CDK infrastructure in Python and your lambda handlers in Python, however note that you your infrastructure language and lambda handler language(s) are not tied to one another, you can mix and match as you like. Just specify the language in `runtime.languages` for any language you would like to write lambda handlers in.
 
 #### Create Your API Project
 
 Use the project in your `.projenrc.ts`. It can either be part of an [`nx-monorepo`](../nx-monorepo/README.md) (recommended) or used in a standalone fashion.
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.2/setup.py` & `aws_prototyping_sdk.type_safe_api-0.18.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.type_safe_api",
-    "version": "0.18.2",
+    "version": "0.18.3",
     "description": "@aws-prototyping-sdk/type-safe-api",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-prototyping-sdk",
     "long_description_content_type": "text/markdown",
     "author": "AWS APJ COPE<apj-cope@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_prototyping_sdk.type_safe_api",
         "aws_prototyping_sdk.type_safe_api._jsii"
     ],
     "package_data": {
         "aws_prototyping_sdk.type_safe_api._jsii": [
-            "type-safe-api@0.18.2.jsii.tgz"
+            "type-safe-api@0.18.3.jsii.tgz"
         ],
         "aws_prototyping_sdk.type_safe_api": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk/type_safe_api/__init__.py` & `aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk/type_safe_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,19 @@
   // CDK infrastructure in TypeScript
   infrastructure: {
     language: Language.TYPESCRIPT,
   },
   // Generate HTML documentation
   documentation: {
     formats: [DocumentationFormat.HTML_REDOC],
-  }
+  },
+  // Generate react-query hooks to interact with the UI from a React website
+  library: {
+    libraries: [Library.TYPESCRIPT_REACT_QUERY_HOOKS],
+  },
 });
 
 // Create a CDK infrastructure project. Can also consider PDKPipelineTsProject as an alternative!
 const infra = new AwsCdkTypeScriptApp({ ... });
 
 // Infrastructure can depend on the generated API infrastructure and runtime
 infra.addDeps(api.infrastructure.typescript!.package.packageName);
@@ -247,14 +251,16 @@
     |_ python
     |_ java
 |_ documentation/ - generated documentation in the formats you specified
     |_ html2
     |_ html_redoc
     |_ plantuml
     |_ markdown
+|_ library/ - generated libraries if specified
+    |_ typescript-react-query-hooks
 ```
 
 ### Smithy IDL
 
 Please refer to the [Smithy documentation](https://smithy.io/2.0/quickstart.html) for how to write models in Smithy. A basic example is provided below:
 
 ```smithy
@@ -1031,14 +1037,154 @@
         return SayHello200Response.of(HelloResponse.builder()
                 .message(String.format("Hello %s!", sayHelloRequestInput.getInput().getRequestParameters().getName()))
                 .build());
     }
 }
 ```
 
+### Libraries
+
+Libraries are generated code projects which are not fully-fledged runtime languages.
+
+#### TypeScript React Query Hooks
+
+This library contains generated [react-query](https://tanstack.com/query/latest) hooks for interacting with your API from a React website. You can generate these by adding the following options to your `TypeSafeApiProject` in your `.projenrc`:
+
+```python
+new TypeSafeApiProject({
+  library: {
+    libraries: [Library.TYPESCRIPT_REACT_QUERY_HOOKS],
+  },
+  ...
+});
+```
+
+##### Usage in a React Website
+
+First, make sure you create an instance of the API client (making sure to set the base URL and fetch instance). For example:
+
+```python
+export const useMyApiClient = () => useMemo(() => new MyApi(new Configuration({
+  basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
+  fetchApi: window.fetch.bind(window),
+})), []);
+```
+
+Note that if you are using the [Cloudscape React Website](../cloudscape-react-ts-website/README.md) with [AWS NorthStar](https://aws.github.io/aws-northstar/) and IAM (Sigv4) Auth for your API, you can use NorthStar's [`useSigv4Client()` hook](https://aws.github.io/aws-northstar/?path=/story/components-cognitoauth-sigv4client-docs--page) to create
+an instance of `fetch` which will sign requests with the logged in user's credentials. For example:
+
+```python
+export const useMyApiClient = () => {
+  const { client } = useSigv4Client();
+  return useMemo(() => client.current ? new MyApi(new Configuration({
+    basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
+    fetchApi: client.current,
+  })) : undefined, [client.current]);
+};
+```
+
+Next, instantiate the client provider above where you would like to use the hooks in your component hierarchy (such as above your router). For example:
+
+```tsx
+const api = useMyApiClient();
+
+return api ? (
+  <MyApiClientContext.Provider value={api}>
+    { /* Components within the provider may make use of the hooks */ }
+  </MyApiClientContext.Provider>
+) : <p>Loading...</p>;
+```
+
+Finally, you can import and use your generated hooks. For example:
+
+```tsx
+export const MyComponent: FC<MyComponentProps> = () => {
+  const sayHello = useSayHello({ name: 'World' });
+
+  return (
+    sayHello.isLoading ? (
+      <p>Loading...</p>
+    ) : (
+      sayHello.isError ? (
+        <p>Error!</p>
+      ) : (
+        <h1>{sayHello.data.message}</h1>
+      )
+    )
+  );
+};
+```
+
+##### Paginated Operations
+
+You can generate `useInfiniteQuery` hooks instead of `useQuery` hooks for paginated API operations, by making use of the vendor extension `x-paginated` in your operation in the OpenAPI specification. You must specify both the `inputToken` and `outputToken`, which indicate the properties from the input and output used for pagination. For example in OpenAPI:
+
+```yaml
+paths:
+  /pets:
+    get:
+      x-paginated:
+        # Input property with the token to request the next page
+        inputToken: nextToken
+        # Output property with the token to request the next page
+        outputToken: nextToken
+      parameters:
+        - in: query
+          name: nextToken
+          schema:
+            type: string
+          required: true
+      responses:
+        200:
+          description: Successful response
+          content:
+            application/json:
+              schema:
+                type: object
+                properties:
+                  nextToken:
+                    type: string
+```
+
+In Smithy, until [custom vendor extensions can be rendered via traits](https://github.com/awslabs/smithy/pull/1609), you can add the `x-paginated` vendor extension via `smithyBuildOptions` in your `TypeSafeApiProject`, for example:
+
+```python
+new TypeSafeApiProject({
+  model: {
+    language: ModelLanguage.SMITHY,
+    options: {
+      smithy: {
+        serviceName: {
+          namespace: 'com.mycompany',
+          serviceName: 'MyApi',
+        },
+        smithyBuildOptions: {
+          projections: {
+            openapi: {
+              plugins: {
+                openapi: {
+                  jsonAdd: {
+                    // Add the x-paginated vendor extension to the GET /pets operation
+                    '/paths/~1pets/get/x-paginated': {
+                      inputToken: 'nextToken',
+                      outputToken: 'nextToken',
+                    },
+                  },
+                },
+              },
+            },
+          },
+        },
+      },
+    },
+  },
+  ...
+});
+```
+
 ### Quick Start: Python
 
 This guide assumes you want to write your CDK infrastructure in Python and your lambda handlers in Python, however note that you your infrastructure language and lambda handler language(s) are not tied to one another, you can mix and match as you like. Just specify the language in `runtime.languages` for any language you would like to write lambda handlers in.
 
 #### Create Your API Project
 
 Use the project in your `.projenrc.ts`. It can either be part of an [`nx-monorepo`](../nx-monorepo/README.md) (recommended) or used in a standalone fashion.
@@ -2868,14 +3014,112 @@
 
     def __repr__(self) -> str:
         return "GeneratedCodeProjects(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+@jsii.data_type(
+    jsii_type="@aws-prototyping-sdk/type-safe-api.GeneratedLibraryOptions",
+    jsii_struct_bases=[],
+    name_mapping={"typescript_react_query_hooks": "typescriptReactQueryHooks"},
+)
+class GeneratedLibraryOptions:
+    def __init__(
+        self,
+        *,
+        typescript_react_query_hooks: typing.Optional[typing.Union[_projen_typescript_04054675.TypeScriptProjectOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> None:
+        '''(experimental) Options for generated libraries.
+
+        :param typescript_react_query_hooks: (experimental) Options for the generated typescript react-query hooks library. These override the default inferred options.
+
+        :stability: experimental
+        '''
+        if isinstance(typescript_react_query_hooks, dict):
+            typescript_react_query_hooks = _projen_typescript_04054675.TypeScriptProjectOptions(**typescript_react_query_hooks)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__aaba6490bdd657ac25f54e9f2eaacb24cb65c191d4ec347ee3547a98abae3956)
+            check_type(argname="argument typescript_react_query_hooks", value=typescript_react_query_hooks, expected_type=type_hints["typescript_react_query_hooks"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if typescript_react_query_hooks is not None:
+            self._values["typescript_react_query_hooks"] = typescript_react_query_hooks
+
+    @builtins.property
+    def typescript_react_query_hooks(
+        self,
+    ) -> typing.Optional[_projen_typescript_04054675.TypeScriptProjectOptions]:
+        '''(experimental) Options for the generated typescript react-query hooks library.
+
+        These override the default inferred options.
+
+        :stability: experimental
+        '''
+        result = self._values.get("typescript_react_query_hooks")
+        return typing.cast(typing.Optional[_projen_typescript_04054675.TypeScriptProjectOptions], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "GeneratedLibraryOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@aws-prototyping-sdk/type-safe-api.GeneratedLibraryProjects",
+    jsii_struct_bases=[],
+    name_mapping={"typescript_react_query_hooks": "typescriptReactQueryHooks"},
+)
+class GeneratedLibraryProjects:
+    def __init__(
+        self,
+        *,
+        typescript_react_query_hooks: typing.Optional[_projen_typescript_04054675.TypeScriptProject] = None,
+    ) -> None:
+        '''(experimental) Generated library projects.
+
+        :param typescript_react_query_hooks: (experimental) Generated typescript react-query hooks project.
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__31ee7e756a53a88db35aef6ee5d346bfd3c90aab725573d11722d24b6973ea0e)
+            check_type(argname="argument typescript_react_query_hooks", value=typescript_react_query_hooks, expected_type=type_hints["typescript_react_query_hooks"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if typescript_react_query_hooks is not None:
+            self._values["typescript_react_query_hooks"] = typescript_react_query_hooks
+
+    @builtins.property
+    def typescript_react_query_hooks(
+        self,
+    ) -> typing.Optional[_projen_typescript_04054675.TypeScriptProject]:
+        '''(experimental) Generated typescript react-query hooks project.
+
+        :stability: experimental
+        '''
+        result = self._values.get("typescript_react_query_hooks")
+        return typing.cast(typing.Optional[_projen_typescript_04054675.TypeScriptProject], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "GeneratedLibraryProjects(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class IamAuthorizer(
     Authorizer,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-prototyping-sdk/type-safe-api.IamAuthorizer",
 ):
     '''(experimental) An IAM authorizer.
 
@@ -3150,15 +3394,15 @@
         )
 
         return typing.cast(ApiGatewayIntegration, jsii.invoke(self, "render", [props]))
 
 
 @jsii.enum(jsii_type="@aws-prototyping-sdk/type-safe-api.Language")
 class Language(enum.Enum):
-    '''(experimental) Supported languages for code generation.
+    '''(experimental) Supported languages for runtimes and infrastructure.
 
     :stability: experimental
     '''
 
     TYPESCRIPT = "TYPESCRIPT"
     '''
     :stability: experimental
@@ -3169,14 +3413,91 @@
     '''
     JAVA = "JAVA"
     '''
     :stability: experimental
     '''
 
 
+@jsii.enum(jsii_type="@aws-prototyping-sdk/type-safe-api.Library")
+class Library(enum.Enum):
+    '''(experimental) Supported libraries for code generation.
+
+    :stability: experimental
+    '''
+
+    TYPESCRIPT_REACT_QUERY_HOOKS = "TYPESCRIPT_REACT_QUERY_HOOKS"
+    '''
+    :stability: experimental
+    '''
+
+
+@jsii.data_type(
+    jsii_type="@aws-prototyping-sdk/type-safe-api.LibraryConfiguration",
+    jsii_struct_bases=[],
+    name_mapping={"libraries": "libraries", "options": "options"},
+)
+class LibraryConfiguration:
+    def __init__(
+        self,
+        *,
+        libraries: typing.Sequence[Library],
+        options: typing.Optional[typing.Union[GeneratedLibraryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> None:
+        '''(experimental) Configuration for generated libraries.
+
+        :param libraries: (experimental) The library to generate.
+        :param options: (experimental) Options for the generated library package. Note that only options for the specified libraries will apply
+
+        :stability: experimental
+        '''
+        if isinstance(options, dict):
+            options = GeneratedLibraryOptions(**options)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__cf885e298875e06aa5677eb9355657441701a5f252c8eca8317f989a12fb7d82)
+            check_type(argname="argument libraries", value=libraries, expected_type=type_hints["libraries"])
+            check_type(argname="argument options", value=options, expected_type=type_hints["options"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "libraries": libraries,
+        }
+        if options is not None:
+            self._values["options"] = options
+
+    @builtins.property
+    def libraries(self) -> typing.List[Library]:
+        '''(experimental) The library to generate.
+
+        :stability: experimental
+        '''
+        result = self._values.get("libraries")
+        assert result is not None, "Required property 'libraries' is missing"
+        return typing.cast(typing.List[Library], result)
+
+    @builtins.property
+    def options(self) -> typing.Optional[GeneratedLibraryOptions]:
+        '''(experimental) Options for the generated library package.
+
+        Note that only options for the specified libraries will apply
+
+        :stability: experimental
+        '''
+        result = self._values.get("options")
+        return typing.cast(typing.Optional[GeneratedLibraryOptions], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "LibraryConfiguration(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 @jsii.data_type(
     jsii_type="@aws-prototyping-sdk/type-safe-api.ManagedRule",
     jsii_struct_bases=[],
     name_mapping={"name": "name", "vendor": "vendor"},
 )
 class ManagedRule:
     def __init__(self, *, name: builtins.str, vendor: builtins.str) -> None:
@@ -4810,14 +5131,15 @@
     def __init__(
         self,
         *,
         infrastructure: typing.Union[InfrastructureConfiguration, typing.Dict[builtins.str, typing.Any]],
         model: typing.Union[ModelConfiguration, typing.Dict[builtins.str, typing.Any]],
         runtime: typing.Union[RuntimeConfiguration, typing.Dict[builtins.str, typing.Any]],
         documentation: typing.Optional[typing.Union[DocumentationConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
+        library: typing.Optional[typing.Union[LibraryConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
         name: builtins.str,
         commit_generated: typing.Optional[builtins.bool] = None,
         git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         logging: typing.Optional[typing.Union[_projen_04054675.LoggerOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         outdir: typing.Optional[builtins.str] = None,
         parent: typing.Optional[_projen_04054675.Project] = None,
@@ -4828,14 +5150,15 @@
         renovatebot_options: typing.Optional[typing.Union[_projen_04054675.RenovatebotOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param infrastructure: (experimental) Configuration for generated infrastructure.
         :param model: (experimental) Configuration for the API model.
         :param runtime: (experimental) Configuration for generated runtime projects (containing types, clients and server code).
         :param documentation: (experimental) Configuration for generated documentation.
+        :param library: (experimental) Configuration for generated libraries. Libraries are projects which are generated from your model, but are not fully-fledged runtimes, for example react hooks or clients in languages that aren't supported as runtimes.
         :param name: (experimental) This is the name of your project. Default: $BASEDIR
         :param commit_generated: (experimental) Whether to commit the managed files by default. Default: true
         :param git_ignore_options: (experimental) Configuration options for .gitignore file.
         :param git_options: (experimental) Configuration options for git.
         :param logging: (experimental) Configure logging options such as verbosity. Default: {}
         :param outdir: (experimental) The root directory of the project. Relative to this directory, all files are synthesized. If this project has a parent, this directory is relative to the parent directory and it cannot be the same as the parent or any of it's other sub-projects. Default: "."
         :param parent: (experimental) The parent project, if this project is part of a bigger project.
@@ -4848,14 +5171,15 @@
         :stability: experimental
         '''
         options = TypeSafeApiProjectOptions(
             infrastructure=infrastructure,
             model=model,
             runtime=runtime,
             documentation=documentation,
+            library=library,
             name=name,
             commit_generated=commit_generated,
             git_ignore_options=git_ignore_options,
             git_options=git_options,
             logging=logging,
             outdir=outdir,
             parent=parent,
@@ -4876,14 +5200,25 @@
         Only the property corresponding to ``infrastructure.language`` will be defined.
 
         :stability: experimental
         '''
         return typing.cast(GeneratedCodeProjects, jsii.get(self, "infrastructure"))
 
     @builtins.property
+    @jsii.member(jsii_name="library")
+    def library(self) -> GeneratedLibraryProjects:
+        '''(experimental) Generated library projects.
+
+        Only the properties corresponding to specified ``library.libraries`` will be defined.
+
+        :stability: experimental
+        '''
+        return typing.cast(GeneratedLibraryProjects, jsii.get(self, "library"))
+
+    @builtins.property
     @jsii.member(jsii_name="model")
     def model(self) -> TypeSafeApiModelProject:
         '''(experimental) Project for the api model.
 
         :stability: experimental
         '''
         return typing.cast(TypeSafeApiModelProject, jsii.get(self, "model"))
@@ -4917,14 +5252,15 @@
         "projenrc_json_options": "projenrcJsonOptions",
         "renovatebot": "renovatebot",
         "renovatebot_options": "renovatebotOptions",
         "infrastructure": "infrastructure",
         "model": "model",
         "runtime": "runtime",
         "documentation": "documentation",
+        "library": "library",
     },
 )
 class TypeSafeApiProjectOptions(_projen_04054675.ProjectOptions):
     def __init__(
         self,
         *,
         name: builtins.str,
@@ -4939,14 +5275,15 @@
         projenrc_json_options: typing.Optional[typing.Union[_projen_04054675.ProjenrcJsonOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         renovatebot: typing.Optional[builtins.bool] = None,
         renovatebot_options: typing.Optional[typing.Union[_projen_04054675.RenovatebotOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         infrastructure: typing.Union[InfrastructureConfiguration, typing.Dict[builtins.str, typing.Any]],
         model: typing.Union[ModelConfiguration, typing.Dict[builtins.str, typing.Any]],
         runtime: typing.Union[RuntimeConfiguration, typing.Dict[builtins.str, typing.Any]],
         documentation: typing.Optional[typing.Union[DocumentationConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
+        library: typing.Optional[typing.Union[LibraryConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''(experimental) Options for the TypeSafeApiProject.
 
         :param name: (experimental) This is the name of your project. Default: $BASEDIR
         :param commit_generated: (experimental) Whether to commit the managed files by default. Default: true
         :param git_ignore_options: (experimental) Configuration options for .gitignore file.
         :param git_options: (experimental) Configuration options for git.
@@ -4958,14 +5295,15 @@
         :param projenrc_json_options: (experimental) Options for .projenrc.json. Default: - default options
         :param renovatebot: (experimental) Use renovatebot to handle dependency upgrades. Default: false
         :param renovatebot_options: (experimental) Options for renovatebot. Default: - default options
         :param infrastructure: (experimental) Configuration for generated infrastructure.
         :param model: (experimental) Configuration for the API model.
         :param runtime: (experimental) Configuration for generated runtime projects (containing types, clients and server code).
         :param documentation: (experimental) Configuration for generated documentation.
+        :param library: (experimental) Configuration for generated libraries. Libraries are projects which are generated from your model, but are not fully-fledged runtimes, for example react hooks or clients in languages that aren't supported as runtimes.
 
         :stability: experimental
         '''
         if isinstance(git_ignore_options, dict):
             git_ignore_options = _projen_04054675.IgnoreFileOptions(**git_ignore_options)
         if isinstance(git_options, dict):
             git_options = _projen_04054675.GitOptions(**git_options)
@@ -4979,14 +5317,16 @@
             infrastructure = InfrastructureConfiguration(**infrastructure)
         if isinstance(model, dict):
             model = ModelConfiguration(**model)
         if isinstance(runtime, dict):
             runtime = RuntimeConfiguration(**runtime)
         if isinstance(documentation, dict):
             documentation = DocumentationConfiguration(**documentation)
+        if isinstance(library, dict):
+            library = LibraryConfiguration(**library)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__abde6fa90ff9fea9e430aaca82f0c910c5ecc24d1205ba19958f47080d5b15fb)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument commit_generated", value=commit_generated, expected_type=type_hints["commit_generated"])
             check_type(argname="argument git_ignore_options", value=git_ignore_options, expected_type=type_hints["git_ignore_options"])
             check_type(argname="argument git_options", value=git_options, expected_type=type_hints["git_options"])
             check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
@@ -4997,14 +5337,15 @@
             check_type(argname="argument projenrc_json_options", value=projenrc_json_options, expected_type=type_hints["projenrc_json_options"])
             check_type(argname="argument renovatebot", value=renovatebot, expected_type=type_hints["renovatebot"])
             check_type(argname="argument renovatebot_options", value=renovatebot_options, expected_type=type_hints["renovatebot_options"])
             check_type(argname="argument infrastructure", value=infrastructure, expected_type=type_hints["infrastructure"])
             check_type(argname="argument model", value=model, expected_type=type_hints["model"])
             check_type(argname="argument runtime", value=runtime, expected_type=type_hints["runtime"])
             check_type(argname="argument documentation", value=documentation, expected_type=type_hints["documentation"])
+            check_type(argname="argument library", value=library, expected_type=type_hints["library"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "name": name,
             "infrastructure": infrastructure,
             "model": model,
             "runtime": runtime,
         }
         if commit_generated is not None:
@@ -5027,14 +5368,16 @@
             self._values["projenrc_json_options"] = projenrc_json_options
         if renovatebot is not None:
             self._values["renovatebot"] = renovatebot
         if renovatebot_options is not None:
             self._values["renovatebot_options"] = renovatebot_options
         if documentation is not None:
             self._values["documentation"] = documentation
+        if library is not None:
+            self._values["library"] = library
 
     @builtins.property
     def name(self) -> builtins.str:
         '''(experimental) This is the name of your project.
 
         :default: $BASEDIR
 
@@ -5207,14 +5550,26 @@
         '''(experimental) Configuration for generated documentation.
 
         :stability: experimental
         '''
         result = self._values.get("documentation")
         return typing.cast(typing.Optional[DocumentationConfiguration], result)
 
+    @builtins.property
+    def library(self) -> typing.Optional[LibraryConfiguration]:
+        '''(experimental) Configuration for generated libraries.
+
+        Libraries are projects which are generated from your model, but are not
+        fully-fledged runtimes, for example react hooks or clients in languages that aren't supported as runtimes.
+
+        :stability: experimental
+        '''
+        result = self._values.get("library")
+        return typing.cast(typing.Optional[LibraryConfiguration], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -6145,22 +6500,26 @@
     "CustomAuthorizer",
     "CustomAuthorizerProps",
     "CustomAuthorizerType",
     "DocumentationConfiguration",
     "DocumentationFormat",
     "GeneratedCodeOptions",
     "GeneratedCodeProjects",
+    "GeneratedLibraryOptions",
+    "GeneratedLibraryProjects",
     "IamAuthorizer",
     "InfrastructureConfiguration",
     "Integration",
     "IntegrationGrantProps",
     "IntegrationRenderProps",
     "Integrations",
     "LambdaIntegration",
     "Language",
+    "Library",
+    "LibraryConfiguration",
     "ManagedRule",
     "MethodAndPath",
     "ModelConfiguration",
     "ModelLanguage",
     "ModelOptions",
     "NoneAuthorizer",
     "OpenApiDefinition",
@@ -6292,14 +6651,28 @@
     java: typing.Optional[_projen_java_04054675.JavaProject] = None,
     python: typing.Optional[_projen_python_04054675.PythonProject] = None,
     typescript: typing.Optional[_projen_typescript_04054675.TypeScriptProject] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__aaba6490bdd657ac25f54e9f2eaacb24cb65c191d4ec347ee3547a98abae3956(
+    *,
+    typescript_react_query_hooks: typing.Optional[typing.Union[_projen_typescript_04054675.TypeScriptProjectOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__31ee7e756a53a88db35aef6ee5d346bfd3c90aab725573d11722d24b6973ea0e(
+    *,
+    typescript_react_query_hooks: typing.Optional[_projen_typescript_04054675.TypeScriptProject] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__42832742ccb56b4504cad0e669390b735f9f726fc938f2b7eb2d7878b53e3faf(
     *,
     language: Language,
     options: typing.Optional[typing.Union[GeneratedCodeOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
@@ -6312,14 +6685,22 @@
 
 def _typecheckingstub__d4f33cbf9ca3cf26ca56b9477805b0ee2228ee2f97e63a0addace46ae5267b4d(
     lambda_function: _aws_cdk_aws_lambda_ceddda9d.IFunction,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__cf885e298875e06aa5677eb9355657441701a5f252c8eca8317f989a12fb7d82(
+    *,
+    libraries: typing.Sequence[Library],
+    options: typing.Optional[typing.Union[GeneratedLibraryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__b5526168b6baf723196f879ba4ca6bcce6f57e83cf0e96d3c912a0ab422a07e3(
     *,
     name: builtins.str,
     vendor: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
@@ -6516,14 +6897,15 @@
     projenrc_json_options: typing.Optional[typing.Union[_projen_04054675.ProjenrcJsonOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     renovatebot: typing.Optional[builtins.bool] = None,
     renovatebot_options: typing.Optional[typing.Union[_projen_04054675.RenovatebotOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     infrastructure: typing.Union[InfrastructureConfiguration, typing.Dict[builtins.str, typing.Any]],
     model: typing.Union[ModelConfiguration, typing.Dict[builtins.str, typing.Any]],
     runtime: typing.Union[RuntimeConfiguration, typing.Dict[builtins.str, typing.Any]],
     documentation: typing.Optional[typing.Union[DocumentationConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
+    library: typing.Optional[typing.Union[LibraryConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__767125a1376366edf6341c113fbc39f6e469b47eea26e1fa3720cfc786f2d558(
     *,
     cidr_allow_list: typing.Optional[typing.Union[CidrAllowList, typing.Dict[builtins.str, typing.Any]]] = None,
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO` & `aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk.type_safe_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-prototyping-sdk.type-safe-api
-Version: 0.18.2
+Version: 0.18.3
 Summary: @aws-prototyping-sdk/type-safe-api
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -72,15 +72,19 @@
   // CDK infrastructure in TypeScript
   infrastructure: {
     language: Language.TYPESCRIPT,
   },
   // Generate HTML documentation
   documentation: {
     formats: [DocumentationFormat.HTML_REDOC],
-  }
+  },
+  // Generate react-query hooks to interact with the UI from a React website
+  library: {
+    libraries: [Library.TYPESCRIPT_REACT_QUERY_HOOKS],
+  },
 });
 
 // Create a CDK infrastructure project. Can also consider PDKPipelineTsProject as an alternative!
 const infra = new AwsCdkTypeScriptApp({ ... });
 
 // Infrastructure can depend on the generated API infrastructure and runtime
 infra.addDeps(api.infrastructure.typescript!.package.packageName);
@@ -270,14 +274,16 @@
     |_ python
     |_ java
 |_ documentation/ - generated documentation in the formats you specified
     |_ html2
     |_ html_redoc
     |_ plantuml
     |_ markdown
+|_ library/ - generated libraries if specified
+    |_ typescript-react-query-hooks
 ```
 
 ### Smithy IDL
 
 Please refer to the [Smithy documentation](https://smithy.io/2.0/quickstart.html) for how to write models in Smithy. A basic example is provided below:
 
 ```smithy
@@ -1054,14 +1060,154 @@
         return SayHello200Response.of(HelloResponse.builder()
                 .message(String.format("Hello %s!", sayHelloRequestInput.getInput().getRequestParameters().getName()))
                 .build());
     }
 }
 ```
 
+### Libraries
+
+Libraries are generated code projects which are not fully-fledged runtime languages.
+
+#### TypeScript React Query Hooks
+
+This library contains generated [react-query](https://tanstack.com/query/latest) hooks for interacting with your API from a React website. You can generate these by adding the following options to your `TypeSafeApiProject` in your `.projenrc`:
+
+```python
+new TypeSafeApiProject({
+  library: {
+    libraries: [Library.TYPESCRIPT_REACT_QUERY_HOOKS],
+  },
+  ...
+});
+```
+
+##### Usage in a React Website
+
+First, make sure you create an instance of the API client (making sure to set the base URL and fetch instance). For example:
+
+```python
+export const useMyApiClient = () => useMemo(() => new MyApi(new Configuration({
+  basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
+  fetchApi: window.fetch.bind(window),
+})), []);
+```
+
+Note that if you are using the [Cloudscape React Website](../cloudscape-react-ts-website/README.md) with [AWS NorthStar](https://aws.github.io/aws-northstar/) and IAM (Sigv4) Auth for your API, you can use NorthStar's [`useSigv4Client()` hook](https://aws.github.io/aws-northstar/?path=/story/components-cognitoauth-sigv4client-docs--page) to create
+an instance of `fetch` which will sign requests with the logged in user's credentials. For example:
+
+```python
+export const useMyApiClient = () => {
+  const { client } = useSigv4Client();
+  return useMemo(() => client.current ? new MyApi(new Configuration({
+    basePath: 'https://example123.execute-api.ap-southeast-2.amazonaws.com/prod',
+    fetchApi: client.current,
+  })) : undefined, [client.current]);
+};
+```
+
+Next, instantiate the client provider above where you would like to use the hooks in your component hierarchy (such as above your router). For example:
+
+```tsx
+const api = useMyApiClient();
+
+return api ? (
+  <MyApiClientContext.Provider value={api}>
+    { /* Components within the provider may make use of the hooks */ }
+  </MyApiClientContext.Provider>
+) : <p>Loading...</p>;
+```
+
+Finally, you can import and use your generated hooks. For example:
+
+```tsx
+export const MyComponent: FC<MyComponentProps> = () => {
+  const sayHello = useSayHello({ name: 'World' });
+
+  return (
+    sayHello.isLoading ? (
+      <p>Loading...</p>
+    ) : (
+      sayHello.isError ? (
+        <p>Error!</p>
+      ) : (
+        <h1>{sayHello.data.message}</h1>
+      )
+    )
+  );
+};
+```
+
+##### Paginated Operations
+
+You can generate `useInfiniteQuery` hooks instead of `useQuery` hooks for paginated API operations, by making use of the vendor extension `x-paginated` in your operation in the OpenAPI specification. You must specify both the `inputToken` and `outputToken`, which indicate the properties from the input and output used for pagination. For example in OpenAPI:
+
+```yaml
+paths:
+  /pets:
+    get:
+      x-paginated:
+        # Input property with the token to request the next page
+        inputToken: nextToken
+        # Output property with the token to request the next page
+        outputToken: nextToken
+      parameters:
+        - in: query
+          name: nextToken
+          schema:
+            type: string
+          required: true
+      responses:
+        200:
+          description: Successful response
+          content:
+            application/json:
+              schema:
+                type: object
+                properties:
+                  nextToken:
+                    type: string
+```
+
+In Smithy, until [custom vendor extensions can be rendered via traits](https://github.com/awslabs/smithy/pull/1609), you can add the `x-paginated` vendor extension via `smithyBuildOptions` in your `TypeSafeApiProject`, for example:
+
+```python
+new TypeSafeApiProject({
+  model: {
+    language: ModelLanguage.SMITHY,
+    options: {
+      smithy: {
+        serviceName: {
+          namespace: 'com.mycompany',
+          serviceName: 'MyApi',
+        },
+        smithyBuildOptions: {
+          projections: {
+            openapi: {
+              plugins: {
+                openapi: {
+                  jsonAdd: {
+                    // Add the x-paginated vendor extension to the GET /pets operation
+                    '/paths/~1pets/get/x-paginated': {
+                      inputToken: 'nextToken',
+                      outputToken: 'nextToken',
+                    },
+                  },
+                },
+              },
+            },
+          },
+        },
+      },
+    },
+  },
+  ...
+});
+```
+
 ### Quick Start: Python
 
 This guide assumes you want to write your CDK infrastructure in Python and your lambda handlers in Python, however note that you your infrastructure language and lambda handler language(s) are not tied to one another, you can mix and match as you like. Just specify the language in `runtime.languages` for any language you would like to write lambda handlers in.
 
 #### Create Your API Project
 
 Use the project in your `.projenrc.ts`. It can either be part of an [`nx-monorepo`](../nx-monorepo/README.md) (recommended) or used in a standalone fashion.
```

### Comparing `aws_prototyping_sdk.type_safe_api-0.18.2/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt` & `aws_prototyping_sdk.type_safe_api-0.18.3/src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_prototyping_sdk.type_safe_api.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/requires.txt
 src/aws_prototyping_sdk.type_safe_api.egg-info/top_level.txt
 src/aws_prototyping_sdk/type_safe_api/__init__.py
 src/aws_prototyping_sdk/type_safe_api/py.typed
 src/aws_prototyping_sdk/type_safe_api/_jsii/__init__.py
-src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.2.jsii.tgz
+src/aws_prototyping_sdk/type_safe_api/_jsii/type-safe-api@0.18.3.jsii.tgz
```

