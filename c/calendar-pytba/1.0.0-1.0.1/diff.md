# Comparing `tmp/calendar_pytba-1.0.0.tar.gz` & `tmp/calendar_pytba-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendar_pytba-1.0.0.tar", max compression
+gzip compressed data, was "calendar_pytba-1.0.1.tar", max compression
```

## Comparing `calendar_pytba-1.0.0.tar` & `calendar_pytba-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-06-03 07:19:21.340893 calendar_pytba-1.0.0/LICENSE
--rw-r--r--   0        0        0      375 2023-06-03 08:41:26.115192 calendar_pytba-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       41 2023-06-03 07:48:53.714950 calendar_pytba-1.0.0/pytba_calendar/__init__.py
--rw-r--r--   0        0        0     6995 2023-06-03 08:08:08.707580 calendar_pytba-1.0.0/pytba_calendar/main.py
--rw-r--r--   0        0        0        0 2023-06-03 07:22:55.353512 calendar_pytba-1.0.0/pytba_calendar/utils/__init__.py
--rw-r--r--   0        0        0     3944 2023-06-02 15:56:03.774911 calendar_pytba-1.0.0/pytba_calendar/utils/handler.py
--rw-r--r--   0        0        0     2315 2023-06-03 07:06:22.851772 calendar_pytba-1.0.0/pytba_calendar/utils/text.py
--rw-r--r--   0        0        0      444 2023-06-02 16:26:52.379094 calendar_pytba-1.0.0/pytba_calendar/utils/types.py
--rw-r--r--   0        0        0      399 2023-06-03 07:17:23.804405 calendar_pytba-1.0.0/readme.md
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 calendar_pytba-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-03 09:21:07.424210 calendar_pytba-1.0.1/LICENSE
+-rw-r--r--   0        0        0       41 2023-06-03 09:21:07.424210 calendar_pytba-1.0.1/calendar_pytba/__init__.py
+-rw-r--r--   0        0        0     6995 2023-06-03 09:21:07.424210 calendar_pytba-1.0.1/calendar_pytba/main.py
+-rw-r--r--   0        0        0        0 2023-06-03 09:21:07.424210 calendar_pytba-1.0.1/calendar_pytba/utils/__init__.py
+-rw-r--r--   0        0        0     3944 2023-06-03 09:21:07.424210 calendar_pytba-1.0.1/calendar_pytba/utils/handler.py
+-rw-r--r--   0        0        0     2315 2023-06-03 09:21:07.424210 calendar_pytba-1.0.1/calendar_pytba/utils/text.py
+-rw-r--r--   0        0        0      444 2023-06-03 09:21:07.424210 calendar_pytba-1.0.1/calendar_pytba/utils/types.py
+-rw-r--r--   0        0        0      374 2023-06-03 09:21:07.444210 calendar_pytba-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      662 2023-06-03 09:21:07.444210 calendar_pytba-1.0.1/readme.md
+-rw-r--r--   0        0        0     1056 1970-01-01 00:00:00.000000 calendar_pytba-1.0.1/PKG-INFO
```

### Comparing `calendar_pytba-1.0.0/LICENSE` & `calendar_pytba-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `calendar_pytba-1.0.0/pytba_calendar/main.py` & `calendar_pytba-1.0.1/calendar_pytba/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import calendar
 import datetime
 
 from dateutil.relativedelta import relativedelta
 from telebot import types  # noqa
 
-from pytba_calendar.utils import text
-from pytba_calendar.utils.types import CalendarLanguage, CallBackData
+from calendar_pytba.utils import text
+from calendar_pytba.utils.types import CalendarLanguage, CallBackData
 
 
 class Calendar:
     def __init__(
         self,
         language: str = CalendarLanguage.EN,
         empty_day_symbol: str = " ",
@@ -19,15 +19,15 @@
         week_days_names: dict = text.WEEK_DAYS_NAMES,
         week_days_short_names: dict = text.WEEK_DAYS_SHORT_NAMES,
     ):
         """
         The language is responsible for writing the names of the months,
         days of the week, and other elements of the calendar.
         You can pass the language value as a string, see available
-        languages in pytba_calendar.utils.types.CalendarLanguage
+        languages in calendar_pytba.utils.types.CalendarLanguage
         :param language: str, CalendarLanguage class attribute
         :param empty_day_symbol: str, character to be displayed on days of the week where there are no numbers
         :param next_page_symbol: str, scroll forward button symbol
         :param previous_page_symbol: str, scroll backward button symbol
         :param month_names: dict, dictionary with the names of the months
         :param week_days_names: dict, dictionary with the names of the weekdays
         :param week_days_short_names: dict, dictionary with the short names of the weekdays
```

### Comparing `calendar_pytba-1.0.0/pytba_calendar/utils/handler.py` & `calendar_pytba-1.0.1/calendar_pytba/utils/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 
 from telebot import TeleBot, types
 
-from pytba_calendar import Calendar
-from pytba_calendar.utils import text
-from pytba_calendar.utils.types import CalendarLanguage, CallBackData
+from calendar_pytba import Calendar
+from calendar_pytba.utils import text
+from calendar_pytba.utils.types import CalendarLanguage, CallBackData
 
 
 def _extract_month_year(data: str) -> list:
     return [int(_) for _ in data.split(":")[1:3]]
 
 
 def callback_handler(bot: TeleBot, language: str = CalendarLanguage.EN):
```

### Comparing `calendar_pytba-1.0.0/pytba_calendar/utils/text.py` & `calendar_pytba-1.0.1/calendar_pytba/utils/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pytba_calendar.utils.types import CalendarLanguage
+from calendar_pytba.utils.types import CalendarLanguage
 
 MONTH_NAMES = {
     CalendarLanguage.EN: {
         1: "January",
         2: "February",
         3: "March",
         4: "April",
```

