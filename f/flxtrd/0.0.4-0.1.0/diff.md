# Comparing `tmp/flxtrd-0.0.4.tar.gz` & `tmp/flxtrd-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flxtrd-0.0.4.tar", max compression
+gzip compressed data, was "flxtrd-0.1.0.tar", max compression
```

## Comparing `flxtrd-0.0.4.tar` & `flxtrd-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,18 @@
--rw-r--r--   0        0        0     9135 2023-05-17 07:19:03.818074 flxtrd-0.0.4/LICENSE
--rw-r--r--   0        0        0     1489 2023-05-26 12:52:03.065023 flxtrd-0.0.4/README.md
--rw-r--r--   0        0        0     1936 2023-05-26 12:46:40.793011 flxtrd-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      417 2023-05-26 12:05:54.244915 flxtrd-0.0.4/src/flxtrd/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 11:38:00.772850 flxtrd-0.0.4/src/flxtrd/core/__init__.py
--rw-r--r--   0        0        0      148 2023-05-26 11:56:09.804892 flxtrd-0.0.4/src/flxtrd/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1902 2023-05-26 12:52:17.085024 flxtrd-0.0.4/src/flxtrd/core/__pycache__/api_client.cpython-310.pyc
--rw-r--r--   0        0        0     1756 2023-05-26 12:44:23.737005 flxtrd-0.0.4/src/flxtrd/core/api_client.py
--rw-r--r--   0        0        0        0 2023-05-26 11:38:08.360850 flxtrd-0.0.4/src/flxtrd/core/plugins/__init__.py
--rw-r--r--   0        0        0      156 2023-05-26 12:00:50.840903 flxtrd-0.0.4/src/flxtrd/core/plugins/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1793 2023-05-26 12:36:19.900987 flxtrd-0.0.4/src/flxtrd/core/plugins/__pycache__/auth.cpython-310.pyc
--rw-r--r--   0        0        0     1017 2023-05-26 12:41:50.480999 flxtrd-0.0.4/src/flxtrd/core/plugins/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      957 2023-05-26 12:36:19.916987 flxtrd-0.0.4/src/flxtrd/core/plugins/__pycache__/log.cpython-310.pyc
--rw-r--r--   0        0        0     1041 2023-05-26 12:35:35.412985 flxtrd-0.0.4/src/flxtrd/core/plugins/auth.py
--rw-r--r--   0        0        0      469 2023-05-26 12:41:28.000999 flxtrd-0.0.4/src/flxtrd/core/plugins/base.py
--rw-r--r--   0        0        0      430 2023-05-26 12:36:16.552986 flxtrd-0.0.4/src/flxtrd/core/plugins/log.py
--rw-r--r--   0        0        0        0 2023-05-26 11:37:40.696849 flxtrd-0.0.4/src/flxtrd/protocols/__init__.py
--rw-r--r--   0        0        0      153 2023-05-26 11:56:09.816892 flxtrd-0.0.4/src/flxtrd/protocols/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      733 2023-05-26 12:08:38.328922 flxtrd-0.0.4/src/flxtrd/protocols/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0      798 2023-05-26 11:31:42.840835 flxtrd-0.0.4/src/flxtrd/protocols/__pycache__/base_api.cpython-310.pyc
--rw-r--r--   0        0        0      260 2023-05-26 12:08:28.712921 flxtrd-0.0.4/src/flxtrd/protocols/base.py
--rw-r--r--   0        0        0        0 2023-05-26 11:45:29.372867 flxtrd-0.0.4/src/flxtrd/protocols/grpc/__init__.py
--rw-r--r--   0        0        0      158 2023-05-26 12:07:00.048918 flxtrd-0.0.4/src/flxtrd/protocols/grpc/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      570 2023-05-26 12:07:00.048918 flxtrd-0.0.4/src/flxtrd/protocols/grpc/__pycache__/grpc_api.cpython-310.pyc
--rw-r--r--   0        0        0      527 2023-05-26 11:32:55.156838 flxtrd-0.0.4/src/flxtrd/protocols/grpc/__pycache__/grpc_client.cpython-310.pyc
--rw-r--r--   0        0        0      777 2023-05-26 12:06:20.196916 flxtrd-0.0.4/src/flxtrd/protocols/grpc/grpc_api.py
--rw-r--r--   0        0        0        0 2023-05-26 12:00:47.920903 flxtrd-0.0.4/src/flxtrd/protocols/rest/__init__.py
--rw-r--r--   0        0        0      158 2023-05-26 12:00:50.596903 flxtrd-0.0.4/src/flxtrd/protocols/rest/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1348 2023-05-26 12:30:30.944973 flxtrd-0.0.4/src/flxtrd/protocols/rest/__pycache__/rest_api.cpython-310.pyc
--rw-r--r--   0        0        0      841 2023-05-25 12:34:41.675840 flxtrd-0.0.4/src/flxtrd/protocols/rest/__pycache__/rest_client.cpython-310.pyc
--rw-r--r--   0        0        0     1145 2023-05-26 12:20:23.344949 flxtrd-0.0.4/src/flxtrd/protocols/rest/rest_api.py
--rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 flxtrd-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     9136 2023-06-03 18:45:23.386447 flxtrd-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4046 2023-06-03 18:48:16.702096 flxtrd-0.1.0/README.md
+-rw-r--r--   0        0        0     2117 2023-06-03 18:45:23.386447 flxtrd-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      610 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:23:00.709774 flxtrd-0.1.0/src/flxtrd/core/__init__.py
+-rw-r--r--   0        0        0     4769 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/api_client.py
+-rw-r--r--   0        0        0      581 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/logger.py
+-rw-r--r--   0        0        0        0 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/plugins/__init__.py
+-rw-r--r--   0        0        0     4405 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/plugins/auth.py
+-rw-r--r--   0        0        0      441 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/plugins/base.py
+-rw-r--r--   0        0        0     1248 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/plugins/devices.py
+-rw-r--r--   0        0        0      501 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/plugins/log.py
+-rw-r--r--   0        0        0     2451 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/core/types.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:23:00.709774 flxtrd-0.1.0/src/flxtrd/protocols/__init__.py
+-rw-r--r--   0        0        0     8590 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/protocols/ampq.py
+-rw-r--r--   0        0        0      257 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/protocols/base.py
+-rw-r--r--   0        0        0     1545 2023-06-03 18:45:23.386447 flxtrd-0.1.0/src/flxtrd/protocols/restapi.py
+-rw-r--r--   0        0        0     4787 1970-01-01 00:00:00.000000 flxtrd-0.1.0/PKG-INFO
```

### Comparing `flxtrd-0.0.4/LICENSE` & `flxtrd-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -44,8 +44,8 @@
 
 7. Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
 
 8. Limitation of Liability. In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
 
 9. Accepting Warranty or Additional Liability. While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
 
-END OF TERMS AND CONDITIONS
+END OF TERMS AND CONDITIONS
```

### Comparing `flxtrd-0.0.4/pyproject.toml` & `flxtrd-0.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flxtrd"
-version = "0.0.4"
+version = "0.1.0"
 description = "Public client API for the flexible energy trading market GLocalFlex."
 authors = ["glocalflex"]
 repository = "https://github.com/glocalflex/GLocalFlexTrade"
 documentation = "https://glocalflex.github.io/GLocalFlexTrade/"
 readme = "README.md"
 # packages = [
 #   {include = "src"},
@@ -22,42 +22,51 @@
 mypy = "^0.981"
 pre-commit = "^2.20.0"
 tox = "^3.25.1"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^8.5.10"
+mkdocs-glightbox = {version = ">=0.3.4"}
 mkdocstrings = {extras = ["python"], version = "^0.19.0"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # [tool.poetry.scripts]
 # gflex-trading-bot = "gflex.client:main"
 
+[tool.flake8]
+max-line-length = 90
+max-complexity = 18
+ignore = "F401 E501"
+
 [tool.black]
-line-length = 120
-target-version = ['py37']
+line-length = 90
+target-version = ['py310']
 preview = true
 
 [tool.mypy]
 files = ["flxtrd"]
 disallow_untyped_defs = "True"
 disallow_any_unimported = "True"
 no_implicit_optional = "True"
 check_untyped_defs = "True"
 warn_return_any = "True"
 warn_unused_ignores = "True"
 show_error_codes = "True"
 
+[tool.isort]
+profile = "black"
+
 [tool.ruff]
 target-version = "py37"
-line-length = 120
-fix = true
+line-length = 90
+fix = false
 select = [
     # flake8-2020
     "YTT",
     # flake8-bandit
     "S",
     # flake8-bugbear
     "B",
@@ -87,20 +96,20 @@
     "TRY",
 ]
 ignore = [
     # LineTooLong
     "E501",
     # DoNotAssignLambda
     "E731",
+    # Import unused
+    "F401"
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S101"]
 
 [tool.coverage.report]
 skip_empty = true
 
 [tool.coverage.run]
 branch = true
-source = ["flxtrd"]
-
-
+# source = ["flxtrd"]
```

### Comparing `flxtrd-0.0.4/src/flxtrd/protocols/rest/rest_api.py` & `flxtrd-0.1.0/src/flxtrd/protocols/restapi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,50 @@
+from typing import Optional
+
 import requests
-from typing import List, Optional
 
-from flxtrd.core.plugins.base import BasePlugin
 from flxtrd.protocols.base import BaseAPI
 
+
 class RestAPI(BaseAPI):
-    """REST API implementation that connects to public API"""
-    
+    """Example REST API class that uses the requests library to make HTTP requests"""
+
     def __init__(self, base_url: str):
         super().__init__(base_url=base_url)
 
-    def send_request(self, method: str,
-                     endpoint: str,
-                     params: Optional[dict] = None,
-                     data: Optional[dict] = None,
-                     **kwargs) -> dict:
-        
-        url = self.base_url + endpoint
-        headers = kwargs.get('headers', {})
-        params = kwargs.get('params', {})
-        data = kwargs.get('data', {})
-        print(self)
-        print(f"Send Request to {self.base_url}")
-        print(f"method: {method} url: {url} headers: {headers} params: {params} data: {data}")
-        response = {"status": 200, "data":"successfully simulated a request"}
-        # Make HTTP request using a library of your choice (e.g., requests)
-        # response = requests.request(method, url, headers=headers, params=params, data=data)
+    def send_request(
+        self,
+        method: str,
+        endpoint: str,
+        params: Optional[dict] = None,
+        data: Optional[dict] = None,
+        headers: Optional[dict] = None,
+        ssl: bool = True,
+        verify_ssl: bool = True,
+        **kwargs,
+    ) -> dict:
+        if ssl:
+            url = f"https://{self.base_url + endpoint}"
+        else:
+            url = f"http://{self.base_url + endpoint}"
+
+        response = requests.request(
+            method,
+            url,
+            headers=headers,
+            params=params,
+            data=data,
+            verify=verify_ssl,
+        )
+
+        return response, self.check_status(response, url, endpoint)
 
-        return response
+    def check_status(self, response: requests.Response, url, endpoint) -> bool:
+        """Checks the status code of the response"""
+        if response.status_code == 200:
+            return False
+        elif response.status_code == 401:
+            return "Authentication failed"
+        elif response.status_code == 404:
+            return f"{url} not found"
+        elif response.status_code == 500:
+            return f"""Internal server error, endpoint is correct but data or parameters might be wrong. Check the API documentation for endpoint {endpoint} """
```

