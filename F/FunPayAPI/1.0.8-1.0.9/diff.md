# Comparing `tmp/FunPayAPI-1.0.8.tar.gz` & `tmp/FunPayAPI-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FunPayAPI-1.0.8.tar", last modified: Fri May 19 09:59:42 2023, max compression
+gzip compressed data, was "FunPayAPI-1.0.9.tar", last modified: Sat Jun  3 08:08:18 2023, max compression
```

## Comparing `FunPayAPI-1.0.8.tar` & `FunPayAPI-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 09:59:42.931732 FunPayAPI-1.0.8/
-drwxrwxrwx   0        0        0        0 2023-05-19 09:59:42.897732 FunPayAPI-1.0.8/FunPayAPI/
--rw-rw-rw-   0        0        0      162 2023-05-15 12:08:20.000000 FunPayAPI-1.0.8/FunPayAPI/__init__.py
--rw-rw-rw-   0        0        0    62476 2023-05-19 09:58:25.000000 FunPayAPI-1.0.8/FunPayAPI/account.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:59:42.924731 FunPayAPI-1.0.8/FunPayAPI/common/
--rw-rw-rw-   0        0        0        0 2023-05-12 17:46:25.000000 FunPayAPI-1.0.8/FunPayAPI/common/__init__.py
--rw-rw-rw-   0        0        0     4842 2023-05-14 16:49:23.000000 FunPayAPI-1.0.8/FunPayAPI/common/enums.py
--rw-rw-rw-   0        0        0     7842 2023-05-14 23:54:13.000000 FunPayAPI-1.0.8/FunPayAPI/common/exceptions.py
--rw-rw-rw-   0        0        0     8922 2023-05-19 09:07:17.000000 FunPayAPI-1.0.8/FunPayAPI/common/utils.py
--rw-rw-rw-   0        0        0    38978 2023-05-19 09:36:22.000000 FunPayAPI-1.0.8/FunPayAPI/types.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:59:42.930731 FunPayAPI-1.0.8/FunPayAPI/updater/
--rw-rw-rw-   0        0        0        0 2023-05-12 17:46:18.000000 FunPayAPI-1.0.8/FunPayAPI/updater/__init__.py
--rw-rw-rw-   0        0        0     8216 2023-05-11 19:12:41.000000 FunPayAPI-1.0.8/FunPayAPI/updater/events.py
--rw-rw-rw-   0        0        0    20435 2023-05-19 08:54:31.000000 FunPayAPI-1.0.8/FunPayAPI/updater/runner.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:59:42.914730 FunPayAPI-1.0.8/FunPayAPI.egg-info/
--rw-rw-rw-   0        0        0     3602 2023-05-19 09:59:42.000000 FunPayAPI-1.0.8/FunPayAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-05-19 09:59:42.000000 FunPayAPI-1.0.8/FunPayAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 09:59:42.000000 FunPayAPI-1.0.8/FunPayAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-19 09:59:42.000000 FunPayAPI-1.0.8/FunPayAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 09:59:42.000000 FunPayAPI-1.0.8/FunPayAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35801 2023-05-11 21:13:41.000000 FunPayAPI-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     3602 2023-05-19 09:59:42.931732 FunPayAPI-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3011 2023-05-12 11:49:15.000000 FunPayAPI-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 09:59:42.931732 FunPayAPI-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      928 2023-05-19 09:59:32.000000 FunPayAPI-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 08:08:18.674287 FunPayAPI-1.0.9/
+drwxrwxrwx   0        0        0        0 2023-06-03 08:08:18.643287 FunPayAPI-1.0.9/FunPayAPI/
+-rw-rw-rw-   0        0        0      162 2023-05-15 12:08:20.000000 FunPayAPI-1.0.9/FunPayAPI/__init__.py
+-rw-rw-rw-   0        0        0    65511 2023-06-03 08:01:41.000000 FunPayAPI-1.0.9/FunPayAPI/account.py
+drwxrwxrwx   0        0        0        0 2023-06-03 08:08:18.668286 FunPayAPI-1.0.9/FunPayAPI/common/
+-rw-rw-rw-   0        0        0        0 2023-05-12 17:46:25.000000 FunPayAPI-1.0.9/FunPayAPI/common/__init__.py
+-rw-rw-rw-   0        0        0     4842 2023-05-14 16:49:23.000000 FunPayAPI-1.0.9/FunPayAPI/common/enums.py
+-rw-rw-rw-   0        0        0     7842 2023-05-14 23:54:13.000000 FunPayAPI-1.0.9/FunPayAPI/common/exceptions.py
+-rw-rw-rw-   0        0        0     8922 2023-05-19 09:07:17.000000 FunPayAPI-1.0.9/FunPayAPI/common/utils.py
+-rw-rw-rw-   0        0        0    38978 2023-05-19 09:36:22.000000 FunPayAPI-1.0.9/FunPayAPI/types.py
+drwxrwxrwx   0        0        0        0 2023-06-03 08:08:18.673286 FunPayAPI-1.0.9/FunPayAPI/updater/
+-rw-rw-rw-   0        0        0        0 2023-05-12 17:46:18.000000 FunPayAPI-1.0.9/FunPayAPI/updater/__init__.py
+-rw-rw-rw-   0        0        0     8216 2023-05-11 19:12:41.000000 FunPayAPI-1.0.9/FunPayAPI/updater/events.py
+-rw-rw-rw-   0        0        0    22148 2023-06-03 06:55:19.000000 FunPayAPI-1.0.9/FunPayAPI/updater/runner.py
+drwxrwxrwx   0        0        0        0 2023-06-03 08:08:18.657286 FunPayAPI-1.0.9/FunPayAPI.egg-info/
+-rw-rw-rw-   0        0        0     3602 2023-06-03 08:08:18.000000 FunPayAPI-1.0.9/FunPayAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-03 08:08:18.000000 FunPayAPI-1.0.9/FunPayAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 08:08:18.000000 FunPayAPI-1.0.9/FunPayAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-03 08:08:18.000000 FunPayAPI-1.0.9/FunPayAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-03 08:08:18.000000 FunPayAPI-1.0.9/FunPayAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35801 2023-05-11 21:13:41.000000 FunPayAPI-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3602 2023-06-03 08:08:18.673286 FunPayAPI-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3011 2023-05-12 11:49:15.000000 FunPayAPI-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-03 08:08:18.674287 FunPayAPI-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      928 2023-06-03 08:07:47.000000 FunPayAPI-1.0.9/setup.py
```

### Comparing `FunPayAPI-1.0.8/FunPayAPI/account.py` & `FunPayAPI-1.0.9/FunPayAPI/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,17 @@
 
         self.__subcategories: list[types.SubCategory] = []
         self.__sorted_subcategories: dict[types.SubCategoryTypes, dict[int, types.SubCategory]] = {
             types.SubCategoryTypes.COMMON: {},
             types.SubCategoryTypes.CURRENCY: {}
         }
 
+        self.__bot_character = "⁤"
+        """Если сообщение начинается с этого символа, значит оно отправлено ботом."""
+
     def method(self, request_method: Literal["post", "get"], api_method: str, headers: dict, payload: Any,
                exclude_phpsessid: bool = False, raise_not_200: bool = False) -> requests.Response:
         """
         Отправляет запрос к FunPay. Добавляет в заголовки запроса user_agent и куки.
 
         :param request_method: метод запроса ("get" / "post").
         :type request_method: :obj:`str` `post` or `get`
@@ -159,14 +162,62 @@
             self.__setup_categories(html_response)
 
         self.last_update = int(time.time())
         self.html = html_response
         self.__initiated = True
         return self
 
+    def get_subcategory_public_lots(self, subcategory_type: enums.SubCategoryTypes, subcategory_id: int) -> list[types.LotShortcut]:
+        """
+        Получает список всех опубликованных лотов переданной подкатегории.
+
+        :param subcategory_type: тип подкатегории.
+        :type subcategory_type: :class:`FunPayAPI.enums.SubCategoryTypes`
+
+        :param subcategory_id: ID подкатегории.
+        :type subcategory_id: :obj:`int`
+
+        :return: список всех опубликованных лотов переданной подкатегории.
+        :rtype: :obj:`list` of :class:`FunPayAPI.types.LotShortcut`
+        """
+        if not self.is_initiated:
+            raise exceptions.AccountNotInitiatedError()
+
+        meth = f"lots/{subcategory_id}/" if subcategory_type is enums.SubCategoryTypes.COMMON else f"chips/{subcategory_id}/"
+        response = self.method("get", meth, {"accept": "*/*"}, {}, raise_not_200=True)
+        html_response = response.content.decode()
+        parser = BeautifulSoup(html_response, "html.parser")
+
+        username = parser.find("div", {"class": "user-link-name"})
+        if not username:
+            raise exceptions.UnauthorizedError(response)
+
+        offers = parser.find_all("a", {"class": "tc-item"})
+        if not offers:
+            return []
+
+        subcategory_obj = self.get_subcategory(subcategory_type, subcategory_id)
+        result = []
+        for offer in offers:
+            offer_id = offer["href"].split("id=")[1]
+            description = offer.find("div", {"class": "tc-desc-text"})
+            description = description.text if description else None
+            server = offer.find("div", {"class": "tc-server hidden-xxs"})
+            if not server:
+                server = offer.find("div", {"class": "tc-server hidden-xs"})
+            server = server.text if server else None
+
+            if subcategory_type is types.SubCategoryTypes.COMMON:
+                price = float(offer.find("div", {"class": "tc-price"})["data-s"])
+            else:
+                price = float(offer.find("div", {"class": "tc-price"}).find("div").text.split()[0])
+            lot_obj = types.LotShortcut(offer_id, server, description, price, subcategory_obj, str(offer))
+            result.append(lot_obj)
+        return result
+
     def get_balance(self, lot_id: int = 18853876) -> types.Balance:
         """
         Получает информацию о балансе пользователя.
 
         :param lot_id: ID лота, на котором проверять баланс.
         :type lot_id: :obj:`int`, опционально
 
@@ -365,15 +416,15 @@
             "data": {"node": chat_id, "last_message": -1, "content": text}
         }
 
         if image_id is not None:
             request["data"]["image_id"] = image_id
             request["data"]["content"] = ""
         else:
-            request["data"]["content"] = text or ""
+            request["data"]["content"] = f"{self.__bot_character}{text}" if text else ""
 
         objects = [
             {
                 "type": "chat_node",
                 "id": chat_id,
                 "tag": "00000000",
                 "data": {"node": chat_id, "last_message": -1, "content": ""}
@@ -396,22 +447,22 @@
         mes = json_response["objects"][0]["data"]["messages"][-1]
         parser = BeautifulSoup(mes["html"], "html.parser")
         try:
             if image_link := parser.find("a", {"class": "chat-img-link"}):
                 image_link = image_link.get("href")
                 message_text = None
             else:
-                message_text = parser.find("div", {"class": "message-text"}).text
+                message_text = parser.find("div", {"class": "message-text"}).text.replace(self.__bot_character, "", 1)
         except Exception as e:
             logger.debug("SEND_MESSAGE RESPONSE")
             logger.debug(response.content.decode())
             raise e
 
-        message_obj = types.Message(int(mes["id"]), message_text, chat_id, chat_name,
-                                    self.username, self.id, mes["html"], image_link)
+        message_obj = types.Message(int(mes["id"]), message_text, chat_id, chat_name, self.username, self.id,
+                                    mes["html"], image_link)
         if self.runner and isinstance(chat_id, int):
             if add_to_ignore_list:
                 self.runner.mark_as_by_bot(chat_id, message_obj.id)
             if update_last_saved_message:
                 self.runner.update_last_message(chat_id, message_text)
         return message_obj
 
@@ -1323,23 +1374,34 @@
             else:
                 image_link = None
                 if author_id == 0:
                     message_text = parser.find("div", {"class": "alert alert-with-icon alert-info"}).text.strip()
                 else:
                     message_text = parser.find("div", {"class": "message-text"}).text
 
+            by_bot = False
+            if message_text.startswith(self.__bot_character):
+                message_text = message_text.replace(self.__bot_character, "", 1)
+                by_bot = True
+
             message_obj = types.Message(i["id"], message_text, chat_id, interlocutor_username,
                                         None, author_id, i["html"], image_link, determine_msg_type=False)
+            message_obj.by_bot = by_bot
+
             if author_id != 0:
                 message_obj.type = types.MessageTypes.NON_SYSTEM
             else:
                 message_obj.type = message_obj.get_message_type()
             messages.append(message_obj)
 
         # todo
         debug_text = ""
         for i in messages:
             i.author = ids.get(i.author_id)
             i.chat_name = interlocutor_username
             debug_text += f"{i.author} | {i.author_id} | {str(i)[:20]} /\\"
         logger.debug(debug_text)
         return messages
+
+    @property
+    def bot_character(self) -> str:
+        return self.__bot_character
```

### Comparing `FunPayAPI-1.0.8/FunPayAPI/common/enums.py` & `FunPayAPI-1.0.9/FunPayAPI/common/enums.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.8/FunPayAPI/common/exceptions.py` & `FunPayAPI-1.0.9/FunPayAPI/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.8/FunPayAPI/common/utils.py` & `FunPayAPI-1.0.9/FunPayAPI/common/utils.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.8/FunPayAPI/types.py` & `FunPayAPI-1.0.9/FunPayAPI/types.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.8/FunPayAPI/updater/events.py` & `FunPayAPI-1.0.9/FunPayAPI/updater/events.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.8/FunPayAPI/updater/runner.py` & `FunPayAPI-1.0.9/FunPayAPI/updater/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from __future__ import annotations
+
+import re
 from typing import TYPE_CHECKING, Generator
 if TYPE_CHECKING:
     from ..account import Account
 
 import json
 import logging
 from bs4 import BeautifulSoup
@@ -53,25 +55,33 @@
 
         self.__first_request = True
         self.__last_msg_event_tag = utils.random_tag()
         self.__last_order_event_tag = utils.random_tag()
 
         self.saved_orders: dict[str, types.OrderShortcut] = {}
         """Сохраненные состояния заказов ({ID заказа: экземпляр types.OrderShortcut})."""
-        self.last_messages: dict[int, str] = {}
-        """ID последний сообщений ({ID чата: текст сообщения (до 250 символов)})."""
+
+        self.last_messages: dict[int, list[str, str | None]] = {}
+        """ID последний сообщений ({ID чата: (текст сообщения (до 250 символов), время сообщения)})."""
+
+        self.init_messages: dict[int, str] = {}
+        """Текста инит. чатов (для generate_new_message_events)."""
+
         self.by_bot_ids: dict[int, list[int]] = {}
         """ID сообщений, отправленных с помощью self.account.send_message ({ID чата: [ID сообщения, ...]})."""
+
         self.last_messages_ids: dict[int, int] = {}
         """ID последних сообщений в чатах ({ID чата: ID последнего сообщения})."""
 
         self.account: Account = account
         """Экземпляр аккаунта, к которому привязан Runner."""
         self.account.runner = self
 
+        self.__msg_time_re = re.compile(r"\d{2}:\d{2}")
+
     def get_updates(self) -> dict:
         """
         Запрашивает список событий FunPay.
 
         :return: ответ FunPay.
         :rtype: :obj:`dict`
         """
@@ -149,31 +159,47 @@
         """
         events, lcmc_events = [], []
         self.__last_msg_event_tag = obj.get("tag")
         parser = BeautifulSoup(obj["data"]["html"], "html.parser")
         chats = parser.find_all("a", {"class": "contact-item"})
 
         # Получаем все изменившиеся чаты
-        for msg in chats:
-            chat_id = int(msg["data-id"])
-            last_msg_text = msg.find("div", {"class": "contact-item-message"})
-            if not last_msg_text:
+        for chat in chats:
+            chat_id = int(chat["data-id"])
+            # Если чат удален админами - скип.
+            if not (last_msg_text := chat.find("div", {"class": "contact-item-message"})):
                 continue
+
             last_msg_text = last_msg_text.text
-            if self.last_messages.get(chat_id) == last_msg_text:
-                continue
-            unread = True if "unread" in msg.get("class") else False
-            chat_with = msg.find("div", {"class": "media-user-name"}).text
-            chat_obj = types.ChatShortcut(chat_id, chat_with, last_msg_text, unread, str(msg))
+            if last_msg_text.startswith(self.account.bot_character):
+                last_msg_text = last_msg_text.replace(self.account.bot_character, "", 1)
+            last_msg_time = chat.find("div", {"class": "contact-item-time"}).text
+
+            # Если текст последнего сообщения совпадает с сохраненным
+            if chat_id in self.last_messages and self.last_messages[chat_id][0] == last_msg_text:
+                # Если есть сохраненное время сообщения для данного чата
+                if self.last_messages[chat_id][1]:
+                    # Если время ласт сообщения не имеет формат ЧЧ:ММ или совпадает с сохраненным - скип чата
+                    if not self.__msg_time_re.fullmatch(last_msg_time) or self.last_messages[chat_id][1] == last_msg_time:
+                        continue
+                # Если нет сохраненного времени сообщения для данного чата - скип чата
+                else:
+                    continue
+
+            unread = True if "unread" in chat.get("class") else False
+            chat_with = chat.find("div", {"class": "media-user-name"}).text
+            chat_obj = types.ChatShortcut(chat_id, chat_with, last_msg_text, unread, str(chat))
             self.account.add_chats([chat_obj])
-            self.last_messages[chat_id] = last_msg_text
+            self.last_messages[chat_id] = [last_msg_text, last_msg_time]
 
             if self.__first_request:
                 events.append(InitialChatEvent(self.__last_msg_event_tag, chat_obj))
+                self.init_messages[chat_id] = last_msg_text
                 continue
+
             lcmc_events.append(LastChatMessageChangedEvent(self.__last_msg_event_tag, chat_obj))
 
         if lcmc_events:
             events.append(ChatsListChangedEvent(self.__last_msg_event_tag))
 
         if not self.make_msg_requests:
             events.extend(lcmc_events)
@@ -201,67 +227,71 @@
         :return: словарь с событиями новых сообщений в формате {ID чата: [список событий]}
         :rtype: :obj:`dict` {:obj:`int`: :obj:`list` of :class:`FunPayAPI.updater.events.NewMessageEvent`}
         """
         attempts = 3
         while attempts:
             attempts -= 1
             try:
-                chats_messages = self.account.get_chats_histories(chats_data)
+                chats = self.account.get_chats_histories(chats_data)
                 break
             except exceptions.RequestFailedError as e:
                 logger.error(e)
             except:
                 logger.error(f"Не удалось получить истории чатов {list(chats_data.keys())}.")
                 logger.debug("TRACEBACK", exc_info=True)
             time.sleep(1)
         else:
             logger.error(f"Не удалось получить истории чатов {list(chats_data.keys())}: превышено кол-во попыток.")
             return {}
 
         result = {}
-        for chat_id in chats_messages:
-            messages = chats_messages[chat_id]
-            result[chat_id] = []
-            self.by_bot_ids[chat_id] = [] if not self.by_bot_ids.get(chat_id) else self.by_bot_ids[chat_id]
+
+        for cid in chats:
+            messages = chats[cid]
+            result[cid] = []
+            self.by_bot_ids[cid] = self.by_bot_ids.get(cid) or []
 
             # Удаляем все сообщения, у которых ID меньше сохраненного последнего сообщения
-            if self.last_messages_ids.get(chat_id):
-                messages = [i for i in messages if i.id > self.last_messages_ids[chat_id]]
+            if self.last_messages_ids.get(cid):
+                messages = [i for i in messages if i.id > self.last_messages_ids[cid]]
             if not messages:
                 continue
 
             # Отмечаем все сообщения, отправленные с помощью Account.send_message()
-            if self.by_bot_ids.get(chat_id):
+            if self.by_bot_ids.get(cid):
                 for i in messages:
-                    if i.id in self.by_bot_ids[chat_id]:
+                    if not i.by_bot and i.id in self.by_bot_ids[cid]:
                         i.by_bot = True
 
             stack = MessageEventsStack()
 
-            # если в runner'е нет сохраненного ID последнего сообщения, сохраняем ID последнего сообщения и возвращаем
-            # только 1 событие (нового последнего сообщения).
-            if not self.last_messages_ids.get(chat_id):
-                self.last_messages_ids[chat_id] = messages[-1].id  # Перезаписываем ID последнего сообщение
-                last_message = messages[-1]
-                event = NewMessageEvent(self.__last_msg_event_tag, last_message, stack)
-                stack.add_events([event])
-                result[chat_id] = [event]
-                # Чистим игнор. ID, которые меньше сохраненного ID последнего сообщения, дабы не забивать память.
-                self.by_bot_ids[chat_id] = [i for i in self.by_bot_ids[chat_id] if i >
-                                            self.last_messages_ids[chat_id]]
-                continue
+            # Если нет сохраненного ID последнего сообщения
+            if not self.last_messages_ids.get(cid):
+                # Если данный чат был доступен при первом запросе и есть сохраненное последнее сообщение,
+                # то ищем новые сообщения относительно последнего сохраненного текста
+                if init_msg_text := self.init_messages.get(cid):
+                    del self.init_messages[cid]
+                    temp = []
+                    for i in reversed(messages):
+                        if i.text[:250] == init_msg_text:
+                            break
+                        temp.append(i)
+                    messages = list(reversed(temp))
+
+                # Если данного чата не было при первом запросе, в результат добавляем только ласт сообщение истории.
+                else:
+                    messages = messages[-1:]
 
-            self.last_messages_ids[chat_id] = messages[-1].id  # Перезаписываем ID последнего сообщение
-            self.by_bot_ids[chat_id] = [i for i in self.by_bot_ids[chat_id] if i >
-                                        self.last_messages_ids[chat_id]]
+            self.last_messages_ids[cid] = messages[-1].id  # Перезаписываем ID последнего сообщение
+            self.by_bot_ids[cid] = [i for i in self.by_bot_ids[cid] if i > self.last_messages_ids[cid]]  # чистим память
 
             for msg in messages:
                 event = NewMessageEvent(self.__last_msg_event_tag, msg, stack)
                 stack.add_events([event])
-                result[chat_id].append(event)
+                result[cid].append(event)
         return result
 
     def parse_order_updates(self, obj) -> list[InitialOrderEvent | OrdersListChangedEvent | NewOrderEvent |
                                                OrderStatusChangedEvent]:
         """
         Парсит события, связанные с продажами.
 
@@ -310,27 +340,30 @@
                 self.update_order(order)
 
             elif order.status != self.saved_orders[order.id].status:
                 events.append(OrderStatusChangedEvent(self.__last_order_event_tag, order))
                 self.update_order(order)
         return events
 
-    def update_last_message(self, chat_id: int, message_text: str | None):
+    def update_last_message(self, chat_id: int, message_text: str | None, message_time: str | None = None):
         """
         Обновляет сохраненный текст последнего сообщения чата.
 
         :param chat_id: ID чата.
         :type chat_id: :obj:`int`
 
         :param message_text: текст сообщения (если `None`, заменяется за "Изображение").
         :type message_text: :obj:`str` or :obj:`None`
+
+        :param message_time: время отправки сообщения в формате ЧЧ:ММ. Используется исключительно Runner'ом.
+        :type message_time: :obj:`str` or :obj:`None`, опционально
         """
         if message_text is None:
             message_text = "Изображение"
-        self.last_messages[chat_id] = message_text[:250]
+        self.last_messages[chat_id] = [message_text[:250], message_time]
 
     def update_order(self, order: types.OrderShortcut):
         """
         Обновляет сохраненное состояние переданного заказа.
 
         :param order: экземпляр заказа, который нужно обновить.
         :type order: :class:`FunPayAPI.types.OrderShortcut`
```

### Comparing `FunPayAPI-1.0.8/FunPayAPI.egg-info/PKG-INFO` & `FunPayAPI-1.0.9/FunPayAPI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: FunPayAPI
-Version: 1.0.8
+Version: 1.0.9
 Summary: Прослойка между FunPayAPI и клиентом.
 Home-page: https://github.com/woopertail/FunPayAPI
 Author: Woopertail
 Author-email: woopertail@gmail.com
-License: GPL2
+License: GPL3
 Keywords: funpay bot api tools
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: FunPayAPI Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: FunPayAPI Version: 1.0.9 Summary:
 ÐÑÐ¾ÑÐ»Ð¾Ð¹ÐºÐ° Ð¼ÐµÐ¶Ð´Ñ FunPayAPI Ð¸ ÐºÐ»Ð¸ÐµÐ½ÑÐ¾Ð¼. Home-page: https:/
 /github.com/woopertail/FunPayAPI Author: Woopertail Author-email:
-woopertail@gmail.com License: GPL2 Keywords: funpay bot api tools Platform:
+woopertail@gmail.com License: GPL3 Keywords: funpay bot api tools Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python :: 3 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Description-Content-Type: text/markdown License-File: LICENSE [https://
 i.ibb.co/tJKk0QS/Fun-Pay-API-darkmode.png]
                            ****** FunPay API ******
  *** ÐÐ¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð´Ð»Ñ Ð»ÐµÐ³ÐºÐ¾Ð³Ð¾ Ð½Ð°Ð¿Ð¸ÑÐ°Ð½Ð¸Ñ Ð±Ð¾ÑÐ¾Ð²
```

### Comparing `FunPayAPI-1.0.8/LICENSE` & `FunPayAPI-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.8/PKG-INFO` & `FunPayAPI-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: FunPayAPI
-Version: 1.0.8
+Version: 1.0.9
 Summary: Прослойка между FunPayAPI и клиентом.
 Home-page: https://github.com/woopertail/FunPayAPI
 Author: Woopertail
 Author-email: woopertail@gmail.com
-License: GPL2
+License: GPL3
 Keywords: funpay bot api tools
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: FunPayAPI Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: FunPayAPI Version: 1.0.9 Summary:
 ÐÑÐ¾ÑÐ»Ð¾Ð¹ÐºÐ° Ð¼ÐµÐ¶Ð´Ñ FunPayAPI Ð¸ ÐºÐ»Ð¸ÐµÐ½ÑÐ¾Ð¼. Home-page: https:/
 /github.com/woopertail/FunPayAPI Author: Woopertail Author-email:
-woopertail@gmail.com License: GPL2 Keywords: funpay bot api tools Platform:
+woopertail@gmail.com License: GPL3 Keywords: funpay bot api tools Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python :: 3 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Description-Content-Type: text/markdown License-File: LICENSE [https://
 i.ibb.co/tJKk0QS/Fun-Pay-API-darkmode.png]
                            ****** FunPay API ******
  *** ÐÐ¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð´Ð»Ñ Ð»ÐµÐ³ÐºÐ¾Ð³Ð¾ Ð½Ð°Ð¿Ð¸ÑÐ°Ð½Ð¸Ñ Ð±Ð¾ÑÐ¾Ð²
```

### Comparing `FunPayAPI-1.0.8/README.md` & `FunPayAPI-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.8/setup.py` & `FunPayAPI-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_desc = f.read()
 
 
 setup(name='FunPayAPI',
-      version="1.0.8",
+      version="1.0.9",
       description='Прослойка между FunPayAPI и клиентом.',
       long_description=long_desc,
       long_description_content_type="text/markdown",
       author='Woopertail',
       author_email='woopertail@gmail.com',
       url='https://github.com/woopertail/FunPayAPI',
       packages=find_packages("."),
-      license='GPL2',
+      license='GPL3',
       keywords='funpay bot api tools',
       install_requires=['requests==2.28.1', 'beautifulsoup4', 'requests_toolbelt==0.10.1'],
       classifiers=[
           'Development Status :: 5 - Production/Stable',
           'Programming Language :: Python :: 3',
           'Environment :: Console',
           'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
```

