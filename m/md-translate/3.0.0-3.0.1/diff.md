# Comparing `tmp/md_translate-3.0.0.tar.gz` & `tmp/md_translate-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md_translate-3.0.0.tar", max compression
+gzip compressed data, was "md_translate-3.0.1.tar", max compression
```

## Comparing `md_translate-3.0.0.tar` & `md_translate-3.0.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-06-02 10:39:28.552558 md_translate-3.0.0/LICENSE
--rw-r--r--   0        0        0     3503 2023-06-02 10:39:28.552558 md_translate-3.0.0/README.md
--rw-r--r--   0        0        0        0 2023-06-02 10:39:28.552558 md_translate-3.0.0/md_translate/__init__.py
--rw-r--r--   0        0        0     4198 2023-06-02 10:39:28.552558 md_translate-3.0.0/md_translate/application.py
--rw-r--r--   0        0        0      230 2023-06-02 10:39:28.552558 md_translate-3.0.0/md_translate/document/__init__.py
--rw-r--r--   0        0        0     6485 2023-06-02 10:39:28.552558 md_translate-3.0.0/md_translate/document/blocks.py
--rw-r--r--   0        0        0     5960 2023-06-02 10:39:28.552558 md_translate-3.0.0/md_translate/document/document.py
--rw-r--r--   0        0        0     3654 2023-06-02 10:39:28.552558 md_translate-3.0.0/md_translate/document/parser.py
--rw-r--r--   0        0        0      763 2023-06-02 10:39:28.552558 md_translate-3.0.0/md_translate/main.py
--rw-r--r--   0        0        0      157 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/settings/__init__.py
--rw-r--r--   0        0        0     4683 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/settings/_base_settings.py
--rw-r--r--   0        0        0     2687 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/settings/_settings_to_cli.py
--rw-r--r--   0        0        0      439 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/__init__.py
--rw-r--r--   0        0        0      650 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/_base_translator.py
--rw-r--r--   0        0        0     4960 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/_selenium_base.py
--rw-r--r--   0        0        0     1559 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/bing.py
--rw-r--r--   0        0        0     2089 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/deepl.py
--rw-r--r--   0        0        0     1812 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/google.py
--rw-r--r--   0        0        0        0 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/randomizer/__init__.py
--rw-r--r--   0        0        0     6618 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/randomizer/const.py
--rw-r--r--   0        0        0     1107 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/randomizer/randomizer.py
--rw-r--r--   0        0        0     1660 2023-06-02 10:39:28.556558 md_translate-3.0.0/md_translate/translators/yandex.py
--rw-r--r--   0        0        0     2179 2023-06-02 10:39:28.556558 md_translate-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     4791 1970-01-01 00:00:00.000000 md_translate-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-03 19:58:43.303453 md_translate-3.0.1/LICENSE
+-rw-r--r--   0        0        0     5353 2023-06-03 19:58:43.303453 md_translate-3.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/__init__.py
+-rw-r--r--   0        0        0     4457 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/application.py
+-rw-r--r--   0        0        0      230 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/document/__init__.py
+-rw-r--r--   0        0        0     6485 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/document/blocks.py
+-rw-r--r--   0        0        0     5960 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/document/document.py
+-rw-r--r--   0        0        0     3654 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/document/parser.py
+-rw-r--r--   0        0        0      905 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/exceptions.py
+-rw-r--r--   0        0        0      737 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/main.py
+-rw-r--r--   0        0        0      157 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/settings/__init__.py
+-rw-r--r--   0        0        0     5909 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/settings/_base_settings.py
+-rw-r--r--   0        0        0     2687 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/settings/_settings_to_cli.py
+-rw-r--r--   0        0        0      439 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/__init__.py
+-rw-r--r--   0        0        0      687 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/_base_translator.py
+-rw-r--r--   0        0        0     4960 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/_selenium_base.py
+-rw-r--r--   0        0        0     1517 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/bing.py
+-rw-r--r--   0        0        0     2059 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/deepl.py
+-rw-r--r--   0        0        0     1839 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/google.py
+-rw-r--r--   0        0        0        0 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/randomizer/__init__.py
+-rw-r--r--   0        0        0     6618 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/randomizer/const.py
+-rw-r--r--   0        0        0     1107 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/randomizer/randomizer.py
+-rw-r--r--   0        0        0     1675 2023-06-03 19:58:43.303453 md_translate-3.0.1/md_translate/translators/yandex.py
+-rw-r--r--   0        0        0     2214 2023-06-03 19:58:43.303453 md_translate-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6599 1970-01-01 00:00:00.000000 md_translate-3.0.1/PKG-INFO
```

### Comparing `md_translate-3.0.0/LICENSE` & `md_translate-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.0/README.md` & `md_translate-3.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Markdown Docs Translator
 
 ![Python](https://img.shields.io/badge/python-v3.10+-blue.svg)
 ![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)
 
-Markdown Docs Translator is an automated translator for markdown documents, built with Python. The tool supports multiple translation services and provides a variety of options to customize the translation process.
+Markdown Docs Translator is an automated translator for Markdown documents, built with Python. The tool supports multiple translation services and provides a variety of options to customize the translation process.
 
 ## Features
 
 - Support for multiple translation services (Yandex, Google, Bing, Deepl).
 - Multithreading for faster translations.
 - Options to overwrite original files, drop original files, or create a new file with translated text.
 - Caching for faster repeat translations.
@@ -43,42 +43,42 @@
 - `source_lang` is the language code of the source document.
 - `target_lang` is the language code for the translation.
 - `service` is the translating service to use (yandex, google, bing, deepl).
 - `OPTIONS` are additional options that can be specified as listed below.
 
 ### Options
 
-| Option                        | Description                          |
-| ----------------------------- | ------------------------------------ |
-| `-F, --from-lang TEXT`        | Source language code \[required\]    |
-| `-T, --to-lang TEXT`          | Target language code \[required\]    |
-| `-P, --service`               | Translating service \[required\]     |
-| `-X, --processes INTEGER`     | Number of processes to use           |
-| `-N, --new-file`              | Create new file with translated text |
-| `-I, --ignore-cache`          | Ignore cache                         |
-| `-S, --save-temp-on-complete` | Save temporary files on complete     |
-| `-O, --overwrite`             | Overwrite original files             |
-| `-V, --verbose`               | Verbosity level                      |
-| `-D, --drop-original`         | Drop original files                  |
-| `--help`                      | Show help message and exit           |
+| Option                        | Description                                                                                                                                                                        |
+| ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `-F, --from-lang TEXT`        | Source language code \[required\]                                                                                                                                                  |
+| `-T, --to-lang TEXT`          | Target language code \[required\]                                                                                                                                                  |
+| `-P, --service`               | Translating service \[required\]                                                                                                                                                   |
+| `-X, --processes INTEGER`     | Number of processes to use. Will be applied to each file separately                                                                                                                |
+| `-N, --new-file`              | Create a new file with translated text (original file will remain unchanged). The new file will be created in the same directory as the original file with a "\_translated" suffix |
+| `-I, --ignore-cache`          | Ignore cache files. If cache exists, it will be overwritten                                                                                                                        |
+| `-S, --save-temp-on-complete` | Save cache files upon completion. If not set, they will be deleted                                                                                                                 |
+| `-O, --overwrite`             | Already translated files will be overwritten. Otherwise, these files will be skipped                                                                                               |
+| `-D, --drop-original`         | Remove original lines from translated file. These lines will be replaced with translated ones                                                                                      |
+| `-V, --verbose`               | Verbosity level                                                                                                                                                                    |
+| `--help`                      | Show help message and exit                                                                                                                                                         |
 
 Currently supported services are:
 
 - `Yandex`
 - `Google`
 - `Bing`
 - `Deepl`
 
 ### Configuring with a Configuration File
 
 Options for the application can be defined through a configuration file as well. This file should be named `settings.json` and is typically located at `~/.config/md_translate`.
 
 If you choose to use a non-default location for the config file, you can specify its path using the `--config` or `-C` option.
 
-This configuration file can encompass all CLI options with the exception of `path`, `from_lang`, `to_lang`, and `service`. These particular options need to be stated directly in the CLI.
+This configuration file can encompass all CLI options except `path`, `from_lang`, `to_lang`, `service` and `config_file_path`. These particular options need to be stated directly in the CLI.
 
 The configuration file should be a valid JSON file and adhere to the following structure:
 
 ```json
 {
     "processes": 4,
     "new_file": true,
```

### Comparing `md_translate-3.0.0/md_translate/application.py` & `md_translate-3.0.1/md_translate/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import multiprocessing
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import click
 
 from md_translate.document import MarkdownDocument
+from md_translate.exceptions import NoMdFilesFound, NoTargetFileFound
 
 if TYPE_CHECKING:
     from md_translate.settings import Settings
 
 
 class Application:
     def __init__(self, settings: 'Settings'):
@@ -53,37 +54,24 @@
             'urllib3',
             'WDM',
         ]
         for logger_name in LOGGER_NAMES_TO_DISABLE:
             logging.getLogger(logger_name).setLevel(logging.CRITICAL)
 
     def _get_files_to_process(self) -> list[Path]:
-        path = self._settings.path
-
-        if not isinstance(path, list):
-            path = [path]
-        files_to_process = []
-        for path_to_process in path:
-            if not path_to_process.exists():
-                raise click.ClickException(f'Path not found: {path_to_process}')
-            if path_to_process.is_file():
-                self._logger.debug('Found file: %s', path_to_process)
-                files_to_process.append(path_to_process)
-            else:
-                found_files = path_to_process.glob('**/*.md')
-                for found_file in found_files:
-                    self._logger.debug('Found file: %s', found_file)
-                    files_to_process.append(found_file)
-
+        files_to_process = self._aggregate_files_to_process()
         source_files = [
             file_to_process
             for file_to_process in files_to_process
             if '_translated' not in file_to_process.name
         ]
 
+        if not source_files:
+            raise NoMdFilesFound('No markdown files found to process')
+
         common_path_part = Path(
             *(
                 part
                 for part in source_files[0].parts
                 if all(part in file.parts for file in source_files)
             )
         )
@@ -91,25 +79,41 @@
         self._logger.info(
             'Found %s files to process: %s',
             len(source_files),
             ', '.join([str(f.relative_to(common_path_part)) for f in source_files]),
         )
         return source_files
 
+    def _aggregate_files_to_process(self) -> list[Path]:
+        paths = self._settings.path
+        files_to_process = []
+        for path_to_process in paths:
+            if not path_to_process.exists():
+                raise NoTargetFileFound(f'Path not found: {path_to_process}')
+            if path_to_process.is_file():
+                self._logger.debug('Found file: %s', path_to_process)
+                files_to_process.append(path_to_process)
+            else:
+                found_files = path_to_process.glob('**/*.md')
+                for found_file in found_files:
+                    self._logger.debug('Found file: %s', found_file)
+                    files_to_process.append(found_file)
+        return files_to_process
+
     def process_file(self, file_to_process: Path) -> None:
         translation_provider = self._settings.service_provider(self._settings)
         self._logger.info('Processing file: %s', file_to_process)
         try:
             document = MarkdownDocument.from_file(
                 file_to_process,
                 settings=self._settings,
             )
         except Exception as e:
             self._logger.error('Error processing file: %s', file_to_process)
-            self._logger.error(e)
+            self._logger.exception(e)
             return
         if not document.should_be_translated():
             self._logger.info('Skipping file: %s. Already translated', file_to_process.name)
             return
         with translation_provider as provider:
             try:
                 document.translate(provider)
```

### Comparing `md_translate-3.0.0/md_translate/document/blocks.py` & `md_translate-3.0.1/md_translate/document/blocks.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.0/md_translate/document/document.py` & `md_translate-3.0.1/md_translate/document/document.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.0/md_translate/document/parser.py` & `md_translate-3.0.1/md_translate/document/parser.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.0/md_translate/main.py` & `md_translate-3.0.1/md_translate/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,13 +18,12 @@
     **cli_arguments: Any,
 ) -> None:
     dump_config = cli_arguments.pop('dump_config', False)
     config_file = cli_arguments.pop('config', None)
     settings = Settings.initiate(click_params=cli_arguments, config_file_path=config_file)
     if dump_config:
         settings.dump_settings()
-    exit_code = Application(settings).run()
-    exit(exit_code)
+    exit(Application(settings).run())
 
 
 if __name__ == "__main__":
     main()  # pragma: no cover
```

### Comparing `md_translate-3.0.0/md_translate/settings/_settings_to_cli.py` & `md_translate-3.0.1/md_translate/settings/_settings_to_cli.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.0/md_translate/translators/_selenium_base.py` & `md_translate-3.0.1/md_translate/translators/_selenium_base.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.0/md_translate/translators/bing.py` & `md_translate-3.0.1/md_translate/translators/bing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.remote.webelement import WebElement
 
+from md_translate.exceptions import safe_run
+
 from ._selenium_base import SeleniumBaseTranslator
 
 
 class BingTranslateProvider(SeleniumBaseTranslator):
     HOST = 'https://www.bing.com/translator/'
 
     def get_url(self) -> str:
@@ -16,29 +18,23 @@
 
     def get_input_element(self) -> WebElement:
         return self._driver.find_element(by=self.WEBDRIVER_BY.ID, value='tta_input_ta')
 
     def get_output_element(self) -> WebElement:
         return self._driver.find_element(by=self.WEBDRIVER_BY.ID, value='tta_output_ta')
 
+    @safe_run(NoSuchElementException, default_return_value=False)
     def check_for_translation(self) -> bool:
-        try:
-            container = self._driver.find_element(by=self.WEBDRIVER_BY.ID, value='rich_tta')
-            if 'ttastable' in container.get_attribute('class'):
-                return True
-            return False
-        except NoSuchElementException:
-            return False
+        container = self._driver.find_element(by=self.WEBDRIVER_BY.ID, value='rich_tta')
+        return 'ttastable' in container.get_attribute('class')
 
     def accept_cookies(self) -> None:
         self.click_cookies_accept('Accept')
 
+    @safe_run(NoSuchElementException, default_return_value=False)
     def check_for_antispam(self) -> bool:
-        try:
-            container = self._driver.find_element(by=self.WEBDRIVER_BY.ID, value='t_enter_captcha')
-            return container.is_displayed()
-        except NoSuchElementException:
-            return False
+        container = self._driver.find_element(by=self.WEBDRIVER_BY.ID, value='t_enter_captcha')
+        return container.is_displayed()
 
     @staticmethod
     def get_translated_data(output_element: WebElement) -> str:
         return output_element.get_attribute('value')
```

### Comparing `md_translate-3.0.0/md_translate/translators/deepl.py` & `md_translate-3.0.1/md_translate/translators/deepl.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.remote.webelement import WebElement
 
+from md_translate.exceptions import safe_run
+
 from ._selenium_base import SeleniumBaseTranslator
 
 
 class DeeplTranslateProvider(SeleniumBaseTranslator):
     HOST = 'https://www.deepl.com/translator/'
 
     TRANSLATION_TIMEOUT = 30
@@ -20,40 +22,34 @@
 
     def get_output_element(self) -> WebElement:
         return self._driver.find_element(
             by=self.WEBDRIVER_BY.CSS_SELECTOR,
             value='[data-testid="translator-target-input"]',
         )
 
+    @safe_run(NoSuchElementException, default_return_value=False)
     def check_for_translation(self) -> bool:
-        try:
-            container = self._driver.find_element(by=self.WEBDRIVER_BY.ID, value='dl_translator')
-            return 'lmt--active_translation_request' not in container.get_attribute('class')
-        except NoSuchElementException:
-            return False
+        container = self._driver.find_element(by=self.WEBDRIVER_BY.ID, value='dl_translator')
+        return 'lmt--active_translation_request' not in container.get_attribute('class')
 
     def accept_cookies(self) -> None:
         self.click_cookies_accept('Accept')
 
+    @safe_run(NoSuchElementException, default_return_value=None)
     def click_cookies_accept(self, btn_text: str) -> None:
-        try:
-            cookies_accept_button = self._driver.find_element(
-                by=self.WEBDRIVER_BY.CLASS_NAME, value='dl_cookieBanner--buttonAll'
-            )
-            if cookies_accept_button:
-                cookies_accept_button.click()
-        except NoSuchElementException:
-            return
+        cookies_accept_button = self._driver.find_element(
+            by=self.WEBDRIVER_BY.CLASS_NAME, value='dl_cookieBanner--buttonAll'
+        )
+        if cookies_accept_button:
+            cookies_accept_button.click()
 
+    @safe_run(NoSuchElementException, default_return_value=False)
     def check_for_antispam(self) -> bool:
-        try:
-            container = self._driver.find_element(
-                by=self.WEBDRIVER_BY.XPATH,
-                value='//*[text()="You’ve reached your free usage limit.*"]',
-            )
-            return container.is_displayed()
-        except NoSuchElementException:
-            return False
+        container = self._driver.find_element(
+            by=self.WEBDRIVER_BY.XPATH,
+            value='//*[text()="You’ve reached your free usage limit.*"]',
+        )
+        return container.is_displayed()
 
     @staticmethod
     def get_translated_data(output_element: WebElement) -> str:
         return output_element.get_attribute('value')
```

### Comparing `md_translate-3.0.0/md_translate/translators/google.py` & `md_translate-3.0.1/md_translate/translators/google.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.remote.webelement import WebElement
 
+from md_translate.exceptions import safe_run
+
 from ._selenium_base import SeleniumBaseTranslator
 
 
 class GoogleTranslateProvider(SeleniumBaseTranslator):
     HOST = 'https://translate.google.com/'
 
     def get_url(self) -> str:
@@ -20,20 +22,18 @@
         ).find_element(by=self.WEBDRIVER_BY.TAG_NAME, value='textarea')
 
     def get_output_element(self) -> WebElement:
         return self._driver.find_element(
             by=self.WEBDRIVER_BY.XPATH, value='//div[@aria-live="polite"]'
         ).find_element(by=self.WEBDRIVER_BY.CSS_SELECTOR, value=f'span[lang="{self.to_language}"]')
 
+    @safe_run(NoSuchElementException, default_return_value=False)
     def check_for_translation(self) -> bool:
-        try:
-            element = self.get_output_element()
-            return element.text != ''
-        except NoSuchElementException:
-            return False
+        element = self.get_output_element()
+        return element.text != ''
 
     def accept_cookies(self) -> None:
         if 'consent.google.com' in self._driver.current_url:
             buttons = self._driver.find_elements(by=self.WEBDRIVER_BY.TAG_NAME, value='button')
             buttons[1].click()
 
     def check_for_antispam(self) -> bool:
```

### Comparing `md_translate-3.0.0/md_translate/translators/randomizer/const.py` & `md_translate-3.0.1/md_translate/translators/randomizer/const.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.0/md_translate/translators/randomizer/randomizer.py` & `md_translate-3.0.1/md_translate/translators/randomizer/randomizer.py`

 * *Files identical despite different names*

### Comparing `md_translate-3.0.0/md_translate/translators/yandex.py` & `md_translate-3.0.1/md_translate/translators/yandex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.remote.webelement import WebElement
 
+from md_translate.exceptions import safe_run
+
 from ._selenium_base import SeleniumBaseTranslator
 
 
 class YandexTranslateProvider(SeleniumBaseTranslator):
     HOST = 'https://translate.yandex.com/'
 
     COOKIES_ACCEPT_BTN_TEXT = 'Accept'
@@ -17,23 +19,21 @@
 
     def get_input_element(self) -> WebElement:
         return self._driver.find_element(by=self.WEBDRIVER_BY.CLASS_NAME, value='textinput')
 
     def get_output_element(self) -> WebElement:
         return self._driver.find_element(by=self.WEBDRIVER_BY.ID, value='translation')
 
+    @safe_run(NoSuchElementException, default_return_value=False)
     def check_for_translation(self) -> bool:
-        try:
-            container = self._driver.find_element(by=self.WEBDRIVER_BY.ID, value='textbox2')
-            if 'fetching' in container.get_attribute('class'):
-                return False
-            element = self._driver.find_element(by=self.WEBDRIVER_BY.ID, value='translation')
-            return element.text != ''
-        except NoSuchElementException:
+        container = self._driver.find_element(by=self.WEBDRIVER_BY.ID, value='textbox2')
+        if 'fetching' in container.get_attribute('class'):
             return False
+        element = self._driver.find_element(by=self.WEBDRIVER_BY.ID, value='translation')
+        return element.text != ''
 
     def accept_cookies(self) -> None:
         self.click_cookies_accept('Accept')
 
     def check_for_antispam(self) -> bool:
         try:
             self._driver.find_element(
```

### Comparing `md_translate-3.0.0/pyproject.toml` & `md_translate-3.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "md_translate"
-version = "3.0.0"
+version = "3.0.1"
 description = "CLI tool to translate markdown files"
 authors = ["Ilya Chichak <ilyachch@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/ilyachch/md_docs-trans-app"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -29,15 +29,14 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-requests = "^2.24.0"
 selenium = "^4.5.0"
 mistune = "^2.0.4"
 pydantic = "^1.10.2"
 click = "^8.1.3"
 webdriver-manager = "^3.8.6"
 
 [tool.poetry.group.dev.dependencies]
@@ -64,15 +63,18 @@
 
 [tool.isort]
 profile = "black"
 line_length = 99
 src_paths = ["md_translate"]
 
 [tool.pytest.ini_options]
-addopts = """"""
+addopts = "-m 'not web'"
+markers = [
+    "web: mark test as web test",
+]
 
 [tool.coverage.run]
 source = [
     "md_translate",
 ]
 omit = [
     "tests/*",
```

### Comparing `md_translate-3.0.0/PKG-INFO` & `md_translate-3.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md-translate
-Version: 3.0.0
+Version: 3.0.1
 Summary: CLI tool to translate markdown files
 Home-page: https://github.com/ilyachch/md_docs-trans-app
 License: MIT
 Author: Ilya Chichak
 Author-email: ilyachch@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -21,26 +21,25 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: mistune (>=2.0.4,<3.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
-Requires-Dist: requests (>=2.24.0,<3.0.0)
 Requires-Dist: selenium (>=4.5.0,<5.0.0)
 Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0)
 Project-URL: Repository, https://github.com/ilyachch/md_docs-trans-app
 Description-Content-Type: text/markdown
 
 # Markdown Docs Translator
 
 ![Python](https://img.shields.io/badge/python-v3.10+-blue.svg)
 ![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)
 
-Markdown Docs Translator is an automated translator for markdown documents, built with Python. The tool supports multiple translation services and provides a variety of options to customize the translation process.
+Markdown Docs Translator is an automated translator for Markdown documents, built with Python. The tool supports multiple translation services and provides a variety of options to customize the translation process.
 
 ## Features
 
 - Support for multiple translation services (Yandex, Google, Bing, Deepl).
 - Multithreading for faster translations.
 - Options to overwrite original files, drop original files, or create a new file with translated text.
 - Caching for faster repeat translations.
@@ -76,42 +75,42 @@
 - `source_lang` is the language code of the source document.
 - `target_lang` is the language code for the translation.
 - `service` is the translating service to use (yandex, google, bing, deepl).
 - `OPTIONS` are additional options that can be specified as listed below.
 
 ### Options
 
-| Option                        | Description                          |
-| ----------------------------- | ------------------------------------ |
-| `-F, --from-lang TEXT`        | Source language code \[required\]    |
-| `-T, --to-lang TEXT`          | Target language code \[required\]    |
-| `-P, --service`               | Translating service \[required\]     |
-| `-X, --processes INTEGER`     | Number of processes to use           |
-| `-N, --new-file`              | Create new file with translated text |
-| `-I, --ignore-cache`          | Ignore cache                         |
-| `-S, --save-temp-on-complete` | Save temporary files on complete     |
-| `-O, --overwrite`             | Overwrite original files             |
-| `-V, --verbose`               | Verbosity level                      |
-| `-D, --drop-original`         | Drop original files                  |
-| `--help`                      | Show help message and exit           |
+| Option                        | Description                                                                                                                                                                        |
+| ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `-F, --from-lang TEXT`        | Source language code \[required\]                                                                                                                                                  |
+| `-T, --to-lang TEXT`          | Target language code \[required\]                                                                                                                                                  |
+| `-P, --service`               | Translating service \[required\]                                                                                                                                                   |
+| `-X, --processes INTEGER`     | Number of processes to use. Will be applied to each file separately                                                                                                                |
+| `-N, --new-file`              | Create a new file with translated text (original file will remain unchanged). The new file will be created in the same directory as the original file with a "\_translated" suffix |
+| `-I, --ignore-cache`          | Ignore cache files. If cache exists, it will be overwritten                                                                                                                        |
+| `-S, --save-temp-on-complete` | Save cache files upon completion. If not set, they will be deleted                                                                                                                 |
+| `-O, --overwrite`             | Already translated files will be overwritten. Otherwise, these files will be skipped                                                                                               |
+| `-D, --drop-original`         | Remove original lines from translated file. These lines will be replaced with translated ones                                                                                      |
+| `-V, --verbose`               | Verbosity level                                                                                                                                                                    |
+| `--help`                      | Show help message and exit                                                                                                                                                         |
 
 Currently supported services are:
 
 - `Yandex`
 - `Google`
 - `Bing`
 - `Deepl`
 
 ### Configuring with a Configuration File
 
 Options for the application can be defined through a configuration file as well. This file should be named `settings.json` and is typically located at `~/.config/md_translate`.
 
 If you choose to use a non-default location for the config file, you can specify its path using the `--config` or `-C` option.
 
-This configuration file can encompass all CLI options with the exception of `path`, `from_lang`, `to_lang`, and `service`. These particular options need to be stated directly in the CLI.
+This configuration file can encompass all CLI options except `path`, `from_lang`, `to_lang`, `service` and `config_file_path`. These particular options need to be stated directly in the CLI.
 
 The configuration file should be a valid JSON file and adhere to the following structure:
 
 ```json
 {
     "processes": 4,
     "new_file": true,
```

