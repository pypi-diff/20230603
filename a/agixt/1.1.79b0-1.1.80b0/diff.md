# Comparing `tmp/agixt-1.1.79b0.tar.gz` & `tmp/agixt-1.1.80b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.79b0.tar", max compression
+gzip compressed data, was "agixt-1.1.80b0.tar", max compression
```

## Comparing `agixt-1.1.79b0.tar` & `agixt-1.1.80b0.tar`

### file list

```diff
@@ -1,111 +1,112 @@
--rw-r--r--   0        0        0     1087 2023-06-02 14:04:16.786770 agixt-1.1.79b0/LICENSE
--rw-r--r--   0        0        0    19685 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/AGiXT.py
--rw-r--r--   0        0        0    24299 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/Agent.py
--rw-r--r--   0        0        0     7237 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/Chain.py
--rw-r--r--   0        0        0     1101 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/Config.py
--rw-r--r--   0        0        0     5904 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/Embedding.py
--rw-r--r--   0        0        0     6474 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/Extensions.py
--rw-r--r--   0        0        0      606 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/Main.py
--rw-r--r--   0        0        0     9626 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/Memories.py
--rw-r--r--   0        0        0     1943 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/Prompts.py
--rw-r--r--   0        0        0     7099 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/Tasks.py
--rw-r--r--   0        0        0       38 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/WORKSPACE/example.txt
--rw-r--r--   0        0        0      230 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/__init__.py
--rw-r--r--   0        0        0      209 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/agents/gpt4free/config.json
--rw-r--r--   0        0        0        0 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/agents/gpt4free.yaml
--rw-r--r--   0        0        0    12707 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/app.py
--rw-r--r--   0        0        0     1793 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/auth_libs/Cfig.py
--rw-r--r--   0        0        0     1165 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/auth_libs/Redirect.py
--rw-r--r--   0        0        0     4261 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/auth_libs/Users.py
--rw-r--r--   0        0        0     2012 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/chains/Smart Chat.json
--rw-r--r--   0        0        0    10644 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/chains/Test_Commands.json
--rw-r--r--   0        0        0      410 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/chains/Write a Poem.json
--rw-r--r--   0        0        0     1566 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/components/agent_selector.py
--rw-r--r--   0        0        0       42 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/config.yaml
--rw-r--r--   0        0        0    11935 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/example.ipynb
--rw-r--r--   0        0        0     6026 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/agixt_agent.py
--rw-r--r--   0        0        0      860 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/briantts.py
--rw-r--r--   0        0        0     1174 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/dalle.py
--rw-r--r--   0        0        0     2818 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/discord.py
--rw-r--r--   0        0        0     1170 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/elevenlabs.py
--rw-r--r--   0        0        0     6647 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/file_system.py
--rw-r--r--   0        0        0     1841 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/github.py
--rw-r--r--   0        0        0     2042 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/google.py
--rw-r--r--   0        0        0      539 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/gtts.py
--rw-r--r--   0        0        0     2475 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/huggingface.py
--rw-r--r--   0        0        0      622 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/macostts.py
--rw-r--r--   0        0        0     4236 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/microsoft_365.py
--rw-r--r--   0        0        0     1899 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/searxng.py
--rw-r--r--   0        0        0     1001 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/sendgrid_email.py
--rw-r--r--   0        0        0      315 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/times.py
--rw-r--r--   0        0        0     1169 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/twitter.py
--rw-r--r--   0        0        0     2287 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/extensions/web_playwright.py
--rw-r--r--   0        0        0    10464 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/pages/0-Agent_Settings.py
--rw-r--r--   0        0        0     2035 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/pages/1-Learning.py
--rw-r--r--   0        0        0     2491 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/pages/2-Prompts.py
--rw-r--r--   0        0        0    13398 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/pages/3-Chains.py
--rw-r--r--   0        0        0     2909 2023-06-02 14:04:16.786770 agixt-1.1.79b0/agixt/pages/4-Chat.py
--rw-r--r--   0        0        0     3006 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/pages/5-Instructions.py
--rw-r--r--   0        0        0     1616 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/pages/6-Tasks.py
--rw-r--r--   0        0        0     1808 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/pages/Login.py
--rw-r--r--   0        0        0     5603 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/pages/Profile.py
--rw-r--r--   0        0        0     1828 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/pages/Register.py
--rw-r--r--   0        0        0      145 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/Chat.txt
--rw-r--r--   0        0        0      175 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0        0        0      991 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/Create New Command.txt
--rw-r--r--   0        0        0     1011 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/Execution.txt
--rw-r--r--   0        0        0     1172 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/Instruction.txt
--rw-r--r--   0        0        0      372 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0        0        0      170 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0        0        0      424 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0        0        0      326 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/Prioritize.txt
--rw-r--r--   0        0        0      236 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0        0        0      343 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0        0        0      268 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0        0        0      298 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0        0        0      142 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0        0        0      468 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0        0        0      522 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0        0        0      452 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0        0        0      427 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0        0        0      154 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0        0        0      501 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0        0        0      554 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0        0        0      186 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0        0        0      155 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/Tell Me How.txt
--rw-r--r--   0        0        0      162 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/Title a Poem.txt
--rw-r--r--   0        0        0      308 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/Validation.txt
--rw-r--r--   0        0        0      850 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0        0        0      308 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/WebSearch.txt
--rw-r--r--   0        0        0       28 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/Write a Poem.txt
--rw-r--r--   0        0        0     1172 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
--rw-r--r--   0        0        0     1172 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0        0        0      771 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/instruct.txt
--rw-r--r--   0        0        0      818 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/starchat/instruct.txt
--rw-r--r--   0        0        0      610 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/prompts/vicuna/instruct.txt
--rw-r--r--   0        0        0     2147 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/__init__.py
--rw-r--r--   0        0        0     1611 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/azure.py
--rw-r--r--   0        0        0      487 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/bard.py
--rw-r--r--   0        0        0     2050 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/bing.py
--rw-r--r--   0        0        0      974 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/chatgpt.py
--rw-r--r--   0        0        0     1006 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/claude.py
--rw-r--r--   0        0        0      757 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/fastchat.py
--rw-r--r--   0        0        0      867 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/gpt4all.py
--rw-r--r--   0        0        0     4491 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/gpt4free.py
--rw-r--r--   0        0        0     1188 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0        0        0     1001 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/huggingchat.py
--rw-r--r--   0        0        0     1432 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/huggingface.py
--rw-r--r--   0        0        0     1085 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/kobold.py
--rw-r--r--   0        0        0     1939 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/llamacpp.py
--rw-r--r--   0        0        0     2177 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/llamacppapi.py
--rw-r--r--   0        0        0     1579 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/oobabooga.py
--rw-r--r--   0        0        0     1464 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/openai.py
--rw-r--r--   0        0        0      844 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/palm.py
--rw-r--r--   0        0        0     3826 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/runpod.py
--rw-r--r--   0        0        0     3100 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/provider/transformer.py
--rw-r--r--   0        0        0      538 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/starchat.sh
--rw-r--r--   0        0        0     2845 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/test-commands.ipynb
--rw-r--r--   0        0        0     8553 2023-06-02 14:04:16.790770 agixt-1.1.79b0/agixt/test-memory.ipynb
--rw-r--r--   0        0        0    13215 2023-06-02 14:04:16.794770 agixt-1.1.79b0/docs/README.md
--rw-r--r--   0        0        0     2838 2023-06-02 14:04:16.806770 agixt-1.1.79b0/pyproject.toml
--rw-r--r--   0        0        0    16070 1970-01-01 00:00:00.000000 agixt-1.1.79b0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-03 11:55:38.759473 agixt-1.1.80b0/LICENSE
+-rw-r--r--   0        0        0    21022 2023-06-03 11:55:38.759473 agixt-1.1.80b0/agixt/AGiXT.py
+-rw-r--r--   0        0        0    24299 2023-06-03 11:55:38.759473 agixt-1.1.80b0/agixt/Agent.py
+-rw-r--r--   0        0        0     7564 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Chain.py
+-rw-r--r--   0        0        0     1101 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Config.py
+-rw-r--r--   0        0        0     5900 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Embedding.py
+-rw-r--r--   0        0        0     6474 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Extensions.py
+-rw-r--r--   0        0        0      606 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Main.py
+-rw-r--r--   0        0        0     9647 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Memories.py
+-rw-r--r--   0        0        0     1943 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Prompts.py
+-rw-r--r--   0        0        0     7099 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Tasks.py
+-rw-r--r--   0        0        0       38 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/WORKSPACE/example.txt
+-rw-r--r--   0        0        0      230 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/__init__.py
+-rw-r--r--   0        0        0      244 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/agents/gpt4free/config.json
+-rw-r--r--   0        0        0        0 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/agents/gpt4free.yaml
+-rw-r--r--   0        0        0    12707 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/app.py
+-rw-r--r--   0        0        0     1793 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/auth_libs/Cfig.py
+-rw-r--r--   0        0        0     1165 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/auth_libs/Redirect.py
+-rw-r--r--   0        0        0     4261 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/auth_libs/Users.py
+-rw-r--r--   0        0        0     2012 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/chains/Smart Chat.json
+-rw-r--r--   0        0        0    10644 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/chains/Test_Commands.json
+-rw-r--r--   0        0        0      566 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/chains/Write a Poem.json
+-rw-r--r--   0        0        0      959 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/chains/Write a Poem_responses.json
+-rw-r--r--   0        0        0     1566 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/components/agent_selector.py
+-rw-r--r--   0        0        0       42 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/config.yaml
+-rw-r--r--   0        0        0    11935 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/example.ipynb
+-rw-r--r--   0        0        0     6026 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/agixt_agent.py
+-rw-r--r--   0        0        0      860 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/briantts.py
+-rw-r--r--   0        0        0     1174 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/dalle.py
+-rw-r--r--   0        0        0     2818 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/discord.py
+-rw-r--r--   0        0        0     1170 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/elevenlabs.py
+-rw-r--r--   0        0        0     6647 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/file_system.py
+-rw-r--r--   0        0        0     1841 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/github.py
+-rw-r--r--   0        0        0     2042 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/google.py
+-rw-r--r--   0        0        0      539 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/gtts.py
+-rw-r--r--   0        0        0     2475 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/huggingface.py
+-rw-r--r--   0        0        0      622 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/macostts.py
+-rw-r--r--   0        0        0     4236 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/microsoft_365.py
+-rw-r--r--   0        0        0     1899 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/searxng.py
+-rw-r--r--   0        0        0     1001 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0        0        0      315 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/times.py
+-rw-r--r--   0        0        0     1169 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/twitter.py
+-rw-r--r--   0        0        0     2287 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/web_playwright.py
+-rw-r--r--   0        0        0    10464 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/0-Agent_Settings.py
+-rw-r--r--   0        0        0     2035 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/1-Learning.py
+-rw-r--r--   0        0        0     2491 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/2-Prompts.py
+-rw-r--r--   0        0        0    13672 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/3-Chains.py
+-rw-r--r--   0        0        0     2909 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/4-Chat.py
+-rw-r--r--   0        0        0     3006 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/5-Instructions.py
+-rw-r--r--   0        0        0     1616 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/6-Tasks.py
+-rw-r--r--   0        0        0     1808 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/Login.py
+-rw-r--r--   0        0        0     5603 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/Profile.py
+-rw-r--r--   0        0        0     1828 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/Register.py
+-rw-r--r--   0        0        0      145 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Chat.txt
+-rw-r--r--   0        0        0      175 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0        0        0      991 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Create New Command.txt
+-rw-r--r--   0        0        0     1011 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Execution.txt
+-rw-r--r--   0        0        0     1172 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Instruction.txt
+-rw-r--r--   0        0        0      372 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0        0        0      170 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0        0        0      424 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0        0        0      326 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Prioritize.txt
+-rw-r--r--   0        0        0      236 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0        0        0      343 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0        0        0      268 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0        0        0      298 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0        0        0      142 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0        0        0      468 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0        0        0      522 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0        0        0      452 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0        0        0      427 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0        0        0      154 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0        0        0      501 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0        0        0      554 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0        0        0      186 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0        0        0      155 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0        0        0      162 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0        0        0      308 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Validation.txt
+-rw-r--r--   0        0        0      850 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0        0        0      308 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/WebSearch.txt
+-rw-r--r--   0        0        0       28 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Write a Poem.txt
+-rw-r--r--   0        0        0     1172 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
+-rw-r--r--   0        0        0     1172 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0        0        0      771 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/instruct.txt
+-rw-r--r--   0        0        0      818 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/starchat/instruct.txt
+-rw-r--r--   0        0        0      610 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/vicuna/instruct.txt
+-rw-r--r--   0        0        0     2147 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/__init__.py
+-rw-r--r--   0        0        0     1611 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/azure.py
+-rw-r--r--   0        0        0      487 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/bard.py
+-rw-r--r--   0        0        0     2050 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/bing.py
+-rw-r--r--   0        0        0      974 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/chatgpt.py
+-rw-r--r--   0        0        0     1006 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/claude.py
+-rw-r--r--   0        0        0      757 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/fastchat.py
+-rw-r--r--   0        0        0      867 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/gpt4all.py
+-rw-r--r--   0        0        0     4491 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/gpt4free.py
+-rw-r--r--   0        0        0     1188 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0        0        0     1001 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/huggingchat.py
+-rw-r--r--   0        0        0     1432 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/huggingface.py
+-rw-r--r--   0        0        0     1085 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/kobold.py
+-rw-r--r--   0        0        0     1939 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/llamacpp.py
+-rw-r--r--   0        0        0     2177 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0        0        0     1579 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/oobabooga.py
+-rw-r--r--   0        0        0     1464 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/openai.py
+-rw-r--r--   0        0        0      844 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/palm.py
+-rw-r--r--   0        0        0     3826 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/runpod.py
+-rw-r--r--   0        0        0     3100 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/transformer.py
+-rw-r--r--   0        0        0      538 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/starchat.sh
+-rw-r--r--   0        0        0     2845 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/test-commands.ipynb
+-rw-r--r--   0        0        0     9929 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/test-memory.ipynb
+-rw-r--r--   0        0        0    13215 2023-06-03 11:55:38.767473 agixt-1.1.80b0/docs/README.md
+-rw-r--r--   0        0        0     2838 2023-06-03 11:55:38.779473 agixt-1.1.80b0/pyproject.toml
+-rw-r--r--   0        0        0    16070 1970-01-01 00:00:00.000000 agixt-1.1.80b0/PKG-INFO
```

### Comparing `agixt-1.1.79b0/LICENSE` & `agixt-1.1.80b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/AGiXT.py` & `agixt-1.1.80b0/agixt/AGiXT.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,14 +52,27 @@
         try:
             with open(os.path.join("chains", f"{chain_name}_responses.json"), "r") as f:
                 responses = json.load(f)
             return responses.get(str(step_number))
         except:
             return ""
 
+    def get_step_content(self, chain_name, step_number, prompt_content):
+        new_prompt_content = {}
+        for arg, value in prompt_content.items():
+            if "{STEP" in value:
+                # get the response from the step number
+                step_response = self.get_step_response(
+                    chain_name=chain_name, step_number=step_number
+                )
+                # replace the {STEPx} with the response
+                value = value.replace(f"{{STEP{step_number}}}", step_response)
+            new_prompt_content[arg] = value
+        return new_prompt_content
+
     async def format_prompt(
         self,
         task: str = "",
         top_results: int = 5,
         prompt="",
         chain_name="",
         step_number=0,
@@ -80,33 +93,48 @@
             try:
                 context = await memories.context_agent(
                     query=task, top_results_num=top_results
                 )
             except:
                 context = "None."
         command_list = self.agent.get_commands_string()
+        if chain_name != "":
+            try:
+                for arg, value in kwargs.items():
+                    if "{STEP" in value:
+                        # get the response from the step number
+                        step_response = self.get_step_response(
+                            chain_name=chain_name, step_number=step_number
+                        )
+                        # replace the {STEPx} with the response
+                        value = value.replace(f"{{STEP{step_number}}}", step_response)
+                        kwargs[arg] = value
+            except:
+                logging.info("No args to replace.")
+            if "{STEP" in prompt:
+                step_response = self.get_step_response(
+                    chain_name=chain_name, step_number=step_number
+                )
+                prompt = prompt.replace(f"{{STEP{step_number}}}", step_response)
+            if "{STEP" in task:
+                step_response = self.get_step_response(
+                    chain_name=chain_name, step_number=step_number
+                )
+                task = task.replace(f"{{STEP{step_number}}}", step_response)
         formatted_prompt = self.custom_format(
-            prompt,
+            string=prompt,
             task=task,
             agent_name=self.agent_name,
             COMMANDS=self.agent_commands,
             context=context,
             command_list=command_list,
             date=datetime.now().strftime("%B %d, %Y %I:%M %p"),
             **kwargs,
         )
-        if "{STEP" in formatted_prompt:
-            # get the response from the step number
-            step_response = self.get_step_response(
-                chain_name=chain_name, step_number=step_number
-            )
-            # replace the {STEPx} with the response
-            formatted_prompt = formatted_prompt.replace(
-                f"{{STEP{step_number}}}", step_response
-            )
+
         if not self.nlp:
             self.load_spacy_model()
         tokens = len(self.nlp(formatted_prompt))
         logging.info(f"FORMATTED PROMPT: {formatted_prompt}")
         return formatted_prompt, prompt, tokens
 
     async def run(
@@ -392,15 +420,15 @@
                 # Search for the command in the available_commands list, and if found, use the command's name attribute for execution
                 if command_name is not None:
                     for available_command in self.agent.available_commands:
                         if command_name in [
                             available_command["friendly_name"],
                             available_command["name"],
                         ]:
-                            command_name = available_command["friendly_name"]
+                            command_name = available_command["name"]
                             try:
                                 # Check if the command is a valid command in the self.avent.available_commands list
                                 command_output = await self.agent.execute(
                                     command_name, command_args
                                 )
                                 logging.info("Running Command Execution Validation...")
                                 validate_command = await self.run(
```

### Comparing `agixt-1.1.79b0/agixt/Agent.py` & `agixt-1.1.80b0/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/Chain.py` & `agixt-1.1.80b0/agixt/Chain.py`

 * *Files 14% similar despite different names*

```diff
@@ -84,17 +84,19 @@
             if "prompt" in step_data and "step" in step_data:
                 logging.info(f"Running step {step_data['step']}")
                 step_response = await self.run_chain_step(
                     step=step_data, chain_name=chain_name
                 )  # Get the response of the current step.
                 responses[step_data["step"]] = step_response  # Store the response.
                 logging.info(f"Response: {step_response}")
-        # Write the responses to the json file.
-        with open(os.path.join("chains", f"{chain_name}_responses.json"), "w") as f:
-            json.dump(responses, f)
+                # Write the responses to the json file.
+                with open(
+                    os.path.join("chains", f"{chain_name}_responses.json"), "w"
+                ) as f:
+                    json.dump(responses, f)
         return responses
 
     def get_step_response(self, chain_name, step_number="all"):
         try:
             with open(os.path.join("chains", f"{chain_name}_responses.json"), "r") as f:
                 responses = json.load(f)
             print(responses)
@@ -103,73 +105,74 @@
             else:
                 return responses.get(str(step_number))
         except:
             return ""
 
     def get_step_content(self, chain_name, step_number, prompt_content):
         new_prompt_content = {}
-        for arg, value in prompt_content.items():
-            if "{STEP" in value:
+        if isinstance(prompt_content, dict):
+            for arg, value in prompt_content.items():
+                if "{STEP" in value:
+                    # Get the step number from value between {STEP and }
+                    new_step_number = int(value.split("{STEP")[1].split("}")[0])
+                    # get the response from the step number
+                    step_response = self.get_step_response(
+                        chain_name=chain_name, step_number=new_step_number
+                    )
+                    # replace the {STEPx} with the response
+                    value = value.replace(f"{{STEP{new_step_number}}}", step_response)
+                new_prompt_content[arg] = value
+        elif isinstance(prompt_content, str):
+            if "{STEP" in prompt_content:
+                # Get the step number from value between {STEP and }
+                new_step_number = int(prompt_content.split("{STEP")[1].split("}")[0])
                 # get the response from the step number
                 step_response = self.get_step_response(
-                    chain_name=chain_name, step_number=step_number
+                    chain_name=chain_name, step_number=new_step_number
                 )
                 # replace the {STEPx} with the response
-                value = value.replace(f"{{STEP{step_number}}}", step_response)
-            new_prompt_content[arg] = value
+                new_prompt_content = prompt_content.replace(
+                    f"{{STEP{new_step_number}}}", step_response
+                )
         return new_prompt_content
 
     async def run_chain_step(self, step: dict = {}, chain_name=""):
         logging.info(step)
         if step:
             if "prompt_type" in step:
-                prompt_type = step["prompt_type"]
-                prompt = step["prompt"]
                 agent_name = step["agent_name"]
                 agent = AGiXT(agent_name)
+                prompt_type = step["prompt_type"]
                 step_number = step["step"]
-                try:
-                    command_name = prompt["command_name"]
-                except:
-                    command_name = ""
+                if "prompt_name" in step["prompt"]:
+                    prompt_name = step["prompt"]["prompt_name"]
+                else:
+                    prompt_name = ""
+                args = self.get_step_content(chain_name, step_number, step["prompt"])
                 if prompt_type == "Command":
-                    commands_args = prompt.copy()
-                    for arg in commands_args:
-                        commands_args[arg] = self.get_step_content(
-                            chain_name, step_number, commands_args[arg]
-                        )
                     return await Extensions(
                         agent_config=agent.agent.agent_config
                     ).execute_command(
-                        command_name=command_name, command_args=commands_args
-                    )
-                try:
-                    prompt_content = Prompts().get_prompt(
-                        prompt_name=prompt["prompt_name"]
-                    )
-                    prompt_content = self.get_step_content(
-                        chain_name, step_number, prompt_content
+                        command_name=args["command_name"], command_args=args
                     )
-                except:
-                    return None
-                if prompt_type == "Prompt":
+                elif prompt_type == "Prompt":
                     result = await agent.run(
-                        prompt=prompt["prompt_name"],
+                        prompt=prompt_name,
                         chain_name=chain_name,
                         step_number=step_number,
-                        **prompt,
+                        **args,
                     )
                 elif prompt_type == "Chain":
-                    result = await self.run_chain(prompt["chain_name"])
+                    result = await self.run_chain(step["prompt"]["chain_name"])
                 elif prompt_type == "Smart Instruct":
-                    result = await agent.smart_instruct(task=prompt_content, **prompt)
+                    result = await agent.smart_instruct(**args)
                 elif prompt_type == "Smart Chat":
-                    result = await agent.smart_chat(task=prompt_content, **prompt)
+                    result = await agent.smart_chat(**args)
                 elif prompt_type == "Task":
-                    result = await agent.run_task(objective=prompt_content, **prompt)
+                    result = await agent.run_task(**args)
         if result:
             return result
         else:
             return None
 
 
 if __name__ == "__main__":
```

### Comparing `agixt-1.1.79b0/agixt/Config.py` & `agixt-1.1.80b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/Embedding.py` & `agixt-1.1.80b0/agixt/Embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,22 +97,22 @@
     async def embed_text(self, text):
         embed, chunk_size = await self.get_embedder()
         return await embed(text)
 
     async def default(self):
         chunk_size = 128
         embed = HuggingFaceTextEmbedding(
-            model_name="all-mpnet-base-v2", log=logging
+            model_id="all-mpnet-base-v2", log=logging
         ).generate_embeddings_async
         return embed, chunk_size
 
     async def large_local(self):
         chunk_size = 500
         embed = HuggingFaceTextEmbedding(
-            model_name="gtr-t5-large", log=logging
+            model_id="gtr-t5-large", log=logging
         ).generate_embeddings_async
         return embed, chunk_size
 
     async def azure(self):
         chunk_size = 1000
         embed = AzureTextEmbedding(
             deployment_name=self.AGENT_CONFIG["settings"]["AZURE_DEPLOYMENT_NAME"],
```

### Comparing `agixt-1.1.79b0/agixt/Extensions.py` & `agixt-1.1.80b0/agixt/Extensions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/Main.py` & `agixt-1.1.80b0/agixt/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/Memories.py` & `agixt-1.1.80b0/agixt/Memories.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self.collection = None
         self.nlp = None
         self.chunk_size = 128
         memories_dir = os.path.join(os.getcwd(), "agents", self.agent_name, "memories")
         self.chroma_client = ChromaMemoryStore(
             persist_directory=memories_dir,
             client_settings=Settings(
-                chroma_db_impl="duckdb+parquet",
+                chroma_db_impl="chromadb.db.duckdb.PersistentDuckDB",
                 persist_directory=memories_dir,
                 anonymized_telemetry=False,
             ),
         )
 
     def load_spacy_model(self):
         if not self.nlp:
```

### Comparing `agixt-1.1.79b0/agixt/Prompts.py` & `agixt-1.1.80b0/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/Tasks.py` & `agixt-1.1.80b0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/app.py` & `agixt-1.1.80b0/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/auth_libs/Cfig.py` & `agixt-1.1.80b0/agixt/auth_libs/Cfig.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/auth_libs/Redirect.py` & `agixt-1.1.80b0/agixt/auth_libs/Redirect.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/auth_libs/Users.py` & `agixt-1.1.80b0/agixt/auth_libs/Users.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/chains/Smart Chat.json` & `agixt-1.1.80b0/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/chains/Test_Commands.json` & `agixt-1.1.80b0/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/components/agent_selector.py` & `agixt-1.1.80b0/agixt/components/agent_selector.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/example.ipynb` & `agixt-1.1.80b0/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/agixt_agent.py` & `agixt-1.1.80b0/agixt/extensions/agixt_agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/briantts.py` & `agixt-1.1.80b0/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/dalle.py` & `agixt-1.1.80b0/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/discord.py` & `agixt-1.1.80b0/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/elevenlabs.py` & `agixt-1.1.80b0/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/file_system.py` & `agixt-1.1.80b0/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/github.py` & `agixt-1.1.80b0/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/google.py` & `agixt-1.1.80b0/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/gtts.py` & `agixt-1.1.80b0/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/huggingface.py` & `agixt-1.1.80b0/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/macostts.py` & `agixt-1.1.80b0/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/microsoft_365.py` & `agixt-1.1.80b0/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/searxng.py` & `agixt-1.1.80b0/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/sendgrid_email.py` & `agixt-1.1.80b0/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/twitter.py` & `agixt-1.1.80b0/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/extensions/web_playwright.py` & `agixt-1.1.80b0/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/pages/0-Agent_Settings.py` & `agixt-1.1.80b0/agixt/pages/0-Agent_Settings.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/pages/1-Learning.py` & `agixt-1.1.80b0/agixt/pages/1-Learning.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/pages/2-Prompts.py` & `agixt-1.1.80b0/agixt/pages/2-Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/pages/3-Chains.py` & `agixt-1.1.80b0/agixt/pages/3-Chains.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 st.header("Manage Chains")
 st.markdown("### Predefined Injection Variables")
 st.markdown(
     """
     Any of these variables can be used in command arguments or prompt arguments to inject data into the prompt. These can also be used inside of any Custom Prompt.
 - `{agent_name}` will cause the agent name to be injected.
-- `{context}` will cause the current context from memory to be injected.
+- `{context}` will cause the current context from memory to be injected. (Only applies to prompts but is still a reserved variable name.)
 - `{date}` will cause the current date and timestamp to be injected.
 - `{COMMANDS}` will cause the available commands list to be injected and for automatic commands execution from the agent based on its suggestions.
 - `{command_list}` will cause the available commands list to be injected, but will not execute any commands the AI chooses. Useful on validation steps.
 - `{STEPx}` will cause the step `x` response from a chain to be injected. For example, `{STEP1}` will inject the first step's response in a chain.
 """
 )
 
@@ -150,43 +150,57 @@
                 index=available_prompts.index(prompt.get("prompt_name", "")) + 1
                 if "prompt_name" in prompt
                 else 0,
             )
 
             if modify_prompt_name:
                 prompt_args = Prompts().get_prompt_args(modify_prompt_name)
-                formatted_prompt_args = ", ".join(
-                    [
-                        f"{arg}: {st.text_input(arg, value=prompt.get(arg, ''), key=f'{arg}_{step_number}')} "
-                        for arg in prompt_args
-                        if arg != "context"
-                        and arg != "command_list"
-                        and arg != "COMMANDS"
-                    ]
-                )
-                modify_prompt = f"{modify_prompt_name}({formatted_prompt_args})"
+                if prompt_args:
+                    if isinstance(prompt_args, str):
+                        prompt_args = [prompt_args]
+                    try:
+                        modify_prompt["prompt_name"] = modify_prompt_name
+                        for arg in prompt_args:
+                            if (
+                                arg != "context"
+                                and arg != "command_list"
+                                and arg != "COMMANDS"
+                            ):
+                                modify_prompt[arg] = st.text_input(
+                                    arg,
+                                    value=prompt.get(arg, "") if arg in prompt else "",
+                                    key=f"{arg}_{step_number}",
+                                )
+                    except:
+                        pass
         else:
             modify_prompt = ""
 
         if st.button("Modify Step", key=f"modify_{step_number}"):
+            modify_prompt = {}
+            if modify_prompt_type == "Command":
+                modify_prompt["command_name"] = command_name
+                for arg in command_args:
+                    if arg != "context" and arg != "command_list" and arg != "COMMANDS":
+                        modify_prompt[arg] = st.session_state[f"{arg}_{step_number}"]
+            elif modify_prompt_type == "Prompt":
+                modify_prompt["prompt_name"] = modify_prompt_name
+                for arg in prompt_args:
+                    if arg != "context" and arg != "command_list" and arg != "COMMANDS":
+                        modify_prompt[arg] = st.session_state[f"{arg}_{step_number}"]
+
             Chain().update_step(
-                selected_chain_name,
-                step_number,
-                modify_agent_name,
-                modify_prompt_type,
-                modify_prompt,
+                chain_name=selected_chain_name,
+                step_number=step_number,
+                agent_name=modify_agent_name,
+                prompt_type=modify_prompt_type,
+                prompt=modify_prompt,
             )
             st.success(f"Step {step_number} updated in chain '{selected_chain_name}'.")
             st.experimental_rerun()
-            return {
-                "step": modify_step_number,
-                "agent_name": modify_agent_name,
-                "prompt_type": modify_prompt_type,
-                "prompt": modify_prompt,
-            }
         return step
 
     st.write("Existing Steps:")
     if chain:
         for step in chain:
             if step is not None:
                 try:
@@ -262,15 +276,26 @@
         if (
             selected_chain_name
             and step_number
             and agent_name
             and prompt_type
             and prompt
         ):
-            if step_action == "Add Step":
+            prompt_data = {}
+            if prompt_type == "Command":
+                prompt_data["command_name"] = command_name
+                for arg in command_args:
+                    if arg != "context" and arg != "command_list" and arg != "COMMANDS":
+                        prompt_data[arg] = st.session_state[f"add_step_{arg}"]
+            elif prompt_type == "Prompt":
+                prompt_data["prompt_name"] = prompt_name
+                for arg in prompt_args:
+                    if arg != "context" and arg != "command_list" and arg != "COMMANDS":
+                        prompt_data[arg] = st.session_state[f"add_step_{arg}"]
+            elif step_action == "Update Step":
                 if prompt_type == "Command":
                     prompt_data = {"command_name": command_name}
                     for arg in command_args:
                         if (
                             arg != "context"
                             and arg != "command_list"
                             and arg != "COMMANDS"
@@ -282,53 +307,22 @@
                         if (
                             arg != "context"
                             and arg != "command_list"
                             and arg != "COMMANDS"
                         ):
                             prompt_data[arg] = st.session_state[f"add_step_{arg}"]
 
-                Chain().add_chain_step(
+                Chain().update_step(
                     chain_name=selected_chain_name,
                     step_number=step_number,
                     agent_name=agent_name,
                     prompt_type=prompt_type,
                     prompt=prompt_data,
                 )
                 st.success(
-                    f"Step {step_number} added to chain '{selected_chain_name}'."
-                )
-                st.experimental_rerun()
-            elif step_action == "Update Step":
-                if prompt_type == "Command":
-                    prompt_data = {"command_name": command_name}
-                    for arg in command_args:
-                        if (
-                            arg != "context"
-                            and arg != "command_list"
-                            and arg != "COMMANDS"
-                        ):
-                            prompt_data[arg] = st.session_state[f"add_step_{arg}"]
-                elif prompt_type == "Prompt":
-                    prompt_data = {"prompt_name": prompt_name}
-                    for arg in prompt_args:
-                        if (
-                            arg != "context"
-                            and arg != "command_list"
-                            and arg != "COMMANDS"
-                        ):
-                            prompt_data[arg] = st.session_state[f"add_step_{arg}"]
-
-                Chain().update_step(
-                    selected_chain_name,
-                    step_number,
-                    agent_name,
-                    prompt_type,
-                    prompt_data,
-                )
-                st.success(
                     f"Step {step_number} updated in chain '{selected_chain_name}'."
                 )
                 st.experimental_rerun()
             elif step_action == "Delete Step":
                 Chain().delete_step(selected_chain_name, step_number)
                 st.success(
                     f"Step {step_number} deleted from chain '{selected_chain_name}'."
```

### Comparing `agixt-1.1.79b0/agixt/pages/4-Chat.py` & `agixt-1.1.80b0/agixt/pages/4-Chat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/pages/5-Instructions.py` & `agixt-1.1.80b0/agixt/pages/5-Instructions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/pages/6-Tasks.py` & `agixt-1.1.80b0/agixt/pages/6-Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/pages/Login.py` & `agixt-1.1.80b0/agixt/pages/Login.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/pages/Profile.py` & `agixt-1.1.80b0/agixt/pages/Profile.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/pages/Register.py` & `agixt-1.1.80b0/agixt/pages/Register.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/prompts/Create New Command.txt` & `agixt-1.1.80b0/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/prompts/Execution.txt` & `agixt-1.1.80b0/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/prompts/Instruction.txt` & `agixt-1.1.80b0/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.1.80b0/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.1.80b0/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/prompts/ValidationFailed.txt` & `agixt-1.1.80b0/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.1.80b0/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.1.80b0/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/prompts/instruct.txt` & `agixt-1.1.80b0/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/prompts/starchat/instruct.txt` & `agixt-1.1.80b0/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/prompts/vicuna/instruct.txt` & `agixt-1.1.80b0/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/__init__.py` & `agixt-1.1.80b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/azure.py` & `agixt-1.1.80b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/bing.py` & `agixt-1.1.80b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/chatgpt.py` & `agixt-1.1.80b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/claude.py` & `agixt-1.1.80b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/fastchat.py` & `agixt-1.1.80b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/gpt4all.py` & `agixt-1.1.80b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/gpt4free.py` & `agixt-1.1.80b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.80b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/huggingchat.py` & `agixt-1.1.80b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/huggingface.py` & `agixt-1.1.80b0/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/kobold.py` & `agixt-1.1.80b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/llamacpp.py` & `agixt-1.1.80b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/llamacppapi.py` & `agixt-1.1.80b0/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/oobabooga.py` & `agixt-1.1.80b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/openai.py` & `agixt-1.1.80b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/palm.py` & `agixt-1.1.80b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/runpod.py` & `agixt-1.1.80b0/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/provider/transformer.py` & `agixt-1.1.80b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/starchat.sh` & `agixt-1.1.80b0/agixt/starchat.sh`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/agixt/test-commands.ipynb` & `agixt-1.1.80b0/agixt/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/docs/README.md` & `agixt-1.1.80b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.79b0/pyproject.toml` & `agixt-1.1.80b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AGiXT"
-version = "v1.1.79-beta"
+version = "v1.1.80-beta"
 description = "An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day."
 homepage = "https://AGiXT.com"
 documentation = "https://AGiXT.com"
 keywords = ["AI", "AGI", "Agent", "skynet"]
 license = "MIT"
 authors = ["Josh XT <josh@devxt.com>"]
 maintainers = [
```

### Comparing `agixt-1.1.79b0/PKG-INFO` & `agixt-1.1.80b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.79b0
+Version: 1.1.80b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Home-page: https://AGiXT.com
 License: MIT
 Keywords: AI,AGI,Agent,skynet
 Author: Josh XT
 Author-email: josh@devxt.com
 Maintainer: localAGI
```

