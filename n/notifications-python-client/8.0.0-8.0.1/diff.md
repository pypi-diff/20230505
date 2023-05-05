# Comparing `tmp/notifications_python_client-8.0.0-py3-none-any.whl.zip` & `tmp/notifications_python_client-8.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9423 bytes, number of entries: 12
--rw-r--r--  2.0 unx      646 b- defN 23-Feb-27 14:33 notifications_python_client/__init__.py
--rw-r--r--  2.0 unx     4682 b- defN 23-Feb-27 14:33 notifications_python_client/authentication.py
--rw-r--r--  2.0 unx     4017 b- defN 23-Feb-27 14:33 notifications_python_client/base.py
--rw-r--r--  2.0 unx     2438 b- defN 23-Feb-27 14:33 notifications_python_client/errors.py
--rw-r--r--  2.0 unx     5889 b- defN 23-Feb-27 14:33 notifications_python_client/notifications.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-27 14:33 notifications_python_client/py.typed
--rw-r--r--  2.0 unx      536 b- defN 23-Feb-27 14:33 notifications_python_client/utils.py
--rw-r--r--  2.0 unx     1094 b- defN 23-Feb-27 14:48 notifications_python_client-8.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1039 b- defN 23-Feb-27 14:48 notifications_python_client-8.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-27 14:48 notifications_python_client-8.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       28 b- defN 23-Feb-27 14:48 notifications_python_client-8.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1152 b- defN 23-Feb-27 14:48 notifications_python_client-8.0.0.dist-info/RECORD
-12 files, 21613 bytes uncompressed, 7427 bytes compressed:  65.6%
+Zip file size: 9326 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      637 b- defN 23-May-05 12:59 notifications_python_client/__init__.py
+-rw-r--r--  2.0 unx     4662 b- defN 23-May-05 12:59 notifications_python_client/authentication.py
+-rw-r--r--  2.0 unx     3683 b- defN 23-May-05 12:59 notifications_python_client/base.py
+-rw-r--r--  2.0 unx     2438 b- defN 23-May-05 12:59 notifications_python_client/errors.py
+-rw-r--r--  2.0 unx     5435 b- defN 23-May-05 12:59 notifications_python_client/notifications.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 12:59 notifications_python_client/py.typed
+-rw-r--r--  2.0 unx      537 b- defN 23-May-05 12:59 notifications_python_client/utils.py
+-rw-r--r--  2.0 unx     1094 b- defN 23-May-05 13:16 notifications_python_client-8.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1039 b- defN 23-May-05 13:16 notifications_python_client-8.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 13:16 notifications_python_client-8.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 23-May-05 13:16 notifications_python_client-8.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1152 b- defN 23-May-05 13:16 notifications_python_client-8.0.1.dist-info/RECORD
+12 files, 20797 bytes uncompressed, 7330 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: notifications_python_client/py.typed
 Comment: 
 
 Filename: notifications_python_client/utils.py
 Comment: 
 
-Filename: notifications_python_client-8.0.0.dist-info/LICENSE
+Filename: notifications_python_client-8.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: notifications_python_client-8.0.0.dist-info/METADATA
+Filename: notifications_python_client-8.0.1.dist-info/METADATA
 Comment: 
 
-Filename: notifications_python_client-8.0.0.dist-info/WHEEL
+Filename: notifications_python_client-8.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: notifications_python_client-8.0.0.dist-info/top_level.txt
+Filename: notifications_python_client-8.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: notifications_python_client-8.0.0.dist-info/RECORD
+Filename: notifications_python_client-8.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## notifications_python_client/__init__.py

```diff
@@ -3,17 +3,15 @@
 # Given a version number MAJOR.MINOR.PATCH, increment the:
 # - MAJOR version when you make incompatible API changes,
 # - MINOR version when you add functionality in a backwards-compatible manner, and
 # - PATCH version when you make backwards-compatible bug fixes.
 #
 # -- http://semver.org/
 
-__version__ = '8.0.0'
+__version__ = "8.0.1"
 
 from notifications_python_client.errors import (  # noqa
     REQUEST_ERROR_MESSAGE,
     REQUEST_ERROR_STATUS_CODE,
 )
-from notifications_python_client.notifications import (  # noqa
-    NotificationsAPIClient,
-)
+from notifications_python_client.notifications import NotificationsAPIClient  # noqa
 from notifications_python_client.utils import prepare_upload  # noqa
```

## notifications_python_client/authentication.py

```diff
@@ -36,23 +36,17 @@
     :param secret: Application signing secret
     :param client_id: Identifier for the client
     :return: JWT token for this request
     """
     assert secret, "Missing secret key"
     assert client_id, "Missing client id"
 
-    headers = {
-        "typ": __type__,
-        "alg": __algorithm__
-    }
-
-    claims = {
-        'iss': client_id,
-        'iat': epoch_seconds()
-    }
+    headers = {"typ": __type__, "alg": __algorithm__}
+
+    claims = {"iss": client_id, "iat": epoch_seconds()}
     t = jwt.encode(payload=claims, key=secret, headers=headers)
     if isinstance(t, str):
         return t
     else:
         return t.decode()
 
 
@@ -65,20 +59,20 @@
     :return issuer: iss field of the JWT token
     :raises TokenIssuerError: if iss field not present
     :raises TokenDecodeError: if token does not conform to JWT spec
     """
     try:
         unverified = decode_token(token)
 
-        if 'iss' not in unverified:
+        if "iss" not in unverified:
             raise TokenIssuerError
 
-        return unverified.get('iss')
-    except jwt.DecodeError:
-        raise TokenDecodeError
+        return unverified.get("iss")
+    except jwt.DecodeError as e:
+        raise TokenDecodeError from e
 
 
 def decode_jwt_token(token, secret):
     """
     Validates and decodes the JWT token
     Token checked for
         - signature of JWT token
@@ -93,49 +87,45 @@
     :raises TokenDecodeError: If the token cannot be decoded because it failed validation
     :raises TokenAlgorithmError: If the algorithm is not recognised
     :raises TokenError: If any other type of jwt exception is raised when trying jwt.decode
     """
     try:
         # check signature of the token
         decoded_token = jwt.decode(
-            token,
-            key=secret,
-            options={"verify_signature": True},
-            algorithms=[__algorithm__],
-            leeway=__bound__
+            token, key=secret, options={"verify_signature": True}, algorithms=[__algorithm__], leeway=__bound__
         )
         return validate_jwt_token(decoded_token)
-    except jwt.InvalidIssuedAtError:
-        raise TokenExpiredError("Token has invalid iat field", decode_token(token))
-    except jwt.ImmatureSignatureError:
-        raise TokenExpiredError(INVALID_FUTURE_TOKEN_ERROR_MESSAGE, decode_token(token))
-    except jwt.DecodeError:
-        raise TokenDecodeError
-    except jwt.InvalidAlgorithmError:
-        raise TokenAlgorithmError
-    except jwt.InvalidTokenError:
+    except jwt.InvalidIssuedAtError as e:
+        raise TokenExpiredError("Token has invalid iat field", decode_token(token)) from e
+    except jwt.ImmatureSignatureError as e:
+        raise TokenExpiredError(INVALID_FUTURE_TOKEN_ERROR_MESSAGE, decode_token(token)) from e
+    except jwt.DecodeError as e:
+        raise TokenDecodeError from e
+    except jwt.InvalidAlgorithmError as e:
+        raise TokenAlgorithmError from e
+    except jwt.InvalidTokenError as e:
         # At this point, we have not caught a specific exception we care about enough to show
         # a precise error message (ie something to do with the iat, iss or alg fields).
         # If there is a different reason our token is invalid we will throw a generic error as we
         # don't wish to provide exact messages for every type of error that jwt might encounter.
         # https://github.com/jpadilla/pyjwt/blob/master/jwt/exceptions.py
         # https://pyjwt.readthedocs.io/en/latest/api.html#exceptions
-        raise TokenError
+        raise TokenError from e
 
 
 def validate_jwt_token(decoded_token):
     # token has all the required fields
-    if 'iss' not in decoded_token:
+    if "iss" not in decoded_token:
         raise TokenIssuerError
-    if 'iat' not in decoded_token:
+    if "iat" not in decoded_token:
         raise TokenIssuedAtError
 
     # check iat time is within bounds
     now = epoch_seconds()
-    iat = int(decoded_token['iat'])
+    iat = int(decoded_token["iat"])
     if now > (iat + __bound__):
         raise TokenExpiredError("Token has expired", decoded_token)
     if iat > (now + __bound__):
         raise TokenExpiredError(INVALID_FUTURE_TOKEN_ERROR_MESSAGE, decoded_token)
 
     return True
```

## notifications_python_client/base.py

```diff
@@ -9,20 +9,15 @@
 from notifications_python_client.authentication import create_jwt_token
 from notifications_python_client.errors import HTTPError, InvalidResponse
 
 logger = logging.getLogger(__name__)
 
 
 class BaseAPIClient(object):
-    def __init__(
-            self,
-            api_key,
-            base_url='https://api.notifications.service.gov.uk',
-            timeout=30
-    ):
+    def __init__(self, api_key, base_url="https://api.notifications.service.gov.uk", timeout=30):
         """
         Initialise the client
         Error if either of base_url or secret missing
         :param base_url - base URL of GOV.UK Notify API:
         :param secret - application secret - used to sign the request:
         :param timeout - request timeout on the client
         :return:
@@ -50,35 +45,29 @@
     def delete(self, url, data=None):
         return self.request("DELETE", url, data=data)
 
     def generate_headers(self, api_token):
         return {
             "Content-type": "application/json",
             "Authorization": "Bearer {}".format(api_token),
-            "User-agent": "NOTIFY-API-PYTHON-CLIENT/{}".format(__version__)
+            "User-agent": "NOTIFY-API-PYTHON-CLIENT/{}".format(__version__),
         }
 
     def request(self, method, url, data=None, params=None):
-        logger.debug("API request {} {}".format(method, url))
+        logger.debug("API request %s %s", method, url)
         url, kwargs = self._create_request_objects(url, data, params)
 
         response = self._perform_request(method, url, kwargs)
 
         return self._process_json_response(response)
 
     def _create_request_objects(self, url, data, params):
-        api_token = create_jwt_token(
-            self.api_key,
-            self.service_id
-        )
-
-        kwargs = {
-            "headers": self.generate_headers(api_token),
-            "timeout": self.timeout
-        }
+        api_token = create_jwt_token(self.api_key, self.service_id)
+
+        kwargs = {"headers": self.generate_headers(api_token), "timeout": self.timeout}
 
         if data is not None:
             kwargs.update(data=self._serialize_data(data))
 
         if params is not None:
             kwargs.update(params=params)
 
@@ -94,39 +83,27 @@
             return list(obj)
 
         raise TypeError
 
     def _perform_request(self, method, url, kwargs):
         start_time = time.monotonic()
         try:
-            response = requests.request(
-                method,
-                url,
-                **kwargs
-            )
+            response = requests.request(method, url, **kwargs)
             response.raise_for_status()
             return response
         except requests.RequestException as e:
             api_error = HTTPError.create(e)
-            logger.error(
-                "API {} request on {} failed with {} '{}'".format(
-                    method,
-                    url,
-                    api_error.status_code,
-                    api_error.message
-                )
+            logger.warning(
+                "API %s request on %s failed with %s '%s'", method, url, api_error.status_code, api_error.message
             )
             raise api_error
         finally:
             elapsed_time = time.monotonic() - start_time
-            logger.debug("API {} request on {} finished in {}".format(method, url, elapsed_time))
+            logger.debug("API %s request on %s finished in %s", method, url, elapsed_time)
 
     def _process_json_response(self, response):
         try:
             if response.status_code == 204:
                 return
             return response.json()
-        except ValueError:
-            raise InvalidResponse(
-                response,
-                message="No JSON response object could be decoded"
-            )
+        except ValueError as e:
+            raise InvalidResponse(response, message="No JSON response object could be decoded") from e
```

## notifications_python_client/errors.py

```diff
@@ -6,80 +6,80 @@
 REQUEST_ERROR_MESSAGE = "Request failed"
 
 TOKEN_ERROR_GUIDANCE = "See our requirements for JSON Web Tokens at https://docs.notifications.service.gov.uk/rest-api.html#authorisation-header"  # noqa
 TOKEN_ERROR_DEFAULT_ERROR_MESSAGE = "Invalid token: " + TOKEN_ERROR_GUIDANCE
 
 
 class TokenError(Exception):
-
     def __init__(self, message=None, token=None):
         self.message = message + ". " + TOKEN_ERROR_GUIDANCE if message else TOKEN_ERROR_DEFAULT_ERROR_MESSAGE
         self.token = token
 
 
 class TokenExpiredError(TokenError):
     pass
 
 
 class TokenAlgorithmError(TokenError):
     def __init__(self):
-        super().__init__('Invalid token: algorithm used is not HS256')
+        super().__init__("Invalid token: algorithm used is not HS256")
 
 
 class TokenDecodeError(TokenError):
     def __init__(self, message=None):
-        super().__init__(message or 'Invalid token: signature')
+        super().__init__(message or "Invalid token: signature")
 
 
 class TokenIssuerError(TokenDecodeError):
     def __init__(self):
-        super().__init__('Invalid token: iss field not provided')
+        super().__init__("Invalid token: iss field not provided")
 
 
 class TokenIssuedAtError(TokenDecodeError):
     def __init__(self):
-        super().__init__('Invalid token: iat field not provided')
+        super().__init__("Invalid token: iat field not provided")
 
 
 class APIError(Exception):
     def __init__(self, response: Response = None, message: str = None):
         self.response = response
         self._message = message
 
     def __str__(self):
         return "{} - {}".format(self.status_code, self.message)
 
     @property
     def message(self) -> Union[str, List[dict]]:
         try:
             json_resp = self.response.json()  # type: ignore
-            return json_resp.get('message', json_resp.get('errors'))
+            return json_resp.get("message", json_resp.get("errors"))
         except (TypeError, ValueError, AttributeError, KeyError):
             return self._message or REQUEST_ERROR_MESSAGE
 
     @property
     def status_code(self) -> int:
         try:
             return self.response.status_code  # type: ignore
         except AttributeError:
             return REQUEST_ERROR_STATUS_CODE
 
 
 class HTTPError(APIError):
     @staticmethod
-    def create(e: RequestException) -> 'HTTPError':
+    def create(e: RequestException) -> "HTTPError":
         error = HTTPError(e.response)
         if error.status_code == 503:
             error = HTTP503Error(e.response)
         return error
 
 
 class HTTP503Error(HTTPError):
     """Specific instance of HTTPError for 503 errors
 
     Used for detecting whether failed requests should be retried.
     """
+
     pass
 
 
 class InvalidResponse(APIError):
     pass
```

## notifications_python_client/notifications.py

```diff
@@ -6,163 +6,120 @@
 from notifications_python_client.base import BaseAPIClient
 
 logger = logging.getLogger(__name__)
 
 
 class NotificationsAPIClient(BaseAPIClient):
     def send_sms_notification(
-        self,
-        phone_number,
-        template_id,
-        personalisation=None,
-        reference=None,
-        sms_sender_id=None
+        self, phone_number, template_id, personalisation=None, reference=None, sms_sender_id=None
     ):
-        notification = {
-            "phone_number": phone_number,
-            "template_id": template_id
-        }
+        notification = {"phone_number": phone_number, "template_id": template_id}
         if personalisation:
-            notification.update({'personalisation': personalisation})
+            notification.update({"personalisation": personalisation})
         if reference:
-            notification.update({'reference': reference})
+            notification.update({"reference": reference})
         if sms_sender_id:
-            notification.update({'sms_sender_id': sms_sender_id})
-        return self.post(
-            '/v2/notifications/sms',
-            data=notification)
+            notification.update({"sms_sender_id": sms_sender_id})
+        return self.post("/v2/notifications/sms", data=notification)
 
     def send_email_notification(
-        self,
-        email_address,
-        template_id,
-        personalisation=None,
-        reference=None,
-        email_reply_to_id=None
+        self, email_address, template_id, personalisation=None, reference=None, email_reply_to_id=None
     ):
-        notification = {
-            "email_address": email_address,
-            "template_id": template_id
-        }
+        notification = {"email_address": email_address, "template_id": template_id}
         if personalisation:
-            notification.update({'personalisation': personalisation})
+            notification.update({"personalisation": personalisation})
         if reference:
-            notification.update({'reference': reference})
+            notification.update({"reference": reference})
         if email_reply_to_id:
-            notification.update({'email_reply_to_id': email_reply_to_id})
-        return self.post(
-            '/v2/notifications/email',
-            data=notification)
+            notification.update({"email_reply_to_id": email_reply_to_id})
+        return self.post("/v2/notifications/email", data=notification)
 
     def send_letter_notification(self, template_id, personalisation, reference=None):
-        notification = {
-            "template_id": template_id,
-            "personalisation": personalisation
-        }
+        notification = {"template_id": template_id, "personalisation": personalisation}
         if reference:
-            notification.update({'reference': reference})
-        return self.post(
-            '/v2/notifications/letter',
-            data=notification
-        )
+            notification.update({"reference": reference})
+        return self.post("/v2/notifications/letter", data=notification)
 
     def send_precompiled_letter_notification(self, reference, pdf_file, postage=None):
-        content = base64.b64encode(pdf_file.read()).decode('utf-8')
-        notification = {
-            "reference": reference,
-            "content": content
-        }
+        content = base64.b64encode(pdf_file.read()).decode("utf-8")
+        notification = {"reference": reference, "content": content}
 
         if postage:
             notification["postage"] = postage
 
-        return self.post(
-            '/v2/notifications/letter',
-            data=notification
-        )
+        return self.post("/v2/notifications/letter", data=notification)
 
     def get_received_texts(self, older_than=None):
         if older_than:
-            query_string = '?older_than={}'.format(older_than)
+            query_string = "?older_than={}".format(older_than)
         else:
-            query_string = ''
+            query_string = ""
 
-        return self.get('/v2/received-text-messages{}'.format(query_string))
+        return self.get("/v2/received-text-messages{}".format(query_string))
 
     def get_received_texts_iterator(self, older_than=None):
         result = self.get_received_texts(older_than=older_than)
-        received_texts = result.get('received_text_messages')
+        received_texts = result.get("received_text_messages")
         while received_texts:
             for received_text in received_texts:
                 yield received_text
-            next_link = result['links'].get('next')
-            received_text_id = re.search(
-                "[0-F]{8}-[0-F]{4}-[0-F]{4}-[0-F]{4}-[0-F]{12}", next_link, re.I).group(0)
+            next_link = result["links"].get("next")
+            received_text_id = re.search("[0-F]{8}-[0-F]{4}-[0-F]{4}-[0-F]{4}-[0-F]{12}", next_link, re.I).group(0)
             result = self.get_received_texts_iterator(older_than=received_text_id)
-            received_texts = result.get('received_text_messages')
+            received_texts = result.get("received_text_messages")
 
     def get_notification_by_id(self, id):
-        return self.get('/v2/notifications/{}'.format(id))
+        return self.get("/v2/notifications/{}".format(id))
 
     def get_pdf_for_letter(self, id):
-        url = '/v2/notifications/{}/pdf'.format(id)
-        logger.debug("API request {} {}".format('GET', url))
+        url = "/v2/notifications/{}/pdf".format(id)
+        logger.debug("API request %s %s", "GET", url)
         url, kwargs = self._create_request_objects(url, data=None, params=None)
 
-        response = self._perform_request('GET', url, kwargs)
+        response = self._perform_request("GET", url, kwargs)
 
         return BytesIO(response.content)
 
     def get_all_notifications(
-        self,
-        status=None,
-        template_type=None,
-        reference=None,
-        older_than=None,
-        include_jobs=None
+        self, status=None, template_type=None, reference=None, older_than=None, include_jobs=None
     ):
         data = {}
         if status:
-            data.update({'status': status})
+            data.update({"status": status})
         if template_type:
-            data.update({'template_type': template_type})
+            data.update({"template_type": template_type})
         if reference:
-            data.update({'reference': reference})
+            data.update({"reference": reference})
         if older_than:
-            data.update({'older_than': older_than})
+            data.update({"older_than": older_than})
         if include_jobs:
-            data.update({'include_jobs': include_jobs})
-        return self.get(
-            '/v2/notifications',
-            params=data
-        )
+            data.update({"include_jobs": include_jobs})
+        return self.get("/v2/notifications", params=data)
 
     def get_all_notifications_iterator(self, status=None, template_type=None, reference=None, older_than=None):
         result = self.get_all_notifications(status, template_type, reference, older_than)
-        notifications = result.get('notifications')
+        notifications = result.get("notifications")
         while notifications:
             for notification in notifications:
                 yield notification
-            next_link = result['links'].get('next')
+            next_link = result["links"].get("next")
             notification_id = re.search("[0-F]{8}-[0-F]{4}-[0-F]{4}-[0-F]{4}-[0-F]{12}", next_link, re.I).group(0)
             result = self.get_all_notifications(status, template_type, reference, notification_id)
-            notifications = result.get('notifications')
+            notifications = result.get("notifications")
 
     def post_template_preview(self, template_id, personalisation):
-        template = {
-            "personalisation": personalisation
-        }
-        return self.post('/v2/template/{}/preview'.format(template_id), data=template)
+        template = {"personalisation": personalisation}
+        return self.post("/v2/template/{}/preview".format(template_id), data=template)
 
     def get_template(self, template_id):
-        return self.get('/v2/template/{}'.format(template_id))
+        return self.get("/v2/template/{}".format(template_id))
 
     def get_template_version(self, template_id, version):
-        return self.get('/v2/template/{}/version/{}'.format(template_id, version))
+        return self.get("/v2/template/{}/version/{}".format(template_id, version))
 
     def get_all_template_versions(self, template_id):
-        return self.get('service/{}/template/{}/versions'.format(self.service_id, template_id))
+        return self.get("service/{}/template/{}/versions".format(self.service_id, template_id))
 
     def get_all_templates(self, template_type=None):
-        _template_type = '?type={}'.format(template_type) if template_type else ''
+        _template_type = "?type={}".format(template_type) if template_type else ""
 
-        return self.get('/v2/templates{}'.format(_template_type))
+        return self.get("/v2/templates{}".format(_template_type))
```

## notifications_python_client/utils.py

```diff
@@ -3,17 +3,17 @@
 DOCUMENT_UPLOAD_SIZE_LIMIT = 2 * 1024 * 1024
 
 
 def prepare_upload(f, is_csv=False, confirm_email_before_download=None, retention_period=None):
     contents = f.read()
 
     if len(contents) > DOCUMENT_UPLOAD_SIZE_LIMIT:
-        raise ValueError('File is larger than 2MB')
+        raise ValueError("File is larger than 2MB")
 
     file_data = {
-        'file': base64.b64encode(contents).decode('ascii'),
-        'is_csv': is_csv,
-        'confirm_email_before_download': confirm_email_before_download,
-        'retention_period': retention_period
+        "file": base64.b64encode(contents).decode("ascii"),
+        "is_csv": is_csv,
+        "confirm_email_before_download": confirm_email_before_download,
+        "retention_period": retention_period,
     }
 
     return file_data
```

## Comparing `notifications_python_client-8.0.0.dist-info/LICENSE` & `notifications_python_client-8.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `notifications_python_client-8.0.0.dist-info/METADATA` & `notifications_python_client-8.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notifications-python-client
-Version: 8.0.0
+Version: 8.0.1
 Summary: Python API client for GOV.UK Notify.
 Home-page: https://github.com/alphagov/notifications-python-client
 Author: Government Digital Service
 License: MIT
 Keywords: gds govuk notify
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `notifications_python_client-8.0.0.dist-info/RECORD` & `notifications_python_client-8.0.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-notifications_python_client/__init__.py,sha256=Nta3zqorEqSpL8Ym6dcpCx9rNJyEcwB9bowb8lCOfHo,646
-notifications_python_client/authentication.py,sha256=Q0-YWCC6be3zqCsr_-RiJH4d2t7HqYP10DF2RwebDKU,4682
-notifications_python_client/base.py,sha256=zWJh1stvvnmGZQDI6RAhchatZn5jHmFM305XB64as9o,4017
-notifications_python_client/errors.py,sha256=UbSrhz3ZnFeY648-QDB1M5gebI3R3-BbaEhb2e-P3r0,2438
-notifications_python_client/notifications.py,sha256=QS7LNaRpDxzIWt4fchpsVFcm5dH_tpVWxAGYotw_VyQ,5889
+notifications_python_client/__init__.py,sha256=YkzQc_agFM_YSEtCM3B8XjkczZH0mgOmeSt49RQ_vhU,637
+notifications_python_client/authentication.py,sha256=HUOchdPtdMv20EFgD6O1xDnPqHUgpcwOSTKm772D1UU,4662
+notifications_python_client/base.py,sha256=q4kluPfYRAF370WmHbYuBWZ5mLyXrW0QiCof-xv4SSM,3683
+notifications_python_client/errors.py,sha256=Jsby_ww6xiJVpEQl-b4Psdawz9LE390rtoCuXLjxMbU,2438
+notifications_python_client/notifications.py,sha256=Ns6QOQSEVKmMtBCuWqVHyB0YyYDqdits4Yau_IY2ub0,5435
 notifications_python_client/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-notifications_python_client/utils.py,sha256=GEg4jG8XS8m8WycQoshTRe7N6VtxlpooyfksC-A-MTg,536
-notifications_python_client-8.0.0.dist-info/LICENSE,sha256=ArTAWSfEszf0_SxXDz1S9HbshIn78-RfUZLDF0UgULA,1094
-notifications_python_client-8.0.0.dist-info/METADATA,sha256=PmPS0F7eH_kHKXMthmAxN0f6qoMiNzrFYCOJ0CMWtkw,1039
-notifications_python_client-8.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-notifications_python_client-8.0.0.dist-info/top_level.txt,sha256=RAa3Hvf6kd59bZGL4QBm5zVsiv6MegJquMXAQubXM3A,28
-notifications_python_client-8.0.0.dist-info/RECORD,,
+notifications_python_client/utils.py,sha256=XPsQuFJ2pP4IGh8OKJeoBw-eM6W1MJKlfkNlMHKhbHM,537
+notifications_python_client-8.0.1.dist-info/LICENSE,sha256=ArTAWSfEszf0_SxXDz1S9HbshIn78-RfUZLDF0UgULA,1094
+notifications_python_client-8.0.1.dist-info/METADATA,sha256=zHshrfOhiivkREPiW8aUFY5rzRfd7Tz0Yvo-rvLE8ks,1039
+notifications_python_client-8.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+notifications_python_client-8.0.1.dist-info/top_level.txt,sha256=RAa3Hvf6kd59bZGL4QBm5zVsiv6MegJquMXAQubXM3A,28
+notifications_python_client-8.0.1.dist-info/RECORD,,
```

