# Comparing `tmp/agixt-1.1.80b0.tar.gz` & `tmp/agixt-1.1.81b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.80b0.tar", max compression
+gzip compressed data, was "agixt-1.1.81b0.tar", max compression
```

## Comparing `agixt-1.1.80b0.tar` & `agixt-1.1.81b0.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0     1087 2023-06-03 11:55:38.759473 agixt-1.1.80b0/LICENSE
--rw-r--r--   0        0        0    21022 2023-06-03 11:55:38.759473 agixt-1.1.80b0/agixt/AGiXT.py
--rw-r--r--   0        0        0    24299 2023-06-03 11:55:38.759473 agixt-1.1.80b0/agixt/Agent.py
--rw-r--r--   0        0        0     7564 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Chain.py
--rw-r--r--   0        0        0     1101 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Config.py
--rw-r--r--   0        0        0     5900 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Embedding.py
--rw-r--r--   0        0        0     6474 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Extensions.py
--rw-r--r--   0        0        0      606 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Main.py
--rw-r--r--   0        0        0     9647 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Memories.py
--rw-r--r--   0        0        0     1943 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Prompts.py
--rw-r--r--   0        0        0     7099 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/Tasks.py
--rw-r--r--   0        0        0       38 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/WORKSPACE/example.txt
--rw-r--r--   0        0        0      230 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/__init__.py
--rw-r--r--   0        0        0      244 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/agents/gpt4free/config.json
--rw-r--r--   0        0        0        0 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/agents/gpt4free.yaml
--rw-r--r--   0        0        0    12707 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/app.py
--rw-r--r--   0        0        0     1793 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/auth_libs/Cfig.py
--rw-r--r--   0        0        0     1165 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/auth_libs/Redirect.py
--rw-r--r--   0        0        0     4261 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/auth_libs/Users.py
--rw-r--r--   0        0        0     2012 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/chains/Smart Chat.json
--rw-r--r--   0        0        0    10644 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/chains/Test_Commands.json
--rw-r--r--   0        0        0      566 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/chains/Write a Poem.json
--rw-r--r--   0        0        0      959 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/chains/Write a Poem_responses.json
--rw-r--r--   0        0        0     1566 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/components/agent_selector.py
--rw-r--r--   0        0        0       42 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/config.yaml
--rw-r--r--   0        0        0    11935 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/example.ipynb
--rw-r--r--   0        0        0     6026 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/agixt_agent.py
--rw-r--r--   0        0        0      860 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/briantts.py
--rw-r--r--   0        0        0     1174 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/dalle.py
--rw-r--r--   0        0        0     2818 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/discord.py
--rw-r--r--   0        0        0     1170 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/elevenlabs.py
--rw-r--r--   0        0        0     6647 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/file_system.py
--rw-r--r--   0        0        0     1841 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/github.py
--rw-r--r--   0        0        0     2042 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/google.py
--rw-r--r--   0        0        0      539 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/gtts.py
--rw-r--r--   0        0        0     2475 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/huggingface.py
--rw-r--r--   0        0        0      622 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/macostts.py
--rw-r--r--   0        0        0     4236 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/microsoft_365.py
--rw-r--r--   0        0        0     1899 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/searxng.py
--rw-r--r--   0        0        0     1001 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/sendgrid_email.py
--rw-r--r--   0        0        0      315 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/times.py
--rw-r--r--   0        0        0     1169 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/twitter.py
--rw-r--r--   0        0        0     2287 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/extensions/web_playwright.py
--rw-r--r--   0        0        0    10464 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/0-Agent_Settings.py
--rw-r--r--   0        0        0     2035 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/1-Learning.py
--rw-r--r--   0        0        0     2491 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/2-Prompts.py
--rw-r--r--   0        0        0    13672 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/3-Chains.py
--rw-r--r--   0        0        0     2909 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/4-Chat.py
--rw-r--r--   0        0        0     3006 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/5-Instructions.py
--rw-r--r--   0        0        0     1616 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/6-Tasks.py
--rw-r--r--   0        0        0     1808 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/Login.py
--rw-r--r--   0        0        0     5603 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/Profile.py
--rw-r--r--   0        0        0     1828 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/pages/Register.py
--rw-r--r--   0        0        0      145 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Chat.txt
--rw-r--r--   0        0        0      175 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0        0        0      991 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Create New Command.txt
--rw-r--r--   0        0        0     1011 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Execution.txt
--rw-r--r--   0        0        0     1172 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Instruction.txt
--rw-r--r--   0        0        0      372 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0        0        0      170 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0        0        0      424 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0        0        0      326 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Prioritize.txt
--rw-r--r--   0        0        0      236 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0        0        0      343 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0        0        0      268 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0        0        0      298 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0        0        0      142 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0        0        0      468 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0        0        0      522 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0        0        0      452 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0        0        0      427 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0        0        0      154 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0        0        0      501 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0        0        0      554 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0        0        0      186 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0        0        0      155 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Tell Me How.txt
--rw-r--r--   0        0        0      162 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Title a Poem.txt
--rw-r--r--   0        0        0      308 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Validation.txt
--rw-r--r--   0        0        0      850 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0        0        0      308 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/WebSearch.txt
--rw-r--r--   0        0        0       28 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/Write a Poem.txt
--rw-r--r--   0        0        0     1172 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
--rw-r--r--   0        0        0     1172 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0        0        0      771 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/instruct.txt
--rw-r--r--   0        0        0      818 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/starchat/instruct.txt
--rw-r--r--   0        0        0      610 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/prompts/vicuna/instruct.txt
--rw-r--r--   0        0        0     2147 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/__init__.py
--rw-r--r--   0        0        0     1611 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/azure.py
--rw-r--r--   0        0        0      487 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/bard.py
--rw-r--r--   0        0        0     2050 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/bing.py
--rw-r--r--   0        0        0      974 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/chatgpt.py
--rw-r--r--   0        0        0     1006 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/claude.py
--rw-r--r--   0        0        0      757 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/fastchat.py
--rw-r--r--   0        0        0      867 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/gpt4all.py
--rw-r--r--   0        0        0     4491 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/gpt4free.py
--rw-r--r--   0        0        0     1188 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0        0        0     1001 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/huggingchat.py
--rw-r--r--   0        0        0     1432 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/huggingface.py
--rw-r--r--   0        0        0     1085 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/kobold.py
--rw-r--r--   0        0        0     1939 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/llamacpp.py
--rw-r--r--   0        0        0     2177 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/llamacppapi.py
--rw-r--r--   0        0        0     1579 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/oobabooga.py
--rw-r--r--   0        0        0     1464 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/openai.py
--rw-r--r--   0        0        0      844 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/palm.py
--rw-r--r--   0        0        0     3826 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/runpod.py
--rw-r--r--   0        0        0     3100 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/provider/transformer.py
--rw-r--r--   0        0        0      538 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/starchat.sh
--rw-r--r--   0        0        0     2845 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/test-commands.ipynb
--rw-r--r--   0        0        0     9929 2023-06-03 11:55:38.763473 agixt-1.1.80b0/agixt/test-memory.ipynb
--rw-r--r--   0        0        0    13215 2023-06-03 11:55:38.767473 agixt-1.1.80b0/docs/README.md
--rw-r--r--   0        0        0     2838 2023-06-03 11:55:38.779473 agixt-1.1.80b0/pyproject.toml
--rw-r--r--   0        0        0    16070 1970-01-01 00:00:00.000000 agixt-1.1.80b0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-03 13:06:26.929239 agixt-1.1.81b0/LICENSE
+-rw-r--r--   0        0        0    21022 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/AGiXT.py
+-rw-r--r--   0        0        0    24299 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Agent.py
+-rw-r--r--   0        0        0     8781 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Chain.py
+-rw-r--r--   0        0        0     1101 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Config.py
+-rw-r--r--   0        0        0     5900 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Embedding.py
+-rw-r--r--   0        0        0     6474 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Extensions.py
+-rw-r--r--   0        0        0      606 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Main.py
+-rw-r--r--   0        0        0     9492 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Memories.py
+-rw-r--r--   0        0        0     1943 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Prompts.py
+-rw-r--r--   0        0        0     7099 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/Tasks.py
+-rw-r--r--   0        0        0       38 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/WORKSPACE/example.txt
+-rw-r--r--   0        0        0      230 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/__init__.py
+-rw-r--r--   0        0        0      244 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/agents/gpt4free/config.json
+-rw-r--r--   0        0        0        0 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/agents/gpt4free.yaml
+-rw-r--r--   0        0        0    13452 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/app.py
+-rw-r--r--   0        0        0     1793 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/auth_libs/Cfig.py
+-rw-r--r--   0        0        0     1165 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/auth_libs/Redirect.py
+-rw-r--r--   0        0        0     4261 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/auth_libs/Users.py
+-rw-r--r--   0        0        0     2012 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/chains/Smart Chat.json
+-rw-r--r--   0        0        0    10644 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/chains/Test_Commands.json
+-rw-r--r--   0        0        0      566 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/chains/Write a Poem.json
+-rw-r--r--   0        0        0      959 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/chains/Write a Poem_responses.json
+-rw-r--r--   0        0        0     1566 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/components/agent_selector.py
+-rw-r--r--   0        0        0       42 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/config.yaml
+-rw-r--r--   0        0        0    11935 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/example.ipynb
+-rw-r--r--   0        0        0     6026 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/agixt_agent.py
+-rw-r--r--   0        0        0      860 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/briantts.py
+-rw-r--r--   0        0        0     1174 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/dalle.py
+-rw-r--r--   0        0        0     2818 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/discord.py
+-rw-r--r--   0        0        0     1170 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/elevenlabs.py
+-rw-r--r--   0        0        0     6647 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/file_system.py
+-rw-r--r--   0        0        0     1841 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/github.py
+-rw-r--r--   0        0        0     2042 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/google.py
+-rw-r--r--   0        0        0      539 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/gtts.py
+-rw-r--r--   0        0        0     2475 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/huggingface.py
+-rw-r--r--   0        0        0      622 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/macostts.py
+-rw-r--r--   0        0        0     4236 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/microsoft_365.py
+-rw-r--r--   0        0        0     1899 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/searxng.py
+-rw-r--r--   0        0        0     1001 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0        0        0      315 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/times.py
+-rw-r--r--   0        0        0     1169 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/twitter.py
+-rw-r--r--   0        0        0     2287 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/extensions/web_playwright.py
+-rw-r--r--   0        0        0    10464 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/0-Agent_Settings.py
+-rw-r--r--   0        0        0     2035 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/1-Learning.py
+-rw-r--r--   0        0        0     2491 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/2-Prompts.py
+-rw-r--r--   0        0        0    13672 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/3-Chains.py
+-rw-r--r--   0        0        0     2909 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/4-Chat.py
+-rw-r--r--   0        0        0     3006 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/5-Instructions.py
+-rw-r--r--   0        0        0     1616 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/6-Tasks.py
+-rw-r--r--   0        0        0     1808 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/Login.py
+-rw-r--r--   0        0        0     5603 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/Profile.py
+-rw-r--r--   0        0        0     1828 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/pages/Register.py
+-rw-r--r--   0        0        0      145 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Chat.txt
+-rw-r--r--   0        0        0      175 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0        0        0      991 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Create New Command.txt
+-rw-r--r--   0        0        0     1011 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Execution.txt
+-rw-r--r--   0        0        0     1172 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Instruction.txt
+-rw-r--r--   0        0        0      372 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0        0        0      170 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0        0        0      424 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0        0        0      326 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Prioritize.txt
+-rw-r--r--   0        0        0      236 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0        0        0      343 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0        0        0      268 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0        0        0      298 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0        0        0      142 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0        0        0      468 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0        0        0      522 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0        0        0      452 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0        0        0      427 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0        0        0      154 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0        0        0      501 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0        0        0      554 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0        0        0      186 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0        0        0      155 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0        0        0      162 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0        0        0      308 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Validation.txt
+-rw-r--r--   0        0        0      850 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0        0        0      308 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/WebSearch.txt
+-rw-r--r--   0        0        0       28 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/Write a Poem.txt
+-rw-r--r--   0        0        0     1172 2023-06-03 13:06:26.929239 agixt-1.1.81b0/agixt/prompts/gpt-3.5-turbo/instruct.txt
+-rw-r--r--   0        0        0     1172 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0        0        0      771 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/prompts/instruct.txt
+-rw-r--r--   0        0        0      818 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/prompts/starchat/instruct.txt
+-rw-r--r--   0        0        0      610 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/prompts/vicuna/instruct.txt
+-rw-r--r--   0        0        0     2147 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/__init__.py
+-rw-r--r--   0        0        0     1611 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/azure.py
+-rw-r--r--   0        0        0      487 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/bard.py
+-rw-r--r--   0        0        0     2050 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/bing.py
+-rw-r--r--   0        0        0      974 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/chatgpt.py
+-rw-r--r--   0        0        0     1006 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/claude.py
+-rw-r--r--   0        0        0      757 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/fastchat.py
+-rw-r--r--   0        0        0      867 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/gpt4all.py
+-rw-r--r--   0        0        0     4491 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/gpt4free.py
+-rw-r--r--   0        0        0     1188 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0        0        0     1001 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/huggingchat.py
+-rw-r--r--   0        0        0     1432 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/huggingface.py
+-rw-r--r--   0        0        0     1085 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/kobold.py
+-rw-r--r--   0        0        0     2042 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/llamacpp.py
+-rw-r--r--   0        0        0      969 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0        0        0     1579 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/oobabooga.py
+-rw-r--r--   0        0        0     1464 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/openai.py
+-rw-r--r--   0        0        0      844 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/palm.py
+-rw-r--r--   0        0        0     3826 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/runpod.py
+-rw-r--r--   0        0        0     3100 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/provider/transformer.py
+-rw-r--r--   0        0        0      538 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/starchat.sh
+-rw-r--r--   0        0        0     2845 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/test-commands.ipynb
+-rw-r--r--   0        0        0     9929 2023-06-03 13:06:26.933240 agixt-1.1.81b0/agixt/test-memory.ipynb
+-rw-r--r--   0        0        0    13198 2023-06-03 13:06:26.933240 agixt-1.1.81b0/docs/README.md
+-rw-r--r--   0        0        0     2838 2023-06-03 13:06:26.945243 agixt-1.1.81b0/pyproject.toml
+-rw-r--r--   0        0        0    16053 1970-01-01 00:00:00.000000 agixt-1.1.81b0/PKG-INFO
```

### Comparing `agixt-1.1.80b0/LICENSE` & `agixt-1.1.81b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/AGiXT.py` & `agixt-1.1.81b0/agixt/AGiXT.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/Agent.py` & `agixt-1.1.81b0/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/Chain.py` & `agixt-1.1.81b0/agixt/Chain.py`

 * *Files 16% similar despite different names*

```diff
@@ -72,14 +72,40 @@
                 return step
         return None
 
     def get_steps(self, chain_name):
         chain_data = self.get_chain(chain_name=chain_name)
         return chain_data["steps"]
 
+    def move_step(self, chain_name, current_step_number, new_step_number):
+        chain_data = self.get_chain(chain_name=chain_name)
+        if not 1 <= new_step_number <= len(
+            chain_data["steps"]
+        ) or current_step_number not in [step["step"] for step in chain_data["steps"]]:
+            print(f"Error: Invalid step numbers.")
+            return
+        moved_step = None
+        for step in chain_data["steps"]:
+            if step["step"] == current_step_number:
+                moved_step = step
+                chain_data["steps"].remove(step)
+                break
+        for step in chain_data["steps"]:
+            if new_step_number < current_step_number:
+                if new_step_number <= step["step"] < current_step_number:
+                    step["step"] += 1
+            else:
+                if current_step_number < step["step"] <= new_step_number:
+                    step["step"] -= 1
+        moved_step["step"] = new_step_number
+        chain_data["steps"].append(moved_step)
+        chain_data["steps"] = sorted(chain_data["steps"], key=lambda x: x["step"])
+        with open(os.path.join("chains", f"{chain_name}.json"), "w") as f:
+            json.dump(chain_data, f)
+
     async def run_chain(self, chain_name):
         chain_data = self.get_chain(chain_name=chain_name)
         logging.info(f"Running chain '{chain_name}'")
         responses = {}  # Create a dictionary to hold responses.
         for step_data in chain_data["steps"]:
             if "prompt" in step_data and "step" in step_data:
                 logging.info(f"Running step {step_data['step']}")
```

### Comparing `agixt-1.1.80b0/agixt/Config.py` & `agixt-1.1.81b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/Embedding.py` & `agixt-1.1.81b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/Extensions.py` & `agixt-1.1.81b0/agixt/Extensions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/Main.py` & `agixt-1.1.81b0/agixt/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/Memories.py` & `agixt-1.1.81b0/agixt/Memories.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,18 +93,14 @@
             await self.chroma_client.upsert_async(
                 collection_name="memories",
                 record=record,
             )
             self.chroma_client._client.persist()
         except Exception as e:
             logging.info(f"Failed to store memory: {e}")
-        try:
-            self.chroma_client._client.close()
-        except Exception as e:
-            logging.info(f"Failed to close chroma client: {e}")
 
     async def store_result(
         self, task_name: str, result: str, external_source_name: str = None
     ):
         if result:
             if not isinstance(result, str):
                 result = str(result)
```

### Comparing `agixt-1.1.80b0/agixt/Prompts.py` & `agixt-1.1.81b0/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/Tasks.py` & `agixt-1.1.81b0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/app.py` & `agixt-1.1.81b0/agixt/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,301 +112,314 @@
 async def get_providers():
     providers = CFG.get_providers()
     return {"providers": providers}
 
 
 @app.get("/api/provider/{provider_name}", tags=["Provider"])
 async def get_provider_settings(provider_name: str):
-    settings = get_provider_options(provider_name)
+    settings = get_provider_options(provider_name=provider_name)
     return {"settings": settings}
 
 
 @app.get("/api/embedding_providers", tags=["Provider"])
 async def get_embed_providers():
     providers = get_embedding_providers()
     return {"providers": providers}
 
 
 @app.post("/api/agent", tags=["Agent"])
 async def add_agent(agent: AgentSettings) -> Dict[str, str]:
-    agent_info = Agent(agent.agent_name).add_agent(agent.agent_name, agent.settings)
+    agent_info = Agent(agent.agent_name).add_agent(
+        agent_name=agent.agent_name, provider_settings=agent.settings
+    )
     return {"message": "Agent added", "agent_file": agent_info["agent_file"]}
 
 
 @app.patch("/api/agent/{agent_name}", tags=["Agent"])
 async def rename_agent(agent_name: str, new_name: AgentNewName) -> ResponseMessage:
-    Agent(agent_name).rename_agent(agent_name, new_name.new_name)
+    Agent(agent_name=agent_name).rename_agent(
+        agent_name=agent_name, new_name=new_name.new_name
+    )
     return ResponseMessage(
         message=f"Agent {agent_name} renamed to {new_name.new_name}."
     )
 
 
 @app.put("/api/agent/{agent_name}", tags=["Agent"])
 async def update_agent_settings(
     agent_name: str, settings: AgentSettings
 ) -> ResponseMessage:
-    update_config = Agent(agent_name).update_agent_config(settings.settings, "settings")
+    update_config = Agent(agent_name=agent_name).update_agent_config(
+        new_config=settings.settings, config_key="settings"
+    )
     return ResponseMessage(message=update_config)
 
 
 @app.delete("/api/agent/{agent_name}", tags=["Agent"])
 async def delete_agent(agent_name: str) -> ResponseMessage:
-    result, status_code = Agent(agent_name).delete_agent(agent_name)
+    result, status_code = Agent(agent_name=agent_name).delete_agent(
+        agent_name=agent_name
+    )
     if status_code == 200:
         return ResponseMessage(message=result["message"])
     else:
         raise HTTPException(status_code=status_code, detail=result["message"])
 
 
 @app.get("/api/agent", tags=["Agent"])
 async def get_agents():
     agents = CFG.get_agents()
     return {"agents": agents}
 
 
 @app.get("/api/agent/{agent_name}", tags=["Agent"])
 async def get_agentconfig(agent_name: str):
-    agent_config = Agent(agent_name).get_agent_config()
+    agent_config = Agent(agent_name=agent_name).get_agent_config()
     return {"agent": agent_config}
 
 
 @app.get("/api/{agent_name}/chat", tags=["Agent"])
 async def get_chat_history(agent_name: str):
-    chat_history = Agent(agent_name).get_chat_history(agent_name)
+    chat_history = Agent(agent_name=agent_name).get_chat_history(agent_name=agent_name)
     return {"chat_history": chat_history}
 
 
 @app.delete("/api/agent/{agent_name}/memory", tags=["Agent"])
 async def wipe_agent_memories(agent_name: str) -> ResponseMessage:
-    Agent(agent_name).wipe_agent_memories(agent_name)
+    Agent(agent_name=agent_name).wipe_agent_memories(agent_name=agent_name)
     return ResponseMessage(message=f"Memories for agent {agent_name} deleted.")
 
 
 @app.post("/api/agent/{agent_name}/instruct", tags=["Agent"])
 async def instruct(agent_name: str, prompt: Prompt):
-    agent = AGiXT(agent_name)
+    agent = AGiXT(agent_name=agent_name)
     response = await agent.run(
         task=prompt.prompt,
         prompt="instruct",
     )
     return {"response": str(response)}
 
 
 @app.post("/api/agent/{agent_name}/smartinstruct/{shots}", tags=["Agent"])
 async def smartinstruct(agent_name: str, shots: int, prompt: Prompt):
-    agent = AGiXT(agent_name)
+    agent = AGiXT(agent_name=agent_name)
     response = await agent.smart_instruct(task=prompt.prompt, shots=int(shots))
     return {"response": str(response)}
 
 
 @app.post("/api/agent/{agent_name}/chat", tags=["Agent"])
 async def chat(agent_name: str, prompt: Prompt):
-    agent = AGiXT(agent_name)
-    response = await agent.run(prompt.prompt, prompt="Chat", context_results=6)
+    agent = AGiXT(agent_name=agent_name)
+    response = await agent.run(task=prompt.prompt, prompt="Chat", context_results=6)
     return {"response": str(response)}
 
 
 @app.post("/api/agent/{agent_name}/smartchat/{shots}", tags=["Agent"])
 async def smartchat(agent_name: str, shots: int, prompt: Prompt):
-    agent = AGiXT(agent_name)
-    response = await agent.smart_chat(prompt.prompt, shots=shots)
+    agent = AGiXT(agent_name=agent_name)
+    response = await agent.smart_chat(task=prompt.prompt, shots=shots)
     return {"response": str(response)}
 
 
 @app.get("/api/agent/{agent_name}/command", tags=["Agent"])
 async def get_commands(agent_name: str):
-    agent = Agent(agent_name)
+    agent = Agent(agent_name=agent_name)
     return {"commands": agent.agent_config["commands"]}
 
 
 @app.patch("/api/agent/{agent_name}/command", tags=["Agent"])
 async def toggle_command(
     agent_name: str, payload: ToggleCommandPayload
 ) -> ResponseMessage:
-    agent = Agent(agent_name)
+    agent = Agent(agent_name=agent_name)
     print(payload)
     try:
         if payload.command_name == "*":
             for each_command_name in agent.agent_config["commands"]:
                 agent.agent_config["commands"][each_command_name] = payload.enable
 
-            agent.update_agent_config(agent.agent_config["commands"], "commands")
+            agent.update_agent_config(
+                new_config=agent.agent_config["commands"], config_key="commands"
+            )
             return ResponseMessage(
                 message=f"All commands enabled for agent '{agent_name}'."
             )
         else:
             agent.agent_config["commands"][payload.command_name] = payload.enable
-            agent.update_agent_config(agent.agent_config["commands"], "commands")
+            agent.update_agent_config(
+                new_config=agent.agent_config["commands"], config_key="commands"
+            )
             return ResponseMessage(
                 message=f"Command '{payload.command_name}' toggled for agent '{agent_name}'."
             )
     except Exception as e:
         logging.info(e)
         raise HTTPException(
             status_code=500,
             detail=f"Error enabling all commands for agent '{agent_name}': {str(e)}",
         )
 
 
 @app.post("/api/agent/{agent_name}/task", tags=["Agent"])
 async def start_task_agent(agent_name: str, objective: Objective) -> ResponseMessage:
+    task = Tasks(agent_name=agent_name)
     # If it's running stop it.
-    task_status = Tasks(agent_name).get_status()
+    task_status = task.get_status()
     if task_status != False:
-        Tasks(agent_name).stop_tasks()
+        task.stop_tasks()
         return ResponseMessage(message="Task agent stopped")
     # If it's not running start it.
-    Tasks(agent_name).run_task(objective=objective.objective)
+    task.run_task(objective=objective.objective)
     return ResponseMessage(message="Task agent started")
 
 
 @app.get("/api/agent/{agent_name}/task", tags=["Agent"])
 async def get_task_output(agent_name: str) -> TaskOutput:
-    task_output = Tasks(agent_name).get_task_output()
+    task_output = Tasks(agent_name=agent_name).get_task_output()
     if task_output != False:
         return TaskOutput(
             output=task_output,
             message="Task agent is not running",
         )
     else:
         return TaskOutput(
             output="",
             message="Task agent is not running",
         )
 
 
 @app.get("/api/agent/{agent_name}/task/status", tags=["Agent"])
 async def get_task_status(agent_name: str):
-    task_status = Tasks(agent_name).get_status()
+    task_status = Tasks(agent_name=agent_name).get_status()
     return {"status": task_status}
 
 
 @app.get("/api/chain", tags=["Chain"])
 async def get_chains():
     chains = Chain().get_chains()
     return chains
 
 
 @app.get("/api/chain/{chain_name}", tags=["Chain"])
 async def get_chain(chain_name: str):
-    chain_data = Chain().get_chain(chain_name)
+    chain_data = Chain().get_chain(chain_name=chain_name)
     return {"chain": chain_data}
 
 
 @app.post("/api/chain/{chain_name}/run", tags=["Chain"])
 async def run_chain(chain_name: str) -> ResponseMessage:
-    await Chain().run_chain(chain_name)
+    await Chain().run_chain(chain_name=chain_name)
     return {"message": f"Chain '{chain_name}' started."}
 
 
 @app.post("/api/chain", tags=["Chain"])
 async def add_chain(chain_name: ChainName) -> ResponseMessage:
-    Chain().add_chain(chain_name.chain_name)
+    Chain().add_chain(chain_name=chain_name.chain_name)
     return ResponseMessage(message=f"Chain '{chain_name.chain_name}' created.")
 
 
 @app.put("/api/chain/{chain_name}", tags=["Chain"])
 async def rename_chain(chain_name: str, new_name: ChainNewName) -> ResponseMessage:
-    Chain().rename_chain(chain_name, new_name.new_name)
+    Chain().rename_chain(chain_name=chain_name, new_name=new_name.new_name)
     return ResponseMessage(
         message=f"Chain '{chain_name}' renamed to '{new_name.new_name}'."
     )
 
 
 @app.delete("/api/chain/{chain_name}", tags=["Chain"])
 async def delete_chain(chain_name: str) -> ResponseMessage:
-    Chain().delete_chain(chain_name)
+    Chain().delete_chain(chain_name=chain_name)
     return ResponseMessage(message=f"Chain '{chain_name}' deleted.")
 
 
 @app.post("/api/chain/{chain_name}/step", tags=["Chain"])
 async def add_step(chain_name: str, step_info: StepInfo) -> ResponseMessage:
     Chain().add_chain_step(
-        chain_name,
-        step_info.step_number,
-        step_info.prompt_type,
-        step_info.prompt,
-        step_info.agent_name,
+        chain_name=chain_name,
+        step_number=step_info.step_number,
+        prompt_type=step_info.prompt_type,
+        prompt=step_info.prompt,
+        agent_name=step_info.agent_name,
     )
     return {"message": f"Step {step_info.step_number} added to chain '{chain_name}'."}
 
 
 @app.put("/api/chain/{chain_name}/step/{step_number}", tags=["Chain"])
 async def update_step(
     chain_name: str, step_number: int, chain_step: ChainStep
 ) -> ResponseMessage:
     Chain().update_step(
-        chain_name,
-        chain_step.step_number,
-        chain_step.prompt_type,
-        chain_step.prompt,
-        chain_step.agent_name,
+        chain_name=chain_name,
+        step_number=chain_step.step_number,
+        prompt_type=chain_step.prompt_type,
+        prompt=chain_step.prompt,
+        agent_name=chain_step.agent_name,
     )
     return {
         "message": f"Step {chain_step.step_number} updated for chain '{chain_name}'."
     }
 
 
 @app.patch("/api/chain/{chain_name}/step/move", tags=["Chain"])
 async def move_step(
     chain_name: str, chain_step_new_info: ChainStepNewInfo
 ) -> ResponseMessage:
     Chain().move_step(
-        chain_name,
-        chain_step_new_info.old_step_number,
-        chain_step_new_info.new_step_number,
+        chain_name=chain_name,
+        current_step_number=chain_step_new_info.old_step_number,
+        new_step_number=chain_step_new_info.new_step_number,
     )
     return {
         "message": f"Step {chain_step_new_info.old_step_number} moved to {chain_step_new_info.new_step_number} in chain '{chain_name}'."
     }
 
 
 @app.delete("/api/chain/{chain_name}/step/{step_number}", tags=["Chain"])
 async def delete_step(chain_name: str, step_number: int) -> ResponseMessage:
-    Chain().delete_step(chain_name, step_number)
+    Chain().delete_step(chain_name=chain_name, step_number=step_number)
     return {"message": f"Step {step_number} deleted from chain '{chain_name}'."}
 
 
 @app.post("/api/prompt", tags=["Prompt"])
 async def add_prompt(prompt: CustomPromptModel) -> ResponseMessage:
     try:
-        Prompts().add_prompt(prompt.prompt_name, prompt.prompt)
+        Prompts().add_prompt(prompt_name=prompt.prompt_name, prompt=prompt.prompt)
         return ResponseMessage(message=f"Prompt '{prompt.prompt_name}' added.")
     except Exception as e:
         raise HTTPException(status_code=400, detail=str(e))
 
 
 @app.get("/api/prompt/{prompt_name}", tags=["Prompt"], response_model=CustomPromptModel)
 async def get_prompt(prompt_name: str):
     try:
-        prompt_content = Prompts().get_prompt(prompt_name)
+        prompt_content = Prompts().get_prompt(prompt_name=prompt_name)
         return {"prompt_name": prompt_name, "prompt": prompt_content}
     except Exception as e:
         raise HTTPException(status_code=404, detail=str(e))
 
 
 @app.get("/api/prompt", response_model=PromptList, tags=["Prompt"])
 async def get_prompts():
     prompts = Prompts().get_prompts()
     return {"prompts": prompts}
 
 
 @app.delete("/api/prompt/{prompt_name}", tags=["Prompt"])
 async def delete_prompt(prompt_name: str) -> ResponseMessage:
     try:
-        Prompts().delete_prompt(prompt_name)
+        Prompts().delete_prompt(prompt_name=prompt_name)
         return ResponseMessage(message=f"Prompt '{prompt_name}' deleted.")
     except Exception as e:
         raise HTTPException(status_code=404, detail=str(e))
 
 
 @app.put("/api/prompt/{prompt_name}", tags=["Prompt"])
 async def update_prompt(prompt: CustomPromptModel) -> ResponseMessage:
     try:
-        Prompts().update_prompt(prompt.prompt_name, prompt.prompt)
+        Prompts().update_prompt(prompt_name=prompt.prompt_name, prompt=prompt.prompt)
         return ResponseMessage(message=f"Prompt '{prompt.prompt_name}' updated.")
     except Exception as e:
         raise HTTPException(status_code=404, detail=str(e))
 
 
 if __name__ == "__main__":
     uvicorn.run(app, host="127.0.0.1", port=7437)
```

### Comparing `agixt-1.1.80b0/agixt/auth_libs/Cfig.py` & `agixt-1.1.81b0/agixt/auth_libs/Cfig.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/auth_libs/Redirect.py` & `agixt-1.1.81b0/agixt/auth_libs/Redirect.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/auth_libs/Users.py` & `agixt-1.1.81b0/agixt/auth_libs/Users.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/chains/Smart Chat.json` & `agixt-1.1.81b0/agixt/chains/Smart Chat.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/chains/Test_Commands.json` & `agixt-1.1.81b0/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/chains/Write a Poem.json` & `agixt-1.1.81b0/agixt/chains/Write a Poem.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/chains/Write a Poem_responses.json` & `agixt-1.1.81b0/agixt/chains/Write a Poem_responses.json`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/components/agent_selector.py` & `agixt-1.1.81b0/agixt/components/agent_selector.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/example.ipynb` & `agixt-1.1.81b0/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/agixt_agent.py` & `agixt-1.1.81b0/agixt/extensions/agixt_agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/briantts.py` & `agixt-1.1.81b0/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/dalle.py` & `agixt-1.1.81b0/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/discord.py` & `agixt-1.1.81b0/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/elevenlabs.py` & `agixt-1.1.81b0/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/file_system.py` & `agixt-1.1.81b0/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/github.py` & `agixt-1.1.81b0/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/google.py` & `agixt-1.1.81b0/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/gtts.py` & `agixt-1.1.81b0/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/huggingface.py` & `agixt-1.1.81b0/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/macostts.py` & `agixt-1.1.81b0/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/microsoft_365.py` & `agixt-1.1.81b0/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/searxng.py` & `agixt-1.1.81b0/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/sendgrid_email.py` & `agixt-1.1.81b0/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/twitter.py` & `agixt-1.1.81b0/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/extensions/web_playwright.py` & `agixt-1.1.81b0/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/pages/0-Agent_Settings.py` & `agixt-1.1.81b0/agixt/pages/0-Agent_Settings.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/pages/1-Learning.py` & `agixt-1.1.81b0/agixt/pages/1-Learning.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/pages/2-Prompts.py` & `agixt-1.1.81b0/agixt/pages/2-Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/pages/3-Chains.py` & `agixt-1.1.81b0/agixt/pages/3-Chains.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/pages/4-Chat.py` & `agixt-1.1.81b0/agixt/pages/4-Chat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/pages/5-Instructions.py` & `agixt-1.1.81b0/agixt/pages/5-Instructions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/pages/6-Tasks.py` & `agixt-1.1.81b0/agixt/pages/6-Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/pages/Login.py` & `agixt-1.1.81b0/agixt/pages/Login.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/pages/Profile.py` & `agixt-1.1.81b0/agixt/pages/Profile.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/pages/Register.py` & `agixt-1.1.81b0/agixt/pages/Register.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/prompts/Create New Command.txt` & `agixt-1.1.81b0/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/prompts/Execution.txt` & `agixt-1.1.81b0/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/prompts/Instruction.txt` & `agixt-1.1.81b0/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.1.81b0/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.1.81b0/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/prompts/ValidationFailed.txt` & `agixt-1.1.81b0/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.1.81b0/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.1.81b0/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/prompts/instruct.txt` & `agixt-1.1.81b0/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/prompts/starchat/instruct.txt` & `agixt-1.1.81b0/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/prompts/vicuna/instruct.txt` & `agixt-1.1.81b0/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/__init__.py` & `agixt-1.1.81b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/azure.py` & `agixt-1.1.81b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/bing.py` & `agixt-1.1.81b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/chatgpt.py` & `agixt-1.1.81b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/claude.py` & `agixt-1.1.81b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/fastchat.py` & `agixt-1.1.81b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/gpt4all.py` & `agixt-1.1.81b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/gpt4free.py` & `agixt-1.1.81b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.81b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/huggingchat.py` & `agixt-1.1.81b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/huggingface.py` & `agixt-1.1.81b0/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/kobold.py` & `agixt-1.1.81b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/oobabooga.py` & `agixt-1.1.81b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/openai.py` & `agixt-1.1.81b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/palm.py` & `agixt-1.1.81b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/runpod.py` & `agixt-1.1.81b0/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/provider/transformer.py` & `agixt-1.1.81b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/starchat.sh` & `agixt-1.1.81b0/agixt/starchat.sh`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/test-commands.ipynb` & `agixt-1.1.81b0/agixt/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/agixt/test-memory.ipynb` & `agixt-1.1.81b0/agixt/test-memory.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.1.80b0/docs/README.md` & `agixt-1.1.81b0/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,21 @@
 
 - [AGiXT](#agixt)
   - [Table of Contents 📖](#table-of-contents-)
   - [⚠️ Disclaimers!](#️-disclaimers)
     - [Monitor Your Usage!](#monitor-your-usage)
     - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
-  - [Quickstart with Docker](#quickstart-with-docker)
-    - [Windows Docker Desktop (streamlit only example)](#windows-docker-desktop-streamlit-only-example)
-    - [Alternative Docker Compose Profiles](#alternative-docker-compose-profiles)
-    - [Development using docker](#development-using-docker)
-  - [Local Development](#local-development)
+  - [Quickstart using docker](#quickstart-using-docker)
+  - [Development using docker](#development-using-docker)
+  - [Development using poetry](#development-using-poetry)
+      - [Install poetry](#install-poetry)
+      - [Setup AGiXT](#setup-agixt)
+      - [Run Streamlit](#run-streamlit)
+      - [Run REST](#run-rest)
     - [API Endpoints](#api-endpoints)
   - [Configuration](#configuration)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
   - [Acknowledgments](#acknowledgments)
@@ -62,15 +64,15 @@
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
 ## Quickstart using docker
 
-see [Quick Start](https://github.com/Josh-XT/AGiXT/edit/main/docs/1-Getting%20started/Quick%20Start.md)
+Visit our [Quick Start](https://josh-xt.github.io/AGiXT/1-Getting%20started/Quick%20Start.html) documentation.
 
 ## Development using docker
 ```
 git clone https://github.com/Josh-XT/AGiXT
 cd AGiXT
 docker compose -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
```

### Comparing `agixt-1.1.80b0/pyproject.toml` & `agixt-1.1.81b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AGiXT"
-version = "v1.1.80-beta"
+version = "v1.1.81-beta"
 description = "An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day."
 homepage = "https://AGiXT.com"
 documentation = "https://AGiXT.com"
 keywords = ["AI", "AGI", "Agent", "skynet"]
 license = "MIT"
 authors = ["Josh XT <josh@devxt.com>"]
 maintainers = [
```

### Comparing `agixt-1.1.80b0/PKG-INFO` & `agixt-1.1.81b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.80b0
+Version: 1.1.81b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Home-page: https://AGiXT.com
 License: MIT
 Keywords: AI,AGI,Agent,skynet
 Author: Josh XT
 Author-email: josh@devxt.com
 Maintainer: localAGI
@@ -85,19 +85,21 @@
 
 - [AGiXT](#agixt)
   - [Table of Contents 📖](#table-of-contents-)
   - [⚠️ Disclaimers!](#️-disclaimers)
     - [Monitor Your Usage!](#monitor-your-usage)
     - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
-  - [Quickstart with Docker](#quickstart-with-docker)
-    - [Windows Docker Desktop (streamlit only example)](#windows-docker-desktop-streamlit-only-example)
-    - [Alternative Docker Compose Profiles](#alternative-docker-compose-profiles)
-    - [Development using docker](#development-using-docker)
-  - [Local Development](#local-development)
+  - [Quickstart using docker](#quickstart-using-docker)
+  - [Development using docker](#development-using-docker)
+  - [Development using poetry](#development-using-poetry)
+      - [Install poetry](#install-poetry)
+      - [Setup AGiXT](#setup-agixt)
+      - [Run Streamlit](#run-streamlit)
+      - [Run REST](#run-rest)
     - [API Endpoints](#api-endpoints)
   - [Configuration](#configuration)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
   - [Acknowledgments](#acknowledgments)
@@ -125,15 +127,15 @@
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
 ## Quickstart using docker
 
-see [Quick Start](https://github.com/Josh-XT/AGiXT/edit/main/docs/1-Getting%20started/Quick%20Start.md)
+Visit our [Quick Start](https://josh-xt.github.io/AGiXT/1-Getting%20started/Quick%20Start.html) documentation.
 
 ## Development using docker
 ```
 git clone https://github.com/Josh-XT/AGiXT
 cd AGiXT
 docker compose -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
```

