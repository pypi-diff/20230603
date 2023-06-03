# Comparing `tmp/caqui-1.0.5.tar.gz` & `tmp/caqui-1.0.6.tar.gz`

## Comparing `caqui-1.0.5.tar` & `caqui-1.0.6.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-1.0.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 caqui-1.0.5/sample.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 caqui-1.0.5/test-requirements.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-1.0.5/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.0.5/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.0.5/.vscode/settings.json
--rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.0.5/caqui/__init__.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 caqui-1.0.5/caqui/asynchronous.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.0.5/caqui/constants.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.0.5/caqui/exceptions.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 caqui-1.0.5/caqui/helper.py
--rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 caqui-1.0.5/caqui/synchronous.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/constants.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/fake_responses.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/test_sniffer.py
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/feature/test_functions.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/html/playground.html
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/integration/test_async_scenarios.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/integration/test_sync_scenarios.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/unit/__initi__.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/unit/test_async_unit.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/unit/test_helper.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 caqui-1.0.5/tests/unit/test_sync_unit.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 caqui-1.0.5/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.0.5/LICENSE
--rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 caqui-1.0.5/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 caqui-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    10402 2020-02-02 00:00:00.000000 caqui-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-1.0.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 caqui-1.0.6/sample.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 caqui-1.0.6/test-requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-1.0.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-1.0.6/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-1.0.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.0.6/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.0.6/.vscode/settings.json
+-rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.0.6/caqui/__init__.py
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 caqui-1.0.6/caqui/asynchronous.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.0.6/caqui/constants.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.0.6/caqui/exceptions.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 caqui-1.0.6/caqui/helper.py
+-rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 caqui-1.0.6/caqui/synchronous.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/constants.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/fake_responses.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/test_sniffer.py
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/feature/test_sync_and_async.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/html/playground.html
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/integration/test_async_scenarios.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/integration/test_sync_scenarios.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/unit/__initi__.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/unit/test_async_unit.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/unit/test_helper.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 caqui-1.0.6/tests/unit/test_sync_unit.py
+-rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-1.0.6/utils/coverage.sh
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 caqui-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.0.6/LICENSE
+-rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 caqui-1.0.6/README.md
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 caqui-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 caqui-1.0.6/PKG-INFO
```

### Comparing `caqui-1.0.5/CODE_OF_CONDUCT.md` & `caqui-1.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.5/sample.py` & `caqui-1.0.6/sample.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md` & `caqui-1.0.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md` & `caqui-1.0.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.5/.github/workflows/python-app.yml` & `caqui-1.0.6/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.0.5/.github/workflows/python-publish.yml` & `caqui-1.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.0.5/caqui/__init__.py` & `caqui-1.0.6/caqui/__init__.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.5/caqui/synchronous.py` & `caqui-1.0.6/caqui/synchronous.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import requests
 import json
 from caqui.exceptions import WebDriverError
-from caqui.helper import get_element
+from caqui import helper
 
 HEADERS = {
     "Accept-Encoding": "identity",
     "Accept": "application/json",
     "Content-Type": "application/json;charset=UTF-8",
     "Connection": "keep-alive",
 }
 
 
-def __get(url, payload):
+def __get(url):
     try:
-        return requests.request("GET", url, headers=HEADERS, data=payload).json()
+        return requests.request("GET", url, headers=HEADERS, data={}).json()
     except Exception as error:
         raise WebDriverError("'GET' request failed.") from error
 
 
 def __post(url, payload):
     try:
         return requests.request("POST", url, headers=HEADERS, data=payload).json()
@@ -28,74 +28,145 @@
 def __delete(url):
     try:
         return requests.request("DELETE", url, headers={}, data={}).json()
     except Exception as error:
         raise WebDriverError("'DELETE' request failed.") from error
 
 
+def go_back(driver_url, session):
+    """
+    This command causes the browser to traverse one step backward in the joint session history of the
+    current browse. This is equivalent to pressing the back button in the browser.
+    """
+    try:
+        url = f"{driver_url}/session/{session}/back"
+        __post(url, {})
+        return True
+    except Exception as error:
+        raise WebDriverError(f"Failed to go back to page.") from error
+
+
+def get_url(driver_url, session):
+    """Return the URL from web page:"""
+    try:
+        url = f"{driver_url}/session/{session}/url"
+        response = __get(url)
+        return response.get("value")
+    except Exception as error:
+        raise WebDriverError(f"Failed to get page url.") from error
+
+
+def get_timeouts(driver_url, session):
+    """
+    Return the configured timeouts:
+        {"implicit": 0, "pageLoad": 300000, "script": 30000}
+    """
+    try:
+        url = f"{driver_url}/session/{session}/timeouts"
+        response = __get(url)
+        return response.get("value")
+    except Exception as error:
+        raise WebDriverError(f"Failed to get timeouts.") from error
+
+
+def get_status(driver_url):
+    """
+    Return the status and details of the WebDriver:
+        "build": {
+                "version": "113.0.5672.63 (0e1a4471d5ae5bf128b1bd8f4d627c8cbd55f70c-refs/branch-heads/5672@{#912})"
+            },
+            "message": "ChromeDriver ready for new sessions.",
+            "os": {"arch": "x86_64", "name": "Linux", "version": "5.4.0-150-generic"},
+            "ready": True,
+        }
+    """
+    try:
+        url = f"{driver_url}/status"
+        return __get(url)
+    except Exception as error:
+        raise WebDriverError(f"Failed to get status.") from error
+
+
+def get_title(driver_url, session):
+    """Get the page title"""
+    try:
+        url = f"{driver_url}/session/{session}/title"
+        response = __get(url)
+        return response.get("value")
+    except Exception as error:
+        raise WebDriverError(f"Failed to get page title.") from error
+
+
 def find_elements(driver_url, session, locator_type, locator_value):
+    """Search the DOM elements by 'locator', for example, 'xpath'"""
     try:
         url = f"{driver_url}/session/{session}/elements"
         payload = json.dumps({"using": locator_type, "value": locator_value})
         response = __post(url, payload)
         return [x.get("ELEMENT") for x in response.get("value")]
     except Exception as error:
         raise WebDriverError(
             f"Failed to find elements by '{locator_type}'-'{locator_value}'."
         ) from error
 
 
 def get_property(driver_url, session, element, property):
+    """Get the given HTML property of an element, for example, 'href'"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/property/{property}"
-        response = __get(url, {})
+        response = __get(url)
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get value from element.") from error
 
 
 def go_to_page(driver_url, session, page_url):
+    """Navigate to 'page_url'"""
     try:
         url = f"{driver_url}/session/{session}/url"
         payload = json.dumps({"url": page_url})
         __post(url, payload)
         return True
     except Exception as error:
         raise WebDriverError(f"Failed to navigate to '{page_url}'") from error
 
 
 def close_session(driver_url, session):
+    """Close an opened session and close the browser"""
     try:
         url = f"{driver_url}/session/{session}"
         __delete(url)
         return True
     except Exception as error:
         raise WebDriverError("Failed to close session.") from error
 
 
 def get_text(driver_url, session, element):
+    """Get the text of an element"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/text"
-        response = __get(url, {})
+        response = __get(url)
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get text from element.") from error
 
 
 def send_keys(driver_url, session, element, text):
+    """Fill an editable element, for example a textarea, with a given text"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/value"
         payload = json.dumps({"text": text, "value": [*text], "id": element})
         __post(url, payload)
         return True
     except Exception as error:
         raise WebDriverError(f"Failed to send key '{text}'.") from error
 
 
 def click(driver_url, session, element):
+    """Click on an element"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/click"
         payload = json.dumps({"id": element})
         __post(url, payload)
         return True
     except Exception as error:
         raise WebDriverError("Failed to click on element.") from error
@@ -109,26 +180,28 @@
         return session_id
 
     # Chrome response
     return response.get("sessionId")
 
 
 def get_session(driver_url, capabilities):
+    """Opens a browser and a session. This session is used for all functions to perform events in the page"""
     try:
         url = f"{driver_url}/session"
         data = json.dumps(capabilities)
         response = __post(url, payload=data)
         return __get_session(response)
     except Exception as error:
         raise WebDriverError("Failed to open session.") from error
 
 
 def find_element(driver_url, session, locator_type, locator_value):
+    """Find an element by a 'locator', for example 'xpath'"""
     try:
         url = f"{driver_url}/session/{session}/element"
         payload = json.dumps({"using": locator_type, "value": locator_value})
         response = __post(url, payload)
-        return get_element(response)
+        return helper.get_element(response)
     except Exception as error:
         raise WebDriverError(
             f"Failed to find element by '{locator_type}'-'{locator_value}'."
         ) from error
```

### Comparing `caqui-1.0.5/tests/fake_responses.py` & `caqui-1.0.6/tests/fake_responses.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,20 +21,56 @@
         "sessionId": "4358a5b53794586af59678fc1653dc40",
         "status": 0,
         "value": {"ELEMENT": "0.8851292311864847-1"},
     }
 )
 
 FIND_ELEMENT = DEFAULT
-GET_URL = DEFAULT
 SEND_KEYS = DEFAULT
 CLICK = DEFAULT
 CLOSE_SESSION = DEFAULT
 GO_TO_PAGE = DEFAULT
 
+GET_URL = dict_to_json(
+    {
+        "sessionId": "af67b8ef665d30a687f37365d229fb53",
+        "status": 0,
+        "value": "file:///html/playground.html",
+    }
+)
+GET_TIMEOUTS = dict_to_json(
+    {
+        "sessionId": "10754c8ec2e19133235223f1914ea376",
+        "status": 0,
+        "value": {"implicit": 0, "pageLoad": 300000, "script": 30000},
+    }
+)
+
+
+GET_STATUS = dict_to_json(
+    {
+        "value": {
+            "build": {
+                "version": "113.0.5672.63 (0e1a4471d5ae5bf128b1bd8f4d627c8cbd55f70c-refs/branch-heads/5672@{#912})"
+            },
+            "message": "ChromeDriver ready for new sessions.",
+            "os": {"arch": "x86_64", "name": "Linux", "version": "5.4.0-150-generic"},
+            "ready": True,
+        }
+    }
+)
+
+GET_TITLE = dict_to_json(
+    {
+        "sessionId": "07b00b2e94be84920495d83890c82b60",
+        "status": 0,
+        "value": "Sample page",
+    }
+)
+
 FIND_ELEMENTS = dict_to_json(
     {
         "sessionId": "9be93a374d185216134bf0c3fafee52e",
         "status": 0,
         "value": [
             {"ELEMENT": "C230605181E69CB2C4C36B8E83FE1245_element_1"},
             {"ELEMENT": "C230605181E69CB2C4C36B8E83FE1245_element_2"},
@@ -51,15 +87,14 @@
     }
 )
 
 GET_TEXT = dict_to_json(
     {"sessionId": "5be82d4cd17af92d7ea53a36900d78cb", "status": 0, "value": "any"}
 )
 
-
 GET_SESSION = dict_to_json(
     {
         "sessionId": "4358a5b53794586af59678fc1653dc40",
         "status": 0,
         "value": {
             "acceptInsecureCerts": True,
             "acceptSslCerts": True,
```

### Comparing `caqui-1.0.5/tests/test_sniffer.py` & `caqui-1.0.6/tests/test_sniffer.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,19 +17,30 @@
     }
 
     driver = webdriver.Remote(
         command_executor="http://localhost:9999",
         desired_capabilities=desired_capabilities,
     )
     driver.get(PAGE_URL)
+    driver
     yield driver
     driver.quit()
 
 
 @mark.skip("used just to discover request data")
+def test_back(setup):
+    assert setup.back() == "any"
+
+
+@mark.skip("used just to discover request data")
+def test_get_title(setup):
+    assert setup.title == "any"
+
+
+@mark.skip("used just to discover request data")
 def test_get_attribute(setup):
     driver = setup
     element = driver.find_element("xpath", "//a")
     assert element.get_property("href") == "any"
 
 
 @mark.skip("used just to discover request data")
```

### Comparing `caqui-1.0.5/tests/feature/test_functions.py` & `caqui-1.0.6/tests/feature/test_sync_and_async.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,14 +20,58 @@
         PAGE_URL,
     )
     yield driver_url, session
     synchronous.close_session(driver_url, session)
 
 
 @mark.asyncio
+async def test_go_back(__setup):
+    driver_url, session = __setup
+
+    assert synchronous.go_back(driver_url, session) is True
+    assert await asynchronous.go_back(driver_url, session) is True
+
+
+@mark.asyncio
+async def test_get_url(__setup):
+    driver_url, session = __setup
+    expected = "playground.html"
+
+    assert expected in synchronous.get_url(driver_url, session)
+    assert expected in await asynchronous.get_url(driver_url, session)
+
+
+@mark.asyncio
+async def test_get_timeouts(__setup):
+    driver_url, session = __setup
+    expected = "implicit"
+
+    assert expected in synchronous.get_timeouts(driver_url, session)
+    assert expected in await asynchronous.get_timeouts(driver_url, session)
+
+
+@mark.asyncio
+async def test_get_status(__setup):
+    driver_url, _ = __setup
+    expected = "ready"
+    assert expected in synchronous.get_status(driver_url).get("value")
+    response = await asynchronous.get_status(driver_url)
+    assert expected in response.get("value")
+
+
+@mark.asyncio
+async def test_get_title(__setup):
+    driver_url, session = __setup
+    expected = "Sample page"
+
+    assert synchronous.get_title(driver_url, session) == expected
+    assert await asynchronous.get_title(driver_url, session) == expected
+
+
+@mark.asyncio
 async def test_find_elements(__setup):
     driver_url, session = __setup
     locator_type = "xpath"
     locator_value = "//input"
 
     elements = synchronous.find_elements(
         driver_url, session, locator_type, locator_value
```

### Comparing `caqui-1.0.5/tests/html/playground.html` & `caqui-1.0.6/tests/html/playground.html`

 * *Files identical despite different names*

### Comparing `caqui-1.0.5/tests/integration/test_async_scenarios.py` & `caqui-1.0.6/tests/integration/test_async_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.5/tests/integration/test_sync_scenarios.py` & `caqui-1.0.6/tests/integration/test_sync_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.5/tests/unit/test_helper.py` & `caqui-1.0.6/tests/unit/test_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,31 @@
-from caqui.helper import get_elements
+from caqui.helper import get_elements, get_element
 from pytest import mark
-from tests.fake_responses import FIND_ELEMENTS
+from tests.fake_responses import FIND_ELEMENTS, FIND_ELEMENT
+
+
+@mark.parametrize(
+    "response,expected",
+    [
+        (
+            {
+                "value": {
+                    "element-6066-11e4-a52e-4f735466cecf": "c4cab128-a0a4-4355-93a5-ffd6c7a8b042"
+                },
+            },
+            "c4cab128-a0a4-4355-93a5-ffd6c7a8b042",
+        ),
+        (
+            FIND_ELEMENT,
+            "0.8851292311864847-1",
+        ),
+    ],
+)
+def test_get_element(response, expected):
+    assert get_element(response) == expected
 
 
 @mark.parametrize(
     "response,expected",
     [
         (
             {
```

### Comparing `caqui-1.0.5/tests/unit/test_sync_unit.py` & `caqui-1.0.6/tests/unit/test_sync_unit.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,116 +1,87 @@
 from unittest.mock import patch
-from caqui.synchronous import (
-    find_element,
-    get_session,
-    click,
-    send_keys,
-    get_text,
-    close_session,
-    go_to_page,
-    get_property,
-    find_elements,
-)
-from tests.fake_responses import (
-    FIND_ELEMENT,
-    GET_SESSION,
-    CLICK,
-    GET_TEXT,
-    CLOSE_SESSION,
-    GO_TO_PAGE,
-    GET_PROPERTY_VALUE,
-    SEND_KEYS,
-    FIND_ELEMENTS,
-)
-
-
-def __setup():
-    driver_url = "http://any:9999"
-    session = "4358a5b53794586af59678fc1653dc40"
-    element = "0.8851292311864847-1"
-    return driver_url, session, element
+from caqui import synchronous
+from tests import fake_responses
 
 
-@patch("requests.request", return_value=FIND_ELEMENTS)
+@patch("requests.request", return_value=fake_responses.GET_URL)
+def test_get_url(*args):
+    expected = "playground.html"
+
+    assert expected in synchronous.get_url("", "")
+
+
+@patch("requests.request", return_value=fake_responses.GET_TIMEOUTS)
+def test_get_timeouts(*args):
+    expected = "implicit"
+
+    assert expected in synchronous.get_timeouts("", "")
+
+
+@patch("requests.request", return_value=fake_responses.GET_STATUS)
+def test_get_status(*args):
+    assert synchronous.get_status("").get("value").get("ready") is True
+
+
+@patch("requests.request", return_value=fake_responses.GET_TITLE)
+def test_get_title(*args):
+    expected = "Sample page"
+
+    assert synchronous.get_title("", "") == expected
+
+
+@patch("requests.request", return_value=fake_responses.FIND_ELEMENTS)
 def test_find_elements(*args):
-    driver_url, session, _ = __setup()
-    locator_type = "xpath"
-    locator_value = "//input"
     element = "C230605181E69CB2C4C36B8E83FE1245_element_2"
 
-    elements = find_elements(driver_url, session, locator_type, locator_value)
+    elements = synchronous.find_elements("", "", "", "")
 
     assert element in elements
     assert len(elements) == 3
 
 
-@patch("requests.request", return_value=GET_PROPERTY_VALUE)
+@patch("requests.request", return_value=fake_responses.GET_PROPERTY_VALUE)
 def test_get_property(*args):
-    driver_url, session, _ = __setup()
-    element = "any"
-    property = "value"
     expected = "any_value"
 
-    assert get_property(driver_url, session, element, property) == expected
+    assert synchronous.get_property("", "", "", "") == expected
 
 
-@patch("requests.request", return_value=GO_TO_PAGE)
+@patch("requests.request", return_value=fake_responses.GO_TO_PAGE)
 def test_go_to_page(*args):
-    driver_url, session, _ = __setup()
-    url = "http://any.com"
-
-    assert go_to_page(driver_url, session, url) is True
+    assert synchronous.go_to_page("", "", "") is True
 
 
-@patch("requests.request", return_value=CLOSE_SESSION)
+@patch("requests.request", return_value=fake_responses.CLOSE_SESSION)
 def test_close_session(*args):
-    driver_url, session, _ = __setup()
+    assert synchronous.close_session("", "") is True
 
-    assert close_session(driver_url, session) is True
 
-
-@patch("requests.request", return_value=GET_TEXT)
+@patch("requests.request", return_value=fake_responses.GET_TEXT)
 def test_get_text(*args):
-    driver_url, session, element = __setup()
     expected = "any"
 
-    assert get_text(driver_url, session, element) == expected
+    assert synchronous.get_text("", "", "") == expected
 
 
-@patch("requests.request", return_value=SEND_KEYS)
+@patch("requests.request", return_value=fake_responses.SEND_KEYS)
 def test_send_keys(*args):
-    driver_url, session, element = __setup()
-    text = "any"
-
-    assert send_keys(driver_url, session, element, text) is True
+    assert synchronous.send_keys("", "", "", "") is True
 
 
-@patch("requests.request", return_value=CLICK)
+@patch("requests.request", return_value=fake_responses.CLICK)
 def test_click(*args):
-    driver_url, session, element = __setup()
-
-    assert click(driver_url, session, element) is True
+    assert synchronous.click("", "", "") is True
 
 
-@patch("requests.request", return_value=GET_SESSION)
+@patch("requests.request", return_value=fake_responses.GET_SESSION)
 def test_get_session(*args):
-    driver_url = "http://any:9999"
-    payload = {
-        "desiredCapabilities": {
-            "browserName": "firefox",
-            "marionette": True,
-            "acceptInsecureCerts": True,
-        }
-    }
     expected = "4358a5b53794586af59678fc1653dc40"
 
-    assert get_session(driver_url, payload) == expected
+    assert synchronous.get_session("", "") == expected
 
 
-@patch("requests.request", return_value=FIND_ELEMENT)
+@patch("requests.request", return_value=fake_responses.FIND_ELEMENT)
 def test_find_element(*args):
-    driver_url, session, _ = __setup()
-    locator_type = "xpath"
-    locator_value = "//input"
     expected = "0.8851292311864847-1"
 
-    assert find_element(driver_url, session, locator_type, locator_value) == expected
+    assert synchronous.find_element("", "", "", "") == expected
```

### Comparing `caqui-1.0.5/.gitignore` & `caqui-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `caqui-1.0.5/LICENSE` & `caqui-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `caqui-1.0.5/README.md` & `caqui-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.5/pyproject.toml` & `caqui-1.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 [tool.setuptools.packages.find]
 include = ["caqui*"]
 exclude = ["tests*", "utils", ".vscode", ".git*", "dist"]
 
 [project]
 name = "caqui"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Douglas Cardoso", email="noemail@noemail.com" },
 ]
 description = "Run asynchronous commands in WebDrivers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
   "requests",
```

### Comparing `caqui-1.0.5/PKG-INFO` & `caqui-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: caqui
-Version: 1.0.5
+Version: 1.0.6
 Summary: Run asynchronous commands in WebDrivers
 Project-URL: Homepage, https://github.com/douglasdcm/caqui
 Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
 Author-email: Douglas Cardoso <noemail@noemail.com>
 License-File: LICENSE
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: aiohttp
 Requires-Dist: requests
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: caqui Version: 1.0.5 Summary: Run asynchronous
+Metadata-Version: 2.1 Name: caqui Version: 1.0.6 Summary: Run asynchronous
 commands in WebDrivers Project-URL: Homepage, https://github.com/douglasdcm/
 caqui Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
 Author-email: Douglas Cardoso
-noemail.com> License-File: LICENSE Classifier: Development Status :: 3 - Alpha
+noemail.com> License-File: LICENSE Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.7 Requires-Dist: aiohttp Requires-Dist: requests Description-
 Content-Type: text/markdown # Caqui **Caqui** is intended to command executions
 against Drivers synchronously and asynchronously. Launch the Driver as a server
 and send requests to it. The intention is that the user does not worry about
 which Driver he/she is using. It can be **Web**Drivers like [Selenium](https://
```

