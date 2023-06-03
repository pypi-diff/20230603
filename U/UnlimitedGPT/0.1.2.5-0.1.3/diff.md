# Comparing `tmp/UnlimitedGPT-0.1.2.5.tar.gz` & `tmp/UnlimitedGPT-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnlimitedGPT-0.1.2.5.tar", last modified: Thu Jun  1 10:15:27 2023, max compression
+gzip compressed data, was "UnlimitedGPT-0.1.3.tar", last modified: Sat Jun  3 21:40:43 2023, max compression
```

## Comparing `UnlimitedGPT-0.1.2.5.tar` & `UnlimitedGPT-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-01 10:15:27.166330 UnlimitedGPT-0.1.2.5/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4270 2023-06-01 10:15:27.166330 UnlimitedGPT-0.1.2.5/PKG-INFO
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-01 10:15:27.162330 UnlimitedGPT-0.1.2.5/UnlimitedGPT/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    26342 2023-06-01 10:10:07.000000 UnlimitedGPT-0.1.2.5/UnlimitedGPT/UnlimitedGPT.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.1.2.5/UnlimitedGPT/__init__.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-01 10:15:27.166330 UnlimitedGPT-0.1.2.5/UnlimitedGPT/internal/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2387 2023-06-01 10:05:00.000000 UnlimitedGPT-0.1.2.5/UnlimitedGPT/internal/chatgpt_data.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-31 16:19:36.000000 UnlimitedGPT-0.1.2.5/UnlimitedGPT/internal/driver.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      115 2023-05-31 17:42:42.000000 UnlimitedGPT-0.1.2.5/UnlimitedGPT/internal/exceptions.py
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-31 20:14:14.000000 UnlimitedGPT-0.1.2.5/UnlimitedGPT/internal/objects.py
-drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-01 10:15:27.162330 UnlimitedGPT-0.1.2.5/UnlimitedGPT.egg-info/
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4270 2023-06-01 10:15:26.000000 UnlimitedGPT-0.1.2.5/UnlimitedGPT.egg-info/PKG-INFO
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-06-01 10:15:26.000000 UnlimitedGPT-0.1.2.5/UnlimitedGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-06-01 10:15:26.000000 UnlimitedGPT-0.1.2.5/UnlimitedGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-06-01 10:15:26.000000 UnlimitedGPT-0.1.2.5/UnlimitedGPT.egg-info/requires.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-06-01 10:15:26.000000 UnlimitedGPT-0.1.2.5/UnlimitedGPT.egg-info/top_level.txt
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-06-01 10:15:27.166330 UnlimitedGPT-0.1.2.5/setup.cfg
--rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1775 2023-06-01 10:13:32.000000 UnlimitedGPT-0.1.2.5/setup.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-03 21:40:43.095474 UnlimitedGPT-0.1.3/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4268 2023-06-03 21:40:43.095474 UnlimitedGPT-0.1.3/PKG-INFO
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-03 21:40:43.087476 UnlimitedGPT-0.1.3/UnlimitedGPT/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)    27442 2023-06-03 21:33:51.000000 UnlimitedGPT-0.1.3/UnlimitedGPT/UnlimitedGPT.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      268 2023-05-28 13:45:50.000000 UnlimitedGPT-0.1.3/UnlimitedGPT/__init__.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-03 21:40:43.091475 UnlimitedGPT-0.1.3/UnlimitedGPT/internal/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     2379 2023-06-03 21:04:32.000000 UnlimitedGPT-0.1.3/UnlimitedGPT/internal/chatgpt_data.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1065 2023-05-31 16:19:36.000000 UnlimitedGPT-0.1.3/UnlimitedGPT/internal/driver.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      115 2023-06-03 21:40:19.000000 UnlimitedGPT-0.1.3/UnlimitedGPT/internal/exceptions.py
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     3024 2023-05-31 20:14:14.000000 UnlimitedGPT-0.1.3/UnlimitedGPT/internal/objects.py
+drwxrwxr-x   0 sxvxge    (1000) sxvxge    (1000)        0 2023-06-03 21:40:43.091475 UnlimitedGPT-0.1.3/UnlimitedGPT.egg-info/
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     4268 2023-06-03 21:40:42.000000 UnlimitedGPT-0.1.3/UnlimitedGPT.egg-info/PKG-INFO
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)      380 2023-06-03 21:40:42.000000 UnlimitedGPT-0.1.3/UnlimitedGPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)        1 2023-06-03 21:40:42.000000 UnlimitedGPT-0.1.3/UnlimitedGPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       36 2023-06-03 21:40:42.000000 UnlimitedGPT-0.1.3/UnlimitedGPT.egg-info/requires.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       35 2023-06-03 21:40:42.000000 UnlimitedGPT-0.1.3/UnlimitedGPT.egg-info/top_level.txt
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)       38 2023-06-03 21:40:43.095474 UnlimitedGPT-0.1.3/setup.cfg
+-rw-rw-r--   0 sxvxge    (1000) sxvxge    (1000)     1773 2023-06-03 21:39:00.000000 UnlimitedGPT-0.1.3/setup.py
```

### Comparing `UnlimitedGPT-0.1.2.5/PKG-INFO` & `UnlimitedGPT-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.2.5
+Version: 0.1.3
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
```

### Comparing `UnlimitedGPT-0.1.2.5/UnlimitedGPT/UnlimitedGPT.py` & `UnlimitedGPT-0.1.3/UnlimitedGPT/UnlimitedGPT.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,30 +44,28 @@
     """
 
     def __init__(
         self,
         session_token: str,
         conversation_id: str = '',
         proxy: Optional[str] = None,
-        disable_moderation: bool = True,
+        disable_moderation: bool = False,
         verbose: bool = False,
         headless: bool = False,
         chrome_args: list = [],
     ) -> None:
         self._session_token = session_token
         self._conversation_id = conversation_id
         self._proxy = proxy
         self._disable_moderation = disable_moderation
         self._headless = headless
         self._chrome_args = chrome_args
         self._clicked_buttons = False
         self._init_logger(verbose)
 
-        if not self._session_token:
-            raise ValueError("session_token is required")
         if self._proxy and not re.findall(
             r'(https?|socks(4|5)?):\/\/.+:\d{1,5}', self._proxy # type: ignore
         ):
             raise ValueError('Invalid proxy format')
 
         self._init_browser()
         finalize(self, self.__del__)
@@ -173,15 +171,15 @@
                 {'urls': ['https://chat.openai.com/backend-api/moderations']},
             )
 
         self.logger.debug('Ensuring Cloudflare cookies...')
         self._ensure_cf()
 
         self.logger.debug('Opening chat page...')
-        self.driver.get(f'{CGPTV.chatgpt_chat_url}/{self._conversation_id}')
+        self.driver.get(f'{CGPTV.chat_url}/{self._conversation_id}')
         self._check_blocking_elements()
 
         self._is_active = True
         Thread(target=self._keep_alive, daemon=True).start()
 
     def _keep_alive(self) -> None:
         """
@@ -205,31 +203,31 @@
     def _check_blocking_elements(self) -> None:
         """
         Check for blocking elements and dismiss them.
         """
         self.logger.debug('Looking for blocking elements...')
         try:
             intro = WebDriverWait(self.driver, 5).until(
-                EC.presence_of_element_located(CGPTV.chatgpt_intro)
+                EC.presence_of_element_located(CGPTV.intro)
             )
             self.logger.debug('Dismissing intro...')
             self.driver.execute_script('arguments[0].remove()', intro)
-        except TimeoutException:
+        except TimeoutException: # type: ignore
             pass
 
-        alerts = self.driver.find_elements(*CGPTV.chatgpt_alert)
+        alerts = self.driver.find_elements(*CGPTV.alert)
         if alerts:
             if 'unable to load conversation' in alerts[0].text.lower():
                 raise InvalidConversationID(alerts[0].text)
             self.logger.debug('Dismissing alert...')
             self.driver.execute_script('arguments[0].remove()', alerts[0])
 
         if not self._clicked_buttons:
-            for button in CGPTV.chatgpt_info_buttons:
-                self.driver.safe_click(button, 60)
+            for button in CGPTV.info_buttons:
+                self.driver.safe_click(button, timeout = 60)
             self._clicked_buttons = True
 
     def _ensure_cf(self, retry: int = 3) -> None:
         """
         Ensure Cloudflare cookies are set.
 
         Args:
@@ -246,15 +244,15 @@
 
         self.logger.debug('Getting Cloudflare challenge...')
         self.driver.get('https://chat.openai.com/api/auth/session')
         try:
             WebDriverWait(self.driver, 10).until_not(
                 EC.presence_of_element_located(CGPTV.cf_challenge_form)
             )
-        except TimeoutException:
+        except TimeoutException: # type: ignore
             self.logger.debug(f'Cloudflare challenge failed, retrying {retry}...')
             if retry > 0:
                 self.logger.debug('Closing tab...')
                 self.driver.close()
                 self.driver.switch_to.window(original_window)
                 return self._ensure_cf(retry - 1)
             raise ValueError('Cloudflare challenge failed')
@@ -301,94 +299,110 @@
             TimeoutException: If the message fails to send.
             ValueError: If the response is invalid.
             ValueError: If the response is not found.
         """
         self.logger.debug(f'Sending message with mode {input_mode}{f" with {input_delay} delay" if input_mode == "SLOW" else ""}...')
 
         textbox = WebDriverWait(self.driver, 60).until(
-            EC.element_to_be_clickable(CGPTV.chatgpt_textbox)
+            EC.element_to_be_clickable(CGPTV.textbox)
         )
         if input_mode == 'INSTANT':
             self.driver.execute_script("arguments[0].value = arguments[1];", textbox, message)
         else:
             for char in message:
                 try:
                     textbox.send_keys(char)
                 except StaleElementReferenceException:
                     textbox = WebDriverWait(self.driver, 60).until(
-                        EC.element_to_be_clickable(CGPTV.chatgpt_textbox)
+                        EC.element_to_be_clickable(CGPTV.textbox)
                     )
                     textbox.send_keys(char)
 
-        while True:
-            value = self.driver.execute_script("return arguments[0].value;", textbox)
-            if len(value.strip().replace('\n', '').replace(' ', '').replace('\r', '')) == 0:
-                break
-            textbox.send_keys(Keys.ENTER)
+        textbox.send_keys('a')
+        textbox.send_keys(Keys.BACKSPACE)
+        
+        textbox.send_keys(Keys.ENTER)
 
         self.logger.debug('Waiting for completion...')
         WebDriverWait(self.driver, timeout).until_not(
-            EC.presence_of_element_located(CGPTV.chatgpt_streaming)
+            EC.presence_of_element_located(CGPTV.streaming)
         )
 
         self.logger.debug('Getting response...')
-        responses = self.driver.find_elements(*CGPTV.chatgpt_big_response)
+        responses = self.driver.find_elements(*CGPTV.big_response)
         if responses:
             response = responses[-1]
             if 'text-red' in response.get_attribute('class'):
                 self.logger.debug('Response is an error')
                 raise ValueError(response.text)
-        response = self.driver.find_elements(*CGPTV.chatgpt_small_response)
+        response = self.driver.find_elements(*CGPTV.small_response)
         try:
             response = response[-1]
         except IndexError:
             self.logger.debug('Response not found, resetting conversation...')
             self.reset_conversation()
             raise ValueError('Response not found')
 
-        content = markdownify(response.get_attribute('innerHTML')).replace(
+        content = markdownify(
+            response.get_attribute('innerHTML'),
+            escape_asterisks=False,
+            escape_underscores=False,
+
+        ).replace(
             'Copy code`', '`'
-        )
+        ).rstrip("\n")
+
+        self.logger.debug(f'Message sent')
 
         return ChatGPTResponse(content, self._conversation_id)
 
     def reset_conversation(self) -> None:
         """
         Resets the conversation.
         """
-        if not self.driver.current_url.startswith(CGPTV.chatgpt_chat_url):
+        if not self.driver.current_url.startswith('https://chat.openai.com/'):
             return self.logger.debug('Current URL is not chat page, skipping reset')
 
         self.logger.debug('Resetting conversation...')
-        try:
-            self.driver.safe_click(CGPTV.chatgpt_new_chat, 60)
-        except NoSuchElementException:
+        clicked = self.driver.safe_click(CGPTV.new_chat, timeout = 60)
+        if not clicked:
             self.logger.debug('New chat button not found')
             return self._get_out_of_menu()
+        self.logger.debug('Conversation reset')
 
     def clear_conversations(self) -> None:
         """
         Clears all conversations.
         """
         self.logger.debug('Clearing all conversations...')
         try:
-            menu_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_button, 60)
+            menu_button_clicked = self.driver.safe_click(CGPTV.menu_button, timeout = 60)
             if not menu_button_clicked:
                 self.logger.debug('Could not click menu button')
                 return self._get_out_of_menu()
+            self.logger.debug('Clicked menu button')
             
-            clear_conversations_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_clear_conversations, 60)
+            clear_conversations_button_clicked = self.driver.safe_click(
+                CGPTV.menu_clear_conversations, timeout = 60
+            )
             if not clear_conversations_button_clicked:
                 self.logger.debug('Could not click clear conversations button')
                 return self._get_out_of_menu()
+            self.logger.debug('Clicked clear conversations button')
             
-            confirm_clear_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_clear_conversations, 60)
+            confirm_clear_button_clicked = self.driver.safe_click(
+                CGPTV.menu_confirm_clear_conversations, timeout = 60
+            )
             if not confirm_clear_button_clicked:
                 self.logger.debug('Could not click confirm clear conversations button')
                 return self._get_out_of_menu()
+            self.logger.debug('Clicked confirm clear conversations button')
+
+            self.logger.debug('Cleared all conversations')
+            self._get_out_of_menu()
         except NoSuchElementException:
             self.logger.debug('Could not find menu buttons')
             return self._get_out_of_menu()
 
     def switch_theme(self, theme: Literal['LIGHT', 'DARK', 'OPPOSITE', 'SYSTEM']) -> None:
         """
         Switch the theme.
@@ -402,59 +416,60 @@
             - `LIGHT`: Light theme.
             - `DARK`: Dark theme.
             - `OPPOSITE`: Switch to the opposite theme.
             - `SYSTEM`: Switch to the system theme.
         """
         self.logger.debug(f'Switching theme to {theme}...')
         try:
-            menu_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_button)
+            menu_button_clicked = self.driver.safe_click(CGPTV.menu_button)
             if not menu_button_clicked:
                 self.logger.debug('Could not click menu button')
                 return self._get_out_of_menu()
-
             self.logger.debug('Clicked menu button')
             
-            settings_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_settings_button)
+            settings_button_clicked = self.driver.safe_click(CGPTV.menu_settings)
             if not settings_button_clicked:
                 self.logger.debug('Could not click settings button')
                 return self._get_out_of_menu()
-
             self.logger.debug('Clicked settings button')
             
-            current_theme_value = self.driver.find_element(*CGPTV.chatgpt_outer_html).get_attribute('class')
+            current_theme_value = self.driver.find_element(*CGPTV.outer_html).get_attribute('class')
             current_theme = 'LIGHT' if 'light' in current_theme_value else 'DARK'
             if theme == current_theme:
                 self.logger.debug('Theme is already set to the desired theme')
                 return self._get_out_of_menu()
+            self.logger.debug(f'Current theme is {current_theme}')
 
-            select_element = self.driver.find_element(*CGPTV.chatgpt_theme_select)
+            select_element = self.driver.find_element(*CGPTV.theme_select)
             ActionChains(self.driver).move_to_element(select_element).perform()
-            select_clicked = self.driver.safe_click(CGPTV.chatgpt_theme_select, 60)
+            select_clicked = self.driver.safe_click(CGPTV.theme_select, timeout = 60)
             if not select_clicked:
                 self.logger.debug('Could not click theme select')
                 return self._get_out_of_menu()
+            self.logger.debug('Clicked theme select')
 
             if theme == 'OPPOSITE':
                 if current_theme == 'SYSTEM':
                     self.logger.debug('Theme cannot be set to opposite of system theme')
                     return self._get_out_of_menu()
                     
                 opposite_theme = 'dark' if current_theme == 'LIGHT' else 'light'
-                option_clicked = self.driver.safe_click((By.CSS_SELECTOR, f'select.rounded option[value={opposite_theme}]'), 60)
+                option_clicked = self.driver.safe_click((By.CSS_SELECTOR, f'select.rounded option[value={opposite_theme}]'), timeout = 60)
                 if not option_clicked:
                     self.logger.debug('Could not click opposite theme option')
                     return self._get_out_of_menu()
                 self.logger.debug(f'Selected opposite theme of {current_theme}')
             else:
-                option_clicked = self.driver.safe_click((By.CSS_SELECTOR, f'select.rounded option[value={theme.lower()}]'), 60)
+                option_clicked = self.driver.safe_click((By.CSS_SELECTOR, f'select.rounded option[value={theme.lower()}]'), timeout = 60)
                 if not option_clicked:
                     self.logger.debug('Could not click theme option')
                     return self._get_out_of_menu()
                 self.logger.debug(f'Selected theme {theme}')
             
+            self.logger.debug('Theme switched')
             self._get_out_of_menu()
         except NoSuchElementException:
             self.logger.debug('Could not find theme buttons')
             return self._get_out_of_menu()
 
     def switch_account(self, session_token: str):
         """
@@ -477,29 +492,31 @@
                 'path': '/',
                 'name': '__Secure-next-auth.session-token',
                 'value': session_token,
                 'httpOnly': True,
                 'secure': True,
             },
         )
+        self.logger.debug('Executed CDP command')
 
         self.logger.debug('Validating authorization...')
         self.driver.get('https://chat.openai.com/api/auth/session')
         response = self.driver.page_source
         if response[0] != '{':
             response = self.driver.find_element(By.TAG_NAME, 'pre').text
         response = loads(response)
         if (not response) or (
             'error' in response and response['error'] == 'RefreshAccessTokenError'
         ):
             raise ValueError('Invalid session token')
         self.logger.debug('Authorization is valid')
 
         self.logger.debug('Opening chat page...')
-        self.driver.get(f'{CGPTV.chatgpt_chat_url}/{self._conversation_id}')
+        self.driver.get(f'{CGPTV.chat_url}/{self._conversation_id}')
+        self.logger.debug('Opened chat page')
         self._check_blocking_elements()
     
     def get_session_data(self) -> SessionData:
         """
         Get the session data.
 
         Returns:
@@ -535,14 +552,15 @@
         self.driver.execute_cdp_cmd(
             'Network.deleteCookies',
             {
                 'name': '__Secure-next-auth.session-token',
                 'url': 'https://chat.openai.com',
             },
         )
+        self.logger.debug('Executed CDP command')
         self.driver.get('https://chat.openai.com/api/auth/session')
         response = self.driver.page_source
         if response[0] != '{':
             response = self.driver.find_element(By.TAG_NAME, 'pre').text
         response = loads(response)
         if response == {}:
             self.logger.debug('Logout successful')
@@ -554,35 +572,35 @@
 
         Args:
         ----------
             state (bool, optional): The state to set the chat history toggle to. Defaults to False.
         """
         self.logger.debug('Disabling chat history...')
         try:
-            menu_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_button)
+            menu_button_clicked = self.driver.safe_click(CGPTV.menu_button)
             if not menu_button_clicked:
                 self.logger.debug('Could not click menu button')
                 return self._get_out_of_menu()
 
             self.logger.debug('Clicked menu button')
             
-            settings_button_clicked = self.driver.safe_click(CGPTV.chatgpt_menu_settings_button)
+            settings_button_clicked = self.driver.safe_click(CGPTV.menu_settings)
             if not settings_button_clicked:
                 self.logger.debug('Could not click settings button')
                 return self._get_out_of_menu()
 
             self.logger.debug('Clicked settings button')
 
             wait = WebDriverWait(self.driver, 60)
 
             # Click "Data controls" button
-            data_controls_button_clicked = self.driver.safe_click(
-                CGPTV.chatgpt_data_controls_button, 60
+            data_controls_clicked = self.driver.safe_click(
+                CGPTV.data_controls, timeout = 60
             )
-            if not data_controls_button_clicked:
+            if not data_controls_clicked:
                 self.logger.debug('Could not click data controls button')
                 return self._get_out_of_menu()
 
             # Click "Disable chat history" button
             # Not using safe_click because it there are some checks that need to be done before clicking
             chat_history_toggle = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, f'button[aria-label="Chat History & Training"]')))
             current_state = True if chat_history_toggle.get_attribute('aria-checked') == 'true' else False
@@ -613,41 +631,59 @@
             TimeoutException: If the click fails to succeed.
             ValueError: If the response is invalid.
             ValueError: If the response is not found.
         """
         self.logger.debug('Regenerating response...')
 
         # Click "Regenerate response" button
-        regenerate_response_button_clicked = self.driver.safe_click(
-            CGPTV.chatgpt_regenerate_response_button, click_timeout
+        regenerate_response_clicked = self.driver.safe_click(
+            CGPTV.regenerate_response, timeout = click_timeout
         )
-        if not regenerate_response_button_clicked:
+        if not regenerate_response_clicked:
             self.logger.debug('Could not click regenerate response button')
             raise TimeoutException('Could not click regenerate response button')
 
         # Get the response, same way as send_message without the part of sending the message
         self.logger.debug('Waiting for completion...')
         WebDriverWait(self.driver, message_timeout).until_not(
-            EC.presence_of_element_located(CGPTV.chatgpt_streaming)
+            EC.presence_of_element_located(CGPTV.streaming)
         )
 
         self.logger.debug('Getting response...')
-        responses = self.driver.find_elements(*CGPTV.chatgpt_big_response)
+        responses = self.driver.find_elements(*CGPTV.big_response)
         if responses:
             response = responses[-1]
             if 'text-red' in response.get_attribute('class'):
                 self.logger.debug('Response is an error')
                 raise ValueError(response.text)
-        response = self.driver.find_elements(*CGPTV.chatgpt_small_response)
+        response = self.driver.find_elements(*CGPTV.small_response)
         try:
             response = response[-1]
         except IndexError:
             self.logger.debug('Response not found, resetting conversation...')
             self.reset_conversation()
             raise ValueError('Response not found')
 
         content = markdownify(response.get_attribute('innerHTML')).replace(
             'Copy code`', '`'
         )
         
         self.logger.debug('Regenerated response')
         return ChatGPTResponse(content, self._conversation_id)
+
+    def switch_conversation(self, conversation_id: str) -> None:
+        """
+        Switch the conversation.
+
+        Args:
+        ----------
+            conversation_id (str): The conversation ID to switch to.
+
+        Raises:
+        ----------
+            InvalidConversationID: If the conversation ID is invalid.
+        """
+        self.logger.debug('Switching conversation...')
+        self.driver.get(f'{CGPTV.chat_url}/{conversation_id}')
+        self._check_blocking_elements()
+        self._conversation_id = conversation_id
+        self.logger.debug(f'Switched conversation to {conversation_id}')
```

### Comparing `UnlimitedGPT-0.1.2.5/UnlimitedGPT/internal/chatgpt_data.py` & `UnlimitedGPT-0.1.3/UnlimitedGPT/internal/chatgpt_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,79 +1,86 @@
 from dataclasses import dataclass
 from selenium.webdriver.common.by import By
 
 @dataclass
 class ChatGPTVariables:
+    # Other
+    outer_html = (By.XPATH, "/html")
     cf_challenge_form = (By.ID, 'challenge-form')
-
-    chatgpt_outer_html = (
-        By.XPATH,
-        "/html"
-    )
-    chatgpt_textbox = (
+    chats_list_first_node = (
         By.XPATH,
-        '/html/body/div[1]/div[2]/div[2]/div/main/div[3]/form/div/div/textarea'
+        '//div[substring(@class, string-length(@class) - string-length("text-sm") + 1)  = "text-sm"]//a',
     )
-    chatgpt_info_buttons = [
+
+    # Popups and such
+    info_buttons = (
         (By.XPATH, '/html/body/div[3]/div/div/div/div[2]/div/div[2]/button'),
         (By.XPATH, '/html/body/div[3]/div/div/div/div[2]/div/div[2]/button[2]'),
         (By.XPATH, '/html/body/div[3]/div/div/div/div[2]/div/div[2]/button[2]'),
-    ]
-    chatgpt_streaming = (
+    )
+    alert = (
+        By.XPATH,
+        '//div[@role="alert"]'
+    )
+    intro = (
+        By.ID,
+        'headlessui-portal-root'
+    )
+    
+    # Responses and such
+    streaming = (
         By.XPATH,
         '//div[starts-with(@class, "result-streaming markdown prose")]'
     )
-    chatgpt_big_response = (
+    big_response = (
         By.XPATH,
         '//div[@class="flex-1 overflow-hidden"]//div[p]'
     )
-    chatgpt_small_response = (
+    small_response = (
         By.XPATH,
         '//div[starts-with(@class, "markdown prose w-full break-words")]',
     )
-    chatgpt_alert = (
+    textbox = (
         By.XPATH,
-        '//div[@role="alert"]'
+        '/html/body/div[1]/div[2]/div[2]/div/main/div[2]/form/div/div/textarea'
     )
-    chatgpt_intro = (
-        By.ID,
-        'headlessui-portal-root'
+    regenerate_response = (
+        By.XPATH,
+        "/html/body/div[1]/div[2]/div[2]/div/main/div[2]/form/div/div[1]/div/button"
     )
-
-    chatgpt_new_chat = (
+    new_chat = (
         By.LINK_TEXT,
         'New chat'
     )
-    chatgpt_chats_list_first_node = (
-        By.XPATH,
-        '//div[substring(@class, string-length(@class) - string-length("text-sm") + 1)  = "text-sm"]//a',
-    )
-    chatgpt_menu_button = (
+
+    # Menu buttons
+    menu_button = (
         By.XPATH,
-        "/html/body/div[1]/div[2]/div[1]/div/div/div/nav/div[3]/div/button"
+        "/html/body/div[1]/div[2]/div[1]/div/div/div/nav/div[4]/div/button"
     )
-    chatgpt_menu_clear_conversations = (
+    menu_clear_conversations = (
         # By.XPATH,
         # "/html/body/div[1]/div[2]/div[1]/div/div/div/nav/div[3]/div/div/nav/a[2]"
         By.LINK_TEXT,
         'Clear conversations'
-    ) # Confirm button is the same path
-    chatgpt_menu_settings_button = (
+    )
+    menu_confirm_clear_conversations = (
+        By.LINK_TEXT,
+        "Confirm clear conversations"
+    )
+    menu_settings = (
         # By.XPATH,
         # "/html/body/div[1]/div[2]/div[1]/div/div/div/nav/div[3]/div/div/nav/a[3]"
         By.LINK_TEXT,
         'Settings'
     )
-    chatgpt_regenerate_response_button = (
-        By.XPATH,
-        "/html/body/div[1]/div[2]/div[2]/div/main/div[3]/form/div/div[1]/div/button"
-    )
-    chatgpt_theme_select = (
+    theme_select = (
         By.CSS_SELECTOR,
         'select.rounded'
     )
-    chatgpt_data_controls_button = (
+    data_controls = (
         By.CSS_SELECTOR,
         'button[data-state="inactive"][id^="radix-"][id$="-trigger-DataControls"]'
     )
-
-    chatgpt_chat_url = 'https://chat.openai.com/chat'
+    
+    # URLs
+    chat_url = 'https://chat.openai.com/chat'
```

### Comparing `UnlimitedGPT-0.1.2.5/UnlimitedGPT/internal/driver.py` & `UnlimitedGPT-0.1.3/UnlimitedGPT/internal/driver.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.1.2.5/UnlimitedGPT/internal/objects.py` & `UnlimitedGPT-0.1.3/UnlimitedGPT/internal/objects.py`

 * *Files identical despite different names*

### Comparing `UnlimitedGPT-0.1.2.5/UnlimitedGPT.egg-info/PKG-INFO` & `UnlimitedGPT-0.1.3/UnlimitedGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnlimitedGPT
-Version: 0.1.2.5
+Version: 0.1.3
 Summary: An unofficial Python wrapper for OpenAI's ChatGPT API
 Home-page: https://github.com/Sxvxgee/UnlimitedGPT
 Author: Sxvxge
 License: GPL-3.0 license
 Project-URL: Documentation, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md
 Project-URL: Issue tracker, https://github.com/Sxvxgee/UnlimitedGPT/issues
 Project-URL: Changelog, https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md
```

### Comparing `UnlimitedGPT-0.1.2.5/setup.py` & `UnlimitedGPT-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     author='Sxvxge',
     url='https://github.com/Sxvxgee/UnlimitedGPT',
     project_urls={
         'Documentation': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/README.md',
         'Issue tracker': 'https://github.com/Sxvxgee/UnlimitedGPT/issues',
         'Changelog': 'https://github.com/Sxvxgee/UnlimitedGPT/blob/main/CHANGELOG.md',
     },
-    version="0.1.2.5",
+    version="0.1.3",
     packages=['UnlimitedGPT', 'UnlimitedGPT/internal'],
     py_modules=['UnlimitedGPT'],
     license='GPL-3.0 license',
     description='An unofficial Python wrapper for OpenAI\'s ChatGPT API',
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
```

