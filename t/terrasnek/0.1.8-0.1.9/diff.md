# Comparing `tmp/terrasnek-0.1.8.tar.gz` & `tmp/terrasnek-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrasnek-0.1.8.tar", last modified: Sun Jan  2 05:10:46 2022, max compression
+gzip compressed data, was "terrasnek-0.1.9.tar", last modified: Wed Feb  9 22:03:12 2022, max compression
```

## Comparing `terrasnek-0.1.8.tar` & `terrasnek-0.1.9.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 neil       (502) staff       (20)        0 2022-01-02 05:10:46.600042 terrasnek-0.1.8/
--rw-r--r--   0 neil       (502) staff       (20)     4832 2022-01-02 05:10:46.599292 terrasnek-0.1.8/PKG-INFO
--rw-r--r--   0 neil       (502) staff       (20)     3729 2021-09-22 02:02:40.000000 terrasnek-0.1.8/README.md
--rw-r--r--   0 neil       (502) staff       (20)       38 2022-01-02 05:10:46.600275 terrasnek-0.1.8/setup.cfg
--rw-r--r--   0 neil       (502) staff       (20)      720 2022-01-02 05:00:32.000000 terrasnek-0.1.8/setup.py
-drwxr-xr-x   0 neil       (502) staff       (20)        0 2022-01-02 05:10:46.573588 terrasnek-0.1.8/terrasnek/
--rw-r--r--   0 neil       (502) staff       (20)      329 2020-06-18 02:40:50.000000 terrasnek-0.1.8/terrasnek/__init__.py
--rw-r--r--   0 neil       (502) staff       (20)     1628 2022-01-02 05:02:00.000000 terrasnek-0.1.8/terrasnek/_constants.py
--rw-r--r--   0 neil       (502) staff       (20)     1860 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/account.py
--rw-r--r--   0 neil       (502) staff       (20)     1459 2021-07-26 20:06:52.000000 terrasnek-0.1.8/terrasnek/admin_module_sharing.py
--rw-r--r--   0 neil       (502) staff       (20)     3626 2021-12-23 02:35:07.000000 terrasnek-0.1.8/terrasnek/admin_orgs.py
--rw-r--r--   0 neil       (502) staff       (20)     1515 2021-12-23 02:35:15.000000 terrasnek-0.1.8/terrasnek/admin_runs.py
--rw-r--r--   0 neil       (502) staff       (20)     5870 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/admin_settings.py
--rw-r--r--   0 neil       (502) staff       (20)     3071 2021-12-02 10:03:35.000000 terrasnek-0.1.8/terrasnek/admin_terraform_versions.py
--rw-r--r--   0 neil       (502) staff       (20)     4098 2021-12-23 02:35:15.000000 terrasnek-0.1.8/terrasnek/admin_users.py
--rw-r--r--   0 neil       (502) staff       (20)     2146 2021-12-23 02:35:15.000000 terrasnek-0.1.8/terrasnek/admin_workspaces.py
--rw-r--r--   0 neil       (502) staff       (20)     2345 2021-12-06 22:04:25.000000 terrasnek-0.1.8/terrasnek/agent_tokens.py
--rw-r--r--   0 neil       (502) staff       (20)     3890 2021-12-23 02:35:15.000000 terrasnek-0.1.8/terrasnek/agents.py
--rw-r--r--   0 neil       (502) staff       (20)    13092 2021-12-02 10:03:35.000000 terrasnek-0.1.8/terrasnek/api.py
--rw-r--r--   0 neil       (502) staff       (20)     1021 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/applies.py
--rw-r--r--   0 neil       (502) staff       (20)     1728 2021-12-02 10:03:35.000000 terrasnek-0.1.8/terrasnek/audit_trails.py
--rw-r--r--   0 neil       (502) staff       (20)     5378 2021-12-23 02:35:07.000000 terrasnek-0.1.8/terrasnek/config_versions.py
--rw-r--r--   0 neil       (502) staff       (20)     1029 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/cost_estimates.py
--rw-r--r--   0 neil       (502) staff       (20)    16937 2021-12-23 02:37:49.000000 terrasnek-0.1.8/terrasnek/endpoint.py
--rw-r--r--   0 neil       (502) staff       (20)     3790 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/exceptions.py
--rw-r--r--   0 neil       (502) staff       (20)     1373 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/feature_sets.py
--rw-r--r--   0 neil       (502) staff       (20)     1369 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/invoices.py
--rw-r--r--   0 neil       (502) staff       (20)      930 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/ip_ranges.py
--rw-r--r--   0 neil       (502) staff       (20)     3825 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/notification_configs.py
--rw-r--r--   0 neil       (502) staff       (20)     2822 2021-09-20 00:57:18.000000 terrasnek-0.1.8/terrasnek/oauth_clients.py
--rw-r--r--   0 neil       (502) staff       (20)     2258 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/oauth_tokens.py
--rw-r--r--   0 neil       (502) staff       (20)     3758 2021-12-23 02:35:15.000000 terrasnek-0.1.8/terrasnek/org_memberships.py
--rw-r--r--   0 neil       (502) staff       (20)     2894 2021-12-23 02:35:15.000000 terrasnek-0.1.8/terrasnek/org_tags.py
--rw-r--r--   0 neil       (502) staff       (20)     1433 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/org_tokens.py
--rw-r--r--   0 neil       (502) staff       (20)     3764 2021-04-13 01:28:07.000000 terrasnek-0.1.8/terrasnek/orgs.py
--rw-r--r--   0 neil       (502) staff       (20)     2289 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/plan_exports.py
--rw-r--r--   0 neil       (502) staff       (20)     1850 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/plans.py
--rw-r--r--   0 neil       (502) staff       (20)     4537 2021-12-23 02:35:07.000000 terrasnek-0.1.8/terrasnek/policies.py
--rw-r--r--   0 neil       (502) staff       (20)     1865 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/policy_checks.py
--rw-r--r--   0 neil       (502) staff       (20)     2636 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/policy_set_params.py
--rw-r--r--   0 neil       (502) staff       (20)     7535 2021-12-23 02:35:15.000000 terrasnek-0.1.8/terrasnek/policy_sets.py
--rw-r--r--   0 neil       (502) staff       (20)     9961 2021-12-23 02:35:15.000000 terrasnek-0.1.8/terrasnek/registry_modules.py
--rw-r--r--   0 neil       (502) staff       (20)     3235 2021-12-23 02:59:33.000000 terrasnek-0.1.8/terrasnek/registry_providers.py
--rw-r--r--   0 neil       (502) staff       (20)     6457 2021-12-23 02:35:07.000000 terrasnek-0.1.8/terrasnek/run_tasks.py
--rw-r--r--   0 neil       (502) staff       (20)     3123 2021-12-23 02:35:15.000000 terrasnek-0.1.8/terrasnek/run_triggers.py
--rw-r--r--   0 neil       (502) staff       (20)     4380 2021-12-23 02:35:07.000000 terrasnek-0.1.8/terrasnek/runs.py
--rw-r--r--   0 neil       (502) staff       (20)     2583 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/ssh_keys.py
--rw-r--r--   0 neil       (502) staff       (20)     1736 2021-12-28 02:42:21.000000 terrasnek-0.1.8/terrasnek/state_version_outputs.py
--rw-r--r--   0 neil       (502) staff       (20)     3919 2021-12-23 02:35:07.000000 terrasnek-0.1.8/terrasnek/state_versions.py
--rw-r--r--   0 neil       (502) staff       (20)     1469 2021-03-16 02:20:36.000000 terrasnek-0.1.8/terrasnek/subscriptions.py
--rw-r--r--   0 neil       (502) staff       (20)     2788 2021-12-23 02:35:15.000000 terrasnek-0.1.8/terrasnek/team_access.py
--rw-r--r--   0 neil       (502) staff       (20)     1818 2021-12-23 01:28:41.000000 terrasnek-0.1.8/terrasnek/team_memberships.py
--rw-r--r--   0 neil       (502) staff       (20)     1498 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/team_tokens.py
--rw-r--r--   0 neil       (502) staff       (20)     3320 2021-12-23 02:35:07.000000 terrasnek-0.1.8/terrasnek/teams.py
--rw-r--r--   0 neil       (502) staff       (20)     2293 2021-12-02 10:03:35.000000 terrasnek-0.1.8/terrasnek/user_tokens.py
--rw-r--r--   0 neil       (502) staff       (20)      954 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/users.py
--rw-r--r--   0 neil       (502) staff       (20)     6618 2021-12-23 01:27:56.000000 terrasnek-0.1.8/terrasnek/var_sets.py
--rw-r--r--   0 neil       (502) staff       (20)     2396 2021-12-02 10:03:35.000000 terrasnek-0.1.8/terrasnek/vars.py
--rw-r--r--   0 neil       (502) staff       (20)     1542 2021-12-23 02:35:15.000000 terrasnek-0.1.8/terrasnek/vcs_events.py
--rw-r--r--   0 neil       (502) staff       (20)     2504 2021-03-16 00:11:38.000000 terrasnek-0.1.8/terrasnek/workspace_vars.py
--rw-r--r--   0 neil       (502) staff       (20)    11587 2021-12-23 02:35:07.000000 terrasnek-0.1.8/terrasnek/workspaces.py
-drwxr-xr-x   0 neil       (502) staff       (20)        0 2022-01-02 05:10:46.576503 terrasnek-0.1.8/terrasnek.egg-info/
--rw-r--r--   0 neil       (502) staff       (20)     4832 2022-01-02 05:10:46.000000 terrasnek-0.1.8/terrasnek.egg-info/PKG-INFO
--rw-r--r--   0 neil       (502) staff       (20)     2890 2022-01-02 05:10:46.000000 terrasnek-0.1.8/terrasnek.egg-info/SOURCES.txt
--rw-r--r--   0 neil       (502) staff       (20)        1 2022-01-02 05:10:46.000000 terrasnek-0.1.8/terrasnek.egg-info/dependency_links.txt
--rw-r--r--   0 neil       (502) staff       (20)       17 2022-01-02 05:10:46.000000 terrasnek-0.1.8/terrasnek.egg-info/requires.txt
--rw-r--r--   0 neil       (502) staff       (20)       15 2022-01-02 05:10:46.000000 terrasnek-0.1.8/terrasnek.egg-info/top_level.txt
-drwxr-xr-x   0 neil       (502) staff       (20)        0 2022-01-02 05:10:46.598660 terrasnek-0.1.8/test/
--rw-r--r--   0 neil       (502) staff       (20)      168 2020-06-18 02:40:50.000000 terrasnek-0.1.8/test/__init__.py
--rw-r--r--   0 neil       (502) staff       (20)     2695 2021-12-02 10:03:35.000000 terrasnek-0.1.8/test/_constants.py
--rw-r--r--   0 neil       (502) staff       (20)     3613 2021-09-18 00:22:50.000000 terrasnek-0.1.8/test/account_test.py
--rw-r--r--   0 neil       (502) staff       (20)     1738 2021-03-16 02:20:50.000000 terrasnek-0.1.8/test/admin_module_sharing_test.py
--rw-r--r--   0 neil       (502) staff       (20)     3623 2021-12-24 01:05:48.000000 terrasnek-0.1.8/test/admin_orgs_test.py
--rw-r--r--   0 neil       (502) staff       (20)     3533 2021-12-23 02:35:15.000000 terrasnek-0.1.8/test/admin_runs_test.py
--rw-r--r--   0 neil       (502) staff       (20)     5519 2021-09-22 02:02:40.000000 terrasnek-0.1.8/test/admin_settings_test.py
--rw-r--r--   0 neil       (502) staff       (20)     2941 2020-10-21 16:14:36.000000 terrasnek-0.1.8/test/admin_terraform_versions_test.py
--rw-r--r--   0 neil       (502) staff       (20)     2085 2021-09-22 02:02:40.000000 terrasnek-0.1.8/test/admin_users_test.py
--rw-r--r--   0 neil       (502) staff       (20)     2019 2021-12-23 02:35:15.000000 terrasnek-0.1.8/test/admin_workspaces_test.py
--rw-r--r--   0 neil       (502) staff       (20)     2503 2021-09-18 00:22:50.000000 terrasnek-0.1.8/test/agent_tokens_test.py
--rw-r--r--   0 neil       (502) staff       (20)     2232 2021-12-02 10:03:35.000000 terrasnek-0.1.8/test/agents_test.py
--rw-r--r--   0 neil       (502) staff       (20)     3742 2021-08-23 22:57:01.000000 terrasnek-0.1.8/test/applies_test.py
--rw-r--r--   0 neil       (502) staff       (20)     1628 2021-12-02 10:03:35.000000 terrasnek-0.1.8/test/audit_trails_test.py
--rw-r--r--   0 neil       (502) staff       (20)    23765 2021-12-24 02:02:03.000000 terrasnek-0.1.8/test/base.py
--rw-r--r--   0 neil       (502) staff       (20)     4701 2021-12-24 01:29:32.000000 terrasnek-0.1.8/test/config_versions_test.py
--rw-r--r--   0 neil       (502) staff       (20)     3725 2021-03-16 00:11:38.000000 terrasnek-0.1.8/test/cost_estimates_test.py
--rw-r--r--   0 neil       (502) staff       (20)      704 2021-03-16 00:11:38.000000 terrasnek-0.1.8/test/feature_sets_test.py
--rw-r--r--   0 neil       (502) staff       (20)      574 2021-09-22 02:02:40.000000 terrasnek-0.1.8/test/invoices_test.py
--rw-r--r--   0 neil       (502) staff       (20)      592 2020-10-21 16:14:36.000000 terrasnek-0.1.8/test/ip_ranges_test.py
--rw-r--r--   0 neil       (502) staff       (20)     4403 2020-10-21 16:14:36.000000 terrasnek-0.1.8/test/notification_configs_test.py
--rw-r--r--   0 neil       (502) staff       (20)     2019 2020-10-21 16:14:36.000000 terrasnek-0.1.8/test/oauth_clients_test.py
--rw-r--r--   0 neil       (502) staff       (20)     2410 2021-09-18 00:22:50.000000 terrasnek-0.1.8/test/oauth_tokens_test.py
--rw-r--r--   0 neil       (502) staff       (20)     3441 2021-09-22 02:02:40.000000 terrasnek-0.1.8/test/org_memberships_test.py
--rw-r--r--   0 neil       (502) staff       (20)     3466 2022-01-02 04:45:47.000000 terrasnek-0.1.8/test/org_tags_test.py
--rw-r--r--   0 neil       (502) staff       (20)     1273 2020-10-21 16:14:36.000000 terrasnek-0.1.8/test/org_tokens_test.py
--rw-r--r--   0 neil       (502) staff       (20)     3251 2021-08-23 22:24:08.000000 terrasnek-0.1.8/test/orgs_test.py
--rw-r--r--   0 neil       (502) staff       (20)     4349 2021-03-16 00:11:38.000000 terrasnek-0.1.8/test/plan_exports_test.py
--rw-r--r--   0 neil       (502) staff       (20)     3787 2021-03-16 00:11:38.000000 terrasnek-0.1.8/test/plans_test.py
--rw-r--r--   0 neil       (502) staff       (20)     4143 2021-09-22 02:02:40.000000 terrasnek-0.1.8/test/policies_test.py
--rw-r--r--   0 neil       (502) staff       (20)     4119 2021-09-18 00:22:50.000000 terrasnek-0.1.8/test/policy_checks_test.py
--rw-r--r--   0 neil       (502) staff       (20)     3119 2020-10-21 16:14:36.000000 terrasnek-0.1.8/test/policy_set_params_test.py
--rw-r--r--   0 neil       (502) staff       (20)     7008 2021-09-22 02:02:40.000000 terrasnek-0.1.8/test/policy_sets_test.py
--rw-r--r--   0 neil       (502) staff       (20)     8934 2021-12-24 01:28:23.000000 terrasnek-0.1.8/test/registry_modules_test.py
--rw-r--r--   0 neil       (502) staff       (20)     2461 2021-12-02 10:03:35.000000 terrasnek-0.1.8/test/registry_providers_test.py
--rw-r--r--   0 neil       (502) staff       (20)     5136 2021-12-02 10:03:35.000000 terrasnek-0.1.8/test/run_tasks_test.py
--rw-r--r--   0 neil       (502) staff       (20)     3013 2021-08-21 01:24:43.000000 terrasnek-0.1.8/test/run_triggers_test.py
--rw-r--r--   0 neil       (502) staff       (20)     7928 2021-09-22 02:02:40.000000 terrasnek-0.1.8/test/runs_test.py
--rw-r--r--   0 neil       (502) staff       (20)     1714 2021-09-18 00:22:50.000000 terrasnek-0.1.8/test/ssh_keys_test.py
--rw-r--r--   0 neil       (502) staff       (20)     3639 2021-12-28 03:39:29.000000 terrasnek-0.1.8/test/state_version_outputs_test.py
--rw-r--r--   0 neil       (502) staff       (20)     4323 2021-12-24 01:22:59.000000 terrasnek-0.1.8/test/state_versions_test.py
--rw-r--r--   0 neil       (502) staff       (20)      681 2021-03-16 00:11:38.000000 terrasnek-0.1.8/test/subscriptions_test.py
--rw-r--r--   0 neil       (502) staff       (20)     3470 2021-08-21 01:24:43.000000 terrasnek-0.1.8/test/team_access_test.py
--rw-r--r--   0 neil       (502) staff       (20)     2001 2021-09-18 00:22:50.000000 terrasnek-0.1.8/test/team_memberships_test.py
--rw-r--r--   0 neil       (502) staff       (20)      978 2021-09-18 00:22:50.000000 terrasnek-0.1.8/test/team_tokens_test.py
--rw-r--r--   0 neil       (502) staff       (20)     2908 2021-04-13 15:57:35.000000 terrasnek-0.1.8/test/teams_test.py
--rw-r--r--   0 neil       (502) staff       (20)     1557 2020-10-21 16:14:36.000000 terrasnek-0.1.8/test/user_tokens_test.py
--rw-r--r--   0 neil       (502) staff       (20)      625 2020-10-21 16:14:36.000000 terrasnek-0.1.8/test/users_test.py
--rw-r--r--   0 neil       (502) staff       (20)     6784 2021-12-02 10:03:35.000000 terrasnek-0.1.8/test/var_sets_test.py
--rw-r--r--   0 neil       (502) staff       (20)     2576 2021-12-02 10:03:35.000000 terrasnek-0.1.8/test/vars_test.py
--rw-r--r--   0 neil       (502) staff       (20)     1223 2021-09-22 02:02:40.000000 terrasnek-0.1.8/test/vcs_events_test.py
--rw-r--r--   0 neil       (502) staff       (20)     2728 2021-08-21 01:24:43.000000 terrasnek-0.1.8/test/workspace_vars_test.py
--rw-r--r--   0 neil       (502) staff       (20)     8689 2021-12-23 03:01:11.000000 terrasnek-0.1.8/test/workspaces_test.py
+drwxr-xr-x   0 neil       (502) staff       (20)        0 2022-02-09 22:03:12.340760 terrasnek-0.1.9/
+-rw-r--r--   0 neil       (502) staff       (20)     4832 2022-02-09 22:03:12.340369 terrasnek-0.1.9/PKG-INFO
+-rw-r--r--   0 neil       (502) staff       (20)     3729 2021-09-22 02:02:40.000000 terrasnek-0.1.9/README.md
+-rw-r--r--   0 neil       (502) staff       (20)       38 2022-02-09 22:03:12.340898 terrasnek-0.1.9/setup.cfg
+-rw-r--r--   0 neil       (502) staff       (20)      720 2022-02-09 21:52:42.000000 terrasnek-0.1.9/setup.py
+drwxr-xr-x   0 neil       (502) staff       (20)        0 2022-02-09 22:03:12.319711 terrasnek-0.1.9/terrasnek/
+-rw-r--r--   0 neil       (502) staff       (20)      329 2020-06-18 02:40:50.000000 terrasnek-0.1.9/terrasnek/__init__.py
+-rw-r--r--   0 neil       (502) staff       (20)     1670 2022-02-09 21:52:34.000000 terrasnek-0.1.9/terrasnek/_constants.py
+-rw-r--r--   0 neil       (502) staff       (20)     1860 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/account.py
+-rw-r--r--   0 neil       (502) staff       (20)     1459 2021-07-26 20:06:52.000000 terrasnek-0.1.9/terrasnek/admin_module_sharing.py
+-rw-r--r--   0 neil       (502) staff       (20)     3626 2021-12-23 02:35:07.000000 terrasnek-0.1.9/terrasnek/admin_orgs.py
+-rw-r--r--   0 neil       (502) staff       (20)     1515 2021-12-23 02:35:15.000000 terrasnek-0.1.9/terrasnek/admin_runs.py
+-rw-r--r--   0 neil       (502) staff       (20)     5870 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/admin_settings.py
+-rw-r--r--   0 neil       (502) staff       (20)     3071 2021-12-02 10:03:35.000000 terrasnek-0.1.9/terrasnek/admin_terraform_versions.py
+-rw-r--r--   0 neil       (502) staff       (20)     4098 2021-12-23 02:35:15.000000 terrasnek-0.1.9/terrasnek/admin_users.py
+-rw-r--r--   0 neil       (502) staff       (20)     2146 2021-12-23 02:35:15.000000 terrasnek-0.1.9/terrasnek/admin_workspaces.py
+-rw-r--r--   0 neil       (502) staff       (20)     2345 2022-01-02 05:11:43.000000 terrasnek-0.1.9/terrasnek/agent_tokens.py
+-rw-r--r--   0 neil       (502) staff       (20)     3890 2022-01-02 05:11:43.000000 terrasnek-0.1.9/terrasnek/agents.py
+-rw-r--r--   0 neil       (502) staff       (20)    13092 2022-02-09 18:35:13.000000 terrasnek-0.1.9/terrasnek/api.py
+-rw-r--r--   0 neil       (502) staff       (20)     1021 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/applies.py
+-rw-r--r--   0 neil       (502) staff       (20)     1728 2021-12-02 10:03:35.000000 terrasnek-0.1.9/terrasnek/audit_trails.py
+-rw-r--r--   0 neil       (502) staff       (20)     5378 2021-12-23 02:35:07.000000 terrasnek-0.1.9/terrasnek/config_versions.py
+-rw-r--r--   0 neil       (502) staff       (20)     1029 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/cost_estimates.py
+-rw-r--r--   0 neil       (502) staff       (20)    16344 2022-02-09 18:53:58.000000 terrasnek-0.1.9/terrasnek/endpoint.py
+-rw-r--r--   0 neil       (502) staff       (20)     3790 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/exceptions.py
+-rw-r--r--   0 neil       (502) staff       (20)     1373 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/feature_sets.py
+-rw-r--r--   0 neil       (502) staff       (20)     1401 2022-02-09 18:53:58.000000 terrasnek-0.1.9/terrasnek/invoices.py
+-rw-r--r--   0 neil       (502) staff       (20)      930 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/ip_ranges.py
+-rw-r--r--   0 neil       (502) staff       (20)     3825 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/notification_configs.py
+-rw-r--r--   0 neil       (502) staff       (20)     2822 2021-09-20 00:57:18.000000 terrasnek-0.1.9/terrasnek/oauth_clients.py
+-rw-r--r--   0 neil       (502) staff       (20)     2258 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/oauth_tokens.py
+-rw-r--r--   0 neil       (502) staff       (20)     3758 2021-12-23 02:35:15.000000 terrasnek-0.1.9/terrasnek/org_memberships.py
+-rw-r--r--   0 neil       (502) staff       (20)     2212 2022-02-04 18:33:17.000000 terrasnek-0.1.9/terrasnek/org_tags.py
+-rw-r--r--   0 neil       (502) staff       (20)     1433 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/org_tokens.py
+-rw-r--r--   0 neil       (502) staff       (20)     3764 2021-04-13 01:28:07.000000 terrasnek-0.1.9/terrasnek/orgs.py
+-rw-r--r--   0 neil       (502) staff       (20)     2289 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/plan_exports.py
+-rw-r--r--   0 neil       (502) staff       (20)     1850 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/plans.py
+-rw-r--r--   0 neil       (502) staff       (20)     4537 2021-12-23 02:35:07.000000 terrasnek-0.1.9/terrasnek/policies.py
+-rw-r--r--   0 neil       (502) staff       (20)     1865 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/policy_checks.py
+-rw-r--r--   0 neil       (502) staff       (20)     2636 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/policy_set_params.py
+-rw-r--r--   0 neil       (502) staff       (20)     7535 2022-01-02 05:11:43.000000 terrasnek-0.1.9/terrasnek/policy_sets.py
+-rw-r--r--   0 neil       (502) staff       (20)     9889 2022-02-09 18:53:58.000000 terrasnek-0.1.9/terrasnek/registry_modules.py
+-rw-r--r--   0 neil       (502) staff       (20)     3185 2022-02-09 18:53:58.000000 terrasnek-0.1.9/terrasnek/registry_providers.py
+-rw-r--r--   0 neil       (502) staff       (20)     6458 2022-02-09 18:53:58.000000 terrasnek-0.1.9/terrasnek/run_tasks.py
+-rw-r--r--   0 neil       (502) staff       (20)     3123 2021-12-23 02:35:15.000000 terrasnek-0.1.9/terrasnek/run_triggers.py
+-rw-r--r--   0 neil       (502) staff       (20)     4380 2021-12-23 02:35:07.000000 terrasnek-0.1.9/terrasnek/runs.py
+-rw-r--r--   0 neil       (502) staff       (20)     2583 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/ssh_keys.py
+-rw-r--r--   0 neil       (502) staff       (20)     1736 2022-01-02 05:11:43.000000 terrasnek-0.1.9/terrasnek/state_version_outputs.py
+-rw-r--r--   0 neil       (502) staff       (20)     3919 2022-01-02 05:11:43.000000 terrasnek-0.1.9/terrasnek/state_versions.py
+-rw-r--r--   0 neil       (502) staff       (20)     1469 2021-03-16 02:20:36.000000 terrasnek-0.1.9/terrasnek/subscriptions.py
+-rw-r--r--   0 neil       (502) staff       (20)     2788 2022-01-02 05:11:43.000000 terrasnek-0.1.9/terrasnek/team_access.py
+-rw-r--r--   0 neil       (502) staff       (20)     1818 2022-01-02 05:11:43.000000 terrasnek-0.1.9/terrasnek/team_memberships.py
+-rw-r--r--   0 neil       (502) staff       (20)     1498 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/team_tokens.py
+-rw-r--r--   0 neil       (502) staff       (20)     3320 2021-12-23 02:35:07.000000 terrasnek-0.1.9/terrasnek/teams.py
+-rw-r--r--   0 neil       (502) staff       (20)     2293 2021-12-02 10:03:35.000000 terrasnek-0.1.9/terrasnek/user_tokens.py
+-rw-r--r--   0 neil       (502) staff       (20)      954 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/users.py
+-rw-r--r--   0 neil       (502) staff       (20)     6551 2022-02-09 18:53:58.000000 terrasnek-0.1.9/terrasnek/var_sets.py
+-rw-r--r--   0 neil       (502) staff       (20)     2396 2021-12-02 10:03:35.000000 terrasnek-0.1.9/terrasnek/vars.py
+-rw-r--r--   0 neil       (502) staff       (20)     1543 2022-02-09 18:53:58.000000 terrasnek-0.1.9/terrasnek/vcs_events.py
+-rw-r--r--   0 neil       (502) staff       (20)     2504 2021-03-16 00:11:38.000000 terrasnek-0.1.9/terrasnek/workspace_vars.py
+-rw-r--r--   0 neil       (502) staff       (20)    11615 2022-01-28 19:37:12.000000 terrasnek-0.1.9/terrasnek/workspaces.py
+drwxr-xr-x   0 neil       (502) staff       (20)        0 2022-02-09 22:03:12.321777 terrasnek-0.1.9/terrasnek.egg-info/
+-rw-r--r--   0 neil       (502) staff       (20)     4832 2022-02-09 22:03:12.000000 terrasnek-0.1.9/terrasnek.egg-info/PKG-INFO
+-rw-r--r--   0 neil       (502) staff       (20)     2890 2022-02-09 22:03:12.000000 terrasnek-0.1.9/terrasnek.egg-info/SOURCES.txt
+-rw-r--r--   0 neil       (502) staff       (20)        1 2022-02-09 22:03:12.000000 terrasnek-0.1.9/terrasnek.egg-info/dependency_links.txt
+-rw-r--r--   0 neil       (502) staff       (20)       17 2022-02-09 22:03:12.000000 terrasnek-0.1.9/terrasnek.egg-info/requires.txt
+-rw-r--r--   0 neil       (502) staff       (20)       15 2022-02-09 22:03:12.000000 terrasnek-0.1.9/terrasnek.egg-info/top_level.txt
+drwxr-xr-x   0 neil       (502) staff       (20)        0 2022-02-09 22:03:12.339887 terrasnek-0.1.9/test/
+-rw-r--r--   0 neil       (502) staff       (20)      168 2020-06-18 02:40:50.000000 terrasnek-0.1.9/test/__init__.py
+-rw-r--r--   0 neil       (502) staff       (20)     2695 2021-12-02 10:03:35.000000 terrasnek-0.1.9/test/_constants.py
+-rw-r--r--   0 neil       (502) staff       (20)     3613 2021-09-18 00:22:50.000000 terrasnek-0.1.9/test/account_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     1738 2021-03-16 02:20:50.000000 terrasnek-0.1.9/test/admin_module_sharing_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     3623 2022-02-09 18:53:58.000000 terrasnek-0.1.9/test/admin_orgs_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     3533 2022-01-02 05:11:43.000000 terrasnek-0.1.9/test/admin_runs_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     5519 2021-09-22 02:02:40.000000 terrasnek-0.1.9/test/admin_settings_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     2941 2020-10-21 16:14:36.000000 terrasnek-0.1.9/test/admin_terraform_versions_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     2085 2021-09-22 02:02:40.000000 terrasnek-0.1.9/test/admin_users_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     2019 2022-01-02 05:11:43.000000 terrasnek-0.1.9/test/admin_workspaces_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     2503 2021-09-18 00:22:50.000000 terrasnek-0.1.9/test/agent_tokens_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     2232 2021-12-02 10:03:35.000000 terrasnek-0.1.9/test/agents_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     3742 2021-08-23 22:57:01.000000 terrasnek-0.1.9/test/applies_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     1628 2021-12-02 10:03:35.000000 terrasnek-0.1.9/test/audit_trails_test.py
+-rw-r--r--   0 neil       (502) staff       (20)    23739 2022-02-09 18:53:58.000000 terrasnek-0.1.9/test/base.py
+-rw-r--r--   0 neil       (502) staff       (20)     4701 2021-12-24 01:29:32.000000 terrasnek-0.1.9/test/config_versions_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     3725 2021-03-16 00:11:38.000000 terrasnek-0.1.9/test/cost_estimates_test.py
+-rw-r--r--   0 neil       (502) staff       (20)      704 2021-03-16 00:11:38.000000 terrasnek-0.1.9/test/feature_sets_test.py
+-rw-r--r--   0 neil       (502) staff       (20)      574 2022-02-09 01:09:45.000000 terrasnek-0.1.9/test/invoices_test.py
+-rw-r--r--   0 neil       (502) staff       (20)      592 2020-10-21 16:14:36.000000 terrasnek-0.1.9/test/ip_ranges_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     4403 2020-10-21 16:14:36.000000 terrasnek-0.1.9/test/notification_configs_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     2019 2020-10-21 16:14:36.000000 terrasnek-0.1.9/test/oauth_clients_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     2410 2021-09-18 00:22:50.000000 terrasnek-0.1.9/test/oauth_tokens_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     3441 2021-09-22 02:02:40.000000 terrasnek-0.1.9/test/org_memberships_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     2215 2022-02-09 18:53:58.000000 terrasnek-0.1.9/test/org_tags_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     1273 2020-10-21 16:14:36.000000 terrasnek-0.1.9/test/org_tokens_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     3251 2021-08-23 22:24:08.000000 terrasnek-0.1.9/test/orgs_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     4349 2021-03-16 00:11:38.000000 terrasnek-0.1.9/test/plan_exports_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     3787 2021-03-16 00:11:38.000000 terrasnek-0.1.9/test/plans_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     4143 2021-09-22 02:02:40.000000 terrasnek-0.1.9/test/policies_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     4119 2021-09-18 00:22:50.000000 terrasnek-0.1.9/test/policy_checks_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     3119 2020-10-21 16:14:36.000000 terrasnek-0.1.9/test/policy_set_params_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     7008 2021-09-22 02:02:40.000000 terrasnek-0.1.9/test/policy_sets_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     8875 2022-02-09 18:53:58.000000 terrasnek-0.1.9/test/registry_modules_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     2461 2021-12-02 10:03:35.000000 terrasnek-0.1.9/test/registry_providers_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     5136 2021-12-02 10:03:35.000000 terrasnek-0.1.9/test/run_tasks_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     3013 2021-08-21 01:24:43.000000 terrasnek-0.1.9/test/run_triggers_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     7928 2021-09-22 02:02:40.000000 terrasnek-0.1.9/test/runs_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     1714 2021-09-18 00:22:50.000000 terrasnek-0.1.9/test/ssh_keys_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     3643 2022-02-09 18:53:58.000000 terrasnek-0.1.9/test/state_version_outputs_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     4323 2022-01-02 05:11:43.000000 terrasnek-0.1.9/test/state_versions_test.py
+-rw-r--r--   0 neil       (502) staff       (20)      681 2021-03-16 00:11:38.000000 terrasnek-0.1.9/test/subscriptions_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     3470 2021-08-21 01:24:43.000000 terrasnek-0.1.9/test/team_access_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     2001 2021-09-18 00:22:50.000000 terrasnek-0.1.9/test/team_memberships_test.py
+-rw-r--r--   0 neil       (502) staff       (20)      978 2021-09-18 00:22:50.000000 terrasnek-0.1.9/test/team_tokens_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     2908 2021-04-13 15:57:35.000000 terrasnek-0.1.9/test/teams_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     1557 2020-10-21 16:14:36.000000 terrasnek-0.1.9/test/user_tokens_test.py
+-rw-r--r--   0 neil       (502) staff       (20)      625 2020-10-21 16:14:36.000000 terrasnek-0.1.9/test/users_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     6784 2021-12-02 10:03:35.000000 terrasnek-0.1.9/test/var_sets_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     2576 2021-12-02 10:03:35.000000 terrasnek-0.1.9/test/vars_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     1224 2022-02-09 18:53:58.000000 terrasnek-0.1.9/test/vcs_events_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     2728 2021-08-21 01:24:43.000000 terrasnek-0.1.9/test/workspace_vars_test.py
+-rw-r--r--   0 neil       (502) staff       (20)     9012 2022-02-09 18:53:58.000000 terrasnek-0.1.9/test/workspaces_test.py
```

### Comparing `terrasnek-0.1.8/PKG-INFO` & `terrasnek-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrasnek
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python client for the Terraform Cloud API
 Home-page: https://github.com/dahlke/terrasnek
 Author: Neil Dahlke
 Author-email: neil.dahlke+terrasnek@gmail.com
 License: UNKNOWN
 Description: # terrasnek
```

### Comparing `terrasnek-0.1.8/README.md` & `terrasnek-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/setup.py` & `terrasnek-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="terrasnek",
-    version="0.1.8",
+    version="0.1.9",
     author="Neil Dahlke",
     author_email="neil.dahlke+terrasnek@gmail.com",
     description="A Python client for the Terraform Cloud API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dahlke/terrasnek",
     packages=setuptools.find_packages(),
```

### Comparing `terrasnek-0.1.8/terrasnek/_constants.py` & `terrasnek-0.1.9/terrasnek/_constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 
 
 # Default Config Items
 TFC_SAAS_HOSTNAME = "app.terraform.io"
 TFC_SAAS_URL = "https://app.terraform.io"
 TERRASNEK_LOG_LEVEL = logging.CRITICAL
-TERRASNEK_VERSION = "0.1.8"
+TERRASNEK_VERSION = "0.1.9"
 MAX_PAGE_SIZE = 100
 
 # Common TFC API HTTP Codes
 HTTP_OK = 200
 HTTP_CREATED = 201
 HTTP_ACCEPTED = 202
 HTTP_NO_CONTENT = 204
@@ -54,7 +54,8 @@
     SENTINEL = "SENTINEL"
     STATE_STORAGE = "STATE_STORAGE"
     SSO = "SSO"
     TEAMS = "TEAMS"
     USER_LIMIT = "USER_LIMIT"
     USAGE_REPORTING = "USAGE_REPORTING"
     VCS_INTEGRATIONS = "VCS_INTEGRATIONS"
+    VIEWABLE_BILLING = "VIEWABLE_BILLING"
```

### Comparing `terrasnek-0.1.8/terrasnek/account.py` & `terrasnek-0.1.9/terrasnek/account.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/admin_module_sharing.py` & `terrasnek-0.1.9/terrasnek/admin_module_sharing.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/admin_orgs.py` & `terrasnek-0.1.9/terrasnek/admin_orgs.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/admin_runs.py` & `terrasnek-0.1.9/terrasnek/admin_runs.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/admin_settings.py` & `terrasnek-0.1.9/terrasnek/admin_settings.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/admin_terraform_versions.py` & `terrasnek-0.1.9/terrasnek/admin_terraform_versions.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/admin_users.py` & `terrasnek-0.1.9/terrasnek/admin_users.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/admin_workspaces.py` & `terrasnek-0.1.9/terrasnek/admin_workspaces.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/agent_tokens.py` & `terrasnek-0.1.9/terrasnek/agent_tokens.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/agents.py` & `terrasnek-0.1.9/terrasnek/agents.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/api.py` & `terrasnek-0.1.9/terrasnek/api.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/applies.py` & `terrasnek-0.1.9/terrasnek/applies.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/audit_trails.py` & `terrasnek-0.1.9/terrasnek/audit_trails.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/config_versions.py` & `terrasnek-0.1.9/terrasnek/config_versions.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/cost_estimates.py` & `terrasnek-0.1.9/terrasnek/cost_estimates.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/endpoint.py` & `terrasnek-0.1.9/terrasnek/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,43 +56,42 @@
     def terraform_enterprise_only(self):
         """
         Return ``True`` if this endpoint is only for Terraform Enterprise, else ``False``.
         """
         return False
 
     def _delete(self, url, data=None):
-        results = None
         req = requests.delete(\
             url, data=json.dumps(data), headers=self._headers, verify=self._verify)
 
-        if req.status_code == HTTP_NO_CONTENT:
-            pass
+        if req.status_code == HTTP_OK:
+            self._logger.debug(f"Terraform Cloud resource at URL [{url}] destroyed.")
+        elif req.status_code == HTTP_NO_CONTENT:
+            self._logger.debug(f"Terraform Cloud resource at URL [{url}] destroyed.")
         elif req.status_code == HTTP_NOT_FOUND:
             err = json.loads(req.content.decode("utf-8"))
             self._logger.debug(err)
             raise TFCHTTPNotFound(err)
         elif req.status_code == HTTP_FORBIDDEN:
             err = json.loads(req.content.decode("utf-8"))
             self._logger.debug(err)
             raise TFCHTTPForbidden(err)
         elif req.status_code == HTTP_API_REQUEST_RATE_LIMIT_REACHED:
             err = json.loads(req.content.decode("utf-8"))
             self._logger.debug(err)
             raise TFCHTTPAPIRequestRateLimit(err)
         else:
-            print("ERROR", req.status_code)
             try:
                 err = json.loads(req.content.decode("utf-8"))
             except json.decoder.JSONDecodeError:
                 err = req.content
             self._logger.debug(err)
             raise TFCHTTPUnclassified(err)
 
-        return results
-
+    # pylint: disable=too-many-statements,too-many-branches
     def _get(self, url, return_raw=None, allow_redirects=None, query=None, filters=None, \
         page=None, page_size=None, search=None, include=None, sort=None, \
         offset=None, limit=None, provider=None, namespace=None, verified=None, \
         since=None):
 
         results = None
 
@@ -123,28 +122,26 @@
 
         if page is not None:
             q_options.append(f"page[number]={page}")
 
         if page_size is not None:
             q_options.append(f"page[size]={page_size}")
 
-        if search is not None:
-            q_options.append(f"page[name]={page_size}")
-
         if sort is not None:
             q_options.append(f"sort={sort}")
 
         if search is not None:
             q_options.append(f"search[name]={search}")
 
         if since is not None:
             q_options.append(f"since={since}")
 
         # V1 Modules API options
-        # FIXME: This parameter needs to be deprecated and removed at some stage.
+        # NOTE: The `offset` parameter is not in use very much now, but remains for
+        # backwards compatibility.
         if offset is not None:
             q_options.append(f"offset={offset}")
 
         if limit is not None:
             q_options.append(f"limit={limit}")
 
         if provider is not None:
@@ -167,23 +164,22 @@
             results = json.loads(req.content)
             self._logger.debug(f"GET to {url} successful")
         elif req.status_code == HTTP_OK and return_raw:
             results = req.content
         elif req.status_code == HTTP_NO_CONTENT:
             results = req.headers
         elif req.history:
-            # TODO: use HTTP_MOVED_TEMPORARILY
-
             # NOTE: If we got redirected, run the get on the new URL, and fix the
-            # URL to match the private module registry URL schema.
+            # URL to match the private module registry URL schema. At some point
+            # in the future, this may need to use HTTP_MOVED_TEMPORARILY.
             url = req.url.replace("/v1/modules/", "/api/registry/v1/modules/")
             results = {"redirect-url": url}
         elif req.status_code == HTTP_MOVED_PERMANENTLY:
-            # FIXME: this isn't doing anything now (this was found in using run-tasks from event-hooks)
-            print("REDIRECTING ORIGINAL", req.url)
+            # TODO: this isn't doing anything now? (this was found in using run-tasks from event-hooks)
+            pass
         elif req.status_code == HTTP_UNAUTHORIZED:
             err = json.loads(req.content.decode("utf-8"))
             self._logger.debug(err)
             raise TFCHTTPUnauthorized(err)
         elif req.status_code == HTTP_NOT_FOUND:
             err = json.loads(req.content.decode("utf-8"))
             self._logger.debug(err)
@@ -197,14 +193,15 @@
                 err = json.loads(req.content.decode("utf-8"))
             except json.decoder.JSONDecodeError:
                 err = req.content
             self._logger.debug(err)
             raise TFCHTTPUnclassified(err)
 
         return results
+    # pylint: disable=too-many-statements,too-many-branches
 
     def _patch(self, url, data=None):
         results = None
 
         self._logger.debug(f"Trying HTTP PATCH to URL: {url} ...")
         req = requests.patch(url, data=json.dumps(data), headers=self._headers, verify=self._verify)
 
@@ -324,35 +321,19 @@
             payload = {}
 
         return self._post(url, data=payload)
 
     def _destroy(self, url, data=None):
         """
         Implementation of the common destroy resource pattern for the TFC API.
-        """
-        req = requests.delete(url, data=data, headers=self._headers, verify=self._verify)
 
-        valid_status_codes = [HTTP_OK, HTTP_NO_CONTENT]
-        if req.status_code in valid_status_codes:
-            self._logger.debug(f"Terraform Cloud resource at URL [{url}] destroyed.")
-        elif req.status_code == HTTP_API_REQUEST_RATE_LIMIT_REACHED:
-            err = json.loads(req.content.decode("utf-8"))
-            self._logger.debug(err)
-            raise TFCHTTPAPIRequestRateLimit(err)
-        elif req.status_code == HTTP_NOT_FOUND:
-            err = json.loads(req.content.decode("utf-8"))
-            self._logger.debug(err)
-            raise TFCHTTPNotFound(err)
-        else:
-            try:
-                err = json.loads(req.content.decode("utf-8"))
-            except json.decoder.JSONDecodeError:
-                err = req.content
-            self._logger.debug(err)
-            raise TFCHTTPUnclassified(err)
+        NOTE: This is basically an alias to the _delete method, but is more
+        along the verbiage used in the docs.
+        """
+        self._delete(url, data=data)
 
     def _list(self, url, query=None, filters=None, \
         page=None, page_size=None, search=None, include=None, sort=None, \
         offset=None, limit=None, provider=None, namespace=None, verified=None, \
         since=None):
         """
         Implementation of the common list resources pattern for the TFC API.
```

### Comparing `terrasnek-0.1.8/terrasnek/exceptions.py` & `terrasnek-0.1.9/terrasnek/exceptions.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/feature_sets.py` & `terrasnek-0.1.9/terrasnek/feature_sets.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/invoices.py` & `terrasnek-0.1.9/terrasnek/invoices.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Module for Terraform Cloud API Endpoint: Invoices.
 """
 
 from .endpoint import TFCEndpoint
+from ._constants import Entitlements
 
 class TFCInvoices(TFCEndpoint):
     """
     `Invoices API Docs \
         <https://www.terraform.io/docs/cloud/api/invoices.html>`_
     """
 
     def __init__(self, instance_url, org_name, headers, well_known_paths, verify, log_level):
         super().__init__(instance_url, org_name, headers, well_known_paths, verify, log_level)
         self._org_base_url = \
             f"{self._api_v2_base_url}/organizations/{org_name}/invoices"
 
     def required_entitlements(self):
-        # TODO: self serve billing?
-        return []
+        return [Entitlements.SELF_SERVE_BILLING]
 
     def terraform_cloud_only(self):
         return True
 
     def terraform_enterprise_only(self):
         return False
```

### Comparing `terrasnek-0.1.8/terrasnek/ip_ranges.py` & `terrasnek-0.1.9/terrasnek/ip_ranges.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/notification_configs.py` & `terrasnek-0.1.9/terrasnek/notification_configs.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/oauth_clients.py` & `terrasnek-0.1.9/terrasnek/oauth_clients.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/oauth_tokens.py` & `terrasnek-0.1.9/terrasnek/oauth_tokens.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/org_memberships.py` & `terrasnek-0.1.9/terrasnek/org_memberships.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/org_tags.py` & `terrasnek-0.1.9/terrasnek/org_tags.py`

 * *Files 21% similar despite different names*

```diff
@@ -55,24 +55,7 @@
             <https://www.terraform.io/docs/cloud/api/organization-tags.html#add-workspaces-to-a-tag>`_
 
         `Add Workspace to a Tag API Doc Sample Payload \
             <https://www.terraform.io/docs/cloud/api/organization-tags.html#sample-payload-1>`_
         """
         url = f"{self._tags_base_url}/{tag_id}/relationships/workspaces"
         return self._post(url, data=payload)
-
-    # NOTE: this endpoint has been temporarily removed
-    # (https://www.terraform.io/docs/cloud/api/organization-tags.html#remove-workspaces-from-a-tag)
-    """
-    def remove_workspaces_from_tag(self, tag_id, payload):
-        \"""
-        ``DELETE /tags/:tag_id/relationships/workspaces``
-
-        `Remove Workspaces from Tags API Doc Reference \
-            <https://www.terraform.io/docs/cloud/api/organization-tags.html#remove-workspaces-from-a-tag>`_
-
-        `Remove Workspaces from Tags API Doc Sample Payload \
-            <>`_
-        \"""
-        url = f"{self._tags_base_url}/{tag_id}/relationships/workspaces"
-        return self._destroy(url, data=payload)
-    """
```

### Comparing `terrasnek-0.1.8/terrasnek/org_tokens.py` & `terrasnek-0.1.9/terrasnek/org_tokens.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/orgs.py` & `terrasnek-0.1.9/terrasnek/orgs.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/plan_exports.py` & `terrasnek-0.1.9/terrasnek/plan_exports.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/plans.py` & `terrasnek-0.1.9/terrasnek/plans.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/policies.py` & `terrasnek-0.1.9/terrasnek/policies.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/policy_checks.py` & `terrasnek-0.1.9/terrasnek/policy_checks.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/policy_set_params.py` & `terrasnek-0.1.9/terrasnek/policy_set_params.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/policy_sets.py` & `terrasnek-0.1.9/terrasnek/policy_sets.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/registry_modules.py` & `terrasnek-0.1.9/terrasnek/registry_modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     def search(self, query, offset=None, limit=None, provider=None, verified=None):
         """
         ``GET <base_url>/search``
 
         `Registry Modules Search API Doc Reference \
             <https://www.terraform.io/docs/registry/api.html#search-modules>`_
         """
-        # FIXME: the slash here is behaving differently from TFE to TFC
         url = f"{self._modules_v1_base_url}/search"
         return self._list(url, \
             query=query, offset=offset, limit=limit, provider=provider,\
             verified=verified)
 
     def show(self, module_name, provider):
         """
```

### Comparing `terrasnek-0.1.8/terrasnek/registry_providers.py` & `terrasnek-0.1.9/terrasnek/registry_providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,15 @@
         super().__init__(instance_url, org_name, headers, well_known_paths, verify, log_level)
         self._org_providers_base_url = f"{self._api_v2_base_url}/organizations/{self._org_name}/registry-providers"
 
     def required_entitlements(self):
         return []
 
     def terraform_cloud_only(self):
-        # TODO: remove this once it goes to TFE GA
-        return True
+        return False
 
     def terraform_enterprise_only(self):
         return False
 
     def create(self, payload):
         """
         ``POST /organizations/:organization_name/registry-providers``
```

### Comparing `terrasnek-0.1.8/terrasnek/run_tasks.py` & `terrasnek-0.1.9/terrasnek/run_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self._tasks_base_url = f"{self._api_v2_base_url}/tasks"
         self._ws_api_v2_base_url = f"{self._api_v2_base_url}/workspaces"
 
     def required_entitlements(self):
         return []
 
     def terraform_cloud_only(self):
-        # TODO: remove this once it goes to TFE GA
+        # FIXME: remove this once it goes to TFE GA
         return True
 
     def terraform_enterprise_only(self):
         return False
 
     def create(self, payload):
         """
```

### Comparing `terrasnek-0.1.8/terrasnek/run_triggers.py` & `terrasnek-0.1.9/terrasnek/run_triggers.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/runs.py` & `terrasnek-0.1.9/terrasnek/runs.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/ssh_keys.py` & `terrasnek-0.1.9/terrasnek/ssh_keys.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/state_version_outputs.py` & `terrasnek-0.1.9/terrasnek/state_version_outputs.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/state_versions.py` & `terrasnek-0.1.9/terrasnek/state_versions.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/subscriptions.py` & `terrasnek-0.1.9/terrasnek/subscriptions.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/team_access.py` & `terrasnek-0.1.9/terrasnek/team_access.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/team_memberships.py` & `terrasnek-0.1.9/terrasnek/team_memberships.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/team_tokens.py` & `terrasnek-0.1.9/terrasnek/team_tokens.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/teams.py` & `terrasnek-0.1.9/terrasnek/teams.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/user_tokens.py` & `terrasnek-0.1.9/terrasnek/user_tokens.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/users.py` & `terrasnek-0.1.9/terrasnek/users.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/var_sets.py` & `terrasnek-0.1.9/terrasnek/var_sets.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,21 @@
     def __init__(self, instance_url, org_name, headers, well_known_paths, verify, log_level):
         super().__init__(instance_url, org_name, headers, well_known_paths, verify, log_level)
         self._org_varsets_base_url = f"{self._api_v2_base_url}/organizations/{self._org_name}/varsets"
         self._endpoint_base_url = f"{self._api_v2_base_url}/varsets"
         self._ws_api_v2_base_url = f"{self._api_v2_base_url}/workspaces"
 
     def required_entitlements(self):
-        # TODO
         return []
 
     def terraform_cloud_only(self):
         # TODO: change when it gets released to TFE
         return True
 
     def terraform_enterprise_only(self):
-        # TODO: change when it gets released to TFE
         return False
 
     def create(self, payload):
         """
         ``POST organizations/:organization_name/varsets``
 
         `Variable Sets Create API Doc Reference \
```

### Comparing `terrasnek-0.1.8/terrasnek/vars.py` & `terrasnek-0.1.9/terrasnek/vars.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/vcs_events.py` & `terrasnek-0.1.9/terrasnek/vcs_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self._vcs_events_api_v2_base_url = \
             f"{self._api_v2_base_url}/organizations/{org_name}/vcs-events"
 
     def required_entitlements(self):
         return []
 
     def terraform_cloud_only(self):
-        # TODO: change this once it is released in TFE.
+        # FIXME: change this once it is released in TFE.
         return True
 
     def terraform_enterprise_only(self):
         return False
 
     def list(self, page=None, page_size=None, include=None, filters=None):
         """
```

### Comparing `terrasnek-0.1.8/terrasnek/workspace_vars.py` & `terrasnek-0.1.9/terrasnek/workspace_vars.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/terrasnek/workspaces.py` & `terrasnek-0.1.9/terrasnek/workspaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,26 +72,26 @@
 
         `Lock Sample Payload \
             <https://www.terraform.io/docs/cloud/api/workspaces.html#sample-payload-2>`_
         """
         url = f"{self._ws_api_v2_base_url}/{workspace_id}/actions/lock"
         return self._post(url, data=payload)
 
-    def list(self, page=None, page_size=None, include=None):
+    def list(self, page=None, page_size=None, include=None, search=None):
         """
         ``GET /organizations/:organization_name/workspaces``
 
         `Workspaces List API Doc Reference \
             <https://www.terraform.io/docs/cloud/api/workspaces.html#list-workspaces>`_
 
         `Query Parameter(s) Details \
             <https://www.terraform.io/docs/cloud/api/workspaces.html#query-parameters>`__
         """
         return self._list(self._org_api_v2_base_url, \
-            page=page, page_size=page_size, include=include)
+            page=page, page_size=page_size, include=include, search=search)
 
     def list_all(self, include=None):
         """
         This function does not correlate to an endpoint in the TFC API Docs specifically,
         but rather is a helper function to wrap the `list` endpoint, which enumerates out
         every page so users do not have to implement the paging logic every time they just
         want to list every workspace in an organization.
```

### Comparing `terrasnek-0.1.8/terrasnek.egg-info/PKG-INFO` & `terrasnek-0.1.9/terrasnek.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrasnek
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python client for the Terraform Cloud API
 Home-page: https://github.com/dahlke/terrasnek
 Author: Neil Dahlke
 Author-email: neil.dahlke+terrasnek@gmail.com
 License: UNKNOWN
 Description: # terrasnek
```

### Comparing `terrasnek-0.1.8/terrasnek.egg-info/SOURCES.txt` & `terrasnek-0.1.9/terrasnek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/_constants.py` & `terrasnek-0.1.9/test/_constants.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/account_test.py` & `terrasnek-0.1.9/test/account_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/admin_module_sharing_test.py` & `terrasnek-0.1.9/test/admin_module_sharing_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/admin_orgs_test.py` & `terrasnek-0.1.9/test/admin_orgs_test.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Module for testing the Terraform Cloud API Endpoint: Admin Orgs.
 """
 
-from .base import TestTFCBaseTestCase
 from terrasnek.exceptions import TFCHTTPNotFound
+from .base import TestTFCBaseTestCase
 from ._constants import PAGE_START, PAGE_SIZE
 
 
 class TestTFCAdminOrgs(TestTFCBaseTestCase):
     """
     Class for testing the Terraform Cloud API Endpoint: Admin Orgs.
     """
```

### Comparing `terrasnek-0.1.8/test/admin_runs_test.py` & `terrasnek-0.1.9/test/admin_runs_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/admin_settings_test.py` & `terrasnek-0.1.9/test/admin_settings_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/admin_terraform_versions_test.py` & `terrasnek-0.1.9/test/admin_terraform_versions_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/admin_users_test.py` & `terrasnek-0.1.9/test/admin_users_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/admin_workspaces_test.py` & `terrasnek-0.1.9/test/admin_workspaces_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/agent_tokens_test.py` & `terrasnek-0.1.9/test/agent_tokens_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/agents_test.py` & `terrasnek-0.1.9/test/agents_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/applies_test.py` & `terrasnek-0.1.9/test/applies_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/audit_trails_test.py` & `terrasnek-0.1.9/test/audit_trails_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/base.py` & `terrasnek-0.1.9/test/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
         cls._logger.debug(f"Purging test org ({cls._test_org_name}) of agent pools...")
         agent_pools = cls._api.agents.list_pools()["data"]
         for agent_pool in agent_pools:
             cls._api.agents.destroy_pool(agent_pool["id"])
         cls._logger.debug(f"Agent pools purged from test org ({cls._test_org_name}).")
 
-        # FIXME: move these once they both go GA or make the tests smarter
+        # FIXME: move these once they both go GA
         if cls._api.is_terraform_cloud():
             cls._logger.debug(f"Purging test org ({cls._test_org_name}) of run tasks...")
             run_tasks = cls._api.run_tasks.list_all()["data"]
             for run_task in run_tasks:
                 cls._api.run_tasks.destroy(run_task["id"])
             cls._logger.debug(f"Run tasks purged from test org ({cls._test_org_name}).")
```

### Comparing `terrasnek-0.1.8/test/config_versions_test.py` & `terrasnek-0.1.9/test/config_versions_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/cost_estimates_test.py` & `terrasnek-0.1.9/test/cost_estimates_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/feature_sets_test.py` & `terrasnek-0.1.9/test/feature_sets_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/invoices_test.py` & `terrasnek-0.1.9/test/invoices_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/ip_ranges_test.py` & `terrasnek-0.1.9/test/ip_ranges_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/notification_configs_test.py` & `terrasnek-0.1.9/test/notification_configs_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/oauth_clients_test.py` & `terrasnek-0.1.9/test/oauth_clients_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/oauth_tokens_test.py` & `terrasnek-0.1.9/test/oauth_tokens_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/org_memberships_test.py` & `terrasnek-0.1.9/test/org_memberships_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/org_tokens_test.py` & `terrasnek-0.1.9/test/org_tokens_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/orgs_test.py` & `terrasnek-0.1.9/test/orgs_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/plan_exports_test.py` & `terrasnek-0.1.9/test/plan_exports_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/plans_test.py` & `terrasnek-0.1.9/test/plans_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/policies_test.py` & `terrasnek-0.1.9/test/policies_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/policy_checks_test.py` & `terrasnek-0.1.9/test/policy_checks_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/policy_set_params_test.py` & `terrasnek-0.1.9/test/policy_set_params_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/policy_sets_test.py` & `terrasnek-0.1.9/test/policy_sets_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/registry_modules_test.py` & `terrasnek-0.1.9/test/registry_modules_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,14 @@
         latest_all_providers = listed_latest_version_all_providers["modules"][0]
         latest_provider_versions = \
             [provider_version["version"] for provider_version in latest_all_providers["versions"]]
         self.assertIn(latest_listed_version, latest_provider_versions)
 
         # List the latest version for a specific provider, compare to the
         # published module version
-        # TODO: this is the test that fails the most often
         listed_latest_version_specific_provider = \
             self._api.registry_modules.list_versions(\
                 published_module_name, TFE_MODULE_PROVIDER_TYPE)
         latest_specific_provider = listed_latest_version_specific_provider["modules"][0]
         latest_specific_versions = \
             [provider_version["version"] for \
                 provider_version in latest_specific_provider["versions"]]
```

### Comparing `terrasnek-0.1.8/test/registry_providers_test.py` & `terrasnek-0.1.9/test/registry_providers_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/run_tasks_test.py` & `terrasnek-0.1.9/test/run_tasks_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/run_triggers_test.py` & `terrasnek-0.1.9/test/run_triggers_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/runs_test.py` & `terrasnek-0.1.9/test/runs_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/ssh_keys_test.py` & `terrasnek-0.1.9/test/ssh_keys_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/state_version_outputs_test.py` & `terrasnek-0.1.9/test/state_version_outputs_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def test_state_version_outputs(self):
         """
         Test the State Version Outputs API endpoints.
         """
 
         # Create a sample state version
         self._api.workspaces.lock(self._ws_id, {"reason": "Unit testing."})
-        self._api.state_versions.create(self._ws_id, self._get_state_version_create_payload())["data"]
+        _ = self._api.state_versions.create(self._ws_id, self._get_state_version_create_payload())["data"]
         self._api.workspaces.unlock(self._ws_id)
 
         # Get the state version ID, using list instead of extracting from the create
         # response to make the test shorter (less calls).
         test_filters = [
             {
                 "keys": ["workspace", "name"],
```

### Comparing `terrasnek-0.1.8/test/state_versions_test.py` & `terrasnek-0.1.9/test/state_versions_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/subscriptions_test.py` & `terrasnek-0.1.9/test/subscriptions_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/team_access_test.py` & `terrasnek-0.1.9/test/team_access_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/team_memberships_test.py` & `terrasnek-0.1.9/test/team_memberships_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/team_tokens_test.py` & `terrasnek-0.1.9/test/team_tokens_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/teams_test.py` & `terrasnek-0.1.9/test/teams_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/user_tokens_test.py` & `terrasnek-0.1.9/test/user_tokens_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/users_test.py` & `terrasnek-0.1.9/test/users_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/var_sets_test.py` & `terrasnek-0.1.9/test/var_sets_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/vars_test.py` & `terrasnek-0.1.9/test/vars_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/vcs_events_test.py` & `terrasnek-0.1.9/test/vcs_events_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,10 +29,10 @@
         # NOTE: Currently, this feature is in beta, and only supports GitLab.
         # Since all of the testing is done with GitHub, this function is
         # provided, but you can see below that the test is not yet very good.
 
         # List the VCS events
         start_page = 0
         page_size = 50
-        # TODO: test filter / include parameters GitHub is supported.
+        # FIXME: Test filter / include parameters GitHub is supported.
         vcs_events = self._api.vcs_events.list(page=start_page, page_size=page_size)["data"]
         self.assertEqual(len(vcs_events), 0)
```

### Comparing `terrasnek-0.1.8/test/workspace_vars_test.py` & `terrasnek-0.1.9/test/workspace_vars_test.py`

 * *Files identical despite different names*

### Comparing `terrasnek-0.1.8/test/workspaces_test.py` & `terrasnek-0.1.9/test/workspaces_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,24 @@
         Test the Workspaces API endpoints.
         """
 
         # Get the number of existing workspaces, then create one and compare them
         workspace = self._api.workspaces.create(
             self._get_ws_no_vcs_create_payload())["data"]
         ws_id = workspace["id"]
+        ws_name = workspace["attributes"]["name"]
 
         # List the workspaces, confirm we have the included values
         listed_ws_raw = self._api.workspaces.list(page=PAGE_START, page_size=PAGE_SIZE, include=["organization"])
         self.assertIn("included", listed_ws_raw)
 
+        # Test the search parameter on listing workspaces
+        search_listed_ws = self._api.workspaces.list(page=PAGE_START, page_size=PAGE_SIZE, search=ws_name)["data"]
+        self.assertTrue(len(search_listed_ws), 1)
+
         listed_ws = listed_ws_raw["data"]
         found_ws = False
         for workspace in listed_ws:
             if workspace["id"] == ws_id:
                 found_ws = True
                 break
         self.assertTrue(found_ws)
@@ -112,17 +117,17 @@
                 "attributes": {
                     "id": None
                 },
                 "type": "workspaces"
             }
         }
         self._api.workspaces.unassign_ssh_key(ws_id, unassign_payload)
-        # TODO: include test when include works?
-        ws_shown_by_id = self._api.workspaces.show(workspace_id=ws_id)["data"]
-        self.assertNotIn("ssh-key", ws_shown_by_id["relationships"])
+        raw_ws_shown_by_id = self._api.workspaces.show(workspace_id=ws_id, include=["organization", "readme"])
+        self.assertIn("included", raw_ws_shown_by_id)
+        self.assertNotIn("ssh-key", raw_ws_shown_by_id["data"]["relationships"])
 
         # Add tags to the workspace
         ws_add_tags_payload = {
             "data": [
                 {
                     "type": "tags",
                     "attributes": {
```

