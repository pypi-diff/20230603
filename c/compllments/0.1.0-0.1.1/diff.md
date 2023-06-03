# Comparing `tmp/compllments-0.1.0.tar.gz` & `tmp/compllments-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compllments-0.1.0.tar", max compression
+gzip compressed data, was "compllments-0.1.1.tar", max compression
```

## Comparing `compllments-0.1.0.tar` & `compllments-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     4315 2023-05-27 03:53:05.383863 compllments-0.1.0/README.md
--rw-r--r--   0        0        0     4039 2023-06-03 21:08:41.271424 compllments-0.1.0/compllments/README.md
--rw-r--r--   0        0        0        0 2023-05-25 18:53:06.598929 compllments-0.1.0/compllments/__init__.py
--rw-r--r--   0        0        0      739 2023-06-03 04:09:37.125392 compllments-0.1.0/compllments/config.py
--rw-r--r--   0        0        0     1006 2023-06-03 03:44:29.212502 compllments-0.1.0/compllments/cron
--rw-r--r--   0        0        0     2802 2023-06-03 20:30:34.760785 compllments-0.1.0/compllments/main.py
--rw-r--r--   0        0        0        0 2023-05-27 03:11:16.146426 compllments-0.1.0/compllments/models/add_models_here.txt
--rw-r--r--   0        0        0        0 2023-05-27 01:12:39.826663 compllments-0.1.0/compllments/utils/__init__.py
--rw-r--r--   0        0        0     3490 2023-06-03 20:30:24.340996 compllments-0.1.0/compllments/utils/model.py
--rw-r--r--   0        0        0     1843 2023-05-27 00:16:56.835613 compllments-0.1.0/compllments/utils/providers.py
--rw-r--r--   0        0        0     1286 2023-06-03 04:10:33.752440 compllments-0.1.0/compllments/utils/texter.py
--rw-r--r--   0        0        0      861 2023-06-03 04:22:01.920610 compllments-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5614 1970-01-01 00:00:00.000000 compllments-0.1.0/setup.py
--rw-r--r--   0        0        0     5256 1970-01-01 00:00:00.000000 compllments-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4048 2023-06-03 21:24:27.947633 compllments-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 18:53:06.598929 compllments-0.1.1/compllments/__init__.py
+-rw-r--r--   0        0        0      714 2023-06-03 21:24:55.159305 compllments-0.1.1/compllments/config.py
+-rw-r--r--   0        0        0     1006 2023-06-03 03:44:29.212502 compllments-0.1.1/compllments/cron
+-rw-r--r--   0        0        0     2802 2023-06-03 21:26:24.797434 compllments-0.1.1/compllments/main.py
+-rw-r--r--   0        0        0        0 2023-05-27 03:11:16.146426 compllments-0.1.1/compllments/models/add_models_here.txt
+-rw-r--r--   0        0        0        0 2023-05-27 01:12:39.826663 compllments-0.1.1/compllments/utils/__init__.py
+-rw-r--r--   0        0        0     3490 2023-06-03 20:30:24.340996 compllments-0.1.1/compllments/utils/model.py
+-rw-r--r--   0        0        0     1843 2023-05-27 00:16:56.835613 compllments-0.1.1/compllments/utils/providers.py
+-rw-r--r--   0        0        0     1286 2023-06-03 04:10:33.752440 compllments-0.1.1/compllments/utils/texter.py
+-rw-r--r--   0        0        0      861 2023-06-03 21:22:35.083293 compllments-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5311 1970-01-01 00:00:00.000000 compllments-0.1.1/setup.py
+-rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 compllments-0.1.1/PKG-INFO
```

### Comparing `compllments-0.1.0/README.md` & `compllments-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,100 @@
-# compLLMents>
+Metadata-Version: 2.1
+Name: compllments
+Version: 0.1.1
+Summary: Send nice texts to your friends using LLMs
+Author: Austin Botelho
+Author-email: austinbotelho@nyu.edu
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: accelerate (>=0.19.0,<0.20.0)
+Requires-Dist: bitsandbytes (>=0.39.0,<0.40.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: einops (>=0.6.1,<0.7.0)
+Requires-Dist: emoji (>=2.4.0,<3.0.0)
+Requires-Dist: langchain (>=0.0.180,<0.0.181)
+Requires-Dist: openai (>=0.27.7,<0.28.0)
+Requires-Dist: poethepoet (>=0.20.0,<0.21.0)
+Requires-Dist: pynput (>=1.7.6,<2.0.0)
+Requires-Dist: pywhatkit (>=5.4,<6.0)
+Requires-Dist: transformers (>=4.29.2,<5.0.0)
+Requires-Dist: twilio (>=8.2.1,<9.0.0)
+Description-Content-Type: text/markdown
 
-## Description
-
-This package enables you to send scheduled, uplifting, AI-generated text messages to yourself and your friends. 
+# compLLMents
 
-It works by first using am LLM to generate a batch of positive and complimentary messages in the language of choice. Then, a multilingual sentiment classifier scores all the generated posts and selects the most positive to send either as an SMS or over WhatsApp.
+<!-- ![GitHub all releases](https://img.shields.io/github/downloads/botelhoa/compLLMents/total?style=plastic)
+![MIT License](https://img.shields.io/bower/l/compLLMents?style=plastic) -->
 
+## Description
 
-DISCLAIMER: If you or someone you know is suffering from mental health difficulties, please seek professional *human* help instead of from chatbots. 
-[Here]() is one good resource of many.
+This package enables you to send scheduled, uplifting, AI-generated text messages to your friends. 
 
+It works by first using an LLM to generate a batch of positive and complimentary messages in the language of your choice. Then, a multilingual sentiment classifier scores all the generated posts and selects the most positive to send either as an SMS or over WhatsApp. [Here](https://colab.research.google.com/drive/1gfTlCWNFgpHdvLR5g8o-OV_a30Pfps60?usp=sharing) is the accompanying Colab notebook.
 
-Provide a short description explaining the what, why, and how of your project. Use the following questions as a guide:
 
-- What was your motivation?
-- Why did you build this project? (Note: the answer is not "Because it was a homework assignment.")
-- What problem does it solve?
-- What did you learn?
+DISCLAIMER: If someone you know is suffering from mental health difficulties, please reach out person-to-person or encourage them to seek professional *human* help instead of from chatbots. [Here](https://www.nimh.nih.gov/health/find-help) is one good resource of many.
 
-## Table of Contents (Optional)
 
-If your README is long, add a table of contents to make it easy for users to find what they need.
+## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
-- [Credits](#credits)
 - [License](#license)
 
 ## Installation
 
 First, ensure that [`poetry`](https://python-poetry.org/docs/#installation) is installed. 
 
 ```
 poetry install
 poe install-pytorch
 ```
 
 To download files to store locally and save time of future downloads, run:
-`download -m path/on/huggingface`
 
-To send SMS messages, first create a free [Twilio](https://www.twilio.com/en-us) account (note: Twilio automatically prepends the message `blah` to free-tier accounts). Copy your credentials from the dashboard into the `TWILIO_CONFIG` dictionary in `config.py`. An example config will look like:
+```
+download -m path/on/huggingface
+```
+
+To send SMS messages, first create a free [Twilio](https://www.twilio.com/en-us) account and create a phone number (note: Twilio automatically prepends the message `Sent from your Twilio trial account` to free-tier accounts). Copy your credentials from the dashboard into the `TWILIO_CONFIG` dictionary in `config.py`. An example config will look like:
+
 ```
  {
     "account_sid": "a_string",
     "auth_token": "a_token",
+    "from_": "+11234567890",
 }
 ```
+To send WhatsApp messages, you must log in from your computer.
 
 ## Usage
 
-Provide instructions and examples for use. Include screenshots as needed.
-
-To add a screenshot, create an `assets/images` folder in your repository and upload your screenshot to it. Then, using the relative filepath, add it to your README using the following syntax:
-
-    ```md
-    ![alt text](assets/images/screenshot.png)
-    ```
-
 Texts are sent by running:
+
 ```
-send -r recipient-name -s sender-name -n +11234567890 -l language -b -t sms
+send -r recipient-name -s sender-name -n +11234567890 -l language -b -t type
 ```
 
-`send --help` explains the parameter options.
+`send --help` explains the parameter options. Pass your OpenAI API key using `-o` to use their models.
 
 You can send custom messages by chaning the text in the `TEMPLATE` object in `main.py`
 
-You can set custom model configuration in the `INFERENCE_CONFIG` object in `conifg.py` including swapping out models, increasing the output length by chaning `max_new_tokens` or increasing the randomness in reponses by raising `temperature` or `top_p`.
+You can set custom model configuration in the `INFERENCE_CONFIG` object in `conifg.py` including swapping out models, increasing the output length by chaning `max_new_tokens` or increasing the randomness in reponses by raising `temperature` or `top_p`. The default language generation model is `mosaicml/mpt-7b-instruct` which is the [best performing open-sourced LLM](https://gpt4all.io/index.html) at the time of creation. The default sentiment analysis model is `cardiffnlp/xlm-roberta-base-sentiment-multilingual` which supports 8 languagees: `arabic`, `english`, `french`, `german`, `hindi`, `italian`, `portuguese`, and, `spanish`. 
 
 
-Below are some example text generations
-```
-```
-
-And here are the sentiment scores for them
-```
-```
-
-To schedule texts to be sent at regular intervals, 
-- crontab setup
-
+To schedule texts to be sent at regular intervals, create a crontab similar to the example in `cron`.
 
 
 ## Tests
 
-
-## Credits
-
-List your collaborators, if any, with links to their GitHub profiles.
-
-If you used any third-party assets that require attribution, list the creators with links to their primary web presence in this section.
-
-If you followed tutorials, include links to those here as well.
+Forethcoming...
 
 
 ## License
 
 MIT License
 
 Copyright (c) [year] [fullname]
@@ -114,17 +113,8 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
-Roadmap
-
-1.   Locally hosted
-2.   Ping API
-3.   Multilingual
-4.   SMS + WhatsApp support
-5.   Select nicest
-6.   cron job scheduling
-7.   publish to pypi
```

### Comparing `compllments-0.1.0/compllments/README.md` & `compllments-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # compLLMents
 
-![GitHub all releases](https://img.shields.io/github/downloads/botelhoa/compLLMents/total?style=plastic)
-![MIT License](https://img.shields.io/bower/l/compLLMents?style=plastic)
+<!-- ![GitHub all releases](https://img.shields.io/github/downloads/botelhoa/compLLMents/total?style=plastic)
+![MIT License](https://img.shields.io/bower/l/compLLMents?style=plastic) -->
 
 ## Description
 
 This package enables you to send scheduled, uplifting, AI-generated text messages to your friends. 
 
 It works by first using an LLM to generate a batch of positive and complimentary messages in the language of your choice. Then, a multilingual sentiment classifier scores all the generated posts and selects the most positive to send either as an SMS or over WhatsApp. [Here](https://colab.research.google.com/drive/1gfTlCWNFgpHdvLR5g8o-OV_a30Pfps60?usp=sharing) is the accompanying Colab notebook.
```

### Comparing `compllments-0.1.0/compllments/cron` & `compllments-0.1.1/compllments/cron`

 * *Files identical despite different names*

### Comparing `compllments-0.1.0/compllments/main.py` & `compllments-0.1.1/compllments/main.py`

 * *Files identical despite different names*

### Comparing `compllments-0.1.0/compllments/utils/model.py` & `compllments-0.1.1/compllments/utils/model.py`

 * *Files identical despite different names*

### Comparing `compllments-0.1.0/compllments/utils/providers.py` & `compllments-0.1.1/compllments/utils/providers.py`

 * *Files identical despite different names*

### Comparing `compllments-0.1.0/compllments/utils/texter.py` & `compllments-0.1.1/compllments/utils/texter.py`

 * *Files identical despite different names*

### Comparing `compllments-0.1.0/pyproject.toml` & `compllments-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "compllments"
-version = "0.1.0"
+version = "0.1.1"
 description = "Send nice texts to your friends using LLMs"
 authors = ["Austin Botelho <austinbotelho@nyu.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pywhatkit = "^5.4"
```

### Comparing `compllments-0.1.0/setup.py` & `compllments-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
 entry_points = \
 {'console_scripts': ['download = compllments.main:download',
                      'send = compllments.main:cli']}
 
 setup_kwargs = {
     'name': 'compllments',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Send nice texts to your friends using LLMs',
-    'long_description': '# compLLMents>\n\n## Description\n\nThis package enables you to send scheduled, uplifting, AI-generated text messages to yourself and your friends. \n\nIt works by first using am LLM to generate a batch of positive and complimentary messages in the language of choice. Then, a multilingual sentiment classifier scores all the generated posts and selects the most positive to send either as an SMS or over WhatsApp.\n\n\nDISCLAIMER: If you or someone you know is suffering from mental health difficulties, please seek professional *human* help instead of from chatbots. \n[Here]() is one good resource of many.\n\n\nProvide a short description explaining the what, why, and how of your project. Use the following questions as a guide:\n\n- What was your motivation?\n- Why did you build this project? (Note: the answer is not "Because it was a homework assignment.")\n- What problem does it solve?\n- What did you learn?\n\n## Table of Contents (Optional)\n\nIf your README is long, add a table of contents to make it easy for users to find what they need.\n\n- [Installation](#installation)\n- [Usage](#usage)\n- [Credits](#credits)\n- [License](#license)\n\n## Installation\n\nFirst, ensure that [`poetry`](https://python-poetry.org/docs/#installation) is installed. \n\n```\npoetry install\npoe install-pytorch\n```\n\nTo download files to store locally and save time of future downloads, run:\n`download -m path/on/huggingface`\n\nTo send SMS messages, first create a free [Twilio](https://www.twilio.com/en-us) account (note: Twilio automatically prepends the message `blah` to free-tier accounts). Copy your credentials from the dashboard into the `TWILIO_CONFIG` dictionary in `config.py`. An example config will look like:\n```\n {\n    "account_sid": "a_string",\n    "auth_token": "a_token",\n}\n```\n\n## Usage\n\nProvide instructions and examples for use. Include screenshots as needed.\n\nTo add a screenshot, create an `assets/images` folder in your repository and upload your screenshot to it. Then, using the relative filepath, add it to your README using the following syntax:\n\n    ```md\n    ![alt text](assets/images/screenshot.png)\n    ```\n\nTexts are sent by running:\n```\nsend -r recipient-name -s sender-name -n +11234567890 -l language -b -t sms\n```\n\n`send --help` explains the parameter options.\n\nYou can send custom messages by chaning the text in the `TEMPLATE` object in `main.py`\n\nYou can set custom model configuration in the `INFERENCE_CONFIG` object in `conifg.py` including swapping out models, increasing the output length by chaning `max_new_tokens` or increasing the randomness in reponses by raising `temperature` or `top_p`.\n\n\nBelow are some example text generations\n```\n```\n\nAnd here are the sentiment scores for them\n```\n```\n\nTo schedule texts to be sent at regular intervals, \n- crontab setup\n\n\n\n## Tests\n\n\n## Credits\n\nList your collaborators, if any, with links to their GitHub profiles.\n\nIf you used any third-party assets that require attribution, list the creators with links to their primary web presence in this section.\n\nIf you followed tutorials, include links to those here as well.\n\n\n## License\n\nMIT License\n\nCopyright (c) [year] [fullname]\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n\nRoadmap\n\n1.   Locally hosted\n2.   Ping API\n3.   Multilingual\n4.   SMS + WhatsApp support\n5.   Select nicest\n6.   cron job scheduling\n7.   publish to pypi\n\n',
+    'long_description': '# compLLMents\n\n<!-- ![GitHub all releases](https://img.shields.io/github/downloads/botelhoa/compLLMents/total?style=plastic)\n![MIT License](https://img.shields.io/bower/l/compLLMents?style=plastic) -->\n\n## Description\n\nThis package enables you to send scheduled, uplifting, AI-generated text messages to your friends. \n\nIt works by first using an LLM to generate a batch of positive and complimentary messages in the language of your choice. Then, a multilingual sentiment classifier scores all the generated posts and selects the most positive to send either as an SMS or over WhatsApp. [Here](https://colab.research.google.com/drive/1gfTlCWNFgpHdvLR5g8o-OV_a30Pfps60?usp=sharing) is the accompanying Colab notebook.\n\n\nDISCLAIMER: If someone you know is suffering from mental health difficulties, please reach out person-to-person or encourage them to seek professional *human* help instead of from chatbots. [Here](https://www.nimh.nih.gov/health/find-help) is one good resource of many.\n\n\n## Table of Contents\n\n- [Installation](#installation)\n- [Usage](#usage)\n- [License](#license)\n\n## Installation\n\nFirst, ensure that [`poetry`](https://python-poetry.org/docs/#installation) is installed. \n\n```\npoetry install\npoe install-pytorch\n```\n\nTo download files to store locally and save time of future downloads, run:\n\n```\ndownload -m path/on/huggingface\n```\n\nTo send SMS messages, first create a free [Twilio](https://www.twilio.com/en-us) account and create a phone number (note: Twilio automatically prepends the message `Sent from your Twilio trial account` to free-tier accounts). Copy your credentials from the dashboard into the `TWILIO_CONFIG` dictionary in `config.py`. An example config will look like:\n\n```\n {\n    "account_sid": "a_string",\n    "auth_token": "a_token",\n    "from_": "+11234567890",\n}\n```\nTo send WhatsApp messages, you must log in from your computer.\n\n## Usage\n\nTexts are sent by running:\n\n```\nsend -r recipient-name -s sender-name -n +11234567890 -l language -b -t type\n```\n\n`send --help` explains the parameter options. Pass your OpenAI API key using `-o` to use their models.\n\nYou can send custom messages by chaning the text in the `TEMPLATE` object in `main.py`\n\nYou can set custom model configuration in the `INFERENCE_CONFIG` object in `conifg.py` including swapping out models, increasing the output length by chaning `max_new_tokens` or increasing the randomness in reponses by raising `temperature` or `top_p`. The default language generation model is `mosaicml/mpt-7b-instruct` which is the [best performing open-sourced LLM](https://gpt4all.io/index.html) at the time of creation. The default sentiment analysis model is `cardiffnlp/xlm-roberta-base-sentiment-multilingual` which supports 8 languagees: `arabic`, `english`, `french`, `german`, `hindi`, `italian`, `portuguese`, and, `spanish`. \n\n\nTo schedule texts to be sent at regular intervals, create a crontab similar to the example in `cron`.\n\n\n## Tests\n\nForethcoming...\n\n\n## License\n\nMIT License\n\nCopyright (c) [year] [fullname]\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n\n',
     'author': 'Austin Botelho',
     'author_email': 'austinbotelho@nyu.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

