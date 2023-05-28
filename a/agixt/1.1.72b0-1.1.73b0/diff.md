# Comparing `tmp/agixt-1.1.72b0.tar.gz` & `tmp/agixt-1.1.73b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.72b0.tar", last modified: Wed May 24 16:11:02 2023, max compression
+gzip compressed data, was "agixt-1.1.73b0.tar", max compression
```

## Comparing `agixt-1.1.72b0.tar` & `agixt-1.1.73b0.tar`

### file list

```diff
@@ -1,49 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:02.015688 agixt-1.1.72b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-24 16:10:49.000000 agixt-1.1.72b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 16:10:49.000000 agixt-1.1.72b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-24 16:11:02.015688 agixt-1.1.72b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:02.011688 agixt-1.1.72b0/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/Tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12960 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:02.015688 agixt-1.1.72b0/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/llamacppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 16:10:49.000000 agixt-1.1.72b0/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:02.011688 agixt-1.1.72b0/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-24 16:11:01.000000 agixt-1.1.72b0/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-24 16:11:02.000000 agixt-1.1.72b0/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:11:01.000000 agixt-1.1.72b0/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-24 16:11:01.000000 agixt-1.1.72b0/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 16:11:01.000000 agixt-1.1.72b0/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:02.015688 agixt-1.1.72b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-24 16:10:49.000000 agixt-1.1.72b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 16:10:49.000000 agixt-1.1.72b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:11:02.015688 agixt-1.1.72b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-24 16:10:49.000000 agixt-1.1.72b0/setup.py
+-rw-r--r--   0        0        0     1087 2023-05-27 13:20:13.458149 agixt-1.1.73b0/LICENSE
+-rw-r--r--   0        0        0    19449 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/AGiXT.py
+-rw-r--r--   0        0        0    22250 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/API-Tests.ipynb
+-rw-r--r--   0        0        0    14112 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/Agent.py
+-rw-r--r--   0        0        0     6918 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/Chain.py
+-rw-r--r--   0        0        0     6224 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/Commands.py
+-rw-r--r--   0        0        0     1101 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/Config.py
+-rw-r--r--   0        0        0     1960 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/CustomPrompt.py
+-rw-r--r--   0        0        0     7045 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/Embedding.py
+-rw-r--r--   0        0        0      606 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/Main.py
+-rw-r--r--   0        0        0     9615 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/Memories.py
+-rw-r--r--   0        0        0     7128 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/Tasks.py
+-rw-r--r--   0        0        0       38 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/WORKSPACE/example.txt
+-rw-r--r--   0        0        0      236 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/agents/gpt4free/config.json
+-rw-r--r--   0        0        0        0 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/agents/gpt4free.yaml
+-rw-r--r--   0        0        0    12742 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/app.py
+-rw-r--r--   0        0        0     1609 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/auth_libs/Cfig.py
+-rw-r--r--   0        0        0     1410 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/auth_libs/Login.py
+-rw-r--r--   0        0        0     5840 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/auth_libs/Profile.py
+-rw-r--r--   0        0        0     1165 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/auth_libs/Redirect.py
+-rw-r--r--   0        0        0     1866 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/auth_libs/Register.py
+-rw-r--r--   0        0        0     3229 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/auth_libs/Users.py
+-rw-r--r--   0        0        0     2012 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/chains/Smart Chat.json
+-rw-r--r--   0        0        0     1526 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/commands/audio_text.py
+-rw-r--r--   0        0        0      555 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/commands/chain_commands.py
+-rw-r--r--   0        0        0     3826 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/commands/cicd.py
+-rw-r--r--   0        0        0     1074 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/commands/create_new_command.py
+-rw-r--r--   0        0        0     2862 2023-05-27 13:20:13.458149 agixt-1.1.73b0/agixt/commands/discord_commands.py
+-rw-r--r--   0        0        0     3190 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/execute_code.py
+-rw-r--r--   0        0        0     4055 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/file_operations.py
+-rw-r--r--   0        0        0     1635 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/github.py
+-rw-r--r--   0        0        0     2899 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/google.py
+-rw-r--r--   0        0        0     2130 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/image_generator.py
+-rw-r--r--   0        0        0     4198 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/microsoft_365_email.py
+-rw-r--r--   0        0        0     1561 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/searxng_commands.py
+-rw-r--r--   0        0        0      989 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/sendgrid_email.py
+-rw-r--r--   0        0        0      303 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/times.py
+-rw-r--r--   0        0        0     1157 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/twitter.py
+-rw-r--r--   0        0        0     2899 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/voice.py
+-rw-r--r--   0        0        0     2269 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/web_playwright.py
+-rw-r--r--   0        0        0     3372 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/web_requests.py
+-rw-r--r--   0        0        0     4357 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/web_selenium.py
+-rw-r--r--   0        0        0      949 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/commands/work_with_ai.py
+-rw-r--r--   0        0        0     1566 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/components/agent_selector.py
+-rw-r--r--   0        0        0       42 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/config.yaml
+-rw-r--r--   0        0        0    11963 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/example.ipynb
+-rw-r--r--   0        0        0     1132 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/model-prompts/gpt-3.5-turbo/instruct.txt
+-rw-r--r--   0        0        0     1132 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/model-prompts/gpt-4/instruct.txt
+-rw-r--r--   0        0        0      777 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/model-prompts/starchat/instruct.txt
+-rw-r--r--   0        0        0      569 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/model-prompts/vicuna/instruct.txt
+-rw-r--r--   0        0        0    10211 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/pages/0-Agent_Settings.py
+-rw-r--r--   0        0        0     1726 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/pages/1-Learning.py
+-rw-r--r--   0        0        0     2779 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/pages/2-Chat.py
+-rw-r--r--   0        0        0     2887 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/pages/3-Instructions.py
+-rw-r--r--   0        0        0     1571 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/pages/4-Tasks.py
+-rw-r--r--   0        0        0    11954 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/pages/5-Chains.py
+-rw-r--r--   0        0        0     2513 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/pages/6-Custom_Prompts.py
+-rw-r--r--   0        0        0      145 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/Chat.txt
+-rw-r--r--   0        0        0      175 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0        0        0      991 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/Create New Command.txt
+-rw-r--r--   0        0        0     1018 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/Execution.txt
+-rw-r--r--   0        0        0     1132 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/Instruction.txt
+-rw-r--r--   0        0        0      372 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0        0        0      424 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0        0        0      326 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/Prioritize.txt
+-rw-r--r--   0        0        0      236 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0        0        0      316 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0        0        0      268 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0        0        0      298 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0        0        0      142 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0        0        0      441 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0        0        0      522 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0        0        0      452 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0        0        0      427 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0        0        0      154 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0        0        0      474 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0        0        0      554 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0        0        0      186 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0        0        0      155 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0        0        0      270 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/Validation.txt
+-rw-r--r--   0        0        0      782 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0        0        0      308 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/WebSearch.txt
+-rw-r--r--   0        0        0      730 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/prompts/instruct.txt
+-rw-r--r--   0        0        0     2147 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/__init__.py
+-rw-r--r--   0        0        0     1611 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/azure.py
+-rw-r--r--   0        0        0      487 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/bard.py
+-rw-r--r--   0        0        0     2050 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/bing.py
+-rw-r--r--   0        0        0      974 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/chatgpt.py
+-rw-r--r--   0        0        0     1006 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/claude.py
+-rw-r--r--   0        0        0      757 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/fastchat.py
+-rw-r--r--   0        0        0      867 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/gpt4all.py
+-rw-r--r--   0        0        0     2593 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/gpt4free.py
+-rw-r--r--   0        0        0     1188 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0        0        0     1001 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/huggingchat.py
+-rw-r--r--   0        0        0     1035 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/kobold.py
+-rw-r--r--   0        0        0     1939 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/llamacpp.py
+-rw-r--r--   0        0        0     2177 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/llamacppapi.py
+-rw-r--r--   0        0        0     1579 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/oobabooga.py
+-rw-r--r--   0        0        0     1464 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/openai.py
+-rw-r--r--   0        0        0      844 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/palm.py
+-rw-r--r--   0        0        0     3100 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/provider/transformer.py
+-rw-r--r--   0        0        0      538 2023-05-27 13:20:13.462149 agixt-1.1.73b0/agixt/starchat.sh
+-rw-r--r--   0        0        0    13394 2023-05-27 13:20:13.466149 agixt-1.1.73b0/docs/README.md
+-rw-r--r--   0        0        0     2145 2023-05-27 13:20:13.478149 agixt-1.1.73b0/pyproject.toml
+-rw-r--r--   0        0        0    15693 1970-01-01 00:00:00.000000 agixt-1.1.73b0/PKG-INFO
```

### Comparing `agixt-1.1.72b0/LICENSE` & `agixt-1.1.73b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/PKG-INFO` & `agixt-1.1.73b0/docs/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: agixt
-Version: 1.1.72b0
-Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
-Author: Josh XT
-Author-email: josh@devxt.com
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # AGiXT
 ![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic) 
 [![STATUS](https://img.shields.io/badge/status-beta-blue?label=Release%20Status&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
 
 [![GitHub](https://img.shields.io/badge/GitHub-Frontend_Repository-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
@@ -100,20 +90,27 @@
 ```
 
 ## Local Development
 
 Clone the repository for the AGiXT back end and start it.
 
 ```
-git clone https://github.com/Josh-XT/AGiXT
-cd AGiXT/agixt
-pip install -r requirements.txt
+git clone https://github.com/Josh-XT/AGiXT && cd AGiXT
+pip install poetry
+export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
+poetry install --with gpt4free
 playwright install
-streamlit run Main.py
+cd agixt
 ```
+#### Run Streamlit 
+`poetry run streamlit run Main.py`
+
+#### Run REST
+`poetry run uvicorn app:app --port 7437`
+
 
 Access the web interface at http://localhost:8501
 
 ### API Endpoints
 
 AGiXT provides several API endpoints for managing agents, prompts and chains.
```

### Comparing `agixt-1.1.72b0/agixt/AGiXT.py` & `agixt-1.1.73b0/agixt/AGiXT.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import re
+import os
 import asyncio
 import regex
 import json
 import time
 import spacy
 from datetime import datetime
 from Agent import Agent
 from CustomPrompt import CustomPrompt
-from duckduckgo_search import ddg
+from commands.searxng_commands import searxng_commands
 from urllib.parse import urlparse
+import logging
 
 
 class AGiXT:
     def __init__(self, agent_name: str = "AGiXT"):
         self.agent_name = agent_name
         self.agent = Agent(self.agent_name)
         self.agent_commands = self.agent.get_commands_string()
@@ -42,26 +44,39 @@
             else:
                 return str(value)
 
         pattern = r"(?<!{){([^{}\n]+)}(?!})"
         result = re.sub(pattern, replace, string)
         return result
 
+    def get_step_response(self, chain_name, step_number):
+        try:
+            with open(os.path.join("chains", f"{chain_name}_responses.json"), "r") as f:
+                responses = json.load(f)
+            return responses.get(str(step_number))
+        except:
+            return ""
+
     def format_prompt(
         self,
-        task: str,
+        task: str = "",
         top_results: int = 5,
         prompt="",
+        chain_name="",
+        step_number=0,
         **kwargs,
     ):
         cp = CustomPrompt()
         if prompt == "":
             prompt = task
         else:
-            prompt = cp.get_prompt(prompt_name=prompt, model=self.agent.AI_MODEL)
+            try:
+                prompt = cp.get_prompt(prompt_name=prompt, model=self.agent.AI_MODEL)
+            except:
+                prompt = prompt
         if top_results == 0:
             context = "None"
         else:
             try:
                 context = self.agent.memories.context_agent(
                     query=task, top_results_num=top_results
                 )
@@ -74,61 +89,76 @@
             agent_name=self.agent_name,
             COMMANDS=self.agent_commands,
             context=context,
             command_list=command_list,
             date=datetime.now().strftime("%B %d, %Y %I:%M %p"),
             **kwargs,
         )
+        if "{STEP" in formatted_prompt:
+            # get the response from the step number
+            step_response = self.get_step_response(
+                chain_name=chain_name, step_number=step_number
+            )
+            # replace the {STEPx} with the response
+            formatted_prompt = formatted_prompt.replace(
+                f"{{STEP{step_number}}}", step_response
+            )
         if not self.nlp:
             self.load_spacy_model()
         tokens = len(self.nlp(formatted_prompt))
+        logging.info(f"FORMATTED PROMPT: {formatted_prompt}")
         return formatted_prompt, prompt, tokens
 
     def run(
         self,
-        task: str,
+        task: str = "",
         prompt: str = "",
         context_results: int = 5,
         websearch: bool = False,
         websearch_depth: int = 3,
         async_exec: bool = False,
         learn_file: str = "",
+        chain_name: str = "",
+        step_number: int = 0,
         **kwargs,
     ):
+        logging.info(f"KWARGS: {kwargs}")
         if learn_file != "":
             learning_file = self.agent.memories.read_file(file_path=learn_file)
             if learning_file == False:
                 return "Failed to read file."
         formatted_prompt, unformatted_prompt, tokens = self.format_prompt(
             task=task,
             top_results=context_results,
             prompt=prompt,
+            chain_name=chain_name,
+            step_number=step_number,
             **kwargs,
         )
         if websearch:
             if async_exec:
                 loop = asyncio.new_event_loop()
                 asyncio.set_event_loop(loop)
                 loop.run_until_complete(
                     self.websearch_agent(task=task, depth=websearch_depth)
                 )
             else:
                 self.websearch_agent(task=task, depth=websearch_depth)
         try:
             self.response = self.agent.instruct(formatted_prompt, tokens=tokens)
         except Exception as e:
-            print(f"Error: {e}")
-            print(f"PROMPT CONTENT: {formatted_prompt}")
-            print(f"TOKENS: {tokens}")
+            logging.info(f"Error: {e}")
+            logging.info(f"PROMPT CONTENT: {formatted_prompt}")
+            logging.info(f"TOKENS: {tokens}")
             self.failures += 1
             if self.failures == 5:
                 self.failures == 0
-                print("Failed to get a response 5 times in a row.")
+                logging.info("Failed to get a response 5 times in a row.")
                 return None
-            print(f"Retrying in 10 seconds...")
+            logging.info(f"Retrying in 10 seconds...")
             time.sleep(10)
             if context_results > 0:
                 context_results = context_results - 1
             self.response = self.run(
                 task=task,
                 prompt=prompt,
                 context_results=context_results,
@@ -158,15 +188,15 @@
                 if execution_response:
                     return_response += (
                         f"\n\nCommand Execution Response:\n{execution_response}"
                     )
             except:
                 return_response = self.response
             self.response = return_response
-        print(f"Response: {self.response}")
+        logging.info(f"Response: {self.response}")
         if self.response != "" and self.response != None:
             try:
                 self.agent.memories.store_result(task, self.response)
             except:
                 pass
             self.agent.log_interaction("USER", task)
             self.agent.log_interaction(self.agent_name, self.response)
@@ -313,17 +343,17 @@
             if len(cleaned_json) == 0:
                 return False
             if isinstance(cleaned_json, list):
                 cleaned_json = cleaned_json[0]
             response = json.loads(cleaned_json)
             return response
         except:
-            print("INVALID JSON RESPONSE")
-            print(execution_response)
-            print("... Trying again.")
+            logging.info("INVALID JSON RESPONSE")
+            logging.info(execution_response)
+            logging.info("... Trying again.")
             if context_results != 0:
                 context_results = context_results - 1
             else:
                 context_results = 0
             execution_response = self.run(
                 task=task, context_results=context_results, **kwargs
             )
@@ -336,15 +366,15 @@
         task,
         command_name,
         command_args,
         command_output,
         context_results,
         **kwargs,
     ):
-        print(
+        logging.info(
             f"Command {command_name} did not execute as expected with args {command_args}. Trying again.."
         )
         revalidate = self.run(
             task=task,
             prompt="ValidationFailed",
             command_name=command_name,
             command_args=command_args,
@@ -368,15 +398,15 @@
                         ]:
                             command_name = available_command["name"]
                             try:
                                 # Check if the command is a valid command in the self.avent.available_commands list
                                 command_output = self.agent.execute(
                                     command_name, command_args
                                 )
-                                print("Running Command Execution Validation...")
+                                logging.info("Running Command Execution Validation...")
                                 validate_command = self.run(
                                     task=task,
                                     prompt="Validation",
                                     command_name=command_name,
                                     command_args=command_args,
                                     command_output=command_output,
                                     **kwargs,
@@ -387,15 +417,15 @@
                                     command_name,
                                     command_args,
                                     command_output,
                                     **kwargs,
                                 )
 
                             if validate_command.startswith("Y"):
-                                print(
+                                logging.info(
                                     f"Command {command_name} executed successfully with args {command_args}."
                                 )
                                 response = f"\nExecuted Command:{command_name} with args {command_args}.\nCommand Output: {command_output}\n"
                                 return response
                             else:
                                 revalidate = self.run(
                                     task=task,
@@ -410,16 +440,16 @@
                                 )
                 else:
                     if command_name == "None.":
                         return "\nNo commands were executed.\n"
                     else:
                         return f"\Command not recognized: {command_name} ."
         except:
-            print("\nERROR IN EXECUTION_AGENT, validated_response:\n")
-            print(validated_response)
+            logging.info("\nERROR IN EXECUTION_AGENT, validated_response:\n")
+            logging.info(validated_response)
             return "\nNo commands were executed.\n"
 
     async def websearch_agent(
         self, task: str = "What are the latest breakthroughs in AI?", depth: int = 3
     ):
         async def resursive_browsing(task, links):
             try:
@@ -428,21 +458,24 @@
                     word for word in words if urlparse(word).scheme in ["http", "https"]
                 ]
             except:
                 links = links
             if links is not None:
                 for link in links:
                     if "href" in link:
-                        url = link["href"]
+                        try:
+                            url = link["href"]
+                        except:
+                            url = link
                     else:
                         url = link
                     url = re.sub(r"^.*?(http)", r"http", url)
                     # Check if url is an actual url
                     if url.startswith("http"):
-                        print(f"Scraping: {url}")
+                        logging.info(f"Scraping: {url}")
                         if url not in self.browsed_links:
                             self.browsed_links.append(url)
                             (
                                 collected_data,
                                 link_list,
                             ) = await self.agent.memories.read_website(url)
                             if link_list is not None:
@@ -454,16 +487,29 @@
                                             task=task,
                                             prompt="Pick-a-Link",
                                             links=link_list,
                                         )
                                         if not pick_a_link.startswith("None"):
                                             await resursive_browsing(task, pick_a_link)
                                     except:
-                                        print(f"Issues reading {url}. Moving on...")
+                                        logging.info(
+                                            f"Issues reading {url}. Moving on..."
+                                        )
 
         results = self.run(task=task, prompt="WebSearch")
         results = results.split("\n")
         for result in results:
             search_string = result.lstrip("0123456789. ")
-            links = ddg(search_string, max_results=depth)
+            try:
+                searx_server = self.agent.PROVIDER_SETTINGS["SEARXNG_INSTANCE_URL"]
+            except:
+                searx_server = ""
+            try:
+                links = searxng_commands(
+                    SEARXNG_INSTANCE_URL=searx_server
+                ).search_searx(search_string)
+                if len(links) > depth:
+                    links = links[:depth]
+            except:
+                links = None
             if links is not None:
                 await resursive_browsing(task, links)
```

### Comparing `agixt-1.1.72b0/agixt/Agent.py` & `agixt-1.1.73b0/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/agixt/Chain.py` & `agixt-1.1.73b0/agixt/Chain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import json
 from AGiXT import AGiXT
 import argparse
 from CustomPrompt import CustomPrompt
 from Commands import Commands
+import logging
 
 
 class Chain:
     def get_chain(self, chain_name):
         with open(os.path.join("chains", f"{chain_name}.json"), "r") as f:
             chain_data = json.load(f)
         return chain_data
@@ -73,21 +74,21 @@
 
     def get_steps(self, chain_name):
         chain_data = self.get_chain(chain_name)
         return chain_data["steps"]
 
     def run_chain(self, chain_name):
         chain_data = self.get_chain(chain_name)
-        print(f"Running chain '{chain_name}'")
+        logging.info(f"Running chain '{chain_name}'")
         responses = {}  # Create a dictionary to hold responses.
         for step_data in chain_data["steps"]:
             if "prompt" in step_data and "step" in step_data:
-                print(f"Running step {step_data['step']}")
+                logging.info(f"Running step {step_data['step']}")
                 step_response = self.run_chain_step(
-                    step_data
+                    step_data, chain_name
                 )  # Get the response of the current step.
                 responses[step_data["step"]] = step_response  # Store the response.
         # Write the responses to the json file.
         with open(os.path.join("chains", f"{chain_name}_responses.json"), "w") as f:
             json.dump(responses, f)
         return responses
 
@@ -113,52 +114,51 @@
             )
             # replace the {STEPx} with the response
             prompt_content = prompt_content.replace(
                 f"{{STEP{step_number}}}", step_response
             )
         return prompt_content
 
-    def run_chain_step(self, step):
+    def run_chain_step(self, step, chain_name):
+        logging.info(step)
         if step:
             if "prompt_type" in step:
                 prompt_type = step["prompt_type"]
                 prompt = step["prompt"]
                 agent_name = step["agent_name"]
                 step_number = step["step"]
                 try:
                     command_name = prompt["command_name"]
-                    prompt = {k: v for k, v in prompt.items() if k != "command_name"}
                 except:
                     command_name = ""
                 if prompt_type == "Command":
                     commands_args = prompt
                     for prompt_content in prompt:
                         commands_args[prompt_content] = self.get_step_content(
                             chain_name, step_number, prompt_content
                         )
                     return Commands(agent_name=agent_name).execute_command(
                         command_name, commands_args
                     )
                 try:
-                    prompt_name = prompt["prompt_name"]
-                    prompt = {
-                        k: v
-                        for k, v in prompt.items()
-                        if k != "prompt_name" and k != "task"
-                    }
-                    prompt_content = CustomPrompt().get_prompt(prompt_name)
+                    prompt_content = CustomPrompt().get_prompt(
+                        prompt_name=prompt["prompt_name"]
+                    )
                     prompt_content = self.get_step_content(
                         chain_name, step_number, prompt_content
                     )
                     agent = AGiXT(agent_name)
                 except:
                     return None
                 if prompt_type == "Prompt":
                     result = agent.run(
-                        task=prompt_content, prompt=prompt_name, **prompt
+                        prompt=prompt["prompt_name"],
+                        chain_name=chain_name,
+                        step_number=step_number,
+                        **prompt,
                     )
                 elif prompt_type == "Chain":
                     result = self.run_chain(prompt["chain_name"])
                 elif prompt_type == "Smart Instruct":
                     result = agent.smart_instruct(task=prompt_content, **prompt)
                 elif prompt_type == "Smart Chat":
                     result = agent.smart_chat(task=prompt_content, **prompt)
```

### Comparing `agixt-1.1.72b0/agixt/Commands.py` & `agixt-1.1.73b0/agixt/Commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import importlib
 import os
 import glob
 from inspect import signature, Parameter
+import logging
 
 
 class Commands:
     def __init__(self, agent_config, load_commands_flag: bool = True):
         self.agent_config = agent_config
         if load_commands_flag:
             self.commands = self.load_commands()
@@ -82,14 +83,15 @@
                                 command_name,
                                 getattr(module, module_name),
                                 command_function.__name__,
                                 params,
                             )
                         )
         # Return the commands list
+        logging.debug(f"loaded commands: {commands}")
         return commands
 
     def get_extension_settings(self):
         settings = {}
         command_files = glob.glob("commands/*.py")
         for command_file in command_files:
             module_name = os.path.splitext(os.path.basename(command_file))[0]
```

### Comparing `agixt-1.1.72b0/agixt/CustomPrompt.py` & `agixt-1.1.73b0/agixt/CustomPrompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
         # if prompts folder does not exist, create it
         if not os.path.exists("prompts"):
             os.mkdir("prompts")
         # if prompt file does not exist, create it
         if not os.path.exists(os.path.join("prompts", f"{prompt_name}.txt")):
             with open(os.path.join("prompts", f"{prompt_name}.txt"), "w") as f:
                 f.write(prompt)
-        else:
-            raise Exception("Prompt already exists")
 
     def get_prompt(self, prompt_name, model="default"):
         try:
             with open(f"model-prompts/{model}/{prompt_name}.txt", "r") as f:
                 return f.read()
         except:
             try:
```

### Comparing `agixt-1.1.72b0/agixt/Embedding.py` & `agixt-1.1.73b0/agixt/Embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import requests
 import inspect
 import openai
 from chromadb.utils import embedding_functions
 from chromadb.api.types import Documents, EmbeddingFunction, Embeddings
+import logging
 
 
 class GooglePalmEmbeddingFunction(EmbeddingFunction):
     """To use this EmbeddingFunction, you must have the google.generativeai Python package installed and have a PaLM API key."""
 
     def __init__(self, api_key: str, model_name: str = "models/embedding-gecko-001"):
         if not api_key:
@@ -123,15 +124,15 @@
         # We also need to return the correct chunk size
         self.AGENT_CONFIG = AGENT_CONFIG
         try:
             embedder = self.AGENT_CONFIG["settings"]["embedder"]
             self.embed, self.chunk_size = self.__getattribute__(embedder)()
         except:
             self.embed, self.chunk_size = self.default()
-            print("Embedder not found, using default embedder")
+            logging.info("Embedder not found, using default embedder")
 
     def default(self):
         chunk_size = 128
         embed = embedding_functions.SentenceTransformerEmbeddingFunction(
             model_name="all-mpnet-base-v2"
         )
         return embed, chunk_size
```

### Comparing `agixt-1.1.72b0/agixt/Main.py` & `agixt-1.1.73b0/agixt/Main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Main.py
 import streamlit as st
 from components.agent_selector import agent_selector
 
-
 st.set_page_config(
     page_title="AGiXT",
     page_icon=":robot:",
     layout="wide",
     initial_sidebar_state="expanded",
 )
 agent_name, agent = agent_selector()
```

### Comparing `agixt-1.1.72b0/agixt/Memories.py` & `agixt-1.1.73b0/agixt/Memories.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from datetime import datetime
 from collections import Counter
 import pandas as pd
 import docx2txt
 import pdfplumber
 from playwright.async_api import async_playwright
 from bs4 import BeautifulSoup
+import logging
 
 
 class Memories:
     def __init__(self, agent_name: str = "AGiXT", agent_config=None):
         self.agent_name = agent_name
         self.agent_config = agent_config
         self.chroma_client = None
@@ -52,15 +53,15 @@
         self.embedding_function = embedder.embed
         self.chunk_size = embedder.chunk_size
         try:
             return self.chroma_client.get_collection(
                 name="memories", embedding_function=self.embedding_function
             )
         except ValueError:
-            print(f"Memories for {self.agent_name} do not exist. Creating...")
+            logging.info(f"Memories for {self.agent_name} do not exist. Creating...")
             return self.chroma_client.create_collection(
                 name="memories", embedding_function=self.embedding_function
             )
 
     def generate_id(self, content: str, timestamp: str):
         return sha256((content + timestamp).encode()).hexdigest()
 
@@ -71,15 +72,15 @@
         try:
             self.collection.add(
                 ids=id,
                 documents=content,
                 metadatas=metadatas,
             )
         except Exception as e:
-            print(f"Failed to store memory: {e}")
+            logging.info(f"Failed to store memory: {e}")
 
     def store_result(self, task_name: str, result: str):
         if not self.chroma_client:
             self.chroma_client = self.initialize_chroma_client()
             self.collection = self.get_or_create_collection()
         if result:
             timestamp = datetime.now()  # current time as datetime object
@@ -106,27 +107,29 @@
         if count == 0:
             return []
         results = self.collection.query(
             query_texts=query,
             n_results=min(top_results_num, count),
             include=["metadatas"],
         )
-        # Parse timestamps and sort the results by timestamp in descending order
         sorted_results = sorted(
             results["metadatas"][0],
             key=lambda item: datetime.strptime(
                 item.get("timestamp") or "1970-01-01T00:00:00.000",
                 "%Y-%m-%dT%H:%M:%S.%f",
             ),
             reverse=True,
         )
-
+        # TODO: Before sending results, ask AI if each chunk it is relevant to the task-
+        #   so that we're only injecting relevant memories into the context.
+        # This will ensure we aren't injecting memories that aren't relevant.
+        # Need to research to find out how to do this locally instead of sending more shots to the AI.
         context = [item["result"] for item in sorted_results]
         trimmed_context = self.trim_context(context)
-        print(f"CONTEXT: {trimmed_context}")
+        logging.info(f"CONTEXT: {trimmed_context}")
         context_str = "\n".join(trimmed_context)
         response = f"Context: {context_str}\n\n"
         return response
 
     def trim_context(self, context: List[str]) -> List[str]:
         if not self.nlp:
             self.load_spacy_model()
```

### Comparing `agixt-1.1.72b0/agixt/Tasks.py` & `agixt-1.1.73b0/agixt/Tasks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from AGiXT import AGiXT
 import re
 import os
 import json
 import yaml
 from Agent import Agent
 from collections import deque
+import logging
 
 
 class Tasks:
     def __init__(self, agent_name: str = "AGiXT"):
         self.agent_name = agent_name
         self.ai = AGiXT(self.agent_name)
         self.primary_objective = None
         self.task_list = deque([])
         self.output_list = []
         self.stop_running_event = False
+        if not os.path.exists(f"agents/{self.agent_name}/tasks"):
+            os.makedirs(f"agents/{self.agent_name}/tasks")
 
-    def load_task(self):
-        out_file = re.sub(r"[^\w\s]", "", self.primary_objective)
+    def load_task(self, task):
+        out_file = re.sub(r"[^\w\s]", "", task)
         out_file = out_file[:25]
         try:
             with open(f"agents/{self.agent_name}/{out_file}.json", "r") as f:
                 task_state = json.load(f)
 
             self.task_list = deque(task_state["task_list"])
             self.output_list = task_state["tasks"]
             self.primary_objective = task_state["primary_objective"]
-            print(f"Successfully loaded task '{out_file}'.")
+            logging.info(f"Successfully loaded task '{out_file}'.")
 
         except FileNotFoundError:
-            print(f"No saved task found with the name '{out_file}'.")
+            logging.info(f"No saved task found with the name '{out_file}'.")
         except Exception as e:
-            print(f"An error occurred while loading the task: {e}")
+            logging.info(f"An error occurred while loading the task: {e}")
 
     def get_status(self):
-        if self.task_list:
+        if self.task_list != deque([]) and self.output_list != []:
             return True
         else:
             return False
 
     def update_task(self, task_id, task_name, task_output):
         # Check if the task exists at agents/{agent_name}/tasks/{self.primary_objective}.json
         # We need to stip out symbols except spaces in primary objective and truncate the primary objective to 15 characters
@@ -74,22 +77,22 @@
     def get_task_output(self):
         out_file = re.sub(r"[^\w\s]", "", self.primary_objective)
         out_file = out_file[:25]
         try:
             with open(f"agents/{self.agent_name}/tasks/{out_file}.json", "r") as f:
                 task_output = json.load(f)
 
-            print(f"Successfully loaded task output for '{out_file}'.")
+            logging.info(f"Successfully loaded task output for '{out_file}'.")
             return task_output
 
         except FileNotFoundError:
-            print(f"No saved task output found with the name '{out_file}'.")
+            logging.info(f"No saved task output found with the name '{out_file}'.")
             return None
         except Exception as e:
-            print(f"An error occurred while loading the task output: {e}")
+            logging.info(f"An error occurred while loading the task output: {e}")
             return None
 
     def get_tasks_files(self):
         files = os.listdir(os.path.join("agents", self.agent_name, "tasks"))
         files = [file[:-5] for file in files]
         return files
 
@@ -133,52 +136,52 @@
         smart: bool = False,
         load_task: str = "",
         **kwargs,
     ):
         initial_task = "Break down the objective into a list of small achievable tasks in the form of instructions that lead up to achieving the ultimate goal of the objective."
         if load_task != "":
             self.load_task(load_task)
-            print(f"Loaded task '{load_task}'.\n\n")
+            logging.info(f"Loaded task '{load_task}'.\n\n")
         else:
             self.primary_objective = objective
             self.task_list = deque(
                 [
                     {
                         "task_id": 1,
                         "task_name": initial_task,
                     }
                 ]
             )
-            print(f"Starting task with objective: {self.primary_objective}.\n\n")
+            logging.info(f"Starting task with objective: {self.primary_objective}.\n\n")
 
         while not self.stop_running_event and self.task_list != deque([]):
             task = self.task_list.popleft()
             if task["task_name"] in ["None", "None.", ""]:
                 self.stop_tasks()
                 continue
-            print(f"\nExecuting task {task['task_id']}: {task['task_name']}\n")
+            logging.info(f"\nExecuting task {task['task_id']}: {task['task_name']}\n")
             if smart != True:
                 result = self.instruction_agent(task=task["task_name"], **kwargs)
             else:
                 result = self.ai.smart_instruct(
                     task=task["task_name"],
                     shots=3,
                     async_exec=async_exec,
                     objective=self.primary_objective,
                     **kwargs,
                 )
             self.update_task(task["task_id"], task["task_name"], result)
-            print(f"\nTask Result:\n\n{result}\n")
+            logging.info(f"\nTask Result:\n\n{result}\n")
             if task["task_name"] == initial_task:
                 lines = result.split("\n") if "\n" in result else [result]
                 new_tasks = []
                 for line in lines:
                     match = re.match(r"(\d+)\.\s+(.*)", line)
                     if match:
                         task_id, task_name = match.groups()
                         new_tasks.append(
                             {"task_id": int(task_id), "task_name": task_name.strip()}
                         )
                 self.task_list = deque(new_tasks)
         if not self.task_list:
             self.stop_tasks()
-        print("All tasks completed or stopped.")
+        logging.info("All tasks completed or stopped.")
```

### Comparing `agixt-1.1.72b0/agixt/app.py` & `agixt-1.1.73b0/agixt/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,21 @@
 from Chain import Chain
 from Tasks import Tasks
 from CustomPrompt import CustomPrompt
 from typing import Optional, Dict, List, Any
 from provider import get_provider_options
 from Embedding import get_embedding_providers
 import os
-
-this_directory = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(this_directory, "version"), encoding="utf-8") as f:
-    version = f.read().strip()
+import logging
 
 CFG = Config()
 app = FastAPI(
     title="AGiXT",
     description="AGiXT is an Artificial Intelligence Automation platform for creating and managing AI agents. Visit the GitHub repo for more information or to report issues. https://github.com/Josh-XT/AGiXT/",
-    version=version,
+    version="1.0.0",  # API version according to https://restfulapi.net/versioning/
     docs_url="/",
 )
 agent_threads = {}
 agent_stop_events = {}
 
 app.add_middleware(
     CORSMiddleware,
@@ -214,42 +211,41 @@
     agent = AGiXT(agent_name)
     response = agent.smart_chat(prompt.prompt, shots=shots)
     return {"response": str(response)}
 
 
 @app.get("/api/agent/{agent_name}/command", tags=["Agent"])
 async def get_commands(agent_name: str):
-    commands = Commands(agent_name)
-    available_commands = commands.get_available_commands()
-    return {"commands": available_commands}
+    agent = Agent(agent_name)
+    return {"commands": agent.agent_config["commands"]}
 
 
 @app.patch("/api/agent/{agent_name}/command", tags=["Agent"])
 async def toggle_command(
     agent_name: str, payload: ToggleCommandPayload
 ) -> ResponseMessage:
     agent = Agent(agent_name)
+    print(payload)
     try:
         if payload.command_name == "*":
-            commands = Commands(agent_name)
-            for each_command_name in commands.agent_config["commands"]:
-                commands.agent_config["commands"][each_command_name] = payload.enable
-            agent.update_agent_config(commands.agent_config["commands"], "commands")
+            for each_command_name in agent.agent_config["commands"]:
+                agent.agent_config["commands"][each_command_name] = payload.enable
+
+            agent.update_agent_config(agent.agent_config["commands"], "commands")
             return ResponseMessage(
                 message=f"All commands enabled for agent '{agent_name}'."
             )
         else:
-            commands = Commands(agent_name)
-            commands.agent_config["commands"][payload.command_name] = payload.enable
-            agent.update_agent_config(commands.agent_config["commands"], "commands")
+            agent.agent_config["commands"][payload.command_name] = payload.enable
+            agent.update_agent_config(agent.agent_config["commands"], "commands")
             return ResponseMessage(
                 message=f"Command '{payload.command_name}' toggled for agent '{agent_name}'."
             )
     except Exception as e:
-        print(e)
+        logging.info(e)
         raise HTTPException(
             status_code=500,
             detail=f"Error enabling all commands for agent '{agent_name}': {str(e)}",
         )
 
 
 @app.post("/api/agent/{agent_name}/task", tags=["Agent"])
```

### Comparing `agixt-1.1.72b0/agixt/provider/__init__.py` & `agixt-1.1.73b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/agixt/provider/azure.py` & `agixt-1.1.73b0/agixt/provider/azure.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from time import time
 from openai.error import RateLimitError
 import openai
+import logging
 
 
 class AzureProvider:
     def __init__(
         self,
         AZURE_API_KEY: str = "",
         AZURE_OPENAI_ENDPOINT: str = "",
@@ -37,10 +38,10 @@
                     messages=messages,
                     max_tokens=int(self.MAX_TOKENS),
                     temperature=float(self.AI_TEMPERATURE),
                 )["choices"][0]["message"]["content"]
                 return resp
 
             except RateLimitError:
-                print("Rate limit exceeded. Retrying after 20 seconds.")
+                logging.info("Rate limit exceeded. Retrying after 20 seconds.")
                 time.sleep(20)
                 continue
```

### Comparing `agixt-1.1.72b0/agixt/provider/bing.py` & `agixt-1.1.73b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/agixt/provider/chatgpt.py` & `agixt-1.1.73b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/agixt/provider/claude.py` & `agixt-1.1.73b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/agixt/provider/fastchat.py` & `agixt-1.1.73b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/agixt/provider/gpt4all.py` & `agixt-1.1.73b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/agixt/provider/gpt4free.py` & `agixt-1.1.73b0/agixt/provider/gpt4free.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import gpt4free
 import time
+import logging
 
 
 class Gpt4freeProvider:
     def __init__(
         self,
         AI_MODEL: str = "gpt-3.5-turbo",
         AI_TEMPERATURE: float = 0.7,
@@ -20,42 +21,42 @@
 
     def instruct(self, prompt, tokens: int = 0):
         final_response = None
         while final_response is None:
             for provider in self.providers:
                 try:
                     if provider not in self.FAILED_PROVIDERS:
-                        print(f"[GPT4Free] Using: {provider}")
+                        logging.info(f"[GPT4Free] Using: {provider}")
                         response = gpt4free.Completion.create(
                             getattr(gpt4free.Provider, provider),
                             prompt=prompt,
                         )
                         if response:
                             if "text" in response:
                                 final_response = response["text"]
                             if "status" in response and response["status"] == "Fail":
                                 self.FAILED_PROVIDERS.append(provider)
-                                print(f"Failed to use {provider}")
+                                logging.info(f"Failed to use {provider}")
                                 final_response = None
                             if (
                                 response
                                 == "Unable to fetch the response, Please try again."
                             ):
                                 self.FAILED_PROVIDERS.append(provider)
-                                print(f"Failed to use {provider}")
+                                logging.info(f"Failed to use {provider}")
                                 final_response = None
                             if final_response == None:
                                 final_response = response
                     if final_response:
                         if len(final_response) > 1:
                             return final_response
                 except:
-                    print(f"Failed to use {provider}")
+                    logging.info(f"Failed to use {provider}")
                     self.FAILED_PROVIDERS.append(provider)
                     final_response = None
 
             if len(self.FAILED_PROVIDERS) == len(self.providers):
                 self.FAILED_PROVIDERS = []
-                print(
+                logging.info(
                     "All providers failed, sleeping for 10 seconds before trying again..."
                 )
                 time.sleep(10)
```

### Comparing `agixt-1.1.72b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.73b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/agixt/provider/huggingchat.py` & `agixt-1.1.73b0/agixt/provider/huggingchat.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from hugchat import hugchat
+import logging
 
 
 class HuggingchatProvider:
     def __init__(
         self,
         AI_TEMPERATURE: float = 0.7,
         MAX_TOKENS: int = 2000,
@@ -22,9 +23,9 @@
             id = chatbot.new_conversation()
             response = chatbot.chat(
                 text=prompt,
                 temperature=float(self.AI_TEMPERATURE),
             )
             return response
         except Exception as e:
-            print(e)
+            logging.info(e)
             return f"HuggingChat Provider Failure: {e}."
```

### Comparing `agixt-1.1.72b0/agixt/provider/kobold.py` & `agixt-1.1.73b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/agixt/provider/llamacpp.py` & `agixt-1.1.73b0/agixt/provider/llamacpp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import subprocess
 import sys
 import os
+import logging
 
 try:
     from llama_cpp import Llama
 except:
     subprocess.check_call([sys.executable, "-m", "pip", "install", "llama-cpp-python"])
     from llama_cpp import Llama
 
@@ -45,15 +46,15 @@
             self.model = Llama(
                 model_path=self.MODEL_PATH,
                 n_gpu_layers=int(self.GPU_LAYERS),
                 n_threads=int(self.THREADS),
                 n_ctx=max_tokens,
             )
         else:
-            print("Unable to find model path.")
+            logging.info("Unable to find model path.")
             return None
         response = self.model(
             prompt,
             stop=[self.STOP_SEQUENCE],
             temperature=float(self.AI_TEMPERATURE),
             echo=True,
         )
```

### Comparing `agixt-1.1.72b0/agixt/provider/llamacppapi.py` & `agixt-1.1.73b0/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/agixt/provider/oobabooga.py` & `agixt-1.1.73b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/agixt/provider/openai.py` & `agixt-1.1.73b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/agixt/provider/palm.py` & `agixt-1.1.73b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/agixt/provider/transformer.py` & `agixt-1.1.73b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.72b0/agixt.egg-info/PKG-INFO` & `agixt-1.1.73b0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,77 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.72b0
+Version: 1.1.73b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
+Home-page: https://AGiXT.com
+License: MIT
+Keywords: AI,AGI,Agent,skynet
 Author: Josh XT
 Author-email: josh@devxt.com
-Requires-Python: >=3.10
+Maintainer: localAGI
+Maintainer-email: 132956819+localagi@users.noreply.github.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: EdgeGPT
+Requires-Dist: GoogleBard
+Requires-Dist: InstructorEmbedding
+Requires-Dist: PyGithub
+Requires-Dist: accelerate
+Requires-Dist: anthropic
+Requires-Dist: argparse
+Requires-Dist: beautifulsoup4
+Requires-Dist: captcha-solver
+Requires-Dist: chromadb
+Requires-Dist: cryptography (==38.0.4)
+Requires-Dist: discord
+Requires-Dist: docker
+Requires-Dist: docx2txt
+Requires-Dist: duckduckgo_search (==3.3.0)
+Requires-Dist: fastapi
+Requires-Dist: ffmpeg
+Requires-Dist: flask-bcrypt
+Requires-Dist: gitpython
+Requires-Dist: google-api-python-client
+Requires-Dist: google-auth
+Requires-Dist: google-auth-httplib2
+Requires-Dist: google-auth-oauthlib
+Requires-Dist: google-cloud-aiplatform
+Requires-Dist: google-generativeai
+Requires-Dist: gtts
+Requires-Dist: hugchat
+Requires-Dist: jsonschema
+Requires-Dist: llama-cpp-python
+Requires-Dist: nomic
+Requires-Dist: openai
+Requires-Dist: pdfplumber
+Requires-Dist: playsound (==1.2.2)
+Requires-Dist: playwright
+Requires-Dist: pre-commit
+Requires-Dist: protobuf (==3.20.*)
+Requires-Dist: pynacl
+Requires-Dist: python-git
+Requires-Dist: pytz
+Requires-Dist: random-password-generator
+Requires-Dist: revChatGPT
+Requires-Dist: selenium
+Requires-Dist: sendgrid
+Requires-Dist: sentence-transformers
+Requires-Dist: spacy
+Requires-Dist: streamlit
+Requires-Dist: tiktoken
+Requires-Dist: torch
+Requires-Dist: transformers (>=4.29.2,<5.0.0)
+Requires-Dist: tweepy
+Requires-Dist: uvicorn
+Requires-Dist: webdriver_manager
+Project-URL: Documentation, https://AGiXT.com
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # AGiXT
 ![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic) 
 [![STATUS](https://img.shields.io/badge/status-beta-blue?label=Release%20Status&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
 
@@ -100,20 +161,27 @@
 ```
 
 ## Local Development
 
 Clone the repository for the AGiXT back end and start it.
 
 ```
-git clone https://github.com/Josh-XT/AGiXT
-cd AGiXT/agixt
-pip install -r requirements.txt
+git clone https://github.com/Josh-XT/AGiXT && cd AGiXT
+pip install poetry
+export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring
+poetry install --with gpt4free
 playwright install
-streamlit run Main.py
+cd agixt
 ```
+#### Run Streamlit 
+`poetry run streamlit run Main.py`
+
+#### Run REST
+`poetry run uvicorn app:app --port 7437`
+
 
 Access the web interface at http://localhost:8501
 
 ### API Endpoints
 
 AGiXT provides several API endpoints for managing agents, prompts and chains.
 
@@ -159,7 +227,8 @@
 - [![BabyAGI](https://img.shields.io/badge/GitHub-babyagi-white?logo=github&style=plastic) ![BabyAGI](https://img.shields.io/github/stars/yoheinakajima/babyagi?style=social)](https://github.com/yoheinakajima/babyagi)
 - [![Auto-GPT](https://img.shields.io/badge/GitHub-Auto--GPT-white?logo=github&style=plastic) ![Auto-GPT](https://img.shields.io/github/stars/Significant-Gravitas/Auto-GPT?style=social)](https://github.com/Significant-Gravitas/Auto-GPT)
 
 Please consider exploring and contributing to these projects if you like what we are doing.
 
 ## History
 ![Star History Chart](https://api.star-history.com/svg?repos=Josh-XT/AGiXT&type=Dat)
+
```

