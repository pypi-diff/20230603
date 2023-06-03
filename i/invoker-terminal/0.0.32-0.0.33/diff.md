# Comparing `tmp/invoker_terminal-0.0.32.tar.gz` & `tmp/invoker_terminal-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invoker_terminal-0.0.32.tar", last modified: Sat Jun  3 14:09:53 2023, max compression
+gzip compressed data, was "invoker_terminal-0.0.33.tar", last modified: Sat Jun  3 14:30:43 2023, max compression
```

## Comparing `invoker_terminal-0.0.32.tar` & `invoker_terminal-0.0.33.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:53.939976 invoker_terminal-0.0.32/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-03 14:09:53.939976 invoker_terminal-0.0.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:53.923976 invoker_terminal-0.0.32/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:53.927976 invoker_terminal-0.0.32/invoker_terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/ast_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:53.931976 invoker_terminal-0.0.32/invoker_terminal/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/commands/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/commands/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/commands/ipfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/commands/new_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/commands/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/commands/wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:53.935976 invoker_terminal-0.0.32/invoker_terminal/cores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/cores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/cores/anchor.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/cores/invoker_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/cores/ipfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/cores/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:53.935976 invoker_terminal-0.0.32/invoker_terminal/idl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/idl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/idl/invoker_network_market.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:53.935976 invoker_terminal-0.0.32/invoker_terminal/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/inputs/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/inputs/fileinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/inputs/inputbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/inputs/numberinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/inputs/rangeinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/inputs/selectinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/inputs/textinput.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:53.935976 invoker_terminal-0.0.32/invoker_terminal/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/outputs/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:53.939976 invoker_terminal-0.0.32/invoker_terminal/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/storage/deployed_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/storage/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:53.939976 invoker_terminal-0.0.32/invoker_terminal/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/templates/Dockerfile_template
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/templates/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/templates/requirements.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/invoker_terminal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:53.927976 invoker_terminal-0.0.32/invoker_terminal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-03 14:09:53.000000 invoker_terminal-0.0.32/invoker_terminal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-03 14:09:53.000000 invoker_terminal-0.0.32/invoker_terminal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 14:09:53.000000 invoker_terminal-0.0.32/invoker_terminal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-03 14:09:53.000000 invoker_terminal-0.0.32/invoker_terminal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-03 14:09:53.000000 invoker_terminal-0.0.32/invoker_terminal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-03 14:09:53.000000 invoker_terminal-0.0.32/invoker_terminal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 14:09:53.939976 invoker_terminal-0.0.32/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:53.939976 invoker_terminal-0.0.32/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-03 14:09:43.000000 invoker_terminal-0.0.32/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:43.738975 invoker_terminal-0.0.33/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-03 14:30:43.738975 invoker_terminal-0.0.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:43.722975 invoker_terminal-0.0.33/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:43.726975 invoker_terminal-0.0.33/invoker_terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/ast_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:43.730975 invoker_terminal-0.0.33/invoker_terminal/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/commands/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/commands/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/commands/ipfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/commands/new_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/commands/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/commands/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:43.734975 invoker_terminal-0.0.33/invoker_terminal/cores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/cores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/cores/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/cores/invoker_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/cores/ipfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/cores/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:43.734975 invoker_terminal-0.0.33/invoker_terminal/idl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/idl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/idl/invoker_network_market.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:43.734975 invoker_terminal-0.0.33/invoker_terminal/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/inputs/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/inputs/fileinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/inputs/inputbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/inputs/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/inputs/rangeinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/inputs/selectinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/inputs/textinput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:43.738975 invoker_terminal-0.0.33/invoker_terminal/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/outputs/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:43.738975 invoker_terminal-0.0.33/invoker_terminal/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/storage/deployed_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/storage/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:43.738975 invoker_terminal-0.0.33/invoker_terminal/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/templates/Dockerfile_template
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/templates/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/templates/requirements.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/invoker_terminal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:43.726975 invoker_terminal-0.0.33/invoker_terminal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-03 14:30:43.000000 invoker_terminal-0.0.33/invoker_terminal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-03 14:30:43.000000 invoker_terminal-0.0.33/invoker_terminal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 14:30:43.000000 invoker_terminal-0.0.33/invoker_terminal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-03 14:30:43.000000 invoker_terminal-0.0.33/invoker_terminal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-03 14:30:43.000000 invoker_terminal-0.0.33/invoker_terminal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-03 14:30:43.000000 invoker_terminal-0.0.33/invoker_terminal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 14:30:43.738975 invoker_terminal-0.0.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:43.738975 invoker_terminal-0.0.33/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-03 14:30:34.000000 invoker_terminal-0.0.33/tests/test_base.py
```

### Comparing `invoker_terminal-0.0.32/HISTORY.md` & `invoker_terminal-0.0.33/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Fix version. [The Invoker]
+- Release: version  🚀 [The Invoker]
 - Add invoke to configless commands. [The Invoker]
 - Release: version  🚀 [The Invoker]
 - Bump to v0.0.31. [The Invoker]
 - Release: version  🚀 [The Invoker]
 - Pump version to 0.0.30. [The Invoker]
 - Release: version  🚀 [The Invoker]
 - Bump 0.0.29. [The Invoker]
```

### Comparing `invoker_terminal-0.0.32/LICENSE` & `invoker_terminal-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/PKG-INFO` & `invoker_terminal-0.0.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoker_terminal
-Version: 0.0.32
+Version: 0.0.33
 Summary: Awesome invoker_terminal created by m00dy
 Home-page: https://github.com/m00dy/invoker-terminal/
 Author: m00dy
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `invoker_terminal-0.0.32/README.md` & `invoker_terminal-0.0.33/README.md`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/ast_check.py` & `invoker_terminal-0.0.33/invoker_terminal/ast_check.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/cli.py` & `invoker_terminal-0.0.33/invoker_terminal/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,17 @@
 
     if args.env == "m" and "mainnet" in config:
         print("Environment " + getEnvText("MAINNET"))
         config["active"]["rpc_url"] = config["mainnet"]["rpc_url"]
         config["active"]["websocket_url"] = config["mainnet"]["websocket_url"]
 
     # print(config.has_section('system'))
-    if args.command != ["init"] or args.command != ["invoke"]:
+    configLessCmds = ['init', 'invoke']
+    cmd = args.command[0]
+    if not cmd in configLessCmds:
         if not config.has_section("system"):
             parser.error(
                 """
 
             needs a valid config before running
 
             type "{PROGRAM_NAME} init" to generate config
```

### Comparing `invoker_terminal-0.0.32/invoker_terminal/client.py` & `invoker_terminal-0.0.33/invoker_terminal/client.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/commands/build.py` & `invoker_terminal-0.0.33/invoker_terminal/commands/build.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/commands/daemon.py` & `invoker_terminal-0.0.33/invoker_terminal/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/commands/deploy.py` & `invoker_terminal-0.0.33/invoker_terminal/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/commands/init.py` & `invoker_terminal-0.0.33/invoker_terminal/commands/init.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/commands/new_task.py` & `invoker_terminal-0.0.33/invoker_terminal/commands/new_task.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/commands/status.py` & `invoker_terminal-0.0.33/invoker_terminal/commands/status.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/commands/test.py` & `invoker_terminal-0.0.33/invoker_terminal/commands/test.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/commands/wallet.py` & `invoker_terminal-0.0.33/invoker_terminal/commands/wallet.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/constants.py` & `invoker_terminal-0.0.33/invoker_terminal/constants.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/cores/anchor.py` & `invoker_terminal-0.0.33/invoker_terminal/cores/anchor.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/cores/invoker_init.py` & `invoker_terminal-0.0.33/invoker_terminal/cores/invoker_init.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/cores/ipfs.py` & `invoker_terminal-0.0.33/invoker_terminal/cores/ipfs.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/idl/invoker_network_market.json` & `invoker_terminal-0.0.33/invoker_terminal/idl/invoker_network_market.json`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/inputs/decorators.py` & `invoker_terminal-0.0.33/invoker_terminal/inputs/decorators.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/inputs/numberinput.py` & `invoker_terminal-0.0.33/invoker_terminal/inputs/numberinput.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/inputs/rangeinput.py` & `invoker_terminal-0.0.33/invoker_terminal/inputs/rangeinput.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/inputs/textinput.py` & `invoker_terminal-0.0.33/invoker_terminal/inputs/textinput.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/outputs/output.py` & `invoker_terminal-0.0.33/invoker_terminal/outputs/output.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/server.py` & `invoker_terminal-0.0.33/invoker_terminal/server.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/storage/deployed_models.py` & `invoker_terminal-0.0.33/invoker_terminal/storage/deployed_models.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/templates/Dockerfile_template` & `invoker_terminal-0.0.33/invoker_terminal/templates/Dockerfile_template`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/templates/model.py` & `invoker_terminal-0.0.33/invoker_terminal/templates/model.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal/utils.py` & `invoker_terminal-0.0.33/invoker_terminal/utils.py`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/invoker_terminal.egg-info/PKG-INFO` & `invoker_terminal-0.0.33/invoker_terminal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoker-terminal
-Version: 0.0.32
+Version: 0.0.33
 Summary: Awesome invoker_terminal created by m00dy
 Home-page: https://github.com/m00dy/invoker-terminal/
 Author: m00dy
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `invoker_terminal-0.0.32/invoker_terminal.egg-info/SOURCES.txt` & `invoker_terminal-0.0.33/invoker_terminal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invoker_terminal-0.0.32/setup.py` & `invoker_terminal-0.0.33/setup.py`

 * *Files identical despite different names*

